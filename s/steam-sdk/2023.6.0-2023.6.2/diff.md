# Comparing `tmp/steam-sdk-2023.6.0.tar.gz` & `tmp/steam-sdk-2023.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\steam-sdk-2023.6.0.tar", last modified: Thu Jun  1 21:57:18 2023, max compression
+gzip compressed data, was "dist\steam-sdk-2023.6.2.tar", last modified: Fri Jun  2 10:59:09 2023, max compression
```

## Comparing `steam-sdk-2023.6.0.tar` & `steam-sdk-2023.6.2.tar`

### file list

```diff
@@ -1,183 +1,185 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 21:57:18.469019 steam-sdk-2023.6.0/
--rw-rw-rw-   0        0        0      122 2023-02-02 15:29:21.000000 steam-sdk-2023.6.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1550 2023-06-01 21:57:18.468019 steam-sdk-2023.6.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-01 21:57:18.469019 steam-sdk-2023.6.0/setup.cfg
--rw-rw-rw-   0        0        0      797 2023-06-01 21:56:21.000000 steam-sdk-2023.6.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-01 21:57:17.290632 steam-sdk-2023.6.0/steam_sdk/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 21:57:17.344487 steam-sdk-2023.6.0/steam_sdk/analyses/
--rw-rw-rw-   0        0        0   125649 2023-05-22 14:09:18.000000 steam-sdk-2023.6.0/steam_sdk/analyses/AnalysisSTEAM.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/analyses/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 21:57:17.346482 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 21:57:17.365432 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/__init__.py
--rw-rw-rw-   0        0        0    23368 2022-10-12 14:45:26.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py
-drwxrwxrwx   0        0        0        0 2023-06-01 21:57:17.440070 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/__init__.py
--rw-rw-rw-   0        0        0    16757 2022-10-06 23:30:28.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py
--rw-rw-rw-   0        0        0     2800 2022-09-12 16:26:14.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py
--rw-rw-rw-   0        0        0     6828 2022-09-10 00:21:21.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py
--rw-rw-rw-   0        0        0    95412 2022-10-24 19:22:58.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py
--rw-rw-rw-   0        0        0     2652 2022-09-09 21:29:03.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py
--rw-rw-rw-   0        0        0     2341 2022-09-09 21:29:03.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py
-drwxrwxrwx   0        0        0        0 2023-06-01 21:57:17.455304 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/__init__.py
--rw-rw-rw-   0        0        0    22374 2022-09-28 09:57:32.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py
-drwxrwxrwx   0        0        0        0 2023-06-01 21:57:17.484725 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/
--rw-rw-rw-   0        0        0        0 2022-09-26 06:59:06.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/__init__.py
--rw-rw-rw-   0        0        0     5210 2022-09-28 09:57:32.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py
--rw-rw-rw-   0        0        0     4527 2022-09-28 09:57:32.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py
--rw-rw-rw-   0        0        0     2921 2022-09-28 09:57:32.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py
-drwxrwxrwx   0        0        0        0 2023-06-01 21:57:17.499855 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/
--rw-rw-rw-   0        0        0        0 2022-09-26 06:59:06.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/__init__.py
--rw-rw-rw-   0        0        0    29433 2022-09-30 09:15:14.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py
-drwxrwxrwx   0        0        0        0 2023-06-01 21:57:17.522272 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/
--rw-rw-rw-   0        0        0        0 2022-09-26 06:59:06.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/__init__.py
--rw-rw-rw-   0        0        0     5210 2022-09-28 09:57:32.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py
--rw-rw-rw-   0        0        0     4704 2022-09-28 09:57:32.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py
--rw-rw-rw-   0        0        0     4852 2022-09-28 09:57:32.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py
-drwxrwxrwx   0        0        0        0 2023-06-01 21:57:17.534681 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/custom_function_test_1/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/custom_function_test_1/__init__.py
--rw-rw-rw-   0        0        0     1307 2022-09-10 00:27:54.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py
-drwxrwxrwx   0        0        0        0 2023-06-01 21:57:17.627402 steam-sdk-2023.6.0/steam_sdk/builders/
--rw-rw-rw-   0        0        0    12924 2023-05-19 10:14:24.000000 steam-sdk-2023.6.0/steam_sdk/builders/BuilderFiQuS.py
--rw-rw-rw-   0        0        0   162736 2023-05-25 09:34:00.000000 steam-sdk-2023.6.0/steam_sdk/builders/BuilderLEDET.py
--rw-rw-rw-   0        0        0    35758 2023-05-22 14:09:16.000000 steam-sdk-2023.6.0/steam_sdk/builders/BuilderModel.py
--rw-rw-rw-   0        0        0    12686 2022-09-07 00:41:51.000000 steam-sdk-2023.6.0/steam_sdk/builders/BuilderProteCCT.py
--rw-rw-rw-   0        0        0     6749 2022-08-22 11:29:04.000000 steam-sdk-2023.6.0/steam_sdk/builders/BuilderPyBBQ.py
--rw-rw-rw-   0        0        0    12076 2023-05-10 14:10:46.000000 steam-sdk-2023.6.0/steam_sdk/builders/BuilderSIGMA.py
--rw-rw-rw-   0        0        0    11689 2023-01-18 09:46:00.000000 steam-sdk-2023.6.0/steam_sdk/builders/SelfMutualInductanceCalculation.py
--rw-rw-rw-   0        0        0     7941 2022-12-06 11:41:34.000000 steam-sdk-2023.6.0/steam_sdk/builders/Solenoids.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/builders/__init__.py
--rw-rw-rw-   0        0        0     8352 2023-02-02 15:39:34.000000 steam-sdk-2023.6.0/steam_sdk/builders/geometricFunctions.py
-drwxrwxrwx   0        0        0        0 2023-06-01 21:57:17.628402 steam-sdk-2023.6.0/steam_sdk/configs/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/configs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 21:57:17.629399 steam-sdk-2023.6.0/steam_sdk/configs/plotters/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/configs/plotters/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 21:57:17.640478 steam-sdk-2023.6.0/steam_sdk/configs/tools_defaults/
-drwxrwxrwx   0        0        0        0 2023-06-01 21:57:17.650471 steam-sdk-2023.6.0/steam_sdk/configs/tools_defaults/LEDET/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/configs/tools_defaults/LEDET/__init__.py
--rw-rw-rw-   0        0        0    32991 2023-05-25 09:35:34.000000 steam-sdk-2023.6.0/steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx
--rw-rw-rw-   0        0        0     1426 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/configs/tools_defaults/ToolDefaultReader.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/configs/tools_defaults/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 21:57:17.652444 steam-sdk-2023.6.0/steam_sdk/cosims/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/cosims/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 21:57:17.846793 steam-sdk-2023.6.0/steam_sdk/data/
--rw-rw-rw-   0        0        0    10200 2023-05-12 14:38:34.000000 steam-sdk-2023.6.0/steam_sdk/data/DataAnalysis.py
--rw-rw-rw-   0        0        0     7983 2023-05-19 12:19:03.000000 steam-sdk-2023.6.0/steam_sdk/data/DataConductor.py
--rw-rw-rw-   0        0        0     3281 2022-09-30 09:15:14.000000 steam-sdk-2023.6.0/steam_sdk/data/DataDakota.py
--rw-rw-rw-   0        0        0     2865 2023-05-04 08:10:45.000000 steam-sdk-2023.6.0/steam_sdk/data/DataEventCircuit.py
--rw-rw-rw-   0        0        0     4193 2023-05-09 19:16:09.000000 steam-sdk-2023.6.0/steam_sdk/data/DataEventMagnet.py
--rw-rw-rw-   0        0        0    12762 2023-05-19 10:14:24.000000 steam-sdk-2023.6.0/steam_sdk/data/DataFiQuS.py
--rw-rw-rw-   0        0        0    10823 2023-05-25 07:24:44.000000 steam-sdk-2023.6.0/steam_sdk/data/DataLEDET.py
--rw-rw-rw-   0        0        0     4314 2022-08-22 11:29:04.000000 steam-sdk-2023.6.0/steam_sdk/data/DataModelCircuit.py
--rw-rw-rw-   0        0        0     5869 2022-09-28 09:57:32.000000 steam-sdk-2023.6.0/steam_sdk/data/DataModelConductor.py
--rw-rw-rw-   0        0        0    35376 2023-05-25 09:55:42.000000 steam-sdk-2023.6.0/steam_sdk/data/DataModelMagnet.py
--rw-rw-rw-   0        0        0     2636 2023-05-09 19:16:09.000000 steam-sdk-2023.6.0/steam_sdk/data/DataParsimConductor.py
--rw-rw-rw-   0        0        0        0 2022-09-07 00:41:51.000000 steam-sdk-2023.6.0/steam_sdk/data/DataParsims.py
--rw-rw-rw-   0        0        0     1995 2022-03-07 20:47:17.000000 steam-sdk-2023.6.0/steam_sdk/data/DataProteCCT.py
--rw-rw-rw-   0        0        0     2105 2022-09-28 09:57:32.000000 steam-sdk-2023.6.0/steam_sdk/data/DataPyBBQ.py
--rw-rw-rw-   0        0        0     8068 2023-05-25 09:55:42.000000 steam-sdk-2023.6.0/steam_sdk/data/DataRoxieParser.py
--rw-rw-rw-   0        0        0     6791 2023-05-09 19:16:09.000000 steam-sdk-2023.6.0/steam_sdk/data/DataSIGMA.py
--rw-rw-rw-   0        0        0     1729 2023-05-25 11:21:07.000000 steam-sdk-2023.6.0/steam_sdk/data/DataSettings.py
--rw-rw-rw-   0        0        0     3204 2023-01-05 21:02:33.000000 steam-sdk-2023.6.0/steam_sdk/data/DataSignal.py
--rw-rw-rw-   0        0        0    23052 2023-05-25 07:24:44.000000 steam-sdk-2023.6.0/steam_sdk/data/DictionaryLEDET.py
--rw-rw-rw-   0        0        0     4482 2022-08-23 08:56:30.000000 steam-sdk-2023.6.0/steam_sdk/data/DictionaryProteCCT.py
--rw-rw-rw-   0        0        0     2902 2022-09-28 09:57:32.000000 steam-sdk-2023.6.0/steam_sdk/data/DictionaryPyBBQ.py
--rw-rw-rw-   0        0        0    27819 2023-05-25 07:24:44.000000 steam-sdk-2023.6.0/steam_sdk/data/TemplateLEDET.py
--rw-rw-rw-   0        0        0     7903 2022-03-30 17:37:43.000000 steam-sdk-2023.6.0/steam_sdk/data/TemplateProteCCT.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 21:57:17.933100 steam-sdk-2023.6.0/steam_sdk/drivers/
--rw-rw-rw-   0        0        0     3151 2022-12-06 11:41:34.000000 steam-sdk-2023.6.0/steam_sdk/drivers/DriverAnalysis.py
--rw-rw-rw-   0        0        0     2711 2022-12-06 11:41:34.000000 steam-sdk-2023.6.0/steam_sdk/drivers/DriverDakota.py
--rw-rw-rw-   0        0        0     1299 2023-02-02 08:17:41.000000 steam-sdk-2023.6.0/steam_sdk/drivers/DriverFiQuS.py
--rw-rw-rw-   0        0        0     3482 2022-12-16 13:26:54.000000 steam-sdk-2023.6.0/steam_sdk/drivers/DriverLEDET.py
--rw-rw-rw-   0        0        0     1924 2022-10-31 08:36:49.000000 steam-sdk-2023.6.0/steam_sdk/drivers/DriverPSPICE.py
--rw-rw-rw-   0        0        0     2062 2022-09-26 06:59:06.000000 steam-sdk-2023.6.0/steam_sdk/drivers/DriverProteCCT.py
--rw-rw-rw-   0        0        0     2219 2022-06-02 08:33:55.000000 steam-sdk-2023.6.0/steam_sdk/drivers/DriverPyBBQ.py
--rw-rw-rw-   0        0        0     3905 2023-05-19 10:14:24.000000 steam-sdk-2023.6.0/steam_sdk/drivers/DriverSIGMA.py
--rw-rw-rw-   0        0        0     1932 2022-10-31 08:36:49.000000 steam-sdk-2023.6.0/steam_sdk/drivers/DriverXYCE.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/drivers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 21:57:18.142286 steam-sdk-2023.6.0/steam_sdk/parsers/
--rw-rw-rw-   0        0        0     4984 2022-08-22 11:29:04.000000 steam-sdk-2023.6.0/steam_sdk/parsers/CSD_Reader.py
--rw-rw-rw-   0        0        0      317 2023-04-17 13:02:30.000000 steam-sdk-2023.6.0/steam_sdk/parsers/ParserCOMSOLToTxt.py
--rw-rw-rw-   0        0        0     2290 2022-06-24 07:36:06.000000 steam-sdk-2023.6.0/steam_sdk/parsers/ParserCond2d.py
--rw-rw-rw-   0        0        0     1081 2023-05-24 11:49:42.000000 steam-sdk-2023.6.0/steam_sdk/parsers/ParserCsd.py
--rw-rw-rw-   0        0        0     6220 2023-01-16 11:54:48.000000 steam-sdk-2023.6.0/steam_sdk/parsers/ParserCsv.py
--rw-rw-rw-   0        0        0     1650 2023-01-13 08:48:18.000000 steam-sdk-2023.6.0/steam_sdk/parsers/ParserDakota.py
--rw-rw-rw-   0        0        0     1030 2023-03-13 09:01:17.000000 steam-sdk-2023.6.0/steam_sdk/parsers/ParserDatToCsv.py
--rw-rw-rw-   0        0        0     8536 2023-02-02 15:29:22.000000 steam-sdk-2023.6.0/steam_sdk/parsers/ParserExcel.py
--rw-rw-rw-   0        0        0     2287 2022-09-30 09:15:14.000000 steam-sdk-2023.6.0/steam_sdk/parsers/ParserFiQuS.py
--rw-rw-rw-   0        0        0    48055 2023-05-25 09:53:27.000000 steam-sdk-2023.6.0/steam_sdk/parsers/ParserLEDET.py
--rw-rw-rw-   0        0        0    12436 2022-11-21 14:56:04.000000 steam-sdk-2023.6.0/steam_sdk/parsers/ParserMap2d.py
--rw-rw-rw-   0        0        0    14159 2023-05-22 14:09:18.000000 steam-sdk-2023.6.0/steam_sdk/parsers/ParserMat.py
--rw-rw-rw-   0        0        0    63401 2023-05-31 09:59:27.000000 steam-sdk-2023.6.0/steam_sdk/parsers/ParserPSPICE.py
--rw-rw-rw-   0        0        0     4780 2023-03-03 12:33:32.000000 steam-sdk-2023.6.0/steam_sdk/parsers/ParserPdf.py
--rw-rw-rw-   0        0        0     6838 2023-02-03 13:16:35.000000 steam-sdk-2023.6.0/steam_sdk/parsers/ParserProteCCT.py
--rw-rw-rw-   0        0        0     2942 2022-09-26 06:59:06.000000 steam-sdk-2023.6.0/steam_sdk/parsers/ParserProtePyBBQ.py
--rw-rw-rw-   0        0        0    95752 2023-05-25 09:55:42.000000 steam-sdk-2023.6.0/steam_sdk/parsers/ParserRoxie.py
--rw-rw-rw-   0        0        0     1928 2023-05-09 19:16:09.000000 steam-sdk-2023.6.0/steam_sdk/parsers/ParserSIGMA.py
--rw-rw-rw-   0        0        0    11707 2022-09-07 14:38:46.000000 steam-sdk-2023.6.0/steam_sdk/parsers/ParserTdms.py
--rw-rw-rw-   0        0        0    55281 2023-02-02 12:20:26.000000 steam-sdk-2023.6.0/steam_sdk/parsers/ParserXYCE.py
--rw-rw-rw-   0        0        0     4195 2023-05-22 14:09:18.000000 steam-sdk-2023.6.0/steam_sdk/parsers/ParserYAML.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/parsers/__init__.py
--rw-rw-rw-   0        0        0        2 2022-09-02 10:44:52.000000 steam-sdk-2023.6.0/steam_sdk/parsers/dict_to_in.py
-drwxrwxrwx   0        0        0        0 2023-06-01 21:57:18.204066 steam-sdk-2023.6.0/steam_sdk/parsims/
--rw-rw-rw-   0        0        0    61782 2023-05-23 14:33:11.000000 steam-sdk-2023.6.0/steam_sdk/parsims/ParsimConductor.py
--rw-rw-rw-   0        0        0      916 2022-09-26 06:59:06.000000 steam-sdk-2023.6.0/steam_sdk/parsims/ParsimDakota.py
--rw-rw-rw-   0        0        0    72533 2023-05-19 10:14:24.000000 steam-sdk-2023.6.0/steam_sdk/parsims/ParsimEventCircuit.py
--rw-rw-rw-   0        0        0    48206 2023-05-25 09:55:42.000000 steam-sdk-2023.6.0/steam_sdk/parsims/ParsimEventMagnet.py
--rw-rw-rw-   0        0        0     1972 2023-01-24 08:05:20.000000 steam-sdk-2023.6.0/steam_sdk/parsims/ParsimSweep.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/parsims/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 21:57:18.250904 steam-sdk-2023.6.0/steam_sdk/plotters/
--rw-rw-rw-   0        0        0     8053 2023-05-12 14:38:34.000000 steam-sdk-2023.6.0/steam_sdk/plotters/PlotterAnalysis.py
--rw-rw-rw-   0        0        0    20391 2023-05-25 09:55:42.000000 steam-sdk-2023.6.0/steam_sdk/plotters/PlotterMap2d.py
--rw-rw-rw-   0        0        0    39596 2022-06-20 13:00:15.000000 steam-sdk-2023.6.0/steam_sdk/plotters/PlotterModel.py
--rw-rw-rw-   0        0        0    22987 2022-12-06 11:41:34.000000 steam-sdk-2023.6.0/steam_sdk/plotters/PlotterParametric.py
--rw-rw-rw-   0        0        0     8863 2023-05-25 09:55:42.000000 steam-sdk-2023.6.0/steam_sdk/plotters/PlotterRoxie.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/plotters/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 21:57:18.259619 steam-sdk-2023.6.0/steam_sdk/postprocs/
--rw-rw-rw-   0        0        0     5564 2022-09-26 06:59:06.000000 steam-sdk-2023.6.0/steam_sdk/postprocs/PostprocsMetrics.py
--rw-rw-rw-   0        0        0        0 2022-09-14 13:30:58.000000 steam-sdk-2023.6.0/steam_sdk/postprocs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 21:57:18.423866 steam-sdk-2023.6.0/steam_sdk/utils/
--rw-rw-rw-   0        0        0     2679 2023-03-13 09:01:17.000000 steam-sdk-2023.6.0/steam_sdk/utils/MTF_reading_functions.py
--rw-rw-rw-   0        0        0    14942 2022-06-30 20:06:54.000000 steam-sdk-2023.6.0/steam_sdk/utils/ModifyModelData.py
--rw-rw-rw-   0        0        0     4707 2023-05-22 14:09:18.000000 steam-sdk-2023.6.0/steam_sdk/utils/ModifyModelDataMagnet.py
--rw-rw-rw-   0        0        0     2747 2023-05-22 14:09:18.000000 steam-sdk-2023.6.0/steam_sdk/utils/ModifyModelDataconductor.py
--rw-rw-rw-   0        0        0      313 2022-03-01 14:21:51.000000 steam-sdk-2023.6.0/steam_sdk/utils/NumpyEncoder.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/utils/__init__.py
--rw-rw-rw-   0        0        0      686 2022-06-12 12:41:34.000000 steam-sdk-2023.6.0/steam_sdk/utils/clean_NaN_from_signal.py
--rw-rw-rw-   0        0        0     3837 2023-02-03 13:26:48.000000 steam-sdk-2023.6.0/steam_sdk/utils/compare_two_parameters.py
--rw-rw-rw-   0        0        0      590 2023-05-09 19:16:09.000000 steam-sdk-2023.6.0/steam_sdk/utils/create_coordinate_file_SIGMA.py
--rw-rw-rw-   0        0        0     1279 2023-04-17 13:02:30.000000 steam-sdk-2023.6.0/steam_sdk/utils/get_attribute_type.py
--rw-rw-rw-   0        0        0      167 2022-06-11 12:54:31.000000 steam-sdk-2023.6.0/steam_sdk/utils/isNaN.py
--rw-rw-rw-   0        0        0      299 2022-04-12 00:42:08.000000 steam-sdk-2023.6.0/steam_sdk/utils/make_folder_if_not_existing.py
--rw-rw-rw-   0        0        0     4512 2022-05-02 08:49:48.000000 steam-sdk-2023.6.0/steam_sdk/utils/misc.py
--rw-rw-rw-   0        0        0     1592 2023-04-17 13:02:30.000000 steam-sdk-2023.6.0/steam_sdk/utils/parse_str_to_list.py
--rw-rw-rw-   0        0        0      388 2022-04-11 18:20:26.000000 steam-sdk-2023.6.0/steam_sdk/utils/rgetattr.py
--rw-rw-rw-   0        0        0      460 2023-01-07 20:16:27.000000 steam-sdk-2023.6.0/steam_sdk/utils/rhasattr.py
--rw-rw-rw-   0        0        0      383 2022-04-11 18:20:26.000000 steam-sdk-2023.6.0/steam_sdk/utils/sgetattr.py
--rw-rw-rw-   0        0        0      863 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/utils/tic_toc.py
--rw-rw-rw-   0        0        0      168 2022-06-07 19:34:59.000000 steam-sdk-2023.6.0/steam_sdk/utils/unique.py
--rw-rw-rw-   0        0        0     7005 2023-05-12 14:38:34.000000 steam-sdk-2023.6.0/steam_sdk/utils/utils_PC.py
-drwxrwxrwx   0        0        0        0 2023-06-01 21:57:18.453889 steam-sdk-2023.6.0/steam_sdk/viewers/
--rw-rw-rw-   0        0        0    35919 2023-03-23 14:48:07.000000 steam-sdk-2023.6.0/steam_sdk/viewers/Viewer.py
--rw-rw-rw-   0        0        0     6127 2022-06-13 00:34:14.000000 steam-sdk-2023.6.0/steam_sdk/viewers/ViewerMeas.py
--rw-rw-rw-   0        0        0     1667 2022-06-20 13:06:20.000000 steam-sdk-2023.6.0/steam_sdk/viewers/ViewerSim.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/viewers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 21:57:18.463547 steam-sdk-2023.6.0/steam_sdk/wrappers/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/wrappers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 21:57:18.464544 steam-sdk-2023.6.0/steam_sdk/wrappers/java/
-drwxrwxrwx   0        0        0        0 2023-06-01 21:57:18.465541 steam-sdk-2023.6.0/steam_sdk/wrappers/java/SING/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/wrappers/java/SING/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 21:57:18.467047 steam-sdk-2023.6.0/steam_sdk/wrappers/java/SING/jars/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/wrappers/java/SING/jars/__init__.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/wrappers/java/__init__.py
--rw-rw-rw-   0        0        0     1834 2022-07-05 13:48:59.000000 steam-sdk-2023.6.0/steam_sdk/wrappers/wrapper_yaml.py
-drwxrwxrwx   0        0        0        0 2023-06-01 21:57:17.319557 steam-sdk-2023.6.0/steam_sdk.egg-info/
--rw-rw-rw-   0        0        0     1550 2023-06-01 21:57:16.000000 steam-sdk-2023.6.0/steam_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6686 2023-06-01 21:57:17.000000 steam-sdk-2023.6.0/steam_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 21:57:16.000000 steam-sdk-2023.6.0/steam_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1597 2023-06-01 21:57:16.000000 steam-sdk-2023.6.0/steam_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-01 21:57:16.000000 steam-sdk-2023.6.0/steam_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 10:59:09.304987 steam-sdk-2023.6.2/
+-rw-rw-rw-   0        0        0      122 2023-03-15 09:29:53.000000 steam-sdk-2023.6.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1550 2023-06-02 10:59:09.303987 steam-sdk-2023.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-02 10:59:09.304987 steam-sdk-2023.6.2/setup.cfg
+-rw-rw-rw-   0        0        0      797 2023-06-02 10:57:55.000000 steam-sdk-2023.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:59:09.033493 steam-sdk-2023.6.2/steam_sdk/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:59:09.043619 steam-sdk-2023.6.2/steam_sdk/analyses/
+-rw-rw-rw-   0        0        0   125865 2023-06-02 10:53:43.000000 steam-sdk-2023.6.2/steam_sdk/analyses/AnalysisSTEAM.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/analyses/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:59:09.044618 steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:59:09.047618 steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/__init__.py
+-rw-rw-rw-   0        0        0    23368 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:59:09.058859 steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/__init__.py
+-rw-rw-rw-   0        0        0    16757 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py
+-rw-rw-rw-   0        0        0     2800 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py
+-rw-rw-rw-   0        0        0     6828 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py
+-rw-rw-rw-   0        0        0    95412 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py
+-rw-rw-rw-   0        0        0     2652 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py
+-rw-rw-rw-   0        0        0     2341 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:59:09.061863 steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/__init__.py
+-rw-rw-rw-   0        0        0    22374 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:59:09.069999 steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/__init__.py
+-rw-rw-rw-   0        0        0     5210 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py
+-rw-rw-rw-   0        0        0     4527 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py
+-rw-rw-rw-   0        0        0     2921 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:59:09.071998 steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/__init__.py
+-rw-rw-rw-   0        0        0    29433 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:59:09.077997 steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/__init__.py
+-rw-rw-rw-   0        0        0     5210 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py
+-rw-rw-rw-   0        0        0     4704 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py
+-rw-rw-rw-   0        0        0     4852 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:59:09.080159 steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/custom_function_test_1/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/custom_function_test_1/__init__.py
+-rw-rw-rw-   0        0        0     1307 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:59:09.106368 steam-sdk-2023.6.2/steam_sdk/builders/
+-rw-rw-rw-   0        0        0    12924 2023-05-12 15:08:26.000000 steam-sdk-2023.6.2/steam_sdk/builders/BuilderFiQuS.py
+-rw-rw-rw-   0        0        0   162736 2023-05-25 11:58:42.000000 steam-sdk-2023.6.2/steam_sdk/builders/BuilderLEDET.py
+-rw-rw-rw-   0        0        0    35847 2023-06-02 08:04:33.000000 steam-sdk-2023.6.2/steam_sdk/builders/BuilderModel.py
+-rw-rw-rw-   0        0        0    12686 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/builders/BuilderProteCCT.py
+-rw-rw-rw-   0        0        0     6749 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/builders/BuilderPyBBQ.py
+-rw-rw-rw-   0        0        0    12076 2023-05-10 14:13:23.000000 steam-sdk-2023.6.2/steam_sdk/builders/BuilderSIGMA.py
+-rw-rw-rw-   0        0        0    11689 2023-01-18 15:24:33.000000 steam-sdk-2023.6.2/steam_sdk/builders/SelfMutualInductanceCalculation.py
+-rw-rw-rw-   0        0        0     7941 2022-12-19 08:13:58.000000 steam-sdk-2023.6.2/steam_sdk/builders/Solenoids.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/builders/__init__.py
+-rw-rw-rw-   0        0        0     8352 2023-03-15 09:29:53.000000 steam-sdk-2023.6.2/steam_sdk/builders/geometricFunctions.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:59:09.108367 steam-sdk-2023.6.2/steam_sdk/configs/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/configs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:59:09.109488 steam-sdk-2023.6.2/steam_sdk/configs/plotters/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/configs/plotters/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:59:09.111490 steam-sdk-2023.6.2/steam_sdk/configs/tools_defaults/
+drwxrwxrwx   0        0        0        0 2023-06-02 10:59:09.113490 steam-sdk-2023.6.2/steam_sdk/configs/tools_defaults/LEDET/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/configs/tools_defaults/LEDET/__init__.py
+-rw-rw-rw-   0        0        0    32991 2023-05-25 11:58:42.000000 steam-sdk-2023.6.2/steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx
+-rw-rw-rw-   0        0        0     1426 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/configs/tools_defaults/ToolDefaultReader.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/configs/tools_defaults/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:59:09.115489 steam-sdk-2023.6.2/steam_sdk/cosims/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/cosims/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:59:09.159284 steam-sdk-2023.6.2/steam_sdk/data/
+-rw-rw-rw-   0        0        0    10200 2023-05-12 13:31:31.000000 steam-sdk-2023.6.2/steam_sdk/data/DataAnalysis.py
+-rw-rw-rw-   0        0        0     7983 2023-05-22 11:27:05.000000 steam-sdk-2023.6.2/steam_sdk/data/DataConductor.py
+-rw-rw-rw-   0        0        0     3281 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/data/DataDakota.py
+-rw-rw-rw-   0        0        0     2865 2023-04-24 12:48:33.000000 steam-sdk-2023.6.2/steam_sdk/data/DataEventCircuit.py
+-rw-rw-rw-   0        0        0     4193 2023-05-09 14:50:49.000000 steam-sdk-2023.6.2/steam_sdk/data/DataEventMagnet.py
+-rw-rw-rw-   0        0        0    12762 2023-05-12 15:08:26.000000 steam-sdk-2023.6.2/steam_sdk/data/DataFiQuS.py
+-rw-rw-rw-   0        0        0    10823 2023-05-25 11:58:42.000000 steam-sdk-2023.6.2/steam_sdk/data/DataLEDET.py
+-rw-rw-rw-   0        0        0     4314 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/data/DataModelCircuit.py
+-rw-rw-rw-   0        0        0     5869 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/data/DataModelConductor.py
+-rw-rw-rw-   0        0        0    35376 2023-05-25 11:58:27.000000 steam-sdk-2023.6.2/steam_sdk/data/DataModelMagnet.py
+-rw-rw-rw-   0        0        0     2636 2023-05-09 14:50:49.000000 steam-sdk-2023.6.2/steam_sdk/data/DataParsimConductor.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/data/DataParsims.py
+-rw-rw-rw-   0        0        0     1995 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/data/DataProteCCT.py
+-rw-rw-rw-   0        0        0     2105 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/data/DataPyBBQ.py
+-rw-rw-rw-   0        0        0     8068 2023-05-25 11:58:27.000000 steam-sdk-2023.6.2/steam_sdk/data/DataRoxieParser.py
+-rw-rw-rw-   0        0        0     6791 2023-05-09 14:51:04.000000 steam-sdk-2023.6.2/steam_sdk/data/DataSIGMA.py
+-rw-rw-rw-   0        0        0     1650 2023-03-15 09:29:53.000000 steam-sdk-2023.6.2/steam_sdk/data/DataSettings.py
+-rw-rw-rw-   0        0        0     3204 2023-01-11 12:50:11.000000 steam-sdk-2023.6.2/steam_sdk/data/DataSignal.py
+-rw-rw-rw-   0        0        0    23052 2023-05-25 11:58:42.000000 steam-sdk-2023.6.2/steam_sdk/data/DictionaryLEDET.py
+-rw-rw-rw-   0        0        0     4482 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/data/DictionaryProteCCT.py
+-rw-rw-rw-   0        0        0     2902 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/data/DictionaryPyBBQ.py
+-rw-rw-rw-   0        0        0    27819 2023-05-25 11:58:42.000000 steam-sdk-2023.6.2/steam_sdk/data/TemplateLEDET.py
+-rw-rw-rw-   0        0        0     7903 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/data/TemplateProteCCT.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:59:09.173421 steam-sdk-2023.6.2/steam_sdk/drivers/
+-rw-rw-rw-   0        0        0     3151 2022-12-19 08:13:58.000000 steam-sdk-2023.6.2/steam_sdk/drivers/DriverAnalysis.py
+-rw-rw-rw-   0        0        0     2711 2022-12-19 08:13:58.000000 steam-sdk-2023.6.2/steam_sdk/drivers/DriverDakota.py
+-rw-rw-rw-   0        0        0     1299 2023-03-15 09:29:53.000000 steam-sdk-2023.6.2/steam_sdk/drivers/DriverFiQuS.py
+-rw-rw-rw-   0        0        0     3482 2022-12-19 08:13:58.000000 steam-sdk-2023.6.2/steam_sdk/drivers/DriverLEDET.py
+-rw-rw-rw-   0        0        0     1924 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/drivers/DriverPSPICE.py
+-rw-rw-rw-   0        0        0     2062 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/drivers/DriverProteCCT.py
+-rw-rw-rw-   0        0        0     2219 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/drivers/DriverPyBBQ.py
+-rw-rw-rw-   0        0        0     4506 2023-06-02 10:56:11.000000 steam-sdk-2023.6.2/steam_sdk/drivers/DriverSIGMA.py
+-rw-rw-rw-   0        0        0     1932 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/drivers/DriverXYCE.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/drivers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:59:09.219153 steam-sdk-2023.6.2/steam_sdk/parsers/
+-rw-rw-rw-   0        0        0     4984 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/parsers/CSD_Reader.py
+-rw-rw-rw-   0        0        0      317 2023-03-29 12:41:10.000000 steam-sdk-2023.6.2/steam_sdk/parsers/ParserCOMSOLToTxt.py
+-rw-rw-rw-   0        0        0     2290 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/parsers/ParserCond2d.py
+-rw-rw-rw-   0        0        0     1081 2023-05-25 11:58:42.000000 steam-sdk-2023.6.2/steam_sdk/parsers/ParserCsd.py
+-rw-rw-rw-   0        0        0     6220 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/parsers/ParserCsv.py
+-rw-rw-rw-   0        0        0     1650 2023-01-13 08:06:15.000000 steam-sdk-2023.6.2/steam_sdk/parsers/ParserDakota.py
+-rw-rw-rw-   0        0        0     1030 2023-03-15 09:29:53.000000 steam-sdk-2023.6.2/steam_sdk/parsers/ParserDatToCsv.py
+-rw-rw-rw-   0        0        0     8536 2023-03-15 09:29:53.000000 steam-sdk-2023.6.2/steam_sdk/parsers/ParserExcel.py
+-rw-rw-rw-   0        0        0     2287 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/parsers/ParserFiQuS.py
+-rw-rw-rw-   0        0        0    48055 2023-05-25 11:58:42.000000 steam-sdk-2023.6.2/steam_sdk/parsers/ParserLEDET.py
+-rw-rw-rw-   0        0        0    12436 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/parsers/ParserMap2d.py
+-rw-rw-rw-   0        0        0    10920 2023-05-12 13:31:31.000000 steam-sdk-2023.6.2/steam_sdk/parsers/ParserMat.py
+-rw-rw-rw-   0        0        0    63401 2023-06-01 14:44:35.000000 steam-sdk-2023.6.2/steam_sdk/parsers/ParserPSPICE.py
+-rw-rw-rw-   0        0        0     4780 2023-03-15 09:29:53.000000 steam-sdk-2023.6.2/steam_sdk/parsers/ParserPdf.py
+-rw-rw-rw-   0        0        0     6838 2023-03-15 09:29:53.000000 steam-sdk-2023.6.2/steam_sdk/parsers/ParserProteCCT.py
+-rw-rw-rw-   0        0        0     2942 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/parsers/ParserProtePyBBQ.py
+-rw-rw-rw-   0        0        0   109430 2023-06-02 10:49:15.000000 steam-sdk-2023.6.2/steam_sdk/parsers/ParserRoxie.py
+-rw-rw-rw-   0        0        0     1928 2023-05-09 14:51:03.000000 steam-sdk-2023.6.2/steam_sdk/parsers/ParserSIGMA.py
+-rw-rw-rw-   0        0        0    11707 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/parsers/ParserTdms.py
+-rw-rw-rw-   0        0        0    55281 2023-03-15 09:29:53.000000 steam-sdk-2023.6.2/steam_sdk/parsers/ParserXYCE.py
+-rw-rw-rw-   0        0        0     4088 2023-03-15 09:29:53.000000 steam-sdk-2023.6.2/steam_sdk/parsers/ParserYAML.py
+-rw-rw-rw-   0        0        0      975 2023-06-02 08:04:34.000000 steam-sdk-2023.6.2/steam_sdk/parsers/ParserYamlToRoxie.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/parsers/__init__.py
+-rw-rw-rw-   0        0        0        2 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/parsers/dict_to_in.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:59:09.228292 steam-sdk-2023.6.2/steam_sdk/parsims/
+-rw-rw-rw-   0        0        0    61782 2023-05-23 14:30:59.000000 steam-sdk-2023.6.2/steam_sdk/parsims/ParsimConductor.py
+-rw-rw-rw-   0        0        0      916 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/parsims/ParsimDakota.py
+-rw-rw-rw-   0        0        0    72533 2023-05-17 07:23:09.000000 steam-sdk-2023.6.2/steam_sdk/parsims/ParsimEventCircuit.py
+-rw-rw-rw-   0        0        0    48206 2023-05-25 08:00:49.000000 steam-sdk-2023.6.2/steam_sdk/parsims/ParsimEventMagnet.py
+-rw-rw-rw-   0        0        0     1972 2023-01-25 14:04:47.000000 steam-sdk-2023.6.2/steam_sdk/parsims/ParsimSweep.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/parsims/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:59:09.236293 steam-sdk-2023.6.2/steam_sdk/plotters/
+-rw-rw-rw-   0        0        0     8053 2023-05-12 13:31:31.000000 steam-sdk-2023.6.2/steam_sdk/plotters/PlotterAnalysis.py
+-rw-rw-rw-   0        0        0    20391 2023-05-25 11:58:27.000000 steam-sdk-2023.6.2/steam_sdk/plotters/PlotterMap2d.py
+-rw-rw-rw-   0        0        0    39596 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/plotters/PlotterModel.py
+-rw-rw-rw-   0        0        0    22987 2022-12-19 08:13:58.000000 steam-sdk-2023.6.2/steam_sdk/plotters/PlotterParametric.py
+-rw-rw-rw-   0        0        0     8863 2023-05-25 11:58:27.000000 steam-sdk-2023.6.2/steam_sdk/plotters/PlotterRoxie.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/plotters/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:59:09.238478 steam-sdk-2023.6.2/steam_sdk/postprocs/
+-rw-rw-rw-   0        0        0     5564 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/postprocs/PostprocsMetrics.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/postprocs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:59:09.284601 steam-sdk-2023.6.2/steam_sdk/utils/
+-rw-rw-rw-   0        0        0     2679 2023-03-15 09:29:53.000000 steam-sdk-2023.6.2/steam_sdk/utils/MTF_reading_functions.py
+-rw-rw-rw-   0        0        0    14942 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/utils/ModifyModelData.py
+-rw-rw-rw-   0        0        0     4762 2023-06-02 08:04:34.000000 steam-sdk-2023.6.2/steam_sdk/utils/ModifyModelDataMagnet.py
+-rw-rw-rw-   0        0        0     2745 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/utils/ModifyModelDataconductor.py
+-rw-rw-rw-   0        0        0      313 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/utils/NumpyEncoder.py
+-rw-rw-rw-   0        0        0     3151 2023-06-02 08:04:34.000000 steam-sdk-2023.6.2/steam_sdk/utils/ParserRoxieHelpers.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/utils/__init__.py
+-rw-rw-rw-   0        0        0      686 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/utils/clean_NaN_from_signal.py
+-rw-rw-rw-   0        0        0     3837 2023-03-15 09:29:53.000000 steam-sdk-2023.6.2/steam_sdk/utils/compare_two_parameters.py
+-rw-rw-rw-   0        0        0      590 2023-05-09 14:50:57.000000 steam-sdk-2023.6.2/steam_sdk/utils/create_coordinate_file_SIGMA.py
+-rw-rw-rw-   0        0        0     1279 2023-04-24 12:48:33.000000 steam-sdk-2023.6.2/steam_sdk/utils/get_attribute_type.py
+-rw-rw-rw-   0        0        0      167 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/utils/isNaN.py
+-rw-rw-rw-   0        0        0      299 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/utils/make_folder_if_not_existing.py
+-rw-rw-rw-   0        0        0     4512 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/utils/misc.py
+-rw-rw-rw-   0        0        0     1592 2023-04-24 12:48:33.000000 steam-sdk-2023.6.2/steam_sdk/utils/parse_str_to_list.py
+-rw-rw-rw-   0        0        0      388 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/utils/rgetattr.py
+-rw-rw-rw-   0        0        0      460 2023-01-11 12:50:11.000000 steam-sdk-2023.6.2/steam_sdk/utils/rhasattr.py
+-rw-rw-rw-   0        0        0      383 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/utils/sgetattr.py
+-rw-rw-rw-   0        0        0      863 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/utils/tic_toc.py
+-rw-rw-rw-   0        0        0      168 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/utils/unique.py
+-rw-rw-rw-   0        0        0     7005 2023-05-11 09:21:50.000000 steam-sdk-2023.6.2/steam_sdk/utils/utils_PC.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:59:09.292722 steam-sdk-2023.6.2/steam_sdk/viewers/
+-rw-rw-rw-   0        0        0    35919 2023-03-23 12:53:02.000000 steam-sdk-2023.6.2/steam_sdk/viewers/Viewer.py
+-rw-rw-rw-   0        0        0     6127 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/viewers/ViewerMeas.py
+-rw-rw-rw-   0        0        0     1667 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/viewers/ViewerSim.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/viewers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:59:09.296723 steam-sdk-2023.6.2/steam_sdk/wrappers/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.2/steam_sdk/wrappers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:59:09.299987 steam-sdk-2023.6.2/steam_sdk/wrappers/java/
+drwxrwxrwx   0        0        0        0 2023-06-02 10:59:09.300988 steam-sdk-2023.6.2/steam_sdk/wrappers/java/SING/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:43.000000 steam-sdk-2023.6.2/steam_sdk/wrappers/java/SING/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:59:09.302987 steam-sdk-2023.6.2/steam_sdk/wrappers/java/SING/jars/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:43.000000 steam-sdk-2023.6.2/steam_sdk/wrappers/java/SING/jars/__init__.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:43.000000 steam-sdk-2023.6.2/steam_sdk/wrappers/java/__init__.py
+-rw-rw-rw-   0        0        0     1834 2022-11-02 10:29:43.000000 steam-sdk-2023.6.2/steam_sdk/wrappers/wrapper_yaml.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:59:09.040619 steam-sdk-2023.6.2/steam_sdk.egg-info/
+-rw-rw-rw-   0        0        0     1550 2023-06-02 10:59:06.000000 steam-sdk-2023.6.2/steam_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6763 2023-06-02 10:59:06.000000 steam-sdk-2023.6.2/steam_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 10:59:06.000000 steam-sdk-2023.6.2/steam_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1596 2023-06-02 10:59:06.000000 steam-sdk-2023.6.2/steam_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-02 10:59:06.000000 steam-sdk-2023.6.2/steam_sdk.egg-info/top_level.txt
```

### Comparing `steam-sdk-2023.6.0/PKG-INFO` & `steam-sdk-2023.6.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: steam-sdk
-Version: 2023.6.0
+Version: 2023.6.2
 Summary: Source code for APIs for STEAM tools.
 Home-page: https://gitlab.cern.ch/steam/steam_sdk
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: CERN,STEAM,SDK,API
+Keywords: CERN,SDK,STEAM,API
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM_SDK
```

### Comparing `steam-sdk-2023.6.0/setup.py` & `steam-sdk-2023.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='steam-sdk',
-    version="2023.6.0",
+    version="2023.6.2",
     author="STEAM Team",
     author_email="steam-team@cern.ch",
     description="Source code for APIs for STEAM tools.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://gitlab.cern.ch/steam/steam_sdk",
     keywords={'STEAM', 'API', 'SDK', 'CERN'},
```

### Comparing `steam-sdk-2023.6.0/steam_sdk/analyses/AnalysisSTEAM.py` & `steam-sdk-2023.6.2/steam_sdk/analyses/AnalysisSTEAM.py`

 * *Files 0% similar despite different names*

```diff
@@ -330,14 +330,16 @@
                 flag_yaml = True  # Hard-coded for the moment
                 self.setup_sim_LEDET(simulation_name=step.simulation_name, sim_number=step.simulation_number,
                                      flag_yaml=flag_yaml, flag_json=flag_json)
             if 'PyBBQ' in step.software:
                 self.setup_sim_PyBBQ(simulation_name=step.simulation_name, sim_number=step.simulation_number)
             if 'PSPICE' in step.software:
                 self.setup_sim_PSPICE(simulation_name=step.simulation_name, sim_number=step.simulation_number)
+            if 'SIGMA' in step.software: #ADDED
+                self.setup_sim_SIGMA(simulation_name=step.simulation_name, sim_number=step.simulation_number)
             if 'XYCE' in step.software:
                 self.setup_sim_XYCE(simulation_name=step.simulation_name, sim_number=step.simulation_number)
 
         # Add the reference to the model in the dictionary
         self.list_models[step.model_name] = BM
 
     def step_modify_model(self, step, verbose: bool = False):
@@ -424,15 +426,15 @@
                 if 'LEDET' in step.software:
                     flag_json = BM.flag_json
                     flag_yaml = True  # Hard-coded for the moment
                     BM.buildLEDET()
                     self.setup_sim_LEDET(simulation_name=step.simulation_name, sim_number=simulation_number,
                                          flag_yaml=flag_yaml, flag_json=flag_json)
                 if 'SIGMA' in step.software:
-                    make_folder_if_not_existing(os.path.join(self.settings.local_SIGMA_folder, f"{step.simulation_name}_{simulation_number}") )#ADDED
+                    make_folder_if_not_existing(os.path.join(self.settings.local_SIGMA_folder, step.simulation_name, f"{step.simulation_name}_{simulation_number}") )#ADDED
                     BM.buildSIGMA(f"{step.simulation_name}_{simulation_number}", self.library_path)
                     self.setup_sim_SIGMA(simulation_name=step.simulation_name, sim_number=simulation_number)
                 if 'PyBBQ' in step.software:
                     BM.buildPyBBQ()
                     self.setup_sim_PyBBQ(simulation_name=step.simulation_name, sim_number=simulation_number)
                 if 'PSPICE' in step.software:
                     BM.buildPSPICE()
@@ -1042,15 +1044,15 @@
         The original file is then deleted.
         """
 
         # Add simulation number to the list
         self.list_sims.append(sim_number)
 
         # Make simulation folder
-        local_model_folder = os.path.join(self.settings.local_SIGMA_folder, f'{simulation_name}_{str(sim_number)}')
+        local_model_folder = os.path.join(self.settings.local_SIGMA_folder, simulation_name, f'{simulation_name}_{str(sim_number)}')
         make_folder_if_not_existing(local_model_folder)
         sources_folder = os.path.join(local_model_folder, 'sources')
         make_folder_if_not_existing(sources_folder)
         input_folder = os.path.join(local_model_folder, 'input')
         make_folder_if_not_existing(input_folder)
         output_folder = os.path.join(local_model_folder, 'output')
         make_folder_if_not_existing(output_folder)
@@ -1312,15 +1314,15 @@
             local_model_folder = Path(
                 Path(self.settings.local_XYCE_folder) / simulation_name / str(sim_number)).resolve()
             dXYCE = DriverXYCE(path_exe=self.settings.XYCE_path, path_folder_XYCE=local_model_folder, verbose=verbose)
             dXYCE.run_XYCE(simulation_name, suffix='')
         elif software == 'SIGMA':
             local_analysis_folder = simulation_name + '_' + str(sim_number)
             ds = DriverSIGMA(path_folder_SIGMA=self.settings.local_SIGMA_folder,
-                             path_folder_SIGMA_input=os.path.join(self.settings.local_SIGMA_folder,
+                             path_folder_SIGMA_input=os.path.join(self.settings.local_SIGMA_folder, simulation_name,
                                                                       local_analysis_folder), local_analysis_folder=local_analysis_folder, system_settings=self.settings, verbose=verbose)
             ds.run_SIGMA(simulation_name)
         else:
             raise Exception(f'Software {software} not supported for automated running.')
 
 
     def write_stimuli_from_interpolation(self, step, verbose: bool = False):
```

### Comparing `steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py` & `steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py` & `steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py` & `steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py` & `steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py` & `steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py` & `steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py` & `steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py` & `steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py` & `steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py` & `steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py` & `steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py` & `steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py` & `steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py` & `steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py` & `steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py` & `steam-sdk-2023.6.2/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/builders/BuilderFiQuS.py` & `steam-sdk-2023.6.2/steam_sdk/builders/BuilderFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/builders/BuilderLEDET.py` & `steam-sdk-2023.6.2/steam_sdk/builders/BuilderLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/builders/BuilderModel.py` & `steam-sdk-2023.6.2/steam_sdk/builders/BuilderModel.py`

 * *Files 0% similar despite different names*

```diff
@@ -554,26 +554,27 @@
         else:
             bh_data_file_path = os.path.join(Path(__file__).parent.parent.parent, 'tests', 'builders', 'model_library',
                                              'magnets', 'roxie.bhdata')
 
         shutil.copyfile(bh_data_file_path, os.path.join(self.output_path, 'roxie.bhdata'))
 
         coord_source_prev = self.model_data.Options_SIGMA.postprocessing.out_2D_at_points.coordinate_source
-        if self.model_data.Options_SIGMA.postprocessing.out_2D_at_points.coordinate_source == None:
-            if self.model_data.Options_SIGMA.postprocessing.out_2D_at_points.map2d != None:
-                path_map2d = os.path.join(Path(self.path_bh).parent, self.model_data.GeneralParameters.magnet_name,
-                                          'input', self.model_data.Options_SIGMA.postprocessing.out_2D_at_points.map2d)
-                destination_map2d = os.path.join(self.output_path, simulation_name + "_ROXIE_REFERENCE.map2d")
-                # Copy map2d file
-                shutil.copyfile(path_map2d, destination_map2d)
-                coordinate_file_path = os.path.join(self.output_path, simulation_name + "_ROXIE_COORD.csv")
-                # Create coordinate file
-                create_coordinate_file(path_map2d, coordinate_file_path)
-                # Set file as coordinate_source
-                self.model_data.Options_SIGMA.postprocessing.out_2D_at_points.coordinate_source = coordinate_file_path
+        if simulation_name is not None:
+            if self.model_data.Options_SIGMA.postprocessing.out_2D_at_points.coordinate_source == None:
+                if self.model_data.Options_SIGMA.postprocessing.out_2D_at_points.map2d != None:
+                    path_map2d = os.path.join(Path(self.path_bh).parent, self.model_data.GeneralParameters.magnet_name,
+                                              'input', self.model_data.Options_SIGMA.postprocessing.out_2D_at_points.map2d)
+                    destination_map2d = os.path.join(self.output_path, simulation_name + "_ROXIE_REFERENCE.map2d")
+                    # Copy map2d file
+                    shutil.copyfile(path_map2d, destination_map2d)
+                    coordinate_file_path = os.path.join(self.output_path, simulation_name + "_ROXIE_COORD.csv")
+                    # Create coordinate file
+                    create_coordinate_file(path_map2d, coordinate_file_path)
+                    # Set file as coordinate_source
+                    self.model_data.Options_SIGMA.postprocessing.out_2D_at_points.coordinate_source = coordinate_file_path
 
         builder_SIGMA = BuilderSIGMA(model_data=self.model_data, roxie_data=self.roxie_data,
                                      flag_build=self.flag_build, flag_plot_all=self.flag_plot_all, verbose=self.verbose)
         self.model_data.Options_SIGMA.postprocessing.out_2D_at_points.coordinate_source = coord_source_prev
 
         # if map2d specified then copy to working folder,
```

### Comparing `steam-sdk-2023.6.0/steam_sdk/builders/BuilderProteCCT.py` & `steam-sdk-2023.6.2/steam_sdk/builders/BuilderProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/builders/BuilderPyBBQ.py` & `steam-sdk-2023.6.2/steam_sdk/builders/BuilderPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/builders/BuilderSIGMA.py` & `steam-sdk-2023.6.2/steam_sdk/builders/BuilderSIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/builders/SelfMutualInductanceCalculation.py` & `steam-sdk-2023.6.2/steam_sdk/builders/SelfMutualInductanceCalculation.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/builders/Solenoids.py` & `steam-sdk-2023.6.2/steam_sdk/builders/Solenoids.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/builders/geometricFunctions.py` & `steam-sdk-2023.6.2/steam_sdk/builders/geometricFunctions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx` & `steam-sdk-2023.6.2/steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/configs/tools_defaults/ToolDefaultReader.py` & `steam-sdk-2023.6.2/steam_sdk/configs/tools_defaults/ToolDefaultReader.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/data/DataAnalysis.py` & `steam-sdk-2023.6.2/steam_sdk/data/DataAnalysis.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/data/DataConductor.py` & `steam-sdk-2023.6.2/steam_sdk/data/DataConductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/data/DataDakota.py` & `steam-sdk-2023.6.2/steam_sdk/data/DataDakota.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/data/DataEventCircuit.py` & `steam-sdk-2023.6.2/steam_sdk/data/DataEventCircuit.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/data/DataEventMagnet.py` & `steam-sdk-2023.6.2/steam_sdk/data/DataEventMagnet.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/data/DataFiQuS.py` & `steam-sdk-2023.6.2/steam_sdk/data/DataFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/data/DataLEDET.py` & `steam-sdk-2023.6.2/steam_sdk/data/DataLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/data/DataModelCircuit.py` & `steam-sdk-2023.6.2/steam_sdk/data/DataModelCircuit.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/data/DataModelConductor.py` & `steam-sdk-2023.6.2/steam_sdk/data/DataModelConductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/data/DataModelMagnet.py` & `steam-sdk-2023.6.2/steam_sdk/data/DataModelMagnet.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/data/DataParsimConductor.py` & `steam-sdk-2023.6.2/steam_sdk/data/DataParsimConductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/data/DataProteCCT.py` & `steam-sdk-2023.6.2/steam_sdk/data/DataProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/data/DataPyBBQ.py` & `steam-sdk-2023.6.2/steam_sdk/data/DataPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/data/DataRoxieParser.py` & `steam-sdk-2023.6.2/steam_sdk/data/DataRoxieParser.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/data/DataSIGMA.py` & `steam-sdk-2023.6.2/steam_sdk/data/DataSIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/data/DataSettings.py` & `steam-sdk-2023.6.2/steam_sdk/data/DataSettings.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,26 +6,24 @@
         Dataclass of settings for STEAM analyses
         This will be populated either form a local settings file (if flag_permanent_settings=False)
         or from the keys in the input analysis file (if flag_permanent_settings=True)
     """
     comsolexe_path:       str = None  # full path to comsol.exe, only COMSOL53a is supported
     JAVA_jdk_path:        str = None  # full path to folder with java jdk
     CFunLibPath:          str = None  # path to dll files with material properties
-    ANSYS_path:           str = None
     COSIM_path:           str = None  #
     Dakota_path:          str = None  #
     FiQuS_path:           str = None  #
     GetDP_path:           str = None  # full path to CERN GetDP build executable
     LEDET_path:           str = None  #
     ProteCCT_path:        str = None  #
     PSPICE_path:          str = None  #
     PyBBQ_path:           str = None  #
     XYCE_path:            str = None  #
     PSPICE_library_path:  str = None  #
-    local_COSIM_folder:   str = None  #
     local_Dakota_path:    str = None  # full path to local Dakota folder
     local_FiQuS_folder:   str = None  # full path to local FiQuS folder
     local_LEDET_folder:   str = None  # full path to local LEDET folder
     local_PyBBQ_folder:   str = None  # full path to local PyBBQ folder
     local_PSPICE_folder:  str = None  # full path to local PSPICE folder
     local_SIGMA_folder:   str = None  # full path to local SIGMA folder
     local_XYCE_folder:    str = None  # full path to local PSPICE folder
```

### Comparing `steam-sdk-2023.6.0/steam_sdk/data/DataSignal.py` & `steam-sdk-2023.6.2/steam_sdk/data/DataSignal.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/data/DictionaryLEDET.py` & `steam-sdk-2023.6.2/steam_sdk/data/DictionaryLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/data/DictionaryProteCCT.py` & `steam-sdk-2023.6.2/steam_sdk/data/DictionaryProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/data/DictionaryPyBBQ.py` & `steam-sdk-2023.6.2/steam_sdk/data/DictionaryPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/data/TemplateLEDET.py` & `steam-sdk-2023.6.2/steam_sdk/data/TemplateLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/data/TemplateProteCCT.py` & `steam-sdk-2023.6.2/steam_sdk/data/TemplateProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/drivers/DriverAnalysis.py` & `steam-sdk-2023.6.2/steam_sdk/drivers/DriverAnalysis.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/drivers/DriverDakota.py` & `steam-sdk-2023.6.2/steam_sdk/drivers/DriverDakota.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/drivers/DriverFiQuS.py` & `steam-sdk-2023.6.2/steam_sdk/drivers/DriverFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/drivers/DriverLEDET.py` & `steam-sdk-2023.6.2/steam_sdk/drivers/DriverLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/drivers/DriverPSPICE.py` & `steam-sdk-2023.6.2/steam_sdk/drivers/DriverPSPICE.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/drivers/DriverProteCCT.py` & `steam-sdk-2023.6.2/steam_sdk/drivers/DriverProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/drivers/DriverPyBBQ.py` & `steam-sdk-2023.6.2/steam_sdk/drivers/DriverPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/drivers/DriverSIGMA.py` & `steam-sdk-2023.6.2/steam_sdk/drivers/DriverSIGMA.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,27 @@
-import glob
 import os
 import subprocess
 from pathlib import Path
-
 import pandas as pd
-import yaml
-
-from steam_sdk.builders.BuilderSIGMA import BuilderSIGMA
-from steam_sdk.data.DataModelMagnet import DataModelMagnet
 from steam_sdk.parsers.ParserCOMSOLToTxt import ParserCOMSOLToTxt
-from steam_sdk.parsers.ParserRoxie import ParserRoxie
+from steam_pysigma.MainSIGMA import MainSIGMA as MF
 
 
 class DriverSIGMA:
     """
         Class to drive SIGMA models
     """
 
     def __init__(self,
                  path_folder_SIGMA,
                  path_folder_SIGMA_input, local_analysis_folder, system_settings, verbose=False):
         self.path_folder_SIGMA = path_folder_SIGMA
         self.path_folder_SIGMA_input = path_folder_SIGMA_input
         self.local_analysis_folder = local_analysis_folder
         self.system_settings = system_settings
-        from steam_pysigma.MainSIGMA import MainSIGMA as MF
         self.MainSIGMA = MF
 
     @staticmethod
     def export_all_txt_to_concat_csv():
         """
         Export 1D plots vs time to a concatenated csv file. This file can be utilized with the Viewer.
         :return:
@@ -45,24 +38,25 @@
             df_concat = df_concat.loc[:, ~df_concat.columns.duplicated()]
             print(df_concat)
         df_concat = df_concat.reset_index(drop=True)
         df_concat.to_csv("SIGMA_transient_concat_output_1234567890MF.csv", index=False)
 
     def run_SIGMA(self, simulation_name):
         # input_file_path = os.path.join(self.path_folder_SIGMA_input, sim_file_name + '.yaml')
-        model_folder = os.path.join(self.path_folder_SIGMA, self.local_analysis_folder, 'input')
+        current_path = os.getcwd()
+        model_folder = os.path.join(self.path_folder_SIGMA, simulation_name, self.local_analysis_folder, 'input')
         input_file_path = os.path.join(model_folder, self.local_analysis_folder+"_SIGMA.yaml")
         # Run model
-        bh_curve_database = os.path.join(self.path_folder_SIGMA, self.local_analysis_folder, 'sources',
+        bh_curve_database = os.path.join(self.path_folder_SIGMA, simulation_name, self.local_analysis_folder, 'sources',
                      'roxie.bhdata')
-        input_coordinates_path = os.path.join(self.path_folder_SIGMA, self.local_analysis_folder, 'sources',
+        input_coordinates_path = os.path.join(self.path_folder_SIGMA, simulation_name, self.local_analysis_folder, 'sources',
                      self.local_analysis_folder + "_ROXIE_COORD.csv")
         if not Path(input_coordinates_path).exists():
             input_coordinates_path = None
-        path_to_results = os.path.join(self.path_folder_SIGMA, self.local_analysis_folder, 'output')
+        path_to_results = os.path.join(self.path_folder_SIGMA, simulation_name, self.local_analysis_folder, 'output')
         if not Path(path_to_results).exists():
             path_to_results = None
         print(f"Using {model_folder} as input file path")
         print(f"Using {input_file_path} yaml source path")
         print(f"Using {input_coordinates_path} as coordinate file path")
         print(f"Using {bh_curve_database} as bh file path")
         print(f"Using {path_to_results} as path to results")
@@ -74,13 +68,30 @@
         os.chdir(model_folder)
         batch_file_path = os.path.join(model_folder, f"{simulation_name}_Model_Compile_and_Open.bat")
         print(f'Running Comsol model via: {batch_file_path}')
         subprocess.call(batch_file_path)
         proc = subprocess.Popen([batch_file_path], stdout=subprocess.PIPE, stderr=subprocess.PIPE,
                                 universal_newlines=True)
         (stdout, stderr) = proc.communicate()
+
+        log_file_path = os.path.join(path_to_results, "log_bat_file.txt")
+
         if proc.returncode != 0:
             print(stderr)
+            raise ValueError(f"Batch file throws an error, COMSOL model could not be completed! Review error at {log_file_path}.")
         else:
             print(stdout)
+            for line in stdout.split('\n'):
+                if "error" in line.lower():
+                    raise ValueError(
+                        f"Batch file throws an error, COMSOL model could not be completed! Review log at {log_file_path}.")
+
+            print(f"Running batch file passes! See log file at {log_file_path}.")
+
+        with open(log_file_path, 'w') as logfile:
+            logfile.write(stdout)
+        #Return to recovery path
+        os.chdir(current_path)
+
+
```

### Comparing `steam-sdk-2023.6.0/steam_sdk/drivers/DriverXYCE.py` & `steam-sdk-2023.6.2/steam_sdk/drivers/DriverXYCE.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/parsers/CSD_Reader.py` & `steam-sdk-2023.6.2/steam_sdk/parsers/CSD_Reader.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/parsers/ParserCond2d.py` & `steam-sdk-2023.6.2/steam_sdk/parsers/ParserCond2d.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/parsers/ParserCsd.py` & `steam-sdk-2023.6.2/steam_sdk/parsers/ParserCsd.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/parsers/ParserCsv.py` & `steam-sdk-2023.6.2/steam_sdk/parsers/ParserCsv.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/parsers/ParserDakota.py` & `steam-sdk-2023.6.2/steam_sdk/parsers/ParserDakota.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/parsers/ParserDatToCsv.py` & `steam-sdk-2023.6.2/steam_sdk/parsers/ParserDatToCsv.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/parsers/ParserExcel.py` & `steam-sdk-2023.6.2/steam_sdk/parsers/ParserExcel.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/parsers/ParserFiQuS.py` & `steam-sdk-2023.6.2/steam_sdk/parsers/ParserFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/parsers/ParserLEDET.py` & `steam-sdk-2023.6.2/steam_sdk/parsers/ParserLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/parsers/ParserMap2d.py` & `steam-sdk-2023.6.2/steam_sdk/parsers/ParserMap2d.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/parsers/ParserMat.py` & `steam-sdk-2023.6.2/steam_sdk/parsers/ParserMat.py`

 * *Files 18% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     :param full_name_file: full path to the mat file
     :param list_signals: list of signals to read
     :return: dataframe with the selected signals
     '''
 
     with h5py.File(full_name_file, 'r') as simulationSignals:
         df_signals = pd.DataFrame()
-        number_of_time_steps = len(simulationSignals['time_vector'])  #TODO it is bad to hard-code this logic!
+        number_of_time_steps = len(simulationSignals['time_vector'])
         for label_signal in list_signals:
             if ('(' in label_signal) and (')' in label_signal):
                 # Special case: Only certain columns will be read
                 label_signal_split = label_signal.split('(')
                 signal        = label_signal_split[0]
                 rows_columns  = label_signal_split[1].rstrip(')').split(',')
                 label_rows    = rows_columns[0]
@@ -151,77 +151,14 @@
 
             simulationSignal = simulationSignal.flatten()
             df = pd.DataFrame({label_signal: simulationSignal})
             df_signals = pd.concat([df_signals, df], axis=1)
     return df_signals
 
 
-def get_signals_from_mat_to_dict(full_name_file: str, list_signals, bool_transpose: bool = True):
-    '''
-    Reads a mat file and returns a dataframe with the selected signals
-
-    Note: The selected signals can also be define with a special syntax that allows accessing one certain row or column (1-indexed).
-          Example: U_CoilSections(:,2) allows reading the 2nd column of the variable named U_CoilSections
-          Example: U_CoilSections(3,:) allows reading the 3rd row of the variable named U_CoilSections
-          Multiple columns/rows selection not currently supported  #TODO it would be nice to add
-
-    :param full_name_file: full path to the mat file
-    :param list_signals: list of signals to read
-    :return: dict with the selected signals
-    '''
-
-    with h5py.File(full_name_file, 'r') as simulationSignals:
-        dict_signals = {}
-        number_of_time_steps = len(simulationSignals['time_vector'])  #TODO it is bad to hard-code this logic!
-        for label_signal in list_signals:
-            if ('(' in label_signal) and (')' in label_signal):
-                # Special case: Only certain columns will be read
-                label_signal_split = label_signal.split('(')
-                signal        = label_signal_split[0]
-                rows_columns  = label_signal_split[1].rstrip(')').split(',')
-                label_rows    = rows_columns[0]
-                label_columns = rows_columns[1]
-
-
-                # Find slice of selected rows
-                if label_rows == ':':
-                    rows = slice(0, simulationSignals[signal].shape[1])
-                elif ':' in label_rows:
-                    raise Exception('Multiple rows selection not currently supported.')
-                    # label_rows_split = label_rows.split(':')
-                    # rows = slice(int(label_rows_split[0]) - 1, int(label_rows_split[1]) - 1)
-                else:
-                    rows = int(label_rows)
-
-                # Find slice of selected columns
-                if label_columns == ':':
-                    columns = slice(0, simulationSignals[signal].shape[0])
-                elif ':' in label_columns:
-                    raise Exception('Multiple columns selection not currently supported.')
-                    # label_columns_split = label_columns.split(':')
-                    # columns = slice(int(label_columns_split[0])-1, int(label_columns_split[1])-1)
-                else:
-                    columns = int(label_columns)-1
-
-                # Apply slices
-                if bool_transpose:
-                    simulationSignal = np.array(simulationSignals[signal][columns, rows])
-                else:
-                    simulationSignal = np.array(simulationSignals[signal][rows, columns])
-            else:
-                # Regular case: One-column signal is read
-                if bool_transpose:
-                    simulationSignal = np.array(simulationSignals[label_signal]).T
-                else:
-                    simulationSignal = np.array(simulationSignals[label_signal])
-
-            dict_signals[label_signal] = simulationSignal
-    return dict_signals
-
-
 def print_shapes_of_entries(simulationSignals):
     shapes_dict = {}
     for key, value in simulationSignals.items():
         # Check if the value is a dataset
         if isinstance(value, h5py.Dataset):
             # Check the shape of the dataset
             shape = value.shape
```

### Comparing `steam-sdk-2023.6.0/steam_sdk/parsers/ParserPSPICE.py` & `steam-sdk-2023.6.2/steam_sdk/parsers/ParserPSPICE.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/parsers/ParserPdf.py` & `steam-sdk-2023.6.2/steam_sdk/parsers/ParserPdf.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/parsers/ParserProteCCT.py` & `steam-sdk-2023.6.2/steam_sdk/parsers/ParserProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/parsers/ParserProtePyBBQ.py` & `steam-sdk-2023.6.2/steam_sdk/parsers/ParserProtePyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/parsers/ParserRoxie.py` & `steam-sdk-2023.6.2/steam_sdk/parsers/ParserRoxie.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,22 @@
 from typing import Dict
 
 from steam_sdk.builders import geometricFunctions as gf
 from steam_sdk.data import DataRoxieParser as pd
 # import matplotlib.pyplot as plt
 # import matplotlib.lines as lines
 # import matplotlib.patches as patches
+from matplotlib import cm
+from matplotlib.colors import Normalize
+import matplotlib.pyplot as plt
+from matplotlib.lines import Line2D
+from matplotlib.patches import Arc
+
+from steam_sdk.parsers.ParserYamlToRoxie import ParserYamlToRoxie
+from steam_sdk.utils.ParserRoxieHelpers import find_iH_oH_iL_oL
 
 
 def arc_angle_between_point_and_abscissa(p, c):
     """
         Returns the angle of an arc with center c and endpoints at (cx + radius, cy) and (px, py)
         :param p: list of x and y coordinates of a point
         :param c: list of x and y coordinates of the arc center
@@ -459,15 +467,15 @@
         data = self.rawData.cadata  # self.data.cadata
 
         if cadata_content:
             fileContent = cadata_content
         else:
             file = open(self.dir_cadata, "r")
             fileContent = file.read()
-
+        self.windings=[]
         # separate rows
         fileContentByRow = fileContent.split("\n")
 
         for index in range(len(fileContentByRow)):
             fc = fileContentByRow[index]
 
             if fc[0:5] == "CABLE":
@@ -652,18 +660,23 @@
                         else:
                             if group_nr not in groups_list and block_nr not in trans_blocks_list:
                                 raise Exception('The current block is not transformed or belongs to a group that is not'
                                                 'transformed: check "BCS" under "EULER" in the .data file.')
 
                     radius = float(rowSplitStr[3])
                     layer = self.layer_radius.index(radius) + 1
-
+                    imag = int(rowSplitStr[10])
                     turn = float(rowSplitStr[11])
                     if 'symm' in locals():
+                        Avalue= turn * symm / 360 + 1
                         pole = floor(turn * symm / 360 + 1)
+                        # if imag==1 and turn ==0 or imag==0 and turn ==180:
+                        #     pole=2
+                        # else:
+                        #     pole = 1
                     else:
                         pole = block_nr
 
                     data.blocks[rowSplitStr[0]] = pd.Block(type=int(rowSplitStr[1]), nco=int(rowSplitStr[2]),
                                                            radius=radius, phi=float(rowSplitStr[4]),
                                                            alpha=float(rowSplitStr[5]), current=float(rowSplitStr[6]),
                                                            condname=rowSplitStr[7], n1=int(rowSplitStr[8]),
@@ -720,16 +733,20 @@
 
         # Blocks to add to the attribute group.blocks
         blockToAddToGroup = []
 
         # Apply multipole geometry
         if self.group.typexy == 0:
             if verbose:
-                print('typexy = {}: No symmetry action.'.format(self.group.typexy))
-
+                print('typexy = {}: No symmetry action.'.format(self.group.typexy)) ## Pull winding data from yaml files.
+                # here get the winding data from the yaml file. Overwrite the already defined windings in the data.
+                # Function is placed outside this file.
+            # path_model_data = "C:\\Users\\jlidholm\\cernbox\\Git-projects\\steam_sdk\\tests\\builders\\model_library\\magnets\\MED_C_COMB\\input\\modelData_MED_C_COMB.yaml"
+            # pyr = ParserYamlToRoxie(path_model_data)
+            # self.windings = pyr.read_model_data_yaml()
         elif self.group.typexy == 1:
             if verbose:
                 print('typexy = {}: All.'.format(self.group.typexy))
 
             for additionalBlock in self.group.blocks:
                 nOriginalBlocks = nb
                 # idxBlock = additionalBlock - 1
@@ -955,15 +972,15 @@
                     print('Group {} has symmetry of type {} --> Not currently supported.'.format(self.no,
                                                                                                  self.group.symm))
 
         if verbose:
             print('Total number of blocks: {}'.format(len(data.blocks)))
             # Print each BlockParameters object in the list
             for bValue in data.blocks:
-                print(bValue.toString())
+                print(str(bValue))
 
         return data
 
     def applyTransformations(self, coil: pd.Coil = None, verbose: bool = False):
         """
             **Returns updated list of blockParametersList objects, and sets attribute blockParametersList**
 
@@ -1396,22 +1413,37 @@
         # self.ax.add_patch(patches.Circle((coil.bore_center.x, coil.bore_center.y), radius=radius, color='b'))
         # self.ax.add_line(lines.Line2D([corner0[0], corner3[0]], [corner0[1], corner3[1]], color='red'))
         # self.ax.add_line(lines.Line2D([corner3[0], corner2[0]], [corner3[1], corner2[1]], color='red'))
         # self.ax.add_line(lines.Line2D([corner2[0], corner1[0]], [corner2[1], corner1[1]], color='red'))
         # self.ax.add_line(lines.Line2D([corner1[0], corner0[0]], [corner1[1], corner0[1]], color='red'))
         # plt.show()
         if self.block.type == 2 or self.block.nco == 1:
-            block.block_corners.iH = pd.Coord(x=sigDig(corner0[0]), y=sigDig(corner0[1]))  # 1
-            block.block_corners.oH = pd.Coord(x=sigDig(corner3[0]), y=sigDig(corner3[1]))  # 4
-            block.block_corners.iL = pd.Coord(x=sigDig(corner1[0]), y=sigDig(corner1[1]))  # 2
-            block.block_corners.oL = pd.Coord(x=sigDig(corner2[0]), y=sigDig(corner2[1]))  # 3
-            block.block_corners_ins.iH = pd.Coord(x=sigDig(corner0[0]), y=sigDig(corner0[1]))  # 1
-            block.block_corners_ins.oH = pd.Coord(x=sigDig(corner3[0]), y=sigDig(corner3[1]))  # 4
-            block.block_corners_ins.iL = pd.Coord(x=sigDig(corner1[0]), y=sigDig(corner1[1]))  # 2
-            block.block_corners_ins.oL = pd.Coord(x=sigDig(corner2[0]), y=sigDig(corner2[1]))  # 3
+            # block.block_corners.iH = pd.Coord(x=sigDig(corner0[0]), y=sigDig(corner0[1]))  # 1
+            # block.block_corners.oH = pd.Coord(x=sigDig(corner3[0]), y=sigDig(corner3[1]))  # 4
+            # block.block_corners.iL = pd.Coord(x=sigDig(corner1[0]), y=sigDig(corner1[1]))  # 2
+            # block.block_corners.oL = pd.Coord(x=sigDig(corner2[0]), y=sigDig(corner2[1]))  # 3
+            # block.block_corners_ins.iH = pd.Coord(x=sigDig(corner0[0]), y=sigDig(corner0[1]))  # 1
+            # block.block_corners_ins.oH = pd.Coord(x=sigDig(corner3[0]), y=sigDig(corner3[1]))  # 4
+            # block.block_corners_ins.iL = pd.Coord(x=sigDig(corner1[0]), y=sigDig(corner1[1]))  # 2
+            # block.block_corners_ins.oL = pd.Coord(x=sigDig(corner2[0]), y=sigDig(corner2[1]))  # 3
+            bore_center = (0.0,0.0)
+            p1 = (corner0[0], corner0[1])
+            p2 = (corner1[0], corner1[1])
+            p3 = (corner2[0], corner2[1])
+            p4 = (corner3[0], corner3[1])
+            point_oH, point_oL, point_iH, point_iL = find_iH_oH_iL_oL(p1, p2, p3, p4, bore_center)
+            block.block_corners.iH = pd.Coord(x=sigDig(point_iH[0]), y=sigDig(point_iH[1]))  # 1
+            block.block_corners.oH = pd.Coord(x=sigDig(point_oH[0]), y=sigDig(point_oH[1]))  # 4
+            block.block_corners.iL = pd.Coord(x=sigDig(point_iL[0]), y=sigDig(point_iL[1]))  # 2
+            block.block_corners.oL = pd.Coord(x=sigDig(point_oL[0]), y=sigDig(point_oL[1]))  # 3
+            block.block_corners_ins.iH = pd.Coord(x=sigDig(point_iH[0]), y=sigDig(point_iH[1]))  # 1
+            block.block_corners_ins.oH = pd.Coord(x=sigDig(point_oH[0]), y=sigDig(point_oH[1]))  # 4
+            block.block_corners_ins.iL = pd.Coord(x=sigDig(point_iL[0]), y=sigDig(point_iL[1]))  # 2
+            block.block_corners_ins.oL = pd.Coord(x=sigDig(point_oL[0]), y=sigDig(point_oL[1]))  # 3
+
         else:
             new_corners_inner = gf.intersectLineCircle(gf.findLineThroughTwoPoints(corner0, corner3),
                                                        [radius, coil.bore_center.x, coil.bore_center.y])
             if min(abs(new_corners_inner[0][0] - corner0[0]),
                    abs(new_corners_inner[1][0] - corner0[0])) == abs(new_corners_inner[0][0] - corner0[0]):
                 new_inner = new_corners_inner[0]
             else:
@@ -1456,33 +1488,61 @@
             #     gf.findLineThroughTwoPoints(corner1, corner2),
             #     [new_outer_radius, coil.bore_center.x, coil.bore_center.y])
             # if min(abs(new_corners_outer_mid[0][0] - corner2[0]),
             #        abs(new_corners_outer_mid[1][0] - corner2[0])) == abs(new_corners_outer_mid[0][0] - corner2[0]):
             #     mid_outer_beg = new_corners_outer_mid[0]
             # else:
             #     mid_outer_beg = new_corners_outer_mid[1]
-
-            if self.block.imag == 0:
-                block.block_corners.iH = pd.Coord(x=sigDig(mid_inner_end[0]), y=sigDig(mid_inner_end[1]))  # 1
-                block.block_corners.oH = pd.Coord(x=sigDig(mid_outer_end[0]), y=sigDig(mid_outer_end[1]))  # 4
-                block.block_corners.iL = pd.Coord(x=sigDig(mid_inner_beg[0]), y=sigDig(mid_inner_beg[1]))  # 2
-                block.block_corners.oL = pd.Coord(x=sigDig(mid_outer_beg[0]), y=sigDig(mid_outer_beg[1]))  # 3
-                block.block_corners_ins.iH = pd.Coord(x=sigDig(corner0[0]), y=sigDig(corner0[1]))  # 1
-                block.block_corners_ins.oH = pd.Coord(x=sigDig(corner3[0]), y=sigDig(corner3[1]))  # 4
-                block.block_corners_ins.iL = pd.Coord(x=sigDig(corner1[0]), y=sigDig(corner1[1]))  # 2
-                block.block_corners_ins.oL = pd.Coord(x=sigDig(corner2[0]), y=sigDig(corner2[1]))  # 3
-            else:
-                block.block_corners.iL = pd.Coord(x=sigDig(mid_inner_end[0]), y=sigDig(mid_inner_end[1]))
-                block.block_corners.oL = pd.Coord(x=sigDig(mid_outer_end[0]), y=sigDig(mid_outer_end[1]))
-                block.block_corners.iH = pd.Coord(x=sigDig(mid_inner_beg[0]), y=sigDig(mid_inner_beg[1]))
-                block.block_corners.oH = pd.Coord(x=sigDig(mid_outer_beg[0]), y=sigDig(mid_outer_beg[1]))
-                block.block_corners_ins.iL = pd.Coord(x=sigDig(corner0[0]), y=sigDig(corner0[1]))  # 1
-                block.block_corners_ins.oL = pd.Coord(x=sigDig(corner3[0]), y=sigDig(corner3[1]))  # 4
-                block.block_corners_ins.iH = pd.Coord(x=sigDig(corner1[0]), y=sigDig(corner1[1]))  # 2
-                block.block_corners_ins.oH = pd.Coord(x=sigDig(corner2[0]), y=sigDig(corner2[1]))  # 3
+            bore_center = (coil.bore_center.x,coil.bore_center.y)
+            p1 = (mid_inner_end[0], mid_inner_end[1])
+            p2 = (mid_outer_end[0], mid_outer_end[1])
+            p3 = (mid_inner_beg[0], mid_inner_beg[1])
+            p4 = (mid_outer_beg[0], mid_outer_beg[1])
+
+            point_oH, point_oL, point_iH, point_iL = find_iH_oH_iL_oL(p1, p2, p3, p4, bore_center)
+            p1 = (corner0[0], corner0[1])
+            p2 = (corner1[0], corner1[1])
+            p3 = (corner2[0], corner2[1])
+            p4 = (corner3[0], corner3[1])
+            point_oH_ins, point_oL_ins, point_iH_ins, point_iL_ins = find_iH_oH_iL_oL(p1, p2, p3, p4, bore_center)
+
+
+        if point_oH is None or point_oL is None or point_iH is None or point_iL is None:
+            print("Error!!!")
+
+        block.block_corners_ins.iH = pd.Coord(x=sigDig(point_iH_ins[0]), y=sigDig(point_iH_ins[1]))  # 1
+        block.block_corners_ins.oH = pd.Coord(x=sigDig(point_oH_ins[0]), y=sigDig(point_oH_ins[1]))  # 4
+        block.block_corners_ins.iL = pd.Coord(x=sigDig(point_iL_ins[0]), y=sigDig(point_iL_ins[1]))  # 2
+        block.block_corners_ins.oL = pd.Coord(x=sigDig(point_oL_ins[0]), y=sigDig(point_oL_ins[1]))  # 3
+
+        block.block_corners.iH = pd.Coord(x=sigDig(point_iH[0]), y=sigDig(point_iH[1]))  # 1
+        block.block_corners.oH = pd.Coord(x=sigDig(point_oH[0]), y=sigDig(point_oH[1]))  # 4
+        block.block_corners.iL = pd.Coord(x=sigDig(point_iL[0]), y=sigDig(point_iL[1]))  # 2
+        block.block_corners.oL = pd.Coord(x=sigDig(point_oL[0]), y=sigDig(point_oL[1]))  # 3
+        # OLD CODE
+            # if self.block.imag == 0:
+            #     block.block_corners.iH = pd.Coord(x=sigDig(mid_inner_end[0]), y=sigDig(mid_inner_end[1]))  # 1
+            #     block.block_corners.oH = pd.Coord(x=sigDig(mid_outer_end[0]), y=sigDig(mid_outer_end[1]))  # 4
+            #     block.block_corners.iL = pd.Coord(x=sigDig(mid_inner_beg[0]), y=sigDig(mid_inner_beg[1]))  # 2
+            #     block.block_corners.oL = pd.Coord(x=sigDig(mid_outer_beg[0]), y=sigDig(mid_outer_beg[1]))  # 3
+            #     block.block_corners_ins.iH = pd.Coord(x=sigDig(corner0[0]), y=sigDig(corner0[1]))  # 1
+            #     block.block_corners_ins.oH = pd.Coord(x=sigDig(corner3[0]), y=sigDig(corner3[1]))  # 4
+            #     block.block_corners_ins.iL = pd.Coord(x=sigDig(corner1[0]), y=sigDig(corner1[1]))  # 2
+            #     block.block_corners_ins.oL = pd.Coord(x=sigDig(corner2[0]), y=sigDig(corner2[1]))  # 3
+            # else:
+            #
+            #
+            #     block.block_corners.iL = pd.Coord(x=sigDig(mid_inner_end[0]), y=sigDig(mid_inner_end[1]))
+            #     block.block_corners.oL = pd.Coord(x=sigDig(mid_outer_end[0]), y=sigDig(mid_outer_end[1]))
+            #     block.block_corners.iH = pd.Coord(x=sigDig(mid_inner_beg[0]), y=sigDig(mid_inner_beg[1]))
+            #     block.block_corners.oH = pd.Coord(x=sigDig(mid_outer_beg[0]), y=sigDig(mid_outer_beg[1]))
+            #     block.block_corners_ins.iL = pd.Coord(x=sigDig(corner0[0]), y=sigDig(corner0[1]))  # 1
+            #     block.block_corners_ins.oL = pd.Coord(x=sigDig(corner3[0]), y=sigDig(corner3[1]))  # 4
+            #     block.block_corners_ins.iH = pd.Coord(x=sigDig(corner1[0]), y=sigDig(corner1[1]))  # 2
+            #     block.block_corners_ins.oH = pd.Coord(x=sigDig(corner2[0]), y=sigDig(corner2[1]))  # 3
 
             # new_corners_inner = gf.intersectLineCircle(
             #     gf.findLineThroughTwoPoints(corner0, corner3),
             #     [radius, coil.bore_center.x, coil.bore_center.y])
             # if min(abs(new_corners_inner[0][0] - corner0[0]),
             #        abs(new_corners_inner[1][0] - corner0[0])) == abs(new_corners_inner[0][0] - corner0[0]):
             #     new_inner = new_corners_inner[0]
@@ -1543,28 +1603,46 @@
         # plt.figure(figsize=(10, 10))
         # self.ax = plt.axes()
         # self.ax.set_xlim(-0.2, 0.2)
         # self.ax.set_ylim(-0.2, 0.2)
         for pair in blk_layers:
             self.no = int(pair[0])
             self.block = self.roxieData.coil.blocks[pair[0]]
-
+            # # Double check that the winding is correct.
+            # index = None
+            # #self.block.pole = 1
+            #
+            # for i, sublist in enumerate(self.windings):
+            #     if self.no in sublist:
+            #         index = i
+            #         break
+            #
+            # if index is not None:
+            #     print(f"The block {self.no} is present at index {index+1}.")
+            #     self.block.winding = index + 1
+            #     self.roxieData.coil.blocks[str(self.no)].winding = self.block.winding
+            #
+            # else:
+            #     print(f"The block {self.no} is not present in the list.")
+            #
             # Get desired conductor data
             self.cond_name = self.block.condname
             self.getConductorFromCableDatabase(cadata=cadata)
 
             # Calculate x/y positions of the conductor corners and strands
             if verbose:
                 print('Block {} is of type {} --> {}.'.format(self.no, self.block.type, blockTypes[self.block.type]))
 
             self.findConductorPositions(verbose=verbose)
-
-        # if verbose:
+        # for no, blk in self.roxieData.coil.blocks.items():
+        #     self.data.coil.physical_order.append(pd.Order(coil=blk.coil, pole=blk.pole, layer=blk.layer,
+        #                                                   winding=blk.winding, block=int(no)))
+        # # if verbose:
         #     print('Total number of conductors (half-turns): {}'.format(len(self.xPos)))
-        # plt.show()
+        #plt.show()
         return self.data.coil
 
     def getWedgePositions(self, coil: pd.CoilData = None, verbose: bool = False):
         """
             **Returns wedge positions**
 
             Find wedge positions
@@ -1576,14 +1654,73 @@
 
             :return: list
         """
         if coil:
             self.data = pd.RoxieData()
             self.data.coil = coil
 
+        xPos = []
+        yPos = []
+        xBarePos = []
+        yBarePos = []
+        iPos = []
+        xblockCorners = []
+        yblockCorners = []
+        colormap = cm.get_cmap('nipy_spectral')
+        ht_coil = []
+        block_coil = []
+
+        for eo in self.data.coil.physical_order:
+            out = self.data.coil.coils[eo.coil].poles[eo.pole].layers[eo.layer].windings[eo.winding].blocks[eo.block]
+            winding = self.data.coil.coils[eo.coil].poles[eo.pole].layers[eo.layer].windings[eo.winding]
+            block = winding.blocks[eo.block]
+            xblockCorners.append([block.block_corners.iH.x, block.block_corners.oH.x, block.block_corners.oL.x,
+                                  block.block_corners.iL.x])
+            yblockCorners.append([block.block_corners.iH.y, block.block_corners.oH.y, block.block_corners.oL.y,
+                                  block.block_corners.iL.y])
+            block_coil.append(eo.coil)
+            # Save half turn corners
+            for halfTurn_nr, halfTurn in block.half_turns.items():
+                insu = halfTurn.corners.insulated
+                bare = halfTurn.corners.bare
+                xPos.append([insu.iH.x, insu.oH.x, insu.oL.x, insu.iL.x])
+                yPos.append([insu.iH.y, insu.oH.y, insu.oL.y, insu.iL.y])
+                xBarePos.append([bare.iH.x, bare.oH.x, bare.oL.x, bare.iL.x])
+                yBarePos.append([bare.iH.y, bare.oH.y, bare.oL.y, bare.iL.y])
+                iPos.append(block.current_sign)
+
+        # Create normalized scale between zero and number of half turns.
+        normalize = Normalize(vmin=0, vmax=len(xPos))
+
+        # Plot blocks and block number in coil
+        max_size = max(max(xblockCorners, key=max))    # Plot bare half turns
+        for c, (cXBarePos, cYBarePos) in enumerate(zip(xBarePos, yBarePos)):
+            pt1, pt2, pt3, pt4 = (cXBarePos[0], cYBarePos[0]), (cXBarePos[1], cYBarePos[1]), \
+                                 (cXBarePos[2], cYBarePos[2]), (cXBarePos[3], cYBarePos[3])
+            if iPos[c] > 0:
+                line = plt.Polygon([pt1, pt2, pt3, pt4], closed=True, fill=True, facecolor='r', edgecolor='k',
+                                   alpha=.25)
+            else:
+                line = plt.Polygon([pt1, pt2, pt3, pt4], closed=True, fill=True, facecolor='b', edgecolor='k',
+                                   alpha=.25)
+            plt.gca().add_line(line)
+        for c, (xblockCorners, yblockCorners) in enumerate(zip(xblockCorners, yblockCorners)):
+            pt1, pt2, pt3, pt4 = (xblockCorners[0], yblockCorners[0]), (xblockCorners[1], yblockCorners[1]), \
+                                 (xblockCorners[2], yblockCorners[2]), (xblockCorners[3], yblockCorners[3])
+            line = Line2D([pt1[0], pt2[0]], [pt1[1], pt2[1]], color='b')
+            plt.gca().add_line(line)
+            line = Line2D([pt3[0], pt4[0]], [pt3[1], pt4[1]], color='b')
+            plt.gca().add_line(line)
+            bore_center_x, bore_center_y = (
+            self.data.coil.coils[block_coil[c]].bore_center.x, self.data.coil.coils[block_coil[c]].bore_center.y)
+            plot_arcs(pt4, pt1, (bore_center_x, bore_center_y), plt.gca())
+            plot_arcs(pt3, pt2, (bore_center_x, bore_center_y), plt.gca())
+            x_ave_cond, y_ave_cond = sum(xblockCorners) / len(xblockCorners), sum(yblockCorners) / len(yblockCorners)
+            plt.text(x_ave_cond, y_ave_cond, '{}'.format(c + 1), color='b', fontsize=14)
+
         # ax = plt.axes()
 
         wedge_no = 0
         for coil_nr, coil in self.data.coil.coils.items():
             for pole_nr, pole in coil.poles.items():
                 for layer_nr, layer in pole.layers.items():
                     for winding_key, winding in layer.windings.items():
@@ -1594,28 +1731,68 @@
 
                             for block_key, block in winding.blocks.items():
                                 wedge_no += 1
                                 self.data.wedges[wedge_no] = pd.Wedge()
                                 wedge = self.data.wedges[wedge_no]
 
                                 if blocks.index(block_key) == 0:
-                                    wedge.corners = pd.Corner(iH=adj_winding.blocks[adj_blocks[0]].block_corners.iL, iL=block.block_corners.iH,
-                                                              oH=adj_winding.blocks[adj_blocks[0]].block_corners.oL, oL=block.block_corners.oH)
-                                    wedge.corners_ins = pd.Corner(iH=adj_winding.blocks[adj_blocks[0]].block_corners_ins.iL, iL=block.block_corners_ins.iH,
-                                                                  oH=adj_winding.blocks[adj_blocks[0]].block_corners_ins.oL, oL=block.block_corners_ins.oH)
-                                    wedge.order_l = pd.Order(coil=coil_nr, pole=pole_nr, layer=layer_nr, winding=winding_key, block=block_key)
-                                    wedge.order_h = pd.Order(coil=coil_nr, pole=pole_nr, layer=layer_nr, winding=winding_key + 1, block=adj_blocks[0])
+                                    # if block.block_corners.iH.y < 0 and block.block_corners.iH.x>0:
+                                    #     wedge.corners = pd.Corner(iH=adj_winding.blocks[adj_blocks[0]].block_corners.iH, iL=block.block_corners.iL,
+                                    #                               oH=adj_winding.blocks[adj_blocks[0]].block_corners.oH, oL=block.block_corners.oL)
+                                    #     wedge.corners_ins = pd.Corner(iH=adj_winding.blocks[adj_blocks[0]].block_corners_ins.iL, iL=block.block_corners_ins.iH,
+                                    #                                   oH=adj_winding.blocks[adj_blocks[0]].block_corners_ins.oL, oL=block.block_corners_ins.oH)
+                                    #     wedge.order_l = pd.Order(coil=coil_nr, pole=pole_nr, layer=layer_nr, winding=winding_key, block=block_key)
+                                    #     wedge.order_h = pd.Order(coil=coil_nr, pole=pole_nr, layer=layer_nr, winding=winding_key + 1, block=adj_blocks[0])
+                                    #
+                                    # elif block.block_corners.iH.y < 0 and block.block_corners.iH.x<0:
+                                    #     wedge.corners = pd.Corner(iH=adj_winding.blocks[adj_blocks[0]].block_corners.iL, iL=block.block_corners.iH,
+                                    #                               oH=adj_winding.blocks[adj_blocks[0]].block_corners.oL, oL=block.block_corners.oH)
+                                    #     wedge.corners_ins = pd.Corner(iH=adj_winding.blocks[adj_blocks[0]].block_corners_ins.iL, iL=block.block_corners_ins.iH,
+                                    #                                   oH=adj_winding.blocks[adj_blocks[0]].block_corners_ins.oL, oL=block.block_corners_ins.oH)
+                                    #     wedge.order_l = pd.Order(coil=coil_nr, pole=pole_nr, layer=layer_nr, winding=winding_key, block=block_key)
+                                    #     wedge.order_h = pd.Order(coil=coil_nr, pole=pole_nr, layer=layer_nr, winding=winding_key + 1, block=adj_blocks[0])
+                                    # else:
+                                        wedge.corners = pd.Corner(iH=adj_winding.blocks[adj_blocks[0]].block_corners.iL, iL=block.block_corners.iH,
+                                                                  oH=adj_winding.blocks[adj_blocks[0]].block_corners.oL, oL=block.block_corners.oH)
+                                        wedge.corners_ins = pd.Corner(iH=adj_winding.blocks[adj_blocks[0]].block_corners_ins.iL, iL=block.block_corners_ins.iH,
+                                                                      oH=adj_winding.blocks[adj_blocks[0]].block_corners_ins.oL, oL=block.block_corners_ins.oH)
+                                        wedge.order_l = pd.Order(coil=coil_nr, pole=pole_nr, layer=layer_nr, winding=winding_key, block=block_key)
+                                        wedge.order_h = pd.Order(coil=coil_nr, pole=pole_nr, layer=layer_nr, winding=winding_key + 1, block=adj_blocks[0])
                                 else:
+                                    # if block.block_corners.iH.y < 0 and block.block_corners.iH.x<0:
+                                    #     wedge.corners = pd.Corner(iH=adj_winding.blocks[adj_blocks[1]].block_corners.iL, iL=block.block_corners.iH,
+                                    #                               oH=adj_winding.blocks[adj_blocks[1]].block_corners.oL, oL=block.block_corners.oH)
+                                    #     wedge.corners_ins = pd.Corner(iH=adj_winding.blocks[adj_blocks[1]].block_corners_ins.iL, iL=block.block_corners_ins.iH,
+                                    #                                   oH=adj_winding.blocks[adj_blocks[1]].block_corners_ins.oL, oL=block.block_corners_ins.oH)
+                                    # wedge.order_l = pd.Order(coil=coil_nr, pole=pole_nr, layer=layer_nr, winding=winding_key, block=block_key)
+                                    # wedge.order_h = pd.Order(coil=coil_nr, pole=pole_nr, layer=layer_nr, winding=winding_key + 1, block=adj_blocks[0])
+                                    # else:
                                     wedge.corners = pd.Corner(iH=block.block_corners.iL, iL=adj_winding.blocks[adj_blocks[blocks.index(block_key)]].block_corners.iH,
                                                               oH=block.block_corners.oL, oL=adj_winding.blocks[adj_blocks[blocks.index(block_key)]].block_corners.oH)
                                     wedge.corners_ins = pd.Corner(iH=block.block_corners_ins.iL, iL=adj_winding.blocks[adj_blocks[blocks.index(block_key)]].block_corners_ins.iH,
                                                                   oH=block.block_corners_ins.oL, oL=adj_winding.blocks[adj_blocks[blocks.index(block_key)]].block_corners_ins.oH)
                                     wedge.order_h = pd.Order(coil=coil_nr, pole=pole_nr, layer=layer_nr, winding=winding_key, block=block_key)
                                     wedge.order_l = pd.Order(coil=coil_nr, pole=pole_nr, layer=layer_nr, winding=winding_key + 1, block=adj_blocks[blocks.index(block_key)])
 
+                                color='k'
+                                arg = [(wedge.corners.iH.x, wedge.corners.iH.y),
+                                       (wedge.corners.iL.x, wedge.corners.iL.y),
+                                       (wedge.corners.oH.x, wedge.corners.oH.y),
+                                       (wedge.corners.oL.x, wedge.corners.oL.y)]
+                                line = Line2D([arg[0][0], arg[1][0]], [arg[0][1], arg[1][1]], color=color)
+                                plt.gca().add_line(line)
+                                line = Line2D([arg[3][0], arg[2][0]], [arg[3][1], arg[2][1]], color=color)
+                                plt.gca().add_line(line)
+                                line = Line2D([arg[0][0], arg[2][0]], [arg[0][1], arg[2][1]], color=color)
+                                plt.gca().add_line(line)
+                                line = Line2D([arg[3][0], arg[1][0]], [arg[3][1], arg[1][1]], color=color)
+                                plt.gca().add_line(line)
+                                # if block_key>5:
+                                #     break
+
                                 # ax.text(wedge.corners.iH.x, wedge.corners.iH.y, 'iH', style='italic', bbox={'facecolor': 'red', 'pad': 2})
                                 # ax.text(wedge.corners.oH.x, wedge.corners.oH.y, 'oH', style='italic', bbox={'facecolor': 'red', 'pad': 2})
                                 # ax.text(wedge.corners.iL.x, wedge.corners.iL.y, 'iL', style='italic', bbox={'facecolor': 'red', 'pad': 2})
                                 # ax.text(wedge.corners.oL.x, wedge.corners.oL.y, 'oL', style='italic', bbox={'facecolor': 'red', 'pad': 2})
                                 # if blocks.index(block_key) == 0:
                                 #     corners1 = block.block_corners
                                 #     corners2 = adj_winding.blocks[adj_blocks[0]].block_corners
@@ -1644,14 +1821,15 @@
                                                                      oH=wedge.corners_ins.oL, oL=wedge.corners_ins.oH)
                                 wedge.corrected_center.inner = pd.Coord(x=float(sigDig(inner[0])), y=float(sigDig(inner[1])))
                                 wedge.corrected_center.outer = pd.Coord(x=float(sigDig(outer[0])), y=float(sigDig(outer[1])))
                                 wedge.corrected_center_ins.inner = pd.Coord(x=float(sigDig(inner_ins[0])), y=float(sigDig(inner_ins[1])))
                                 wedge.corrected_center_ins.outer = pd.Coord(x=float(sigDig(outer_ins[0])), y=float(sigDig(outer_ins[1])))
                                 # ax.text(wedge.corrected_center.inner.x, wedge.corrected_center.inner.y, 'i' + str(wedge_no), style='italic', bbox={'facecolor': 'blue', 'pad': 2})
                                 # ax.text(wedge.corrected_center.outer.x, wedge.corrected_center.outer.y, 'o' + str(wedge_no), style='italic', bbox={'facecolor': 'blue', 'pad': 2})
+        #plt.show()
 
         return self.data if coil else self.data.wedges
 
     def getData(self, dir_iron: Path = None, dir_data: Path = None, dir_cadata: Path = None,
                 dump_yamls: bool = False, verbose: bool = False):
         """
             **Returns all data**
@@ -1711,7 +1889,29 @@
 
             # Save data for API
             if dump_yamls:
                 with open('data.yaml', 'w') as yaml_file:
                     yaml.dump(self.data.dict(), yaml_file, default_flow_style=False)
 
         return self.data
+
+def plot_arcs(start, end, center, ax, color='b'):
+    """
+    Plot arc using a start coordinate, end coordinate, an axis x and a color
+    """
+
+    # Define the three points
+    radius = np.sqrt((start[0] - center[0]) ** 2 + (start[1] - center[1]) ** 2)
+
+    # Calculate the start and end angles of the arc
+    start_angle = np.arctan2(start[1] - center[1], start[0] - center[0])
+    end_angle = np.arctan2(end[1] - center[1], end[0] - center[0])
+    central_angle = end_angle - start_angle
+
+    # Create the arc object
+    arc = Arc(center, 2 * radius, 2 * radius, angle=0, theta1=start_angle * 180 / np.pi,
+              theta2=end_angle * 180 / np.pi, color=color)
+
+    # If no Axes object was specified, use the current Axes
+
+    # Add the arc to the plot and show the points for reference
+    ax.add_patch(arc)
```

### Comparing `steam-sdk-2023.6.0/steam_sdk/parsers/ParserSIGMA.py` & `steam-sdk-2023.6.2/steam_sdk/parsers/ParserSIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/parsers/ParserTdms.py` & `steam-sdk-2023.6.2/steam_sdk/parsers/ParserTdms.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/parsers/ParserXYCE.py` & `steam-sdk-2023.6.2/steam_sdk/parsers/ParserXYCE.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/parsers/ParserYAML.py` & `steam-sdk-2023.6.2/steam_sdk/parsers/ParserYAML.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,11 +89,8 @@
     data_dict = list_single_row_recursively(data_dict, list_exceptions=list_exceptions)
 
     # Make sure the target folder exists
     make_folder_if_not_existing(os.path.dirname(name_output_file), verbose=False)
 
     # Write yaml file
     with open(name_output_file, 'w') as yaml_file:
-        if with_comments:
-            ruamel.yaml.round_trip_dump(data_dict, yaml_file)
-        else:
-            ruamel_yaml.dump(data_dict, yaml_file)
+        ruamel_yaml.dump(data_dict, yaml_file)
```

### Comparing `steam-sdk-2023.6.0/steam_sdk/parsims/ParsimConductor.py` & `steam-sdk-2023.6.2/steam_sdk/parsims/ParsimConductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/parsims/ParsimDakota.py` & `steam-sdk-2023.6.2/steam_sdk/parsims/ParsimDakota.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/parsims/ParsimEventCircuit.py` & `steam-sdk-2023.6.2/steam_sdk/parsims/ParsimEventCircuit.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/parsims/ParsimEventMagnet.py` & `steam-sdk-2023.6.2/steam_sdk/parsims/ParsimEventMagnet.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/parsims/ParsimSweep.py` & `steam-sdk-2023.6.2/steam_sdk/parsims/ParsimSweep.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/plotters/PlotterAnalysis.py` & `steam-sdk-2023.6.2/steam_sdk/plotters/PlotterAnalysis.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/plotters/PlotterMap2d.py` & `steam-sdk-2023.6.2/steam_sdk/plotters/PlotterMap2d.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/plotters/PlotterModel.py` & `steam-sdk-2023.6.2/steam_sdk/plotters/PlotterModel.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/plotters/PlotterParametric.py` & `steam-sdk-2023.6.2/steam_sdk/plotters/PlotterParametric.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/plotters/PlotterRoxie.py` & `steam-sdk-2023.6.2/steam_sdk/plotters/PlotterRoxie.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/postprocs/PostprocsMetrics.py` & `steam-sdk-2023.6.2/steam_sdk/postprocs/PostprocsMetrics.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/utils/MTF_reading_functions.py` & `steam-sdk-2023.6.2/steam_sdk/utils/MTF_reading_functions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/utils/ModifyModelData.py` & `steam-sdk-2023.6.2/steam_sdk/utils/ModifyModelData.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/utils/ModifyModelDataMagnet.py` & `steam-sdk-2023.6.2/steam_sdk/utils/ModifyModelDataMagnet.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import os
 from pathlib import Path
 import yaml
-import ruamel.yaml
 from steam_sdk.data.DataModelMagnet import DataModelMagnet
 from steam_sdk.parsers.ParserYAML import dict_to_yaml
 
 if __name__ == "__main__":
     path_models = Path.joinpath(Path(__file__).parent.parent.parent, 'C:\\Users\emm\cernbox\SWAN_projects\steam_models\magnets')
-    # path_models = Path.joinpath(Path(__file__).parent.parent.parent, r'E:\Python\steam_models\magnets')
-    # path_models = Path.joinpath(Path(__file__).parent.parent.parent, 'tests/builders/model_library/magnets')
+    path_models = Path.joinpath(Path(__file__).parent.parent.parent, r'C:\Users\jlidholm\cernbox\Git-projects\steam_models\magnets')
+    #path_models = Path.joinpath(Path(__file__).parent.parent.parent, 'tests/builders/model_library/magnets')
     models = [x.parts[-1] for x in Path(path_models).iterdir() if x.is_dir()]
-    #models = ['MCBRD']
+    #models = ['MQXA']
 
     for mm in models:
         # Read file
         file_model_data = Path.joinpath(path_models, mm, 'input', 'modelData_' + mm + '.yaml')
         if os.path.isfile(file_model_data):
             # Load yaml keys into DataAnalysis dataclass
             with open(file_model_data, "r") as stream:
@@ -24,15 +23,14 @@
 
             # Note: Obsolete keys in yaml file will automatically be deleted
 
             # Note: New keys added to DataModelMagnet will automatically be added to the yaml file (UNLESS A VALUE IS ASSIGNED BELOW, THEIR VALUES WILL BE INITIALIZED TO DEFAULT)
 
             # Example to assign value to new keys in model data
             # model_data.Options_LEDET.magnet_inductance.flag_calculate_inductance = True
-            model_data.Options_LEDET.post_processing.flag_importFieldWhenCalculatingHotSpotT = 0
 
             # Example to change positions of key keeping its value (IF THIS IS NOT DONE THE INFOMRATION IN THE ORIGINAL YAML FILE WILL BE LOST!)
             # Note: The following will raise an exception if the keys do not exist in the original yaml file
             # model_data.Options_LEDET.magnet_inductance.LUT_DifferentialInductance_current = dictionary_yaml['GeneralParameters']['magnet_inductance']['fL_I']
             # model_data.Options_LEDET.magnet_inductance.LUT_DifferentialInductance_inductance = dictionary_yaml['GeneralParameters']['magnet_inductance']['fL_L']
             #
             # model_data.Options_LEDET.heat_exchange.heat_exchange_max_distance = dictionary_yaml['CoilWindings']['heat_exchange']['heat_exchange_max_distance']
@@ -42,14 +40,15 @@
             # model_data.Options_LEDET.heat_exchange.iContactAlongHeight_pairs_to_remove = dictionary_yaml['CoilWindings']['heat_exchange']['iContactAlongHeight_pairs_to_remove']
             # model_data.Options_LEDET.heat_exchange.th_insulationBetweenLayers = dictionary_yaml['CoilWindings']['heat_exchange']['th_insulationBetweenLayers']
             #
             # model_data.Options_LEDET.conductor_geometry_used_for_ISCL.alphaDEG_ht = dictionary_yaml['CoilWindings']['multipole']['alphaDEG_ht']
             # model_data.Options_LEDET.conductor_geometry_used_for_ISCL.rotation_ht = dictionary_yaml['CoilWindings']['multipole']['rotation_ht']
             # model_data.Options_LEDET.conductor_geometry_used_for_ISCL.mirror_ht = dictionary_yaml['CoilWindings']['multipole']['mirror_ht']
             # model_data.Options_LEDET.conductor_geometry_used_for_ISCL.mirrorY_ht = dictionary_yaml['CoilWindings']['multipole']['mirrorY_ht']
+            model_data.Quench_Protection.Quench_Heaters.turns_sides = ["O"] * len(model_data.Quench_Protection.Quench_Heaters.iQH_toHalfTurn_From)
 
             # Check and reformat the key values
             model_data = DataModelMagnet(**model_data.dict())
 
             # Write file
             # file_model_data_output = Path.joinpath(path_models, mm, 'input', 'modelData_' + mm + '_MODIFIED.yaml')  # use this line if you wish to test the results of this script
             file_model_data_output = file_model_data  # use this line if you wish to really update all yaml input files
```

### Comparing `steam-sdk-2023.6.0/steam_sdk/utils/ModifyModelDataconductor.py` & `steam-sdk-2023.6.2/steam_sdk/utils/ModifyModelDataconductor.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import yaml
 
 from steam_sdk.data.DataModelConductor import DataModelConductor
 from steam_sdk.parsers.ParserYAML import dict_to_yaml
 
 if __name__ == "__main__":
     path_models = Path.joinpath(Path(__file__).parent.parent.parent, 'C:\\Users\emm\cernbox\SWAN_projects\steam_models\conductors')
-    # path_models = Path.joinpath(Path(__file__).parent.parent.parent, 'tests/builders/model_library/conductors')
+    path_models = Path.joinpath(Path(__file__).parent.parent.parent, 'tests/builders/model_library/conductors')
     models = [x.parts[-1] for x in Path(path_models).iterdir() if x.is_dir()]
 
     for mm in models:
         # Read file
         file_model_data = Path.joinpath(path_models, mm, 'input', 'modelData_' + mm + '.yaml')
         if os.path.isfile(file_model_data):
             # Load yaml keys into DataAnalysis dataclass
```

### Comparing `steam-sdk-2023.6.0/steam_sdk/utils/clean_NaN_from_signal.py` & `steam-sdk-2023.6.2/steam_sdk/utils/clean_NaN_from_signal.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/utils/compare_two_parameters.py` & `steam-sdk-2023.6.2/steam_sdk/utils/compare_two_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/utils/create_coordinate_file_SIGMA.py` & `steam-sdk-2023.6.2/steam_sdk/utils/create_coordinate_file_SIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/utils/get_attribute_type.py` & `steam-sdk-2023.6.2/steam_sdk/utils/get_attribute_type.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/utils/misc.py` & `steam-sdk-2023.6.2/steam_sdk/utils/misc.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/utils/parse_str_to_list.py` & `steam-sdk-2023.6.2/steam_sdk/utils/parse_str_to_list.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/utils/tic_toc.py` & `steam-sdk-2023.6.2/steam_sdk/utils/tic_toc.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/utils/utils_PC.py` & `steam-sdk-2023.6.2/steam_sdk/utils/utils_PC.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/viewers/Viewer.py` & `steam-sdk-2023.6.2/steam_sdk/viewers/Viewer.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/viewers/ViewerMeas.py` & `steam-sdk-2023.6.2/steam_sdk/viewers/ViewerMeas.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/viewers/ViewerSim.py` & `steam-sdk-2023.6.2/steam_sdk/viewers/ViewerSim.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk/wrappers/wrapper_yaml.py` & `steam-sdk-2023.6.2/steam_sdk/wrappers/wrapper_yaml.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.0/steam_sdk.egg-info/PKG-INFO` & `steam-sdk-2023.6.2/steam_sdk.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: steam-sdk
-Version: 2023.6.0
+Version: 2023.6.2
 Summary: Source code for APIs for STEAM tools.
 Home-page: https://gitlab.cern.ch/steam/steam_sdk
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: CERN,STEAM,SDK,API
+Keywords: CERN,SDK,STEAM,API
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM_SDK
```

### Comparing `steam-sdk-2023.6.0/steam_sdk.egg-info/SOURCES.txt` & `steam-sdk-2023.6.2/steam_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -100,14 +100,15 @@
 steam_sdk/parsers/ParserProteCCT.py
 steam_sdk/parsers/ParserProtePyBBQ.py
 steam_sdk/parsers/ParserRoxie.py
 steam_sdk/parsers/ParserSIGMA.py
 steam_sdk/parsers/ParserTdms.py
 steam_sdk/parsers/ParserXYCE.py
 steam_sdk/parsers/ParserYAML.py
+steam_sdk/parsers/ParserYamlToRoxie.py
 steam_sdk/parsers/__init__.py
 steam_sdk/parsers/dict_to_in.py
 steam_sdk/parsims/ParsimConductor.py
 steam_sdk/parsims/ParsimDakota.py
 steam_sdk/parsims/ParsimEventCircuit.py
 steam_sdk/parsims/ParsimEventMagnet.py
 steam_sdk/parsims/ParsimSweep.py
@@ -121,14 +122,15 @@
 steam_sdk/postprocs/PostprocsMetrics.py
 steam_sdk/postprocs/__init__.py
 steam_sdk/utils/MTF_reading_functions.py
 steam_sdk/utils/ModifyModelData.py
 steam_sdk/utils/ModifyModelDataMagnet.py
 steam_sdk/utils/ModifyModelDataconductor.py
 steam_sdk/utils/NumpyEncoder.py
+steam_sdk/utils/ParserRoxieHelpers.py
 steam_sdk/utils/__init__.py
 steam_sdk/utils/clean_NaN_from_signal.py
 steam_sdk/utils/compare_two_parameters.py
 steam_sdk/utils/create_coordinate_file_SIGMA.py
 steam_sdk/utils/get_attribute_type.py
 steam_sdk/utils/isNaN.py
 steam_sdk/utils/make_folder_if_not_existing.py
```

### Comparing `steam-sdk-2023.6.0/steam_sdk.egg-info/requires.txt` & `steam-sdk-2023.6.2/steam_sdk.egg-info/requires.txt`

 * *Files 0% similar despite different names*

```diff
@@ -82,8 +82,8 @@
 tqdm==4.64.1
 traitlets==5.4.0
 typing_extensions==4.3.0
 urllib3==1.26.12
 watchdog==2.1.9
 wcwidth==0.2.5
 zipp==3.8.1
-steam-pysigma==2023.5.11
+steam-pysigma==2023.6.1
```

