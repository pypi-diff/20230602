# Comparing `tmp/naludaq-0.17.7.tar.gz` & `tmp/naludaq-0.18.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naludaq-0.17.7.tar", last modified: Wed May 31 20:11:48 2023, max compression
+gzip compressed data, was "naludaq-0.18.0.tar", last modified: Thu Jun  1 23:50:03 2023, max compression
```

## Comparing `naludaq-0.17.7.tar` & `naludaq-0.18.0.tar`

### file list

```diff
@@ -1,247 +1,251 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.674107 naludaq-0.17.7/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-31 20:11:29.000000 naludaq-0.17.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15635 2023-05-31 20:11:48.674107 naludaq-0.17.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14785 2023-05-31 20:11:29.000000 naludaq-0.17.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-31 20:11:29.000000 naludaq-0.17.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 20:11:48.674107 naludaq-0.17.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-31 20:11:29.000000 naludaq-0.17.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.638105 naludaq-0.17.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.646105 naludaq-0.17.7/src/naludaq/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.646105 naludaq-0.17.7/src/naludaq/backend/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/backend/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/backend/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/backend/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.646105 naludaq-0.17.7/src/naludaq/backend/managers/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/backend/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/backend/managers/acquisitions.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/backend/managers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/backend/managers/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/backend/managers/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/backend/managers/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.646105 naludaq-0.17.7/src/naludaq/backend/models/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/backend/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35624 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/backend/models/acquisition.py
--rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/backend/models/device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.646105 naludaq-0.17.7/src/naludaq/board/
--rw-r--r--   0 runner    (1001) docker     (123)    28790 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/board/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23941 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/board/board_inits.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.650106 naludaq-0.17.7/src/naludaq/board/connections/
--rw-r--r--   0 runner    (1001) docker     (123)    18932 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/board/connections/_FTDI.py
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/board/connections/_MockUART.py
--rw-r--r--   0 runner    (1001) docker     (123)    14633 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/board/connections/_UART.py
--rw-r--r--   0 runner    (1001) docker     (123)    10093 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/board/connections/_USB.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/board/connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/board/connections/base_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/board/connections/base_ethernet.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/board/connections/base_serial.py
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/board/connections/connection_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/board/connections/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/board/connections/udp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.650106 naludaq-0.17.7/src/naludaq/board/initializers/
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/board/initializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/board/initializers/aardvarcv3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/board/initializers/aodsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/board/initializers/init_aodsv2_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/board/initializers/init_hdsocv1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/board/initializers/init_udc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/board/initializers/init_upac96.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/board/initializers/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (123)    17669 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/board/params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.650106 naludaq-0.17.7/src/naludaq/communication/
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/communication/analog_registers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/communication/control_registers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/communication/digital_registers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/communication/i2c.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/communication/i2c_registers.py
--rw-r--r--   0 runner    (1001) docker     (123)    28991 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/communication/registers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.650106 naludaq-0.17.7/src/naludaq/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/analog_debug_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.650106 naludaq-0.17.7/src/naludaq/controllers/biasing_mode/
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/biasing_mode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/biasing_mode/udc16.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.654106 naludaq-0.17.7/src/naludaq/controllers/board/
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/board/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/board/aodsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15185 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/board/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/board/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/board/oleas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/board/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/board/udc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/board/upac.py
--rw-r--r--   0 runner    (1001) docker     (123)     9258 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/board/upac96.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.654106 naludaq-0.17.7/src/naludaq/controllers/connection/
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21101 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/connection/connection_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/connection/upac.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/connection/upac96.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.654106 naludaq-0.17.7/src/naludaq/controllers/external_dac/
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/external_dac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/external_dac/ad5671.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/external_dac/ad5675.py
--rw-r--r--   0 runner    (1001) docker     (123)    11125 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/external_dac/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/external_dac/dac7578.py
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/external_dac/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/external_dac/i2c_dac.py
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/external_dac/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/external_dac/upac32.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.654106 naludaq-0.17.7/src/naludaq/controllers/gainstages/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/gainstages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/gainstages/aodsv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/gainstages/oddsock_aods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.658106 naludaq-0.17.7/src/naludaq/controllers/peripherals/
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/peripherals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/peripherals/aardvarcv3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/peripherals/aodsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/peripherals/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8973 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/peripherals/peripherals_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/peripherals/upac.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/peripherals/upac96.py
--rw-r--r--   0 runner    (1001) docker     (123)    16209 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/project_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.658106 naludaq-0.17.7/src/naludaq/controllers/readout/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/readout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/readout/aardvarcv3.py
--rw-r--r--   0 runner    (1001) docker     (123)    14264 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/readout/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/readout/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/readout/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/si5341_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.658106 naludaq-0.17.7/src/naludaq/controllers/tia/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/tia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/tia/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11997 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/tia/hdsoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.658106 naludaq-0.17.7/src/naludaq/controllers/trigger/
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/trigger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/trigger/aodsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/trigger/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     8881 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/trigger/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/trigger/siread.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/trigger/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/trigger/upac.py
--rw-r--r--   0 runner    (1001) docker     (123)    17145 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/trigger/upac96.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.658106 naludaq-0.17.7/src/naludaq/daq/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/daq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/daq/debugdaq.py
--rw-r--r--   0 runner    (1001) docker     (123)    20482 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/daq/lightdaq.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/daq/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.662107 naludaq-0.17.7/src/naludaq/daq/workers/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/daq/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/daq/workers/answer_parser_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10475 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/daq/workers/csv_storage_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.662107 naludaq-0.17.7/src/naludaq/daq/workers/packager/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/daq/workers/packager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/daq/workers/packager/worker_packager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/daq/workers/packager/worker_packager_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/daq/workers/packager/worker_packager_hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/daq/workers/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/daq/workers/worker_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/daq/workers/worker_serial_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/daq/workers/worker_usb_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.662107 naludaq-0.17.7/src/naludaq/devices/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/devices/eeprom.py
--rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/devices/i2c_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/devices/ltc2990.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.662107 naludaq-0.17.7/src/naludaq/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/helpers/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/helpers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/helpers/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/helpers/register_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/helpers/semiton.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/helpers/validations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.662107 naludaq-0.17.7/src/naludaq/io/
--rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22338 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/io/csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    35939 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/io/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)    12900 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/io/io_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.662107 naludaq-0.17.7/src/naludaq/models/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/models/acq_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9728 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/models/acquisition.py
--rw-r--r--   0 runner    (1001) docker     (123)    15839 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/naludaq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.666107 naludaq-0.17.7/src/naludaq/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10831 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/parsers/aardvarcv3_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/parsers/answer_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/parsers/aodsoc_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/parsers/asocv3_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8271 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/parsers/hdsoc_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.666107 naludaq-0.17.7/src/naludaq/parsers/headers/
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/parsers/headers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/parsers/headers/asoc.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/parsers/headers/asocv2.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/parsers/headers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/parsers/headers/siread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/parsers/headers/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/parsers/headers/upac32.py
--rw-r--r--   0 runner    (1001) docker     (123)    11956 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/parsers/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/parsers/trbhm_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/parsers/udc_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/parsers/upac96_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/parsers/upac_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.666107 naludaq-0.17.7/src/naludaq/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.666107 naludaq-0.17.7/src/naludaq/tools/adc2mv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/adc2mv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/adc2mv/adc_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16214 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/adc2mv/adc_linear_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/adc2mv/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/adc2mv/pre_adc2mv.py
--rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/autoaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.670107 naludaq-0.17.7/src/naludaq/tools/autotrigger/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/autotrigger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/autotrigger/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/board_backup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.670107 naludaq-0.17.7/src/naludaq/tools/dac_sweep/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/dac_sweep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/dac_sweep/dac_sweep_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    11823 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/data_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/ft60x.py
--rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/ftdi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.670107 naludaq-0.17.7/src/naludaq/tools/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/optimizers/bayesian_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/optimizers/gainstagetuner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.670107 naludaq-0.17.7/src/naludaq/tools/pedestals/
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/pedestals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.670107 naludaq-0.17.7/src/naludaq/tools/pedestals/_new/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/pedestals/_new/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/pedestals/_new/aav3.py
--rw-r--r--   0 runner    (1001) docker     (123)    25345 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/pedestals/_new/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/pedestals/_new/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/pedestals/aardvarcv3_pedestals_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/pedestals/hdsoc_pedestals_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/pedestals/pedestals_acq.py
--rw-r--r--   0 runner    (1001) docker     (123)    34274 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/pedestals/pedestals_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/pedestals/pedestals_correcter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/pedestals/pedestals_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10912 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/pedestals/udc16_pedestals_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/pedestals/upac32_pedestals_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    12497 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/pedestals/upac96_pedestals_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.670107 naludaq-0.17.7/src/naludaq/tools/threshold_scan/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/threshold_scan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/threshold_scan/hdsoc_thresholdscan.py
--rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/threshold_scan/threshold_scan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.670107 naludaq-0.17.7/src/naludaq/tools/timing_cal/
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/timing_cal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/timing_cal/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/timing_cal/correcter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.670107 naludaq-0.17.7/src/naludaq/tools/waiter/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/waiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/waiter/eventwaiter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.646105 naludaq-0.17.7/src/naludaq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15635 2023-05-31 20:11:48.000000 naludaq-0.17.7/src/naludaq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8160 2023-05-31 20:11:48.000000 naludaq-0.17.7/src/naludaq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 20:11:48.000000 naludaq-0.17.7/src/naludaq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-31 20:11:48.000000 naludaq-0.17.7/src/naludaq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-31 20:11:48.000000 naludaq-0.17.7/src/naludaq.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.670107 naludaq-0.17.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-31 20:11:29.000000 naludaq-0.17.7/tests/test_naludaq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.697728 naludaq-0.18.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-01 23:49:47.000000 naludaq-0.18.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15635 2023-06-01 23:50:03.697728 naludaq-0.18.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14785 2023-06-01 23:49:47.000000 naludaq-0.18.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-01 23:49:47.000000 naludaq-0.18.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 23:50:03.697728 naludaq-0.18.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-01 23:49:47.000000 naludaq-0.18.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.669728 naludaq-0.18.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.673728 naludaq-0.18.0/src/naludaq/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.673728 naludaq-0.18.0/src/naludaq/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/backend/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/backend/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/backend/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.677728 naludaq-0.18.0/src/naludaq/backend/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/backend/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/backend/managers/acquisitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/backend/managers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/backend/managers/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/backend/managers/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/backend/managers/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.677728 naludaq-0.18.0/src/naludaq/backend/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/backend/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35624 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/backend/models/acquisition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/backend/models/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.677728 naludaq-0.18.0/src/naludaq/board/
+-rw-r--r--   0 runner    (1001) docker     (123)    29652 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/board/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23941 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/board/board_inits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.677728 naludaq-0.18.0/src/naludaq/board/connections/
+-rw-r--r--   0 runner    (1001) docker     (123)    18932 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/board/connections/_FTDI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/board/connections/_MockUART.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14633 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/board/connections/_UART.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10093 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/board/connections/_USB.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/board/connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/board/connections/base_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/board/connections/base_ethernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/board/connections/base_serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/board/connections/connection_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/board/connections/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/board/connections/udp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.677728 naludaq-0.18.0/src/naludaq/board/initializers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/board/initializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/board/initializers/aardvarcv3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/board/initializers/aodsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/board/initializers/init_aodsv2_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/board/initializers/init_hdsocv1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/board/initializers/init_udc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/board/initializers/init_upac96.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/board/initializers/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17669 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/board/params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.681728 naludaq-0.18.0/src/naludaq/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10200 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/communication/_chip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/communication/_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/communication/_fpga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/communication/analog_registers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/communication/chip_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/communication/control_registers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/communication/digital_registers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/communication/i2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/communication/i2c_registers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20429 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/communication/registers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.681728 naludaq-0.18.0/src/naludaq/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/analog_debug_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.681728 naludaq-0.18.0/src/naludaq/controllers/biasing_mode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/biasing_mode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/biasing_mode/udc16.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.681728 naludaq-0.18.0/src/naludaq/controllers/board/
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/board/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/board/aodsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15230 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/board/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/board/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/board/oleas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/board/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/board/udc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/board/upac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9258 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/board/upac96.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.681728 naludaq-0.18.0/src/naludaq/controllers/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21101 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/connection/connection_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/connection/upac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/connection/upac96.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.681728 naludaq-0.18.0/src/naludaq/controllers/external_dac/
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/external_dac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/external_dac/ad5671.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/external_dac/ad5675.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11125 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/external_dac/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/external_dac/dac7578.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/external_dac/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/external_dac/i2c_dac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/external_dac/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/external_dac/upac32.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.685728 naludaq-0.18.0/src/naludaq/controllers/gainstages/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/gainstages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/gainstages/aodsv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/gainstages/oddsock_aods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.685728 naludaq-0.18.0/src/naludaq/controllers/peripherals/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/peripherals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/peripherals/aardvarcv3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/peripherals/aodsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/peripherals/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8973 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/peripherals/peripherals_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/peripherals/upac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/peripherals/upac96.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16209 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/project_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.685728 naludaq-0.18.0/src/naludaq/controllers/readout/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/readout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/readout/aardvarcv3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14273 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/readout/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/readout/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/readout/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/si5341_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.685728 naludaq-0.18.0/src/naludaq/controllers/tia/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/tia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/tia/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11997 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/tia/hdsoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.685728 naludaq-0.18.0/src/naludaq/controllers/trigger/
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/trigger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/trigger/aodsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/trigger/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8884 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/trigger/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/trigger/siread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/trigger/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/trigger/upac.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16581 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/trigger/upac96.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.685728 naludaq-0.18.0/src/naludaq/daq/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/daq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/daq/debugdaq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20482 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/daq/lightdaq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/daq/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.685728 naludaq-0.18.0/src/naludaq/daq/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/daq/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/daq/workers/answer_parser_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10475 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/daq/workers/csv_storage_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.689728 naludaq-0.18.0/src/naludaq/daq/workers/packager/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/daq/workers/packager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/daq/workers/packager/worker_packager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/daq/workers/packager/worker_packager_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10757 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/daq/workers/packager/worker_packager_hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/daq/workers/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/daq/workers/worker_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/daq/workers/worker_serial_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/daq/workers/worker_usb_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.689728 naludaq-0.18.0/src/naludaq/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/devices/eeprom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/devices/i2c_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/devices/ltc2990.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.689728 naludaq-0.18.0/src/naludaq/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/helpers/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/helpers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/helpers/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/helpers/register_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/helpers/semiton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/helpers/validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.689728 naludaq-0.18.0/src/naludaq/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22338 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/io/csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35939 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/io/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12900 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/io/io_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.689728 naludaq-0.18.0/src/naludaq/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/models/acq_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9728 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/models/acquisition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15839 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/naludaq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.689728 naludaq-0.18.0/src/naludaq/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10831 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/parsers/aardvarcv3_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/parsers/answer_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/parsers/aodsoc_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/parsers/asocv3_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8271 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/parsers/hdsoc_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.693728 naludaq-0.18.0/src/naludaq/parsers/headers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/parsers/headers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/parsers/headers/asoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/parsers/headers/asocv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/parsers/headers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/parsers/headers/siread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/parsers/headers/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/parsers/headers/upac32.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11956 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/parsers/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/parsers/trbhm_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/parsers/udc_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/parsers/upac96_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/parsers/upac_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.693728 naludaq-0.18.0/src/naludaq/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.693728 naludaq-0.18.0/src/naludaq/tools/adc2mv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/adc2mv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/adc2mv/adc_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16214 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/adc2mv/adc_linear_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/adc2mv/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/adc2mv/pre_adc2mv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/autoaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.693728 naludaq-0.18.0/src/naludaq/tools/autotrigger/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/autotrigger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/autotrigger/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/board_backup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.693728 naludaq-0.18.0/src/naludaq/tools/dac_sweep/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/dac_sweep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/dac_sweep/dac_sweep_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11823 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/data_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/ft60x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/ftdi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.693728 naludaq-0.18.0/src/naludaq/tools/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/optimizers/bayesian_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/optimizers/gainstagetuner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.693728 naludaq-0.18.0/src/naludaq/tools/pedestals/
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/pedestals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.697728 naludaq-0.18.0/src/naludaq/tools/pedestals/_new/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/pedestals/_new/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/pedestals/_new/aav3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25345 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/pedestals/_new/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/pedestals/_new/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/pedestals/aardvarcv3_pedestals_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/pedestals/hdsoc_pedestals_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/pedestals/pedestals_acq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34274 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/pedestals/pedestals_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/pedestals/pedestals_correcter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/pedestals/pedestals_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10912 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/pedestals/udc16_pedestals_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/pedestals/upac32_pedestals_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12497 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/pedestals/upac96_pedestals_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.697728 naludaq-0.18.0/src/naludaq/tools/threshold_scan/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/threshold_scan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/threshold_scan/hdsoc_thresholdscan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/threshold_scan/threshold_scan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.697728 naludaq-0.18.0/src/naludaq/tools/timing_cal/
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/timing_cal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/timing_cal/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/timing_cal/correcter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.697728 naludaq-0.18.0/src/naludaq/tools/waiter/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/waiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/waiter/eventwaiter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.673728 naludaq-0.18.0/src/naludaq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15635 2023-06-01 23:50:03.000000 naludaq-0.18.0/src/naludaq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-06-01 23:50:03.000000 naludaq-0.18.0/src/naludaq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 23:50:03.000000 naludaq-0.18.0/src/naludaq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-01 23:50:03.000000 naludaq-0.18.0/src/naludaq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-01 23:50:03.000000 naludaq-0.18.0/src/naludaq.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.697728 naludaq-0.18.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-01 23:49:47.000000 naludaq-0.18.0/tests/test_naludaq.py
```

### Comparing `naludaq-0.17.7/LICENSE.txt` & `naludaq-0.18.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/PKG-INFO` & `naludaq-0.18.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naludaq
-Version: 0.17.7
+Version: 0.18.0
 Summary: Backend package for Nalu Scientific hardware
 Home-page: 
 Author: Thomas Yang, Emily Lum, Terry Pham
 Author-email: Marcus Luck <marcus@naluscientific.com>, Mitchell Matsumori-Kelly <mitchell@naluscientific.com>, Alvin Yang <alvin@naluscientific.com>, Kenneth Lauritzen <kenneth@naluscientific.com>, Ben Rotter <ben@naluscientific.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

### Comparing `naludaq-0.17.7/README.md` & `naludaq-0.18.0/README.md`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/pyproject.toml` & `naludaq-0.18.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   { name="Terry Pham" },
 ]
 description = "Backend package for Nalu Scientific hardware"
 readme = "README.md"
 dynamic = ["version"]
 requires-python = ">=3.9"
 dependencies = [
-  "naluconfigs>=10.6",
+  "naluconfigs>=11.0.0",
   "ftd3xx>=1.0",
   "naludaq_rs>=0.1.5",
   "deprecation",
   "ftd2xx>=1.1.2",
   "h5py",
   "numpy<1.24",
   "pyserial==3.4",
```

### Comparing `naludaq-0.17.7/setup.py` & `naludaq-0.18.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     author_email="marcus@naluscientific.com",
     description="Backend package for Nalu hardware",
     python_requires=">=3.9",
     long_description=readme(),
     long_description_content_type="text/markdown",
     url="",
     install_requires=[
-        "naluconfigs>=10.3",
+        "naluconfigs>=11.0.0",
         "ftd3xx>=1.0",
         "naludaq_rs>=0.1.5",
         "deprecation",
         "ftd2xx>=1.1.2",
         "h5py",
         "numpy<1.24",
         "pyserial==3.4",
```

### Comparing `naludaq-0.17.7/src/naludaq/backend/client.py` & `naludaq-0.18.0/src/naludaq/backend/client.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/backend/context.py` & `naludaq-0.18.0/src/naludaq/backend/context.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/backend/exceptions.py` & `naludaq-0.18.0/src/naludaq/backend/exceptions.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/backend/managers/acquisitions.py` & `naludaq-0.18.0/src/naludaq/backend/managers/acquisitions.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/backend/managers/config.py` & `naludaq-0.18.0/src/naludaq/backend/managers/config.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/backend/managers/connection.py` & `naludaq-0.18.0/src/naludaq/backend/managers/connection.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/backend/managers/io.py` & `naludaq-0.18.0/src/naludaq/backend/managers/io.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/backend/models/acquisition.py` & `naludaq-0.18.0/src/naludaq/backend/models/acquisition.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/backend/models/device.py` & `naludaq-0.18.0/src/naludaq/backend/models/device.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/board/__init__.py` & `naludaq-0.18.0/src/naludaq/board/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,14 +161,37 @@
         Doesn't have any validation, is used both to set and get values.
         To set, simply run board.dac_values[chan] = value
         NO validations!
         """
         return self.params["ext_dac"]["channels"]
 
     @property
+    def available_chips(self) -> int:
+        """Get the number of chips on this board"""
+        return len(self.params.get("chips", [0]))
+
+    @property
+    def selected_chips(self) -> list[int]:
+        """Get/set the selected chips for this board.
+
+        This is a pass through for the communication layer's select_chips / selected_chips functions.
+        Selecting chips is done by toggling control registers to mask I/O from the chips that aren't selected.
+        Make sure to restore the selected chips after you're finished with what you're doing.
+        """
+        from naludaq.communication import selected_chips
+
+        return selected_chips(self)
+
+    @selected_chips.setter
+    def selected_chips(self, chips: list[int]):
+        from naludaq.communication.chip_selection import select_chips
+
+        select_chips(self, chips)
+
+    @property
     def channels(self):
         """Get the channels from the params."""
         return self.params["channels"]
 
     @property
     def trigger_values(self):
         """Get/Set Trigger value list
```

### Comparing `naludaq-0.17.7/src/naludaq/board/board_inits.py` & `naludaq-0.18.0/src/naludaq/board/board_inits.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/board/connections/_FTDI.py` & `naludaq-0.18.0/src/naludaq/board/connections/_FTDI.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/board/connections/_MockUART.py` & `naludaq-0.18.0/src/naludaq/board/connections/_MockUART.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/board/connections/_UART.py` & `naludaq-0.18.0/src/naludaq/board/connections/_UART.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/board/connections/_USB.py` & `naludaq-0.18.0/src/naludaq/board/connections/_USB.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/board/connections/base_connection.py` & `naludaq-0.18.0/src/naludaq/board/connections/base_connection.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/board/connections/connection_factory.py` & `naludaq-0.18.0/src/naludaq/board/connections/connection_factory.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/board/connections/tcp.py` & `naludaq-0.18.0/src/naludaq/board/connections/tcp.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/board/connections/udp.py` & `naludaq-0.18.0/src/naludaq/board/connections/udp.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/board/initializers/__init__.py` & `naludaq-0.18.0/src/naludaq/board/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/board/initializers/aardvarcv3.py` & `naludaq-0.18.0/src/naludaq/board/initializers/aardvarcv3.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/board/initializers/aodsoc.py` & `naludaq-0.18.0/src/naludaq/board/initializers/aodsoc.py`

 * *Files 12% similar despite different names*

```diff
@@ -98,15 +98,14 @@
         self.digital_registers.write_all()
 
     @log_function(logger)
     def _analog_startup(self):
         """Start the analog side of the chip by programming all registers."""
         self.analog_registers.write_all()
         self._dll_startup()
-        self._set_default_isel()
 
     @log_function(logger)
     def _dll_startup(self):
         """Starting the delay line on the analog side.
 
         Sets and unsets vanbuff to get the dll going and
         changes the vadjp values to ensure proper SST duty cycle once locked.
@@ -124,24 +123,14 @@
             get_dac_controller(self.board).set_single_dac(channel, value)
 
     def _get_dac_values(self) -> dict:
         """Return a dict with all the {channels: dac_values}"""
         return self.board.params.get("ext_dac", {}).get("channels", {})
 
     @log_function(logger)
-    def _set_default_isel(self):
-        """Set the default isel for each chip individually using the board params"""
-        isel_values = self.board.params["default_isel"]
-
-        for chip, isel in isel_values.items():
-            self._set_chip_tx_enabled([chip])
-            self.analog_write("isel", isel)
-        self._set_chip_tx_enabled()
-
-    @log_function(logger)
     def _init_i2c_devices(self):
         """Initialize I2C devices on the eval card"""
         sendI2cCommand(self.board, "30", ["05"])  # tempSensor to temp reg
         sendI2cCommand(self.board, "D0", ["00111011"])  # set up current sense ADC
 
     def _set_chip_tx_enabled(self, chips: list = [0, 1]):
         """Set whether the TX lines are enabled for each chip.
```

### Comparing `naludaq-0.17.7/src/naludaq/board/initializers/init_aodsv2_eval.py` & `naludaq-0.18.0/src/naludaq/board/initializers/init_aodsv2_eval.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/board/initializers/init_hdsocv1.py` & `naludaq-0.18.0/src/naludaq/board/initializers/init_hdsocv1.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/board/initializers/init_udc.py` & `naludaq-0.18.0/src/naludaq/board/initializers/init_udc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/board/initializers/init_upac96.py` & `naludaq-0.18.0/src/naludaq/board/initializers/init_upac96.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 It contains all UPAC96 specific startup sequence
 """
 import functools
 import logging
 import time
 
 from naludaq.board import initializers
+from naludaq.communication import DigitalRegisters
 from naludaq.controllers import get_board_controller, get_dac_controller
 
 logger = logging.getLogger(__name__)
 
 
 def func_print(func):
     @functools.wraps(func)
@@ -139,23 +140,16 @@
     @func_print
     def _write_chip_ids(self):
         """Write the chip ids to the digital registers
 
         This will allow the parser to recognize which chip the return data
         belongs to.
         """
-        udc_rxout_enable = (
-            self.board.registers["control_registers"]
-            .get("udc_rxout_enable", {})
-            .get("value", 0x3F)
-        )
         for chip in range(self.num_chips):
-            self.control_registers.write("udc_rxout_enable", 2**chip)
-            self.digital_registers.write("chip_id", chip)
-        self.control_registers.write("udc_rxout_enable", udc_rxout_enable)
+            DigitalRegisters(self.board, chip).write("chip_id", chip)
 
     @func_print
     def _analog_startup(self):
         """Start the analog side of the chip"""
         self.analog_registers.write_all()
 
         self._write_reg1()
```

### Comparing `naludaq-0.17.7/src/naludaq/board/params.py` & `naludaq-0.18.0/src/naludaq/board/params.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/communication/__init__.py` & `naludaq-0.18.0/src/naludaq/communication/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 - i2c
 - serial
 
 """
 from logging import getLogger
 
 from .analog_registers import AnalogRegisters
+from .chip_selection import select_chips, select_chips_commands, selected_chips
 from .control_registers import ControlRegisters
 from .digital_registers import DigitalRegisters
 from .i2c import *
 from .i2c_registers import I2CRegisters
 
 LOGGER = getLogger(__name__)
```

### Comparing `naludaq-0.17.7/src/naludaq/communication/analog_registers.py` & `naludaq-0.18.0/src/naludaq/communication/analog_registers.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,99 +23,96 @@
 - write
 - write2addr
 
 
 """
 from logging import getLogger
 
-from naludaq.communication import registers
+from naludaq.communication._chip import ChipRegisters
 
 LOGGER = getLogger(__name__)
 
 
-class AnalogRegisters(registers.WriteRegisters):
-    def __init__(self, board):
-        super().__init__(board, "analog_registers")
-
-        self._write_cmd = (
-            0xB00  # Standard analog write address, changes with board/mode.
-        )
-        self.width_cmd = 3
-        self.width_addr = 2  # hex char
-        self.width_val = 3  # hex char
+class AnalogRegisters(ChipRegisters):
+    def __init__(self, board, chips: "int | list[int]" = None):
+        """Registers controlling the analog part of the ASIC(s).
+
+        For a more thorough explanation of the multichip aspect and its implications,
+        see the `multichip` module.
+
+        Args:
+            board (Board): board object
+            chips (int | list[int] | None): chip(s) to write to. If None, all chips are assumed.
+        """
+        super().__init__(board, "analog_registers", chips)
+        self._write_cmd = 0xB00
+        self._width_cmd = 3
+        self._width_addr = 2  # hex char
+        self._width_val = 3  # hex char
 
     # READ #########################################################
 
-    def _get_value_from_addr(self, addr):
+    def _addr_value(self, addr: str, chip: int):
+        """Reimplemented to correct strobe values."""
+        if self.board.params.get("strobe_values_correction", False):
+            result = self._correct_strobes(addr, chip)
+        else:
+            result = super()._addr_value(addr, chip)
+        return result
+
+    def _correct_strobes(self, addr: str, chip: int) -> int:
         """Generate the value from the hex address.
 
         An address can contain multiple registers.
         Generate the value depending on the bit positions of all registers on the address.
 
         Args:
-            addr(str): Hex value of the address, 2 hex char long.
+            addr (str): Hex value of the address, 2 hex char long.
 
         Returns:
-            integer value of the combined registers.
+            int: value of the combined registers.
 
         Raises:
             AttributeError if the address is not valid.
         """
         addr = addr.upper()
-        value = 0
-        failed = True
         strobe_correction_keys = self.board.params.get("strobe_correction_keys", [])
-        strobe_values_correction = self.board.params.get(
-            "strobe_values_correction", False
-        )
-        for key, val in self.registers.items():
-
-            if val["address"].upper() != addr:
-                continue
-            failed = False
-            key_value = val["value"]
-            key_pos = val["bitposition"]
-            key_width = val["bitwidth"]
+        value = 0
+        for name, register in self.registers_on_address(addr).items():
+            reg_value = register["value"][chip]
+            reg_pos = register["bitposition"]
+            reg_width = register["bitwidth"]
 
             # FIX TIMING REGS, ACCORDING TO BOARD PARAMETER timing_correction
-            if strobe_values_correction and key in strobe_correction_keys:
-                key_value = self._fix_timing(key_value)
-
-            value += 2**key_pos * (int(key_value) % (2**key_width))
-        if failed is True:
-            raise AttributeError("Address is not found")
-
+            if name in strobe_correction_keys:
+                reg_value = self._fix_timing(reg_value)
+            value += 2**reg_pos * (int(reg_value) % (2**reg_width))
         return value
 
-    def _generate_write_request(self, addr: str, value: int) -> str:
+    def _generate_write_atom(self, addr: str, value: int) -> str:
         """Generate the string to send to the board.
 
         OVERLOAD the standard way of generating the command since the analog command parsing
         sometimes
 
         Abstracts the model differences away from the main code, AARDVARCv2 got a timing hack.
 
         Args:
             board(obj)
             name(str): name of the analog register
             value(): Value to set the register to.
         """
-
         write_addr = f"{self._write_cmd:X}"
         cmd_addr = addr
-
         if len(addr) == 3:
             write_addr = f"B{addr[0]}0"
             cmd_addr = f"{addr[1:]}"
-
         if isinstance(value, (int, bool)):
-            value = f"{value:X}".zfill(self.width_val)
-
+            value = f"{value:X}".zfill(self._width_val)
         command = f"{write_addr}{cmd_addr}{value}"  # First 5 hex chars, address should be 3 hex. B001c
-
         return command
 
     @staticmethod
     def _fix_timing(in_value: int):
         """The timing signal data mux is all mixed up for simplicity of routing, so this fixes it
 
         Don't use unless you know what it does. Contains hardcoded values.
```

### Comparing `naludaq-0.17.7/src/naludaq/communication/control_registers.py` & `naludaq-0.18.0/src/naludaq/communication/control_registers.py`

 * *Files 16% similar despite different names*

```diff
@@ -34,27 +34,22 @@
     dc = DigitalRegisters(board)
     dc.read("regname")
     dc.write("regname", intvalue)
 
 """
 from logging import getLogger
 
-from naludaq.communication import registers
+from naludaq.communication import _fpga
+from naludaq.helpers.semiton import SemitonABC
 
 LOGGER = getLogger(__name__)
 
 
-class ControlRegisters(registers.ReadRegisters, registers.WriteRegisters):
+class ControlRegisters(_fpga.FpgaRegisters, SemitonABC):
     """Control Registers
 
     Attributes:
         board:
     """
 
     def __init__(self, board):
         super().__init__(board, "control_registers")
-
-        self._write_cmd = 0xAF
-        self._read_cmd = 0xAD
-        self.width_cmd = 2
-        self.width_addr = 2  # hex char
-        self.width_val = 4  # hex char
```

### Comparing `naludaq-0.17.7/src/naludaq/communication/i2c.py` & `naludaq-0.18.0/src/naludaq/communication/i2c.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/communication/i2c_registers.py` & `naludaq-0.18.0/src/naludaq/communication/i2c_registers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,37 @@
 import logging
 
-from naludaq.backend.managers.io import BoardIoManager
-from naludaq.communication import registers
+from naludaq.communication import _fpga
 from naludaq.helpers.exceptions import I2CError, InvalidBoardModelError
 from naludaq.helpers.semiton import SemitonABC
 
 logger = logging.getLogger("naludaq.i2c_registers")
 
 
-class I2CRegisters(registers.ReadRegisters, registers.WriteRegisters, SemitonABC):
+class I2CRegisters(_fpga.FpgaRegisters, SemitonABC):
     def __init__(self, board):
         """Communication with I2C devices through FPGA registers.
 
         Args:
             board (Board): the board object.
         """
         if "i2c_registers" not in board.registers:
             raise InvalidBoardModelError(
                 f'Board "{board.model}" is missing I2C registers or does not support I2C'
             )
-
         super().__init__(board, "i2c_registers")
-        self._write_cmd = 0xAF
-        self._read_cmd = 0xAD
-        self.width_cmd = 2
-        self.width_addr = 2  # hex char
-        self.width_val = 4  # hex char
 
         # These are the same on all valid boards
         self._i2c_transmit_command = board.params.get("i2c", {}).get(
             "transmit_command", "CA000000"
         )
 
     def transmit_command(self):
-        """Send the command which tells the board to transmit data over the I2C bus"""
+        """Send the command which tells the board to transmit data over the I2C bus.
+
+        Raises:
+            I2CError: if the command fails to send.
+        """
         try:
-            # Tell board to fire i2c commands
-            if self.board.using_new_backend:
-                BoardIoManager(self.board).write(self._i2c_transmit_command)
-            else:
-                self.board.connection.send(self._i2c_transmit_command)
+            self._send_command(self._i2c_transmit_command)
         except Exception as e:
             raise I2CError("Failed to initiate I2C send") from e
```

### Comparing `naludaq-0.17.7/src/naludaq/communication/registers.py` & `naludaq-0.18.0/src/naludaq/communication/registers.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """Base class for registers.
 """
+import abc
 from abc import ABC
 from collections import defaultdict
 from functools import wraps
 from logging import getLogger
-from typing import Iterable
+from typing import Iterable, List
 
 from naludaq.backend.exceptions import ConnectionError
 from naludaq.backend.managers.connection import ConnectionManager
 from naludaq.backend.managers.io import BoardIoManager
 from naludaq.helpers.exceptions import InvalidRegisterError
 
+from . import _common as helpers
+
 LOGGER = getLogger(__name__)
 
 
 def clear_buffer(func):
     @wraps(func)
     def wrapper(self, *args, **kwargs):
         """Clears the board buffer before"""
@@ -29,18 +32,28 @@
 
         return rv
 
     return wrapper
 
 
 class Registers(ABC):
-    """Base class for registers.
+    """Base class for communication with registers.
+    This class should not be used directly; use one of the subclasses instead.
+
+    Inheritence tree:
 
-    By inehriting this class it will be compatible with the other register classes.
-    This standardizes the way register updates are called.
+    ```mermaid
+    graph TD;
+        Registers --> ChipRegisters
+        Registers --> FpgaRegisters
+        ChipRegisters --> DigitalRegisters
+        ChipRegisters --> AnalogRegisters
+        FpgaRegisters --> ControlRegisters
+        FpgaRegisters --> I2CRegisters
+    ```
 
     Atrributes:
     -----------
 
         board: The board to update the registers on.
         width_cmd (int): width of the command type in hex chars
         width_addr (int): width of the address in hex chars
@@ -52,18 +65,18 @@
     def __init__(self, board, register_type: str):
         self.board = board
         self._register_type = register_type
         if not isinstance(getattr(board, "registers", None), dict):
             raise InvalidRegisterError("The board is lacking valid registers")
         if not board.registers.get(register_type, None):
             raise InvalidRegisterError(f"The registers is lacking {register_type}")
-        self.width_cmd = 3
-        self.width_addr = 2  # hex char
-        self.width_val = 3  # hex char
-        self.width_total = 8  # common firmware
+        self._width_cmd = 3
+        self._width_addr = 2  # hex char
+        self._width_val = 3  # hex char
+        self._width_total = 8  # common firmware
 
         self._stopword = None
         self.stopword = self.board.params.get(
             "register_stop_word",
             self.board.params["stop_word"],
         )
 
@@ -87,18 +100,32 @@
         self._stopword = value
 
     @property
     def registers(self) -> dict:
         """Shortcut to board registers"""
         return self.board.registers[self._register_type]
 
-    @property
-    def width_val_bits(self):
-        """Maximum bits a value can be based on command size"""
-        return self.width_val * 4
+    @abc.abstractmethod
+    def set(self, name: str, value: int):
+        """Set the value of a register without writing to the board.
+
+        Args:
+            name (str): Name of the register.
+            value (int): Value to set the register to.
+        """
+
+    @abc.abstractmethod
+    def set_addr(self, addr: "str | int", value: int):
+        """Set the value of registers on the given address without
+        writing to the board.
+
+        Args:
+            addr (str | int): Address of the register.
+            value (int): Value to set the register to.
+        """
 
     # VALIDATIONS ############################################################
     #
     ##########################################################################
     def _validate_addr_or_raise(self, addr: str):
         """Validate the address type and make sure it exists.
 
@@ -107,16 +134,15 @@
 
         Raises:
             ValueError if addr is not a valid hex or if it doesn't exist in register
             TypeError if addr is not a string or int
         """
         if not isinstance(addr, str):
             raise TypeError("Register number needs to be an integer")
-
-        if addr.zfill(self.width_addr).upper() not in self.list_addresses():
+        if addr.zfill(self._width_addr).upper() not in self.list_addresses():
             raise ValueError(f"Address {addr} does not exist in {self._register_type}")
 
     def _validate_name_or_raise(self, name):
         """Name is a user input, make sure it's valid.
 
         Args:
             name(str): Name of the analog register.
@@ -183,15 +209,15 @@
 
         addr = self.registers.get(name.casefold(), False)
         if addr is False:
             raise InvalidRegisterError(f"{name} is not a valid register.")
         addr = addr["address"]
         if isinstance(addr, int):
             addr = f"{addr:X}"  # pragma: no cover
-        addr = addr.zfill(self.width_addr)
+        addr = addr.zfill(self._width_addr)
         return addr.upper()
 
     def _validate_command_or_raise(self, command: str):
         """Make sure a generated command is of the right length."""
         if len(command) != self.width_total:
             raise ValueError(
                 f"Generated command is invalid. A command must be {self.width_total} char, got {command} or length {len(command)}"
@@ -215,26 +241,35 @@
         same way as the registers file.
 
         Returns:
             A dict containing all registers
         """
         return self.registers
 
-    def list_addresses(self):
+    def list_addresses(self) -> List[str]:
         """Generate a list of all available addresses.
 
         This is useful since an address can contain multiple registers.
         The register name can correspond to one or many bits at a specific address.
 
         Returns:
             List of available addresses in hex (str)
         """
         reg_addr = {value["address"].upper() for value in self.registers.values()}
         return sorted(list(reg_addr), key=lambda x: int(x, 16))
 
+    def registers_on_address(self, addr: str) -> dict[str, dict]:
+        self._validate_addr_or_raise(addr)
+        addr = helpers.normalize_address(addr, self._width_addr)
+        return {
+            name: value
+            for name, value in self.registers.items()
+            if value["address"].upper() == addr
+        }
+
     def show(self, name: str) -> str:
         """Returns the internal contents of a register.
 
         Args:
             name (str): The name of the register
 
         Returns:
@@ -252,358 +287,140 @@
         """Send request to the board"""
         if self.board.using_new_backend:
             BoardIoManager(self.board).write(cmd)
         else:
             self.board.connection.send(cmd)
 
     def __repr__(self):
-        return f"{self.registers}(board = {self.board})"  # pragma: no cover
-
-
-class WriteRegisters(Registers):
-    """Writeable registers
-
-    Adds the trait to write registers
+        return f"{type(self).__name__}: {self.registers}(board = {self.board})"  # pragma: no cover
 
-    Functions:
-    ---------
-
-        - ``write(name, value)``
-        - ``write_addr(addr, value)``
-        - ``generate_write(name, value)``
-        - ``generate_write_addr(name, value)``
-        - ``write_all()``
-
-    Attributes:
-    -----------
 
-        _write_cmd: the write command as a hex eg. ``0xAD``
-
-    """
-
-    _write_cmd = None
-
-    # WRITE ##################################################################
+class WriteRegistersABC(Registers):
     def write(self, name: str, value: int = None):
-        """Set a register to a value.
-
-        Update the internal stored reg values and
-        the registers on the hardware simultaniously.
-
-        Args:
-            board
-            name(str): Name of the register.
-            value(int, bool): Value of the register.
-
-        Raises:
-            ValueError if name is not in register.
-            TypeError if name is not a str.
-        """
-        self._validate_name_or_raise(name)
-        name = name.lower()
         if value is not None:
-            self._update_software_register(name, value)
+            self.set(name, value)
+        command = self.generate_write(name, value)
+        self._send_command(command)
 
-        addr = self._get_addr_from_name_or_raise(name)
+    def write_addr(self, addr: "int | str", value: int = None):
+        if value is not None:
+            self.set_addr(addr, value)
+        command = self.generate_write_addr(addr, value)
+        self._send_command(command)
 
-        self._write_register_or_raise(addr)
+    def write_all(self):
+        for addr in self.list_addresses():
+            self.write_addr(addr)
 
     def write_many(self, value_map: dict[str, int]):
         """Write several registers at once.
 
         Args:
             registers (dict[str, int]): mapping of register values to names
         """
         self._validate_value_map_or_raise(value_map)
 
         # update all software registers first to prevent generate_write
         # from using potentially old register values in subsequent writes
         for name, value in value_map.items():
-            self._update_software_register(name, value)
+            self.set(name, value)
 
         addresses = {
             self._get_addr_from_name_or_raise(name) for name in value_map.keys()
         }
         commands = [self.generate_write_addr(addr) for addr in addresses]
         command = "".join(commands)
         self._send_command(command)
 
-    def write_addr(self, addr: "int|str", value=None):
-        """Updates value on both board from register addr.
-
-        You better know what you are doing if you use this function since it'll
-        overwrite the entire address.
-
-        This means several registers might get overwritten!
-
-        If a value is left out the function will use whatever value is previously stored.
-        The intent is to be able to write to registers that have no name yet.
-
-        Args:
-            addr (hex or int): the addr can either be hex or integer.
-            value: the value sent to the board.
-
-        Raises:
-            ValueError if value is not a positive integer
-            TypeError if name is not a str.
-        """
-        if isinstance(addr, int):
-            addr = f"{addr:X}"
-        self._validate_addr_or_raise(addr)
-        addr = addr.zfill(self.width_addr)
-        addr = addr.upper()  # All hex is uppercase
-
-        if value is not None:
-            self._update_software_register_addr(addr, value)
-
-        self._write_register_or_raise(addr)
-
-    def write_all(self):
-        """Write all software registers to the hardware.
-
-        Writes all registers on the board-object to the physical board.
-        It will send all the commands one by one to the board.
-        Effectively syncing the software registers with the board by
-        sending all values in the software to the board.
-        """
-        if self.board.using_new_backend:
-            return self._write_all_new()
-        for addr in self.list_addresses():
-            self._write_register_or_raise(addr)
-
-    def _write_all_new(self, batch_size: int = 32):
-        """Version of the write_all command that writes commands simulataneously.
-
-        Args:
-            batches (int): number of commands per batch to send.
-                Don't make this too high, since serial/d2xx connections are
-                synchronous and so large batches can result in a request timeout
-                before the server finishes writing.
-        """
-        addresses = self.list_addresses()
-        command_batches = [
-            [self.generate_write_addr(addr) for addr in addresses[i : i + batch_size]]
-            for i in range(0, len(addresses), batch_size)
-        ]
-        for commands in command_batches:
-            BoardIoManager(self.board).write_all(commands)
-
-    def _write_register_or_raise(self, addr):
-        """Write a control register to the board using the register addr.
-
-        Uses the value stored in the software and sends to the hardware.
-
-        Args:
-            addr(str): The hex address for the register as str.
-
-        Raises:
-            TypeError: if addr is not an str
-            ValueError: if reg_num is not a valid register.
-        """
-        addr = addr.upper()
-        self._validate_addr_or_raise(addr)
-        value = self._get_value_from_addr(addr)
-
-        cmd = self.generate_write_addr(addr, value)
-
-        self._send_command(cmd)
-
-    # GENERATE ###############################################################
-    #
-    # A series of commands the generates the commands to send and returns a hex str.
-    #
-    ##########################################################################
+    @abc.abstractmethod
     def generate_write(self, name: str, value: int = None) -> str:
-        """Generates a command string for writing to a register.
-
-        This function does not change any hardware or software registers.
+        pass
 
-        Args:
-            name (str): the name of the register
-            value (int): the value, or None to use the value held in the software register.
+    @abc.abstractmethod
+    def generate_write_addr(self, addr: str, value: int = None) -> str:
+        pass
 
-        Returns:
-            The command string
-
-        Raises:
-            ValueError if the address, value or generated command is invalid
-            TypeError if the value is an invalid type
-        """
-        self._validate_name_or_raise(name)
-        name = name.lower()
-        addr = self._get_addr_from_name_or_raise(name)
-        # Fix total comand for address
-
-        if value is not None:
-            addr_val = int(self._get_value_from_addr(addr))
-            bw = self.registers[name]["bitwidth"]
-            bp = self.registers[name]["bitposition"]
-            self._validate_value_or_raise(value, bw)
-            mask = (2**bw - 1) << bp
-            value = addr_val - (addr_val & mask) + ((value & (2**bw - 1)) << bp)
-
-        try:
-            cmd = self.generate_write_addr(addr=addr, value=value)
-        except (ValueError, TypeError, AttributeError):  # pragma: no cover
-            raise  # pragma: no cover
-        return cmd
+    def _generate_write_atom(self, addr: str, value: int) -> str:
+        cmd = f"{self._write_cmd:X}"
+        cmd_addr = addr.zfill(self._width_addr)
+        val = f"{value:X}".zfill(self._width_val)
+        command = f"{cmd}{cmd_addr}{val}"
+        return command.upper()
 
-    def generate_write_addr(self, addr: "int|str", value: int = None) -> str:
-        """Generates a command string for writing to a register.
 
-        This function does not change any hardware or software registers.
+class ReadRegistersABC(Registers):
+    def read(self, name: str) -> dict:
+        """Read from a register with a name.
 
         Args:
-            addr (str): the address of the register
-            value (int): the value, or None to use the value held in the software register.
-
-        Returns:
-            The command string
+            name: Name of the register.
 
         Raises:
-            ValueError if the address, value or generated command is invalid
-            TypeError if the value is an invalid type
+            ValueError if name is not in register.
+            TypeError if name is not a str.
         """
-        if isinstance(addr, int):
-            addr = f"{addr:X}"
-        if not isinstance(addr, str):
-            raise TypeError("address should be either a hex string or hex (0xADDR)")
-        addr = addr.zfill(self.width_addr)
-        addr = addr.upper()
-
-        if value is None:
-            try:
-                value = self._get_value_from_addr(addr)
-            except AttributeError:
-                raise ValueError(f"No value found for address {addr}")
-
-        self._validate_value_or_raise(value, bitwidth=self.width_val_bits)
-
-        command = self._generate_write_request(addr, value)
-        self._validate_command_or_raise(command)
-
-        return command
-
-    def _generate_write_request(self, addr: str, value: int) -> str:
-        """Generate the write command"""
-
-        cmd = f"{self._write_cmd:X}"
-        cmd_addr = addr.zfill(self.width_addr)
-        val = f"{value:X}".zfill(self.width_val)
-        command = f"{cmd}{cmd_addr}{val}"
-        return command.upper()
+        self._validate_name_or_raise(name)
+        addr = self.registers[name]["address"]
+        return self.read_addr_named(addr)[name]
 
-    def _update_software_register(self, name: str, value: int):
-        """Set boardparam digital register, do not change the state of the FPGA
+    def read_addr(self, addr: "int | str") -> int:
+        """Read an address and return the value.
 
         Args:
-            name: Register name.
-            value: Register value.
+            addr (str | int): 8-bit address to read as either int or hex.
         """
-        name = name.lower()
-        self._validate_name_or_raise(name)
-        self._validate_value_or_raise(value, bitwidth=self.registers[name]["bitwidth"])
-
-        self.registers[name]["value"] = value
-
-    def _update_software_register_addr(self, addr: str, value: int):
-        """Update any registers sharing the addr with their part of the value"""
-        self._validate_value_or_raise(
-            value, bitwidth=self.width_val_bits
-        )  # hex is 4 bits
-        for reg in self.list_registers().values():
-            if reg["address"].lower() != addr.lower():
-                continue
-            val = value >> reg["bitposition"]
-            val &= 2 ** reg["bitwidth"] - 1
-            reg["value"] = val
+        command = self.generate_read_addr(addr)
+        return self._read_response(command)
 
-    def _get_value_from_addr(self, addr):
-        """Generate the value from the hex address.
-
-        An address can contain multiple registers.
-        Generate the value depending on the bit positions of all registers on the address.
+    def read_addr_named(self, addr: "int | str") -> dict:
+        """Read an address and return the register dicts for all registers
+        on that address.
 
         Args:
-            addr(str): Hex value of the address, 2 hex char long.
+            addr (str | int): address to read as either int or hex.
 
         Returns:
-            integer value of the combined registers.
-
-        Raises:
-            AttributeError if address is not in the registers.
+            dict: {name: register_dict}
         """
-        regs = [
-            val
-            for val in self.registers.values()
-            if val["address"].upper() == addr.upper()
-        ]
-        if len(regs) == 0:
-            raise AttributeError("Address not found")
-
-        value = 0
-        for val in regs:
-            # key_value, key_addr, key_pos, key_width, _ = val
-            key_value = val["value"]
-            val["address"]
-            key_pos = val["bitposition"]
-            key_width = val["bitwidth"]
-
-            # if key_addr == addr:
-            value += 2**key_pos * (int(key_value) % (2**key_width))
-
-        return value
-
-
-class ReadRegisters(Registers):
-    """Readable registers
-
-    Adds the ability to read registers
-
-
-    Functions:
-    ---------
-
-        - ``read(name)``
-        - ``read_addr(addr)``
-        - ``generate_read(name)``
-        - ``generate_read_addr(name)``
-        - ``read_all()``
-
-    Attributes:
-    -----------
-
-        _read_cmd: the read address as a hex eg. ``0xAF``
-
-    """
+        addr_value = self.read_addr(addr)
+        return {
+            name: reg.copy() | {"value": helpers.full_to_partial_value(addr_value, reg)}
+            for name, reg in self.registers.items()
+            if reg["address"].upper() == addr.upper()
+        }
 
-    _read_cmd = None
+    def read_all(self) -> list:
+        """Read all digital registers from the board.
 
-    @clear_buffer
-    def read(self, name: str) -> int:
-        """Read from a register with a name.
+        Reads the values based on the register number rather than the name.
 
         Args:
-            name: Name of the register.
+            board
 
-        Raises:
-            ValueError if name is not in register.
-            TypeError if name is not a str.
+        Returns:
+            dictionary with {reg_num: values,}
         """
-        self._validate_name_or_raise(name)
-        name = name.lower()
-        reg_addr = self._get_addr_from_name_or_raise(name)
-
-        return_value = self._read_from_hardware(reg_addr)
-        reg = self._parse_response_to_names(return_value, reg_addr)
-
-        return reg[name]
+        if self.board.using_new_backend:
+            addresses = self.list_addresses()
+            commands = [self.generate_read_addr(addr) for addr in addresses]
+            values = {}
+            answers = BoardIoManager(self.board).read_all(commands)
+            for address, answer in zip(addresses, answers):
+                parsed_answer = self._parse_response(answer)["value"]
+                reg = self._registers_from_addr_value(address, parsed_answer)
+                values.update(reg)
+        else:
+            values = {
+                name: register
+                for addr in self.list_addresses()
+                for name, register in self.read_addr_named(addr).items()
+            }
+        return values
 
-    @clear_buffer
-    def read_many(self, names: list[str]) -> list[str]:
+    def read_many(self, names: list[str]) -> dict:
         """Read several registers at once.
 
         Do not use this function to read the same register multiple times,
         as older values will be discarded.
 
         Args:
             names (Iterable[str]): names of registers to read
@@ -632,162 +449,82 @@
             responses = BoardIoManager(self.board).read_all(read_cmds)
         except TimeoutError:
             raise
 
         # parse responses into registers by address
         values = {}
         for (addr, addr_names), response in zip(addresses.items(), responses):
-            response = self._parse_answer(response)["value"]
-            response = self._parse_response_to_names(response, addr)
+            addr_value = self._parse_response(response)["value"]
+            registers = self._registers_from_addr_value(addr, addr_value)
             for name in addr_names:
-                values[name] = response[name]["value"]
+                values[name] = registers[name]["value"]
 
         sorted_values = [values[name] for name in names]
         return sorted_values
 
-    @clear_buffer
-    def read_all(self, overwrite: bool = False):
-        """Read all digital registers from the board.
-
-        Reads the values based on the register number rather than the name.
-
-        Args:
-            board
-
-        Returns:
-            dictionary with {reg_num: values,}
-        """
-        if self.board.using_new_backend:
-            return self._read_all_new()
-        values = dict()
-        for reg_addr in self.list_addresses():
-            response = self._read_from_hardware(reg_addr)
-
-            reg = self._parse_response_to_names(response, reg_addr)
-            values.update(reg)
-        return values
-
-    def _read_all_new(self):
-        """Read all registers [BETA].
-
-        Sends read commands all at once and parses the results.
-
-        Returns:
-            dict: register values structured as {reg_name: reg dict}
-        """
-        addresses = self.list_addresses()
-        commands = [self.generate_read_addr(addr) for addr in addresses]
-        values = {}
-        answers = BoardIoManager(self.board).read_all(commands)
-        for address, answer in zip(addresses, answers):
-            parsed_answer = self._parse_answer(answer)["value"]
-            reg = self._parse_response_to_names(parsed_answer, address)
-            values.update(reg)
-        return values
-
-    @clear_buffer
-    def read_addr(self, addr: int) -> int:
-        """Read an address and return the value.
-
-        Args:
-            addr(hex|int): 8-bit address to read as either int or hex."""
-        addr = f"{addr:02X}".upper()
-        return self._read_from_hardware(addr)
-
     def generate_read(self, name: str) -> str:
         """Generate and return the read command as hex"""
-        self._validate_name_or_raise(name)
-        name = name.lower()
-        addr = self._get_addr_from_name_or_raise(name)
-        cmd = self._generate_read_request(addr)
-        return cmd
+        return self.generate_read_addr(self.registers[name]["address"])
 
-    def generate_read_addr(self, addr: "int|str") -> str:
-        """Generate and return the read addr command as HEX"""
-        if isinstance(addr, int):
-            addr = f"{addr:X}"
-        self._validate_addr_or_raise(addr)
-        addr = addr.upper()
-        cmd = self._generate_read_request(addr)
-        return cmd.upper()
+    @abc.abstractmethod
+    def generate_read_addr(self, addr: "int | str") -> str:
+        """Generate and return the read addr command as hex"""
+        pass
+
+    def _generate_read_atom(self, addr: "int | str") -> str:
+        cmd = f"{self._read_cmd:X}"
+        cmd_addr = addr.zfill(self._width_addr)
+        val = "0".zfill(self._width_val)
+        command = f"{cmd}{cmd_addr}{val}"
+        return command.upper()
 
     @clear_buffer
-    def _read_from_hardware(self, addr: str, *args, **kwargs) -> int:
-        """Read from a digital read register with an address
+    def _read_response(self, command: str) -> int:
+        """Send a read command to the board and parse the response.
 
         Args:
-            addr: Address to read out data from.
+            command (str): command to send to the board.
+
+        Returns:
+            int: value read from the board. Value is -1 if the read failed.
         """
-        cmd = self._generate_read_request(addr)
         try:
             if self.board.using_new_backend:
-                response = BoardIoManager(self.board).read(cmd)
+                response = BoardIoManager(self.board).read(command)
             else:
-                self._send_command(cmd)
-                response = self._read_response()
+                self._send_command(command)
+                response = self.board.connection.read_until(self.stopword)
         except TimeoutError:  # pragma: no cover
             return -1  # pragma: no cover
-        answer = self._parse_answer(response)
-        return answer["value"]
+        return self._parse_response(response)["value"]
 
-    def _generate_read_request(self, addr: str) -> str:
-        """Generate the read command for the firmwares. cmd: RRAA000"""
-        cmd = f"{self._read_cmd:X}"
-        cmd_addr = addr.zfill(self.width_addr)
-        val = "0".zfill(self.width_val)
-        command = f"{cmd}{cmd_addr}{val}"
-        return command.upper()
-
-    def _parse_response_to_names(self, buffer, addr):
-        """Takes the input buffer and parses the response into the registers.
-
-        Each register address can contain multiple register names, this function
-        parses the register address into the correct names.
-
-        Returns:
-            Dictionary with the names: [val, addr, pos, width, rw]
-        """
-        outp = {}
-
-        for key, val in self.registers.items():
-            if val["address"].upper() == addr.upper():
-                position = val["bitposition"]
-                width = val["bitwidth"]
-                mask = 2**width - 1
-                shifted = buffer >> position
-                oval = shifted & mask
-                outp[key] = {}
-
-                for regkey, regval in val.items():
-                    outp[key][regkey] = regval
-                outp[key]["value"] = oval
-
-        return outp
-
-    def _parse_answer(self, buffer):
-        """Parses a raw binary answer into python data formats.
+    def _parse_response(self, buffer: bytes) -> dict:
+        """Parses a raw binary answer into a dictionary.
 
         Args:
             buffer (bytes): Response to parse.
 
         Returns:
-            parsed answer as a dict expected format.
+            dict: parsed response containing keys: "header", "read_reg", "value".
         """
         header = int.from_bytes(buffer[0:2], byteorder="big", signed=False)
-        response = {
+        value = int.from_bytes(buffer[2:4], byteorder="big", signed=False)
+        return {
             "header": header,
-            "read_reg": header & 255,  # only 8 lsb]
-            "value": int.from_bytes(buffer[2:4], byteorder="big", signed=False),
+            "read_reg": header & 0xFF,
+            "value": value,
         }
 
-        return response
-
-    def _read_response(self):
-        """Read a data package based on the register stopword"""
-        return self.board.connection.read_until(self.stopword)  # pragma: no cover
+    def _registers_from_addr_value(self, addr: str, addr_value: int) -> dict:
+        addr = addr.upper()
+        return {
+            name: {"value": helpers.full_to_partial_value(addr_value, reg)} | reg.copy()
+            for name, reg in self.registers.items()
+            if reg["address"].upper() == addr.upper()
+        }
 
 
 # validation #################################################################
 #
 ##############################################################################
 def validate_registermap_or_raise(registers):
     """Validate a regmap, raises error if it's not valid."""
```

### Comparing `naludaq-0.17.7/src/naludaq/controllers/__init__.py` & `naludaq-0.18.0/src/naludaq/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/controllers/analog_debug_controller.py` & `naludaq-0.18.0/src/naludaq/controllers/analog_debug_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/controllers/biasing_mode/__init__.py` & `naludaq-0.18.0/src/naludaq/controllers/biasing_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/controllers/biasing_mode/udc16.py` & `naludaq-0.18.0/src/naludaq/controllers/biasing_mode/udc16.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/controllers/board/__init__.py` & `naludaq-0.18.0/src/naludaq/controllers/board/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/controllers/board/default.py` & `naludaq-0.18.0/src/naludaq/controllers/board/default.py`

 * *Files 1% similar despite different names*

```diff
@@ -308,17 +308,17 @@
         scal += scalhigh << shift_amt
 
         return scal
 
     def get_scal_name(self, i):
         return f"scal{i}"
 
-    def _read_digital_register(self, name):
+    def _read_digital_register(self, name: str, chips: "int | list[int]" = None):
         """Quick access to read digital register value"""
-        return DigitalRegisters(self.board).read(name)["value"]
+        return DigitalRegisters(self.board, chips).read(name)["value"]
 
     def _get_total_channels(self) -> int:
         """Returns the total number of channels on the board."""
         return self.board.channels
 
     def read_firmware_version(self):
         """Read the firmware version.
```

### Comparing `naludaq-0.17.7/src/naludaq/controllers/board/hdsoc.py` & `naludaq-0.18.0/src/naludaq/controllers/board/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/controllers/board/oleas.py` & `naludaq-0.18.0/src/naludaq/controllers/board/oleas.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/controllers/board/udc.py` & `naludaq-0.18.0/src/naludaq/controllers/board/udc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/controllers/board/upac.py` & `naludaq-0.18.0/src/naludaq/controllers/board/upac.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/controllers/board/upac96.py` & `naludaq-0.18.0/src/naludaq/controllers/board/upac96.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/controllers/connection/__init__.py` & `naludaq-0.18.0/src/naludaq/controllers/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/controllers/connection/connection_controller.py` & `naludaq-0.18.0/src/naludaq/controllers/connection/connection_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/controllers/connection/upac.py` & `naludaq-0.18.0/src/naludaq/controllers/connection/upac.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/controllers/connection/upac96.py` & `naludaq-0.18.0/src/naludaq/controllers/connection/upac96.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/controllers/external_dac/__init__.py` & `naludaq-0.18.0/src/naludaq/controllers/external_dac/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/controllers/external_dac/ad5671.py` & `naludaq-0.18.0/src/naludaq/controllers/external_dac/ad5671.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/controllers/external_dac/ad5675.py` & `naludaq-0.18.0/src/naludaq/controllers/external_dac/ad5675.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/controllers/external_dac/base.py` & `naludaq-0.18.0/src/naludaq/controllers/external_dac/base.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/controllers/external_dac/dac7578.py` & `naludaq-0.18.0/src/naludaq/controllers/external_dac/dac7578.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/controllers/external_dac/hdsoc.py` & `naludaq-0.18.0/src/naludaq/controllers/external_dac/hdsoc.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,10 +117,10 @@
 
             sendI2cCommand(self.board, (addr << 1) | rw, words)
             time.sleep(self._send_delay)
 
     def _is_tia_enabled(self) -> bool:
         """Checks if the TIA is enabled for either side."""
         return (
-            not self._board.registers["analog_registers"]["ntia_left"]
-            or not self._board.registers["analog_registers"]["ntia_right"]
+            not self._board.registers["analog_registers"]["ntia_left"][0]
+            or not self._board.registers["analog_registers"]["ntia_right"][0]
         )
```

### Comparing `naludaq-0.17.7/src/naludaq/controllers/external_dac/i2c_dac.py` & `naludaq-0.18.0/src/naludaq/controllers/external_dac/i2c_dac.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/controllers/external_dac/trbhm.py` & `naludaq-0.18.0/src/naludaq/controllers/external_dac/trbhm.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/controllers/external_dac/upac32.py` & `naludaq-0.18.0/src/naludaq/controllers/external_dac/upac32.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/controllers/gainstages/__init__.py` & `naludaq-0.18.0/src/naludaq/controllers/gainstages/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/controllers/gainstages/aodsv2.py` & `naludaq-0.18.0/src/naludaq/controllers/gainstages/aodsv2.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,17 @@
         super().__init__(board)
         self._num_stages = 8
 
     @property
     def sel_values(self) -> "list[bool]":
         """Get a list of sel values from the board registers"""
         analog_registers = self.board.registers["analog_registers"]
-        return [analog_registers[f"sel_{i}"]["value"] for i in range(self._num_stages)]
+        return [
+            analog_registers[f"sel_{i}"]["value"][0] for i in range(self._num_stages)
+        ]
 
     def set_manual(self, stages: List[bool]) -> List[Tuple[int, int]]:
         """Manually set the gainstages.
 
         This will set the gainstages to the values of the index in the list
         Each index corresponds to a gainstage and can be either True or False.
```

### Comparing `naludaq-0.17.7/src/naludaq/controllers/peripherals/__init__.py` & `naludaq-0.18.0/src/naludaq/controllers/peripherals/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/controllers/peripherals/aardvarcv3.py` & `naludaq-0.18.0/src/naludaq/controllers/peripherals/aardvarcv3.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/controllers/peripherals/aodsoc.py` & `naludaq-0.18.0/src/naludaq/controllers/peripherals/aodsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/controllers/peripherals/hdsoc.py` & `naludaq-0.18.0/src/naludaq/controllers/peripherals/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/controllers/peripherals/peripherals_controller.py` & `naludaq-0.18.0/src/naludaq/controllers/peripherals/peripherals_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/controllers/peripherals/upac.py` & `naludaq-0.18.0/src/naludaq/controllers/peripherals/upac.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/controllers/peripherals/upac96.py` & `naludaq-0.18.0/src/naludaq/controllers/peripherals/upac96.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/controllers/project_controller.py` & `naludaq-0.18.0/src/naludaq/controllers/project_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/controllers/readout/__init__.py` & `naludaq-0.18.0/src/naludaq/controllers/readout/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/controllers/readout/aardvarcv3.py` & `naludaq-0.18.0/src/naludaq/controllers/readout/aardvarcv3.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,9 +43,11 @@
 
     def get_readout_channels(self):
         """Get the current channels to read out.
 
         Returns:
             Sorted list of channel numbers to read out.
         """
-        mask = self.board.registers["digital_registers"]["excludechannelmask"]["value"]
+        mask = self.board.registers["digital_registers"]["excludechannelmask"]["value"][
+            0
+        ]
         return [c for c in range(self.board.channels) if (mask >> c) & 1 == 0]
```

### Comparing `naludaq-0.17.7/src/naludaq/controllers/readout/default.py` & `naludaq-0.18.0/src/naludaq/controllers/readout/default.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,27 +27,27 @@
     def __init__(self, board):
         super().__init__(board)
 
     @property
     def windows(self):
         """Get the number of windows to read."""
         reg = "readoutwindows"
-        return self.board.registers["digital_registers"][reg]["value"]
+        return self.board.registers["digital_registers"][reg]["value"][0]
 
     @property
     def lookback(self):
         """Get the number of windows to look back."""
         reg = "readoutlookback"
-        return self.board.registers["digital_registers"][reg]["value"]
+        return self.board.registers["digital_registers"][reg]["value"][0]
 
     @property
     def write_after_trig(self):
         """Get the number of windows to write after trigger."""
         reg = "writeaftertrig"
-        return self.board.registers["digital_registers"][reg]["value"]
+        return self.board.registers["digital_registers"][reg]["value"][0]
 
     def set_record_window(self, record_length: int, pre_trigger: int):
         """Set the read window for non-forced mode using the pre-trigger
         and record length.
 
         Args:
             pre_trigger (int): the number of windows before the trigger event
```

### Comparing `naludaq-0.17.7/src/naludaq/controllers/readout/hdsoc.py` & `naludaq-0.18.0/src/naludaq/controllers/readout/hdsoc.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
         Args:
             amount (int): Maximum number of events to read.
         """
         max_winds = self.board.params["max_numwinds"]
         read_windows = self.board.registers["digital_registers"]["readoutwindows"][
             "value"
-        ]
+        ][0]
         channels = len(self.get_readout_channels())
         if not isinstance(amount, int):
             raise TypeError(f"Amount must be an integer, got {type(amount)}")
 
         numwinds_to_read = amount * read_windows * channels
         if not 0 <= numwinds_to_read <= max_winds:
             raise ValueError(
@@ -71,15 +71,15 @@
 
         Returns:
             The list of channels read out.
         """
         return [
             chan
             for chan in range(self._board.channels)
-            if self._board.registers["analog_registers"][f"ch_{chan}_en"]["value"]
+            if self._board.registers["analog_registers"][f"ch_{chan}_en"]["value"][0]
         ]
 
     def _set_channel_active(self, channel: int, active: bool):
         """Wrapper for an analog register write that connects/disconnects
         the channel to everything, essentially turning it on of off
 
         Args:
```

### Comparing `naludaq-0.17.7/src/naludaq/controllers/readout/trbhm.py` & `naludaq-0.18.0/src/naludaq/controllers/readout/trbhm.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/controllers/si5341_controller.py` & `naludaq-0.18.0/src/naludaq/controllers/si5341_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/controllers/tia/__init__.py` & `naludaq-0.18.0/src/naludaq/controllers/tia/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/controllers/tia/base.py` & `naludaq-0.18.0/src/naludaq/controllers/tia/base.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/controllers/tia/hdsoc.py` & `naludaq-0.18.0/src/naludaq/controllers/tia/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/controllers/trigger/__init__.py` & `naludaq-0.18.0/src/naludaq/controllers/trigger/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/controllers/trigger/aodsoc.py` & `naludaq-0.18.0/src/naludaq/controllers/trigger/aodsoc.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from naludaq.communication import AnalogRegisters
+
 from .default import TriggerController
 
 
 class TriggerControllerAodsoc(TriggerController):
     """Trigger controller for AODSOC boards."""
 
     def __init__(self, board):
@@ -42,20 +44,12 @@
         """Write analog registers with a given register name format using the
         values provided. Writes values to both chips individually.
 
         Args:
             reg_name_format (str): register name format string, must take one integer argument.
             values (list): list of values to write. Should be all 8 values across both chips.
         """
-        for chip in range(self._num_chips):
-            self._select_chips([chip])
-
+        for chip in range(self.board.available_chips):
             for idx in range(self._num_trig_chans_per_chip):
+                name = reg_name_format.format(idx)
                 val = values[idx + chip * self._num_trig_chans_per_chip]
-                self._write_analog_register(reg_name_format.format(idx), val)
-
-        # TX needs to be restored after writing
-        self._select_chips(list(range(self._num_chips)))
-
-    def _select_chips(self, chips: "list[int]"):
-        """Select which chips will be enabled for register writes."""
-        self._write_control_register("ard_tx_en", sum([1 << x for x in chips]))
+                AnalogRegisters(self.board, [chip]).write(name, val)
```

### Comparing `naludaq-0.17.7/src/naludaq/controllers/trigger/default.py` & `naludaq-0.18.0/src/naludaq/controllers/trigger/default.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,36 +191,36 @@
             TypeError if raises is not a bool.
         """
         if not isinstance(raising, bool):
             raise TypeError("raising must be a bool, got %s", type(raising))
 
         self._write_analog_register("sgn", raising)
 
-    def _write_analog_register(self, register, value):
+    def _write_analog_register(self, register, value, chips: "int | list[int]" = None):
         """wrapper for the Analog register coms module.
 
         Args:
             register (str): name of the register to update.
             value: The register value to set.
 
         """
-        AnalogRegisters(self.board).write(register, value)
+        AnalogRegisters(self.board, chips).write(register, value)
 
     def _write_control_register(self, register, value):
         """wrapper for the Control register coms module.
 
         Args:
             register (str): name of the register to update.
             value: The register value to set.
 
         """
         ControlRegisters(self.board).write(register, value)
 
-    def _write_digital_register(self, register, value):
+    def _write_digital_register(self, register, value, chips: "int | list[int]" = None):
         """wrapper for the Digital register coms module.
 
         Args:
             register (str): name of the register to update.
             value: The register value to set.
 
         """
-        DigitalRegisters(self.board).write(register, value)
+        DigitalRegisters(self.board, chips).write(register, value)
```

### Comparing `naludaq-0.17.7/src/naludaq/controllers/trigger/hdsoc.py` & `naludaq-0.18.0/src/naludaq/controllers/trigger/hdsoc.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,8 +215,8 @@
                 "Reference value ranges must each be length 2 (lower & upper)"
             )
         for side, (lower, upper) in values.items():
             self._validate_reference_range_or_raise(side, lower, upper)
 
     def _get_analog_register(self, register: str) -> int:
         """Get the value of an analog register"""
-        return self.board.registers["analog_registers"][register]["value"]
+        return self.board.registers["analog_registers"][register]["value"][0]
```

### Comparing `naludaq-0.17.7/src/naludaq/controllers/trigger/trbhm.py` & `naludaq-0.18.0/src/naludaq/controllers/trigger/trbhm.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from naludaq.communication import AnalogRegisters
+
 from .default import TriggerController
 
 
 class TriggerControllerTrbhm(TriggerController):
     """Trigger controller for TRBHM boards."""
 
     def __init__(self, board):
@@ -36,20 +38,12 @@
         """Write analog registers with a given register name format using the
         values provided. Writes values to both chips individually.
 
         Args:
             reg_name_format (str): register name format string, must take one integer argument.
             values (list): list of values to write. Should be all 8 values across both chips.
         """
-        for chip in range(self._num_chips):
-            self._select_chips([chip])
-
+        for chip in range(self.board.available_chips):
             for idx in range(self._num_trig_chans_per_chip):
+                name = reg_name_format.format(idx)
                 val = values[idx + chip * self._num_trig_chans_per_chip]
-                self._write_analog_register(reg_name_format.format(idx), val)
-
-        # TX needs to be restored after writing
-        self._select_chips(list(range(self._num_chips)))
-
-    def _select_chips(self, chips: "list[int]"):
-        """Select which chips will be enabled for register writes."""
-        self._write_control_register("ard_tx_en", sum([1 << x for x in chips]))
+                AnalogRegisters(self.board, [chip]).write(name, val)
```

### Comparing `naludaq-0.17.7/src/naludaq/controllers/trigger/upac.py` & `naludaq-0.18.0/src/naludaq/controllers/trigger/upac.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/controllers/trigger/upac96.py` & `naludaq-0.18.0/src/naludaq/controllers/trigger/upac96.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 """
 import logging
 from collections import defaultdict
-from contextlib import contextmanager
 
 from naludaq.communication import DigitalRegisters
 from naludaq.helpers.exceptions import InvalidTriggerMaskError
 from naludaq.helpers.helper_functions import type_name
 
 from .default import TriggerController
 
@@ -26,15 +25,17 @@
         self._num_chips = board.params.get("num_chips", 6)
         self._max_threshold = board.params.get("trigger", {}).get("max_val", 4095)
         self._min_threshold = board.params.get("trigger", {}).get("min_val", 0)
         self._channels_per_chip = self._num_channels // self._num_chips
 
     @property
     def enable_trigger_out(self):
-        return self.board.registers["control_registers"].get("coincidence_trigger_select", False)
+        return self.board.registers["control_registers"].get(
+            "coincidence_trigger_select", False
+        )
 
     @enable_trigger_out.setter
     def enable_trigger_out(self, value):
         """enable trigger out
 
         Args:
             value (bool): True for box checked False for box not checked
@@ -64,17 +65,20 @@
                 or contains invalid elements
         """
         self._validate_channel_list_or_raise(channels)
         LOGGER.debug("Setting trigger mask: %s", channels)
         for chip in range(self._num_chips):
             chip_channels = self._filter_channels_for_chip(channels, chip)
             trigmask = self._create_trigger_mask(chip_channels)
-            with self._select_chips([chip]):
-                self._write_digital_register("triggerchannelmask_lo", trigmask & 0xFF)
-                self._write_digital_register("triggerchannelmask_hi", trigmask >> 8)
+            self._write_digital_register(
+                "triggerchannelmask_lo", trigmask & 0xFF, chips=chip
+            )
+            self._write_digital_register(
+                "triggerchannelmask_hi", trigmask >> 8, chips=chip
+            )
 
         # coincidence trigger on chips without any enabled channels doesn't work
         chip_mask = self._make_chip_mask_from_channel_mask(channels)
         self._set_chip_trigger_mask(chip_mask)
 
     def _make_chip_mask_from_channel_mask(self, channels: list[int]) -> list[int]:
         """Creates a chip trigger mask from the given channel trigger mask.
@@ -108,31 +112,30 @@
     def _set_trigger_thresholds(self):
         """Sets the trigger thresholds from board.trigger_values for all channels"""
         trigger_values = self.board.trigger_values
         self._validate_trigger_list_or_raise(trigger_values)
         LOGGER.debug("Setting trigger thresholds: %s", trigger_values)
         threshold_groups = self._group_by_chips(trigger_values)
         for chip, threshold_pair in threshold_groups.items():
-            with self._select_chips([chip]):
-                self._write_threshold_pairs(threshold_pair)
+            self._write_threshold_pairs(threshold_pair, chip)
         self._reset_writemask()
 
-    def _write_threshold_pairs(self, threshold_pair: dict[int, list[int]]):
+    def _write_threshold_pairs(self, threshold_pair: dict[int, list[int]], chip: int):
         """Writes the threshold for the given pairs of threshold values and channels.
 
         Args:
             threshold_pair (dict[int, list[int]]): a dict mapping channels to threshold values.
         """
         for threshold, channels in threshold_pair.items():
             writemask = sum(
                 1 << channel % self._channels_per_chip for channel in channels
             )
-            self._write_digital_register("writemask_l", writemask & 0xFF)
-            self._write_digital_register("writemask_r", writemask >> 8)
-            self._write_analog_register("trgthresh", threshold)
+            self._write_digital_register("writemask_l", writemask & 0xFF, chips=chip)
+            self._write_digital_register("writemask_r", writemask >> 8, chips=chip)
+            self._write_analog_register("trgthresh", threshold, chips=chip)
 
     def set_coincidence_trigger_enabled(self, chips: dict):
         """Sets whether the coincidence trigger is enabled for the given chips.
 
         The coincidence trigger performs "AND"-like logic between channels,
         only emitting a trigger event if multiple channels are triggered at once.
         The period of time for which trigger events are accepted appears to be
@@ -143,20 +146,19 @@
 
         Args:
             chips: a dict with chips (int) as keys, and enabled (bool) for the value
         """
         self._validate_coincidence_trigger_chips_or_raise(chips)
         LOGGER.debug("Setting coincidence trigger: %s", chips)
         for chip, enabled in chips.items():
-            with self._select_chips([chip]):
-                # lowest bit of misc reg enables/disables the coincidence trigger
-                # for the entire ASIC
-                miscreg = self._digital_read("miscreg")
-                miscreg = (miscreg & 0b10) | enabled
-                self._write_digital_register("miscreg", miscreg)
+            # lowest bit of misc reg enables/disables the coincidence trigger
+            # for the entire ASIC
+            miscreg = self._digital_read("miscreg", chip)
+            miscreg = (miscreg & 0b10) | enabled
+            self._write_digital_register("miscreg", miscreg, chips=chip)
 
     def _set_chip_trigger_mask(self, chips: list[int]):
         """Sets the chip trigger mask.
 
         Args:
             chips (list): a list of chips to trigger on
 
@@ -181,16 +183,15 @@
                 Each value should be True for rising edges, or False for falling edges.
         """
         self._validate_edge_list_or_raise(channel_edges)
         LOGGER.debug("Setting trigger edges: %s", channel_edges)
         for chip in range(self._num_chips):
             edge_mask = self._extract_edge_mask_for_chip(channel_edges, chip)
             sgn_l, sgn_r = self._flip_sgn_bytes(edge_mask)
-            with self._select_chips([chip]):
-                self._set_sgn(sgn_l, sgn_r)
+            self._set_sgn(chip, sgn_l, sgn_r)
         self._reset_writemask()
 
     def _extract_edge_mask_for_chip(self, channel_edges: list[bool], chip: int) -> int:
         """Extract the edge mask for the given chip from the given list of edges.
 
         Args:
             channel_edges (list[bool]): list of edge settings for each channel.
@@ -202,30 +203,30 @@
         """
         return sum(
             1 << c
             for c in range(self._channels_per_chip)
             if channel_edges[c + chip * self._channels_per_chip]
         )
 
-    def _set_sgn(self, sgn_l: int, sgn_r: int):
+    def _set_sgn(self, chip: int, sgn_l: int, sgn_r: int):
         """Set the sgn register.
 
         Highest bit is broadcast bit, it's required to be set
         in order to write to each copy of the sgn register individually
 
         Args:
             sgn_l (int): the value to set the sgn register to for the left side
             sgn_r (int): the value to set the sgn register to for the right side
         """
-        self._write_digital_register("writemask_l", 0x1FF)
-        self._write_digital_register("writemask_r", 0)
-        self._write_analog_register("sgn", sgn_l)
-        self._write_digital_register("writemask_l", 0)
-        self._write_digital_register("writemask_r", 0x1FF)
-        self._write_analog_register("sgn", sgn_r)
+        self._write_digital_register("writemask_l", 0x1FF, chips=chip)
+        self._write_digital_register("writemask_r", 0, chips=chip)
+        self._write_analog_register("sgn", sgn_l, chips=chip)
+        self._write_digital_register("writemask_l", 0, chips=chip)
+        self._write_digital_register("writemask_r", 0x1FF, chips=chip)
+        self._write_analog_register("sgn", sgn_r, chips=chip)
 
     def _flip_sgn_bytes(self, sgn_mask: int) -> tuple[int, int]:
         """Flip the bytes of the sgn register mask.
 
         Individual bytes need to be flipped because the bits in
         the sgn register are reversed (i.e. bit 0 corresponds to channel 7).
 
@@ -272,44 +273,29 @@
             groups[chip][val].append(channel)
         return groups
 
     def _filter_channels_for_chip(self, channels: list[int], chip: int) -> list[int]:
         """Filters out channels in the given list that don't belong to the given chip."""
         return list(filter(lambda c: (c // self._channels_per_chip) == chip, channels))
 
-    @contextmanager
-    def _select_chips(self, chips: list[int]):
-        """Set which UDC chips will receive commands sent.
-
-        This method is a context manager, so it should be used with the ``with`` keyword.
-        """
-        original = self.board.registers["control_registers"]["udc_rxout_enable"][
-            "value"
-        ]
-        mask = sum(1 << chip for chip in chips)
-        self._write_control_register("udc_rxout_enable", mask)
-        yield
-        self._write_control_register("udc_rxout_enable", original)
-
     def _reset_writemask(self):
         """Reset the write mask register for all chips.
 
         The writemask register is restored to 0x1FF (broadcast + all channels),
         regardless of what it was set to before. This is important because
         it ensures the other analog registers don't get written improperly
         elsewhere due to the writemask being wrong.
         """
-        with self._select_chips(range(self._num_chips)):
-            self._write_digital_register("writemask_l", 0x1FF)
-            self._write_digital_register("writemask_r", 0x1FF)
+        self._write_digital_register("writemask_l", 0x1FF)
+        self._write_digital_register("writemask_r", 0x1FF)
 
-    def _digital_read(self, name: str) -> int:
+    def _digital_read(self, name: str, chip: int) -> int:
         """Read a digital register"""
         try:
-            return DigitalRegisters(self.board).read(name)["value"]
+            return DigitalRegisters(self.board, chips=chip).read(name)["value"]
         except ConnectionError:
             raise
 
     def _validate_channel_list_or_raise(self, channels):
         """Validates a list of channels, and raises an error
         if there's a problem with them.
```

### Comparing `naludaq-0.17.7/src/naludaq/daq/__init__.py` & `naludaq-0.18.0/src/naludaq/daq/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/daq/debugdaq.py` & `naludaq-0.18.0/src/naludaq/daq/debugdaq.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/daq/lightdaq.py` & `naludaq-0.18.0/src/naludaq/daq/lightdaq.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/daq/preprocess.py` & `naludaq-0.18.0/src/naludaq/daq/preprocess.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/daq/workers/__init__.py` & `naludaq-0.18.0/src/naludaq/daq/workers/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/daq/workers/answer_parser_worker.py` & `naludaq-0.18.0/src/naludaq/daq/workers/answer_parser_worker.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/daq/workers/csv_storage_worker.py` & `naludaq-0.18.0/src/naludaq/daq/workers/csv_storage_worker.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/daq/workers/packager/__init__.py` & `naludaq-0.18.0/src/naludaq/daq/workers/packager/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/daq/workers/packager/worker_packager.py` & `naludaq-0.18.0/src/naludaq/daq/workers/packager/worker_packager.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/daq/workers/packager/worker_packager_debug.py` & `naludaq-0.18.0/src/naludaq/daq/workers/packager/worker_packager_debug.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/daq/workers/packager/worker_packager_hdsoc.py` & `naludaq-0.18.0/src/naludaq/daq/workers/packager/worker_packager_hdsoc.py`

 * *Files 0% similar despite different names*

```diff
@@ -275,15 +275,15 @@
         return complete_event
 
     def _get_enabled_channels(self) -> List[int]:
         """Fetch a list of enabled channels from the board registers."""
         return [
             chan
             for chan in range(self._board.channels)
-            if self._board.registers["analog_registers"][f"ch_{chan}_en"]["value"]
+            if self._board.registers["analog_registers"][f"ch_{chan}_en"]["value"][0]
         ]
 
     def stop(self):
         super().stop()
         # Any incomplete data will be saved in case stop is in middle of event.
         if self._incomplete_event["timing"] != UNUSED_TIMING:
             complete = self._incomplete_event
```

### Comparing `naludaq-0.17.7/src/naludaq/daq/workers/postprocessing.py` & `naludaq-0.18.0/src/naludaq/daq/workers/postprocessing.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/daq/workers/worker_parser.py` & `naludaq-0.18.0/src/naludaq/daq/workers/worker_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/daq/workers/worker_serial_reader.py` & `naludaq-0.18.0/src/naludaq/daq/workers/worker_serial_reader.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/daq/workers/worker_usb_reader.py` & `naludaq-0.18.0/src/naludaq/daq/workers/worker_usb_reader.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/devices/eeprom.py` & `naludaq-0.18.0/src/naludaq/devices/eeprom.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/devices/i2c_device.py` & `naludaq-0.18.0/src/naludaq/devices/i2c_device.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/devices/ltc2990.py` & `naludaq-0.18.0/src/naludaq/devices/ltc2990.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/helpers/decorators.py` & `naludaq-0.18.0/src/naludaq/helpers/decorators.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/helpers/exceptions.py` & `naludaq-0.18.0/src/naludaq/helpers/exceptions.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/helpers/helper_functions.py` & `naludaq-0.18.0/src/naludaq/helpers/helper_functions.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/helpers/register_cache.py` & `naludaq-0.18.0/src/naludaq/helpers/register_cache.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/helpers/semiton.py` & `naludaq-0.18.0/src/naludaq/helpers/semiton.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/io/__init__.py` & `naludaq-0.18.0/src/naludaq/io/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/io/csv_writer.py` & `naludaq-0.18.0/src/naludaq/io/csv_writer.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/io/hdf5.py` & `naludaq-0.18.0/src/naludaq/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/io/io_manager.py` & `naludaq-0.18.0/src/naludaq/io/io_manager.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/models/acq_converters.py` & `naludaq-0.18.0/src/naludaq/models/acq_converters.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/models/acquisition.py` & `naludaq-0.18.0/src/naludaq/models/acquisition.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/naludaq.py` & `naludaq-0.18.0/src/naludaq/naludaq.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/parsers/__init__.py` & `naludaq-0.18.0/src/naludaq/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/parsers/aardvarcv3_parser.py` & `naludaq-0.18.0/src/naludaq/parsers/aardvarcv3_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/parsers/answer_parser.py` & `naludaq-0.18.0/src/naludaq/parsers/answer_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/parsers/aodsoc_parser.py` & `naludaq-0.18.0/src/naludaq/parsers/aodsoc_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/parsers/asocv3_parser.py` & `naludaq-0.18.0/src/naludaq/parsers/asocv3_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/parsers/hdsoc_parser.py` & `naludaq-0.18.0/src/naludaq/parsers/hdsoc_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/parsers/headers/__init__.py` & `naludaq-0.18.0/src/naludaq/parsers/headers/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/parsers/headers/asoc.py` & `naludaq-0.18.0/src/naludaq/parsers/headers/asoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/parsers/headers/asocv2.py` & `naludaq-0.18.0/src/naludaq/parsers/headers/asocv2.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/parsers/headers/base.py` & `naludaq-0.18.0/src/naludaq/parsers/headers/base.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/parsers/headers/siread.py` & `naludaq-0.18.0/src/naludaq/parsers/headers/siread.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/parsers/headers/trbhm.py` & `naludaq-0.18.0/src/naludaq/parsers/headers/trbhm.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/parsers/headers/upac32.py` & `naludaq-0.18.0/src/naludaq/parsers/headers/upac32.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/parsers/parser.py` & `naludaq-0.18.0/src/naludaq/parsers/parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/parsers/trbhm_parser.py` & `naludaq-0.18.0/src/naludaq/parsers/trbhm_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/parsers/udc_parser.py` & `naludaq-0.18.0/src/naludaq/parsers/udc_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/parsers/upac96_parser.py` & `naludaq-0.18.0/src/naludaq/parsers/upac96_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/parsers/upac_parser.py` & `naludaq-0.18.0/src/naludaq/parsers/upac_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/tools/adc2mv/adc_converter.py` & `naludaq-0.18.0/src/naludaq/tools/adc2mv/adc_converter.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/tools/adc2mv/adc_linear_regression.py` & `naludaq-0.18.0/src/naludaq/tools/adc2mv/adc_linear_regression.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/tools/adc2mv/generate.py` & `naludaq-0.18.0/src/naludaq/tools/adc2mv/generate.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/tools/adc2mv/pre_adc2mv.py` & `naludaq-0.18.0/src/naludaq/tools/adc2mv/pre_adc2mv.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/tools/autoaction.py` & `naludaq-0.18.0/src/naludaq/tools/autoaction.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/tools/autotrigger/default.py` & `naludaq-0.18.0/src/naludaq/tools/autotrigger/default.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/tools/board_backup.py` & `naludaq-0.18.0/src/naludaq/tools/board_backup.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/tools/dac_sweep/dac_sweep_controller.py` & `naludaq-0.18.0/src/naludaq/tools/dac_sweep/dac_sweep_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/tools/data_collector.py` & `naludaq-0.18.0/src/naludaq/tools/data_collector.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/tools/features.py` & `naludaq-0.18.0/src/naludaq/tools/features.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/tools/ft60x.py` & `naludaq-0.18.0/src/naludaq/tools/ft60x.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/tools/ftdi.py` & `naludaq-0.18.0/src/naludaq/tools/ftdi.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/tools/metadata.py` & `naludaq-0.18.0/src/naludaq/tools/metadata.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/tools/optimizers/bayesian_optimizer.py` & `naludaq-0.18.0/src/naludaq/tools/optimizers/bayesian_optimizer.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/tools/optimizers/gainstagetuner.py` & `naludaq-0.18.0/src/naludaq/tools/optimizers/gainstagetuner.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/tools/pedestals/__init__.py` & `naludaq-0.18.0/src/naludaq/tools/pedestals/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/tools/pedestals/_new/__init__.py` & `naludaq-0.18.0/src/naludaq/tools/pedestals/_new/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/tools/pedestals/_new/aav3.py` & `naludaq-0.18.0/src/naludaq/tools/pedestals/_new/aav3.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/tools/pedestals/_new/default.py` & `naludaq-0.18.0/src/naludaq/tools/pedestals/_new/default.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/tools/pedestals/_new/hdsoc.py` & `naludaq-0.18.0/src/naludaq/tools/pedestals/_new/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/tools/pedestals/aardvarcv3_pedestals_generator.py` & `naludaq-0.18.0/src/naludaq/tools/pedestals/aardvarcv3_pedestals_generator.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/tools/pedestals/hdsoc_pedestals_controller.py` & `naludaq-0.18.0/src/naludaq/tools/pedestals/hdsoc_pedestals_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/tools/pedestals/pedestals_acq.py` & `naludaq-0.18.0/src/naludaq/tools/pedestals/pedestals_acq.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/tools/pedestals/pedestals_controller.py` & `naludaq-0.18.0/src/naludaq/tools/pedestals/pedestals_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/tools/pedestals/pedestals_correcter.py` & `naludaq-0.18.0/src/naludaq/tools/pedestals/pedestals_correcter.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/tools/pedestals/pedestals_processor.py` & `naludaq-0.18.0/src/naludaq/tools/pedestals/pedestals_processor.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/tools/pedestals/udc16_pedestals_generator.py` & `naludaq-0.18.0/src/naludaq/tools/pedestals/udc16_pedestals_generator.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/tools/pedestals/upac32_pedestals_controller.py` & `naludaq-0.18.0/src/naludaq/tools/pedestals/upac32_pedestals_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/tools/pedestals/upac96_pedestals_generator.py` & `naludaq-0.18.0/src/naludaq/tools/pedestals/upac96_pedestals_generator.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/tools/threshold_scan/__init__.py` & `naludaq-0.18.0/src/naludaq/tools/threshold_scan/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/tools/threshold_scan/hdsoc_thresholdscan.py` & `naludaq-0.18.0/src/naludaq/tools/threshold_scan/hdsoc_thresholdscan.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
         to read correctly.
         """
         AnalogRegisters(self.board).write("tsel_left", left)
         AnalogRegisters(self.board).write("tsel_right", right)
 
     def _get_analog_register(self, register: str) -> int:
         """Get the value of an analog register"""
-        return self.board.registers["analog_registers"][register]["value"]
+        return self.board.registers["analog_registers"][register]["value"][0]
 
     def _validate_scan_settings_or_raise(self):
         """Raise an error if scan settings don't make sense"""
         if self.low_ref_value >= self.high_ref_value:
             raise ValueError("Low reference cannot exceed the high reference")
 
     def _get_scalar_values_vertical(self, pause: float) -> np.ndarray:
```

### Comparing `naludaq-0.17.7/src/naludaq/tools/threshold_scan/threshold_scan.py` & `naludaq-0.18.0/src/naludaq/tools/threshold_scan/threshold_scan.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/tools/timing_cal/__init__.py` & `naludaq-0.18.0/src/naludaq/tools/timing_cal/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/tools/timing_cal/calibration.py` & `naludaq-0.18.0/src/naludaq/tools/timing_cal/calibration.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/tools/timing_cal/correcter.py` & `naludaq-0.18.0/src/naludaq/tools/timing_cal/correcter.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq/tools/waiter/eventwaiter.py` & `naludaq-0.18.0/src/naludaq/tools/waiter/eventwaiter.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.7/src/naludaq.egg-info/PKG-INFO` & `naludaq-0.18.0/src/naludaq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naludaq
-Version: 0.17.7
+Version: 0.18.0
 Summary: Backend package for Nalu Scientific hardware
 Home-page: 
 Author: Thomas Yang, Emily Lum, Terry Pham
 Author-email: Marcus Luck <marcus@naluscientific.com>, Mitchell Matsumori-Kelly <mitchell@naluscientific.com>, Alvin Yang <alvin@naluscientific.com>, Kenneth Lauritzen <kenneth@naluscientific.com>, Ben Rotter <ben@naluscientific.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

### Comparing `naludaq-0.17.7/src/naludaq.egg-info/SOURCES.txt` & `naludaq-0.18.0/src/naludaq.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,19 @@
 src/naludaq/board/initializers/aodsoc.py
 src/naludaq/board/initializers/init_aodsv2_eval.py
 src/naludaq/board/initializers/init_hdsocv1.py
 src/naludaq/board/initializers/init_udc.py
 src/naludaq/board/initializers/init_upac96.py
 src/naludaq/board/initializers/trbhm.py
 src/naludaq/communication/__init__.py
+src/naludaq/communication/_chip.py
+src/naludaq/communication/_common.py
+src/naludaq/communication/_fpga.py
 src/naludaq/communication/analog_registers.py
+src/naludaq/communication/chip_selection.py
 src/naludaq/communication/control_registers.py
 src/naludaq/communication/digital_registers.py
 src/naludaq/communication/i2c.py
 src/naludaq/communication/i2c_registers.py
 src/naludaq/communication/registers.py
 src/naludaq/controllers/__init__.py
 src/naludaq/controllers/analog_debug_controller.py
```

