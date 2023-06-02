# Comparing `tmp/frouros-0.3.0.tar.gz` & `tmp/frouros-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frouros-0.3.0.tar", last modified: Wed May 31 15:32:53 2023, max compression
+gzip compressed data, was "frouros-0.3.1.tar", last modified: Fri Jun  2 13:40:56 2023, max compression
```

## Comparing `frouros-0.3.0.tar` & `frouros-0.3.1.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.939460 frouros-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-05-31 15:32:40.000000 frouros-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-31 15:32:40.000000 frouros-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    21352 2023-05-31 15:32:53.939460 frouros-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    19989 2023-05-31 15:32:40.000000 frouros-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.931460 frouros-0.3.0/frouros/
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.931460 frouros-0.3.0/frouros/callbacks/
--rw-r--r--   0 runner    (1001) docker     (122)      329 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2136 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/callbacks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.931460 frouros-0.3.0/frouros/callbacks/batch/
--rw-r--r--   0 runner    (1001) docker     (122)      211 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/callbacks/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      709 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/callbacks/batch/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     5617 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/callbacks/batch/permutation_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2071 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/callbacks/batch/reset_drift.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.935460 frouros-0.3.0/frouros/callbacks/streaming/
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/callbacks/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      805 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/callbacks/streaming/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2712 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/callbacks/streaming/history.py
--rw-r--r--   0 runner    (1001) docker     (122)     6385 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/callbacks/streaming/msprt.py
--rw-r--r--   0 runner    (1001) docker     (122)     2142 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/callbacks/streaming/warning_samples.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.935460 frouros-0.3.0/frouros/common/
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      240 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/common/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.935460 frouros-0.3.0/frouros/datasets/
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5680 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/datasets/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      454 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/datasets/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1189 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/datasets/real.py
--rw-r--r--   0 runner    (1001) docker     (122)     3008 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/datasets/synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.935460 frouros-0.3.0/frouros/detectors/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2255 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.935460 frouros-0.3.0/frouros/detectors/concept_drift/
--rw-r--r--   0 runner    (1001) docker     (122)      887 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/concept_drift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6144 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/concept_drift/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      282 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/concept_drift/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.935460 frouros-0.3.0/frouros/detectors/concept_drift/streaming/
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/concept_drift/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      567 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/concept_drift/streaming/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.935460 frouros-0.3.0/frouros/detectors/concept_drift/streaming/cusum_based/
--rw-r--r--   0 runner    (1001) docker     (122)      414 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/concept_drift/streaming/cusum_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5351 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/concept_drift/streaming/cusum_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1567 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/concept_drift/streaming/cusum_based/cusum.py
--rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/concept_drift/streaming/cusum_based/geometric_moving_average.py
--rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/concept_drift/streaming/cusum_based/page_hinkley.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.935460 frouros-0.3.0/frouros/detectors/concept_drift/streaming/statistical_process_control/
--rw-r--r--   0 runner    (1001) docker     (122)      479 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/concept_drift/streaming/statistical_process_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10783 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/concept_drift/streaming/statistical_process_control/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2752 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/concept_drift/streaming/statistical_process_control/ddm.py
--rw-r--r--   0 runner    (1001) docker     (122)     4810 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/concept_drift/streaming/statistical_process_control/ecdd.py
--rw-r--r--   0 runner    (1001) docker     (122)    12416 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/concept_drift/streaming/statistical_process_control/eddm.py
--rw-r--r--   0 runner    (1001) docker     (122)    23079 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/concept_drift/streaming/statistical_process_control/hddm.py
--rw-r--r--   0 runner    (1001) docker     (122)     9657 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/concept_drift/streaming/statistical_process_control/rddm.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.935460 frouros-0.3.0/frouros/detectors/concept_drift/streaming/window_based/
--rw-r--r--   0 runner    (1001) docker     (122)      285 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/concept_drift/streaming/window_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19323 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/concept_drift/streaming/window_based/adwin.py
--rw-r--r--   0 runner    (1001) docker     (122)      579 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/concept_drift/streaming/window_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     5958 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/concept_drift/streaming/window_based/kswin.py
--rw-r--r--   0 runner    (1001) docker     (122)     7877 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/concept_drift/streaming/window_based/stepd.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.935460 frouros-0.3.0/frouros/detectors/data_drift/
--rw-r--r--   0 runner    (1001) docker     (122)      591 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6439 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.935460 frouros-0.3.0/frouros/detectors/data_drift/batch/
--rw-r--r--   0 runner    (1001) docker     (122)      515 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3429 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/batch/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.939460 frouros-0.3.0/frouros/detectors/data_drift/batch/distance_based/
--rw-r--r--   0 runner    (1001) docker     (122)      486 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/batch/distance_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8762 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/batch/distance_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1887 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py
--rw-r--r--   0 runner    (1001) docker     (122)     1775 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/batch/distance_based/emd.py
--rw-r--r--   0 runner    (1001) docker     (122)     2133 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py
--rw-r--r--   0 runner    (1001) docker     (122)     2284 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py
--rw-r--r--   0 runner    (1001) docker     (122)     2131 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/batch/distance_based/js.py
--rw-r--r--   0 runner    (1001) docker     (122)     2143 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/batch/distance_based/kl.py
--rw-r--r--   0 runner    (1001) docker     (122)     8142 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/batch/distance_based/mmd.py
--rw-r--r--   0 runner    (1001) docker     (122)     2347 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/batch/distance_based/psi.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.939460 frouros-0.3.0/frouros/detectors/data_drift/batch/statistical_test/
--rw-r--r--   0 runner    (1001) docker     (122)      271 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/batch/statistical_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1111 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/batch/statistical_test/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2493 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/batch/statistical_test/chisquare.py
--rw-r--r--   0 runner    (1001) docker     (122)     2424 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/batch/statistical_test/cvm.py
--rw-r--r--   0 runner    (1001) docker     (122)     1560 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/batch/statistical_test/ks.py
--rw-r--r--   0 runner    (1001) docker     (122)     1477 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      428 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.939460 frouros-0.3.0/frouros/detectors/data_drift/streaming/
--rw-r--r--   0 runner    (1001) docker     (122)      183 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2645 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/streaming/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.939460 frouros-0.3.0/frouros/detectors/data_drift/streaming/distance_based/
--rw-r--r--   0 runner    (1001) docker     (122)      115 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/streaming/distance_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2019 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/streaming/distance_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     3114 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/streaming/distance_based/mmd.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.939460 frouros-0.3.0/frouros/detectors/data_drift/streaming/statistical_test/
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/streaming/statistical_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2288 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/streaming/statistical_test/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     7320 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/streaming/statistical_test/ks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.939460 frouros-0.3.0/frouros/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     3758 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/metrics/prequential_error.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.939460 frouros-0.3.0/frouros/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12327 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.939460 frouros-0.3.0/frouros/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9103 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/tests/integration/test_callback.py
--rw-r--r--   0 runner    (1001) docker     (122)     5330 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/tests/integration/test_concept_drift.py
--rw-r--r--   0 runner    (1001) docker     (122)    14909 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/tests/integration/test_data_drift.py
--rw-r--r--   0 runner    (1001) docker     (122)     1351 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/tests/integration/test_real.py
--rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/tests/integration/test_synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.939460 frouros-0.3.0/frouros/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.939460 frouros-0.3.0/frouros/tests/unit/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/tests/unit/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/tests/unit/metrics/test_prequential_error.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.939460 frouros-0.3.0/frouros/utils/
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    21163 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/utils/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (122)      695 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)      140 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (122)     7742 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/utils/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.931460 frouros-0.3.0/frouros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    21352 2023-05-31 15:32:53.000000 frouros-0.3.0/frouros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4713 2023-05-31 15:32:53.000000 frouros-0.3.0/frouros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-31 15:32:53.000000 frouros-0.3.0/frouros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-31 15:32:53.000000 frouros-0.3.0/frouros.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      350 2023-05-31 15:32:53.000000 frouros-0.3.0/frouros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-05-31 15:32:53.000000 frouros-0.3.0/frouros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1894 2023-05-31 15:32:40.000000 frouros-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-31 15:32:53.939460 frouros-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1854 2023-05-31 15:32:40.000000 frouros-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.146494 frouros-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-06-02 13:40:40.000000 frouros-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-02 13:40:40.000000 frouros-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    21654 2023-06-02 13:40:56.146494 frouros-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    20033 2023-06-02 13:40:40.000000 frouros-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.138495 frouros-0.3.1/frouros/
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.138495 frouros-0.3.1/frouros/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (122)      286 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2139 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/callbacks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.138495 frouros-0.3.1/frouros/callbacks/batch/
+-rw-r--r--   0 runner    (1001) docker     (122)      211 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/callbacks/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      725 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/callbacks/batch/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5625 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/callbacks/batch/permutation_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2079 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/callbacks/batch/reset_drift.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.138495 frouros-0.3.1/frouros/callbacks/streaming/
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/callbacks/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      820 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/callbacks/streaming/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2728 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/callbacks/streaming/history.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6393 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/callbacks/streaming/msprt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2150 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/callbacks/streaming/warning_samples.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.138495 frouros-0.3.1/frouros/common/
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      240 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/common/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.138495 frouros-0.3.1/frouros/datasets/
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5703 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/datasets/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      466 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/datasets/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1214 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/datasets/real.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3041 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/datasets/synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.138495 frouros-0.3.1/frouros/detectors/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2331 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.138495 frouros-0.3.1/frouros/detectors/concept_drift/
+-rw-r--r--   0 runner    (1001) docker     (122)      887 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/concept_drift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6194 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/concept_drift/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      285 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/concept_drift/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.138495 frouros-0.3.1/frouros/detectors/concept_drift/streaming/
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/concept_drift/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/concept_drift/streaming/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.142495 frouros-0.3.1/frouros/detectors/concept_drift/streaming/cusum_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      414 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/concept_drift/streaming/cusum_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5372 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/concept_drift/streaming/cusum_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1567 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/concept_drift/streaming/cusum_based/cusum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/concept_drift/streaming/cusum_based/geometric_moving_average.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/concept_drift/streaming/cusum_based/page_hinkley.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.142495 frouros-0.3.1/frouros/detectors/concept_drift/streaming/statistical_process_control/
+-rw-r--r--   0 runner    (1001) docker     (122)      479 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/concept_drift/streaming/statistical_process_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10816 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/concept_drift/streaming/statistical_process_control/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2752 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/concept_drift/streaming/statistical_process_control/ddm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4831 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/concept_drift/streaming/statistical_process_control/ecdd.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12437 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/concept_drift/streaming/statistical_process_control/eddm.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23112 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/concept_drift/streaming/statistical_process_control/hddm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9678 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/concept_drift/streaming/statistical_process_control/rddm.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.142495 frouros-0.3.1/frouros/detectors/concept_drift/streaming/window_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      285 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/concept_drift/streaming/window_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19342 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/concept_drift/streaming/window_based/adwin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      581 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/concept_drift/streaming/window_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5977 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/concept_drift/streaming/window_based/kswin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7896 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/concept_drift/streaming/window_based/stepd.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.142495 frouros-0.3.1/frouros/detectors/data_drift/
+-rw-r--r--   0 runner    (1001) docker     (122)      591 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6460 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.142495 frouros-0.3.1/frouros/detectors/data_drift/batch/
+-rw-r--r--   0 runner    (1001) docker     (122)      515 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3450 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/batch/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.142495 frouros-0.3.1/frouros/detectors/data_drift/batch/distance_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      486 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/batch/distance_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8810 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/batch/distance_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1796 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/batch/distance_based/emd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2154 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2305 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2156 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/batch/distance_based/js.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2164 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/batch/distance_based/kl.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8167 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/batch/distance_based/mmd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2368 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/batch/distance_based/psi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.142495 frouros-0.3.1/frouros/detectors/data_drift/batch/statistical_test/
+-rw-r--r--   0 runner    (1001) docker     (122)      271 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/batch/statistical_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1110 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/batch/statistical_test/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2514 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/batch/statistical_test/chisquare.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2445 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/batch/statistical_test/cvm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/batch/statistical_test/ks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1498 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      428 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.142495 frouros-0.3.1/frouros/detectors/data_drift/streaming/
+-rw-r--r--   0 runner    (1001) docker     (122)      183 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2666 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/streaming/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.142495 frouros-0.3.1/frouros/detectors/data_drift/streaming/distance_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      115 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/streaming/distance_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2019 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/streaming/distance_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3135 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/streaming/distance_based/mmd.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.142495 frouros-0.3.1/frouros/detectors/data_drift/streaming/statistical_test/
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/streaming/statistical_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2288 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/streaming/statistical_test/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7341 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/streaming/statistical_test/ks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.146494 frouros-0.3.1/frouros/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3758 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/metrics/prequential_error.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.146494 frouros-0.3.1/frouros/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12327 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.146494 frouros-0.3.1/frouros/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9103 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/tests/integration/test_callback.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5329 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/tests/integration/test_concept_drift.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14909 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/tests/integration/test_data_drift.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1351 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/tests/integration/test_real.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/tests/integration/test_synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.146494 frouros-0.3.1/frouros/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.146494 frouros-0.3.1/frouros/tests/unit/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/tests/unit/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/tests/unit/metrics/test_prequential_error.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.146494 frouros-0.3.1/frouros/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21163 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/utils/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (122)      695 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)      140 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7750 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/utils/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.138495 frouros-0.3.1/frouros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    21654 2023-06-02 13:40:55.000000 frouros-0.3.1/frouros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4713 2023-06-02 13:40:56.000000 frouros-0.3.1/frouros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-02 13:40:55.000000 frouros-0.3.1/frouros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-02 13:40:55.000000 frouros-0.3.1/frouros.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      350 2023-06-02 13:40:56.000000 frouros-0.3.1/frouros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-06-02 13:40:56.000000 frouros-0.3.1/frouros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-06-02 13:40:40.000000 frouros-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-02 13:40:56.146494 frouros-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1854 2023-06-02 13:40:40.000000 frouros-0.3.1/setup.py
```

### Comparing `frouros-0.3.0/LICENSE` & `frouros-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `frouros-0.3.0/PKG-INFO` & `frouros-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 Metadata-Version: 2.1
 Name: frouros
-Version: 0.3.0
-Summary: A Python library for drift detection in Machine Learning problems
+Version: 0.3.1
+Summary: An open source Python library for drift detection in machine Learning systems
 Home-page: https://github.com/IFCA/frouros
 Author: Jaime Céspedes Sisniega
 Author-email: cespedes@ifca.unican.es
 Maintainer: Jaime Céspedes Sisniega
 Maintainer-email: cespedes@ifca.unican.es
 License: BSD-3-Clause
 Project-URL: homepage, https://frouros.readthedocs.io
 Project-URL: repository, https://github.com/IFCA/frouros
 Project-URL: documentation, https://frouros.readthedocs.io
 Project-URL: download, https://pypi.org/project/frouros/
-Keywords: drift-detection,concept-drift,data-drift,machine-learning,data-science
+Keywords: drift-detection,concept-drift,data-drift,machine-learning,data-science,machine-learning-operations,machine-learning-systems
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8,<3.12
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: notebooks
 License-File: LICENSE
 
 <p align="center">
-  <img height="115px" src="images/logo.png" alt="frouros_logo">
+  <img height="115px" src="https://raw.githubusercontent.com/IFCA/frouros/main/images/logo.png" alt="logo">
 </p>
 
 ---
 
 <p align="center">
   <!-- CI -->
   <a href="https://github.com/IFCA/frouros/actions/workflows/ci.yml">
```

#### html2text {}

```diff
@@ -1,26 +1,30 @@
-Metadata-Version: 2.1 Name: frouros Version: 0.3.0 Summary: A Python library
-for drift detection in Machine Learning problems Home-page: https://github.com/
-IFCA/frouros Author: Jaime CÃ©spedes Sisniega Author-email:
+Metadata-Version: 2.1 Name: frouros Version: 0.3.1 Summary: An open source
+Python library for drift detection in machine Learning systems Home-page:
+https://github.com/IFCA/frouros Author: Jaime CÃ©spedes Sisniega Author-email:
 cespedes@ifca.unican.es Maintainer: Jaime CÃ©spedes Sisniega Maintainer-email:
 cespedes@ifca.unican.es License: BSD-3-Clause Project-URL: homepage, https://
 frouros.readthedocs.io Project-URL: repository, https://github.com/IFCA/frouros
 Project-URL: documentation, https://frouros.readthedocs.io Project-URL:
 download, https://pypi.org/project/frouros/ Keywords: drift-detection,concept-
-drift,data-drift,machine-learning,data-science Platform: UNKNOWN Classifier:
-Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
-Science/Research Classifier: Topic :: Scientific/Engineering Classifier: Topic
-:: Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
+drift,data-drift,machine-learning,data-science,machine-learning-
+operations,machine-learning-systems Platform: UNKNOWN Classifier: Development
+Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
+Approved :: BSD License Classifier: Topic :: Scientific/Engineering Classifier:
+Topic :: Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
 Scientific/Engineering :: Mathematics Classifier: Topic :: Software Development
-:: Libraries :: Python Modules Classifier: Programming Language :: Python ::
-3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8,<3.12 Description-Content-Type: text/markdown Provides-
-Extra: docs Provides-Extra: notebooks License-File: LICENSE
-                                [frouros_logo]
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3 :: Only Requires-Python: >=3.8,<3.12 Description-
+Content-Type: text/markdown Provides-Extra: docs Provides-Extra: notebooks
+License-File: LICENSE
+                                    [logo]
 ---
        [ci]  [coverage]  [documentation]  [downloads]  [pypi]  [python]
                                 [bsd_3_license]
 Frouros is a Python library for drift detection in machine learning systems
 that provides a combination of classical and more recent algorithms for both
 concept and data drift detection.
                  "Everything changes and nothing stands still"
```

### Comparing `frouros-0.3.0/README.md` & `frouros-0.3.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <p align="center">
-  <img height="115px" src="images/logo.png" alt="frouros_logo">
+  <img height="115px" src="https://raw.githubusercontent.com/IFCA/frouros/main/images/logo.png" alt="logo">
 </p>
 
 ---
 
 <p align="center">
   <!-- CI -->
   <a href="https://github.com/IFCA/frouros/actions/workflows/ci.yml">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-                                [frouros_logo]
+                                    [logo]
 ---
        [ci]  [coverage]  [documentation]  [downloads]  [pypi]  [python]
                                 [bsd_3_license]
 Frouros is a Python library for drift detection in machine learning systems
 that provides a combination of classical and more recent algorithms for both
 concept and data drift detection.
                  "Everything changes and nothing stands still"
```

### Comparing `frouros-0.3.0/frouros/callbacks/base.py` & `frouros-0.3.1/frouros/callbacks/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-"""Callbacks base module."""
+"""Base callback module."""
 
 import abc
 from typing import Optional
 
 
-class Callback(abc.ABC):
+class BaseCallback(abc.ABC):
     """Abstract class representing a callback."""
 
     def __init__(self, name: Optional[str] = None) -> None:
         """Init method.
 
         :param name: name value
         :type name: Optional[str]
@@ -39,23 +39,23 @@
         self._name = self.__class__.__name__ if value is None else value
 
     def set_detector(self, detector) -> None:
         """Set detector method."""
         self.detector = detector
 
     # @property
-    # def detector(self) -> Optional[ConceptDriftBase, DataDriftBatchBase]:
+    # def detector(self) -> Optional[BaseConceptDrift, BaseDataDriftBatch]:
     #     return self._detector
     #
     # @detector.setter
-    # def detector(self, value: Optional[ConceptDriftBase, DataDriftBatchBase]) -> None:
+    # def detector(self, value: Optional[BaseConceptDrift, BaseDataDriftBatch]) -> None:
     #     if not isinstance(
-    #             value, (ConceptDriftBase, DataDriftBatchBase)):
+    #             value, (BaseConceptDrift, BaseDataDriftBatch)):
     #         raise TypeError(
-    #             "value must be of type ConceptDriftBase or DataDriftBatchBase."
+    #             "value must be of type BaseConceptDrift or BaseDataDriftBatch."
     #         )
     #     self._detector = value
 
     def on_fit_start(self, **kwargs) -> None:
         """On fit start method."""
 
     def on_fit_end(self, **kwargs) -> None:
```

### Comparing `frouros-0.3.0/frouros/callbacks/batch/base.py` & `frouros-0.3.1/frouros/callbacks/batch/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-"""Batch base test module."""
+"""Base callback batch module."""
 
 import abc
 
-from frouros.callbacks.base import Callback
+from frouros.callbacks.base import BaseCallback
 
 
-class BatchCallback(Callback):
-    """Batch callback class."""
+class BaseCallbackBatch(BaseCallback):
+    """Callback batch class."""
 
     def on_compare_start(self) -> None:
         """On compare start method."""
 
     def on_compare_end(self, **kwargs) -> None:
         """On compare end method."""
```

### Comparing `frouros-0.3.0/frouros/callbacks/batch/permutation_test.py` & `frouros-0.3.1/frouros/callbacks/batch/permutation_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import multiprocessing
 from typing import Any, Callable, Dict, List, Optional, Tuple
 
 import numpy as np  # type: ignore
 from scipy.stats import norm  # type: ignore
 
-from frouros.callbacks.batch.base import BatchCallback
+from frouros.callbacks.batch.base import BaseCallbackBatch
 from frouros.utils.stats import permutation, z_score
 
 
-class PermutationTestOnBatchData(BatchCallback):
+class PermutationTestOnBatchData(BaseCallbackBatch):
     """Permutation test on batch data callback class."""
 
     def __init__(
         self,
         num_permutations: int,
         num_jobs: int = -1,
         name: Optional[str] = None,
@@ -159,17 +159,17 @@
     #  uncomment commented code when it is solved
 
     # def set_detector(self, detector) -> None:
     #     """Set detector method.
     #
     #     :raises TypeError: Type error exception
     #     """
-    #     if not isinstance(detector, DataDriftBatchBase):
+    #     if not isinstance(detector, BaseDataDriftBatch):
     #         raise TypeError(
     #             f"callback {self.__class__.name} cannot be used with detector"
     #             f" {detector.__class__name}. Must be used with a detector of "
-    #             f"type DataDriftBatchBase."
+    #             f"type BaseDataDriftBatch."
     #         )
     #     self.detector = detector
 
     def reset(self) -> None:
         """Reset method."""
```

### Comparing `frouros-0.3.0/frouros/callbacks/batch/reset_drift.py` & `frouros-0.3.1/frouros/callbacks/batch/reset_drift.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Reset on batch data drift callback module."""
 
 from typing import Optional
 
-from frouros.callbacks.batch.base import BatchCallback
+from frouros.callbacks.batch.base import BaseCallbackBatch
 
 
-class ResetOnBatchDataDrift(BatchCallback):
+class ResetOnBatchDataDrift(BaseCallbackBatch):
     """Reset on batch data drift callback class."""
 
     def __init__(self, alpha: float, name: Optional[str] = None) -> None:
         """Init method.
 
         :param alpha: significance value
         :type alpha: float
@@ -52,17 +52,17 @@
     #  uncomment commented code when it is solved
 
     # def set_detector(self, detector) -> None:
     #     """Set detector method.
     #
     #     :raises TypeError: Type error exception
     #     """
-    #     if not isinstance(detector, DataDriftBatchBase):
+    #     if not isinstance(detector, BaseDataDriftBatch):
     #         raise TypeError(
     #             f"callback {self.__class__.name} cannot be used with detector"
     #             f" {detector.__class__name}. Must be used with a detector of "
-    #             f"type DataDriftBatchBase."
+    #             f"type BaseDataDriftBatch."
     #         )
     #     self.detector = detector
 
     def reset(self) -> None:
         """Reset method."""
```

### Comparing `frouros-0.3.0/frouros/callbacks/streaming/base.py` & `frouros-0.3.1/frouros/callbacks/streaming/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-"""Streaming base test module."""
+"""Base callback streaming module."""
 
 import abc
-
 from typing import Union
 
-from frouros.callbacks.base import Callback
+from frouros.callbacks.base import BaseCallback
 
 
-class StreamingCallback(Callback):
-    """Streaming callback class."""
+class BaseCallbackStreaming(BaseCallback):
+    """Callback streaming class."""
 
     def on_update_start(self, value: Union[int, float], **kwargs) -> None:
         """On update start method."""
 
     def on_update_end(self, value: Union[int, float], **kwargs) -> None:
         """On update end method."""
```

### Comparing `frouros-0.3.0/frouros/callbacks/streaming/history.py` & `frouros-0.3.1/frouros/callbacks/streaming/history.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """History callback module."""
 
 from typing import Any, Dict, List, Optional, Union
 
-from frouros.callbacks.streaming.base import StreamingCallback
-from frouros.utils.stats import Stat
+from frouros.callbacks.streaming.base import BaseCallbackStreaming
+from frouros.utils.stats import BaseStat
 
 
-class History(StreamingCallback):
+class History(BaseCallbackStreaming):
     """History callback class."""
 
     def __init__(self, name: Optional[str] = None) -> None:
         """Init method.
 
         :param name: name value
         :type name: Optional[str]
@@ -45,34 +45,34 @@
         self.history["drift"].append(self.detector.drift)  # type: ignore
         for var in self.additional_vars:
             additional_var = self.detector.additional_vars[var]  # type: ignore
             # FIXME: Extract isinstance check to be done when  # pylint: disable=fixme
             #  add_addtional_vars is called (avoid the same computation)
             self.history[var].append(
                 additional_var.get()
-                if isinstance(additional_var, Stat)
+                if isinstance(additional_var, BaseStat)
                 else additional_var
             )
 
         self.logs.update(**self.history)
 
     # FIXME: set_detector method as a workaround to  # pylint: disable=fixme
     #  avoid circular import problem. Make it an abstract method and
     #  uncomment commented code when it is solved
 
     # def set_detector(self, detector) -> None:
     #     """Set detector method.
     #
     #     :raises TypeError: Type error exception
     #     """
-    #     if not isinstance(detector, ConceptDriftBase):
+    #     if not isinstance(detector, BaseConceptDrift):
     #         raise TypeError(
     #             f"callback {self.__class__.name} cannot be used with detector"
     #             f" {detector.__class__name}. Must be used with a detector of "
-    #             f"type ConceptDriftBase."
+    #             f"type BaseConceptDrift."
     #         )
     #     self.detector = detector
 
     def reset(self) -> None:
         """Reset method."""
         for key in self.history.keys():
             self.history[key].clear()
```

### Comparing `frouros-0.3.0/frouros/callbacks/streaming/msprt.py` & `frouros-0.3.1/frouros/callbacks/streaming/msprt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """mSPRT (Mixing Sequentially Probability Ratio Test) callback module."""
 
 from typing import Union, Tuple, Optional
 
 import numpy as np  # type: ignore
 
-from frouros.callbacks.streaming.base import StreamingCallback
+from frouros.callbacks.streaming.base import BaseCallbackStreaming
 from frouros.utils.stats import CircularMean
 
 
-class mSPRT(StreamingCallback):  # noqa: N801 # pylint: disable=invalid-name
+class mSPRT(BaseCallbackStreaming):  # noqa: N801 # pylint: disable=invalid-name
     """mSPRT (mixing Sequentially Probability Ratio Test) callback class.
 
     :References:
 
     .. [johari2022always] Ramesh, Johari, et al.
         "Always valid inference: Continuous monitoring of a/b tests"
         Operations Research 70.3 (2022): 1806-1821.
```

### Comparing `frouros-0.3.0/frouros/callbacks/streaming/warning_samples.py` & `frouros-0.3.1/frouros/callbacks/streaming/warning_samples.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Warning samples buffer callback module."""
 
 import copy
 from typing import Any, List, Optional, Union
 
-from frouros.callbacks.streaming.base import StreamingCallback
+from frouros.callbacks.streaming.base import BaseCallbackStreaming
 
 
-class WarningSamplesBuffer(StreamingCallback):
+class WarningSamplesBuffer(BaseCallbackStreaming):
     """Store warning samples as a buffer callback class."""
 
     def __init__(self, name: Optional[str] = None) -> None:
         """Init method.
 
         :param name: name to be use
         :type name: Optional[str]
```

### Comparing `frouros-0.3.0/frouros/datasets/base.py` & `frouros-0.3.1/frouros/datasets/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-"""Dataset base module."""
+"""Base dataset module."""
 
 import abc
 import tempfile
-from typing import Any, List, Optional, Union
 import urllib.parse
 from pathlib import Path
+from typing import Any, List, Optional, Union
 
 import numpy as np  # type: ignore
 import requests
 
 from frouros.datasets.exceptions import (
     DownloadError,
     InvalidURLError,
     ReadFileError,
 )
 from frouros.utils.logger import logger
 
 
-class Dataset(abc.ABC):
+class BaseDatasetDownload(abc.ABC):
     """Abstract class representing a downloadable dataset."""
 
     def __init__(
         self,
         url: Union[str, List[str]],
         file_path: Optional[str] = None,
     ) -> None:
@@ -171,15 +171,15 @@
         """
         return (
             f"{self.__class__.__name__}"
             f"(url={self.url}, file_path='{self.file_path}')"
         )
 
 
-class Generator(abc.ABC):
+class BaseDatasetGenerator(abc.ABC):
     """Abstract class representing a dataset generator."""
 
     def __init__(self, seed: Optional[int] = None) -> None:
         """Init method.
 
         :param seed: seed value
         :type seed: Optional[int]
```

### Comparing `frouros-0.3.0/frouros/datasets/real.py` & `frouros-0.3.1/frouros/datasets/real.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Real datasets module."""
 
 from typing import Optional
 
 import numpy as np  # type: ignore
 from scipy.io import arff  # type: ignore
-from frouros.datasets.base import Dataset
 
+from frouros.datasets.base import BaseDatasetDownload
 
-class Elec2(Dataset):
+
+class Elec2(BaseDatasetDownload):
     """Elec2 dataset [harries1999splice]_.
 
     :References:
 
     .. [harries1999splice] Harries, Michael.
         "Splice-2 comparative evaluation: Electricity pricing." (1999).
     """
```

### Comparing `frouros-0.3.0/frouros/datasets/synthetic.py` & `frouros-0.3.1/frouros/datasets/synthetic.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Synthetic datasets module."""
 
 from typing import Tuple, Iterator
 
 import numpy as np  # type: ignore
 
-from frouros.datasets.base import Generator
+from frouros.datasets.base import BaseDatasetGenerator
 from frouros.datasets.exceptions import InvalidBlockError
 
 
-class SEA(Generator):
+class SEA(BaseDatasetGenerator):
     """SEA generator [street2001streaming]_.
 
     :References:
 
     .. [street2001streaming] Street, W. Nick, and YongSeog Kim.
         "A streaming ensemble algorithm (SEA) for large-scale classification."
         Proceedings of the seventh ACM SIGKDD international conference on Knowledge
@@ -55,15 +55,15 @@
         dataset = (
             self._generate_sample(threshold=threshold, noise=noise)
             for _ in range(num_samples)
         )
         return dataset
 
 
-class Dummy(Generator):
+class Dummy(BaseDatasetGenerator):
     """Dummy generator class."""
 
     @staticmethod
     def _generate_sample(class_: int) -> Tuple[np.ndarray, int]:
         X = np.random.uniform(low=0.0, high=10.0, size=(2,))  # noqa: N806
         y = class_ if X[0] + X[1] < 10.0 else 1 - class_
         return X, y
```

### Comparing `frouros-0.3.0/frouros/detectors/base.py` & `frouros-0.3.1/frouros/detectors/data_drift/streaming/distance_based/mmd.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,79 +1,101 @@
-"""Detector base module."""
+"""MMD (Maximum Mean Discrepancy) module."""
 
-import abc
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Callable, Dict, Optional, List, Tuple, Union
 
 import numpy as np  # type: ignore
 
-from frouros.callbacks import Callback
-
-
-class DetectorBase(abc.ABC):
-    """Abstract class representing a detector."""
+from frouros.callbacks.base import BaseCallback
+from frouros.detectors.data_drift.base import NumericalData, MultivariateData
+from frouros.detectors.data_drift.batch import MMD as MMDBatch  # noqa: N811
+from frouros.detectors.data_drift.batch.distance_based.mmd import rbf_kernel
+from frouros.detectors.data_drift.streaming.distance_based.base import (
+    BaseDistanceBased,
+    DistanceResult,
+)
+from frouros.utils.data_structures import CircularQueue
+
+
+class MMD(BaseDistanceBased):
+    """MMD (Maximum Mean Discrepancy) [gretton2012kernel]_ detector.
+
+    :References:
+
+    .. [gretton2012kernel] Gretton, Arthur, et al.
+        "A kernel two-sample test."
+        The Journal of Machine Learning Research 13.1 (2012): 723-773.
+    """
 
     def __init__(
         self,
-        callbacks: Optional[Union[Callback, List[Callback]]] = None,
+        window_size: int,
+        kernel: Callable = rbf_kernel,
+        chunk_size: Optional[int] = None,
+        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
     ) -> None:
         """Init method.
 
+        :param window_size: window size
+        :type window_size: int
+        :param kernel: kernel function
+        :type kernel: Callable
+        :param chunk_size: chunk size value
+        :type chunk_size: Optional[int]
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[Callback, List[Callback]]]
+        :type callbacks: Optional[Union[Callback, List[BaseCallback]]]
         """
-        self.callbacks = callbacks  # type: ignore
+        super().__init__(
+            data_type=NumericalData(),
+            statistical_type=MultivariateData(),
+            callbacks=callbacks,
+        )
+        self.mmd = MMDBatch(
+            kernel=kernel,
+            chunk_size=chunk_size,
+        )
+        self.window_size = window_size
+        self.X_queue = CircularQueue(max_len=self.window_size)
 
     @property
-    def callbacks(self) -> Optional[List[Callback]]:
-        """Callbacks property.
+    def window_size(self) -> int:
+        """Window size property.
 
-        :return: callbacks
-        :rtype: Optional[List[Callback]]
+        :return: window size
+        :rtype: int
         """
-        return self._callbacks  # type: ignore
+        return self._window_size
 
-    @callbacks.setter
-    def callbacks(self, value: Optional[Union[Callback, List[Callback]]]) -> None:
-        """Callbacks setter.
+    @window_size.setter
+    def window_size(self, value: int) -> None:
+        """Window size setter.
 
         :param value: value to be set
-        :type value: Optional[Union[Callback, List[Callback]]]
-        :raises TypeError: Type error exception
+        :type value: int
+        :raises ValueError: Value error exception
         """
-        if value is not None:
-            if isinstance(value, Callback):
-                self._callbacks = [value]
-            elif not all(
-                isinstance(callback, Callback) for callback in value  # type: ignore
-            ):
-                raise TypeError("value must be of type None or a list of Callback.")
-            else:
-                self._callbacks = value  # type: ignore
-        else:
-            self._callbacks = []
-
-    @abc.abstractmethod
-    def reset(self) -> None:
-        """Reset method."""
-
-    def _get_callbacks_logs(self) -> Dict[str, Any]:
-        logs = {
-            callback.name: callback.logs for callback in self.callbacks  # type: ignore
-        }
-        return logs
-
-    @staticmethod
-    def _check_array(X: Any) -> None:  # noqa: N803
-        if not isinstance(X, np.ndarray):
-            raise TypeError("X must be a numpy array")
+        if value < 1:
+            raise ValueError("window_size value must be greater than 0.")
+        self._window_size = value
 
-    def __repr__(self) -> str:
-        """Repr method.
+    def _fit(self, X: np.ndarray) -> None:  # noqa: N803
+        self.mmd.fit(X=X)
+        self.X_ref = self.mmd.X_ref
 
-        :return: repr value
-        :rtype: str
-        """
-        return (
-            f"{self.__class__.__name__}"
-            f"(callbacks=["
-            f"{', '.join([*map(str, self.callbacks)])}])"  # type: ignore
-        )
+    def _reset(self) -> None:
+        super()._reset()
+        self.mmd.reset()
+
+    def _update(self, value: Union[int, float]) -> Optional[DistanceResult]:
+        self.X_queue.enqueue(value=value)
+
+        if self.num_instances < self.window_size:
+            return None
+
+        # FIXME: Handle callback logs. Now are ignored.  # pylint: disable=fixme
+        distance, _ = self.mmd.compare(X=np.array(self.X_queue))
+        return distance
+
+    def _compare(
+        self,
+        X: np.ndarray,  # noqa: N803
+    ) -> Tuple[Optional[DistanceResult], Dict[str, Any]]:  # noqa: N803
+        return self.mmd.compare(X=X)
```

### Comparing `frouros-0.3.0/frouros/detectors/concept_drift/__init__.py` & `frouros-0.3.1/frouros/detectors/concept_drift/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.0/frouros/detectors/concept_drift/base.py` & `frouros-0.3.1/frouros/detectors/concept_drift/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-"""Concept drift base module."""
+"""Base concept drift module."""
 
 import abc
 from typing import Any, Dict, List, Optional, Union
 
-from frouros.callbacks import Callback, History
-from frouros.detectors.base import DetectorBase
+from frouros.callbacks import History
+from frouros.callbacks.base import BaseCallback
+from frouros.detectors.base import BaseDetector
 
 
-class ConceptDriftBaseConfig(abc.ABC):
+class BaseConceptDriftConfig(abc.ABC):
     """Abstract class representing a concept drift configuration class."""
 
     def __init__(
         self,
         min_num_instances: int = 10,
     ) -> None:
         """Init method.
@@ -51,30 +52,30 @@
         """
         return (
             f"{self.__class__.__name__}"
             f"({', '.join(f'{k[1:]}={v}' for k, v in self.__dict__.items())})"
         )
 
 
-class ConceptDriftBase(DetectorBase):
+class BaseConceptDrift(BaseDetector):
     """Abstract class representing a concept drift streaming."""
 
-    config_type = ConceptDriftBaseConfig
+    config_type = BaseConceptDriftConfig
 
     def __init__(
         self,
-        config: Optional[ConceptDriftBaseConfig] = None,
-        callbacks: Optional[Union[Callback, List[Callback]]] = None,
+        config: Optional[BaseConceptDriftConfig] = None,
+        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
     ) -> None:
         """Init method.
 
         :param config: configuration parameters
-        :type config: Optional[ConceptDriftBaseConfig]
+        :type config: Optional[BaseConceptDriftConfig]
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[Callback, List[Callback]]]
+        :type callbacks: Optional[Union[BaseCallback, List[Callback]]]
         """
         super().__init__(callbacks=callbacks)
         self.config = config  # type: ignore
         self.additional_vars = None
 
         self.num_instances = 0
         self.drift = False
@@ -104,28 +105,28 @@
 
         :param value: value to be set
         :type value: Optional[Dict[str, Any]]
         """
         self._additional_vars = value if value is not None else {}
 
     @property
-    def config(self) -> ConceptDriftBaseConfig:
+    def config(self) -> BaseConceptDriftConfig:
         """Config property.
 
         :return: configuration parameters of the estimator
-        :rtype: ConceptDriftBaseConfig
+        :rtype: BaseConceptDriftConfig
         """
         return self._config
 
     @config.setter
-    def config(self, value: Optional[ConceptDriftBaseConfig]) -> None:
+    def config(self, value: Optional[BaseConceptDriftConfig]) -> None:
         """Config setter.
 
         :param value: value to be set
-        :type value: ConceptDriftBaseConfig
+        :type value: BaseConceptDriftConfig
         :raises TypeError: Type error exception
         """
         if value is not None:
             if not isinstance(value, self.config_type):
                 raise TypeError(
                     f"value must be of type " f"{self.config_type.__class__.__name__}."
                 )
```

### Comparing `frouros-0.3.0/frouros/detectors/concept_drift/streaming/__init__.py` & `frouros-0.3.1/frouros/detectors/concept_drift/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.0/frouros/detectors/concept_drift/streaming/base.py` & `frouros-0.3.1/frouros/detectors/concept_drift/streaming/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-"""Concept drift streaming base module."""
+"""Base concept drift streaming module."""
 
 import abc
-
 from typing import Union
 
 from frouros.detectors.concept_drift.base import (
-    ConceptDriftBase,
-    ConceptDriftBaseConfig,
+    BaseConceptDrift,
+    BaseConceptDriftConfig,
 )
 
 
-class ConceptDriftStreamingBaseConfig(ConceptDriftBaseConfig):
+class BaseConceptDriftStreamingConfig(BaseConceptDriftConfig):
     """Abstract class representing a concept drift streaming configuration class."""
 
 
-class ConceptDriftStreamingBase(ConceptDriftBase):
+class BaseConceptDriftStreaming(BaseConceptDrift):
     """Abstract class representing a concept drift streaming detector."""
 
     @abc.abstractmethod
     def _update(self, value: Union[int, float], **kwargs) -> None:
         pass
```

### Comparing `frouros-0.3.0/frouros/detectors/concept_drift/streaming/cusum_based/base.py` & `frouros-0.3.1/frouros/detectors/concept_drift/streaming/cusum_based/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-"""Concept drift CUSUM based base module."""
+"""Base concept drift CUSUM based module."""
 
 import abc
 from typing import List, Optional, Union
 
-from frouros.callbacks import Callback
+from frouros.callbacks.base import BaseCallback
 from frouros.detectors.concept_drift.streaming.base import (
-    ConceptDriftStreamingBase,
-    ConceptDriftStreamingBaseConfig,
+    BaseConceptDriftStreaming,
+    BaseConceptDriftStreamingConfig,
 )
 from frouros.utils.stats import Mean
 
 
-class CUSUMBaseConfig(ConceptDriftStreamingBaseConfig):
+class BaseCUSUMConfig(BaseConceptDriftStreamingConfig):
     """Class representing a CUSUM based configuration class."""
 
     def __init__(
         self,
         lambda_: float = 50.0,
         min_num_instances: int = 30,
     ) -> None:
@@ -120,30 +120,30 @@
         :raises ValueError: Value error exception
         """
         if not 0.0 <= value <= 1.0:
             raise ValueError("alpha must be in the range [0, 1].")
         self._alpha = value
 
 
-class CUSUMBase(ConceptDriftStreamingBase):
+class BaseCUSUM(BaseConceptDriftStreaming):
     """CUSUM based algorithm class."""
 
-    config_type = CUSUMBaseConfig
+    config_type = BaseCUSUMConfig
 
     def __init__(
         self,
-        config: Optional[CUSUMBaseConfig] = None,
-        callbacks: Optional[Union[Callback, List[Callback]]] = None,
+        config: Optional[BaseCUSUMConfig] = None,
+        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
     ) -> None:
         """Init method.
 
         :param config: configuration parameters
-        :type config: Optional[CUSUMBaseConfig]
+        :type config: Optional[BaseCUSUMConfig]
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[Callback, List[Callback]]]
+        :type callbacks: Optional[Union[BaseCallback, List[Callback]]]
         """
         super().__init__(
             config=config,
             callbacks=callbacks,
         )
         self.additional_vars = {
             "mean_error_rate": Mean(),
```

### Comparing `frouros-0.3.0/frouros/detectors/concept_drift/streaming/cusum_based/cusum.py` & `frouros-0.3.1/frouros/detectors/concept_drift/streaming/cusum_based/cusum.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """CUSUM module."""
 
 import numpy as np  # type: ignore
 
 from frouros.detectors.concept_drift.streaming.cusum_based.base import (
-    CUSUMBase,
-    CUSUMBaseConfig,
+    BaseCUSUM,
+    BaseCUSUMConfig,
     DeltaConfig,
 )
 
 
-class CUSUMConfig(CUSUMBaseConfig, DeltaConfig):
+class CUSUMConfig(BaseCUSUMConfig, DeltaConfig):
     """CUSUM [page1954continuous]_ configuration.
 
     :References:
 
     .. [page1954continuous] Page, Ewan S.
         "Continuous inspection schemes."
         Biometrika 41.1/2 (1954): 100-115.
@@ -31,21 +31,21 @@
         :type delta: float
         :param lambda_: delta value
         :type lambda_: float
         :param min_num_instances: minimum numbers of instances
         to start looking for changes
         :type min_num_instances: int
         """
-        CUSUMBaseConfig.__init__(
+        BaseCUSUMConfig.__init__(
             self, lambda_=lambda_, min_num_instances=min_num_instances
         )
         DeltaConfig.__init__(self, delta=delta)
 
 
-class CUSUM(CUSUMBase):
+class CUSUM(BaseCUSUM):
     """CUSUM [page1954continuous]_ detector.
 
     :References:
 
     .. [page1954continuous] Page, Ewan S.
         "Continuous inspection schemes."
         Biometrika 41.1/2 (1954): 100-115.
```

### Comparing `frouros-0.3.0/frouros/detectors/concept_drift/streaming/cusum_based/geometric_moving_average.py` & `frouros-0.3.1/frouros/detectors/concept_drift/streaming/cusum_based/geometric_moving_average.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Geometric Moving Average module."""
 
 from frouros.detectors.concept_drift.streaming.cusum_based.base import (
-    CUSUMBase,
-    CUSUMBaseConfig,
+    BaseCUSUM,
+    BaseCUSUMConfig,
     AlphaConfig,
 )
 
 
-class GeometricMovingAverageConfig(CUSUMBaseConfig, AlphaConfig):
+class GeometricMovingAverageConfig(BaseCUSUMConfig, AlphaConfig):
     """Geometric Moving Average [robertst1959control]_ configuration.
 
     :References:
 
     .. [robertst1959control] Roberts, S. W.
         “Control Chart Tests Based on Geometric Moving Averages.”
         Technometrics, vol. 1, no. 3, 1959, pp. 239–50.
@@ -30,21 +30,21 @@
         :type alpha: float
         :param lambda_: delta value
         :type lambda_: float
         :param min_num_instances: minimum numbers of instances
         to start looking for changes
         :type min_num_instances: int
         """
-        CUSUMBaseConfig.__init__(
+        BaseCUSUMConfig.__init__(
             self, lambda_=lambda_, min_num_instances=min_num_instances
         )
         AlphaConfig.__init__(self, alpha=alpha)
 
 
-class GeometricMovingAverage(CUSUMBase):
+class GeometricMovingAverage(BaseCUSUM):
     """Geometric Moving Average [robertst1959control]_ detector.
 
     :References:
 
     .. [robertst1959control] Roberts, S. W.
         “Control Chart Tests Based on Geometric Moving Averages.”
         Technometrics, vol. 1, no. 3, 1959, pp. 239–50.
```

### Comparing `frouros-0.3.0/frouros/detectors/concept_drift/streaming/cusum_based/page_hinkley.py` & `frouros-0.3.1/frouros/detectors/concept_drift/streaming/cusum_based/page_hinkley.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Page Hinkley module."""
 
 from frouros.detectors.concept_drift.streaming.cusum_based.base import (
-    CUSUMBase,
-    CUSUMBaseConfig,
+    BaseCUSUM,
+    BaseCUSUMConfig,
     DeltaConfig,
     AlphaConfig,
 )
 
 
-class PageHinkleyConfig(CUSUMBaseConfig, DeltaConfig, AlphaConfig):
+class PageHinkleyConfig(BaseCUSUMConfig, DeltaConfig, AlphaConfig):
     """Page Hinkley [page1954continuous]_ configuration.
 
     :References:
 
     .. [page1954continuous] Page, Ewan S.
         "Continuous inspection schemes."
         Biometrika 41.1/2 (1954): 100-115.
@@ -33,22 +33,22 @@
         :type lambda_: float
         :param min_num_instances: minimum numbers of instances
         to start looking for changes
         :type min_num_instances: int
         :param alpha: forgetting factor value
         :type alpha: float
         """
-        CUSUMBaseConfig.__init__(
+        BaseCUSUMConfig.__init__(
             self, min_num_instances=min_num_instances, lambda_=lambda_
         )
         DeltaConfig.__init__(self, delta=delta)
         AlphaConfig.__init__(self, alpha=alpha)
 
 
-class PageHinkley(CUSUMBase):
+class PageHinkley(BaseCUSUM):
     """Page Hinkley [page1954continuous]_ detector.
 
     :References:
 
     .. [page1954continuous] Page, Ewan S.
         "Continuous inspection schemes."
         Biometrika 41.1/2 (1954): 100-115.
```

### Comparing `frouros-0.3.0/frouros/detectors/concept_drift/streaming/statistical_process_control/base.py` & `frouros-0.3.1/frouros/detectors/concept_drift/streaming/statistical_process_control/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-"""Concept drift SPC (statistical process control) base module."""
+"""Base concept drift SPC (statistical process control) module."""
 
 import abc
 from typing import Dict, List, Optional, Tuple, Union
 
 import numpy as np  # type: ignore
 
-from frouros.callbacks import Callback
+from frouros.callbacks.base import BaseCallback
+from frouros.detectors.concept_drift.exceptions import InvalidAverageRunLengthError
 from frouros.detectors.concept_drift.streaming.base import (
-    ConceptDriftStreamingBaseConfig,
-    ConceptDriftStreamingBase,
+    BaseConceptDriftStreamingConfig,
+    BaseConceptDriftStreaming,
 )
-from frouros.detectors.concept_drift.exceptions import InvalidAverageRunLengthError
 from frouros.utils.stats import Mean
 
 
-class SPCBaseConfig(ConceptDriftStreamingBaseConfig):
+class BaseSPCConfig(BaseConceptDriftStreamingConfig):
     """Class representing a SPC configuration class."""
 
     def __init__(
         self,
         warning_level: float = 2.0,
         drift_level: float = 3.0,
         min_num_instances: int = 30,
@@ -78,30 +78,30 @@
         :raises ValueError: Value error exception
         """
         if value <= 0.0:
             raise ValueError("warning level must be greater than 0.0.")
         self._warning_level = value
 
 
-class SPCBase(ConceptDriftStreamingBase):
+class BaseSPC(BaseConceptDriftStreaming):
     """Abstract class representing an SPC estimator."""
 
-    config_type = SPCBaseConfig
+    config_type = BaseSPCConfig
 
     def __init__(
         self,
-        config: Optional[SPCBaseConfig] = None,
-        callbacks: Optional[Union[Callback, List[Callback]]] = None,
+        config: Optional[BaseSPCConfig] = None,
+        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
     ) -> None:
         """Init method.
 
         :param config: configuration parameters
-        :type config: Optional[SPCBaseConfig]
+        :type config: Optional[BaseSPCConfig]
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[Callback, List[Callback]]]
+        :type callbacks: Optional[Union[Callback, List[BaseCallback]]]
         """
         super().__init__(
             config=config,
             callbacks=callbacks,
         )
         self.additional_vars = {
             "warning": False,
@@ -141,30 +141,30 @@
         return {**super().status, "warning": self.warning}
 
     @abc.abstractmethod
     def _update(self, value: Union[int, float], **kwargs) -> None:
         pass
 
 
-class SPCErrorBase(SPCBase):
+class BaseSPCError(BaseSPC):
     """Abstract class representing a SPC error estimator."""
 
-    config_type = SPCBaseConfig
+    config_type = BaseSPCConfig
 
     def __init__(
         self,
-        config: Optional[SPCBaseConfig] = None,
-        callbacks: Optional[Union[Callback, List[Callback]]] = None,
+        config: Optional[BaseSPCConfig] = None,
+        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
     ) -> None:
         """Init method.
 
         :param config: configuration parameters
-        :type config: Optional[SPCBaseConfig]
+        :type config: Optional[BaseSPCConfig]
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[Callback, List[Callback]]]
+        :type callbacks: Optional[Union[Callback, List[BaseCallback]]]
         """
         super().__init__(
             config=config,
             callbacks=callbacks,
         )
         self.additional_vars = {
             "error_rate": Mean(),
@@ -269,15 +269,15 @@
         self.min_std = float("inf")
 
     @abc.abstractmethod
     def _update(self, value: Union[int, float], **kwargs) -> None:
         pass
 
 
-class ECDDBaseConfig(ConceptDriftStreamingBaseConfig):
+class BaseECDDConfig(BaseConceptDriftStreamingConfig):
     """Class representing a ECDD configuration class."""
 
     average_run_length_map = {
         100: lambda p: 2.76
         - 6.23 * p
         + 18.12 * np.power(p, 3)
         - 312.45 * np.power(p, 5)
```

### Comparing `frouros-0.3.0/frouros/detectors/concept_drift/streaming/statistical_process_control/ddm.py` & `frouros-0.3.1/frouros/detectors/concept_drift/streaming/statistical_process_control/ddm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 """DDM (Drift detection method) module."""
 
 from contextlib import suppress
 from typing import Union
 
 from frouros.detectors.concept_drift.streaming.statistical_process_control.base import (
-    SPCBaseConfig,
-    SPCErrorBase,
+    BaseSPCConfig,
+    BaseSPCError,
 )
 
 
-class DDMConfig(SPCBaseConfig):
+class DDMConfig(BaseSPCConfig):
     """DDM (Drift detection method) [gama2004learning]_ configuration.
 
     :References:
 
     .. [gama2004learning] Gama, Joao, et al.
         "Learning with drift detection."
         Advances in Artificial Intelligence–SBIA 2004: 17th Brazilian Symposium on
         Artificial Intelligence, Sao Luis, Maranhao, Brazil, September 29-Ocotber 1,
         2004. Proceedings 17. Springer Berlin Heidelberg, 2004.
     """
 
 
-class DDM(SPCErrorBase):
+class DDM(BaseSPCError):
     """DDM (Drift detection method) [gama2004learning]_ detector.
 
     :References:
 
     .. [gama2004learning] Gama, Joao, et al.
         "Learning with drift detection."
         Advances in Artificial Intelligence–SBIA 2004: 17th Brazilian Symposium on
```

### Comparing `frouros-0.3.0/frouros/detectors/concept_drift/streaming/statistical_process_control/ecdd.py` & `frouros-0.3.1/frouros/detectors/concept_drift/streaming/statistical_process_control/ecdd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 """ECDD (EWMA for Concept Drift Detection) module."""
 
 from typing import List, Optional, Union
 
 import numpy as np  # type: ignore
 
-from frouros.callbacks import Callback
+from frouros.callbacks.base import BaseCallback
 from frouros.detectors.concept_drift.streaming.statistical_process_control.base import (
-    SPCBase,
-    ECDDBaseConfig,
+    BaseSPC,
+    BaseECDDConfig,
 )
 from frouros.utils.stats import EWMA, Mean
 
 
-class ECDDWTConfig(ECDDBaseConfig):
+class ECDDWTConfig(BaseECDDConfig):
     """ECDDWT (EWMA Concept Drift Detection Warning) [ross2012exponentially]_ configuration.
 
     :References:
 
     .. [ross2012exponentially] Ross, Gordon J., et al.
         "Exponentially weighted moving average charts for detecting concept drift."
         Pattern recognition letters 33.2 (2012): 191-198.
     """
 
 
-class ECDDWT(SPCBase):
+class ECDDWT(BaseSPC):
     """ECDDWT (EWMA Concept Drift Detection Warning) [ross2012exponentially]_ detector.
 
     :References:
 
     .. [ross2012exponentially] Ross, Gordon J., et al.
         "Exponentially weighted moving average charts for detecting concept drift."
         Pattern recognition letters 33.2 (2012): 191-198.
     """
 
     config_type = ECDDWTConfig  # type: ignore
 
     def __init__(
         self,
         config: Optional[ECDDWTConfig] = None,
-        callbacks: Optional[Union[Callback, List[Callback]]] = None,
+        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
     ) -> None:
         """Init method.
 
         :param config: configuration parameters
         :type config: Optional[ECDDWTConfig]
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[Callback, List[Callback]]]
+        :type callbacks: Optional[Union[Callback, List[BaseCallback]]]
         """
         super().__init__(
             config=config,  # type: ignore
             callbacks=callbacks,
         )
         self.additional_vars = {
             "p": Mean(),
```

### Comparing `frouros-0.3.0/frouros/detectors/concept_drift/streaming/statistical_process_control/eddm.py` & `frouros-0.3.1/frouros/detectors/concept_drift/streaming/statistical_process_control/eddm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """EDDM (Early drift detection method) module."""
 
 import copy
 from typing import List, Optional, Union
 
 import numpy as np  # type: ignore
 
-from frouros.callbacks import Callback
+from frouros.callbacks.base import BaseCallback
 from frouros.detectors.concept_drift.streaming.statistical_process_control.base import (
-    SPCBaseConfig,
-    SPCBase,
+    BaseSPCConfig,
+    BaseSPC,
 )
 
 
-class EDDMConfig(SPCBaseConfig):
+class EDDMConfig(BaseSPCConfig):
     """EDDM (Early drift detection method) [baena2006early]_ configuration.
 
     :References:
 
     .. [baena2006early] Baena-Garcıa, Manuel, et al. "Early drift detection method."
         Fourth international workshop on knowledge discovery from data streams.
         Vol. 6. 2006.
@@ -129,37 +129,37 @@
         if value < 0:
             raise ValueError(
                 "min_num_misclassified_instances must be greater or equal than 0."
             )
         self._min_num_misclassified_instances = value
 
 
-class EDDM(SPCBase):
+class EDDM(BaseSPC):
     """EDDM (Early drift detection method) [baena2006early]_ detector.
 
     :References:
 
     .. [baena2006early] Baena-Garcıa, Manuel, et al. "Early drift detection method."
         Fourth international workshop on knowledge discovery from data streams.
         Vol. 6. 2006.
     """
 
     config_type = EDDMConfig  # type: ignore
 
     def __init__(
         self,
         config: Optional[EDDMConfig] = None,
-        callbacks: Optional[Union[Callback, List[Callback]]] = None,
+        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
     ) -> None:
         """Init method.
 
         :param config: configuration parameters
         :type config: Optional[EDDMConfig]
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[Callback, List[Callback]]]
+        :type callbacks: Optional[Union[BaseCallback, List[Callback]]]
         """
         # mean_distance_error = 0.0
         super().__init__(
             config=config,
             callbacks=callbacks,
         )
         mean_distance_error = 0.0
```

### Comparing `frouros-0.3.0/frouros/detectors/concept_drift/streaming/statistical_process_control/hddm.py` & `frouros-0.3.1/frouros/detectors/concept_drift/streaming/statistical_process_control/hddm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """HDDM (Hoeffding's inequality drift detection method) module."""
 
 import copy
 from typing import List, Optional, Tuple, Union
 
 import numpy as np  # type: ignore
 
-from frouros.callbacks import Callback
+from frouros.callbacks.base import BaseCallback
 from frouros.detectors.concept_drift.streaming.statistical_process_control.base import (
-    SPCBaseConfig,
-    SPCBase,
+    BaseSPCConfig,
+    BaseSPC,
 )
 from frouros.utils.stats import EWMA, Mean
 
 
-class HDDMBaseConfig(SPCBaseConfig):
+class BaseHDDMConfig(BaseSPCConfig):
     """HDDM (Hoeffding's drift detection method) [frias2014online]_ configuration.
 
     :References:
 
     .. [frias2014online] Frias-Blanco, Isvani, et al.
         "Online and non-parametric drift detection methods based on Hoeffding’s bounds."
         IEEE Transactions on Knowledge and Data Engineering 27.3 (2014): 810-823.
@@ -109,27 +109,27 @@
         :raises ValueError: Value error exception
         """
         if not isinstance(value, bool):
             raise ValueError("two_sided_test must be of type bool.")
         self._two_sided_test = value
 
 
-class HDDMAConfig(HDDMBaseConfig):
+class HDDMAConfig(BaseHDDMConfig):
     """HDDM-A (Hoeffding's drift detection method A-Test) [frias2014online]_ configuration.
 
     :References:
 
     .. [frias2014online] Frias-Blanco, Isvani, et al.
         "Online and non-parametric drift detection methods based on Hoeffding’s bounds."
         IEEE Transactions on Knowledge and Data Engineering 27.3 (2014):
         810-823.
     """
 
 
-class HDDMWConfig(HDDMBaseConfig):
+class HDDMWConfig(BaseHDDMConfig):
     """HDDM-W (Hoeffding's drift detection method W-Test) [frias2014online]_ configuration.
 
     :References:
 
     .. [frias2014online] Frias-Blanco, Isvani, et al.
         "Online and non-parametric drift detection methods based on Hoeffding’s bounds."
         IEEE Transactions on Knowledge and Data Engineering 27.3 (2014):
@@ -314,15 +314,15 @@
         """
         super().update_cut_point(epsilon_z=epsilon_z)
         epsilon_y = self.hoeffding_error_bound(num_values=self.y.num_values)
         if self.y.mean - epsilon_y <= self.z.mean - epsilon_z:
             self.y = copy.deepcopy(self.z)
 
 
-class HDDMA(SPCBase):
+class HDDMA(BaseSPC):
     """HDDM-A (Hoeffding's drift detection method with A-Test) [frias2014online]_ detector.
 
     :References:
 
     .. [frias2014online] Frias-Blanco, Isvani, et al.
         "Online and non-parametric drift detection methods based on Hoeffding’s bounds."
         IEEE Transactions on Knowledge and Data Engineering 27.3 (2014):
@@ -330,22 +330,22 @@
     """
 
     config_type = HDDMAConfig  # type: ignore
 
     def __init__(
         self,
         config: Optional[HDDMAConfig] = None,
-        callbacks: Optional[Union[Callback, List[Callback]]] = None,
+        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
     ) -> None:
         """Init method.
 
         :param config: configuration parameters
         :type config: Optional[HDDMAConfig]
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[Callback, List[Callback]]]
+        :type callbacks: Optional[Union[BaseCallback, List[Callback]]]
         """
         super().__init__(
             config=config,
             callbacks=callbacks,
         )
         self.additional_vars = {
             "test_type": (
@@ -610,15 +610,15 @@
             self.decrease_cut_point = ewma_minus_epsilon
             self.sample_decrease_1 = copy.deepcopy(self.total)
             self.sample_decrease_2 = SampleInfo(lambda_=self.lambda_)
         else:
             self.sample_decrease_2.update(value=value)
 
 
-class HDDMW(SPCBase):
+class HDDMW(BaseSPC):
     """HDDM-W (Hoeffding's drift detection method with W-Test) [frias2014online]_ detector.
 
     :References:
 
     .. [frias2014online] Frias-Blanco, Isvani, et al.
         "Online and non-parametric drift detection methods based on Hoeffding’s bounds."
         IEEE Transactions on Knowledge and Data Engineering 27.3 (2014):
@@ -626,22 +626,22 @@
     """
 
     config_type = HDDMWConfig  # type: ignore
 
     def __init__(
         self,
         config: Optional[HDDMWConfig] = None,
-        callbacks: Optional[Union[Callback, List[Callback]]] = None,
+        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
     ) -> None:
         """Init method.
 
         :param config: configuration parameters
         :type config: Optional[HDDMWConfig]
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[Callback, List[Callback]]]
+        :type callbacks: Optional[Union[BaseCallback, List[Callback]]]
         """
         super().__init__(
             config=config,
             callbacks=callbacks,
         )
         self.additional_vars = {
             "test_type": (
```

### Comparing `frouros-0.3.0/frouros/detectors/concept_drift/streaming/statistical_process_control/rddm.py` & `frouros-0.3.1/frouros/detectors/concept_drift/streaming/statistical_process_control/rddm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """RDDM (Reactive Drift detection method) module."""
 
 from typing import List, Optional, Union
 
-from frouros.callbacks import Callback
+from frouros.callbacks.base import BaseCallback
 from frouros.detectors.concept_drift.streaming.statistical_process_control.base import (
-    SPCBaseConfig,
-    SPCErrorBase,
+    BaseSPCConfig,
+    BaseSPCError,
 )
 from frouros.utils.data_structures import CircularQueue
 from frouros.utils.stats import Mean
 
 
-class RDDMConfig(SPCBaseConfig):
+class RDDMConfig(BaseSPCConfig):
     """RDDM (Reactive Drift detection method) [barros2017rddm]_ configuration.
 
     :References:
 
     .. [barros2017rddm] Barros, Roberto SM, et al.
         "RDDM: Reactive drift detection method."
         Expert Systems with Applications 90 (2017): 344-355.
@@ -106,37 +106,37 @@
 
         :param value: value to be set
         :type value: int
         """
         self._max_num_instances_warning = value
 
 
-class RDDM(SPCErrorBase):
+class RDDM(BaseSPCError):
     """RDDM (Reactive Drift detection method) [barros2017rddm]_ detector.
 
     :References:
 
     .. [barros2017rddm] Barros, Roberto SM, et al.
         "RDDM: Reactive drift detection method."
         Expert Systems with Applications 90 (2017): 344-355.
     """
 
     config_type = RDDMConfig  # type: ignore
 
     def __init__(
         self,
         config: Optional[RDDMConfig] = None,
-        callbacks: Optional[Union[Callback, List[Callback]]] = None,
+        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
     ) -> None:
         """Init method.
 
         :param config: configuration parameters
         :type config: Optional[RDDMConfig]
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[Callback, List[Callback]]]
+        :type callbacks: Optional[Union[BaseCallback, List[Callback]]]
         """
         super().__init__(
             config=config,
             callbacks=callbacks,
         )
         self.additional_vars = {
             "num_warnings": 0,
```

### Comparing `frouros-0.3.0/frouros/detectors/concept_drift/streaming/window_based/adwin.py` & `frouros-0.3.1/frouros/detectors/concept_drift/streaming/window_based/adwin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """ADWIN (ADaptive WINdowing) module."""
 
 from collections import deque
 from typing import List, Optional, Union
 
 import numpy as np  # type: ignore
 
-from frouros.callbacks import Callback
+from frouros.callbacks.base import BaseCallback
 from frouros.detectors.concept_drift.streaming.window_based.base import (
-    WindowBaseConfig,
-    WindowBased,
+    BaseWindowConfig,
+    BaseWindow,
 )
 
 
 class Bucket:
     """Class representing a bucket."""
 
     def __init__(self, m: int) -> None:
@@ -148,15 +148,15 @@
         self.total[idx_start:self.array_size] = 0.0
         self.variance[idx_start:self.array_size] = 0.0
         # fmt: on
 
         self.idx -= num_items_deleted
 
 
-class ADWINConfig(WindowBaseConfig):
+class ADWINConfig(BaseWindowConfig):
     """ADWIN (ADaptive WINdowing) [bifet2007learning]_ configuration.
 
     :References:
 
     .. [bifet2007learning] Bifet, Albert, and Ricard Gavalda.
         "Learning from time-changing data with adaptive windowing."
         Proceedings of the 2007 SIAM international conference on data mining.
@@ -275,15 +275,15 @@
         :raises ValueError: Value error exception
         """
         if value < 1:
             raise ValueError("min_window_size value must be greater than 0.")
         self._min_window_size = value
 
 
-class ADWIN(WindowBased):
+class ADWIN(BaseWindow):
     """ADWIN (ADaptive WINdowing) [bifet2007learning]_ detector.
 
     :References:
 
     .. [bifet2007learning] Bifet, Albert, and Ricard Gavalda.
         "Learning from time-changing data with adaptive windowing."
         Proceedings of the 2007 SIAM international conference on data mining.
@@ -291,22 +291,22 @@
     """
 
     config_type = ADWINConfig
 
     def __init__(
         self,
         config: Optional[ADWINConfig] = None,
-        callbacks: Optional[Union[Callback, List[Callback]]] = None,
+        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
     ) -> None:
         """Init method.
 
         :param config: configuration parameters
         :type config: Optional[ADWINConfig]
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[Callback, List[Callback]]]
+        :type callbacks: Optional[Union[Callback, List[BaseCallback]]]
         """
         super().__init__(
             config=config,
             callbacks=callbacks,
         )
         num_buckets = 0
         self.additional_vars = {
```

### Comparing `frouros-0.3.0/frouros/detectors/concept_drift/streaming/window_based/kswin.py` & `frouros-0.3.1/frouros/detectors/concept_drift/streaming/window_based/kswin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """KSWIN (Kolmogorov-Smirnov Windowing) module."""
 
-from collections import deque
 import itertools
+from collections import deque
 from typing import List, Optional, Union
 
-from scipy.stats import ks_2samp  # type: ignore
 import numpy as np  # type: ignore
+from scipy.stats import ks_2samp  # type: ignore
 
-from frouros.callbacks import Callback
+from frouros.callbacks.base import BaseCallback
 from frouros.detectors.concept_drift.streaming.window_based.base import (
-    WindowBaseConfig,
-    WindowBased,
+    BaseWindowConfig,
+    BaseWindow,
 )
 
 
-class KSWINConfig(WindowBaseConfig):
+class KSWINConfig(BaseWindowConfig):
     """KSWIN (Kolmogorov-Smirnov Windowing) [raab2020reactive]_ configuration.
 
     :References:
 
     .. [raab2020reactive] Raab, Christoph, Moritz Heusinger, and Frank-Michael Schleif.
         "Reactive soft prototype computing for concept drift streams."
         Neurocomputing 416 (2020): 340-351.
@@ -97,37 +97,37 @@
                 "min_num_instances."
             )
         if value < 1:
             raise ValueError("num_test_instances value must be greater than 0.")
         self._num_test_instances = value
 
 
-class KSWIN(WindowBased):
+class KSWIN(BaseWindow):
     """KSWIN (Kolmogorov-Smirnov Windowing) [raab2020reactive]_ detector.
 
     :References:
 
     .. [raab2020reactive] Raab, Christoph, Moritz Heusinger, and Frank-Michael Schleif.
         "Reactive soft prototype computing for concept drift streams."
         Neurocomputing 416 (2020): 340-351.
     """
 
     config_type = KSWINConfig
 
     def __init__(
         self,
         config: Optional[KSWINConfig] = None,
-        callbacks: Optional[Union[Callback, List[Callback]]] = None,
+        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
     ) -> None:
         """Init method.
 
         :param config: configuration parameters
         :type config: Optional[KSWINConfig]
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[Callback, List[Callback]]]
+        :type callbacks: Optional[Union[BaseCallback, List[Callback]]]
         """
         super().__init__(
             config=config,
             callbacks=callbacks,
         )
         self.additional_vars = {
             "window": deque(maxlen=self.config.min_num_instances),
```

### Comparing `frouros-0.3.0/frouros/detectors/concept_drift/streaming/window_based/stepd.py` & `frouros-0.3.1/frouros/detectors/concept_drift/streaming/window_based/stepd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """STEPD (Statistical test of equal proportions) module."""
 
 from typing import List, Optional, Union
 
 import numpy as np  # type: ignore
 from scipy.stats import norm  # type: ignore
 
-from frouros.callbacks import Callback
+from frouros.callbacks.base import BaseCallback
 from frouros.detectors.concept_drift.streaming.window_based.base import (
-    WindowBaseConfig,
-    WindowBased,
+    BaseWindowConfig,
+    BaseWindow,
 )
 from frouros.utils.data_structures import AccuracyQueue
 
 
-class STEPDConfig(WindowBaseConfig):
+class STEPDConfig(BaseWindowConfig):
     """STEPD (Statistical test of equal proportions) [nishida2007detecting]_ configuration.
 
     :References:
 
     .. [nishida2007detecting] Nishida, Kyosuke, and Koichiro Yamauchi.
         "Detecting concept drift using statistical testing." Discovery science.
         Vol. 4755. 2007.
@@ -84,37 +84,37 @@
         if value <= 0.0:
             raise ValueError("alpha_w must be greater than 0.0.")
         if value <= self.alpha_d:
             raise ValueError("alpha_w must be greater than alpha_d.")
         self._alpha_w = value
 
 
-class STEPD(WindowBased):
+class STEPD(BaseWindow):
     """STEPD (Statistical test of equal proportions) [nishida2007detecting]_ detector.
 
     :References:
 
     .. [nishida2007detecting] Nishida, Kyosuke, and Koichiro Yamauchi.
         "Detecting concept drift using statistical testing." Discovery science.
         Vol. 4755. 2007.
     """
 
     config_type = STEPDConfig  # type: ignore
 
     def __init__(
         self,
         config: Optional[STEPDConfig] = None,
-        callbacks: Optional[Union[Callback, List[Callback]]] = None,
+        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
     ) -> None:
         """Init method.
 
         :param config: configuration parameters
         :type config: Optional[STEPDConfig]
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[Callback, List[Callback]]]
+        :type callbacks: Optional[Union[BaseCallback, List[Callback]]]
         """
         super().__init__(
             config=config,
             callbacks=callbacks,
         )
         self.additional_vars = {
             "correct_total": 0,
```

### Comparing `frouros-0.3.0/frouros/detectors/data_drift/__init__.py` & `frouros-0.3.1/frouros/detectors/data_drift/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.0/frouros/detectors/data_drift/base.py` & `frouros-0.3.1/frouros/detectors/data_drift/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-"""Data drift base module."""
+"""Base data drift module."""
 
 
 import abc
 import operator
 from typing import Any, Dict, List, Optional, Union
 
 import numpy as np  # type: ignore
 
-from frouros.callbacks import Callback
-from frouros.detectors.base import DetectorBase
+from frouros.callbacks.base import BaseCallback
+from frouros.detectors.base import BaseDetector
 from frouros.detectors.data_drift.exceptions import DimensionError, MissingFitError
 
 
-class ResultBase(abc.ABC):
+class BaseResult(abc.ABC):
     """Abstract class representing a result."""
 
 
-class DataTypeBase(abc.ABC):
+class BaseDataType(abc.ABC):
     """Abstract class representing a data type."""
 
     @abc.abstractmethod
     def __init__(self) -> None:
         """Init method."""
 
     def __repr__(self) -> str:
@@ -31,33 +31,33 @@
         """
         return (
             f"{self.__class__.__name__}"
             f"({', '.join(f'{k}={v}' for k, v in self.__dict__.items())})"
         )
 
 
-class CategoricalData(DataTypeBase):
+class CategoricalData(BaseDataType):
     """Class representing categorical data."""
 
     def __init__(self) -> None:
         """Init method."""
         super().__init__()
         self.output_type = None
 
 
-class NumericalData(DataTypeBase):
+class NumericalData(BaseDataType):
     """Class representing numerical data."""
 
     def __init__(self) -> None:
         """Init method."""
         super().__init__()
         self.output_type = np.float32
 
 
-class StatisticalTypeBase(abc.ABC):
+class BaseStatisticalType(abc.ABC):
     """Abstract class representing a statistical data type."""
 
     @abc.abstractmethod
     def __init__(self) -> None:
         """Init method."""
 
     def __repr__(self) -> str:
@@ -68,95 +68,95 @@
         """
         return (
             f"{self.__class__.__name__}"
             f"({', '.join(f'{k[1:]}={v}' for k, v in self.__dict__.items())})"
         )
 
 
-class UnivariateData(StatisticalTypeBase):
+class UnivariateData(BaseStatisticalType):
     """Class representing a univariate data type."""
 
     def __init__(self) -> None:
         """Init method."""
         super().__init__()
         self.dim_check = operator.eq
 
 
-class MultivariateData(StatisticalTypeBase):
+class MultivariateData(BaseStatisticalType):
     """Class representing a multivariate data type."""
 
     def __init__(self) -> None:
         """Init method."""
         super().__init__()
         self.dim_check = operator.ge
 
 
-class DataDriftBase(DetectorBase):
+class BaseDataDrift(BaseDetector):
     """Abstract class representing a data drift detector."""
 
     def __init__(
         self,
-        data_type: DataTypeBase,
-        statistical_type: StatisticalTypeBase,
-        callbacks: Optional[Union[Callback, List[Callback]]] = None,
+        data_type: BaseDataType,
+        statistical_type: BaseStatisticalType,
+        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
     ) -> None:
         """Init method.
 
         :param data_type: data type
-        :type data_type: DataTypeBase
+        :type data_type: BaseDataType
         :param statistical_type: statistical type
-        :type statistical_type: StatisticalTypeBase
+        :type statistical_type: BaseStatisticalType
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[Callback, List[Callback]]]
+        :type callbacks: Optional[Union[BaseCallback, List[Callback]]]
         """
         super().__init__(callbacks=callbacks)
         self.data_type = data_type
         self.statistical_type = statistical_type
         self.X_ref = None  # type: ignore
 
     @property
-    def data_type(self) -> DataTypeBase:
+    def data_type(self) -> BaseDataType:
         """Data type property.
 
         :return: data type
-        :rtype: DataTypeBase
+        :rtype: BaseDataType
         """
         return self._data_type
 
     @data_type.setter
-    def data_type(self, value: DataTypeBase) -> None:
+    def data_type(self, value: BaseDataType) -> None:
         """Data type setter.
 
         :param value: value to be set
-        :type value: DataTypeBase
+        :type value: BaseDataType
         :raises TypeError: Type error exception
         """
-        if not isinstance(value, DataTypeBase):
-            raise TypeError("value must be of type DataTypeBase.")
+        if not isinstance(value, BaseDataType):
+            raise TypeError("value must be of type BaseDataType.")
         self._data_type = value
 
     @property
-    def statistical_type(self) -> StatisticalTypeBase:
+    def statistical_type(self) -> BaseStatisticalType:
         """Statistical type property.
 
         :return: statistical type
-        :rtype: StatisticalTypeBase
+        :rtype: BaseStatisticalType
         """
         return self._statistical_type
 
     @statistical_type.setter
-    def statistical_type(self, value: StatisticalTypeBase) -> None:
+    def statistical_type(self, value: BaseStatisticalType) -> None:
         """Statistical type setter.
 
         :param value: value to be set
-        :type value: StatisticalTypeBase
+        :type value: BaseStatisticalType
         :raises TypeError: Type error exception
         """
-        if not isinstance(value, StatisticalTypeBase):
-            raise TypeError("value must be of type StatisticalTypeBase.")
+        if not isinstance(value, BaseStatisticalType):
+            raise TypeError("value must be of type BaseStatisticalType.")
         self._statistical_type = value
 
     @property
     def X_ref(self) -> Optional[np.ndarray]:  # noqa: N802
         """Reference data property.
 
         :return: reference data
```

### Comparing `frouros-0.3.0/frouros/detectors/data_drift/batch/__init__.py` & `frouros-0.3.1/frouros/detectors/data_drift/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.0/frouros/detectors/data_drift/batch/base.py` & `frouros-0.3.1/frouros/detectors/data_drift/batch/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-"""Data drift batch base module."""
+"""Base data drift batch module."""
 
 import abc
-
 from typing import Any, Dict, Optional, List, Tuple, Union
+
 import numpy as np  # type: ignore
 
-from frouros.callbacks import Callback
+from frouros.callbacks.base import BaseCallback
 from frouros.detectors.data_drift.base import (
-    DataDriftBase,
-    DataTypeBase,
-    StatisticalTypeBase,
+    BaseDataDrift,
+    BaseDataType,
+    BaseStatisticalType,
 )
 from frouros.detectors.data_drift.exceptions import (
     MismatchDimensionError,
 )
 
 
-class DataDriftBatchBase(DataDriftBase):
+class BaseDataDriftBatch(BaseDataDrift):
     """Abstract class representing a data drift batch detector."""
 
     def __init__(
         self,
-        data_type: DataTypeBase,
-        statistical_type: StatisticalTypeBase,
-        callbacks: Optional[Union[Callback, List[Callback]]] = None,
+        data_type: BaseDataType,
+        statistical_type: BaseStatisticalType,
+        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
     ) -> None:
         """Init method.
 
         :param data_type: data type
-        :type data_type: DataTypeBase
+        :type data_type: BaseDataType
         :param statistical_type: statistical type
-        :type statistical_type: StatisticalTypeBase
+        :type statistical_type: BaseStatisticalType
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[Callback], List[Callback]]
+        :type callbacks: Optional[Union[Callback], List[BaseCallback]]
         """
         super().__init__(
             callbacks=callbacks,
             data_type=data_type,
             statistical_type=statistical_type,
         )
         for callback in self.callbacks:  # type: ignore
```

### Comparing `frouros-0.3.0/frouros/detectors/data_drift/batch/distance_based/base.py` & `frouros-0.3.1/frouros/detectors/data_drift/batch/distance_based/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,47 @@
-"""Data drift batch distance based base module."""
+"""Base data drift batch distance based module."""
 
 import abc
 from collections import namedtuple
 from typing import Any, Callable, Dict, Optional, List, Tuple, Union
 
 import numpy as np  # type: ignore
 from scipy.stats import rv_histogram  # type: ignore
 
-from frouros.callbacks import Callback
+from frouros.callbacks.base import BaseCallback
 from frouros.detectors.data_drift.base import (
     NumericalData,
-    StatisticalTypeBase,
+    BaseStatisticalType,
     UnivariateData,
 )
-from frouros.detectors.data_drift.batch.base import DataDriftBatchBase
-
+from frouros.detectors.data_drift.batch.base import BaseDataDriftBatch
 
 DistanceResult = namedtuple("DistanceResult", ["distance"])
 
 
-class DistanceBasedBase(DataDriftBatchBase):
+class BaseDistanceBased(BaseDataDriftBatch):
     """Abstract class representing a distance based detector."""
 
     def __init__(
         self,
-        statistical_type: StatisticalTypeBase,
+        statistical_type: BaseStatisticalType,
         statistical_method: Callable,
         statistical_kwargs: Dict[str, Any],
-        callbacks: Optional[Union[Callback, List[Callback]]] = None,
+        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
     ) -> None:
         """Init method.
 
         :param statistical_type: statistical type
-        :type statistical_type: StatisticalTypeBase
+        :type statistical_type: BaseStatisticalType
         :param statistical_method: statistical method
         :type statistical_method: Callable
         :param statistical_kwargs: statistical kwargs
         :type statistical_kwargs: Dict[str, Any]
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[Callback, List[Callback]]]
+        :type callbacks: Optional[Union[BaseCallback, List[BaseCallback]]]
         """
         super().__init__(
             data_type=NumericalData(),
             statistical_type=statistical_type,
             callbacks=callbacks,
         )
         self.statistical_method = statistical_method
@@ -109,32 +108,32 @@
         X_ref: np.ndarray,  # noqa: N803
         X: np.ndarray,  # noqa: N803
         **kwargs,
     ) -> DistanceResult:
         pass
 
 
-class DistanceBinsBasedBase(DistanceBasedBase):
-    """Abstract class representing a distance bins based detector."""
+class BaseDistanceBasedBins(BaseDistanceBased):
+    """Abstract class representing a distance based bins detector."""
 
     def __init__(
         self,
         statistical_method,
         statistical_kwargs,
-        callbacks: Optional[Union[Callback, List[Callback]]] = None,
+        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
         num_bins: int = 10,
     ) -> None:
         """Init method.
 
         :param statistical_method: statistical method
         :type statistical_method: Callable
         :param statistical_kwargs: statistical kwargs
         :type statistical_kwargs: Dict[str, Any]
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[Callback, List[Callback]]]
+        :type callbacks: Optional[Union[BaseCallback, List[Callback]]]
         :param num_bins: number of bins in which to divide probabilities
         :type num_bins: int
         """
         super().__init__(
             statistical_type=UnivariateData(),
             statistical_method=statistical_method,
             statistical_kwargs={**statistical_kwargs, "num_bins": num_bins},
@@ -191,32 +190,32 @@
         self,
         X_ref: np.ndarray,  # noqa: N803
         X: np.ndarray,  # noqa: N803
     ) -> float:
         pass
 
 
-class DistanceProbabilityBasedBase(DistanceBasedBase):
-    """Abstract class representing a distance probability based detector."""
+class BaseDistanceBasedProbability(BaseDistanceBased):
+    """Abstract class representing a distance based probability detector."""
 
     def __init__(
         self,
         statistical_method,
         statistical_kwargs,
-        callbacks: Optional[Union[Callback, List[Callback]]] = None,
+        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
         num_bins: int = 10,
     ) -> None:
         """Init method.
 
         :param statistical_method: statistical method
         :type statistical_method: Callable
         :param statistical_kwargs: statistical kwargs
         :type statistical_kwargs: Dict[str, Any]
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[Callback, List[Callback]]]
+        :type callbacks: Optional[Union[Callback, List[BaseCallback]]]
         :param num_bins: number of bins in which to divide probabilities
         :type num_bins: int
         """
         super().__init__(
             statistical_type=UnivariateData(),
             statistical_method=statistical_method,
             statistical_kwargs=statistical_kwargs,
```

### Comparing `frouros-0.3.0/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py` & `frouros-0.3.1/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """Bhattacharyya distance module."""
 
 from typing import List, Optional, Union
 
 import numpy as np  # type: ignore
 
-from frouros.callbacks import Callback
+from frouros.callbacks.base import BaseCallback
 from frouros.detectors.data_drift.batch.distance_based.base import (
-    DistanceBinsBasedBase,
+    BaseDistanceBasedBins,
 )
 
 
-class BhattacharyyaDistance(DistanceBinsBasedBase):
+class BhattacharyyaDistance(BaseDistanceBasedBins):
     """Bhattacharyya distance [bhattacharyya1946measure]_ detector.
 
     :References:
 
     .. [bhattacharyya1946measure] Bhattacharyya, Anil.
         "On a measure of divergence between two multinomial populations."
         Sankhyā: the indian journal of statistics (1946): 401-406.
     """
 
     def __init__(
         self,
         num_bins: int = 10,
-        callbacks: Optional[Union[Callback, List[Callback]]] = None,
+        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
     ) -> None:
         """Init method.
 
         :param num_bins: number of bins in which to divide probabilities
         :type num_bins: int
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[Callback, List[Callback]]]
+        :type callbacks: Optional[Union[BaseCallback, List[Callback]]]
         """
         super().__init__(
             statistical_method=self._bhattacharyya,
             statistical_kwargs={
                 "num_bins": num_bins,
             },
             callbacks=callbacks,
@@ -52,12 +52,12 @@
     @staticmethod
     def _bhattacharyya(
         X: np.ndarray, Y: np.ndarray, *, num_bins: int  # noqa: N803
     ) -> float:
         (  # noqa: N806
             X_percents,
             Y_percents,
-        ) = DistanceBinsBasedBase._calculate_bins_values(
+        ) = BaseDistanceBasedBins._calculate_bins_values(
             X_ref=X, X=Y, num_bins=num_bins
         )
         bhattacharyya = 1 - np.sum(np.sqrt(X_percents * Y_percents))
         return bhattacharyya
```

### Comparing `frouros-0.3.0/frouros/detectors/data_drift/batch/distance_based/emd.py` & `frouros-0.3.1/frouros/detectors/data_drift/batch/distance_based/emd.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """EMD (Earth Mover's Distance) module."""
 
 from typing import List, Optional, Union
 
 import numpy as np  # type: ignore
 from scipy.stats import wasserstein_distance  # type: ignore
 
-from frouros.callbacks import Callback
+from frouros.callbacks.base import BaseCallback
 from frouros.detectors.data_drift.base import UnivariateData
 from frouros.detectors.data_drift.batch.distance_based.base import (
-    DistanceBasedBase,
+    BaseDistanceBased,
     DistanceResult,
 )
 
 
-class EMD(DistanceBasedBase):
+class EMD(BaseDistanceBased):
     """EMD (Earth Mover's Distance) [rubner2000earth]_ detector.
 
     :References:
 
     .. [rubner2000earth] Rubner, Yossi, Carlo Tomasi, and Leonidas J. Guibas.
         "The earth mover's distance as a metric for image retrieval."
         International journal of computer vision 40.2 (2000): 99.
     """
 
     def __init__(
         self,
-        callbacks: Optional[Union[Callback, List[Callback]]] = None,
+        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
         **kwargs,
     ) -> None:
         """Init method.
 
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[Callback, List[Callback]]]
+        :type callbacks: Optional[Union[BaseCallback, List[Callback]]]
         """
         super().__init__(
             statistical_type=UnivariateData(),
             statistical_method=self._emd,
             statistical_kwargs=kwargs,
             callbacks=callbacks,
         )
```

### Comparing `frouros-0.3.0/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py` & `frouros-0.3.1/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """Hellinger distance module."""
 
 from typing import List, Optional, Union
 
 import numpy as np  # type: ignore
 
-from frouros.callbacks import Callback
+from frouros.callbacks.base import BaseCallback
 from frouros.detectors.data_drift.batch.distance_based.base import (
-    DistanceBinsBasedBase,
+    BaseDistanceBasedBins,
 )
 
 
-class HellingerDistance(DistanceBinsBasedBase):
+class HellingerDistance(BaseDistanceBasedBins):
     """Hellinger distance [hellinger1909neue]_ detector.
 
     :References:
 
     .. [hellinger1909neue] Hellinger, Ernst.
         "Neue begründung der theorie quadratischer formen von unendlichvielen
         veränderlichen."
         Journal für die reine und angewandte Mathematik 1909.136 (1909): 210-271.
     """
 
     def __init__(
         self,
         num_bins: int = 10,
-        callbacks: Optional[Union[Callback, List[Callback]]] = None,
+        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
     ) -> None:
         """Init method.
 
         :param num_bins: number of bins in which to divide probabilities
         :type num_bins: int
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[Callback, List[Callback]]]
+        :type callbacks: Optional[Union[Callback, List[BaseCallback]]]
         """
         sqrt_div = np.sqrt(2)
         super().__init__(
             statistical_method=self._hellinger,
             statistical_kwargs={
                 "num_bins": num_bins,
                 "sqrt_div": sqrt_div,
@@ -61,14 +61,14 @@
     @staticmethod
     def _hellinger(
         X: np.ndarray, Y: np.ndarray, *, num_bins: int, sqrt_div: float  # noqa: N803
     ) -> float:
         (  # noqa: N806
             X_percents,
             Y_percents,
-        ) = DistanceBinsBasedBase._calculate_bins_values(
+        ) = BaseDistanceBasedBins._calculate_bins_values(
             X_ref=X, X=Y, num_bins=num_bins
         )
         hellinger = (
             np.sqrt(np.sum((np.sqrt(X_percents) - np.sqrt(Y_percents)) ** 2)) / sqrt_div
         )
         return hellinger
```

### Comparing `frouros-0.3.0/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py` & `frouros-0.3.1/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """HI (Histogram intersection) normalized complement module."""
 
 from typing import List, Optional, Union
 
 import numpy as np  # type: ignore
 
-from frouros.callbacks import Callback
+from frouros.callbacks.base import BaseCallback
 from frouros.detectors.data_drift.batch.distance_based.base import (
-    DistanceBinsBasedBase,
+    BaseDistanceBasedBins,
 )
 
 
-class HINormalizedComplement(DistanceBinsBasedBase):
+class HINormalizedComplement(BaseDistanceBasedBins):
     """HI (Histogram intersection) normalized complement [swain1991color]_ detector.
 
     :References:
 
     .. [swain1991color] Swain, M. J., and D. H. Ballard.
         "Color Indexing International Journal of Computer
         Vision 7." (1991): 11-32.
     """
 
     def __init__(
         self,
         num_bins: int = 10,
-        callbacks: Optional[Union[Callback, List[Callback]]] = None,
+        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
     ) -> None:
         """Init method.
 
         :param num_bins: number of bins in which to divide probabilities
         :type num_bins: int
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[Callback, List[Callback]]]
+        :type callbacks: Optional[Union[BaseCallback, List[Callback]]]
         """
         super().__init__(
             statistical_method=self._hi_normalized_complement,
             statistical_kwargs={
                 "num_bins": num_bins,
             },
             callbacks=callbacks,
```

### Comparing `frouros-0.3.0/frouros/detectors/data_drift/batch/distance_based/js.py` & `frouros-0.3.1/frouros/detectors/data_drift/batch/distance_based/js.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 """JS (Jensen-Shannon distance) module."""
 
 from typing import Any, Dict, List, Optional, Union
 
 import numpy as np  # type: ignore
 from scipy.spatial.distance import jensenshannon  # type: ignore
 
-from frouros.callbacks import Callback
+from frouros.callbacks.base import BaseCallback
 from frouros.detectors.data_drift.batch.distance_based.base import (
-    DistanceProbabilityBasedBase,
+    BaseDistanceBasedProbability,
     DistanceResult,
 )
 
 
-class JS(DistanceProbabilityBasedBase):
+class JS(BaseDistanceBasedProbability):
     """JS (Jensen-Shannon distance) [lin1991divergence]_ detector.
 
     :References:
 
     .. [lin1991divergence] Lin, Jianhua.
         "Divergence measures based on the Shannon entropy."
         IEEE Transactions on Information theory 37.1 (1991): 145-151.
     """
 
     def __init__(
         self,
         num_bins: int = 10,
-        callbacks: Optional[Union[Callback, List[Callback]]] = None,
+        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
         **kwargs,
     ) -> None:
         """Init method.
 
         :param num_bins: number of bins in which to divide probabilities
         :type num_bins: int
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[Callback, List[Callback]]]
+        :type callbacks: Optional[Union[BaseCallback, List[BaseCallback]]]
         """
         super().__init__(
             statistical_method=self._js,
             statistical_kwargs={
                 "num_bins": num_bins,
                 **kwargs,
             },
@@ -63,14 +63,14 @@
         *,
         num_bins: int,
         **kwargs: Dict[str, Any],
     ) -> float:
         (  # noqa: N806
             X_ref_rvs,
             X_rvs,
-        ) = DistanceProbabilityBasedBase._calculate_probabilities(
+        ) = BaseDistanceBasedProbability._calculate_probabilities(
             X_ref=X,
             X=Y,
             num_bins=num_bins,
         )
         js = jensenshannon(p=X_ref_rvs, q=X_rvs, **kwargs)
         return js
```

### Comparing `frouros-0.3.0/frouros/detectors/data_drift/batch/distance_based/kl.py` & `frouros-0.3.1/frouros/detectors/data_drift/batch/distance_based/kl.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 """KL (Kullback-Leibler divergence distance) module."""
 
 from typing import Any, Dict, List, Optional, Union
 
 import numpy as np  # type: ignore
 from scipy.special import rel_entr  # type: ignore
 
-from frouros.callbacks import Callback
+from frouros.callbacks.base import BaseCallback
 from frouros.detectors.data_drift.batch.distance_based.base import (
-    DistanceProbabilityBasedBase,
+    BaseDistanceBasedProbability,
     DistanceResult,
 )
 
 
-class KL(DistanceProbabilityBasedBase):
+class KL(BaseDistanceBasedProbability):
     """KL (Kullback-Leibler divergence) [kullback1951information]_ detector.
 
     :References:
 
     .. [kullback1951information] Kullback, Solomon, and Richard A. Leibler.
         "On information and sufficiency."
         The annals of mathematical statistics 22.1 (1951): 79-86.
     """
 
     def __init__(
         self,
         num_bins: int = 10,
-        callbacks: Optional[Union[Callback, List[Callback]]] = None,
+        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
         **kwargs,
     ) -> None:
         """Init method.
 
         :param num_bins: number of bins in which to divide probabilities
         :type num_bins: int
         :param callbacks: number of bins in which to divide probabilities
-        :type callbacks: Optional[Union[Callback, List[Callback]]]
+        :type callbacks: Optional[Union[BaseCallback, List[Callback]]]
         """
         super().__init__(
             statistical_method=self._kl,
             statistical_kwargs={**kwargs, "num_bins": num_bins},
             callbacks=callbacks,
         )
         self.num_bins = num_bins
@@ -60,14 +60,14 @@
         *,
         num_bins: int,
         **kwargs: Dict[str, Any],
     ) -> float:
         (  # noqa: N806
             X_ref_rvs,
             X_rvs,
-        ) = DistanceProbabilityBasedBase._calculate_probabilities(
+        ) = BaseDistanceBasedProbability._calculate_probabilities(
             X_ref=X,
             X=Y,
             num_bins=num_bins,
         )
         kl = np.sum(rel_entr(X_rvs, X_ref_rvs, **kwargs))
         return kl
```

### Comparing `frouros-0.3.0/frouros/detectors/data_drift/batch/distance_based/mmd.py` & `frouros-0.3.1/frouros/detectors/data_drift/batch/distance_based/mmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 import math
 from typing import Callable, Generator, Optional, List, Union
 
 import numpy as np  # type: ignore
 import tqdm  # type: ignore
 from scipy.spatial.distance import cdist  # type: ignore
 
-from frouros.callbacks import Callback
+from frouros.callbacks.base import BaseCallback
 from frouros.detectors.data_drift.base import MultivariateData
 from frouros.detectors.data_drift.batch.distance_based.base import (
-    DistanceBasedBase,
+    BaseDistanceBased,
     DistanceResult,
 )
 
 
 def rbf_kernel(
     X: np.ndarray, Y: np.ndarray, std: float = 1.0  # noqa: N803
 ) -> np.ndarray:
@@ -29,38 +29,38 @@
     :type std: float
     :return: Radial basis kernel matrix
     :rtype: numpy.ndarray
     """
     return np.exp(-cdist(X, Y, "sqeuclidean") / 2 * std**2)
 
 
-class MMD(DistanceBasedBase):
+class MMD(BaseDistanceBased):
     """MMD (Maximum Mean Discrepancy) [gretton2012kernel]_ detector.
 
     :References:
 
     .. [gretton2012kernel] Gretton, Arthur, et al.
         "A kernel two-sample test."
         The Journal of Machine Learning Research 13.1 (2012): 723-773.
     """
 
     def __init__(
         self,
         kernel: Callable = rbf_kernel,
         chunk_size: Optional[int] = None,
-        callbacks: Optional[Union[Callback, List[Callback]]] = None,
+        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
     ) -> None:
         """Init method.
 
         :param kernel: kernel function
         :type kernel: Callable
         :param chunk_size: chunk size value
         :type chunk_size: Optional[int]
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[Callback, List[Callback]]]
+        :type callbacks: Optional[Union[BaseCallback, List[BaseCallback]]]
         """
         super().__init__(
             statistical_type=MultivariateData(),
             statistical_method=self._mmd,
             statistical_kwargs={
                 "kernel": kernel,
             },
```

### Comparing `frouros-0.3.0/frouros/detectors/data_drift/batch/distance_based/psi.py` & `frouros-0.3.1/frouros/detectors/data_drift/batch/distance_based/psi.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """PSI (Population Stability Index) module."""
 
 import sys
-
 from typing import List, Optional, Union
+
 import numpy as np  # type: ignore
 
-from frouros.callbacks import Callback
+from frouros.callbacks.base import BaseCallback
 from frouros.detectors.data_drift.batch.distance_based.base import (
-    DistanceBinsBasedBase,
+    BaseDistanceBasedBins,
     DistanceResult,
 )
 
 
-class PSI(DistanceBinsBasedBase):
+class PSI(BaseDistanceBasedBins):
     """PSI (Population Stability Index) [wu2010enterprise]_ detector.
 
     :References:
 
     .. [wu2010enterprise] Wu, Desheng, and David L. Olson.
         "Enterprise risk management: coping with model risk in a large bank."
         Journal of the Operational Research Society 61.2 (2010): 179-190.
     """
 
     def __init__(
         self,
         num_bins: int = 10,
-        callbacks: Optional[Union[Callback, List[Callback]]] = None,
+        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
     ) -> None:
         """Init method.
 
         :param num_bins: number of bins in which to divide probabilities
         :type num_bins: int
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[Callback, List[Callback]]]
+        :type callbacks: Optional[Union[Callback, List[BaseCallback]]]
         """
         super().__init__(
             statistical_method=self._psi,
             statistical_kwargs={
                 "num_bins": num_bins,
             },
             callbacks=callbacks,
@@ -62,15 +62,15 @@
         X: np.ndarray,  # noqa: N803
         Y: np.ndarray,  # noqa: N803
         num_bins: int,
     ) -> float:
         (  # noqa: N806
             X_percents,
             Y_percents,
-        ) = DistanceBinsBasedBase._calculate_bins_values(
+        ) = BaseDistanceBasedBins._calculate_bins_values(
             X_ref=X, X=Y, num_bins=num_bins
         )
         # Replace 0.0 values with the smallest number possible
         # in order to avoid division by zero
         X_percents[X_percents == 0.0] = sys.float_info.min
         Y_percents[Y_percents == 0.0] = sys.float_info.min
         psi = np.sum((Y_percents - X_percents) * np.log(Y_percents / X_percents))
```

### Comparing `frouros-0.3.0/frouros/detectors/data_drift/batch/statistical_test/base.py` & `frouros-0.3.1/frouros/detectors/data_drift/batch/statistical_test/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-"""Data drift statistical test base module."""
+"""Base data drift statistical test module."""
 
 import abc
 from collections import namedtuple
 from typing import Tuple
 
 import numpy as np  # type: ignore
 
-from frouros.detectors.data_drift.batch.base import DataDriftBatchBase
-
+from frouros.detectors.data_drift.batch.base import BaseDataDriftBatch
 
 StatisticalResult = namedtuple("StatisticalResult", ["statistic", "p_value"])
 
 
-class StatisticalTestBase(DataDriftBatchBase):
+class BaseStatisticalTest(BaseDataDriftBatch):
     """Abstract class representing a statistical test."""
 
     def _apply_method(
         self, X_ref: np.ndarray, X: np.ndarray, **kwargs  # noqa: N803
     ) -> Tuple[float, float]:
         statistical_test = self._statistical_test(X_ref=X_ref, X=X, **kwargs)
         return statistical_test
```

### Comparing `frouros-0.3.0/frouros/detectors/data_drift/batch/statistical_test/chisquare.py` & `frouros-0.3.1/frouros/detectors/data_drift/batch/statistical_test/chisquare.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,42 +2,42 @@
 
 import collections
 from typing import Optional, List, Tuple, Union
 
 import numpy as np  # type: ignore
 from scipy.stats import chi2_contingency  # type: ignore
 
-from frouros.callbacks import Callback
+from frouros.callbacks.base import BaseCallback
 from frouros.detectors.data_drift.base import CategoricalData, UnivariateData
 from frouros.detectors.data_drift.batch.statistical_test.base import (  # type: ignore
-    StatisticalTestBase,
+    BaseStatisticalTest,
     StatisticalResult,
 )
 
 
-class ChiSquareTest(StatisticalTestBase):
+class ChiSquareTest(BaseStatisticalTest):
     """ChiSquareTest (Chi-square test) [pearson1900x]_ detector.
 
     :References:
 
     .. [pearson1900x] Pearson, Karl.
         "X. On the criterion that a given system of deviations from the probable in the
         case of a correlated system of variables is such that it can be reasonably
         supposed to have arisen from random sampling."
         The London, Edinburgh, and Dublin Philosophical Magazine and Journal of
         Science 50.302 (1900): 157-175.
     """
 
     def __init__(
-        self, callbacks: Optional[Union[Callback, List[Callback]]] = None
+        self, callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None
     ) -> None:
         """Init method.
 
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[Callback, List[Callback]]]
+        :type callbacks: Optional[Union[Callback, List[BaseCallback]]]
         """
         super().__init__(
             data_type=CategoricalData(),
             statistical_type=UnivariateData(),
             callbacks=callbacks,
         )
```

### Comparing `frouros-0.3.0/frouros/detectors/data_drift/batch/statistical_test/cvm.py` & `frouros-0.3.1/frouros/detectors/data_drift/batch/statistical_test/cvm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 """CVMTest (Cramér-von Mises test) module."""
 
 from typing import Optional, List, Union
 
 import numpy as np  # type: ignore
 from scipy.stats import cramervonmises_2samp  # type: ignore
 
-from frouros.callbacks import Callback
+from frouros.callbacks.base import BaseCallback
 from frouros.detectors.data_drift.base import NumericalData, UnivariateData
-from frouros.detectors.data_drift.exceptions import InsufficientSamplesError
 from frouros.detectors.data_drift.batch.statistical_test.base import (
-    StatisticalTestBase,
+    BaseStatisticalTest,
     StatisticalResult,
 )
+from frouros.detectors.data_drift.exceptions import InsufficientSamplesError
 
 
-class CVMTest(StatisticalTestBase):
+class CVMTest(BaseStatisticalTest):
     """CVMTest (Cramér-von Mises test) [cramer1928composition]_ detector.
 
     :References:
 
     .. [cramer1928composition] Cramér, Harald.
         "On the composition of elementary errors: First paper: Mathematical deductions."
         Scandinavian Actuarial Journal 1928.1 (1928): 13-74.
     """
 
     def __init__(
-        self, callbacks: Optional[Union[Callback, List[Callback]]] = None
+        self, callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None
     ) -> None:
         """Init method.
 
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[Callback, List[Callback]]]
+        :type callbacks: Optional[Union[Callback, List[BaseCallback]]]
         """
         super().__init__(
             data_type=NumericalData(),
             statistical_type=UnivariateData(),
             callbacks=callbacks,
         )
 
-    @StatisticalTestBase.X_ref.setter  # type: ignore[attr-defined]
+    @BaseStatisticalTest.X_ref.setter  # type: ignore[attr-defined]
     def X_ref(self, value: Optional[np.ndarray]) -> None:  # noqa: N802
         """Reference data setter.
 
         :param value: value to be set
         :type value: Optional[numpy.ndarray]
         """
         if value is not None:
```

### Comparing `frouros-0.3.0/frouros/detectors/data_drift/batch/statistical_test/ks.py` & `frouros-0.3.1/frouros/detectors/data_drift/batch/statistical_test/ks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 """KSTest (Kolmogorov-Smirnov test) module."""
 
 from typing import Optional, List, Union
 
 import numpy as np  # type: ignore
 from scipy.stats import ks_2samp  # type: ignore
 
-from frouros.callbacks import Callback
+from frouros.callbacks.base import BaseCallback
 from frouros.detectors.data_drift.base import NumericalData, UnivariateData
 from frouros.detectors.data_drift.batch.statistical_test.base import (
-    StatisticalTestBase,
+    BaseStatisticalTest,
     StatisticalResult,
 )
 
 
-class KSTest(StatisticalTestBase):
+class KSTest(BaseStatisticalTest):
     """KSTest (Kolmogorov-Smirnov test) [massey1951kolmogorov]_ detector.
 
     :References:
 
     .. [massey1951kolmogorov] Massey Jr, Frank J.
         "The Kolmogorov-Smirnov test for goodness of fit."
         Journal of the American statistical Association 46.253 (1951): 68-78.
     """
 
     def __init__(
-        self, callbacks: Optional[Union[Callback, List[Callback]]] = None
+        self, callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None
     ) -> None:
         """Init method.
 
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[Callback, List[Callback]]]
+        :type callbacks: Optional[Union[BaseCallback, List[Callback]]]
         """
         super().__init__(
             data_type=NumericalData(),
             statistical_type=UnivariateData(),
             callbacks=callbacks,
         )
```

### Comparing `frouros-0.3.0/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py` & `frouros-0.3.1/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """Welch's T-test module."""
 
 from typing import Optional, List, Union
 
 import numpy as np  # type: ignore
 from scipy.stats import ttest_ind  # type: ignore
 
-from frouros.callbacks import Callback
+from frouros.callbacks.base import BaseCallback
 from frouros.detectors.data_drift.base import NumericalData, UnivariateData
 from frouros.detectors.data_drift.batch.statistical_test.base import (
-    StatisticalTestBase,
+    BaseStatisticalTest,
     StatisticalResult,
 )
 
 
-class WelchTTest(StatisticalTestBase):
+class WelchTTest(BaseStatisticalTest):
     """Welch's T-test [welch1947generalization]_ detector.
 
     :References:
 
     .. [welch1947generalization] Welch, Bernard L.
         "The generalization of ‘STUDENT'S’problem when several different population
         varlances are involved."
         Biometrika 34.1-2 (1947): 28-35.
     """
 
     def __init__(
-        self, callbacks: Optional[Union[Callback, List[Callback]]] = None
+        self, callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None
     ) -> None:
         """Init method.
 
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[Callback, List[Callback]]]
+        :type callbacks: Optional[Union[Callback, List[BaseCallback]]]
         """
         super().__init__(
             data_type=NumericalData(),
             statistical_type=UnivariateData(),
             callbacks=callbacks,
         )
```

### Comparing `frouros-0.3.0/frouros/detectors/data_drift/streaming/base.py` & `frouros-0.3.1/frouros/detectors/data_drift/streaming/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-"""Data drift batch base module."""
+"""Base data drift batch module."""
 
 import abc
-
 from typing import Any, Dict, Optional, List, Tuple, Union
+
 import numpy as np  # type: ignore
 
-from frouros.callbacks import Callback
+from frouros.callbacks.base import BaseCallback
 from frouros.detectors.data_drift.base import (
-    DataDriftBase,
-    DataTypeBase,
-    ResultBase,
-    StatisticalTypeBase,
+    BaseDataDrift,
+    BaseDataType,
+    BaseResult,
+    BaseStatisticalType,
 )
 
 
-class DataDriftStreamingBase(DataDriftBase):
+class BaseDataDriftStreaming(BaseDataDrift):
     """Abstract class representing a data drift streaming detector."""
 
     def __init__(
         self,
-        data_type: DataTypeBase,
-        statistical_type: StatisticalTypeBase,
-        callbacks: Optional[Union[Callback, List[Callback]]] = None,
+        data_type: BaseDataType,
+        statistical_type: BaseStatisticalType,
+        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
     ) -> None:
         """Init method.
 
         :param data_type: data type
-        :type data_type: DataTypeBase
+        :type data_type: BaseDataType
         :param statistical_type: statistical type
-        :type statistical_type: StatisticalTypeBase
+        :type statistical_type: BaseStatisticalType
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[Callback], List[Callback]]
+        :type callbacks: Optional[Union[Callback], List[BaseCallback]]
         """
         super().__init__(
             callbacks=callbacks,
             data_type=data_type,
             statistical_type=statistical_type,
         )
         self.num_instances = 0
@@ -45,21 +45,21 @@
         """Reset method."""
         super().reset()
         self.num_instances = 0
         self._reset()
 
     def update(
         self, value: Union[int, float]
-    ) -> Tuple[Optional[ResultBase], Dict[str, Any]]:
+    ) -> Tuple[Optional[BaseResult], Dict[str, Any]]:
         """Update detector.
 
         :param value: value to use to update the detector
         :type value: Union[int, float]
         :return: update result
-        :rtype: Optional[ResultBase]
+        :rtype: Optional[BaseResult]
         """
         self._common_checks()  # noqa: N806
         self._specific_checks(X=value)  # noqa: N806
         self.num_instances += 1
 
         for callback in self.callbacks:  # type: ignore
             callback.on_update_start(value=value)  # type: ignore
@@ -81,9 +81,9 @@
         pass
 
     @abc.abstractmethod
     def _reset(self) -> None:
         pass
 
     @abc.abstractmethod
-    def _update(self, value: Union[int, float]) -> Optional[ResultBase]:
+    def _update(self, value: Union[int, float]) -> Optional[BaseResult]:
         pass
```

### Comparing `frouros-0.3.0/frouros/detectors/data_drift/streaming/distance_based/base.py` & `frouros-0.3.1/frouros/detectors/data_drift/streaming/distance_based/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-"""Data drift distance based base module."""
+"""Base data drift distance based module."""
 
 import abc
 from typing import Any, Dict, Optional, Tuple, Union
 
 import numpy as np  # type: ignore
 
-from frouros.detectors.data_drift.base import ResultBase
+from frouros.detectors.data_drift.base import BaseResult
 from frouros.detectors.data_drift.streaming.base import (
-    DataDriftStreamingBase,
+    BaseDataDriftStreaming,
 )
 
 
-class DistanceResult(ResultBase):
+class DistanceResult(BaseResult):
     """Distance result class."""
 
     def __init__(
         self,
         distance: Union[int, float],
     ) -> None:
         """Init method.
@@ -41,15 +41,15 @@
 
         :param value: value to be set
         :type value: Union[int, float]
         """
         self._distance = value
 
 
-class DistanceBasedBase(DataDriftStreamingBase):
+class BaseDistanceBased(BaseDataDriftStreaming):
     """Abstract class representing a distance based."""
 
     @abc.abstractmethod
     def _fit(self, X: np.ndarray) -> None:  # noqa: N803
         pass
 
     @abc.abstractmethod
```

### Comparing `frouros-0.3.0/frouros/detectors/data_drift/streaming/statistical_test/base.py` & `frouros-0.3.1/frouros/detectors/data_drift/streaming/statistical_test/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Data drift statistical test base module."""
 
 import abc
 from typing import Optional, Union
 
 import numpy as np  # type: ignore
 
-from frouros.detectors.data_drift.base import ResultBase
+from frouros.detectors.data_drift.base import BaseResult
 from frouros.detectors.data_drift.streaming.base import (
-    DataDriftStreamingBase,
+    BaseDataDriftStreaming,
 )
 
 
-class StatisticalResult(ResultBase):
+class StatisticalResult(BaseResult):
     """Statistical result class."""
 
     def __init__(
         self,
         statistic: Union[int, float],
         p_value: Union[int, float],
     ) -> None:
@@ -65,15 +65,15 @@
         :type value: Union[int, float]
         """
         if not 0 <= value <= 1:
             raise ValueError("p-value must be between 0 and 1.")
         self._p_value = value
 
 
-class StatisticalTestBase(DataDriftStreamingBase):
+class BaseStatisticalTest(BaseDataDriftStreaming):
     """Abstract class representing a statistical test."""
 
     @abc.abstractmethod
     def _fit(self, X: np.ndarray) -> None:  # noqa: N803
         pass
 
     @abc.abstractmethod
```

### Comparing `frouros-0.3.0/frouros/detectors/data_drift/streaming/statistical_test/ks.py` & `frouros-0.3.1/frouros/detectors/data_drift/streaming/statistical_test/ks.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,55 +3,55 @@
 # FIXME: There seem to be a bug on the treap DS. Uncomment all  # pylint: disable=fixme
 #  the commented code lines when that is solved.
 
 # from copy import deepcopy
 from typing import Optional, List, Union
 
 import numpy as np  # type: ignore
-from scipy.stats.distributions import kstwo  # type: ignore
 from scipy.stats._stats_py import (  # type: ignore
     _compute_prob_outside_square,
     _compute_outer_prob_inside_method,
 )
+from scipy.stats.distributions import kstwo  # type: ignore
 
-from frouros.callbacks import Callback
+from frouros.callbacks.base import BaseCallback
 from frouros.detectors.data_drift.base import NumericalData, UnivariateData
 from frouros.detectors.data_drift.streaming.statistical_test.base import (
-    StatisticalTestBase,
+    BaseStatisticalTest,
     StatisticalResult,
 )
 from frouros.utils.data_structures import CircularQueue
 
 # from frouros.utils.data_structures import Treap
 
 # Value used in scipy
 MAX_AUTO_N = 10000
 
 
-class IncrementalKSTest(StatisticalTestBase):
+class IncrementalKSTest(BaseStatisticalTest):
     """IncrementalKSTest (Incremental Kolmogorov-Smirnov test) [dos2016fast]_ detector.
 
     :References:
 
     .. [dos2016fast] dos Reis, Denis Moreira, et al.
         "Fast unsupervised online drift detection using incremental kolmogorov-smirnov
         test."
         Proceedings of the 22nd ACM SIGKDD international conference on knowledge
         discovery and data mining. 2016.
     """
 
     def __init__(
         self,
-        callbacks: Optional[Union[Callback, List[Callback]]] = None,
+        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
         window_size: int = 10,
     ) -> None:
         """Init method.
 
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[Callback, List[Callback]]]
+        :type callbacks: Optional[Union[BaseCallback, List[Callback]]]
         :param window_size: window size
         :type window_size: int
         """
         super().__init__(
             data_type=NumericalData(),
             statistical_type=UnivariateData(),
             callbacks=callbacks,
```

### Comparing `frouros-0.3.0/frouros/metrics/base.py` & `frouros-0.3.1/frouros/metrics/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Metrics base module."""
+"""Base metrics module."""
 
 import abc
 from typing import Optional
 
 
 class BaseMetric(abc.ABC):
     """Abstract class representing a metric."""
```

### Comparing `frouros-0.3.0/frouros/metrics/prequential_error.py` & `frouros-0.3.1/frouros/metrics/prequential_error.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.0/frouros/tests/conftest.py` & `frouros-0.3.1/frouros/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.0/frouros/tests/integration/test_callback.py` & `frouros-0.3.1/frouros/tests/integration/test_callback.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,32 +25,32 @@
     HDDMA,
     HDDMW,
     KSWIN,
     PageHinkley,
     RDDM,
     STEPD,
 )
-from frouros.detectors.concept_drift.base import ConceptDriftBase
+from frouros.detectors.concept_drift.base import BaseConceptDrift
 from frouros.detectors.concept_drift.streaming.statistical_process_control.base import (
-    SPCBase,
+    BaseSPC,
 )
 from frouros.detectors.data_drift.batch import (
     BhattacharyyaDistance,
     CVMTest,
     EMD,
     HellingerDistance,
     HINormalizedComplement,
     JS,
     KL,
     KSTest,
     MMD,
     PSI,
     WelchTTest,
 )
-from frouros.detectors.data_drift.batch.base import DataDriftBatchBase
+from frouros.detectors.data_drift.batch.base import BaseDataDriftBatch
 from frouros.detectors.data_drift.streaming import MMD as MMDStreaming  # noqa: N811
 
 
 @pytest.mark.parametrize(
     "detector_class, expected_distance, expected_p_value",
     [
         (BhattacharyyaDistance, 0.55516059, 0.0),
@@ -62,26 +62,26 @@
         (MMD, 0.69509004, 2.53277069e-137),
         (PSI, 461.20379435, 4.45088795e-238),
     ],
 )
 def test_batch_permutation_test_data_univariate_different_distribution(
     X_ref_univariate: np.ndarray,  # noqa: N803
     X_test_univariate: np.ndarray,
-    detector_class: DataDriftBatchBase,
+    detector_class: BaseDataDriftBatch,
     expected_distance: float,
     expected_p_value: float,
 ) -> None:
     """Test batch permutation test on data callback.
 
     :param X_ref_univariate: reference univariate data
     :type X_ref_univariate: numpy.ndarray
     :param X_test_univariate: test univariate data
     :type X_test_univariate: numpy.ndarray
     :param detector_class: detector distance
-    :type detector_class: DataDriftBatchBase
+    :type detector_class: BaseDataDriftBatch
     :param expected_distance: expected distance value
     :type expected_distance: float
     :param expected_p_value: expected p-value value
     :type expected_p_value: float
     """
     np.random.seed(seed=31)
 
@@ -110,27 +110,27 @@
 @pytest.mark.parametrize(
     "detector_class",
     [CVMTest, KSTest, WelchTTest],
 )
 def test_batch_reset_on_data_drift(
     X_ref_univariate,  # noqa: N803
     X_test_univariate,
-    detector_class: DataDriftBatchBase,
+    detector_class: BaseDataDriftBatch,
     mocker,
 ) -> None:
     """Test batch reset on data drift callback.
 
     :param X_ref_univariate: reference univariate data
     :type X_ref_univariate: numpy.ndarray
     :param X_test_univariate: test univariate data
     :type X_test_univariate: numpy.ndarray
     :param detector_class: detector distance
-    :type detector_class: DataDriftBatchBase
+    :type detector_class: BaseDataDriftBatch
     """
-    mocker.patch("frouros.detectors.data_drift.batch.base.DataDriftBatchBase.reset")
+    mocker.patch("frouros.detectors.data_drift.batch.base.BaseDataDriftBatch.reset")
 
     detector = detector_class(  # type: ignore
         callbacks=[
             ResetOnBatchDataDrift(
                 alpha=0.01,
             ),
         ],
@@ -155,22 +155,22 @@
         PageHinkley,
         RDDM,
         STEPD,
     ],
 )
 def test_streaming_history_on_concept_drift(
     model_errors: List[int],
-    detector_class: ConceptDriftBase,
+    detector_class: BaseConceptDrift,
 ):
     """Test streaming history on concept drift callback.
 
     :param model_errors: model errors
     :type model_errors: List[int]
     :param detector_class: concept drift detector
-    :type detector_class: ConceptDriftBase
+    :type detector_class: BaseConceptDrift
     """
     name = "history"
     detector = detector_class(callbacks=History(name=name))  # type: ignore
 
     for error in model_errors:
         history = detector.update(value=error)
         status = detector.status
@@ -195,24 +195,24 @@
         HDDMW,
         RDDM,
     ],  # pylint: disable=too-many-locals
 )
 def test_streaming_warning_samples_buffer_on_concept_drift(
     dataset_simple: Tuple[Tuple[np.ndarray, np.ndarray], Tuple[np.ndarray, np.ndarray]],
     model: sklearn.pipeline.Pipeline,
-    detector_class: SPCBase,
+    detector_class: BaseSPC,
 ):
     """Test streaming warning samples buffer on concept drift callback.
 
     :param dataset_simple: dataset with concept drift
     :type dataset_simple: Tuple[Tuple[numpy.ndarray, numpy.ndarray],
     :param model: trained model
     :type model: sklearn.pipeline.Pipeline
     :param detector_class: concept drift detector
-    :type detector_class: SPCBase
+    :type detector_class: BaseSPC
     """
     _, test = dataset_simple  # noqa: N806
 
     detector = detector_class(
         callbacks=WarningSamplesBuffer(name="samples"),  # type: ignore
     )
 
@@ -249,28 +249,28 @@
     [
         (MMDStreaming, 5, 0.27193007, 0.00989585, 101.05240437),
     ],
 )
 def test_streaming_msprt_multivariate_different_distribution(
     X_ref_multivariate: np.ndarray,  # noqa: N803
     X_test_multivariate: np.ndarray,
-    detector_class: DataDriftBatchBase,
+    detector_class: BaseDataDriftBatch,
     expected_drift_idx: int,
     expected_distance_mean: float,
     expected_p_value: float,
     expected_likelihood: float,
 ) -> None:
     """Test streaming mSPRT test on data callback.
 
     :param X_ref_multivariate: reference multivariate data
     :type X_ref_multivariate: numpy.ndarray
     :param X_test_multivariate: test multivariate data
     :type X_test_multivariate: numpy.ndarray
     :param detector_class: detector distance
-    :type detector_class: DataDriftBatchBase
+    :type detector_class: BaseDataDriftBatch
     :param expected_drift_idx: expected drift index
     :type expected_drift_idx: int
     :param expected_distance_mean: expected distance mean value
     :type expected_distance_mean: float
     :param expected_p_value: expected p-value value
     :type expected_p_value: float
     :param expected_likelihood: expected likelihood value
```

### Comparing `frouros-0.3.0/frouros/tests/integration/test_concept_drift.py` & `frouros-0.3.1/frouros/tests/integration/test_concept_drift.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Test concept drift detectors."""
 
 from typing import Callable, Tuple
 
-import pytest  # type: ignore
 import numpy as np  # type: ignore
+import pytest  # type: ignore
 
-from frouros.detectors.concept_drift.base import ConceptDriftBase
+from frouros.detectors.concept_drift import ADWIN, ADWINConfig, KSWIN, KSWINConfig
 from frouros.detectors.concept_drift import (
     CUSUM,
     CUSUMConfig,
     GeometricMovingAverage,
     GeometricMovingAverageConfig,
     PageHinkley,
     PageHinkleyConfig,
@@ -26,16 +26,15 @@
     HDDMW,
     HDDMWConfig,
     RDDM,
     RDDMConfig,
     STEPD,
     STEPDConfig,
 )
-from frouros.detectors.concept_drift import ADWIN, ADWINConfig, KSWIN, KSWINConfig
-
+from frouros.detectors.concept_drift.base import BaseConceptDrift
 
 MIN_NUM_INSTANCES = 30
 CUMSUM_ARGS = {
     "delta": 0.005,
     "lambda_": 50,
 }
 HDDM_ARGS = {
@@ -200,25 +199,25 @@
 ]
 
 
 @pytest.mark.parametrize("detector_info", detectors)
 def test_streaming_detector_normal(
     clf_dataset: Tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray],
     train_prediction_normal: np.ndarray,
-    detector_info: Tuple[ConceptDriftBase, Callable],
+    detector_info: Tuple[BaseConceptDrift, Callable],
 ) -> None:
     """Test streaming detector.
 
     :param clf_dataset: dataset generated using SEA
     :type clf_dataset: Tuple[numpy.ndarray, numpy.ndarray,
     numpy.ndarray, numpy.ndarray]
     :param train_prediction_normal: test prediction values
     :type train_prediction_normal: numpy.ndarray
     :param detector_info: concept drift detector and value function
-    :type detector_info: Tuple[ConceptDriftBase, Callable]
+    :type detector_info: Tuple[BaseConceptDrift, Callable]
     """
     _, _, _, y_test = clf_dataset
     y_pred = train_prediction_normal  # noqa: N806
     detector, value_func = detector_info
 
     for y_sample_pred, y_sample in zip(y_pred, y_test):  # noqa: N806
         value_score = value_func(y_true=y_sample, y_pred=y_sample_pred)
```

### Comparing `frouros-0.3.0/frouros/tests/integration/test_data_drift.py` & `frouros-0.3.1/frouros/tests/integration/test_data_drift.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Test data drift detectors."""
 
 from typing import Tuple, Union
 
-import pytest  # type: ignore
 import numpy as np  # type: ignore
+import pytest  # type: ignore
 
-from frouros.detectors.data_drift.batch.base import DataDriftBatchBase
 from frouros.detectors.data_drift.batch import (
     BhattacharyyaDistance,
     EMD,
     HellingerDistance,
     HINormalizedComplement,
     PSI,
     JS,
@@ -18,14 +17,15 @@
 )
 from frouros.detectors.data_drift.batch import (
     ChiSquareTest,
     CVMTest,
     KSTest,
     WelchTTest,
 )
+from frouros.detectors.data_drift.batch.base import BaseDataDriftBatch
 from frouros.detectors.data_drift.streaming import (  # noqa: N811
     IncrementalKSTest,
     MMD as MMDStreaming,
 )
 
 
 @pytest.mark.parametrize(
@@ -66,25 +66,25 @@
         (KL(), np.inf),
         (HINormalizedComplement(), 0.78),
     ],
 )
 def test_batch_distance_based_univariate(
     X_ref_univariate: np.ndarray,  # noqa: N803
     X_test_univariate: np.ndarray,  # noqa: N803
-    detector: DataDriftBatchBase,
+    detector: BaseDataDriftBatch,
     expected_distance: float,
 ) -> None:
     """Test batch distance based univariate method.
 
     :param X_ref_univariate: reference univariate data
     :type X_ref_univariate: numpy.ndarray
     :param X_test_univariate: test univariate data
     :type X_test_univariate: numpy.ndarray
     :param detector: detector distance
-    :type detector: DataDriftBatchBase
+    :type detector: BaseDataDriftBatch
     :param expected_distance: expected p-value value
     :type expected_distance: float
     """
     _ = detector.fit(X=X_ref_univariate)
     distance, _ = detector.compare(X=X_test_univariate)
 
     assert np.isclose(distance, expected_distance)
@@ -97,25 +97,25 @@
         (HellingerDistance(), 0.74509099),
         (BhattacharyyaDistance(), 0.55516059),
     ],
 )
 def test_batch_distance_bins_based_univariate_different_distribution(
     X_ref_univariate: np.ndarray,  # noqa: N803
     X_test_univariate: np.ndarray,  # noqa: N803
-    detector: DataDriftBatchBase,
+    detector: BaseDataDriftBatch,
     expected_distance: float,
 ) -> None:
     """Test batch distance bins based univariate different distribution method.
 
     :param X_ref_univariate: reference univariate data
     :type X_ref_univariate: numpy.ndarray
     :param X_test_univariate: test univariate data
     :type X_test_univariate: numpy.ndarray
     :param detector: detector distance
-    :type detector: DataDriftBatchBase
+    :type detector: BaseDataDriftBatch
     :param expected_distance: expected p-value value
     :type expected_distance: float
     """
     _ = detector.fit(X=X_ref_univariate)
     distance, _ = detector.compare(X=X_test_univariate)
 
     assert np.isclose(distance, expected_distance)
@@ -127,24 +127,24 @@
         (PSI(), 0.01840072),
         (HellingerDistance(), 0.04792538),
         (BhattacharyyaDistance(), 0.00229684),
     ],
 )
 def test_batch_distance_bins_based_univariate_same_distribution(
     univariate_distribution_p: Tuple[float, float],
-    detector: DataDriftBatchBase,
+    detector: BaseDataDriftBatch,
     expected_distance: float,
     num_samples: int = 500,
 ) -> None:
     """Test batch distance based univariate same distribution method.
 
     :param univariate_distribution_p: mean and standard deviation of distribution p
     :type univariate_distribution_p: Tuple[float, float]
     :param detector: detector distance
-    :type detector: DataDriftBatchBase
+    :type detector: BaseDataDriftBatch
     :param expected_distance: expected p-value value
     :type expected_distance: float
     """
     np.random.seed(seed=31)
     X_ref = np.random.normal(*univariate_distribution_p, size=num_samples)  # noqa: N806
     X_test = np.random.normal(  # noqa: N806
         *univariate_distribution_p, size=num_samples
@@ -162,24 +162,24 @@
         (CVMTest(), 3776.09848103, 5.38105056e-07),
         (KSTest(), 0.99576271, 0.0),
         (WelchTTest(), -287.92032554, 0.0),
     ],
 )
 def test_batch_statistical_univariate(
     elec2_dataset: Tuple[np.ndarray, np.ndarray, np.ndarray],
-    detector: DataDriftBatchBase,
+    detector: BaseDataDriftBatch,
     expected_statistic: float,
     expected_p_value: float,
 ) -> None:
     """Test statistical univariate method.
 
     :param elec2_dataset: Elec2 raw dataset
     :type elec2_dataset: Tuple[numpy.ndarray, numpy.ndarray, numpy.ndarray]
     :param detector: detector test
-    :type detector: DataDriftBatchBase
+    :type detector: BaseDataDriftBatch
     :param expected_statistic: expected statistic value
     :type expected_statistic: float
     :param expected_p_value: expected p-value value
     :type expected_p_value: float
     """
     X_ref, _, X_test = elec2_dataset  # noqa: N806
 
@@ -190,47 +190,47 @@
     assert np.isclose(p_value, expected_p_value)
 
 
 @pytest.mark.parametrize("detector, expected_distance", [(MMD(), 0.10163633)])
 def test_batch_distance_based_multivariate_different_distribution(
     X_ref_multivariate: np.ndarray,  # noqa: N803
     X_test_multivariate: np.ndarray,  # noqa: N803
-    detector: DataDriftBatchBase,
+    detector: BaseDataDriftBatch,
     expected_distance: float,
 ) -> None:
     """Test batch distance based multivariate different distribution method.
 
     :param X_ref_multivariate: reference multivariate data
     :type X_ref_multivariate: numpy.ndarray
     :param X_test_multivariate: test multivariate data
     :type X_test_multivariate: numpy.ndarray
     :param detector: detector test
-    :type detector: DataDriftBatchBase
+    :type detector: BaseDataDriftBatch
     :param expected_distance: expected distance value
     :type expected_distance: float
     """
     _ = detector.fit(X=X_ref_multivariate)
     statistic, _ = detector.compare(X=X_test_multivariate)
 
     assert np.isclose(statistic, expected_distance)
 
 
 @pytest.mark.parametrize("detector, expected_distance", [(MMD(), 0.01570397)])
 def test_batch_distance_based_multivariate_same_distribution(
     multivariate_distribution_p: Tuple[np.ndarray, np.ndarray],
-    detector: DataDriftBatchBase,
+    detector: BaseDataDriftBatch,
     expected_distance: float,
     num_samples: int = 100,
 ) -> None:
     """Test batch distance based multivariate same distribution method.
 
     :param multivariate_distribution_p: mean and covariance matrix of distribution p
     :type multivariate_distribution_p: Tuple[numpy.ndarray, numpy.ndarray]
     :param detector: detector test
-    :type detector: DataDriftBatchBase
+    :type detector: BaseDataDriftBatch
     :param num_samples: number of random samples
     :type num_samples: int
     :param expected_distance: expected distance value
     :type expected_distance: float
     """
     np.random.seed(seed=31)
     X_ref = np.random.multivariate_normal(  # noqa: N806
@@ -249,25 +249,25 @@
 @pytest.mark.parametrize(
     "detector, expected_distance",
     [(MMD(chunk_size=10), 0.10163633), (MMD(chunk_size=None), 0.10163633)],
 )
 def test_batch_distance_based_chunk_size_valid(
     X_ref_multivariate: np.ndarray,  # noqa: N803
     X_test_multivariate: np.ndarray,  # noqa: N803
-    detector: DataDriftBatchBase,
+    detector: BaseDataDriftBatch,
     expected_distance: float,
 ) -> None:
     """Test batch distance based chunk size valid method.
 
     :param X_ref_multivariate: reference multivariate data
     :type X_ref_multivariate: numpy.ndarray
     :param X_test_multivariate: test multivariate data
     :type X_test_multivariate: numpy.ndarray
     :param detector: detector test
-    :type detector: DataDriftBatchBase
+    :type detector: BaseDataDriftBatch
     :param expected_distance: expected distance value
     :type expected_distance: float
     """
     _ = detector.fit(X=X_ref_multivariate)
     statistic, _ = detector.compare(X=X_test_multivariate)
 
     assert np.isclose(statistic.distance, expected_distance)
@@ -300,24 +300,24 @@
     "detector, expected_statistic, expected_p_value",
     [
         (IncrementalKSTest(), 0.27, 0.46046910),
     ],
 )
 def test_streaming_statistical_univariate_same_distribution(
     univariate_distribution_p: Tuple[float, float],
-    detector: DataDriftBatchBase,
+    detector: BaseDataDriftBatch,
     expected_statistic: float,
     expected_p_value: float,
 ) -> None:
     """Test streaming statistical test univariate same distribution method.
 
     :param univariate_distribution_p: mean and standard deviation of distribution p
     :type univariate_distribution_p: Tuple[float, float]
     :param detector: detector statistical test
-    :type detector: DataDriftStreamingBase
+    :type detector: BaseDataDriftStreaming
     :param expected_statistic: expected statistic value
     :type expected_statistic: float
     :param expected_p_value: expected p-value
     :type expected_p_value: float
     """
     np.random.seed(seed=31)
     X_ref = np.random.normal(*univariate_distribution_p, size=100)  # noqa: N806
@@ -338,26 +338,26 @@
     [
         (IncrementalKSTest(), 1.0, 0.0),
     ],
 )
 def test_streaming_statistical_univariate_different_distribution(
     univariate_distribution_p: Tuple[float, float],
     univariate_distribution_q: Tuple[float, float],
-    detector: DataDriftBatchBase,
+    detector: BaseDataDriftBatch,
     expected_statistic: float,
     expected_p_value: float,
 ) -> None:
     """Test streaming statistical test univariate different distribution method.
 
     :param univariate_distribution_p: mean and standard deviation of distribution p
     :type univariate_distribution_p: Tuple[float, float]
     :param univariate_distribution_q: mean and standard deviation of distribution q
     :type univariate_distribution_q: Tuple[float, float]
     :param detector: detector statistical test
-    :type detector: DataDriftStreamingBase
+    :type detector: BaseDataDriftStreaming
     :param expected_statistic: expected statistic value
     :type expected_statistic: float
     :param expected_p_value: expected p-value
     :type expected_p_value: float
     """
     np.random.seed(seed=31)
     X_ref = np.random.normal(*univariate_distribution_p, size=100)  # noqa: N806
@@ -377,23 +377,23 @@
     "detector, expected_distance",
     [
         (MMDStreaming(window_size=10), -0.02327412),
     ],
 )
 def test_streaming_distance_based_univariate_same_distribution(
     univariate_distribution_p: Tuple[float, float],
-    detector: DataDriftBatchBase,
+    detector: BaseDataDriftBatch,
     expected_distance: float,
 ) -> None:
     """Test streaming distance based univariate same distribution method.
 
     :param univariate_distribution_p: mean and standard deviation of distribution p
     :type univariate_distribution_p: Tuple[float, float]
     :param detector: detector statistical test
-    :type detector: DataDriftStreamingBase
+    :type detector: BaseDataDriftStreaming
     :param expected_distance: expected distance value
     :type expected_distance: float
     """
     np.random.seed(seed=31)
     X_ref = np.random.normal(*univariate_distribution_p, size=100)  # noqa: N806
     X_test = np.random.normal(*univariate_distribution_p, size=100)  # noqa: N806
 
@@ -411,25 +411,25 @@
     [
         (MMDStreaming(window_size=10), 0.8656735),
     ],
 )
 def test_streaming_distance_based_univariate_different_distribution(
     univariate_distribution_p: Tuple[float, float],
     univariate_distribution_q: Tuple[float, float],
-    detector: DataDriftBatchBase,
+    detector: BaseDataDriftBatch,
     expected_distance: float,
 ) -> None:
     """Test streaming distance based univariate different distribution method.
 
     :param univariate_distribution_p: mean and standard deviation of distribution p
     :type univariate_distribution_p: Tuple[float, float]
     :param univariate_distribution_q: mean and standard deviation of distribution q
     :type univariate_distribution_q: Tuple[float, float]
     :param detector: detector statistical test
-    :type detector: DataDriftStreamingBase
+    :type detector: BaseDataDriftStreaming
     :param expected_distance: expected distance value
     :type expected_distance: float
     """
     np.random.seed(seed=31)
     X_ref = np.random.normal(*univariate_distribution_p, size=100)  # noqa: N806
     X_test = np.random.normal(*univariate_distribution_q, size=100)  # noqa: N806
```

### Comparing `frouros-0.3.0/frouros/tests/integration/test_real.py` & `frouros-0.3.1/frouros/tests/integration/test_real.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Test real datasets module."""
 
-import pytest  # type: ignore
 import numpy as np  # type: ignore
+import pytest  # type: ignore
 
 from frouros.datasets.exceptions import ReadFileError
 from frouros.datasets.real import Elec2
 
 
 # Elec2 tests
 def test_elec2_file_not_found_error(elec2_raw: Elec2) -> None:
```

### Comparing `frouros-0.3.0/frouros/tests/integration/test_synthetic.py` & `frouros-0.3.1/frouros/tests/integration/test_synthetic.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.0/frouros/tests/unit/metrics/test_prequential_error.py` & `frouros-0.3.1/frouros/tests/unit/metrics/test_prequential_error.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.0/frouros/utils/data_structures.py` & `frouros-0.3.1/frouros/utils/data_structures.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.0/frouros/utils/decorators.py` & `frouros-0.3.1/frouros/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.0/frouros/utils/stats.py` & `frouros-0.3.1/frouros/utils/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 from functools import partial
 from multiprocessing import Pool
 from typing import Any, Callable, Dict, Optional, List, Union
 
 import numpy as np  # type: ignore
 from tqdm import tqdm  # type: ignore
 
-from frouros.utils.logger import logger
 from frouros.utils.data_structures import CircularQueue
+from frouros.utils.logger import logger
 
 
-class Stat(abc.ABC):
+class BaseStat(abc.ABC):
     """Abstract class representing an statistic."""
 
     @abc.abstractmethod
     def get(self) -> float:
         """Get method."""
 
 
-class IncrementalStat(Stat):
+class IncrementalStat(BaseStat):
     """Abstract class representing an incremental statistic."""
 
     @abc.abstractmethod
     def update(self, value: Union[int, float]) -> None:
         """Update abstract method."""
 
     @abc.abstractmethod
```

### Comparing `frouros-0.3.0/frouros.egg-info/PKG-INFO` & `frouros-0.3.1/frouros.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 Metadata-Version: 2.1
 Name: frouros
-Version: 0.3.0
-Summary: A Python library for drift detection in Machine Learning problems
+Version: 0.3.1
+Summary: An open source Python library for drift detection in machine Learning systems
 Home-page: https://github.com/IFCA/frouros
 Author: Jaime Céspedes Sisniega
 Author-email: cespedes@ifca.unican.es
 Maintainer: Jaime Céspedes Sisniega
 Maintainer-email: cespedes@ifca.unican.es
 License: BSD-3-Clause
 Project-URL: homepage, https://frouros.readthedocs.io
 Project-URL: repository, https://github.com/IFCA/frouros
 Project-URL: documentation, https://frouros.readthedocs.io
 Project-URL: download, https://pypi.org/project/frouros/
-Keywords: drift-detection,concept-drift,data-drift,machine-learning,data-science
+Keywords: drift-detection,concept-drift,data-drift,machine-learning,data-science,machine-learning-operations,machine-learning-systems
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8,<3.12
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: notebooks
 License-File: LICENSE
 
 <p align="center">
-  <img height="115px" src="images/logo.png" alt="frouros_logo">
+  <img height="115px" src="https://raw.githubusercontent.com/IFCA/frouros/main/images/logo.png" alt="logo">
 </p>
 
 ---
 
 <p align="center">
   <!-- CI -->
   <a href="https://github.com/IFCA/frouros/actions/workflows/ci.yml">
```

#### html2text {}

```diff
@@ -1,26 +1,30 @@
-Metadata-Version: 2.1 Name: frouros Version: 0.3.0 Summary: A Python library
-for drift detection in Machine Learning problems Home-page: https://github.com/
-IFCA/frouros Author: Jaime CÃ©spedes Sisniega Author-email:
+Metadata-Version: 2.1 Name: frouros Version: 0.3.1 Summary: An open source
+Python library for drift detection in machine Learning systems Home-page:
+https://github.com/IFCA/frouros Author: Jaime CÃ©spedes Sisniega Author-email:
 cespedes@ifca.unican.es Maintainer: Jaime CÃ©spedes Sisniega Maintainer-email:
 cespedes@ifca.unican.es License: BSD-3-Clause Project-URL: homepage, https://
 frouros.readthedocs.io Project-URL: repository, https://github.com/IFCA/frouros
 Project-URL: documentation, https://frouros.readthedocs.io Project-URL:
 download, https://pypi.org/project/frouros/ Keywords: drift-detection,concept-
-drift,data-drift,machine-learning,data-science Platform: UNKNOWN Classifier:
-Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
-Science/Research Classifier: Topic :: Scientific/Engineering Classifier: Topic
-:: Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
+drift,data-drift,machine-learning,data-science,machine-learning-
+operations,machine-learning-systems Platform: UNKNOWN Classifier: Development
+Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
+Approved :: BSD License Classifier: Topic :: Scientific/Engineering Classifier:
+Topic :: Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
 Scientific/Engineering :: Mathematics Classifier: Topic :: Software Development
-:: Libraries :: Python Modules Classifier: Programming Language :: Python ::
-3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8,<3.12 Description-Content-Type: text/markdown Provides-
-Extra: docs Provides-Extra: notebooks License-File: LICENSE
-                                [frouros_logo]
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3 :: Only Requires-Python: >=3.8,<3.12 Description-
+Content-Type: text/markdown Provides-Extra: docs Provides-Extra: notebooks
+License-File: LICENSE
+                                    [logo]
 ---
        [ci]  [coverage]  [documentation]  [downloads]  [pypi]  [python]
                                 [bsd_3_license]
 Frouros is a Python library for drift detection in machine learning systems
 that provides a combination of classical and more recent algorithms for both
 concept and data drift detection.
                  "Everything changes and nothing stands still"
```

### Comparing `frouros-0.3.0/frouros.egg-info/SOURCES.txt` & `frouros-0.3.1/frouros.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `frouros-0.3.0/pyproject.toml` & `frouros-0.3.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 [project]
 name = "frouros"
-version = "0.3.0"
-description = "A Python library for drift detection in Machine Learning problems"
+version = "0.3.1"
+description = "An open source Python library for drift detection in machine Learning systems"
 authors = [
     {name = "Jaime Céspedes Sisniega", email = "cespedes@ifca.unican.es"}
 ]
 maintainers = [
     {name = "Jaime Céspedes Sisniega", email = "cespedes@ifca.unican.es"}
 ]
 readme = "README.md"
 keywords = [
     "drift-detection",
     "concept-drift",
     "data-drift",
     "machine-learning",
     "data-science",
+    "machine-learning-operations",
+    "machine-learning-systems",
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
+    "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
+    "License :: OSI Approved :: BSD License",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Scientific/Engineering :: Mathematics",
+    "Topic :: Software Development",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3 :: Only",
 ]
 requires-python = ">=3.8,<3.12"
 dependencies = [
     "matplotlib>=3.6.0,<3.7",
     "numpy>=1.24.0,<1.25",
     "requests>=2.31.0,<2.32",
     "scipy>=1.10.0,<1.11",
```

### Comparing `frouros-0.3.0/setup.py` & `frouros-0.3.1/setup.py`

 * *Files identical despite different names*

