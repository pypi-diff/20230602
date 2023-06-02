# Comparing `tmp/foxes-0.3.4.tar.gz` & `tmp/foxes-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foxes-0.3.4.tar", last modified: Tue Apr 18 09:48:26 2023, max compression
+gzip compressed data, was "foxes-0.3.5.tar", last modified: Fri Jun  2 09:25:48 2023, max compression
```

## Comparing `foxes-0.3.4.tar` & `foxes-0.3.5.tar`

### file list

```diff
@@ -1,259 +1,261 @@
-drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.912066 foxes-0.3.4/
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     1071 2022-11-29 14:27:28.000000 foxes-0.3.4/LICENSE
--rw-rw-r--   0 jonas     (1001) jonas     (1001)    40774 2022-11-29 14:27:28.000000 foxes-0.3.4/Logo_FOXES.svg
--rw-rw-r--   0 jonas     (1001) jonas     (1001)      215 2023-03-07 14:47:39.000000 foxes-0.3.4/MANIFEST.in
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     6589 2023-04-18 09:48:26.916066 foxes-0.3.4/PKG-INFO
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     5769 2023-04-18 09:34:13.000000 foxes-0.3.4/README.md
-drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.900066 foxes-0.3.4/foxes/
--rw-rw-r--   0 jonas     (1001) jonas     (1001)        6 2023-03-15 10:46:27.000000 foxes-0.3.4/foxes/VERSION
--rw-rw-r--   0 jonas     (1001) jonas     (1001)      712 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/__init__.py
-drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.900066 foxes-0.3.4/foxes/algorithms/
--rw-rw-r--   0 jonas     (1001) jonas     (1001)      131 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/algorithms/__init__.py
-drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.900066 foxes-0.3.4/foxes/algorithms/downwind/
--rw-rw-r--   0 jonas     (1001) jonas     (1001)       53 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/algorithms/downwind/__init__.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)    17373 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/algorithms/downwind/downwind.py
-drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.900066 foxes-0.3.4/foxes/algorithms/downwind/models/
--rw-rw-r--   0 jonas     (1001) jonas     (1001)      242 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/algorithms/downwind/models/__init__.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     2292 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/algorithms/downwind/models/calc_order.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     3339 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/algorithms/downwind/models/farm_wakes_calc.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     4368 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/algorithms/downwind/models/point_wakes_calc.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     1876 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/algorithms/downwind/models/set_amb_farm_results.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     1436 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/algorithms/downwind/models/set_amb_point_results.py
-drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.900066 foxes-0.3.4/foxes/algorithms/iterative/
--rw-rw-r--   0 jonas     (1001) jonas     (1001)       55 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/algorithms/iterative/__init__.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     2056 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/algorithms/iterative/iterative.py
-drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.900066 foxes-0.3.4/foxes/algorithms/iterative/models/
--rw-rw-r--   0 jonas     (1001) jonas     (1001)      161 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/algorithms/iterative/models/__init__.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     5083 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/algorithms/iterative/models/convergence.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     3297 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/algorithms/iterative/models/farm_wakes_calc.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     4084 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/algorithms/iterative/models/loop_runner.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)      201 2023-04-12 10:11:20.000000 foxes-0.3.4/foxes/constants.py
-drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.904066 foxes-0.3.4/foxes/core/
--rw-rw-r--   0 jonas     (1001) jonas     (1001)      762 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/core/__init__.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)    15807 2023-04-12 10:11:20.000000 foxes-0.3.4/foxes/core/algorithm.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     2815 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/core/data.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     7874 2023-04-12 10:11:20.000000 foxes-0.3.4/foxes/core/data_calc_model.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)    12080 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/core/farm_controller.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     7098 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/core/farm_data_model.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)      246 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/core/farm_model.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     5439 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/core/model.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     5062 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/core/partial_wakes_model.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     6952 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/core/point_data_model.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)    12685 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/core/rotor_model.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     8006 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/core/states.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     2929 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/core/turbine.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     1058 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/core/turbine_model.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     1359 2023-04-12 10:11:20.000000 foxes-0.3.4/foxes/core/turbine_type.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     1619 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/core/vertical_profile.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     6499 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/core/wake_frame.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     2901 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/core/wake_model.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     2540 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/core/wake_superposition.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     1636 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/core/wind_farm.py
-drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.904066 foxes-0.3.4/foxes/data/
--rw-rw-r--   0 jonas     (1001) jonas     (1001)      120 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/data/__init__.py
-drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.904066 foxes-0.3.4/foxes/data/farms/
--rw-rw-r--   0 jonas     (1001) jonas     (1001)        0 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/data/farms/__init__.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     1872 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/data/farms/test_farm_67.csv
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     2921 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/data/parse.py
-drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.904066 foxes-0.3.4/foxes/data/power_ct_curves/
--rw-rw-r--   0 jonas     (1001) jonas     (1001)      410 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/data/power_ct_curves/DTU-10MW-D178d3-H119.csv
--rw-rw-r--   0 jonas     (1001) jonas     (1001)      300 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/data/power_ct_curves/IEA-15MW-D240-H150.csv
--rw-rw-r--   0 jonas     (1001) jonas     (1001)      851 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/data/power_ct_curves/IWT-7d5MW-D164-H100.csv
--rw-rw-r--   0 jonas     (1001) jonas     (1001)      401 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/data/power_ct_curves/NREL-5MW-D126-H90.csv
--rw-rw-r--   0 jonas     (1001) jonas     (1001)        0 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/data/power_ct_curves/__init__.py
-drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.904066 foxes-0.3.4/foxes/data/states/
--rw-rw-r--   0 jonas     (1001) jonas     (1001)   427815 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/data/states/WRF-Timeseries-4464.csv.gz
--rw-rw-r--   0 jonas     (1001) jonas     (1001)        0 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/data/states/__init__.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)   126124 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/data/states/abl_states_6000.csv.gz
--rw-rw-r--   0 jonas     (1001) jonas     (1001)    29085 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/data/states/timeseries_3000.csv.gz
--rw-rw-r--   0 jonas     (1001) jonas     (1001)    78694 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/data/states/timeseries_8000.csv.gz
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     4943 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/data/states/wind_rose_bremen.csv
--rw-rw-r--   0 jonas     (1001) jonas     (1001)    10990 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/data/states/wind_rotation.nc
--rw-rw-r--   0 jonas     (1001) jonas     (1001)      519 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/data/static_data.py
-drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.904066 foxes-0.3.4/foxes/input/
--rw-rw-r--   0 jonas     (1001) jonas     (1001)       68 2023-04-12 10:11:20.000000 foxes-0.3.4/foxes/input/__init__.py
-drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.904066 foxes-0.3.4/foxes/input/farm_layout/
--rw-rw-r--   0 jonas     (1001) jonas     (1001)      218 2023-04-12 10:11:20.000000 foxes-0.3.4/foxes/input/farm_layout/__init__.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     3135 2023-04-12 10:11:20.000000 foxes-0.3.4/foxes/input/farm_layout/add_from_csv.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)      550 2023-04-12 10:11:20.000000 foxes-0.3.4/foxes/input/farm_layout/add_from_df.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     1561 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/input/farm_layout/add_from_file.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     1619 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/input/farm_layout/add_from_json.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     1444 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/input/farm_layout/add_grid.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     1175 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/input/farm_layout/add_row.py
-drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.904066 foxes-0.3.4/foxes/input/states/
--rw-rw-r--   0 jonas     (1001) jonas     (1001)      244 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/input/states/__init__.py
-drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.904066 foxes-0.3.4/foxes/input/states/create/
--rw-rw-r--   0 jonas     (1001) jonas     (1001)       81 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/input/states/create/__init__.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     3248 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/input/states/create/random_abl_states.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)    15880 2023-04-13 06:31:59.000000 foxes-0.3.4/foxes/input/states/field_data_nc.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)    12359 2023-03-14 07:04:35.000000 foxes-0.3.4/foxes/input/states/multi_height.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     4362 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/input/states/scan_ws.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     5734 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/input/states/single.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)    10477 2023-03-14 07:04:35.000000 foxes-0.3.4/foxes/input/states/states_table.py
-drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.904066 foxes-0.3.4/foxes/input/windio/
--rw-rw-r--   0 jonas     (1001) jonas     (1001)       29 2023-04-12 10:11:20.000000 foxes-0.3.4/foxes/input/windio/__init__.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     8809 2023-04-12 10:11:20.000000 foxes-0.3.4/foxes/input/windio/windio.py
-drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.904066 foxes-0.3.4/foxes/models/
--rw-rw-r--   0 jonas     (1001) jonas     (1001)      349 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/__init__.py
-drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.904066 foxes-0.3.4/foxes/models/farm_controllers/
--rw-rw-r--   0 jonas     (1001) jonas     (1001)       39 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/farm_controllers/__init__.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)      211 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/farm_controllers/basic.py
-drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.904066 foxes-0.3.4/foxes/models/farm_models/
--rw-rw-r--   0 jonas     (1001) jonas     (1001)       44 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/farm_models/__init__.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     3347 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/farm_models/turbine2farm.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)    12536 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/model_book.py
-drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.904066 foxes-0.3.4/foxes/models/partial_wakes/
--rw-rw-r--   0 jonas     (1001) jonas     (1001)      212 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/partial_wakes/__init__.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)    10395 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/partial_wakes/axiwake.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)    10687 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/partial_wakes/distsliced.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     2571 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/partial_wakes/grid.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     7406 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/partial_wakes/mapped.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     6098 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/partial_wakes/rotor_points.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     9581 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/partial_wakes/top_hat.py
-drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.908066 foxes-0.3.4/foxes/models/point_models/
--rw-rw-r--   0 jonas     (1001) jonas     (1001)      108 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/point_models/__init__.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     4468 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/point_models/set_uniform_data.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     1372 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/point_models/tke2ti.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     1935 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/point_models/wake_deltas.py
-drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.908066 foxes-0.3.4/foxes/models/rotor_models/
--rw-rw-r--   0 jonas     (1001) jonas     (1001)       60 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/rotor_models/__init__.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     5582 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/rotor_models/centre.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     4843 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/rotor_models/grid.py
-drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.908066 foxes-0.3.4/foxes/models/turbine_models/
--rw-rw-r--   0 jonas     (1001) jonas     (1001)      348 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/turbine_models/__init__.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     2533 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/turbine_models/calculator.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     2511 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/turbine_models/kTI_model.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     5390 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/turbine_models/power_mask.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     7409 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/turbine_models/sector_management.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     3393 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/turbine_models/set_XYHD.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     3879 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/turbine_models/set_farm_vars.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     5120 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/turbine_models/table_factors.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     2060 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/turbine_models/thrust2ct.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     1580 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/turbine_models/yaw2yawm.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     1551 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/turbine_models/yawm2yaw.py
-drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.908066 foxes-0.3.4/foxes/models/turbine_types/
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     1422 2023-04-12 10:11:20.000000 foxes-0.3.4/foxes/models/turbine_types/CpCt_file.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     2056 2023-04-12 10:11:20.000000 foxes-0.3.4/foxes/models/turbine_types/CpCt_from_two.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     7686 2023-04-12 10:11:20.000000 foxes-0.3.4/foxes/models/turbine_types/PCt_file.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     8877 2023-04-12 10:11:20.000000 foxes-0.3.4/foxes/models/turbine_types/PCt_from_two.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)      221 2023-04-12 10:11:20.000000 foxes-0.3.4/foxes/models/turbine_types/__init__.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     1284 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/turbine_types/null_type.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)    11131 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/turbine_types/wsrho2PCt_two_files.py
-drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.908066 foxes-0.3.4/foxes/models/vertical_profiles/
--rw-rw-r--   0 jonas     (1001) jonas     (1001)       59 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/vertical_profiles/__init__.py
-drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.908066 foxes-0.3.4/foxes/models/vertical_profiles/abl_log/
--rw-rw-r--   0 jonas     (1001) jonas     (1001)      244 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/vertical_profiles/abl_log/__init__.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     1082 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/vertical_profiles/abl_log/abl_log_neutral_ws.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     1161 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/vertical_profiles/abl_log/abl_log_stable_ws.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     1173 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/vertical_profiles/abl_log/abl_log_unstable_ws.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     2495 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/vertical_profiles/abl_log/abl_log_ws.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     1151 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/vertical_profiles/abl_log/sheared_ws.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)      375 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/vertical_profiles/uniform.py
-drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.908066 foxes-0.3.4/foxes/models/wake_frames/
--rw-rw-r--   0 jonas     (1001) jonas     (1001)      137 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/wake_frames/__init__.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     4646 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/wake_frames/farm_order.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     3740 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/wake_frames/rotor_wd.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)    11929 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/wake_frames/streamlines.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     8001 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/wake_frames/yawed_wakes.py
-drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.908066 foxes-0.3.4/foxes/models/wake_models/
--rw-rw-r--   0 jonas     (1001) jonas     (1001)      207 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/wake_models/__init__.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     2672 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/wake_models/axisymmetric.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     6535 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/wake_models/dist_sliced.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     2637 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/wake_models/gaussian.py
-drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.908066 foxes-0.3.4/foxes/models/wake_models/ti/
--rw-rw-r--   0 jonas     (1001) jonas     (1001)       82 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/wake_models/ti/__init__.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     8169 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/wake_models/ti/crespo_hernandez.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     5947 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/wake_models/ti/iec_ti.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     5038 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/wake_models/top_hat.py
-drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.908066 foxes-0.3.4/foxes/models/wake_models/wind/
--rw-rw-r--   0 jonas     (1001) jonas     (1001)      178 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/wake_models/wind/__init__.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     5278 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/wake_models/wind/bastankhah.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     4768 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/wake_models/wind/jensen.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)    14461 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/wake_models/wind/porte_agel.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)    11735 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/wake_models/wind/turbopark.py
-drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.908066 foxes-0.3.4/foxes/models/wake_superpositions/
--rw-rw-r--   0 jonas     (1001) jonas     (1001)      159 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/wake_superpositions/__init__.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     5889 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/wake_superpositions/linear.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     6678 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/wake_superpositions/max.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     6470 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/models/wake_superpositions/quadratic.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     4758 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/models/wake_superpositions/ti_superp.py
-drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.908066 foxes-0.3.4/foxes/opt/
--rw-rw-r--   0 jonas     (1001) jonas     (1001)      139 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/opt/__init__.py
-drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.912066 foxes-0.3.4/foxes/opt/constraints/
--rw-rw-r--   0 jonas     (1001) jonas     (1001)      114 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/opt/constraints/__init__.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     5879 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/constraints/area_geometry.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     7391 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/constraints/min_dist.py
-drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.912066 foxes-0.3.4/foxes/opt/core/
--rw-rw-r--   0 jonas     (1001) jonas     (1001)      212 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/core/__init__.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     1889 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/core/farm_constraint.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     1888 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/core/farm_objective.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     9490 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/core/farm_opt_problem.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     7652 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/core/farm_vars_problem.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     5570 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/core/pop_states.py
-drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.912066 foxes-0.3.4/foxes/opt/objectives/
--rw-rw-r--   0 jonas     (1001) jonas     (1001)      109 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/objectives/__init__.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     8779 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/objectives/farm_vars.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     3909 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/objectives/max_n_turbines.py
-drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.912066 foxes-0.3.4/foxes/opt/problems/
--rw-rw-r--   0 jonas     (1001) jonas     (1001)       61 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/problems/__init__.py
-drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.912066 foxes-0.3.4/foxes/opt/problems/layout/
--rw-rw-r--   0 jonas     (1001) jonas     (1001)      180 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/problems/layout/__init__.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     5753 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/problems/layout/farm_layout.py
-drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.912066 foxes-0.3.4/foxes/opt/problems/layout/geom_layouts/
--rw-rw-r--   0 jonas     (1001) jonas     (1001)      333 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/problems/layout/geom_layouts/__init__.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     7680 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/problems/layout/geom_layouts/constraints.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     8069 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/problems/layout/geom_layouts/geom_layout.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     7446 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/problems/layout/geom_layouts/geom_layout_gridded.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     9661 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/problems/layout/geom_layouts/geom_reggrid.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)    13910 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/problems/layout/geom_layouts/geom_reggrids.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     5984 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/problems/layout/geom_layouts/objectives.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)    11665 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/problems/layout/reggrids_layout.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)    10479 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/problems/layout/regular_layout.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)    18815 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/opt/problems/opt_farm_vars.py
-drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.912066 foxes-0.3.4/foxes/output/
--rw-rw-r--   0 jonas     (1001) jonas     (1001)      355 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/output/__init__.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)    10501 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/output/farm_layout.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)    15715 2023-04-12 10:11:20.000000 foxes-0.3.4/foxes/output/farm_results_eval.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)    45206 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/output/flow_plots_2d.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     2189 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/output/output.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     2581 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/output/results_writer.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     9970 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/output/rose_plot.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     2347 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/output/state_turbine_map.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     5452 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/output/turbine_type_curves.py
-drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.912066 foxes-0.3.4/foxes/utils/
--rw-rw-r--   0 jonas     (1001) jonas     (1001)      453 2023-03-15 10:38:11.000000 foxes-0.3.4/foxes/utils/__init__.py
-drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.912066 foxes-0.3.4/foxes/utils/abl/
--rw-rw-r--   0 jonas     (1001) jonas     (1001)       88 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/utils/abl/__init__.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     1278 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/utils/abl/neutral.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)      444 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/utils/abl/sheared.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     1728 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/utils/abl/stable.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     1530 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/utils/abl/unstable.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     3313 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/utils/cubic_roots.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     5141 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/utils/data_book.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)      793 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/utils/dict.py
-drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.912066 foxes-0.3.4/foxes/utils/geom2d/
--rw-rw-r--   0 jonas     (1001) jonas     (1001)      179 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/utils/geom2d/__init__.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)    18793 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/utils/geom2d/area_geometry.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     4451 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/utils/geom2d/circle.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     1627 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/utils/geom2d/example_intersection.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     1751 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/utils/geom2d/example_union.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     6091 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/utils/geom2d/half_plane.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     5467 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/utils/geom2d/polygon.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     7770 2023-03-15 10:38:11.000000 foxes-0.3.4/foxes/utils/geopandas_helpers.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     4623 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/utils/pandas_helpers.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)      350 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/utils/plotly_helpers.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     5802 2023-04-12 10:11:20.000000 foxes-0.3.4/foxes/utils/runners.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)      362 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/utils/subclasses.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     2761 2022-11-29 14:27:28.000000 foxes-0.3.4/foxes/utils/two_circles.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     2746 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/utils/wind_dir.py
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     1268 2023-03-07 14:47:39.000000 foxes-0.3.4/foxes/variables.py
-drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-04-18 09:48:26.900066 foxes-0.3.4/foxes.egg-info/
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     6589 2023-04-18 09:48:26.000000 foxes-0.3.4/foxes.egg-info/PKG-INFO
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     7673 2023-04-18 09:48:26.000000 foxes-0.3.4/foxes.egg-info/SOURCES.txt
--rw-rw-r--   0 jonas     (1001) jonas     (1001)        1 2023-04-18 09:48:26.000000 foxes-0.3.4/foxes.egg-info/dependency_links.txt
--rw-rw-r--   0 jonas     (1001) jonas     (1001)      194 2023-04-18 09:48:26.000000 foxes-0.3.4/foxes.egg-info/requires.txt
--rw-rw-r--   0 jonas     (1001) jonas     (1001)        6 2023-04-18 09:48:26.000000 foxes-0.3.4/foxes.egg-info/top_level.txt
--rw-rw-r--   0 jonas     (1001) jonas     (1001)        1 2023-04-18 09:48:26.000000 foxes-0.3.4/foxes.egg-info/zip-safe
--rw-rw-r--   0 jonas     (1001) jonas     (1001)      185 2022-11-29 14:27:28.000000 foxes-0.3.4/pyproject.toml
--rw-rw-r--   0 jonas     (1001) jonas     (1001)     1130 2023-04-18 09:48:26.916066 foxes-0.3.4/setup.cfg
--rw-rw-r--   0 jonas     (1001) jonas     (1001)       69 2022-11-29 14:27:28.000000 foxes-0.3.4/setup.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1071 2023-06-02 08:05:39.000000 foxes-0.3.5/LICENSE
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    40774 2023-06-02 08:05:43.000000 foxes-0.3.5/Logo_FOXES.svg
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      215 2023-06-02 08:05:43.000000 foxes-0.3.5/MANIFEST.in
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     6589 2023-06-02 09:25:48.016762 foxes-0.3.5/PKG-INFO
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5769 2023-06-02 08:05:39.000000 foxes-0.3.5/README.md
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.006762 foxes-0.3.5/foxes/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)        6 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/VERSION
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      717 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/__init__.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.006762 foxes-0.3.5/foxes/algorithms/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      188 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/algorithms/__init__.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.006762 foxes-0.3.5/foxes/algorithms/downwind/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)       53 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/algorithms/downwind/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    17305 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/algorithms/downwind/downwind.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.006762 foxes-0.3.5/foxes/algorithms/downwind/models/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      242 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/algorithms/downwind/models/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2292 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/algorithms/downwind/models/calc_order.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3329 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/algorithms/downwind/models/farm_wakes_calc.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4391 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/algorithms/downwind/models/point_wakes_calc.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1876 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/algorithms/downwind/models/set_amb_farm_results.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1500 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/algorithms/downwind/models/set_amb_point_results.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.006762 foxes-0.3.5/foxes/algorithms/iterative/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)       55 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/algorithms/iterative/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2016 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/algorithms/iterative/iterative.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.006762 foxes-0.3.5/foxes/algorithms/iterative/models/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      161 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/algorithms/iterative/models/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5050 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/algorithms/iterative/models/convergence.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3266 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/algorithms/iterative/models/farm_wakes_calc.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4064 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/algorithms/iterative/models/loop_runner.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1568 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/constants.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.006762 foxes-0.3.5/foxes/core/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      811 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/core/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    16434 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/core/algorithm.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2834 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/core/data.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     7848 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/core/data_calc_model.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    12026 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/core/farm_controller.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     7098 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/core/farm_data_model.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      246 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/core/farm_model.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5498 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/core/model.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5054 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/core/partial_wakes_model.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     6951 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/core/point_data_model.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    12678 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/core/rotor_model.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     8029 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/core/states.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2929 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/core/turbine.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1058 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/core/turbine_model.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1304 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/core/turbine_type.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1619 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/core/vertical_profile.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     6499 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/core/wake_frame.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2901 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/core/wake_model.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2540 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/core/wake_superposition.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1636 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/core/wind_farm.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.006762 foxes-0.3.5/foxes/data/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      152 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/data/__init__.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.006762 foxes-0.3.5/foxes/data/farms/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)        0 2023-06-02 08:05:43.000000 foxes-0.3.5/foxes/data/farms/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1872 2023-06-02 08:05:43.000000 foxes-0.3.5/foxes/data/farms/test_farm_67.csv
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2916 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/data/parse.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.006762 foxes-0.3.5/foxes/data/power_ct_curves/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      410 2023-06-02 08:05:43.000000 foxes-0.3.5/foxes/data/power_ct_curves/DTU-10MW-D178d3-H119.csv
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      300 2023-06-02 08:05:43.000000 foxes-0.3.5/foxes/data/power_ct_curves/IEA-15MW-D240-H150.csv
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      851 2023-06-02 08:05:43.000000 foxes-0.3.5/foxes/data/power_ct_curves/IWT-7d5MW-D164-H100.csv
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      401 2023-06-02 08:05:43.000000 foxes-0.3.5/foxes/data/power_ct_curves/NREL-5MW-D126-H90.csv
+-rw-r--r--   0 jonas     (1000) jonas     (1000)        0 2023-06-02 08:05:43.000000 foxes-0.3.5/foxes/data/power_ct_curves/__init__.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.006762 foxes-0.3.5/foxes/data/states/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)   427815 2023-06-02 08:05:43.000000 foxes-0.3.5/foxes/data/states/WRF-Timeseries-4464.csv.gz
+-rw-r--r--   0 jonas     (1000) jonas     (1000)        0 2023-06-02 08:05:43.000000 foxes-0.3.5/foxes/data/states/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)   126124 2023-06-02 08:05:43.000000 foxes-0.3.5/foxes/data/states/abl_states_6000.csv.gz
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    29085 2023-06-02 08:05:43.000000 foxes-0.3.5/foxes/data/states/timeseries_3000.csv.gz
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    78694 2023-06-02 08:05:43.000000 foxes-0.3.5/foxes/data/states/timeseries_8000.csv.gz
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4943 2023-06-02 08:05:43.000000 foxes-0.3.5/foxes/data/states/wind_rose_bremen.csv
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    10990 2023-06-02 08:05:43.000000 foxes-0.3.5/foxes/data/states/wind_rotation.nc
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      519 2023-06-02 08:05:43.000000 foxes-0.3.5/foxes/data/static_data.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.006762 foxes-0.3.5/foxes/input/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      125 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/input/__init__.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.006762 foxes-0.3.5/foxes/input/farm_layout/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      250 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/input/farm_layout/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3169 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/input/farm_layout/from_csv.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      547 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/input/farm_layout/from_df.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1553 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/input/farm_layout/from_file.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1618 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/input/farm_layout/from_json.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1444 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/input/farm_layout/grid.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1175 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/input/farm_layout/row.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.006762 foxes-0.3.5/foxes/input/states/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      278 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/input/states/__init__.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.006762 foxes-0.3.5/foxes/input/states/create/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)       81 2023-06-02 08:05:43.000000 foxes-0.3.5/foxes/input/states/create/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3247 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/input/states/create/random_abl_states.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    15926 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/input/states/field_data_nc.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    12343 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/input/states/multi_height.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4362 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/input/states/scan_ws.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5734 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/input/states/single.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    10481 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/input/states/states_table.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.006762 foxes-0.3.5/foxes/input/windio/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)       88 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/input/windio/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     8679 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/input/windio/windio.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.006762 foxes-0.3.5/foxes/models/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      375 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/__init__.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.006762 foxes-0.3.5/foxes/models/farm_controllers/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)       71 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/farm_controllers/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      211 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/models/farm_controllers/basic.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.006762 foxes-0.3.5/foxes/models/farm_models/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)       65 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/farm_models/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3347 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/models/farm_models/turbine2farm.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    13156 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/model_book.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.006762 foxes-0.3.5/foxes/models/partial_wakes/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      241 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/partial_wakes/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    10383 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/partial_wakes/axiwake.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    10685 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/partial_wakes/distsliced.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2571 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/models/partial_wakes/grid.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     7397 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/partial_wakes/mapped.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     6126 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/partial_wakes/rotor_points.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     9578 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/partial_wakes/top_hat.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/foxes/models/point_models/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      130 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/point_models/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4430 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/point_models/set_uniform_data.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1372 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/models/point_models/tke2ti.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1935 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/models/point_models/wake_deltas.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/foxes/models/rotor_models/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)       82 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/rotor_models/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5587 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/rotor_models/centre.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4840 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/rotor_models/grid.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/foxes/models/turbine_models/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      419 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/turbine_models/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2531 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/turbine_models/calculator.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2757 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/turbine_models/kTI_model.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5410 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/turbine_models/power_mask.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4415 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/turbine_models/rotor_centre_calc.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     7541 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/turbine_models/sector_management.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3392 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/turbine_models/set_XYHD.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3846 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/turbine_models/set_farm_vars.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5120 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/models/turbine_models/table_factors.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2060 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/models/turbine_models/thrust2ct.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1580 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/models/turbine_models/yaw2yawm.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1551 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/models/turbine_models/yawm2yaw.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/foxes/models/turbine_types/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1429 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/turbine_types/CpCt_file.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2131 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/turbine_types/CpCt_from_two.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     7723 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/turbine_types/PCt_file.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     8853 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/turbine_types/PCt_from_two.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      250 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/turbine_types/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1284 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/models/turbine_types/null_type.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    11067 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/turbine_types/wsrho2PCt_two_files.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/foxes/models/vertical_profiles/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)       93 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/vertical_profiles/__init__.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/foxes/models/vertical_profiles/abl_log/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      289 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/vertical_profiles/abl_log/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1082 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/models/vertical_profiles/abl_log/abl_log_neutral_ws.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1161 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/models/vertical_profiles/abl_log/abl_log_stable_ws.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1173 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/models/vertical_profiles/abl_log/abl_log_unstable_ws.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2495 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/models/vertical_profiles/abl_log/abl_log_ws.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1148 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/vertical_profiles/abl_log/sheared_ws.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      375 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/models/vertical_profiles/uniform.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/foxes/models/wake_frames/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      164 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/wake_frames/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4675 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/wake_frames/farm_order.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3732 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/wake_frames/rotor_wd.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    11876 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/wake_frames/streamlines.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     8181 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/wake_frames/yawed_wakes.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/foxes/models/wake_models/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      228 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/wake_models/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2672 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/models/wake_models/axisymmetric.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     6506 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/wake_models/dist_sliced.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2637 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/models/wake_models/gaussian.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/foxes/models/wake_models/ti/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      124 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/wake_models/ti/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     8307 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/wake_models/ti/crespo_hernandez.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     6126 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/wake_models/ti/iec_ti.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5037 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/wake_models/top_hat.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/foxes/models/wake_models/wind/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      212 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/wake_models/wind/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5463 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/wake_models/wind/bastankhah.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4954 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/wake_models/wind/jensen.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    14670 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/wake_models/wind/porte_agel.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    11887 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/wake_models/wind/turbopark.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/foxes/models/wake_superpositions/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      236 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/wake_superpositions/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5888 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/wake_superpositions/linear.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     6676 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/wake_superpositions/max.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3783 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/wake_superpositions/product.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     6469 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/wake_superpositions/quadratic.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4756 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/wake_superpositions/ti_superp.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/foxes/opt/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      171 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/__init__.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/foxes/opt/constraints/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      158 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/constraints/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5927 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/constraints/area_geometry.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     7419 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/constraints/min_dist.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/foxes/opt/core/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      288 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/core/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1937 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/core/farm_constraint.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1936 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/core/farm_objective.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     9497 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/core/farm_opt_problem.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     7766 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/core/farm_vars_problem.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5600 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/core/pop_states.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/foxes/opt/objectives/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      152 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/objectives/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     8807 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/objectives/farm_vars.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4050 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/objectives/max_n_turbines.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/foxes/opt/problems/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      102 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/problems/__init__.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/foxes/opt/problems/layout/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      228 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/problems/layout/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5753 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/problems/layout/farm_layout.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/foxes/opt/problems/layout/geom_layouts/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      385 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/problems/layout/geom_layouts/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     8090 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/problems/layout/geom_layouts/constraints.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     8052 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/problems/layout/geom_layouts/geom_layout.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     7474 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/problems/layout/geom_layouts/geom_layout_gridded.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     9992 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/problems/layout/geom_layouts/geom_reggrid.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    14102 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/problems/layout/geom_layouts/geom_reggrids.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     6271 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/problems/layout/geom_layouts/objectives.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    11691 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/problems/layout/reggrids_layout.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    10534 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/problems/layout/regular_layout.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    19545 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/problems/opt_farm_vars.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/foxes/output/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      391 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/output/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    10553 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/output/farm_layout.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    15706 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/output/farm_results_eval.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    45193 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/output/flow_plots_2d.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2189 2023-06-02 08:05:43.000000 foxes-0.3.5/foxes/output/output.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2580 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/output/results_writer.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     9997 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/output/rose_plot.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2347 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/output/state_turbine_map.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5450 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/output/turbine_type_curves.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/foxes/utils/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      480 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/utils/__init__.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/foxes/utils/abl/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      134 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/utils/abl/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1278 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/utils/abl/neutral.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      442 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/utils/abl/sheared.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1728 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/utils/abl/stable.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1530 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/utils/abl/unstable.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3308 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/utils/cubic_roots.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5141 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/utils/data_book.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      793 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/utils/dict.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/foxes/utils/geom2d/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      217 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/utils/geom2d/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    18791 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/utils/geom2d/area_geometry.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4450 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/utils/geom2d/circle.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1626 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/utils/geom2d/example_intersection.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1750 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/utils/geom2d/example_union.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     6090 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/utils/geom2d/half_plane.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5462 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/utils/geom2d/polygon.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     7842 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/utils/geopandas_helpers.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4618 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/utils/pandas_helpers.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      350 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/utils/plotly_helpers.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5792 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/utils/runners.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      362 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/utils/subclasses.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2758 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/utils/two_circles.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2746 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/utils/wind_dir.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3401 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/variables.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.006762 foxes-0.3.5/foxes.egg-info/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     6589 2023-06-02 09:25:47.000000 foxes-0.3.5/foxes.egg-info/PKG-INFO
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     7742 2023-06-02 09:25:47.000000 foxes-0.3.5/foxes.egg-info/SOURCES.txt
+-rw-r--r--   0 jonas     (1000) jonas     (1000)        1 2023-06-02 09:25:47.000000 foxes-0.3.5/foxes.egg-info/dependency_links.txt
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      195 2023-06-02 09:25:47.000000 foxes-0.3.5/foxes.egg-info/requires.txt
+-rw-r--r--   0 jonas     (1000) jonas     (1000)        6 2023-06-02 09:25:47.000000 foxes-0.3.5/foxes.egg-info/top_level.txt
+-rw-r--r--   0 jonas     (1000) jonas     (1000)        1 2023-06-02 09:25:47.000000 foxes-0.3.5/foxes.egg-info/zip-safe
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      185 2023-06-02 08:05:39.000000 foxes-0.3.5/pyproject.toml
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1131 2023-06-02 09:25:48.016762 foxes-0.3.5/setup.cfg
+-rw-r--r--   0 jonas     (1000) jonas     (1000)       69 2023-06-02 08:05:43.000000 foxes-0.3.5/setup.py
```

### Comparing `foxes-0.3.4/LICENSE` & `foxes-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `foxes-0.3.4/Logo_FOXES.svg` & `foxes-0.3.5/Logo_FOXES.svg`

 * *Files identical despite different names*

### Comparing `foxes-0.3.4/PKG-INFO` & `foxes-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxes
-Version: 0.3.4
+Version: 0.3.5
 Summary: Farm Optimization and eXtended yield Evaluation Software
 Author: Fraunhofer IWES
 Author-email: jonas.schmidt@iwes.fraunhofer.de
 License: MIT
 Project-URL: Source Code, https://github.com/FraunhoferIWES/foxes
 Project-URL: Bug Tracker, https://github.com/FraunhoferIWES/foxes/issues
 Project-URL: Documentation, https://fraunhoferiwes.github.io/foxes.docs/index.html
```

### Comparing `foxes-0.3.4/README.md` & `foxes-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `foxes-0.3.4/foxes/__init__.py` & `foxes-0.3.5/foxes/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
 Farm Optimization and eXtended yield Evaluation Software
+    
 """
 from .core import WindFarm, Turbine  # noqa: F401
 from .models import ModelBook  # noqa: F401
 from .data import (
     parse_Pct_file_name,
     parse_Pct_two_files,
     FARM,
```

### Comparing `foxes-0.3.4/foxes/algorithms/downwind/downwind.py` & `foxes-0.3.5/foxes/algorithms/downwind/downwind.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from foxes.core import Algorithm, FarmDataModelList
 from foxes.core import PointDataModel, PointDataModelList
 import foxes.algorithms.downwind.models as dm
 import foxes.models as fm
 import foxes.variables as FV
 import foxes.constants as FC
 
-
 class Downwind(Algorithm):
     """
     The downwind algorithm.
 
     The turbines are evaluated once, in the order
     that is calculated by the provided `TurbineOrder`
     object.
@@ -65,26 +64,26 @@
         The number of states
 
     """
 
     FarmWakesCalculation = dm.FarmWakesCalculation
     PointWakesCalculation = dm.point_wakes_calc.PointWakesCalculation
     SetAmbPointResults = dm.set_amb_point_results.SetAmbPointResults
-    
+
     def __init__(
         self,
         mbook,
         farm,
         states,
         wake_models,
         rotor_model="centre",
         wake_frame="rotor_wd",
         partial_wakes_model="auto",
         farm_controller="basic_ctrl",
-        chunks={FV.STATE: 1000},
+        chunks={FC.STATE: 1000},
         dbook=None,
         keep_models=[],
         verbosity=1,
     ):
         super().__init__(mbook, farm, chunks, verbosity, dbook, keep_models)
 
         self.states = states
@@ -137,47 +136,47 @@
             self.print(f"    {i}) {m} [pre-rotor]")
         for i, m in enumerate(self.farm_controller.post_rotor_models.models):
             self.print(
                 f"    {i+len(self.farm_controller.pre_rotor_models.models)}) {m}"
             )
         self.print(deco)
         self.print()
-    
+
     def init_states(self):
         """
         Initialize states, if needed.
         """
         if not self.states.initialized:
             self.update_idata(self.states)
             self.n_states = self.states.size()
 
     def initialize(self):
         """
-        Initializes the algorithm.          
+        Initializes the algorithm.
         """
         self.print(f"\nInitializing algorithm '{self.name}'")
-        super().initialize()           
+        super().initialize()
 
         self.init_states()
 
         mdls = [
             self.rotor_model,
             self.farm_controller,
             self.wake_frame,
             self.partial_wakes_model,
         ] + self.wake_models
 
         self.update_idata(mdls)
 
     def _collect_farm_models(
-            self,
-            vars_to_amb,
-            calc_parameters,
-            ambient,
-        ):
+        self,
+        vars_to_amb,
+        calc_parameters,
+        ambient,
+    ):
         """
         Helper function that creates model list
         """
         # prepare:
         calc_pars = []
         t2f = fm.farm_models.Turbine2FarmModel
         mlist = FarmDataModelList(models=[])
@@ -273,15 +272,16 @@
             self.initialize()
 
         # welcome:
         self._print_deco("calc_farm")
 
         # collect models:
         mlist, calc_pars = self._collect_farm_models(
-            vars_to_amb, calc_parameters, ambient)
+            vars_to_amb, calc_parameters, ambient
+        )
 
         # initialize models and get input model data:
         self.update_idata(mlist)
         models_data = self.get_models_data()
         if persist:
             models_data = models_data.persist()
         self.print("\nInput data:\n\n", models_data, "\n")
@@ -291,15 +291,15 @@
         # run main calculation:
         self.print(
             f"\nCalculating {self.n_states} states for {self.n_turbines} turbines"
         )
         farm_results = mlist.run_calculation(
             self, models_data, out_vars=self.farm_vars, parameters=calc_pars
         )
-        farm_results[FV.TNAME] = ((FV.TURBINE,), self.farm.turbine_names)
+        farm_results[FC.TNAME] = ((FC.TURBINE,), self.farm.turbine_names)
         if FV.ORDER in farm_results:
             farm_results[FV.ORDER] = farm_results[FV.ORDER].astype(FC.ITYPE)
         del models_data
 
         # finalize models:
         if finalize:
             self.print("\n")
@@ -309,21 +309,21 @@
         if ambient:
             dvars = [v for v in farm_results.data_vars.keys() if v in FV.var2amb]
             farm_results = farm_results.drop_vars(dvars)
 
         return farm_results
 
     def _collect_point_models(
-            self,
-            vars,
-            vars_to_amb,
-            calc_parameters,
-            point_models,
-            ambient,
-        ):
+        self,
+        vars,
+        vars_to_amb,
+        calc_parameters,
+        point_models,
+        ambient,
+    ):
         """
         Helper function that creates model list
         """
         # prepare:
         calc_pars = []
         mlist = PointDataModelList(models=[])
 
@@ -430,35 +430,36 @@
             )
 
         # welcome:
         self._print_deco("calc_points", n_points=points.shape[1])
 
         # collect models:
         mlist, calc_pars = self._collect_point_models(
-            vars, vars_to_amb, calc_parameters, point_models, ambient)
+            vars, vars_to_amb, calc_parameters, point_models, ambient
+        )
 
         # initialize models and get input model data:
         self.update_idata(mlist)
         models_data = self.get_models_data()
         if persist_mdata:
             models_data = models_data.persist()
         self.print("\nInput data:\n\n", models_data, "\n")
         self.print(f"\nOutput farm variables:", ", ".join(self.farm_vars))
         self.print(f"\nChunks: {self.chunks}\n")
 
         # chunk farm results:
         if self.chunks is not None:
-            farm_results = farm_results.chunk(chunks={FV.STATE: self.chunks[FV.STATE]})
+            farm_results = farm_results.chunk(chunks={FC.STATE: self.chunks[FC.STATE]})
         self.print("\nInput farm data:\n\n", farm_results, "\n")
 
         # get point data:
-        if FV.STATE in farm_results.coords:
-            sinds = farm_results.coords[FV.STATE]
-        elif models_data is not None and FV.STATE in models_data.coords:
-            sinds = models_data.coords[FV.STATE]
+        if FC.STATE in farm_results.coords:
+            sinds = farm_results.coords[FC.STATE]
+        elif models_data is not None and FC.STATE in models_data.coords:
+            sinds = models_data.coords[FC.STATE]
         else:
             sinds = None
         point_data = self.new_point_data(points, sinds)
         if persist_pdata:
             point_data = point_data.persist()
         self.print("\nInput point data:\n\n", point_data, "\n")
 
@@ -511,12 +512,12 @@
         mdls = [
             self.states,
             self.rotor_model,
             self.farm_controller,
             self.wake_frame,
             self.partial_wakes_model,
         ] + self.wake_models
-        
+
         for m in mdls:
             self.finalize_model(m)
 
         super().finalize(clear_mem)
```

### Comparing `foxes-0.3.4/foxes/algorithms/downwind/models/calc_order.py` & `foxes-0.3.5/foxes/algorithms/downwind/models/calc_order.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.4/foxes/algorithms/downwind/models/farm_wakes_calc.py` & `foxes-0.3.5/foxes/algorithms/downwind/models/farm_wakes_calc.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         idata : dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         self.pwakes = algo.partial_wakes_model
-        
+
         idata = super().initialize(algo, verbosity)
         algo.update_idata(self.pwakes, idata=idata, verbosity=verbosity)
 
         return idata
 
     def calculate(self, algo, mdata, fdata):
         """ "
@@ -87,19 +87,17 @@
         torder = fdata[FV.ORDER]
         n_order = torder.shape[1]
         n_states = mdata.n_states
 
         wdeltas = self.pwakes.new_wake_deltas(algo, mdata, fdata)
 
         for oi in range(n_order):
-
             o = torder[:, oi]
 
             if oi > 0:
-
                 self.pwakes.evaluate_results(
                     algo, mdata, fdata, wdeltas, states_turbine=o
                 )
 
                 trbs = np.zeros((n_states, algo.n_turbines), dtype=bool)
                 np.put_along_axis(trbs, o[:, None], True, axis=1)
```

### Comparing `foxes-0.3.4/foxes/algorithms/downwind/models/point_wakes_calc.py` & `foxes-0.3.5/foxes/algorithms/downwind/models/point_wakes_calc.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,17 @@
         -------
         idata : dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
-        self.pvars = algo.states.output_point_vars(algo) if self._pvars is None else self._pvars
+        self.pvars = (
+            algo.states.output_point_vars(algo) if self._pvars is None else self._pvars
+        )
 
         idata = super().initialize(algo, verbosity)
         if self.emodels is not None:
             algo.update_idata(self.emodels, idata=idata, verbosity=verbosity)
 
         return idata
 
@@ -105,28 +107,27 @@
         results : dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_points)
 
         """
         torder = fdata[FV.ORDER].astype(FC.ITYPE)
         n_order = torder.shape[1]
-        points = pdata[FV.POINTS]
+        points = pdata[FC.POINTS]
 
         wdeltas = {}
         wmodels = []
         for w in algo.wake_models:
             hdeltas = {}
             w.init_wake_deltas(algo, mdata, fdata, pdata.n_points, hdeltas)
             if len(set(self.pvars).intersection(hdeltas.keys())):
                 wdeltas.update(hdeltas)
                 wmodels.append(w)
             del hdeltas
 
         for oi in range(n_order):
-
             o = torder[:, oi]
             wcoos = algo.wake_frame.get_wake_coos(algo, mdata, fdata, o, points)
 
             for w in wmodels:
                 w.contribute_to_wake_deltas(algo, mdata, fdata, o, wcoos, wdeltas)
 
         amb_res = {v: pdata[FV.var2amb[v]] for v in wdeltas}
```

### Comparing `foxes-0.3.4/foxes/algorithms/downwind/models/set_amb_farm_results.py` & `foxes-0.3.5/foxes/algorithms/downwind/models/set_amb_farm_results.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.4/foxes/algorithms/downwind/models/set_amb_point_results.py` & `foxes-0.3.5/foxes/algorithms/downwind/models/set_amb_point_results.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,18 +24,24 @@
 
     def __init__(self, point_vars=None, vars_to_amb=None):
         super().__init__()
         self._pvars = point_vars
         self._vars = vars_to_amb
 
     def initialize(self, algo, verbosity=0):
-        self.pvars = algo.states.output_point_vars(algo) if self._pvars is None else self._pvars
-        self.vars = [v for v in self.pvars if v in FV.var2amb] if self._vars is None else self._vars
+        self.pvars = (
+            algo.states.output_point_vars(algo) if self._pvars is None else self._pvars
+        )
+        self.vars = (
+            [v for v in self.pvars if v in FV.var2amb]
+            if self._vars is None
+            else self._vars
+        )
         return super().initialize(algo, verbosity)
-        
+
     def output_point_vars(self, algo):
         for v in algo.states.output_point_vars(algo):
             if v not in self.vars and v in FV.var2amb:
                 self.vars.append(v)
         return [FV.var2amb[v] for v in self.vars]
 
     def calculate(self, algo, mdata, fdata, pdata):
```

### Comparing `foxes-0.3.4/foxes/algorithms/iterative/iterative.py` & `foxes-0.3.5/foxes/algorithms/iterative/iterative.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,40 +33,41 @@
         Throw error if not converging
 
     """
 
     FarmWakesCalculation = FarmWakesCalculation
 
     def __init__(
-            self, 
-            *args, 
-            conv=DefaultConv(), 
-            max_its=None, 
-            conv_error=True,
-            **kwargs
-        ):
+        self, *args, conv=DefaultConv(), max_its=None, conv_error=True, **kwargs
+    ):
         super().__init__(*args, **kwargs)
         self.conv = conv
         self.max_its = max_its
         self.conv_error = conv_error
 
     def _collect_farm_models(
-            self,
-            vars_to_amb,
-            calc_parameters,
-            ambient,
-        ):
+        self,
+        vars_to_amb,
+        calc_parameters,
+        ambient,
+    ):
         """
         Helper function that creates model list
         """
         # get models from Downwind algorithm:
         mlist, calc_pars = super()._collect_farm_models(
-            vars_to_amb, calc_parameters, ambient)
+            vars_to_amb, calc_parameters, ambient
+        )
 
         # wrap the models into a loop:
-        mlist = LoopRunner(self.conv, mlist.models, max_its=self.max_its, 
-                            conv_error=self.conv_error, verbosity=self.verbosity-1)
+        mlist = LoopRunner(
+            self.conv,
+            mlist.models,
+            max_its=self.max_its,
+            conv_error=self.conv_error,
+            verbosity=self.verbosity - 1,
+        )
 
         # flag only the last model as wake relevant:
-        mlist.model_wflag[-1] = True 
+        mlist.model_wflag[-1] = True
 
         return mlist, calc_pars
```

### Comparing `foxes-0.3.4/foxes/algorithms/iterative/models/convergence.py` & `foxes-0.3.5/foxes/algorithms/iterative/models/convergence.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,57 +1,60 @@
 import numpy as np
 from abc import ABCMeta, abstractmethod
 
 import foxes.variables as FV
 from foxes.utils import delta_wd
 
+
 class ConvCrit(metaclass=ABCMeta):
     """
     Abstract base class for convergence criteria
 
     Parameters
     ----------
     name : str, optional
         The convergence criteria name
-    
+
     Attribute
     ---------
     name : str, optional
         The convergence criteria name
 
     """
+
     def __init__(self, name=None):
         self.name = name if name is not None else type(self).__name__
-        
+
     @abstractmethod
     def check_converged(self, algo, fdata0, fdata1, verbosity=0):
         """
         Check convergence criteria.
 
         Parameters
         ----------
         algo : foxes.core.Algorithm
             The calculation algorithm
         fdata0 : foxes.core.Data
-            The farm data results of previous 
+            The farm data results of previous
             iteration, or None if first
         fdata1 : foxes.core.Data
-            The farm data results of current 
+            The farm data results of current
             iteration, or None if first
         verbosity : int
             The verbosity level, 0 = silent
 
         Returns
         -------
         convergence : bool
             Convergence flag, true if converged
 
         """
         pass
 
+
 class ConvCritList(ConvCrit):
     """
     A list of convergence criteria
 
     Parameters
     ----------
     crits : list of ConvCrit
@@ -61,59 +64,61 @@
 
     Attributes
     ----------
     crits : list of ConvCrit
         The criteria
 
     """
+
     def __init__(self, crits=[], name=None):
         super().__init__(name)
         self.crits = crits
-    
+
     def add_crit(self, crit):
         """
         Add a convergence criterion
 
         Parameters
         ----------
         crit : ConvCrit
             The criterion
 
         """
         self.crits.append(crit)
-    
+
     def check_converged(self, algo, fdata0, fdata1, verbosity=0):
         """
         Check convergence criteria.
 
         Parameters
         ----------
         algo : foxes.core.Algorithm
             The calculation algorithm
         fdata0 : foxes.core.Data
-            The farm data results of previous 
+            The farm data results of previous
             iteration, or None if first
         fdata1 : foxes.core.Data
-            The farm data results of current 
+            The farm data results of current
             iteration, or None if first
         verbosity : int
             The verbosity level, 0 = silent
 
         Returns
         -------
         convergence : bool
             Convergence flag, true if converged
 
         """
         for c in self.crits:
             if not c.check_converged(algo, fdata0, fdata1, verbosity):
                 return False
-        
+
         return True
-    
+
+
 class ConvVarDelta(ConvCrit):
     """
     Requires convergence of a selection of variables.
 
     Parameters
     ----------
     limits : dict
@@ -129,14 +134,15 @@
     limits : dict
         The convergence limits. Keys: variables str,
         values: float values
     wd_vars : list of str
         The wind direction type variables (unit deg)
 
     """
+
     def __init__(self, limits, wd_vars=None, name=None):
         super().__init__(name)
         self.limits = limits
         if wd_vars is None:
             self.wd_vars = [FV.WD, FV.AMB_WD, FV.YAW, FV.AMB_YAW]
         else:
             self.wd_vars = wd_vars
@@ -146,54 +152,57 @@
         Check convergence criteria.
 
         Parameters
         ----------
         algo : foxes.core.Algorithm
             The calculation algorithm
         fdata0 : foxes.core.Data
-            The farm data results of previous 
+            The farm data results of previous
             iteration, or None if first
         fdata1 : foxes.core.Data
-            The farm data results of current 
+            The farm data results of current
             iteration, or None if first
         verbosity : int
             The verbosity level, 0 = silent
 
         Returns
         -------
         convergence : bool
             Convergence flag, true if converged
 
         """
         if fdata0 is None:
             return False
-        
+
         if verbosity > 0:
             print(f"\n{self.name}: Convergence check")
-        
+
         ok = True
         for v, lim in self.limits.items():
-
             if v in self.wd_vars:
                 check = np.max(np.abs(delta_wd(fdata0[v], fdata1[v])))
             else:
                 check = np.max(np.abs(fdata1[v] - fdata0[v]))
             ok = ok and (check <= lim)
-            
+
             if verbosity > 0:
                 r = "FAILED" if check > lim else "OK"
                 print(f"  {v}: delta = {check}, lim = {lim}  --  {r}")
             elif not ok:
                 break
-            
+
         return ok
 
+
 class DefaultConv(ConvVarDelta):
     """
     Default convergence criteria.
     """
+
     def __init__(self):
-        super().__init__({
-            FV.REWS: 1e-5,
-            FV.WD: 1e-4,
-            FV.TI: 1e-6,
-        })
+        super().__init__(
+            {
+                FV.REWS: 1e-5,
+                FV.WD: 1e-4,
+                FV.TI: 1e-6,
+            }
+        )
```

### Comparing `foxes-0.3.4/foxes/algorithms/iterative/models/farm_wakes_calc.py` & `foxes-0.3.5/foxes/algorithms/iterative/models/farm_wakes_calc.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,19 +91,16 @@
         wdeltas = self.pwakes.new_wake_deltas(algo, mdata, fdata)
 
         for oi in range(n_order):
             o = torder[:, oi]
             self.pwakes.contribute_to_wake_deltas(algo, mdata, fdata, o, wdeltas)
 
         for oi in range(n_order):
-
             o = torder[:, oi]
-            self.pwakes.evaluate_results(
-                algo, mdata, fdata, wdeltas, states_turbine=o
-            )
+            self.pwakes.evaluate_results(algo, mdata, fdata, wdeltas, states_turbine=o)
 
             trbs = np.zeros((n_states, algo.n_turbines), dtype=bool)
             np.put_along_axis(trbs, o[:, None], True, axis=1)
 
             res = algo.farm_controller.calculate(
                 algo, mdata, fdata, pre_rotor=False, st_sel=trbs
             )
```

### Comparing `foxes-0.3.4/foxes/algorithms/iterative/models/loop_runner.py` & `foxes-0.3.5/foxes/algorithms/iterative/models/loop_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,27 +37,30 @@
         number of turbines + 1
     conv_error : bool
         Throw error if not converging
     verbosity : int
         The verbosity level, 0 = silent
 
     """
+
     def __init__(
-            self, 
-            conv, 
-            models=[], 
-            model_wflag=None, 
-            max_its=None, 
-            conv_error=True,
-            verbosity=0
-        ):
+        self,
+        conv,
+        models=[],
+        model_wflag=None,
+        max_its=None,
+        conv_error=True,
+        verbosity=0,
+    ):
         super().__init__(models=models)
         self.conv = conv
-        self.verbosity=verbosity
-        self.model_wflag = [False for m in models] if model_wflag is None else model_wflag
+        self.verbosity = verbosity
+        self.model_wflag = (
+            [False for m in models] if model_wflag is None else model_wflag
+        )
         self.max_its = max_its
         self.conv_error = conv_error
 
     def append(self, model, wflag=False):
         """
         Add a model to the list
 
@@ -97,34 +100,35 @@
             Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
         fdata0 = None
         it = 0
         max_its = algo.n_turbines + 1 if self.max_its is None else self.max_its
         while it < max_its:
-
             if self.verbosity > 0:
                 print(f"\n{self.name}: Running iteration {it} (max_its = {max_its})\n")
 
             # run all models at first iteration:
             if fdata0 is None:
                 results = super().calculate(algo, mdata, fdata, parameters)
                 fdata.update(results)
-            
+
             # only run wake relevant models after first iteration:
             else:
                 for mi, m in enumerate(self.models):
                     if self.model_wflag[mi]:
                         results = m.calculate(algo, mdata, fdata, **parameters[mi])
                         fdata.update(results)
             del results
-            
+
             if self.conv.check_converged(self, fdata0, fdata, verbosity=self.verbosity):
                 break
             else:
                 fdata0 = deepcopy(fdata)
                 it += 1
-        
+
         if it >= max_its and self.conv_error:
-            raise ValueError(f"{self.name}: Maximal numer of iterations {max_its} reached, not converging.")
-        
+            raise ValueError(
+                f"{self.name}: Maximal numer of iterations {max_its} reached, not converging."
+            )
+
         return {v: fdata[v] for v in self.output_farm_vars(algo)}
```

### Comparing `foxes-0.3.4/foxes/core/__init__.py` & `foxes-0.3.5/foxes/core/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""
+Abstract classes and core functionality.
+"""
 from .data import Data
 from .model import Model
 from .data_calc_model import DataCalcModel
 from .states import States, ExtendedStates
 from .wind_farm import WindFarm
 from .algorithm import Algorithm
 from .farm_data_model import FarmDataModel, FarmDataModelList
```

### Comparing `foxes-0.3.4/foxes/core/algorithm.py` & `foxes-0.3.5/foxes/core/algorithm.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from .model import Model
 from .farm_data_model import FarmDataModelList
 from .point_data_model import PointDataModelList
 from .farm_controller import FarmController
 from foxes.data import StaticData
 from foxes.utils import Dict, all_subclasses
 import foxes.variables as FV
+import foxes.constants as FC
+
 
 class Algorithm(Model):
     """
     Abstract base class for algorithms.
 
     Algorithms collect required objects for running
     calculations, and contain the calculation functions
@@ -29,15 +31,15 @@
     verbosity : int
         The verbosity level, 0 means silent
     dbook : foxes.DataBook, optional
         The data book, or None for default
     keep_models : list of str
         Keep these models data in memory and do not finalize them
 
-    Parameters
+    Attributes
     ----------
     mbook : foxes.ModelBook
         The model book
     farm : foxes.WindFarm
         The wind farm
     chunks : dict
         The chunks choice for running in parallel with dask,
@@ -97,27 +99,27 @@
                 raise ValueError(
                     f"Input {mtype} data entry '{v}': Second entry is not a numpy array, got: {type(t[1]).__name__}"
                 )
             if len(t[1].shape) != len(t[0]):
                 raise ValueError(
                     f"Input {mtype} data entry '{v}': Wrong data shape, expecting {len(t[0])} dimensions, got {t[1].shape}"
                 )
-            if FV.STATE in t[0]:
-                if t[0][0] != FV.STATE:
+            if FC.STATE in t[0]:
+                if t[0][0] != FC.STATE:
                     raise ValueError(
-                        f"Input {mtype} data entry '{v}': Dimension '{FV.STATE}' not at first position, got {t[0]}"
+                        f"Input {mtype} data entry '{v}': Dimension '{FC.STATE}' not at first position, got {t[0]}"
                     )
-                if FV.POINT in t[0] and t[0][1] != FV.POINT:
+                if FC.POINT in t[0] and t[0][1] != FC.POINT:
                     raise ValueError(
-                        f"Input {mtype} data entry '{v}': Dimension '{FV.POINT}' not at second position, got {t[0]}"
+                        f"Input {mtype} data entry '{v}': Dimension '{FC.POINT}' not at second position, got {t[0]}"
                     )
-            elif FV.POINT in t[0]:
-                if t[0][0] != FV.POINT:
+            elif FC.POINT in t[0]:
+                if t[0][0] != FC.POINT:
                     raise ValueError(
-                        f"Input {mtype} data entry '{v}': Dimension '{FV.POINT}' not at first position, got {t[0]}"
+                        f"Input {mtype} data entry '{v}': Dimension '{FC.POINT}' not at first position, got {t[0]}"
                     )
             for d, s in zip(t[0], t[1].shape):
                 if d not in sizes:
                     sizes[d] = s
                 elif sizes[d] != s:
                     raise ValueError(
                         f"Input {mtype} data entry '{v}': Dimension '{d}' has wrong size, expecting {sizes[d]}, got {s}"
@@ -136,21 +138,21 @@
 
     def __get_xrdata(self, idata, sizes):
         """
         Private helper function
         """
         xrdata = xr.Dataset(**idata)
         if self.chunks is not None:
-            if FV.TURBINE in self.chunks.keys():
+            if FC.TURBINE in self.chunks.keys():
                 raise ValueError(
-                    f"Dimension '{FV.TURBINE}' cannot be chunked, got chunks {self.chunks}"
+                    f"Dimension '{FC.TURBINE}' cannot be chunked, got chunks {self.chunks}"
                 )
-            if FV.RPOINT in self.chunks.keys():
+            if FC.RPOINT in self.chunks.keys():
                 raise ValueError(
-                    f"Dimension '{FV.RPOINT}' cannot be chunked, got chunks {self.chunks}"
+                    f"Dimension '{FC.RPOINT}' cannot be chunked, got chunks {self.chunks}"
                 )
             xrdata = xrdata.chunk(
                 chunks={c: v for c, v in self.chunks.items() if c in sizes}
             )
         return xrdata
 
     def initialize(self):
@@ -168,47 +170,51 @@
         models : foxes.core.Model or list of foxes.core.Model
             The models to initialize
         idata : dict, optional
             The idata dictionary to be updated, else only add
             to idata memory
         verbosity : int, optional
             The verbosity level, 0 = silent
-            
+
         """
         if idata is None and not self.initialized:
-            raise ValueError(f"Algorithm '{self.name}': update_idata called before initialization")
-        
+            raise ValueError(
+                f"Algorithm '{self.name}': update_idata called before initialization"
+            )
+
         verbosity = self.verbosity if verbosity is None else verbosity
 
         if not isinstance(models, list) and not isinstance(models, tuple):
             models = [models]
 
         for m in models:
-
             pr = False
             if m.initialized:
                 try:
                     hidata = self._idata_mem[m.name]
                 except KeyError:
-                    raise KeyError(f"Model '{m.name}' initialized but not found in idata memory")
+                    raise KeyError(
+                        f"Model '{m.name}' initialized but not found in idata memory"
+                    )
 
             else:
-
                 self.print(f"Initializing model '{m.name}'")
                 hidata = m.initialize(self, verbosity)
                 self._idata_mem[m.name] = hidata
 
                 pr = False
                 if isinstance(m, FarmController):
                     if verbosity > 1:
                         print(f"-- {m.name}: Starting sub-model initialization -- ")
                         pr = True
                     self.update_idata(m.pre_rotor_models, idata, verbosity)
                     self.update_idata(m.post_rotor_models, idata, verbosity)
-                elif isinstance(m, FarmDataModelList) or isinstance(m, PointDataModelList):
+                elif isinstance(m, FarmDataModelList) or isinstance(
+                    m, PointDataModelList
+                ):
                     if verbosity > 1:
                         print(f"-- {m.name}: Starting sub-model initialization -- ")
                         pr = True
                     for mm in m.models:
                         self.update_idata(mm, idata, verbosity)
 
             if idata is not None:
@@ -226,18 +232,18 @@
         Returns
         -------
         dict :
             Keys: model name, value: idata dict
 
         """
         return self._idata_mem
-    
+
     def update_n_turbines(self):
         """
-        Reset the number of turbines, 
+        Reset the number of turbines,
         according to self.farm
         """
         if self.n_turbines != self.farm.n_turbines:
             self.n_turbines = self.farm.n_turbines
 
             # resize stored idata, if dependent on turbine coord:
             newk = {}
@@ -246,34 +252,48 @@
                     continue
                 for dname, d in idata["data_vars"].items():
                     k = f"__{mname}_{dname}_turbinv"
                     if k in self.idata_mem:
                         ok = self.idata_mem[k]
                     else:
                         ok = None
-                        if FV.TURBINE in d[0]:
-                            i = d[0].index(FV.TURBINE)
-                            ok = (np.unique(d[1], axis=1).shape[i] == 1)
+                        if FC.TURBINE in d[0]:
+                            i = d[0].index(FC.TURBINE)
+                            ok = np.unique(d[1], axis=1).shape[i] == 1
                         newk[k] = ok
                     if ok is not None:
                         if not ok:
-                            raise ValueError(f"{self.name}: Stored idata entry '{mname}:{dname}' is turbine dependent, unable to reset n_turbines")
-                        if FV.TURBINE in idata["coords"]:
-                            idata["coords"][FV.TURBINE] = np.arange(self.n_turbines)
-                        i = d[0].index(FV.TURBINE)
+                            raise ValueError(
+                                f"{self.name}: Stored idata entry '{mname}:{dname}' is turbine dependent, unable to reset n_turbines"
+                            )
+                        if FC.TURBINE in idata["coords"]:
+                            idata["coords"][FC.TURBINE] = np.arange(self.n_turbines)
+                        i = d[0].index(FC.TURBINE)
                         n0 = d[1].shape[i]
                         if n0 > self.n_turbines:
-                            idata["data_vars"][dname] = (d[0], np.take(d[1], range(self.n_turbines), axis=i))
+                            idata["data_vars"][dname] = (
+                                d[0],
+                                np.take(d[1], range(self.n_turbines), axis=i),
+                            )
                         elif n0 < self.n_turbines:
-                            shp = [d[1].shape[j] if j != i else self.n_turbines-n0 for j in range(len(d[1].shape))]
+                            shp = [
+                                d[1].shape[j] if j != i else self.n_turbines - n0
+                                for j in range(len(d[1].shape))
+                            ]
                             a = np.zeros(shp, dtype=d[1].dtype)
-                            shp = [d[1].shape[j] if j != i else 1 for j in range(len(d[1].shape))]
+                            shp = [
+                                d[1].shape[j] if j != i else 1
+                                for j in range(len(d[1].shape))
+                            ]
                             a[:] = np.take(d[1], -1, axis=i).reshape(shp)
-                            idata["data_vars"][dname] = (d[0], np.append(d[1], a, axis=i))
-            
+                            idata["data_vars"][dname] = (
+                                d[0],
+                                np.append(d[1], a, axis=i),
+                            )
+
             self._idata_mem.update(newk)
 
     def get_models_data(self, idata=None):
         """
         Creates xarray from model input data.
 
         Parameters
@@ -288,15 +308,17 @@
         -------
         xarray.Dataset
             The model input data
 
         """
         if idata is None:
             if not self.initialized:
-                raise ValueError(f"Algorithm '{self.name}': get_models_data called before initialization")
+                raise ValueError(
+                    f"Algorithm '{self.name}': get_models_data called before initialization"
+                )
             idata = self._idata_mem.pop(self.name)
             mnames = [mname for mname in self._idata_mem.keys() if mname[:2] != "__"]
             for mname in mnames:
                 if mname in self.keep_models:
                     hidata = self._idata_mem.get(mname)
                 else:
                     hidata = self._idata_mem.pop(mname)
@@ -323,25 +345,25 @@
             A dataset containing the points data
 
         """
 
         if states_indices is None:
             idata = {"coords": {}, "data_vars": {}}
         else:
-            idata = {"coords": {FV.STATE: states_indices}, "data_vars": {}}
+            idata = {"coords": {FC.STATE: states_indices}, "data_vars": {}}
 
         if (
             len(points.shape) != 3
             or points.shape[0] != self.n_states
             or points.shape[2] != 3
         ):
             raise ValueError(
                 f"points have wrong dimensions, expecting ({self.n_states}, n_points, 3), got {points.shape}"
             )
-        idata["data_vars"][FV.POINTS] = ((FV.STATE, FV.POINT, FV.XYH), points)
+        idata["data_vars"][FC.POINTS] = ((FC.STATE, FC.POINT, FV.XYH), points)
 
         sizes = self.__get_sizes(idata, "point")
         return self.__get_xrdata(idata, sizes)
 
     def finalize_model(self, model, verbosity=None):
         """
         Call the finalization routine of the model,
@@ -353,38 +375,40 @@
             The model to be finalized, if not in the
             keep_models list
         verbosity : int, optional
             The verbosity level, 0 = silent
 
         """
         verbosity = self.verbosity if verbosity is None else verbosity
-  
+
         pr = False
         if isinstance(model, FarmController):
             if verbosity > 1:
                 print(f"Finalizing model '{model.name}'")
                 print(f"-- {model.name}: Starting sub-model finalization -- ")
                 pr = True
             self.finalize_model(model.pre_rotor_models, verbosity)
             self.finalize_model(model.post_rotor_models, verbosity)
-        elif isinstance(model, FarmDataModelList) or isinstance(model, PointDataModelList):
+        elif isinstance(model, FarmDataModelList) or isinstance(
+            model, PointDataModelList
+        ):
             if verbosity > 1:
                 print(f"Finalizing model '{model.name}'")
                 print(f"-- {model.name}: Starting sub-model finalization -- ")
                 pr = True
             for m in model.models:
                 self.finalize_model(m, verbosity)
 
         if model.initialized and model.name not in self.keep_models:
             if not pr and verbosity > 0:
                 print(f"Finalizing model '{model.name}'")
             model.finalize(self, verbosity)
             if model.name in self._idata_mem:
                 del self._idata_mem[model.name]
-        
+
         if pr:
             print(f"-- {model.name}: Finished sub-model finalization -- ")
 
     def finalize(self, clear_mem=False):
         """
         Finalizes the algorithm.
 
@@ -423,12 +447,13 @@
 
         if found:
             for scls in allc:
                 if scls.__name__ == algo_type:
                     return scls(*args, **kwargs)
 
         else:
-            estr = "Algorithm type '{}' is not defined, available types are \n {}".format(
-                algo_type, sorted([i.__name__ for i in allc])
+            estr = (
+                "Algorithm type '{}' is not defined, available types are \n {}".format(
+                    algo_type, sorted([i.__name__ for i in allc])
+                )
             )
             raise KeyError(estr)
-
```

### Comparing `foxes-0.3.4/foxes/core/data.py` & `foxes-0.3.5/foxes/core/data.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,48 +10,47 @@
     Container for data and meta data.
 
     Used during the calculation of single chunks,
     usually for numpy data (not xarray data).
 
     Parameters
     ----------
-    name : str
-        The data container name
     data : dict
         The initial data to be stored
     dims : dict
         The dimensions tuples, same or subset
         of data keys
     loop_dims : array_like of str
         List of the loop dimensions during xarray's
         `apply_ufunc` calculations
-
+    name : str
+        The data container name
+        
     Attributes
     ----------
     dims : dict
         The dimensions tuples, same or subset
         of data keys
     loop_dims : array_like of str
         List of the loop dimensions during xarray's
         `apply_ufunc` calculations
     sizes : dict
         The dimension sizes
 
     """
 
-    def __init__(self, data, dims, loop_dims):
+    def __init__(self, data, dims, loop_dims, name="data"):
         super().__init__(name="data")
 
         self.update(data)
         self.dims = dims
         self.loop_dims = loop_dims
 
         self.sizes = {}
         for v, d in data.items():
-
             dim = dims[v]
 
             # remove axes of size 1, added by dask for extra loop dimensions:
             if len(dim) != len(d.shape):
                 for li, l in enumerate(loop_dims):
                     if d.shape[li] == 1 and (len(dim) < li + 1 or dim[li] != l):
                         self[v] = np.squeeze(d, axis=li)
@@ -60,30 +59,29 @@
                 if c not in self.sizes:
                     self.sizes[c] = self[v].shape[ci]
                 elif self.sizes[c] != self[v].shape[ci]:
                     raise ValueError(
                         f"Inconsistent size for data entry '{v}', dimension '{c}': Expecting {self.sizes[c]}, found {self[v].shape[ci]} in shape {self[v].shape}"
                     )
 
-        if FV.STATE in self.sizes:
-            self.n_states = self.sizes[FV.STATE]
-        if FV.TURBINE in self.sizes:
-            self.n_turbines = self.sizes[FV.TURBINE]
-        if FV.POINT in self.sizes:
-            self.n_points = self.sizes[FV.POINT]
+        if FC.STATE in self.sizes:
+            self.n_states = self.sizes[FC.STATE]
+        if FC.TURBINE in self.sizes:
+            self.n_turbines = self.sizes[FC.TURBINE]
+        if FC.POINT in self.sizes:
+            self.n_points = self.sizes[FC.POINT]
 
         if (
             FV.X in data
             and FV.Y in data
             and FV.H in data
-            and dims[FV.X] == (FV.STATE, FV.TURBINE)
-            and dims[FV.Y] == (FV.STATE, FV.TURBINE)
-            and dims[FV.H] == (FV.STATE, FV.TURBINE)
+            and dims[FV.X] == (FC.STATE, FC.TURBINE)
+            and dims[FV.Y] == (FC.STATE, FC.TURBINE)
+            and dims[FV.H] == (FC.STATE, FC.TURBINE)
         ):
-
             self[FV.TXYH] = np.zeros(
                 (self.n_states, self.n_turbines, 3), dtype=FC.DTYPE
             )
 
             self[FV.TXYH][:, :, 0] = self[FV.X]
             self[FV.TXYH][:, :, 1] = self[FV.Y]
             self[FV.TXYH][:, :, 2] = self[FV.H]
```

### Comparing `foxes-0.3.4/foxes/core/data_calc_model.py` & `foxes-0.3.5/foxes/core/data_calc_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,17 @@
 from abc import abstractmethod
 from dask.distributed import progress
 from dask.diagnostics import ProgressBar
 
 from .model import Model
 from .data import Data
 from foxes.utils.runners import DaskRunner
-import foxes.variables as FV
 import foxes.constants as FC
 
 
-
 class DataCalcModel(Model):
     """
     Abstract base class for models with
     that run calculation on xarray Dataset
     data.
 
     The calculations are run via xarray's
@@ -71,15 +69,14 @@
         """
         Wrapper that mitigates between apply_ufunc and `calculate`.
         """
 
         # reconstruct original data:
         data = []
         for hvars in dvars:
-
             v2l = {v: lvars.index(v) for v in hvars if v in lvars}
             v2e = {v: evars.index(v) for v in hvars if v in evars}
 
             hdata = {v: ldata[v2l[v]] if v in v2l else edata[v2e[v]] for v in hvars}
             hdims = {v: ldims[v2l[v]] if v in v2l else edims[v2e[v]] for v in hvars}
 
             data.append(Data(hdata, hdims, loop_dims))
@@ -157,41 +154,42 @@
         out_vars: list of str
             The calculation output variables
         loop_dims : array_like of str
             List of the loop dimensions during xarray's
             `apply_ufunc` calculations
         out_core_vars : list of str
             The core dimensions of the output data, use
-            `FV.VARS` for variables dimension (required)
+            `FC.VARS` for variables dimension (required)
         **calc_pars : dict, optional
             Additional arguments for the `calculate` function
 
         Returns
         -------
         results : xarray.Dataset
             The calculation results
 
         """
         # check:
         if not self.initialized:
-            raise ValueError(f"DataCalcModel '{self.name}': run_calculation called for uninitialized model")
+            raise ValueError(
+                f"DataCalcModel '{self.name}': run_calculation called for uninitialized model"
+            )
 
         # prepare:
         loopd = set(loop_dims)
 
         # extract loop-var dependent and independent data:
         ldata = []
         lvars = []
         ldims = []
         edata = []
         evars = []
         edims = []
         dvars = []
         for ds in data:
-
             hvarsl = [v for v, d in ds.items() if len(loopd.intersection(d.dims))]
             ldata += [ds[v] for v in hvarsl]
             ldims += [ds[v].dims for v in hvarsl]
             lvars += hvarsl
 
             hvarse = [v for v in ds.keys() if v not in hvarsl]
             edata += [ds[v].values for v in hvarse]
@@ -207,24 +205,24 @@
                     edata.append(d.values)
                     edims.append((c,))
                     evars.append(c)
 
             dvars.append(list(ds.keys()) + list(ds.coords.keys()))
 
         # setup dask options:
-        dargs = dict(output_sizes={FV.VARS: len(out_vars)})
-        if FV.TURBINE in loopd and FV.TURBINE not in ldims.values():
-            dargs["output_sizes"][FV.TURBINE] = algo.n_turbines
-        if FV.VARS not in out_core_vars:
+        dargs = dict(output_sizes={FC.VARS: len(out_vars)})
+        if FC.TURBINE in loopd and FC.TURBINE not in ldims.values():
+            dargs["output_sizes"][FC.TURBINE] = algo.n_turbines
+        if FC.VARS not in out_core_vars:
             raise ValueError(
-                f"Model '{self.name}': Expecting '{FV.VARS}' in out_core_vars, got {out_core_vars}"
+                f"Model '{self.name}': Expecting '{FC.VARS}' in out_core_vars, got {out_core_vars}"
             )
 
         # setup arguments for wrapper function:
-        out_dims = loop_dims + list(set(out_core_vars).difference([FV.VARS]))
+        out_dims = loop_dims + list(set(out_core_vars).difference([FC.VARS]))
         wargs = dict(
             algo=algo,
             dvars=dvars,
             lvars=lvars,
             ldims=ldims,
             evars=evars,
             edims=edims,
@@ -245,16 +243,14 @@
             output_dtypes=[FC.DTYPE],
             dask="parallelized",
             dask_gufunc_kwargs=dargs,
             kwargs=wargs,
         )
 
         # reorganize results Dataset:
-        results = (
-            results.assign_coords({FV.VARS: out_vars}).to_dataset(dim=FV.VARS)
-        )
+        results = results.assign_coords({FC.VARS: out_vars}).to_dataset(dim=FC.VARS)
 
         if DaskRunner.is_distributed() and len(ProgressBar.active):
             progress(results.persist())
 
         # update data by calculation results:
         return results.compute()
```

### Comparing `foxes-0.3.4/foxes/core/farm_controller.py` & `foxes-0.3.5/foxes/core/farm_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import numpy as np
 
 from .farm_data_model import FarmDataModelList, FarmDataModel
 from .turbine_model import TurbineModel
 from .turbine_type import TurbineType
 import foxes.constants as FC
-import foxes.variables as FV
-
 
 class FarmController(FarmDataModel):
     """
     Analyses selected turbine models and handles their call.
 
     Parameters
     ----------
@@ -78,31 +76,28 @@
         mnames = [[m.name for m in mlist] for mlist in models]
         tmis = np.zeros(algo.n_turbines, dtype=FC.ITYPE)
         news = True
         while news:
             news = False
 
             for ti, mlist in enumerate(models):
-
                 if tmis[ti] < len(mlist):
-
                     mname = mnames[ti][tmis[ti]]
                     isnext = True
                     for tj, jnames in enumerate(mnames):
                         if (
                             tj != ti
                             and mname in jnames
                             and tmis[tj] < len(jnames)
                             and jnames[tmis[tj]] != mname
                         ):
                             isnext = False
                             break
 
                     if isnext:
-
                         m = models[ti][tmis[ti]]
                         tmodels.append(m)
 
                         tsel = np.zeros((algo.n_states, algo.n_turbines), dtype=bool)
                         for tj, jnames in enumerate(mnames):
                             mi = tmis[tj]
                             if mi < len(jnames) and jnames[mi] == mname:
@@ -146,15 +141,14 @@
         # check turbine models, and find turbine types and pre/post-rotor models:
         self.turbine_types = [None for t in algo.farm.turbines]
         prer_models = [[] for t in algo.farm.turbines]
         postr_models = [[] for t in algo.farm.turbines]
         for ti, t in enumerate(algo.farm.turbines):
             prer = None
             for mi, mname in enumerate(t.models):
-
                 istype = False
                 if mname in algo.mbook.turbine_types:
                     m = algo.mbook.turbine_types[mname]
                     if not isinstance(m, TurbineType):
                         raise TypeError(
                             f"Model {mname} type {type(m).__name__} is not derived from {TurbineType.__name__}"
                         )
@@ -168,15 +162,15 @@
                             raise TypeError(
                                 f"Model {mname} type {type(mm).__name__} is not derived from {TurbineModel.__name__}"
                             )
                 else:
                     raise KeyError(
                         f"Model {mname} not found in model book types or models"
                     )
-                    
+
                 if istype:
                     if self.turbine_types[ti] is None:
                         self.turbine_types[ti] = m
                     else:
                         raise ValueError(
                             f"Turbine {ti}, {t.name}: Multiple turbine types found in self.turbine_models list, {self.turbine_types[ti].name} and {mname}"
                         )
@@ -214,15 +208,15 @@
             raise ValueError(f"Controller '{self.name}': No turbine model found.")
 
     def __get_pars(self, algo, models, ptype, mdata=None, st_sel=None, from_data=True):
         """
         Private helper function for gathering model parameters.
         """
         if from_data:
-            s = mdata[FV.TMODEL_SELS]
+            s = mdata[FC.TMODEL_SELS]
         else:
             s = self.turbine_model_sels
         if st_sel is not None:
             s = s & st_sel[:, :, None]
 
         pars = [
             {"st_sel": s[:, :, self.turbine_model_names.index(m.name)]} for m in models
@@ -259,20 +253,20 @@
 
         """
         idata = super().initialize(algo, verbosity)
 
         self.collect_models(algo)
 
         # done by algo.update_idata
-        #algo.update_idata([self.pre_rotor_models, self.post_rotor_models], 
+        # algo.update_idata([self.pre_rotor_models, self.post_rotor_models],
         #    idata=idata, verbosity=verbosity)
 
-        idata["coords"][FV.TMODELS] = self.turbine_model_names
-        idata["data_vars"][FV.TMODEL_SELS] = (
-            (FV.STATE, FV.TURBINE, FV.TMODELS),
+        idata["coords"][FC.TMODELS] = self.turbine_model_names
+        idata["data_vars"][FC.TMODEL_SELS] = (
+            (FC.STATE, FC.TURBINE, FC.TMODELS),
             self.turbine_model_sels,
         )
 
         return idata
 
     def output_farm_vars(self, algo):
         """
@@ -324,15 +318,15 @@
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
         s = self.pre_rotor_models if pre_rotor else self.post_rotor_models
         pars = self.__get_pars(algo, s.models, "calc", mdata, st_sel, from_data=True)
         res = s.calculate(algo, mdata, fdata, parameters=pars)
-        self.turbine_model_sels = mdata[FV.TMODEL_SELS]
+        self.turbine_model_sels = mdata[FC.TMODEL_SELS]
         return res
 
     def finalize(self, algo, verbosity=0):
         """
         Finalizes the model.
 
         Parameters
```

### Comparing `foxes-0.3.4/foxes/core/farm_data_model.py` & `foxes-0.3.5/foxes/core/farm_data_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from abc import abstractmethod
 
 from .data_calc_model import DataCalcModel
-import foxes.variables as FV
-
+import foxes.constants as FC
 
 class FarmDataModel(DataCalcModel):
     """
     Abstract base class for models that modify
     farm data.
 
     Parameters
@@ -95,16 +94,16 @@
             The calculation results
 
         """
         return super().run_calculation(
             algo,
             *data,
             out_vars=out_vars,
-            loop_dims=[FV.STATE],
-            out_core_vars=[FV.TURBINE, FV.VARS],
+            loop_dims=[FC.STATE],
+            out_core_vars=[FC.TURBINE, FC.VARS],
             **calc_pars,
         )
 
     def __add__(self, m):
         if isinstance(m, list):
             return FarmDataModelList([self] + m)
         elif isinstance(m, FarmDataModelList):
@@ -193,15 +192,15 @@
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         idata = super().initialize(algo, verbosity)
 
         # done by algo.update_idata
-        #algo.update_idata(self.models, idata=idata, verbosity=verbosity)
+        # algo.update_idata(self.models, idata=idata, verbosity=verbosity)
 
         return idata
 
     def calculate(self, algo, mdata, fdata, parameters=[]):
         """
         The main model calculation.
```

### Comparing `foxes-0.3.4/foxes/core/model.py` & `foxes-0.3.5/foxes/core/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,14 @@
         The model name
 
     """
 
     _ids = {}
 
     def __init__(self):
-
         t = type(self).__name__
         if t not in self._ids:
             self._ids[t] = count(0)
         self._id = next(self._ids[t])
 
         ext = "" if self._id == 0 else f"{self._id}"
         self.name = f"{type(self).__name__}{ext}"
@@ -97,15 +96,17 @@
         idata : dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         if self.initialized:
-            raise ValueError(f"Model '{self.name}': initialize called for already initialized object")
+            raise ValueError(
+                f"Model '{self.name}': initialize called for already initialized object"
+            )
         self.__initialized = True
         return {"coords": {}, "data_vars": {}}
 
     def finalize(self, algo, verbosity=0):
         """
         Finalizes the model.
 
@@ -114,15 +115,17 @@
         algo : foxes.core.Algorithm
             The calculation algorithm
         verbosity : int
             The verbosity level, 0 = silent
 
         """
         if not self.initialized:
-            raise ValueError(f"Model '{self.name}': Finalization called for uninitialized object")
+            raise ValueError(
+                f"Model '{self.name}': Finalization called for uninitialized object"
+            )
         self.__initialized = False
 
     def get_data(
         self,
         variable,
         data,
         st_sel=None,
```

### Comparing `foxes-0.3.4/foxes/core/partial_wakes_model.py` & `foxes-0.3.5/foxes/core/partial_wakes_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
         """
         self.wake_models = algo.wake_models if self._wmodels is None else self._wmodels
         self.wake_frame = algo.wake_frame if self._wframe is None else self._wframe
 
         idata = super().initialize(algo, verbosity)
         algo.update_idata(self.wake_models, idata=idata, verbosity=verbosity)
-        
+
         return idata
 
     @abstractmethod
     def new_wake_deltas(self, algo, mdata, fdata):
         """
         Creates new initial wake deltas, filled
         with zeros.
```

### Comparing `foxes-0.3.4/foxes/core/point_data_model.py` & `foxes-0.3.5/foxes/core/point_data_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from abc import abstractmethod
 
 from .data_calc_model import DataCalcModel
-import foxes.variables as FV
-
+import foxes.constants as FC
 
 class PointDataModel(DataCalcModel):
     """
     Abstract base class for models that modify
     point based data.
     """
 
@@ -80,16 +79,16 @@
             The calculation results
 
         """
         return super().run_calculation(
             algo,
             *data,
             out_vars=out_vars,
-            loop_dims=[FV.STATE, FV.POINT],
-            out_core_vars=[FV.VARS],
+            loop_dims=[FC.STATE, FC.POINT],
+            out_core_vars=[FC.VARS],
             **calc_pars,
         )
 
     def __add__(self, m):
         if isinstance(m, list):
             return PointDataModelList([self] + m)
         elif isinstance(m, PointDataModelList):
```

### Comparing `foxes-0.3.4/foxes/core/rotor_model.py` & `foxes-0.3.5/foxes/core/rotor_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 import foxes.variables as FV
 import foxes.constants as FC
 from .farm_data_model import FarmDataModel
 from .data import Data
 from foxes.utils import wd2uv, uv2wd
 
-
 class RotorModel(FarmDataModel):
     """
     Abstract base class of rotor models.
 
     Rotor models calculate ambient farm data from
     states, and provide rotor points and weights
     for the calculation of rotor effective quantities.
@@ -210,24 +209,22 @@
             FV.WS in self.calc_vars
             or FV.WD in self.calc_vars
             or FV.YAW in self.calc_vars
             or FV.REWS in self.calc_vars
             or FV.REWS2 in self.calc_vars
             or FV.REWS3 in self.calc_vars
         ):
-
             wd = rpoint_results[FV.WD]
             ws = rpoint_results[FV.WS]
             uvp = wd2uv(wd, ws, axis=-1)
             uv = np.einsum("stpd,p->std", uvp, weights)
 
         wd = None
         vdone = []
         for v in self.calc_vars:
-
             if v not in fdata:
                 fdata[v] = np.zeros((n_states, n_turbines), dtype=FC.DTYPE)
 
             if v == FV.WD or v == FV.YAW:
                 if wd is None:
                     wd = uv2wd(uv, axis=-1)
                 self._set_res(fdata, v, wd, stsel)
@@ -241,32 +238,29 @@
         del uv, wd
 
         if (
             FV.REWS in self.calc_vars
             or FV.REWS2 in self.calc_vars
             or FV.REWS3 in self.calc_vars
         ):
-
             if stsel is None:
                 yaw = fdata[FV.YAW].copy()
             else:
                 yaw = fdata[FV.YAW][stsel][:, None]
             nax = wd2uv(yaw, axis=-1)
             wsp = np.einsum("stpd,std->stp", uvp, nax)
 
             for v in self.calc_vars:
-
                 if v == FV.REWS:
                     rews = np.maximum(np.einsum("stp,p->st", wsp, weights), 0.0)
                     self._set_res(fdata, v, rews, stsel)
                     del rews
                     vdone.append(v)
 
                 elif v == FV.REWS2:
-
                     # For highly inhomogeneous wind fields
                     # and multiple rotor points some of the uv
                     # vectors may have negative projections onto the
                     # turbine axis direction:
                     if uvp.shape[2] > 1:
                         rews2 = np.sqrt(
                             np.maximum(
@@ -279,15 +273,14 @@
                     else:
                         rews2 = np.sqrt(np.einsum("stp,p->st", wsp**2, weights))
                     self._set_res(fdata, v, rews2, stsel)
                     del rews2
                     vdone.append(v)
 
                 elif v == FV.REWS3:
-
                     # For highly inhomogeneous wind fields
                     # and multiple rotor points some of the uv
                     # vectors may have negative projections onto the
                     # turbine axis direction:
                     if uvp.shape[2] > 1:
                         rews3 = np.maximum(
                             np.einsum("stp,p->st", wsp**3, weights), 0.0
@@ -354,53 +347,53 @@
         results : dict
             results dict. Keys: Variable name str. Values:
             numpy.ndarray with results, shape: (n_states, n_turbines)
 
         """
 
         if rpoints is None:
-            rpoints = mdata.get(FV.RPOINTS, self.get_rotor_points(algo, mdata, fdata))
+            rpoints = mdata.get(FC.RPOINTS, self.get_rotor_points(algo, mdata, fdata))
         if states_turbine is not None:
             n_states = mdata.n_states
             stsel = (np.arange(n_states), states_turbine)
             rpoints = rpoints[stsel][:, None]
         n_states, n_turbines, n_rpoints, __ = rpoints.shape
         n_points = n_turbines * n_rpoints
 
         if weights is None:
-            weights = mdata.get(FV.RWEIGHTS, self.rotor_point_weights())
+            weights = mdata.get(FC.RWEIGHTS, self.rotor_point_weights())
 
         if store_rpoints:
-            mdata[FV.RPOINTS] = rpoints
-            mdata.dims[FV.RPOINTS] = (FV.STATE, FV.TURBINE, FV.RPOINT, FV.XYH)
+            mdata[FC.RPOINTS] = rpoints
+            mdata.dims[FC.RPOINTS] = (FC.STATE, FC.TURBINE, FC.RPOINT, FV.XYH)
         if store_rweights:
-            mdata[FV.RWEIGHTS] = weights
-            mdata.dims[FV.RWEIGHTS] = (FV.RPOINT,)
+            mdata[FC.RWEIGHTS] = weights
+            mdata.dims[FC.RWEIGHTS] = (FC.RPOINT,)
 
         svars = algo.states.output_point_vars(algo)
         points = rpoints.reshape(n_states, n_points, 3)
-        pdata = {FV.POINTS: points}
-        pdims = {FV.POINTS: (FV.STATE, FV.POINT, FV.XYH)}
+        pdata = {FC.POINTS: points}
+        pdims = {FC.POINTS: (FC.STATE, FC.POINT, FV.XYH)}
         pdata.update(
             {v: np.full((n_states, n_points), np.nan, dtype=FC.DTYPE) for v in svars}
         )
-        pdims.update({v: (FV.STATE, FV.POINT) for v in svars})
-        pdata = Data(pdata, pdims, loop_dims=[FV.STATE, FV.POINT])
+        pdims.update({v: (FC.STATE, FC.POINT) for v in svars})
+        pdata = Data(pdata, pdims, loop_dims=[FC.STATE, FC.POINT])
         del pdims, points
 
         sres = algo.states.calculate(algo, mdata, fdata, pdata)
         pdata.update(sres)
         del sres
 
         rpoint_results = {}
         for v in svars:
             rpoint_results[v] = pdata[v].reshape(n_states, n_turbines, n_rpoints)
 
         if store_amb_res:
-            mdata[FV.AMB_RPOINT_RESULTS] = rpoint_results
+            mdata[FC.AMB_RPOINT_RESULTS] = rpoint_results
 
         self.eval_rpoint_results(
             algo,
             mdata,
             fdata,
             rpoint_results,
             weights,
```

### Comparing `foxes-0.3.4/foxes/core/states.py` & `foxes-0.3.5/foxes/core/states.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from abc import abstractmethod
 
 from .point_data_model import PointDataModel, PointDataModelList
 import foxes.variables as FV
-
+import foxes.constants as FC
 
 class States(PointDataModel):
     """
     Abstract base class for states.
 
     States describe ambient meteorological data,
     typically wind speed, wind direction, turbulence
@@ -72,26 +72,26 @@
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         sinds = self.index()
         if sinds is not None:
-            idata["coords"][FV.STATE] = sinds
+            idata["coords"][FC.STATE] = sinds
 
         weights = self.weights(algo)
         if len(weights.shape) != 2:
             raise ValueError(
-                f"States '{self.name}': Wrong weights dimension, expecing ({FV.STATE}, {FV.TURBINE}), got shape {weights.shape}"
+                f"States '{self.name}': Wrong weights dimension, expecing ({FC.STATE}, {FC.TURBINE}), got shape {weights.shape}"
             )
         if weights.shape[1] != algo.n_turbines:
             raise ValueError(
-                f"States '{self.name}': Wrong size of second axis dimension '{FV.TURBINE}': Expecting {algo.n_turbines}, got {weights.shape[1]}"
+                f"States '{self.name}': Wrong size of second axis dimension '{FC.TURBINE}': Expecting {algo.n_turbines}, got {weights.shape[1]}"
             )
-        idata["data_vars"][FV.WEIGHT] = ((FV.STATE, FV.TURBINE), weights)
+        idata["data_vars"][FV.WEIGHT] = ((FC.STATE, FC.TURBINE), weights)
 
         return idata
 
     def output_point_vars(self, algo):
         """
         The variables which are being modified by the model.
 
@@ -103,15 +103,15 @@
         Returns
         -------
         output_vars : list of str
             The output variable names
 
         """
         return [FV.WS, FV.WD, FV.TI, FV.RHO]
-    
+
     def __add__(self, s):
         if isinstance(s, list):
             return ExtendedStates(self, s)
         elif isinstance(s, ExtendedStates):
             if s.states is not self:
                 raise ValueError(
                     f"Cannot add extended states, since not based on same states"
@@ -281,15 +281,15 @@
         ----------
         algo : foxes.core.Algorithm
             The calculation algorithm
         verbosity : int
             The verbosity level
 
         """
-        self.pmodels.finalize(algo,  verbosity)
+        self.pmodels.finalize(algo, verbosity)
         super().finalize(algo, verbosity)
 
     def __add__(self, m):
         models = self.pmodels.models[1:]
         if isinstance(m, list):
             return ExtendedStates(self.states, models + m)
         elif isinstance(m, ExtendedStates):
```

### Comparing `foxes-0.3.4/foxes/core/turbine.py` & `foxes-0.3.5/foxes/core/turbine.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.4/foxes/core/turbine_model.py` & `foxes-0.3.5/foxes/core/turbine_model.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.4/foxes/core/turbine_type.py` & `foxes-0.3.5/foxes/core/turbine_type.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from .turbine_model import TurbineModel
 import foxes.constants as FC
 
+
 class TurbineType(TurbineModel):
     """
     Abstract base class for turbine type models.
 
     Rotor diameter and hub height can be overwritten
     by individual settings in the Turbine object.
 
@@ -33,25 +34,20 @@
     P_nominal : float
         The nominal power in kW
     P_unit : str
         The unit of power
 
     """
 
-    def __init__(
-            self, 
-            name=None, 
-            D=None, 
-            H=None, 
-            P_nominal=None,
-            P_unit="kW"
-        ):
+    def __init__(self, name=None, D=None, H=None, P_nominal=None, P_unit="kW"):
         super().__init__()
 
         self.name = name if name is not None else type(self).__name__
         self.D = D
         self.H = H
         self.P_nominal = P_nominal
         self.P_unit = P_unit
 
         if P_unit not in FC.P_UNITS:
-            raise KeyError(f"Turbine type '{self.name}': Unkown P_unit '{P_unit}', expecting {list(FC.P_UNITS.keys())}")
+            raise KeyError(
+                f"Turbine type '{self.name}': Unkown P_unit '{P_unit}', expecting {list(FC.P_UNITS.keys())}"
+            )
```

### Comparing `foxes-0.3.4/foxes/core/vertical_profile.py` & `foxes-0.3.5/foxes/core/vertical_profile.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.4/foxes/core/wake_frame.py` & `foxes-0.3.5/foxes/core/wake_frame.py`

 * *Files 12% similar despite different names*

```diff
@@ -87,34 +87,36 @@
         fdata : foxes.core.Data
             The farm data
         states_source_turbine : numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
         x : numpy.ndarray
             The wake frame x coordinates, shape: (n_states, n_points)
-        
+
         Returns
         -------
         points : numpy.ndarray
             The centreline points, shape: (n_states, n_points, 3)
 
         """
-        raise NotImplementedError(f"Wake frame '{self.name}': Centreline points requested but not implemented.")
-    
+        raise NotImplementedError(
+            f"Wake frame '{self.name}': Centreline points requested but not implemented."
+        )
+
     def calc_centreline_integral(
-            self, 
-            algo, 
-            mdata, 
-            fdata, 
-            states_source_turbine,
-            variables,
-            x,
-            dx,
-            **ipars,
-        ):
+        self,
+        algo,
+        mdata,
+        fdata,
+        states_source_turbine,
+        variables,
+        x,
+        dx,
+        **ipars,
+    ):
         """
         Integrates variables along the centreline.
 
         Parameters
         ----------
         algo : foxes.core.Algorithm
             The calculation algorithm
@@ -124,15 +126,15 @@
             The farm data
         states_source_turbine : numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
         variables : list of str
             The variables to be integrated
         x : numpy.ndarray
-            The wake frame x coordinates of the upper integral bounds, 
+            The wake frame x coordinates of the upper integral bounds,
             shape: (n_states, n_points)
         dx : float
             The step size of the integral
         ipars : dict, optional
             Additional interpolation parameters
 
         Returns
@@ -143,36 +145,35 @@
         """
         # prepare:
         n_states, n_points = x.shape
         vrs = [FV.amb2var.get(v, v) for v in variables]
         n_vars = len(vrs)
 
         # calc evaluation points:
-        xmin = 0.
+        xmin = 0.0
         xmax = np.max(x)
-        n_steps = int((xmax - xmin)/dx)
-        if xmin + n_steps*dx < xmax:
+        n_steps = int((xmax - xmin) / dx)
+        if xmin + n_steps * dx < xmax:
             n_steps += 1
         n_ix = n_steps + 1
-        xs = np.arange(xmin, xmin+n_ix*dx, dx)
+        xs = np.arange(xmin, xmin + n_ix * dx, dx)
         xpts = np.zeros((n_states, n_steps), dtype=FC.DTYPE)
         xpts[:] = xs[None, 1:]
-        pts = self.get_centreline_points(algo, mdata, fdata, states_source_turbine, xpts)
+        pts = self.get_centreline_points(
+            algo, mdata, fdata, states_source_turbine, xpts
+        )
 
         # run ambient calculation:
-        pdata = {FV.POINTS: pts}
-        pdims = {FV.POINTS: (FV.STATE, FV.POINT, FV.XYH)}
+        pdata = {FC.POINTS: pts}
+        pdims = {FC.POINTS: (FC.STATE, FC.POINT, FV.XYH)}
         pdata.update(
-            {
-                v: np.full((n_states, n_steps), np.nan, dtype=FC.DTYPE)
-                for v in vrs
-            }
+            {v: np.full((n_states, n_steps), np.nan, dtype=FC.DTYPE) for v in vrs}
         )
-        pdims.update({v: (FV.STATE, FV.POINT) for v in vrs})
-        pdata = Data(pdata, pdims, loop_dims=[FV.STATE, FV.POINT])
+        pdims.update({v: (FC.STATE, FC.POINT) for v in vrs})
+        pdata = Data(pdata, pdims, loop_dims=[FC.STATE, FC.POINT])
         res = algo.states.calculate(algo, mdata, fdata, pdata)
         pdata.update(res)
         amb2var = algo.SetAmbPointResults()
         amb2var.initialize(algo, verbosity=0)
         res = amb2var.calculate(algo, mdata, fdata, pdata)
         pdata.update(res)
         del pdims, res, amb2var
@@ -187,23 +188,29 @@
         # calc wakes:
         if not ambient:
             wcalc = algo.PointWakesCalculation(vrs)
             wcalc.initialize(algo, verbosity=0)
             res = wcalc.calculate(algo, mdata, fdata, pdata)
             pdata.update(res)
             del wcalc, res
-        
+
         # collect integration results:
         iresults = np.zeros((n_states, n_ix, n_vars), dtype=FC.DTYPE)
         for vi, v in enumerate(variables):
             for i in range(n_steps):
-                iresults[:, i+1, vi] = iresults[:, i, vi] + pdata[v][:, i] * dx 
+                iresults[:, i + 1, vi] = iresults[:, i, vi] + pdata[v][:, i] * dx
 
         # interpolate to x of interest:
         qts = np.zeros((n_states, n_points, 2), dtype=FC.DTYPE)
         qts[:, :, 0] = np.arange(n_states)[:, None]
         qts[:, :, 1] = x
-        qts = qts.reshape(n_states*n_points, 2)
-        results = interpn((np.arange(n_states), xs), iresults, qts, bounds_error=False, 
-                            fill_value=0., **ipars)
+        qts = qts.reshape(n_states * n_points, 2)
+        results = interpn(
+            (np.arange(n_states), xs),
+            iresults,
+            qts,
+            bounds_error=False,
+            fill_value=0.0,
+            **ipars,
+        )
 
         return results.reshape(n_states, n_points, n_vars)
```

### Comparing `foxes-0.3.4/foxes/core/wake_model.py` & `foxes-0.3.5/foxes/core/wake_model.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.4/foxes/core/wake_superposition.py` & `foxes-0.3.5/foxes/core/wake_superposition.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.4/foxes/core/wind_farm.py` & `foxes-0.3.5/foxes/core/wind_farm.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.4/foxes/data/farms/test_farm_67.csv` & `foxes-0.3.5/foxes/data/farms/test_farm_67.csv`

 * *Files identical despite different names*

### Comparing `foxes-0.3.4/foxes/data/parse.py` & `foxes-0.3.5/foxes/data/parse.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,30 +25,29 @@
     i = sname.find(".")
     if i >= 0:
         if "-" in sname[i:]:
             warnings.warn(
                 f"Illegal use of '.' in '{sname}', please replace by 'd' for float value dots. Parsing stopped."
             )
             return pars
-    
+
     if "-" in sname and "_" in sname:
         warnings.warn(
             f"Illegal file name '{file_name}': Contains both '-' and '_'. Parsing stopped."
         )
         return pars
 
     if "-" in sname:
         pieces = sname.split("-")
     elif "_" in sname:
         pieces = sname.split("_")
 
     pars["name"] = pieces[0]
     pieces = pieces[1:]
     for p in pieces:
-
         if p[-1] == "W":
             if p[-2] == "k":
                 pars["P_nominal"] = float(p[:-2].replace("d", "."))
             elif p[-2] == "M":
                 pars["P_nominal"] = 1.0e3 * float(p[:-2].replace("d", "."))
             elif p[-2] == "G":
                 pars["P_nominal"] = 1.0e6 * float(p[:-2].replace("d", "."))
```

### Comparing `foxes-0.3.4/foxes/data/power_ct_curves/IWT-7d5MW-D164-H100.csv` & `foxes-0.3.5/foxes/data/power_ct_curves/IWT-7d5MW-D164-H100.csv`

 * *Files identical despite different names*

### Comparing `foxes-0.3.4/foxes/data/states/WRF-Timeseries-4464.csv.gz` & `foxes-0.3.5/foxes/data/states/WRF-Timeseries-4464.csv.gz`

 * *Files identical despite different names*

### Comparing `foxes-0.3.4/foxes/data/states/abl_states_6000.csv.gz` & `foxes-0.3.5/foxes/data/states/abl_states_6000.csv.gz`

 * *Files identical despite different names*

### Comparing `foxes-0.3.4/foxes/data/states/timeseries_3000.csv.gz` & `foxes-0.3.5/foxes/data/states/timeseries_3000.csv.gz`

 * *Files identical despite different names*

### Comparing `foxes-0.3.4/foxes/data/states/timeseries_8000.csv.gz` & `foxes-0.3.5/foxes/data/states/timeseries_8000.csv.gz`

 * *Files identical despite different names*

### Comparing `foxes-0.3.4/foxes/data/states/wind_rose_bremen.csv` & `foxes-0.3.5/foxes/data/states/wind_rose_bremen.csv`

 * *Files identical despite different names*

### Comparing `foxes-0.3.4/foxes/data/states/wind_rotation.nc` & `foxes-0.3.5/foxes/data/states/wind_rotation.nc`

 * *Files identical despite different names*

### Comparing `foxes-0.3.4/foxes/data/static_data.py` & `foxes-0.3.5/foxes/data/static_data.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.4/foxes/input/farm_layout/add_from_csv.py` & `foxes-0.3.5/foxes/input/farm_layout/from_csv.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,16 +20,14 @@
     turbine_base_name_count_shift=False,
     verbosity=1,
     **turbine_parameters,
 ):
     """
     Add turbines to wind farm via csv input file.
 
-    Additional turbine_parameters are forwarded to the WindFarm.add_turbine().
-
     Parameters
     ----------
     farm : foxes.WindFarm
         The wind farm
     data_source : str or pandas.DataFrame
         The input csv file or data source
     col_index : str, optional
@@ -58,14 +56,16 @@
     turbine_ids : list, optional
         The turbine ids, or None for
         index
     turbine_base_name_count_shift : bool, optional
         Start turbine names by 1 instead of 0
     verbosity : int
         The verbosity level, 0 = silent
+    turbine_parameters : dict, optional
+        Additional parameters are forwarded to the WindFarm.add_turbine().
 
     """
 
     if isinstance(data_source, pd.DataFrame):
         data = data_source
     else:
         if verbosity:
@@ -73,15 +73,14 @@
         data = pd.read_csv(data_source, index_col=col_index)
 
     tmodels = turbine_parameters.pop("turbine_models", [])
     H = turbine_parameters.pop("H", None)
     D = turbine_parameters.pop("D", None)
 
     for i in data.index:
-
         s = 1 if turbine_base_name_count_shift else 0
         tname = (
             f"{turbine_base_name}{i+s}" if col_name is None else data.loc[i, col_name]
         )
         txy = data.loc[i, [col_x, col_y]].values
 
         if turbine_ids is not None:
```

### Comparing `foxes-0.3.4/foxes/input/farm_layout/add_from_df.py` & `foxes-0.3.5/foxes/input/farm_layout/from_df.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from .add_from_csv import add_from_csv
+from .from_csv import add_from_csv
+
 
 def add_from_df(
     farm,
     data_source,
     *args,
     **kwargs,
 ):
```

### Comparing `foxes-0.3.4/foxes/input/farm_layout/add_from_file.py` & `foxes-0.3.5/foxes/input/farm_layout/from_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 
 from foxes.data import FARM, StaticData
-from .add_from_json import add_from_json
-from .add_from_csv import add_from_csv
+from .from_json import add_from_json
+from .from_csv import add_from_csv
 
 
 def add_from_file(farm, file_path, *args, verbosity=1, dbook=None, **kwargs):
     """
     Add turbines from file.
 
     The method is inferred according to the file suffix.
```

### Comparing `foxes-0.3.4/foxes/input/farm_layout/add_from_json.py` & `foxes-0.3.5/foxes/input/farm_layout/from_json.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,14 @@
     farm_name = keys[0]
     fdict = dict[farm_name]
 
     if set_farm_name:
         farm.name = farm_name
 
     for wt_name, wdict in fdict.items():
-
         pars = deepcopy(turbine_parameters)
         if "D" in wdict:
             pars["D"] = wdict["D"]
         if "H" in wdict:
             pars["H"] = wdict["H"]
         if "turbine_models" in wdict:
             pars["turbine_models"] = wdict["turbine_models"] + pars.get(
```

### Comparing `foxes-0.3.4/foxes/input/farm_layout/add_grid.py` & `foxes-0.3.5/foxes/input/farm_layout/grid.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.4/foxes/input/farm_layout/add_row.py` & `foxes-0.3.5/foxes/input/farm_layout/row.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.4/foxes/input/states/create/random_abl_states.py` & `foxes-0.3.5/foxes/input/states/create/random_abl_states.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     -------
     data : pandas.DataFrame
         The created states data
 
     """
 
     data = pd.DataFrame(index=range(n_states))
-    data.index.name = FV.STATE
+    data.index.name = FC.STATE
 
     for v, mm in cols_minmax.items():
         data[v] = np.random.uniform(low=mm[0], high=mm[1], size=(n_states,)).astype(
             FC.DTYPE
         )
 
     cmol = var2col.get(FV.MOL, FV.MOL)
@@ -96,15 +96,14 @@
         print("Writing file", file_path)
 
     data = create_random_abl_states(
         n_states, cols_minmax, var2col, mol_abs_range, normalize
     )
 
     if digits is not None:
-
         hdigits = {c: 4 for c in cols_minmax.keys()}
 
         wcol = var2col.get(FV.WEIGHT, FV.WEIGHT)
         if wcol in cols_minmax:
             hdigits[wcol] = None
 
         mcol = var2col.get(FV.MOL, FV.MOL)
```

### Comparing `foxes-0.3.4/foxes/input/states/field_data_nc.py` & `foxes-0.3.5/foxes/input/states/field_data_nc.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         h_coord="height",
         pre_load=True,
         weight_ncvar=None,
         bounds_error=True,
         fill_value=None,
         time_format="%Y-%m-%d_%H:%M:%S",
         sel=None,
-        verbosity=1
+        verbosity=1,
     ):
         super().__init__()
 
         self.data_source = data_source
         self.states_coord = states_coord
         self.ovars = output_vars
         self.fixed_vars = fixed_vars
@@ -131,58 +131,60 @@
 
         self._inds = None
         self._N = None
         self._weights = None
 
         # pre-load file reading, usually prior to DaskRunner:
         if not isinstance(self.data_source, xr.Dataset):
-
             if "*" in str(self.data_source):
                 pass
             else:
-                self.data_source = StaticData().get_file_path(STATES, self.data_source, check_raw=True)
+                self.data_source = StaticData().get_file_path(
+                    STATES, self.data_source, check_raw=True
+                )
             if verbosity:
                 if pre_load:
-                    print(f"States '{self.name}': Reading data from '{self.data_source}'")
+                    print(
+                        f"States '{self.name}': Reading data from '{self.data_source}'"
+                    )
                 else:
-                    print(f"States '{self.name}': Reading index from '{self.data_source}'")
+                    print(
+                        f"States '{self.name}': Reading index from '{self.data_source}'"
+                    )
 
             with xr.open_mfdataset(
                 str(self.data_source),
                 parallel=False,
                 concat_dim=self.states_coord,
                 combine="nested",
                 data_vars="minimal",
                 coords="minimal",
                 compat="override",
             ) as ds:
-                
                 dss = ds if self.sel is None else ds.sel(self.sel)
                 if pre_load:
                     self.data_source = dss.load()
                 else:
                     self.data_source = dss
                 self._get_inds(dss)
 
     def _get_inds(self, ds):
         """
-        Helper function for index and weights 
+        Helper function for index and weights
         reading
         """
         for c in [self.states_coord, self.x_coord, self.y_coord, self.h_coord]:
             if not c in ds:
                 raise KeyError(
                     f"States '{self.name}': Missing coordinate '{c}' in data"
                 )
 
         self._inds = ds[self.states_coord].to_numpy()
         if self.time_format is not None:
-            self._inds = pd.to_datetime(
-                self._inds, format=self.time_format
-            ).to_numpy()
+            self._inds = pd.to_datetime(self._inds, format=self.time_format).to_numpy()
         self._N = len(self._inds)
 
         if self.weight_ncvar is not None:
             self._weights = ds[self.weight_ncvar].to_numpy()
 
         for v in self.ovars:
             if v in self.var2ncvar:
@@ -190,16 +192,16 @@
                 if not ncv in ds:
                     raise KeyError(
                         f"States '{self.name}': nc variable '{ncv}' not found in data, found: {sorted(list(ds.keys()))}"
                     )
             elif v not in self.fixed_vars:
                 raise ValueError(
                     f"States '{self.name}': Variable '{v}' neither found in var2ncvar not in fixed_vars"
-                )  
-                
+                )
+
     def _get_data(self, ds, verbosity):
         """
         Helper function for data extraction
         """
         x = ds[self.x_coord].to_numpy()
         y = ds[self.y_coord].to_numpy()
         h = ds[self.h_coord].to_numpy()
@@ -277,15 +279,15 @@
         -------
         idata : dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
-        
+
         if (FV.WS in self.ovars and FV.WD not in self.ovars) or (
             FV.WS not in self.ovars and FV.WD in self.ovars
         ):
             raise KeyError(
                 f"States '{self.name}': Missing '{FV.WS}' or '{FV.WD}' in output variables {self.ovars}"
             )
 
@@ -305,37 +307,36 @@
                 (self._N, algo.n_turbines), 1.0 / self._N, dtype=FC.DTYPE
             )
 
         idata = super().initialize(algo, verbosity)
         self._update_idata(algo, idata)
 
         if self.pre_load:
-
             self.X = self.var(FV.X)
             self.Y = self.var(FV.Y)
             self.H = self.var(FV.H)
             self.VARS = self.var("vars")
             self.DATA = self.var("data")
 
             ds = self.data_source
 
             h = ds[self.h_coord].to_numpy()
             y = ds[self.y_coord].to_numpy()
             x = ds[self.x_coord].to_numpy()
             v = list(self._dkys.keys())
-            coos = (FV.STATE, self.H, self.Y, self.X, self.VARS)
+            coos = (FC.STATE, self.H, self.Y, self.X, self.VARS)
             data = self._get_data(ds, verbosity)
             data = (coos, data)
 
             idata["coords"][self.H] = h
             idata["coords"][self.Y] = y
             idata["coords"][self.X] = x
             idata["coords"][self.VARS] = v
             idata["data_vars"][self.DATA] = data
-        
+
         return idata
 
     def size(self):
         """
         The total number of states.
 
         Returns
@@ -414,28 +415,28 @@
         -------
         results : dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_points)
 
         """
         # prepare:
-        points = pdata[FV.POINTS]
+        points = pdata[FC.POINTS]
         n_pts = points.shape[1]
         n_states = fdata.n_states
 
         # pick pre-loaded data:
         if self.pre_load:
             x = mdata[self.X]
             y = mdata[self.Y]
             h = mdata[self.H]
             data = mdata[self.DATA].copy()
 
         # read data for this chunk:
         else:
-            i0 = np.where(self._inds == mdata[FV.STATE][0])[0][0]
+            i0 = np.where(self._inds == mdata[FC.STATE][0])[0][0]
             s = slice(i0, i0 + n_states)
             ds = self.data_source.isel({self.states_coord: s}).load()
 
             x = ds[self.x_coord].to_numpy()
             y = ds[self.y_coord].to_numpy()
             h = ds[self.h_coord].to_numpy()
             data = self._get_data(ds, verbosity=0)
@@ -492,8 +493,7 @@
                     out[v] = data[..., self._dkys[v]]
                 else:
                     out[v] = np.full(
                         (n_states, n_pts), self.fixed_vars[v], dtype=FC.DTYPE
                     )
 
         return out
-
```

### Comparing `foxes-0.3.4/foxes/input/states/multi_height.py` & `foxes-0.3.5/foxes/input/states/multi_height.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         ----------
         states_sel : slice or range or list of int, optional
             States subset selection
         states_loc : list, optional
             State index selection via pandas loc function
         verbosity : int
             The verbosity level, 0 = silent
-            
+
         """
         if self.initialized:
             if algo is None:
                 raise KeyError(f"{self.name}: Missing algo for reset")
             elif algo.states is not self:
                 raise ValueError(f"{self.states}: algo.states differs from self")
             self.finalize(algo, verbosity)
@@ -232,22 +232,22 @@
         self._update_idata(algo, idata)
 
         idata["coords"][self.H] = self.heights
         idata["coords"][self.VARS] = list(self._cmap.keys())
 
         n_hts = len(self.heights)
         n_vrs = int(len(data.columns) / n_hts)
-        dims = (FV.STATE, self.VARS, self.H)
+        dims = (FC.STATE, self.VARS, self.H)
         idata["data_vars"][self.DATA] = (
             dims,
             data.to_numpy().reshape(self._N, n_vrs, n_hts),
         )
 
         for v, d in self._solo.items():
-            idata["data_vars"][self.var(v)] = ((FV.STATE,), d)
+            idata["data_vars"][self.var(v)] = ((FC.STATE,), d)
 
         return idata
 
     def size(self):
         """
         The total number of states.
 
@@ -266,15 +266,15 @@
         Returns
         -------
         indices : array_like
             The index labels of states, or None for default integers
 
         """
         return self._inds
-    
+
     def output_point_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
         algo : foxes.core.Algorithm
@@ -327,15 +327,15 @@
         -------
         results : dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_points)
 
         """
         h = mdata[self.H]
-        z = pdata[FV.POINTS][:, :, 2]
+        z = pdata[FC.POINTS][:, :, 2]
         n_h = len(h)
         vrs = list(mdata[self.VARS])
 
         coeffs = np.zeros((n_h, n_h), dtype=FC.DTYPE)
         np.fill_diagonal(coeffs, 1.0)
         ipars = dict(assume_sorted=True, bounds_error=True)
         ipars.update(self.ipars)
```

### Comparing `foxes-0.3.4/foxes/input/states/scan_ws.py` & `foxes-0.3.5/foxes/input/states/scan_ws.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         self.WS = self.var(FV.WS)
 
         idata = super().initialize(algo, verbosity)
         self._update_idata(algo, idata)
-        idata["data_vars"][self.WS] = ((FV.STATE,), self._wsl)
+        idata["data_vars"][self.WS] = ((FC.STATE,), self._wsl)
 
         return idata
 
     def size(self):
         """
         The total number of states.
```

### Comparing `foxes-0.3.4/foxes/input/states/single.py` & `foxes-0.3.5/foxes/input/states/single.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,17 +190,17 @@
                 (pdata.n_states, pdata.n_points), self.ti, dtype=FC.DTYPE
             )
         if self.rho is not None:
             pdata[FV.RHO] = np.full(
                 (pdata.n_states, pdata.n_points), self.rho, dtype=FC.DTYPE
             )
 
-        z = pdata[FV.POINTS][:, :, 2]
+        z = pdata[FC.POINTS][:, :, 2]
         if len(self._profiles):
-            z = pdata[FV.POINTS][:, :, 2]
+            z = pdata[FC.POINTS][:, :, 2]
             for k, v in self.profdata.items():
                 pdata[k] = v
             for v, p in self._profiles.items():
                 pres = p.calculate(pdata, z)
                 pdata[v] = pres
 
         return {v: pdata[v] for v in self.output_point_vars(algo)}
```

### Comparing `foxes-0.3.4/foxes/input/states/states_table.py` & `foxes-0.3.5/foxes/input/states/states_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,17 @@
         self.var2col = var2col
         self.fixed_vars = fixed_vars
         self.profdicts = profiles
         self.states_sel = states_sel
         self.states_loc = states_loc
 
         if self.states_loc is not None and self.states_sel is not None:
-            raise ValueError(f"States '{self.name}': Cannot handle both 'states_sel' and 'states_loc', please pick one")
+            raise ValueError(
+                f"States '{self.name}': Cannot handle both 'states_sel' and 'states_loc', please pick one"
+            )
 
         self._weights = None
         self._N = None
         self._tvars = None
 
     def reset(self, algo=None, states_sel=None, states_loc=None, verbosity=0):
         """
@@ -98,25 +100,25 @@
         ----------
         states_sel : slice or range or list of int, optional
             States subset selection
         states_loc : list, optional
             State index selection via pandas loc function
         verbosity : int
             The verbosity level, 0 = silent
-            
+
         """
         if self.initialized:
             if algo is None:
                 raise KeyError(f"{self.name}: Missing algo for reset")
             elif algo.states is not self:
                 raise ValueError(f"{self.states}: algo.states differs from self")
             self.finalize(algo, verbosity)
         self.states_sel = states_sel
         self.states_loc = states_loc
-        
+
     def initialize(self, algo, verbosity=0):
         """
         Initializes the model.
 
         This includes loading all required data from files. The model
         should return all array type data as part of the idata return
         dictionary (and not store it under self, for memory reasons). This
@@ -210,19 +212,20 @@
                     f"States '{self.name}': Missing variable '{c}' in states table columns, profiles or fixed vars"
                 )
         data = data[tcols]
 
         idata = super().initialize(algo, verbosity)
         self._update_idata(algo, idata)
         idata["coords"][self.VARS] = self._tvars
-        idata["data_vars"][self.DATA] = ((FV.STATE, self.VARS), data.to_numpy())
+        idata["data_vars"][self.DATA] = ((FC.STATE, self.VARS), data.to_numpy())
+
+        algo.update_idata(
+            list(self._profiles.values()), idata=idata, verbosity=verbosity
+        )
 
-        algo.update_idata(list(self._profiles.values()),
-            idata=idata, verbosity=verbosity)
-            
         return idata
 
     def size(self):
         """
         The total number of states.
 
         Returns
@@ -240,15 +243,15 @@
         Returns
         -------
         indices : array_like
             The index labels of states, or None for default integers
 
         """
         return self._inds
-    
+
     def output_point_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
         algo : foxes.core.Algorithm
@@ -300,15 +303,15 @@
         Returns
         -------
         results : dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_points)
 
         """
-        z = pdata[FV.POINTS][:, :, 2]
+        z = pdata[FC.POINTS][:, :, 2]
 
         for i, v in enumerate(self._tvars):
             pdata[v][:] = mdata[self.DATA][:, i, None]
 
         for v, f in self.fixed_vars.items():
             pdata[v] = np.full((pdata.n_states, pdata.n_points), f, dtype=FC.DTYPE)
```

### Comparing `foxes-0.3.4/foxes/input/windio/windio.py` & `foxes-0.3.5/foxes/input/windio/windio.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,45 +7,46 @@
 from foxes.models import ModelBook
 from foxes.input.states import StatesTable
 from foxes.input.farm_layout import add_from_df
 from foxes.models.turbine_types import CpCtFromTwo
 import foxes.constants as FC
 import foxes.variables as FV
 
+
 def read_resource(res_yaml, fixed_vars={}, **kwargs):
     """
     Reads a WindIO energy resource
 
     Parameters
     ----------
     res_yaml : str
         Path to the yaml file
     fixed_vars : dict
-        Additional fixes variables that do 
+        Additional fixes variables that do
         not occur in the yaml
     kwargs : dict, optional
         Additional arguments for StatesTable
 
     Returns
     -------
     states: foxes.states.StatesTable
         The uniform states
 
     """
     res_yaml = Path(res_yaml)
 
-    with open(res_yaml, 'r') as file:
+    with open(res_yaml, "r") as file:
         res = yaml.load(file, Loader=yaml.loader.BaseLoader)
     wres = res["wind_resource"]
 
     wd = np.array(wres["wind_direction"], dtype=FC.DTYPE)
     ws = np.array(wres["wind_speed"], dtype=FC.DTYPE)
     n_wd = len(wd)
     n_ws = len(ws)
-    n = n_wd*n_ws
+    n = n_wd * n_ws
 
     data = np.zeros((n_wd, n_ws, 2), dtype=FC.DTYPE)
     data[:, :, 0] = wd[:, None]
     data[:, :, 1] = ws[None, :]
     names = ["wind_direction", "wind_speed"]
 
     def _to_data(v, d, dims):
@@ -64,46 +65,44 @@
             if dims[0] == "wind_direction" and dims[1] == "wind_speed":
                 hdata[:, :, 0] = np.array(d, dtype=FC.DTYPE)
             elif dims[1] == "wind_direction" and dims[0] == "wind_speed":
                 hdata[:, :, 0] = np.swapaxes(np.array(d, dtype=FC.DTYPE), 0, 1)
             else:
                 raise ValueError(f"Cannot handle dims = {dims} for data '{v}'")
         else:
-            raise ValueError(f"Can not accept more than two dimensions, got {dims} for data '{v}'")
+            raise ValueError(
+                f"Can not accept more than two dimensions, got {dims} for data '{v}'"
+            )
         data = np.append(data, hdata, axis=2)
         names.append(v)
 
     vmap = {
         "wind_direction": FV.WD,
         "wind_speed": FV.WS,
         "turbulence_intensity": FV.TI,
         "air_density": FV.RHO,
-        "probability": FV.WEIGHT
+        "probability": FV.WEIGHT,
     }
 
     for v, d in wres.items():
         if v in vmap and isinstance(d, dict):
             _to_data(v, d["data"], d["dims"])
 
     n_vars = len(names)
-    data = data.reshape(n, n_vars)    
+    data = data.reshape(n, n_vars)
 
     data = pd.DataFrame(index=range(n), data=data, columns=names)
     data.index.name = "state"
     data.rename(columns=vmap, inplace=True)
-    
+
     ovars = {v: v for v in data.columns if v != FV.WEIGHT}
     ovars.update({k: v for k, v in fixed_vars.items() if k not in data.columns})
 
-    return StatesTable(
-        data,
-        output_vars=ovars,
-        fixed_vars=fixed_vars,
-        **kwargs
-    )
+    return StatesTable(data, output_vars=ovars, fixed_vars=fixed_vars, **kwargs)
+
 
 def read_site(site_yaml, **kwargs):
     """
     Reads a WindIO site
 
     Parameters
     ----------
@@ -116,24 +115,25 @@
     -------
     states : foxes.states.States
         The states object
 
     """
     site_yaml = Path(site_yaml)
 
-    with open(site_yaml, 'r') as file:
+    with open(site_yaml, "r") as file:
         site = yaml.load(file, Loader=yaml.loader.BaseLoader)
 
     res_yaml = site["energy_resource"]
     if res_yaml[0] == ".":
-        res_yaml = (site_yaml.parent/res_yaml).resolve()
+        res_yaml = (site_yaml.parent / res_yaml).resolve()
     states = read_resource(res_yaml, **kwargs)
 
     return states
 
+
 def read_farm(farm_yaml, mbook=None, layout=-1, turbine_models=[], **kwargs):
     """
     Reads a WindIO wind farm
 
     Parameters
     ----------
     farm_yaml : str
@@ -154,39 +154,39 @@
     farm : foxes.WindFarm
         The wind farm
 
     """
     mbook = ModelBook() if mbook is None else mbook
     farm_yaml = Path(farm_yaml)
 
-    with open(farm_yaml, 'r') as file:
+    with open(farm_yaml, "r") as file:
         fdict = yaml.load(file, Loader=yaml.loader.BaseLoader)
 
     if isinstance(layout, str):
-        layout = fdict['layouts'][layout]
+        layout = fdict["layouts"][layout]
     else:
-        lname = list(fdict['layouts'].keys())[layout]
-        layout = fdict['layouts'][lname]
+        lname = list(fdict["layouts"].keys())[layout]
+        layout = fdict["layouts"][lname]
 
     x = np.array(layout["coordinates"]["x"], dtype=FC.DTYPE)
     y = np.array(layout["coordinates"]["y"], dtype=FC.DTYPE)
     N = len(x)
     ldata = pd.DataFrame(index=range(N))
     ldata.index.name = "index"
     ldata["x"] = x
     ldata["y"] = y
 
     if "turbines" in fdict:
         turbines_yaml = fdict["turbines"]
         if turbines_yaml[0] == ".":
-            turbines_yaml = (farm_yaml.parent/turbines_yaml).resolve()
+            turbines_yaml = (farm_yaml.parent / turbines_yaml).resolve()
 
-        with open(turbines_yaml, 'r') as file:
+        with open(turbines_yaml, "r") as file:
             tdict = yaml.load(file, Loader=yaml.loader.BaseLoader)
-        
+
         pdict = tdict["performance"]
 
     else:
         tdict = fdict
         pdict = fdict
 
     ct_ws = np.array(pdict["Ct_curve"]["Ct_wind_speeds"], dtype=FC.DTYPE)
@@ -198,25 +198,28 @@
     cp_data = pd.DataFrame(index=range(len(cp_ws)))
     cp_data["ws"] = cp_ws
     cp_data["cp"] = np.array(pdict["Cp_curve"]["Cp_values"], dtype=FC.DTYPE)
 
     D = float(tdict["rotor_diameter"])
     H = float(tdict["hub_height"])
 
-    mbook.turbine_types["windio_turbine"] = CpCtFromTwo(cp_data, ct_data, col_ws_cp_file="ws",
-                                                        col_cp="cp", D=D, H=H)
+    mbook.turbine_types["windio_turbine"] = CpCtFromTwo(
+        cp_data, ct_data, col_ws_cp_file="ws", col_cp="cp", D=D, H=H
+    )
 
     models = ["windio_turbine"] + turbine_models
     farm = WindFarm(name=fdict["name"])
     add_from_df(farm, ldata, col_x="x", col_y="y", turbine_models=models, **kwargs)
 
     return mbook, farm
 
-def read_anlyses(analyses, mbook, farm, states, keymap={}, 
-                 algo_type="Downwind", **algo_pars):
+
+def read_anlyses(
+    analyses, mbook, farm, states, keymap={}, algo_type="Downwind", **algo_pars
+):
     """
     Reads a WindIO wind farm
 
     Parameters
     ----------
     analyses : dict
         The analyses sub-dict of the case
@@ -227,35 +230,31 @@
     states : foxes.states.States
         The states object
     keymap : dict
         Translation from windio to foxes keywords
     algo_type : str
         The default algorithm class name
     algo_pars : dict, optional
-        Additional parameters for the algorithm 
+        Additional parameters for the algorithm
         constructor
 
     Returns
     -------
     algo : foxes.core.Algorithm
         The algorithm
 
     """
     wmodel = analyses["wake_model"]["name"]
     wmodels = [keymap.get(wmodel, wmodel)]
 
     return Algorithm.new(
-        algo_type,
-        mbook,
-        farm,
-        states,
-        wake_models=wmodels,
-        **algo_pars
+        algo_type, mbook, farm, states, wake_models=wmodels, **algo_pars
     )
 
+
 def read_case(case_yaml, site_pars={}, farm_pars={}, ana_pars={}):
     """
     Reads a WindIO case
 
     Parameters
     ----------
     case_yaml : str
@@ -277,34 +276,34 @@
         The states object
     algo : foxes.core.Algorithm
         The algorithm
 
     """
     case_yaml = Path(case_yaml)
 
-    with open(case_yaml, 'r') as file:
+    with open(case_yaml, "r") as file:
         case = yaml.load(file, Loader=yaml.loader.BaseLoader)
-    
+
     site_yaml = case["site"]
     if site_yaml[0] == ".":
-        site_yaml = (case_yaml.parent/site_yaml).resolve()
+        site_yaml = (case_yaml.parent / site_yaml).resolve()
     states = read_site(site_yaml, **site_pars)
 
     farm_yaml = case["wind_farm"]
     if farm_yaml[0] == ".":
-        farm_yaml = (case_yaml.parent/farm_yaml).resolve()
+        farm_yaml = (case_yaml.parent / farm_yaml).resolve()
     mbook, farm = read_farm(farm_yaml, **farm_pars)
 
     attr_dict = case["attributes"]
-    algo = read_anlyses(attr_dict["analyses"], mbook, farm,
-                        states, **ana_pars)
+    algo = read_anlyses(attr_dict["analyses"], mbook, farm, states, **ana_pars)
 
     return mbook, farm, states, algo
 
-if __name__ == "__main__":
 
+if __name__ == "__main__":
     import argparse
+
     parser = argparse.ArgumentParser()
     parser.add_argument("case_yaml", help="The case yaml file")
     args = parser.parse_args()
 
-    read_case(args.case_yaml)
+    read_case(args.case_yaml)
```

### Comparing `foxes-0.3.4/foxes/models/farm_models/turbine2farm.py` & `foxes-0.3.5/foxes/models/farm_models/turbine2farm.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.4/foxes/models/model_book.py` & `foxes-0.3.5/foxes/models/model_book.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 import numpy as np
 
 import foxes.models as fm
 import foxes.variables as FV
 from foxes.utils import Dict
-from foxes.core import TurbineModel, RotorModel, FarmModel, PointDataModel, FarmController
+from foxes.core import (
+    TurbineModel,
+    RotorModel,
+    FarmModel,
+    PointDataModel,
+    FarmController,
+)
 
 
 class ModelBook:
     """
     Container for all kinds of models.
 
     Parameters
@@ -53,33 +59,40 @@
         values: foxes.core.WakeModel
     sources : foxes.utils.Dict
         All sources dict
 
     """
 
     def __init__(self, Pct_file=None):
-
         self.point_models = Dict(name="point_models")
         self.point_models["tke2ti"] = fm.point_models.TKE2TI()
 
         self.rotor_models = Dict(name="rotor_models")
         rvars = [FV.REWS, FV.REWS2, FV.REWS3, FV.TI, FV.RHO]
         self.rotor_models["centre"] = fm.rotor_models.CentreRotor(calc_vars=rvars)
         nlist = list(range(2, 11)) + [20]
         for n in nlist:
             self.rotor_models[f"grid{n**2}"] = fm.rotor_models.GridRotor(
                 calc_vars=rvars, n=n, reduce=True
             )
 
         self.turbine_types = Dict(name="turbine_types")
         self.turbine_types["null_type"] = fm.turbine_types.NullType()
-        self.turbine_types["NREL5MW"] = fm.turbine_types.PCtFile("NREL-5MW-D126-H90.csv")
-        self.turbine_types["DTU10MW"] = fm.turbine_types.PCtFile("DTU-10MW-D178d3-H119.csv")
-        self.turbine_types["IEA15MW"] = fm.turbine_types.PCtFile("IEA-15MW-D240-H150.csv")
-        self.turbine_types["IWT7.5MW"] = fm.turbine_types.PCtFile("IWT-7d5MW-D164-H100.csv")
+        self.turbine_types["NREL5MW"] = fm.turbine_types.PCtFile(
+            "NREL-5MW-D126-H90.csv"
+        )
+        self.turbine_types["DTU10MW"] = fm.turbine_types.PCtFile(
+            "DTU-10MW-D178d3-H119.csv"
+        )
+        self.turbine_types["IEA15MW"] = fm.turbine_types.PCtFile(
+            "IEA-15MW-D240-H150.csv"
+        )
+        self.turbine_types["IWT7.5MW"] = fm.turbine_types.PCtFile(
+            "IWT-7d5MW-D164-H100.csv"
+        )
         if Pct_file is not None:
             self.turbine_types["Pct"] = fm.turbine_types.PCtFile(Pct_file)
 
         self.turbine_models = Dict(
             name="turbine_models",
             kTI=fm.turbine_models.kTI(),
             kTI_02=fm.turbine_models.kTI(kTI=0.2),
@@ -90,14 +103,20 @@
             kTI_amb_04=fm.turbine_models.kTI(ti_var=FV.AMB_TI, kTI=0.4),
             kTI_amb_05=fm.turbine_models.kTI(ti_var=FV.AMB_TI, kTI=0.5),
             thrust2ct=fm.turbine_models.Thrust2Ct(),
             PMask=fm.turbine_models.PowerMask(),
             yaw2yawm=fm.turbine_models.YAW2YAWM(),
             yawm2yaw=fm.turbine_models.YAWM2YAW(),
         )
+        self.turbine_models["hubh_data"] = fm.turbine_models.RotorCentreCalc({
+            f"{FV.WD}_HH": FV.WD,
+            f"{FV.WS}_HH": FV.WS,
+            f"{FV.TI}_HH": FV.TI,
+            f"{FV.RHO}_HH": FV.RHO,
+        })
 
         self.farm_models = Dict(
             name="farm_models",
             **{
                 f"farm_{mname}": fm.farm_models.Turbine2FarmModel(m)
                 for mname, m in self.turbine_models.items()
             },
@@ -127,17 +146,19 @@
 
         self.wake_frames = Dict(
             name="wake_frames",
             rotor_wd=fm.wake_frames.RotorWD(var_wd=FV.WD),
             rotor_wd_farmo=fm.wake_frames.FarmOrder(),
             yawed=fm.wake_frames.YawedWakes(),
         )
-        stps = [1., 5., 10., 50., 100., 500.]
+        stps = [1.0, 5.0, 10.0, 50.0, 100.0, 500.0]
         for s in stps:
-            self.wake_frames[f"streamlines_{int(s)}"] = fm.wake_frames.Streamlines(step=s)
+            self.wake_frames[f"streamlines_{int(s)}"] = fm.wake_frames.Streamlines(
+                step=s
+            )
         for s in stps:
             self.wake_frames[f"streamlines_{int(s)}_yawed"] = fm.wake_frames.YawedWakes(
                 base_frame=fm.wake_frames.Streamlines(step=s)
             )
         for s in stps:
             self.wake_frames[f"streamlines_{int(s)}_farmo"] = fm.wake_frames.FarmOrder(
                 base_frame=fm.wake_frames.Streamlines(step=s)
@@ -163,14 +184,18 @@
             ),
             max=fm.wake_superpositions.MaxSuperposition(
                 scalings=f"source_turbine_{FV.REWS}"
             ),
             max_amb=fm.wake_superpositions.MaxSuperposition(
                 scalings=f"source_turbine_{FV.AMB_REWS}"
             ),
+            product=fm.wake_superpositions.ProductSuperposition(),
+            product_lim=fm.wake_superpositions.ProductSuperposition(
+                lim_low={FV.WS: 1e-4},
+            ),
             ti_linear=fm.wake_superpositions.TISuperposition(
                 ti_superp="linear", superp_to_amb="quadratic"
             ),
             ti_quadratic=fm.wake_superpositions.TISuperposition(
                 ti_superp="quadratic", superp_to_amb="quadratic"
             ),
             ti_max=fm.wake_superpositions.TISuperposition(
@@ -183,17 +208,18 @@
             "linear",
             "linear_lim",
             "linear_amb",
             "quadratic",
             "quadratic_amb",
             "max",
             "max_amb",
+            "product",
+            "product_lim",
         ]
         for s in slist:
-
             self.wake_models[f"Jensen_{s}"] = fm.wake_models.wind.JensenWake(
                 superposition=s
             )
             self.wake_models[f"Jensen_{s}_k002"] = fm.wake_models.wind.JensenWake(
                 k=0.02, superposition=s
             )
             self.wake_models[f"Jensen_{s}_k004"] = fm.wake_models.wind.JensenWake(
@@ -205,20 +231,20 @@
             self.wake_models[f"Jensen_{s}_k0075"] = fm.wake_models.wind.JensenWake(
                 k=0.075, superposition=s
             )
 
             self.wake_models[f"Bastankhah_{s}"] = fm.wake_models.wind.BastankhahWake(
                 superposition=s
             )
-            self.wake_models[f"Bastankhah_{s}_k002"] = fm.wake_models.wind.BastankhahWake(
-                k=0.02, superposition=s
-            )
-            self.wake_models[f"Bastankhah_{s}_k004"] = fm.wake_models.wind.BastankhahWake(
-                k=0.04, superposition=s
-            )
+            self.wake_models[
+                f"Bastankhah_{s}_k002"
+            ] = fm.wake_models.wind.BastankhahWake(k=0.02, superposition=s)
+            self.wake_models[
+                f"Bastankhah_{s}_k004"
+            ] = fm.wake_models.wind.BastankhahWake(k=0.04, superposition=s)
 
             self.wake_models[f"PorteAgel_{s}"] = fm.wake_models.wind.PorteAgelWake(
                 superposition=s
             )
             self.wake_models[f"PorteAgel_{s}_k002"] = fm.wake_models.wind.PorteAgelWake(
                 superposition=s, k=0.02
             )
@@ -230,22 +256,22 @@
                 A=0.02, superposition=s
             )
             self.wake_models[f"TurbOPark_{s}_A004"] = fm.wake_models.wind.TurbOParkWake(
                 A=0.04, superposition=s
             )
 
             As = [0.02, 0.04]
-            dxs = [0.01, 1., 5., 10., 50., 100.]
+            dxs = [0.01, 1.0, 5.0, 10.0, 50.0, 100.0]
             for A in As:
                 for dx in dxs:
                     a = str(A).replace(".", "")
                     d = str(dx).replace(".", "") if dx < 1 else int(dx)
-                    self.wake_models[f"TurbOParkIX_{s}_A{a}_dx{d}"] = fm.wake_models.wind.TurbOParkWakeIX(
-                        A=A, superposition=s, dx=dx
-                    )
+                    self.wake_models[
+                        f"TurbOParkIX_{s}_A{a}_dx{d}"
+                    ] = fm.wake_models.wind.TurbOParkWakeIX(A=A, superposition=s, dx=dx)
 
         slist = ["ti_linear", "ti_quadratic", "ti_max"]
         for s in slist:
             self.wake_models[
                 f"CrespoHernandez_{s[3:]}"
             ] = fm.wake_models.ti.CrespoHernandezTIWake(superposition=s)
             self.wake_models[
```

### Comparing `foxes-0.3.4/foxes/models/partial_wakes/axiwake.py` & `foxes-0.3.5/foxes/models/partial_wakes/axiwake.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         algo.update_idata(self.rotor_model, idata=idata, verbosity=verbosity)
 
         for w in self.wake_models:
             if not isinstance(w, AxisymmetricWakeModel):
                 raise TypeError(
                     f"Partial wakes '{self.name}': Cannot be applied to wake model '{w.name}', since not an AxisymmetricWakeModel"
                 )
-        
+
         return idata
 
     def new_wake_deltas(self, algo, mdata, fdata):
         """
         Creates new initial wake deltas, filled
         with zeros.
 
@@ -164,15 +164,14 @@
             n[sel] /= R[sel][:, None]
         if np.any(~sel):
             n[:, :, 0][~sel] = 1
 
         # case wake centre outside rotor disk:
         sel = (x > 1e-5) & (R > D / 2)
         if np.any(sel):
-
             n_sel = np.sum(sel)
             Rsel = np.zeros((n_sel, self.n + 1), dtype=FC.DTYPE)
             Rsel[:] = R[sel][:, None]
             Dsel = D[sel][:, None]
 
             # equal delta R2:
             R1 = np.zeros((n_sel, self.n + 1), dtype=FC.DTYPE)
@@ -186,15 +185,14 @@
             hA = hA[:, 1:] - hA[:, :-1]
             weights[sel] = hA / np.sum(hA, axis=-1)[:, None]
             del hA, Rsel, Dsel, R1, R2
 
         # case wake centre inside rotor disk:
         sel = (x > 1e-5) & (R < D / 2)
         if np.any(sel):
-
             n_sel = np.sum(sel)
             Rsel = np.zeros((n_sel, self.n + 1), dtype=FC.DTYPE)
             Rsel[:] = R[sel][:, None]
             Dsel = D[sel][:, None]
 
             # equal delta R2:
             R1 = np.zeros((n_sel, self.n + 1), dtype=FC.DTYPE)
@@ -213,21 +211,19 @@
             hA = calc_area(R1, R2, Rsel)
             hA = hA[:, 1:] - hA[:, :-1]
             weights[sel] = hA / np.sum(hA, axis=-1)[:, None]
             del hA, hr, Rsel, Dsel, R1, R2
 
         # evaluate wake models:
         for w in self.wake_models:
-
             wdeltas, sp_sel = w.calc_wakes_spsel_x_r(
                 algo, mdata, fdata, states_source_turbine, x, r
             )
 
             for v, wdel in wdeltas.items():
-
                 d = np.einsum("ps,ps->p", wdel, weights[sp_sel])
 
                 try:
                     superp = w.superp[v]
                 except KeyError:
                     raise KeyError(
                         f"Model '{self.name}': Missing wake superposition entry for variable '{v}' in wake model '{w.name}', found {sorted(list(w.superp.keys()))}"
@@ -268,17 +264,17 @@
             For each state, the index of one turbine
             for which to evaluate the wake deltas.
             Shape: (n_states,)
         update_amb_res : bool
             Flag for updating ambient results
 
         """
-        weights = self.get_data(FV.RWEIGHTS, mdata)
-        amb_res = self.get_data(FV.AMB_RPOINT_RESULTS, mdata)
-        rpoints = self.get_data(FV.RPOINTS, mdata)
+        weights = self.get_data(FC.RWEIGHTS, mdata)
+        amb_res = self.get_data(FC.AMB_RPOINT_RESULTS, mdata)
+        rpoints = self.get_data(FC.RPOINTS, mdata)
         n_states, n_turbines, n_rpoints, __ = rpoints.shape
 
         wres = {}
         st_sel = (np.arange(n_states), states_turbine)
         for v, ares in amb_res.items():
             wres[v] = ares.reshape(n_states, n_turbines, n_rpoints)[st_sel]
         del amb_res
@@ -289,15 +285,15 @@
         for w in self.wake_models:
             w.finalize_wake_deltas(algo, mdata, fdata, wres, wdel)
 
         for v in wres.keys():
             if v in wake_deltas:
                 wres[v] += wdel[v]
                 if update_amb_res:
-                    mdata[FV.AMB_RPOINT_RESULTS][v][st_sel] = wres[v]
+                    mdata[FC.AMB_RPOINT_RESULTS][v][st_sel] = wres[v]
             wres[v] = wres[v][:, None]
 
         self.rotor_model.eval_rpoint_results(
             algo, mdata, fdata, wres, weights, states_turbine=states_turbine
         )
 
     def finalize(self, algo, verbosity=0):
```

### Comparing `foxes-0.3.4/foxes/models/partial_wakes/distsliced.py` & `foxes-0.3.5/foxes/models/partial_wakes/distsliced.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,17 +91,18 @@
                 raise TypeError(
                     f"Partial wakes '{self.name}': Cannot be applied to wake model '{w.name}', since not an DistSlicedWakeModel"
                 )
 
         self.YZ = self.var("YZ")
         self.W = self.var(FV.WEIGHT)
 
-        algo.update_idata([self.rotor_model, self.grotor], 
-            idata=idata, verbosity=verbosity)
-        
+        algo.update_idata(
+            [self.rotor_model, self.grotor], idata=idata, verbosity=verbosity
+        )
+
         return idata
 
     def new_wake_deltas(self, algo, mdata, fdata):
         """
         Creates new initial wake deltas, filled
         with zeros.
 
@@ -172,25 +173,23 @@
             algo, mdata, fdata, states_source_turbine, points
         )
         yz = wcoos.reshape(n_states, n_turbines, n_rpoints, 3)[:, :, :, 1:3]
         del points, wcoos
 
         # evaluate wake models:
         for w in self.wake_models:
-
             wdeltas, sp_sel = w.calc_wakes_spsel_x_yz(
                 algo, mdata, fdata, states_source_turbine, x, yz
             )
 
             wsps = np.zeros((n_states, n_turbines, n_rpoints), dtype=bool)
             wsps[:] = sp_sel[:, :, None]
             wsps = wsps.reshape(n_states, n_points)
 
             for v, wdel in wdeltas.items():
-
                 d = np.zeros((n_states, n_turbines, n_rpoints), dtype=FC.DTYPE)
                 d[sp_sel] = wdel
                 d = d.reshape(n_states, n_points)[wsps]
 
                 try:
                     superp = w.superp[v]
                 except KeyError:
@@ -233,17 +232,17 @@
             For each state, the index of one turbine
             for which to evaluate the wake deltas.
             Shape: (n_states,)
         update_amb_res : bool
             Flag for updating ambient results
 
         """
-        amb_res = self.get_data(FV.AMB_RPOINT_RESULTS, mdata)
-        rpoints = self.get_data(FV.RPOINTS, mdata)
-        rweights = self.get_data(FV.RWEIGHTS, mdata)
+        amb_res = self.get_data(FC.AMB_RPOINT_RESULTS, mdata)
+        rpoints = self.get_data(FC.RPOINTS, mdata)
+        rweights = self.get_data(FC.RWEIGHTS, mdata)
         wweights = self.grotor.rotor_point_weights()
         n_wpoints = self.grotor.n_rotor_points()
         n_states, n_turbines, n_rpoints, __ = rpoints.shape
         st_sel = (np.arange(n_states), states_turbine)
 
         uv = None
         if (FV.WS in amb_res and FV.WD not in amb_res) or (
@@ -252,15 +251,14 @@
             raise KeyError(
                 f"Model '{self.name}': Missing one of the variables '{FV.WS}', '{FV.WD}' in ambient rotor results: {list(amb_res.keys())}"
             )
 
         elif FV.WD in amb_res and np.any(
             np.min(amb_res[FV.WD], axis=2) != np.max(amb_res[FV.WD], axis=2)
         ):
-
             wd = amb_res[FV.WD].reshape(n_states, n_turbines, n_rpoints)[st_sel]
             ws = amb_res[FV.WS].reshape(n_states, n_turbines, n_rpoints)[st_sel]
             uv = wd2uv(wd, ws, axis=-1)
             uv = np.einsum("spd,p->sd", uv, rweights)
             del ws, wd
 
         wres = {}
@@ -283,15 +281,15 @@
         for v in wdel.keys():
             wdel[v] = np.einsum("sp,p->s", wdel[v], wweights)[:, None]
 
         for v in wres.keys():
             if v in wake_deltas:
                 wres[v] += wdel[v]
                 if update_amb_res:
-                    mdata[FV.AMB_RPOINT_RESULTS][v][st_sel] = wres[v]
+                    mdata[FC.AMB_RPOINT_RESULTS][v][st_sel] = wres[v]
             wres[v] = wres[v][:, None]
 
         self.rotor_model.eval_rpoint_results(
             algo, mdata, fdata, wres, np.array([1.0]), states_turbine=states_turbine
         )
 
     def finalize(self, algo, verbosity=0):
```

### Comparing `foxes-0.3.4/foxes/models/partial_wakes/grid.py` & `foxes-0.3.5/foxes/models/partial_wakes/grid.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.4/foxes/models/partial_wakes/mapped.py` & `foxes-0.3.5/foxes/models/partial_wakes/mapped.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,14 @@
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         idata = super().initialize(algo, verbosity)
 
         pws = {}
         for w in self.wake_models:
-
             pdat = None
             if w.name in self.wname2pwake:
                 pdat = deepcopy(self.wname2pwake[w.name])
 
             if pdat is None:
                 for pwcls, tdat in self.wtype2pwake.items():
                     if isinstance(w, pwcls):
@@ -116,15 +115,15 @@
         self._pwakes = []
         for pname, pars in pws.items():
             if verbosity:
                 print(
                     f"Partial wakes '{self.name}': Applying {pname} to {[w.name for w in pars['wake_models']]}"
                 )
             self._pwakes.append(PartialWakesModel.new(pname, **pars))
-        
+
         algo.update_idata(self._pwakes, idata=idata, verbosity=verbosity)
 
         return idata
 
     def new_wake_deltas(self, algo, mdata, fdata):
         """
         Creates new initial wake deltas, filled
```

### Comparing `foxes-0.3.4/foxes/models/partial_wakes/rotor_points.py` & `foxes-0.3.5/foxes/models/partial_wakes/rotor_points.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 
 from foxes.core import PartialWakesModel
 import foxes.variables as FV
-
+import foxes.constants as FC
 
 class RotorPoints(PartialWakesModel):
     """
     Partial wakes calculation directly by the
     rotor model.
 
     Parameters
@@ -68,15 +68,15 @@
 
         Returns
         -------
         rpoints : numpy.ndarray
             All rotor points, shape: (n_states, n_points, 3)
 
         """
-        rpoints = self.get_data(FV.RPOINTS, mdata)
+        rpoints = self.get_data(FC.RPOINTS, mdata)
         n_states, n_turbines, n_rpoints, __ = rpoints.shape
         return rpoints.reshape(n_states, n_turbines * n_rpoints, 3)
 
     def new_wake_deltas(self, algo, mdata, fdata):
         """
         Creates new initial wake deltas, filled
         with zeros.
@@ -162,17 +162,17 @@
             For each state, the index of one turbine
             for which to evaluate the wake deltas.
             Shape: (n_states,)
         update_amb_res : bool
             Flag for updating ambient results
 
         """
-        weights = self.get_data(FV.RWEIGHTS, mdata)
-        amb_res = self.get_data(FV.AMB_RPOINT_RESULTS, mdata)
-        rpoints = self.get_data(FV.RPOINTS, mdata)
+        weights = self.get_data(FC.RWEIGHTS, mdata)
+        amb_res = self.get_data(FC.AMB_RPOINT_RESULTS, mdata)
+        rpoints = self.get_data(FC.RPOINTS, mdata)
         n_states, n_turbines, n_rpoints, __ = rpoints.shape
 
         wres = {}
         st_sel = (np.arange(n_states), states_turbine)
         for v, ares in amb_res.items():
             wres[v] = ares.reshape(n_states, n_turbines, n_rpoints)[st_sel]
         del amb_res
@@ -183,13 +183,13 @@
         for w in self.wake_models:
             w.finalize_wake_deltas(algo, mdata, fdata, wres, wdel)
 
         for v in wres.keys():
             if v in wake_deltas:
                 wres[v] += wdel[v]
                 if update_amb_res:
-                    mdata[FV.AMB_RPOINT_RESULTS][v][st_sel] = wres[v]
+                    mdata[FC.AMB_RPOINT_RESULTS][v][st_sel] = wres[v]
             wres[v] = wres[v][:, None]
 
         algo.rotor_model.eval_rpoint_results(
             algo, mdata, fdata, wres, weights, states_turbine=states_turbine
         )
```

### Comparing `foxes-0.3.4/foxes/models/partial_wakes/top_hat.py` & `foxes-0.3.5/foxes/models/partial_wakes/top_hat.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,28 +172,25 @@
 
         ct = np.zeros((n_states, n_points), dtype=FC.DTYPE)
         ct[:] = fdata[FV.CT][stsel][:, None]
         x = mdata[self.WCOOS_X]
 
         sel0 = (ct > 0.0) & (x > 0.0)
         if np.any(sel0):
-
             R = mdata[self.WCOOS_R]
             r = np.zeros_like(R)
             D = fdata[FV.D]
 
             for w in self.wake_models:
-
                 wr = w.calc_wake_radius(
                     algo, mdata, fdata, states_source_turbine, x, ct
                 )
 
                 sel_sp = sel0 & (wr > R - D / 2)
                 if np.any(sel_sp):
-
                     hx = x[sel_sp]
                     hct = ct[sel_sp]
                     hwr = wr[sel_sp]
 
                     clw = w.calc_centreline_wake_deltas(
                         algo, mdata, fdata, states_source_turbine, sel_sp, hx, hwr, hct
                     )
@@ -247,17 +244,17 @@
             For each state, the index of one turbine
             for which to evaluate the wake deltas.
             Shape: (n_states,)
         update_amb_res : bool
             Flag for updating ambient results
 
         """
-        weights = self.get_data(FV.RWEIGHTS, mdata)
-        amb_res = self.get_data(FV.AMB_RPOINT_RESULTS, mdata)
-        rpoints = self.get_data(FV.RPOINTS, mdata)
+        weights = self.get_data(FC.RWEIGHTS, mdata)
+        amb_res = self.get_data(FC.AMB_RPOINT_RESULTS, mdata)
+        rpoints = self.get_data(FC.RPOINTS, mdata)
         n_states, n_turbines, n_rpoints, __ = rpoints.shape
 
         wres = {}
         st_sel = (np.arange(n_states), states_turbine)
         for v, ares in amb_res.items():
             wres[v] = ares.reshape(n_states, n_turbines, n_rpoints)[st_sel]
         del amb_res
@@ -268,15 +265,15 @@
         for w in self.wake_models:
             w.finalize_wake_deltas(algo, mdata, fdata, wres, wdel)
 
         for v in wres.keys():
             if v in wake_deltas:
                 wres[v] += wdel[v]
                 if update_amb_res:
-                    mdata[FV.AMB_RPOINT_RESULTS][v][st_sel] = wres[v]
+                    mdata[FC.AMB_RPOINT_RESULTS][v][st_sel] = wres[v]
             wres[v] = wres[v][:, None]
 
         self.rotor_model.eval_rpoint_results(
             algo, mdata, fdata, wres, weights, states_turbine=states_turbine
         )
 
     def finalize(self, algo, verbosity=0):
```

### Comparing `foxes-0.3.4/foxes/models/point_models/set_uniform_data.py` & `foxes-0.3.5/foxes/models/point_models/set_uniform_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         output_vars,
         var2col={},
         pd_read_pars={},
     ):
         self.data_source = data_source
         self.ovars = output_vars
         self.var2col = var2col
-        
+
         self._rpars = pd_read_pars
 
     def initialize(self, algo, verbosity=0):
         """
         Initializes the model.
 
         This includes loading all required data from files. The model
@@ -85,21 +85,19 @@
             pass
         else:
             if verbosity:
                 print(f"States '{self.name}': Reading file {self.data_source}")
             rpars = dict(index_col=0)
             rpars.update(self._rpars)
             data = PandasFileHelper().read_file(self.data_source, **rpars)
-            data = data[
-                [self.var2col.get(v, v) for v in self.ovars]
-            ].to_numpy(FC.DTYPE)
+            data = data[[self.var2col.get(v, v) for v in self.ovars]].to_numpy(FC.DTYPE)
 
         idata = super().initialize(algo, verbosity)
         idata["coords"][self.VARS] = self.ovars
-        idata["data_vars"][self.DATA] = ((FV.STATE, self.VARS), data)
+        idata["data_vars"][self.DATA] = ((FC.STATE, self.VARS), data)
 
         return idata
 
     def output_point_vars(self, algo):
         """
         The variables which are being modified by the model.
```

### Comparing `foxes-0.3.4/foxes/models/point_models/tke2ti.py` & `foxes-0.3.5/foxes/models/point_models/tke2ti.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.4/foxes/models/point_models/wake_deltas.py` & `foxes-0.3.5/foxes/models/point_models/wake_deltas.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.4/foxes/models/rotor_models/centre.py` & `foxes-0.3.5/foxes/models/rotor_models/centre.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,54 +140,50 @@
             FV.WS in self.calc_vars
             or FV.WD in self.calc_vars
             or FV.YAW in self.calc_vars
             or FV.REWS in self.calc_vars
             or FV.REWS2 in self.calc_vars
             or FV.REWS3 in self.calc_vars
         ):
-
             wd = rpoint_results[FV.WD]
             ws = rpoint_results[FV.WS]
             uvp = wd2uv(wd, ws, axis=-1)
             uv = uvp[:, :, 0]
 
         wd = None
         vdone = []
         for v in self.calc_vars:
-
             if v not in fdata:
                 fdata[v] = np.zeros((n_states, n_turbines), dtype=FC.DTYPE)
 
             if v == FV.WD or v == FV.YAW:
                 if wd is None:
                     wd = uv2wd(uv, axis=-1)
                 self._set_res(fdata, v, wd, stsel)
                 vdone.append(v)
 
             elif v == FV.WS:
-                self._set_res(fdata, v, ws, stsel)
+                self._set_res(fdata, v, ws[:, :, 0], stsel)
                 del ws
                 vdone.append(v)
         del uv, wd
 
         if (
             FV.REWS in self.calc_vars
             or FV.REWS2 in self.calc_vars
             or FV.REWS3 in self.calc_vars
         ):
-
             if stsel is None:
                 yaw = fdata[FV.YAW]
             else:
                 yaw = fdata[FV.YAW][stsel][:, None]
             nax = wd2uv(yaw, axis=-1)
             wsp = np.einsum("stpd,std->stp", uvp, nax)
 
             for v in self.calc_vars:
-
                 if v == FV.REWS or v == FV.REWS2 or v == FV.REWS3:
                     rews = wsp[:, :, 0]
                     self._set_res(fdata, v, rews, stsel)
                     del rews
                     vdone.append(v)
 
             del wsp
```

### Comparing `foxes-0.3.4/foxes/models/rotor_models/grid.py` & `foxes-0.3.5/foxes/models/rotor_models/grid.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,19 +81,17 @@
         x, y = np.meshgrid(x, x, indexing="ij")
 
         self.dpoints = np.zeros([N, 3], dtype=FC.DTYPE)
         self.dpoints[:, 1] = x.reshape(N)
         self.dpoints[:, 2] = y.reshape(N)
 
         if self.reduce:
-
             self.weights = np.zeros((self.n, self.n), dtype=FC.DTYPE)
             for i in range(0, self.n):
                 for j in range(0, self.n):
-
                     d = delta / self.nint
                     hx = [
                         x[i, j] - delta / 2.0 + (k + 0.5) * d for k in range(self.nint)
                     ]
                     hy = [
                         y[i, j] - delta / 2.0 + (k + 0.5) * d for k in range(self.nint)
                     ]
@@ -106,15 +104,14 @@
             self.weights = self.weights.reshape(N)
             sel = self.weights > 0.0
             self.dpoints = self.dpoints[sel]
             self.weights = self.weights[sel]
             self.weights /= np.sum(self.weights)
 
         else:
-
             self.dpoints[:, 1] = x.reshape(N)
             self.dpoints[:, 2] = y.reshape(N)
             self.weights = np.ones(N, dtype=FC.DTYPE) / N
 
         return super().initialize(algo, verbosity)
 
     def n_rotor_points(self):
```

### Comparing `foxes-0.3.4/foxes/models/turbine_models/calculator.py` & `foxes-0.3.5/foxes/models/turbine_models/calculator.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,29 +11,29 @@
     ----------
     in_vars : list of str
         The input farm vairables
     out_vars : list of str
         The output variables
     func : Function
         The function: f(in0, in1, ..., stsel) -> (out0, ou1, ...)
-        where inX and outY are numpy.ndarrays and 
+        where inX and outY are numpy.ndarrays and
         st_sel is the boolean state-turbine selection.
         All arrays have shape (n_states, n_turbines).
     kwargs : dict, optional
         Additional arguments for TurbineModel
 
     Attributes
     ----------
     in_vars : list of str
         The input farm vairables
     out_vars : list of str
         The output variables
     func : Function
         The function: f(in0, in1, ..., stsel) -> (out0, ou1, ...)
-        where inX and outY are numpy.ndarrays and 
+        where inX and outY are numpy.ndarrays and
         st_sel is the boolean state-turbine selection.
         All arrays have shape (n_states, n_turbines).
 
     """
 
     def __init__(self, in_vars, out_vars, func, **kwargs):
         super().__init__(**kwargs)
```

### Comparing `foxes-0.3.4/foxes/models/turbine_models/kTI_model.py` & `foxes-0.3.5/foxes/models/turbine_models/kTI_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,27 +19,37 @@
         Uniform value for `kb`. If not given it
         will be searched in farm data, and zero by default
     ti_var : str
         The `TI` variable name
     ti_val : float, optional
         The uniform value of `TI`. If not given it
         will be searched in farm data
+    k_var : str
+        The variable name for k
+
+    Attributes
+    ----------
+    ti_var : str
+        The `TI` variable name
+    k_var : str
+        The variable name for k
 
     """
 
-    def __init__(self, kTI=None, kb=None, ti_var=FV.TI, ti_val=None):
+    def __init__(self, kTI=None, kb=None, ti_var=FV.TI, ti_val=None, k_var=FV.K):
         super().__init__()
 
         self.ti_var = ti_var
+        self.k_var = k_var
         setattr(self, ti_var, ti_val)
         setattr(self, FV.KTI, kTI)
         setattr(self, FV.KB, 0 if kb is None else kb)
 
     def __repr__(self):
-        return super().__repr__() + f"(kTI={getattr(self, FV.KTI)}, ti={self.ti_var})"
+        return super().__repr__() + f"({self.k_var}, kTI={getattr(self, FV.KTI)}, ti={self.ti_var})"
 
     def output_farm_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
@@ -48,15 +58,15 @@
 
         Returns
         -------
         output_vars : list of str
             The output variable names
 
         """
-        return [FV.K]
+        return [self.k_var]
 
     def calculate(self, algo, mdata, fdata, st_sel):
         """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
@@ -81,13 +91,13 @@
 
         """
         kTI = self.get_data(FV.KTI, fdata, st_sel)
         kb = self.get_data(FV.KB, fdata, st_sel)
         ti = self.get_data(self.ti_var, fdata, st_sel)
 
         k = fdata.get(
-            FV.K, np.zeros((fdata.n_states, fdata.n_turbines), dtype=FC.DTYPE)
+            self.k_var, np.zeros((fdata.n_states, fdata.n_turbines), dtype=FC.DTYPE)
         )
 
         k[st_sel] = kTI * ti + kb
 
-        return {FV.K: k}
+        return {self.k_var: k}
```

### Comparing `foxes-0.3.4/foxes/models/turbine_models/power_mask.py` & `foxes-0.3.5/foxes/models/turbine_models/power_mask.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,31 +82,31 @@
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         self._P_rated = []
         for t in algo.farm_controller.turbine_types:
             Pnom = FC.DTYPE(t.P_nominal)
             if np.isnan(Pnom):
-                raise ValueError(f"Model '{self.name}': P_nominal is NaN for turbine type '{t.name}'")
+                raise ValueError(
+                    f"Model '{self.name}': P_nominal is NaN for turbine type '{t.name}'"
+                )
             self._P_rated.append(Pnom)
         self._P_rated = np.array(self._P_rated, dtype=FC.DTYPE)
-        
+
         return super().initialize(algo, verbosity)
 
     @classmethod
     def update_P_ct(cls, data, max_P, rated_P, factor_P, var_ws=FV.REWS3, P_lim=100):
-
         # select power entries for which this is active:
         P = data[FV.P]
         sel = ~np.isnan(max_P) & (
             ((max_P < rated_P) & (P > max_P))
             | ((max_P > rated_P) & (P > rated_P - P_lim))
         )
         if np.any(sel):
-
             # apply selection:
             max_P = max_P[sel]
             ws = data[var_ws][sel]
             rho = data[FV.RHO][sel]
             r = data[FV.D][sel] / 2
             P = P[sel]
             ct = data[FV.CT][sel]
@@ -164,15 +164,15 @@
         Returns
         -------
         results : dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
-        
+
         # prepare:
         max_P = fdata[FV.MAX_P]
         rated_P = self._P_rated[None, :]
 
         # calculate:
         self.update_P_ct(fdata, max_P, rated_P, self.factor_P, var_ws=self.var_ws_P)
```

### Comparing `foxes-0.3.4/foxes/models/turbine_models/sector_management.py` & `foxes-0.3.5/foxes/models/turbine_models/sector_management.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 import pandas as pd
 
 from foxes.core import TurbineModel
 from foxes.utils import PandasFileHelper
 import foxes.variables as FV
-
+import foxes.constants as FC
 
 class SectorManagement(TurbineModel):
     """
     Changes variables based on variable range conditions.
 
     Parameters
     ----------
@@ -60,14 +60,15 @@
         self._tvars = target_vars
         self._colmap = colmap
         self._perds = var_periods
         self._rpars = pd_file_read_pars
 
         self._rdata = None
         self._tdata = None
+        self._trbs = None
 
     def initialize(self, algo, verbosity=0):
         """
         Initializes the model.
 
         This includes loading all required data from files. The model
         should return all array type data as part of the idata return
@@ -93,31 +94,31 @@
         if isinstance(self.source, pd.DataFrame):
             data = self.source
         else:
             if verbosity > 0:
                 print(f"{self.name}: Reading file {self.source}")
             data = PandasFileHelper.read_file(self.source, **self._rpars)
 
-        if self._col_i is not None and self._col_t is None:
-            data.reset_index(inplace=True)
-        elif self._col_i is None and self._col_t is not None:
-            tnames = algo.farm.turbine_names
-            inds = [tnames.index(name) for name in data[self._col_t]]
-            data[FV.TURBINE] = inds
-            self._col_i = FV.TURBINE
-        else:
-            raise KeyError(
-                f"{self.name}: Please either specify 'col_tinds' or 'col_tnames'"
-            )
-        self._trbs = data[self._col_i].to_numpy()
+        if self._trbs is None:
+            if self._col_i is not None and self._col_t is None:
+                data.reset_index(inplace=True)
+            elif self._col_i is None and self._col_t is not None:
+                tnames = algo.farm.turbine_names
+                inds = [tnames.index(name) for name in data[self._col_t]]
+                data[FC.TURBINE] = inds
+                self._col_i = FC.TURBINE
+            else:
+                raise KeyError(
+                    f"{self.name}: Please either specify 'col_tinds' or 'col_tnames'"
+                )
+            self._trbs = data[self._col_i].to_numpy()
         n_trbs = len(self._trbs)
 
         self._rcols = []
         for v in self._rvars:
-
             col_vmin = f"{v}_min"
             col_vmin = self._colmap.get(col_vmin, col_vmin)
             if col_vmin not in data.columns:
                 raise KeyError(
                     f"{self.name}: Missing column '{col_vmin}', maybe add it to 'colmap'?"
                 )
```

### Comparing `foxes-0.3.4/foxes/models/turbine_models/set_XYHD.py` & `foxes-0.3.5/foxes/models/turbine_models/set_XYHD.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,14 @@
                 fdata[FV.Y] = fdata[FV.TXYH][..., 1]
             if self.set_H:
                 fdata[FV.H] = fdata[FV.TXYH][..., 2]
 
         for ti in range(n_turbines):
             ssel = st_sel[:, ti]
             if np.any(ssel):
-
                 if np.all(ssel):
                     ssel = np.s_[:]
 
                 if self.set_XY:
                     fdata[FV.X][ssel, ti] = algo.farm.turbines[ti].xy[0]
                     fdata[FV.Y][ssel, ti] = algo.farm.turbines[ti].xy[1]
```

### Comparing `foxes-0.3.4/foxes/models/turbine_models/set_farm_vars.py` & `foxes-0.3.5/foxes/models/turbine_models/set_farm_vars.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import numpy as np
 
 from foxes.core import TurbineModel
 import foxes.constants as FC
-import foxes.variables as FV
-
 
 class SetFarmVars(TurbineModel):
     """
     Set farm data variables to given data.
 
     Parameters
     ----------
@@ -89,19 +87,18 @@
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         idata = super().initialize(algo, verbosity)
 
         for i, v in enumerate(self.vars):
-
             data = np.full((algo.n_states, algo.n_turbines), np.nan, dtype=FC.DTYPE)
             data[:] = self._vdata[i]
 
-            idata["data_vars"][self.var(v)] = ((FV.STATE, FV.TURBINE), data)
+            idata["data_vars"][self.var(v)] = ((FC.STATE, FC.TURBINE), data)
 
         return idata
 
     def calculate(self, algo, mdata, fdata, st_sel):
         """ "
         The main model calculation.
 
@@ -128,24 +125,22 @@
 
         """
         n_states = fdata.n_states
         n_turbines = fdata.n_turbines
         allt = np.all(st_sel)
 
         for v in self.vars:
-
             data = mdata[self.var(v)]
             hsel = ~np.isnan(data)
             hallt = np.all(hsel)
 
             if allt and hallt:
                 fdata[v][:] = data
 
             else:
-
                 if v not in fdata:
                     fdata[v] = np.full((n_states, n_turbines), np.nan, dtype=FC.DTYPE)
 
                 tsel = st_sel & hsel
                 fdata[v][tsel] = data[tsel]
 
         return {v: fdata[v] for v in self.vars}
```

### Comparing `foxes-0.3.4/foxes/models/turbine_models/table_factors.py` & `foxes-0.3.5/foxes/models/turbine_models/table_factors.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.4/foxes/models/turbine_models/thrust2ct.py` & `foxes-0.3.5/foxes/models/turbine_models/thrust2ct.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.4/foxes/models/turbine_models/yaw2yawm.py` & `foxes-0.3.5/foxes/models/turbine_models/yaw2yawm.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.4/foxes/models/turbine_models/yawm2yaw.py` & `foxes-0.3.5/foxes/models/turbine_models/yawm2yaw.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.4/foxes/models/turbine_types/CpCt_file.py` & `foxes-0.3.5/foxes/models/turbine_types/CpCt_file.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
 import pandas as pd
 
 from .PCt_file import PCtFile
 from foxes.data import parse_Pct_file_name
 from foxes.utils import PandasFileHelper
 
+
 class CpCtFile(PCtFile):
     """
     Calculate power and ct by interpolating
     from cp-ct-curve data file (or pandas DataFrame).
 
     Parameters
     ----------
@@ -39,15 +40,15 @@
         if not isinstance(data_source, pd.DataFrame):
             pars = parse_Pct_file_name(data_source)
             pars.update(parameters)
             data = PandasFileHelper.read_file(data_source, **pd_file_read_pars)
         else:
             data = data_source
             pars = parameters
-        
+
         D = pars["D"]
-        A = np.pi*(D/2)**2
+        A = np.pi * (D / 2) ** 2
         ws = data[col_ws].to_numpy()
         cp = data[col_cp].to_numpy()
-        data["P"] = 0.5*rho*A*cp*ws**3
+        data["P"] = 0.5 * rho * A * cp * ws**3
 
         super().__init__(data, col_ws=col_ws, col_P="P", rho=rho, **pars)
```

### Comparing `foxes-0.3.4/foxes/models/turbine_types/CpCt_from_two.py` & `foxes-0.3.5/foxes/models/turbine_types/CpCt_from_two.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 import pandas as pd
 
 from .PCt_from_two import PCtFromTwo
 from foxes.data import parse_Pct_two_files
 from foxes.utils import PandasFileHelper
 import foxes.constants as FC
 
+
 class CpCtFromTwo(PCtFromTwo):
     """
     Calculate power and ct by interpolating
-    cp and ct from two files (or two pandas 
+    cp and ct from two files (or two pandas
     DataFrames).
 
     Parameters
     ----------
     data_source_cp : str or pandas.DataFrame
         The file path, static name, or data
     data_source_ct : str or pandas.DataFrame
@@ -50,16 +51,23 @@
             pars = parse_Pct_two_files(data_source_cp, data_source_ct)
             data_cp = PandasFileHelper.read_file(data_source_cp, **pd_file_read_pars_cp)
             data_ct = PandasFileHelper.read_file(data_source_ct, **pd_file_read_pars_ct)
         else:
             data_cp = data_source_cp
             data_ct = data_source_ct
             pars = parameters
-        
+
         D = pars["D"]
-        A = np.pi*(D/2)**2
+        A = np.pi * (D / 2) ** 2
         ws = data_cp[col_ws_cp_file].to_numpy()
         cp = data_cp[col_cp].to_numpy()
-        data_cp["P"] = 0.5*rho*A*cp*ws**3 / FC.P_UNITS[FC.kW]
+        data_cp["P"] = 0.5 * rho * A * cp * ws**3 / FC.P_UNITS[FC.kW]
 
-        super().__init__(data_cp, data_ct, col_ws_P_file=col_ws_cp_file, col_P="P", 
-                         rho=rho, P_unit=FC.kW, **pars)
+        super().__init__(
+            data_cp,
+            data_ct,
+            col_ws_P_file=col_ws_cp_file,
+            col_P="P",
+            rho=rho,
+            P_unit=FC.kW,
+            **pars,
+        )
```

### Comparing `foxes-0.3.4/foxes/models/turbine_types/PCt_file.py` & `foxes-0.3.5/foxes/models/turbine_types/PCt_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from foxes.core import TurbineType
 from foxes.utils import PandasFileHelper
 from foxes.data import PCTCURVE, parse_Pct_file_name
 import foxes.variables as FV
 import foxes.constants as FC
 
+
 class PCtFile(TurbineType):
     """
     Calculate power and ct by interpolating
     from power-ct-curve data file (or pandas DataFrame).
 
     Parameters
     ----------
@@ -154,15 +155,17 @@
         self.data_ws = data.index.to_numpy()
         self.data_P = data[self.col_P].to_numpy()
         self.data_ct = data[self.col_ct].to_numpy()
 
         if self.P_nominal is None:
             self.P_nominal = np.max(self.data_P) / FC.P_UNITS[self.P_unit]
             if verbosity > 0:
-                print(f"Turbine type '{self.name}': Setting P_nominal = {self.P_nominal:.2f} {self.P_unit}")
+                print(
+                    f"Turbine type '{self.name}': Setting P_nominal = {self.P_nominal:.2f} {self.P_unit}"
+                )
 
         return super().initialize(algo, verbosity)
 
     def calculate(self, algo, mdata, fdata, st_sel):
         """ "
         The main model calculation.
 
@@ -189,26 +192,24 @@
 
         """
         rews2 = fdata[self.WSCT][st_sel]
         rews3 = fdata[self.WSP][st_sel]
 
         # apply air density correction:
         if self.rho is not None:
-
             # correct wind speed by air density, such
             # that in the partial load region the
             # correct value is reconstructed:
             rho = fdata[FV.RHO][st_sel]
             rews2 *= (self.rho / rho) ** 0.5
             rews3 *= (self.rho / rho) ** (1.0 / 3.0)
             del rho
 
         # in yawed case, calc yaw corrected wind speed:
         if FV.YAWM in fdata and (self.p_P is not None or self.p_ct is not None):
-
             # calculate corrected wind speed wsc,
             # gives ws**3 * cos**p_P in partial load region
             # and smoothly deals with full load region:
             yawm = fdata[FV.YAWM][st_sel]
             if np.any(np.isnan(yawm)):
                 raise ValueError(
                     f"{self.name}: Found NaN values for variable '{FV.YAWM}'. Maybe change order in turbine_models?"
```

### Comparing `foxes-0.3.4/foxes/models/turbine_types/PCt_from_two.py` & `foxes-0.3.5/foxes/models/turbine_types/PCt_from_two.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from foxes.core import TurbineType
 from foxes.utils import PandasFileHelper
 from foxes.data import PCTCURVE, parse_Pct_two_files
 import foxes.variables as FV
 import foxes.constants as FC
 
+
 class PCtFromTwo(TurbineType):
     """
     Calculate power and ct by interpolating
     from power curve and ct curve data files.
 
     Parameters
     ----------
@@ -83,15 +84,14 @@
         p_P=1.88,
         var_ws_ct=FV.REWS2,
         var_ws_P=FV.REWS3,
         pd_file_read_pars_P={},
         pd_file_read_pars_ct={},
         **parameters,
     ):
-
         if not isinstance(data_source_P, pd.DataFrame) or not isinstance(
             data_source_ct, pd.DataFrame
         ):
             pars = parse_Pct_two_files(data_source_P, data_source_ct)
         else:
             pars = parameters
         super().__init__(**pars)
@@ -157,40 +157,38 @@
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         # read power curve:
         if isinstance(self.source_P, pd.DataFrame):
             self._data_P = self.source_P
         else:
-            fpath = algo.dbook.get_file_path(
-                PCTCURVE, self.source_P, check_raw=True
-            )
+            fpath = algo.dbook.get_file_path(PCTCURVE, self.source_P, check_raw=True)
             self._data_P = PandasFileHelper.read_file(fpath, **self.rpars_P)
 
         self._data_P = self._data_P.set_index(self.col_ws_P_file).sort_index()
         self._data_ws_P = self._data_P.index.to_numpy()
         self._data_P = self._data_P[self.col_P].to_numpy()
 
         # read ct curve:
         if isinstance(self.source_ct, pd.DataFrame):
             self._data_ct = self.source_ct
         else:
-            fpath = algo.dbook.get_file_path(
-                PCTCURVE, self.source_ct, check_raw=True
-            )
+            fpath = algo.dbook.get_file_path(PCTCURVE, self.source_ct, check_raw=True)
             self._data_ct = PandasFileHelper.read_file(fpath, **self.rpars_ct)
 
         self._data_ct = self._data_ct.set_index(self.col_ws_ct_file).sort_index()
         self._data_ws_ct = self._data_ct.index.to_numpy()
         self._data_ct = self._data_ct[self.col_ct].to_numpy()
 
         if self.P_nominal is None:
             self.P_nominal = np.max(self._data_P) / FC.P_UNITS[self.P_unit]
             if verbosity > 0:
-                print(f"Turbine type '{self.name}': Setting P_nominal = {self.P_nominal:.2f} {self.P_unit}")
+                print(
+                    f"Turbine type '{self.name}': Setting P_nominal = {self.P_nominal:.2f} {self.P_unit}"
+                )
 
         return super().initialize(algo, verbosity)
 
     def calculate(self, algo, mdata, fdata, st_sel):
         """ "
         The main model calculation.
 
@@ -217,26 +215,24 @@
 
         """
         rews2 = fdata[self.WSCT][st_sel]
         rews3 = fdata[self.WSP][st_sel]
 
         # apply air density correction:
         if self.rho is not None:
-
             # correct wind speed by air density, such
             # that in the partial load region the
             # correct value is reconstructed:
             rho = fdata[FV.RHO][st_sel]
             rews2 *= (self.rho / rho) ** 0.5
             rews3 *= (self.rho / rho) ** (1.0 / 3.0)
             del rho
 
         # in yawed case, calc yaw corrected wind speed:
         if FV.YAWM in fdata and (self.p_P is not None or self.p_ct is not None):
-
             # calculate corrected wind speed wsc,
             # gives ws**3 * cos**p_P in partial load region
             # and smoothly deals with full load region:
             yawm = fdata[FV.YAWM][st_sel]
             if np.any(np.isnan(yawm)):
                 raise ValueError(
                     f"{self.name}: Found NaN values for variable '{FV.YAWM}'. Maybe change order in turbine_models?"
```

### Comparing `foxes-0.3.4/foxes/models/turbine_types/null_type.py` & `foxes-0.3.5/foxes/models/turbine_types/null_type.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.4/foxes/models/turbine_types/wsrho2PCt_two_files.py` & `foxes-0.3.5/foxes/models/turbine_types/wsrho2PCt_two_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,34 +151,30 @@
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         # read power curve:
         if isinstance(self.source_P, pd.DataFrame):
             data = self.source_P
         else:
-            fpath = algo.dbook.get_file_path(
-                PCTCURVE, self.source_P, check_raw=True
-            )
+            fpath = algo.dbook.get_file_path(PCTCURVE, self.source_P, check_raw=True)
             pars = {"index_col": 0}
             pars.update(self.rpars_P)
             data = PandasFileHelper.read_file(fpath, **pars)
 
         data.sort_index(inplace=True)
         data.columns = data.columns.astype(FC.DTYPE)
         self._ws_P = data.index.to_numpy(FC.DTYPE)
         self._rho_P = np.sort(data.columns.to_numpy())
         self._P = data[self._rho_P].to_numpy(FC.DTYPE)
 
         # read ct curve:
         if isinstance(self.source_ct, pd.DataFrame):
             data = self.source_ct
         else:
-            fpath = algo.dbook.get_file_path(
-                PCTCURVE, self.source_ct, check_raw=True
-            )
+            fpath = algo.dbook.get_file_path(PCTCURVE, self.source_ct, check_raw=True)
             pars = {"index_col": 0}
             pars.update(self.rpars_ct)
             data = PandasFileHelper.read_file(fpath, **pars)
 
         data.sort_index(inplace=True)
         data.columns = data.columns.astype(FC.DTYPE)
         self._ws_ct = data.index.to_numpy(FC.DTYPE)
@@ -237,24 +233,22 @@
             & (fdata[self.WSP] >= self._ws_P[0])
             & (fdata[self.WSP] <= self._ws_P[-1])
         )
         st_sel_P0 = st_sel & ~st_sel_P
         if np.any(st_sel_P0):
             fdata[FV.P][st_sel_P0] = 0
         if np.any(st_sel_P):
-
             # prepare interpolation:
             n_sel = np.sum(st_sel_P)
             qts = np.zeros((n_sel, 2), dtype=FC.DTYPE)  # ws, rho
             qts[:, 0] = fdata[self.WSP][st_sel_P]
             qts[:, 1] = fdata[FV.RHO][st_sel_P]
 
             # apply yaw corrections:
             if FV.YAWM in fdata and self.p_P is not None:
-
                 # calculate corrected wind speed wsc,
                 # gives ws**3 * cos**p_P in partial load region
                 # and smoothly deals with full load region:
                 yawm = fdata[FV.YAWM][st_sel_P]
                 if np.any(np.isnan(yawm)):
                     raise ValueError(
                         f"{self.name}: Found NaN values for variable '{FV.YAWM}'. Maybe change order in turbine_models?"
@@ -279,24 +273,22 @@
             & (fdata[self.WSCT] >= self._ws_P[0])
             & (fdata[self.WSCT] <= self._ws_P[-1])
         )
         st_sel_ct0 = st_sel & ~st_sel_ct
         if np.any(st_sel_ct0):
             fdata[FV.CT][st_sel_ct0] = 0
         if np.any(st_sel_ct):
-
             # prepare interpolation:
             n_sel = np.sum(st_sel_ct)
             qts = np.zeros((n_sel, 2), dtype=FC.DTYPE)  # ws, rho
             qts[:, 0] = fdata[self.WSP][st_sel_ct]
             qts[:, 1] = fdata[FV.RHO][st_sel_ct]
 
             # apply yaw corrections:
             if FV.YAWM in fdata and self.p_ct is not None:
-
                 # calculate corrected wind speed wsc,
                 # gives ws**3 * cos**p_P in partial load region
                 # and smoothly deals with full load region:
                 yawm = fdata[FV.YAWM][st_sel_ct]
                 if np.any(np.isnan(yawm)):
                     raise ValueError(
                         f"{self.name}: Found NaN values for variable '{FV.YAWM}'. Maybe change order in turbine_models?"
```

### Comparing `foxes-0.3.4/foxes/models/vertical_profiles/abl_log/abl_log_neutral_ws.py` & `foxes-0.3.5/foxes/models/vertical_profiles/abl_log/abl_log_neutral_ws.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.4/foxes/models/vertical_profiles/abl_log/abl_log_stable_ws.py` & `foxes-0.3.5/foxes/models/vertical_profiles/abl_log/abl_log_stable_ws.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.4/foxes/models/vertical_profiles/abl_log/abl_log_unstable_ws.py` & `foxes-0.3.5/foxes/models/vertical_profiles/abl_log/abl_log_unstable_ws.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.4/foxes/models/vertical_profiles/abl_log/abl_log_ws.py` & `foxes-0.3.5/foxes/models/vertical_profiles/abl_log/abl_log_ws.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.4/foxes/models/vertical_profiles/abl_log/sheared_ws.py` & `foxes-0.3.5/foxes/models/vertical_profiles/abl_log/sheared_ws.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,30 +2,27 @@
 
 from foxes.core import VerticalProfile
 from foxes.utils import abl
 import foxes.constants as FC
 import foxes.variables as FV
 
 
-
 class ShearedProfile(VerticalProfile):
-
     def input_vars(self):
         """
         The input variables needed for the profile
         calculation.
 
         Returns
         -------
         vars : list of str
             The variable names
         """
         return [FV.WS, FV.H, FV.SHEAR]
 
-
     def calculate(self, data, heights):
         """
         Run the profile calculation.
 
         Parameters
         ----------
         data : dict
```

### Comparing `foxes-0.3.4/foxes/models/wake_frames/farm_order.py` & `foxes-0.3.5/foxes/models/wake_frames/farm_order.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import numpy as np
 
 import foxes.constants as FC
 from .rotor_wd import RotorWD
 from foxes.core import WakeFrame
 
+
 class FarmOrder(WakeFrame):
     """
     Invokes turbine ordering as defined
     by the wind farm.
 
     Warning: This is for testing purposes only, and in general
     only gives correct calculation results when used
@@ -106,15 +107,17 @@
 
         Returns
         -------
         wake_coos : numpy.ndarray
             The wake coordinates, shape: (n_states, n_points, 3)
 
         """
-        return self.base_frame.get_wake_coos(algo, mdata, fdata, states_source_turbine, points)
+        return self.base_frame.get_wake_coos(
+            algo, mdata, fdata, states_source_turbine, points
+        )
 
     def get_centreline_points(self, algo, mdata, fdata, states_source_turbine, x):
         """
         Gets the points along the centreline for given
         values of x.
 
         Parameters
@@ -126,23 +129,25 @@
         fdata : foxes.core.Data
             The farm data
         states_source_turbine : numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
         x : numpy.ndarray
             The wake frame x coordinates, shape: (n_states, n_points)
-        
+
         Returns
         -------
         points : numpy.ndarray
             The centreline points, shape: (n_states, n_points, 3)
 
         """
-        return self.base_frame.get_centreline_points(algo, mdata, fdata, states_source_turbine, x)
-        
+        return self.base_frame.get_centreline_points(
+            algo, mdata, fdata, states_source_turbine, x
+        )
+
     def finalize(self, algo, verbosity=0):
         """
         Finalizes the model.
 
         Parameters
         ----------
         algo : foxes.core.Algorithm
```

### Comparing `foxes-0.3.4/foxes/models/wake_frames/rotor_wd.py` & `foxes-0.3.5/foxes/models/wake_frames/rotor_wd.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
         fdata : foxes.core.Data
             The farm data
         states_source_turbine : numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
         x : numpy.ndarray
             The wake frame x coordinates, shape: (n_states, n_points)
-        
+
         Returns
         -------
         points : numpy.ndarray
             The centreline points, shape: (n_states, n_points, 3)
 
         """
         n_states = mdata.n_states
```

### Comparing `foxes-0.3.4/foxes/models/wake_frames/streamlines.py` & `foxes-0.3.5/foxes/models/wake_frames/streamlines.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,14 @@
         """
         self.DATA = self.var("DATA")
         self.CNTR = self.var("CNTR")
         self.PRES = self.var("PRES")
         return super().initialize(algo, verbosity)
 
     def _init_data(self, mdata, fdata):
-
         # prepare:
         n_states = mdata.n_states
         n_turbines = mdata.n_turbines
 
         # x, y, z, u, v, w, len
         mdata[self.DATA] = np.full(
             (n_states, n_turbines, self.n_delstor, 7), np.nan, dtype=FC.DTYPE
@@ -114,15 +113,15 @@
                     (n_states, n_turbines, self.n_delstor, 7),
                     np.nan,
                     dtype=FC.DTYPE,
                 ),
                 axis=2,
             )
             mdata[self.DATA] = data
-        
+
         # data aliases:
         spts = data[..., :3]
         sn = data[..., 3:6]
         slen = data[..., 6]
 
         # calculate next point:
         p0 = spts[:, :, n_spts - 1]
@@ -130,24 +129,21 @@
         spts[:, :, n_spts] = p0 + self.step * n0
         slen[:, :, n_spts] = slen[:, :, n_spts - 1] + self.step
         newpts = spts[:, :, n_spts]
         del p0, n0
 
         # calculate next tangential vector:
         svars = algo.states.output_point_vars(algo)
-        pdata = {FV.POINTS: newpts}
-        pdims = {FV.POINTS: (FV.STATE, FV.POINT, FV.XYH)}
+        pdata = {FC.POINTS: newpts}
+        pdims = {FC.POINTS: (FC.STATE, FC.POINT, FV.XYH)}
         pdata.update(
-            {
-                v: np.full((n_states, n_turbines), np.nan, dtype=FC.DTYPE)
-                for v in svars
-            }
+            {v: np.full((n_states, n_turbines), np.nan, dtype=FC.DTYPE) for v in svars}
         )
-        pdims.update({v: (FV.STATE, FV.POINT) for v in svars})
-        pdata = Data(pdata, pdims, loop_dims=[FV.STATE, FV.POINT])
+        pdims.update({v: (FC.STATE, FC.POINT) for v in svars})
+        pdata = Data(pdata, pdims, loop_dims=[FC.STATE, FC.POINT])
         data[:, :, n_spts, 5] = 0.0
         data[:, :, n_spts, 3:5] = wd2uv(
             algo.states.calculate(algo, mdata, fdata, pdata)[FV.WD]
         )
         mdata[self.CNTR] += 1
 
         return newpts, data, mdata[self.CNTR]
@@ -176,17 +172,16 @@
             for ti in range(n_turbines):
                 dists[:, ti, ti] = 1e20
         inds = np.argmin(dists, axis=3)
         dists = np.take_along_axis(dists, inds[:, :, :, None], axis=3)[..., 0]
         done = inds < n_spts - 1
 
         # calc streamline points, as many as needed:
-        maxl = np.nanmax(data[:, :, n_spts-1, 6])
+        maxl = np.nanmax(data[:, :, n_spts - 1, 6])
         while maxl + self.step <= self.max_length and not np.all(done):
-
             # print("CALC STREAMLINES, TODO", np.sum(~done))
 
             # add next streamline point:
             newpts, data, n_spts = self._add_next_point(algo, mdata, fdata)
 
             # evaluate distance:
             d = np.linalg.norm(points[:, None] - newpts[:, :, None], axis=-1)
@@ -196,15 +191,15 @@
             sel = d < dists
             if np.any(sel):
                 dists[sel] = d[sel]
                 inds[sel] = n_spts - 1
 
             # rotation:
             done = inds < n_spts - 1
-            maxl = np.nanmax(data[:, :, n_spts-1, 6])
+            maxl = np.nanmax(data[:, :, n_spts - 1, 6])
             del newpts
 
         # shrink to size:
         mdata[self.DATA] = data[:, :, :n_spts]
         del data, spts, sn
 
         # select streamline points:
@@ -229,20 +224,20 @@
         return coos
 
     def _ensure_min_length(self, algo, mdata, fdata, length):
         """
         Helper function, ensures minimal length of streamlines
         """
         data = mdata[self.DATA]
-        slen = data[:, :, mdata[self.CNTR]-1, 6]
+        slen = data[:, :, mdata[self.CNTR] - 1, 6]
         minl = np.nanmin(slen)
         maxl = np.nanmax(slen)
         while maxl + self.step <= self.max_length and minl < length:
             __, data, n_spts = self._add_next_point(algo, mdata, fdata)
-            slen = data[:, :, n_spts-1, 6]
+            slen = data[:, :, n_spts - 1, 6]
             minl = np.nanmin(slen)
             maxl = np.nanmax(slen)
 
     def calc_order(self, algo, mdata, fdata):
         """ "
         Calculates the order of turbine evaluation.
 
@@ -341,15 +336,15 @@
         fdata : foxes.core.Data
             The farm data
         states_source_turbine : numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
         x : numpy.ndarray
             The wake frame x coordinates, shape: (n_states, n_points)
-        
+
         Returns
         -------
         points : numpy.ndarray
             The centreline points, shape: (n_states, n_points, 3)
 
         """
         # calculate long enough streamlines:
@@ -363,13 +358,13 @@
         n_spts = spts.shape[1]
         xs = self.step * np.arange(n_spts)
 
         # interpolate to x of interest:
         qts = np.zeros((n_states, n_points, 2), dtype=FC.DTYPE)
         qts[:, :, 0] = np.arange(n_states)[:, None]
         qts[:, :, 1] = x
-        qts = qts.reshape(n_states*n_points, 2)
-        ipars = dict(bounds_error=False, fill_value=0.)
+        qts = qts.reshape(n_states * n_points, 2)
+        ipars = dict(bounds_error=False, fill_value=0.0)
         ipars.update(self.cl_ipars)
         results = interpn((np.arange(n_states), xs), spts, qts, **ipars)
 
         return results.reshape(n_states, n_points, 3)
```

### Comparing `foxes-0.3.4/foxes/models/wake_frames/yawed_wakes.py` & `foxes-0.3.5/foxes/models/wake_frames/yawed_wakes.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,44 +23,50 @@
         to this number, by default 0.9999
     alpha : float, optional
         model parameter used to determine onset of far wake region
     beta : float, optional
         model parameter used to determine onset of far wake region
     base_frame : foxes.core.WakeFrame
         The wake frame from which to start
+    k_var : str
+        The variable name for k
 
     Attributes
     ----------
     model : PorteAgelModel
         The model for computing common data
     K : float
         The wake growth parameter k. If not given here
         it will be searched in the farm data.
     YAWM : float
         The yaw misalignment YAWM. If not given here
         it will be searched in the farm data.
     base_frame : foxes.core.WakeFrame
         The wake frame from which to start
+    k_var : str
+        The variable name for k
 
     """
 
     def __init__(
         self,
         k=None,
         ct_max=0.9999,
         alpha=0.58,
         beta=0.07,
         base_frame=RotorWD(),
+        k_var=FV.K,
     ):
         super().__init__()
 
         self.base_frame = base_frame
         self.model = PorteAgelModel(ct_max, alpha, beta)
+        self.k_var = k_var
 
-        setattr(self, FV.K, k)
+        setattr(self, k_var, k)
         setattr(self, FV.YAWM, 0.0)
 
     def initialize(self, algo, verbosity=0):
         """
         Initializes the model.
 
         This includes loading all required data from files. The model
@@ -120,48 +126,47 @@
         # prepare:
         n_states = mdata.n_states
         n_points = x.shape[1]
         st_sel = (np.arange(n_states), states_source_turbine)
 
         # get gamma:
         gamma = np.zeros((n_states, n_points), dtype=FC.DTYPE)
-        gamma[:] = self.get_data(FV.YAWM, fdata, upcast="farm", data_prio=True)[st_sel][:, None]
+        gamma[:] = self.get_data(FV.YAWM, fdata, upcast="farm", data_prio=True)[st_sel][
+            :, None
+        ]
         gamma *= np.pi / 180
 
         # get k:
         k = np.zeros((n_states, n_points), dtype=FC.DTYPE)
-        k[:] = self.get_data(FV.K, fdata, upcast="farm")[st_sel][:, None]
+        k[:] = self.get_data(self.k_var, fdata, upcast="farm")[st_sel][:, None]
 
         # run model calculation:
         self.model.calc_data(mdata, fdata, states_source_turbine, x, gamma, k)
 
         # select targets:
         sp_sel = self.model.get_data(PorteAgelModel.SP_SEL, mdata)
         if np.any(sp_sel):
-
             # prepare:
             n_sp_sel = np.sum(sp_sel)
             ydef = np.zeros((n_sp_sel,), dtype=FC.DTYPE)
 
             # collect data:
             near = self.model.get_data(PorteAgelModel.NEAR, mdata)
             far = ~near
 
             # near wake:
             if np.any(near):
-
                 # collect data:
                 delta = self.model.get_data(PorteAgelModel.DELTA_NEAR, mdata)
 
                 # set deflection:
                 ydef[near] = delta
 
             # far wake:
             if np.any(far):
-
                 # collect data:
                 delta = self.model.get_data(PorteAgelModel.DELTA_FAR, mdata)
 
                 # set deflection:
                 ydef[far] = delta
 
             # apply deflection:
@@ -217,40 +222,43 @@
         fdata : foxes.core.Data
             The farm data
         states_source_turbine : numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
         x : numpy.ndarray
             The wake frame x coordinates, shape: (n_states, n_points)
-        
+
         Returns
         -------
         points : numpy.ndarray
             The centreline points, shape: (n_states, n_points, 3)
 
         """
-        points = self.base_frame.get_centreline_points(algo, mdata, fdata, 
-                    states_source_turbine, x)
+        points = self.base_frame.get_centreline_points(
+            algo, mdata, fdata, states_source_turbine, x
+        )
 
         nx = np.zeros_like(points)
         nx[:, 0] = points[:, 1] - points[:, 0]
         nx[:, -1] = points[:, -1] - points[:, -2]
-        nx[:, 1:-1] = 0.5*(points[:, 1:-1] - points[:, :-2]) + 0.5*(points[:, 2:] - points[:, 1:-1])
+        nx[:, 1:-1] = 0.5 * (points[:, 1:-1] - points[:, :-2]) + 0.5 * (
+            points[:, 2:] - points[:, 1:-1]
+        )
         nx /= np.linalg.norm(nx, axis=-1)[:, :, None]
 
         nz = np.zeros_like(nx)
         nz[:, :, 2] = 1
         ny = np.cross(nz, nx, axis=-1)
         del nx, nz
 
         y = np.zeros_like(x)
         self._update_y(mdata, fdata, states_source_turbine, x, y)
 
         points += y[:, :, None] * ny
-        
+
         return points
 
     def finalize(self, algo, verbosity=0):
         """
         Finalizes the model.
 
         Parameters
```

### Comparing `foxes-0.3.4/foxes/models/wake_models/axisymmetric.py` & `foxes-0.3.5/foxes/models/wake_models/axisymmetric.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.4/foxes/models/wake_models/dist_sliced.py` & `foxes-0.3.5/foxes/models/wake_models/dist_sliced.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,17 +61,16 @@
 
         """
         self.superp = {
             v: algo.mbook.wake_superpositions[s] for v, s in self.superpositions.items()
         }
 
         idata = super().initialize(algo, verbosity)
-        algo.update_idata(list(self.superp.values()),
-            idata=idata, verbosity=verbosity)
-        
+        algo.update_idata(list(self.superp.values()), idata=idata, verbosity=verbosity)
+
         return idata
 
     @abstractmethod
     def calc_wakes_spsel_x_yz(self, algo, mdata, fdata, states_source_turbine, x, yz):
         """
         Calculate wake deltas.
 
@@ -138,15 +137,14 @@
         yz = wake_coos[:, :, None, 1:3]
 
         wdeltas, sp_sel = self.calc_wakes_spsel_x_yz(
             algo, mdata, fdata, states_source_turbine, x, yz
         )
 
         for v, hdel in wdeltas.items():
-
             try:
                 superp = self.superp[v]
             except KeyError:
                 raise KeyError(
                     f"Model '{self.name}': Missing wake superposition entry for variable '{v}', found {sorted(list(self.superp.keys()))}"
                 )
 
@@ -202,8 +200,7 @@
         verbosity : int
             The verbosity level, 0 = silent
 
         """
         for s in self.superp.values():
             s.finalize(algo, verbosity)
         super().finalize(algo, verbosity)
-
```

### Comparing `foxes-0.3.4/foxes/models/wake_models/gaussian.py` & `foxes-0.3.5/foxes/models/wake_models/gaussian.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.4/foxes/models/wake_models/ti/crespo_hernandez.py` & `foxes-0.3.5/foxes/models/wake_models/ti/crespo_hernandez.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,16 @@
         Model parameter
     e1 : float
         Model parameter
     e2 : float
         Model parameter
     e3 : float
         Model parameter
+    k_var : str
+        The variable name for k
 
     Attributes
     ----------
     k : float
         The wake growth parameter k. If not given here
         it will be searched in the farm data.
     a_near : float
@@ -63,14 +65,16 @@
         Flag for using ambient TI instead of local
         wake corrected TI
     sbeta_factor : float
         Factor multiplying sbeta
     near_wake_D : float
         The near wake distance in units of D,
         calculated from TI and ct if None
+    k_var : str
+        The variable name for k
 
     """
 
     def __init__(
         self,
         superposition,
         k=None,
@@ -79,31 +83,34 @@
         near_wake_D=None,
         ct_max=0.9999,
         a_near=0.362,
         a_far=0.73,
         e1=0.83,
         e2=-0.0325,
         e3=-0.32,
+        k_var=FV.K
     ):
         super().__init__(superpositions={FV.TI: superposition}, ct_max=ct_max)
 
         self.a_near = a_near
         self.a_far = a_far
         self.e1 = e1
         self.e2 = e2
         self.e3 = e3
         self.use_ambti = use_ambti
         self.sbeta_factor = sbeta_factor
         self.near_wake_D = near_wake_D
+        self.k_var = k_var
 
-        setattr(self, FV.K, k)
+        setattr(self, k_var, k)
 
     def __repr__(self):
+        k = getattr(self, self.k_var)
         s = super().__repr__()
-        s += f"(k={getattr(self, FV.K)}, sp={self.superpositions[FV.TI]})"
+        s += f"({self.k_var}={k}, sp={self.superpositions[FV.TI]})"
         return s
 
     def init_wake_deltas(self, algo, mdata, fdata, n_points, wake_deltas):
         """
         Initialize wake delta storage.
 
         They are added on the fly to the wake_deltas dict.
@@ -162,17 +169,15 @@
         n_states = fdata.n_states
         st_sel = (np.arange(n_states), states_source_turbine)
 
         # get D:
         D = fdata[FV.D][st_sel][:, None]
 
         # get k:
-        k = self.get_data(FV.K, fdata, st_sel)
-        if isinstance(k, np.ndarray):
-            k = k[:, None]
+        k = self.get_data(self.k_var, fdata, upcast="farm")[st_sel][:, None]
 
         # calculate:
         sbeta = np.sqrt(0.5 * (1 + np.sqrt(1 - ct)) / np.sqrt(1 - ct))
         sblim = 1 / (np.sqrt(8) * self.sbeta_factor)
         sbeta[sbeta > sblim] = sblim
         radius = 2 * (k * x + self.sbeta_factor * sbeta * D)
 
@@ -247,15 +252,14 @@
         # calc near wake:
         sel = x < near_wake_D * D
         if np.any(sel):
             wake_deltas[sel] = self.a_near * (1.0 - np.sqrt(1.0 - ct[sel]))
 
         # calc far wake:
         if np.any(~sel):
-
             # calculate delta:
             #
             # Note the sign flip of the exponent ti[~sel]**(-0.0325)
             # compared to the original paper. This was found in
             # https://doi.org/10.1016/j.jweia.2018.04.010, Eq. (46)
             # Without this flip the near and far wake areas are not
             # smoothly connected.
```

### Comparing `foxes-0.3.4/foxes/models/wake_models/ti/iec_ti.py` & `foxes-0.3.5/foxes/models/wake_models/ti/iec_ti.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,41 +26,47 @@
         will be looked up in model book
     opening_angle : float
         The wake opening angle. The wake growth parameter k is calculated
         based on the wake opening angle.
     ct_max : float
         The maximal value for ct, values beyond will be limited
         to this number
-
+    k_var : str
+        The variable name for k
 
     Attributes
     ----------
     opening_angle : float
         The wake opening angle. The wake growth parameter k is calculated
         based on the wake opening angle.
+    k_var : str
+        The variable name for k
 
     """
 
     def __init__(
         self,
         superposition,
         opening_angle=21.6,
         ct_max=0.9999,
         iec_type="2019",
+        k_var=FV.K
     ):
         super().__init__(superpositions={FV.TI: superposition}, ct_max=ct_max)
 
         k = float(np.tan(np.deg2rad(opening_angle / 2.0)))
 
         self.iec_type = iec_type
-        setattr(self, FV.K, k)
+        self.k_var = k_var
+        setattr(self, k_var, k)
 
     def __repr__(self):
+        k = getattr(self, self.k_var)
         s = super().__repr__()
-        s += f"(k={getattr(self, FV.K)}, sp={self.superpositions[FV.TI]})"
+        s += f"({self.k_var}={k}, sp={self.superpositions[FV.TI]})"
         return s
 
     def init_wake_deltas(self, algo, mdata, fdata, n_points, wake_deltas):
         """
         Initialize wake delta storage.
 
         They are added on the fly to the wake_deltas dict.
@@ -116,15 +122,15 @@
 
         """
         # prepare:
         n_states = fdata.n_states
         st_sel = (np.arange(n_states), states_source_turbine)
 
         # get k:
-        k = self.get_data(FV.K, fdata, st_sel, data_prio=False)
+        k = self.get_data(self.k_var, fdata, st_sel, data_prio=False)
         if isinstance(k, np.ndarray):
             k = k[:, None]
 
         # calculate:
         radius = k * x
 
         return radius
```

### Comparing `foxes-0.3.4/foxes/models/wake_models/top_hat.py` & `foxes-0.3.5/foxes/models/wake_models/top_hat.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,14 @@
         ct[ct > self.ct_max] = self.ct_max
 
         wake_r = self.calc_wake_radius(algo, mdata, fdata, states_source_turbine, x, ct)
 
         wdeltas = {}
         sp_sel = (ct > 0.0) & (x > 1e-5) & np.any(r < wake_r[:, :, None], axis=2)
         if np.any(sp_sel):
-
             x = x[sp_sel]
             r = r[sp_sel]
             ct = ct[sp_sel]
             wake_r = wake_r[sp_sel]
 
             cl_del = self.calc_centreline_wake_deltas(
                 algo, mdata, fdata, states_source_turbine, sp_sel, x, wake_r, ct
```

### Comparing `foxes-0.3.4/foxes/models/wake_models/wind/bastankhah.py` & `foxes-0.3.5/foxes/models/wake_models/wind/bastankhah.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,39 +24,45 @@
         The wake growth parameter k. If not given here
         it will be searched in the farm data.
     sbeta_factor : float
         Factor multiplying sbeta
     ct_max : float
         The maximal value for ct, values beyond will be limited
         to this number
+    k_var : str
+        The variable name for k
 
     Attributes
     ----------
     k : float, optional
         The wake growth parameter k. If not given here
         it will be searched in the farm data.
     sbeta_factor : float
         Factor multiplying sbeta
     ct_max : float
         The maximal value for ct, values beyond will be limited
         to this number
+    k_var : str
+        The variable name for k
 
     """
 
-    def __init__(self, superposition, k=None, sbeta_factor=0.25, ct_max=0.9999):
+    def __init__(self, superposition, k=None, sbeta_factor=0.25, ct_max=0.9999, k_var=FV.K):
         super().__init__(superpositions={FV.WS: superposition})
 
         self.ct_max = ct_max
         self.sbeta_factor = sbeta_factor
+        self.k_var = k_var
 
-        setattr(self, FV.K, k)
+        setattr(self, k_var, k)
 
     def __repr__(self):
+        k = getattr(self, self.k_var)
         s = super().__repr__()
-        s += f"(k={self.k}, sp={self.superpositions[FV.WS]})"
+        s += f"({self.k_var}={k}, sp={self.superpositions[FV.WS]})"
         return s
 
     def init_wake_deltas(self, algo, mdata, fdata, n_points, wake_deltas):
         """
         Initialize wake delta storage.
 
         They are added on the fly to the wake_deltas dict.
@@ -119,27 +125,26 @@
         ct = np.zeros((n_states, n_points), dtype=FC.DTYPE)
         ct[:] = self.get_data(FV.CT, fdata)[st_sel][:, None]
         ct[ct > self.ct_max] = self.ct_max
 
         # select targets:
         sp_sel = (x > 1e-5) & (ct > 0.0)
         if np.any(sp_sel):
-
             # apply selection:
             x = x[sp_sel]
             ct = ct[sp_sel]
 
             # get D:
             D = np.zeros((n_states, n_points), dtype=FC.DTYPE)
             D[:] = self.get_data(FV.D, fdata)[st_sel][:, None]
             D = D[sp_sel]
 
             # get k:
             k = np.zeros((n_states, n_points), dtype=FC.DTYPE)
-            k[:] = self.get_data(FV.K, fdata, upcast="farm")[st_sel][:, None]
+            k[:] = self.get_data(self.k_var, fdata, upcast="farm")[st_sel][:, None]
             k = k[sp_sel]
 
             # calculate sigma:
             sbeta = np.sqrt(0.5 * (1 + np.sqrt(1.0 - ct)) / np.sqrt(1.0 - ct))
             sblim = 1 / (np.sqrt(8) * self.sbeta_factor)
             sbeta[sbeta > sblim] = sblim
             sigma = k * x + self.sbeta_factor * sbeta * D
```

### Comparing `foxes-0.3.4/foxes/models/wake_models/wind/jensen.py` & `foxes-0.3.5/foxes/models/wake_models/wind/jensen.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,31 +17,37 @@
         will be looked up in model book
     k : float, optional
         The wake growth parameter k. If not given here
         it will be searched in the farm data.
     ct_max : float
         The maximal value for ct, values beyond will be limited
         to this number
+    k_var : str
+        The variable name for k
 
     Attributes
     ----------
     k : float, optional
         The wake growth parameter k. If not given here
         it will be searched in the farm data.
+    k_var : str
+        The variable name for k
 
     """
 
-    def __init__(self, superposition, k=None, ct_max=0.9999):
+    def __init__(self, superposition, k=None, ct_max=0.9999, k_var=FV.K):
         super().__init__(superpositions={FV.WS: superposition}, ct_max=ct_max)
 
-        setattr(self, FV.K, k)
+        self.k_var = k_var
+        setattr(self, k_var, k)
 
     def __repr__(self):
+        k = getattr(self, self.k_var)
         s = super().__repr__()
-        s += f"(k={self.k}, sp={self.superpositions[FV.WS]})"
+        s += f"({self.k_var}={k}, sp={self.superpositions[FV.WS]})"
         return s
 
     def init_wake_deltas(self, algo, mdata, fdata, n_points, wake_deltas):
         """
         Initialize wake delta storage.
 
         They are added on the fly to the wake_deltas dict.
@@ -96,15 +102,15 @@
             The wake radii, shape: (n_states, n_points)
 
         """
         n_states = mdata.n_states
         st_sel = (np.arange(n_states), states_source_turbine)
 
         R = fdata[FV.D][st_sel][:, None] / 2
-        k = self.get_data(FV.K, fdata, st_sel)
+        k = self.get_data(self.k_var, fdata, st_sel)
 
         if isinstance(k, np.ndarray):
             k = k[:, None]
 
         return R + k * x
 
     def calc_centreline_wake_deltas(
```

### Comparing `foxes-0.3.4/foxes/models/wake_models/wind/porte_agel.py` & `foxes-0.3.5/foxes/models/wake_models/wind/porte_agel.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         n_states = mdata.n_states
         n_points = x.shape[1]
         st_sel = (np.arange(n_states), states_source_turbine)
 
         # store parameters:
         out = {self.PARS: self.pars}
         out[self.CHECK] = (
-            mdata[FV.STATE][0],
+            mdata[FC.STATE][0],
             states_source_turbine[0],
             x.shape,
         )
 
         # get D:
         D = np.zeros((n_states, n_points), dtype=FC.DTYPE)
         D[:] = fdata[FV.D][st_sel][:, None]
@@ -119,15 +119,14 @@
         ct = np.zeros((n_states, n_points), dtype=FC.DTYPE)
         ct[:] = fdata[FV.CT][st_sel][:, None]
         ct[ct > self.ct_max] = self.ct_max
 
         # select targets:
         sp_sel = (x > 1e-5) & (ct > 0.0)
         if np.any(sp_sel):
-
             # get ws:
             ws = np.zeros((n_states, n_points), dtype=FC.DTYPE)
             ws[:] = fdata[FV.REWS][st_sel][:, None]
 
             # get TI:
             ti = np.zeros((n_states, n_points), dtype=FC.DTYPE)
             ti[:] = fdata[FV.TI][st_sel][:, None]
@@ -162,15 +161,14 @@
             sigma_y = k * (x - x0) + sigma_y0
             sigma_z = k * (x - x0) + simga_z0
 
             # calc near wake data:
             near = x < x0
             out[self.NEAR] = near
             if np.any(near):
-
                 # apply filter:
                 wsn = ws[near]
                 ctn = ct[near]
                 cosgn = cosg[near]
 
                 # initial velocity deficits, Eq. (6.4):
                 uR = 0.5 * ctn * cosgn / (1 - np.sqrt(1 - ctn * cosgn))
@@ -191,15 +189,14 @@
 
                 # cleanup:
                 del wsn, ctn, cosgn, uR, u0, d, r_pc_0, r_pc
 
             # calc far wake data:
             far = ~near
             if np.any(far):
-
                 # apply filter:
                 ws = ws[far]
                 ct = ct[far]
                 sigma_y = sigma_y[far]
                 sigma_z = sigma_z[far]
                 cosg = cosg[far]
                 D = D[far]
@@ -253,15 +250,15 @@
         Returns
         -------
         check : bool
             True if data exists
 
         """
         check = (
-            mdata[FV.STATE][0],
+            mdata[FC.STATE][0],
             states_source_turbine[0],
             x.shape,
         )
         return self.MDATA_KEY in mdata and mdata[self.MDATA_KEY][self.CHECK] == check
 
     def get_data(self, key, mdata):
         """
@@ -308,39 +305,45 @@
     ct_max : float
         The maximal value for ct, values beyond will be limited
         to this number, by default 0.9999
     alpha : float
         model parameter used to determine onset of far wake region
     beta : float
         model parameter used to determine onset of far wake region
+    k_var : str
+        The variable name for k
 
     Attributes
     ----------
     model : PorteAgelModel
         The model for computing common data
     K : float
         The wake growth parameter k. If not given here
         it will be searched in the farm data.
     YAWM : float
         The yaw misalignment YAWM. If not given here
         it will be searched in the farm data.
+    k_var : str
+        The variable name for k
 
     """
 
-    def __init__(self, superposition, k=None, ct_max=0.9999, alpha=0.58, beta=0.07):
+    def __init__(self, superposition, k=None, ct_max=0.9999, alpha=0.58, beta=0.07, k_var=FV.K):
         super().__init__(superpositions={FV.WS: superposition})
 
         self.model = PorteAgelModel(ct_max, alpha, beta)
+        self.k_var = k_var
 
-        setattr(self, FV.K, k)
+        setattr(self, k_var, k)
         setattr(self, FV.YAWM, 0.0)
 
     def __repr__(self):
+        k = getattr(self, self.k_var)
         s = super().__repr__()
-        s += f"(k={self.k}, sp={self.superpositions[FV.WS]})"
+        s += f"({self.k_var}={k}, sp={self.superpositions[FV.WS]})"
         return s
 
     def init_wake_deltas(self, algo, mdata, fdata, n_points, wake_deltas):
         """
         Initialize wake delta storage.
 
         They are added on the fly to the wake_deltas dict.
@@ -400,43 +403,42 @@
         n_states = mdata.n_states
         n_points = x.shape[1]
         n_y_per_z = yz.shape[2]
         st_sel = (np.arange(n_states), states_source_turbine)
 
         # calculate model data:
         if not self.model.has_data(mdata, states_source_turbine, x):
-
             # get gamma:
             gamma = np.zeros((n_states, n_points), dtype=FC.DTYPE)
-            gamma[:] = self.get_data(FV.YAWM, fdata, upcast="farm", data_prio=True)[st_sel][:, None]
+            gamma[:] = self.get_data(FV.YAWM, fdata, upcast="farm", data_prio=True)[
+                st_sel
+            ][:, None]
             gamma *= np.pi / 180
 
             # get k:
             k = np.zeros((n_states, n_points), dtype=FC.DTYPE)
-            k[:] = self.get_data(FV.K, fdata, upcast="farm")[st_sel][:, None]
+            k[:] = self.get_data(self.k_var, fdata, upcast="farm")[st_sel][:, None]
 
             # run calculation:
             self.model.calc_data(mdata, fdata, states_source_turbine, x, gamma, k)
 
         # select targets:
         sp_sel = self.model.get_data(PorteAgelModel.SP_SEL, mdata)
         n_sp_sel = np.sum(sp_sel)
         wdeltas = {FV.WS: np.zeros((n_sp_sel, n_y_per_z), dtype=FC.DTYPE)}
         if np.any(sp_sel):
-
             # apply filter:
             yz = yz[sp_sel]
 
             # collect data:
             near = self.model.get_data(PorteAgelModel.NEAR, mdata)
             far = ~near
 
             # near wake:
             if np.any(near):
-
                 # collect data:
                 ampl = self.model.get_data(PorteAgelModel.AMPL_NEAR, mdata)
                 r_pc = self.model.get_data(PorteAgelModel.R_PC, mdata)
                 s = self.model.get_data(PorteAgelModel.R_PC_S, mdata)
 
                 # radial dependency:
                 r = np.linalg.norm(yz[near], axis=-1)
@@ -448,15 +450,14 @@
                 rfactor[sel_oc] = np.exp(-0.5 * ((r - r_pc) / s) ** 2)
 
                 # set deficit, Eq. (6.13):
                 wdeltas[FV.WS][near] = ampl[:, None] * rfactor
 
             # far wake:
             if np.any(far):
-
                 # apply filter:
                 yz = yz[far]
 
                 # collect data:
                 ampl = self.model.get_data(PorteAgelModel.AMPL_FAR, mdata)[:, None]
                 sigma_y = self.model.get_data(PorteAgelModel.SIGMA_Y_FAR, mdata)[
                     :, None
```

### Comparing `foxes-0.3.4/foxes/models/wake_models/wind/turbopark.py` & `foxes-0.3.5/foxes/models/wake_models/wind/turbopark.py`

 * *Files 5% similar despite different names*

```diff
@@ -125,15 +125,14 @@
         ct = np.zeros((n_states, n_points), dtype=FC.DTYPE)
         ct[:] = fdata[FV.CT][st_sel][:, None]
         ct[ct > self.ct_max] = self.ct_max
 
         # select targets:
         sp_sel = (x > 1e-5) & (ct > 0.0)
         if np.any(sp_sel):
-
             # apply selection:
             x = x[sp_sel]
             ct = ct[sp_sel]
 
             # get D:
             D = np.zeros((n_states, n_points), dtype=FC.DTYPE)
             D[:] = fdata[FV.D][st_sel][:, None]
@@ -142,39 +141,42 @@
             # get TI:
             ati = np.zeros((n_states, n_points), dtype=FC.DTYPE)
             ati[:] = fdata[FV.AMB_TI][st_sel][:, None]
             ati = ati[sp_sel]
 
             # calculate sigma:
             sbeta = np.sqrt(0.5 * (1 + np.sqrt(1.0 - ct)) / np.sqrt(1.0 - ct))
-            #sblim = 1 / (np.sqrt(8) * self.sbeta_factor)
-            #sbeta[sbeta > sblim] = sblim
+            # sblim = 1 / (np.sqrt(8) * self.sbeta_factor)
+            # sbeta[sbeta > sblim] = sblim
             epsilon = self.sbeta_factor * sbeta
 
             alpha = self.c1 * ati
             beta = self.c2 * ati / np.sqrt(ct)
 
             # calculate sigma (eqn 4)
             sigma = D * (
                 epsilon
-                + self.A*ati/beta
+                + self.A
+                * ati
+                / beta
                 * (
-                    np.sqrt((alpha + beta*x/D)**2 + 1)
+                    np.sqrt((alpha + beta * x / D) ** 2 + 1)
                     - np.sqrt(1 + alpha**2)
                     - np.log(
-                        (np.sqrt((alpha + beta*x/D)**2 + 1) + 1)*alpha
+                        (np.sqrt((alpha + beta * x / D) ** 2 + 1) + 1)
+                        * alpha
                         / ((np.sqrt(1 + alpha**2) + 1) * (alpha + beta * x / D))
                     )
                 )
             )
 
             del (
                 x,
                 sbeta,
-                #sblim,
+                # sblim,
                 alpha,
                 beta,
                 epsilon,
             )
 
             # calculate amplitude, same as in Bastankha model (eqn 7)
             if self.sbeta_factor < 0.25:
@@ -190,14 +192,15 @@
             sp_sel = np.zeros_like(x, dtype=bool)
             n_sp = np.sum(sp_sel)
             ampld = np.zeros(n_sp, dtype=FC.DTYPE)
             sigma = np.zeros(n_sp, dtype=FC.DTYPE)
 
         return {FV.WS: (ampld, sigma)}, sp_sel
 
+
 class TurbOParkWakeIX(GaussianWakeModel):
     """
     The generalized TurbOPark wake model, integrating TI over the streamline.
 
     https://iopscience.iop.org/article/10.1088/1742-6596/2265/2/022063/pdf
 
     Parameters
@@ -236,20 +239,20 @@
         The TI variable
     ipars : dict
         Additional parameters for centreline integration
 
     """
 
     def __init__(
-        self, 
-        superposition, 
+        self,
+        superposition,
         dx,
-        A, 
-        sbeta_factor=0.25, 
-        ct_max=0.9999, 
+        A,
+        sbeta_factor=0.25,
+        ct_max=0.9999,
         ti_var=FV.TI,
         **ipars,
     ):
         super().__init__(superpositions={FV.WS: superposition})
 
         self.dx = dx
         self.A = A
@@ -327,42 +330,48 @@
         ct = np.zeros((n_states, n_points), dtype=FC.DTYPE)
         ct[:] = fdata[FV.CT][st_sel][:, None]
         ct[ct > self.ct_max] = self.ct_max
 
         # select targets:
         sp_sel = (x > 1e-5) & (ct > 0.0)
         if np.any(sp_sel):
-
             # apply selection:
-            #x = x[sp_sel]
+            # x = x[sp_sel]
             ct = ct[sp_sel]
 
             # get D:
             D = np.zeros((n_states, n_points), dtype=FC.DTYPE)
             D[:] = fdata[FV.D][st_sel][:, None]
             D = D[sp_sel]
 
             # calculate sigma:
             sbeta = np.sqrt(0.5 * (1 + np.sqrt(1.0 - ct)) / np.sqrt(1.0 - ct))
-            #sblim = 1 / (np.sqrt(8) * self.sbeta_factor)
-            #sbeta[sbeta > sblim] = sblim
+            # sblim = 1 / (np.sqrt(8) * self.sbeta_factor)
+            # sbeta[sbeta > sblim] = sblim
             epsilon = self.sbeta_factor * sbeta
 
             # get TI by integratiion along centre line:
-            ti_ix = algo.wake_frame.calc_centreline_integral(algo, mdata, fdata, 
-                                states_source_turbine, [self.ti_var], x, 
-                                dx=self.dx, **self.ipars)[:, :, 0]
+            ti_ix = algo.wake_frame.calc_centreline_integral(
+                algo,
+                mdata,
+                fdata,
+                states_source_turbine,
+                [self.ti_var],
+                x,
+                dx=self.dx,
+                **self.ipars,
+            )[:, :, 0]
 
             # calculate sigma (eqn 1, plus epsilon from eqn 4 for x = 0)
             sigma = D * epsilon + self.A * ti_ix[sp_sel]
 
             del (
                 x,
                 sbeta,
-                #sblim,
+                # sblim,
                 epsilon,
             )
 
             # calculate amplitude, same as in Bastankha model (eqn 7)
             if self.sbeta_factor < 0.25:
                 radicant = 1.0 - ct / (8 * (sigma / D) ** 2)
                 reals = radicant >= 0
```

### Comparing `foxes-0.3.4/foxes/models/wake_superpositions/linear.py` & `foxes-0.3.5/foxes/models/wake_superpositions/linear.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,14 @@
             and len(scaling) >= 14
             and (
                 scaling == f"source_turbine"
                 or scaling == "source_turbine_amb"
                 or (len(scaling) > 15 and scaling[14] == "_")
             )
         ):
-
             if scaling == f"source_turbine":
                 var = variable
             elif scaling == "source_turbine_amb":
                 var = FV.var2amb[variable]
             else:
                 var = scaling[15:]
```

### Comparing `foxes-0.3.4/foxes/models/wake_superpositions/max.py` & `foxes-0.3.5/foxes/models/wake_superpositions/max.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,14 @@
         else:
             scaling = self.scalings
 
         wake_model_result = np.abs(wake_model_result)
         odelta = wake_delta[sel_sp]
 
         if scaling is None:
-
             wake_delta[sel_sp] = np.maximum(odelta, wake_model_result)
             return wake_delta
 
         elif isinstance(scaling, numbers.Number):
             wake_delta[sel_sp] = np.maximum(odelta, scaling * wake_model_result)
             return wake_delta
 
@@ -138,15 +137,14 @@
             and len(scaling) >= 14
             and (
                 scaling == f"source_turbine"
                 or scaling == "source_turbine_amb"
                 or (len(scaling) > 15 and scaling[14] == "_")
             )
         ):
-
             if scaling == f"source_turbine":
                 var = variable
             elif scaling == "source_turbine_amb":
                 var = FV.var2amb[variable]
             else:
                 var = scaling[15:]
```

### Comparing `foxes-0.3.4/foxes/models/wake_superpositions/quadratic.py` & `foxes-0.3.5/foxes/models/wake_superpositions/quadratic.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,14 @@
             and len(scaling) >= 14
             and (
                 scaling == f"source_turbine"
                 or scaling == "source_turbine_amb"
                 or (len(scaling) > 15 and scaling[14] == "_")
             )
         ):
-
             if scaling == f"source_turbine":
                 var = variable
             elif scaling == "source_turbine_amb":
                 var = FV.var2amb[variable]
             else:
                 var = scaling[15:]
```

### Comparing `foxes-0.3.4/foxes/models/wake_superpositions/ti_superp.py` & `foxes-0.3.5/foxes/models/wake_superpositions/ti_superp.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,27 +120,25 @@
         final_wake_delta : numpy.ndarray
             The final wake delta, which will be added to the ambient
             results by simple plus operation. Shape: (n_states, n_points)
 
         """
         # linear superposition to ambient:
         if self.superp_to_amb == "linear":
-
             if self.ti_superp == "linear" or self.ti_superp == "max":
                 return wake_delta
             elif self.ti_superp == "quadratic":
                 return np.sqrt(wake_delta)
             else:
                 raise ValueError(
                     f"Unknown ti_superp = '{self.ti_superp}', valid choices: linear, quadratic, max"
                 )
 
         # quadratic superposition to ambient:
         elif self.superp_to_amb == "quadratic":
-
             if self.ti_superp == "linear" or self.ti_superp == "max":
                 return np.sqrt(wake_delta**2 + amb_results**2) - amb_results
             elif self.ti_superp == "quadratic":
                 return np.sqrt(wake_delta + amb_results**2) - amb_results
             else:
                 raise ValueError(
                     f"Unknown ti_superp = '{self.ti_superp}', valid choices: linear, quadratic, max"
```

### Comparing `foxes-0.3.4/foxes/opt/constraints/area_geometry.py` & `foxes-0.3.5/foxes/opt/constraints/area_geometry.py`

 * *Files 5% similar despite different names*

```diff
@@ -125,17 +125,17 @@
         xy = vars_float.reshape(self.n_components(), 2)[s]
 
         dists = self.geometry.points_distance(xy)
         dists[self.geometry.points_inside(xy)] *= -1
 
         if self.disc_inside:
             if self.D is None:
-                dists += problem_results[FV.D].to_numpy()[0, self.sel_turbines][s]/2
+                dists += problem_results[FV.D].to_numpy()[0, self.sel_turbines][s] / 2
             else:
-                dists += self.D/2
+                dists += self.D / 2
 
         return dists
 
     def calc_population(self, vars_int, vars_float, problem_results, components=None):
         """
         Calculate values for all individuals of a population.
 
@@ -167,17 +167,19 @@
 
         dists = self.geometry.points_distance(xy)
         dists[self.geometry.points_inside(xy)] *= -1
         dists = dists.reshape(n_pop, n_cmpnts)
 
         if self.disc_inside:
             if self.D is None:
-                dists += problem_results[FV.D].to_numpy()[None, 0, self.sel_turbines][s]/2
+                dists += (
+                    problem_results[FV.D].to_numpy()[None, 0, self.sel_turbines][s] / 2
+                )
             else:
-                dists += self.D/2
+                dists += self.D / 2
 
         return dists
 
 
 class FarmBoundaryConstraint(AreaGeometryConstraint):
     """
     Constrains turbine positions to the inside of
```

### Comparing `foxes-0.3.4/foxes/opt/constraints/min_dist.py` & `foxes-0.3.5/foxes/opt/constraints/min_dist.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 
 from foxes.opt.core.farm_constraint import FarmConstraint
 import foxes.variables as FV
-
+import foxes.constants as FC
 
 class MinDistConstraint(FarmConstraint):
     """
     Turbines must keep at least a minimal
     spatial distance.
 
     Parameters
@@ -191,15 +191,15 @@
         -------
         values : np.array
             The component values, shape: (n_pop, n_sel_components)
 
         """
         n_pop = problem_results["n_pop"].values
         n_states = problem_results["n_org_states"].values
-        n_turbines = problem_results.dims[FV.TURBINE]
+        n_turbines = problem_results.dims[FC.TURBINE]
 
         xy = np.stack(
             [problem_results[FV.X].to_numpy(), problem_results[FV.Y].to_numpy()],
             axis=-1,
         )
         xy = xy.reshape(n_pop, n_states, n_turbines, 2)
         if not np.all(np.abs(np.min(xy, axis=1) - np.max(xy, axis=1)) < 1e-13):
```

### Comparing `foxes-0.3.4/foxes/opt/core/farm_constraint.py` & `foxes-0.3.5/foxes/opt/core/farm_constraint.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,19 @@
 
         Returns
         -------
         list of int :
             The list of selected turbines
 
         """
-        return self.problem.sel_turbines if self._sel_turbines is None else self._sel_turbines
+        return (
+            self.problem.sel_turbines
+            if self._sel_turbines is None
+            else self._sel_turbines
+        )
 
     @property
     def n_sel_turbines(self):
         """
         The numer of selected turbines
 
         Returns
```

### Comparing `foxes-0.3.4/foxes/opt/core/farm_objective.py` & `foxes-0.3.5/foxes/opt/core/farm_objective.py`

 * *Files 11% similar despite different names*

```diff
@@ -46,15 +46,19 @@
 
         Returns
         -------
         list of int :
             The list of selected turbines
 
         """
-        return self.problem.sel_turbines if self._sel_turbines is None else self._sel_turbines
+        return (
+            self.problem.sel_turbines
+            if self._sel_turbines is None
+            else self._sel_turbines
+        )
 
     @property
     def n_sel_turbines(self):
         """
         The numer of selected turbines
 
         Returns
```

### Comparing `foxes-0.3.4/foxes/opt/core/farm_opt_problem.py` & `foxes-0.3.5/foxes/opt/core/farm_opt_problem.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from iwopy import Problem
 
 from foxes.utils.runners import DefaultRunner
-import foxes.variables as FV
+import foxes.constants as FC
 from .pop_states import PopStates
 
 
 class FarmOptProblem(Problem):
     """
     Abstract base class of wind farm optimization problems.
 
@@ -74,15 +74,19 @@
 
         Returns
         -------
         list of int :
             Indices of the selected turbines
 
         """
-        return self._sel_turbines if self._sel_turbines is not None else list(range(self.farm.n_turbines))
+        return (
+            self._sel_turbines
+            if self._sel_turbines is not None
+            else list(range(self.farm.n_turbines))
+        )
 
     @property
     def n_sel_turbines(self):
         """
         The numer of selected turbines
 
         Returns
@@ -101,15 +105,15 @@
         Returns
         -------
         bool :
             True if all turbines are subject to optimization
 
         """
         return len(self.sel_turbines) == self.algo.n_turbines
-    
+
     @property
     def counter(self):
         """
         The current value of the application counter
 
         Returns
         -------
@@ -189,15 +193,15 @@
                             keep = False
                             break
                     if not keep:
                         break
                 if keep:
                     self.algo.keep_models.append(mname)
 
-    def initialize(self, drop_vars=[FV.STATE], exclude=None, verbosity=1):
+    def initialize(self, drop_vars=[FC.STATE], exclude=None, verbosity=1):
         """
         Initialize the object.
 
         Parameters
         ----------
         drop_vars : list of str
             Variables that decide about dropping model
@@ -233,21 +237,21 @@
         """
         Reset the states in the algorithm
         """
         if states is not self.algo.states:
             if self.algo.initialized:
                 self.algo.finalize()
             self.algo.states = states
-    
+
     def update_problem_individual(self, vars_int, vars_float):
         """
         Update the algo and other data using
         the latest optimization variables.
-        
-        This function is called before running the farm 
+
+        This function is called before running the farm
         calculation.
 
         Parameters
         ----------
         vars_int : np.array
             The integer variable values, shape: (n_vars_int,)
         vars_float : np.array
@@ -259,16 +263,16 @@
             self._reset_states(self.algo.states.states)
             self.algo.n_states = self._org_n_states
 
     def update_problem_population(self, vars_int, vars_float):
         """
         Update the algo and other data using
         the latest optimization variables.
-        
-        This function is called before running the farm 
+
+        This function is called before running the farm
         calculation.
 
         Parameters
         ----------
         vars_int : np.array
             The integer variable values, shape: (n_pop, n_vars_int,)
         vars_float : np.array
@@ -296,15 +300,15 @@
 
         Returns
         -------
         problem_results : Any
             The results of the variable application
             to the problem
 
-        """       
+        """
         self._count += 1
         self.update_problem_individual(vars_int, vars_float)
         return self.runner.run(self.algo.calc_farm, kwargs=self.calc_farm_args)
 
     def apply_population(self, vars_int, vars_float):
         """
         Apply new variables to the problem,
@@ -321,15 +325,15 @@
         -------
         problem_results : Any
             The results of the variable application
             to the problem
 
         """
         self._count += 1
-        
+
         self.update_problem_population(vars_int, vars_float)
         results = self.runner.run(self.algo.calc_farm, kwargs=self.calc_farm_args)
         results["n_pop"] = len(vars_float)
         results["n_org_states"] = self._org_n_states
 
         return results
```

### Comparing `foxes-0.3.4/foxes/opt/core/farm_vars_problem.py` & `foxes-0.3.5/foxes/opt/core/farm_vars_problem.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         Parameters
         ----------
         pre_rotor_vars : list of str or dict
             The pre_rotor farm variables. If dict, then
             key: sub-model str, value: var names as list of str
         post_rotor_vars : list of str or dict
             The post_rotor farm variables. If dict, then
-            key: sub-model str, value: var names as list of str   
+            key: sub-model str, value: var names as list of str
         verbosity : int
             The verbosity level, 0 = silent
         kwargs : dict, optional
             Additional parameters for super class init
 
         """
         self._vars_pre = {}
@@ -40,38 +40,41 @@
             self._vars_post = {m: v for m, v in post_rotor_vars.items() if len(v)}
         elif len(post_rotor_vars):
             self._vars_post = {self.name: post_rotor_vars}
 
         cnt = 0
         for src, pre in zip((self._vars_pre, self._vars_post), (True, False)):
             for mname, vrs in src.items():
-
                 if mname in self.algo.mbook.turbine_models:
                     m = self.algo.mbook.turbine_models[mname]
                     if not isinstance(m, SetFarmVars):
                         raise KeyError(
                             f"FarmOptProblem '{self.name}': Turbine model entry '{mname}' already exists in model book, and is not of type SetFarmVars"
                         )
                     elif m.pre_rotor != pre:
-                        raise ValueError(f"FarmOptProblem '{self.name}': Turbine model entry '{mname}' exists in model book, and disagrees on pre_rotor = {pre}")
+                        raise ValueError(
+                            f"FarmOptProblem '{self.name}': Turbine model entry '{mname}' exists in model book, and disagrees on pre_rotor = {pre}"
+                        )
                 else:
                     self.algo.mbook.turbine_models[mname] = SetFarmVars(pre_rotor=pre)
 
                 found = False
                 for t in self.algo.farm.turbines:
                     if mname in t.models:
                         found = True
                         break
                 if not found:
                     raise ValueError(
                         f"FarmOptProblem '{self.name}': Missing entry '{mname}' among any of the turbine models"
                     )
                 cnt += len(vrs)
         if not cnt:
-            raise ValueError(f"Problem '{self.name}': Neither pre_rotor_vars not post_rotor_vars containing variables")
+            raise ValueError(
+                f"Problem '{self.name}': Neither pre_rotor_vars not post_rotor_vars containing variables"
+            )
 
         super().initialize(verbosity=verbosity, **kwargs)
 
     @abstractmethod
     def opt2farm_vars_individual(self, vars_int, vars_float):
         """
         Translates optimization variables to farm variables
@@ -121,16 +124,16 @@
         """
         pass
 
     def update_problem_individual(self, vars_int, vars_float):
         """
         Update the algo and other data using
         the latest optimization variables.
-        
-        This function is called before running the farm 
+
+        This function is called before running the farm
         calculation.
 
         Parameters
         ----------
         vars_int : np.array
             The integer variable values, shape: (n_vars_int,)
         vars_float : np.array
@@ -156,22 +159,24 @@
                         data = np.zeros(
                             (n_states, self.algo.n_turbines), dtype=FC.DTYPE
                         )
                         data[:, self.sel_turbines] = vals
                         model.add_var(v, data)
 
         if len(fvars):
-            raise KeyError(f"Problem '{self.name}': Too many farm vars from opt2farm_vars_individual: {list(fvars.keys())}")
-        
+            raise KeyError(
+                f"Problem '{self.name}': Too many farm vars from opt2farm_vars_individual: {list(fvars.keys())}"
+            )
+
     def update_problem_population(self, vars_int, vars_float):
         """
         Update the algo and other data using
         the latest optimization variables.
-        
-        This function is called before running the farm 
+
+        This function is called before running the farm
         calculation.
 
         Parameters
         ----------
         vars_int : np.array
             The integer variable values, shape: (n_pop, n_vars_int,)
         vars_float : np.array
@@ -202,8 +207,10 @@
                             (n_pstates, self.algo.n_turbines), dtype=FC.DTYPE
                         )
                         data[:, self.sel_turbines] = vals.reshape(shp1)
                         model.add_var(v, data)
                         del data
 
         if len(fvars):
-            raise KeyError(f"Problem '{self.name}': Too many farm vars from opt2farm_vars_population: {list(fvars.keys())}")
+            raise KeyError(
+                f"Problem '{self.name}': Too many farm vars from opt2farm_vars_population: {list(fvars.keys())}"
+            )
```

### Comparing `foxes-0.3.4/foxes/opt/core/pop_states.py` & `foxes-0.3.5/foxes/opt/core/pop_states.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,40 +53,42 @@
         -------
         idata : dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
-        self.STATE0 = self.var(FV.STATE + "0")
+        self.STATE0 = self.var(FC.STATE + "0")
         self.SMAP = self.var("SMAP")
 
         idata = super().initialize(algo, verbosity)
         self._update_idata(algo, idata)
 
         if not self.states.name in algo._idata_mem:
-            raise KeyError(f"States idata '{self.states.name}' not found in algo idata memory")
+            raise KeyError(
+                f"States idata '{self.states.name}' not found in algo idata memory"
+            )
         else:
             idata0 = algo._idata_mem[self.states.name]
 
         for cname, coord in idata0["coords"].items():
-            if cname != FV.STATE:
+            if cname != FC.STATE:
                 idata["coords"][cname] = coord
             else:
                 idata["coords"][self.STATE0] = coord
 
         for dname, (dims0, data0) in idata0["data_vars"].items():
             if dname != FV.WEIGHT:
-                hdims = tuple([d if d != FV.STATE else self.STATE0 for d in dims0])
+                hdims = tuple([d if d != FC.STATE else self.STATE0 for d in dims0])
                 idata["data_vars"][dname] = (hdims, data0)
 
         smap = np.zeros((self.n_pop, self.states.size()), dtype=np.int32)
         smap[:] = np.arange(self.states.size())[None, :]
         smap = smap.reshape(self.size())
-        idata["data_vars"][self.SMAP] = ((FV.STATE,), smap)
+        idata["data_vars"][self.SMAP] = ((FC.STATE,), smap)
 
         found = False
         for dname, (dims0, data0) in idata["data_vars"].items():
             if self.STATE0 in dims0:
                 found = True
                 break
         if not found:
@@ -175,15 +177,15 @@
         smap = mdata[self.SMAP]
         for dname, data in mdata.items():
             dms = mdata.dims[dname]
             if dname == self.SMAP or dname == self.STATE0:
                 pass
             elif dms[0] == self.STATE0:
                 hdata[dname] = data[smap]
-                hdims[dname] = tuple([FV.STATE] + list(dms)[1:])
+                hdims[dname] = tuple([FC.STATE] + list(dms)[1:])
             elif self.STATE0 in dms:
                 raise ValueError(
                     f"States '{self.name}': Found states variable not at dimension 0 for mdata entry '{dname}': {dms}"
                 )
             else:
                 hdata[dname] = data
                 hdims[dname] = dms
```

### Comparing `foxes-0.3.4/foxes/opt/objectives/farm_vars.py` & `foxes-0.3.5/foxes/opt/objectives/farm_vars.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import xarray as xr
 
 from foxes.opt.core.farm_objective import FarmObjective
 from foxes import variables as FV
-
+import foxes.constants as FC
 
 class FarmVarObjective(FarmObjective):
     """
     Objectives based on farm variables.
 
     Parameters
     ----------
@@ -61,15 +61,15 @@
         **kwargs,
     ):
         super().__init__(problem, name, **kwargs)
         self.variable = variable
         self.minimize = minimize
         self.deps = deps
         self.scale = scale
-        self.rules = {FV.STATE: contract_states, FV.TURBINE: contract_turbines}
+        self.rules = {FC.STATE: contract_states, FC.TURBINE: contract_turbines}
 
     def initialize(self, verbosity=0):
         """
         Initialize the object.
 
         Parameters
         ----------
@@ -172,15 +172,14 @@
 
         """
         data = problem_results[self.variable]
         if self.n_sel_turbines < self.farm.n_turbines:
             data = data[:, self.sel_turbines]
         data = self._contract(data) / self.scale
 
-
         return np.array([data], dtype=np.float64)
 
     def calc_population(self, vars_int, vars_float, problem_results, components=None):
         """
         Calculate values for all individuals of a population.
 
         Parameters
@@ -199,21 +198,21 @@
         -------
         values : np.array
             The component values, shape: (n_pop, n_sel_components)
 
         """
         n_pop = problem_results["n_pop"].values
         n_states = problem_results["n_org_states"].values
-        n_turbines = problem_results.dims[FV.TURBINE]
+        n_turbines = problem_results.dims[FC.TURBINE]
         data = (
             problem_results[self.variable]
             .to_numpy()
             .reshape(n_pop, n_states, n_turbines)
         )
-        data = xr.DataArray(data, dims=(FV.POP, FV.STATE, FV.TURBINE))
+        data = xr.DataArray(data, dims=(FC.POP, FC.STATE, FC.TURBINE))
 
         if self.n_sel_turbines < self.farm.n_turbines:
             data = data[:, self.sel_turbines]
 
         return self._contract(data / self.scale).to_numpy()[:, None]
 
     def finalize_individual(self, vars_int, vars_float, problem_results, verbosity=1):
@@ -258,15 +257,14 @@
         The name of the objective function
     kwargs : dict, optional
         Additional parameters for `FarmVarObjective`
 
     """
 
     def __init__(self, problem, name="maximize_power", **kwargs):
-
         if "scale" in kwargs:
             scale = kwargs.pop("scale")
         else:
             scale = 0.0
             ttypes = problem.algo.mbook.turbine_types
             for t in problem.farm.turbines:
                 for mname in t.models:
@@ -281,14 +279,15 @@
             contract_states="mean",
             contract_turbines="sum",
             minimize=False,
             scale=scale,
             **kwargs,
         )
 
+
 class MinimalMaxTI(FarmVarObjective):
     """
     Minimize the maximal turbine TI
 
     Parameters
     ----------
     problem : foxes.opt.FarmOptProblem
@@ -297,19 +296,18 @@
         The name of the objective function
     kwargs : dict, optional
         Additional parameters for `FarmVarObjective`
 
     """
 
     def __init__(self, problem, name="minimize_TI", **kwargs):
-
-        scale = kwargs.pop("scale") if "scale" in kwargs else 1.
+        scale = kwargs.pop("scale") if "scale" in kwargs else 1.0
         super().__init__(
             problem,
             name,
             variable=FV.TI,
             contract_states="max",
             contract_turbines="max",
             minimize=True,
             scale=scale,
             **kwargs,
-        )
+        )
```

### Comparing `foxes-0.3.4/foxes/opt/objectives/max_n_turbines.py` & `foxes-0.3.5/foxes/opt/objectives/max_n_turbines.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import numpy as np
 
 from foxes.opt.core.farm_objective import FarmObjective
-import foxes.variables as FV
+import foxes.constants as FC
 
 class MaxNTurbines(FarmObjective):
     """
     Maximizes the number of turrbines.
 
     Parameters
     ----------
     problem : foxes.opt.FarmOptProblem
         The underlying optimization problem
     name : str
         The name of the objective function
     check_valid : bool
-        Check FV.VALID variable before counting
+        Check FC.VALID variable before counting
     kwargs : dict, optional
         Additional parameters for `FarmObjective`
 
     Attributes
     ----------
     check_valid : bool
-        Check FV.VALID variable before counting
+        Check FC.VALID variable before counting
 
     """
 
     def __init__(
         self,
         problem,
         name="max_n_turbines",
@@ -80,18 +80,20 @@
 
         Returns
         -------
         values : np.array
             The component values, shape: (n_sel_components,)
 
         """
-        if FV.VALID in problem_results and self.check_valid:
-            vld = np.sum(problem_results[FV.VALID].to_numpy(), axis=1)
+        if FC.VALID in problem_results and self.check_valid:
+            vld = np.sum(problem_results[FC.VALID].to_numpy(), axis=1)
             if np.min(vld) != np.max(vld):
-                raise ValueError(f"Objective '{self.name}': Number of valid turbines is state dependend, counting impossible")
+                raise ValueError(
+                    f"Objective '{self.name}': Number of valid turbines is state dependend, counting impossible"
+                )
             return np.array([vld[0]], dtype=np.float64)
         else:
             return np.array([self.farm.n_turbines], dtype=np.float64)
 
     def calc_population(self, vars_int, vars_float, problem_results, components=None):
         """
         Calculate values for all individuals of a population.
@@ -114,15 +116,20 @@
             The component values, shape: (n_pop, n_sel_components)
 
         """
         n_pop = problem_results["n_pop"].to_numpy()
         if self.check_valid:
             n_states = problem_results["n_org_states"].to_numpy()
             n_turbines = self.farm.n_turbines
-            vld = problem_results[FV.VALID].to_numpy().reshape(n_pop, n_states, n_turbines)
+            vld = (
+                problem_results[FC.VALID]
+                .to_numpy()
+                .reshape(n_pop, n_states, n_turbines)
+            )
             vld = np.sum(vld, axis=2)
             if np.any(np.min(vld, axis=1) != np.max(vld, axis=1)):
-                raise ValueError(f"Objective '{self.name}': Number of valid turbines is state dependend, counting impossible")
+                raise ValueError(
+                    f"Objective '{self.name}': Number of valid turbines is state dependend, counting impossible"
+                )
             return vld[:, 0, None]
         else:
             return np.full((n_pop, 1), self.farm.n_turbines, dtype=vars_float.dtype)
-
```

### Comparing `foxes-0.3.4/foxes/opt/problems/layout/farm_layout.py` & `foxes-0.3.5/foxes/opt/problems/layout/farm_layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,26 +77,26 @@
         return out.reshape(self.n_sel_turbines * 2)
 
     def initialize(self, verbosity=1, **kwargs):
         """
         Initialize the object.
 
         Parameters
-        ---------- 
+        ----------
         verbosity : int
             The verbosity level, 0 = silent
         kwargs : dict, optional
             Additional parameters for super class init
 
         """
         super().initialize(
             pre_rotor_vars=[FV.X, FV.Y],
             post_rotor_vars=[],
             verbosity=verbosity,
-            **kwargs
+            **kwargs,
         )
 
     def opt2farm_vars_individual(self, vars_int, vars_float):
         """
         Translates optimization variables to farm variables
 
         Parameters
```

### Comparing `foxes-0.3.4/foxes/opt/problems/layout/geom_layouts/constraints.py` & `foxes-0.3.5/foxes/opt/problems/layout/geom_layouts/constraints.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,83 +1,100 @@
 import numpy as np
 from scipy.spatial.distance import cdist
 from iwopy import Constraint
 
 import foxes.constants as FC
 
-class Valid(Constraint):
 
+class Valid(Constraint):
     def __init__(self, problem, name="valid", **kwargs):
-        super().__init__(problem, name, vnames_int=problem.var_names_int(), 
-            vnames_float=problem.var_names_float(), **kwargs)
+        super().__init__(
+            problem,
+            name,
+            vnames_int=problem.var_names_int(),
+            vnames_float=problem.var_names_float(),
+            **kwargs,
+        )
 
     def n_components(self):
         return 1
 
     def calc_individual(self, vars_int, vars_float, problem_results, cmpnts=None):
         __, valid = problem_results
         return np.sum(~valid)
 
     def calc_population(self, vars_int, vars_float, problem_results, cmpnts=None):
         __, valid = problem_results
         return np.sum(~valid, axis=1)[:, None]
 
-class Boundary(Constraint):
 
+class Boundary(Constraint):
     def __init__(self, problem, n_turbines=None, D=None, name="boundary", **kwargs):
-        super().__init__(problem, name, vnames_int=problem.var_names_int(), 
-            vnames_float=problem.var_names_float(), **kwargs)
+        super().__init__(
+            problem,
+            name,
+            vnames_int=problem.var_names_int(),
+            vnames_float=problem.var_names_float(),
+            **kwargs,
+        )
         self.n_turbines = problem.n_turbines if n_turbines is None else n_turbines
         self.D = problem.D if D is None else D
 
     def n_components(self):
         return self.n_turbines
 
     def calc_individual(self, vars_int, vars_float, problem_results, cmpnts=None):
         xy, __ = problem_results
-        
+
         dists = self.problem.boundary.points_distance(xy)
         dists[self.problem.boundary.points_inside(xy)] *= -1
 
         if self.D is not None:
-            dists += self.D/2
-        
+            dists += self.D / 2
+
         return dists
 
     def calc_population(self, vars_int, vars_float, problem_results, cmpnts=None):
         xy, __ = problem_results
         n_pop, n_xy = xy.shape[:2]
 
-        xy = xy.reshape(n_pop*n_xy, 2)
+        xy = xy.reshape(n_pop * n_xy, 2)
         dists = self.problem.boundary.points_distance(xy)
         dists[self.problem.boundary.points_inside(xy)] *= -1
         dists = dists.reshape(n_pop, n_xy)
 
         if self.D is not None:
-            dists += self.D/2
+            dists += self.D / 2
 
         return dists
 
-class MinDist(Constraint):
 
-    def __init__(self, problem, min_dist=None, n_turbines=None, name="min_dist", **kwargs):
-        super().__init__(problem, name, vnames_int=problem.var_names_int(), 
-            vnames_float=problem.var_names_float(), **kwargs)
+class MinDist(Constraint):
+    def __init__(
+        self, problem, min_dist=None, n_turbines=None, name="min_dist", **kwargs
+    ):
+        super().__init__(
+            problem,
+            name,
+            vnames_int=problem.var_names_int(),
+            vnames_float=problem.var_names_float(),
+            **kwargs,
+        )
         self.min_dist = problem.min_dist if min_dist is None else min_dist
         self.n_turbines = problem.n_turbines if n_turbines is None else n_turbines
 
     def initialize(self, verbosity=0):
         """
         Initialize the constaint.
 
         Parameters
         ----------
         verbosity : int
             The verbosity level, 0 = silent
-            
+
         """
         N = self.n_turbines
         self._i2t = []  # i --> (ti, tj)
         self._t2i = np.full([N, N], -1)  # (ti, tj) --> i
         i = 0
         for ti in range(N):
             for tj in range(N):
@@ -106,56 +123,72 @@
         xy, __ = problem_results
 
         a = np.take_along_axis(xy, self._i2t[None, :, 0, None], axis=1)
         b = np.take_along_axis(xy, self._i2t[None, :, 1, None], axis=1)
         d = np.linalg.norm(a - b, axis=-1)
 
         return self.min_dist - d
-    
-class CMinN(Constraint):
 
+
+class CMinN(Constraint):
     def __init__(self, problem, N, name="cminN", **kwargs):
-        super().__init__(problem, name, vnames_int=problem.var_names_int(), 
-            vnames_float=problem.var_names_float(), **kwargs)
+        super().__init__(
+            problem,
+            name,
+            vnames_int=problem.var_names_int(),
+            vnames_float=problem.var_names_float(),
+            **kwargs,
+        )
         self.N = N
 
     def n_components(self):
         return 1
 
     def calc_individual(self, vars_int, vars_float, problem_results, cmpnts=None):
         __, valid = problem_results
         return self.N - np.sum(valid)
 
     def calc_population(self, vars_int, vars_float, problem_results, cmpnts=None):
         __, valid = problem_results
         return self.N - np.sum(valid, axis=1)[:, None]
 
-class CMaxN(Constraint):
 
+class CMaxN(Constraint):
     def __init__(self, problem, N, name="cmaxN", **kwargs):
-        super().__init__(problem, name, vnames_int=problem.var_names_int(), 
-            vnames_float=problem.var_names_float(), **kwargs)
+        super().__init__(
+            problem,
+            name,
+            vnames_int=problem.var_names_int(),
+            vnames_float=problem.var_names_float(),
+            **kwargs,
+        )
         self.N = N
 
     def n_components(self):
         return 1
 
     def calc_individual(self, vars_int, vars_float, problem_results, cmpnts=None):
         __, valid = problem_results
         return np.sum(valid) - self.N
 
     def calc_population(self, vars_int, vars_float, problem_results, cmpnts=None):
         __, valid = problem_results
         return np.sum(valid, axis=1)[:, None] - self.N
 
-class CFixN(Constraint):
 
+class CFixN(Constraint):
     def __init__(self, problem, N, name="cfixN", **kwargs):
-        super().__init__(problem, name, vnames_int=problem.var_names_int(), 
-            vnames_float=problem.var_names_float(), tol=0.1, **kwargs)
+        super().__init__(
+            problem,
+            name,
+            vnames_int=problem.var_names_int(),
+            vnames_float=problem.var_names_float(),
+            tol=0.1,
+            **kwargs,
+        )
         self.N = N
 
     def n_components(self):
         return 2
 
     def calc_individual(self, vars_int, vars_float, problem_results, cmpnts=None):
         __, valid = problem_results
@@ -163,42 +196,47 @@
         return np.array([self.N - vld, vld - self.N])
 
     def calc_population(self, vars_int, vars_float, problem_results, cmpnts=None):
         __, valid = problem_results
         vld = np.sum(valid, axis=1)
         return np.stack([self.N - vld, vld - self.N], axis=-1)
 
-class CMinDensity(Constraint):
 
+class CMinDensity(Constraint):
     def __init__(self, problem, min_value, dfactor=1, name="min_density"):
-        super().__init__(problem, name, vnames_int=problem.var_names_int(), 
-            vnames_float=problem.var_names_float())
+        super().__init__(
+            problem,
+            name,
+            vnames_int=problem.var_names_int(),
+            vnames_float=problem.var_names_float(),
+        )
         self.min_value = min_value
         self.dfactor = dfactor
 
     def n_components(self):
         return 1
-    
+
     def initialize(self, verbosity):
         super().initialize(verbosity)
-        
+
         # define regular grid of probe points:
         geom = self.problem.boundary
         pmin = geom.p_min()
         pmax = geom.p_max()
         detlta = self.problem.min_dist / self.dfactor
         self._probes = np.stack(
             np.meshgrid(
-                np.arange(pmin[0]-detlta, pmax[0]+2*detlta, detlta),
-                np.arange(pmin[1]-detlta, pmax[1]+2*detlta, detlta),
-                indexing='ij'
-            ), axis=-1
+                np.arange(pmin[0] - detlta, pmax[0] + 2 * detlta, detlta),
+                np.arange(pmin[1] - detlta, pmax[1] + 2 * detlta, detlta),
+                indexing="ij",
+            ),
+            axis=-1,
         )
         nx, ny = self._probes.shape[:2]
-        n = nx*ny
+        n = nx * ny
         self._probes = self._probes.reshape(n, 2)
 
         # reduce to points within geometry:
         valid = geom.points_inside(self._probes)
         self._probes = self._probes[valid]
 
     def calc_individual(self, vars_int, vars_float, problem_results, cmpnts=None):
@@ -211,9 +249,9 @@
         n_pop = vars_float.shape[0]
         xy, valid = problem_results
         out = np.full(n_pop, 1e20, dtype=FC.DTYPE)
         for pi in range(n_pop):
             if np.any(valid[pi]):
                 hxy = xy[pi][valid[pi]]
                 dists = cdist(self._probes, hxy)
-                out[pi] = np.nanmax(np.nanmin(dists, axis=1)) -  self.min_value
-        return out[:, None]
+                out[pi] = np.nanmax(np.nanmin(dists, axis=1)) - self.min_value
+        return out[:, None]
```

### Comparing `foxes-0.3.4/foxes/opt/problems/layout/geom_layouts/geom_layout.py` & `foxes-0.3.5/foxes/opt/problems/layout/geom_layouts/geom_layout.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
 import matplotlib.pyplot as plt
 from scipy.spatial.distance import cdist
 from iwopy import Problem
 
 import foxes.constants as FC
 
+
 class GeomLayout(Problem):
     """
     A layout within a boundary geometry, purely
     defined by geometrical optimization (no wakes).
 
     This optimization problem does not involve
     wind farms.
@@ -38,21 +39,21 @@
         The diameter of circle fully within boundary
     calc_valid : bool
         Evaluate validity
 
     """
 
     def __init__(
-            self, 
-            boundary, 
-            n_turbines, 
-            min_dist=None,
-            D=None,
-            calc_valid=None,
-        ):
+        self,
+        boundary,
+        n_turbines,
+        min_dist=None,
+        D=None,
+        calc_valid=None,
+    ):
         super().__init__(name="geom_reg_grids")
 
         self.boundary = boundary
         self.n_turbines = n_turbines
         self.D = D
         self.min_dist = min_dist
         self.calc_valid = calc_valid
@@ -95,22 +96,24 @@
         -------
         values : numpy.ndarray
             Initial float values, shape: (n_vars_float,)
 
         """
         pmin = self.boundary.p_min()
         pmax = self.boundary.p_max()
-        pc = 0.5*(pmin + pmax)
-        delta = 0.8*(pmax-pmin)
+        pc = 0.5 * (pmin + pmax)
+        delta = 0.8 * (pmax - pmin)
 
         vals = np.zeros((self.n_turbines, 2), dtype=FC.DTYPE)
-        vals[:] = pc[None, :] - 0.5*delta[None, :]
-        vals[:] += np.arange(self.n_turbines)[:, None]*delta[None, :]/(self.n_turbines-1)
+        vals[:] = pc[None, :] - 0.5 * delta[None, :]
+        vals[:] += (
+            np.arange(self.n_turbines)[:, None] * delta[None, :] / (self.n_turbines - 1)
+        )
 
-        return vals.reshape(self.n_turbines*2)
+        return vals.reshape(self.n_turbines * 2)
 
     def min_values_float(self):
         """
         The minimal values of the float variables.
 
         Use -numpy.inf for unbounded.
 
@@ -118,15 +121,15 @@
         -------
         values : numpy.ndarray
             Minimal float values, shape: (n_vars_float,)
 
         """
         vals = np.zeros((self.n_turbines, 2), dtype=FC.DTYPE)
         vals[:] = self.boundary.p_min()[None, :]
-        return vals.reshape(self.n_turbines*2)
+        return vals.reshape(self.n_turbines * 2)
 
     def max_values_float(self):
         """
         The maximal values of the float variables.
 
         Use numpy.inf for unbounded.
 
@@ -134,15 +137,15 @@
         -------
         values : numpy.ndarray
             Maximal float values, shape: (n_vars_float,)
 
         """
         vals = np.zeros((self.n_turbines, 2), dtype=FC.DTYPE)
         vals[:] = self.boundary.p_max()[None, :]
-        return vals.reshape(self.n_turbines*2)
+        return vals.reshape(self.n_turbines * 2)
 
     def apply_individual(self, vars_int, vars_float):
         """
         Apply new variables to the problem.
 
         Parameters
         ----------
@@ -153,35 +156,34 @@
 
         Returns
         -------
         problem_results : Any
             The results of the variable application
             to the problem
 
-        """       
+        """
         xy = vars_float.reshape(self.n_turbines, 2)
 
         valid = None
         if self.calc_valid:
             if self.D is None:
                 valid = self.boundary.points_inside(xy)
             else:
-                valid = (
-                    self.boundary.points_inside(xy) &
-                    (self.boundary.points_distance(xy) >= self.D / 2)
+                valid = self.boundary.points_inside(xy) & (
+                    self.boundary.points_distance(xy) >= self.D / 2
                 )
-            
+
             if self.min_dist is not None:
                 dists = cdist(xy, xy)
                 np.fill_diagonal(dists, 1e20)
                 dists = np.min(dists, axis=1)
-                valid[dists<self.min_dist] = False
-        
+                valid[dists < self.min_dist] = False
+
         return xy, valid
-    
+
     def apply_population(self, vars_int, vars_float):
         """
         Apply new variables to the problem,
         for a whole population.
 
         Parameters
         ----------
@@ -198,34 +200,35 @@
 
         """
         n_pop = vars_float.shape[0]
         xy = vars_float.reshape(n_pop, self.n_turbines, 2)
 
         valid = None
         if self.calc_valid:
-            qts = xy.reshape(n_pop*self.n_turbines, 2)
+            qts = xy.reshape(n_pop * self.n_turbines, 2)
             if self.D is None:
                 valid = self.boundary.points_inside(qts)
             else:
-                valid = (
-                    self.boundary.points_inside(qts) &
-                    (self.boundary.points_distance(qts) >= self.D / 2)
+                valid = self.boundary.points_inside(qts) & (
+                    self.boundary.points_distance(qts) >= self.D / 2
                 )
             valid = valid.reshape(n_pop, self.n_turbines)
 
             if self.min_dist is not None:
                 for pi in range(n_pop):
                     dists = cdist(xy[pi], xy[pi])
                     np.fill_diagonal(dists, 1e20)
                     dists = np.min(dists, axis=1)
-                    valid[pi, dists<self.min_dist] = False
-        
+                    valid[pi, dists < self.min_dist] = False
+
         return xy, valid
 
-    def get_fig(self, xy=None, valid=None, ax=None, title=None, true_circle=True, **bargs):
+    def get_fig(
+        self, xy=None, valid=None, ax=None, title=None, true_circle=True, **bargs
+    ):
         """
         Return plotly figure axis.
 
         Parameters
         ----------
         xy : numpy.ndarary, optional
             The xy coordinate array, shape: (n_points, 2)
@@ -235,36 +238,38 @@
             The figure axis
         title : str, optional
             The figure title
         true_circle : bool
             Draw points as circles with diameter self.D
         bars : dict, optional
             The boundary plot arguments
-        
+
         Returns
         -------
         ax : pyplot.Axis
             The figure axis
 
         """
         if ax is None:
             __, ax = plt.subplots()
-        
+
         hbargs = {"fill_mode": "inside_lightgray"}
         hbargs.update(bargs)
         self.boundary.add_to_figure(ax, **hbargs)
 
         if xy is not None:
             if valid is not None:
                 xy = xy[valid]
             if not true_circle or self.D is None:
                 ax.scatter(xy[:, 0], xy[:, 1], color="orange")
             else:
                 for x, y in xy:
-                    ax.add_patch(plt.Circle((x, y), self.D/2, color="blue", fill=True))
+                    ax.add_patch(
+                        plt.Circle((x, y), self.D / 2, color="blue", fill=True)
+                    )
 
         ax.set_aspect("equal", adjustable="box")
         ax.set_xlabel("x [m]")
         ax.set_ylabel("y [m]")
 
         if title is None:
             if xy is None:
```

### Comparing `foxes-0.3.4/foxes/opt/problems/layout/geom_layouts/geom_layout_gridded.py` & `foxes-0.3.5/foxes/opt/problems/layout/geom_layouts/geom_layout_gridded.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
 import matplotlib.pyplot as plt
 from scipy.spatial.distance import cdist
 from iwopy import Problem
 
 import foxes.constants as FC
 
+
 class GeomLayoutGridded(Problem):
     """
     A layout within a boundary geometry, purely
     defined by geometrical optimization (no wakes),
     on a fixes background point grid.
 
     This optimization problem does not involve
@@ -39,21 +40,21 @@
         The minimal distance between points
     D : float
         The diameter of circle fully within boundary
 
     """
 
     def __init__(
-            self, 
-            boundary, 
-            n_turbines, 
-            grid_spacing,
-            min_dist=None,
-            D=None,
-        ):
+        self,
+        boundary,
+        n_turbines,
+        grid_spacing,
+        min_dist=None,
+        D=None,
+    ):
         super().__init__(name="geom_reg_grids")
 
         self.boundary = boundary
         self.n_turbines = n_turbines
         self.grid_spacing = grid_spacing
         self.D = D
         self.min_dist = min_dist
@@ -71,37 +72,40 @@
 
         """
         super().initialize(verbosity)
 
         pmin = self.boundary.p_min()
         pmax = self.boundary.p_max() + self.grid_spacing
         self._pts = np.stack(
-                np.meshgrid(
-                    np.arange(pmin[0], pmax[0], self.grid_spacing),
-                    np.arange(pmin[1], pmax[1], self.grid_spacing),
-                    indexing='ij'
-                ), axis=-1)
+            np.meshgrid(
+                np.arange(pmin[0], pmax[0], self.grid_spacing),
+                np.arange(pmin[1], pmax[1], self.grid_spacing),
+                indexing="ij",
+            ),
+            axis=-1,
+        )
         nx, ny = self._pts.shape[:2]
-        self._pts = self._pts.reshape(nx*ny, 2)
+        self._pts = self._pts.reshape(nx * ny, 2)
 
         if self.D is None:
             valid = self.boundary.points_inside(self._pts)
         else:
-            valid = (
-                self.boundary.points_inside(self._pts) &
-                (self.boundary.points_distance(self._pts) >= self.D / 2)
+            valid = self.boundary.points_inside(self._pts) & (
+                self.boundary.points_distance(self._pts) >= self.D / 2
             )
         self._pts = self._pts[valid]
         self._N = len(self._pts)
 
-        if verbosity>0:
+        if verbosity > 0:
             print(f"Problem '{self.name}': n_bgd_pts = {self._N}")
 
         if self._N < self.n_turbines:
-            raise ValueError(f"Problem '{self.name}': Background grid only provides {self._N} points for {self.n_turbines} turbines")
+            raise ValueError(
+                f"Problem '{self.name}': Background grid only provides {self._N} points for {self.n_turbines} turbines"
+            )
 
         self.apply_individual(self.initial_values_int(), self.initial_values_float())
 
     def var_names_int(self):
         """
         The names of int variables.
 
@@ -143,15 +147,15 @@
 
         Returns
         -------
         values : numpy.ndarray
             Maximal int values, shape: (n_vars_int,)
 
         """
-        return np.full(self.n_turbines, self._N-1, dtype=FC.ITYPE)
+        return np.full(self.n_turbines, self._N - 1, dtype=FC.ITYPE)
 
     def apply_individual(self, vars_int, vars_float):
         """
         Apply new variables to the problem.
 
         Parameters
         ----------
@@ -162,21 +166,21 @@
 
         Returns
         -------
         problem_results : Any
             The results of the variable application
             to the problem
 
-        """       
+        """
         xy = self._pts[vars_int.astype(FC.ITYPE)]
         __, ui = np.unique(vars_int, return_index=True)
         valid = np.zeros(self.n_turbines, dtype=bool)
         valid[ui] = True
         return xy, valid
-    
+
     def apply_population(self, vars_int, vars_float):
         """
         Apply new variables to the problem,
         for a whole population.
 
         Parameters
         ----------
@@ -190,25 +194,27 @@
         problem_results : Any
             The results of the variable application
             to the problem
 
         """
         n_pop = vars_int.shape[0]
 
-        vint = vars_int.reshape(n_pop*self.n_turbines).astype(FC.ITYPE)
+        vint = vars_int.reshape(n_pop * self.n_turbines).astype(FC.ITYPE)
         xy = self._pts[vint, :].reshape(n_pop, self.n_turbines, 2)
 
         valid = np.zeros((n_pop, self.n_turbines), dtype=bool)
         for pi in range(n_pop):
             __, ui = np.unique(vars_int[pi], return_index=True)
             valid[pi, ui] = True
 
         return xy, valid
 
-    def get_fig(self, xy=None, valid=None, ax=None, title=None, true_circle=True, **bargs):
+    def get_fig(
+        self, xy=None, valid=None, ax=None, title=None, true_circle=True, **bargs
+    ):
         """
         Return plotly figure axis.
 
         Parameters
         ----------
         xy : numpy.ndarary, optional
             The xy coordinate array, shape: (n_points, 2)
@@ -218,36 +224,38 @@
             The figure axis
         title : str, optional
             The figure title
         true_circle : bool
             Draw points as circles with diameter self.D
         bars : dict, optional
             The boundary plot arguments
-        
+
         Returns
         -------
         ax : pyplot.Axis
             The figure axis
 
         """
         if ax is None:
             __, ax = plt.subplots()
-        
+
         hbargs = {"fill_mode": "inside_lightgray"}
         hbargs.update(bargs)
         self.boundary.add_to_figure(ax, **hbargs)
 
         if xy is not None:
             if valid is not None:
                 xy = xy[valid]
             if not true_circle or self.D is None:
                 ax.scatter(xy[:, 0], xy[:, 1], color="orange")
             else:
                 for x, y in xy:
-                    ax.add_patch(plt.Circle((x, y), self.D/2, color="blue", fill=True))
+                    ax.add_patch(
+                        plt.Circle((x, y), self.D / 2, color="blue", fill=True)
+                    )
 
         ax.set_aspect("equal", adjustable="box")
         ax.set_xlabel("x [m]")
         ax.set_ylabel("y [m]")
 
         if title is None:
             if xy is None:
```

### Comparing `foxes-0.3.4/foxes/opt/problems/layout/geom_layouts/geom_reggrid.py` & `foxes-0.3.5/foxes/opt/problems/layout/geom_layouts/geom_reggrid.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
 import matplotlib.pyplot as plt
 from scipy.spatial.distance import cdist
 from iwopy import Problem
 
 import foxes.constants as FC
 
+
 class GeomRegGrid(Problem):
     """
     A regular grid within a boundary geometry.
 
     This optimization problem does not involve
     wind farms.
 
@@ -37,21 +38,21 @@
         The maximal distance between points
     D : float
         The diameter of circle fully within boundary
 
     """
 
     def __init__(
-            self, 
-            boundary, 
-            n_turbines,
-            min_dist, 
-            max_dist=None,
-            D=None,
-        ):
+        self,
+        boundary,
+        n_turbines,
+        min_dist,
+        max_dist=None,
+        D=None,
+    ):
         super().__init__(name="geom_reg_grid")
 
         self.boundary = boundary
         self.n_turbines = n_turbines
         self.min_dist = float(min_dist)
         self.max_dist = float(max_dist) if max_dist is not None else max_dist
         self.D = D
@@ -72,19 +73,22 @@
             The verbosity level, 0 = silent
 
         """
         super().initialize(verbosity)
 
         pmin = self.boundary.p_min()
         pmax = self.boundary.p_max()
-        self._pc = 0.5*(pmin + pmax)
+        self._pc = 0.5 * (pmin + pmax)
         self._diag = np.linalg.norm(pmax - pmin)
         self.max_dist = self._diag if self.max_dist is None else self.max_dist
-        self._nrow = int(np.maximum(self._diag/self.min_dist, np.sqrt(self.n_turbines)+0.5)) + 3
-        
+        self._nrow = (
+            int(np.maximum(self._diag / self.min_dist, np.sqrt(self.n_turbines) + 0.5))
+            + 3
+        )
+
         if verbosity > 0:
             print(f"Grid data:")
             print(f"  pmin        = {pmin}")
             print(f"  pmax        = {pmax}")
             print(f"  min dist    = {self.min_dist}")
             print(f"  max dist    = {self.max_dist}")
             print(f"  n row max   = {self._nrow}")
@@ -98,16 +102,15 @@
 
         Returns
         -------
         names : list of str
             The names of the float variables
 
         """
-        return list(np.array(
-            [self._SX, self._SY, self._DX, self._DY, self._ALPHA]))
+        return list(np.array([self._SX, self._SY, self._DX, self._DY, self._ALPHA]))
 
     def initial_values_float(self):
         """
         The initial values of the float variables.
 
         Returns
         -------
@@ -147,15 +150,15 @@
         values : numpy.ndarray
             Maximal float values, shape: (n_vars_float,)
 
         """
         vals = np.zeros(5, dtype=FC.DTYPE)
         vals[:2] = 0.5
         vals[2:4] = self.max_dist
-        vals[4] = 90.
+        vals[4] = 90.0
         return vals
 
     def apply_individual(self, vars_int, vars_float):
         """
         Apply new variables to the problem.
 
         Parameters
@@ -167,41 +170,44 @@
 
         Returns
         -------
         problem_results : Any
             The results of the variable application
             to the problem
 
-        """       
+        """
         sx, sy, dx, dy, alpha = vars_float
 
         a = np.deg2rad(alpha)
         nax = np.stack([np.cos(a), np.sin(a)], axis=-1)
         nay = np.stack([-np.sin(a), np.cos(a)], axis=-1)
 
         pts = (
-            self._pc[None, None, :] +
-            (np.arange(self._nrow)[:, None, None] - (self._nrow-1)/2 + sx)*dx*nax[None, None, :] +
-            (np.arange(self._nrow)[None, :, None] - (self._nrow-1)/2 + sy)*dy*nay[None, None, :]
+            self._pc[None, None, :]
+            + (np.arange(self._nrow)[:, None, None] - (self._nrow - 1) / 2 + sx)
+            * dx
+            * nax[None, None, :]
+            + (np.arange(self._nrow)[None, :, None] - (self._nrow - 1) / 2 + sy)
+            * dy
+            * nay[None, None, :]
         )
         pts = pts.reshape(self._nrow**2, 2)
 
         if self.D is None:
             valid = self.boundary.points_inside(pts)
         else:
-            valid= (
-                self.boundary.points_inside(pts) &
-                (self.boundary.points_distance(pts) >= self.D / 2)
+            valid = self.boundary.points_inside(pts) & (
+                self.boundary.points_distance(pts) >= self.D / 2
             )
 
         nvl = np.sum(valid)
         if nvl >= self.n_turbines:
-            return pts[valid][:self.n_turbines], np.ones(self.n_turbines, dtype=bool)
+            return pts[valid][: self.n_turbines], np.ones(self.n_turbines, dtype=bool)
         else:
-            qts = np.append(pts[valid], pts[~valid][:(self.n_turbines-nvl)], axis=0)
+            qts = np.append(pts[valid], pts[~valid][: (self.n_turbines - nvl)], axis=0)
             vld = np.zeros(self.n_turbines, dtype=bool)
             vld[:nvl] = True
             return qts, vld
 
     def apply_population(self, vars_int, vars_float):
         """
         Apply new variables to the problem,
@@ -223,50 +229,67 @@
         """
         n_pop = vars_float.shape[0]
         sx = vars_float[:, 0]
         sy = vars_float[:, 1]
         dx = vars_float[:, 2]
         dy = vars_float[:, 3]
         alpha = vars_float[:, 4]
-        
+
         a = np.deg2rad(alpha)
         nax = np.stack([np.cos(a), np.sin(a)], axis=-1)
         nay = np.stack([-np.sin(a), np.cos(a)], axis=-1)
 
         pts = (
-            self._pc[None, None, None, :] +
-            (np.arange(self._nrow)[None, :, None, None] - (self._nrow-1)/2 + sx[:, None, None, None])*dx[:, None, None, None]*nax[:, None, None, :] +
-            (np.arange(self._nrow)[None, None, :, None] - (self._nrow-1)/2 + sy[:, None, None, None])*dy[:, None, None, None]*nay[:, None, None, :]
+            self._pc[None, None, None, :]
+            + (
+                np.arange(self._nrow)[None, :, None, None]
+                - (self._nrow - 1) / 2
+                + sx[:, None, None, None]
+            )
+            * dx[:, None, None, None]
+            * nax[:, None, None, :]
+            + (
+                np.arange(self._nrow)[None, None, :, None]
+                - (self._nrow - 1) / 2
+                + sy[:, None, None, None]
+            )
+            * dy[:, None, None, None]
+            * nay[:, None, None, :]
         )
-        pts = pts.reshape(n_pop*self._nrow**2, 2)
+        pts = pts.reshape(n_pop * self._nrow**2, 2)
 
         if self.D is None:
             valid = self.boundary.points_inside(pts)
         else:
-            valid= (
-                self.boundary.points_inside(pts) &
-                (self.boundary.points_distance(pts) >= self.D / 2)
+            valid = self.boundary.points_inside(pts) & (
+                self.boundary.points_distance(pts) >= self.D / 2
             )
         valid = valid.reshape(n_pop, self._nrow**2)
         pts = pts.reshape(n_pop, self._nrow**2, 2)
 
         nvl = np.sum(valid, axis=1)
         qts = np.zeros((n_pop, self.n_turbines, 2), dtype=FC.DTYPE)
         vld = np.zeros((n_pop, self.n_turbines), dtype=bool)
         for pi in range(n_pop):
             if nvl[pi] >= self.n_turbines:
-                qts[pi] = pts[pi, valid[pi]][:self.n_turbines]
+                qts[pi] = pts[pi, valid[pi]][: self.n_turbines]
                 vld[pi] = np.ones(self.n_turbines, dtype=bool)
             else:
-                qts[pi] = np.append(pts[pi, valid[pi]], pts[pi, ~valid[pi]][:(self.n_turbines-nvl[pi])], axis=0)
-                vld[pi, :nvl[pi]] = True
+                qts[pi] = np.append(
+                    pts[pi, valid[pi]],
+                    pts[pi, ~valid[pi]][: (self.n_turbines - nvl[pi])],
+                    axis=0,
+                )
+                vld[pi, : nvl[pi]] = True
 
         return qts, vld
 
-    def get_fig(self, xy=None, valid=None, ax=None, title=None, true_circle=True, **bargs):
+    def get_fig(
+        self, xy=None, valid=None, ax=None, title=None, true_circle=True, **bargs
+    ):
         """
         Return plotly figure axis.
 
         Parameters
         ----------
         xy : numpy.ndarary, optional
             The xy coordinate array, shape: (n_points, 2)
@@ -276,36 +299,38 @@
             The figure axis
         title : str, optional
             The figure title
         true_circle : bool
             Draw points as circles with diameter self.D
         bars : dict, optional
             The boundary plot arguments
-        
+
         Returns
         -------
         ax : pyplot.Axis
             The figure axis
 
         """
         if ax is None:
             __, ax = plt.subplots()
-        
+
         hbargs = {"fill_mode": "inside_lightgray"}
         hbargs.update(bargs)
         self.boundary.add_to_figure(ax, **hbargs)
 
         if xy is not None:
             if valid is not None:
                 xy = xy[valid]
             if not true_circle or self.D is None:
                 ax.scatter(xy[:, 0], xy[:, 1], color="orange")
             else:
                 for x, y in xy:
-                    ax.add_patch(plt.Circle((x, y), self.D/2, color="blue", fill=True))
+                    ax.add_patch(
+                        plt.Circle((x, y), self.D / 2, color="blue", fill=True)
+                    )
 
         ax.set_aspect("equal", adjustable="box")
         ax.set_xlabel("x [m]")
         ax.set_ylabel("y [m]")
 
         if title is None:
             if xy is None:
```

### Comparing `foxes-0.3.4/foxes/opt/problems/layout/geom_layouts/geom_reggrids.py` & `foxes-0.3.5/foxes/opt/problems/layout/geom_layouts/geom_reggrids.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
 import matplotlib.pyplot as plt
 from scipy.spatial.distance import cdist
 from iwopy import Problem
 
 import foxes.constants as FC
 
+
 class GeomRegGrids(Problem):
     """
     A regular grid within a boundary geometry.
 
     This optimization problem does not involve
     wind farms.
 
@@ -45,23 +46,23 @@
         The maximal distance between points
     D : float
         The diameter of circle fully within boundary
 
     """
 
     def __init__(
-            self, 
-            boundary, 
-            min_dist, 
-            n_grids, 
-            n_max=None,
-            n_row_max=None, 
-            max_dist=None,
-            D=None,
-        ):
+        self,
+        boundary,
+        min_dist,
+        n_grids,
+        n_max=None,
+        n_row_max=None,
+        max_dist=None,
+        D=None,
+    ):
         super().__init__(name="geom_reg_grids")
 
         self.boundary = boundary
         self.n_grids = n_grids
         self.n_max = n_max
         self.n_row_max = n_row_max
         self.min_dist = float(min_dist)
@@ -92,27 +93,27 @@
         pmax = self.boundary.p_max()
         self._span = pmax - pmin
         self._diag = np.linalg.norm(self._span)
         self.max_dist = self._diag if self.max_dist is None else self.max_dist
         self._nrow = self.n_row_max
         if self.n_row_max is None:
             if self.n_max is None:
-                self._nrow = int(self._diag/self.min_dist)
+                self._nrow = int(self._diag / self.min_dist)
                 if self._nrow * self.min_dist < self._diag:
                     self._nrow += 1
                 self._nrow += 1
             else:
                 self._nrow = self.n_max
         if self.n_max is None:
-            self.n_max = self.n_grids*self._nrow**2
+            self.n_max = self.n_grids * self._nrow**2
         elif self.n_max <= self._nrow:
             self._nrow = self.n_max
         self._pmin = pmin - self._diag - self.min_dist
         self._pmax = pmax + self.min_dist
-        
+
         if verbosity > 0:
             print(f"Grid data:")
             print(f"  pmin        = {self._pmin}")
             print(f"  pmax        = {self._pmax}")
             print(f"  min dist    = {self.min_dist}")
             print(f"  max dist    = {self.max_dist}")
             print(f"  n row max   = {self._nrow}")
@@ -139,74 +140,74 @@
 
         Returns
         -------
         values : numpy.ndarray
             Initial int values, shape: (n_vars_int,)
 
         """
-        return np.full(self.n_grids*2, 2, dtype=FC.ITYPE)
+        return np.full(self.n_grids * 2, 2, dtype=FC.ITYPE)
 
     def min_values_int(self):
         """
         The minimal values of the integer variables.
 
         Use -self.INT_INF for unbounded.
 
         Returns
         -------
         values : numpy.ndarray
             Minimal int values, shape: (n_vars_int,)
 
         """
-        return np.ones(self.n_grids*2, dtype=FC.ITYPE)
+        return np.ones(self.n_grids * 2, dtype=FC.ITYPE)
 
     def max_values_int(self):
         """
         The maximal values of the integer variables.
 
         Use self.INT_INF for unbounded.
 
         Returns
         -------
         values : numpy.ndarray
             Maximal int values, shape: (n_vars_int,)
 
         """
-        return np.full(self.n_grids*2, self._nrow, dtype=FC.ITYPE)
+        return np.full(self.n_grids * 2, self._nrow, dtype=FC.ITYPE)
 
     def var_names_float(self):
         """
         The names of float variables.
 
         Returns
         -------
         names : list of str
             The names of the float variables
 
         """
-        return list(np.array(
-            [self._OX, self._OY, self._DX, self._DY, self._ALPHA]
-            ).T.flat)
+        return list(
+            np.array([self._OX, self._OY, self._DX, self._DY, self._ALPHA]).T.flat
+        )
 
     def initial_values_float(self):
         """
         The initial values of the float variables.
 
         Returns
         -------
         values : numpy.ndarray
             Initial float values, shape: (n_vars_float,)
 
         """
         n = 5
         vals = np.zeros((self.n_grids, n), dtype=FC.DTYPE)
-        vals[:, :2] = self._pmin + self._diag + self.min_dist + self._span/2
-        vals[:, 2:4] = 2*self.min_dist
+        vals[:, :2] = self._pmin + self._diag + self.min_dist + self._span / 2
+        vals[:, 2:4] = 2 * self.min_dist
         vals[:, 5:] = 0
-        return vals.reshape(self.n_grids*n)
+        return vals.reshape(self.n_grids * n)
 
     def min_values_float(self):
         """
         The minimal values of the float variables.
 
         Use -numpy.inf for unbounded.
 
@@ -216,16 +217,16 @@
             Minimal float values, shape: (n_vars_float,)
 
         """
         n = 5
         vals = np.zeros((self.n_grids, n), dtype=FC.DTYPE)
         vals[:, :2] = self._pmin
         vals[:, 2:4] = self.min_dist
-        vals[:, 5:] = -self._diag/3
-        return vals.reshape(self.n_grids*n)
+        vals[:, 5:] = -self._diag / 3
+        return vals.reshape(self.n_grids * n)
 
     def max_values_float(self):
         """
         The maximal values of the float variables.
 
         Use numpy.inf for unbounded.
 
@@ -235,17 +236,17 @@
             Maximal float values, shape: (n_vars_float,)
 
         """
         n = 5
         vals = np.zeros((self.n_grids, n), dtype=FC.DTYPE)
         vals[:, :2] = self._pmax
         vals[:, 2:4] = self.max_dist
-        vals[:, 4] = 90.
-        vals[:, 5:] = self._diag/3
-        return vals.reshape(self.n_grids*n)
+        vals[:, 4] = 90.0
+        vals[:, 5:] = self._diag / 3
+        return vals.reshape(self.n_grids * n)
 
     def apply_individual(self, vars_int, vars_float):
         """
         Apply new variables to the problem.
 
         Parameters
         ----------
@@ -256,15 +257,15 @@
 
         Returns
         -------
         problem_results : Any
             The results of the variable application
             to the problem
 
-        """       
+        """
         vint = vars_int.reshape(self.n_grids, 2)
         vflt = vars_float.reshape(self.n_grids, 5)
         nx = vint[:, 0]
         ny = vint[:, 1]
         ox = vflt[:, 0]
         oy = vflt[:, 1]
         dx = vflt[:, 2]
@@ -278,41 +279,43 @@
         naz[:, 2] = 1
         nay = np.cross(naz, nax)
 
         valid = np.zeros(n_points, dtype=bool)
         pts = np.full((n_points, 2), np.nan, dtype=FC.DTYPE)
         n0 = 0
         for gi in range(self.n_grids):
-
             n = nx[gi] * ny[gi]
             n1 = n0 + n
 
             if n1 <= n_points:
                 qts = pts[n0:n1].reshape(nx[gi], ny[gi], 2)
             else:
                 qts = np.zeros((nx[gi], ny[gi], 2), dtype=FC.DTYPE)
 
             qts[:, :, 0] = ox[gi]
             qts[:, :, 1] = oy[gi]
-            qts[:] += np.arange(nx[gi])[:, None, None] * dx[gi] * nax[gi, None, None, :2]
-            qts[:] += np.arange(ny[gi])[None, :, None] * dy[gi] * nay[gi, None, None, :2]
+            qts[:] += (
+                np.arange(nx[gi])[:, None, None] * dx[gi] * nax[gi, None, None, :2]
+            )
+            qts[:] += (
+                np.arange(ny[gi])[None, :, None] * dy[gi] * nay[gi, None, None, :2]
+            )
             qts = qts.reshape(n, 2)
 
             if n1 > n_points:
                 n1 = n_points
-                qts = qts[:(n1-n0)]
+                qts = qts[: (n1 - n0)]
                 pts[n0:] = qts
 
             # set out of boundary points invalid:
             if self.D is None:
                 valid[n0:n1] = self.boundary.points_inside(qts)
             else:
-                valid[n0:n1] = (
-                    self.boundary.points_inside(qts) &
-                    (self.boundary.points_distance(qts) >= self.D / 2)
+                valid[n0:n1] = self.boundary.points_inside(qts) & (
+                    self.boundary.points_distance(qts) >= self.D / 2
                 )
 
             # set points invalid which are too close to other grids:
             if n0 > 0:
                 dists = cdist(qts, pts[:n0])
                 valid[n0:n1][np.any(dists < self.min_dist, axis=1)] = False
 
@@ -360,56 +363,64 @@
         nay = np.cross(naz, nax)
 
         valid = np.zeros((n_pop, n_points), dtype=bool)
         pts = np.full((n_pop, n_points, 2), np.nan, dtype=FC.DTYPE)
         for pi in range(n_pop):
             n0 = 0
             for gi in range(self.n_grids):
-
                 n = nx[pi, gi] * ny[pi, gi]
                 n1 = n0 + n
 
                 if n1 <= n_points:
                     qts = pts[pi, n0:n1].reshape(nx[pi, gi], ny[pi, gi], 2)
                 else:
                     qts = np.zeros((nx[pi, gi], ny[pi, gi], 2), dtype=FC.DTYPE)
 
                 qts[:, :, 0] = ox[pi, gi]
                 qts[:, :, 1] = oy[pi, gi]
-                qts[:] += np.arange(nx[pi, gi])[:, None, None] * dx[pi, gi] * nax[pi, gi, None, None, :2]
-                qts[:] += np.arange(ny[pi, gi])[None, :, None] * dy[pi, gi] * nay[pi, gi, None, None, :2]
+                qts[:] += (
+                    np.arange(nx[pi, gi])[:, None, None]
+                    * dx[pi, gi]
+                    * nax[pi, gi, None, None, :2]
+                )
+                qts[:] += (
+                    np.arange(ny[pi, gi])[None, :, None]
+                    * dy[pi, gi]
+                    * nay[pi, gi, None, None, :2]
+                )
                 qts = qts.reshape(n, 2)
 
                 if n1 > n_points:
                     n1 = n_points
-                    qts = qts[:(n1-n0)]
+                    qts = qts[: (n1 - n0)]
                     pts[pi, n0:] = qts
 
                 # set out of boundary points invalid:
                 if self.D is None:
                     valid[pi, n0:n1] = self.boundary.points_inside(qts)
                 else:
-                    valid[pi, n0:n1] = (
-                        self.boundary.points_inside(qts) &
-                        (self.boundary.points_distance(qts) >= self.D / 2)
+                    valid[pi, n0:n1] = self.boundary.points_inside(qts) & (
+                        self.boundary.points_distance(qts) >= self.D / 2
                     )
 
                 # set points invalid which are too close to other grids:
                 if n0 > 0:
                     dists = cdist(qts, pts[pi, :n0])
                     valid[pi, n0:n1][np.any(dists < self.min_dist, axis=1)] = False
 
                 n0 = n1
 
                 if n0 >= n_points:
                     break
 
         return pts, valid
 
-    def get_fig(self, xy=None, valid=None, ax=None, title=None, true_circle=True, **bargs):
+    def get_fig(
+        self, xy=None, valid=None, ax=None, title=None, true_circle=True, **bargs
+    ):
         """
         Return plotly figure axis.
 
         Parameters
         ----------
         xy : numpy.ndarary, optional
             The xy coordinate array, shape: (n_points, 2)
@@ -419,36 +430,38 @@
             The figure axis
         title : str, optional
             The figure title
         true_circle : bool
             Draw points as circles with diameter self.D
         bars : dict, optional
             The boundary plot arguments
-        
+
         Returns
         -------
         ax : pyplot.Axis
             The figure axis
 
         """
         if ax is None:
             __, ax = plt.subplots()
-        
+
         hbargs = {"fill_mode": "inside_lightgray"}
         hbargs.update(bargs)
         self.boundary.add_to_figure(ax, **hbargs)
 
         if xy is not None:
             if valid is not None:
                 xy = xy[valid]
             if not true_circle or self.D is None:
                 ax.scatter(xy[:, 0], xy[:, 1], color="orange")
             else:
                 for x, y in xy:
-                    ax.add_patch(plt.Circle((x, y), self.D/2, color="blue", fill=True))
+                    ax.add_patch(
+                        plt.Circle((x, y), self.D / 2, color="blue", fill=True)
+                    )
 
         ax.set_aspect("equal", adjustable="box")
         ax.set_xlabel("x [m]")
         ax.set_ylabel("y [m]")
 
         if title is None:
             if xy is None:
```

### Comparing `foxes-0.3.4/foxes/opt/problems/layout/geom_layouts/objectives.py` & `foxes-0.3.5/foxes/opt/problems/layout/geom_layouts/objectives.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 import numpy as np
 from iwopy import Objective
 from scipy.spatial.distance import cdist
 
 import foxes.constants as FC
 
-class OMaxN(Objective):
 
+class OMaxN(Objective):
     def __init__(self, problem, name="maxN"):
-        super().__init__(problem, name, vnames_int=problem.var_names_int(), 
-            vnames_float=problem.var_names_float())
+        super().__init__(
+            problem,
+            name,
+            vnames_int=problem.var_names_int(),
+            vnames_float=problem.var_names_float(),
+        )
 
     def n_components(self):
         return 1
 
     def maximize(self):
         return [True]
 
@@ -20,27 +24,31 @@
         __, valid = problem_results
         return np.sum(valid)
 
     def calc_population(self, vars_int, vars_float, problem_results, cmpnts=None):
         __, valid = problem_results
         return np.sum(valid, axis=1)[:, None]
 
-class OMinN(OMaxN):
 
+class OMinN(OMaxN):
     def __init__(self, problem, name="ominN"):
         super().__init__(problem, name)
 
     def maximize(self):
         return [False]
 
-class OFixN(Objective):
 
+class OFixN(Objective):
     def __init__(self, problem, N, name="ofixN"):
-        super().__init__(problem, name, vnames_int=problem.var_names_int(), 
-            vnames_float=problem.var_names_float())
+        super().__init__(
+            problem,
+            name,
+            vnames_int=problem.var_names_int(),
+            vnames_float=problem.var_names_float(),
+        )
         self.N = N
 
     def n_components(self):
         return 1
 
     def maximize(self):
         return [False]
@@ -51,19 +59,23 @@
         return np.maximum(N - self.N, self.N - N)
 
     def calc_population(self, vars_int, vars_float, problem_results, cmpnts=None):
         __, valid = problem_results
         N = np.sum(valid, axis=1, dtype=np.float64)[:, None]
         return np.maximum(N - self.N, self.N - N)
 
-class MaxGridSpacing(Objective):
 
+class MaxGridSpacing(Objective):
     def __init__(self, problem, name="max_dxdy"):
-        super().__init__(problem, name, vnames_int=problem.var_names_int(), 
-            vnames_float=problem.var_names_float())
+        super().__init__(
+            problem,
+            name,
+            vnames_int=problem.var_names_int(),
+            vnames_float=problem.var_names_float(),
+        )
 
     def n_components(self):
         return 1
 
     def maximize(self):
         return [True]
 
@@ -74,45 +86,50 @@
 
     def calc_population(self, vars_int, vars_float, problem_results, cmpnts=None):
         n_pop = vars_float.shape[0]
         vflt = vars_float.reshape(n_pop, self.problem.n_grids, 5)
         delta = np.minimum(vflt[:, :, 2], vflt[:, :, 3])
         return np.nanmin(delta, axis=1)[:, None]
 
-class MaxDensity(Objective):
 
+class MaxDensity(Objective):
     def __init__(self, problem, dfactor=1, min_dist=None, name="max_density"):
-        super().__init__(problem, name, vnames_int=problem.var_names_int(), 
-            vnames_float=problem.var_names_float())
+        super().__init__(
+            problem,
+            name,
+            vnames_int=problem.var_names_int(),
+            vnames_float=problem.var_names_float(),
+        )
         self.dfactor = dfactor
         self.min_dist = problem.min_dist if min_dist is None else min_dist
 
     def n_components(self):
         return 1
 
     def maximize(self):
         return [False]
-    
+
     def initialize(self, verbosity):
         super().initialize(verbosity)
-        
+
         # define regular grid of probe points:
         geom = self.problem.boundary
         pmin = geom.p_min()
         pmax = geom.p_max()
         detlta = self.min_dist / self.dfactor
         self._probes = np.stack(
             np.meshgrid(
-                np.arange(pmin[0]-detlta, pmax[0]+2*detlta, detlta),
-                np.arange(pmin[1]-detlta, pmax[1]+2*detlta, detlta),
-                indexing='ij'
-            ), axis=-1
+                np.arange(pmin[0] - detlta, pmax[0] + 2 * detlta, detlta),
+                np.arange(pmin[1] - detlta, pmax[1] + 2 * detlta, detlta),
+                indexing="ij",
+            ),
+            axis=-1,
         )
         nx, ny = self._probes.shape[:2]
-        n = nx*ny
+        n = nx * ny
         self._probes = self._probes.reshape(n, 2)
 
         # reduce to points within geometry:
         valid = geom.points_inside(self._probes)
         self._probes = self._probes[valid]
 
     def calc_individual(self, vars_int, vars_float, problem_results, cmpnts=None):
@@ -128,59 +145,66 @@
         for pi in range(n_pop):
             if np.any(valid[pi]):
                 hxy = xy[pi][valid[pi]]
                 dists = cdist(self._probes, hxy)
                 out[pi] = np.nanmax(np.nanmin(dists, axis=1))
         return out[:, None]
 
-class MeMiMaDist(Objective):
 
-    def __init__(self, problem, scale=500., c1=1, c2=1, c3=1, name="MiMaMean"):
-        super().__init__(problem, name, vnames_int=problem.var_names_int(), 
-            vnames_float=problem.var_names_float())
+class MeMiMaDist(Objective):
+    def __init__(self, problem, scale=500.0, c1=1, c2=1, c3=1, name="MiMaMean"):
+        super().__init__(
+            problem,
+            name,
+            vnames_int=problem.var_names_int(),
+            vnames_float=problem.var_names_float(),
+        )
         self.scale = scale
         self.c1 = c1
         self.c2 = c2
         self.c3 = c3
 
     def n_components(self):
         return 1
 
     def maximize(self):
         return [True]
 
     def calc_individual(self, vars_int, vars_float, problem_results, cmpnts=None):
-
         xy, valid = problem_results
-        #xy = xy[valid]
-        
+        # xy = xy[valid]
+
         dists = cdist(xy, xy)
         np.fill_diagonal(dists, np.inf)
         dists = np.min(dists, axis=1) / self.scale / len(xy)
 
         mean = np.average(dists)
-        mi   = np.min(dists)
-        ma   = np.max(dists)
+        mi = np.min(dists)
+        ma = np.max(dists)
         return np.atleast_1d(
-            self.c1*mean**2 - self.c2*( mean - mi )**2 - self.c3*( mean - ma )**2)
+            self.c1 * mean**2
+            - self.c2 * (mean - mi) ** 2
+            - self.c3 * (mean - ma) ** 2
+        )
 
     def calc_population(self, vars_int, vars_float, problem_results, cmpnts=None):
-
         xy, valid = problem_results
         n_pop, n_xy = xy.shape[:2]
-        
+
         out = np.zeros((n_pop, 1), dtype=FC.DTYPE)
         for pi in range(n_pop):
+            hxy = xy[pi]  # , valid[pi]]
 
-            hxy = xy[pi]#, valid[pi]]
-            
             dists = cdist(hxy, hxy)
             np.fill_diagonal(dists, np.inf)
             dists = np.min(dists, axis=1) / self.scale / n_xy
-            
-            mean       = np.average(dists)
-            mi         = np.min(dists)
-            ma         = np.max(dists)
-            out[pi, 0] = self.c1*mean**2 - self.c2*( mean - mi )**2 - self.c3*( mean - ma )**2
+
+            mean = np.average(dists)
+            mi = np.min(dists)
+            ma = np.max(dists)
+            out[pi, 0] = (
+                self.c1 * mean**2
+                - self.c2 * (mean - mi) ** 2
+                - self.c3 * (mean - ma) ** 2
+            )
 
         return out
-
```

### Comparing `foxes-0.3.4/foxes/opt/problems/layout/reggrids_layout.py` & `foxes-0.3.5/foxes/opt/problems/layout/reggrids_layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,44 +38,49 @@
     Attributes
     ----------
     min_spacing : float
         The minimal turbine spacing
     n_grids : int
         The number of grids
     max_n_row : int
-        The maximal number of turbines per 
+        The maximal number of turbines per
         grid and row
 
     """
 
     def __init__(
         self,
         name,
         algo,
-        min_dist, 
-        n_grids=1, 
-        n_row_max=None, 
+        min_dist,
+        n_grids=1,
+        n_row_max=None,
         max_dist=None,
         runner=None,
         **kwargs,
     ):
         super().__init__(name, algo, runner, **kwargs)
 
         b = algo.farm.boundary
         assert b is not None, f"Problem '{self.name}': Missing wind farm boundary."
-        
-        self._geomp = GeomRegGrids(b, min_dist=min_dist, n_grids=n_grids,
-            n_row_max=n_row_max, max_dist=max_dist)
+
+        self._geomp = GeomRegGrids(
+            b,
+            min_dist=min_dist,
+            n_grids=n_grids,
+            n_row_max=n_row_max,
+            max_dist=max_dist,
+        )
 
     def initialize(self, verbosity=1, **kwargs):
         """
         Initialize the object.
 
         Parameters
-        ---------- 
+        ----------
         verbosity : int
             The verbosity level, 0 = silent
         kwargs : dict, optional
             Additional parameters for super class init
 
         """
         self._geomp.objs = self.objs
@@ -85,24 +90,25 @@
         self._mname = self.name + "_calc"
         for t in self.algo.farm.turbines:
             if self._mname not in t.models:
                 t.models.append(self._mname)
         self._turbine = deepcopy(self.farm.turbines[-1])
 
         self.algo.mbook.turbine_models[self._mname] = Calculator(
-            in_vars=[FV.VALID, FV.P, FV.CT],
-            out_vars=[FV.VALID, FV.P, FV.CT],
-            func=lambda valid, P, ct, st_sel: (valid, P*valid, ct*valid),
-            pre_rotor=False)
+            in_vars=[FC.VALID, FV.P, FV.CT],
+            out_vars=[FC.VALID, FV.P, FV.CT],
+            func=lambda valid, P, ct, st_sel: (valid, P * valid, ct * valid),
+            pre_rotor=False,
+        )
 
         super().initialize(
-            pre_rotor_vars=[FV.X, FV.Y, FV.VALID],
+            pre_rotor_vars=[FV.X, FV.Y, FC.VALID],
             post_rotor_vars=[],
             verbosity=verbosity,
-            **kwargs
+            **kwargs,
         )
 
     def var_names_int(self):
         """
         The names of int variables.
 
         Returns
@@ -205,16 +211,16 @@
         """
         return self._geomp.max_values_float()
 
     def update_problem_individual(self, vars_int, vars_float):
         """
         Update the algo and other data using
         the latest optimization variables.
-        
-        This function is called before running the farm 
+
+        This function is called before running the farm
         calculation.
 
         Parameters
         ----------
         vars_int : np.array
             The integer variable values, shape: (n_vars_int,)
         vars_float : np.array
@@ -229,23 +235,23 @@
         elif n0 < n:
             for i in range(n0, n):
                 self.farm.turbines.append(deepcopy(self._turbine))
                 self.farm.turbines[-1].index = n0 + i
                 self.farm.turbines[-1].name = f"T{n0 + i}"
         if n != n0:
             self.algo.update_n_turbines()
-        
+
         super().update_problem_individual(vars_int, vars_float)
 
     def update_problem_population(self, vars_int, vars_float):
         """
         Update the algo and other data using
         the latest optimization variables.
-        
-        This function is called before running the farm 
+
+        This function is called before running the farm
         calculation.
 
         Parameters
         ----------
         vars_int : np.array
             The integer variable values, shape: (n_pop, n_vars_int,)
         vars_float : np.array
@@ -261,15 +267,15 @@
         elif n0 < n:
             for i in range(n0, n):
                 self.farm.turbines.append(deepcopy(self._turbine))
                 self.farm.turbines[-1].index = n0 + i
                 self.farm.turbines[-1].name = f"T{n0 + i}"
         if n != n0:
             self.algo.update_n_turbines()
-        
+
         super().update_problem_population(vars_int, vars_float)
 
     def opt2farm_vars_individual(self, vars_int, vars_float):
         """
         Translates optimization variables to farm variables
 
         Parameters
@@ -290,33 +296,29 @@
 
         """
         pts, vld = self._geomp.apply_individual(vars_int, vars_float)
 
         n_pts = pts.shape[0]
         n_states = self.algo.n_states
         n_turbines = self.farm.n_turbines
-        
+
         pmi = np.min(self._geomp._pmin)
         points = np.full((n_states, n_turbines, 2), pmi, dtype=FC.DTYPE)
         if n_pts <= n_turbines:
             points[:, :n_pts] = pts[None, :, :]
         else:
             points[:] = pts[None, :n_turbines, :]
 
         valid = np.zeros((n_states, n_turbines), dtype=FC.DTYPE)
         if n_pts <= n_turbines:
             valid[:, :n_pts] = vld[None, :]
         else:
             valid[:] = vld[None, :n_turbines]
 
-        farm_vars = {
-            FV.X: points[:, :, 0],
-            FV.Y: points[:, :, 1],
-            FV.VALID: valid
-        }
+        farm_vars = {FV.X: points[:, :, 0], FV.Y: points[:, :, 1], FC.VALID: valid}
 
         return farm_vars
 
     def opt2farm_vars_population(self, vars_int, vars_float, n_states):
         """
         Translates optimization variables to farm variables
 
@@ -357,15 +359,15 @@
             valid[:, :, :n_pts] = vld[:, None, :]
         else:
             valid[:] = vld[:, None, :n_turbines]
 
         farm_vars = {
             FV.X: points[:, :, :, 0],
             FV.Y: points[:, :, :, 1],
-            FV.VALID: valid
+            FC.VALID: valid,
         }
 
         return farm_vars
 
     def finalize_individual(self, vars_int, vars_float, verbosity=1):
         """
         Finalization, given the champion data.
@@ -395,11 +397,15 @@
         n_xy = xy.shape[0]
 
         self.farm.turbines = self.farm.turbines[:n_xy]
         for ti, t in enumerate(self.farm.turbines):
             t.xy = xy[ti]
             t.index = ti
             t.name = f"T{ti}"
-            t.models = [mname for mname in t.models if mname not in [self.name, self._mname]]
+            t.models = [
+                mname for mname in t.models if mname not in [self.name, self._mname]
+            ]
         self.algo.update_n_turbines()
 
-        return FarmOptProblem.finalize_individual(self, vars_int, vars_float, verbosity=1)
+        return FarmOptProblem.finalize_individual(
+            self, vars_int, vars_float, verbosity=1
+        )
```

### Comparing `foxes-0.3.4/foxes/opt/problems/layout/regular_layout.py` & `foxes-0.3.5/foxes/opt/problems/layout/regular_layout.py`

 * *Files 9% similar despite different names*

```diff
@@ -47,46 +47,47 @@
         self.min_spacing = min_spacing
 
     def initialize(self, verbosity=1, **kwargs):
         """
         Initialize the object.
 
         Parameters
-        ----------  
+        ----------
         verbosity : int
             The verbosity level, 0 = silent
         kwargs : dict, optional
             Additional parameters for super class init
 
         """
         self._mname = self.name + "_calc"
         for t in self.algo.farm.turbines:
             if self._mname not in t.models:
                 t.models.append(self._mname)
         self._turbine = deepcopy(self.farm.turbines[-1])
 
         self.algo.mbook.turbine_models[self._mname] = Calculator(
-            in_vars=[FV.VALID, FV.P, FV.CT],
-            out_vars=[FV.VALID, FV.P, FV.CT],
-            func=lambda valid, P, ct, st_sel: (valid, P*valid, ct*valid),
-            pre_rotor=False)
+            in_vars=[FC.VALID, FV.P, FV.CT],
+            out_vars=[FC.VALID, FV.P, FV.CT],
+            func=lambda valid, P, ct, st_sel: (valid, P * valid, ct * valid),
+            pre_rotor=False,
+        )
 
         b = self.farm.boundary
         assert b is not None, f"Problem '{self.name}': Missing wind farm boundary."
         pmax = b.p_max()
         pmin = b.p_min()
         self._pmin = pmin
-        self._xy0 = 0.5*(pmin+pmax)
-        self._halfspan = (pmax - pmin)/2
+        self._xy0 = 0.5 * (pmin + pmax)
+        self._halfspan = (pmax - pmin) / 2
         self._halflen = np.linalg.norm(self._halfspan)
-        self.max_spacing = 2*(self._halflen + self.min_spacing)
-        self._halfn = int(self._halflen/self.min_spacing)
+        self.max_spacing = 2 * (self._halflen + self.min_spacing)
+        self._halfn = int(self._halflen / self.min_spacing)
         if self._halfn * self.min_spacing < self._halflen:
             self._halfn += 1
-        self._nrow = 2*self._halfn+1
+        self._nrow = 2 * self._halfn + 1
         self._nturb = self._nrow**2
 
         if verbosity > 0:
             print(f"Problem '{self.name}':")
             print(f"  xy0          = {self._xy0}")
             print(f"  span         = {np.linalg.norm(self._halfspan*2):.2f}")
             print(f"  min spacing  = {self.min_spacing:.2f}")
@@ -98,94 +99,94 @@
         if self.farm.n_turbines < self._nturb:
             for i in range(self._nturb - self.farm.n_turbines):
                 ti = len(self.farm.turbines)
                 self.farm.turbines.append(deepcopy(self._turbine))
                 self.farm.turbines[-1].index = ti
                 self.farm.turbines[-1].name = f"T{ti}"
         elif self.farm.n_turbines > self._nturb:
-            self.farm.turbines = self.farm.turbines[:self._nturb]
+            self.farm.turbines = self.farm.turbines[: self._nturb]
         self.algo.n_turbines = self._nturb
 
         super().initialize(
-            pre_rotor_vars=[FV.X, FV.Y, FV.VALID],
+            pre_rotor_vars=[FV.X, FV.Y, FC.VALID],
             post_rotor_vars=[],
-            drop_vars=[FV.STATE, FV.TURBINE],
+            drop_vars=[FC.STATE, FC.TURBINE],
             verbosity=verbosity,
-            **kwargs
+            **kwargs,
         )
 
     def var_names_float(self):
         """
         The names of float variables.
 
         Returns
         -------
         names : list of str
             The names of the float variables
 
         """
         return [
-            self.SPACING_X, 
-            self.SPACING_Y, 
+            self.SPACING_X,
+            self.SPACING_Y,
             self.OFFSET_X,
             self.OFFSET_Y,
-            self.ANGLE]
+            self.ANGLE,
+        ]
 
     def initial_values_float(self):
         """
         The initial values of the float variables.
 
         Returns
         -------
         values : numpy.ndarray
             Initial float values, shape: (n_vars_float,)
 
         """
-        return [
-            self.min_spacing, 
-            self.min_spacing, 
-            0., 0., 0.]
+        return [self.min_spacing, self.min_spacing, 0.0, 0.0, 0.0]
 
     def min_values_float(self):
         """
         The minimal values of the float variables.
 
         Use -numpy.inf for unbounded.
 
         Returns
         -------
         values : numpy.ndarray
             Minimal float values, shape: (n_vars_float,)
 
         """
         return [
-            self.min_spacing, 
-            self.min_spacing, 
-            -self._halfspan[0] - self.min_spacing, 
-            -self._halfspan[1] - self.min_spacing, 
-            0.]
+            self.min_spacing,
+            self.min_spacing,
+            -self._halfspan[0] - self.min_spacing,
+            -self._halfspan[1] - self.min_spacing,
+            0.0,
+        ]
 
     def max_values_float(self):
         """
         The maximal values of the float variables.
 
         Use numpy.inf for unbounded.
 
         Returns
         -------
         values : numpy.ndarray
             Maximal float values, shape: (n_vars_float,)
 
         """
         return [
-                self.max_spacing, 
-                self.max_spacing, 
-                self._halfspan[0] + self.min_spacing,
-                self._halfspan[1] + self.min_spacing,
-                90.]
+            self.max_spacing,
+            self.max_spacing,
+            self._halfspan[0] + self.min_spacing,
+            self._halfspan[1] + self.min_spacing,
+            90.0,
+        ]
 
     def opt2farm_vars_individual(self, vars_int, vars_float):
         """
         Translates optimization variables to farm variables
 
         Parameters
         ----------
@@ -205,34 +206,34 @@
 
         """
 
         dx, dy, ox, oy, a = vars_float
         n_states = self.algo.n_states
         nx = self._nrow
         ny = self._nrow
-        
+
         a = np.deg2rad(a)
-        nax = np.array([np.cos(a), np.sin(a), 0.], dtype=FC.DTYPE)
-        nay = np.cross(np.array([0., 0., 1.], dtype=FC.DTYPE), nax)
+        nax = np.array([np.cos(a), np.sin(a), 0.0], dtype=FC.DTYPE)
+        nay = np.cross(np.array([0.0, 0.0, 1.0], dtype=FC.DTYPE), nax)
         x0 = self._xy0 + np.array([ox, oy], dtype=FC.DTYPE)
 
         pts = np.zeros((n_states, nx, ny, 2), dtype=FC.DTYPE)
         pts[:] = (
-            x0[None, None, None, :] 
-            + np.arange(nx)[None, :, None, None] * dx * nax[None, None, None, :2] 
+            x0[None, None, None, :]
+            + np.arange(nx)[None, :, None, None] * dx * nax[None, None, None, :2]
             + np.arange(ny)[None, None, :, None] * dy * nay[None, None, None, :2]
         )
 
-        pts = pts.reshape(n_states, nx*ny, 2)
-        valid = self.farm.boundary.points_inside(pts.reshape(n_states*nx*ny, 2))
+        pts = pts.reshape(n_states, nx * ny, 2)
+        valid = self.farm.boundary.points_inside(pts.reshape(n_states * nx * ny, 2))
 
         farm_vars = {
             FV.X: pts[:, :, 0],
             FV.Y: pts[:, :, 1],
-            FV.VALID: valid.reshape(n_states, nx*ny).astype(FC.DTYPE)
+            FC.VALID: valid.reshape(n_states, nx * ny).astype(FC.DTYPE),
         }
 
         return farm_vars
 
     def opt2farm_vars_population(self, vars_int, vars_float, n_states):
         """
         Translates optimization variables to farm variables
@@ -255,15 +256,15 @@
             value: numpy.ndarray with values, shape:
             (n_pop, n_states, n_sel_turbines)
 
         """
         n_pop = len(vars_float)
         n_turbines = self.farm.n_turbines
         dx = vars_float[:, 0]
-        dy = vars_float[:, 1] 
+        dy = vars_float[:, 1]
         ox = vars_float[:, 2]
         oy = vars_float[:, 3]
         nx = self._nrow
         ny = self._nrow
         a = vars_float[:, 4]
         N = self._nturb
 
@@ -274,30 +275,34 @@
         nay = np.cross(naz, nax)
 
         pts = np.zeros((n_pop, n_states, nx, ny, 2), dtype=FC.DTYPE)
         pts[:] = self._xy0[None, None, None, None, :]
         pts[..., 0] += ox[:, None, None, None]
         pts[..., 1] += oy[:, None, None, None]
         pts[:] += (
-            np.arange(nx)[None, None, :, None, None] * dx[:, None, None, None, None] 
-            * nax[:, None, None, None, :2] 
-            + np.arange(ny)[None, None, None, :, None] * dy[:, None, None, None, None] 
+            np.arange(nx)[None, None, :, None, None]
+            * dx[:, None, None, None, None]
+            * nax[:, None, None, None, :2]
+            + np.arange(ny)[None, None, None, :, None]
+            * dy[:, None, None, None, None]
             * nay[:, None, None, None, :2]
-            )
+        )
 
-        qts = np.zeros((n_pop, n_states, n_turbines, 2)) 
+        qts = np.zeros((n_pop, n_states, n_turbines, 2))
         qts[:, :N] = pts.reshape(n_pop, n_states, N, 2)
         del pts
 
-        valid = self.farm.boundary.points_inside(qts.reshape(n_pop*n_states*n_turbines, 2))
+        valid = self.farm.boundary.points_inside(
+            qts.reshape(n_pop * n_states * n_turbines, 2)
+        )
 
         farm_vars = {
             FV.X: qts[:, :, :, 0],
             FV.Y: qts[:, :, :, 1],
-            FV.VALID: valid.reshape(n_pop, n_states, n_turbines).astype(FC.DTYPE)
+            FC.VALID: valid.reshape(n_pop, n_states, n_turbines).astype(FC.DTYPE),
         }
 
         return farm_vars
 
     def finalize_individual(self, vars_int, vars_float, verbosity=1):
         """
         Finalization, given the champion data.
@@ -319,20 +324,22 @@
         objs : np.array
             The objective function values, shape: (n_objectives,)
         cons : np.array
             The constraints values, shape: (n_constraints,)
 
         """
         farm_vars = self.opt2farm_vars_individual(vars_int, vars_float)
-        sel = np.where(farm_vars[FV.VALID][0])[0]
+        sel = np.where(farm_vars[FC.VALID][0])[0]
         x = farm_vars[FV.X][0, sel]
         y = farm_vars[FV.Y][0, sel]
-        
+
         self.farm.turbines = [t for i, t in enumerate(self.farm.turbines) if i in sel]
         for i, t in enumerate(self.farm.turbines):
             t.xy = np.array([x[i], y[i]], dtype=FC.DTYPE)
             t.models = [m for m in t.models if m not in [self.name, self._mname]]
             t.index = i
             t.name = f"T{i}"
         self.algo.update_n_turbines()
 
-        return FarmOptProblem.finalize_individual(self, vars_int, vars_float, verbosity=1)
+        return FarmOptProblem.finalize_individual(
+            self, vars_int, vars_float, verbosity=1
+        )
```

### Comparing `foxes-0.3.4/foxes/opt/problems/opt_farm_vars.py` & `foxes-0.3.5/foxes/opt/problems/opt_farm_vars.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,43 +2,44 @@
 import pandas as pd
 
 from foxes.opt.core import FarmVarsProblem
 from foxes.models.turbine_models import SetFarmVars
 import foxes.variables as FV
 import foxes.constants as FC
 
+
 class OptFarmVars(FarmVarsProblem):
     """
     Optimize a selection of farm variables.
 
     Parameters
     ----------
     args : tuple, optional
         Arguments for `FarmVarsProblem`
     kwargs : dict, optional
         Keyword arguments for `FarmVarsProblem`
 
     """
-    
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._vars = None
 
     def add_var(
-        self, 
-        name, 
-        typ, 
-        init, 
-        min, 
-        max, 
-        level="uniform", 
+        self,
+        name,
+        typ,
+        init,
+        min,
+        max,
+        level="uniform",
         sel=None,
         pre_rotor=False,
         model_key=None,
-        ):
+    ):
         """
         Add a variable.
 
         Parameters
         ----------
         name : str
             The foxes farm variable name
@@ -49,56 +50,67 @@
         min : float or int
             The min value
         max : float or int
             The max value
         level : str
             Choices: uniform, state, turbine, state-turbine
         sel : numpy.ndarray, optional
-            States/turbines/state-turbine selection, 
+            States/turbines/state-turbine selection,
             depending on the level
         pre_rotor : bool
             Apply this variable before rotor model
         model_key : str, optional
             Creates sub-model which can then be placed in the
             turbine model list. Repeated keys are added to the
             same turbine model
 
         """
         if not hasattr(FV, name):
-            raise ValueError(f"Problem '{self.name}': Name '{name}' is not a foxes variable.")
+            raise ValueError(
+                f"Problem '{self.name}': Name '{name}' is not a foxes variable."
+            )
         if typ is not float and typ is not int:
-            raise TypeError(f"Problem '{self.name}': Expecting float or int, got type '{type(typ).__name__}'")
+            raise TypeError(
+                f"Problem '{self.name}': Expecting float or int, got type '{type(typ).__name__}'"
+            )
 
         mname = self.name if model_key is None else model_key
         if mname in self.algo.mbook.turbine_models:
             m = self.algo.mbook.turbine_models[mname]
             if not isinstance(m, SetFarmVars):
                 raise KeyError(
                     f"Problem '{self.name}': Turbine model entry '{mname}' already exists in model book, and is not of type SetFarmVars"
                 )
             elif m.pre_rotor != pre_rotor:
-                raise ValueError(f"Problem '{self.name}': Turbine model entry '{mname}' exists in model book, and disagrees on pre_rotor = {pre_rotor}")
+                raise ValueError(
+                    f"Problem '{self.name}': Turbine model entry '{mname}' exists in model book, and disagrees on pre_rotor = {pre_rotor}"
+                )
         else:
             self.algo.mbook.turbine_models[mname] = SetFarmVars(pre_rotor=pre_rotor)
 
         if self._vars is None:
-            i0 = 0 
+            i0 = 0
             i0i = 0
             i0f = 0
         else:
             if name in self._vars["var"].tolist():
-                raise ValueError(f"Problem '{self.name}': Attempt to add variable '{name}' twice")
+                raise ValueError(
+                    f"Problem '{self.name}': Attempt to add variable '{name}' twice"
+                )
             i0 = len(self._vars.index)
             grps = self._vars.groupby("type")
             i0i = len(grps.get_group("int").index) if "int" in grps.groups.keys() else 0
-            i0f = len(grps.get_group("float").index) if "float" in grps.groups.keys() else 0
+            i0f = (
+                len(grps.get_group("float").index)
+                if "float" in grps.groups.keys()
+                else 0
+            )
             del grps
 
         if level == "uniform":
-
             hdata = pd.DataFrame(index=[i0])
             hdata.loc[i0, "name"] = name
             hdata.loc[i0, "var"] = name
             hdata.loc[i0, "type"] = "int" if typ is int else "float"
             hdata.loc[i0, "index"] = i0i if typ is int else i0f
             hdata.loc[i0, "level"] = level
             hdata.loc[i0, "state"] = -1
@@ -107,23 +119,22 @@
             hdata.loc[i0, "init"] = np.array([init], dtype=FC.DTYPE)
             hdata.loc[i0, "min"] = np.array([min], dtype=FC.DTYPE)
             hdata.loc[i0, "max"] = np.array([max], dtype=FC.DTYPE)
             hdata.loc[i0, "pre_rotor"] = pre_rotor
             hdata.loc[i0, "model_key"] = mname
 
         elif level == "state":
-
             if not self.algo.initialized:
                 self.algo.initialize()
-                
+
             states = np.arange(self.algo.n_states)
             if sel is not None:
                 states = states[sel]
             inds = i0 + np.arange(len(states))
-            tinds = inds-i0+i0i if typ is int else inds-i0+i0f
+            tinds = inds - i0 + i0i if typ is int else inds - i0 + i0f
 
             hdata = pd.DataFrame(index=inds)
             hdata.loc[inds, "name"] = [f"{name}_{i:05d}" for i in range(len(states))]
             hdata.loc[inds, "var"] = name
             hdata.loc[inds, "type"] = "int" if typ is int else "float"
             hdata.loc[inds, "index"] = tinds
             hdata.loc[inds, "level"] = level
@@ -136,87 +147,93 @@
                 data[:] = d
                 hdata.loc[inds, c] = data
 
             hdata.loc[inds, "pre_rotor"] = pre_rotor
             hdata.loc[inds, "model_key"] = mname
 
         elif level == "turbine":
-
             if sel is None:
                 turbines = self.sel_turbines
             else:
                 turbines = np.arange(self.algo.n_turbines)[sel]
             inds = i0 + np.arange(len(turbines))
-            tinds = inds-i0+i0i if typ is int else inds-i0+i0f
+            tinds = inds - i0 + i0i if typ is int else inds - i0 + i0f
 
             hdata = pd.DataFrame(index=inds)
             hdata.loc[inds, "name"] = [f"{name}_{i:04d}" for i in range(len(turbines))]
             hdata.loc[inds, "var"] = name
             hdata.loc[inds, "type"] = "int" if typ is int else "float"
             hdata.loc[inds, "index"] = tinds
             hdata.loc[inds, "level"] = level
             hdata.loc[inds, "state"] = -1
             hdata.loc[inds, "turbine"] = turbines
-            hdata.loc[inds, "sel_turbine"] = [self.sel_turbines.index(ti) for ti in turbines]
-            
+            hdata.loc[inds, "sel_turbine"] = [
+                self.sel_turbines.index(ti) for ti in turbines
+            ]
+
             for c, d in [("init", init), ("min", min), ("max", max)]:
                 data = np.full(len(inds), np.nan, dtype=FC.DTYPE)
                 data[:] = d
                 hdata.loc[inds, c] = data
 
             hdata.loc[inds, "pre_rotor"] = pre_rotor
             hdata.loc[inds, "model_key"] = mname
 
         elif level == "state-turbine":
-
             if not self.algo.initialized:
                 self.algo.initialize()
 
             n_states = self.algo.n_states
             n_turbines = self.algo.n_turbines
             if sel is None:
                 sel = np.zeros((n_states, n_turbines), dtype=bool)
                 sel[:, self.sel_turbines] = True
             else:
                 sel = np.array(sel, dtype=bool)
-            st = np.arange(n_states*n_turbines).reshape(n_states, n_turbines)[sel]
+            st = np.arange(n_states * n_turbines).reshape(n_states, n_turbines)[sel]
             whr = np.where(sel)
             n_inds = len(st)
             inds = i0 + np.arange(n_inds)
-            tinds = inds-i0+i0i if typ is int else inds-i0+i0f
+            tinds = inds - i0 + i0i if typ is int else inds - i0 + i0f
 
             hdata = pd.DataFrame(index=inds)
-            hdata.loc[inds, "name"] = [f"{name}_{whr[0][i]:05d}_{whr[1][i]:04d}" for i in range(len(st))]
+            hdata.loc[inds, "name"] = [
+                f"{name}_{whr[0][i]:05d}_{whr[1][i]:04d}" for i in range(len(st))
+            ]
             hdata.loc[inds, "var"] = name
             hdata.loc[inds, "type"] = "int" if typ is int else "float"
             hdata.loc[inds, "index"] = tinds
             hdata.loc[inds, "level"] = level
             hdata.loc[inds, "state"] = whr[0]
             hdata.loc[inds, "turbine"] = whr[1]
-            hdata.loc[inds, "sel_turbine"] = [self.sel_turbines.index(ti) for ti in whr[1]]
+            hdata.loc[inds, "sel_turbine"] = [
+                self.sel_turbines.index(ti) for ti in whr[1]
+            ]
 
             for c, d in [("init", init), ("min", min), ("max", max)]:
                 data = np.full(n_inds, np.nan, dtype=FC.DTYPE)
                 if isinstance(d, np.ndarray) and len(d.shape) > 1:
                     data[:] = d[sel]
                 else:
                     data[:] = d
                 hdata.loc[inds, c] = data
 
             hdata.loc[inds, "pre_rotor"] = pre_rotor
             hdata.loc[inds, "model_key"] = mname
 
         else:
-            raise ValueError(f"Problem '{self.name}': Unknown level '{level}'. Choices: uniform, state, turbine, state-turbine")
+            raise ValueError(
+                f"Problem '{self.name}': Unknown level '{level}'. Choices: uniform, state, turbine, state-turbine"
+            )
 
         if self._vars is None:
             self._vars = hdata
         else:
             self._vars = pd.concat([self._vars, hdata], axis=0)
-        
+
         icols = ["index", "state", "turbine", "sel_turbine"]
         for c in icols:
             self._vars[c] = self._vars[c].astype(FC.ITYPE)
 
     def initialize(self, verbosity=1, **kwargs):
         """
         Initialize the object.
@@ -226,53 +243,59 @@
         verbosity : int
             The verbosity level, 0 = silent
         kwargs : dict, optional
             Additional parameters for super class init
 
         """
         if self._vars is None:
-            raise ValueError(f"Problem '{self.name}': No variables added for optimization.")
+            raise ValueError(
+                f"Problem '{self.name}': No variables added for optimization."
+            )
 
         if verbosity > 0:
             print(f"Problem '{self.name}': Optimization variable list")
             print()
             print(self._vars)
             print()
 
         prev = {}
         postv = {}
         for (mname, pre), g in self._vars.groupby(["model_key", "pre_rotor"]):
             if (pre and mname in postv) or (not pre and mname in prev):
-                raise ValueError(f"Problem '{self.name}': Model '{mname}' reveived both pre_rotor and non-pre_rotor variables")
+                raise ValueError(
+                    f"Problem '{self.name}': Model '{mname}' reveived both pre_rotor and non-pre_rotor variables"
+                )
             tg = prev if pre else postv
             if mname not in tg:
                 tg[mname] = set(g["var"].tolist())
             else:
                 tg[mname] = tg[mname].update(g["var"].tolist())
 
         super().initialize(
             pre_rotor_vars={mname: list(vrs) for mname, vrs in prev.items()},
             post_rotor_vars={mname: list(vrs) for mname, vrs in postv.items()},
             verbosity=verbosity,
-            **kwargs
+            **kwargs,
         )
 
     def var_names_int(self):
         """
         The names of int variables.
 
         Returns
         -------
         names : list of str
             The names of the int variables
 
         """
         if self._vars is None:
-            raise ValueError(f"Problem '{self.name}': No variables added for optimization.")
-        
+            raise ValueError(
+                f"Problem '{self.name}': No variables added for optimization."
+            )
+
         grps = self._vars.groupby("type")
         if "int" not in grps.groups.keys():
             return []
         else:
             return grps.get_group("int")["name"].tolist()
 
     def initial_values_int(self):
@@ -282,15 +305,17 @@
         Returns
         -------
         values : numpy.ndarray
             Initial int values, shape: (n_vars_int,)
 
         """
         if self._vars is None:
-            raise ValueError(f"Problem '{self.name}': No variables added for optimization.")
+            raise ValueError(
+                f"Problem '{self.name}': No variables added for optimization."
+            )
 
         grps = self._vars.groupby("type")
         if "int" not in grps.groups.keys():
             return []
         else:
             return grps.get_group("int")["init"].to_numpy(FC.ITYPE)
 
@@ -303,15 +328,17 @@
         Returns
         -------
         values : numpy.ndarray
             Minimal int values, shape: (n_vars_int,)
 
         """
         if self._vars is None:
-            raise ValueError(f"Problem '{self.name}': No variables added for optimization.")
+            raise ValueError(
+                f"Problem '{self.name}': No variables added for optimization."
+            )
 
         grps = self._vars.groupby("type")
         if "int" not in grps.groups.keys():
             return []
         else:
             return grps.get_group("int")["min"].to_numpy(FC.ITYPE)
 
@@ -324,15 +351,17 @@
         Returns
         -------
         values : numpy.ndarray
             Maximal int values, shape: (n_vars_int,)
 
         """
         if self._vars is None:
-            raise ValueError(f"Problem '{self.name}': No variables added for optimization.")
+            raise ValueError(
+                f"Problem '{self.name}': No variables added for optimization."
+            )
 
         grps = self._vars.groupby("type")
         if "int" not in grps.groups.keys():
             return []
         else:
             return grps.get_group("int")["max"].to_numpy(FC.ITYPE)
 
@@ -343,15 +372,17 @@
         Returns
         -------
         names : list of str
             The names of the float variables
 
         """
         if self._vars is None:
-            raise ValueError(f"Problem '{self.name}': No variables added for optimization.")
+            raise ValueError(
+                f"Problem '{self.name}': No variables added for optimization."
+            )
 
         grps = self._vars.groupby("type")
         if "float" not in grps.groups.keys():
             return []
         else:
             return grps.get_group("float")["name"].tolist()
 
@@ -362,15 +393,17 @@
         Returns
         -------
         values : numpy.ndarray
             Initial float values, shape: (n_vars_float,)
 
         """
         if self._vars is None:
-            raise ValueError(f"Problem '{self.name}': No variables added for optimization.")
+            raise ValueError(
+                f"Problem '{self.name}': No variables added for optimization."
+            )
 
         grps = self._vars.groupby("type")
         if "float" not in grps.groups.keys():
             return []
         else:
             return grps.get_group("float")["init"].to_numpy(FC.DTYPE)
 
@@ -383,15 +416,17 @@
         Returns
         -------
         values : numpy.ndarray
             Minimal float values, shape: (n_vars_float,)
 
         """
         if self._vars is None:
-            raise ValueError(f"Problem '{self.name}': No variables added for optimization.")
+            raise ValueError(
+                f"Problem '{self.name}': No variables added for optimization."
+            )
 
         grps = self._vars.groupby("type")
         if "float" not in grps.groups.keys():
             return []
         else:
             return grps.get_group("float")["min"].to_numpy(FC.DTYPE)
 
@@ -404,15 +439,17 @@
         Returns
         -------
         values : numpy.ndarray
             Maximal float values, shape: (n_vars_float,)
 
         """
         if self._vars is None:
-            raise ValueError(f"Problem '{self.name}': No variables added for optimization.")
+            raise ValueError(
+                f"Problem '{self.name}': No variables added for optimization."
+            )
 
         grps = self._vars.groupby("type")
         if "float" not in grps.groups.keys():
             return []
         else:
             return grps.get_group("float")["max"].to_numpy(FC.DTYPE)
 
@@ -439,43 +476,44 @@
         """
         n_states = self.algo.n_states
         n_sturb = self.n_sel_turbines
 
         farm_vars = {}
         grps = self._vars.groupby(["type", "var", "level"])
         for (typ, var, level), g in grps:
-
             src = vars_int if typ == "int" else vars_float
             i0 = g.index[0]
             i1 = g.index[-1]
-            data = src[np.s_[i0:i1+1]]
+            data = src[np.s_[i0 : i1 + 1]]
 
             if level == "uniform":
                 farm_vars[var] = np.full((n_states, n_sturb), data[0], dtype=FC.DTYPE)
-            
+
             elif level == "state":
                 farm_vars[var] = np.full((n_states, n_sturb), np.nan, dtype=FC.DTYPE)
                 if np.all(g["state"] == np.arange(n_states)):
                     farm_vars[var][:] = data[:, None]
                 else:
                     farm_vars[var][g["state"]] = data[:, None]
-            
+
             elif level == "turbine":
                 farm_vars[var] = np.full((n_states, n_sturb), np.nan, dtype=FC.DTYPE)
                 if np.all(g["sel_turbine"] == np.arange(n_sturb)):
                     farm_vars[var][:] = data[None, :]
                 else:
                     farm_vars[var][:, g["sel_turbine"]] = data[None, :]
-            
+
             elif level == "state-turbine":
                 farm_vars[var] = np.full((n_states, n_sturb), np.nan, dtype=FC.DTYPE)
                 farm_vars[var][g["state"], g["sel_turbine"]] = data
-            
+
             else:
-                raise ValueError(f"Problem '{self.name}': Unknown level '{level}' encountered for variable '{var}'. Valid choices: uniform, state, turbine, state-turbine")
+                raise ValueError(
+                    f"Problem '{self.name}': Unknown level '{level}' encountered for variable '{var}'. Valid choices: uniform, state, turbine, state-turbine"
+                )
 
         return farm_vars
 
     def opt2farm_vars_population(self, vars_int, vars_float, n_states):
         """
         Translates optimization variables to farm variables
 
@@ -500,39 +538,48 @@
         """
         n_pop = vars_float.shape[0]
         n_sturb = self.n_sel_turbines
 
         farm_vars = {}
         grps = self._vars.groupby(["type", "var", "level"])
         for (typ, var, level), g in grps:
-
             src = vars_int if typ == "int" else vars_float
             i0 = g.index[0]
             i1 = g.index[-1]
-            data = src[:, np.s_[i0:i1+1]]
+            data = src[:, np.s_[i0 : i1 + 1]]
 
             if level == "uniform":
-                farm_vars[var] = np.full((n_pop, n_states, n_sturb), np.nan, dtype=FC.DTYPE)
+                farm_vars[var] = np.full(
+                    (n_pop, n_states, n_sturb), np.nan, dtype=FC.DTYPE
+                )
                 farm_vars[var][:] = data[:, 0, None, None]
-            
+
             elif level == "state":
-                farm_vars[var] = np.full((n_pop, n_states, n_sturb), np.nan, dtype=FC.DTYPE)
+                farm_vars[var] = np.full(
+                    (n_pop, n_states, n_sturb), np.nan, dtype=FC.DTYPE
+                )
                 if np.all(g["state"] == np.arange(n_states)):
                     farm_vars[var][:] = data[:, :, None]
                 else:
                     farm_vars[var][:, g["state"]] = data[:, :, None]
-            
+
             elif level == "turbine":
-                farm_vars[var] = np.full((n_pop, n_states, n_sturb), np.nan, dtype=FC.DTYPE)
+                farm_vars[var] = np.full(
+                    (n_pop, n_states, n_sturb), np.nan, dtype=FC.DTYPE
+                )
                 if np.all(g["sel_turbine"] == np.arange(n_sturb)):
                     farm_vars[var][:] = data[:, None, :]
                 else:
                     farm_vars[var][:, :, g["sel_turbine"]] = data[:, None, :]
-            
+
             elif level == "state-turbine":
-                farm_vars[var] = np.full((n_pop, n_states, n_sturb), np.nan, dtype=FC.DTYPE)
+                farm_vars[var] = np.full(
+                    (n_pop, n_states, n_sturb), np.nan, dtype=FC.DTYPE
+                )
                 farm_vars[var][:, g["state"], g["sel_turbine"]] = data
-           
+
             else:
-                raise ValueError(f"Problem '{self.name}': Unknown level '{level}' encountered for variable '{var}'. Valid choices: uniform, state, turbine, state-turbine")
+                raise ValueError(
+                    f"Problem '{self.name}': Unknown level '{level}' encountered for variable '{var}'. Valid choices: uniform, state, turbine, state-turbine"
+                )
 
         return farm_vars
```

### Comparing `foxes-0.3.4/foxes/output/farm_layout.py` & `foxes-0.3.5/foxes/output/farm_layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,14 @@
         The rotor diameter, if not from data
 
     """
 
     def __init__(
         self, farm, farm_results=None, from_results=False, results_state=None, D=None
     ):
-
         self.farm = farm
         self.fres = farm_results
         self.from_res = from_results
         self.rstate = results_state
         self.D = D
 
         if from_results and farm_results is None:
@@ -171,19 +170,20 @@
             ax = fig.add_subplot(111)
         else:
             ax = fig.axes[0] if ax is None else ax
 
         D = self.D
         x = None
         if self.farm.n_turbines:
-
             if normalize_D and D is None:
                 if self.from_res:
                     if self.fres[FV.D].min() != self.fres[FV.D].max():
-                        raise ValueError(f"Expecting uniform D, found {self.fres[FV.D]}")
+                        raise ValueError(
+                            f"Expecting uniform D, found {self.fres[FV.D]}"
+                        )
                     D = self.fres[FV.D][0]
                 else:
                     D = None
                     for ti, t in enumerate(self.farm.turbines):
                         hD = t.D
                         if D is None:
                             D = hD
```

### Comparing `foxes-0.3.4/foxes/output/farm_results_eval.py` & `foxes-0.3.5/foxes/output/farm_results_eval.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,14 @@
                 nas = np.zeros_like(fields[-1], dtype=bool)
             nas = nas | np.isnan(fields[-1])
 
         inds = ["st" for v in fields] + ["st"]
         expr = ",".join(inds) + "->" + rhs
 
         if np.any(nas):
-
             sel = ~np.any(nas, axis=1)
             fields = [f[sel] for f in fields]
 
             weights0 = self.results[FV.WEIGHT].to_numpy()
             w0 = np.sum(weights0, axis=0)[None, :]
             weights = weights0[sel]
             w1 = np.sum(weights, axis=0)[None, :]
@@ -95,15 +94,15 @@
 
         Returns
         -------
         data : pandas.DataFrame
             The results per turbine
 
         """
-        n_turbines = self.results.dims[FV.TURBINE]
+        n_turbines = self.results.dims[FC.TURBINE]
 
         rdata = {}
         for v, op in vars_op.items():
             if op == "mean":
                 rdata[v] = self.weinsum("t", v)
             elif op == "sum":
                 vdata = self.results[v].to_numpy()
@@ -119,15 +118,15 @@
                 rdata[v] = np.std(vdata, axis=0)
             else:
                 raise KeyError(
                     f"Unknown operation '{op}' for variable '{v}'. Please choose: sum, mean, min, max"
                 )
 
         data = pd.DataFrame(index=range(n_turbines), data=rdata)
-        data.index.name = FV.TURBINE
+        data.index.name = FC.TURBINE
 
         return data
 
     def reduce_turbines(self, vars_op):
         """
         Reduces the turbine dimension by some operation
 
@@ -140,15 +139,15 @@
 
         Returns
         -------
         data : pandas.DataFrame
             The results per state
 
         """
-        states = self.results.coords[FV.STATE].to_numpy()
+        states = self.results.coords[FC.STATE].to_numpy()
 
         rdata = {}
         for v, op in vars_op.items():
             if op == "mean":
                 rdata[v] = self.weinsum("s", v)
             elif op == "sum":
                 vdata = self.results[v].to_numpy()
@@ -161,15 +160,15 @@
                 rdata[v] = np.max(vdata, axis=1)
             else:
                 raise KeyError(
                     f"Unknown operation '{op}' for variable '{v}'. Please choose: sum, mean, min, max"
                 )
 
         data = pd.DataFrame(index=states, data=rdata)
-        data.index.name = FV.STATE
+        data.index.name = FC.STATE
 
         return data
 
     def reduce_all(self, states_op, turbines_op):
         """
         Reduces states and turbine dimension by some operation
 
@@ -404,20 +403,20 @@
                 [FC.P_UNITS[t.P_unit] for t in algo.farm_controller.turbine_types],
                 dtype=FC.DTYPE,
             )[:, None]
         elif algo is None and P_unit_W is not None:
             pass
         else:
             raise KeyError("Expecting either 'algo' or 'P_unit_W'")
-        
+
         # compute yield per turbine
-        if np.issubdtype(self.results[FV.STATE].dtype, np.datetime64):
+        if np.issubdtype(self.results[FC.STATE].dtype, np.datetime64):
             if hours is not None:
                 raise KeyError("Unexpected parameter 'hours' for timeseries data")
-            times = self.results[FV.STATE].to_numpy()
+            times = self.results[FC.STATE].to_numpy()
             if delta_t is None:
                 delta_t = times[-1] - times[-2]
             duration = times[-1] - times[0] + delta_t
             duration_seconds = np.int64(duration.astype(np.int64) / 1e9)
             duration_hours = duration_seconds / 3600
         elif hours is None and annual == True:
             duration_hours = 8760
```

### Comparing `foxes-0.3.4/foxes/output/flow_plots_2d.py` & `foxes-0.3.5/foxes/output/flow_plots_2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,18 +98,17 @@
 
         hax.autoscale_view()
         hax.set_xlabel(xlabel)
         hax.set_ylabel(ylabel)
         hax.set_title(title if title is not None else f"State {s}")
         hax.set_aspect("equal", adjustable="box")
 
-        
-        if invert_axis == 'x':
+        if invert_axis == "x":
             hax.invert_xaxis()
-        elif invert_axis == 'y':
+        elif invert_axis == "y":
             hax.invert_yaxis()
 
         if add_bar:
             divider = make_axes_locatable(hax)
             cax = divider.append_axes("right", size="5%", pad=0.05)
             vlab = vlabel if vlabel is not None else var
             hfig.colorbar(im, cax=cax, orientation="vertical", label=vlab)
@@ -299,15 +298,15 @@
             vmin /= normalize_var
             vmax /= normalize_var
 
         # normalize x and y:
         if normalize_xy is not None:
             x_pos /= normalize_xy
             y_pos /= normalize_xy
-    
+
         if title is None:
             title = f"States mean, z =  {int(np.round(z_pos))} m"
 
         # create plot:
         out = self._get_fig(
             var,
             fig,
@@ -785,15 +784,15 @@
             ylabel,
             zlabel,
             title,
             add_bar,
             vlabel,
             ret_state,
             ret_im,
-            invert_axis='x',
+            invert_axis="x",
         )
 
         return out
 
     def gen_states_fig_xy(
         self,
         var,
@@ -976,16 +975,15 @@
 
         # normalize x and y:
         if normalize_xy is not None:
             x_pos /= normalize_xy
             y_pos /= normalize_xy
 
         # loop over states:
-        for si, s in enumerate(self.fres[FV.STATE].to_numpy()):
-
+        for si, s in enumerate(self.fres[FC.STATE].to_numpy()):
             ttl = f"State {s}" if title is None else title
             ttl += f", z =  {int(np.round(z_pos))} m"
 
             out = self._get_fig(
                 var,
                 fig,
                 figsize,
@@ -1014,15 +1012,15 @@
 
             yield out
 
     def gen_states_fig_xz(
         self,
         var,
         resolution,
-        x_direction=270.,
+        x_direction=270.0,
         xmin=None,
         zmin=0.0,
         xmax=None,
         zmax=None,
         xlabel="x [m]",
         zlabel="z [m]",
         y=None,
@@ -1218,16 +1216,15 @@
         # normalize x and z:
         if normalize_x is not None:
             x_pos /= normalize_x
         if normalize_z is not None:
             z_pos /= normalize_z
 
         # loop over states:
-        for si, s in enumerate(self.fres[FV.STATE].to_numpy()):
-
+        for si, s in enumerate(self.fres[FC.STATE].to_numpy()):
             ttl = f"State {s}" if title is None else title
             ttl += f", x direction = {x_direction}°"
             ttl += f", y =  {int(np.round(y_pos))} m"
 
             out = self._get_fig(
                 var,
                 fig,
@@ -1257,15 +1254,15 @@
 
             yield out
 
     def gen_states_fig_yz(
         self,
         var,
         resolution,
-        x_direction=270.,
+        x_direction=270.0,
         ymin=None,
         zmin=0.0,
         ymax=None,
         zmax=None,
         ylabel="y [m]",
         zlabel="z [m]",
         x=None,
@@ -1370,15 +1367,15 @@
             The image object
 
         """
 
         # prepare:
         n_states = self.algo.n_states
         n_turbines = self.algo.n_turbines
-        n_x = np.append(wd2uv(x_direction), [0.0], axis=0) ## -180 to get [1,0,0]
+        n_x = np.append(wd2uv(x_direction), [0.0], axis=0)  ## -180 to get [1,0,0]
         n_z = np.array([0.0, 0.0, 1.0])
         n_y = np.cross(n_z, n_x)
 
         # project to axes:
         xyz = np.zeros((n_states, n_turbines, 3), dtype=FC.DTYPE)
         xyz[:, :, 0] = self.fres[FV.X]
         xyz[:, :, 1] = self.fres[FV.Y]
@@ -1460,16 +1457,15 @@
         # normalize x and z:
         if normalize_y is not None:
             y_pos /= normalize_y
         if normalize_z is not None:
             z_pos /= normalize_z
 
         # loop over states:
-        for si, s in enumerate(self.fres[FV.STATE].to_numpy()):
-
+        for si, s in enumerate(self.fres[FC.STATE].to_numpy()):
             ttl = f"State {s}" if title is None else title
             ttl += f", x direction = {x_direction}°"
             ttl += f", x =  {int(np.round(x_pos))} m"
 
             out = self._get_fig(
                 var,
                 fig,
@@ -1491,11 +1487,11 @@
                 zlabel,
                 ttl,
                 add_bar,
                 vlabel,
                 ret_state,
                 ret_im,
                 quiv=quiv,
-                invert_axis='x',
+                invert_axis="x",
             )
 
             yield out
```

### Comparing `foxes-0.3.4/foxes/output/output.py` & `foxes-0.3.5/foxes/output/output.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.4/foxes/output/results_writer.py` & `foxes-0.3.5/foxes/output/results_writer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .output import Output
-import foxes.variables as FV
+import foxes.constants as FC
 
 
 class ResultsWriter(Output):
     """
     Writes results farm data to file.
 
     Parameters
@@ -17,21 +17,20 @@
     ----------
     data : pandas.DataFrame
         The farm results
 
     """
 
     def __init__(self, farm_results=None, data=None):
-
         if farm_results is not None and data is None:
             self.data = farm_results.to_dataframe().reset_index()
-            self.data[FV.TNAME] = farm_results[FV.TNAME].to_numpy()[
-                self.data[FV.TURBINE]
+            self.data[FC.TNAME] = farm_results[FC.TNAME].to_numpy()[
+                self.data[FC.TURBINE]
             ]
-            self.data.set_index([FV.STATE, FV.TURBINE], inplace=True)
+            self.data.set_index([FC.STATE, FC.TURBINE], inplace=True)
         elif farm_results is None and data is not None:
             self.data = data
         else:
             raise KeyError(
                 f"ResultsWriter: Either give 'farm_results' or 'data' arguments"
             )
 
@@ -78,10 +77,10 @@
             if len(inds):
                 for s, ns in inds.items():
                     data = data.rename_axis(index={s: ns})
         else:
             data = self.data[list(variables)]
 
         if turbine_names:
-            data = data.reset_index().set_index([FV.STATE, FV.TNAME])
+            data = data.reset_index().set_index([FC.STATE, FC.TNAME])
 
         super().write(file_path, data, **kwargs)
```

### Comparing `foxes-0.3.4/foxes/output/rose_plot.py` & `foxes-0.3.5/foxes/output/rose_plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 import pandas as pd
 import plotly.express as px
 
 import foxes.variables as FV
+import foxes.constants as FC
 from foxes.utils import wd2uv, uv2wd
 from foxes.algorithms import Downwind
 from foxes.core import WindFarm, Turbine
 from foxes.models import ModelBook
 from .output import Output
 
 
@@ -23,23 +24,22 @@
     ----------
     results : pandas.DataFrame
         The calculation results (farm or points)
 
     """
 
     def __init__(self, results):
-
         dims = list(results.dims.keys())
-        if dims[1] == FV.TURBINE:
-            self._rtype = FV.TURBINE
-        elif dims[1] == FV.POINT:
-            self._rtype = FV.POINT
+        if dims[1] == FC.TURBINE:
+            self._rtype = FC.TURBINE
+        elif dims[1] == FC.POINT:
+            self._rtype = FC.POINT
         else:
             raise KeyError(
-                f"Results dimension 1 is neither '{FV.TURBINE}' nor '{FV.POINT}': dims = {results.dims}"
+                f"Results dimension 1 is neither '{FC.TURBINE}' nor '{FC.POINT}': dims = {results.dims}"
             )
 
         self.results = results.to_dataframe()
 
     @classmethod
     def get_data_info(cls, dname):
         """
@@ -144,15 +144,15 @@
         uv = wd2uv(data[wd_var].to_numpy())
         data["u"] = uv[:, 0]
         data["v"] = uv[:, 1]
 
         data[FV.WEIGHT] *= 100
         data = data.rename(columns={FV.WEIGHT: "frequency"})
 
-        el = turbine if self._rtype == FV.TURBINE else point
+        el = turbine if self._rtype == FC.TURBINE else point
         if el is None:
             data = data.groupby(level=0).mean()
         else:
             sname = data.index.names[0]
             grp = data.reset_index().groupby(self._rtype)
             data = grp.get_group(el).set_index(sname)
 
@@ -328,15 +328,14 @@
         The evaluation point, shape: (3,)
     mbook : foxes.models.ModelBook, optional
         The model book
 
     """
 
     def __init__(self, states, point, mbook=None, ws_var=FV.AMB_REWS):
-
         farm = WindFarm()
         farm.add_turbine(
             Turbine(
                 xy=point[:2],
                 H=point[2],
                 turbine_models=["null_type"],
             ),
```

### Comparing `foxes-0.3.4/foxes/output/state_turbine_map.py` & `foxes-0.3.5/foxes/output/state_turbine_map.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import matplotlib.pyplot as plt
 import numpy as np
 
-import foxes.variables as FV
+import foxes.constants as FC
 from .output import Output
 
 
 class StateTurbineMap(Output):
     """
     Creates heat maps with turbines on the one
     and states on the other axis.
@@ -52,16 +52,16 @@
 
         Returns
         -------
         ax : pyplot.Axis
             The plot axis
 
         """
-        turbines = self.results[FV.TURBINE].to_numpy()
-        states = self.results[FV.STATE].to_numpy()
+        turbines = self.results[FC.TURBINE].to_numpy()
+        states = self.results[FC.STATE].to_numpy()
 
         if ax is None:
             __, ax = plt.subplots(figsize=figsize)
         fig = ax.get_figure()
 
         ds = states[-1] - states[-2]
         states = np.append(states, states[-1] + ds)
```

### Comparing `foxes-0.3.4/foxes/output/turbine_type_curves.py` & `foxes-0.3.5/foxes/output/turbine_type_curves.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
             y_labels = [None for v in vars]
         if not isinstance(axs, (list, tuple, np.ndarray)):
             axs = [axs]
 
         ws = np.arange(ws_min, ws_max + ws_step, ws_step, dtype=FC.DTYPE)
         n_states = len(ws)
         sdata = pd.DataFrame(index=range(n_states))
-        sdata.index.name = FV.STATE
+        sdata.index.name = FC.STATE
         sdata[FV.WS] = ws
 
         models = [turbine_type]
 
         states = StatesTable(
             sdata,
             output_vars={FV.WS, FV.WD, FV.TI, FV.RHO},
@@ -128,15 +128,14 @@
         )
 
         algo = Downwind(self.mbook, farm, states, wake_models=[], verbosity=0)
 
         results = algo.calc_farm()
 
         if P_max is not None:
-
             sname = f"_{type(self).__name__}_set_Pmax"
             self.mbook.turbine_models[sname] = SetFarmVars()
             self.mbook.turbine_models[sname].add_var(FV.MAX_P, P_max)
             models += [sname, "PMask"]
 
             farm = WindFarm()
             farm.add_turbine(
@@ -147,15 +146,14 @@
             algo = Downwind(self.mbook, farm, states, wake_models=[], verbosity=0)
 
             results1 = algo.calc_farm()
 
             del self.mbook.turbine_models[sname]
 
         for i, v in enumerate(vars):
-
             ax = axs[i]
             if ax is None:
                 __, ax = plt.subplots(figsize=figsize)
 
             pargs = {"linewidth": 2.5}
             pargs.update(kwargs)
             ax.plot(ws, results[v][:, 0], label="default", **pargs)
```

### Comparing `foxes-0.3.4/foxes/utils/abl/neutral.py` & `foxes-0.3.5/foxes/utils/abl/neutral.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.4/foxes/utils/abl/stable.py` & `foxes-0.3.5/foxes/utils/abl/stable.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.4/foxes/utils/abl/unstable.py` & `foxes-0.3.5/foxes/utils/abl/unstable.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.4/foxes/utils/cubic_roots.py` & `foxes-0.3.5/foxes/utils/cubic_roots.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,29 +49,27 @@
     R = (9 * b_a * c_a - 27 * d_a - 2 * b_a * b_a2) / 54
     Q3 = Q * Q * Q
     D = Q3 + R * R
     b_a_3 = (1.0 / 3.0) * b_a
 
     sel = Q == 0.0
     if np.any(sel):
-
         o = out[sel, 0]
 
         sel2 = R == 0.0
         if np.any(sel2):
             o[sel2] = -b_a_3[sel][sel2]
 
         if np.any(~sel2):
             o[~sel2] = np.pow(2 * R[sel][~sel2], 1 / 3.0) - b_a_3[sel][~sel2]
 
         out[sel, 0] = o
 
     sel = D <= 0.0
     if np.any(sel):
-
         # Three real roots
         theta = np.arccos(R[sel] / np.sqrt(-Q3[sel]))
         sqrt_Q = np.sqrt(-Q[sel])
 
         out[sel, 0] = 2 * sqrt_Q * np.cos(theta / 3.0) - b_a_3[sel]
         out[sel, 1] = 2 * sqrt_Q * np.cos((theta + 2 * np.pi) / 3.0) - b_a_3[sel]
         out[sel, 2] = 2 * sqrt_Q * np.cos((theta + 4 * np.pi) / 3.0) - b_a_3[sel]
@@ -96,41 +94,38 @@
     a3: numpy.ndarray
         The coefficients a[3], or None for ones
 
     """
 
     N = len(a0)
     for n in range(N):
-
         c0 = a0[n]
         c1 = a1[n]
         c2 = a2[n]
         c3 = a3[n]
 
         print(f"Polynomial {n}: a = {(c0,c1,c2,c3)}")
 
         rts = np.unique(roots[n])
         rts = rts[~np.isnan(rts)]
 
         for x in rts:
-
             f = c0 + c1 * x + c2 * x**2 + c3 * x**3
             ok = np.abs(f) <= tol
 
             print(f"  root x = {x}: f(x) = {f}     {'OK' if ok else 'FAILED'}")
 
             if not ok:
                 raise Exception("NOT OK!")
 
         if len(rts) == 0:
             print("  no real roots.")
 
 
 if __name__ == "__main__":
-
     N = 100
     a0 = np.random.uniform(-10.0, 10.0, N)
     a1 = np.random.uniform(-10.0, 10.0, N)
     a2 = np.random.uniform(-10.0, 10.0, N)
     a3 = np.random.uniform(1.0, 10.0, N)
 
     roots = cubic_roots(a0, a1, a2, a3)
```

### Comparing `foxes-0.3.4/foxes/utils/data_book.py` & `foxes-0.3.5/foxes/utils/data_book.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.4/foxes/utils/dict.py` & `foxes-0.3.5/foxes/utils/dict.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.4/foxes/utils/geom2d/area_geometry.py` & `foxes-0.3.5/foxes/utils/geom2d/area_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,14 @@
         pars_boundary : dict
             Parameters for boundary plotting command
         pars_distance : dict
             Parameters for distance plotting command
 
         """
         if fill_mode is not None:
-
             if "Nx" in pars_distance or "Ny" in pars_distance:
                 Nx = pars_distance.pop("Nx")
                 Ny = pars_distance.pop("Ny")
             elif "N" in pars_distance:
                 Nx = pars_distance.pop("N")
                 Ny = Nx
             else:
@@ -455,15 +454,14 @@
             return self.geometries[0].points_distance(points, return_nearest)
 
         n_pts = len(points)
         dist = np.full(n_pts, np.inf, dtype=np.float64)
         pins = np.zeros(n_pts, dtype=bool)
         nerst = np.zeros((n_pts, 2), dtype=np.float64) if return_nearest else None
         for g in self.geometries:
-
             res = g.points_distance(points, return_nearest)
             ins = g.points_inside(points)
             d = res[0] if return_nearest else res
 
             # was outside, is outside:
             sel = ~pins & ~ins & (d < dist)
             if np.any(sel):
```

### Comparing `foxes-0.3.4/foxes/utils/geom2d/circle.py` & `foxes-0.3.5/foxes/utils/geom2d/circle.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,14 @@
 
         super().add_to_figure(
             ax, show_boundary, fill_mode, pars_boundary, pars_distance
         )
 
 
 if __name__ == "__main__":
-
     centre = np.array([3.0, 4.0])
     radius = 2.5
     N = 500
 
     fig, ax = plt.subplots()
     g = Circle(centre, radius)
     g.add_to_figure(ax, fill_mode="dist_inside")
```

### Comparing `foxes-0.3.4/foxes/utils/geom2d/example_intersection.py` & `foxes-0.3.5/foxes/utils/geom2d/example_intersection.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import matplotlib.pyplot as plt
 
 from .circle import Circle
 from .polygon import ClosedPolygon
 from .area_geometry import AreaIntersection
 
 if __name__ == "__main__":
-
     centres = []
     radii = []
     N = 500
 
     plist = [
         np.array([[1.0, 1.0], [1.3, 6], [5.8, 6.2], [6.5, 0.8]]),
         np.array([[1.5, 1.5], [1.5, 8], [2.5, 8], [2.5, 1.5]]),
```

### Comparing `foxes-0.3.4/foxes/utils/geom2d/example_union.py` & `foxes-0.3.5/foxes/utils/geom2d/example_union.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import matplotlib.pyplot as plt
 
 from .circle import Circle
 from .polygon import ClosedPolygon
 from .area_geometry import AreaUnion
 
 if __name__ == "__main__":
-
     boundary = (
         ClosedPolygon(
             np.array([[0, 0], [0, 1200], [1000, 800], [900, -200]], dtype=np.float64)
         )
         + ClosedPolygon(
             np.array([[500, 0], [500, 1500], [1000, 1500], [1000, 0]], dtype=np.float64)
         )
```

### Comparing `foxes-0.3.4/foxes/utils/geom2d/half_plane.py` & `foxes-0.3.5/foxes/utils/geom2d/half_plane.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,15 +167,14 @@
             The inverted geometry
 
         """
         return HalfPlane(self.centre, -self.n)
 
 
 if __name__ == "__main__":
-
     from .circle import Circle
 
     p0 = [4, 5]
     n = [1.0, 0.3]
 
     centre = np.array([3.0, 4.0])
     radius = 2.5
```

### Comparing `foxes-0.3.4/foxes/utils/geom2d/polygon.py` & `foxes-0.3.5/foxes/utils/geom2d/polygon.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,15 +22,14 @@
         The polygon points
     poly : matplotlib.path.Path
         The closed polygon geometry
 
     """
 
     def __init__(self, points):
-
         self.points = points
 
         if not np.all(points[0] == points[-1]):
             self.points = np.append(self.points, points[[0]], axis=0)
 
         self.poly = Path(self.points, closed=True)
 
@@ -89,29 +88,26 @@
             dists = np.take_along_axis(dists, mini[:, None], axis=1)[:, 0]
             minp = self.points[mini]
             del mini
         else:
             dists = np.min(dists, axis=1)
 
         for pi in range(len(self.points) - 1):
-
             pA = self.points[pi]
             pB = self.points[pi + 1]
             n = pB - pA
             d = np.linalg.norm(n)
 
             if d > 0:
-
                 n /= d
                 q = points - pA[None, :]
                 x = np.einsum("pd,d->p", q, n)
 
                 sel = (x > 0) & (x < d)
                 if np.any(sel):
-
                     x = x[sel]
                     y2 = np.maximum(np.linalg.norm(q[sel], axis=1) ** 2 - x**2, 0.0)
 
                     dsel = dists[sel]
                     dists[sel] = np.minimum(dsel, np.sqrt(y2))
 
                     if return_nearest:
@@ -178,15 +174,14 @@
 
         super().add_to_figure(
             ax, show_boundary, fill_mode, pars_boundary, pars_distance
         )
 
 
 if __name__ == "__main__":
-
     points = np.array([[1.0, 1.0], [1.3, 6], [5.8, 6.2], [6.5, 0.8]])
     N = 500
 
     fig, ax = plt.subplots()
     g = ClosedPolygon(points)
     g.add_to_figure(ax, fill_mode="dist_inside")
     plt.show()
```

### Comparing `foxes-0.3.4/foxes/utils/geopandas_helpers.py` & `foxes-0.3.5/foxes/utils/geopandas_helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,70 +3,76 @@
 
 import foxes.constants as FC
 from .dict import Dict
 from .geom2d import AreaUnion, ClosedPolygon
 
 try:
     import geopandas as gpd
+
     IMPORT_GPD_OK = True
 except ImportError:
     gpd = None
     IMPORT_GPD_OK = False
 
 try:
     import utm
+
     IMPORT_UTM_OK = True
 except ImportError:
     utm = None
     IMPORT_UTM_OK = False
 
+
 def check_import_gpd():
     """
     Checks if library import worked,
     raises error otherwise.
     """
     if not IMPORT_GPD_OK:
         print("\n\nFailed to import geopandas. Please install, either via pip:\n")
         print("  pip install geopandas\n")
         print("or via conda:\n")
         print("  conda install -c conda-forge geopandas\n")
         raise ImportError("Failed to import geopandas")
 
+
 def check_import_utm():
     """
     Checks if library import worked,
     raises error otherwise.
     """
     if not IMPORT_UTM_OK:
         print("\n\nFailed to import utm. Please install, either via pip:\n")
         print("  pip install utm\n")
         print("or via conda:\n")
         print("  conda install -c conda-forge utm\n")
         raise ImportError("Failed to import utm")
 
+
 def read_shp(fname, **kwargs):
     """
     Read a shape file
 
     Parameters
     ----------
     fname : str
         Path to the .shp file
     kwargs : dict, optional
         Additional parameters for geopandas.read_file()
-    
+
     Returns
     -------
     data : geopandas.GeoDataFrame
         The data frame in WSG84
 
     """
     check_import_gpd()
-    gpdf=gpd.read_file(fname, **kwargs)
-    return gpdf.to_crs("EPSG:4326") # Convert to WGS84
+    gpdf = gpd.read_file(fname, **kwargs)
+    return gpdf.to_crs("EPSG:4326")  # Convert to WGS84
+
 
 def shp2csv(ifile, ofile, in_kwargs={}, out_kwargs={}, verbosity=1):
     """
     Read shape file, write csv file
 
     Parameters
     ----------
@@ -82,51 +88,53 @@
         The verbosity level, 0 = silent
 
     """
     if verbosity > 0:
         print("Reading file", ifile)
 
     gpdf = read_shp(ifile, **in_kwargs)
-    
+
     if verbosity > 0:
         print("Writing file", ofile)
-    
+
     gpdf.to_csv(ofile, **out_kwargs)
 
     return gpdf
 
+
 def _extract_poly_coords(geom):
     """
     Helper function for shapefile reading
     """
-    if geom.geom_type == 'Polygon':
+    if geom.geom_type == "Polygon":
         exterior_coords = geom.exterior.coords[:]
         interior_coords = []
         for interior in geom.interiors:
             interior_coords.append(interior.coords[:])
-    elif geom.geom_type == 'MultiPolygon':
+    elif geom.geom_type == "MultiPolygon":
         exterior_coords = []
         interior_coords = []
         for part in geom.geoms:
             epe, epi = _extract_poly_coords(part)  # Recursive call
             exterior_coords.append(epe)
             interior_coords.append(epi)
     else:
-        raise ValueError('Unhandled geometry type: ' + repr(geom.type))
+        raise ValueError("Unhandled geometry type: " + repr(geom.type))
     return exterior_coords, interior_coords
 
+
 def read_shp_polygons(
-        fname, 
-        names=None, 
-        name_col="Name", 
-        geom_col="geometry",
-        to_utm=True,
-        ret_utm_zone=False,
-        **kwargs
-    ):
+    fname,
+    names=None,
+    name_col="Name",
+    geom_col="geometry",
+    to_utm=True,
+    ret_utm_zone=False,
+    **kwargs,
+):
     """
     Reads the polygon points from a shp file.
 
     Parameters
     ----------
     fname : str
         Path to the .shp file
@@ -170,60 +178,67 @@
         utmz = int(to_utm[:-1]) if isinstance(to_utm, str) else None
         utml = to_utm[-1] if isinstance(to_utm, str) else None
 
     exterior = Dict()
     interior = Dict()
     names = pnames if names is None else names
     for name in names:
-        if name == name:    # exclude nan values 
+        if name == name:  # exclude nan values
             if not name in pnames:
-                raise KeyError(f"Name '{name}' not found in file '{fname}'. Names: {pnames}")
+                raise KeyError(
+                    f"Name '{name}' not found in file '{fname}'. Names: {pnames}"
+                )
 
             a = pdf.loc[pnames.index(name), geom_col]
             epe, epi = _extract_poly_coords(a)
 
             def _to_utm(poly):
                 nonlocal utmz, utml
                 utm_poly = np.zeros_like(poly)
                 utm_poly[:, 0], utm_poly[:, 1], utmz, utml = utm.from_latlon(
-                    poly[:, 1], poly[:, 0], force_zone_number=utmz, force_zone_letter=utml)
+                    poly[:, 1],
+                    poly[:, 0],
+                    force_zone_number=utmz,
+                    force_zone_letter=utml,
+                )
                 return utm_poly
 
             def _to_numpy(data):
                 if not len(data):
                     return []
                 if isinstance(data[0], tuple):
                     out = np.array(data, dtype=FC.DTYPE)
                     return _to_utm(out) if apply_utm else out
                 return [_to_numpy(d) for d in data]
-            
+
             exterior[name] = _to_numpy(epe)
             interior[name] = _to_numpy(epi)
 
     if ret_utm_zone:
         return exterior, interior, f"{utmz}{utml}"
     else:
-        return exterior, interior      
+        return exterior, interior
+
 
 def shp2geom2d(*args, ret_utm_zone=False, **kwargs):
     """
     Read shapefile into geom2d geometry
 
     Parameters
     ----------
     args : tuple, optional
         Arguments for read_shp_polygons()
     ret_utm_zone : bool
         Return UTM zone plus letter as str
     kwargs : dict, optional
         Keyword arguments for read_shp_polygons()
-    
+
     Returns
     -------
-    geom : foxes.tools.geom2D.AreaGeometry 
+    geom : foxes.tools.geom2D.AreaGeometry
         The geometry object
     utm_zone_str : str, optional
         The utem zone plus letter as str, e.g. "32U"
 
     """
 
     exint = read_shp_polygons(*args, ret_utm_zone=ret_utm_zone, **kwargs)
@@ -239,31 +254,33 @@
             return ClosedPolygon(data)
         gs = [_create_geom(g) for g in data]
         gs = [g for g in gs if g is not None]
         return AreaUnion(gs) if len(gs) else None
 
     gext = _create_geom(exint[0])
     gint = _create_geom(exint[1])
-    geom = gext-gint if gint is not None else gext
+    geom = gext - gint if gint is not None else gext
 
     if ret_utm_zone:
         return geom, exint[2]
     else:
         return geom
 
 
 if __name__ == "__main__":
-
     # define arguments and options:
     parser = argparse.ArgumentParser()
     parser.add_argument("shp_file", help="The input .shp file")
     parser.add_argument("-n", "--names", help="Area names", default=None, nargs="+")
-    parser.add_argument("--no_utm", help="switch off conversion to UTM", action="store_true")
+    parser.add_argument(
+        "--no_utm", help="switch off conversion to UTM", action="store_true"
+    )
     args = parser.parse_args()
 
     g = shp2geom2d(args.shp_file, to_utm=not args.no_utm, names=args.names)
 
     import matplotlib.pyplot as plt
+
     fig, ax = plt.subplots()
     g.add_to_figure(ax)
     plt.show()
     plt.close(fig)
```

### Comparing `foxes-0.3.4/foxes/utils/pandas_helpers.py` & `foxes-0.3.5/foxes/utils/pandas_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,18 +91,16 @@
             The data
 
         """
         fname = str(file_path)
         L = len(fname)
         f = None
         for fmt in cls.DATA_FILE_FORMATS:
-
             l = len(fmt)
             if fname[L - l :] == fmt:
-
                 if fmt[:3] == "csv":
                     f = pd.read_csv
 
                 elif fmt == "h5":
                     f = pd.read_hdf
 
                 elif fmt == "nc":
@@ -149,29 +147,26 @@
                 )
             else:
                 out[c] = data[c]
 
         L = len(file_path)
         f = None
         for fmt in cls.DATA_FILE_FORMATS:
-
             l = len(fmt)
             if file_path[L - l :] == fmt:
-
                 if fmt[:3] == "csv":
                     f = out.to_csv
 
                 elif fmt == "h5":
                     f = out.to_hdf
 
                 elif fmt == "nc":
                     f = out.to_netcdf
 
                 if f is not None:
-
                     pars = cls.DEFAULT_WRITING_PARAMETERS[fmt]
                     pars.update(kwargs)
 
                     f(file_path, **pars)
 
                     return
```

### Comparing `foxes-0.3.4/foxes/utils/runners.py` & `foxes-0.3.5/foxes/utils/runners.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from abc import abstractmethod, ABCMeta
-from copy import deepcopy
 import dask
 from dask.distributed import Client, LocalCluster
 from dask.distributed import get_client
 from dask.diagnostics import ProgressBar
 
+import foxes.constants as FC
+
 class Runner(metaclass=ABCMeta):
     """
     Abstract base class for runners.
     """
 
     def __init__(self):
         self._initialized = False
@@ -172,21 +173,20 @@
     @classmethod
     def is_distributed(cls):
         try:
             get_client()
             return True
         except ValueError:
             return False
-    
+
     def initialize(self):
         """
         Initialize the runner
         """
         if self.scheduler == "distributed":
-
             self.print("Launching dask cluster..")
 
             self._cluster = LocalCluster(**self.cluster_args)
             self._client = Client(self._cluster, **self.client_args)
 
             self.print(self._cluster)
             self.print(f"Dashboard: {self._client.dashboard_link}\n")
@@ -228,15 +228,14 @@
         return results
 
     def finalize(self):
         """
         Finallize the runner
         """
         if self.scheduler == "distributed":
-
             self.print("\n\nShutting down dask cluster")
             self._client.close()
             self._cluster.close()
-        
+
         dask.config.refresh()
 
         super().finalize()
```

### Comparing `foxes-0.3.4/foxes/utils/two_circles.py` & `foxes-0.3.5/foxes/utils/two_circles.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,35 +79,32 @@
 
     # prepare:
     out = np.zeros_like(d)
 
     # condition d < r1 + r2:
     sel0 = d < r1 + r2
     if np.any(sel0):
-
         # condition r1 >= r2:
         sela = r1 >= r2
         selr = sel0 & sela
         if np.any(selr):
-
             # condition d <= r1 - r2:
             selb = d <= r1 - r2
             seld = selr & selb
             if np.any(seld):
                 out[seld] = np.pi * r2[seld] ** 2
 
             # condition d > r1 - r2:
             seld = selr & (~selb)
             if np.any(seld):
                 out[seld] = area(r1[seld], r2[seld], d[seld])
 
         # condition r1 < r2:
         selr = sel0 & (~sela)
         if np.any(selr):
-
             # condition d <= r2 - r1:
             selb = d <= r2 - r1
             seld = selr & selb
             if np.any(seld):
                 out[seld] = np.pi * r1[seld] ** 2
 
             # condition d > r2 - r1:
```

### Comparing `foxes-0.3.4/foxes/utils/wind_dir.py` & `foxes-0.3.5/foxes/utils/wind_dir.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.4/foxes.egg-info/PKG-INFO` & `foxes-0.3.5/foxes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxes
-Version: 0.3.4
+Version: 0.3.5
 Summary: Farm Optimization and eXtended yield Evaluation Software
 Author: Fraunhofer IWES
 Author-email: jonas.schmidt@iwes.fraunhofer.de
 License: MIT
 Project-URL: Source Code, https://github.com/FraunhoferIWES/foxes
 Project-URL: Bug Tracker, https://github.com/FraunhoferIWES/foxes/issues
 Project-URL: Documentation, https://fraunhoferiwes.github.io/foxes.docs/index.html
```

### Comparing `foxes-0.3.4/foxes.egg-info/SOURCES.txt` & `foxes-0.3.5/foxes.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -65,20 +65,20 @@
 foxes/data/states/abl_states_6000.csv.gz
 foxes/data/states/timeseries_3000.csv.gz
 foxes/data/states/timeseries_8000.csv.gz
 foxes/data/states/wind_rose_bremen.csv
 foxes/data/states/wind_rotation.nc
 foxes/input/__init__.py
 foxes/input/farm_layout/__init__.py
-foxes/input/farm_layout/add_from_csv.py
-foxes/input/farm_layout/add_from_df.py
-foxes/input/farm_layout/add_from_file.py
-foxes/input/farm_layout/add_from_json.py
-foxes/input/farm_layout/add_grid.py
-foxes/input/farm_layout/add_row.py
+foxes/input/farm_layout/from_csv.py
+foxes/input/farm_layout/from_df.py
+foxes/input/farm_layout/from_file.py
+foxes/input/farm_layout/from_json.py
+foxes/input/farm_layout/grid.py
+foxes/input/farm_layout/row.py
 foxes/input/states/__init__.py
 foxes/input/states/field_data_nc.py
 foxes/input/states/multi_height.py
 foxes/input/states/scan_ws.py
 foxes/input/states/single.py
 foxes/input/states/states_table.py
 foxes/input/states/create/__init__.py
@@ -105,14 +105,15 @@
 foxes/models/rotor_models/__init__.py
 foxes/models/rotor_models/centre.py
 foxes/models/rotor_models/grid.py
 foxes/models/turbine_models/__init__.py
 foxes/models/turbine_models/calculator.py
 foxes/models/turbine_models/kTI_model.py
 foxes/models/turbine_models/power_mask.py
+foxes/models/turbine_models/rotor_centre_calc.py
 foxes/models/turbine_models/sector_management.py
 foxes/models/turbine_models/set_XYHD.py
 foxes/models/turbine_models/set_farm_vars.py
 foxes/models/turbine_models/table_factors.py
 foxes/models/turbine_models/thrust2ct.py
 foxes/models/turbine_models/yaw2yawm.py
 foxes/models/turbine_models/yawm2yaw.py
@@ -148,14 +149,15 @@
 foxes/models/wake_models/wind/bastankhah.py
 foxes/models/wake_models/wind/jensen.py
 foxes/models/wake_models/wind/porte_agel.py
 foxes/models/wake_models/wind/turbopark.py
 foxes/models/wake_superpositions/__init__.py
 foxes/models/wake_superpositions/linear.py
 foxes/models/wake_superpositions/max.py
+foxes/models/wake_superpositions/product.py
 foxes/models/wake_superpositions/quadratic.py
 foxes/models/wake_superpositions/ti_superp.py
 foxes/opt/__init__.py
 foxes/opt/constraints/__init__.py
 foxes/opt/constraints/area_geometry.py
 foxes/opt/constraints/min_dist.py
 foxes/opt/core/__init__.py
```

### Comparing `foxes-0.3.4/setup.cfg` & `foxes-0.3.5/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 [options.extras_require]
 test = 
 	flake8
 	pytest
 doc = 
 	sphinx
-	sphinx_rtd_theme
+	sphinx-immaterial
 	nbsphinx
 	ipykernel
 	ipywidgets
 	m2r2
 scripts = 
 
 [egg_info]
```

