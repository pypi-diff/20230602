# Comparing `tmp/naluconfigs-10.8.0.tar.gz` & `tmp/naluconfigs-11.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naluconfigs-10.8.0.tar", last modified: Tue May 23 21:12:27 2023, max compression
+gzip compressed data, was "naluconfigs-11.0.0.tar", last modified: Thu Jun  1 23:43:16 2023, max compression
```

## Comparing `naluconfigs-10.8.0.tar` & `naluconfigs-11.0.0.tar`

### file list

```diff
@@ -1,70 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:12:27.312542 naluconfigs-10.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-05-23 21:12:27.312542 naluconfigs-10.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-23 21:12:06.000000 naluconfigs-10.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-23 21:12:06.000000 naluconfigs-10.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 21:12:27.312542 naluconfigs-10.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-23 21:12:06.000000 naluconfigs-10.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:12:27.300542 naluconfigs-10.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:12:27.300542 naluconfigs-10.8.0/src/naluconfigs/
--rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-05-23 21:12:06.000000 naluconfigs-10.8.0/src/naluconfigs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-23 21:12:06.000000 naluconfigs-10.8.0/src/naluconfigs/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:12:27.300542 naluconfigs-10.8.0/src/naluconfigs/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:12:27.308542 naluconfigs-10.8.0/src/naluconfigs/data/clocks/
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-05-23 21:12:06.000000 naluconfigs-10.8.0/src/naluconfigs/data/clocks/AODS_300GCC.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-05-23 21:12:06.000000 naluconfigs-10.8.0/src/naluconfigs/data/clocks/AODS_8M.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-05-23 21:12:06.000000 naluconfigs-10.8.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2-13GSa_711MGCC-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-05-23 21:12:06.000000 naluconfigs-10.8.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2_GCC781_DebugSE-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-05-23 21:12:06.000000 naluconfigs-10.8.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv3_GCC781_DebugSE-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-05-23 21:12:06.000000 naluconfigs-10.8.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv4_GCC781_DebugSE-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-05-23 21:12:06.000000 naluconfigs-10.8.0/src/naluconfigs/data/clocks/Si5341-RevD-ASoC_lambchop-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-05-23 21:12:06.000000 naluconfigs-10.8.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_15_625SysClk_400GccClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-05-23 21:12:06.000000 naluconfigs-10.8.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GCCclk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-05-23 21:12:06.000000 naluconfigs-10.8.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GccClk_156_25TxClk_31_25TxDivClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-05-23 21:12:06.000000 naluconfigs-10.8.0/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR-NexysFMC_78_125SysClk_312_5GccClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-05-23 21:12:06.000000 naluconfigs-10.8.0/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR_78_125SysClk_312_5GccClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-05-23 21:12:06.000000 naluconfigs-10.8.0/src/naluconfigs/data/clocks/Si5341-RevD-Lambchop-Registers_compSysclk.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-05-23 21:12:06.000000 naluconfigs-10.8.0/src/naluconfigs/data/clocks/Si5341-RevD-TR-BHM_78_125SysClk_781_25GccClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-05-23 21:12:07.000000 naluconfigs-10.8.0/src/naluconfigs/data/clocks/Si5341-RevD-UDC_78_125SlowClk_78_125IntermediateClk_312_5FastClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-05-23 21:12:07.000000 naluconfigs-10.8.0/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_GCC450M_debugse3125-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-05-23 21:12:07.000000 naluconfigs-10.8.0/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_simple_GCC300M_Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-05-23 21:12:07.000000 naluconfigs-10.8.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC123M_1xSysClk_v32andup_6250ksed.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-05-23 21:12:07.000000 naluconfigs-10.8.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-05-23 21:12:07.000000 naluconfigs-10.8.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup_6250ksed.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-05-23 21:12:07.000000 naluconfigs-10.8.0/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-05-23 21:12:07.000000 naluconfigs-10.8.0/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC450M_1xSysClk_v32andup_6250ksed.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-05-23 21:12:07.000000 naluconfigs-10.8.0/src/naluconfigs/data/clocks/Si5341_TRBHM_10GSaps_GCCsstx2_Registers.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:12:27.312542 naluconfigs-10.8.0/src/naluconfigs/data/registers/
--rw-r--r--   0 runner    (1001) docker     (123)    21701 2023-05-23 21:12:07.000000 naluconfigs-10.8.0/src/naluconfigs/data/registers/aardvarcv2.yml
--rw-r--r--   0 runner    (1001) docker     (123)    22900 2023-05-23 21:12:07.000000 naluconfigs-10.8.0/src/naluconfigs/data/registers/aardvarcv3.yml
--rw-r--r--   0 runner    (1001) docker     (123)    32645 2023-05-23 21:12:07.000000 naluconfigs-10.8.0/src/naluconfigs/data/registers/aardvarcv4.yml
--rw-r--r--   0 runner    (1001) docker     (123)    29188 2023-05-23 21:12:07.000000 naluconfigs-10.8.0/src/naluconfigs/data/registers/aodsoc_aods.yml
--rw-r--r--   0 runner    (1001) docker     (123)    24812 2023-05-23 21:12:07.000000 naluconfigs-10.8.0/src/naluconfigs/data/registers/aodsoc_asoc.yml
--rw-r--r--   0 runner    (1001) docker     (123)    25656 2023-05-23 21:12:07.000000 naluconfigs-10.8.0/src/naluconfigs/data/registers/aodsv1.yml
--rw-r--r--   0 runner    (1001) docker     (123)    26883 2023-05-23 21:12:07.000000 naluconfigs-10.8.0/src/naluconfigs/data/registers/aodsv2_eval.yml
--rw-r--r--   0 runner    (1001) docker     (123)    17697 2023-05-23 21:12:07.000000 naluconfigs-10.8.0/src/naluconfigs/data/registers/asoc.yml
--rw-r--r--   0 runner    (1001) docker     (123)    21848 2023-05-23 21:12:07.000000 naluconfigs-10.8.0/src/naluconfigs/data/registers/asocv2.yml
--rw-r--r--   0 runner    (1001) docker     (123)    25960 2023-05-23 21:12:07.000000 naluconfigs-10.8.0/src/naluconfigs/data/registers/asocv3.yml
--rw-r--r--   0 runner    (1001) docker     (123)    67433 2023-05-23 21:12:07.000000 naluconfigs-10.8.0/src/naluconfigs/data/registers/hdsocv1_evalr2.yml
--rw-r--r--   0 runner    (1001) docker     (123)    33711 2023-05-23 21:12:07.000000 naluconfigs-10.8.0/src/naluconfigs/data/registers/hiper.yml
--rw-r--r--   0 runner    (1001) docker     (123)    32912 2023-05-23 21:12:07.000000 naluconfigs-10.8.0/src/naluconfigs/data/registers/hiper_fmc.yml
--rw-r--r--   0 runner    (1001) docker     (123)    25224 2023-05-23 21:12:07.000000 naluconfigs-10.8.0/src/naluconfigs/data/registers/oleas_box2.yml
--rw-r--r--   0 runner    (1001) docker     (123)    19243 2023-05-23 21:12:07.000000 naluconfigs-10.8.0/src/naluconfigs/data/registers/siread.yml
--rw-r--r--   0 runner    (1001) docker     (123)    27563 2023-05-23 21:12:07.000000 naluconfigs-10.8.0/src/naluconfigs/data/registers/trbhm.yml
--rw-r--r--   0 runner    (1001) docker     (123)    21959 2023-05-23 21:12:07.000000 naluconfigs-10.8.0/src/naluconfigs/data/registers/udc16.yml
--rw-r--r--   0 runner    (1001) docker     (123)    18905 2023-05-23 21:12:07.000000 naluconfigs-10.8.0/src/naluconfigs/data/registers/upac32.yml
--rw-r--r--   0 runner    (1001) docker     (123)    18885 2023-05-23 21:12:07.000000 naluconfigs-10.8.0/src/naluconfigs/data/registers/upac96.yml
--rw-r--r--   0 runner    (1001) docker     (123)    16876 2023-05-23 21:12:07.000000 naluconfigs-10.8.0/src/naluconfigs/data/registers/upaci.yml
--rw-r--r--   0 runner    (1001) docker     (123)    16909 2023-05-23 21:12:07.000000 naluconfigs-10.8.0/src/naluconfigs/data/registers/zdigitizer.yml
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-23 21:12:07.000000 naluconfigs-10.8.0/src/naluconfigs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-05-23 21:12:07.000000 naluconfigs-10.8.0/src/naluconfigs/postprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:12:27.304542 naluconfigs-10.8.0/src/naluconfigs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-05-23 21:12:27.000000 naluconfigs-10.8.0/src/naluconfigs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-05-23 21:12:27.000000 naluconfigs-10.8.0/src/naluconfigs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 21:12:27.000000 naluconfigs-10.8.0/src/naluconfigs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-23 21:12:27.000000 naluconfigs-10.8.0/src/naluconfigs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 21:12:27.000000 naluconfigs-10.8.0/src/naluconfigs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:12:27.312542 naluconfigs-10.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-23 21:12:07.000000 naluconfigs-10.8.0/tests/test_hex_addr_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-05-23 21:12:07.000000 naluconfigs-10.8.0/tests/test_i2c_registers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-23 21:12:07.000000 naluconfigs-10.8.0/tests/test_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-05-23 21:12:07.000000 naluconfigs-10.8.0/tests/test_range_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:43:16.134607 naluconfigs-11.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-01 23:43:16.134607 naluconfigs-11.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 23:43:16.134607 naluconfigs-11.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:43:16.126607 naluconfigs-11.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:43:16.126607 naluconfigs-11.0.0/src/naluconfigs/
+-rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/_constructors.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:43:16.126607 naluconfigs-11.0.0/src/naluconfigs/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:43:16.130607 naluconfigs-11.0.0/src/naluconfigs/data/clocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/data/clocks/AODS_300GCC.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/data/clocks/AODS_8M.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2-13GSa_711MGCC-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2_GCC781_DebugSE-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv3_GCC781_DebugSE-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv4_GCC781_DebugSE-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/data/clocks/Si5341-RevD-ASoC_lambchop-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_15_625SysClk_400GccClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GCCclk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GccClk_156_25TxClk_31_25TxDivClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR-NexysFMC_78_125SysClk_312_5GccClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR_78_125SysClk_312_5GccClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/data/clocks/Si5341-RevD-Lambchop-Registers_compSysclk.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/data/clocks/Si5341-RevD-TR-BHM_78_125SysClk_781_25GccClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/data/clocks/Si5341-RevD-UDC_78_125SlowClk_78_125IntermediateClk_312_5FastClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_GCC450M_debugse3125-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_simple_GCC300M_Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC123M_1xSysClk_v32andup_6250ksed.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup_6250ksed.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC450M_1xSysClk_v32andup_6250ksed.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/data/clocks/Si5341_TRBHM_10GSaps_GCCsstx2_Registers.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:43:16.134607 naluconfigs-11.0.0/src/naluconfigs/data/registers/
+-rw-r--r--   0 runner    (1001) docker     (123)    21701 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/data/registers/aardvarcv2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11284 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/data/registers/aardvarcv3.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    32645 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/data/registers/aardvarcv4.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/data/registers/aodsoc_aods.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    13745 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/data/registers/aodsoc_asoc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11376 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/data/registers/aodsv1.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11388 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/data/registers/aodsv2_eval.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    17697 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/data/registers/asoc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    21848 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/data/registers/asocv2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    14828 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/data/registers/asocv3.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    16221 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/data/registers/hdsocv1_evalr2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    33711 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/data/registers/hiper.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    32912 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/data/registers/hiper_fmc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    25224 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/data/registers/oleas_box2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    19243 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/data/registers/siread.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    15698 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/data/registers/trbhm.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11671 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/data/registers/udc16.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    18905 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/data/registers/upac32.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/data/registers/upac96.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    16876 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/data/registers/upaci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    16909 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/data/registers/zdigitizer.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/src/naluconfigs/postprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:43:16.126607 naluconfigs-11.0.0/src/naluconfigs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-01 23:43:16.000000 naluconfigs-11.0.0/src/naluconfigs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-06-01 23:43:16.000000 naluconfigs-11.0.0/src/naluconfigs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 23:43:16.000000 naluconfigs-11.0.0/src/naluconfigs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-01 23:43:16.000000 naluconfigs-11.0.0/src/naluconfigs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-01 23:43:16.000000 naluconfigs-11.0.0/src/naluconfigs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:43:16.134607 naluconfigs-11.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/tests/test_hex_addr_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/tests/test_i2c_registers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/tests/test_multichip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/tests/test_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-06-01 23:42:59.000000 naluconfigs-11.0.0/tests/test_range_keys.py
```

### Comparing `naluconfigs-10.8.0/PKG-INFO` & `naluconfigs-11.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naluconfigs
-Version: 10.8.0
+Version: 11.0.0
 Summary: Home for board configs
 Home-page: 
 Author: Thomas Yang, Emily Lum
 Author-email: Marcus Luck <marcus@naluscientific.com>, Mitchell Matsumori-Kelly <mitchell@naluscientific.com>, Alvin Yang <alvin@naluscientific.com>, Kenneth Lauritzen <kenneth@naluscientific.com>, Ben Rotter <ben@naluscientific.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

### Comparing `naluconfigs-10.8.0/README.md` & `naluconfigs-11.0.0/README.md`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.8.0/pyproject.toml` & `naluconfigs-11.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.8.0/setup.py` & `naluconfigs-11.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.8.0/src/naluconfigs/__init__.py` & `naluconfigs-11.0.0/src/naluconfigs/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,21 @@
 import os
 import shutil
-import sys
 from pathlib import Path
 from typing import List, Tuple
 
 import numpy as np
 import yaml
 
-try:
-    from yaml import CDumper as Dumper
-    from yaml import CLoader as Loader
-except ImportError:
-    from yaml import Loader, Dumper
-
 from naluconfigs.exceptions import ConfigurationFileParsingError, InvalidBoardModelError
 from naluconfigs.postprocess import process_configuration as _process_configuration
 
+from . import _constructors
 from ._version import __version__
-
-# Determine bundle directory in case this package exists in a pyinstaller app
-if getattr(sys, "frozen", False) and hasattr(sys, "_MEIPASS"):
-    _BUNDLE_DIR = Path(sys._MEIPASS) / "naluconfigs"
-else:
-    _BUNDLE_DIR = Path(__file__).parent
-
-
-_CONFIGS_DIR = Path.cwd() / _BUNDLE_DIR / "data"
-_REGISTERS_DIR = _CONFIGS_DIR / "registers"
-_CLOCKS_DIR = _CONFIGS_DIR / "clocks"
+from .helpers import CLOCKS_DIR, REGISTERS_DIR
 
 _VALID_BOARDS = [
     "aardvarcv2",
     "aardvarcv3",
     "aardvarcv4",
     "aodsv1",
     "aodsv2_eval",
@@ -108,15 +92,14 @@
     # Create destination directory structure
     destination_dir = Path(destination_dir).resolve()
     (destination_dir / "registers").mkdir(parents=True, exist_ok=True)
     (destination_dir / "clocks").mkdir(exist_ok=True)
 
     # Copy over all the files for the requested board models
     for board in boards:
-
         # Copy the .yml file
         try:
             src_param_file = get_register_file(board)
             dest_param_file = destination_dir / "registers" / src_param_file.name
 
             shutil.copyfile(src_param_file, dest_param_file)
             output_paths[board] = {"registers_file": dest_param_file}
@@ -151,15 +134,15 @@
         OSError if the config file cannot be accessed
     """
     if model not in _VALID_BOARDS:
         raise InvalidBoardModelError(f'Invalid board model "{model}"')
 
     # Load the configs from file
     try:
-        yml_file = _REGISTERS_DIR / (model + ".yml")
+        yml_file = REGISTERS_DIR / (model + ".yml")
         result = get_configuration_from_file(yml_file)
     except OSError:
         raise
     except ConfigurationFileParsingError:
         raise
 
     return result
@@ -208,15 +191,15 @@
     Raises:
         InvalidBoardModelError if the model is not supported.
         FileNotFoundError if the config file cannot be found
     """
     if model not in _VALID_BOARDS:
         raise InvalidBoardModelError(f'Invalid board model "{model}"')
 
-    yml_file = _REGISTERS_DIR / (model + ".yml")
+    yml_file = REGISTERS_DIR / (model + ".yml")
     if not yml_file.exists():
         raise FileNotFoundError(f"Could not locate the register file at {yml_file}")
 
     return yml_file
 
 
 def get_clock(model: str) -> Tuple[list, Path]:
@@ -258,15 +241,15 @@
     if model not in _VALID_BOARDS:
         raise InvalidBoardModelError(f'Invalid board model "{model}"')
 
     # (wastefully) parse the params file to get the clock file name
     config = get_configuration(model)
 
     if "clock_file" in config["params"]:
-        return _CLOCKS_DIR / config["params"]["clock_file"]
+        return CLOCKS_DIR / config["params"]["clock_file"]
     else:
         return None
 
 
 def _load_yaml_file(filename) -> dict:
     """Loads a yaml file into a dict.
 
@@ -280,15 +263,15 @@
 
     Raises:
         OSError if file cannot be accessed.
         YAMLError if YAML file is not valid.
     """
     try:
         with open(filename, "r") as fp:
-            return yaml.load(fp, Loader=Loader)
+            return yaml.load(fp, Loader=_constructors.CustomYamlLoader)
     except OSError:
         raise
     except yaml.YAMLError:
         raise
 
 
 def _load_clock_file(filename) -> list:
```

### Comparing `naluconfigs-10.8.0/src/naluconfigs/data/clocks/AODS_300GCC.txt` & `naluconfigs-11.0.0/src/naluconfigs/data/clocks/AODS_300GCC.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.8.0/src/naluconfigs/data/clocks/AODS_8M.txt` & `naluconfigs-11.0.0/src/naluconfigs/data/clocks/AODS_8M.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.8.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2-13GSa_711MGCC-Registers.txt` & `naluconfigs-11.0.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2-13GSa_711MGCC-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.8.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2_GCC781_DebugSE-Registers.txt` & `naluconfigs-11.0.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2_GCC781_DebugSE-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.8.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv3_GCC781_DebugSE-Registers.txt` & `naluconfigs-11.0.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv3_GCC781_DebugSE-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.8.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv4_GCC781_DebugSE-Registers.txt` & `naluconfigs-11.0.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv4_GCC781_DebugSE-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.8.0/src/naluconfigs/data/clocks/Si5341-RevD-ASoC_lambchop-Registers.txt` & `naluconfigs-11.0.0/src/naluconfigs/data/clocks/Si5341-RevD-ASoC_lambchop-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.8.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_15_625SysClk_400GccClk-Registers.txt` & `naluconfigs-11.0.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_15_625SysClk_400GccClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.8.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GCCclk-Registers.txt` & `naluconfigs-11.0.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GCCclk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.8.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GccClk_156_25TxClk_31_25TxDivClk-Registers.txt` & `naluconfigs-11.0.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GccClk_156_25TxClk_31_25TxDivClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.8.0/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR-NexysFMC_78_125SysClk_312_5GccClk-Registers.txt` & `naluconfigs-11.0.0/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR-NexysFMC_78_125SysClk_312_5GccClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.8.0/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR_78_125SysClk_312_5GccClk-Registers.txt` & `naluconfigs-11.0.0/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR_78_125SysClk_312_5GccClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.8.0/src/naluconfigs/data/clocks/Si5341-RevD-Lambchop-Registers_compSysclk.txt` & `naluconfigs-11.0.0/src/naluconfigs/data/clocks/Si5341-RevD-Lambchop-Registers_compSysclk.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.8.0/src/naluconfigs/data/clocks/Si5341-RevD-TR-BHM_78_125SysClk_781_25GccClk-Registers.txt` & `naluconfigs-11.0.0/src/naluconfigs/data/clocks/Si5341-RevD-TR-BHM_78_125SysClk_781_25GccClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.8.0/src/naluconfigs/data/clocks/Si5341-RevD-UDC_78_125SlowClk_78_125IntermediateClk_312_5FastClk-Registers.txt` & `naluconfigs-11.0.0/src/naluconfigs/data/clocks/Si5341-RevD-UDC_78_125SlowClk_78_125IntermediateClk_312_5FastClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.8.0/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_GCC450M_debugse3125-Registers.txt` & `naluconfigs-11.0.0/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_GCC450M_debugse3125-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.8.0/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_simple_GCC300M_Registers.txt` & `naluconfigs-11.0.0/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_simple_GCC300M_Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.8.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC123M_1xSysClk_v32andup_6250ksed.txt` & `naluconfigs-11.0.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC123M_1xSysClk_v32andup_6250ksed.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.8.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup.txt` & `naluconfigs-11.0.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.8.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup_6250ksed.txt` & `naluconfigs-11.0.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup_6250ksed.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.8.0/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt` & `naluconfigs-11.0.0/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.8.0/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC450M_1xSysClk_v32andup_6250ksed.txt` & `naluconfigs-11.0.0/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC450M_1xSysClk_v32andup_6250ksed.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.8.0/src/naluconfigs/data/clocks/Si5341_TRBHM_10GSaps_GCCsstx2_Registers.txt` & `naluconfigs-11.0.0/src/naluconfigs/data/clocks/Si5341_TRBHM_10GSaps_GCCsstx2_Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.8.0/src/naluconfigs/data/registers/aardvarcv2.yml` & `naluconfigs-11.0.0/src/naluconfigs/data/registers/aardvarcv2.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.8.0/src/naluconfigs/data/registers/aardvarcv3.yml` & `naluconfigs-11.0.0/src/naluconfigs/data/registers/asocv2.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,743 +1,692 @@
-model: aardvarcv3
+model: asocv2
 features:
-  adc2mv: true
-  dac_sweep: true
-  ext_dac: true
+  adc2mv: false
+  dac_sweep: false
   pedestals: true
   threshold_scan: true
   tia_dac: false
-  timing_calibration: true
-  naludaq_rs: true
+  timing_calibration: false
+  naludaq_rs: false
 params:
-  chanmask: 3072
+  chanmask: 1536
   channels: 4
-  chanshift: 10
-  clock_file: Si5341-RevD-AARDVARCv3_GCC781_DebugSE-Registers.txt
+  chanshift: 9
+  clock_file: Si5341_ASoCv2_GCC450M_1xSysClk_v32andup_6250ksed.txt
   connections:
     - serial
     - d2xx
-    - udp
   si5341_address: 0xE8
   default_baud:
-    115200: 53
-  default_baudrate: 115200
-  default_clock: 100000000.0
+    111111: 53
+  default_baudrate: 111111
+  default_clock: 96000000.0
   default_divider: 53
-  default_trigger_value: 1500
-  threshold_scan:
-    min_vref: 0
-    max_vref: 2500
-    start: 500
-    stop: 3500
-    stepsize: 5
-    units: counts
   expected_scalmon: 2500
   ext_dac:
-    chip: dac7578
-    max_mv: 1200
-    max_counts: 4095
+    chip: ad5675
+    max_mv: 2500
+    max_counts: 65535
     channels:
-      0..3: 2048
+      0..3: 30000
     address_mapping:
-      0..3: 0x4E
+      0..3: 0xC
     channel_mapping:
-      0: 2
-      1: 6
-      2: 3
-      3: 7
+      0: 1
+      1: 0
+      2: 5
+      3: 4
   headers: 3
-  new_firmware: True
-  numregs: 64
-  pedestals_blocks: 16
+  numregs: 36
+  pedestals_blocks: 32
   peripherals:
-    current_1v2:
+    current:
       chan: 0
       addr: 0xD0
       bits: 16
       gain: 8
-      r_sense: 0.05
-    current_2v5:
-      chan: 1
-      addr: 0xD0
-      bits: 16
-      gain: 8
-      r_sense: 0.05
     vadjn:
       chan: 0
       addr: 0xD8
       bits: 16
       gain: 1
     vadjp:
       chan: 1
       addr: 0xD8
       bits: 16
       gain: 1
   possible_bauds:
-    115200: 53
-    230400: 26
-    691200: 8
-    1041667: 5
+    111111: 53
+    600000: 9
+    1500000: 3
   resolution: 12
   samples: 64
-  samplingrate: 10.0
+  samplingrate: 3.2
   stop_word: !!binary |
     +s4=
-  strobe_values_correction: True  # Shift the strobe values on certain boards with swapped internal routing.
-  strobe_correction_keys:
-    - calstrb_le
-    - calstrb_te
-    - wrstrb1_le
-    - wrstrb1_te
-    - wrstrb2_le
-    - wrstrb2_te
-    - wrsync1_le
-    - wrsync1_te
-    - wrsync2_le
-    - wrsync2_te
   wait: AE000001
-  wbias: 2000
-  windmask: 1022
-  windows: 510
+  wbias: 848
+  windmask: 510
+  windows: 254
+  yaml_version: 35.0
 registers:
   analog_registers:
-    cal:
-      address: 0x01
+    cmpbias:
+      address: 0x14
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 0
-    cal_buff:
-      address: 0x3B
+      value: 1000
+    cmpbias2:
+      address: 0x16
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 3500
-    cal_isel:
-      address: 0x3A
+      value: 737
+    dbbias:
+      address: 0x18
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 0
-    calstrb_le:
-      address: 0x25
+      value: 1300
+    isel:
+      address: 0x1B
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 0
-    calstrb_te:
-      address: 0x26
+      value: 2300
+    itbias:
+      address: 0x12
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 30
-    inp0vcurrn:
+      value: 2048
+    ittbias:
       address: 0x11
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 1604
-    inp0vcurrp:
-      address: 0x13
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2218
-    inp0vgmn:
-      address: 0x0D
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2389
-    inp0vgmp:
-      address: 0x0F
-      bitposition: 0
-      bitwidth: 12
+      value: 2048
+    mont_on:
+      address: 0x17
+      bitposition: 3
+      bitwidth: 1
       description: ''
       readwrite: w
-      value: 1536
-    inp1vcurrn:
-      address: 0x09
+      value: true
+    mont_select:
+      address: 0x17
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 3
       description: ''
       readwrite: w
-      value: 2218
-    inp1vcurrp:
-      address: 0x0B
+      value: 0
+    offset_00:
+      address: 0x01
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 1604
-    inp1vgmn:
-      address: 0x05
+      value: 0
+    offset_01:
+      address: 0x04
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2389
-    inp1vgmp:
+      value: 0
+    offset_02:
       address: 0x07
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 1536
-    inp2vcurrn:
-      address: 0x2A
+      value: 0
+    offset_03:
+      address: 0x0A
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 1604
-    inp2vcurrp:
-      address: 0x28
+      value: 0
+    pubias:
+      address: 0x15
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2218
-    inp2vgmn:
-      address: 0x2E
+      value: 3112
+    qbias:
+      address: 0x1C
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2389
-    inp2vgmp:
-      address: 0x2C
+      value: 2048
+    qbuff:
+      address: 0x1D
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 1536
-    inp3vcurrn:
-      address: 0x32
+      value: 2048
+    sbbias:
+      address: 0x19
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 1604
-    inp3vcurrp:
-      address: 0x30
+      value: 1300
+    scvbias0:
+      address: 0x0C
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2218
-    inp3vgmn:
-      address: 0x36
+      value: 800
+    scvbias1:
+      address: 0x0D
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2389
-    inp3vgmp:
-      address: 0x34
+      value: 800
+    scvbias2:
+      address: 0x0E
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 1536
-    isel:
-      address: 0x15
+      value: 800
+    scvbias3:
+      address: 0x0F
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2730
-    mont1_on:
-      address: 0x00
-      bitposition: 3
-      bitwidth: 1
-      description: ''
-      readwrite: w
-      value: false
-    mont1_select:
-      address: 0x00
-      bitposition: 4
-      bitwidth: 2
-      description: ''
-      readwrite: w
-      value: 0
-    mont2_on:
-      address: 0x00
-      bitposition: 0
+      value: 800
+    sgn:
+      address: 0x17
+      bitposition: 6
       bitwidth: 1
       description: ''
       readwrite: w
       value: false
-    mont2_select:
-      address: 0x00
-      bitposition: 1
-      bitwidth: 2
-      description: ''
-      readwrite: w
-      value: 0
-    qbias:
-      address: 0x18
+    sspin_le:
+      address: 0x2B
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2048
-    sc0_vbias:
-      address: 0x12
+      value: 100
+    sspin_te:
+      address: 0x2C
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 1570
-    sc0_vstab:
-      address: 0x10
-      bitposition: 0
-      bitwidth: 12
+      value: 25
+    sstin_ext:
+      address: 0x17
+      bitposition: 4
+      bitwidth: 1
       description: ''
       readwrite: w
-      value: 1365
-    sc1_vbias:
-      address: 0x0A
+      value: true
+    sstoutfb:
+      address: 0x22
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 1570
-    sc1_vstab:
-      address: 0x08
+      value: 119
+    tbbias:
+      address: 0x10
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 1365
-    sc2_vbias:
-      address: 0x29
+      value: 1000
+    trigger_threshold_00:
+      address: 0x00
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 1570
-    sc2_vstab:
-      address: 0x2B
+      value: 1800
+    trigger_threshold_01:
+      address: 0x03
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 1365
-    sc3_vbias:
-      address: 0x31
+      value: 1800
+    trigger_threshold_02:
+      address: 0x06
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 1570
-    sc3_vstab:
-      address: 0x33
+      value: 1800
+    trigger_threshold_03:
+      address: 0x09
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 1365
-    sgn:
-      address: 0x00
-      bitposition: 10
-      bitwidth: 1
-      description: ''
-      readwrite: w
-      value: false
-    sspin:
-      address: 0x00
-      bitposition: 6
-      bitwidth: 2
-      description: ''
-      readwrite: w
-      value: 3
-    sstin_sel:
-      address: 0x00
-      bitposition: 9
+      value: 1800
+    tsel:
+      address: 0x17
+      bitposition: 5
       bitwidth: 1
       description: ''
       readwrite: w
       value: true
-    sta_vcomp:
-      address: 0x02
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 1000
     vadjn:
-      address: 0x1C
+      address: 0x1E
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 1696
-    vadjn_sw:
-      address: 0x00
-      bitposition: 8
-      bitwidth: 1
-      description: ''
-      readwrite: w
-      value: true
+      value: 1550
     vadjp:
-      address: 0x19
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 0
-    vlimn:
-      address: 0x1B
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 0
-    vlimp:
-      address: 0x1A
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 4095
-    trigger_threshold_00:
-      address: 0x0E
+      address: 0x20
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 0
-    trigger_threshold_01:
-      address: 0x06
+      value: 2200
+    vanbuff:
+      address: 0x1F
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
       value: 0
-    trigger_threshold_02:
-      address: 0x2D
+    vapbuff:
+      address: 0x21
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 0
-    trigger_threshold_03:
-      address: 0x35
+      value: 2816
+    vdischarge:
+      address: 0x1A
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
       value: 0
-    vrmpvbias:
-      address: 0x17
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 1570
-    vtune:
-      address: 0x16
+    wbbias:
+      address: 0x13
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 1365
+      value: 2048
     wbias_00:
-      address: 0x0C
+      address: 0x02
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2000
+      value: 700
     wbias_01:
-      address: 0x04
+      address: 0x05
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2000
+      value: 700
     wbias_02:
-      address: 0x2F
+      address: 0x08
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2000
+      value: 700
     wbias_03:
-      address: 0x37
+      address: 0x0B
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2000
-    wrstrb1_le:
-      address: 0x1D
+      value: 700
+    wr_strb1_le:
+      address: 0x23
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 40
-    wrstrb1_te:
-      address: 0x1E
+      value: 64
+    wr_strb1_te:
+      address: 0x24
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 100
-    wrstrb2_le:
-      address: 0x21
+      value: 83
+    wr_strb2_le:
+      address: 0x25
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 103
-    wrstrb2_te:
-      address: 0x22
+      value: 0
+    wr_strb2_te:
+      address: 0x26
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 36
-    wrsync1_le:
-      address: 0x1F
+      value: 29
+    wr_sync1_le:
+      address: 0x27
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 0
-    wrsync1_te:
-      address: 0x20
+      value: 10
+    wr_sync1_te:
+      address: 0x28
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
       value: 50
-    wrsync2_le:
-      address: 0x23
+    wr_sync2_le:
+      address: 0x29
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 64
-    wrsync2_te:
-      address: 0x24
+      value: 80
+    wr_sync2_te:
+      address: 0x2A
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 114
+      value: 110
   control_registers:
-    1v2_en:
-      address: 0x17
-      bitposition: 1
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: true
     2v5_en:
-      address: 0x17
+      address: 0x16
       bitposition: 0
       bitwidth: 1
       description: ''
       readwrite: rw
       value: true
-    3v3_i2c_en:
-      address: 0x17
-      bitposition: 2
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: true
-    8b10b_en:
-      address: 0x19
-      bitposition: 12
+    2v5_pll_en:
+      address: 0x16
+      bitposition: 1
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
+      value: false
     addr:
-      address: 0x16
+      address: 0x15
       bitposition: 0
       bitwidth: 9
       description: ''
       readwrite: rw
       value: 0
     addr_user:
-      address: 0x16
+      address: 0x15
       bitposition: 15
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
+    brightness_blue:
+      address: 0x0A
+      bitposition: 0
+      bitwidth: 8
+      description: ''
+      readwrite: rw
+      value: 0
+    brightness_red:
+      address: 0x0B
+      bitposition: 0
+      bitwidth: 8
+      description: ''
+      readwrite: rw
+      value: 0
+    brightness_white:
+      address: 0x0A
+      bitposition: 8
+      bitwidth: 8
+      description: ''
+      readwrite: rw
+      value: 0
     chansel:
       address: 0x06
       bitposition: 12
       bitwidth: 4
       description: ''
       readwrite: rw
       value: 15
-    clk1v8_en:
-      address: 0x17
-      bitposition: 4
+    clk_1v8_nshutdown:
+      address: 0x16
+      bitposition: 2
       bitwidth: 1
       description: ''
       readwrite: rw
       value: true
-    clk2v5_en:
-      address: 0x17
-      bitposition: 3
+    clk_2v5_en:
+      address: 0x16
+      bitposition: 6
       bitwidth: 1
       description: ''
       readwrite: rw
       value: true
-    clk_fdec:
-      address: 0x17
-      bitposition: 9
+    clk_i2c_sel:
+      address: 0x16
+      bitposition: 5
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: false
-    clk_finc:
-      address: 0x17
-      bitposition: 8
+      value: true
+    clk_noe:
+      address: 0x16
+      bitposition: 4
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
-    clk_i2c_sel:
-      address: 0x17
-      bitposition: 5
+    clk_nrst:
+      address: 0x16
+      bitposition: 3
       bitwidth: 1
       description: ''
       readwrite: rw
       value: true
-    clk_oeb:
-      address: 0x17
-      bitposition: 6
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    clk_reset:
-      address: 0x17
+    clk_nsync:
+      address: 0x16
       bitposition: 7
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
-    clk_sync:
-      address: 0x17
+    dac_nrst:
+      address: 0x16
       bitposition: 10
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: false
+      value: 1
     data:
       address: 0x14
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
     data_user:
       address: 0x14
       bitposition: 15
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
-    debug_data:
-      address: 0x15
-      bitposition: 0
-      bitwidth: 12
+    digrst:
+      address: 0x16
+      bitposition: 9
+      bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    debug_data_user:
-      address: 0x15
-      bitposition: 15
+    digser_8b10b_en:
+      address: 0x1D
+      bitposition: 12
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
-    digrst:
-      address: 0x16
-      bitposition: 9
-      bitwidth: 1
+    digser_numwords:
+      address: 0x1D
+      bitposition: 2
+      bitwidth: 6
       description: ''
       readwrite: rw
       value: 0
-    digser_rst:
-      address: 0x19
+    digser_oneshot:
+      address: 0x1D
+      bitposition: 1
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: false
+    digser_reset:
+      address: 0x1D
       bitposition: 13
       bitwidth: 1
       description: ''
       readwrite: rw
+      value: false
+    digser_rx_en:
+      address: 0x1D
+      bitposition: 0
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: false
+    digser_slow_sysclk:
+      address: 0x1D
+      bitposition: 10
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: 0
+    digser_speed:
+      address: 0x1D
+      bitposition: 8
+      bitwidth: 2
+      description: ''
+      readwrite: rw
       value: 0
+    digser_tx_en:
+      address: 0x1D
+      bitposition: 11
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: false
+    ext_en:
+      address: 0x0B
+      bitposition: 9
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: true
     exttrig:
       address: 0x04
       bitposition: 10
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
+    fake:
+      address: 0x06
+      bitposition: 0
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: 0
     gccclr:
       address: 0x04
-      bitposition: 4
+      bitposition: 3
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: false
+    i2c_sel:
+      address: 0x16
+      bitposition: 11
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
+    i2c_switch:
+      address: 0x16
+      bitposition: 8
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: 0
     identifier:
       address: 0x00
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
-      value: 43714
-    iomode0:
-      address: 0x04
-      bitposition: 0
+      value: 0
+    in_sel:
+      address: 0x0B
+      bitposition: 12
       bitwidth: 1
       description: ''
       readwrite: rw
       value: true
-    iomode1:
+    iomode0:
       address: 0x04
-      bitposition: 6
+      bitposition: 7
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: false
-    leds:
-      address: 0x18
-      bitposition: 0
-      bitwidth: 16
+      value: 1
+    iomode1:
+      address: 0x04
+      bitposition: 8
+      bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
     loadwait:
       address: 0x07
       bitposition: 8
       bitwidth: 4
       description: ''
       readwrite: rw
       value: 15
+    nasa_trig_sel_ext:
+      address: 0x1D
+      bitposition: 15
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: true
     nramp:
       address: 0x04
-      bitposition: 5
+      bitposition: 4
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
     nrw:
       address: 0x04
       bitposition: 11
@@ -748,38 +697,45 @@
     numwinds:
       address: 0x08
       bitposition: 0
       bitwidth: 8
       description: ''
       readwrite: rw
       value: 1
+    out_sel:
+      address: 0x0B
+      bitposition: 11
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: false
     pclk:
       address: 0x04
-      bitposition: 2
+      bitposition: 1
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
     pclkwidth:
       address: 0x07
       bitposition: 12
       bitwidth: 4
       description: ''
       readwrite: rw
       value: 15
-    ramplen:
-      address: 0x06
-      bitposition: 0
-      bitwidth: 12
+    rden:
+      address: 0x04
+      bitposition: 6
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 2000
+      value: false
     regclr:
       address: 0x04
-      bitposition: 1
+      bitposition: 0
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
     runevs:
       address: 0x05
       bitposition: 0
@@ -804,21 +760,14 @@
     rx_data2:
       address: 0x1C
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
-    rx_data3:
-      address: 0x1D
-      bitposition: 0
-      bitwidth: 16
-      description: ''
-      readwrite: rw
-      value: 0
     rx_data4:
       address: 0x1E
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
@@ -869,160 +818,146 @@
       bitposition: 12
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
     selany:
       address: 0x04
-      bitposition: 3
+      bitposition: 2
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
-    slow_sysclk:
-      address: 0x19
-      bitposition: 10
+    sst_speed:
+      address: 0x1D
+      bitposition: 14
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
+      value: false
     stopacq:
       address: 0x04
       bitposition: 13
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
+    switch_nen:
+      address: 0x0B
+      bitposition: 13
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: true
     syncloc:
-      address: 0x09
+      address: 0x0E
       bitposition: 0
       bitwidth: 8
       description: ''
       readwrite: rw
       value: 0
-    sysclk:
-      address: 0x04
-      bitposition: 8
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
     sysrst:
       address: 0x04
-      bitposition: 9
+      bitposition: 14
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: true
-    tx_en:
-      address: 0x19
-      bitposition: 11
+      value: false
+    trig_sel:
+      address: 0x0B
+      bitposition: 10
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
+      value: false
     windsel:
       address: 0x07
       bitposition: 0
       bitwidth: 8
       description: ''
       readwrite: rw
       value: 0
-    wrstrboff:
+    wren:
       address: 0x04
-      bitposition: 7
+      bitposition: 5
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
   digital_registers:
-    bank:
-      address: 0x1D
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: rw
-      value: 0
-    banknum:
-      address: 0x9D
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: rw
-      value: 0
     chipid:
       address: 0x89
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 2730
-    donetimeoutn:
-      address: 0xA0
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: rw
-      value: 0
     convertresetwait:
       address: 0x84
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 1
     enabletestpatt:
       address: 0x88
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
-    excludechannelmask:
-      address: 0x96
+    fineoffset:
+      address: 0x8D
       bitposition: 0
-      bitwidth: 4
+      bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
     loadwait:
       address: 0x8B
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
-    miscreg:
-      address: 0x8D
+    masktrig:
+      address: 0x90
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
     pclkwidth:
       address: 0x8C
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
-    readoutchannels:
-      address: 0x87
+    pll:
+      address: 0x93
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
     readoutlookback:
       address: 0x85
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 18
+    readoutoffset:
+      address: 0x87
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: rw
+      value: 122
     readoutwindows:
       address: 0x86
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 10
@@ -1071,85 +1006,92 @@
     scalmon:
       address: 0x08
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
-    scs_misc:
-      address: 0x9E
+    speed:
+      address: 0x92
       bitposition: 0
       bitwidth: 12
-      description: 'Controls the cap/comparator variants in the test structure'
+      description: ''
       readwrite: rw
       value: 0
     testpatin:
       address: 0x0A
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
-    test_dline:
-      address: 0x9F
+    waitaddr:
+      address: 0x8F
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: rw
+      value: 0
+    waitread:
+      address: 0x8E
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
     wraddrjunk:
       address: 0x82
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
-      value: 255
+      value: 127
     wraddrstart:
       address: 0x80
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
     wraddrstop:
       address: 0x81
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
-      value: 254
+      value: 126
     writeaftertrig:
       address: 0x83
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 5
+    writedelay:
+      address: 0x91
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: rw
+      value: 0
   i2c_registers:
     i2c_en:
-      address: 0x0F
+      address: 0x09
       bitposition: 14
       bitwidth: 1
       description: ''
       readwrite: rw
       value: true
     i2c_send:
       address: 0x0F
       bitposition: 15
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    i2c_words:
-      address: 0x0F
-      bitposition: 8
-      bitwidth: 3
-      description: ''
-      readwrite: rw
-      value: 0
     i2c_addr:
       address: 0x0F
       bitposition: 0
       bitwidth: 8
       description: ''
       readwrite: rw
       value: 0
@@ -1177,35 +1119,42 @@
     i2c_data3:
       address: 0x13
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
+    i2c_words:
+      address: 0x0F
+      bitposition: 8
+      bitwidth: 3
+      description: ''
+      readwrite: rw
+      value: 0
     response0:
-      address: 0x48
+      address: 0x2C
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: r
       value: 0
     response1:
-      address: 0x49
+      address: 0x2D
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: r
       value: 0
     response2:
-      address: 0x4A
+      address: 0x2E
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: r
       value: 0
     response3:
-      address: 0x4B
+      address: 0x2F
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: r
       value: 0
```

### Comparing `naluconfigs-10.8.0/src/naluconfigs/data/registers/aardvarcv4.yml` & `naluconfigs-11.0.0/src/naluconfigs/data/registers/aardvarcv4.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.8.0/src/naluconfigs/data/registers/aodsoc_aods.yml` & `naluconfigs-11.0.0/src/naluconfigs/data/registers/hiper_fmc.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,598 +1,496 @@
-model: aodsoc_aods
+model: hiper_fmc
 features:
-  adc2mv: true
-  dac_sweep: true
-  ext_dac: true
+  adc2mv: false
+  dac_sweep: false
+  ext_dac: false
   pedestals: true
-  threshold_scan: true
+  threshold_scan: false
   tia_dac: false
   timing_calibration: false
-  naludaq_rs: true
+  naludaq_rs: false
 params:
-  chanmask: 0x300
-  channels: 8
-  chanshift: 8
-  # clock_file: '' # AODSoC boards have fixed clocks
+  chanmask: 3072
+  channels: 4
+  chanshift: 10
+  clock_file: Si5341-RevD-HIPeR-NexysFMC_78_125SysClk_312_5GccClk-Registers.txt
   connections:
     - serial
     - d2xx
-  si5341_address: 0xEE
-  timing_hack: false
+  si5341_address: 0xE8
   default_baud:
-    115200: 868
-  default_baudrate: 115200
+    3000000: 33
+  default_baudrate: 3000000
   default_clock: 100000000.0
-  default_divider: 868
-  default_isel:
-    0: 2610
-    1: 2627
+  default_divider: 33
   default_trigger_value: 1500
-  threshold_scan:
-    min_vref: 0
-    max_vref: 2500
-    start: 500
-    stop: 3500
-    stepsize: 5
-    units: counts
   expected_scalmon: 2500
   ext_dac:
-    chip: dac7578
-    max_mv: 2500
+    max_mv: 1200
     max_counts: 4095
     channels:
-      0..7: 2048
-    address_mapping:
-      0..7: 0x48
-    channel_mapping:
-      0: 7
-      1: 5
-      2: 3
-      3: 1
-      4: 0
-      5: 2
-      6: 4
-      7: 6
+      0: 2048
+      1: 2048
+      2: 2048
+      3: 2048
   headers: 3
   numregs: 64
   pedestals_blocks: 16
-  peripherals:
-    vadjn_0:
-      chan: 3
-      addr: 0x4C
-    vadjn_1:
-      chan: 2
-      addr: 0x4C
-    ldo_voltage:
-      chan: 1
-      addr: 0x4C
-    chip_voltage:
-      chan: 2
-      addr: 0x4C
-    current_resistor: 0.010
   possible_bauds:
-    115200: 868
-    1000000: 100
-    2000000: 50
+    # 115200: 53
+    # 230400: 26
+    # 691200: 8
+    # 1041667: 5
     3000000: 33
   resolution: 12
   samples: 64
-  samplingrate: 1.0
-  stop_word: "cafe"
+  samplingrate: 10.0
+  stop_word: !!binary |
+    pa9a/Dw8
   wait: AE000001
   wbias: 848
-  windmask: 0x0FF
-  windows: 254
+  windmask: 1022
+  windows: 64
 registers:
   analog_registers:
-    cmpbias:
-      address: 0x14
+    cal:
+      address: 0x01
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 1000
-    cmpbias2:
-      address: 0x16
+      value: 0
+    cal_buff:
+      address: 0x3B
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 737
-    dbbias:
-      address: 0x18
+      value: 3500
+    cal_isel:
+      address: 0x3A
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 1300
-    isel:
-      address: 0x1B
+      value: 0
+    calstrb_le:
+      address: 0x25
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2300  # 2680
-    itbias:
-      address: 0x12
+      value: 1 # 0
+    calstrb_te:
+      address: 0x26
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2048
-    ittbias:
+      value: 61 # 30
+    inp0vcurrn:
       address: 0x11
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2048
-    mont_on:
-      address: 0x17
-      bitposition: 3
-      bitwidth: 1
-      description: ''
-      readwrite: w
-      value: 0
-    mont_select:
-      address: 0x17
+      value: 1604
+    inp0vcurrp:
+      address: 0x13
       bitposition: 0
-      bitwidth: 3
+      bitwidth: 12
       description: ''
       readwrite: w
-      value: 0
-    offset_00:
-      address: 0x01
+      value: 2218
+    inp0vgmn:
+      address: 0x0D
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 0
-    offset_01:
-      address: 0x04
+      value: 2389
+    inp0vgmp:
+      address: 0x0F
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 0
-    offset_02:
-      address: 0x07
+      value: 1536
+    inp1vcurrn:
+      address: 0x09
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 0
-    offset_03:
-      address: 0x0A
+      value: 2218
+    inp1vcurrp:
+      address: 0x0B
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 0
-    pubias:
-      address: 0x15
+      value: 1604
+    inp1vgmn:
+      address: 0x05
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 3112
-    qbias:
-      address: 0x1C
+      value: 2389
+    inp1vgmp:
+      address: 0x07
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2048
-    qbuff:
-      address: 0x1D
+      value: 1536
+    inp2vcurrn:
+      address: 0x2A
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2048
-    sbbias:
-      address: 0x19
+      value: 1604
+    inp2vcurrp:
+      address: 0x28
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 1300
-    sel_0:
-      address: 0x80
-      bitposition: 10
-      bitwidth: 1
-      description: 'Ch0 Input MUX - 0: RF0 Input; 1: Buffered version of RF Input'
-      readwrite: w
-      value: 0
-    sel_1:
-      address: 0x80
-      bitposition: 11
-      bitwidth: 1
-      description: 'Ch0 Input MUX - 0: RF1 Input; 1: Output of Ch1 Gain MUX'
-      readwrite: w
-      value: 0
-    sel_2:
-      address: 0x80
-      bitposition: 0
-      bitwidth: 1
-      description: 'Ch0 Input MUX - 0: RF2 Input; 1: Buffered (w/gain) copy of Ch1; unity gain controlled by VBIAS3_1-2'
-      readwrite: w
-      value: 0
-    sel_3:
-      address: 0x80
-      bitposition: 1
-      bitwidth: 1
-      description: 'Ch0 Input MUX - 0: RF3 Input; 1: Output of Ch3 Gain MUX'
-      readwrite: w
-      value: 0
-    sel_4:
-      address: 0x80
-      bitposition: 2
-      bitwidth: 1
-      description: 'Ch0 Input MUX - 0: OUT3 OFF (HiZ); 1: Buffered version of RF Input'
-      readwrite: w
-      value: 0
-    sel_5:
-      address: 0x80
-      bitposition: 3
-      bitwidth: 1
-      description: 'Ch1 gain MUX: 0: 8x then unity gain; 1: 3-stage amp then unity gain controlled by VBIAS2_3-4'
-      readwrite: w
-      value: 0
-    sel_6:
-      address: 0x80
-      bitposition: 5
-      bitwidth: 1
-      description: 'Ch3 gain MUX: 0: 8x then unity gain; 1: 3-stage amp then unity gain controlled by VBIAS4_3-4'
-      readwrite: w
-      value: 0
-    sel_7:
-      address: 0x80
-      bitposition: 4
-      bitwidth: 1
-      description: 'Gain Stage Input for Ch3; 0: Output from CH2 1: Output from CH0'
-      readwrite: w
-      value: 0
-    scvbias0:
-      address: 0x0D
+      value: 2218
+    inp2vgmn:
+      address: 0x2E
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2048 #800  # 1800?
-    scvbias1:
-      address: 0x0E
+      value: 2389
+    inp2vgmp:
+      address: 0x2C
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2048 #800  # 1800?
-    scvbias2:
-      address: 0x0F
+      value: 1536
+    inp3vcurrn:
+      address: 0x32
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2048 #800  # 1800?
-    scvbias3:
-      address: 0x10
+      value: 1604
+    inp3vcurrp:
+      address: 0x30
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2048 #800  # 1800?
-    sgn:
-      address: 0x17
-      bitposition: 6
-      bitwidth: 1
+      value: 2218
+    inp3vgmn:
+      address: 0x36
+      bitposition: 0
+      bitwidth: 12
       description: ''
       readwrite: w
-      value: 0
-    sspin_le:
-      address: 0x2B
+      value: 2389
+    inp3vgmp:
+      address: 0x34
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 100
-    sspin_te:
-      address: 0x2C
+      value: 1536
+    isel:
+      address: 0x15
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 25
-    sstin_ext:
-      address: 0x17
-      bitposition: 4
+      value: 2730
+    mont1_on:
+      address: 0x00
+      bitposition: 3
       bitwidth: 1
       description: ''
       readwrite: w
-      value: 0
-    sstoutfb:
-      address: 0x22
-      bitposition: 0
-      bitwidth: 12
+      value: false
+    mont1_select:
+      address: 0x00
+      bitposition: 4
+      bitwidth: 2
       description: ''
       readwrite: w
-      value: 126
-    tbbias:
-      address: 0x0C
+      value: 0
+    mont2_on:
+      address: 0x00
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 1
       description: ''
       readwrite: w
-      value: 1000
-    trigger_threshold_00:
+      value: false
+    mont2_select:
       address: 0x00
-      bitposition: 0
-      bitwidth: 12
+      bitposition: 1
+      bitwidth: 2
       description: ''
       readwrite: w
-      value: 1800
-    trigger_threshold_01:
-      address: 0x03
+      value: 0
+    qbias:
+      address: 0x18
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 1800
-    trigger_threshold_02:
-      address: 0x06
+      value: 2048
+    sc0_vbias:
+      address: 0x12
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 1800
-    trigger_threshold_03:
-      address: 0x09
+      value: 1570
+    sc0_vstab:
+      address: 0x10
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 1800
-    tsel:
-      address: 0x17
-      bitposition: 5
-      bitwidth: 1
-      description: ''
-      readwrite: w
-      value: 1
-    tsbias_1:
-      address: 0x8A
+      value: 1365
+    sc1_vbias:
+      address: 0x0A
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 0
-    tsbias_2:
-      address: 0x8B
+      value: 1570
+    sc1_vstab:
+      address: 0x08
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 0
-    vadjn:
-      address: 0x1E
+      value: 1365
+    sc2_vbias:
+      address: 0x29
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 1550
-    vadjp:
-      address: 0x20
+      value: 1570
+    sc2_vstab:
+      address: 0x2B
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2200
-    vanbuff:
-      address: 0x1F
+      value: 1365
+    sc3_vbias:
+      address: 0x31
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 0
-    vapbuff:
-      address: 0x21
+      value: 1570
+    sc3_vstab:
+      address: 0x33
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2816
-    vbias0_0:
-      address: 0x81
-      bitposition: 0
-      bitwidth: 12
+      value: 1365
+    sgn:
+      address: 0x00
+      bitposition: 10
+      bitwidth: 1
       description: ''
       readwrite: w
-      value: 2801
-    vbias0_1:
-      address: 0x82
-      bitposition: 0
-      bitwidth: 12
+      value: false
+    sspin:
+      address: 0x00
+      bitposition: 6
+      bitwidth: 2
       description: ''
       readwrite: w
-      value: 2604
-    vbias1_0:
-      address: 0x85
-      bitposition: 0
-      bitwidth: 12
+      value: 3
+    sstin_sel:
+      address: 0x00
+      bitposition: 9
+      bitwidth: 1
       description: ''
       readwrite: w
-      value: 2801
-    vbias1_1:
-      address: 0x84
+      value: true
+    sta_vcomp:
+      address: 0x02
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2604
-    vbias1_2:
-      address: 0x89
+      value: 1000
+    vadjn:
+      address: 0x1C
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 0
-    vbias1_3:
-      address: 0x90
+      value: 1696
+    vadjn_sw:
+      address: 0x00
+      bitposition: 8
+      bitwidth: 1
+      description: ''
+      readwrite: w
+      value: true
+    vadjp:
+      address: 0x19
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
       value: 0
-    vbias2_0:
-      address: 0x86
+    vlimn:
+      address: 0x1B
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2801
-    vbias2_1:
-      address: 0x87
+      value: 0
+    vlimp:
+      address: 0x1A
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2604
-    vbias3_0:
-      address: 0x92
+      value: 4095
+    trigger_threshold_00:
+      address: 0x0E
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2801
-    vbias3_1:
-      address: 0x88
+      value: 0
+    trigger_threshold_01:
+      address: 0x06
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2604
-    vbias3_2:
-      address: 0x91
+      value: 0
+    trigger_threshold_02:
+      address: 0x2D
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
       value: 0
-    vbias3_3:
-      address: 0x93
+    trigger_threshold_03:
+      address: 0x35
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
       value: 0
-    vdischarge:
-      address: 0x1A
+    vrmpvbias:
+      address: 0x17
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 0
-    wbbias:
-      address: 0x13
+      value: 1570
+    vtune:
+      address: 0x16
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2048
+      value: 1365
     wbias_00:
-      address: 0x02
+      address: 0x0C
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 700
+      value: 0
     wbias_01:
-      address: 0x05
+      address: 0x04
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 700
+      value: 0
     wbias_02:
-      address: 0x08
+      address: 0x2F
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 700
+      value: 0
     wbias_03:
-      address: 0x0B
+      address: 0x37
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 700
-    wr_strb1_le:
-      address: 0x23
+      value: 0
+    wrstrb1_le:
+      address: 0x1D
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 64
-    wr_strb1_te:
-      address: 0x24
+      value: 114 # 40
+    wrstrb1_te:
+      address: 0x1E
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 83  #67 ??
-    wr_strb2_le:
-      address: 0x25
+      value: 54
+    wrstrb2_le:
+      address: 0x21
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 0
-    wr_strb2_te:
-      address: 0x26
+      value: 13 # 103
+    wrstrb2_te:
+      address: 0x22
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 29  # 3??
-    wr_sync1_le:
-      address: 0x27
+      value: 73 # 36
+    wrsync1_le:
+      address: 0x1F
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 10
-    wr_sync1_te:
-      address: 0x28
+      value: 1 # 0
+    wrsync1_te:
+      address: 0x20
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 50
-    wr_sync2_le:
-      address: 0x29
+      value: 101 #50
+    wrsync2_le:
+      address: 0x23
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 80
-    wr_sync2_te:
-      address: 0x2A
+      value: 126 # 64
+    wrsync2_te:
+      address: 0x24
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 110
+      value: 26 # 114
   control_registers:
-    i2c_bus_sel:
-      address: 0x14
-      bitposition: 0
-      bitwidth: 1
-      description: 'Select i2c bus 1 or 2, 0: i2c bus 1, 1: i2c bus 2'
-      readwrite: rw
-      value: false
     1v2_en:
       address: 0x17
       bitposition: 1
       bitwidth: 1
       description: ''
       readwrite: rw
       value: true
@@ -613,35 +511,35 @@
     8b10b_en:
       address: 0x19
       bitposition: 12
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    amp_pwrdn_out:
-      address: 0x1A
-      bitposition: 0
-      bitwidth: 8
-      description: 'Onboard amplifiers active high means amp off'
-      readwrite: rw
-      value: 0
     addr:
       address: 0x16
       bitposition: 0
       bitwidth: 9
       description: ''
       readwrite: rw
       value: 0
     addr_user:
       address: 0x16
       bitposition: 15
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
+    ard_trig_0_in:  # TODO: New register, verify address and value
+      address: 0x47
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: r
+      value: 0
     chansel:
       address: 0x06
       bitposition: 12
       bitwidth: 4
       description: ''
       readwrite: rw
       value: 15
@@ -697,14 +595,42 @@
     clk_sync:
       address: 0x17
       bitposition: 10
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
+    clk_sel0:  # TODO: Newly added, verify default value
+      address: 0x17
+      bitposition: 11
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: false
+    clk_sel1:  # TODO: Newly added, verify default value
+      address: 0x17
+      bitposition: 12
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: false
+    data:
+      address: 0x14
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: rw
+      value: 0
+    data_user:
+      address: 0x14
+      bitposition: 15
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: false
     debug_data:
       address: 0x15
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
@@ -725,70 +651,140 @@
     digser_rst:
       address: 0x19
       bitposition: 13
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
+    digser_tx_storage0:  # TODO: New register, verify address and value
+      address: 0x4D
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: r
+      value: 0
+    digser_tx_storage1:  # TODO: New register, verify address and value
+      address: 0x4E
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: r
+      value: 0
+    digser_tx_storage2:  # TODO: New register, verify address and value
+      address: 0x4F
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: r
+      value: 0
+    digser_tx_storage3:  # TODO: New register, verify address and value
+      address: 0x50
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: r
+      value: 0
+    digser_tx_storage4:  # TODO: New register, verify address and value
+      address: 0x51
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: r
+      value: 0
+    digser_tx_storage5:  # TODO: New register, verify address and value
+      address: 0x52
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: r
+      value: 0
+    digser_tx_storage6:  # TODO: New register, verify address and value
+      address: 0x53
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: r
+      value: 0
+    digser_tx_storage7:  # TODO: New register, verify address and value
+      address: 0x54
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: r
+      value: 0
+    digser_tx_storage8:  # TODO: New register, verify address and value
+      address: 0x55
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: r
+      value: 0
+    digser_tx_storage9:  # TODO: New register, verify address and value
+      address: 0x56
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: r
+      value: 0
     exttrig:
       address: 0x04
       bitposition: 10
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
     gccclr:
       address: 0x04
       bitposition: 4
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
-    idac_ldac:
-      address: 0x1B
+    iaddr_read:  # TODO: New register, verify address and value
+      address: 0x44
       bitposition: 0
-      bitwidth: 1
-      description: 'pin on AD7578'
-      readwrite: rw
-      value: 0
-    idac_nclr:
-      address: 0x1B
-      bitposition: 1
-      bitwidth: 1
-      description: 'pin on AD7578'
-      readwrite: rw
-      value: 1
-    fifo_unload_or_event_en:
-      address: 0x1F
-      bitposition: 0
-      bitwidth: 1
-      description: 'Once data is loaded into the FIFO it will not be sent out to the UART until the end of the current event. Use this mode for capturing sampled data events. '
-      readwrite: rw
+      bitwidth: 9
+      description: ''
+      readwrite: r
       value: 0
     identifier:
       address: 0x00
       bitposition: 0
       bitwidth: 16
+      description: 'Board model/version unique identifier'
+      readwrite: r
+      value: 43714
+    idigital_lastdigread:  # TODO: New register, verify address and value
+      address: 0x43
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: r
+      value: 0
+    idigital_readout_count:  # TODO: New register, verify address and value
+      address: 0x45
+      bitposition: 0
+      bitwidth: 16
       description: ''
-      readwrite: rw
-      value: 310
+      readwrite: r
+      value: 0
     iomode0:
       address: 0x04
       bitposition: 0
       bitwidth: 1
-      description: ''
+      description: 'HIPeR 10bit Serial Mode0=0'
       readwrite: rw
-      value: true
+      value: false
     iomode1:
       address: 0x04
       bitposition: 6
       bitwidth: 1
-      description: ''
+      description: 'HIPeR 10bit Serial Mode1=1'
       readwrite: rw
-      value: false
+      value: true
     leds:
       address: 0x18
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
@@ -851,14 +847,63 @@
     runevs:
       address: 0x05
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
       value: 1
+    rx_data0:
+      address: 0x1A
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: rw
+      value: 0
+    rx_data1:
+      address: 0x1B
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: rw
+      value: 0
+    rx_data2:
+      address: 0x1C
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: rw
+      value: 0
+    rx_data3:
+      address: 0x1D
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: rw
+      value: 0
+    rx_data4:
+      address: 0x1E
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: rw
+      value: 0
+    rx_data5:
+      address: 0x1F
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: rw
+      value: 0
+    rx_data6:
+      address: 0x20
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: rw
+      value: 0
     rx_en:
       address: 0x19
       bitposition: 0
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
@@ -900,14 +945,21 @@
     slow_sysclk:
       address: 0x19
       bitposition: 10
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
+    sst_double:  # TODO: OR rx_off?? John S documnentation ot clear
+      address: 0x19
+      bitposition: 14
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: 0
     stopacq:
       address: 0x04
       bitposition: 13
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
@@ -935,496 +987,517 @@
     tx_en:
       address: 0x19
       bitposition: 11
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
+    version:  # TODO: New register, verify address and value
+      address: 0x01
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: w
+      value: 0
     windsel:
       address: 0x07
       bitposition: 0
       bitwidth: 8
       description: ''
       readwrite: rw
       value: 0
     wrstrboff:
       address: 0x04
       bitposition: 7
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
-    rxout_pol:
-      address: 0x22
+    crc_en:
+      address: 0x21
       bitposition: 0
-      bitwidth: 16
-      description: ''
+      bitwidth: 1
+      description: 'HIPeR Serial Command CRC Enable'
       readwrite: rw
-      value: 6400
-    txin_pol:
-      address: 0x23
-      bitposition: 0
-      bitwidth: 16
-      description: ''
+      value: 0
+    eof_en:
+      address: 0x21
+      bitposition: 1
+      bitwidth: 1
+      description: 'HIPeR Serial Command EOF Enable'
       readwrite: rw
-      value: 4412
-    ard_header:
+      value: 0
+    header_en:
       address: 0x21
-      bitposition: 0
+      bitposition: 2
       bitwidth: 1
-      description: 'Enable AARDVARC debug header.'
+      description: 'HIPeR Chip data header, add a header to all data from a chip: BBB + chip_number(hex)'
       readwrite: rw
       value: 1
-    ard_rx_en:
-      address: 0x1D
+    footer_en:
+      address: 0x21
+      bitposition: 3
+      bitwidth: 1
+      description: 'HIPeR Chip data footer, add a footer to all data from a chip: FFF + chip_number(hex)'
+      readwrite: rw
+      value: 1
+    rxout_pol:
+      address: 0x22
       bitposition: 0
       bitwidth: 16
-      description: 'TR-BHM ASIC Rx Enable register 29dec. Bit 0 and 1 enable transmitting data to ASICs. Need to set these bits to send data to the ASICs'
+      description: 'HIPeR RxOut Input Polarity Control'
       readwrite: rw
-      value: 3
-    ard_tx_en:
-      address: 0x1E
+      value: 6400
+    txin_pol:
+      address: 0x23
       bitposition: 0
       bitwidth: 16
-      description: 'TR-BHM ASIC Tx Enable register 30dec. Bit 0 and 1 enable receiving data from ASICs. Need to set these bits to get data back from the ASICs'
+      description: 'HIPeR TxIn Output Polarity Control'
       readwrite: rw
-      value: 3
-    ard0_clk_sel:
+      value: 4412
+    txin_en:
       address: 0x24
       bitposition: 0
-      bitwidth: 2
-      description: ''
+      bitwidth: 16
+      description: 'HIPeR TxIn Input Enable. Data from ASIC to FPGA. Keep off unless receving data or registersfrom ASIC'
       readwrite: rw
       value: 0
-    ard1_clk_sel:
+    rxout_en:
       address: 0x25
       bitposition: 0
-      bitwidth: 2
-      description: ''
-      readwrite: rw
-      value: 1
-    motor_trig_en:
-      address: 0x27
-      bitposition: 0
-      bitwidth: 1
-      description: ''
+      bitwidth: 16
+      description: 'HIPeR RxOut Output Enable. Data from FPGA to ASIC. Keep on unless busy_locked is high.'
       readwrite: rw
-      value: 0
-    motor_trig_evts:
+      value: 65535
+    amp_pwrdn_n:
       address: 0x26
       bitposition: 0
       bitwidth: 16
-      description: ''
-      readwrite: rw
-      value: 1
-    oleas_en_trig:
-      address: 0x0A
-      bitposition: 10
-      bitwidth: 1
-      description: ''
+      description: 'HIPeR AMP PowerDown_n'
       readwrite: rw
       value: 0
-    oleas_pol_a:
-      address: 0x0A
-      bitposition: 11
+    # txin_logic:  # TODO: New register, verify address and value
+    #   address: 0x26
+    #   bitposition: 0
+    #   bitwidth: 16
+    #   description: ''
+    #   readwrite: rw
+    #   value: 0
+    v2v5_pwr_good:  # TODO: New register, verify address and value
+      address: 0x46
+      bitposition: 0
       bitwidth: 1
       description: ''
-      readwrite: rw
+      readwrite: r
       value: 0
-    oleas_pol_b:
-      address: 0x0A
-      bitposition: 12
+    v1v2_pwr_good:  # TODO: New register, verify address and value
+      address: 0x46
+      bitposition: 1
       bitwidth: 1
       description: ''
-      readwrite: rw
+      readwrite: r
       value: 0
-    oleas_en_a:
-      address: 0x0A
-      bitposition: 13
+    dac_r_update:
+      address: 0x27
+      bitposition: 15
       bitwidth: 1
-      description: ''
+      description: 'HIPeR SPI DAC Right Side Update Toggle'
       readwrite: rw
       value: 0
-    oleas_en_b:
-      address: 0x0A
-      bitposition: 14
-      bitwidth: 1
-      description: ''
+    dac_r_cmd:
+      address: 0x27
+      bitposition: 8
+      bitwidth: 4
+      description: 'HIPeR DAC Right Side SPI Command'
       readwrite: rw
-      value: 0
-    oleas_loop:
-      address: 0x0A
-      bitposition: 0
-      bitwidth: 5
-      description: ''
+      value: 3
+    dac_r_addr:
+      address: 0x27
+      bitposition: 4
+      bitwidth: 4
+      description: 'HIPeR DAC Right Side SPI Address'
       readwrite: rw
       value: 15
-    oleas_length_a:
-      address: 0x0B
+    dac_r_asic:
+      address: 0x27
       bitposition: 0
-      bitwidth: 16
-      description: ''
+      bitwidth: 4
+      description: 'HIPeR DAC Right Side ASIC Address'
       readwrite: rw
       value: 0
-    oleas_length_b:
-      address: 0x0D
+    dac_r_value:
+      address: 0x28
       bitposition: 0
-      bitwidth: 16
-      description: ''
+      bitwidth: 12
+      description: 'HIPeR DAC Right Side 12 bit Value'
       readwrite: rw
       value: 0
-    oleas_delay_a:
-      address: 0x0C
-      bitposition: 0
-      bitwidth: 16
-      description: ''
+    dac_l_update:
+      address: 0x29
+      bitposition: 15
+      bitwidth: 1
+      description: 'HIPeR SPI DAC Left Side Update Toggle'
       readwrite: rw
       value: 0
-    oleas_delay_b:
-      address: 0x0E
+    dac_l_cmd:
+      address: 0x29
+      bitposition: 8
+      bitwidth: 4
+      description: 'HIPeR DAC Left Side SPI Command'
+      readwrite: rw
+      value: 3
+    dac_l_addr:
+      address: 0x29
+      bitposition: 4
+      bitwidth: 4
+      description: 'HIPeR DAC Left Side SPI Address'
+      readwrite: rw
+      value: 15
+    dac_l_asic:
+      address: 0x29
       bitposition: 0
-      bitwidth: 16
-      description: ''
+      bitwidth: 4
+      description: 'HIPeR DAC Left Side ASIC Address'
       readwrite: rw
       value: 0
-    testmode:
-      address: 0x20
+    dac_l_value:
+      address: 0x2A
       bitposition: 0
-      bitwidth: 1
-      description: ''
+      bitwidth: 12
+      description: 'HIPeR DAC Left Side 12 bit Value'
       readwrite: rw
       value: 0
-  digital_registers:
-    chipid:
-      address: 0x89
+    exttrig_en:
+      address: 0x2B
       bitposition: 0
-      bitwidth: 12
-      description: ''
+      bitwidth: 16
+      description: 'HIPeR External Trigger Mask, set to one per chip'
       readwrite: rw
-      value: 2730
-    convertresetwait:
-      address: 0x84
+      value: 0
+    max_trig_count:
+      address: 0x2C
       bitposition: 0
-      bitwidth: 8
-      description: ''
+      bitwidth: 16
+      description: 'Maximum triggers before masking ext trig inputs'
       readwrite: rw
-      value: 1
-    enabletestpatt:
-      address: 0x88
+      value: 0
+    trig_count_reset:
+      address: 0x2D
       bitposition: 0
       bitwidth: 1
-      description: ''
+      description: 'Toggle to reset trig_count, if left at 1, triggers are disabled'
       readwrite: rw
       value: 0
-    excludechannelmask:
-      address: 0x96
+    idle_det:
+      address: 0x5D
       bitposition: 0
-      bitwidth: 4
-      description: ''
-      readwrite: rw
+      bitwidth: 16
+      description: 'HIPeR TxIn Idle Detect Status'
+      readwrite: r
       value: 0
-    fineoffset:
-      address: 0x8D
+    busy_locked:
+      address: 0x5C
       bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: rw
+      bitwidth: 16
+      description: 'HIPeR RxOut Busy_Locked Status'
+      readwrite: r
       value: 0
-    loadwait:
-      address: 0x8B
+  digital_registers:
+    bank:
+      address: 0x1D
       bitposition: 0
-      bitwidth: 7
+      bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
-    masktrig:
-      address: 0x90
+    pulselength32:  # TODO: New register, verify address and value
+      address: 0x9A
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
-    max0:
-      address: 0xA1
+    chipid:
+      address: 0x89
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
-      value: 0
-    max1:
-      address: 0xA2
+      value: 2730
+    convertresetwait:
+      address: 0x84
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
-      value: 0
-    max2:
-      address: 0xA3
+      value: 1
+    donetimeoutn:  # TODO: New register, verify address and value
+      address: 0xA0
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
-    max3:
-      address: 0xA4
+    enabletestpatt:
+      address: 0x88
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
-    min0:
-      address: 0x9D
+    excludechan:  # TODO: New register, verify address and value
+      address: 0x96
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 4
       description: ''
       readwrite: rw
       value: 0
-    min1:
-      address: 0x9E
+    loadwait:
+      address: 0x8B
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
-    min2:
-      address: 0x9F
+    masktrig:  # TODO: New register, verify address and value
+      address: 0x90
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
-    min3:
-      address: 0xA0
+    miscreg:
+      address: 0x8D
       bitposition: 0
       bitwidth: 12
-      description: ''
+      description: 'HIPeR MISCREG = 2'
       readwrite: rw
-      value: 0
+      value: 2
     pclkwidth:
       address: 0x8C
       bitposition: 0
-      bitwidth: 7
+      bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
-    pll:
+    pllmisc:  # TODO: New register, verify address and value
       address: 0x93
       bitposition: 0
-      bitwidth: 6
-      description: ''
+      bitwidth: 5
+      description: 'HIPeR PLLMISC = 0'
       readwrite: rw
       value: 0
-    pulselength10:
+    pulselength10:  # TODO: New register, verify address and value
       address: 0x99
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
-    pulselength32:
-      address: 0x9A
+    readoutchannels:
+      address: 0x87
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
     readoutlookback:
       address: 0x85
       bitposition: 0
-      bitwidth: 8
+      bitwidth: 12
       description: ''
       readwrite: rw
       value: 18
-    readoutoffset:
-      address: 0x87
-      bitposition: 0
-      bitwidth: 8
-      description: ''
-      readwrite: rw
-      value: 122
     readoutwindows:
       address: 0x86
       bitposition: 0
-      bitwidth: 8
+      bitwidth: 12
       description: ''
       readwrite: rw
       value: 10
     regclr:
       address: 0x8A
       bitposition: 0
-      bitwidth: 1
+      bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
-    roilength10:
+    roilength10:  # TODO: New register, verify address and value
       address: 0x9B
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
-    roilength32:
+    roilength32:  # TODO: New register, verify address and value
       address: 0x9C
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
     scal0:
       address: 0x00
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: w
+      readwrite: rw
       value: 0
     scal1:
       address: 0x01
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: w
+      readwrite: rw
       value: 0
     scal2:
       address: 0x02
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: w
+      readwrite: rw
       value: 0
     scal3:
       address: 0x03
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: w
+      readwrite: rw
       value: 0
     scalhigh:
       address: 0x40
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: w
+      readwrite: rw
       value: 0
     scalmon:
       address: 0x08
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: w
+      readwrite: rw
       value: 0
-    speed:
+    speed:  # TODO: New register, verify address and value
       address: 0x92
       bitposition: 0
       bitwidth: 10
       description: ''
       readwrite: rw
       value: 0
+    test_caps:  # TODO: New register, verify address and value
+      address: 0x9E
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: rw
+      value: 0
+    test_dline:  # TODO: New register, verify address and value
+      address: 0x9F
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: rw
+      value: 0
     testpatin:
       address: 0x0A
       bitposition: 0
-      bitwidth: 3
+      bitwidth: 12
       description: ''
-      readwrite: w
+      readwrite: rw
       value: 0
-    trigfinedelay10:
+    trigfinedelay10:  # TODO: New register, verify address and value
       address: 0x97
       bitposition: 0
       bitwidth: 8
       description: ''
       readwrite: rw
       value: 0
-    trigfinedelay32:
+    trigfinedelay32:  # TODO: New register, verify address and value
       address: 0x98
       bitposition: 0
       bitwidth: 8
       description: ''
       readwrite: rw
       value: 0
-    txspeed:
+    txspeed:  # TODO: New register, verify address and value
       address: 0x94
       bitposition: 0
-      bitwidth: 1
-      description: ''
+      bitwidth: 2
+      description: 'HIPeR TXSPEED = 2'
       readwrite: rw
-      value: 0
-    waitaddr:
+      value: 2
+    waitaddr:  # TODO: New register, verify address and value
       address: 0x8F
       bitposition: 0
       bitwidth: 3
       description: ''
       readwrite: rw
       value: 0
-    waitread:
+    waitread:  # TODO: New register, verify address and value
       address: 0x8E
       bitposition: 0
       bitwidth: 3
-      description: ''
+      description: 'HIPeR WAITREAD = 1'
       readwrite: rw
       value: 1
-    wlc_on:
+    wlc_on:  # TODO: New register, verify address and value
       address: 0x95
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
     wraddrjunk:
       address: 0x82
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
-      value: 127
+      value: 255
     wraddrstart:
       address: 0x80
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
     wraddrstop:
       address: 0x81
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
-      value: 126
+      value: 31
     writeaftertrig:
       address: 0x83
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 5
-    writedelay:
+    writedelay:  # TODO: New register, verify address and value
       address: 0x91
       bitposition: 0
       bitwidth: 3
       description: ''
       readwrite: rw
       value: 0
   i2c_registers:
     i2c_en:
       address: 0x0F
       bitposition: 14
       bitwidth: 1
       description: ''
       readwrite: rw
       value: true
-    # i2c_send:
-    #   address: 0x0F
-    #   bitposition: 15
-    #   bitwidth: 1
-    #   description: ''
-    #   readwrite: rw
-    #   value: 0
-    i2c_words:
+    i2c_send:
       address: 0x0F
-      bitposition: 8
-      bitwidth: 3
+      bitposition: 15
+      bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
     i2c_addr:
       address: 0x0F
       bitposition: 0
       bitwidth: 8
@@ -1455,14 +1528,21 @@
     i2c_data3:
       address: 0x13
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
+    i2c_words:
+      address: 0x0F
+      bitposition: 8
+      bitwidth: 3
+      description: ''
+      readwrite: rw
+      value: 0
     response0:
       address: 0x48
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: r
       value: 0
```

### Comparing `naluconfigs-10.8.0/src/naluconfigs/data/registers/aodsoc_asoc.yml` & `naluconfigs-11.0.0/src/naluconfigs/data/registers/oleas_box2.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,664 +1,743 @@
-model: aodsoc_asoc
+model: aodsv1
 features:
   adc2mv: false
   dac_sweep: false
-  ext_dac: true
+  ext_dac: false
   pedestals: true
   threshold_scan: true
   tia_dac: false
   timing_calibration: false
-  naludaq_rs: true
+  naludaq_rs: false
 params:
-  chanmask: 0x300
-  channels: 8
-  chanshift: 8
-  # clock_file: '' # AODSoC boards have fixed clocks
+  chanmask: 1536
+  channels: 4
+  chanshift: 9
+  clock_file: AODS_300GCC.txt  #  AODS_debugpulse_240MGCC_10Mref.txt
   connections:
     - serial
     - d2xx
-  si5341_address: 0xEE
-  timing_hack: true
+  si5341_address: 0xE8
   default_baud:
-    115200: 868
-  default_baudrate: 115200
-  default_clock: 100000000.0
-  default_divider: 868
-  default_isel:
-    0: 2610
-    1: 2627
-  default_trigger_value: 1500
+    111111: 53
+  default_baudrate: 111111
+  default_clock: 200000000.0
+  default_divider: 53
+  default_trigger_value: 2000
   threshold_scan:
     min_vref: 0
     max_vref: 2500
     start: 500
     stop: 3500
     stepsize: 5
     units: counts
   expected_scalmon: 2500
   ext_dac:
-    chip: dac7578
     max_mv: 2500
-    max_counts: 4095
+    max_counts: 65535
     channels:
-      0..7: 2048
-    address_mapping:
-      0..7: 0x48
-    channel_mapping:
-      0: 7
-      1: 5
-      2: 3
-      3: 1
-      4: 0
-      5: 2
-      6: 4
-      7: 6
+      0: 32768
+      1: 34800
+      2: 31500
+      3: 32768
   headers: 3
-  numregs: 64
-  pedestals_blocks: 16
+  numregs: 36
+  pedestals_blocks: 32
   peripherals:
-    vadjn_0:
-      chan: 3
-      addr: 0x4C
-    vadjn_1:
-      chan: 2
-      addr: 0x4C
-    ldo_voltage:
+    current:
+      chan: 0
+      addr: 0xD0
+      bits: 16
+      gain: 8
+    vadjn:
+      chan: 0
+      addr: 0xD8
+      bits: 16
+      gain: 1
+    vadjp:
       chan: 1
-      addr: 0x4C
-    chip_voltage:
-      chan: 2
-      addr: 0x4C
-    current_resistor: 0.010
+      addr: 0xD8
+      bits: 16
+      gain: 1
   possible_bauds:
-    115200: 868
-    1000000: 100
-    2000000: 50
-    3000000: 33
+    111111: 53
+    1500000: 3
   resolution: 12
   samples: 64
-  samplingrate: 3.2
-  stop_word: "cafe"
+  samplingrate: 1.0
+  stop_word: !!binary |
+    +s4=
   wait: AE000001
   wbias: 848
-  windmask: 0x0FF
-  windows: 254
+  windmask: 510
+  windows: 40
 registers:
   analog_registers:
     cmpbias:
       address: 0x14
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 1000
     cmpbias2:
       address: 0x16
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 737
     dbbias:
       address: 0x18
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 1300
     isel:
       address: 0x1B
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
-      value: 2950
+      readwrite: w
+      value: 2300  # 2680
     itbias:
       address: 0x12
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 2048
     ittbias:
       address: 0x11
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 2048
     mont_on:
       address: 0x17
       bitposition: 3
       bitwidth: 1
       description: ''
-      readwrite: rw
-      value: true
+      readwrite: w
+      value: 0
     mont_select:
       address: 0x17
       bitposition: 0
       bitwidth: 3
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 0
     offset_00:
       address: 0x01
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 0
     offset_01:
       address: 0x04
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 0
     offset_02:
       address: 0x07
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 0
     offset_03:
       address: 0x0A
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 0
     pubias:
       address: 0x15
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 3112
     qbias:
       address: 0x1C
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 2048
     qbuff:
       address: 0x1D
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 2048
     sbbias:
       address: 0x19
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 1300
+    sel_0:
+      address: 0x80
+      bitposition: 10
+      bitwidth: 1
+      description: ''  # mgiht need to describe this one
+      readwrite: w
+      value: 1
+    sel_1:
+      address: 0x80
+      bitposition: 11
+      bitwidth: 1
+      description: ''  # mgiht need to describe this one
+      readwrite: w
+      value: 1
+    sel_2:
+      address: 0x80
+      bitposition: 0
+      bitwidth: 1
+      description: ''  # mgiht need to describe this one
+      readwrite: w
+      value: 0
+    sel_3:
+      address: 0x80
+      bitposition: 1
+      bitwidth: 1
+      description: ''  # mgiht need to describe this one
+      readwrite: w
+      value: 1
+    sel_4:
+      address: 0x80
+      bitposition: 2
+      bitwidth: 1
+      description: ''  # mgiht need to describe this one
+      readwrite: w
+      value: 1
     scvbias0:
-      address: 0x0C
+      address: 0x0D
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
-      value: 800
+      readwrite: w
+      value: 2048 #800  # 1800?
     scvbias1:
-      address: 0x0D
+      address: 0x0E
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
-      value: 800
+      readwrite: w
+      value: 2048 #800  # 1800?
     scvbias2:
-      address: 0x0E
+      address: 0x0F
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
-      value: 800
+      readwrite: w
+      value: 2048 #800  # 1800?
     scvbias3:
-      address: 0x0F
+      address: 0x10
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
-      value: 800
+      readwrite: w
+      value: 2048 #800  # 1800?
     sgn:
       address: 0x17
       bitposition: 6
       bitwidth: 1
       description: ''
-      readwrite: rw
-      value: false
+      readwrite: w
+      value: 0
     sspin_le:
       address: 0x2B
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 100
     sspin_te:
       address: 0x2C
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 25
     sstin_ext:
       address: 0x17
       bitposition: 4
       bitwidth: 1
       description: ''
-      readwrite: rw
-      value: true
+      readwrite: w
+      value: 0
     sstoutfb:
       address: 0x22
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
-      value: 119
+      readwrite: w
+      value: 126
     tbbias:
-      address: 0x10
+      address: 0x0C
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 1000
     trigger_threshold_00:
       address: 0x00
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 1800
     trigger_threshold_01:
       address: 0x03
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 1800
     trigger_threshold_02:
       address: 0x06
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 1800
     trigger_threshold_03:
       address: 0x09
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 1800
     tsel:
       address: 0x17
       bitposition: 5
       bitwidth: 1
       description: ''
-      readwrite: rw
-      value: true
+      readwrite: w
+      value: 0
+    tsbias_1:
+      address: 0x8A
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: w
+      value: 0
+    tsbias_2:
+      address: 0x8B
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: w
+      value: 0
     vadjn:
       address: 0x1E
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 1550
     vadjp:
       address: 0x20
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 2200
     vanbuff:
       address: 0x1F
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 0
     vapbuff:
       address: 0x21
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 2816
+    vbias0_0:
+      address: 0x81
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: w
+      value: 2801
+    vbias0_1:
+      address: 0x82
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: w
+      value: 2604
+    vbias1_0:
+      address: 0x83
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: w
+      value: 2801
+    vbias1_1:
+      address: 0x84
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: w
+      value: 2604
+    vbias2_0:
+      address: 0x85
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: w
+      value: 2801
+    vbias2_1:
+      address: 0x86
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: w
+      value: 2604
+    vbias3_0:
+      address: 0x87
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: w
+      value: 2801
+    vbias3_1:
+      address: 0x88
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: w
+      value: 2604
     vdischarge:
       address: 0x1A
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 0
     wbbias:
       address: 0x13
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 2048
     wbias_00:
       address: 0x02
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 700
     wbias_01:
       address: 0x05
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 700
     wbias_02:
       address: 0x08
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 700
     wbias_03:
       address: 0x0B
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 700
     wr_strb1_le:
       address: 0x23
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 64
     wr_strb1_te:
       address: 0x24
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
-      value: 83
+      readwrite: w
+      value: 83  #67 ??
     wr_strb2_le:
       address: 0x25
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 0
     wr_strb2_te:
       address: 0x26
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
-      value: 29
+      readwrite: w
+      value: 29  # 3??
     wr_sync1_le:
       address: 0x27
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 10
     wr_sync1_te:
       address: 0x28
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 50
     wr_sync2_le:
       address: 0x29
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 80
     wr_sync2_te:
       address: 0x2A
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 110
   control_registers:
-    1v2_en:
-      address: 0x17
-      bitposition: 1
-      bitwidth: 1
-      description: ''
+    trig_mux:
+      address: 0x22
+      bitposition: 5
+      bitwidth: 4
+      description: 'evttrig driver'
       readwrite: rw
-      value: true
+      value: 3
+    fpga_misc_t:
+      address: 0x22
+      bitposition: 0
+      bitwidth: 4
+      description: 'fpga misc output disable'
+      readwrite: rw
+      value: 15
     2v5_en:
-      address: 0x17
+      address: 0x16
       bitposition: 0
       bitwidth: 1
       description: ''
       readwrite: rw
       value: true
-    3v3_i2c_en:
-      address: 0x17
-      bitposition: 2
+    2v5_pll_en:
+      address: 0x16
+      bitposition: 1
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: true
-    8b10b_en:
-      address: 0x19
-      bitposition: 12
-      bitwidth: 1
+      value: false
+    addr:
+      address: 0x15
+      bitposition: 0
+      bitwidth: 9
       description: ''
       readwrite: rw
       value: 0
-    amp_pwrdn_out:
-      address: 0x1A
+    addr_user:
+      address: 0x15
+      bitposition: 15
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: false
+    brightness_blue:
+      address: 0x0A
       bitposition: 0
       bitwidth: 8
-      description: 'Onboard amplifiers active high means amp off'
+      description: ''
       readwrite: rw
       value: 0
-    addr:
-      address: 0x16
+    brightness_red:
+      address: 0x0B
       bitposition: 0
-      bitwidth: 9
+      bitwidth: 8
       description: ''
       readwrite: rw
       value: 0
-    addr_user:
-      address: 0x16
-      bitposition: 15
-      bitwidth: 1
+    brightness_white:
+      address: 0x0A
+      bitposition: 8
+      bitwidth: 8
       description: ''
       readwrite: rw
-      value: false
+      value: 0
     chansel:
       address: 0x06
       bitposition: 12
       bitwidth: 4
       description: ''
       readwrite: rw
       value: 15
-    clk1v8_en:
-      address: 0x17
-      bitposition: 4
+    clk_1v8_nshutdown:
+      address: 0x16
+      bitposition: 2
       bitwidth: 1
       description: ''
       readwrite: rw
       value: true
-    clk2v5_en:
-      address: 0x17
-      bitposition: 3
+    clk_2v5_en:
+      address: 0x16
+      bitposition: 6
       bitwidth: 1
       description: ''
       readwrite: rw
       value: true
-    clk_fdec:
-      address: 0x17
-      bitposition: 9
+    clk_i2c_sel:
+      address: 0x16
+      bitposition: 5
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: false
-    clk_finc:
-      address: 0x17
-      bitposition: 8
+      value: true
+    clk_noe:
+      address: 0x16
+      bitposition: 4
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
-    clk_i2c_sel:
-      address: 0x17
-      bitposition: 5
+    clk_nrst:
+      address: 0x16
+      bitposition: 3
       bitwidth: 1
       description: ''
       readwrite: rw
       value: true
-    clk_oeb:
-      address: 0x17
-      bitposition: 6
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    clk_reset:
-      address: 0x17
+    clk_nsync:
+      address: 0x16
       bitposition: 7
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
-    clk_sync:
-      address: 0x17
+    dac_nrst:
+      address: 0x16
       bitposition: 10
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: false
+      value: 1
     data:
       address: 0x14
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
     data_user:
       address: 0x14
       bitposition: 15
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
-    debug_data:
-      address: 0x15
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: rw
-      value: 0
-    debug_data_user:
-      address: 0x15
-      bitposition: 15
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
     digrst:
       address: 0x16
       bitposition: 9
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    digser_rst:
-      address: 0x19
-      bitposition: 13
+    ext_en:
+      address: 0x0B
+      bitposition: 9
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
+      value: false
     exttrig:
       address: 0x04
       bitposition: 10
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
-    gccclr:
-      address: 0x04
-      bitposition: 4
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    idac_ldac:
-      address: 0x1B
+    fake:
+      address: 0x06
       bitposition: 0
       bitwidth: 1
-      description: 'pin on AD7578'
+      description: ''
       readwrite: rw
       value: 0
-    idac_nclr:
-      address: 0x1B
-      bitposition: 1
+    gccclr:
+      address: 0x04
+      bitposition: 3
       bitwidth: 1
-      description: 'pin on AD7578'
+      description: ''
       readwrite: rw
-      value: 1
-    fifo_unload_or_event_en:
-      address: 0x1F
-      bitposition: 0
+      value: false
+    i2c_switch:
+      address: 0x16
+      bitposition: 8
       bitwidth: 1
-      description: 'Once data is loaded into the FIFO it will not be sent out to the UART until the end of the current event. Use this mode for capturing sampled data events. '
+      description: ''
       readwrite: rw
       value: 0
     identifier:
       address: 0x00
       bitposition: 0
       bitwidth: 16
       description: ''
+      readwrite: r
+      value: 41173
+    in_sel:
+      address: 0x0B
+      bitposition: 12
+      bitwidth: 1
+      description: ''
       readwrite: rw
-      value: 309
+      value: true
     iomode0:
       address: 0x04
-      bitposition: 0
+      bitposition: 7
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: true
+      value: 1
     iomode1:
       address: 0x04
-      bitposition: 6
+      bitposition: 8
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: false
-    leds:
-      address: 0x18
-      bitposition: 0
-      bitwidth: 16
-      description: ''
-      readwrite: rw
       value: 0
     loadwait:
       address: 0x07
       bitposition: 8
       bitwidth: 4
       description: ''
       readwrite: rw
       value: 15
     nramp:
       address: 0x04
-      bitposition: 5
+      bitposition: 4
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
     nrw:
       address: 0x04
       bitposition: 11
@@ -669,49 +748,105 @@
     numwinds:
       address: 0x08
       bitposition: 0
       bitwidth: 8
       description: ''
       readwrite: rw
       value: 1
+    out_sel:
+      address: 0x0B
+      bitposition: 11
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: false
     pclk:
       address: 0x04
-      bitposition: 2
+      bitposition: 1
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
     pclkwidth:
       address: 0x07
       bitposition: 12
       bitwidth: 4
       description: ''
       readwrite: rw
       value: 15
-    ramplen:
-      address: 0x06
-      bitposition: 0
-      bitwidth: 12
+    rden:
+      address: 0x04
+      bitposition: 6
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 2000
+      value: false
     regclr:
       address: 0x04
-      bitposition: 1
+      bitposition: 0
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
     runevs:
       address: 0x05
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
       value: 1
+    rx_data0:
+      address: 0x1A
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: rw
+      value: 0
+    rx_data1:
+      address: 0x1B
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: rw
+      value: 0
+    rx_data2:
+      address: 0x1C
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: rw
+      value: 0
+    rx_data3:
+      address: 0x1D
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: rw
+      value: 0
+    rx_data4:
+      address: 0x1E
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: rw
+      value: 0
+    rx_data5:
+      address: 0x1F
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: rw
+      value: 0
+    rx_data6:
+      address: 0x20
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: rw
+      value: 0
     rx_en:
       address: 0x19
       bitposition: 0
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
@@ -741,276 +876,185 @@
       bitposition: 12
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
     selany:
       address: 0x04
-      bitposition: 3
+      bitposition: 2
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
-    slow_sysclk:
-      address: 0x19
-      bitposition: 10
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: 0
     stopacq:
       address: 0x04
       bitposition: 13
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
+    switch_nen:
+      address: 0x0B
+      bitposition: 13
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: true
     syncloc:
-      address: 0x09
+      address: 0x0E
       bitposition: 0
       bitwidth: 8
       description: ''
       readwrite: rw
       value: 0
-    sysclk:
-      address: 0x04
-      bitposition: 8
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
     sysrst:
       address: 0x04
-      bitposition: 9
+      bitposition: 14
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: true
-    tx_en:
-      address: 0x19
-      bitposition: 11
+      value: false
+    trig_sel:
+      address: 0x0B
+      bitposition: 10
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
+      value: false
     windsel:
       address: 0x07
       bitposition: 0
       bitwidth: 8
       description: ''
       readwrite: rw
       value: 0
-    wrstrboff:
+    wren:
       address: 0x04
-      bitposition: 7
+      bitposition: 5
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
-    rxout_pol:
-      address: 0x22
-      bitposition: 0
-      bitwidth: 16
-      description: ''
-      readwrite: rw
-      value: 6400
-    txin_pol:
-      address: 0x23
-      bitposition: 0
-      bitwidth: 16
-      description: ''
-      readwrite: rw
-      value: 4412
-    ard_header:
-      address: 0x21
-      bitposition: 0
-      bitwidth: 1
-      description: 'Enable AARDVARC debug header.'
-      readwrite: rw
-      value: 1
-    ard_rx_en:
-      address: 0x1D
-      bitposition: 0
-      bitwidth: 16
-      description: 'TR-BHM ASIC Rx Enable register 29dec. Bit 0 and 1 enable transmitting data to ASICs. Need to set these bits to send data to the ASICs'
-      readwrite: rw
-      value: 3
-    ard_tx_en:
-      address: 0x1E
-      bitposition: 0
-      bitwidth: 16
-      description: 'TR-BHM ASIC Tx Enable register 30dec. Bit 0 and 1 enable receiving data from ASICs. Need to set these bits to get data back from the ASICs'
-      readwrite: rw
-      value: 3
-    ard0_clk_sel:
-      address: 0x24
+  digital_registers:
+    chipid:
+      address: 0x89
       bitposition: 0
-      bitwidth: 2
+      bitwidth: 12
       description: ''
       readwrite: rw
-      value: 0
-    ard1_clk_sel:
-      address: 0x25
+      value: 2730
+    convertresetwait:
+      address: 0x84
       bitposition: 0
-      bitwidth: 2
+      bitwidth: 8
       description: ''
       readwrite: rw
       value: 1
-    motor_trig_en:
-      address: 0x27
-      bitposition: 0
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: 0
-    motor_trig_evts:
-      address: 0x26
+    enabletestpatt:
+      address: 0x88
       bitposition: 0
-      bitwidth: 16
-      description: ''
-      readwrite: rw
-      value: 1
-    oleas_en_trig:
-      address: 0x0A
-      bitposition: 10
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: 0
-    oleas_pol_a:
-      address: 0x0A
-      bitposition: 11
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: 0
-    oleas_pol_b:
-      address: 0x0A
-      bitposition: 12
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: 0
-    oleas_en_a:
-      address: 0x0A
-      bitposition: 13
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    oleas_en_b:
-      address: 0x0A
-      bitposition: 14
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: 0
-    oleas_loop:
-      address: 0x0A
-      bitposition: 0
-      bitwidth: 5
-      description: ''
-      readwrite: rw
-      value: 15
-    oleas_length_a:
-      address: 0x0B
+    excludechannelmask:
+      address: 0x96
       bitposition: 0
-      bitwidth: 16
+      bitwidth: 4
       description: ''
       readwrite: rw
       value: 0
-    oleas_length_b:
-      address: 0x0D
+    fineoffset:
+      address: 0x8D
       bitposition: 0
-      bitwidth: 16
+      bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
-    oleas_delay_a:
-      address: 0x0C
+    loadwait:
+      address: 0x8B
       bitposition: 0
-      bitwidth: 16
+      bitwidth: 7
       description: ''
       readwrite: rw
       value: 0
-    oleas_delay_b:
-      address: 0x0E
+    masktrig:
+      address: 0x90
       bitposition: 0
-      bitwidth: 16
+      bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
-    testmode:
-      address: 0x20
+    max0:
+      address: 0xA1
       bitposition: 0
-      bitwidth: 1
+      bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
-  digital_registers:
-    chipid:
-      address: 0x89
+    max1:
+      address: 0xA2
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
-      value: 2730
-    convertresetwait:
-      address: 0x84
+      value: 0
+    max2:
+      address: 0xA3
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
-      value: 1
-    enabletestpatt:
-      address: 0x88
+      value: 0
+    max3:
+      address: 0xA4
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
-    excludechannelmask:
-      address: 0x96
+    min0:
+      address: 0x9D
       bitposition: 0
-      bitwidth: 4
+      bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
-    fineoffset:
-      address: 0x8D
+    min1:
+      address: 0x9E
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
-    loadwait:
-      address: 0x8B
+    min2:
+      address: 0x9F
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
-    masktrig:
-      address: 0x90
+    min3:
+      address: 0xA0
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
     pclkwidth:
       address: 0x8C
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 7
       description: ''
       readwrite: rw
       value: 0
     pll:
       address: 0x93
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 6
       description: ''
       readwrite: rw
       value: 0
     pulselength10:
       address: 0x99
       bitposition: 0
       bitwidth: 12
@@ -1023,36 +1067,36 @@
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
     readoutlookback:
       address: 0x85
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 8
       description: ''
       readwrite: rw
       value: 18
     readoutoffset:
       address: 0x87
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 8
       description: ''
       readwrite: rw
       value: 122
     readoutwindows:
       address: 0x86
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 8
       description: ''
       readwrite: rw
       value: 10
     regclr:
       address: 0x8A
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
     roilength10:
       address: 0x9B
       bitposition: 0
       bitwidth: 12
@@ -1067,64 +1111,64 @@
       readwrite: rw
       value: 0
     scal0:
       address: 0x00
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 0
     scal1:
       address: 0x01
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 0
     scal2:
       address: 0x02
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 0
     scal3:
       address: 0x03
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 0
     scalhigh:
       address: 0x40
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 0
     scalmon:
       address: 0x08
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 0
     speed:
       address: 0x92
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 10
       description: ''
       readwrite: rw
       value: 0
     testpatin:
       address: 0x0A
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 3
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 0
     trigfinedelay10:
       address: 0x97
       bitposition: 0
       bitwidth: 8
       description: ''
       readwrite: rw
@@ -1135,32 +1179,32 @@
       bitwidth: 8
       description: ''
       readwrite: rw
       value: 0
     txspeed:
       address: 0x94
       bitposition: 0
-      bitwidth: 2
+      bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
     waitaddr:
       address: 0x8F
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 3
       description: ''
       readwrite: rw
       value: 0
     waitread:
       address: 0x8E
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 3
       description: ''
       readwrite: rw
-      value: 0
+      value: 1
     wlc_on:
       address: 0x95
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
@@ -1180,48 +1224,41 @@
       value: 0
     wraddrstop:
       address: 0x81
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
-      value: 126
+      value: 19
     writeaftertrig:
       address: 0x83
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 5
     writedelay:
       address: 0x91
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 3
       description: ''
       readwrite: rw
       value: 0
   i2c_registers:
     i2c_en:
-      address: 0x0F
+      address: 0x09
       bitposition: 14
       bitwidth: 1
       description: ''
       readwrite: rw
       value: true
-    # i2c_send:
-    #   address: 0x0F
-    #   bitposition: 15
-    #   bitwidth: 1
-    #   description: ''
-    #   readwrite: rw
-    #   value: 0
-    i2c_words:
+    i2c_send:
       address: 0x0F
-      bitposition: 8
-      bitwidth: 3
+      bitposition: 15
+      bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
     i2c_addr:
       address: 0x0F
       bitposition: 0
       bitwidth: 8
@@ -1252,35 +1289,42 @@
     i2c_data3:
       address: 0x13
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
+    i2c_words:
+      address: 0x0F
+      bitposition: 8
+      bitwidth: 3
+      description: ''
+      readwrite: rw
+      value: 0
     response0:
-      address: 0x48
+      address: 0x2C
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: r
       value: 0
     response1:
-      address: 0x49
+      address: 0x2D
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: r
       value: 0
     response2:
-      address: 0x4A
+      address: 0x2E
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: r
       value: 0
     response3:
-      address: 0x4B
+      address: 0x2F
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: r
       value: 0
```

### Comparing `naluconfigs-10.8.0/src/naluconfigs/data/registers/aodsv1.yml` & `naluconfigs-11.0.0/src/naluconfigs/data/registers/asoc.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,59 +1,43 @@
-model: aodsv1
+model: asoc
 features:
   adc2mv: false
-  dac_sweep: true
-  ext_dac: true
+  dac_sweep: false
   pedestals: true
   threshold_scan: true
   tia_dac: false
   timing_calibration: false
-  naludaq_rs: true
+  naludaq_rs: false
 params:
-  chanmask: 1536
+  chanmask: 6144
   channels: 4
-  chanshift: 9
-  clock_file: AODS_300GCC.txt  #  AODS_debugpulse_240MGCC_10Mref.txt
+  chanshift: 11
+  clock_file: Si5341-RevD-Lambchop-Registers_compSysclk.txt
   connections:
     - serial
     - d2xx
   si5341_address: 0xE8
   default_baud:
-    111111: 53
-  default_baudrate: 111111
-  default_clock: 200000000.0
+    115200: 53
+  default_baudrate: 115200
+  default_clock: 100000000.0
   default_divider: 53
-  default_trigger_value: 2000
-  threshold_scan:
-    min_vref: 0
-    max_vref: 2500
-    start: 500
-    stop: 3500
-    stepsize: 5
-    units: counts
   expected_scalmon: 2500
   ext_dac:
-    chip: ad5671
     max_mv: 2500
     max_counts: 4095
     channels:
-      0: 2048
-      1: 2175
-      2: 1968
-      3: 2048
-    address_mapping:
-      0..3: 0xC
-    channel_mapping:
-      0: 1
-      1: 0
-      2: 5
-      3: 4
-  headers: 3
-  numregs: 36
-  pedestals_blocks: 32
+      0: 2000
+      1: 2000
+      2: 2000
+      3: 2000
+  headers: 4
+  last_window_fix_amount: 47
+  numregs: 32
+  pedestals_blocks: 64
   peripherals:
     current:
       chan: 0
       addr: 0xD0
       bits: 16
       gain: 8
     vadjn:
@@ -62,40 +46,26 @@
       bits: 16
       gain: 1
     vadjp:
       chan: 1
       addr: 0xD8
       bits: 16
       gain: 1
-    eeprom:
-      addr: 0x50 # 7-bit
-      capacity: 0x20000 # bytes
-      page_size: 256 # bytes
-      segments:
-        analog_registers:
-          begin: 0
-          length: 300
-        digital_registers:
-          begin: 300
-          length: 330
-        control_registers:
-          begin: 630
-          length: 70
   possible_bauds:
-    111111: 53
-    1500000: 3
+    115200: 53
+    3000000: 1
   resolution: 12
   samples: 64
-  samplingrate: 1.0
+  samplingrate: 3.2
   stop_word: !!binary |
     +s4=
   wait: AE000001
   wbias: 848
   windmask: 510
-  windows: 254
+  windows: 256
 registers:
   analog_registers:
     cmpbias:
       address: 0x14
       bitposition: 0
       bitwidth: 12
       description: ''
@@ -117,15 +87,15 @@
       value: 1300
     isel:
       address: 0x1B
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2300  # 2680
+      value: 2700
     itbias:
       address: 0x12
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
       value: 2048
@@ -138,15 +108,15 @@
       value: 2048
     mont_on:
       address: 0x17
       bitposition: 3
       bitwidth: 1
       description: ''
       readwrite: w
-      value: 0
+      value: true
     mont_select:
       address: 0x17
       bitposition: 0
       bitwidth: 3
       description: ''
       readwrite: w
       value: 0
@@ -187,267 +157,162 @@
       value: 3112
     qbias:
       address: 0x1C
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2048
+      value: 800
     qbuff:
       address: 0x1D
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
       value: 2048
     sbbias:
       address: 0x19
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
       value: 1300
-    sel_0:
-      address: 0x80
-      bitposition: 10
-      bitwidth: 1
-      description: ''  # mgiht need to describe this one
-      readwrite: w
-      value: 0
-    sel_1:
-      address: 0x80
-      bitposition: 11
-      bitwidth: 1
-      description: ''  # mgiht need to describe this one
-      readwrite: w
-      value: 0
-    sel_2:
-      address: 0x80
-      bitposition: 0
-      bitwidth: 1
-      description: ''  # mgiht need to describe this one
-      readwrite: w
-      value: 0
-    sel_3:
-      address: 0x80
-      bitposition: 1
-      bitwidth: 1
-      description: ''  # mgiht need to describe this one
-      readwrite: w
-      value: 0
-    sel_4:
-      address: 0x80
-      bitposition: 2
-      bitwidth: 1
-      description: ''  # mgiht need to describe this one
-      readwrite: w
-      value: 0
     scvbias0:
       address: 0x0D
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2048 #800  # 1800?
+      value: 2048
     scvbias1:
       address: 0x0E
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2048 #800  # 1800?
+      value: 2048
     scvbias2:
       address: 0x0F
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2048 #800  # 1800?
+      value: 2048
     scvbias3:
       address: 0x10
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2048 #800  # 1800?
+      value: 2048
     sgn:
       address: 0x17
       bitposition: 6
       bitwidth: 1
       description: ''
       readwrite: w
-      value: 0
+      value: false
     sspin_le:
       address: 0x2B
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 100
+      value: 95
     sspin_te:
       address: 0x2C
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 25
+      value: 5
     sstin_ext:
       address: 0x17
       bitposition: 4
       bitwidth: 1
       description: ''
       readwrite: w
-      value: 0
+      value: false
     sstoutfb:
       address: 0x22
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 126
+      value: 114
     tbbias:
       address: 0x0C
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
       value: 1000
     trigger_threshold_00:
       address: 0x00
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 1800
+      value: 0
     trigger_threshold_01:
       address: 0x03
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 1800
+      value: 0
     trigger_threshold_02:
       address: 0x06
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 1800
+      value: 0
     trigger_threshold_03:
       address: 0x09
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 1800
+      value: 0
     tsel:
       address: 0x17
       bitposition: 5
       bitwidth: 1
       description: ''
       readwrite: w
-      value: 0
-    tsbias_1:
-      address: 0x8A
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 0
-    tsbias_2:
-      address: 0x8B
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 0
+      value: true
     vadjn:
       address: 0x1E
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 1550
+      value: 1800
     vadjp:
       address: 0x20
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2200
+      value: 2405
     vanbuff:
       address: 0x1F
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
       value: 0
     vapbuff:
       address: 0x21
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
       value: 2816
-    vbias0_0:
-      address: 0x81
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2801
-    vbias0_1:
-      address: 0x82
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2604
-    vbias1_0:
-      address: 0x83
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2801
-    vbias1_1:
-      address: 0x84
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2604
-    vbias2_0:
-      address: 0x85
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2801
-    vbias2_1:
-      address: 0x86
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2604
-    vbias3_0:
-      address: 0x87
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2801
-    vbias3_1:
-      address: 0x88
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2604
     vdischarge:
       address: 0x1A
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
       value: 0
@@ -460,306 +325,327 @@
       value: 2048
     wbias_00:
       address: 0x02
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 700
+      value: 350
     wbias_01:
       address: 0x05
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 700
+      value: 350
     wbias_02:
       address: 0x08
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 700
+      value: 350
     wbias_03:
       address: 0x0B
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 700
+      value: 350
     wr_strb1_le:
       address: 0x23
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 64
+      value: 65
     wr_strb1_te:
       address: 0x24
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 83  #67 ??
+      value: 90
     wr_strb2_le:
       address: 0x25
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
       value: 0
     wr_strb2_te:
       address: 0x26
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 29  # 3??
+      value: 25
     wr_sync1_le:
       address: 0x27
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
       value: 10
     wr_sync1_te:
       address: 0x28
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 50
+      value: 15
     wr_sync2_le:
       address: 0x29
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
       value: 80
     wr_sync2_te:
       address: 0x2A
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 110
+      value: 85
   control_registers:
-    trig_mux:
-      address: 0x22
-      bitposition: 5
-      bitwidth: 4
-      description: 'evttrig driver'
-      readwrite: rw
-      value: 3
-    fpga_misc_t:
-      address: 0x22
-      bitposition: 0
-      bitwidth: 4
-      description: 'fpga misc output disable'
-      readwrite: rw
-      value: 15
-    2v5_en:
-      address: 0x16
-      bitposition: 0
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: true
-    2v5_pll_en:
+    3v3_en_main:
       address: 0x16
-      bitposition: 1
+      bitposition: 6
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: false
+      value: 1
     addr:
       address: 0x15
       bitposition: 0
       bitwidth: 9
       description: ''
       readwrite: rw
       value: 0
     addr_user:
       address: 0x15
       bitposition: 15
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
-    brightness_blue:
-      address: 0x0A
-      bitposition: 0
-      bitwidth: 8
-      description: ''
-      readwrite: rw
-      value: 0
-    brightness_red:
-      address: 0x0B
-      bitposition: 0
-      bitwidth: 8
-      description: ''
-      readwrite: rw
-      value: 0
-    brightness_white:
-      address: 0x0A
-      bitposition: 8
-      bitwidth: 8
-      description: ''
-      readwrite: rw
-      value: 0
     chansel:
       address: 0x06
       bitposition: 12
       bitwidth: 4
       description: ''
       readwrite: rw
       value: 15
-    clk_1v8_nshutdown:
+    clk_cal_en:
       address: 0x16
-      bitposition: 2
+      bitposition: 10
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: true
-    clk_2v5_en:
+      value: 0
+    clk_oe:
       address: 0x16
-      bitposition: 6
+      bitposition: 4
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: true
-    clk_i2c_sel:
+      value: 0
+    clk_rst:
       address: 0x16
       bitposition: 5
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: true
-    clk_noe:
-      address: 0x16
-      bitposition: 4
-      bitwidth: 1
+      value: 0
+    coin_chanmask:
+      address: 0x17
+      bitposition: 12
+      bitwidth: 4
       description: ''
       readwrite: rw
-      value: false
-    clk_nrst:
-      address: 0x16
-      bitposition: 3
-      bitwidth: 1
+      value: 0
+    coin_length:
+      address: 0x17
+      bitposition: 0
+      bitwidth: 6
       description: ''
       readwrite: rw
-      value: true
-    clk_nsync:
+      value: 0
+    coin_or_ext:
       address: 0x16
-      bitposition: 7
+      bitposition: 12
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: false
-    dac_nrst:
-      address: 0x16
-      bitposition: 10
+      value: 0
+    coin_pol:
+      address: 0x18
+      bitposition: 0
+      bitwidth: 4
+      description: ''
+      readwrite: rw
+      value: 0
+    coin_triglen:
+      address: 0x17
+      bitposition: 6
+      bitwidth: 6
+      description: ''
+      readwrite: rw
+      value: 0
+    dac_a:
+      address: 0x09
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: rw
+      value: 2000
+    dac_b:
+      address: 0x0A
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: rw
+      value: 2000
+    dac_c:
+      address: 0x0B
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: rw
+      value: 2000
+    dac_d:
+      address: 0x0C
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: rw
+      value: 2000
+    dac_send:
+      address: 0x09
+      bitposition: 15
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 1
+      value: false
     data:
       address: 0x14
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
     data_user:
       address: 0x14
       bitposition: 15
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
-    digrst:
-      address: 0x16
-      bitposition: 9
+    debug:
+      address: 0x04
+      bitposition: 0
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
-    ext_en:
-      address: 0x0B
+      value: false
+    digrst:
+      address: 0x16
       bitposition: 9
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: true
+      value: 0
     exttrig:
       address: 0x04
       bitposition: 10
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
     fake:
-      address: 0x06
-      bitposition: 0
+      address: 0x08
+      bitposition: 8
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    gccclr:
-      address: 0x04
-      bitposition: 3
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    i2c_switch:
+    fpgarst:
       address: 0x16
       bitposition: 8
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    identifier:
-      address: 0x00
-      bitposition: 0
-      bitwidth: 16
+    gccclr:
+      address: 0x04
+      bitposition: 4
+      bitwidth: 1
       description: ''
-      readwrite: r
-      value: 41173
-    in_sel:
-      address: 0x0B
-      bitposition: 12
+      readwrite: rw
+      value: false
+    i2c_en:
+      address: 0x09
+      bitposition: 14
       bitwidth: 1
       description: ''
       readwrite: rw
       value: true
-    iomode0:
-      address: 0x04
-      bitposition: 7
+    i2c_switch:
+      address: 0x16
+      bitposition: 3
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 1
-    iomode1:
-      address: 0x04
-      bitposition: 8
+      value: false
+    i2c_upperdeck:
+      address: 0x16
+      bitposition: 11
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
     loadwait:
       address: 0x07
       bitposition: 8
       bitwidth: 4
       description: ''
       readwrite: rw
       value: 15
+    ls_oe:
+      address: 0x16
+      bitposition: 7
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: 1
+    muxfast:
+      address: 0x16
+      bitposition: 0
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: 0
+    muxfinal:
+      address: 0x16
+      bitposition: 2
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: 0
+    muxslow:
+      address: 0x16
+      bitposition: 1
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: 1
     nramp:
       address: 0x04
-      bitposition: 4
+      bitposition: 5
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
     nrw:
       address: 0x04
       bitposition: 11
@@ -769,193 +655,116 @@
       value: false
     numwinds:
       address: 0x08
       bitposition: 0
       bitwidth: 8
       description: ''
       readwrite: rw
-      value: 1
-    out_sel:
-      address: 0x0B
-      bitposition: 11
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
+      value: 10
     pclk:
       address: 0x04
-      bitposition: 1
+      bitposition: 2
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
     pclkwidth:
       address: 0x07
       bitposition: 12
       bitwidth: 4
       description: ''
       readwrite: rw
       value: 15
+    ramp:
+      address: 0x06
+      bitposition: 0
+      bitwidth: 11
+      description: ''
+      readwrite: rw
+      value: 1500
     rden:
       address: 0x04
-      bitposition: 6
+      bitposition: 7
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
     regclr:
       address: 0x04
-      bitposition: 0
+      bitposition: 1
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
     runevs:
       address: 0x05
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
       value: 1
-    rx_data0:
-      address: 0x1A
-      bitposition: 0
-      bitwidth: 16
-      description: ''
-      readwrite: rw
-      value: 0
-    rx_data1:
-      address: 0x1B
-      bitposition: 0
-      bitwidth: 16
-      description: ''
-      readwrite: rw
-      value: 0
-    rx_data2:
-      address: 0x1C
-      bitposition: 0
-      bitwidth: 16
-      description: ''
-      readwrite: rw
-      value: 0
-    rx_data3:
-      address: 0x1D
-      bitposition: 0
-      bitwidth: 16
-      description: ''
-      readwrite: rw
-      value: 0
-    rx_data4:
-      address: 0x1E
-      bitposition: 0
-      bitwidth: 16
-      description: ''
-      readwrite: rw
-      value: 0
-    rx_data5:
-      address: 0x1F
-      bitposition: 0
-      bitwidth: 16
-      description: ''
-      readwrite: rw
-      value: 0
-    rx_data6:
-      address: 0x20
-      bitposition: 0
-      bitwidth: 16
-      description: ''
-      readwrite: rw
-      value: 0
-    rx_en:
-      address: 0x19
-      bitposition: 0
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: 0
-    rx_num_words:
-      address: 0x19
-      bitposition: 2
-      bitwidth: 6
-      description: ''
-      readwrite: rw
-      value: 0
-    rx_oneshot:
-      address: 0x19
-      bitposition: 1
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: 0
-    rx_speed:
-      address: 0x19
-      bitposition: 8
-      bitwidth: 2
-      description: ''
-      readwrite: rw
-      value: 0
     sel:
       address: 0x04
       bitposition: 12
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
     selany:
       address: 0x04
-      bitposition: 2
+      bitposition: 3
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
+    si570:
+      address: 0x0D
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: rw
+      value: 0
     stopacq:
       address: 0x04
       bitposition: 13
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
-    switch_nen:
-      address: 0x0B
-      bitposition: 13
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: true
     syncloc:
       address: 0x0E
       bitposition: 0
       bitwidth: 8
       description: ''
       readwrite: rw
       value: 0
-    sysrst:
+    sysclk:
       address: 0x04
-      bitposition: 14
+      bitposition: 8
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
-    trig_sel:
-      address: 0x0B
-      bitposition: 10
+    sysrst:
+      address: 0x04
+      bitposition: 9
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: false
+      value: true
     windsel:
       address: 0x07
       bitposition: 0
       bitwidth: 8
       description: ''
       readwrite: rw
       value: 0
     wren:
       address: 0x04
-      bitposition: 5
+      bitposition: 6
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
   digital_registers:
     chipid:
       address: 0x89
@@ -963,273 +772,70 @@
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 2730
     convertresetwait:
       address: 0x84
       bitposition: 0
-      bitwidth: 8
+      bitwidth: 12
       description: ''
       readwrite: rw
       value: 1
     enabletestpatt:
       address: 0x88
       bitposition: 0
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: 0
-    excludechannelmask:
-      address: 0x96
-      bitposition: 0
-      bitwidth: 4
-      description: ''
-      readwrite: rw
-      value: 0
-    fineoffset:
-      address: 0x8D
-      bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
     loadwait:
       address: 0x8B
       bitposition: 0
-      bitwidth: 7
-      description: ''
-      readwrite: rw
-      value: 0
-    masktrig:
-      address: 0x90
-      bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
-    max0:
-      address: 0xA1
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: rw
-      value: 0
-    max1:
-      address: 0xA2
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: rw
-      value: 0
-    max2:
-      address: 0xA3
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: rw
-      value: 0
-    max3:
-      address: 0xA4
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: rw
-      value: 0
-    min0:
-      address: 0x9D
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: rw
-      value: 0
-    min1:
-      address: 0x9E
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: rw
-      value: 0
-    min2:
-      address: 0x9F
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: rw
-      value: 0
-    min3:
-      address: 0xA0
+    miscreg:
+      address: 0x8D
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
     pclkwidth:
       address: 0x8C
       bitposition: 0
-      bitwidth: 7
-      description: ''
-      readwrite: rw
-      value: 0
-    pll:
-      address: 0x93
-      bitposition: 0
-      bitwidth: 6
-      description: ''
-      readwrite: rw
-      value: 0
-    pulselength10:
-      address: 0x99
-      bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
-    pulselength32:
-      address: 0x9A
+    readoutchannels:
+      address: 0x87
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
     readoutlookback:
       address: 0x85
       bitposition: 0
-      bitwidth: 8
+      bitwidth: 12
       description: ''
       readwrite: rw
       value: 18
-    readoutoffset:
-      address: 0x87
-      bitposition: 0
-      bitwidth: 8
-      description: ''
-      readwrite: rw
-      value: 122
     readoutwindows:
       address: 0x86
       bitposition: 0
-      bitwidth: 8
+      bitwidth: 12
       description: ''
       readwrite: rw
       value: 10
     regclr:
       address: 0x8A
       bitposition: 0
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: 0
-    roilength10:
-      address: 0x9B
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: rw
-      value: 0
-    roilength32:
-      address: 0x9C
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: rw
-      value: 0
-    scal0:
-      address: 0x00
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 0
-    scal1:
-      address: 0x01
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 0
-    scal2:
-      address: 0x02
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 0
-    scal3:
-      address: 0x03
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 0
-    scalhigh:
-      address: 0x40
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 0
-    scalmon:
-      address: 0x08
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 0
-    speed:
-      address: 0x92
-      bitposition: 0
-      bitwidth: 10
-      description: ''
-      readwrite: rw
-      value: 0
-    testpatin:
-      address: 0x0A
-      bitposition: 0
-      bitwidth: 3
-      description: ''
-      readwrite: w
-      value: 0
-    trigfinedelay10:
-      address: 0x97
-      bitposition: 0
-      bitwidth: 8
-      description: ''
-      readwrite: rw
-      value: 0
-    trigfinedelay32:
-      address: 0x98
-      bitposition: 0
-      bitwidth: 8
-      description: ''
-      readwrite: rw
-      value: 0
-    txspeed:
-      address: 0x94
-      bitposition: 0
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: 0
-    waitaddr:
-      address: 0x8F
-      bitposition: 0
-      bitwidth: 3
-      description: ''
-      readwrite: rw
-      value: 0
-    waitread:
-      address: 0x8E
-      bitposition: 0
-      bitwidth: 3
-      description: ''
-      readwrite: rw
-      value: 1
-    wlc_on:
-      address: 0x95
-      bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
     wraddrjunk:
       address: 0x82
       bitposition: 0
@@ -1254,29 +860,15 @@
     writeaftertrig:
       address: 0x83
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 5
-    writedelay:
-      address: 0x91
-      bitposition: 0
-      bitwidth: 3
-      description: ''
-      readwrite: rw
-      value: 0
   i2c_registers:
-    i2c_en:
-      address: 0x09
-      bitposition: 14
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: true
     i2c_send:
       address: 0x0F
       bitposition: 15
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
@@ -1319,34 +911,34 @@
       address: 0x13
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
     response0:
-      address: 0x2C
+      address: 0x28
       bitposition: 0
       bitwidth: 16
       description: ''
-      readwrite: r
+      readwrite: rw
       value: 0
     response1:
-      address: 0x2D
+      address: 0x29
       bitposition: 0
       bitwidth: 16
       description: ''
-      readwrite: r
+      readwrite: rw
       value: 0
     response2:
-      address: 0x2E
+      address: 0x2A
       bitposition: 0
       bitwidth: 16
       description: ''
-      readwrite: r
+      readwrite: rw
       value: 0
     response3:
-      address: 0x2F
+      address: 0x2B
       bitposition: 0
       bitwidth: 16
       description: ''
-      readwrite: r
+      readwrite: rw
       value: 0
```

### Comparing `naluconfigs-10.8.0/src/naluconfigs/data/registers/aodsv2_eval.yml` & `naluconfigs-11.0.0/src/naluconfigs/data/registers/hiper.yml`

 * *Files 19% similar despite different names*

```diff
@@ -1,60 +1,41 @@
-model: aodsv2_eval
+model: hiper
 features:
-  threshold_scan: true
-  timing_calibration: false
   adc2mv: false
   dac_sweep: false
+  ext_dac: false
   pedestals: true
+  threshold_scan: false
   tia_dac: false
-  ext_dac: true
-  naludaq_rs: true
+  timing_calibration: false
+  naludaq_rs: false
 params:
-  chanmask: 1536
-  channels: 4
-  chanshift: 9
-  clock_file: AODS_300GCC.txt  #  AODS_debugpulse_240MGCC_10Mref.txt
+  chanmask: 3072
+  channels: 14
+  chanshift: 10
+  clock_file: Si5341-RevD-HIPeR_78_125SysClk_312_5GccClk-Registers.txt
   connections:
     - serial
     - d2xx
-    - udp
-  si5341_address: 0xE8
+  si5341_address: 0xEE
   default_baud:
-    111111: 53
-  default_baudrate: 111111
-  default_clock: 200000000.0
-  default_divider: 53
-  default_trigger_value: 2000
-  threshold_scan:
-    min_vref: 0
-    max_vref: 2500
-    start: 500
-    stop: 3500
-    stepsize: 5
-    units: counts
+    3000000: 33
+  default_baudrate: 3000000
+  default_clock: 100000000.0
+  default_divider: 33
+  default_trigger_value: 1500
   expected_scalmon: 2500
   ext_dac:
-    chip: ad5671
-    max_mv: 2500
-    max_counts: 4096
+    max_mv: 1200
+    max_counts: 4095
     channels:
-      0: 2048
-      1: 2175
-      2: 1968
-      3: 2048
-    address_mapping:
-      0..3: 0xC
-    channel_mapping:
-      0: 1
-      1: 0
-      2: 5
-      3: 4
+      0..13: 0
   headers: 3
-  numregs: 36
-  pedestals_blocks: 32
+  numregs: 64
+  pedestals_blocks: 16
   peripherals:
     current:
       chan: 0
       addr: 0xD0
       bits: 16
       gain: 8
     vadjn:
@@ -63,746 +44,777 @@
       bits: 16
       gain: 1
     vadjp:
       chan: 1
       addr: 0xD8
       bits: 16
       gain: 1
-    eeprom:
-      addr: 0x50 # 7-bit
-      capacity: 0x20000 # bytes
-      page_size: 256 # bytes
-      segments:
-        analog_registers:
-          begin: 0
-          length: 300
-        digital_registers:
-          begin: 300
-          length: 330
-        control_registers:
-          begin: 630
-          length: 70
   possible_bauds:
-    111111: 53
-    1500000: 3
+    #115200: 53
+    # 230400: 26
+    # 691200: 8
+    # 1041667: 5
+    3000000: 33
   resolution: 12
   samples: 64
-  samplingrate: 1.0
+  samplingrate: 10.0
   stop_word: !!binary |
-    +s4=
+    pa9a/Dw8
   wait: AE000001
-  wbias: 848
-  windmask: 510
-  windows: 254
+  wbias: 2000
+  windmask: 1022
+  windows: 64
 registers:
   analog_registers:
-    cmpbias:
-      address: 0x14
+    cal:
+      address: 0x01
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 1000
-    cmpbias2:
-      address: 0x16
+      value: 0
+    cal_buff:
+      address: 0x3B
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 737
-    dbbias:
-      address: 0x18
+      value: 3500
+    cal_isel:
+      address: 0x3A
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 1300
-    isel:
-      address: 0x1B
+      value: 0
+    calstrb_le:
+      address: 0x25
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2530  # 2680
-    itbias:
-      address: 0x12
+      value: 1 # 0
+    calstrb_te:
+      address: 0x26
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2048
-    ittbias:
+      value: 61 # 30
+    inp0vcurrn:
       address: 0x11
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2048
-    mont_on:
-      address: 0x17
-      bitposition: 3
-      bitwidth: 1
+      value: 1604
+    inp0vcurrp:
+      address: 0x13
+      bitposition: 0
+      bitwidth: 12
       description: ''
       readwrite: w
-      value: 0
-    mont_select:
-      address: 0x17
+      value: 2218
+    inp0vgmn:
+      address: 0x0D
       bitposition: 0
-      bitwidth: 3
+      bitwidth: 12
       description: ''
       readwrite: w
-      value: 0
-    offset_00:
-      address: 0x01
+      value: 2389
+    inp0vgmp:
+      address: 0x0F
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 0
-    offset_01:
-      address: 0x04
+      value: 1536
+    inp1vcurrn:
+      address: 0x09
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 0
-    offset_02:
-      address: 0x07
+      value: 2218
+    inp1vcurrp:
+      address: 0x0B
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 0
-    offset_03:
-      address: 0x0A
+      value: 1604
+    inp1vgmn:
+      address: 0x05
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 0
-    pubias:
-      address: 0x15
+      value: 2389
+    inp1vgmp:
+      address: 0x07
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 3112
-    qbias:
-      address: 0x1C
+      value: 1536
+    inp2vcurrn:
+      address: 0x2A
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2048
-    qbuff:
-      address: 0x1D
+      value: 1604
+    inp2vcurrp:
+      address: 0x28
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2048
-    sbbias:
-      address: 0x19
+      value: 2218
+    inp2vgmn:
+      address: 0x2E
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 1300
-    sel_0:
-      address: 0x80
-      bitposition: 10
-      bitwidth: 1
-      description: 'Ch0 Input MUX - 0: RF0 Input; 1: Buffered version of RF Input'
-      readwrite: w
-      value: 0
-    sel_1:
-      address: 0x80
-      bitposition: 11
-      bitwidth: 1
-      description: 'Ch0 Input MUX - 0: RF1 Input; 1: Output of Ch1 Gain MUX'
-      readwrite: w
-      value: 0
-    sel_2:
-      address: 0x80
+      value: 2389
+    inp2vgmp:
+      address: 0x2C
       bitposition: 0
-      bitwidth: 1
-      description: 'Ch0 Input MUX - 0: RF2 Input; 1: Buffered (w/gain) copy of Ch1; unity gain controlled by VBIAS3_1-2'
-      readwrite: w
-      value: 0
-    sel_3:
-      address: 0x80
-      bitposition: 1
-      bitwidth: 1
-      description: 'Ch0 Input MUX - 0: RF3 Input; 1: Output of Ch3 Gain MUX'
-      readwrite: w
-      value: 0
-    sel_4:
-      address: 0x80
-      bitposition: 2
-      bitwidth: 1
-      description: 'Ch0 Input MUX - 0: OUT3 OFF (HiZ); 1: Buffered version of RF Input'
-      readwrite: w
-      value: 1
-    sel_5:
-      address: 0x80
-      bitposition: 3
-      bitwidth: 1
-      description: 'Ch1 gain MUX: 0: 8x then unity gain; 1: 3-stage amp then unity gain controlled by VBIAS2_3-4'
-      readwrite: w
-      value: 0
-    sel_6:
-      address: 0x80
-      bitposition: 5
-      bitwidth: 1
-      description: 'Ch3 gain MUX: 0: 8x then unity gain; 1: 3-stage amp then unity gain controlled by VBIAS4_3-4'
-      readwrite: w
-      value: 0
-    sel_7:
-      address: 0x80
-      bitposition: 4
-      bitwidth: 1
-      description: 'Gain Stage Input for Ch3; 0: Output from CH2 1: Output from CH0'
+      bitwidth: 12
+      description: ''
       readwrite: w
-      value: 0
-    misc_ts:
-      address: 0x80
-      bitposition: 7
-      bitwidth: 3
-      description: 'diode temperature sensors'
+      value: 1536
+    inp3vcurrn:
+      address: 0x32
+      bitposition: 0
+      bitwidth: 12
+      description: ''
       readwrite: w
-      value: 0
-    scvbias0:
-      address: 0x0D
+      value: 1604
+    inp3vcurrp:
+      address: 0x30
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2048 #800  # 1800?
-    scvbias1:
-      address: 0x0E
+      value: 2218
+    inp3vgmn:
+      address: 0x36
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2048 #800  # 1800?
-    scvbias2:
-      address: 0x0F
+      value: 2389
+    inp3vgmp:
+      address: 0x34
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2048 #800  # 1800?
-    scvbias3:
-      address: 0x10
+      value: 1536
+    isel:
+      address: 0x15
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2048 #800  # 1800?
-    sgn:
-      address: 0x17
-      bitposition: 6
+      value: 2730
+    mont1_on:
+      address: 0x00
+      bitposition: 3
       bitwidth: 1
       description: ''
       readwrite: w
-      value: 0
-    sspin_le:
-      address: 0x2B
-      bitposition: 0
-      bitwidth: 12
+      value: false
+    mont1_select:
+      address: 0x00
+      bitposition: 4
+      bitwidth: 2
       description: ''
       readwrite: w
-      value: 100
-    sspin_te:
-      address: 0x2C
+      value: 0
+    mont2_on:
+      address: 0x00
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 1
       description: ''
       readwrite: w
-      value: 25
-    sstin_ext:
-      address: 0x17
-      bitposition: 4
-      bitwidth: 1
+      value: false
+    mont2_select:
+      address: 0x00
+      bitposition: 1
+      bitwidth: 2
       description: ''
       readwrite: w
       value: 0
-    sstoutfb:
-      address: 0x22
+    qbias:
+      address: 0x18
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 126
-    tbbias:
-      address: 0x0C
+      value: 2048
+    sc0_vbias:
+      address: 0x12
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 1000
-    trigger_threshold_00:
-      address: 0x00
+      value: 1570
+    sc0_vstab:
+      address: 0x10
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 1800
-    trigger_threshold_01:
-      address: 0x03
+      value: 1365
+    sc1_vbias:
+      address: 0x0A
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 1800
-    trigger_threshold_02:
-      address: 0x06
+      value: 1570
+    sc1_vstab:
+      address: 0x08
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 1800
-    trigger_threshold_03:
-      address: 0x09
+      value: 1365
+    sc2_vbias:
+      address: 0x29
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 1800
-    tsel:
-      address: 0x17
-      bitposition: 5
-      bitwidth: 1
-      description: ''
-      readwrite: w
-      value: 1
-    vadjn:
-      address: 0x1E
+      value: 1570
+    sc2_vstab:
+      address: 0x2B
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 1550
-    vadjp:
-      address: 0x20
+      value: 1365
+    sc3_vbias:
+      address: 0x31
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2200
-    vanbuff:
-      address: 0x1F
+      value: 1570
+    sc3_vstab:
+      address: 0x33
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 0
-    vapbuff:
-      address: 0x21
-      bitposition: 0
-      bitwidth: 12
+      value: 1365
+    sgn:
+      address: 0x00
+      bitposition: 10
+      bitwidth: 1
       description: ''
       readwrite: w
-      value: 2816
-    vbias0_0:
-      address: 0x81
-      bitposition: 0
-      bitwidth: 12
+      value: false
+    sspin:
+      address: 0x00
+      bitposition: 6
+      bitwidth: 2
       description: ''
       readwrite: w
-      value: 2801
-    vbias0_1:
-      address: 0x82
-      bitposition: 0
-      bitwidth: 12
+      value: 3
+    sstin_sel:
+      address: 0x00
+      bitposition: 9
+      bitwidth: 1
       description: ''
       readwrite: w
-      value: 2604
-    vbias1_0:
-      address: 0x85
+      value: true
+    sta_vcomp:
+      address: 0x02
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2801
-    vbias1_1:
-      address: 0x84
+      value: 1000
+    vadjn:
+      address: 0x1C
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2604
-    vbias1_2:
-      address: 0x89
-      bitposition: 0
-      bitwidth: 12
+      value: 1696
+    vadjn_sw:
+      address: 0x00
+      bitposition: 8
+      bitwidth: 1
       description: ''
       readwrite: w
-      value: 2048
-    vbias1_3:
-      address: 0x8A
+      value: true
+    vadjp:
+      address: 0x19
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 1147
-    vbias2_0:
-      address: 0x86
+      value: 0
+    vlimn:
+      address: 0x1B
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2801
-    vbias2_1:
-      address: 0x87
+      value: 0
+    vlimp:
+      address: 0x1A
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2604
-    vbias3_0:
-      address: 0x8C
+      value: 4095
+    trigger_threshold_00:
+      address: 0x0E
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2801
-    vbias3_1:
-      address: 0x88
+      value: 0
+    trigger_threshold_01:
+      address: 0x06
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2604
-    vbias3_2:
-      address: 0x8B
+      value: 0
+    trigger_threshold_02:
+      address: 0x2D
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2048
-    vbias3_3:
-      address: 0x8D
+      value: 0
+    trigger_threshold_03:
+      address: 0x35
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 1147
-    vdischarge:
-      address: 0x1A
+      value: 0
+    vrmpvbias:
+      address: 0x17
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 0
-    wbbias:
-      address: 0x13
+      value: 1570
+    vtune:
+      address: 0x16
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2048
+      value: 1365
     wbias_00:
-      address: 0x02
+      address: 0x0C
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 700
+      value: 0
     wbias_01:
-      address: 0x05
+      address: 0x04
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 700
+      value: 0
     wbias_02:
-      address: 0x08
+      address: 0x2F
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 700
+      value: 0
     wbias_03:
-      address: 0x0B
+      address: 0x37
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 700
-    wr_strb1_le:
-      address: 0x23
+      value: 0
+    wrstrb1_le:
+      address: 0x1D
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 64
-    wr_strb1_te:
-      address: 0x24
+      value: 114 # 40
+    wrstrb1_te:
+      address: 0x1E
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 83  #67 ??
-    wr_strb2_le:
-      address: 0x25
+      value: 54
+    wrstrb2_le:
+      address: 0x21
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 0
-    wr_strb2_te:
-      address: 0x26
+      value: 13 # 103
+    wrstrb2_te:
+      address: 0x22
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 29  # 3??
-    wr_sync1_le:
-      address: 0x27
+      value: 73 # 36
+    wrsync1_le:
+      address: 0x1F
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 10
-    wr_sync1_te:
-      address: 0x28
+      value: 1 # 0
+    wrsync1_te:
+      address: 0x20
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 50
-    wr_sync2_le:
-      address: 0x29
+      value: 101 #50
+    wrsync2_le:
+      address: 0x23
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 80
-    wr_sync2_te:
-      address: 0x2A
+      value: 126 # 64
+    wrsync2_te:
+      address: 0x24
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 110
+      value: 26 # 114
   control_registers:
-    trig_mux:
-      address: 0x22
-      bitposition: 5
-      bitwidth: 4
-      description: 'evttrig driver'
-      readwrite: rw
-      value: 3
-    fpga_misc_t:
-      address: 0x22
-      bitposition: 0
-      bitwidth: 4
-      description: 'fpga misc output disable'
+    1v2_en:
+      address: 0x17
+      bitposition: 1
+      bitwidth: 1
+      description: ''
       readwrite: rw
-      value: 15
+      value: true
     2v5_en:
-      address: 0x16
+      address: 0x17
       bitposition: 0
       bitwidth: 1
       description: ''
       readwrite: rw
       value: true
-    2v5_pll_en:
-      address: 0x16
-      bitposition: 1
+    3v3_i2c_en:
+      address: 0x17
+      bitposition: 2
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: false
+      value: true
+    8b10b_en:
+      address: 0x19
+      bitposition: 12
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: 0
     addr:
-      address: 0x15
+      address: 0x16
       bitposition: 0
       bitwidth: 9
       description: ''
       readwrite: rw
       value: 0
     addr_user:
-      address: 0x15
+      address: 0x16
       bitposition: 15
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
-    brightness_blue:
-      address: 0x0A
-      bitposition: 0
-      bitwidth: 8
-      description: ''
-      readwrite: rw
-      value: 0
-    brightness_red:
-      address: 0x0B
+    ard_trig_0_in:  # TODO: New register, verify address and value
+      address: 0x47
       bitposition: 0
-      bitwidth: 8
-      description: ''
-      readwrite: rw
-      value: 0
-    brightness_white:
-      address: 0x0A
-      bitposition: 8
-      bitwidth: 8
+      bitwidth: 16
       description: ''
-      readwrite: rw
+      readwrite: r
       value: 0
     chansel:
       address: 0x06
       bitposition: 12
       bitwidth: 4
       description: ''
       readwrite: rw
       value: 15
-    clk_1v8_nshutdown:
-      address: 0x16
-      bitposition: 2
+    clk1v8_en:
+      address: 0x17
+      bitposition: 4
       bitwidth: 1
       description: ''
       readwrite: rw
       value: true
-    clk_2v5_en:
-      address: 0x16
-      bitposition: 6
+    clk2v5_en:
+      address: 0x17
+      bitposition: 3
       bitwidth: 1
       description: ''
       readwrite: rw
       value: true
-    clk_i2c_sel:
-      address: 0x16
-      bitposition: 5
+    clk_fdec:
+      address: 0x17
+      bitposition: 9
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: true
-    clk_noe:
-      address: 0x16
-      bitposition: 4
+      value: false
+    clk_finc:
+      address: 0x17
+      bitposition: 8
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
-    clk_nrst:
-      address: 0x16
-      bitposition: 3
+    clk_i2c_sel:
+      address: 0x17
+      bitposition: 5
       bitwidth: 1
       description: ''
       readwrite: rw
       value: true
-    clk_nsync:
-      address: 0x16
+    clk_oeb:
+      address: 0x17
+      bitposition: 6
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: false
+    clk_reset:
+      address: 0x17
       bitposition: 7
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
-    dac_nrst:
-      address: 0x16
+    clk_sync:
+      address: 0x17
       bitposition: 10
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 1
+      value: false
+    clk_sel0:  # TODO: Newly added, verify default value
+      address: 0x17
+      bitposition: 11
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: false
+    clk_sel1:  # TODO: Newly added, verify default value
+      address: 0x17
+      bitposition: 12
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: false
     data:
       address: 0x14
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
     data_user:
       address: 0x14
       bitposition: 15
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
+    debug_data:
+      address: 0x15
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: rw
+      value: 0
+    debug_data_user:
+      address: 0x15
+      bitposition: 15
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: false
     digrst:
       address: 0x16
       bitposition: 9
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    ext_en:
-      address: 0x0B
-      bitposition: 9
+    digser_rst:
+      address: 0x19
+      bitposition: 13
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: true
+      value: 0
+    digser_tx_storage0:  # TODO: New register, verify address and value
+      address: 0x4D
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: r
+      value: 0
+    digser_tx_storage1:  # TODO: New register, verify address and value
+      address: 0x4E
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: r
+      value: 0
+    digser_tx_storage2:  # TODO: New register, verify address and value
+      address: 0x4F
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: r
+      value: 0
+    digser_tx_storage3:  # TODO: New register, verify address and value
+      address: 0x50
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: r
+      value: 0
+    digser_tx_storage4:  # TODO: New register, verify address and value
+      address: 0x51
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: r
+      value: 0
+    digser_tx_storage5:  # TODO: New register, verify address and value
+      address: 0x52
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: r
+      value: 0
+    digser_tx_storage6:  # TODO: New register, verify address and value
+      address: 0x53
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: r
+      value: 0
+    digser_tx_storage7:  # TODO: New register, verify address and value
+      address: 0x54
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: r
+      value: 0
+    digser_tx_storage8:  # TODO: New register, verify address and value
+      address: 0x55
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: r
+      value: 0
+    digser_tx_storage9:  # TODO: New register, verify address and value
+      address: 0x56
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: r
+      value: 0
     exttrig:
       address: 0x04
       bitposition: 10
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
-    fake:
-      address: 0x06
-      bitposition: 0
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: 0
     gccclr:
       address: 0x04
-      bitposition: 3
+      bitposition: 4
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
-    i2c_switch:
-      address: 0x16
-      bitposition: 8
-      bitwidth: 1
+    iaddr_read:  # TODO: New register, verify address and value
+      address: 0x44
+      bitposition: 0
+      bitwidth: 9
       description: ''
-      readwrite: rw
+      readwrite: r
       value: 0
     identifier:
       address: 0x00
       bitposition: 0
       bitwidth: 16
+      description: 'Board model/version unique identifier'
+      readwrite: r
+      value: 43714
+    idigital_lastdigread:  # TODO: New register, verify address and value
+      address: 0x43
+      bitposition: 0
+      bitwidth: 12
       description: ''
       readwrite: r
-      value: 41173
-    in_sel:
-      address: 0x0B
-      bitposition: 12
-      bitwidth: 1
+      value: 0
+    idigital_readout_count:  # TODO: New register, verify address and value
+      address: 0x45
+      bitposition: 0
+      bitwidth: 16
       description: ''
-      readwrite: rw
-      value: true
+      readwrite: r
+      value: 0
     iomode0:
       address: 0x04
-      bitposition: 7
+      bitposition: 0
       bitwidth: 1
-      description: ''
+      description: 'HIPeR 10bit Serial Mode0=0'
       readwrite: rw
-      value: 1
+      value: false
     iomode1:
       address: 0x04
-      bitposition: 8
+      bitposition: 6
       bitwidth: 1
+      description: 'HIPeR 10bit Serial Mode1=1'
+      readwrite: rw
+      value: true
+    leds:
+      address: 0x18
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
     loadwait:
       address: 0x07
       bitposition: 8
       bitwidth: 4
       description: ''
       readwrite: rw
       value: 15
     nramp:
       address: 0x04
-      bitposition: 4
+      bitposition: 5
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
     nrw:
       address: 0x04
       bitposition: 11
@@ -813,45 +825,38 @@
     numwinds:
       address: 0x08
       bitposition: 0
       bitwidth: 8
       description: ''
       readwrite: rw
       value: 1
-    out_sel:
-      address: 0x0B
-      bitposition: 11
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
     pclk:
       address: 0x04
-      bitposition: 1
+      bitposition: 2
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
     pclkwidth:
       address: 0x07
       bitposition: 12
       bitwidth: 4
       description: ''
       readwrite: rw
       value: 15
-    rden:
-      address: 0x04
-      bitposition: 6
-      bitwidth: 1
+    ramplen:
+      address: 0x06
+      bitposition: 0
+      bitwidth: 12
       description: ''
       readwrite: rw
-      value: false
+      value: 2000
     regclr:
       address: 0x04
-      bitposition: 0
+      bitposition: 1
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
     runevs:
       address: 0x05
       bitposition: 0
@@ -941,403 +946,599 @@
       bitposition: 12
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
     selany:
       address: 0x04
-      bitposition: 2
+      bitposition: 3
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
-    stopacq:
-      address: 0x04
-      bitposition: 13
+    slow_sysclk:
+      address: 0x19
+      bitposition: 10
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: false
-    switch_nen:
-      address: 0x0B
+      value: 0
+    sst_double:  # TODO: OR rx_off?? John S documnentation ot clear
+      address: 0x19
+      bitposition: 14
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: 0
+    stopacq:
+      address: 0x04
       bitposition: 13
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: true
+      value: false
     syncloc:
-      address: 0x0E
+      address: 0x09
       bitposition: 0
       bitwidth: 8
       description: ''
       readwrite: rw
       value: 0
-    sysrst:
+    sysclk:
       address: 0x04
-      bitposition: 14
+      bitposition: 8
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
-    trig_sel:
-      address: 0x0B
-      bitposition: 10
+    sysrst:
+      address: 0x04
+      bitposition: 9
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: false
+      value: true
+    tx_en:
+      address: 0x19
+      bitposition: 11
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: 0
+    version:  # TODO: New register, verify address and value
+      address: 0x01
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: w
+      value: 0
     windsel:
       address: 0x07
       bitposition: 0
       bitwidth: 8
       description: ''
       readwrite: rw
       value: 0
-    wren:
+    wrstrboff:
       address: 0x04
-      bitposition: 5
+      bitposition: 7
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
-  digital_registers:
-    chipid:
-      address: 0x89
+    crc_en:
+      address: 0x21
       bitposition: 0
-      bitwidth: 12
-      description: ''
+      bitwidth: 1
+      description: 'HIPeR Serial Command CRC Enable'
       readwrite: rw
-      value: 2730
-    convertresetwait:
-      address: 0x84
-      bitposition: 0
-      bitwidth: 8
-      description: ''
+      value: 0
+    eof_en:
+      address: 0x21
+      bitposition: 1
+      bitwidth: 1
+      description: 'HIPeR Serial Command EOF Enable'
+      readwrite: rw
+      value: 0
+    header_en:
+      address: 0x21
+      bitposition: 2
+      bitwidth: 1
+      description: 'HIPeR Chip data header, add a header to all data from a chip: BBB + chip_number(hex)'
       readwrite: rw
       value: 1
-    enabletestpatt:
-      address: 0x88
+    footer_en:
+      address: 0x21
+      bitposition: 3
+      bitwidth: 1
+      description: 'HIPeR Chip data footer, add a footer to all data from a chip: FFF + chip_number(hex)'
+      readwrite: rw
+      value: 1
+    packet_footer_en:
+      address: 0x21
+      bitposition: 4
+      bitwidth: 1
+      description: 'HIPeR pack footer, add a footer after all chips data have been read. 0xFACE'
+      readwrite: rw
+      value: 1
+    rxout_pol:
+      address: 0x22
+      bitposition: 0
+      bitwidth: 16
+      description: 'HIPeR RxOut Input Polarity Control'
+      readwrite: rw
+      value: 6400
+    txin_pol:
+      address: 0x23
+      bitposition: 0
+      bitwidth: 16
+      description: 'HIPeR TxIn Output Polarity Control'
+      readwrite: rw
+      value: 4412
+    txin_en:
+      address: 0x24
+      bitposition: 0
+      bitwidth: 16
+      description: 'HIPeR TxIn Input Enable. Data from ASIC to FPGA. Keep off unless receving data or registersfrom ASIC'
+      readwrite: rw
+      value: 0
+    rxout_en:
+      address: 0x25
+      bitposition: 0
+      bitwidth: 16
+      description: 'HIPeR RxOut Output Enable. Data from FPGA to ASIC. Keep on unless busy_locked is high.'
+      readwrite: rw
+      value: 65535
+    amp_pwrdn_n:
+      address: 0x26
+      bitposition: 0
+      bitwidth: 16
+      description: 'HIPeR AMP PowerDown_n'
+      readwrite: rw
+      value: 0
+    # txin_logic:  # TODO: New register, verify address and value
+    #   address: 0x26
+    #   bitposition: 0
+    #   bitwidth: 16
+    #   description: ''
+    #   readwrite: rw
+    #   value: 0
+    v2v5_pwr_good:  # TODO: New register, verify address and value
+      address: 0x46
       bitposition: 0
       bitwidth: 1
       description: ''
+      readwrite: r
+      value: 0
+    v1v2_pwr_good:  # TODO: New register, verify address and value
+      address: 0x46
+      bitposition: 1
+      bitwidth: 1
+      description: ''
+      readwrite: r
+      value: 0
+    dac_r_update:
+      address: 0x27
+      bitposition: 15
+      bitwidth: 1
+      description: 'HIPeR SPI DAC Right Side Update Toggle'
       readwrite: rw
       value: 0
-    excludechannelmask:
-      address: 0x96
+    dac_r_cmd:
+      address: 0x27
+      bitposition: 8
+      bitwidth: 4
+      description: 'HIPeR DAC Right Side SPI Command'
+      readwrite: rw
+      value: 3
+    dac_r_addr:
+      address: 0x27
+      bitposition: 4
+      bitwidth: 4
+      description: 'HIPeR DAC Right Side SPI Address'
+      readwrite: rw
+      value: 15
+    dac_r_asic:
+      address: 0x27
       bitposition: 0
       bitwidth: 4
-      description: ''
+      description: 'HIPeR DAC Right Side ASIC Address'
       readwrite: rw
       value: 0
-    fineoffset:
-      address: 0x8D
+    dac_r_value:
+      address: 0x28
       bitposition: 0
       bitwidth: 12
-      description: ''
+      description: 'HIPeR DAC Right Side 12 bit Value'
       readwrite: rw
       value: 0
-    loadwait:
-      address: 0x8B
+    dac_l_update:
+      address: 0x29
+      bitposition: 15
+      bitwidth: 1
+      description: 'HIPeR SPI DAC Left Side Update Toggle'
+      readwrite: rw
+      value: 0
+    dac_l_cmd:
+      address: 0x29
+      bitposition: 8
+      bitwidth: 4
+      description: 'HIPeR DAC Left Side SPI Command'
+      readwrite: rw
+      value: 3
+    dac_l_addr:
+      address: 0x29
+      bitposition: 4
+      bitwidth: 4
+      description: 'HIPeR DAC Left Side SPI Address'
+      readwrite: rw
+      value: 15
+    dac_l_asic:
+      address: 0x29
       bitposition: 0
-      bitwidth: 7
-      description: ''
+      bitwidth: 4
+      description: 'HIPeR DAC Left Side ASIC Address'
       readwrite: rw
       value: 0
-    masktrig:
-      address: 0x90
+    dac_l_value:
+      address: 0x2A
       bitposition: 0
       bitwidth: 12
-      description: ''
+      description: 'HIPeR DAC Left Side 12 bit Value'
       readwrite: rw
       value: 0
-    max0:
-      address: 0xA1
+    exttrig_en:
+      address: 0x2B
       bitposition: 0
-      bitwidth: 12
-      description: ''
+      bitwidth: 16
+      description: 'HIPeR External Trigger Mask, set to one per chip'
       readwrite: rw
       value: 0
-    max1:
-      address: 0xA2
+    max_trig_count:
+      address: 0x2C
       bitposition: 0
-      bitwidth: 12
-      description: ''
+      bitwidth: 16
+      description: 'Maximum triggers before masking ext trig inputs'
       readwrite: rw
       value: 0
-    max2:
-      address: 0xA3
+    trig_count_reset:
+      address: 0x2D
       bitposition: 0
-      bitwidth: 12
-      description: ''
+      bitwidth: 1
+      description: 'Toggle to reset trig_count, if left at 1, triggers are disabled'
       readwrite: rw
       value: 0
-    max3:
-      address: 0xA4
+    idle_det:
+      address: 0x5D
+      bitposition: 0
+      bitwidth: 16
+      description: 'HIPeR TxIn Idle Detect Status'
+      readwrite: r
+      value: 0
+    busy_locked:
+      address: 0x5C
+      bitposition: 0
+      bitwidth: 16
+      description: 'HIPeR RxOut Busy_Locked Status'
+      readwrite: r
+      value: 0
+  digital_registers:
+    bank:
+      address: 0x9D
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
-    min0:
-      address: 0x9D
+    # pulselength32:  # TODO: New register, verify address and value
+    #   address: 0x9A
+    #   bitposition: 0
+    #   bitwidth: 12
+    #   description: ''
+    #   readwrite: rw
+    #   value: 0
+    chipid:
+      address: 0x89
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
-      value: 0
-    min1:
-      address: 0x9E
+      value: 2730
+    convertresetwait:
+      address: 0x84
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
-      value: 0
-    min2:
-      address: 0x9F
+      value: 1
+    # donetimeoutn:  # TODO: New register, verify address and value
+    #   address: 0xA0
+    #   bitposition: 0
+    #   bitwidth: 12
+    #   description: ''
+    #   readwrite: rw
+    #   value: 0
+    enabletestpatt:
+      address: 0x88
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
-    min3:
-      address: 0xA0
+    # excludechan:  # TODO: New register, verify address and value
+    #   address: 0x96
+    #   bitposition: 0
+    #   bitwidth: 4
+    #   description: ''
+    #   readwrite: rw
+    #   value: 0
+    loadwait:
+      address: 0x8B
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
+    # masktrig:  # TODO: New register, verify address and value
+    #   address: 0x90
+    #   bitposition: 0
+    #   bitwidth: 12
+    #   description: ''
+    #   readwrite: rw
+    #   value: 0
+    miscreg:
+      address: 0x8D
+      bitposition: 0
+      bitwidth: 12
+      description: 'HIPeR MISCREG = 2'
+      readwrite: rw
+      value: 2
     pclkwidth:
       address: 0x8C
       bitposition: 0
-      bitwidth: 7
+      bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
-    pll:
+    pllmisc:  # TODO: New register, verify address and value
       address: 0x93
       bitposition: 0
-      bitwidth: 6
-      description: ''
-      readwrite: rw
-      value: 0
-    pulselength10:
-      address: 0x99
-      bitposition: 0
-      bitwidth: 12
-      description: ''
+      bitwidth: 5
+      description: 'HIPeR PLLMISC = 0'
       readwrite: rw
       value: 0
-    pulselength32:
-      address: 0x9A
+    # pulselength10:  # TODO: New register, verify address and value
+    #   address: 0x99
+    #   bitposition: 0
+    #   bitwidth: 12
+    #   description: ''
+    #   readwrite: rw
+    #   value: 0
+    # pulselength32:  # TODO: New register, verify address and value
+    #   address: 0x9A
+    #   bitposition: 0
+    #   bitwidth: 12
+    #   description: ''
+    #   readwrite: rw
+    #   value: 0
+    readoutchannels:
+      address: 0x87
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
     readoutlookback:
       address: 0x85
       bitposition: 0
-      bitwidth: 8
+      bitwidth: 12
       description: ''
       readwrite: rw
       value: 18
-    readoutoffset:
-      address: 0x87
-      bitposition: 0
-      bitwidth: 8
-      description: ''
-      readwrite: rw
-      value: 122
     readoutwindows:
       address: 0x86
       bitposition: 0
-      bitwidth: 8
+      bitwidth: 12
       description: ''
       readwrite: rw
       value: 10
     regclr:
       address: 0x8A
       bitposition: 0
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: 0
-    roilength10:
-      address: 0x9B
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: rw
-      value: 0
-    roilength32:
-      address: 0x9C
-      bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
+    # roilength10:  # TODO: New register, verify address and value
+    #   address: 0x9B
+    #   bitposition: 0
+    #   bitwidth: 12
+    #   description: ''
+    #   readwrite: rw
+    #   value: 0
+    # roilength32:  # TODO: New register, verify address and value
+    #   address: 0x9C
+    #   bitposition: 0
+    #   bitwidth: 12
+    #   description: ''
+    #   readwrite: rw
+    #   value: 0
     scal0:
       address: 0x00
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: w
+      readwrite: rw
       value: 0
     scal1:
       address: 0x01
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: w
+      readwrite: rw
       value: 0
     scal2:
       address: 0x02
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: w
+      readwrite: rw
       value: 0
     scal3:
       address: 0x03
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: w
+      readwrite: rw
       value: 0
     scalhigh:
       address: 0x40
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: w
+      readwrite: rw
       value: 0
     scalmon:
       address: 0x08
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: w
-      value: 0
-    speed:
-      address: 0x92
-      bitposition: 0
-      bitwidth: 10
-      description: ''
       readwrite: rw
       value: 0
+    # speed:  # TODO: New register, verify address and value
+    #   address: 0x92
+    #   bitposition: 0
+    #   bitwidth: 10
+    #   description: ''
+    #   readwrite: rw
+    #   value: 0
+    # test_caps:  # TODO: New register, verify address and value
+    #   address: 0x9E
+    #   bitposition: 0
+    #   bitwidth: 12
+    #   description: ''
+    #   readwrite: rw
+    #   value: 0
+    # test_dline:  # TODO: New register, verify address and value
+    #   address: 0x9F
+    #   bitposition: 0
+    #   bitwidth: 12
+    #   description: ''
+    #   readwrite: rw
+    #   value: 0
     testpatin:
       address: 0x0A
       bitposition: 0
-      bitwidth: 3
-      description: ''
-      readwrite: w
-      value: 0
-    trigfinedelay10:
-      address: 0x97
-      bitposition: 0
-      bitwidth: 8
-      description: ''
-      readwrite: rw
-      value: 0
-    trigfinedelay32:
-      address: 0x98
-      bitposition: 0
-      bitwidth: 8
+      bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
-    txspeed:
+    # trigfinedelay10:  # TODO: New register, verify address and value
+    #   address: 0x97
+    #   bitposition: 0
+    #   bitwidth: 8
+    #   description: ''
+    #   readwrite: rw
+    #   value: 0
+    # trigfinedelay32:  # TODO: New register, verify address and value
+    #   address: 0x98
+    #   bitposition: 0
+    #   bitwidth: 8
+    #   description: ''
+    #   readwrite: rw
+    #   value: 0
+    txspeed:  # TODO: New register, verify address and value
       address: 0x94
       bitposition: 0
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: 0
-    waitaddr:
-      address: 0x8F
-      bitposition: 0
-      bitwidth: 3
-      description: ''
+      bitwidth: 2
+      description: 'HIPeR TXSPEED = 2'
       readwrite: rw
-      value: 0
-    waitread:
+      value: 2
+    # waitaddr:  # TODO: New register, verify address and value
+    #   address: 0x8F
+    #   bitposition: 0
+    #   bitwidth: 3
+    #   description: ''
+    #   readwrite: rw
+    #   value: 0
+    waitread:  # TODO: New register, verify address and value
       address: 0x8E
       bitposition: 0
       bitwidth: 3
-      description: ''
+      description: 'HIPeR WAITREAD = 1'
       readwrite: rw
       value: 1
-    wlc_on:
-      address: 0x95
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: rw
-      value: 0
+    # wlc_on:  # TODO: New register, verify address and value
+    #   address: 0x95
+    #   bitposition: 0
+    #   bitwidth: 12
+    #   description: ''
+    #   readwrite: rw
+    #   value: 0
     wraddrjunk:
       address: 0x82
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
-      value: 127
+      value: 255
     wraddrstart:
       address: 0x80
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
     wraddrstop:
       address: 0x81
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
-      value: 126
+      value: 31
     writeaftertrig:
       address: 0x83
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
-      value: 5
-    writedelay:
-      address: 0x91
-      bitposition: 0
-      bitwidth: 3
-      description: ''
-      readwrite: rw
-      value: 0
+      value: 31
+    # writedelay:  # TODO: New register, verify address and value
+    #   address: 0x91
+    #   bitposition: 0
+    #   bitwidth: 3
+    #   description: ''
+    #   readwrite: rw
+    #   value: 0
   i2c_registers:
     i2c_en:
-      address: 0x09
+      address: 0x0F
       bitposition: 14
       bitwidth: 1
       description: ''
       readwrite: rw
       value: true
     i2c_send:
       address: 0x0F
       bitposition: 15
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    i2c_words:
+    i2c_addr:
       address: 0x0F
-      bitposition: 8
-      bitwidth: 3
+      bitposition: 0
+      bitwidth: 8
       description: ''
       readwrite: rw
       value: 0
-    i2c_addr:
+    i2c_words:
       address: 0x0F
-      bitposition: 0
-      bitwidth: 8
+      bitposition: 8
+      bitwidth: 3
       description: ''
       readwrite: rw
       value: 0
     i2c_data0:
       address: 0x10
       bitposition: 0
       bitwidth: 16
@@ -1362,34 +1563,34 @@
       address: 0x13
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
     response0:
-      address: 0x2C
+      address: 0x48
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: r
       value: 0
     response1:
-      address: 0x2D
+      address: 0x49
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: r
       value: 0
     response2:
-      address: 0x2E
+      address: 0x4A
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: r
       value: 0
     response3:
-      address: 0x2F
+      address: 0x4B
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: r
       value: 0
```

### Comparing `naluconfigs-10.8.0/src/naluconfigs/data/registers/asoc.yml` & `naluconfigs-11.0.0/src/naluconfigs/data/registers/siread.yml`

 * *Files 7% similar despite different names*

```diff
@@ -1,885 +1,956 @@
-model: asoc
+model: siread
 features:
   adc2mv: false
   dac_sweep: false
-  pedestals: true
-  threshold_scan: true
+  pedestals: false
+  threshold_scan: false
   tia_dac: false
   timing_calibration: false
   naludaq_rs: false
 params:
-  chanmask: 6144
-  channels: 4
-  chanshift: 11
-  clock_file: Si5341-RevD-Lambchop-Registers_compSysclk.txt
+  chanmask: 3968
+  channels: 32
   connections:
     - serial
     - d2xx
-  si5341_address: 0xE8
   default_baud:
-    115200: 53
-  default_baudrate: 115200
-  default_clock: 100000000.0
+    230400: 53
+  default_baudrate: 230400
+  default_clock: 200000000.0
   default_divider: 53
   expected_scalmon: 2500
-  ext_dac:
-    max_mv: 2500
-    max_counts: 4095
-    channels:
-      0: 2000
-      1: 2000
-      2: 2000
-      3: 2000
-  headers: 4
+  headers: 3
   last_window_fix_amount: 47
   numregs: 32
-  pedestals_blocks: 64
-  peripherals:
-    current:
-      chan: 0
-      addr: 0xD0
-      bits: 16
-      gain: 8
-    vadjn:
-      chan: 0
-      addr: 0xD8
-      bits: 16
-      gain: 1
-    vadjp:
-      chan: 1
-      addr: 0xD8
-      bits: 16
-      gain: 1
+  pedestals_blocks: 8
   possible_bauds:
-    115200: 53
-    3000000: 1
+    230400: 53
+    625000: 19
   resolution: 12
-  samples: 64
-  samplingrate: 3.2
+  samples: 32
+  samplingrate: 1.0
   stop_word: !!binary |
     +s4=
   wait: AE000001
-  wbias: 848
-  windmask: 510
-  windows: 256
+  wbias: 750
+  windmask: 126
+  windows: 64
 registers:
   analog_registers:
+    cloadn:
+      address: 0x100
+      bitposition: 10
+      bitwidth: 1
+      description: ''
+      readwrite: w
+      value: 1
+    cloadp:
+      address: 0x100
+      bitposition: 9
+      bitwidth: 1
+      description: ''
+      readwrite: w
+      value: 0
     cmpbias:
-      address: 0x14
+      address: 0x117
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 1000
+      value: 1242
     cmpbias2:
-      address: 0x16
+      address: 0x119
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 737
+      value: 846
     dbbias:
-      address: 0x18
+      address: 0x112
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 1300
+      value: 1100
     isel:
-      address: 0x1B
+      address: 0x115
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2700
+      value: 2770
     itbias:
-      address: 0x12
+      address: 0x11F
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: w
+      value: 1000
+    mont_on:
+      address: 0x100
+      bitposition: 8
+      bitwidth: 1
+      description: ''
+      readwrite: w
+      value: 1
+    mont_select:
+      address: 0x100
+      bitposition: 5
+      bitwidth: 3
+      description: ''
+      readwrite: w
+      value: 4
+    ped_00:
+      address: 0x000
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
       value: 2048
-    ittbias:
-      address: 0x11
+    ped_01:
+      address: 0x001
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
       value: 2048
-    mont_on:
-      address: 0x17
-      bitposition: 3
-      bitwidth: 1
+    ped_02:
+      address: 0x002
+      bitposition: 0
+      bitwidth: 12
       description: ''
       readwrite: w
-      value: true
-    mont_select:
-      address: 0x17
+      value: 2048
+    ped_03:
+      address: 0x003
       bitposition: 0
-      bitwidth: 3
+      bitwidth: 12
       description: ''
       readwrite: w
-      value: 0
-    offset_00:
-      address: 0x01
+      value: 2048
+    ped_04:
+      address: 0x010
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 0
-    offset_01:
-      address: 0x04
+      value: 2048
+    ped_05:
+      address: 0x011
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 0
-    offset_02:
-      address: 0x07
+      value: 2048
+    ped_06:
+      address: 0x012
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 0
-    offset_03:
-      address: 0x0A
+      value: 2048
+    ped_07:
+      address: 0x013
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 0
-    pubias:
-      address: 0x15
+      value: 2048
+    ped_08:
+      address: 0x020
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 3112
-    qbias:
-      address: 0x1C
+      value: 2048
+    ped_09:
+      address: 0x021
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 800
-    qbuff:
-      address: 0x1D
+      value: 2048
+    ped_10:
+      address: 0x022
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
       value: 2048
-    sbbias:
-      address: 0x19
+    ped_11:
+      address: 0x023
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 1300
-    scvbias0:
-      address: 0x0D
+      value: 2048
+    ped_12:
+      address: 0x030
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
       value: 2048
-    scvbias1:
-      address: 0x0E
+    ped_13:
+      address: 0x031
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
       value: 2048
-    scvbias2:
-      address: 0x0F
+    ped_14:
+      address: 0x032
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
       value: 2048
-    scvbias3:
-      address: 0x10
+    ped_15:
+      address: 0x033
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
       value: 2048
-    sgn:
-      address: 0x17
-      bitposition: 6
-      bitwidth: 1
+    ped_16:
+      address: 0x040
+      bitposition: 0
+      bitwidth: 12
       description: ''
       readwrite: w
-      value: false
-    sspin_le:
-      address: 0x2B
+      value: 2048
+    ped_17:
+      address: 0x041
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 95
-    sspin_te:
-      address: 0x2C
+      value: 2048
+    ped_18:
+      address: 0x042
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 5
-    sstin_ext:
-      address: 0x17
-      bitposition: 4
-      bitwidth: 1
+      value: 2048
+    ped_19:
+      address: 0x043
+      bitposition: 0
+      bitwidth: 12
       description: ''
       readwrite: w
-      value: false
-    sstoutfb:
-      address: 0x22
+      value: 2048
+    ped_20:
+      address: 0x050
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 114
-    tbbias:
-      address: 0x0C
+      value: 2048
+    ped_21:
+      address: 0x051
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 1000
-    trigger_threshold_00:
-      address: 0x00
+      value: 2048
+    ped_22:
+      address: 0x052
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 0
-    trigger_threshold_01:
-      address: 0x03
+      value: 2048
+    ped_23:
+      address: 0x053
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 0
-    trigger_threshold_02:
-      address: 0x06
+      value: 2048
+    ped_24:
+      address: 0x060
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 0
-    trigger_threshold_03:
-      address: 0x09
+      value: 2048
+    ped_25:
+      address: 0x061
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 0
-    tsel:
-      address: 0x17
-      bitposition: 5
-      bitwidth: 1
+      value: 2048
+    ped_26:
+      address: 0x062
+      bitposition: 0
+      bitwidth: 12
       description: ''
       readwrite: w
-      value: true
-    vadjn:
-      address: 0x1E
+      value: 2048
+    ped_27:
+      address: 0x063
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 1800
-    vadjp:
-      address: 0x20
+      value: 2048
+    ped_28:
+      address: 0x070
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2405
-    vanbuff:
-      address: 0x1F
+      value: 2048
+    ped_29:
+      address: 0x071
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: w
+      value: 2048
+    ped_30:
+      address: 0x072
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: w
+      value: 2048
+    ped_31:
+      address: 0x073
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: w
+      value: 2048
+    pedbias_0:
+      address: 0x004
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: w
+      value: 15
+    pedbias_1:
+      address: 0x014
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: w
+      value: 15
+    pedbias_2:
+      address: 0x024
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: w
+      value: 15
+    pedbias_3:
+      address: 0x034
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: w
+      value: 15
+    pedbias_4:
+      address: 0x044
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: w
+      value: 15
+    pedbias_5:
+      address: 0x054
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: w
+      value: 15
+    pedbias_6:
+      address: 0x064
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: w
+      value: 15
+    pedbias_7:
+      address: 0x074
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: w
+      value: 15
+    pubias:
+      address: 0x118
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: w
+      value: 3112
+    qbias:
+      address: 0x101
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
       value: 0
-    vapbuff:
-      address: 0x21
+    qbuff:
+      address: 0x102
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 2816
-    vdischarge:
-      address: 0x1A
+      value: 1062
+    sbbias:
+      address: 0x113
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: w
+      value: 1300
+    scvbias:
+      address: 0x11E
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
+      value: 3000
+    scvstab:
+      address: 0x11D
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: w
+      value: 1000
+    sgn:
+      address: 0x100
+      bitposition: 2
+      bitwidth: 1
+      description: ''
+      readwrite: w
       value: 0
-    wbbias:
-      address: 0x13
+    spmbias:
+      address: 0x11A
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
       value: 2048
-    wbias_00:
-      address: 0x02
+    sspin_le:
+      address: 0x108
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 350
-    wbias_01:
-      address: 0x05
+      value: 60
+    sspin_te:
+      address: 0x109
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 350
-    wbias_02:
-      address: 0x08
+      value: 50
+    sstoutfb:
+      address: 0x107
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 350
-    wbias_03:
-      address: 0x0B
+      value: 58
+    tbbias:
+      address: 0x11C
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 350
-    wr_strb1_le:
-      address: 0x23
+      value: 2048
+    term:
+      address: 0x100
+      bitposition: 0
+      bitwidth: 2
+      description: ''
+      readwrite: w
+      value: 3
+    thresh_00:
+      address: 0x005
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 65
-    wr_strb1_te:
-      address: 0x24
+      value: 0
+    thresh_01:
+      address: 0x006
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 90
-    wr_strb2_le:
-      address: 0x25
+      value: 0
+    thresh_02:
+      address: 0x007
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
       value: 0
-    wr_strb2_te:
-      address: 0x26
+    thresh_03:
+      address: 0x008
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 25
-    wr_sync1_le:
-      address: 0x27
+      value: 0
+    thresh_04:
+      address: 0x015
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 10
-    wr_sync1_te:
-      address: 0x28
+      value: 0
+    thresh_05:
+      address: 0x016
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 15
-    wr_sync2_le:
-      address: 0x29
+      value: 0
+    thresh_06:
+      address: 0x017
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 80
-    wr_sync2_te:
-      address: 0x2A
+      value: 0
+    thresh_07:
+      address: 0x018
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: w
-      value: 85
-  control_registers:
-    3v3_en_main:
-      address: 0x16
-      bitposition: 6
-      bitwidth: 1
+      value: 0
+    thresh_08:
+      address: 0x025
+      bitposition: 0
+      bitwidth: 12
       description: ''
-      readwrite: rw
-      value: 1
-    addr:
-      address: 0x15
+      readwrite: w
+      value: 0
+    thresh_09:
+      address: 0x026
       bitposition: 0
-      bitwidth: 9
+      bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 0
-    addr_user:
-      address: 0x15
-      bitposition: 15
-      bitwidth: 1
+    thresh_10:
+      address: 0x027
+      bitposition: 0
+      bitwidth: 12
       description: ''
-      readwrite: rw
-      value: false
-    chansel:
-      address: 0x06
-      bitposition: 12
-      bitwidth: 4
+      readwrite: w
+      value: 0
+    thresh_11:
+      address: 0x028
+      bitposition: 0
+      bitwidth: 12
       description: ''
-      readwrite: rw
-      value: 15
-    clk_cal_en:
-      address: 0x16
-      bitposition: 10
-      bitwidth: 1
+      readwrite: w
+      value: 0
+    thresh_12:
+      address: 0x035
+      bitposition: 0
+      bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 0
-    clk_oe:
-      address: 0x16
-      bitposition: 4
-      bitwidth: 1
+    thresh_13:
+      address: 0x036
+      bitposition: 0
+      bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 0
-    clk_rst:
-      address: 0x16
-      bitposition: 5
-      bitwidth: 1
+    thresh_14:
+      address: 0x037
+      bitposition: 0
+      bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 0
-    coin_chanmask:
-      address: 0x17
-      bitposition: 12
-      bitwidth: 4
+    thresh_15:
+      address: 0x038
+      bitposition: 0
+      bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 0
-    coin_length:
-      address: 0x17
+    thresh_16:
+      address: 0x045
       bitposition: 0
-      bitwidth: 6
+      bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 0
-    coin_or_ext:
-      address: 0x16
-      bitposition: 12
-      bitwidth: 1
+    thresh_17:
+      address: 0x046
+      bitposition: 0
+      bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 0
-    coin_pol:
-      address: 0x18
+    thresh_18:
+      address: 0x047
       bitposition: 0
-      bitwidth: 4
+      bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 0
-    coin_triglen:
-      address: 0x17
-      bitposition: 6
-      bitwidth: 6
+    thresh_19:
+      address: 0x048
+      bitposition: 0
+      bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 0
-    dac_a:
-      address: 0x09
+    thresh_20:
+      address: 0x055
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
-      value: 2000
-    dac_b:
-      address: 0x0A
+      readwrite: w
+      value: 0
+    thresh_21:
+      address: 0x056
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
-      value: 2000
-    dac_c:
-      address: 0x0B
+      readwrite: w
+      value: 0
+    thresh_22:
+      address: 0x057
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
-      value: 2000
-    dac_d:
-      address: 0x0C
+      readwrite: w
+      value: 0
+    thresh_23:
+      address: 0x058
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
-      value: 2000
-    dac_send:
-      address: 0x09
-      bitposition: 15
-      bitwidth: 1
+      readwrite: w
+      value: 0
+    thresh_24:
+      address: 0x065
+      bitposition: 0
+      bitwidth: 12
       description: ''
-      readwrite: rw
-      value: false
-    data:
-      address: 0x14
+      readwrite: w
+      value: 0
+    thresh_25:
+      address: 0x066
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 0
-    data_user:
-      address: 0x14
-      bitposition: 15
-      bitwidth: 1
+    thresh_26:
+      address: 0x067
+      bitposition: 0
+      bitwidth: 12
       description: ''
-      readwrite: rw
-      value: false
-    debug:
-      address: 0x04
+      readwrite: w
+      value: 0
+    thresh_27:
+      address: 0x068
       bitposition: 0
-      bitwidth: 1
+      bitwidth: 12
       description: ''
-      readwrite: rw
-      value: false
-    digrst:
-      address: 0x16
-      bitposition: 9
-      bitwidth: 1
+      readwrite: w
+      value: 0
+    thresh_28:
+      address: 0x075
+      bitposition: 0
+      bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 0
-    exttrig:
-      address: 0x04
-      bitposition: 10
-      bitwidth: 1
+    thresh_29:
+      address: 0x076
+      bitposition: 0
+      bitwidth: 12
       description: ''
-      readwrite: rw
-      value: false
-    fake:
-      address: 0x08
-      bitposition: 8
-      bitwidth: 1
+      readwrite: w
+      value: 0
+    thresh_30:
+      address: 0x077
+      bitposition: 0
+      bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 0
-    fpgarst:
-      address: 0x16
-      bitposition: 8
-      bitwidth: 1
+    thresh_31:
+      address: 0x078
+      bitposition: 0
+      bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
       value: 0
-    gccclr:
-      address: 0x04
-      bitposition: 4
-      bitwidth: 1
+    trgbias:
+      address: 0x11B
+      bitposition: 0
+      bitwidth: 12
       description: ''
-      readwrite: rw
-      value: false
-    i2c_en:
-      address: 0x09
-      bitposition: 14
-      bitwidth: 1
+      readwrite: w
+      value: 2419
+    vadjn:
+      address: 0x103
+      bitposition: 0
+      bitwidth: 12
       description: ''
-      readwrite: rw
-      value: true
-    i2c_switch:
-      address: 0x16
-      bitposition: 3
-      bitwidth: 1
+      readwrite: w
+      value: 2360
+    vadjp:
+      address: 0x105
+      bitposition: 0
+      bitwidth: 12
       description: ''
-      readwrite: rw
-      value: false
-    i2c_upperdeck:
-      address: 0x16
-      bitposition: 11
-      bitwidth: 1
+      readwrite: w
+      value: 768
+    vanbuff:
+      address: 0x104
+      bitposition: 0
+      bitwidth: 12
       description: ''
-      readwrite: rw
+      readwrite: w
+      value: 1152
+    vapbuff:
+      address: 0x106
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: w
+      value: 1300
+    vdischarge:
+      address: 0x114
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: w
       value: 0
-    loadwait:
-      address: 0x07
-      bitposition: 8
-      bitwidth: 4
+    wbbias:
+      address: 0x116
+      bitposition: 0
+      bitwidth: 12
       description: ''
-      readwrite: rw
-      value: 15
-    ls_oe:
-      address: 0x16
-      bitposition: 7
-      bitwidth: 1
+      readwrite: w
+      value: 1000
+    wr_addr_incr1_le:
+      address: 0x10A
+      bitposition: 0
+      bitwidth: 12
       description: ''
-      readwrite: rw
-      value: 1
-    muxfast:
-      address: 0x16
+      readwrite: w
+      value: 5
+    wr_addr_incr1_te:
+      address: 0x10B
       bitposition: 0
-      bitwidth: 1
+      bitwidth: 12
       description: ''
-      readwrite: rw
-      value: 0
-    muxfinal:
-      address: 0x16
-      bitposition: 2
-      bitwidth: 1
+      readwrite: w
+      value: 25
+    wr_addr_incr2_le:
+      address: 0x10E
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: w
+      value: 33
+    wr_addr_incr2_te:
+      address: 0x10F
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: w
+      value: 53
+    wrstrb1_le:
+      address: 0x10C
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: w
+      value: 20
+    wrstrb1_te:
+      address: 0x10D
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: w
+      value: 40
+    wrstrb2_le:
+      address: 0x110
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: w
+      value: 56
+    wrstrb2_te:
+      address: 0x111
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: w
+      value: 12
+  control_registers:
+    chansela:
+      address: 0x0A
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
-    muxslow:
-      address: 0x16
-      bitposition: 1
-      bitwidth: 1
+    chanselb:
+      address: 0x0B
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
       value: 1
-    nramp:
+    clk_oe:
       address: 0x04
-      bitposition: 5
+      bitposition: 2
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: false
-    nrw:
-      address: 0x04
-      bitposition: 11
+      value: true
+    digrst:
+      address: 0x0C
+      bitposition: 1
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
-    numwinds:
-      address: 0x08
+    fifo_full_level:
+      address: 0x14
       bitposition: 0
-      bitwidth: 8
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 10
-    pclk:
-      address: 0x04
-      bitposition: 2
+      value: 0
+    i2c_switch:
+      address: 0x16
+      bitposition: 3
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
-    pclkwidth:
+    loadwait:
       address: 0x07
-      bitposition: 12
+      bitposition: 6
       bitwidth: 4
       description: ''
       readwrite: rw
       value: 15
+    lookback:
+      address: 0x08
+      bitposition: 6
+      bitwidth: 6
+      description: ''
+      readwrite: rw
+      value: 0
+    numwinds:
+      address: 0x08
+      bitposition: 0
+      bitwidth: 6
+      description: ''
+      readwrite: rw
+      value: 2
     ramp:
       address: 0x06
       bitposition: 0
       bitwidth: 11
       description: ''
       readwrite: rw
       value: 1500
-    rden:
-      address: 0x04
-      bitposition: 7
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
     regclr:
       address: 0x04
-      bitposition: 1
+      bitposition: 0
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
     runevs:
       address: 0x05
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
       value: 1
-    sel:
-      address: 0x04
-      bitposition: 12
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    selany:
+    sstpattern:
       address: 0x04
-      bitposition: 3
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    si570:
-      address: 0x0D
-      bitposition: 0
-      bitwidth: 16
+      bitposition: 4
+      bitwidth: 8
       description: ''
       readwrite: rw
-      value: 0
+      value: 128
     stopacq:
-      address: 0x04
-      bitposition: 13
+      address: 0x08
+      bitposition: 12
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: false
+      value: 0
     syncloc:
       address: 0x0E
       bitposition: 0
       bitwidth: 8
       description: ''
       readwrite: rw
       value: 0
-    sysclk:
-      address: 0x04
-      bitposition: 8
+    sysrst:
+      address: 0x0C
+      bitposition: 0
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
-    sysrst:
+    v2v5_en:
       address: 0x04
-      bitposition: 9
+      bitposition: 1
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: true
-    windsel:
-      address: 0x07
-      bitposition: 0
-      bitwidth: 8
-      description: ''
-      readwrite: rw
-      value: 0
-    wren:
+      value: false
+    wraddrsync:
       address: 0x04
-      bitposition: 6
+      bitposition: 3
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
-  digital_registers:
-    chipid:
-      address: 0x89
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: rw
-      value: 2730
-    convertresetwait:
-      address: 0x84
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: rw
-      value: 1
-    enabletestpatt:
-      address: 0x88
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: rw
-      value: 0
-    loadwait:
-      address: 0x8B
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: rw
-      value: 0
-    miscreg:
-      address: 0x8D
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: rw
-      value: 0
-    pclkwidth:
-      address: 0x8C
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: rw
-      value: 0
-    readoutchannels:
-      address: 0x87
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: rw
-      value: 0
-    readoutlookback:
-      address: 0x85
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: rw
-      value: 18
-    readoutwindows:
-      address: 0x86
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: rw
-      value: 10
-    regclr:
-      address: 0x8A
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: rw
-      value: 0
-    wraddrjunk:
-      address: 0x82
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: rw
-      value: 127
-    wraddrstart:
-      address: 0x80
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: rw
-      value: 0
-    wraddrstop:
-      address: 0x81
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: rw
-      value: 126
     writeaftertrig:
-      address: 0x83
-      bitposition: 0
-      bitwidth: 12
+      address: 0x07
+      bitposition: 10
+      bitwidth: 6
       description: ''
       readwrite: rw
-      value: 5
+      value: 2
+  digital_registers: {}
   i2c_registers:
-    i2c_send:
-      address: 0x0F
-      bitposition: 15
+    i2c_en:
+      address: 0x09
+      bitposition: 14
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
-    i2c_words:
+      value: true
+    i2c_send:
       address: 0x0F
-      bitposition: 8
-      bitwidth: 3
+      bitposition: 15
+      bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
     i2c_addr:
       address: 0x0F
       bitposition: 0
       bitwidth: 8
@@ -910,35 +981,42 @@
     i2c_data3:
       address: 0x13
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
+    i2c_words:
+      address: 0x0F
+      bitposition: 8
+      bitwidth: 3
+      description: ''
+      readwrite: rw
+      value: 0
     response0:
       address: 0x28
       bitposition: 0
       bitwidth: 16
       description: ''
-      readwrite: rw
+      readwrite: r
       value: 0
     response1:
       address: 0x29
       bitposition: 0
       bitwidth: 16
       description: ''
-      readwrite: rw
+      readwrite: r
       value: 0
     response2:
       address: 0x2A
       bitposition: 0
       bitwidth: 16
       description: ''
-      readwrite: rw
+      readwrite: r
       value: 0
     response3:
       address: 0x2B
       bitposition: 0
       bitwidth: 16
       description: ''
-      readwrite: rw
+      readwrite: r
       value: 0
```

### Comparing `naluconfigs-10.8.0/src/naluconfigs/data/registers/siread.yml` & `naluconfigs-11.0.0/src/naluconfigs/data/registers/hdsocv1_evalr2.yml`

 * *Files 23% similar despite different names*

```diff
@@ -1,1022 +1,677 @@
-model: siread
+model: hdsocv1_evalr2
 features:
-  adc2mv: false
-  dac_sweep: false
-  pedestals: false
-  threshold_scan: false
-  tia_dac: false
+  adc2mv: true
+  dac_sweep: true
+  ext_dac: true
+  pedestals: true
+  threshold_scan: true
+  tia_dac: true
   timing_calibration: false
-  naludaq_rs: false
+  naludaq_rs: true
 params:
-  chanmask: 3968
+  chanmask: 0x3f
   channels: 32
+  chanshift: 0x0
+  chips:
+    0:
+      !include_chip
+      from: hdsocv1::params
+  clock_file: Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GccClk_156_25TxClk_31_25TxDivClk-Registers.txt
   connections:
     - serial
     - d2xx
+    - udp
+  si5341_address: 0xEE
   default_baud:
-    230400: 53
-  default_baudrate: 230400
-  default_clock: 200000000.0
-  default_divider: 53
-  expected_scalmon: 2500
-  headers: 3
-  last_window_fix_amount: 47
-  numregs: 32
-  pedestals_blocks: 8
+    115200: 826
+  default_baudrate: 115200
+  default_clock: 100000000.0
+  default_divider: 826
+  default_trigger_value: 1
+  trigger:
+    max_vref: 2500
+    min_vref: 0
+    ref_bits: 4
+    val_bits: 8
+    min_counts: 1
+    max_counts: 255
+  threshold_scan:
+    low_ref: 0
+    high_ref: 15
+    start: 1
+    stop: 255
+    stepsize: 5
+    units: mv
+  ext_dac:
+    chip: dac7578
+    max_mv: 2500
+    max_counts: 4095
+    channels:
+      0..31: 1804
+    address_mapping:
+      0..7: 0x49
+      8..15: 0x4A
+      16..23: 0x48
+      24..31: 0x4B
+    channel_mapping:
+      0, 14, 17, 31: 1
+      1, 15, 16, 30: 0
+      2, 12, 19, 29: 3
+      3, 13, 18, 28: 2
+      4, 10, 21, 27: 5
+      5, 11, 20, 26: 4
+      6, 8, 23, 25: 7
+      7, 9, 22, 24: 6
+  headers: 4
+  i2c:
+    max_command_words: 4
+    max_response_words: 4
+  max_numwinds: 400000
+  minimum_firmware_version: 938
+  new_firmware: True
+  numregs: 64
+  pedestals_blocks: 16
+  peripherals:
+    fpga_voltage:
+      chan: 1
+      addr: 0x4C # 7-bit
+    chip_voltage:
+      chan: 4
+      addr: 0x4C # 7-bit
+    board_voltage:
+      chan: vcc
+      addr: 0x4C # 7-bit
+    vadjn_left:
+      chan: 1
+      addr: 0xD8
+      bits: 16
+      gain: 1
+    vadjp_left:
+      chan: 0
+      addr: 0xD8
+      bits: 16
+      gain: 1
+    vadjn_right:
+      chan: 2
+      addr: 0xD8
+      bits: 16
+      gain: 1
+    vadjp_right:
+      chan: 3
+      addr: 0xD8
+      bits: 16
+      gain: 1
   possible_bauds:
-    230400: 53
-    625000: 19
+    115200: 868
+    2000000: 50
+    # 691200: 8
+    # 1041667: 5
   resolution: 12
   samples: 32
-  samplingrate: 1.0
-  stop_word: !!binary |
-    +s4=
+  samplingrate: 1000000000
+  stop_word: FA5A
+  register_stop_word: CAFE
+  tia_dac:
+    max_vref: 2500
+    min_vref: 0
+    ref_bits: 4
+    val_bits: 8
   wait: AE000001
-  wbias: 750
-  windmask: 126
-  windows: 64
+  wbias: 2000
+  windmask: 1022
+  windows: 62
 registers:
   analog_registers:
-    cloadn:
-      address: 0x100
-      bitposition: 10
-      bitwidth: 1
-      description: ''
-      readwrite: w
-      value: 1
-    cloadp:
-      address: 0x100
-      bitposition: 9
-      bitwidth: 1
-      description: ''
-      readwrite: w
-      value: 0
-    cmpbias:
-      address: 0x117
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 1242
-    cmpbias2:
-      address: 0x119
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 846
-    dbbias:
-      address: 0x112
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 1100
-    isel:
-      address: 0x115
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2770
-    itbias:
-      address: 0x11F
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 1000
-    mont_on:
-      address: 0x100
-      bitposition: 8
-      bitwidth: 1
-      description: ''
-      readwrite: w
-      value: 1
-    mont_select:
-      address: 0x100
-      bitposition: 5
-      bitwidth: 3
-      description: ''
-      readwrite: w
-      value: 4
-    ped_00:
-      address: 0x000
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2048
-    ped_01:
-      address: 0x001
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2048
-    ped_02:
-      address: 0x002
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2048
-    ped_03:
-      address: 0x003
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2048
-    ped_04:
-      address: 0x010
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2048
-    ped_05:
-      address: 0x011
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2048
-    ped_06:
-      address: 0x012
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2048
-    ped_07:
-      address: 0x013
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2048
-    ped_08:
-      address: 0x020
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2048
-    ped_09:
-      address: 0x021
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2048
-    ped_10:
-      address: 0x022
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2048
-    ped_11:
-      address: 0x023
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2048
-    ped_12:
-      address: 0x030
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2048
-    ped_13:
-      address: 0x031
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2048
-    ped_14:
-      address: 0x032
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2048
-    ped_15:
-      address: 0x033
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2048
-    ped_16:
-      address: 0x040
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2048
-    ped_17:
-      address: 0x041
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2048
-    ped_18:
-      address: 0x042
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2048
-    ped_19:
-      address: 0x043
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2048
-    ped_20:
-      address: 0x050
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2048
-    ped_21:
-      address: 0x051
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2048
-    ped_22:
-      address: 0x052
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2048
-    ped_23:
-      address: 0x053
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2048
-    ped_24:
-      address: 0x060
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2048
-    ped_25:
-      address: 0x061
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2048
-    ped_26:
-      address: 0x062
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2048
-    ped_27:
-      address: 0x063
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2048
-    ped_28:
-      address: 0x070
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2048
-    ped_29:
-      address: 0x071
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2048
-    ped_30:
-      address: 0x072
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2048
-    ped_31:
-      address: 0x073
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2048
-    pedbias_0:
-      address: 0x004
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 15
-    pedbias_1:
-      address: 0x014
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 15
-    pedbias_2:
-      address: 0x024
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 15
-    pedbias_3:
-      address: 0x034
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 15
-    pedbias_4:
-      address: 0x044
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 15
-    pedbias_5:
-      address: 0x054
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 15
-    pedbias_6:
-      address: 0x064
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 15
-    pedbias_7:
-      address: 0x074
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 15
-    pubias:
-      address: 0x118
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 3112
-    qbias:
-      address: 0x101
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 0
-    qbuff:
-      address: 0x102
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 1062
-    sbbias:
-      address: 0x113
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 1300
-    scvbias:
-      address: 0x11E
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 3000
-    scvstab:
-      address: 0x11D
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 1000
-    sgn:
-      address: 0x100
-      bitposition: 2
-      bitwidth: 1
-      description: ''
-      readwrite: w
-      value: 0
-    spmbias:
-      address: 0x11A
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2048
-    sspin_le:
-      address: 0x108
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 60
-    sspin_te:
-      address: 0x109
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 50
-    sstoutfb:
-      address: 0x107
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 58
-    tbbias:
-      address: 0x11C
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2048
-    term:
-      address: 0x100
-      bitposition: 0
-      bitwidth: 2
-      description: ''
-      readwrite: w
-      value: 3
-    thresh_00:
-      address: 0x005
+    !include_registers
+      from: hdsocv1::registers::analog_registers
+  digital_registers:
+    !include_registers
+      from: hdsocv1::registers::digital_registers
+  control_registers:
+    identifier:
+      address: 0x00
       bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 0
-    thresh_01:
-      address: 0x006
+      bitwidth: 16
+      description: '2-byte chip identifier'
+      readwrite: r
+      value: 19804
+    version:
+      address: 0x01
       bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
+      bitwidth: 16
+      description: 'Firmware version'
+      readwrite: r
       value: 0
-    thresh_02:
-      address: 0x007
+    reg_data0:
+      address: 0x02
       bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
+      bitwidth: 4
+      description: 'Digital command register data bits 19 downto 16'
+      readwrite: r
       value: 0
-    thresh_03:
-      address: 0x008
+    reg_data1:
+      address: 0x03
       bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
+      bitwidth: 16
+      description: 'Digital command register data bits 15 downto 0'
+      readwrite: r
       value: 0
-    thresh_04:
-      address: 0x015
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
+    mode_sel:
+      address: 0x02
+      bitposition: 4
+      bitwidth: 8
+      description: 'Digital command mode data'
+      readwrite: r
       value: 0
-    thresh_05:
-      address: 0x016
+    iomode0:
+      address: 0x04
       bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
+      bitwidth: 1
+      description: 'analog and EN10b8b'
+      readwrite: rw
+      value: 1
+    regclr:
+      address: 0x04
+      bitposition: 1
+      bitwidth: 1
+      description: 'HDSoC INREGCLR pin; resets digital control module, wave fifos, and digital serial rx/tx en'
+      readwrite: rw
       value: 0
-    thresh_06:
-      address: 0x017
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
+    pclk:
+      address: 0x04
+      bitposition: 2
+      bitwidth: 1
+      description: 'HDSoC DEBUG_PCLK pin (analog debug)'
+      readwrite: rw
       value: 0
-    thresh_07:
-      address: 0x018
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
+    nramp:
+      address: 0x04
+      bitposition: 5
+      bitwidth: 1
+      description: 'HDSoC DEBUG_NRAMP pin (analog debug)'
+      readwrite: rw
       value: 0
-    thresh_08:
-      address: 0x025
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
+    iomode1:
+      address: 0x04
+      bitposition: 6
+      bitwidth: 1
+      description: 'ASIC parallel (value = 0) or serial (value = 1) communication'
+      readwrite: rw
       value: 0
-    thresh_09:
-      address: 0x026
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
+    sysrst:
+      address: 0x04
+      bitposition: 9
+      bitwidth: 1
+      description: 'HDSoC SYSRST pin; resets digital control module, wave fifos, and digital serial rx/tx en'
+      readwrite: rw
+      value: 1
+    exttrig:
+      address: 0x04
+      bitposition: 10
+      bitwidth: 1
+      description: 'HDSoC evtTrig_DEBUG_GCCClr pin; external trigger'
+      readwrite: rw
       value: 0
-    thresh_10:
-      address: 0x027
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
+    nrw:
+      address: 0x04
+      bitposition: 11
+      bitwidth: 1
+      description: 'HDSoC R_NW_parllel_DEBUG_RNW pin when in analog debug mode'
+      readwrite: rw
       value: 0
-    thresh_11:
-      address: 0x028
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
+    sel:
+      address: 0x04
+      bitposition: 12
+      bitwidth: 1
+      description: 'HDSoC SEL_parallel pin when in analog debug mode'
+      readwrite: rw
       value: 0
-    thresh_12:
-      address: 0x035
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
+    stopacq:
+      address: 0x04
+      bitposition: 13
+      bitwidth: 1
+      description: 'Stops digital control module from writing packet into wave fifos'
+      readwrite: rw
       value: 0
-    thresh_13:
-      address: 0x036
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
+    t_user:
+      address: 0x04
+      bitposition: 15
+      bitwidth: 1
+      description: 'HDSoC Data_IOT pin when in analog debug mode'
+      readwrite: rw
       value: 0
-    thresh_14:
-      address: 0x037
+    write_address:
+      address: 0x05
       bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
+      bitwidth: 5
+      description: 'HDSoC DEBUG_Write_Address bus'
+      readwrite: rw
       value: 0
-    thresh_15:
-      address: 0x038
+    loadwait:
+      address: 0x07
+      bitposition: 8
+      bitwidth: 4
+      description: 'number of sys_clk_2x cycles to wait before monitoring DATA_VALID from ASIC'
+      readwrite: rw
+      value: 15
+    pclkwidth:
+      address: 0x07
+      bitposition: 12
+      bitwidth: 4
+      description: 'number of sys_clk_2x cycles per 12-bit data read/write operation'
+      readwrite: rw
+      value: 15
+    numwinds:
+      address: 0x08
       bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 0
-    thresh_16:
-      address: 0x045
+      bitwidth: 16
+      description: 'manually-set number of packets to read from serial interface'
+      readwrite: rw
+      value: 1
+    debug_data:
+      address: 0x14
       bitposition: 0
       bitwidth: 12
-      description: ''
-      readwrite: w
+      description: 'HDSoC Data when in analog debug mode'
+      readwrite: rw
       value: 0
-    thresh_17:
-      address: 0x046
+    debug_addr:
+      address: 0x15
       bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
+      bitwidth: 10
+      description: 'HDSoC ADDR when in analog debug mode'
+      readwrite: rw
       value: 0
-    thresh_18:
-      address: 0x047
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
+    idig_rst:
+      address: 0x16
+      bitposition: 9
+      bitwidth: 1
+      description: 'manual digital (control module) reset'
+      readwrite: rw
       value: 0
-    thresh_19:
-      address: 0x048
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
+    wave_fifo_rst:
+      address: 0x16
+      bitposition: 10
+      bitwidth: 1
+      description: 'manual wave fifo reset'
+      readwrite: rw
       value: 0
-    thresh_20:
-      address: 0x055
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
+    clk_sync:
+      address: 0x17
+      bitposition: 10
+      bitwidth: 1
+      description: 'SI5341A Sync'
+      readwrite: rw
       value: 0
-    thresh_21:
-      address: 0x056
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
+    clk_reset:
+      address: 0x17
+      bitposition: 7
+      bitwidth: 1
+      description: 'SI5341A Reset'
+      readwrite: rw
       value: 0
-    thresh_22:
-      address: 0x057
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
+    clk_oeb:
+      address: 0x17
+      bitposition: 6
+      bitwidth: 1
+      description: 'SI5341A OE_n'
+      readwrite: rw
       value: 0
-    thresh_23:
-      address: 0x058
+    clk_i2c_sel:
+      address: 0x17
+      bitposition: 5
+      bitwidth: 1
+      description: 'currently unused, but NaluDaq throws an error'
+      readwrite: rw
+      value: true
+    clk1v8_en:
+      address: 0x17
+      bitposition: 4
+      bitwidth: 1
+      description: 'SI5341A 1.8V Enable'
+      readwrite: rw
+      value: False
+    clk2v5_en:
+      address: 0x17
+      bitposition: 3
+      bitwidth: 1
+      description: 'SI5341A 2.5V Enable'
+      readwrite: rw
+      value: False
+    3v3_i2c_en:
+      address: 0x17
+      bitposition: 2
+      bitwidth: 1
+      description: 'currently unused, but NaluDaq throws an error'
+      readwrite: rw
+      value: true
+    1v2_en:
+      address: 0x17
+      bitposition: 1
+      bitwidth: 1
+      description: 'currently unused, but NaluDaq throws an error'
+      readwrite: rw
+      value: False
+    2v5_en:
+      address: 0x17
       bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
+      bitwidth: 1
+      description: 'HDSoC 2.5V Enable'
+      readwrite: rw
+      value: False
+    ser_rx_neg_pol:
+      address: 0x19
+      bitposition: 1
+      bitwidth: 1
+      description: 'digital serial receive negative polarity flag; currently unused'
+      readwrite: rw
       value: 0
-    thresh_24:
-      address: 0x065
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
+    ser_rx_crc_en:
+      address: 0x19
+      bitposition: 2
+      bitwidth: 1
+      description: 'digital serial receive CRC enable'
+      readwrite: rw
       value: 0
-    thresh_25:
-      address: 0x066
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
+    ser_rx_eof_en:
+      address: 0x19
+      bitposition: 3
+      bitwidth: 1
+      description: 'digital serial receive EOF enable'
+      readwrite: rw
       value: 0
-    thresh_26:
-      address: 0x067
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
+    ser_rx_div:
+      address: 0x19
+      bitposition: 4
+      bitwidth: 4
+      description: 'digital serial receive divider value; currently unused'
+      readwrite: rw
       value: 0
-    thresh_27:
-      address: 0x068
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
+    ser_tx_neg_pol:
+      address: 0x19
+      bitposition: 13
+      bitwidth: 1
+      description: 'digital serial transfer negative polarity flag; currently unused'
+      readwrite: rw
       value: 0
-    thresh_28:
-      address: 0x075
+    pedram_addr:
+      address: 0x1D
       bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
+      bitwidth: 16
+      description: 'currently unused'
+      readwrite: rw
       value: 0
-    thresh_29:
-      address: 0x076
+    pedram_data:
+      address: 0x1E
       bitposition: 0
       bitwidth: 12
-      description: ''
-      readwrite: w
+      description: 'currently unused'
+      readwrite: rw
       value: 0
-    thresh_30:
-      address: 0x077
+    analog_debug_disable:
+      address: 0x1F
       bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
+      bitwidth: 1
+      description: 'manual disable of analog debug functions; analog debug mode enabled when iomode0 = iomode1 = 0'
+      readwrite: rw
       value: 0
-    thresh_31:
-      address: 0x078
+    auto_numwinds_en:
+      address: 0x20
       bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
+      bitwidth: 1
+      description: 'enables automatic numwinds calculation based on digital commands and manual timeout value; currently unused'
+      readwrite: rw
       value: 0
-    trgbias:
-      address: 0x11B
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2419
-    vadjn:
-      address: 0x103
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2360
-    vadjp:
-      address: 0x105
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 768
-    vanbuff:
-      address: 0x104
+    timeout15_0:
+      address: 0x21
       bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 1152
-    vapbuff:
-      address: 0x106
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 1300
-    vdischarge:
-      address: 0x114
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
+      bitwidth: 16
+      description: 'lower 16 bits of timeout value; currently unused'
+      readwrite: rw
       value: 0
-    wbbias:
-      address: 0x116
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 1000
-    wr_addr_incr1_le:
-      address: 0x10A
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 5
-    wr_addr_incr1_te:
-      address: 0x10B
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 25
-    wr_addr_incr2_le:
-      address: 0x10E
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 33
-    wr_addr_incr2_te:
-      address: 0x10F
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 53
-    wrstrb1_le:
-      address: 0x10C
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 20
-    wrstrb1_te:
-      address: 0x10D
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 40
-    wrstrb2_le:
-      address: 0x110
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 56
-    wrstrb2_te:
-      address: 0x111
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 12
-  control_registers:
-    chansela:
-      address: 0x0A
+    timeout31_16:
+      address: 0x22
       bitposition: 0
       bitwidth: 16
-      description: ''
+      description: 'upper 16 bits of timeout value; currently unused'
       readwrite: rw
       value: 0
-    chanselb:
-      address: 0x0B
+    eth_addr_sel:
+      address: 0x28
       bitposition: 0
-      bitwidth: 16
-      description: ''
+      bitwidth: 2
+      description: 'enables manually set destination (bit 0) and source (bit 1) IP addresses'
       readwrite: rw
-      value: 1
-    clk_oe:
-      address: 0x04
+      value: 0
+    eth_port_sel:
+      address: 0x28
       bitposition: 2
-      bitwidth: 1
-      description: ''
+      bitwidth: 2
+      description: 'enables manually set destination (bit 0) and source (bit 1) UDP ports'
       readwrite: rw
-      value: true
-    digrst:
-      address: 0x0C
-      bitposition: 1
+      value: 0
+    tx_mode:
+      address: 0x28
+      bitposition: 4
       bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    fifo_full_level:
-      address: 0x14
-      bitposition: 0
-      bitwidth: 16
-      description: ''
+      description: 'selects ethernet (value = 1) or UART (value = 0) transmission'
       readwrite: rw
       value: 0
-    i2c_switch:
-      address: 0x16
-      bitposition: 3
+    eth_ar_en:
+      address: 0x28
+      bitposition: 5
       bitwidth: 1
-      description: ''
+      description: 'enables auto-response destination IP address; currently unused'
       readwrite: rw
-      value: false
-    loadwait:
-      address: 0x07
+      value: 0
+    eth_dhcp_en:
+      address: 0x28
       bitposition: 6
-      bitwidth: 4
-      description: ''
+      bitwidth: 1
+      description: 'enables DHCP resolution of source IP address; currently unused'
       readwrite: rw
-      value: 15
-    lookback:
-      address: 0x08
-      bitposition: 6
-      bitwidth: 6
-      description: ''
+      value: 0
+    eth_dest_addr15_0:
+      address: 0x29
+      bitposition: 0
+      bitwidth: 16
+      description: 'lower 16 bits of ethernet destination IP address'
       readwrite: rw
       value: 0
-    numwinds:
-      address: 0x08
+    eth_dest_addr31_16:
+      address: 0x2A
       bitposition: 0
-      bitwidth: 6
-      description: ''
+      bitwidth: 16
+      description: 'upper 16 bits of ethernet destination IP address'
       readwrite: rw
-      value: 2
-    ramp:
-      address: 0x06
+      value: 0
+    eth_src_addr15_0:
+      address: 0x2B
       bitposition: 0
-      bitwidth: 11
-      description: ''
+      bitwidth: 16
+      description: 'lower 16 bits of ethernet source IP address'
       readwrite: rw
-      value: 1500
-    regclr:
-      address: 0x04
+      value: 0
+    eth_src_addr31_16:
+      address: 0x2C
       bitposition: 0
-      bitwidth: 1
-      description: ''
+      bitwidth: 16
+      description: 'upper 16 bits of ethernet source IP address'
       readwrite: rw
-      value: false
-    runevs:
-      address: 0x05
+      value: 0
+    eth_dest_port:
+      address: 0x2D
       bitposition: 0
       bitwidth: 16
-      description: ''
+      description: 'UDP destination port'
       readwrite: rw
-      value: 1
-    sstpattern:
-      address: 0x04
-      bitposition: 4
-      bitwidth: 8
-      description: ''
+      value: 0
+    eth_src_port:
+      address: 0x2E
+      bitposition: 0
+      bitwidth: 16
+      description: 'UDP source port'
       readwrite: rw
-      value: 128
-    stopacq:
-      address: 0x08
-      bitposition: 12
+      value: 0
+    pg_2v5:
+      address: 0x46
+      bitposition: 0
       bitwidth: 1
-      description: ''
-      readwrite: rw
+      description: 'PG HDSoC 2v5 input'
+      readwrite: r
       value: 0
-    syncloc:
-      address: 0x0E
+    clk_intr_n:
+      address: 0x47
       bitposition: 0
-      bitwidth: 8
-      description: ''
-      readwrite: rw
+      bitwidth: 1
+      description: 'SI5341A Intr_n input'
+      readwrite: r
       value: 0
-    sysrst:
-      address: 0x0C
+    clk_lol_n:
+      address: 0x47
+      bitposition: 1
+      bitwidth: 1
+      description: 'SI5341A LOL_n input'
+      readwrite: r
+      value: 0
+    fpga_clk_locked:
+      address: 0x59
       bitposition: 0
       bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    v2v5_en:
-      address: 0x04
+      description: 'fpga system clock locked flag'
+      readwrite: r
+      value: 0
+    asic_clk_locked:
+      address: 0x59
       bitposition: 1
       bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    wraddrsync:
-      address: 0x04
+      description: 'SI5341A-generated ASIC clock locked flag'
+      readwrite: r
+      value: 0
+    ser_tx_clk_locked:
+      address: 0x59
+      bitposition: 2
+      bitwidth: 1
+      description: 'digital serial transfer clock locked flag'
+      readwrite: r
+      value: 0
+    rx_en:
+      address: 0x59
       bitposition: 3
       bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    writeaftertrig:
-      address: 0x07
-      bitposition: 10
-      bitwidth: 6
-      description: ''
-      readwrite: rw
-      value: 2
-  digital_registers: {}
+      description: 'digital serial receive enabled'
+      readwrite: r
+      value: 0
+    tx_en:
+      address: 0x59
+      bitposition: 4
+      bitwidth: 1
+      description: 'digital serial transfer enabled'
+      readwrite: r
+      value: 0
+    idly_cnt_val:
+      address: 0x59
+      bitposition: 8
+      bitwidth: 5
+      description: 'input delay count value; currently unused'
+      readwrite: r
+      value: 0
+    dhcp_addr15_0:
+      address: 0x5A
+      bitposition: 0
+      bitwidth: 16
+      description: 'DHCP resolved address bits 15 downto 0'
+      readwrite: r
+      value: 0
+    ch_en15_0:
+      address: 0x5C
+      bitposition: 0
+      bitwidth: 16
+      description: 'enabled channels vector bits 15 downto 0'
+      readwrite: r
+      value: 0
+    ch_en31_16:
+      address: 0x5D
+      bitposition: 0
+      bitwidth: 16
+      description: 'enabled channels vector bits 31 downto 16'
+      readwrite: r
+      value: 0
   i2c_registers:
     i2c_en:
-      address: 0x09
-      bitposition: 14
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: true
-    i2c_send:
       address: 0x0F
-      bitposition: 15
+      bitposition: 14
       bitwidth: 1
-      description: ''
+      description: 'enables I2C output'
       readwrite: rw
-      value: 0
+      value: 1
     i2c_addr:
       address: 0x0F
       bitposition: 0
       bitwidth: 8
-      description: ''
+      description: 'Address of device I2C data is being sent to'
+      readwrite: rw
+      value: 0
+    i2c_words:
+      address: 0x0F
+      bitposition: 8
+      bitwidth: 4
+      description: 'number of 8-bit data words to be sent over I2C'
       readwrite: rw
       value: 0
     i2c_data0:
       address: 0x10
       bitposition: 0
       bitwidth: 16
-      description: ''
+      description: 'I2C data bits 63 downto 48; words read justified to LSB'
       readwrite: rw
       value: 0
     i2c_data1:
       address: 0x11
       bitposition: 0
       bitwidth: 16
-      description: ''
+      description: 'I2C data bits 47 downto 32; words read justified to LSB'
       readwrite: rw
       value: 0
     i2c_data2:
       address: 0x12
       bitposition: 0
       bitwidth: 16
-      description: ''
+      description: 'I2C data bits 31 downto 16; words read justified to LSB'
       readwrite: rw
       value: 0
     i2c_data3:
       address: 0x13
       bitposition: 0
       bitwidth: 16
-      description: ''
-      readwrite: rw
-      value: 0
-    i2c_words:
-      address: 0x0F
-      bitposition: 8
-      bitwidth: 3
-      description: ''
+      description: 'I2C data bits 15 downto 0; words read justified to LSB'
       readwrite: rw
       value: 0
     response0:
-      address: 0x28
+      address: 0x48
       bitposition: 0
       bitwidth: 16
-      description: ''
+      description: 'I2C response bits 63 downto 48; bits received justified to LSb'
       readwrite: r
       value: 0
     response1:
-      address: 0x29
+      address: 0x49
       bitposition: 0
       bitwidth: 16
-      description: ''
+      description: 'I2C response bits 47 downto 32; bits received justified to LSb'
       readwrite: r
       value: 0
     response2:
-      address: 0x2A
+      address: 0x4A
       bitposition: 0
       bitwidth: 16
-      description: ''
+      description: 'I2C response bits 31 downto 16; bits received justified to LSb'
       readwrite: r
       value: 0
     response3:
-      address: 0x2B
+      address: 0x4B
       bitposition: 0
       bitwidth: 16
-      description: ''
+      description: 'I2C response bits 15 downto 0; bits received justified to LSb'
       readwrite: r
       value: 0
```

### Comparing `naluconfigs-10.8.0/src/naluconfigs/data/registers/trbhm.yml` & `naluconfigs-11.0.0/src/naluconfigs/data/registers/upac32.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,64 +1,52 @@
-model: trbhm
+model: upac32
 features:
-  adc2mv: true
+  adc2mv: false
   dac_sweep: false
   ext_dac: true
   pedestals: true
-  threshold_scan: true
+  threshold_scan: false
   tia_dac: false
-  timing_calibration: true
-  naludaq_rs: true
+  timing_calibration: false
+  naludaq_rs: false
 params:
-  chanmask: 0xF000
-  channels: 8
-  chanshift: 10
-  clock_file: Si5341_TRBHM_10GSaps_GCCsstx2_Registers.txt
+  chanmask: 511
+  channels: 32
+  chanshift: 3
   connections:
     - serial
     - d2xx
-    - udp
-  si5341_address: 0xEE
-  timing_hack: true
   default_baud:
-    115200: 868
+    115200: 432
   default_baudrate: 115200
-  default_clock: 100000000.0
-  default_divider: 868
-  default_trigger_value: 1500
-  threshold_scan:
-    min_vref: 0
-    max_vref: 2500
-    start: 500
-    stop: 3500
-    stepsize: 5
-    units: counts
-  expected_scalmon: 2500
+  default_clock: 200000000.0
+  default_divider: 432
+  default_trigger_value: 0
   ext_dac:
-    chip: ltc2620
     max_mv: 1200
-    max_counts: 4095
+    max_counts: 65535
     channels:
-      0..7: 2048
-    chip_mapping: # asic channel: dac chip number
-      0..3: 0
-      4..7: 1
-      cal0: 0
-      cal1: 1
-    channel_mapping: # asic channel: ext. dac channel
-      0, 4: 0
-      1, 5: 2
-      2, 6: 5
-      3, 7: 7
-      cal0: 4
-      cal1: 4
-  headers: 3
-  new_firmware: True
-  numregs: 64
-  pedestals_blocks: 16
+      0,8,16,24: 30000
+    register_mapping:
+      0: dac_vbias00_07_out
+      8: dac_vbias08_15_out
+      16: dac_vbias16_23_out
+      24: dac_vbias24_31_out
+  trigger:
+    triggers_available: 8
+    max_val: 2047
+    min_val: 0
+    default: false
+  num_trigger_channels: 8
+  expected_scalmon: 2500
+  headers: 0
+  last_window_fix_amount: 47
+  lastbits: 0
+  numregs: 32
+  pedestals_blocks: 8
   peripherals:
     current:
       chan: 0
       addr: 0xD0
       bits: 16
       gain: 8
     vadjn:
@@ -68,1297 +56,811 @@
       gain: 1
     vadjp:
       chan: 1
       addr: 0xD8
       bits: 16
       gain: 1
   possible_bauds:
-    115200: 868
-    1000000: 100
-    2000000: 50
-    3000000: 33
-  resolution: 12
-  samples: 64
-  samplingrate: 10.0
-  stop_word: BEEFBEEF
-  register_stop_word: FACE
-  strobe_values_correction: True  # Shift the strobe values on certain boards with swapped internal routing.
-  strobe_correction_keys:
-    - calstrb_le
-    - calstrb_te
-    - wrstrb1_le
-    - wrstrb1_te
-    - wrstrb2_le
-    - wrstrb2_te
-    - wrsync1_le
-    - wrsync1_te
-    - wrsync2_le
-    - wrsync2_te
+    115200: 432
+    460800: 108
+    # 2000000: 25
+    # 3000000: 17
+  resolution: 11
+  samples: 132
+  samplingrate: 9.2
+  stop_word: !!binary |
+    +s4=
   wait: AE000001
-  wbias: 2000
-  windmask: 0x3FE
-  windows: 510
+  wbias: 750
+  windmask: 7
+  windows: 8
 registers:
-  analog_registers:
-    cal:
-      address: 0x01
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 0
-    cal_buff:
-      address: 0x3B
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 3500
-    cal_isel:
-      address: 0x3A
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 0
-    calstrb_le:
-      address: 0x25
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 0
-    calstrb_te:
-      address: 0x26
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 30
-    inp0vcurrn:
-      address: 0x11
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 1604
-    inp0vcurrp:
-      address: 0x13
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2218
-    inp0vgmn:
-      address: 0x0D
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2389
-    inp0vgmp:
-      address: 0x0F
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 1536
-    inp1vcurrn:
-      address: 0x09
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2218
-    inp1vcurrp:
-      address: 0x0B
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 1604
-    inp1vgmn:
-      address: 0x05
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2389
-    inp1vgmp:
-      address: 0x07
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 1536
-    inp2vcurrn:
-      address: 0x2A
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 1604
-    inp2vcurrp:
+  control_registers:
+    avdd_en:
       address: 0x28
       bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2218
-    inp2vgmn:
-      address: 0x2E
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2389
-    inp2vgmp:
-      address: 0x2C
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 1536
-    inp3vcurrn:
-      address: 0x32
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 1604
-    inp3vcurrp:
-      address: 0x30
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2218
-    inp3vgmn:
-      address: 0x36
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2389
-    inp3vgmp:
-      address: 0x34
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 1536
-    isel:
-      address: 0x15
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2730
-    mont1_on:
-      address: 0x00
-      bitposition: 3
       bitwidth: 1
       description: ''
-      readwrite: w
-      value: false
-    mont1_select:
-      address: 0x00
-      bitposition: 4
-      bitwidth: 2
-      description: ''
-      readwrite: w
-      value: 0
-    mont2_on:
-      address: 0x00
-      bitposition: 0
-      bitwidth: 1
-      description: ''
-      readwrite: w
-      value: false
-    mont2_select:
-      address: 0x00
-      bitposition: 1
-      bitwidth: 2
-      description: ''
-      readwrite: w
+      readwrite: rw
       value: 0
-    qbias:
-      address: 0x18
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2048
-    sc0_vbias:
-      address: 0x12
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 1570
-    sc0_vstab:
-      address: 0x10
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 1365
-    sc1_vbias:
-      address: 0x0A
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 1570
-    sc1_vstab:
-      address: 0x08
+    baud_rate_divisor:
+      address: 0x03
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
-      readwrite: w
-      value: 1365
-    sc2_vbias:
-      address: 0x29
-      bitposition: 0
-      bitwidth: 12
+      readwrite: rw
+      value: 108
+    cdce62002_power_down_n:
+      address: 0x13
+      bitposition: 15
+      bitwidth: 16
       description: ''
-      readwrite: w
-      value: 1570
-    sc2_vstab:
-      address: 0x2B
+      readwrite: rw
+      value: 1
+    cdce62002_read_register_0_lsw:
+      address: 0x92
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
-      readwrite: w
-      value: 1365
-    sc3_vbias:
-      address: 0x31
+      readwrite: rw
+      value: 21976
+    cdce62002_read_register_0_msw:
+      address: 0x91
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
-      readwrite: w
-      value: 1570
-    sc3_vstab:
-      address: 0x33
+      readwrite: rw
+      value: 1104
+    cdce62002_read_register_1_lsw:
+      address: 0x94
       bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 1365
-    sgn:
-      address: 0x00
-      bitposition: 10
-      bitwidth: 1
-      description: ''
-      readwrite: w
-      value: false
-    sspin:
-      address: 0x00
-      bitposition: 6
-      bitwidth: 2
-      description: ''
-      readwrite: w
-      value: 3
-    sstin_sel:
-      address: 0x00
-      bitposition: 9
-      bitwidth: 1
+      bitwidth: 16
       description: ''
-      readwrite: w
-      value: true
-    sta_vcomp:
-      address: 0x02
+      readwrite: rw
+      value: 903
+    cdce62002_read_register_1_msw:
+      address: 0x93
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
-      readwrite: w
-      value: 1000
-    vadjn:
-      address: 0x1C
+      readwrite: rw
+      value: 57376
+    cdce62002_read_register_2_lsw:
+      address: 0x96
       bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 1696
-    vadjn_sw:
-      address: 0x00
-      bitposition: 8
-      bitwidth: 1
+      bitwidth: 16
       description: ''
-      readwrite: w
-      value: true
-    vadjp:
-      address: 0x19
+      readwrite: rw
+      value: 24832
+    cdce62002_read_register_2_msw:
+      address: 0x95
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
-      readwrite: w
-      value: 0
-    vlimn:
-      address: 0x1B
+      readwrite: rw
+      value: 14850
+    cdce62002_register_0_lsw_out:
+      address: 0x0C
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
-      readwrite: w
-      value: 0
-    vlimp:
-      address: 0x1A
+      readwrite: rw
+      value: 1104  # same
+    cdce62002_register_0_msw_out:
+      address: 0x0D
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
-      readwrite: w
-      value: 4095
-    trigger_threshold_00:
+      readwrite: rw
+      value: 0x5550  # 21976
+    cdce62002_register_1_lsw_out:
       address: 0x0E
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
-      readwrite: w
-      value: 0
-    trigger_threshold_01:
-      address: 0x06
+      readwrite: rw
+      value: 0xa091  # 57377
+    cdce62002_register_1_msw_out:
+      address: 0x0F
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
-      readwrite: w
-      value: 0
-    trigger_threshold_02:
-      address: 0x2D
-      bitposition: 0
-      bitwidth: 12
+      readwrite: rw
+      value: 0x838d  # 33671
+    cdce62002_write_strobe:
+      address: 0x13
+      bitposition: 11
+      bitwidth: 1
       description: ''
-      readwrite: w
+      readwrite: rw
       value: 0
-    trigger_threshold_03:
-      address: 0x35
+    conversion_wait_count_value:
+      address: 0x14
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
-      readwrite: w
+      readwrite: rw
       value: 0
-    vrmpvbias:
-      address: 0x17
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 1570
-    vtune:
-      address: 0x16
+    dac_rovcp_1_out:
+      address: 0x08
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
-      readwrite: w
-      value: 1365
-    wbias_00:
-      address: 0x0C
+      readwrite: rw
+      value: 256
+    dac_rovcp_2_out:
+      address: 0x09
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
-      readwrite: w
-      value: 2000
-    wbias_01:
+      readwrite: rw
+      value: 256
+    dac_vbias00_07_out:
       address: 0x04
       bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2000
-    wbias_02:
-      address: 0x2F
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2000
-    wbias_03:
-      address: 0x37
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 2000
-    wrstrb1_le:
-      address: 0x1D
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 40
-    wrstrb1_te:
-      address: 0x1E
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 100
-    wrstrb2_le:
-      address: 0x21
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 103
-    wrstrb2_te:
-      address: 0x22
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 36
-    wrsync1_le:
-      address: 0x1F
-      bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
-      readwrite: w
-      value: 0
-    wrsync1_te:
-      address: 0x20
+      readwrite: rw
+      value: 27306
+    dac_vbias08_15_out:
+      address: 0x05
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
-      readwrite: w
-      value: 50
-    wrsync2_le:
-      address: 0x23
+      readwrite: rw
+      value: 27306
+    dac_vbias16_23_out:
+      address: 0x0A
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
-      readwrite: w
-      value: 64
-    wrsync2_te:
-      address: 0x24
+      readwrite: rw
+      value: 27306
+    dac_vbias24_31_out:
+      address: 0x0B
       bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 114
-  control_registers:
-    1v2_en:
-      address: 0x17
-      bitposition: 1
-      bitwidth: 1
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: true
-    2v5_en:
-      address: 0x17
+      value: 27306
+    dac_vreset1_2_out:
+      address: 0x06
       bitposition: 0
-      bitwidth: 1
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: true
-    3v3_i2c_en:
-      address: 0x17
-      bitposition: 2
-      bitwidth: 1
+      value: 11264
+    dac_vreset3_4_out:
+      address: 0x07
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: true
-    8b10b_en:
-      address: 0x19
+      value: 11264
+    dac_write_strobe:
+      address: 0x13
       bitposition: 12
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    amp_en:
-      address: 0x1A
-      bitposition: 0
-      bitwidth: 8
-      description: Enable onboard amplifiers
-      readwrite: rw
-      value: 0
-    addr:
-      address: 0x16
-      bitposition: 0
-      bitwidth: 9
-      description: ''
-      readwrite: rw
-      value: 0
-    addr_user:
-      address: 0x16
-      bitposition: 15
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    chansel:
-      address: 0x06
-      bitposition: 12
-      bitwidth: 4
-      description: ''
-      readwrite: rw
-      value: 15
-    clk1v8_en:
-      address: 0x17
+    diagnostic_read_data:
+      address: 0x10
       bitposition: 4
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: true
-    clk2v5_en:
-      address: 0x17
-      bitposition: 3
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: true
-    clk_fdec:
-      address: 0x17
-      bitposition: 9
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    clk_finc:
-      address: 0x17
-      bitposition: 8
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    clk_i2c_sel:
-      address: 0x17
-      bitposition: 5
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: true
-    clk_oeb:
-      address: 0x17
-      bitposition: 6
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    clk_reset:
-      address: 0x17
-      bitposition: 7
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    clk_sync:
-      address: 0x17
-      bitposition: 10
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    data:
-      address: 0x14
-      bitposition: 0
-      bitwidth: 12
+      bitwidth: 4
       description: ''
       readwrite: rw
       value: 0
-    data_user:
-      address: 0x14
-      bitposition: 15
+    # dll_start:
+    #   address: 0x13
+    #   bitposition: 7
+    #   bitwidth: 1
+    #   description: ''
+    #   readwrite: rw
+    #   value: 0
+    ftdi_cts:
+      address: 0x29
+      bitposition: 2
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: false
-    debug_data:
-      address: 0x15
+      value: 0
+    ftdi_rts_bit_0:
+      address: 0x88
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
-    debug_data_user:
-      address: 0x15
-      bitposition: 15
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    digrst:
-      address: 0x16
-      bitposition: 9
-      bitwidth: 1
+    gpio_pd:
+      address: 0x28
+      bitposition: 2
+      bitwidth: 5
       description: ''
       readwrite: rw
       value: 0
-    digser_rst:
-      address: 0x19
-      bitposition: 13
-      bitwidth: 1
+    gpio_input_header_5:
+      address: 0x85
+      bitposition: 0
+      bitwidth: 8
       description: ''
       readwrite: rw
-      value: 0
-    eth_addr_sel:
-      address: 0x2F
+      value: 255
+    identifier:
+      address: 0x00
       bitposition: 0
-      bitwidth: 2
-      description: 'enables manually set destination (bit 0) and source (bit 1) IP addresses'
-      readwrite: rw
-      value: 0
-    eth_port_sel:
-      address: 0x2F
-      bitposition: 2
-      bitwidth: 2
-      description: 'enables manually set destination (bit 0) and source (bit 1) UDP ports'
+      bitwidth: 16
+      description: ''
       readwrite: rw
-      value: 0
-    tx_mode:
-      address: 0x2F
+      value: 57005
+    # mclk_clock_monitor:
+    #   address: 0x28
+    #   bitposition: 10
+    #   bitwidth: 1
+    #   description: ''
+    #   readwrite: rw
+    #   value: 0
+    optical_trigger_en:
+      address: 0x29
       bitposition: 4
       bitwidth: 1
-      description: 'selects ethernet (value = 1) or UART (value = 0) transmission'
+      description: ''
       readwrite: rw
       value: 0
-    eth_ar_en:
-      address: 0x2F
-      bitposition: 5
-      bitwidth: 1
-      description: 'enables auto-response destination IP address; currently unused'
+    optical_trigger_input_bit_0:
+      address: 0x8A
+      bitposition: 0
+      bitwidth: 16
+      description: ''
       readwrite: rw
       value: 0
-    eth_dhcp_en:
-      address: 0x2F
-      bitposition: 6
+    pd_bias_en:
+      address: 0x29
+      bitposition: 1
       bitwidth: 1
-      description: 'enables DHCP resolution of source IP address; currently unused'
+      description: ''
       readwrite: rw
       value: 0
-    eth_dest_addr15_0:
-      address: 0x30
+    # pll_clock_monitor:
+    #   address: 0x28
+    #   bitposition: 9
+    #   bitwidth: 1
+    #   description: ''
+    #   readwrite: rw
+    #   value: 1
+    # pll_clockout:
+    #   address: 0x28
+    #   bitposition: 11
+    #   bitwidth: 1
+    #   description: ''
+    #   readwrite: rw
+    #   value: 0
+    pll_lock_bit_0:
+      address: 0x86
       bitposition: 0
       bitwidth: 16
-      description: 'lower 16 bits of ethernet destination IP address'
+      description: ''
       readwrite: rw
-      value: 0
-    eth_dest_addr31_16:
-      address: 0x31
+      value: 1
+    psec4a_a_ro_feedback_calculated_value:
+      address: 0xA8
       bitposition: 0
       bitwidth: 16
-      description: 'upper 16 bits of ethernet destination IP address'
+      description: ''
       readwrite: rw
-      value: 0
-    eth_src_addr15_0:
-      address: 0x32
+      value: 247
+    psec4a_a_ro_monitor_clock_count_lsw:
+      address: 0x99
       bitposition: 0
       bitwidth: 16
-      description: 'lower 16 bits of ethernet source IP address'
+      description: ''
       readwrite: rw
       value: 0
-    eth_src_addr31_16:
-      address: 0x33
+    psec4a_a_ro_monitor_clock_count_msw:
+      address: 0x98
       bitposition: 0
       bitwidth: 16
-      description: 'upper 16 bits of ethernet source IP address'
+      description: ''
       readwrite: rw
       value: 0
-    eth_dest_port:
-      address: 0x34
+    psec4a_a_vcdl_monitor_clock_count_lsw:
+      address: 0xA1
       bitposition: 0
       bitwidth: 16
-      description: 'UDP destination port'
+      description: ''
       readwrite: rw
       value: 0
-    eth_src_port:
-      address: 0x35
+    psec4a_a_vcdl_monitor_clock_count_msw:
+      address: 0xA0
       bitposition: 0
       bitwidth: 16
-      description: 'UDP source port'
+      description: ''
       readwrite: rw
       value: 0
-    exttrig:
-      address: 0x04
-      bitposition: 10
-      bitwidth: 1
+    psec4a_b_ro_feedback_calculated_value:
+      address: 0xA9
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: false
-    gccclr:
-      address: 0x04
-      bitposition: 4
-      bitwidth: 1
+      value: 269
+    psec4a_b_ro_monitor_clock_count_lsw:
+      address: 0x9B
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: false
-    idac_update:
-      address: 0x1B
-      bitposition: 14
-      bitwidth: 2
-      description: 'This bit toggled 0-1-0 will start the SPI firmware block that loads the DAC values base on the other registers'
-      readwrite: rw
-      value: 0
-    idac_command:
-      address: 0x1B
-      bitposition: 8
-      bitwidth: 4
-      description: 'Is the command from the data sheet with options on what the LTC2620 does with the data written to it. The data sheet is attached most often this is an "0011'
-      readwrite: rw
-      value: 0
-    idac_address:
-      address: 0x1B
-      bitposition: 4
-      bitwidth: 4
-      description: 'Is the DAC Channel number from the data sheet.'
-      readwrite: rw
       value: 0
-    idac_chip_number:
-      address: 0x1B
+    psec4a_b_ro_monitor_clock_count_msw:
+      address: 0x9A
       bitposition: 0
-      bitwidth: 4
-      description: 'IS the DAC number "0000" or "0001"  there are two DACs in the design.'
+      bitwidth: 16
+      description: ''
       readwrite: rw
       value: 0
-    idac_value:
-      address: 0x1C
+    psec4a_b_vcdl_monitor_clock_count_lsw:
+      address: 0xA3
       bitposition: 0
-      bitwidth: 12
-      description: '12 bit DAC value.'
+      bitwidth: 16
+      description: ''
       readwrite: rw
       value: 0
-    fifo_unload_or_event_en:
-      address: 0x1F
+    psec4a_b_vcdl_monitor_clock_count_msw:
+      address: 0xA2
       bitposition: 0
-      bitwidth: 1
-      description: 'Once data is loaded into the FIFO it will not be sent out to the UART until the end of the current event. Use this mode for capturing sampled data events. '
+      bitwidth: 16
+      description: ''
       readwrite: rw
       value: 0
-    identifier:
-      address: 0x00
+    psec4a_biascomp_out:
+      address: 0x1A
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
-      value: 43714
-    iomode0:
-      address: 0x04
+      value: 512
+    psec4a_biasdllfirst_out:
+      address: 0x1C
       bitposition: 0
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: true
-    iomode1:
-      address: 0x04
-      bitposition: 6
-      bitwidth: 1
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: false
-    leds:
-      address: 0x18
+      value: 256
+    psec4a_biasdlllast_out:
+      address: 0x1B
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0
-    loadwait:
-      address: 0x07
-      bitposition: 8
-      bitwidth: 4
-      description: ''
-      readwrite: rw
-      value: 15
-    nramp:
-      address: 0x04
-      bitposition: 5
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    nrw:
-      address: 0x04
-      bitposition: 11
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    numwinds:
-      address: 0x08
+      value: 256
+    psec4a_biasdlln_out:
+      address: 0x1E
       bitposition: 0
-      bitwidth: 8
-      description: ''
-      readwrite: rw
-      value: 1
-    pclk:
-      address: 0x04
-      bitposition: 2
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    pclkwidth:
-      address: 0x07
-      bitposition: 12
-      bitwidth: 4
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 15
-    ramplen:
-      address: 0x06
+      value: 592
+    psec4a_biasdllp_out:
+      address: 0x1D
       bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: rw
-      value: 2000
-    regclr:
-      address: 0x04
-      bitposition: 1
-      bitwidth: 1
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: false
-    runevs:
-      address: 0x05
+      value: 416
+    psec4a_biasrampbuf_out:
+      address: 0x19
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
-      value: 1
-    rx_en:
-      address: 0x19
+      value: 432
+    psec4a_biasrampslope_out:
+      address: 0x27
       bitposition: 0
-      bitwidth: 1
+      bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
-    rx_num_words:
-      address: 0x19
-      bitposition: 2
-      bitwidth: 6
+    psec4a_biastrign_out:
+      address: 0x17
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0
-    rx_oneshot:
-      address: 0x19
-      bitposition: 1
-      bitwidth: 1
+      value: 0x0200  # 0
+    psec4a_biasxfer_out:
+      address: 0x18
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
+      value: 512
+    psec4a_mclk_source_clock_count_lsw:
+      address: 0x8F
+      bitposition: 0
+      bitwidth: 16
+      description: 'Read-only Debug clock, should be the same as VCDL when read out'
+      readwrite: r
       value: 0
-    rx_speed:
-      address: 0x19
-      bitposition: 8
-      bitwidth: 2
-      description: ''
-      readwrite: rw
+    psec4a_mclk_source_clock_count_msw:
+      address: 0x8E
+      bitposition: 0
+      bitwidth: 16
+      description: 'Read-only Debug clock, should be the same as VCDL when read out'
+      readwrite: r
       value: 0
-    sel:
-      address: 0x04
-      bitposition: 12
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    selany:
-      address: 0x04
-      bitposition: 3
-      bitwidth: 1
+    psec4a_c_ro_feedback_calculated_value:
+      address: 0xAA
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: false
-    slow_sysclk:
-      address: 0x19
-      bitposition: 10
-      bitwidth: 1
+      value: 326
+    psec4a_c_ro_monitor_clock_count_lsw:
+      address: 0x9D
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
-    stopacq:
-      address: 0x04
-      bitposition: 13
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    syncloc:
-      address: 0x09
+    psec4a_c_ro_monitor_clock_count_msw:
+      address: 0x9C
       bitposition: 0
-      bitwidth: 8
+      bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
-    sysclk:
-      address: 0x04
-      bitposition: 8
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    sysrst:
-      address: 0x04
-      bitposition: 9
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: true
-    tx_en:
-      address: 0x19
-      bitposition: 11
-      bitwidth: 1
+    psec4a_c_vcdl_monitor_clock_count_lsw:
+      address: 0xA5
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
-    uart_tx_disable:
-      address: 0x28
-      bitposition: 2
-      bitwidth: 1
-      description: Set to 1 to disable UART output from the board
-      readwrite: rw
-      value: 0
-    windsel:
-      address: 0x07
+    psec4a_c_vcdl_monitor_clock_count_msw:
+      address: 0xA4
       bitposition: 0
-      bitwidth: 8
+      bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
-    wrstrboff:
-      address: 0x04
-      bitposition: 7
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    rxout_pol:
-      address: 0x22
+    psec4a_d_ro_feedback_calculated_value:
+      address: 0xAB
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
-      value: 6400
-    txin_pol:
-      address: 0x23
+      value: 246
+    psec4a_d_ro_monitor_clock_count_lsw:
+      address: 0x9F
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
-      value: 4412
-    ard_header:
-      address: 0x21
-      bitposition: 0
-      bitwidth: 1
-      description: 'Enable AARDVARC debug header.'
-      readwrite: rw
-      value: 1
-    ard_rx_en:
-      address: 0x1D
+      value: 0
+    psec4a_d_ro_monitor_clock_count_msw:
+      address: 0x9E
       bitposition: 0
       bitwidth: 16
-      description: 'TR-BHM ASIC Rx Enable register 29dec. Bit 0 and 1 enable transmitting data to ASICs. Need to set these bits to send data to the ASICs'
+      description: ''
       readwrite: rw
-      value: 3
-    ard_tx_en:
-      address: 0x1E
+      value: 0
+    psec4a_d_vcdl_monitor_clock_count_lsw:
+      address: 0xA7
       bitposition: 0
       bitwidth: 16
-      description: 'TR-BHM ASIC Tx Enable register 30dec. Bit 0 and 1 enable receiving data from ASICs. Need to set these bits to get data back from the ASICs'
+      description: ''
       readwrite: rw
-      value: 3
-    ard_clk_select_0:
-      address: 0x24
+      value: 0
+    psec4a_d_vcdl_monitor_clock_count_msw:
+      address: 0xA6
       bitposition: 0
-      bitwidth: 1
-      description: 'TR-BHM chip 0 phase select\n 00: 0 deg\n 01: 90 deg\n 10: 180 deg\n 11: 270 deg'
+      bitwidth: 16
+      description: ''
       readwrite: rw
       value: 0
-    ard_clk_select_1:
-      address: 0x25
-      bitposition: 0
+    # psec4a_mode:
+    #   address: 0x13
+    #   bitposition: 5
+    #   bitwidth: 2
+    #   description: ''
+    #   readwrite: rw
+    #   value: 0
+    xref_address_mode:
+      address: 0x13
+      bitposition: 5
       bitwidth: 1
-      description: 'TR-BHM chip 1 phase select\n 00: 0 deg\n 01: 90 deg\n 10: 180 deg\n 11: 270 deg'
+      description: ''
       readwrite: rw
       value: 0
-  digital_registers:
-    bank:
-      address: 0x1D
+    psec4a_rovcp:
+      address: 0x16
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0
-    banknum:
-      address: 0x9D
+      value: 300
+    psec4a_status:
+      address: 0x84
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0
-    chipid:
-      address: 0x89
+      value: 4852
+    psec4a_trigthresh0_out:
+      address: 0x1F
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 2730
-    donetimeoutn:
-      address: 0xA0
+      value: 0  # 0
+    psec4a_trigthresh1_out:
+      address: 0x20
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0
-    convertresetwait:
-      address: 0x84
+      value: 0  # 0
+    psec4a_trigthresh2_out:
+      address: 0x21
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 1
-    enabletestpatt:
-      address: 0x88
+      value: 0  # 0
+    psec4a_trigthresh3_out:
+      address: 0x22
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0
-    excludechannelmask:
-      address: 0x96
+      value: 0  # 0
+    psec4a_trigthresh4_out:
+      address: 0x23
       bitposition: 0
-      bitwidth: 4
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0
-    loadwait:
-      address: 0x8B
+      value: 0  # 0
+    psec4a_trigthresh5_out:
+      address: 0x24
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0
-    miscreg:
-      address: 0x8D
+      value: 0  # 0
+    psec4a_trigthresh6_out:
+      address: 0x25
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 2
-    pclkwidth:
-      address: 0x8C
+      value: 0  # 0
+    psec4a_trigthresh7_out:
+      address: 0x26
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0
-    readoutchannels:
-      address: 0x87
-      bitposition: 0
-      bitwidth: 12
+      value: 0  # 0
+    reread_data:
+      address: 0x10
+      bitposition: 9
+      bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    readoutlookback:
-      address: 0x85
+    ring_oscillator_feedback_target_value_lsw:
+      address: 0x11
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 18
-    readoutwindows:
-      address: 0x86
+      value: 29529
+    ring_oscillator_feedback_target_value_msw:
+      address: 0x12
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 10
-    regclr:
-      address: 0x8A
+      value: 7
+    ro_feedback_enable:
+      address: 0x13
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
-    scal0:
-      address: 0x00
-      bitposition: 0
-      bitwidth: 12
+      value: 1
+    ro_monitor_reset:
+      address: 0x29
+      bitposition: 3
+      bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    scal1:
-      address: 0x01
-      bitposition: 0
-      bitwidth: 12
-      description: ''
+    self_trigger_or_enable:
+      address: 0x13
+      bitposition: 6
+      bitwidth: 1
+      description: 'Enable Self Trigger OR function in PSEC4A'
       readwrite: rw
-      value: 0
-    scal2:
-      address: 0x02
-      bitposition: 0
-      bitwidth: 12
+      value: 1
+    serial_data_select:
+      address: 0x28
+      bitposition: 12
+      bitwidth: 4
       description: ''
       readwrite: rw
       value: 0
-    scal3:
-      address: 0x03
+    serial_write_strobe:
+      address: 0x10
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    scalhigh:
-      address: 0x40
-      bitposition: 0
-      bitwidth: 12
+    software_trigger:
+      address: 0x13
+      bitposition: 4
+      bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    scalmon:
-      address: 0x08
-      bitposition: 0
-      bitwidth: 12
+    speed_select:
+      address: 0x13
+      bitposition: 3
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
-    scs_misc:
-      address: 0x9E
+      value: 1
+    # system_clock_monitor:
+    #   address: 0x28
+    #   bitposition: 8
+    #   bitwidth: 1
+    #   description: ''
+    #   readwrite: rw
+    #   value: 1
+    trig_out1:
+      address: 0x90
       bitposition: 0
-      bitwidth: 12
-      description: 'Controls the cap/comparator variants in the test structure'
+      bitwidth: 4
+      description: 'DCBA chiporder'
       readwrite: rw
       value: 0
-    testpatin:
-      address: 0x0A
-      bitposition: 0
-      bitwidth: 12
-      description: ''
+    trigger_mask_enable:
+      address: 0x29
+      bitposition: 8
+      bitwidth: 8
+      description: 'Trigger mask where each bit is a corresponding chip'
       readwrite: rw
-      value: 0
-    test_dline:
-      address: 0x9F
-      bitposition: 0
-      bitwidth: 12
-      description: ''
+      value: 255  # '11111111'
+    trigger_mode:
+      address: 0x29
+      bitposition: 5
+      bitwidth: 2
+      description: '<html><head/><body><p>Set the triggermode:<br/>
+        00: Software Trigger, the default.<br/>
+        01: Auto Trigger, 2Hz auto trigger rate.<br/>
+        10: External Trigger, trigger on trig in.<br/>
+        11: Self Trigger, trigger on signal levels.
+        </p></body></html>'
       readwrite: rw
       value: 0
-    wraddrjunk:
-      address: 0x82
-      bitposition: 0
-      bitwidth: 12
+    trigger_reset:
+      address: 0x13
+      bitposition: 13
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 255
-    wraddrstart:
-      address: 0x80
-      bitposition: 0
-      bitwidth: 12
+      value: 0
+    # trigger_scaler:
+    #   address: 0x97
+    #   bitposition: 0
+    #   bitwidth: 8
+    #   description: ''
+    #   readwrite: rw
+    #   value: 0
+    trigger_sign:
+      address: 0x13
+      bitposition: 1
+      bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    wraddrstop:
+    uart_status:
       address: 0x81
       bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: rw
-      value: 254
-    writeaftertrig:
-      address: 0x83
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: rw
-      value: 5
-    waitread:
-      address: 0x8E
-      bitposition: 0
-      bitwidth: 3
+      bitwidth: 8
       description: ''
       readwrite: rw
-      value: 1
-    txspeed:
-      address: 0x94
-      bitposition: 0
-      bitwidth: 2
+      value: 84
+    uart_handshake_en_out:
+      address: 0x10
+      bitposition: 8
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 2
-    pllmisc:
-      address: 0x93
+      value: false
+    version_number:
+      address: 0x80
       bitposition: 0
-      bitwidth: 6
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0
-  i2c_registers:
-    i2c_en:
-      address: 0x0F
-      bitposition: 14
+      value: 4101
+    wave_fifo_reset:
+      address: 0x10
+      bitposition: 1
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: true
-    i2c_send:
-      address: 0x0F
-      bitposition: 15
+      value: 0
+    xfer_reset:
+      address: 0x13
+      bitposition: 2
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
-    i2c_addr:
-      address: 0x0F
+      value: 1
+    ltc2992_p1_in_23_to_16:
+      address: 0xAC
       bitposition: 0
-      bitwidth: 8
-      description: ''
-      readwrite: rw
+      bitwidth: 16
+      description: 'Top bits for PDBIAS Power readout from the LTC2992 sensor chip'
+      readwrite: r
       value: 0
-    i2c_data0:
-      address: 0x10
+    ltc2992_p1_in_15_to_0:
+      address: 0xAD
       bitposition: 0
       bitwidth: 16
-      description: ''
-      readwrite: rw
+      description: 'Bottom bits for PDBIAS Power readout from the LTC2992 sensor chip'
+      readwrite: r
       value: 0
-    i2c_data1:
-      address: 0x11
+    ltc2992_i1_in:
+      address: 0xAE
       bitposition: 0
       bitwidth: 16
-      description: ''
-      readwrite: rw
+      description: 'PDBIAS current readout from the LTC2992 sensor chip'
+      readwrite: r
       value: 0
-    i2c_data2:
-      address: 0x12
+    ltc2992_s1_in:
+      address: 0xAF
       bitposition: 0
       bitwidth: 16
-      description: ''
-      readwrite: rw
+      description: 'PDBIAS Voltage readout from the LTC2992 sensor chip'
+      readwrite: r
       value: 0
-    i2c_data3:
-      address: 0x13
+    ltc2992_g1_in:
+      address: 0xB0
       bitposition: 0
       bitwidth: 16
-      description: ''
-      readwrite: rw
-      value: 0
-    i2c_words:
-      address: 0x0F
-      bitposition: 8
-      bitwidth: 3
-      description: ''
-      readwrite: rw
+      description: 'Bottom bits for LTC2992 sensor chip'
+      readwrite: r
       value: 0
-    response0:
-      address: 0x48
+    ltc2992_p2_in_23_to_16:
+      address: 0xB1
       bitposition: 0
       bitwidth: 16
-      description: ''
+      description: 'Top bits for 1.2V rail power readout from the LTC2992 sensor chip'
       readwrite: r
       value: 0
-    response1:
-      address: 0x49
+    ltc2992_p2_in_15_to_0:
+      address: 0xB2
       bitposition: 0
       bitwidth: 16
-      description: ''
+      description: 'Top bits for 1.2V rail power readout from the LTC2992 sensor chip'
       readwrite: r
       value: 0
-    response2:
-      address: 0x4A
+    ltc2992_i2_in:
+      address: 0xB3
       bitposition: 0
       bitwidth: 16
-      description: ''
+      description: '1.2V rail current readout from the LTC2992 sensor chip'
       readwrite: r
       value: 0
-    response3:
-      address: 0x4B
+    ltc2992_s2_in:
+      address: 0xB4
       bitposition: 0
       bitwidth: 16
-      description: ''
+      description: '1.2V rail voltage readout from the LTC2992 sensor chip'
       readwrite: r
       value: 0
```

### Comparing `naluconfigs-10.8.0/src/naluconfigs/data/registers/udc16.yml` & `naluconfigs-11.0.0/src/naluconfigs/data/registers/upaci.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,55 +1,31 @@
-model: udc16
-features:
-  adc2mv: false
-  dac_sweep: true
-  ext_dac: true
-  pedestals: true
-  threshold_scan: false
-  tia_dac: false
-  timing_calibration: false
-  naludaq_rs: true
+model: upaci
 params:
-  chanmask: 0xFF00
-  channels: 16
-  chanshift: 8
-  clock_file: Si5341-RevD-UDC_78_125SlowClk_78_125IntermediateClk_312_5FastClk-Registers.txt
+  chanmask: 511
+  channels: 32
+  chanshift: 3
   connections:
     - serial
     - d2xx
-    - udp
-  si5341_address: 0xEE
   default_baud:
-    2000000: 50
-  default_baudrate: 2000000
+    115200: 434
+  default_baudrate: 115200
   default_clock: 200000000.0
-  default_divider: 50
+  default_divider: 434
   default_trigger_value: 0
-  intamp_bias_mode_chan0_7: 'c'
-  intamp_bias_mode_chan8_15: 'c'
   ext_dac:
-    chip: dac7578
-    max_mv: 1250
-    max_counts: 3930
-    min_counts: 0
+    max_mv: 1200
+    max_counts: 65535
     channels:
-      0..15: 2000
-    address_mapping:
-      0..7: 0x4B
-      8..15: 0x48
-    channel_mapping:
-      0, 08: 0
-      1, 09: 1
-      2, 10: 2
-      3, 11: 3
-      4, 12: 4
-      5, 13: 5
-      6, 14: 6
-      7, 15: 7
+      0: 30000
+      8: 30000
+      16: 30000
+      24: 30000
   trigger:
+    triggers_available: 8
     max_val: 2047
     min_val: 0
     default: false
   num_trigger_channels: 8
   expected_scalmon: 2500
   headers: 0
   last_window_fix_amount: 47
@@ -59,981 +35,756 @@
   peripherals:
     current:
       chan: 0
       addr: 0xD0
       bits: 16
       gain: 8
     vadjn:
-      chan: 1
+      chan: 0
       addr: 0xD8
       bits: 16
       gain: 1
     vadjp:
-      chan: 0
+      chan: 1
       addr: 0xD8
       bits: 16
       gain: 1
   possible_bauds:
-    2000000: 50
-  resolution: 10
-  samples: 64
+    115200: 434
+    2000000: 25
+  resolution: 11
+  samples: 132
   samplingrate: 9.2
-  stop_word: CAFE
-  strobe_values_correction: True  # Shift the strobe values on certain boards with swapped internal routing.
-  strobe_correction_keys:
-    - digsync_le
-    - digsync_te
-    - wrstrb1_le
-    - wrstrb1_te
-    - wrstrb2_le
-    - wrstrb2_te
-    - wrsync1_le
-    - wrsync1_te
-    - wrsync2_le
-    - wrsync2_te
+  stop_word: !!binary |
+    +s4=
   wait: AE000001
   wbias: 750
-  windmask: 0x00FF
-  windows: 64
+  windmask: 7
+  windows: 8
 registers:
   control_registers:
-    identifier:
-      address: 0x00
+    avdd_en:
+      address: 0x28
       bitposition: 0
-      bitwidth: 16
-      description: 'Unique board identifier'
+      bitwidth: 1
+      description: ''
       readwrite: rw
-      value: 0x4D5C
-    version:
-      address: 0x01
+      value: 0
+    baud_rate_divisor:
+      address: 0x03
       bitposition: 0
       bitwidth: 16
-      description: 'Current firmware version'
+      description: ''
       readwrite: rw
-      value: 0
-    data_iot:
-      address: 0x04
+      value: 108
+    cdce62002_power_down_n:
+      address: 0x13
       bitposition: 15
-      bitwidth: 1
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0
-    stopacq:
-      address: 0x04
-      bitposition: 13
-      bitwidth: 1
+      value: 1
+    cdce62002_read_register_0_lsw:
+      address: 0x92
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0
-    sel:
-      address: 0x04
-      bitposition: 12
-      bitwidth: 1
+      value: 21976
+    cdce62002_read_register_0_msw:
+      address: 0x91
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0
-    nrw:
-      address: 0x04
-      bitposition: 11
-      bitwidth: 1
+      value: 1104
+    cdce62002_read_register_1_lsw:
+      address: 0x94
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0
-    exttrig:
-      address: 0x04
-      bitposition: 10
-      bitwidth: 1
+      value: 903
+    cdce62002_read_register_1_msw:
+      address: 0x93
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0
-    sysrst:
-      address: 0x04
-      bitposition: 9
-      bitwidth: 1
+      value: 57376
+    cdce62002_read_register_2_lsw:
+      address: 0x96
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0
-    iomode1:
-      address: 0x04
-      bitposition: 6
-      bitwidth: 1
+      value: 24832
+    cdce62002_read_register_2_msw:
+      address: 0x95
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 1
-    nramp:
-      address: 0x04
-      bitposition: 5
-      bitwidth: 1
+      value: 14850
+    cdce62002_register_0_lsw_out:
+      address: 0x0C
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0
-    gccclr:
-      address: 0x04
-      bitposition: 4
-      bitwidth: 1
+      value: 1104  # same
+    cdce62002_register_0_msw_out:
+      address: 0x0D
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0
-    selany:
-      address: 0x04
-      bitposition: 3
-      bitwidth: 1
+      value: 0x5550  # 21976
+    cdce62002_register_1_lsw_out:
+      address: 0x0E
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0
-    pclk:
-      address: 0x04
-      bitposition: 2
-      bitwidth: 1
+      value: 0xa091  # 57377
+    cdce62002_register_1_msw_out:
+      address: 0x0F
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0
-    regclr:
-      address: 0x04
-      bitposition: 1
+      value: 0x838d  # 33671
+    cdce62002_write_strobe:
+      address: 0x13
+      bitposition: 11
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    iomode0:
-      address: 0x04
+    conversion_wait_count_value:
+      address: 0x14
       bitposition: 0
-      bitwidth: 1
+      bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
-    pclkwidth:
-      address: 0x07
-      bitposition: 8
-      bitwidth: 4
-      description: ''
-      readwrite: rw
-      value: 15
-    loadwait:
-      address: 0x07
-      bitposition: 12
-      bitwidth: 4
+    dac_rovcp_1_out:
+      address: 0x08
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 15
-    udc_arm:
+      value: 256
+    dac_rovcp_2_out:
       address: 0x09
       bitposition: 0
-      bitwidth: 1
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0
-    reread_data:
-      address: 0x0C
+      value: 256
+    dac_vbias00_07_out:
+      address: 0x04
       bitposition: 0
-      bitwidth: 1
-      description: 'Ask the FPGA to send whatever event is in the output buffer'
+      bitwidth: 16
+      description: ''
       readwrite: rw
-      value: 0
-    debug_data_to_write:
-      address: 0x14
+      value: 27306
+    dac_vbias08_15_out:
+      address: 0x05
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0
-    debug_addr:
-      address: 0x15
+      value: 27306
+    dac_vbias16_23_out:
+      address: 0x0A
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0
-    wave_fifo_reset:
-      address: 0x16
-      bitposition: 10
-      bitwidth: 1
-      description: 'Reset the waveform FIFO, effectively flushing any data in the output FIFO'
-      readwrite: rw
-      value: 0
-    digrst:
-      address: 0x16
-      bitposition: 9
-      bitwidth: 1
-      description: 'Toggle the digital reset pin, resets the ASIC.'
+      value: 27306
+    dac_vbias24_31_out:
+      address: 0x0B
+      bitposition: 0
+      bitwidth: 16
+      description: ''
       readwrite: rw
-      value: 0
-    2v5_en:
-      address: 0x17
+      value: 27306
+    dac_vreset1_2_out:
+      address: 0x06
       bitposition: 0
-      bitwidth: 1
-      description: 'Enable the 2.5V rail'
+      bitwidth: 16
+      description: ''
       readwrite: rw
-      value: 0
-    1v2_en:
-      address: 0x17
-      bitposition: 1
-      bitwidth: 1
-      description: 'Enable the 1.2V rail'
+      value: 11264
+    dac_vreset3_4_out:
+      address: 0x07
+      bitposition: 0
+      bitwidth: 16
+      description: ''
       readwrite: rw
-      value: 0
-    clk2v5_en:
-      address: 0x17
-      bitposition: 3
+      value: 11264
+    dac_write_strobe:
+      address: 0x13
+      bitposition: 12
       bitwidth: 1
-      description: 'Enable the clock specific 2.5V rail.'
+      description: ''
       readwrite: rw
       value: 0
-    clk1v8_en:
-      address: 0x17
+    diagnostic_read_data:
+      address: 0x10
       bitposition: 4
-      bitwidth: 1
-      description: 'Enable the clock specific 1.8V rail.'
+      bitwidth: 4
+      description: ''
       readwrite: rw
       value: 0
-    clk_oeb:
-      address: 0x17
-      bitposition: 6
+    # dll_start:
+    #   address: 0x13
+    #   bitposition: 7
+    #   bitwidth: 1
+    #   description: ''
+    #   readwrite: rw
+    #   value: 0
+    ftdi_cts:
+      address: 0x29
+      bitposition: 2
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    clk_reset:
-      address: 0x17
-      bitposition: 7
-      bitwidth: 1
+    ftdi_rts_bit_0:
+      address: 0x88
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
-    clk_sync:
-      address: 0x17
-      bitposition: 10
-      bitwidth: 1
+    gpio_pd:
+      address: 0x28
+      bitposition: 2
+      bitwidth: 5
       description: ''
       readwrite: rw
       value: 0
-    tx_packet_marker:
-      address: 0x18
+    gpio_input_header_5:
+      address: 0x85
       bitposition: 0
-      bitwidth: 6
+      bitwidth: 8
       description: ''
       readwrite: rw
-      value: 0
-    rx_enable:
-      address: 0x19
+      value: 255
+    identifier:
+      address: 0x00
       bitposition: 0
-      bitwidth: 1
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0
-    rx_reg_polarity:
-      address: 0x19
-      bitposition: 1
+      value: 57005
+    # mclk_clock_monitor:
+    #   address: 0x28
+    #   bitposition: 10
+    #   bitwidth: 1
+    #   description: ''
+    #   readwrite: rw
+    #   value: 0
+    optical_trigger_en:
+      address: 0x29
+      bitposition: 4
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    rx_divider:
-      address: 0x19
-      bitposition: 4
-      bitwidth: 4
+    optical_trigger_input_bit_0:
+      address: 0x8A
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
-    tx_enable:
-      address: 0x19
-      bitposition: 12
+    pd_bias_en:
+      address: 0x29
+      bitposition: 1
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    tx_reg_polarity:
-      address: 0x19
-      bitposition: 13
-      bitwidth: 1
+    # pll_clock_monitor:
+    #   address: 0x28
+    #   bitposition: 9
+    #   bitwidth: 1
+    #   description: ''
+    #   readwrite: rw
+    #   value: 1
+    # pll_clockout:
+    #   address: 0x28
+    #   bitposition: 11
+    #   bitwidth: 1
+    #   description: ''
+    #   readwrite: rw
+    #   value: 0
+    pll_lock_bit_0:
+      address: 0x86
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0
-    tx_10_bit_data:
-      address: 0x19
-      bitposition: 14
-      bitwidth: 1
+      value: 1
+    psec4a_a_ro_feedback_calculated_value:
+      address: 0xA8
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0
-    analog_debug_en:
-      address: 0x1F
+      value: 247
+    psec4a_a_ro_monitor_clock_count_lsw:
+      address: 0x99
       bitposition: 0
-      bitwidth: 1
-      description: 'Enable analog debug mode, bypassing the digital side of the chip. Allows the user to communicate directly with the analog side.'
+      bitwidth: 16
+      description: ''
       readwrite: rw
       value: 0
-    v1v2_power_good:
-      address: 0x46
-      bitposition: 0
-      bitwidth: 1
-      description: 'Read-Only status register'
-      readwrite: r
-      value: 0
-    temperature_event:
-      address: 0x46
-      bitposition: 1
-      bitwidth: 1
-      description: 'Read-Only status register'
-      readwrite: r
-      value: 0
-    udc_mon_in:
-      address: 0x47
-      bitposition: 0
-      bitwidth: 1
-      description: 'Read-Only status register'
-      readwrite: r
-      value: 0
-    i2c_dataout_genwr_3:
-      address: 0x48
+    psec4a_a_ro_monitor_clock_count_msw:
+      address: 0x98
       bitposition: 0
       bitwidth: 16
-      description: 'Read-Only status register'
-      readwrite: r
+      description: ''
+      readwrite: rw
       value: 0
-    i2c_dataout_genwr_2:
-      address: 0x49
+    psec4a_a_vcdl_monitor_clock_count_lsw:
+      address: 0xA1
       bitposition: 0
       bitwidth: 16
-      description: 'Read-Only status register'
-      readwrite: r
+      description: ''
+      readwrite: rw
       value: 0
-    i2c_dataout_genwr_1:
-      address: 0x4A
+    psec4a_a_vcdl_monitor_clock_count_msw:
+      address: 0xA0
       bitposition: 0
       bitwidth: 16
-      description: 'Read-Only status register'
-      readwrite: r
+      description: ''
+      readwrite: rw
       value: 0
-    i2c_dataout_genwr_0:
-      address: 0x4B
+    psec4a_b_ro_feedback_calculated_value:
+      address: 0xA9
       bitposition: 0
       bitwidth: 16
-      description: 'Read-Only status register'
-      readwrite: r
-      value: 0
-    udc_triggerout_in:
-      address: 0x4C
-      bitposition: 2
-      bitwidth: 1
-      description: 'Read-Only status register'
-      readwrite: r
-      value: 0
-    si5341a_intr_n_in:
-      address: 0x4C
-      bitposition: 1
-      bitwidth: 1
-      description: 'Read-Only status register'
-      readwrite: r
-      value: 0
-    si5341a_lol_n_in:
-      address: 0x4C
-      bitposition: 0
-      bitwidth: 1
-      description: 'Read-Only status register'
-      readwrite: r
-      value: 0
-    system_clock_locked:
-      address: 0x59
+      description: ''
+      readwrite: rw
+      value: 269
+    psec4a_b_ro_monitor_clock_count_lsw:
+      address: 0x9B
       bitposition: 0
-      bitwidth: 1
-      description: 'Read-Only status register'
-      readwrite: r
-      value: 0
-    sys_clock_locked:
-      address: 0x59
-      bitposition: 1
-      bitwidth: 1
-      description: 'Read-Only status register'
-      readwrite: r
-      value: 0
-    idigser_tx_idle_locked:
-      address: 0x59
-      bitposition: 2
-      bitwidth: 1
-      description: 'Read-Only status register'
-      readwrite: r
-      value: 0
-    udc_busy_locked_in:
-      address: 0x59
-      bitposition: 3
-      bitwidth: 1
-      description: 'Read-Only status register'
-      readwrite: r
+      bitwidth: 16
+      description: ''
+      readwrite: rw
       value: 0
-  digital_registers:
-    scalmon:
-      address: 0x08
+    psec4a_b_ro_monitor_clock_count_msw:
+      address: 0x9A
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
-      readwrite: r
+      readwrite: rw
       value: 0
-    scalmon2:
-      address: 0x0B
+    psec4a_b_vcdl_monitor_clock_count_lsw:
+      address: 0xA3
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
-      readwrite: r
+      readwrite: rw
       value: 0
-    start_window_addr:
-      address: 0x0F
+    psec4a_b_vcdl_monitor_clock_count_msw:
+      address: 0xA2
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
-      readwrite: r
+      readwrite: rw
       value: 0
-    high_addr:
-      address: 0x40
+    psec4a_biascomp_out:
+      address: 0x1A
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
-      readwrite: r
-      value: 0
-    writeaftertrig:
-      address: 0x83
+      readwrite: rw
+      value: 512
+    psec4a_biasdllfirst_out:
+      address: 0x1C
       bitposition: 0
-      bitwidth: 12
-      description: 'Clock cycles to continue writing after trigger, translates to windows to write after trig event.'
+      bitwidth: 16
+      description: ''
       readwrite: rw
-      value: 0
-    convert_reset_wait:
-      address: 0x84
+      value: 256
+    psec4a_biasdlllast_out:
+      address: 0x1B
       bitposition: 0
-      bitwidth: 8
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 1
-    enable_testpattern:
-      address: 0x88
+      value: 256
+    psec4a_biasdlln_out:
+      address: 0x1E
       bitposition: 0
-      bitwidth: 1
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0
-    chip_id:
-      address: 0x89
+      value: 592
+    psec4a_biasdllp_out:
+      address: 0x1D
       bitposition: 0
-      bitwidth: 12
-      description: 'Identifier for the chip. Lowest 6-bits will be the identifier in the packet header, for multichip systems.'
+      bitwidth: 16
+      description: ''
       readwrite: rw
-      value: 0
-    regclr:
-      address: 0x8A
+      value: 416
+    psec4a_biasrampbuf_out:
+      address: 0x19
       bitposition: 0
-      bitwidth: 1
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0
-    loadwait:
-      address: 0x8B
+      value: 432
+    psec4a_biasrampslope_out:
+      address: 0x27
       bitposition: 0
-      bitwidth: 6
+      bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
-    pclkwidth:
-      address: 0x8C
+    psec4a_biastrign_out:
+      address: 0x17
       bitposition: 0
-      bitwidth: 6
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 2
-    miscreg:
-      address: 0x8D
-      bitposition: 4
-      bitwidth: 2
+      value: 0x0200  # 0
+    psec4a_biasxfer_out:
+      address: 0x18
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
+      value: 512
+    psec4a_mclk_source_clock_count_lsw:
+      address: 0x8F
+      bitposition: 0
+      bitwidth: 16
+      description: 'Read-only Debug clock, should be the same as VCDL when read out'
+      readwrite: r
       value: 0
-    waitread:
+    psec4a_mclk_source_clock_count_msw:
       address: 0x8E
       bitposition: 0
-      bitwidth: 4
-      description: ''
-      readwrite: rw
-      value: 0x00F
-    waitaddr:
-      address: 0x8F
+      bitwidth: 16
+      description: 'Read-only Debug clock, should be the same as VCDL when read out'
+      readwrite: r
+      value: 0
+    psec4a_c_ro_feedback_calculated_value:
+      address: 0xAA
       bitposition: 0
-      bitwidth: 4
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0xF
-    triggerchannelmask_lo:
-      address: 0x90
+      value: 326
+    psec4a_c_ro_monitor_clock_count_lsw:
+      address: 0x9D
       bitposition: 0
-      bitwidth: 8
+      bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
-    writedelay:
-      address: 0x91
+    psec4a_c_ro_monitor_clock_count_msw:
+      address: 0x9C
       bitposition: 0
-      bitwidth: 4
+      bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
-    triggerchannelmask_hi:
-      address: 0x92
+    psec4a_c_vcdl_monitor_clock_count_lsw:
+      address: 0xA5
       bitposition: 0
-      bitwidth: 8
+      bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
-    txspeed:
-      address: 0x94
+    psec4a_c_vcdl_monitor_clock_count_msw:
+      address: 0xA4
       bitposition: 0
-      bitwidth: 2
+      bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
-    excludechannelmask_lo:
-      address: 0x96
+    psec4a_d_ro_feedback_calculated_value:
+      address: 0xAB
       bitposition: 0
-      bitwidth: 8
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0
-    excludechannelmask_hi:
-      address: 0x97
+      value: 246
+    psec4a_d_ro_monitor_clock_count_lsw:
+      address: 0x9F
       bitposition: 0
-      bitwidth: 8
+      bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
-    done_timeout_n:
-      address: 0xA0
+    psec4a_d_ro_monitor_clock_count_msw:
+      address: 0x9E
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
-    chansel_sram:
-      address: 0xA1
+    psec4a_d_vcdl_monitor_clock_count_lsw:
+      address: 0xA7
       bitposition: 0
-      bitwidth: 4
+      bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
-    writemask_l:
-      address: 0xA2
-      bitposition: 0
-      bitwidth: 8
-      description: 'Enable channel specific behavior an the right side'
-      readwrite: rw
-      value: 0xFF
-    writemask_r:
-      address: 0xA3
+    psec4a_d_vcdl_monitor_clock_count_msw:
+      address: 0xA6
       bitposition: 0
-      bitwidth: 8
-      description: 'Enable channel specific behavior an the right side'
-      readwrite: rw
-      value: 0xFF
-    writemask_common_l:
-      address: 0xA2
-      bitposition: 8
-      bitwidth: 1
-      description: 'Enable writing to all common registers on the left side, useful for the reg1 register which has a different behaviour l and r'
+      bitwidth: 16
+      description: ''
       readwrite: rw
-      value: 1
-    writemask_common_r:
-      address: 0xA3
-      bitposition: 8
+      value: 0
+    # psec4a_mode:
+    #   address: 0x13
+    #   bitposition: 5
+    #   bitwidth: 2
+    #   description: ''
+    #   readwrite: rw
+    #   value: 0
+    xref_address_mode:
+      address: 0x13
+      bitposition: 5
       bitwidth: 1
-      description: 'Enable writing to all commong registers on the right side, useful for the reg1 register which has a different behaviour l and r'
-      readwrite: rw
-      value: 1
-  analog_registers:
-    vadjp:
-      address: 0x00
-      bitposition: 0
-      bitwidth: 12
       description: ''
-      readwrite: w
+      readwrite: rw
       value: 0
-    vlimp:
-      address: 0x01
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 0xFFF
-    vlimn:
-      address: 0x02
+    psec4a_rovcp:
+      address: 0x16
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
-      readwrite: w
-      value: 0
-    vadjn:
-      address: 0x03
+      readwrite: rw
+      value: 300
+    psec4a_status:
+      address: 0x84
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
-      readwrite: w
-      value: 0x6A0
-    wrstrb1_le:
-      address: 0x04
+      readwrite: rw
+      value: 4852
+    psec4a_trigthresh1_out:
+      address: 0x1F
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
-      readwrite: w
-      value: 0x028 # dec: 40
-    wrstrb1_te:
-      address: 0x05
+      readwrite: rw
+      value: 1536  # 0
+    psec4a_trigthresh2_out:
+      address: 0x20
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
-      readwrite: w
-      value: 0x064 # dec: 100
-    wrsync1_le:
-      address: 0x06
+      readwrite: rw
+      value: 1536  # 0
+    psec4a_trigthresh3_out:
+      address: 0x21
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
-      readwrite: w
-      value: 0x001
-    wrsync1_te:
-      address: 0x07
+      readwrite: rw
+      value: 1536  # 0
+    psec4a_trigthresh4_out:
+      address: 0x22
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
-      readwrite: w
-      value: 0x065 # dec: 103
-    wrstrb2_le:
-      address: 0x08
+      readwrite: rw
+      value: 1536  # 0
+    psec4a_trigthresh5_out:
+      address: 0x23
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
-      readwrite: w
-      value: 0x067
-    wrstrb2_te:
-      address: 0x09
+      readwrite: rw
+      value: 1536  # 0
+    psec4a_trigthresh6_out:
+      address: 0x24
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
-      readwrite: w
-      value: 0x024 # dec: 36
-    wrsync2_le:
-      address: 0x0A
+      readwrite: rw
+      value: 1536  # 0
+    psec4a_trigthresh7_out:
+      address: 0x25
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
-      readwrite: w
-      value: 0x07E
-    wrsync2_te:
-      address: 0x0B
+      readwrite: rw
+      value: 1536  # 0
+    psec4a_trigthresh8_out:
+      address: 0x26
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
-      readwrite: w
-      value: 0x01A
-    digsync_le:
-      address: 0x0C
-      bitposition: 0
-      bitwidth: 12
+      readwrite: rw
+      value: 1536  # 0
+    reread_data:
+      address: 0x10
+      bitposition: 9
+      bitwidth: 1
       description: ''
-      readwrite: w
-      value: 0x002
-    digsync_te:
-      address: 0x0D
+      readwrite: rw
+      value: 0
+    ring_oscillator_feedback_target_value_lsw:
+      address: 0x11
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
-      readwrite: w
-      value: 0x041
-    qbias:
-      address: 0x0E
+      readwrite: rw
+      value: 29529
+    ring_oscillator_feedback_target_value_msw:
+      address: 0x12
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
-      readwrite: w
-      value: 0x800
-    sgn:
-      address: 0x0F
+      readwrite: rw
+      value: 7
+    ro_feedback_enable:
+      address: 0x13
       bitposition: 0
-      bitwidth: 8
-      description: ''
-      readwrite: w
-      value: 0
-    sspin:
-      address: 0x0F
-      bitposition: 8
-      bitwidth: 2
+      bitwidth: 1
       description: ''
-      readwrite: w
-      value: 0
-    vadjn_sw:
-      address: 0x0F
-      bitposition: 10
+      readwrite: rw
+      value: 1
+    ro_monitor_reset:
+      address: 0x29
+      bitposition: 3
       bitwidth: 1
       description: ''
-      readwrite: w
+      readwrite: rw
       value: 0
-    sstscrsel:
-      address: 0x0F
-      bitposition: 11
+    self_trigger_or_enable:
+      address: 0x13
+      bitposition: 6
       bitwidth: 1
+      description: 'Enable Self Trigger OR function in PSEC4A'
+      readwrite: rw
+      value: 1
+    serial_data_select:
+      address: 0x28
+      bitposition: 12
+      bitwidth: 4
       description: ''
-      readwrite: w
+      readwrite: rw
       value: 0
-    reg1:
+    serial_write_strobe:
       address: 0x10
       bitposition: 0
-      bitwidth: 12
-      description: 'This is a special overloaded register that require you to read the manual!'
-      readwrite: w
-      value: 0x02D  # Don't you dare touch unless you check the Excel spreadsheet!
-    # montiming_sel_1:
-    #   address: 0x10
-    #   bitposition: 0
-    #   bitwidth: 3
-    #   description: ''
-    #   readwrite: w
-    #   value: 5
-    # montiming_sel_2:
-    #   address: 0x10
-    #   bitposition: 3
-    #   bitwidth: 3
-    #   description: ''
-    #   readwrite: w
-    #   value: 5
-    # txsel:
-    #   address: 0x10
-    #   bitposition: 7
-    #   bitwidth: 1
-    #   description: ''
-    #   readwrite: w
-    #   value: 0
-    # gccsel:
-    #   address: 0x10
-    #   bitposition: 8
-    #   bitwidth: 1
-    #   description: ''
-    #   readwrite: w
-    #   value: 0
-    # div_by_5:
-    #   address: 0x10
-    #   bitposition: 9
-    #   bitwidth: 1
-    #   description: ''
-    #   readwrite: w
-    #   value: 0
-    # montiming_sel_w:
-    #   address: 0x10
-    #   bitposition: 10
-    #   bitwidth: 1
-    #   description: ''
-    #   readwrite: w
-    #   value: 5
-    # montiming_sel_1_r:
-    #   address: 0x10
-    #   bitposition: 0
-    #   bitwidth: 3
-    #   description: ''
-    #   readwrite: w
-    #   value: 5
-    # montiming_sel_2_r:
-    #   address: 0x10
-    #   bitposition: 3
-    #   bitwidth: 3
-    #   description: ''
-    #   readwrite: w
-    #   value: 0
-    # dig_sync_e_sel_r:
-    #   address: 0x10
-    #   bitposition: 7
-    #   bitwidth: 1
-    #   description: ''
-    #   readwrite: w
-    #   value: 0
-    # montimingsel_e_r:
-    #   address: 0x10
-    #   bitposition: 8
-    #   bitwidth: 1
-    #   description: ''
-    #   readwrite: w
-    #   value: 0
-    # montiming_sel_e_nw_r:
-    #   address: 0x10
-    #   bitposition: 9
-    #   bitwidth: 1
-    #   description: ''
-    #   readwrite: w
-    #   value: 0
-    # dig_sync_w_sel_r:
-    #   address: 0x10
-    #   bitposition: 10
-    #   bitwidth: 1
-    #   description: ''
-    #   readwrite: w
-    #   value: 0
-    cmpbias1:
-      address: 0x11
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 0x4E8
-    cmpbias2:
-      address: 0x12
-      bitposition: 0
-      bitwidth: 12
+      bitwidth: 1
       description: ''
-      readwrite: w
-      value: 0x000
-    isel:
+      readwrite: rw
+      value: 0
+    software_trigger:
       address: 0x13
       bitposition: 4
-      bitwidth: 8
+      bitwidth: 1
       description: ''
-      readwrite: w
-      value: 0xAA  # default 800 mV
-    rampcap:
+      readwrite: rw
+      value: 0
+    speed_select:
       address: 0x13
-      bitposition: 0
-      bitwidth: 4
-      description: 'Can be used to change the ramp capacitor value, the actual values, ask Chris'
-      readwrite: w
-      value: 0x0
-    scvbias:
-      address: 0x14
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 0x622
-    scvstab:
-      address: 0x15
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 0x555
-    trgthresh:
-      address: 0x16
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 0x640
-    comp:
-      address: 0x17
-      bitposition: 0
-      bitwidth: 8
-      description: ''
-      readwrite: w
-      value: 0x00
-    ramp7_4:
-      address: 0x17
-      bitposition: 8
-      bitwidth: 4
-      description: ''
-      readwrite: w
-      value: 0x0
-    ramp3_0:
-      address: 0x18
-      bitposition: 0
-      bitwidth: 4
-      description: ''
-      readwrite: w
-      value: 0x0
-    transfer:
-      address: 0x18
-      bitposition: 4
-      bitwidth: 8
-      description: ''
-      readwrite: w
-      value: 0x00
-    unknown:
-      address: 0x19
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 0x000
-    wbias:
-      address: 0x1A
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 0x7D0
-  i2c_registers:
-    i2c_en:
-      address: 0x0F
-      bitposition: 14
+      bitposition: 3
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 1
-    i2c_words:
-      address: 0x0F
-      bitposition: 8
-      bitwidth: 4
-      description: 'number of words to send in the i2c command.'
-      readwrite: rw
-      value: 0
-    i2c_addr:
-      address: 0x0F
+    # system_clock_monitor:
+    #   address: 0x28
+    #   bitposition: 8
+    #   bitwidth: 1
+    #   description: ''
+    #   readwrite: rw
+    #   value: 1
+    trig_out1:
+      address: 0x90
       bitposition: 0
-      bitwidth: 8
-      description: 'i2c address for the commands in the string builder'
+      bitwidth: 4
+      description: 'DCBA chiporder'
       readwrite: rw
       value: 0
-    i2c_data0:
-      address: 0x10
-      bitposition: 0
+    trigger_mask_enable:
+      address: 0x29
+      bitposition: 8
       bitwidth: 8
-      description: 'Data storage used by the i2c string builder, for both rx and tx data'
+      description: 'Trigger mask where each bit is a corresponding chip'
       readwrite: rw
-      value: 0
-    i2c_data1:
-      address: 0x11
-      bitposition: 0
-      bitwidth: 16
-      description: 'Data storage used by the i2c string builder, for both rx and tx data'
+      value: 255  # '11111111'
+    trigger_mode:
+      address: 0x29
+      bitposition: 5
+      bitwidth: 2
+      description: '<html><head/><body><p>Set the triggermode:<br/>
+        00: Software Trigger, the default.<br/>
+        01: Auto Trigger, 2Hz auto trigger rate.<br/>
+        10: External Trigger, trigger on trig in.<br/>
+        11: Self Trigger, trigger on signal levels.
+        </p></body></html>'
       readwrite: rw
       value: 0
-    i2c_data2:
-      address: 0x12
-      bitposition: 0
-      bitwidth: 16
-      description: 'Data storage used by the i2c string builder, for both rx and tx data'
+    trigger_reset:
+      address: 0x13
+      bitposition: 13
+      bitwidth: 1
+      description: ''
       readwrite: rw
       value: 0
-    i2c_data3:
+    # trigger_scaler:
+    #   address: 0x97
+    #   bitposition: 0
+    #   bitwidth: 8
+    #   description: ''
+    #   readwrite: rw
+    #   value: 0
+    trigger_sign:
       address: 0x13
-      bitposition: 0
-      bitwidth: 16
-      description: 'Data storage used by the i2c string builder, for both rx and tx data'
+      bitposition: 1
+      bitwidth: 1
+      description: ''
       readwrite: rw
       value: 0
-    response0:
-      address: 0x28
+    uart_status:
+      address: 0x81
       bitposition: 0
-      bitwidth: 16
+      bitwidth: 8
       description: ''
-      readwrite: r
-      value: 0
-    response1:
-      address: 0x29
-      bitposition: 0
-      bitwidth: 16
+      readwrite: rw
+      value: 84
+    uart_handshake_en_out:
+      address: 0x10
+      bitposition: 8
+      bitwidth: 1
       description: ''
-      readwrite: r
-      value: 0
-    response2:
-      address: 0x2A
+      readwrite: rw
+      value: false
+    version_number:
+      address: 0x80
       bitposition: 0
       bitwidth: 16
       description: ''
-      readwrite: r
-      value: 0
-    response3:
-      address: 0x2B
-      bitposition: 0
-      bitwidth: 16
+      readwrite: rw
+      value: 4101
+    wave_fifo_reset:
+      address: 0x10
+      bitposition: 1
+      bitwidth: 1
       description: ''
-      readwrite: r
+      readwrite: rw
       value: 0
+    xfer_reset:
+      address: 0x13
+      bitposition: 2
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: 1
```

### Comparing `naluconfigs-10.8.0/src/naluconfigs/data/registers/upac32.yml` & `naluconfigs-11.0.0/src/naluconfigs/data/registers/zdigitizer.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,29 @@
-model: upac32
-features:
-  adc2mv: false
-  dac_sweep: false
-  ext_dac: true
-  pedestals: true
-  threshold_scan: false
-  tia_dac: false
-  timing_calibration: false
-  naludaq_rs: false
+model: zdigitizer
 params:
   chanmask: 511
   channels: 32
   chanshift: 3
   connections:
     - serial
     - d2xx
   default_baud:
-    115200: 432
+    115200: 217
   default_baudrate: 115200
   default_clock: 200000000.0
-  default_divider: 432
+  default_divider: 217
   default_trigger_value: 0
   ext_dac:
     max_mv: 1200
     max_counts: 65535
     channels:
-      0,8,16,24: 30000
-    register_mapping:
-      0: dac_vbias00_07_out
-      8: dac_vbias08_15_out
-      16: dac_vbias16_23_out
-      24: dac_vbias24_31_out
+      0: 30000
+      8: 30000
+      16: 30000
+      24: 30000
   trigger:
     triggers_available: 8
     max_val: 2047
     min_val: 0
     default: false
   num_trigger_channels: 8
   expected_scalmon: 2500
@@ -56,18 +45,16 @@
       gain: 1
     vadjp:
       chan: 1
       addr: 0xD8
       bits: 16
       gain: 1
   possible_bauds:
-    115200: 432
-    460800: 108
-    # 2000000: 25
-    # 3000000: 17
+    115200: 217
+    1000000: 25
   resolution: 11
   samples: 132
   samplingrate: 9.2
   stop_word: !!binary |
     +s4=
   wait: AE000001
   wbias: 750
@@ -337,14 +324,28 @@
     pll_lock_bit_0:
       address: 0x86
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
       value: 1
+    # psec4a_mclk_source_clock_count_lsw:
+    #   address: 0x8F
+    #   bitposition: 0
+    #   bitwidth: 16
+    #   description: 'Read-only Debug clock, should be the same as VCDL when read out'
+    #   readwrite: r
+    #   value: 0
+    # psec4a_mclk_source_clock_count_msw:
+    #   address: 0x8E
+    #   bitposition: 0
+    #   bitwidth: 16
+    #   description: 'Read-only Debug clock, should be the same as VCDL when read out'
+    #   readwrite: r
+    #   value: 0
     psec4a_a_ro_feedback_calculated_value:
       address: 0xA8
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
       value: 247
@@ -470,28 +471,14 @@
     psec4a_biasxfer_out:
       address: 0x18
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
       value: 512
-    psec4a_mclk_source_clock_count_lsw:
-      address: 0x8F
-      bitposition: 0
-      bitwidth: 16
-      description: 'Read-only Debug clock, should be the same as VCDL when read out'
-      readwrite: r
-      value: 0
-    psec4a_mclk_source_clock_count_msw:
-      address: 0x8E
-      bitposition: 0
-      bitwidth: 16
-      description: 'Read-only Debug clock, should be the same as VCDL when read out'
-      readwrite: r
-      value: 0
     psec4a_c_ro_feedback_calculated_value:
       address: 0xAA
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
       value: 326
@@ -582,70 +569,70 @@
     psec4a_status:
       address: 0x84
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
       value: 4852
-    psec4a_trigthresh0_out:
+    psec4a_trigthresh1_out:
       address: 0x1F
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0  # 0
-    psec4a_trigthresh1_out:
+      value: 1536  # 0
+    psec4a_trigthresh2_out:
       address: 0x20
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0  # 0
-    psec4a_trigthresh2_out:
+      value: 1536  # 0
+    psec4a_trigthresh3_out:
       address: 0x21
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0  # 0
-    psec4a_trigthresh3_out:
+      value: 1536  # 0
+    psec4a_trigthresh4_out:
       address: 0x22
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0  # 0
-    psec4a_trigthresh4_out:
+      value: 1536  # 0
+    psec4a_trigthresh5_out:
       address: 0x23
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0  # 0
-    psec4a_trigthresh5_out:
+      value: 1536  # 0
+    psec4a_trigthresh6_out:
       address: 0x24
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0  # 0
-    psec4a_trigthresh6_out:
+      value: 1536  # 0
+    psec4a_trigthresh7_out:
       address: 0x25
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0  # 0
-    psec4a_trigthresh7_out:
+      value: 1536  # 0
+    psec4a_trigthresh8_out:
       address: 0x26
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0  # 0
+      value: 1536  # 0
     reread_data:
       address: 0x10
       bitposition: 9
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
@@ -797,70 +784,7 @@
     xfer_reset:
       address: 0x13
       bitposition: 2
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 1
-    ltc2992_p1_in_23_to_16:
-      address: 0xAC
-      bitposition: 0
-      bitwidth: 16
-      description: 'Top bits for PDBIAS Power readout from the LTC2992 sensor chip'
-      readwrite: r
-      value: 0
-    ltc2992_p1_in_15_to_0:
-      address: 0xAD
-      bitposition: 0
-      bitwidth: 16
-      description: 'Bottom bits for PDBIAS Power readout from the LTC2992 sensor chip'
-      readwrite: r
-      value: 0
-    ltc2992_i1_in:
-      address: 0xAE
-      bitposition: 0
-      bitwidth: 16
-      description: 'PDBIAS current readout from the LTC2992 sensor chip'
-      readwrite: r
-      value: 0
-    ltc2992_s1_in:
-      address: 0xAF
-      bitposition: 0
-      bitwidth: 16
-      description: 'PDBIAS Voltage readout from the LTC2992 sensor chip'
-      readwrite: r
-      value: 0
-    ltc2992_g1_in:
-      address: 0xB0
-      bitposition: 0
-      bitwidth: 16
-      description: 'Bottom bits for LTC2992 sensor chip'
-      readwrite: r
-      value: 0
-    ltc2992_p2_in_23_to_16:
-      address: 0xB1
-      bitposition: 0
-      bitwidth: 16
-      description: 'Top bits for 1.2V rail power readout from the LTC2992 sensor chip'
-      readwrite: r
-      value: 0
-    ltc2992_p2_in_15_to_0:
-      address: 0xB2
-      bitposition: 0
-      bitwidth: 16
-      description: 'Top bits for 1.2V rail power readout from the LTC2992 sensor chip'
-      readwrite: r
-      value: 0
-    ltc2992_i2_in:
-      address: 0xB3
-      bitposition: 0
-      bitwidth: 16
-      description: '1.2V rail current readout from the LTC2992 sensor chip'
-      readwrite: r
-      value: 0
-    ltc2992_s2_in:
-      address: 0xB4
-      bitposition: 0
-      bitwidth: 16
-      description: '1.2V rail voltage readout from the LTC2992 sensor chip'
-      readwrite: r
-      value: 0
```

### Comparing `naluconfigs-10.8.0/src/naluconfigs/data/registers/upac96.yml` & `naluconfigs-11.0.0/src/naluconfigs/data/registers/trbhm.yml`

 * *Files 17% similar despite different names*

```diff
@@ -1,876 +1,738 @@
-model: upac96
+model: trbhm
 features:
-  adc2mv: false
-  dac_sweep: true
+  adc2mv: true
+  dac_sweep: false
   ext_dac: true
   pedestals: true
-  threshold_scan: false
+  threshold_scan: true
   tia_dac: false
-  timing_calibration: false
-  naludaq_rs: false
+  timing_calibration: true
+  naludaq_rs: true
 params:
-  num_chips: 6  # Number of chips, to be replaced with the actual chips
-  chanmask: 0xFF00
-  channels: 96
-  chanshift: 8
-  clock_file: Si5341-RevD-UDC_78_125SlowClk_78_125IntermediateClk_312_5FastClk-Registers.txt
+  chanmask: 0xF000
+  channels: 8
+  chanshift: 10
+  chips:
+    0..1:
+      !include_chip
+      from: aardvarcv3::params
+  clock_file: Si5341_TRBHM_10GSaps_GCCsstx2_Registers.txt
   connections:
     - serial
     - d2xx
-    - d3xx
+    - udp
   si5341_address: 0xEE
+  timing_hack: true
   default_baud:
-    115200: 678
+    115200: 868
   default_baudrate: 115200
-  default_clock: 50000000.0
-  default_divider: 434
-  default_trigger_value: 0
+  default_clock: 100000000.0
+  default_divider: 868
+  default_trigger_value: 1500
+  threshold_scan:
+    min_vref: 0
+    max_vref: 2500
+    start: 500
+    stop: 3500
+    stepsize: 5
+    units: counts
+  expected_scalmon: 2500
   ext_dac:
-    chip: dac7578
-    max_mv: 1250
-    max_counts: 3930
-    min_counts: 0
+    chip: ltc2620
+    max_mv: 1200
+    max_counts: 4095
     channels:
-      0,16,32,48,64,80: 2000
-    address_mapping:
-      0,16,32,48,64,80: 0x48
-    channel_mapping:
-      0: 7
-      16: 2
-      32: 5
-      48: 0
-      64: 4
-      80: 6
-  trigger:
-    max_val: 4095
-    min_val: 0
-    default: false
-  num_trigger_channels: 8
-  expected_scalmon: 2500
-  headers: 0
-  last_window_fix_amount: 47
-  lastbits: 0
-  numregs: 32
-  pedestals_blocks: 64
+      0..7: 2048
+    chip_mapping: # asic channel: dac chip number
+      0..3: 0
+      4..7: 1
+      cal0: 0
+      cal1: 1
+    channel_mapping: # asic channel: ext. dac channel
+      0, 4: 0
+      1, 5: 2
+      2, 6: 5
+      3, 7: 7
+      cal0: 4
+      cal1: 4
+  headers: 3
+  new_firmware: True
+  numregs: 64
+  pedestals_blocks: 16
   peripherals:
-    readout_pcb_temp:
-      addr: 0b0011_000
-    power_pcb_temp:
-      addr: 0b0011_001
-    udc1_1v2:
-      addr: 0b1001_101
-      chan: 1
-    udc1_2v5:
-      addr: 0b1001_101
-      chan: 2
-    udc2_1v2:
-      addr: 0b1001_100
+    current:
+      chan: 0
+      addr: 0xD0
+      bits: 16
+      gain: 8
+    vadjn:
+      chan: 0
+      addr: 0xD8
+      bits: 16
+      gain: 1
+    vadjp:
       chan: 1
-    udc2_2v5:
-      addr: 0b1001_100
-      chan: 2
-    fpga_1v0:
-      addr: 0b1001_100
-      chan: 4
-    fpga_1v8:
-      addr: 0b1001_100
-      chan: 3
-    fpga_io_2v5:
-      addr: 0b1001_101
-      chan: 4
-    fpga_io_3v3:
-      addr: 0b1001_101
-      chan: 3
+      addr: 0xD8
+      bits: 16
+      gain: 1
   possible_bauds:
-    115200: 678
-    1000000: 78
-    2000000: 39
-  resolution: 10
+    115200: 868
+    1000000: 100
+    2000000: 50
+    3000000: 33
+  resolution: 12
   samples: 64
-  samplingrate: 9.2
-  stop_word: FACECAFE
+  samplingrate: 10.0
+  stop_word: BEEFBEEF
   register_stop_word: FACE
   strobe_values_correction: True  # Shift the strobe values on certain boards with swapped internal routing.
   strobe_correction_keys:
-    - digsync_le
-    - digsync_te
+    - calstrb_le
+    - calstrb_te
     - wrstrb1_le
     - wrstrb1_te
     - wrstrb2_le
     - wrstrb2_te
     - wrsync1_le
     - wrsync1_te
     - wrsync2_le
     - wrsync2_te
   wait: AE000001
-  wbias: 750
-  windmask: 0x00FF
-  windows: 64
+  wbias: 2000
+  windmask: 0x3FE
+  windows: 510
 registers:
+  analog_registers:
+    !include_registers
+      from: aardvarcv3::registers::analog_registers
+      value_count: 2
+      override:
+        isel:
+          value: [2730, 2730]
+  digital_registers:
+    !include_registers
+      from: aardvarcv3::registers::digital_registers
+      value_count: 2
+      override:
+        chipid:
+          value: [2730, 2730]
+        miscreg:
+          value: [2, 2]
   control_registers:
-    identifier:
-      address: 0x00
-      bitposition: 0
-      bitwidth: 16
-      description: 'Unique board identifier'
-      readwrite: rw
-      value: 0x03E8
-    version:
-      address: 0x01
-      bitposition: 0
-      bitwidth: 16
-      description: 'Current firmware version'
+    1v2_en:
+      address: 0x17
+      bitposition: 1
+      bitwidth: 1
+      description: ''
       readwrite: rw
-      value: 0x0000
-    regclr:
-      address: 0x04
+      value: true
+    2v5_en:
+      address: 0x17
       bitposition: 0
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
-    sysrst:
-      address: 0x04
-      bitposition: 1
+      value: true
+    3v3_i2c_en:
+      address: 0x17
+      bitposition: 2
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
-    eventtrig:
-      address: 0x04
-      bitposition: 2
+      value: true
+    8b10b_en:
+      address: 0x19
+      bitposition: 12
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    arm:
-      address: 0x04
-      bitposition: 3
-      bitwidth: 1
+    amp_en:
+      address: 0x1A
+      bitposition: 0
+      bitwidth: 8
+      description: Enable onboard amplifiers
+      readwrite: rw
+      value: 0
+    addr:
+      address: 0x16
+      bitposition: 0
+      bitwidth: 9
       description: ''
       readwrite: rw
       value: 0
-    abort:
-      address: 0x04
-      bitposition: 4
+    addr_user:
+      address: 0x16
+      bitposition: 15
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
-    continuousmode:
-      address: 0x04
-      bitposition: 5
+      value: false
+    chansel:
+      address: 0x06
+      bitposition: 12
+      bitwidth: 4
+      description: ''
+      readwrite: rw
+      value: 15
+    clk1v8_en:
+      address: 0x17
+      bitposition: 4
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
-    reread_data: #udc reread
-      address: 0x04
-      bitposition: 6
+      value: true
+    clk2v5_en:
+      address: 0x17
+      bitposition: 3
       bitwidth: 1
-      description: 'Ask the FPGA to send whatever event is in the output buffer'
+      description: ''
       readwrite: rw
-      value: 0
-    digrst:
-      address: 0x04
-      bitposition: 7
+      value: true
+    clk_fdec:
+      address: 0x17
+      bitposition: 9
       bitwidth: 1
-      description:
+      description: ''
       readwrite: rw
-      value: 0
-    pwr_udc1_en:
-      address: 0x04
+      value: false
+    clk_finc:
+      address: 0x17
       bitposition: 8
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
-    pwr_udc2_en:
-      address: 0x04
-      bitposition: 9
+      value: false
+    clk_i2c_sel:
+      address: 0x17
+      bitposition: 5
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
-    usb_fifo_disable:
-      address: 0x04
-      bitposition: 10
+      value: true
+    clk_oeb:
+      address: 0x17
+      bitposition: 6
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
-    uart_fifo_disable:
-      address: 0x04
-      bitposition: 11
+      value: false
+    clk_reset:
+      address: 0x17
+      bitposition: 7
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
-    trigger_select:
-      address: 0x04
-      bitposition: 12
-      bitwidth: 2
+      value: false
+    clk_sync:
+      address: 0x17
+      bitposition: 10
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
-    trigger_monitor_disable:
-      address: 0x04
-      bitposition: 14
-      bitwidth: 1
-      description: 'Disable the trigger monitor signal, needs to be disabled during pedestals capture.'
+      value: false
+    data:
+      address: 0x14
+      bitposition: 0
+      bitwidth: 12
+      description: ''
       readwrite: rw
       value: 0
-    coincidence_trigger_select:
-      address: 0x04
+    data_user:
+      address: 0x14
       bitposition: 15
       bitwidth: 1
-      description: Controls whether the coincidence trigger signal is routed through the debug_trigger_out pin
+      description: ''
       readwrite: rw
-      value: 0
-    udc_rxout_enable:
-      address: 0x05
+      value: false
+    debug_data:
+      address: 0x15
       bitposition: 0
-      bitwidth: 6
+      bitwidth: 12
       description: ''
       readwrite: rw
-      value: 0x3F
-    udc_rx_negative_polarity:
-      address: 0x05
-      bitposition: 8
-      bitwidth: 6
+      value: 0
+    debug_data_user:
+      address: 0x15
+      bitposition: 15
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0x37
-    udc_txin_enable:
-      address: 0x06
-      bitposition: 0
-      bitwidth: 6
+      value: false
+    digrst:
+      address: 0x16
+      bitposition: 9
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0x3F
-    udc_tx_negative_polarity:
-      address: 0x06
-      bitposition: 8
-      bitwidth: 6
+      value: 0
+    digser_rst:
+      address: 0x19
+      bitposition: 13
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0x27
-    udc_select:
-      address: 0x0D
+      value: 0
+    eth_addr_sel:
+      address: 0x2F
       bitposition: 0
-      bitwidth: 3
-      description: ''
+      bitwidth: 2
+      description: 'enables manually set destination (bit 0) and source (bit 1) IP addresses'
       readwrite: rw
       value: 0
-    udc_trigger_mask:
-      address: 0x0D
-      bitposition: 8
-      bitwidth: 6
-      description: 'Select which chips are used for the trigger, 1 = use chip, 0 = ignore chip, bit 0 = chip 0, bit 5 = chip 5'
+    eth_port_sel:
+      address: 0x2F
+      bitposition: 2
+      bitwidth: 2
+      description: 'enables manually set destination (bit 0) and source (bit 1) UDP ports'
       readwrite: rw
-      value: 0x3F
-    system_clock_locked:
-      address: 0x24
-      bitposition: 0
-      bitwidth: 1
-      description: 'Read-Only status register'
-      readwrite: r
       value: 0
-    usb_clock_locked:
-      address: 0x24
-      bitposition: 1
+    tx_mode:
+      address: 0x2F
+      bitposition: 4
       bitwidth: 1
-      description: 'Read-Only status register'
-      readwrite: r
-      value: 0
-    udc_tx_idle_locked:
-      address: 0x25
-      bitposition: 0
-      bitwidth: 6
-      description: 'Read-Only status register'
-      readwrite: r
-      value: 0
-    udc_rxout_locked:
-      address: 0x26
-      bitposition: 0
-      bitwidth: 6
-      description: 'Read-Only status register'
-      readwrite: r
+      description: 'selects ethernet (value = 1) or UART (value = 0) transmission'
+      readwrite: rw
       value: 0
-    sdata_in_phase:
-      address: 0x0E
-      bitposition: 0
-      bitwidth: 6
-      description: 'Sets the phase relation of the FPGA SERDES input data to the SERDES clock: 0=>0 degrees: 1=>180 degrees'
+    eth_ar_en:
+      address: 0x2F
+      bitposition: 5
+      bitwidth: 1
+      description: 'enables auto-response destination IP address; currently unused'
       readwrite: rw
-      value: 0x1
-    sdata_out_phase:
-      address: 0x0E
+      value: 0
+    eth_dhcp_en:
+      address: 0x2F
       bitposition: 6
-      bitwidth: 6
-      description: 'Sets the phase relation of the FPGA SERDES output data to the SERDES clock: 0=>0 degrees: 1=>180 degrees'
+      bitwidth: 1
+      description: 'enables DHCP resolution of source IP address; currently unused'
       readwrite: rw
-      value: 0x0
-  digital_registers:
-    scalmon:
-      address: 0x08
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: r
-      value: 0
-    scalmon2:
-      address: 0x0B
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: r
-      value: 0
-    start_window_addr:
-      address: 0x0F
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: r
-      value: 0
-    high_addr:
-      address: 0x40
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: r
       value: 0
-    writeaftertrig:
-      address: 0x83
+    eth_dest_addr15_0:
+      address: 0x30
       bitposition: 0
-      bitwidth: 12
-      description: 'Clock cycles to continue writing after trigger, translates to windows to write after trig event.'
+      bitwidth: 16
+      description: 'lower 16 bits of ethernet destination IP address'
       readwrite: rw
       value: 0
-    convert_reset_wait:
-      address: 0x84
+    eth_dest_addr31_16:
+      address: 0x31
       bitposition: 0
-      bitwidth: 8
-      description: ''
+      bitwidth: 16
+      description: 'upper 16 bits of ethernet destination IP address'
       readwrite: rw
-      value: 1
-    enable_testpattern:
-      address: 0x88
+      value: 0
+    eth_src_addr15_0:
+      address: 0x32
       bitposition: 0
-      bitwidth: 1
-      description: ''
+      bitwidth: 16
+      description: 'lower 16 bits of ethernet source IP address'
       readwrite: rw
       value: 0
-    chip_id:
-      address: 0x89
+    eth_src_addr31_16:
+      address: 0x33
       bitposition: 0
-      bitwidth: 12
-      description: 'Identifier for the chip. Lowest 6-bits will be the identifier in the packet header, for multichip systems.'
+      bitwidth: 16
+      description: 'upper 16 bits of ethernet source IP address'
       readwrite: rw
       value: 0
-    regclr:
-      address: 0x8A
+    eth_dest_port:
+      address: 0x34
       bitposition: 0
-      bitwidth: 1
-      description: ''
+      bitwidth: 16
+      description: 'UDP destination port'
       readwrite: rw
       value: 0
-    loadwait:
-      address: 0x8B
+    eth_src_port:
+      address: 0x35
       bitposition: 0
-      bitwidth: 7
-      description: ''
+      bitwidth: 16
+      description: 'UDP source port'
       readwrite: rw
       value: 0
-    pclkwidth:
-      address: 0x8C
-      bitposition: 0
-      bitwidth: 7
+    exttrig:
+      address: 0x04
+      bitposition: 10
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 2
-    miscreg:
-      address: 0x8D
+      value: false
+    gccclr:
+      address: 0x04
       bitposition: 4
-      bitwidth: 2
+      bitwidth: 1
       description: ''
       readwrite: rw
+      value: false
+    idac_update:
+      address: 0x1B
+      bitposition: 14
+      bitwidth: 2
+      description: 'This bit toggled 0-1-0 will start the SPI firmware block that loads the DAC values base on the other registers'
+      readwrite: rw
       value: 0
-    waitread:
-      address: 0x8E
-      bitposition: 0
+    idac_command:
+      address: 0x1B
+      bitposition: 8
       bitwidth: 4
-      description: ''
+      description: 'Is the command from the data sheet with options on what the LTC2620 does with the data written to it. The data sheet is attached most often this is an "0011'
       readwrite: rw
-      value: 0xF
-    waitaddr:
-      address: 0x8F
-      bitposition: 0
+      value: 0
+    idac_address:
+      address: 0x1B
+      bitposition: 4
       bitwidth: 4
-      description: ''
-      readwrite: rw
-      value: 0xF
-    triggerchannelmask_lo:
-      address: 0x90
-      bitposition: 0
-      bitwidth: 8
-      description: ''
+      description: 'Is the DAC Channel number from the data sheet.'
       readwrite: rw
       value: 0
-    writedelay:
-      address: 0x91
+    idac_chip_number:
+      address: 0x1B
       bitposition: 0
       bitwidth: 4
-      description: ''
+      description: 'IS the DAC number "0000" or "0001"  there are two DACs in the design.'
       readwrite: rw
       value: 0
-    triggerchannelmask_hi:
-      address: 0x92
+    idac_value:
+      address: 0x1C
       bitposition: 0
-      bitwidth: 8
-      description: ''
+      bitwidth: 12
+      description: '12 bit DAC value.'
       readwrite: rw
       value: 0
-    txspeed:
-      address: 0x94
+    fifo_unload_or_event_en:
+      address: 0x1F
       bitposition: 0
-      bitwidth: 2
-      description: ''
+      bitwidth: 1
+      description: 'Once data is loaded into the FIFO it will not be sent out to the UART until the end of the current event. Use this mode for capturing sampled data events. '
       readwrite: rw
       value: 0
-    excludechannelmask_lo:
-      address: 0x96
+    identifier:
+      address: 0x00
       bitposition: 0
-      bitwidth: 8
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0
-    excludechannelmask_hi:
-      address: 0x97
+      value: 43714
+    iomode0:
+      address: 0x04
       bitposition: 0
-      bitwidth: 8
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
-    done_timeout_n:
-      address: 0xA0
+      value: true
+    iomode1:
+      address: 0x04
+      bitposition: 6
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: false
+    leds:
+      address: 0x18
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
-    chansel_sram:
-      address: 0xA1
-      bitposition: 0
+    loadwait:
+      address: 0x07
+      bitposition: 8
       bitwidth: 4
       description: ''
       readwrite: rw
-      value: 0
-    writemask_l:
-      address: 0xA2
-      bitposition: 0
-      bitwidth: 9
-      description: 'Enable channel specific behavior an the right side'
+      value: 15
+    nramp:
+      address: 0x04
+      bitposition: 5
+      bitwidth: 1
+      description: ''
       readwrite: rw
-      value: 0x1FF
-    writemask_r:
-      address: 0xA3
-      bitposition: 0
-      bitwidth: 9
-      description: 'Enable channel specific behavior an the right side'
+      value: false
+    nrw:
+      address: 0x04
+      bitposition: 11
+      bitwidth: 1
+      description: ''
       readwrite: rw
-      value: 0x1FF
-  analog_registers:
-    vadjp:
-      address: 0x00
+      value: false
+    numwinds:
+      address: 0x08
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 8
       description: ''
-      readwrite: w
-      value: 0
-    vlimp:
-      address: 0x01
-      bitposition: 0
-      bitwidth: 12
+      readwrite: rw
+      value: 1
+    pclk:
+      address: 0x04
+      bitposition: 2
+      bitwidth: 1
       description: ''
-      readwrite: w
-      value: 0xFFF
-    vlimn:
-      address: 0x02
-      bitposition: 0
-      bitwidth: 12
+      readwrite: rw
+      value: false
+    pclkwidth:
+      address: 0x07
+      bitposition: 12
+      bitwidth: 4
       description: ''
-      readwrite: w
-      value: 0
-    vadjn:
-      address: 0x03
+      readwrite: rw
+      value: 15
+    ramplen:
+      address: 0x06
       bitposition: 0
       bitwidth: 12
       description: ''
-      readwrite: w
-      value: 0x6A0
-    wrstrb1_le:
+      readwrite: rw
+      value: 2000
+    regclr:
       address: 0x04
-      bitposition: 0
-      bitwidth: 12
+      bitposition: 1
+      bitwidth: 1
       description: ''
-      readwrite: w
-      value: 0x028
-    wrstrb1_te:
+      readwrite: rw
+      value: false
+    runevs:
       address: 0x05
       bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 0x064
-    wrsync1_le:
-      address: 0x06
-      bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
-      readwrite: w
-      value: 0x000
-    wrsync1_te:
-      address: 0x07
+      readwrite: rw
+      value: 1
+    rx_en:
+      address: 0x19
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 1
       description: ''
-      readwrite: w
-      value: 0x032
-    wrstrb2_le:
-      address: 0x08
-      bitposition: 0
-      bitwidth: 12
+      readwrite: rw
+      value: 0
+    rx_num_words:
+      address: 0x19
+      bitposition: 2
+      bitwidth: 6
       description: ''
-      readwrite: w
-      value: 0x067
-    wrstrb2_te:
-      address: 0x09
-      bitposition: 0
-      bitwidth: 12
+      readwrite: rw
+      value: 0
+    rx_oneshot:
+      address: 0x19
+      bitposition: 1
+      bitwidth: 1
       description: ''
-      readwrite: w
-      value: 0x024
-    wrsync2_le:
-      address: 0x0A
-      bitposition: 0
-      bitwidth: 12
+      readwrite: rw
+      value: 0
+    rx_speed:
+      address: 0x19
+      bitposition: 8
+      bitwidth: 2
       description: ''
-      readwrite: w
-      value: 0x040
-    wrsync2_te:
-      address: 0x0B
-      bitposition: 0
-      bitwidth: 12
+      readwrite: rw
+      value: 0
+    sel:
+      address: 0x04
+      bitposition: 12
+      bitwidth: 1
       description: ''
-      readwrite: w
-      value: 0x072
-    digsync_le:
-      address: 0x0C
-      bitposition: 0
-      bitwidth: 12
+      readwrite: rw
+      value: false
+    selany:
+      address: 0x04
+      bitposition: 3
+      bitwidth: 1
       description: ''
-      readwrite: w
-      value: 0x002
-    digsync_te:
-      address: 0x0D
-      bitposition: 0
-      bitwidth: 12
+      readwrite: rw
+      value: false
+    slow_sysclk:
+      address: 0x19
+      bitposition: 10
+      bitwidth: 1
       description: ''
-      readwrite: w
-      value: 0x041
-    qbias:
-      address: 0x0E
-      bitposition: 0
-      bitwidth: 12
+      readwrite: rw
+      value: 0
+    stopacq:
+      address: 0x04
+      bitposition: 13
+      bitwidth: 1
       description: ''
-      readwrite: w
-      value: 0x800
-    sgn:
-      address: 0x0F
+      readwrite: rw
+      value: false
+    syncloc:
+      address: 0x09
       bitposition: 0
       bitwidth: 8
       description: ''
-      readwrite: w
+      readwrite: rw
       value: 0
-    sspin:
-      address: 0x0F
+    sysclk:
+      address: 0x04
       bitposition: 8
-      bitwidth: 2
+      bitwidth: 1
       description: ''
-      readwrite: w
-      value: 0
-    vadjn_sw:
-      address: 0x0F
-      bitposition: 10
+      readwrite: rw
+      value: false
+    sysrst:
+      address: 0x04
+      bitposition: 9
       bitwidth: 1
       description: ''
-      readwrite: w
-      value: 0
-    sstscrsel:
-      address: 0x0F
+      readwrite: rw
+      value: true
+    tx_en:
+      address: 0x19
       bitposition: 11
       bitwidth: 1
       description: ''
-      readwrite: w
+      readwrite: rw
       value: 0
-    reg1:
-      address: 0x10
-      bitposition: 0
-      bitwidth: 12
-      description: |
-        This is a special overloaded register that require you to read the manual!
-        A strange register, corresponding to two different physical registers. To write to them separately,
-        you need to set the most significant bit of "writemask_l" and "writemask_r", depending on whether
-        you want to talk to the left version of this register or the right version.
-      readwrite: w
-      value: 0x02D  # Don't you dare touch unless you check the Excel spreadsheet!
-    # montiming_sel_1:
-    #   address: 0x10
-    #   bitposition: 0
-    #   bitwidth: 3
-    #   description: ''
-    #   readwrite: w
-    #   value: 0x101
-    # montiming_sel_2:
-    #   address: 0x10
-    #   bitposition: 3
-    #   bitwidth: 3
-    #   description: ''
-    #   readwrite: w
-    #   value: 0x101
-    # txsel:
-    #   address: 0x10
-    #   bitposition: 7
-    #   bitwidth: 1
-    #   description: ''
-    #   readwrite: w
-    #   value: 0
-    # gccsel:
-    #   address: 0x10
-    #   bitposition: 8
-    #   bitwidth: 1
-    #   description: ''
-    #   readwrite: w
-    #   value: 1
-    # div_by_5:
-    #   address: 0x10
-    #   bitposition: 9
-    #   bitwidth: 1
-    #   description: ''
-    #   readwrite: w
-    #   value: 0
-    # montiming_sel_w:
-    #   address: 0x10
-    #   bitposition: 10
-    #   bitwidth: 1
-    #   description: ''
-    #   readwrite: w
-    #   value: 0
-    # montiming_sel_1_r:
-    #   address: 0x10
-    #   bitposition: 0
-    #   bitwidth: 3
-    #   description: ''
-    #   readwrite: w
-    #   value: 0x101
-    # montiming_sel_2_r:
-    #   address: 0x10
-    #   bitposition: 3
-    #   bitwidth: 3
-    #   description: ''
-    #   readwrite: w
-    #   value: 0x101
-    # dig_sync_e_sel_r:
-    #   address: 0x10
-    #   bitposition: 7
-    #   bitwidth: 1
-    #   description: ''
-    #   readwrite: w
-    #   value: 0
-    # montimingsel_e_r:
-    #   address: 0x10
-    #   bitposition: 8
-    #   bitwidth: 1
-    #   description: ''
-    #   readwrite: w
-    #   value: 1
-    # montiming_sel_e_nw_r:
-    #   address: 0x10
-    #   bitposition: 9
-    #   bitwidth: 1
-    #   description: ''
-    #   readwrite: w
-    #   value: 0
-    # dig_sync_w_sel_r:
-    #   address: 0x10
-    #   bitposition: 10
-    #   bitwidth: 1
-    #   description: ''
-    #   readwrite: w
-    #   value: 0
-    cmpbias1:
-      address: 0x11
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 0x3E8
-    cmpbias2:
-      address: 0x12
+    uart_tx_disable:
+      address: 0x28
+      bitposition: 2
+      bitwidth: 1
+      description: Set to 1 to disable UART output from the board
+      readwrite: rw
+      value: 0
+    windsel:
+      address: 0x07
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 8
       description: ''
-      readwrite: w
-      value: 0x000
-    isel:
-      address: 0x13
-      bitposition: 0
-      bitwidth: 12
+      readwrite: rw
+      value: 0
+    wrstrboff:
+      address: 0x04
+      bitposition: 7
+      bitwidth: 1
       description: ''
-      readwrite: w
-      value: 0x000
-    scvbias:
-      address: 0x14
+      readwrite: rw
+      value: false
+    rxout_pol:
+      address: 0x22
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
-      readwrite: w
-      value: 0x622
-    scvstab:
-      address: 0x15
+      readwrite: rw
+      value: 6400
+    txin_pol:
+      address: 0x23
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
-      readwrite: w
-      value: 0x555
-    trgthresh:
-      address: 0x16
+      readwrite: rw
+      value: 4412
+    ard_header:
+      address: 0x21
       bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 0x640
-    comparator:
-      address: 0x17
+      bitwidth: 1
+      description: 'Enable AARDVARC debug header.'
+      readwrite: rw
+      value: 1
+    ard_rx_en:
+      address: 0x1D
       bitposition: 0
-      bitwidth: 8
-      description: |
-        Comparator mode, sets the comparator mode for ch0..7 or 8..15.
-        Need to set dig_reg writemask_l and writemask_r to write the different sides.
-      readwrite: w
-      value: 0x00
-    ramp7_4:
-      address: 0x17
-      bitposition: 8
-      bitwidth: 4
-      description: ''
-      readwrite: w
-      value: 0x0
-    ramp3_0:
-      address: 0x18
+      bitwidth: 16
+      description: 'TR-BHM ASIC Rx Enable register 29dec. Bit 0 and 1 enable transmitting data to ASICs. Need to set these bits to send data to the ASICs'
+      readwrite: rw
+      value: 3
+    ard_tx_en:
+      address: 0x1E
       bitposition: 0
-      bitwidth: 4
-      description: ''
-      readwrite: w
-      value: 0x0
-    transfer:
-      address: 0x18
-      bitposition: 4
-      bitwidth: 8
-      description: ''
-      readwrite: w
-      value: 0xFF
-    unknown:
-      address: 0x19
+      bitwidth: 16
+      description: 'TR-BHM ASIC Tx Enable register 30dec. Bit 0 and 1 enable receiving data from ASICs. Need to set these bits to get data back from the ASICs'
+      readwrite: rw
+      value: 3
+    ard_clk_select_0:
+      address: 0x24
       bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 0x000
-    wbias:
-      address: 0x1A
+      bitwidth: 1
+      description: 'TR-BHM chip 0 phase select\n 00: 0 deg\n 01: 90 deg\n 10: 180 deg\n 11: 270 deg'
+      readwrite: rw
+      value: 0
+    ard_clk_select_1:
+      address: 0x25
       bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: w
-      value: 0x7D0
-
+      bitwidth: 1
+      description: 'TR-BHM chip 1 phase select\n 00: 0 deg\n 01: 90 deg\n 10: 180 deg\n 11: 270 deg'
+      readwrite: rw
+      value: 0
   i2c_registers:
     i2c_en:
       address: 0x0F
       bitposition: 14
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 1
-    i2c_words:
+      value: true
+    i2c_send:
       address: 0x0F
-      bitposition: 8
-      bitwidth: 4
-      description: 'number of words to send in the i2c command.'
+      bitposition: 15
+      bitwidth: 1
+      description: ''
       readwrite: rw
       value: 0
     i2c_addr:
       address: 0x0F
       bitposition: 0
       bitwidth: 8
-      description: 'i2c address for the commands in the string builder'
+      description: ''
       readwrite: rw
       value: 0
     i2c_data0:
       address: 0x10
       bitposition: 0
       bitwidth: 16
-      description: 'Data storage used by the i2c string builder, for both rx and tx data'
+      description: ''
       readwrite: rw
       value: 0
     i2c_data1:
       address: 0x11
       bitposition: 0
       bitwidth: 16
-      description: 'Data storage used by the i2c string builder, for both rx and tx data'
+      description: ''
       readwrite: rw
       value: 0
     i2c_data2:
       address: 0x12
       bitposition: 0
       bitwidth: 16
-      description: 'Data storage used by the i2c string builder, for both rx and tx data'
+      description: ''
       readwrite: rw
       value: 0
     i2c_data3:
       address: 0x13
       bitposition: 0
       bitwidth: 16
-      description: 'Data storage used by the i2c string builder, for both rx and tx data'
+      description: ''
+      readwrite: rw
+      value: 0
+    i2c_words:
+      address: 0x0F
+      bitposition: 8
+      bitwidth: 3
+      description: ''
       readwrite: rw
       value: 0
     response0:
-      address: 0x20
+      address: 0x48
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: r
       value: 0
     response1:
-      address: 0x21
+      address: 0x49
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: r
       value: 0
     response2:
-      address: 0x22
+      address: 0x4A
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: r
       value: 0
     response3:
-      address: 0x23
+      address: 0x4B
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: r
       value: 0
```

### Comparing `naluconfigs-10.8.0/src/naluconfigs/data/registers/upaci.yml` & `naluconfigs-11.0.0/src/naluconfigs/data/registers/asocv3.yml`

 * *Files 7% similar despite different names*

```diff
@@ -1,41 +1,60 @@
-model: upaci
+model: asocv3
+features:
+  adc2mv: true
+  dac_sweep: true
+  ext_dac: true
+  pedestals: true
+  threshold_scan: true
+  tia_dac: false
+  timing_calibration: true
+  naludaq_rs: true
 params:
-  chanmask: 511
-  channels: 32
-  chanshift: 3
+  chanmask: 1536
+  channels: 4
+  chanshift: 9
+  chips:
+    0:
+      !include_chip
+      from: asocv3::params
+  clock_file: Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt
   connections:
     - serial
     - d2xx
+    - udp
+  si5341_address: 0xE8
   default_baud:
-    115200: 434
-  default_baudrate: 115200
-  default_clock: 200000000.0
-  default_divider: 434
-  default_trigger_value: 0
+    115200: 826
+  default_baudrate: 111111
+  default_clock: 96000000.0
+  default_divider: 53
+  expected_scalmon: 2500
+  threshold_scan:
+    min_vref: 0
+    max_vref: 2500
+    start: 500
+    stop: 3500
+    stepsize: 5
+    units: counts
   ext_dac:
-    max_mv: 1200
-    max_counts: 65535
+    chip: ad5671
+    max_mv: 2500
+    max_counts: 4095
     channels:
-      0: 30000
-      8: 30000
-      16: 30000
-      24: 30000
-  trigger:
-    triggers_available: 8
-    max_val: 2047
-    min_val: 0
-    default: false
-  num_trigger_channels: 8
-  expected_scalmon: 2500
-  headers: 0
-  last_window_fix_amount: 47
-  lastbits: 0
-  numregs: 32
-  pedestals_blocks: 8
+      0..3: 2048
+    address_mapping:
+      0..3: 0xC
+    channel_mapping:
+      0: 1
+      1: 0
+      2: 5
+      3: 4
+  headers: 3
+  numregs: 36
+  pedestals_blocks: 32
   peripherals:
     current:
       chan: 0
       addr: 0xD0
       bits: 16
       gain: 8
     vadjn:
@@ -44,747 +63,688 @@
       bits: 16
       gain: 1
     vadjp:
       chan: 1
       addr: 0xD8
       bits: 16
       gain: 1
+    eeprom:
+      addr: 0x50 # 7-bit
+      capacity: 0x20000 # bytes
+      page_size: 256 # bytes
+      segments:
+        analog_registers:
+          begin: 0
+          length: 300
+        digital_registers:
+          begin: 300
+          length: 330
+        control_registers:
+          begin: 630
+          length: 70
   possible_bauds:
-    115200: 434
-    2000000: 25
-  resolution: 11
-  samples: 132
-  samplingrate: 9.2
+    115200: 868
+    2000000: 50
+  roi_enabled: true
+  resolution: 12
+  samples: 64
+  samplingrate: 3.2
   stop_word: !!binary |
     +s4=
   wait: AE000001
-  wbias: 750
-  windmask: 7
-  windows: 8
+  wbias: 848
+  windmask: 510
+  windows: 254
+  yaml_version: 35.0
 registers:
+  analog_registers:
+    !include_registers
+      from: asocv3::registers::analog_registers
+  digital_registers:
+    !include_registers
+      from: asocv3::registers::digital_registers
   control_registers:
-    avdd_en:
-      address: 0x28
+    2v5_en:
+      address: 0x16
       bitposition: 0
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
-    baud_rate_divisor:
-      address: 0x03
+      value: true
+    2v5_pll_en:
+      address: 0x16
+      bitposition: 1
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: false
+    addr:
+      address: 0x15
       bitposition: 0
-      bitwidth: 16
+      bitwidth: 9
       description: ''
       readwrite: rw
-      value: 108
-    cdce62002_power_down_n:
-      address: 0x13
+      value: 0
+    addr_user:
+      address: 0x15
       bitposition: 15
-      bitwidth: 16
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 1
-    cdce62002_read_register_0_lsw:
-      address: 0x92
+      value: false
+    brightness_blue:
+      address: 0x0A
       bitposition: 0
-      bitwidth: 16
+      bitwidth: 8
       description: ''
       readwrite: rw
-      value: 21976
-    cdce62002_read_register_0_msw:
-      address: 0x91
+      value: 0
+    brightness_red:
+      address: 0x0B
       bitposition: 0
-      bitwidth: 16
+      bitwidth: 8
       description: ''
       readwrite: rw
-      value: 1104
-    cdce62002_read_register_1_lsw:
-      address: 0x94
-      bitposition: 0
-      bitwidth: 16
+      value: 0
+    brightness_white:
+      address: 0x0A
+      bitposition: 8
+      bitwidth: 8
       description: ''
       readwrite: rw
-      value: 903
-    cdce62002_read_register_1_msw:
-      address: 0x93
-      bitposition: 0
-      bitwidth: 16
+      value: 0
+    chansel:
+      address: 0x06
+      bitposition: 12
+      bitwidth: 4
       description: ''
       readwrite: rw
-      value: 57376
-    cdce62002_read_register_2_lsw:
-      address: 0x96
-      bitposition: 0
-      bitwidth: 16
+      value: 15
+    clk_1v8_nshutdown:
+      address: 0x16
+      bitposition: 2
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 24832
-    cdce62002_read_register_2_msw:
-      address: 0x95
-      bitposition: 0
-      bitwidth: 16
+      value: true
+    clk_2v5_en:
+      address: 0x16
+      bitposition: 6
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 14850
-    cdce62002_register_0_lsw_out:
-      address: 0x0C
-      bitposition: 0
-      bitwidth: 16
+      value: true
+    clk_i2c_sel:
+      address: 0x16
+      bitposition: 5
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 1104  # same
-    cdce62002_register_0_msw_out:
-      address: 0x0D
-      bitposition: 0
-      bitwidth: 16
+      value: true
+    clk_noe:
+      address: 0x16
+      bitposition: 4
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0x5550  # 21976
-    cdce62002_register_1_lsw_out:
-      address: 0x0E
-      bitposition: 0
-      bitwidth: 16
+      value: false
+    clk_nrst:
+      address: 0x16
+      bitposition: 3
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0xa091  # 57377
-    cdce62002_register_1_msw_out:
-      address: 0x0F
-      bitposition: 0
-      bitwidth: 16
+      value: true
+    clk_nsync:
+      address: 0x16
+      bitposition: 7
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0x838d  # 33671
-    cdce62002_write_strobe:
-      address: 0x13
-      bitposition: 11
+      value: false
+    dac_nrst:
+      address: 0x16
+      bitposition: 10
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
-    conversion_wait_count_value:
+      value: 1
+    data:
       address: 0x14
       bitposition: 0
-      bitwidth: 16
+      bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
-    dac_rovcp_1_out:
-      address: 0x08
-      bitposition: 0
-      bitwidth: 16
-      description: ''
-      readwrite: rw
-      value: 256
-    dac_rovcp_2_out:
-      address: 0x09
-      bitposition: 0
-      bitwidth: 16
+    data_user:
+      address: 0x14
+      bitposition: 15
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 256
-    dac_vbias00_07_out:
-      address: 0x04
-      bitposition: 0
-      bitwidth: 16
+      value: false
+    digrst:
+      address: 0x16
+      bitposition: 9
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 27306
-    dac_vbias08_15_out:
-      address: 0x05
-      bitposition: 0
-      bitwidth: 16
+      value: 0
+    digser_8b10b_en:
+      address: 0x1D
+      bitposition: 12
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 27306
-    dac_vbias16_23_out:
-      address: 0x0A
-      bitposition: 0
-      bitwidth: 16
+      value: false
+    digser_numwords:
+      address: 0x1D
+      bitposition: 2
+      bitwidth: 6
       description: ''
       readwrite: rw
-      value: 27306
-    dac_vbias24_31_out:
-      address: 0x0B
-      bitposition: 0
-      bitwidth: 16
+      value: 0
+    digser_oneshot:
+      address: 0x1D
+      bitposition: 1
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 27306
-    dac_vreset1_2_out:
-      address: 0x06
-      bitposition: 0
-      bitwidth: 16
+      value: false
+    digser_reset:
+      address: 0x1D
+      bitposition: 13
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 11264
-    dac_vreset3_4_out:
-      address: 0x07
+      value: false
+    digser_rx_en:
+      address: 0x1D
       bitposition: 0
-      bitwidth: 16
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 11264
-    dac_write_strobe:
-      address: 0x13
-      bitposition: 12
+      value: false
+    digser_slow_sysclk:
+      address: 0x1D
+      bitposition: 10
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    diagnostic_read_data:
-      address: 0x10
-      bitposition: 4
-      bitwidth: 4
+    digser_speed:
+      address: 0x1D
+      bitposition: 8
+      bitwidth: 2
       description: ''
       readwrite: rw
       value: 0
-    # dll_start:
-    #   address: 0x13
-    #   bitposition: 7
-    #   bitwidth: 1
-    #   description: ''
-    #   readwrite: rw
-    #   value: 0
-    ftdi_cts:
-      address: 0x29
-      bitposition: 2
+    digser_tx_en:
+      address: 0x1D
+      bitposition: 11
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
-    ftdi_rts_bit_0:
-      address: 0x88
-      bitposition: 0
-      bitwidth: 16
-      description: ''
-      readwrite: rw
-      value: 0
-    gpio_pd:
-      address: 0x28
-      bitposition: 2
-      bitwidth: 5
+      value: false
+    ext_en:
+      address: 0x0B
+      bitposition: 9
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
-    gpio_input_header_5:
-      address: 0x85
-      bitposition: 0
-      bitwidth: 8
+      value: true
+    exttrig:
+      address: 0x04
+      bitposition: 10
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 255
-    identifier:
-      address: 0x00
+      value: false
+    fake:
+      address: 0x06
       bitposition: 0
-      bitwidth: 16
-      description: ''
-      readwrite: rw
-      value: 57005
-    # mclk_clock_monitor:
-    #   address: 0x28
-    #   bitposition: 10
-    #   bitwidth: 1
-    #   description: ''
-    #   readwrite: rw
-    #   value: 0
-    optical_trigger_en:
-      address: 0x29
-      bitposition: 4
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    optical_trigger_input_bit_0:
-      address: 0x8A
-      bitposition: 0
-      bitwidth: 16
+    gccclr:
+      address: 0x04
+      bitposition: 3
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
-    pd_bias_en:
-      address: 0x29
-      bitposition: 1
+      value: false
+    i2c_sel:
+      address: 0x16
+      bitposition: 11
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
-    # pll_clock_monitor:
-    #   address: 0x28
-    #   bitposition: 9
-    #   bitwidth: 1
-    #   description: ''
-    #   readwrite: rw
-    #   value: 1
-    # pll_clockout:
-    #   address: 0x28
-    #   bitposition: 11
-    #   bitwidth: 1
-    #   description: ''
-    #   readwrite: rw
-    #   value: 0
-    pll_lock_bit_0:
-      address: 0x86
-      bitposition: 0
-      bitwidth: 16
+      value: true
+    i2c_switch:
+      address: 0x16
+      bitposition: 8
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 1
-    psec4a_a_ro_feedback_calculated_value:
-      address: 0xA8
+      value: 0
+    identifier:
+      address: 0x00
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
-      value: 247
-    psec4a_a_ro_monitor_clock_count_lsw:
-      address: 0x99
+      value: 42435
+    version:
+      address: 0x01
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
-    psec4a_a_ro_monitor_clock_count_msw:
-      address: 0x98
-      bitposition: 0
-      bitwidth: 16
+    in_sel:
+      address: 0x0B
+      bitposition: 12
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
-    psec4a_a_vcdl_monitor_clock_count_lsw:
-      address: 0xA1
-      bitposition: 0
-      bitwidth: 16
+      value: true
+    iomode0:
+      address: 0x04
+      bitposition: 7
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
-    psec4a_a_vcdl_monitor_clock_count_msw:
-      address: 0xA0
-      bitposition: 0
-      bitwidth: 16
+      value: 1
+    iomode1:
+      address: 0x04
+      bitposition: 8
+      bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    psec4a_b_ro_feedback_calculated_value:
-      address: 0xA9
-      bitposition: 0
-      bitwidth: 16
+    loadwait:
+      address: 0x07
+      bitposition: 8
+      bitwidth: 4
       description: ''
       readwrite: rw
-      value: 269
-    psec4a_b_ro_monitor_clock_count_lsw:
-      address: 0x9B
-      bitposition: 0
-      bitwidth: 16
+      value: 15
+    nasa_trig_sel_ext:
+      address: 0x1D
+      bitposition: 15
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
-    psec4a_b_ro_monitor_clock_count_msw:
-      address: 0x9A
-      bitposition: 0
-      bitwidth: 16
+      value: true
+    nramp:
+      address: 0x04
+      bitposition: 4
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
-    psec4a_b_vcdl_monitor_clock_count_lsw:
-      address: 0xA3
-      bitposition: 0
-      bitwidth: 16
+      value: false
+    nrw:
+      address: 0x04
+      bitposition: 11
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
-    psec4a_b_vcdl_monitor_clock_count_msw:
-      address: 0xA2
+      value: false
+    numwinds:
+      address: 0x08
       bitposition: 0
-      bitwidth: 16
+      bitwidth: 8
       description: ''
       readwrite: rw
-      value: 0
-    psec4a_biascomp_out:
-      address: 0x1A
-      bitposition: 0
-      bitwidth: 16
+      value: 1
+    out_sel:
+      address: 0x0B
+      bitposition: 11
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 512
-    psec4a_biasdllfirst_out:
-      address: 0x1C
-      bitposition: 0
-      bitwidth: 16
+      value: false
+    pclk:
+      address: 0x04
+      bitposition: 1
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 256
-    psec4a_biasdlllast_out:
-      address: 0x1B
-      bitposition: 0
-      bitwidth: 16
+      value: false
+    pclkwidth:
+      address: 0x07
+      bitposition: 12
+      bitwidth: 4
       description: ''
       readwrite: rw
-      value: 256
-    psec4a_biasdlln_out:
-      address: 0x1E
-      bitposition: 0
-      bitwidth: 16
+      value: 15
+    rden:
+      address: 0x04
+      bitposition: 6
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 592
-    psec4a_biasdllp_out:
-      address: 0x1D
+      value: false
+    regclr:
+      address: 0x04
       bitposition: 0
-      bitwidth: 16
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 416
-    psec4a_biasrampbuf_out:
-      address: 0x19
+      value: false
+    runevs:
+      address: 0x05
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
-      value: 432
-    psec4a_biasrampslope_out:
-      address: 0x27
+      value: 1
+    rx_data0:
+      address: 0x1A
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
-    psec4a_biastrign_out:
-      address: 0x17
-      bitposition: 0
-      bitwidth: 16
-      description: ''
-      readwrite: rw
-      value: 0x0200  # 0
-    psec4a_biasxfer_out:
-      address: 0x18
+    rx_data1:
+      address: 0x1B
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
-      value: 512
-    psec4a_mclk_source_clock_count_lsw:
-      address: 0x8F
-      bitposition: 0
-      bitwidth: 16
-      description: 'Read-only Debug clock, should be the same as VCDL when read out'
-      readwrite: r
-      value: 0
-    psec4a_mclk_source_clock_count_msw:
-      address: 0x8E
-      bitposition: 0
-      bitwidth: 16
-      description: 'Read-only Debug clock, should be the same as VCDL when read out'
-      readwrite: r
       value: 0
-    psec4a_c_ro_feedback_calculated_value:
-      address: 0xAA
+    rx_data2:
+      address: 0x1C
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
-      value: 326
-    psec4a_c_ro_monitor_clock_count_lsw:
-      address: 0x9D
+      value: 0
+    rx_data4:
+      address: 0x1E
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
-    psec4a_c_ro_monitor_clock_count_msw:
-      address: 0x9C
+    rx_data5:
+      address: 0x1F
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
-    psec4a_c_vcdl_monitor_clock_count_lsw:
-      address: 0xA5
+    rx_data6:
+      address: 0x20
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
-    psec4a_c_vcdl_monitor_clock_count_msw:
-      address: 0xA4
+    rx_en:
+      address: 0x19
       bitposition: 0
-      bitwidth: 16
+      bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    psec4a_d_ro_feedback_calculated_value:
-      address: 0xAB
-      bitposition: 0
-      bitwidth: 16
+    rx_num_words:
+      address: 0x19
+      bitposition: 2
+      bitwidth: 6
       description: ''
       readwrite: rw
-      value: 246
-    psec4a_d_ro_monitor_clock_count_lsw:
-      address: 0x9F
-      bitposition: 0
-      bitwidth: 16
+      value: 0
+    rx_oneshot:
+      address: 0x19
+      bitposition: 1
+      bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    psec4a_d_ro_monitor_clock_count_msw:
-      address: 0x9E
-      bitposition: 0
-      bitwidth: 16
+    rx_speed:
+      address: 0x19
+      bitposition: 8
+      bitwidth: 2
       description: ''
       readwrite: rw
       value: 0
-    psec4a_d_vcdl_monitor_clock_count_lsw:
-      address: 0xA7
-      bitposition: 0
-      bitwidth: 16
+    sel:
+      address: 0x04
+      bitposition: 12
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
-    psec4a_d_vcdl_monitor_clock_count_msw:
-      address: 0xA6
-      bitposition: 0
-      bitwidth: 16
+      value: false
+    selany:
+      address: 0x04
+      bitposition: 2
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
-    # psec4a_mode:
-    #   address: 0x13
-    #   bitposition: 5
-    #   bitwidth: 2
-    #   description: ''
-    #   readwrite: rw
-    #   value: 0
-    xref_address_mode:
-      address: 0x13
-      bitposition: 5
+      value: false
+    sst_speed:
+      address: 0x1D
+      bitposition: 14
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
-    psec4a_rovcp:
-      address: 0x16
-      bitposition: 0
-      bitwidth: 16
+      value: false
+    stopacq:
+      address: 0x04
+      bitposition: 13
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 300
-    psec4a_status:
-      address: 0x84
-      bitposition: 0
-      bitwidth: 16
+      value: false
+    switch_nen:
+      address: 0x0B
+      bitposition: 13
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 4852
-    psec4a_trigthresh1_out:
-      address: 0x1F
+      value: true
+    syncloc:
+      address: 0x0E
       bitposition: 0
-      bitwidth: 16
+      bitwidth: 8
       description: ''
       readwrite: rw
-      value: 1536  # 0
-    psec4a_trigthresh2_out:
-      address: 0x20
-      bitposition: 0
-      bitwidth: 16
+      value: 0
+    sysrst:
+      address: 0x04
+      bitposition: 14
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 1536  # 0
-    psec4a_trigthresh3_out:
-      address: 0x21
-      bitposition: 0
-      bitwidth: 16
+      value: false
+    trig_sel:
+      address: 0x0B
+      bitposition: 10
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 1536  # 0
-    psec4a_trigthresh4_out:
+      value: false
+    trigger_mux:
       address: 0x22
+      bitposition: 5
+      bitwidth: 4
+      description: 'Change which trigger type is used to trigger the chip, there are 8 diffeerent modes.'
+      readwrite: rw
+      value: 8
+    windsel:
+      address: 0x07
       bitposition: 0
-      bitwidth: 16
+      bitwidth: 8
       description: ''
       readwrite: rw
-      value: 1536  # 0
-    psec4a_trigthresh5_out:
-      address: 0x23
-      bitposition: 0
-      bitwidth: 16
+      value: 0
+    wren:
+      address: 0x04
+      bitposition: 5
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 1536  # 0
-    psec4a_trigthresh6_out:
-      address: 0x24
+      value: false
+    eth_addr_sel:
+      address: 0x28
       bitposition: 0
-      bitwidth: 16
-      description: ''
+      bitwidth: 2
+      description: 'enables manually set destination (bit 0) and source (bit 1) IP addresses'
+      readwrite: rw
+      value: 0
+    eth_port_sel:
+      address: 0x28
+      bitposition: 2
+      bitwidth: 2
+      description: 'enables manually set destination (bit 0) and source (bit 1) UDP ports'
+      readwrite: rw
+      value: 0
+    tx_mode:
+      address: 0x28
+      bitposition: 4
+      bitwidth: 1
+      description: 'selects ethernet (value = 1) or UART (value = 0) transmission'
+      readwrite: rw
+      value: 0
+    eth_ar_en:
+      address: 0x28
+      bitposition: 5
+      bitwidth: 1
+      description: 'enables auto-response destination IP address; currently unused'
       readwrite: rw
-      value: 1536  # 0
-    psec4a_trigthresh7_out:
-      address: 0x25
+      value: 0
+    eth_dhcp_en:
+      address: 0x28
+      bitposition: 6
+      bitwidth: 1
+      description: 'enables DHCP resolution of source IP address; currently unused'
+      readwrite: rw
+      value: 0
+    eth_dest_addr15_0:
+      address: 0x29
       bitposition: 0
       bitwidth: 16
-      description: ''
+      description: 'lower 16 bits of ethernet destination IP address'
       readwrite: rw
-      value: 1536  # 0
-    psec4a_trigthresh8_out:
-      address: 0x26
+      value: 0
+    eth_dest_addr31_16:
+      address: 0x2A
       bitposition: 0
       bitwidth: 16
-      description: ''
+      description: 'upper 16 bits of ethernet destination IP address'
       readwrite: rw
-      value: 1536  # 0
-    reread_data:
-      address: 0x10
-      bitposition: 9
-      bitwidth: 1
-      description: ''
+      value: 0
+    eth_src_addr15_0:
+      address: 0x2B
+      bitposition: 0
+      bitwidth: 16
+      description: 'lower 16 bits of ethernet source IP address'
       readwrite: rw
       value: 0
-    ring_oscillator_feedback_target_value_lsw:
-      address: 0x11
+    eth_src_addr31_16:
+      address: 0x2C
       bitposition: 0
       bitwidth: 16
-      description: ''
+      description: 'upper 16 bits of ethernet source IP address'
       readwrite: rw
-      value: 29529
-    ring_oscillator_feedback_target_value_msw:
-      address: 0x12
+      value: 0
+    eth_dest_port:
+      address: 0x2D
       bitposition: 0
       bitwidth: 16
-      description: ''
+      description: 'UDP destination port'
       readwrite: rw
-      value: 7
-    ro_feedback_enable:
-      address: 0x13
+      value: 0
+    eth_src_port:
+      address: 0x2E
       bitposition: 0
+      bitwidth: 16
+      description: 'UDP source port'
+      readwrite: rw
+      value: 0
+  i2c_registers:
+    i2c_en:
+      address: 0x09
+      bitposition: 14
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 1
-    ro_monitor_reset:
-      address: 0x29
-      bitposition: 3
+      value: true
+    i2c_send:
+      address: 0x0F
+      bitposition: 15
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    self_trigger_or_enable:
-      address: 0x13
-      bitposition: 6
-      bitwidth: 1
-      description: 'Enable Self Trigger OR function in PSEC4A'
-      readwrite: rw
-      value: 1
-    serial_data_select:
-      address: 0x28
-      bitposition: 12
-      bitwidth: 4
+    i2c_words:
+      address: 0x0F
+      bitposition: 8
+      bitwidth: 3
       description: ''
       readwrite: rw
       value: 0
-    serial_write_strobe:
-      address: 0x10
+    i2c_addr:
+      address: 0x0F
       bitposition: 0
-      bitwidth: 1
+      bitwidth: 8
       description: ''
       readwrite: rw
       value: 0
-    software_trigger:
-      address: 0x13
-      bitposition: 4
-      bitwidth: 1
+    i2c_data0:
+      address: 0x10
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
-    speed_select:
-      address: 0x13
-      bitposition: 3
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: 1
-    # system_clock_monitor:
-    #   address: 0x28
-    #   bitposition: 8
-    #   bitwidth: 1
-    #   description: ''
-    #   readwrite: rw
-    #   value: 1
-    trig_out1:
-      address: 0x90
+    i2c_data1:
+      address: 0x11
       bitposition: 0
-      bitwidth: 4
-      description: 'DCBA chiporder'
-      readwrite: rw
-      value: 0
-    trigger_mask_enable:
-      address: 0x29
-      bitposition: 8
-      bitwidth: 8
-      description: 'Trigger mask where each bit is a corresponding chip'
-      readwrite: rw
-      value: 255  # '11111111'
-    trigger_mode:
-      address: 0x29
-      bitposition: 5
-      bitwidth: 2
-      description: '<html><head/><body><p>Set the triggermode:<br/>
-        00: Software Trigger, the default.<br/>
-        01: Auto Trigger, 2Hz auto trigger rate.<br/>
-        10: External Trigger, trigger on trig in.<br/>
-        11: Self Trigger, trigger on signal levels.
-        </p></body></html>'
+      bitwidth: 16
+      description: ''
       readwrite: rw
       value: 0
-    trigger_reset:
-      address: 0x13
-      bitposition: 13
-      bitwidth: 1
+    i2c_data2:
+      address: 0x12
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
-    # trigger_scaler:
-    #   address: 0x97
-    #   bitposition: 0
-    #   bitwidth: 8
-    #   description: ''
-    #   readwrite: rw
-    #   value: 0
-    trigger_sign:
+    i2c_data3:
       address: 0x13
-      bitposition: 1
-      bitwidth: 1
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
-    uart_status:
-      address: 0x81
+    response0:
+      address: 0x2C
       bitposition: 0
-      bitwidth: 8
-      description: ''
-      readwrite: rw
-      value: 84
-    uart_handshake_en_out:
-      address: 0x10
-      bitposition: 8
-      bitwidth: 1
+      bitwidth: 16
       description: ''
-      readwrite: rw
-      value: false
-    version_number:
-      address: 0x80
+      readwrite: r
+      value: 0
+    response1:
+      address: 0x2D
       bitposition: 0
       bitwidth: 16
       description: ''
-      readwrite: rw
-      value: 4101
-    wave_fifo_reset:
-      address: 0x10
-      bitposition: 1
-      bitwidth: 1
+      readwrite: r
+      value: 0
+    response2:
+      address: 0x2E
+      bitposition: 0
+      bitwidth: 16
       description: ''
-      readwrite: rw
+      readwrite: r
       value: 0
-    xfer_reset:
-      address: 0x13
-      bitposition: 2
-      bitwidth: 1
+    response3:
+      address: 0x2F
+      bitposition: 0
+      bitwidth: 16
       description: ''
-      readwrite: rw
-      value: 1
+      readwrite: r
+      value: 0
```

### Comparing `naluconfigs-10.8.0/src/naluconfigs/data/registers/zdigitizer.yml` & `naluconfigs-11.0.0/src/naluconfigs/data/registers/aodsoc_aods.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,790 +1,696 @@
-model: zdigitizer
+model: aodsoc_aods
+features:
+  adc2mv: true
+  dac_sweep: true
+  ext_dac: true
+  pedestals: true
+  threshold_scan: true
+  tia_dac: false
+  timing_calibration: false
+  naludaq_rs: true
 params:
-  chanmask: 511
-  channels: 32
-  chanshift: 3
+  chanmask: 0x300
+  channels: 8
+  chanshift: 8
+  chips:
+    0..1:
+      !include_chip
+      from: aodsv2::params
+  # clock_file: '' # AODSoC boards have fixed clocks
   connections:
     - serial
     - d2xx
+  si5341_address: 0xEE
+  timing_hack: false
   default_baud:
-    115200: 217
+    115200: 868
   default_baudrate: 115200
-  default_clock: 200000000.0
-  default_divider: 217
-  default_trigger_value: 0
+  default_clock: 100000000.0
+  default_divider: 868
+  default_trigger_value: 1500
+  threshold_scan:
+    min_vref: 0
+    max_vref: 2500
+    start: 500
+    stop: 3500
+    stepsize: 5
+    units: counts
+  expected_scalmon: 2500
   ext_dac:
-    max_mv: 1200
-    max_counts: 65535
+    chip: dac7578
+    max_mv: 2500
+    max_counts: 4095
     channels:
-      0: 30000
-      8: 30000
-      16: 30000
-      24: 30000
-  trigger:
-    triggers_available: 8
-    max_val: 2047
-    min_val: 0
-    default: false
-  num_trigger_channels: 8
-  expected_scalmon: 2500
-  headers: 0
-  last_window_fix_amount: 47
-  lastbits: 0
-  numregs: 32
-  pedestals_blocks: 8
+      0..7: 2048
+    address_mapping:
+      0..7: 0x48
+    channel_mapping:
+      0: 7
+      1: 5
+      2: 3
+      3: 1
+      4: 0
+      5: 2
+      6: 4
+      7: 6
+  headers: 3
+  numregs: 64
+  pedestals_blocks: 16
   peripherals:
-    current:
-      chan: 0
-      addr: 0xD0
-      bits: 16
-      gain: 8
-    vadjn:
-      chan: 0
-      addr: 0xD8
-      bits: 16
-      gain: 1
-    vadjp:
+    vadjn_0:
+      chan: 3
+      addr: 0x4C
+    vadjn_1:
+      chan: 2
+      addr: 0x4C
+    ldo_voltage:
       chan: 1
-      addr: 0xD8
-      bits: 16
-      gain: 1
+      addr: 0x4C
+    chip_voltage:
+      chan: 2
+      addr: 0x4C
+    current_resistor: 0.010
   possible_bauds:
-    115200: 217
-    1000000: 25
-  resolution: 11
-  samples: 132
-  samplingrate: 9.2
-  stop_word: !!binary |
-    +s4=
+    115200: 868
+    1000000: 100
+    2000000: 50
+    3000000: 33
+  resolution: 12
+  samples: 64
+  samplingrate: 1.0
+  stop_word: "cafe"
   wait: AE000001
-  wbias: 750
-  windmask: 7
-  windows: 8
+  wbias: 848
+  windmask: 0x0FF
+  windows: 254
 registers:
+  analog_registers:
+    !include_registers
+      from: aodsv2::registers::analog_registers
+      value_count: 2
+      override:
+        isel:
+          value: [2610, 2627]
+        sel_4:
+          value: [0, 0]
+  digital_registers:
+    !include_registers
+      from: aodsv2::registers::digital_registers
+      value_count: 2
   control_registers:
-    avdd_en:
-      address: 0x28
+    i2c_bus_sel:
+      address: 0x14
       bitposition: 0
       bitwidth: 1
+      description: 'Select i2c bus 1 or 2, 0: i2c bus 1, 1: i2c bus 2'
+      readwrite: rw
+      value: false
+    1v2_en:
+      address: 0x17
+      bitposition: 1
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
-    baud_rate_divisor:
-      address: 0x03
+      value: true
+    2v5_en:
+      address: 0x17
       bitposition: 0
-      bitwidth: 16
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 108
-    cdce62002_power_down_n:
-      address: 0x13
-      bitposition: 15
-      bitwidth: 16
+      value: true
+    3v3_i2c_en:
+      address: 0x17
+      bitposition: 2
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 1
-    cdce62002_read_register_0_lsw:
-      address: 0x92
-      bitposition: 0
-      bitwidth: 16
+      value: true
+    8b10b_en:
+      address: 0x19
+      bitposition: 12
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 21976
-    cdce62002_read_register_0_msw:
-      address: 0x91
+      value: 0
+    amp_pwrdn_out:
+      address: 0x1A
       bitposition: 0
-      bitwidth: 16
-      description: ''
+      bitwidth: 8
+      description: 'Onboard amplifiers active high means amp off'
       readwrite: rw
-      value: 1104
-    cdce62002_read_register_1_lsw:
-      address: 0x94
+      value: 0
+    addr:
+      address: 0x16
       bitposition: 0
-      bitwidth: 16
+      bitwidth: 9
       description: ''
       readwrite: rw
-      value: 903
-    cdce62002_read_register_1_msw:
-      address: 0x93
-      bitposition: 0
-      bitwidth: 16
+      value: 0
+    addr_user:
+      address: 0x16
+      bitposition: 15
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 57376
-    cdce62002_read_register_2_lsw:
-      address: 0x96
-      bitposition: 0
-      bitwidth: 16
+      value: false
+    chansel:
+      address: 0x06
+      bitposition: 12
+      bitwidth: 4
       description: ''
       readwrite: rw
-      value: 24832
-    cdce62002_read_register_2_msw:
-      address: 0x95
-      bitposition: 0
-      bitwidth: 16
+      value: 15
+    clk1v8_en:
+      address: 0x17
+      bitposition: 4
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 14850
-    cdce62002_register_0_lsw_out:
-      address: 0x0C
-      bitposition: 0
-      bitwidth: 16
+      value: true
+    clk2v5_en:
+      address: 0x17
+      bitposition: 3
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 1104  # same
-    cdce62002_register_0_msw_out:
-      address: 0x0D
-      bitposition: 0
-      bitwidth: 16
+      value: true
+    clk_fdec:
+      address: 0x17
+      bitposition: 9
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0x5550  # 21976
-    cdce62002_register_1_lsw_out:
-      address: 0x0E
-      bitposition: 0
-      bitwidth: 16
+      value: false
+    clk_finc:
+      address: 0x17
+      bitposition: 8
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0xa091  # 57377
-    cdce62002_register_1_msw_out:
-      address: 0x0F
-      bitposition: 0
-      bitwidth: 16
+      value: false
+    clk_i2c_sel:
+      address: 0x17
+      bitposition: 5
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0x838d  # 33671
-    cdce62002_write_strobe:
-      address: 0x13
-      bitposition: 11
+      value: true
+    clk_oeb:
+      address: 0x17
+      bitposition: 6
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
-    conversion_wait_count_value:
-      address: 0x14
+      value: false
+    clk_reset:
+      address: 0x17
+      bitposition: 7
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: false
+    clk_sync:
+      address: 0x17
+      bitposition: 10
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: false
+    debug_data:
+      address: 0x15
       bitposition: 0
-      bitwidth: 16
+      bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
-    dac_rovcp_1_out:
-      address: 0x08
-      bitposition: 0
-      bitwidth: 16
+    debug_data_user:
+      address: 0x15
+      bitposition: 15
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 256
-    dac_rovcp_2_out:
-      address: 0x09
-      bitposition: 0
-      bitwidth: 16
+      value: false
+    digrst:
+      address: 0x16
+      bitposition: 9
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: 0
+    digser_rst:
+      address: 0x19
+      bitposition: 13
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 256
-    dac_vbias00_07_out:
+      value: 0
+    exttrig:
       address: 0x04
-      bitposition: 0
-      bitwidth: 16
+      bitposition: 10
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 27306
-    dac_vbias08_15_out:
-      address: 0x05
-      bitposition: 0
-      bitwidth: 16
+      value: false
+    gccclr:
+      address: 0x04
+      bitposition: 4
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 27306
-    dac_vbias16_23_out:
-      address: 0x0A
+      value: false
+    idac_ldac:
+      address: 0x1B
       bitposition: 0
-      bitwidth: 16
-      description: ''
+      bitwidth: 1
+      description: 'pin on AD7578'
       readwrite: rw
-      value: 27306
-    dac_vbias24_31_out:
-      address: 0x0B
+      value: 0
+    idac_nclr:
+      address: 0x1B
+      bitposition: 1
+      bitwidth: 1
+      description: 'pin on AD7578'
+      readwrite: rw
+      value: 1
+    fifo_unload_or_event_en:
+      address: 0x1F
       bitposition: 0
-      bitwidth: 16
-      description: ''
+      bitwidth: 1
+      description: 'Once data is loaded into the FIFO it will not be sent out to the UART until the end of the current event. Use this mode for capturing sampled data events. '
       readwrite: rw
-      value: 27306
-    dac_vreset1_2_out:
-      address: 0x06
+      value: 0
+    identifier:
+      address: 0x00
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
-      value: 11264
-    dac_vreset3_4_out:
-      address: 0x07
+      value: 310
+    iomode0:
+      address: 0x04
       bitposition: 0
-      bitwidth: 16
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 11264
-    dac_write_strobe:
-      address: 0x13
-      bitposition: 12
+      value: true
+    iomode1:
+      address: 0x04
+      bitposition: 6
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
-    diagnostic_read_data:
-      address: 0x10
-      bitposition: 4
-      bitwidth: 4
+      value: false
+    leds:
+      address: 0x18
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
-    # dll_start:
-    #   address: 0x13
-    #   bitposition: 7
-    #   bitwidth: 1
-    #   description: ''
-    #   readwrite: rw
-    #   value: 0
-    ftdi_cts:
-      address: 0x29
-      bitposition: 2
-      bitwidth: 1
+    loadwait:
+      address: 0x07
+      bitposition: 8
+      bitwidth: 4
       description: ''
       readwrite: rw
-      value: 0
-    ftdi_rts_bit_0:
-      address: 0x88
-      bitposition: 0
-      bitwidth: 16
+      value: 15
+    nramp:
+      address: 0x04
+      bitposition: 5
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
-    gpio_pd:
-      address: 0x28
-      bitposition: 2
-      bitwidth: 5
+      value: false
+    nrw:
+      address: 0x04
+      bitposition: 11
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
-    gpio_input_header_5:
-      address: 0x85
+      value: false
+    numwinds:
+      address: 0x08
       bitposition: 0
       bitwidth: 8
       description: ''
       readwrite: rw
-      value: 255
-    identifier:
-      address: 0x00
-      bitposition: 0
-      bitwidth: 16
+      value: 1
+    pclk:
+      address: 0x04
+      bitposition: 2
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 57005
-    # mclk_clock_monitor:
-    #   address: 0x28
-    #   bitposition: 10
-    #   bitwidth: 1
-    #   description: ''
-    #   readwrite: rw
-    #   value: 0
-    optical_trigger_en:
-      address: 0x29
-      bitposition: 4
-      bitwidth: 1
+      value: false
+    pclkwidth:
+      address: 0x07
+      bitposition: 12
+      bitwidth: 4
       description: ''
       readwrite: rw
-      value: 0
-    optical_trigger_input_bit_0:
-      address: 0x8A
+      value: 15
+    ramplen:
+      address: 0x06
       bitposition: 0
-      bitwidth: 16
+      bitwidth: 12
       description: ''
       readwrite: rw
-      value: 0
-    pd_bias_en:
-      address: 0x29
+      value: 2000
+    regclr:
+      address: 0x04
       bitposition: 1
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
-    # pll_clock_monitor:
-    #   address: 0x28
-    #   bitposition: 9
-    #   bitwidth: 1
-    #   description: ''
-    #   readwrite: rw
-    #   value: 1
-    # pll_clockout:
-    #   address: 0x28
-    #   bitposition: 11
-    #   bitwidth: 1
-    #   description: ''
-    #   readwrite: rw
-    #   value: 0
-    pll_lock_bit_0:
-      address: 0x86
+      value: false
+    runevs:
+      address: 0x05
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
       value: 1
-    # psec4a_mclk_source_clock_count_lsw:
-    #   address: 0x8F
-    #   bitposition: 0
-    #   bitwidth: 16
-    #   description: 'Read-only Debug clock, should be the same as VCDL when read out'
-    #   readwrite: r
-    #   value: 0
-    # psec4a_mclk_source_clock_count_msw:
-    #   address: 0x8E
-    #   bitposition: 0
-    #   bitwidth: 16
-    #   description: 'Read-only Debug clock, should be the same as VCDL when read out'
-    #   readwrite: r
-    #   value: 0
-    psec4a_a_ro_feedback_calculated_value:
-      address: 0xA8
-      bitposition: 0
-      bitwidth: 16
-      description: ''
-      readwrite: rw
-      value: 247
-    psec4a_a_ro_monitor_clock_count_lsw:
-      address: 0x99
+    rx_en:
+      address: 0x19
       bitposition: 0
-      bitwidth: 16
+      bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    psec4a_a_ro_monitor_clock_count_msw:
-      address: 0x98
-      bitposition: 0
-      bitwidth: 16
+    rx_num_words:
+      address: 0x19
+      bitposition: 2
+      bitwidth: 6
       description: ''
       readwrite: rw
       value: 0
-    psec4a_a_vcdl_monitor_clock_count_lsw:
-      address: 0xA1
-      bitposition: 0
-      bitwidth: 16
+    rx_oneshot:
+      address: 0x19
+      bitposition: 1
+      bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    psec4a_a_vcdl_monitor_clock_count_msw:
-      address: 0xA0
-      bitposition: 0
-      bitwidth: 16
+    rx_speed:
+      address: 0x19
+      bitposition: 8
+      bitwidth: 2
       description: ''
       readwrite: rw
       value: 0
-    psec4a_b_ro_feedback_calculated_value:
-      address: 0xA9
-      bitposition: 0
-      bitwidth: 16
+    sel:
+      address: 0x04
+      bitposition: 12
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 269
-    psec4a_b_ro_monitor_clock_count_lsw:
-      address: 0x9B
-      bitposition: 0
-      bitwidth: 16
+      value: false
+    selany:
+      address: 0x04
+      bitposition: 3
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
-    psec4a_b_ro_monitor_clock_count_msw:
-      address: 0x9A
-      bitposition: 0
-      bitwidth: 16
+      value: false
+    slow_sysclk:
+      address: 0x19
+      bitposition: 10
+      bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    psec4a_b_vcdl_monitor_clock_count_lsw:
-      address: 0xA3
-      bitposition: 0
-      bitwidth: 16
+    stopacq:
+      address: 0x04
+      bitposition: 13
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
-    psec4a_b_vcdl_monitor_clock_count_msw:
-      address: 0xA2
+      value: false
+    syncloc:
+      address: 0x09
       bitposition: 0
-      bitwidth: 16
+      bitwidth: 8
       description: ''
       readwrite: rw
       value: 0
-    psec4a_biascomp_out:
-      address: 0x1A
-      bitposition: 0
-      bitwidth: 16
-      description: ''
-      readwrite: rw
-      value: 512
-    psec4a_biasdllfirst_out:
-      address: 0x1C
-      bitposition: 0
-      bitwidth: 16
+    sysclk:
+      address: 0x04
+      bitposition: 8
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 256
-    psec4a_biasdlllast_out:
-      address: 0x1B
-      bitposition: 0
-      bitwidth: 16
+      value: false
+    sysrst:
+      address: 0x04
+      bitposition: 9
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 256
-    psec4a_biasdlln_out:
-      address: 0x1E
-      bitposition: 0
-      bitwidth: 16
+      value: true
+    tx_en:
+      address: 0x19
+      bitposition: 11
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 592
-    psec4a_biasdllp_out:
-      address: 0x1D
+      value: 0
+    windsel:
+      address: 0x07
       bitposition: 0
-      bitwidth: 16
+      bitwidth: 8
       description: ''
       readwrite: rw
-      value: 416
-    psec4a_biasrampbuf_out:
-      address: 0x19
-      bitposition: 0
-      bitwidth: 16
+      value: 0
+    wrstrboff:
+      address: 0x04
+      bitposition: 7
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 432
-    psec4a_biasrampslope_out:
-      address: 0x27
+      value: false
+    rxout_pol:
+      address: 0x22
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0
-    psec4a_biastrign_out:
-      address: 0x17
+      value: 6400
+    txin_pol:
+      address: 0x23
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0x0200  # 0
-    psec4a_biasxfer_out:
-      address: 0x18
+      value: 4412
+    ard_header:
+      address: 0x21
       bitposition: 0
-      bitwidth: 16
-      description: ''
+      bitwidth: 1
+      description: 'Enable AARDVARC debug header.'
       readwrite: rw
-      value: 512
-    psec4a_c_ro_feedback_calculated_value:
-      address: 0xAA
+      value: 1
+    ard_rx_en:
+      address: 0x1D
       bitposition: 0
       bitwidth: 16
-      description: ''
+      description: 'TR-BHM ASIC Rx Enable register 29dec. Bit 0 and 1 enable transmitting data to ASICs. Need to set these bits to send data to the ASICs'
       readwrite: rw
-      value: 326
-    psec4a_c_ro_monitor_clock_count_lsw:
-      address: 0x9D
+      value: 3
+    ard_tx_en:
+      address: 0x1E
       bitposition: 0
       bitwidth: 16
-      description: ''
+      description: 'TR-BHM ASIC Tx Enable register 30dec. Bit 0 and 1 enable receiving data from ASICs. Need to set these bits to get data back from the ASICs'
       readwrite: rw
-      value: 0
-    psec4a_c_ro_monitor_clock_count_msw:
-      address: 0x9C
+      value: 3
+    ard0_clk_sel:
+      address: 0x24
       bitposition: 0
-      bitwidth: 16
+      bitwidth: 2
       description: ''
       readwrite: rw
       value: 0
-    psec4a_c_vcdl_monitor_clock_count_lsw:
-      address: 0xA5
+    ard1_clk_sel:
+      address: 0x25
       bitposition: 0
-      bitwidth: 16
+      bitwidth: 2
       description: ''
       readwrite: rw
-      value: 0
-    psec4a_c_vcdl_monitor_clock_count_msw:
-      address: 0xA4
+      value: 1
+    motor_trig_en:
+      address: 0x27
       bitposition: 0
-      bitwidth: 16
+      bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    psec4a_d_ro_feedback_calculated_value:
-      address: 0xAB
+    motor_trig_evts:
+      address: 0x26
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
-      value: 246
-    psec4a_d_ro_monitor_clock_count_lsw:
-      address: 0x9F
-      bitposition: 0
-      bitwidth: 16
+      value: 1
+    oleas_en_trig:
+      address: 0x0A
+      bitposition: 10
+      bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    psec4a_d_ro_monitor_clock_count_msw:
-      address: 0x9E
-      bitposition: 0
-      bitwidth: 16
+    oleas_pol_a:
+      address: 0x0A
+      bitposition: 11
+      bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    psec4a_d_vcdl_monitor_clock_count_lsw:
-      address: 0xA7
-      bitposition: 0
-      bitwidth: 16
+    oleas_pol_b:
+      address: 0x0A
+      bitposition: 12
+      bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    psec4a_d_vcdl_monitor_clock_count_msw:
-      address: 0xA6
-      bitposition: 0
-      bitwidth: 16
+    oleas_en_a:
+      address: 0x0A
+      bitposition: 13
+      bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    # psec4a_mode:
-    #   address: 0x13
-    #   bitposition: 5
-    #   bitwidth: 2
-    #   description: ''
-    #   readwrite: rw
-    #   value: 0
-    xref_address_mode:
-      address: 0x13
-      bitposition: 5
+    oleas_en_b:
+      address: 0x0A
+      bitposition: 14
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    psec4a_rovcp:
-      address: 0x16
+    oleas_loop:
+      address: 0x0A
       bitposition: 0
-      bitwidth: 16
+      bitwidth: 5
       description: ''
       readwrite: rw
-      value: 300
-    psec4a_status:
-      address: 0x84
+      value: 15
+    oleas_length_a:
+      address: 0x0B
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
-      value: 4852
-    psec4a_trigthresh1_out:
-      address: 0x1F
+      value: 0
+    oleas_length_b:
+      address: 0x0D
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
-      value: 1536  # 0
-    psec4a_trigthresh2_out:
-      address: 0x20
+      value: 0
+    oleas_delay_a:
+      address: 0x0C
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
-      value: 1536  # 0
-    psec4a_trigthresh3_out:
-      address: 0x21
+      value: 0
+    oleas_delay_b:
+      address: 0x0E
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
-      value: 1536  # 0
-    psec4a_trigthresh4_out:
-      address: 0x22
+      value: 0
+    testmode:
+      address: 0x20
       bitposition: 0
-      bitwidth: 16
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 1536  # 0
-    psec4a_trigthresh5_out:
-      address: 0x23
-      bitposition: 0
-      bitwidth: 16
+      value: 0
+  i2c_registers:
+    i2c_en:
+      address: 0x0F
+      bitposition: 14
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 1536  # 0
-    psec4a_trigthresh6_out:
-      address: 0x24
-      bitposition: 0
-      bitwidth: 16
+      value: true
+    # i2c_send:
+    #   address: 0x0F
+    #   bitposition: 15
+    #   bitwidth: 1
+    #   description: ''
+    #   readwrite: rw
+    #   value: 0
+    i2c_words:
+      address: 0x0F
+      bitposition: 8
+      bitwidth: 3
       description: ''
       readwrite: rw
-      value: 1536  # 0
-    psec4a_trigthresh7_out:
-      address: 0x25
+      value: 0
+    i2c_addr:
+      address: 0x0F
       bitposition: 0
-      bitwidth: 16
+      bitwidth: 8
       description: ''
       readwrite: rw
-      value: 1536  # 0
-    psec4a_trigthresh8_out:
-      address: 0x26
+      value: 0
+    i2c_data0:
+      address: 0x10
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
-      value: 1536  # 0
-    reread_data:
-      address: 0x10
-      bitposition: 9
-      bitwidth: 1
-      description: ''
-      readwrite: rw
       value: 0
-    ring_oscillator_feedback_target_value_lsw:
+    i2c_data1:
       address: 0x11
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
-      value: 29529
-    ring_oscillator_feedback_target_value_msw:
+      value: 0
+    i2c_data2:
       address: 0x12
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
-      value: 7
-    ro_feedback_enable:
-      address: 0x13
-      bitposition: 0
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: 1
-    ro_monitor_reset:
-      address: 0x29
-      bitposition: 3
-      bitwidth: 1
-      description: ''
-      readwrite: rw
       value: 0
-    self_trigger_or_enable:
+    i2c_data3:
       address: 0x13
-      bitposition: 6
-      bitwidth: 1
-      description: 'Enable Self Trigger OR function in PSEC4A'
-      readwrite: rw
-      value: 1
-    serial_data_select:
-      address: 0x28
-      bitposition: 12
-      bitwidth: 4
-      description: ''
-      readwrite: rw
-      value: 0
-    serial_write_strobe:
-      address: 0x10
       bitposition: 0
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: 0
-    software_trigger:
-      address: 0x13
-      bitposition: 4
-      bitwidth: 1
+      bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
-    speed_select:
-      address: 0x13
-      bitposition: 3
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: 1
-    # system_clock_monitor:
-    #   address: 0x28
-    #   bitposition: 8
-    #   bitwidth: 1
-    #   description: ''
-    #   readwrite: rw
-    #   value: 1
-    trig_out1:
-      address: 0x90
+    response0:
+      address: 0x48
       bitposition: 0
-      bitwidth: 4
-      description: 'DCBA chiporder'
-      readwrite: rw
-      value: 0
-    trigger_mask_enable:
-      address: 0x29
-      bitposition: 8
-      bitwidth: 8
-      description: 'Trigger mask where each bit is a corresponding chip'
-      readwrite: rw
-      value: 255  # '11111111'
-    trigger_mode:
-      address: 0x29
-      bitposition: 5
-      bitwidth: 2
-      description: '<html><head/><body><p>Set the triggermode:<br/>
-        00: Software Trigger, the default.<br/>
-        01: Auto Trigger, 2Hz auto trigger rate.<br/>
-        10: External Trigger, trigger on trig in.<br/>
-        11: Self Trigger, trigger on signal levels.
-        </p></body></html>'
-      readwrite: rw
-      value: 0
-    trigger_reset:
-      address: 0x13
-      bitposition: 13
-      bitwidth: 1
+      bitwidth: 16
       description: ''
-      readwrite: rw
+      readwrite: r
       value: 0
-    # trigger_scaler:
-    #   address: 0x97
-    #   bitposition: 0
-    #   bitwidth: 8
-    #   description: ''
-    #   readwrite: rw
-    #   value: 0
-    trigger_sign:
-      address: 0x13
-      bitposition: 1
-      bitwidth: 1
+    response1:
+      address: 0x49
+      bitposition: 0
+      bitwidth: 16
       description: ''
-      readwrite: rw
+      readwrite: r
       value: 0
-    uart_status:
-      address: 0x81
+    response2:
+      address: 0x4A
       bitposition: 0
-      bitwidth: 8
-      description: ''
-      readwrite: rw
-      value: 84
-    uart_handshake_en_out:
-      address: 0x10
-      bitposition: 8
-      bitwidth: 1
+      bitwidth: 16
       description: ''
-      readwrite: rw
-      value: false
-    version_number:
-      address: 0x80
+      readwrite: r
+      value: 0
+    response3:
+      address: 0x4B
       bitposition: 0
       bitwidth: 16
       description: ''
-      readwrite: rw
-      value: 4101
-    wave_fifo_reset:
-      address: 0x10
-      bitposition: 1
-      bitwidth: 1
-      description: ''
-      readwrite: rw
+      readwrite: r
       value: 0
-    xfer_reset:
-      address: 0x13
-      bitposition: 2
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: 1
```

### Comparing `naluconfigs-10.8.0/src/naluconfigs/exceptions.py` & `naluconfigs-11.0.0/src/naluconfigs/exceptions.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.8.0/src/naluconfigs/postprocess.py` & `naluconfigs-11.0.0/src/naluconfigs/postprocess.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.8.0/src/naluconfigs.egg-info/PKG-INFO` & `naluconfigs-11.0.0/src/naluconfigs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naluconfigs
-Version: 10.8.0
+Version: 11.0.0
 Summary: Home for board configs
 Home-page: 
 Author: Thomas Yang, Emily Lum
 Author-email: Marcus Luck <marcus@naluscientific.com>, Mitchell Matsumori-Kelly <mitchell@naluscientific.com>, Alvin Yang <alvin@naluscientific.com>, Kenneth Lauritzen <kenneth@naluscientific.com>, Ben Rotter <ben@naluscientific.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

### Comparing `naluconfigs-10.8.0/src/naluconfigs.egg-info/SOURCES.txt` & `naluconfigs-11.0.0/src/naluconfigs.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 README.md
 pyproject.toml
 setup.py
 src/naluconfigs/__init__.py
+src/naluconfigs/_constructors.py
 src/naluconfigs/_version.py
 src/naluconfigs/exceptions.py
+src/naluconfigs/helpers.py
 src/naluconfigs/postprocess.py
 src/naluconfigs.egg-info/PKG-INFO
 src/naluconfigs.egg-info/SOURCES.txt
 src/naluconfigs.egg-info/dependency_links.txt
 src/naluconfigs.egg-info/requires.txt
 src/naluconfigs.egg-info/top_level.txt
 src/naluconfigs/data/clocks/AODS_300GCC.txt
@@ -52,9 +54,10 @@
 src/naluconfigs/data/registers/udc16.yml
 src/naluconfigs/data/registers/upac32.yml
 src/naluconfigs/data/registers/upac96.yml
 src/naluconfigs/data/registers/upaci.yml
 src/naluconfigs/data/registers/zdigitizer.yml
 tests/test_hex_addr_converter.py
 tests/test_i2c_registers.py
+tests/test_multichip.py
 tests/test_post_processing.py
 tests/test_range_keys.py
```

### Comparing `naluconfigs-10.8.0/tests/test_hex_addr_converter.py` & `naluconfigs-11.0.0/tests/test_hex_addr_converter.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.8.0/tests/test_i2c_registers.py` & `naluconfigs-11.0.0/tests/test_i2c_registers.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.8.0/tests/test_post_processing.py` & `naluconfigs-11.0.0/tests/test_post_processing.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-10.8.0/tests/test_range_keys.py` & `naluconfigs-11.0.0/tests/test_range_keys.py`

 * *Files identical despite different names*

