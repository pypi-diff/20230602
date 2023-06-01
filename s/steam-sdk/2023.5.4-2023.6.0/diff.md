# Comparing `tmp/steam-sdk-2023.5.4.tar.gz` & `tmp/steam-sdk-2023.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\steam-sdk-2023.5.4.tar", last modified: Wed May 17 08:03:47 2023, max compression
+gzip compressed data, was "dist\steam-sdk-2023.6.0.tar", last modified: Thu Jun  1 21:57:18 2023, max compression
```

## Comparing `steam-sdk-2023.5.4.tar` & `steam-sdk-2023.6.0.tar`

### file list

```diff
@@ -1,183 +1,183 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 08:03:47.145883 steam-sdk-2023.5.4/
--rw-rw-rw-   0        0        0      122 2023-03-15 09:29:53.000000 steam-sdk-2023.5.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1550 2023-05-17 08:03:47.142627 steam-sdk-2023.5.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-17 08:03:47.146213 steam-sdk-2023.5.4/setup.cfg
--rw-rw-rw-   0        0        0      797 2023-05-17 08:01:49.000000 steam-sdk-2023.5.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-17 08:03:46.842264 steam-sdk-2023.5.4/steam_sdk/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 08:03:46.852402 steam-sdk-2023.5.4/steam_sdk/analyses/
--rw-rw-rw-   0        0        0   125641 2023-05-17 07:57:55.000000 steam-sdk-2023.5.4/steam_sdk/analyses/AnalysisSTEAM.py
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/analyses/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 08:03:46.855581 steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 08:03:46.858581 steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/__init__.py
--rw-rw-rw-   0        0        0    23368 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py
-drwxrwxrwx   0        0        0        0 2023-05-17 08:03:46.872701 steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/__init__.py
--rw-rw-rw-   0        0        0    16757 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py
--rw-rw-rw-   0        0        0     2800 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py
--rw-rw-rw-   0        0        0     6828 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py
--rw-rw-rw-   0        0        0    95412 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py
--rw-rw-rw-   0        0        0     2652 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py
--rw-rw-rw-   0        0        0     2341 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py
-drwxrwxrwx   0        0        0        0 2023-05-17 08:03:46.875906 steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/__init__.py
--rw-rw-rw-   0        0        0    22374 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py
-drwxrwxrwx   0        0        0        0 2023-05-17 08:03:46.881906 steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/__init__.py
--rw-rw-rw-   0        0        0     5210 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py
--rw-rw-rw-   0        0        0     4527 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py
--rw-rw-rw-   0        0        0     2921 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py
-drwxrwxrwx   0        0        0        0 2023-05-17 08:03:46.884907 steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/__init__.py
--rw-rw-rw-   0        0        0    29433 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py
-drwxrwxrwx   0        0        0        0 2023-05-17 08:03:46.893069 steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/__init__.py
--rw-rw-rw-   0        0        0     5210 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py
--rw-rw-rw-   0        0        0     4704 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py
--rw-rw-rw-   0        0        0     4852 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py
-drwxrwxrwx   0        0        0        0 2023-05-17 08:03:46.896068 steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/custom_function_test_1/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/custom_function_test_1/__init__.py
--rw-rw-rw-   0        0        0     1307 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py
-drwxrwxrwx   0        0        0        0 2023-05-17 08:03:46.917697 steam-sdk-2023.5.4/steam_sdk/builders/
--rw-rw-rw-   0        0        0    12924 2023-05-12 15:08:26.000000 steam-sdk-2023.5.4/steam_sdk/builders/BuilderFiQuS.py
--rw-rw-rw-   0        0        0   162619 2023-05-12 15:08:26.000000 steam-sdk-2023.5.4/steam_sdk/builders/BuilderLEDET.py
--rw-rw-rw-   0        0        0    34658 2023-05-17 07:59:42.000000 steam-sdk-2023.5.4/steam_sdk/builders/BuilderModel.py
--rw-rw-rw-   0        0        0    12686 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/builders/BuilderProteCCT.py
--rw-rw-rw-   0        0        0     6749 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/builders/BuilderPyBBQ.py
--rw-rw-rw-   0        0        0    12076 2023-05-10 14:13:23.000000 steam-sdk-2023.5.4/steam_sdk/builders/BuilderSIGMA.py
--rw-rw-rw-   0        0        0    11689 2023-01-18 15:24:33.000000 steam-sdk-2023.5.4/steam_sdk/builders/SelfMutualInductanceCalculation.py
--rw-rw-rw-   0        0        0     7941 2022-12-19 08:13:58.000000 steam-sdk-2023.5.4/steam_sdk/builders/Solenoids.py
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/builders/__init__.py
--rw-rw-rw-   0        0        0     8352 2023-03-15 09:29:53.000000 steam-sdk-2023.5.4/steam_sdk/builders/geometricFunctions.py
-drwxrwxrwx   0        0        0        0 2023-05-17 08:03:46.919698 steam-sdk-2023.5.4/steam_sdk/configs/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/configs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 08:03:46.921699 steam-sdk-2023.5.4/steam_sdk/configs/plotters/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/configs/plotters/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 08:03:46.924698 steam-sdk-2023.5.4/steam_sdk/configs/tools_defaults/
-drwxrwxrwx   0        0        0        0 2023-05-17 08:03:46.926807 steam-sdk-2023.5.4/steam_sdk/configs/tools_defaults/LEDET/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/configs/tools_defaults/LEDET/__init__.py
--rw-rw-rw-   0        0        0    32890 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx
--rw-rw-rw-   0        0        0     1426 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/configs/tools_defaults/ToolDefaultReader.py
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/configs/tools_defaults/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 08:03:46.928807 steam-sdk-2023.5.4/steam_sdk/cosims/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/cosims/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 08:03:46.978626 steam-sdk-2023.5.4/steam_sdk/data/
--rw-rw-rw-   0        0        0    10200 2023-05-12 13:31:31.000000 steam-sdk-2023.5.4/steam_sdk/data/DataAnalysis.py
--rw-rw-rw-   0        0        0     8040 2023-05-05 12:54:05.000000 steam-sdk-2023.5.4/steam_sdk/data/DataConductor.py
--rw-rw-rw-   0        0        0     3281 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/data/DataDakota.py
--rw-rw-rw-   0        0        0     2865 2023-04-24 12:48:33.000000 steam-sdk-2023.5.4/steam_sdk/data/DataEventCircuit.py
--rw-rw-rw-   0        0        0     4193 2023-05-09 14:50:49.000000 steam-sdk-2023.5.4/steam_sdk/data/DataEventMagnet.py
--rw-rw-rw-   0        0        0    12762 2023-05-12 15:08:26.000000 steam-sdk-2023.5.4/steam_sdk/data/DataFiQuS.py
--rw-rw-rw-   0        0        0    10767 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/data/DataLEDET.py
--rw-rw-rw-   0        0        0     4314 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/data/DataModelCircuit.py
--rw-rw-rw-   0        0        0     5869 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/data/DataModelConductor.py
--rw-rw-rw-   0        0        0    35579 2023-05-12 15:08:26.000000 steam-sdk-2023.5.4/steam_sdk/data/DataModelMagnet.py
--rw-rw-rw-   0        0        0     2636 2023-05-09 14:50:49.000000 steam-sdk-2023.5.4/steam_sdk/data/DataParsimConductor.py
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/data/DataParsims.py
--rw-rw-rw-   0        0        0     1995 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/data/DataProteCCT.py
--rw-rw-rw-   0        0        0     2105 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/data/DataPyBBQ.py
--rw-rw-rw-   0        0        0     7899 2023-03-21 08:33:21.000000 steam-sdk-2023.5.4/steam_sdk/data/DataRoxieParser.py
--rw-rw-rw-   0        0        0     6791 2023-05-09 14:51:04.000000 steam-sdk-2023.5.4/steam_sdk/data/DataSIGMA.py
--rw-rw-rw-   0        0        0     1650 2023-03-15 09:29:53.000000 steam-sdk-2023.5.4/steam_sdk/data/DataSettings.py
--rw-rw-rw-   0        0        0     3204 2023-01-11 12:50:11.000000 steam-sdk-2023.5.4/steam_sdk/data/DataSignal.py
--rw-rw-rw-   0        0        0    22928 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/data/DictionaryLEDET.py
--rw-rw-rw-   0        0        0     4482 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/data/DictionaryProteCCT.py
--rw-rw-rw-   0        0        0     2902 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/data/DictionaryPyBBQ.py
--rw-rw-rw-   0        0        0    27540 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/data/TemplateLEDET.py
--rw-rw-rw-   0        0        0     7903 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/data/TemplateProteCCT.py
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 08:03:47.000982 steam-sdk-2023.5.4/steam_sdk/drivers/
--rw-rw-rw-   0        0        0     3151 2022-12-19 08:13:58.000000 steam-sdk-2023.5.4/steam_sdk/drivers/DriverAnalysis.py
--rw-rw-rw-   0        0        0     2711 2022-12-19 08:13:58.000000 steam-sdk-2023.5.4/steam_sdk/drivers/DriverDakota.py
--rw-rw-rw-   0        0        0     1299 2023-03-15 09:29:53.000000 steam-sdk-2023.5.4/steam_sdk/drivers/DriverFiQuS.py
--rw-rw-rw-   0        0        0     3482 2022-12-19 08:13:58.000000 steam-sdk-2023.5.4/steam_sdk/drivers/DriverLEDET.py
--rw-rw-rw-   0        0        0     1924 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/drivers/DriverPSPICE.py
--rw-rw-rw-   0        0        0     2062 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/drivers/DriverProteCCT.py
--rw-rw-rw-   0        0        0     2219 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/drivers/DriverPyBBQ.py
--rw-rw-rw-   0        0        0     3905 2023-05-17 07:23:11.000000 steam-sdk-2023.5.4/steam_sdk/drivers/DriverSIGMA.py
--rw-rw-rw-   0        0        0     1932 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/drivers/DriverXYCE.py
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/drivers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 08:03:47.062242 steam-sdk-2023.5.4/steam_sdk/parsers/
--rw-rw-rw-   0        0        0     4984 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/parsers/CSD_Reader.py
--rw-rw-rw-   0        0        0      317 2023-03-29 12:41:10.000000 steam-sdk-2023.5.4/steam_sdk/parsers/ParserCOMSOLToTxt.py
--rw-rw-rw-   0        0        0     2290 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/parsers/ParserCond2d.py
--rw-rw-rw-   0        0        0     1077 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/parsers/ParserCsd.py
--rw-rw-rw-   0        0        0     6220 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/parsers/ParserCsv.py
--rw-rw-rw-   0        0        0     1650 2023-01-13 08:06:15.000000 steam-sdk-2023.5.4/steam_sdk/parsers/ParserDakota.py
--rw-rw-rw-   0        0        0     1030 2023-03-15 09:29:53.000000 steam-sdk-2023.5.4/steam_sdk/parsers/ParserDatToCsv.py
--rw-rw-rw-   0        0        0     8536 2023-03-15 09:29:53.000000 steam-sdk-2023.5.4/steam_sdk/parsers/ParserExcel.py
--rw-rw-rw-   0        0        0     2287 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/parsers/ParserFiQuS.py
--rw-rw-rw-   0        0        0    48056 2023-03-15 09:29:53.000000 steam-sdk-2023.5.4/steam_sdk/parsers/ParserLEDET.py
--rw-rw-rw-   0        0        0    12436 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/parsers/ParserMap2d.py
--rw-rw-rw-   0        0        0    10920 2023-05-12 13:31:31.000000 steam-sdk-2023.5.4/steam_sdk/parsers/ParserMat.py
--rw-rw-rw-   0        0        0    61567 2023-04-13 09:38:44.000000 steam-sdk-2023.5.4/steam_sdk/parsers/ParserPSPICE.py
--rw-rw-rw-   0        0        0     4780 2023-03-15 09:29:53.000000 steam-sdk-2023.5.4/steam_sdk/parsers/ParserPdf.py
--rw-rw-rw-   0        0        0     6838 2023-03-15 09:29:53.000000 steam-sdk-2023.5.4/steam_sdk/parsers/ParserProteCCT.py
--rw-rw-rw-   0        0        0     2942 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/parsers/ParserProtePyBBQ.py
--rw-rw-rw-   0        0        0    92213 2023-03-27 14:04:47.000000 steam-sdk-2023.5.4/steam_sdk/parsers/ParserRoxie.py
--rw-rw-rw-   0        0        0     1928 2023-05-09 14:51:03.000000 steam-sdk-2023.5.4/steam_sdk/parsers/ParserSIGMA.py
--rw-rw-rw-   0        0        0    11707 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/parsers/ParserTdms.py
--rw-rw-rw-   0        0        0    55281 2023-03-15 09:29:53.000000 steam-sdk-2023.5.4/steam_sdk/parsers/ParserXYCE.py
--rw-rw-rw-   0        0        0     4088 2023-03-15 09:29:53.000000 steam-sdk-2023.5.4/steam_sdk/parsers/ParserYAML.py
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/parsers/__init__.py
--rw-rw-rw-   0        0        0        2 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/parsers/dict_to_in.py
-drwxrwxrwx   0        0        0        0 2023-05-17 08:03:47.073421 steam-sdk-2023.5.4/steam_sdk/parsims/
--rw-rw-rw-   0        0        0    61764 2023-05-12 13:31:31.000000 steam-sdk-2023.5.4/steam_sdk/parsims/ParsimConductor.py
--rw-rw-rw-   0        0        0      916 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/parsims/ParsimDakota.py
--rw-rw-rw-   0        0        0    72533 2023-05-17 07:23:09.000000 steam-sdk-2023.5.4/steam_sdk/parsims/ParsimEventCircuit.py
--rw-rw-rw-   0        0        0    47819 2023-05-12 13:31:31.000000 steam-sdk-2023.5.4/steam_sdk/parsims/ParsimEventMagnet.py
--rw-rw-rw-   0        0        0     1972 2023-01-25 14:04:47.000000 steam-sdk-2023.5.4/steam_sdk/parsims/ParsimSweep.py
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/parsims/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 08:03:47.082588 steam-sdk-2023.5.4/steam_sdk/plotters/
--rw-rw-rw-   0        0        0     8053 2023-05-12 13:31:31.000000 steam-sdk-2023.5.4/steam_sdk/plotters/PlotterAnalysis.py
--rw-rw-rw-   0        0        0    20399 2023-05-09 14:51:04.000000 steam-sdk-2023.5.4/steam_sdk/plotters/PlotterMap2d.py
--rw-rw-rw-   0        0        0    39596 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/plotters/PlotterModel.py
--rw-rw-rw-   0        0        0    22987 2022-12-19 08:13:58.000000 steam-sdk-2023.5.4/steam_sdk/plotters/PlotterParametric.py
--rw-rw-rw-   0        0        0     8871 2023-04-24 12:43:05.000000 steam-sdk-2023.5.4/steam_sdk/plotters/PlotterRoxie.py
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/plotters/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 08:03:47.085807 steam-sdk-2023.5.4/steam_sdk/postprocs/
--rw-rw-rw-   0        0        0     5564 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/postprocs/PostprocsMetrics.py
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/postprocs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 08:03:47.125265 steam-sdk-2023.5.4/steam_sdk/utils/
--rw-rw-rw-   0        0        0     2679 2023-03-15 09:29:53.000000 steam-sdk-2023.5.4/steam_sdk/utils/MTF_reading_functions.py
--rw-rw-rw-   0        0        0    14942 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/utils/ModifyModelData.py
--rw-rw-rw-   0        0        0     4762 2023-05-17 07:23:11.000000 steam-sdk-2023.5.4/steam_sdk/utils/ModifyModelDataMagnet.py
--rw-rw-rw-   0        0        0     2745 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/utils/ModifyModelDataconductor.py
--rw-rw-rw-   0        0        0      313 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/utils/NumpyEncoder.py
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/utils/__init__.py
--rw-rw-rw-   0        0        0      686 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/utils/clean_NaN_from_signal.py
--rw-rw-rw-   0        0        0     3837 2023-03-15 09:29:53.000000 steam-sdk-2023.5.4/steam_sdk/utils/compare_two_parameters.py
--rw-rw-rw-   0        0        0      590 2023-05-09 14:50:57.000000 steam-sdk-2023.5.4/steam_sdk/utils/create_coordinate_file_SIGMA.py
--rw-rw-rw-   0        0        0     1279 2023-04-24 12:48:33.000000 steam-sdk-2023.5.4/steam_sdk/utils/get_attribute_type.py
--rw-rw-rw-   0        0        0      167 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/utils/isNaN.py
--rw-rw-rw-   0        0        0      299 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/utils/make_folder_if_not_existing.py
--rw-rw-rw-   0        0        0     4512 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/utils/misc.py
--rw-rw-rw-   0        0        0     1592 2023-04-24 12:48:33.000000 steam-sdk-2023.5.4/steam_sdk/utils/parse_str_to_list.py
--rw-rw-rw-   0        0        0      388 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/utils/rgetattr.py
--rw-rw-rw-   0        0        0      460 2023-01-11 12:50:11.000000 steam-sdk-2023.5.4/steam_sdk/utils/rhasattr.py
--rw-rw-rw-   0        0        0      383 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/utils/sgetattr.py
--rw-rw-rw-   0        0        0      863 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/utils/tic_toc.py
--rw-rw-rw-   0        0        0      168 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/utils/unique.py
--rw-rw-rw-   0        0        0     7005 2023-05-11 09:21:50.000000 steam-sdk-2023.5.4/steam_sdk/utils/utils_PC.py
-drwxrwxrwx   0        0        0        0 2023-05-17 08:03:47.132407 steam-sdk-2023.5.4/steam_sdk/viewers/
--rw-rw-rw-   0        0        0    35919 2023-03-23 12:53:02.000000 steam-sdk-2023.5.4/steam_sdk/viewers/Viewer.py
--rw-rw-rw-   0        0        0     6127 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/viewers/ViewerMeas.py
--rw-rw-rw-   0        0        0     1667 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/viewers/ViewerSim.py
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/viewers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 08:03:47.134406 steam-sdk-2023.5.4/steam_sdk/wrappers/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.4/steam_sdk/wrappers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 08:03:47.135406 steam-sdk-2023.5.4/steam_sdk/wrappers/java/
-drwxrwxrwx   0        0        0        0 2023-05-17 08:03:47.139627 steam-sdk-2023.5.4/steam_sdk/wrappers/java/SING/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:43.000000 steam-sdk-2023.5.4/steam_sdk/wrappers/java/SING/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 08:03:47.140626 steam-sdk-2023.5.4/steam_sdk/wrappers/java/SING/jars/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:43.000000 steam-sdk-2023.5.4/steam_sdk/wrappers/java/SING/jars/__init__.py
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:43.000000 steam-sdk-2023.5.4/steam_sdk/wrappers/java/__init__.py
--rw-rw-rw-   0        0        0     1834 2022-11-02 10:29:43.000000 steam-sdk-2023.5.4/steam_sdk/wrappers/wrapper_yaml.py
-drwxrwxrwx   0        0        0        0 2023-05-17 08:03:46.849403 steam-sdk-2023.5.4/steam_sdk.egg-info/
--rw-rw-rw-   0        0        0     1550 2023-05-17 08:03:44.000000 steam-sdk-2023.5.4/steam_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6686 2023-05-17 08:03:44.000000 steam-sdk-2023.5.4/steam_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 08:03:44.000000 steam-sdk-2023.5.4/steam_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1597 2023-05-17 08:03:44.000000 steam-sdk-2023.5.4/steam_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-17 08:03:44.000000 steam-sdk-2023.5.4/steam_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 21:57:18.469019 steam-sdk-2023.6.0/
+-rw-rw-rw-   0        0        0      122 2023-02-02 15:29:21.000000 steam-sdk-2023.6.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1550 2023-06-01 21:57:18.468019 steam-sdk-2023.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-01 21:57:18.469019 steam-sdk-2023.6.0/setup.cfg
+-rw-rw-rw-   0        0        0      797 2023-06-01 21:56:21.000000 steam-sdk-2023.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 21:57:17.290632 steam-sdk-2023.6.0/steam_sdk/
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 21:57:17.344487 steam-sdk-2023.6.0/steam_sdk/analyses/
+-rw-rw-rw-   0        0        0   125649 2023-05-22 14:09:18.000000 steam-sdk-2023.6.0/steam_sdk/analyses/AnalysisSTEAM.py
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/analyses/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 21:57:17.346482 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 21:57:17.365432 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/__init__.py
+-rw-rw-rw-   0        0        0    23368 2022-10-12 14:45:26.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py
+drwxrwxrwx   0        0        0        0 2023-06-01 21:57:17.440070 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/__init__.py
+-rw-rw-rw-   0        0        0    16757 2022-10-06 23:30:28.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py
+-rw-rw-rw-   0        0        0     2800 2022-09-12 16:26:14.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py
+-rw-rw-rw-   0        0        0     6828 2022-09-10 00:21:21.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py
+-rw-rw-rw-   0        0        0    95412 2022-10-24 19:22:58.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py
+-rw-rw-rw-   0        0        0     2652 2022-09-09 21:29:03.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py
+-rw-rw-rw-   0        0        0     2341 2022-09-09 21:29:03.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py
+drwxrwxrwx   0        0        0        0 2023-06-01 21:57:17.455304 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/__init__.py
+-rw-rw-rw-   0        0        0    22374 2022-09-28 09:57:32.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py
+drwxrwxrwx   0        0        0        0 2023-06-01 21:57:17.484725 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/
+-rw-rw-rw-   0        0        0        0 2022-09-26 06:59:06.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/__init__.py
+-rw-rw-rw-   0        0        0     5210 2022-09-28 09:57:32.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py
+-rw-rw-rw-   0        0        0     4527 2022-09-28 09:57:32.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py
+-rw-rw-rw-   0        0        0     2921 2022-09-28 09:57:32.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py
+drwxrwxrwx   0        0        0        0 2023-06-01 21:57:17.499855 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/
+-rw-rw-rw-   0        0        0        0 2022-09-26 06:59:06.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/__init__.py
+-rw-rw-rw-   0        0        0    29433 2022-09-30 09:15:14.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py
+drwxrwxrwx   0        0        0        0 2023-06-01 21:57:17.522272 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/
+-rw-rw-rw-   0        0        0        0 2022-09-26 06:59:06.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/__init__.py
+-rw-rw-rw-   0        0        0     5210 2022-09-28 09:57:32.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py
+-rw-rw-rw-   0        0        0     4704 2022-09-28 09:57:32.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py
+-rw-rw-rw-   0        0        0     4852 2022-09-28 09:57:32.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py
+drwxrwxrwx   0        0        0        0 2023-06-01 21:57:17.534681 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/custom_function_test_1/
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/custom_function_test_1/__init__.py
+-rw-rw-rw-   0        0        0     1307 2022-09-10 00:27:54.000000 steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py
+drwxrwxrwx   0        0        0        0 2023-06-01 21:57:17.627402 steam-sdk-2023.6.0/steam_sdk/builders/
+-rw-rw-rw-   0        0        0    12924 2023-05-19 10:14:24.000000 steam-sdk-2023.6.0/steam_sdk/builders/BuilderFiQuS.py
+-rw-rw-rw-   0        0        0   162736 2023-05-25 09:34:00.000000 steam-sdk-2023.6.0/steam_sdk/builders/BuilderLEDET.py
+-rw-rw-rw-   0        0        0    35758 2023-05-22 14:09:16.000000 steam-sdk-2023.6.0/steam_sdk/builders/BuilderModel.py
+-rw-rw-rw-   0        0        0    12686 2022-09-07 00:41:51.000000 steam-sdk-2023.6.0/steam_sdk/builders/BuilderProteCCT.py
+-rw-rw-rw-   0        0        0     6749 2022-08-22 11:29:04.000000 steam-sdk-2023.6.0/steam_sdk/builders/BuilderPyBBQ.py
+-rw-rw-rw-   0        0        0    12076 2023-05-10 14:10:46.000000 steam-sdk-2023.6.0/steam_sdk/builders/BuilderSIGMA.py
+-rw-rw-rw-   0        0        0    11689 2023-01-18 09:46:00.000000 steam-sdk-2023.6.0/steam_sdk/builders/SelfMutualInductanceCalculation.py
+-rw-rw-rw-   0        0        0     7941 2022-12-06 11:41:34.000000 steam-sdk-2023.6.0/steam_sdk/builders/Solenoids.py
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/builders/__init__.py
+-rw-rw-rw-   0        0        0     8352 2023-02-02 15:39:34.000000 steam-sdk-2023.6.0/steam_sdk/builders/geometricFunctions.py
+drwxrwxrwx   0        0        0        0 2023-06-01 21:57:17.628402 steam-sdk-2023.6.0/steam_sdk/configs/
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/configs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 21:57:17.629399 steam-sdk-2023.6.0/steam_sdk/configs/plotters/
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/configs/plotters/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 21:57:17.640478 steam-sdk-2023.6.0/steam_sdk/configs/tools_defaults/
+drwxrwxrwx   0        0        0        0 2023-06-01 21:57:17.650471 steam-sdk-2023.6.0/steam_sdk/configs/tools_defaults/LEDET/
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/configs/tools_defaults/LEDET/__init__.py
+-rw-rw-rw-   0        0        0    32991 2023-05-25 09:35:34.000000 steam-sdk-2023.6.0/steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx
+-rw-rw-rw-   0        0        0     1426 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/configs/tools_defaults/ToolDefaultReader.py
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/configs/tools_defaults/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 21:57:17.652444 steam-sdk-2023.6.0/steam_sdk/cosims/
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/cosims/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 21:57:17.846793 steam-sdk-2023.6.0/steam_sdk/data/
+-rw-rw-rw-   0        0        0    10200 2023-05-12 14:38:34.000000 steam-sdk-2023.6.0/steam_sdk/data/DataAnalysis.py
+-rw-rw-rw-   0        0        0     7983 2023-05-19 12:19:03.000000 steam-sdk-2023.6.0/steam_sdk/data/DataConductor.py
+-rw-rw-rw-   0        0        0     3281 2022-09-30 09:15:14.000000 steam-sdk-2023.6.0/steam_sdk/data/DataDakota.py
+-rw-rw-rw-   0        0        0     2865 2023-05-04 08:10:45.000000 steam-sdk-2023.6.0/steam_sdk/data/DataEventCircuit.py
+-rw-rw-rw-   0        0        0     4193 2023-05-09 19:16:09.000000 steam-sdk-2023.6.0/steam_sdk/data/DataEventMagnet.py
+-rw-rw-rw-   0        0        0    12762 2023-05-19 10:14:24.000000 steam-sdk-2023.6.0/steam_sdk/data/DataFiQuS.py
+-rw-rw-rw-   0        0        0    10823 2023-05-25 07:24:44.000000 steam-sdk-2023.6.0/steam_sdk/data/DataLEDET.py
+-rw-rw-rw-   0        0        0     4314 2022-08-22 11:29:04.000000 steam-sdk-2023.6.0/steam_sdk/data/DataModelCircuit.py
+-rw-rw-rw-   0        0        0     5869 2022-09-28 09:57:32.000000 steam-sdk-2023.6.0/steam_sdk/data/DataModelConductor.py
+-rw-rw-rw-   0        0        0    35376 2023-05-25 09:55:42.000000 steam-sdk-2023.6.0/steam_sdk/data/DataModelMagnet.py
+-rw-rw-rw-   0        0        0     2636 2023-05-09 19:16:09.000000 steam-sdk-2023.6.0/steam_sdk/data/DataParsimConductor.py
+-rw-rw-rw-   0        0        0        0 2022-09-07 00:41:51.000000 steam-sdk-2023.6.0/steam_sdk/data/DataParsims.py
+-rw-rw-rw-   0        0        0     1995 2022-03-07 20:47:17.000000 steam-sdk-2023.6.0/steam_sdk/data/DataProteCCT.py
+-rw-rw-rw-   0        0        0     2105 2022-09-28 09:57:32.000000 steam-sdk-2023.6.0/steam_sdk/data/DataPyBBQ.py
+-rw-rw-rw-   0        0        0     8068 2023-05-25 09:55:42.000000 steam-sdk-2023.6.0/steam_sdk/data/DataRoxieParser.py
+-rw-rw-rw-   0        0        0     6791 2023-05-09 19:16:09.000000 steam-sdk-2023.6.0/steam_sdk/data/DataSIGMA.py
+-rw-rw-rw-   0        0        0     1729 2023-05-25 11:21:07.000000 steam-sdk-2023.6.0/steam_sdk/data/DataSettings.py
+-rw-rw-rw-   0        0        0     3204 2023-01-05 21:02:33.000000 steam-sdk-2023.6.0/steam_sdk/data/DataSignal.py
+-rw-rw-rw-   0        0        0    23052 2023-05-25 07:24:44.000000 steam-sdk-2023.6.0/steam_sdk/data/DictionaryLEDET.py
+-rw-rw-rw-   0        0        0     4482 2022-08-23 08:56:30.000000 steam-sdk-2023.6.0/steam_sdk/data/DictionaryProteCCT.py
+-rw-rw-rw-   0        0        0     2902 2022-09-28 09:57:32.000000 steam-sdk-2023.6.0/steam_sdk/data/DictionaryPyBBQ.py
+-rw-rw-rw-   0        0        0    27819 2023-05-25 07:24:44.000000 steam-sdk-2023.6.0/steam_sdk/data/TemplateLEDET.py
+-rw-rw-rw-   0        0        0     7903 2022-03-30 17:37:43.000000 steam-sdk-2023.6.0/steam_sdk/data/TemplateProteCCT.py
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 21:57:17.933100 steam-sdk-2023.6.0/steam_sdk/drivers/
+-rw-rw-rw-   0        0        0     3151 2022-12-06 11:41:34.000000 steam-sdk-2023.6.0/steam_sdk/drivers/DriverAnalysis.py
+-rw-rw-rw-   0        0        0     2711 2022-12-06 11:41:34.000000 steam-sdk-2023.6.0/steam_sdk/drivers/DriverDakota.py
+-rw-rw-rw-   0        0        0     1299 2023-02-02 08:17:41.000000 steam-sdk-2023.6.0/steam_sdk/drivers/DriverFiQuS.py
+-rw-rw-rw-   0        0        0     3482 2022-12-16 13:26:54.000000 steam-sdk-2023.6.0/steam_sdk/drivers/DriverLEDET.py
+-rw-rw-rw-   0        0        0     1924 2022-10-31 08:36:49.000000 steam-sdk-2023.6.0/steam_sdk/drivers/DriverPSPICE.py
+-rw-rw-rw-   0        0        0     2062 2022-09-26 06:59:06.000000 steam-sdk-2023.6.0/steam_sdk/drivers/DriverProteCCT.py
+-rw-rw-rw-   0        0        0     2219 2022-06-02 08:33:55.000000 steam-sdk-2023.6.0/steam_sdk/drivers/DriverPyBBQ.py
+-rw-rw-rw-   0        0        0     3905 2023-05-19 10:14:24.000000 steam-sdk-2023.6.0/steam_sdk/drivers/DriverSIGMA.py
+-rw-rw-rw-   0        0        0     1932 2022-10-31 08:36:49.000000 steam-sdk-2023.6.0/steam_sdk/drivers/DriverXYCE.py
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/drivers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 21:57:18.142286 steam-sdk-2023.6.0/steam_sdk/parsers/
+-rw-rw-rw-   0        0        0     4984 2022-08-22 11:29:04.000000 steam-sdk-2023.6.0/steam_sdk/parsers/CSD_Reader.py
+-rw-rw-rw-   0        0        0      317 2023-04-17 13:02:30.000000 steam-sdk-2023.6.0/steam_sdk/parsers/ParserCOMSOLToTxt.py
+-rw-rw-rw-   0        0        0     2290 2022-06-24 07:36:06.000000 steam-sdk-2023.6.0/steam_sdk/parsers/ParserCond2d.py
+-rw-rw-rw-   0        0        0     1081 2023-05-24 11:49:42.000000 steam-sdk-2023.6.0/steam_sdk/parsers/ParserCsd.py
+-rw-rw-rw-   0        0        0     6220 2023-01-16 11:54:48.000000 steam-sdk-2023.6.0/steam_sdk/parsers/ParserCsv.py
+-rw-rw-rw-   0        0        0     1650 2023-01-13 08:48:18.000000 steam-sdk-2023.6.0/steam_sdk/parsers/ParserDakota.py
+-rw-rw-rw-   0        0        0     1030 2023-03-13 09:01:17.000000 steam-sdk-2023.6.0/steam_sdk/parsers/ParserDatToCsv.py
+-rw-rw-rw-   0        0        0     8536 2023-02-02 15:29:22.000000 steam-sdk-2023.6.0/steam_sdk/parsers/ParserExcel.py
+-rw-rw-rw-   0        0        0     2287 2022-09-30 09:15:14.000000 steam-sdk-2023.6.0/steam_sdk/parsers/ParserFiQuS.py
+-rw-rw-rw-   0        0        0    48055 2023-05-25 09:53:27.000000 steam-sdk-2023.6.0/steam_sdk/parsers/ParserLEDET.py
+-rw-rw-rw-   0        0        0    12436 2022-11-21 14:56:04.000000 steam-sdk-2023.6.0/steam_sdk/parsers/ParserMap2d.py
+-rw-rw-rw-   0        0        0    14159 2023-05-22 14:09:18.000000 steam-sdk-2023.6.0/steam_sdk/parsers/ParserMat.py
+-rw-rw-rw-   0        0        0    63401 2023-05-31 09:59:27.000000 steam-sdk-2023.6.0/steam_sdk/parsers/ParserPSPICE.py
+-rw-rw-rw-   0        0        0     4780 2023-03-03 12:33:32.000000 steam-sdk-2023.6.0/steam_sdk/parsers/ParserPdf.py
+-rw-rw-rw-   0        0        0     6838 2023-02-03 13:16:35.000000 steam-sdk-2023.6.0/steam_sdk/parsers/ParserProteCCT.py
+-rw-rw-rw-   0        0        0     2942 2022-09-26 06:59:06.000000 steam-sdk-2023.6.0/steam_sdk/parsers/ParserProtePyBBQ.py
+-rw-rw-rw-   0        0        0    95752 2023-05-25 09:55:42.000000 steam-sdk-2023.6.0/steam_sdk/parsers/ParserRoxie.py
+-rw-rw-rw-   0        0        0     1928 2023-05-09 19:16:09.000000 steam-sdk-2023.6.0/steam_sdk/parsers/ParserSIGMA.py
+-rw-rw-rw-   0        0        0    11707 2022-09-07 14:38:46.000000 steam-sdk-2023.6.0/steam_sdk/parsers/ParserTdms.py
+-rw-rw-rw-   0        0        0    55281 2023-02-02 12:20:26.000000 steam-sdk-2023.6.0/steam_sdk/parsers/ParserXYCE.py
+-rw-rw-rw-   0        0        0     4195 2023-05-22 14:09:18.000000 steam-sdk-2023.6.0/steam_sdk/parsers/ParserYAML.py
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/parsers/__init__.py
+-rw-rw-rw-   0        0        0        2 2022-09-02 10:44:52.000000 steam-sdk-2023.6.0/steam_sdk/parsers/dict_to_in.py
+drwxrwxrwx   0        0        0        0 2023-06-01 21:57:18.204066 steam-sdk-2023.6.0/steam_sdk/parsims/
+-rw-rw-rw-   0        0        0    61782 2023-05-23 14:33:11.000000 steam-sdk-2023.6.0/steam_sdk/parsims/ParsimConductor.py
+-rw-rw-rw-   0        0        0      916 2022-09-26 06:59:06.000000 steam-sdk-2023.6.0/steam_sdk/parsims/ParsimDakota.py
+-rw-rw-rw-   0        0        0    72533 2023-05-19 10:14:24.000000 steam-sdk-2023.6.0/steam_sdk/parsims/ParsimEventCircuit.py
+-rw-rw-rw-   0        0        0    48206 2023-05-25 09:55:42.000000 steam-sdk-2023.6.0/steam_sdk/parsims/ParsimEventMagnet.py
+-rw-rw-rw-   0        0        0     1972 2023-01-24 08:05:20.000000 steam-sdk-2023.6.0/steam_sdk/parsims/ParsimSweep.py
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/parsims/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 21:57:18.250904 steam-sdk-2023.6.0/steam_sdk/plotters/
+-rw-rw-rw-   0        0        0     8053 2023-05-12 14:38:34.000000 steam-sdk-2023.6.0/steam_sdk/plotters/PlotterAnalysis.py
+-rw-rw-rw-   0        0        0    20391 2023-05-25 09:55:42.000000 steam-sdk-2023.6.0/steam_sdk/plotters/PlotterMap2d.py
+-rw-rw-rw-   0        0        0    39596 2022-06-20 13:00:15.000000 steam-sdk-2023.6.0/steam_sdk/plotters/PlotterModel.py
+-rw-rw-rw-   0        0        0    22987 2022-12-06 11:41:34.000000 steam-sdk-2023.6.0/steam_sdk/plotters/PlotterParametric.py
+-rw-rw-rw-   0        0        0     8863 2023-05-25 09:55:42.000000 steam-sdk-2023.6.0/steam_sdk/plotters/PlotterRoxie.py
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/plotters/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 21:57:18.259619 steam-sdk-2023.6.0/steam_sdk/postprocs/
+-rw-rw-rw-   0        0        0     5564 2022-09-26 06:59:06.000000 steam-sdk-2023.6.0/steam_sdk/postprocs/PostprocsMetrics.py
+-rw-rw-rw-   0        0        0        0 2022-09-14 13:30:58.000000 steam-sdk-2023.6.0/steam_sdk/postprocs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 21:57:18.423866 steam-sdk-2023.6.0/steam_sdk/utils/
+-rw-rw-rw-   0        0        0     2679 2023-03-13 09:01:17.000000 steam-sdk-2023.6.0/steam_sdk/utils/MTF_reading_functions.py
+-rw-rw-rw-   0        0        0    14942 2022-06-30 20:06:54.000000 steam-sdk-2023.6.0/steam_sdk/utils/ModifyModelData.py
+-rw-rw-rw-   0        0        0     4707 2023-05-22 14:09:18.000000 steam-sdk-2023.6.0/steam_sdk/utils/ModifyModelDataMagnet.py
+-rw-rw-rw-   0        0        0     2747 2023-05-22 14:09:18.000000 steam-sdk-2023.6.0/steam_sdk/utils/ModifyModelDataconductor.py
+-rw-rw-rw-   0        0        0      313 2022-03-01 14:21:51.000000 steam-sdk-2023.6.0/steam_sdk/utils/NumpyEncoder.py
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/utils/__init__.py
+-rw-rw-rw-   0        0        0      686 2022-06-12 12:41:34.000000 steam-sdk-2023.6.0/steam_sdk/utils/clean_NaN_from_signal.py
+-rw-rw-rw-   0        0        0     3837 2023-02-03 13:26:48.000000 steam-sdk-2023.6.0/steam_sdk/utils/compare_two_parameters.py
+-rw-rw-rw-   0        0        0      590 2023-05-09 19:16:09.000000 steam-sdk-2023.6.0/steam_sdk/utils/create_coordinate_file_SIGMA.py
+-rw-rw-rw-   0        0        0     1279 2023-04-17 13:02:30.000000 steam-sdk-2023.6.0/steam_sdk/utils/get_attribute_type.py
+-rw-rw-rw-   0        0        0      167 2022-06-11 12:54:31.000000 steam-sdk-2023.6.0/steam_sdk/utils/isNaN.py
+-rw-rw-rw-   0        0        0      299 2022-04-12 00:42:08.000000 steam-sdk-2023.6.0/steam_sdk/utils/make_folder_if_not_existing.py
+-rw-rw-rw-   0        0        0     4512 2022-05-02 08:49:48.000000 steam-sdk-2023.6.0/steam_sdk/utils/misc.py
+-rw-rw-rw-   0        0        0     1592 2023-04-17 13:02:30.000000 steam-sdk-2023.6.0/steam_sdk/utils/parse_str_to_list.py
+-rw-rw-rw-   0        0        0      388 2022-04-11 18:20:26.000000 steam-sdk-2023.6.0/steam_sdk/utils/rgetattr.py
+-rw-rw-rw-   0        0        0      460 2023-01-07 20:16:27.000000 steam-sdk-2023.6.0/steam_sdk/utils/rhasattr.py
+-rw-rw-rw-   0        0        0      383 2022-04-11 18:20:26.000000 steam-sdk-2023.6.0/steam_sdk/utils/sgetattr.py
+-rw-rw-rw-   0        0        0      863 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/utils/tic_toc.py
+-rw-rw-rw-   0        0        0      168 2022-06-07 19:34:59.000000 steam-sdk-2023.6.0/steam_sdk/utils/unique.py
+-rw-rw-rw-   0        0        0     7005 2023-05-12 14:38:34.000000 steam-sdk-2023.6.0/steam_sdk/utils/utils_PC.py
+drwxrwxrwx   0        0        0        0 2023-06-01 21:57:18.453889 steam-sdk-2023.6.0/steam_sdk/viewers/
+-rw-rw-rw-   0        0        0    35919 2023-03-23 14:48:07.000000 steam-sdk-2023.6.0/steam_sdk/viewers/Viewer.py
+-rw-rw-rw-   0        0        0     6127 2022-06-13 00:34:14.000000 steam-sdk-2023.6.0/steam_sdk/viewers/ViewerMeas.py
+-rw-rw-rw-   0        0        0     1667 2022-06-20 13:06:20.000000 steam-sdk-2023.6.0/steam_sdk/viewers/ViewerSim.py
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/viewers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 21:57:18.463547 steam-sdk-2023.6.0/steam_sdk/wrappers/
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/wrappers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 21:57:18.464544 steam-sdk-2023.6.0/steam_sdk/wrappers/java/
+drwxrwxrwx   0        0        0        0 2023-06-01 21:57:18.465541 steam-sdk-2023.6.0/steam_sdk/wrappers/java/SING/
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/wrappers/java/SING/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 21:57:18.467047 steam-sdk-2023.6.0/steam_sdk/wrappers/java/SING/jars/
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/wrappers/java/SING/jars/__init__.py
+-rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2023.6.0/steam_sdk/wrappers/java/__init__.py
+-rw-rw-rw-   0        0        0     1834 2022-07-05 13:48:59.000000 steam-sdk-2023.6.0/steam_sdk/wrappers/wrapper_yaml.py
+drwxrwxrwx   0        0        0        0 2023-06-01 21:57:17.319557 steam-sdk-2023.6.0/steam_sdk.egg-info/
+-rw-rw-rw-   0        0        0     1550 2023-06-01 21:57:16.000000 steam-sdk-2023.6.0/steam_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6686 2023-06-01 21:57:17.000000 steam-sdk-2023.6.0/steam_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 21:57:16.000000 steam-sdk-2023.6.0/steam_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1597 2023-06-01 21:57:16.000000 steam-sdk-2023.6.0/steam_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-01 21:57:16.000000 steam-sdk-2023.6.0/steam_sdk.egg-info/top_level.txt
```

### Comparing `steam-sdk-2023.5.4/PKG-INFO` & `steam-sdk-2023.6.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: steam-sdk
-Version: 2023.5.4
+Version: 2023.6.0
 Summary: Source code for APIs for STEAM tools.
 Home-page: https://gitlab.cern.ch/steam/steam_sdk
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: STEAM,CERN,API,SDK
+Keywords: CERN,STEAM,SDK,API
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM_SDK
```

### Comparing `steam-sdk-2023.5.4/setup.py` & `steam-sdk-2023.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='steam-sdk',
-    version="2023.5.4",
+    version="2023.6.0",
     author="STEAM Team",
     author_email="steam-team@cern.ch",
     description="Source code for APIs for STEAM tools.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://gitlab.cern.ch/steam/steam_sdk",
     keywords={'STEAM', 'API', 'SDK', 'CERN'},
```

### Comparing `steam-sdk-2023.5.4/steam_sdk/analyses/AnalysisSTEAM.py` & `steam-sdk-2023.6.0/steam_sdk/analyses/AnalysisSTEAM.py`

 * *Files 0% similar despite different names*

```diff
@@ -293,15 +293,15 @@
             print('Making model object named {}'.format(str(step.model_name)))
         ## Assuming the steam-models directory structure if 'steam-models' or model_library found at the end of library path.
         # Else assuming library path directs straight to the model
         if (str(self.library_path).endswith('steam_models')) or (str(self.library_path).endswith('steam-models')) or (
                 str(self.library_path).endswith('model_library')):
             file_model_data = os.path.join(self.library_path, step.case_model + 's', step.file_model_data, 'input',
                                            'modelData_' + step.file_model_data + '.yaml')
-        elif isinstance(self.library_path, str):
+        elif isinstance(self.library_path, (str, Path)):
             if self.library_path == 'same_as_analysis_yaml_use_model_name':
                 file_model_data = '.' + os.sep + step.file_model_data + os.sep + 'input' + os.sep + 'modelData_' + step.file_model_data + '.yaml'
                 file_model_data = Path(file_model_data).resolve()
             else:
                 file_model_data = os.path.join(self.library_path, 'modelData_' + step.file_model_data + '.yaml')
 
         case_model = step.case_model
```

### Comparing `steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py` & `steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py` & `steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py` & `steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py` & `steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py` & `steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py` & `steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py` & `steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py` & `steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py` & `steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py` & `steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py` & `steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py` & `steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py` & `steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py` & `steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py` & `steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py` & `steam-sdk-2023.6.0/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/builders/BuilderFiQuS.py` & `steam-sdk-2023.6.0/steam_sdk/builders/BuilderFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/builders/BuilderLEDET.py` & `steam-sdk-2023.6.0/steam_sdk/builders/BuilderLEDET.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,14 +148,17 @@
 
                 # Load conductor data from DataModelConductor keys
                 self.loadConductorData(overwrite_conductor_to_group = [1])
 
                 # Assign default values to LEDET variables defining coil windings parameters
                 self.assignDefaultValuesWindings()
 
+                # If needed, convert QH parameters from strings to integers
+                self.convert_QH_parameters()
+
 
     def loadDefaultVariableDescriptions(self, fileVariableDescriptions: str):
         """
             **Loads and sets the LEDET descriptions**
 
             Function to load and set the descriptions of LEDET parameters
 
@@ -378,15 +381,15 @@
         self.Tc0_NbTi_ht_inGroup = np.array([])
         self.Bc2_NbTi_ht_inGroup = np.array([])
         self.c1_Ic_NbTi_inGroup = np.array([])
         self.c2_Ic_NbTi_inGroup = np.array([])
         self.Tc0_Nb3Sn_inGroup = np.array([])
         self.Bc2_Nb3Sn_inGroup = np.array([])
         self.Jc_Nb3Sn0_inGroup = np.array([])
-        self.alpha_Nb3Sn0_inGroup = np.array([])
+        self.alpha_Nb3Sn_inGroup = np.array([])
         self.f_scaling_Jc_BSCCO2212_inGroup = np.array([])
         self.selectedFit_inGroup = np.array([], dtype=np.uint32)
         self.fitParameters_inGroup = np.empty((8, 0))  # Special case: This variable will be written as a matrix with 8 rows TODO find a solution for this special one - in LEDET this can be a matrix
 
         # For each group, load the cable, strand, and Jc-fit parameters according to their type
         for group, conductor_type in enumerate(conductor_to_group):
             if self.verbose: print('Group/Block #{}. Selected conductor: {}'.format(group + 1, conductor_type))
@@ -401,15 +404,15 @@
             'Tc0_NbTi_ht_inGroup',
             'Bc2_NbTi_ht_inGroup',
             'c1_Ic_NbTi_inGroup',
             'c2_Ic_NbTi_inGroup',
             'Tc0_Nb3Sn_inGroup',
             'Bc2_Nb3Sn_inGroup',
             'Jc_Nb3Sn0_inGroup',
-            'alpha_Nb3Sn0_inGroup',
+            'alpha_Nb3Sn_inGroup',
             'f_scaling_Jc_BSCCO2212_inGroup',
             'selectedFit_inGroup',
             ]
         for var in list_conductor_vars:
             temp_var = getattr(self, var)  # not efficient coding, but it should improve readibility
             if not np.all(np.isnan(temp_var)):
                 # The values will be changed from nan to 0.0 unless they are all nan (in that case, they'll remain nan)
@@ -443,15 +446,15 @@
         self.setAttribute(self.Inputs, 'Tc0_NbTi_ht_inGroup', self.Tc0_NbTi_ht_inGroup)
         self.setAttribute(self.Inputs, 'Bc2_NbTi_ht_inGroup', self.Bc2_NbTi_ht_inGroup)
         self.setAttribute(self.Inputs, 'c1_Ic_NbTi_inGroup', self.c1_Ic_NbTi_inGroup)
         self.setAttribute(self.Inputs, 'c2_Ic_NbTi_inGroup', self.c2_Ic_NbTi_inGroup)
         self.setAttribute(self.Inputs, 'Tc0_Nb3Sn_inGroup', self.Tc0_Nb3Sn_inGroup)
         self.setAttribute(self.Inputs, 'Bc2_Nb3Sn_inGroup', self.Bc2_Nb3Sn_inGroup)
         self.setAttribute(self.Inputs, 'Jc_Nb3Sn0_inGroup', self.Jc_Nb3Sn0_inGroup)
-        self.setAttribute(self.Inputs, 'alpha_Nb3Sn0_inGroup', self.alpha_Nb3Sn0_inGroup)
+        self.setAttribute(self.Inputs, 'alpha_Nb3Sn_inGroup', self.alpha_Nb3Sn_inGroup)
         self.setAttribute(self.Inputs, 'f_scaling_Jc_BSCCO2212_inGroup', self.f_scaling_Jc_BSCCO2212_inGroup)
         self.setAttribute(self.Inputs, 'selectedFit_inGroup', self.selectedFit_inGroup)
         self.setAttribute(self.Inputs, 'fitParameters_inGroup', self.fitParameters_inGroup)
         #TODO: CUDI3
 
 
     def loadCableData(self, conductor_id):
@@ -566,15 +569,15 @@
             self.Tc0_NbTi_ht_inGroup  = np.append(self.Tc0_NbTi_ht_inGroup, conductor.Jc_fit.Tc0_CUDI1)
             self.Bc2_NbTi_ht_inGroup  = np.append(self.Bc2_NbTi_ht_inGroup, conductor.Jc_fit.Bc20_CUDI1)
             self.c1_Ic_NbTi_inGroup   = np.append(self.c1_Ic_NbTi_inGroup  , conductor.Jc_fit.C1_CUDI1)
             self.c2_Ic_NbTi_inGroup   = np.append(self.c2_Ic_NbTi_inGroup  , conductor.Jc_fit.C2_CUDI1)
             self.Tc0_Nb3Sn_inGroup    = np.append(self.Tc0_Nb3Sn_inGroup, 0)
             self.Bc2_Nb3Sn_inGroup    = np.append(self.Bc2_Nb3Sn_inGroup, 0)
             self.Jc_Nb3Sn0_inGroup    = np.append(self.Jc_Nb3Sn0_inGroup, 0)
-            self.alpha_Nb3Sn0_inGroup = np.append(self.alpha_Nb3Sn0_inGroup, np.nan)
+            self.alpha_Nb3Sn_inGroup  = np.append(self.alpha_Nb3Sn_inGroup, np.nan)
             self.f_scaling_Jc_BSCCO2212_inGroup = np.append(self.f_scaling_Jc_BSCCO2212_inGroup, np.nan)
             self.selectedFit_inGroup = np.append(self.selectedFit_inGroup, 6)  # TODO: not yet supported by LEDET
             temp_fitParam = np.array([conductor.Jc_fit.Tc0_CUDI1, conductor.Jc_fit.Bc20_CUDI1, conductor.Jc_fit.C1_CUDI1, conductor.Jc_fit.C2_CUDI1, 0, 0, 0, 0])  # Last values not needed for this fit and set to 0
             self.fitParameters_inGroup = np.column_stack((self.fitParameters_inGroup, temp_fitParam))  # At each step, add one more column to the matrix
         # TODO: CUDI3 to enable for quench protection simulations
         elif type_JcFit == 'CUDI3':
             self.selectedFit_inGroup = np.append(self.selectedFit_inGroup, 3)  # TODO: not yet supported by LEDET
@@ -597,41 +600,41 @@
             self.Tc0_NbTi_ht_inGroup            = np.append(self.Tc0_NbTi_ht_inGroup  , 0)
             self.Bc2_NbTi_ht_inGroup            = np.append(self.Bc2_NbTi_ht_inGroup  , 0)
             self.c1_Ic_NbTi_inGroup             = np.append(self.c1_Ic_NbTi_inGroup   , 0)
             self.c2_Ic_NbTi_inGroup             = np.append(self.c2_Ic_NbTi_inGroup   , 0)
             self.Tc0_Nb3Sn_inGroup              = np.append(self.Tc0_Nb3Sn_inGroup    , conductor.Jc_fit.Tc0_Summers)
             self.Bc2_Nb3Sn_inGroup              = np.append(self.Bc2_Nb3Sn_inGroup    , conductor.Jc_fit.Bc20_Summers)
             self.Jc_Nb3Sn0_inGroup              = np.append(self.Jc_Nb3Sn0_inGroup    , conductor.Jc_fit.Jc0_Summers)
-            self.alpha_Nb3Sn0_inGroup           = np.append(self.alpha_Nb3Sn0_inGroup, np.nan)
+            self.alpha_Nb3Sn_inGroup            = np.append(self.alpha_Nb3Sn_inGroup, np.nan)
             self.f_scaling_Jc_BSCCO2212_inGroup = np.append(self.f_scaling_Jc_BSCCO2212_inGroup, np.nan)
             self.selectedFit_inGroup = np.append(self.selectedFit_inGroup             , 4)
             temp_fitParam = np.array([conductor.Jc_fit.Tc0_Summers, conductor.Jc_fit.Bc20_Summers, conductor.Jc_fit.Jc0_Summers, 0, 0, 0, 0, 0])  # Last values not needed for this fit and set to 0
             self.fitParameters_inGroup          = np.column_stack((self.fitParameters_inGroup, temp_fitParam))  # At each step, add one more column to the matrix
         elif type_JcFit == 'Bordini':
             self.Tc0_NbTi_ht_inGroup            = np.append(self.Tc0_NbTi_ht_inGroup  , 0)
             self.Bc2_NbTi_ht_inGroup            = np.append(self.Bc2_NbTi_ht_inGroup  , 0)
             self.c1_Ic_NbTi_inGroup             = np.append(self.c1_Ic_NbTi_inGroup   , 0)
             self.c2_Ic_NbTi_inGroup             = np.append(self.c2_Ic_NbTi_inGroup   , 0)
             self.Tc0_Nb3Sn_inGroup              = np.append(self.Tc0_Nb3Sn_inGroup    , conductor.Jc_fit.Tc0_Bordini)
             self.Bc2_Nb3Sn_inGroup              = np.append(self.Bc2_Nb3Sn_inGroup    , conductor.Jc_fit.Bc20_Bordini)
             self.Jc_Nb3Sn0_inGroup              = np.append(self.Jc_Nb3Sn0_inGroup    , conductor.Jc_fit.C0_Bordini)
-            self.alpha_Nb3Sn0_inGroup           = np.append(self.alpha_Nb3Sn0_inGroup , conductor.Jc_fit.alpha_Bordini)
+            self.alpha_Nb3Sn_inGroup            = np.append(self.alpha_Nb3Sn_inGroup , conductor.Jc_fit.alpha_Bordini)
             self.f_scaling_Jc_BSCCO2212_inGroup = np.append(self.f_scaling_Jc_BSCCO2212_inGroup, np.nan)
             self.selectedFit_inGroup            = np.append(self.selectedFit_inGroup  , 5)  # TODO: not yet supported by LEDET
             temp_fitParam = np.array([conductor.Jc_fit.Tc0_Bordini, conductor.Jc_fit.Bc20_Bordini, conductor.Jc_fit.C0_Bordini, conductor.Jc_fit.alpha_Bordini, 0, 0, 0, 0])  # Last values not needed for this fit and set to 0
             self.fitParameters_inGroup          = np.column_stack((self.fitParameters_inGroup, temp_fitParam))  # At each step, add one more column to the matrix
         elif type_JcFit == 'BSCCO_2212_LBNL':
             self.Tc0_NbTi_ht_inGroup            = np.append(self.Tc0_NbTi_ht_inGroup  , 0)
             self.Bc2_NbTi_ht_inGroup            = np.append(self.Bc2_NbTi_ht_inGroup  , 0)
             self.c1_Ic_NbTi_inGroup             = np.append(self.c1_Ic_NbTi_inGroup   , 0)
             self.c2_Ic_NbTi_inGroup             = np.append(self.c2_Ic_NbTi_inGroup   , 0)
             self.Tc0_Nb3Sn_inGroup              = np.append(self.Tc0_Nb3Sn_inGroup    , 0)
             self.Bc2_Nb3Sn_inGroup              = np.append(self.Bc2_Nb3Sn_inGroup    , 0)
             self.Jc_Nb3Sn0_inGroup              = np.append(self.Jc_Nb3Sn0_inGroup    , 0)
-            self.alpha_Nb3Sn0_inGroup           = np.append(self.alpha_Nb3Sn0_inGroup, np.nan)
+            self.alpha_Nb3Sn_inGroup            = np.append(self.alpha_Nb3Sn_inGroup, np.nan)
             self.f_scaling_Jc_BSCCO2212_inGroup = np.append(self.f_scaling_Jc_BSCCO2212_inGroup, conductor.Jc_fit.f_scaling_Jc_BSCCO2212)  # TODO problem when only some conductors have BSCO2212
             self.selectedFit_inGroup            = np.append(self.selectedFit_inGroup  , 51)  # TODO: not yet supported by LEDET
             temp_fitParam = np.array([conductor.Jc_fit.f_scaling_Jc_BSCCO2212, 0, 0, 0, 0, 0, 0, 0])  # Last values not needed for this fit and set to 0
             self.fitParameters_inGroup          = np.column_stack((self.fitParameters_inGroup, temp_fitParam))  # At each step, add one more column to the matrix
         else:
             raise Exception('Group #{}. Selected Jc-fit type ({}) is not supported.'.format(conductor_id, type_JcFit))
```

### Comparing `steam-sdk-2023.5.4/steam_sdk/builders/BuilderModel.py` & `steam-sdk-2023.6.0/steam_sdk/builders/BuilderModel.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from steam_sdk.parsers.ParserRoxie import ParserRoxie
 from steam_sdk.parsers.ParserMap2d import getParametersFromMap2d
 from steam_sdk.parsers.ParserYAML import dict_to_yaml, yaml_to_data
 from steam_sdk.plotters import PlotterRoxie
 from steam_sdk.plotters.PlotterModel import PlotterModel
 from steam_sdk.utils.create_coordinate_file_SIGMA import create_coordinate_file
 
+
 class BuilderModel:
     """
         Class to generate STEAM models, which can be later on written to input files of supported programs
     """
 
     def __init__(self,
                  file_model_data: str = None, software: [str] = None, case_model: str = 'magnet',
@@ -106,15 +107,15 @@
                 self.loadRoxieData()
 
                 # Build model
                 for s in self.software:
                     if s == 'FiQuS':    self.buildFiQuS()
                     if s == 'LEDET':    self.buildLEDET()
                     if s == 'ProteCCT': self.buildProteCCT()
-                    if s == 'SIGMA':    self.buildSIGMA()   # TODO: raise error when wrong software selected?
+                    if s == 'SIGMA':    self.buildSIGMA()  # TODO: raise error when wrong software selected?
 
                 if flag_dump_all:
                     self.dumpAll()
 
                 if flag_plot_all:
                     PlotterRoxie.plot_all(self.roxie_data)
                     PM = PlotterModel(self.roxie_data)
@@ -128,23 +129,25 @@
 
             # If flag_build set true, the model will be generated during the initialization
             if flag_build:
                 if self.verbose:
                     print('output_path: {}'.format(self.output_path))
 
                 # Load model data from the input .yaml file
-                self.loadModelData()  #TODO consider if this should be moved before the "if flag_build" statement
+                self.loadModelData()  # TODO consider if this should be moved before the "if flag_build" statement
 
                 # Set paths of input files and settings
                 self.set_input_paths()
 
                 # Build circuit model
                 for s in self.software:
-                    if s == 'PSPICE': self.buildPSPICE()
-                    elif s == 'XYCE': self.buildXYCE()
+                    if s == 'PSPICE':
+                        self.buildPSPICE()
+                    elif s == 'XYCE':
+                        self.buildXYCE()
                     else:
                         raise Exception('Please specify software (PSPICE/XYCE).')
 
         ### Case of a conductor model
         elif self.case_model == 'conductor':
             # Initialize
             self.conductor_data: DataModelConductor = DataModelConductor()
@@ -160,15 +163,15 @@
 
                 # Set paths of input files and settings
                 self.set_input_paths()
 
                 # Build model
                 for s in self.software:
                     if s == 'LEDET':    self.buildLEDET()
-                    if s == 'PyBBQ':    self.buildPyBBQ() # TODO: raise error when wrong software selected?
+                    if s == 'PyBBQ':    self.buildPyBBQ()  # TODO: raise error when wrong software selected?
 
         # Display time stamp
         if self.verbose:
             print(f'BuilderModel ended. Time stamp: {datetime.datetime.now()}')
 
     def set_input_paths(self):
         """
@@ -179,15 +182,14 @@
         # Find folder where the input file is located, which will be used as the "anchor" for all input files
         self.path_magnet = Path(self.file_model_data).parent
         self.path_data = None
         self.path_map2d = None
         self.path_cadata = None
         self.path_iron = None
 
-
         if self.case_model == 'magnet':
             # Set a few paths relative to the "anchor" path
             # If input paths are not defined, their value remains to their default None
             # The construct Path(x / y).resolve() allows defining relative paths in the .yaml input file
             if self.model_data.Sources.coil_fromROXIE:
                 self.path_data = Path(self.path_magnet / self.model_data.Sources.coil_fromROXIE).resolve()
             if self.model_data.Sources.magnetic_field_fromROXIE:
@@ -249,19 +251,19 @@
             raise Exception('No .yaml path provided.')
 
         if self.case_model == 'magnet':
             # Load yaml keys into DataModelMagnet dataclass
             self.model_data = yaml_to_data(self.file_model_data, DataModelMagnet)
         elif self.case_model == 'circuit':
             for s in self.software:
-                if s=='PSPICE':
+                if s == 'PSPICE':
                     Parser = ParserPSPICE(self.circuit_data)
                     Parser.readFromYaml(self.file_model_data)
                     self.circuit_data = Parser.circuit_data
-                elif s=='XYCE':
+                elif s == 'XYCE':
                     Parser = ParserXYCE(self.circuit_data)
                     Parser.readFromYaml(self.file_model_data)
                     self.circuit_data = Parser.circuit_data
                 else:
                     raise Exception('Please specify software (PSPICE/XYCE).')
         elif self.case_model == 'conductor':
             # Load yaml keys into DataModelConductor dataclass
@@ -302,49 +304,53 @@
         """
 
         builder_FiQuS = BuilderFiQuS(model_data=self.model_data, roxie_data=self.roxie_data,
                                      flag_build=self.flag_build, flag_plot_all=self.flag_plot_all, verbose=self.verbose)
 
         # Write output files
         self.parser_FiQuS = ParserFiQuS(builder_FiQuS, verbose=self.verbose)
-        self.parser_FiQuS.writeFiQuS2yaml(output_path=self.output_path, simulation_name=simulation_name, append_str_to_magnet_name='_FiQuS')
+        self.parser_FiQuS.writeFiQuS2yaml(output_path=self.output_path, simulation_name=simulation_name,
+                                          append_str_to_magnet_name='_FiQuS')
 
     def buildLEDET(self):
         """
             Building a LEDET model
             case_model is a string defining the type of model to build (magnet or conductor)
         """
 
         if self.case_model == 'magnet':
             magnet_name = self.model_data.GeneralParameters.magnet_name
-            nameFileSMIC = os.path.join(self.output_path, magnet_name + '_selfMutualInductanceMatrix.csv')  # full path of the .csv file with self-mutual inductances to write
+            nameFileSMIC = os.path.join(self.output_path,
+                                        magnet_name + '_selfMutualInductanceMatrix.csv')  # full path of the .csv file with self-mutual inductances to write
 
             # Copy/edit the ROXIE map2d file
             if self.path_map2d:
                 suffix = "_All"
                 if self.model_data.Options_LEDET.field_map_files.flag_modify_map2d_ribbon_cable == 1:
                     #     # [[...half_turn_length, Ribbon...n_strands],.....]
                     # TODO: geometry when conductor has a combination of ribbon and non-ribbon cables
 
                     # List of flags that are True is the cable type is "Ribbon"
                     list_flag_ribbon = []
                     for i, cond in enumerate(self.model_data.CoilWindings.conductor_to_group):
                         list_flag_ribbon.append(self.model_data.Conductors[cond - 1].cable.type == 'Ribbon')
 
                     nT_from_original_map2d, nStrands_inGroup_original_map2d, _, _, _, _, _, _ = getParametersFromMap2d(
-                        map2dFile=self.path_map2d, headerLines=self.model_data.Options_LEDET.field_map_files.headerLines,
+                        map2dFile=self.path_map2d,
+                        headerLines=self.model_data.Options_LEDET.field_map_files.headerLines,
                         verbose=self.verbose)
 
                     n_groups_original_file = len(nT_from_original_map2d)
                     geometry_ribbon_cable = []
 
                     for i in range(n_groups_original_file):
                         list = [None, None]
                         list[0] = int(nStrands_inGroup_original_map2d[i])  # layers
-                        list[1] = nT_from_original_map2d[i]  # number of half-turns; in case it is not a ribbon cable, it is going to be ignored in the modify-ribbon-cable function
+                        list[1] = nT_from_original_map2d[
+                            i]  # number of half-turns; in case it is not a ribbon cable, it is going to be ignored in the modify-ribbon-cable function
                         geometry_ribbon_cable.append(list)
 
                     if self.verbose:
                         print('geometry_ribbon_cable: {}'.format(geometry_ribbon_cable))
 
                     file_name_output = copy_modified_map2d_ribbon_cable(magnet_name,
                                                                         self.path_map2d,
@@ -373,15 +379,16 @@
                 shutil.copy2(input_path_full, output_path_full)
                 if self.verbose:
                     print('File {} copied to {}.'.format(input_path_full, output_path_full))
 
             builder_ledet = BuilderLEDET(path_magnet=self.path_magnet, input_model_data=self.model_data,
                                          input_roxie_data=self.roxie_data, input_map2d=self.map2d_file_modified,
                                          smic_write_path=nameFileSMIC, flag_build=self.flag_build,
-                                         flag_plot_all=self.flag_plot_all, verbose=self.verbose, case_model=self.case_model)
+                                         flag_plot_all=self.flag_plot_all, verbose=self.verbose,
+                                         case_model=self.case_model)
 
             # Copy or modify+copy magnet-name_E....map2d files
             number_input_files = len([entry for entry in os.listdir(self.path_magnet) if
                                       os.path.isfile(os.path.join(self.path_magnet, entry))])
             for file in range(number_input_files + 1):
                 suffix = '_E{}'.format(file)
                 path_map2d_E = os.path.join(self.path_magnet, magnet_name + suffix + '.map2d')
@@ -398,26 +405,29 @@
                         copy_map2d(magnet_name, path_map2d_E, self.output_path,
                                    self.model_data.Options_LEDET.field_map_files.flagIron,
                                    self.model_data.Options_LEDET.field_map_files.flagSelfField, suffix=suffix,
                                    verbose=self.verbose)
 
             # Write output excel file
             parser_ledet = ParserLEDET(builder_ledet)
-            nameFileLEDET = os.path.join(self.output_path, magnet_name + '.xlsx')  # full path of the LEDET input file to write
+            nameFileLEDET = os.path.join(self.output_path,
+                                         magnet_name + '.xlsx')  # full path of the LEDET input file to write
             parser_ledet.writeLedet2Excel(full_path_file_name=nameFileLEDET, verbose=self.verbose,
                                           SkipConsistencyCheck=True)
 
             # Write output yaml file
-            nameFileLedetYaml = os.path.join(self.output_path, magnet_name + '.yaml')  # full path of the LEDET input file to write
+            nameFileLedetYaml = os.path.join(self.output_path,
+                                             magnet_name + '.yaml')  # full path of the LEDET input file to write
             parser_ledet.write2yaml(full_path_file_name=nameFileLedetYaml, verbose=self.verbose,
                                     SkipConsistencyCheck=True)
 
             # Write output json file
             if self.flag_json:
-                nameFileLedetJson = os.path.join(self.output_path, magnet_name + '.json')  # full path of the LEDET input file to write
+                nameFileLedetJson = os.path.join(self.output_path,
+                                                 magnet_name + '.json')  # full path of the LEDET input file to write
                 parser_ledet.write2json(full_path_file_name=nameFileLedetJson, verbose=self.verbose,
                                         SkipConsistencyCheck=True)
 
         elif self.case_model == 'conductor':
             conductor_name = self.conductor_data.GeneralParameters.conductor_name
 
             # Copy the ROXIE map2d file, if defined in the input file
@@ -450,26 +460,29 @@
                                          input_map2d=self.map2d_file_modified,
                                          flag_build=self.flag_build, flag_plot_all=self.flag_plot_all,
                                          verbose=self.verbose,
                                          case_model=self.case_model)
 
             # Write output excel file
             parser_ledet = ParserLEDET(builder_ledet)
-            nameFileLEDET = os.path.join(self.output_path, conductor_name + '.xlsx')  # full path of the LEDET input file to write
+            nameFileLEDET = os.path.join(self.output_path,
+                                         conductor_name + '.xlsx')  # full path of the LEDET input file to write
             parser_ledet.writeLedet2Excel(full_path_file_name=nameFileLEDET, verbose=self.verbose,
                                           SkipConsistencyCheck=True)
 
             # Write output yaml file
-            nameFileLedetYaml = os.path.join(self.output_path, conductor_name + '.yaml')  # full path of the LEDET input file to write
+            nameFileLedetYaml = os.path.join(self.output_path,
+                                             conductor_name + '.yaml')  # full path of the LEDET input file to write
             parser_ledet.write2yaml(full_path_file_name=nameFileLedetYaml, verbose=self.verbose,
                                     SkipConsistencyCheck=True)
 
             # Write output json file
             if self.flag_json:
-                nameFileLedetJson = os.path.join(self.output_path, conductor_name + '.json')  # full path of the LEDET input file to write
+                nameFileLedetJson = os.path.join(self.output_path,
+                                                 conductor_name + '.json')  # full path of the LEDET input file to write
                 parser_ledet.write2json(full_path_file_name=nameFileLedetJson, verbose=self.verbose,
                                         SkipConsistencyCheck=True)
 
         else:
             raise Exception('Case model {} is not supported when building a LEDET model.'.format(self.case_model))
 
     def buildProteCCT(self):
@@ -479,71 +492,80 @@
 
         magnet_name = self.model_data.GeneralParameters.magnet_name
         builder_protecct = BuilderProteCCT(input_model_data=self.model_data, flag_build=self.flag_build,
                                            verbose=self.verbose)
 
         # Write output excel file
         parser_protecct = ParserProteCCT(builder_protecct)
-        nameFileProteCCT = os.path.join(self.output_path, f'{magnet_name}_ProteCCT.xlsx')  # full path of the ProteCCT input file to write
+        nameFileProteCCT = os.path.join(self.output_path,
+                                        f'{magnet_name}_ProteCCT.xlsx')  # full path of the ProteCCT input file to write
         parser_protecct.writeProtecct2Excel(full_path_file_name=nameFileProteCCT, verbose=self.verbose,
                                             SkipConsistencyCheck=True)
 
     def buildPSPICE(self):
         """
             Build a PSPICE circuit netlist model
         """
         # Write output .cir file
         parser_pspice = ParserPSPICE(circuit_data=self.circuit_data, path_input=self.path_magnet,
                                      output_path=self.output_path)
-        nameFilePSPICE = os.path.join(self.output_path, self.circuit_data.GeneralParameters.circuit_name + '.cir')  # full path of the PSPICE netlist to write
+        nameFilePSPICE = os.path.join(self.output_path,
+                                      self.circuit_data.GeneralParameters.circuit_name + '.cir')  # full path of the PSPICE netlist to write
         parser_pspice.write2pspice(full_path_file_name=nameFilePSPICE, verbose=self.verbose)
 
         # Copy additional files
         parser_pspice.copy_additional_files()
 
-
     def buildXYCE(self):
         """
             Build a PSPICE circuit netlist model
         """
         # Write output .cir file
-        parser_xyce = ParserXYCE(circuit_data=self.circuit_data, path_input=self.path_magnet,output_path=self.output_path)
-        nameFileXYCE = os.path.join(self.output_path, self.circuit_data.GeneralParameters.circuit_name + '.cir')  # full path of the PSPICE netlist to write
+        parser_xyce = ParserXYCE(circuit_data=self.circuit_data, path_input=self.path_magnet,
+                                 output_path=self.output_path)
+        nameFileXYCE = os.path.join(self.output_path,
+                                    self.circuit_data.GeneralParameters.circuit_name + '.cir')  # full path of the PSPICE netlist to write
         parser_xyce.write2XYCE(nameFileXYCE, verbose=self.verbose)
         parser_xyce.copy_additional_files(flag_translate=True, verbose=self.verbose)
         parser_xyce.resolve_paths_netlist(nameFileXYCE)
 
-
     def buildPyBBQ(self):
         """
             Building a PyBBQ model
         """
 
         conductor_name = self.conductor_data.GeneralParameters.conductor_name
         builder_PyBBQ = BuilderPyBBQ(input_model_data=self.conductor_data, flag_build=self.flag_build,
                                      verbose=self.verbose)
 
         # Write output yaml file
         parser_PyBBQ = ParserPyBBQ(builder_PyBBQ)
-        nameFilePyBBQ = os.path.join(self.output_path, conductor_name + '.yaml')  # full path of the PyBBQ input file to write
+        nameFilePyBBQ = os.path.join(self.output_path,
+                                     conductor_name + '.yaml')  # full path of the PyBBQ input file to write
         parser_PyBBQ.writePyBBQ2yaml(full_path_file_name=nameFilePyBBQ, verbose=self.verbose)
 
-    def buildSIGMA(self, simulation_name = None, library_path = None):
+    def buildSIGMA(self, simulation_name=None, library_path=None):
         """
                   Building a SIGMA model
                   :param simulation_name: This is used in analysis steam to change yaml name from magnet name to simulation name
         """
         # Copy necessary files to working folder
-        bh_data_file_path = os.path.join(library_path, "magnets", "roxie.bhdata")
+        if library_path != None:
+            bh_data_file_path = os.path.join(library_path, "magnets", "roxie.bhdata")
+        else:
+            bh_data_file_path = os.path.join(Path(__file__).parent.parent.parent, 'tests', 'builders', 'model_library',
+                                             'magnets', 'roxie.bhdata')
+
         shutil.copyfile(bh_data_file_path, os.path.join(self.output_path, 'roxie.bhdata'))
 
-        coord_source_prev=self.model_data.Options_SIGMA.postprocessing.out_2D_at_points.coordinate_source
+        coord_source_prev = self.model_data.Options_SIGMA.postprocessing.out_2D_at_points.coordinate_source
         if self.model_data.Options_SIGMA.postprocessing.out_2D_at_points.coordinate_source == None:
             if self.model_data.Options_SIGMA.postprocessing.out_2D_at_points.map2d != None:
-                path_map2d = os.path.join(Path(self.path_bh).parent, self.model_data.GeneralParameters.magnet_name, 'input', self.model_data.Options_SIGMA.postprocessing.out_2D_at_points.map2d )
+                path_map2d = os.path.join(Path(self.path_bh).parent, self.model_data.GeneralParameters.magnet_name,
+                                          'input', self.model_data.Options_SIGMA.postprocessing.out_2D_at_points.map2d)
                 destination_map2d = os.path.join(self.output_path, simulation_name + "_ROXIE_REFERENCE.map2d")
                 # Copy map2d file
                 shutil.copyfile(path_map2d, destination_map2d)
                 coordinate_file_path = os.path.join(self.output_path, simulation_name + "_ROXIE_COORD.csv")
                 # Create coordinate file
                 create_coordinate_file(path_map2d, coordinate_file_path)
                 # Set file as coordinate_source
@@ -574,29 +596,29 @@
         if self.case_model != 'circuit':
             raise Exception(f'This method can only be used for circuit models, but case_model={self.case_model}')
 
         # TODO: Think on whether this is good to add as a default option
         # if selected_circuit_name is None:
         #     selected_circuit_name = self.circuit_data.GeneralParameters.circuit_name
 
-        circuit_param = find_by_position(input_file_name, 0, selected_circuit_name)  # TODO make it more robust by referring to a key rather than the first column
-        #del circuit_param[0]
+        circuit_param = find_by_position(input_file_name, 0,
+                                         selected_circuit_name)  # TODO make it more robust by referring to a key rather than the first column
+        # del circuit_param[0]
         param_names = find_column_list(input_file_name)
-        #del param_names[0]
+        # del param_names[0]
         dict_circuit = {k: v for k, v in zip(param_names, circuit_param)}
 
         for key, value in dict_circuit.items():
             if key in self.circuit_data.GlobalParameters.global_parameters:
                 if self.circuit_data.GlobalParameters.global_parameters[key] != value:
                     if verbose:
-                        print(f'Circuit {self.circuit_data.GeneralParameters.circuit_name}: Value of parameter {key} was changed from {self.circuit_data.GlobalParameters.global_parameters[key]} to {value}')
+                        print(
+                            f'Circuit {self.circuit_data.GeneralParameters.circuit_name}: Value of parameter {key} was changed from {self.circuit_data.GlobalParameters.global_parameters[key]} to {value}')
                     self.circuit_data.GlobalParameters.global_parameters[key] = value
 
-
-
     def dumpAll(self):
         """
             Writes model data and data from Roxie parser in a combined .yaml file
         """
         # TODO add one more layer for model_data and roxie_data
         if self.verbose:
             print('Writing model data and data from Roxie parser in a combined .yaml file')
@@ -614,11 +636,12 @@
 
         # If the output folder is not an empty string, and it does not exist, make it
         if self.dump_all_path != '' and not os.path.isdir(self.dump_all_path):
             print("Output folder {} does not exist. Making it now".format(self.dump_all_path))
             Path(self.dump_all_path).mkdir(parents=True)
 
         # Write output .yaml file
-        dump_all_full_path = os.path.join(dump_all_path, self.model_data.GeneralParameters.magnet_name + '_all_data.yaml')
+        dump_all_full_path = os.path.join(dump_all_path,
+                                          self.model_data.GeneralParameters.magnet_name + '_all_data.yaml')
         # with open(dump_all_full_path, 'w') as outfile:
         #     yaml.dump(all_data_dict, outfile, default_flow_style=False, sort_keys=False)
         dict_to_yaml(all_data_dict, dump_all_full_path, list_exceptions=['Conductors'])
```

### Comparing `steam-sdk-2023.5.4/steam_sdk/builders/BuilderProteCCT.py` & `steam-sdk-2023.6.0/steam_sdk/builders/BuilderProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/builders/BuilderPyBBQ.py` & `steam-sdk-2023.6.0/steam_sdk/builders/BuilderPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/builders/BuilderSIGMA.py` & `steam-sdk-2023.6.0/steam_sdk/builders/BuilderSIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/builders/SelfMutualInductanceCalculation.py` & `steam-sdk-2023.6.0/steam_sdk/builders/SelfMutualInductanceCalculation.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/builders/Solenoids.py` & `steam-sdk-2023.6.0/steam_sdk/builders/Solenoids.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/builders/geometricFunctions.py` & `steam-sdk-2023.6.0/steam_sdk/builders/geometricFunctions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx` & `steam-sdk-2023.6.0/steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx`

 * *Files 17% similar despite different names*

```diff
@@ -177,74 +177,74 @@
 00000b00: dfb6 ce8b 94dc 4e83 48d1 083b dc01 7f46  ......N.H..;...F
 00000b10: 5891 0ada af94 ee9c 1fdf 105b f5f2 6264  X..........[..bd
 00000b20: 32ee 0db3 aa93 befc 71f6 371d 267e 949e  2.......q.7.&~..
 00000b30: 8ed2 d3f3 f4b5 8057 d8d7 a3e4 ebf3 e40d  .......W........
 00000b40: 31bc 9ffa 7131 d3d1 0fd3 c0e5 a907 4a04  1...q1........J.
 00000b50: 5d1b d42f a1ea 597a 9b04 c8e8 f442 142f  ]../..Yz.....B./
 00000b60: 0000 00ff ff03 0050 4b03 0414 0006 0008  .......PK.......
-00000b70: 0000 0021 0026 7b5a 8391 0300 003e 0d00  ...!.&{Z.....>..
+00000b70: 0000 0021 00c7 95ea a591 0300 003e 0d00  ...!.........>..
 00000b80: 0018 0000 0078 6c2f 776f 726b 7368 6565  .....xl/workshee
 00000b90: 7473 2f73 6865 6574 342e 786d 6c94 97db  ts/sheet4.xml...
 00000ba0: 72e2 300c 86ef 7766 df21 93fb 9203 500e  r.0...wf.!....P.
-00000bb0: 0374 4a29 85b6 b4f4 c4ee ad09 0632 4de2  .tJ).........2M.
-00000bc0: 6c6c a07d fb55 120e 91ea 76e0 0688 3e4b  ll.}.U....v...>K
-00000bd0: b6e5 5f8e 685d 7c84 81b1 e689 f445 d436  .._.h]|......E.6
-00000be0: 9d92 6d1a 3cf2 c4cc 8f16 6df3 edb5 7f56  ..m.<.....m....V
-00000bf0: 370d a958 3463 8188 78db fce4 d2bc e8fc  7..X4c..x.......
-00000c00: fed5 da88 e45d 2e39 5706 4488 64db 5c2a  .....].9W.D.d.\*
-00000c10: 1537 2d4b 7a4b 1e32 5912 318f 80cc 4512  .7-KzK.2Y.1...E.
-00000c20: 3205 8fc9 c292 71c2 d92c 730a 03cb b5ed  2.....q..,s.....
-00000c30: 732b 647e 64e6 119a c931 31c4 7cee 7bbc  s+d~d....11.|.{.
-00000c40: 27bc 55c8 2395 0749 78c0 14ac 5f2e fd58  '.U.#..Ix..._..X
-00000c50: eea2 85de 31e1 4296 bcaf e233 4f84 3184  ....1.B....3O.1.
-00000c60: 98fa 81af 3eb3 a0a6 117a cde1 2212 099b  ....>....z.."...
-00000c70: 06b0 ef0f a7c2 bc5d ecec e14b f8d0 f712  .......]...K....
-00000c80: 21c5 5c95 209c 952f f4eb 9e1b 56c3 8248  !.\. ../....V..H
-00000c90: 9dd6 cc87 1da4 6937 123e 6f9b 974e 73e2  ......i7.>o..Ns.
-00000ca0: d8a6 d569 6509 9af8 7c23 0bbf 8d34 df53  ...ie...|#...4.S
-00000cb0: 21de 5330 9cb5 4d1b 4248 1e70 2fdd b9c1  !.S0..M.BH.p/...
-00000cc0: e06b cdaf 7810 40a4 2a1c d9bf 3c68 b5f9  .k..x.@.*...<h..
-00000cd0: b7df cbc3 5afb b89d d6e1 f76e 8e7e 764e  ....Z......n.~vN
-00000ce0: e3c4 98f1 395b 05ea 596c 06dc 5f2c 1588  ....9[..Yl.._,..
-00000cf0: 02e2 653b 6ece 3e7b 5c7a 9077 98be e456  ..e;n.>{\z.w...V
-00000d00: d3c5 7a22 8010 f069 847e 2a20 c81b fbc8  ..z"...i.~* ....
-00000d10: be37 fe4c 2ddb 66dd 2ed5 1cbb 51ae 4114  .7.L-.f.....Q.A.
-00000d20: 6f25 9508 ffe4 c0d9 bae7 8eee d611 beb7  o%..............
-00000d30: 8e95 e31c cb3b c7da ded3 fdd1 d3ca 979c  .....;..........
-00000d40: 65a3 c714 ebb4 12b1 3140 7cb0 7619 b354  e.......1@|.v..T
-00000d50: ca4e d385 75e8 f70c 9b4d 075f c268 4883  .N..u....M._.hH.
-00000d60: 8453 5877 dc7a ad65 ad21 adde 9676 31ad  .SXw.z.e.!...v1.
-00000d70: 637a 8569 03d3 1ea2 0d1b d36b 4c1d 4cfb  cz.i.......kL.L.
-00000d80: 98ba 98de 605a c674 8069 05d3 6191 96ab  ....`Z.t.i..a...
-00000d90: e798 de62 df2a a677 9812 df7b 4c49 2647  ...b.*.w...{LI&G
-00000da0: 9892 4c3e 604a 32f9 88d6 6c93 4c8e 3125  ..L>`J2...l.L.1%
-00000db0: 997c c294 64f2 1953 92c9 971f cff7 15fb  .|..d..S........
-00000dc0: 923c bf61 4a32 39c1 f490 490b 34bc 1732  .<.aJ29...I.4..2
-00000dd0: 68f7 0421 c3e8 bd90 cb36 1532 a654 c86e  h..!.....6.2.T.n
-00000de0: 2e7f 2260 adf5 5a6b ed6b ad37 5aeb 406b  .."`..Zk.k.7Z.@k
-00000df0: 1d6a adb7 5aeb 9dd6 7aaf b58e b4d6 07ad  .j..Z...z.......
-00000e00: f551 6b1d 6bad 4f5a ebb3 d6fa 925b 8934  .Qk.k.OZ.....[.4
-00000e10: 5fb5 d637 ad75 42ad 4828 7077 9e20 1418  _..7.uB.H(pw. ..
-00000e20: 5d10 0aa9 b52e a20e a9b5 ab22 75e9 9dd6  ].........."u...
-00000e30: c394 6cf7 1a53 5289 7d4c 4925 de60 4a6a  ..l..SR.}LI%.`Jj
-00000e40: 6d80 d64c efb4 21f6 2595 788b 29b9 d3ee  m..L..!.%.x.)...
-00000e50: 3025 4575 8f29 29aa 11a6 24cf 0ff8 1448  0%Eu.))...$....H
-00000e60: 9e1f 3125 991c 634a 32f9 84e9 2193 4832  ..1%..cJ2...!.H2
-00000e70: 696f 517c 4966 0d42 bd94 bedd 35ef cb32  ioQ|If.B....5..2
-00000e80: dc0f f9eb 32f5 8366 a020 a18a 7d58 009a  ....2..f. ..}X..
-00000e90: e2fc 2455 c2e8 bd2a 2b36 39ff 2ea6 87f3  ..$U...*+69.....
-00000ea0: 4713 42e7 7042 19c0 e8c2 8444 165d 4cbf  G.B.pB.....D.]L.
-00000eb0: b9a0 d39e faf8 4e03 278d 5ed0 981e b484  ......N.'.^.....
-00000ec0: 76d8 3869 4218 5dd8 212d 7444 0b85 8e26  v.8iB.].!-tD...&
-00000ed0: 8496 f3ab 4e2a df36 92fb a62a 756b 9b78  ....N*.6...*uk.x
-00000ee0: 0aa2 e26e 1afb b03e 87aa 28ef 6df3 ce2e  ...n...>..(.m...
-00000ef0: 660b 3e62 c9c2 8fa4 11f0 79d6 b7a6 524d  f.>b......y...RM
-00000f00: f2ce 16fa 4478 5022 ce9a bfa9 50d0 9d66  ....DxP"....P..f
-00000f10: 3f97 f03f 8543 9767 9780 cf85 50bb 07e8  ?..?.C.g....P...
-00000f20: 78ad fd3f 9fce 7f00 0000 ffff 0300 504b  x..?..........PK
+00000bb0: 43e8 9452 0a6d 69e9 89dd 5b13 0c64 9ac4  C..R.mi...[..d..
+00000bc0: d9d8 40fb f6ab 249c a4ba 1db8 2189 3e4b  ..@...$.....!.>K
+00000bd0: b694 df8e 685d 7c44 a1b1 e2a9 0c44 ec99  ....h]|D.....D..
+00000be0: 4ec9 360d 1efb 621a c473 cf7c 7bed 9dd5  N.6...b..s.|{...
+00000bf0: 4d43 2a16 4f59 2862 ee99 9f5c 9a17 eddf  MC*.OY(b...\....
+00000c00: bf5a 6b91 becb 05e7 ca80 08b1 f4cc 8552  .Zk............R
+00000c10: 49d3 b2a4 bfe0 1193 2591 f018 c84c a411  I.......%....L..
+00000c20: 53f0 98ce 2d99 a49c 4d73 a728 b45c db3e  S...-...Ms.(.\.>
+00000c30: b722 16c4 6611 a199 1e13 43cc 6681 cfbb  ."..f.....C.f...
+00000c40: c25f 463c 5645 9094 874c c1fa e522 48e4  ._F<VE...L..."H.
+00000c50: 365a e41f 132e 62e9 fb32 39f3 4594 4088  6Z....b..29.E.@.
+00000c60: 4910 06ea 330f 6a1a 91df 1ccc 6391 b249  I...3.j.....c..I
+00000c70: 0879 7f38 15e6 6f63 e70f 5fc2 4781 9f0a  .y.8..oc.._.G...
+00000c80: 2966 aa04 e1ac 62a1 5f73 6e58 0d0b 22b5  )f....b._snX..".
+00000c90: 5bd3 0032 c8ca 6ea4 7ce6 9997 4e73 ecd8  [..2..n.|...Ns..
+00000ca0: a6d5 6ee5 051a 077c 2d0f ee8d acde 1321  ..n....|-......!
+00000cb0: de33 3098 7aa6 0d21 240f b99f 656e 30b8  .30.z..!$...en0.
+00000cc0: acf8 150f 4388 5485 57f6 af08 5a6d feed  ....C.T.W...Zm..
+00000cd0: 758b b0d6 2e6e bbb5 bfdf ced1 cbdf d328  u....n.........(
+00000ce0: 35a6 7cc6 96a1 7a16 eb3e 0fe6 0b05 a280  5.|...z..>......
+00000cf0: 7879 c6cd e967 974b 1fea 0ed3 97dc 6ab6  xy...g.K......j.
+00000d00: 585f 8410 027e 8d28 c804 0475 631f f975  X_...~.(...uc..u
+00000d10: 1d4c d5c2 33eb 76a9 e6d8 8d72 0da2 f84b  .L..3.v....r...K
+00000d20: a944 f4a7 00ce c6bd 7074 378e 70dd 3856  .D......pt7.p.8V
+00000d30: 8e73 2c6f 1d6b 3b4f f747 4fab 5872 5e8d  .s,o.k;O.GO.Xr^.
+00000d40: 2e53 acdd 4ac5 da00 f1c1 da65 c232 293b  .S..J......e.2);
+00000d50: 4d17 d6a1 cf19 92cd 065f c268 2883 84b7  M........_.h(...
+00000d60: b06a bbf5 5acb 5a41 59fd 0ded 605a c7f4  .j..Z.ZAY...`Z..
+00000d70: 0ad3 06a6 5d44 1b36 a6d7 983a 98f6 3075  ....]D.6...:..0u
+00000d80: 31bd c1b4 8c69 1fd3 0aa6 8343 5aae 9e63  1....i.....CZ..c
+00000d90: 7a8b 7dab 98de 614a 7cef 3125 951c 624a  z.}...aJ|.1%..bJ
+00000da0: 2af9 8029 a9e4 235a b34d 2a39 c294 54f2  *..)..#Z.M*9..T.
+00000db0: 0953 52c9 674c 4925 5f7e 7cbf afd8 97d4  .SR.gLI%_~|.....
+00000dc0: f90d 5352 c931 a6fb 4a5a a0e1 9d90 41bb  ..SR.1..JZ....A.
+00000dd0: 2708 1946 ef84 5cb6 a990 31a5 4276 0bf9  '..F..\...1.Bv..
+00000de0: 1301 6bad d75a 6b4f 6bbd d15a fb5a eb40  ..k..ZkOk..Z.Z.@
+00000df0: 6bbd d55a efb4 d67b ad75 a8b5 3e68 ad8f  k..Z...{.u..>h..
+00000e00: 5aeb 486b 7dd2 5a9f b5d6 97c2 4aa4 f9aa  Z.Hk}.Z.....J...
+00000e10: b5be 69ad 636a 4542 81b3 f304 a1c0 e803  ..i.cjEB........
+00000e20: a190 bdd6 41d4 217b edea 90ba f44c eb62  ....A.!{.....L.b
+00000e30: 4ad2 bdc6 94ec c41e a664 27de 604a f65a  J........d'.`J.Z
+00000e40: 1fad 999e 6903 ec4b 76e2 2da6 e44c bbc3  ....i..Kv.-..L..
+00000e50: 946c aa7b 4cc9 a61a 624a eafc 80df 02a9  .l.{L...bJ......
+00000e60: f323 a6a4 9223 4c49 259f 30dd 5712 4926  .#...#LI%.0.W.I&
+00000e70: eb2d 0e3f 9279 8350 2f65 5f77 cdf7 b20c  .-.?.y.P/e_w....
+00000e80: e743 f1b9 ccfc a019 3890 50c5 de2f 0f4d  .C......8.P../.M
+00000e90: 717e 922a 61f4 4e95 159b e4d4 c1f4 9b9c  q~.*a.N.........
+00000ea0: a073 3861 1bc0 e883 0989 a43a 98ee 4583  .s8a.......:..E.
+00000eb0: 32cc 7aea e33b 0d5c 34a2 b40e a67b a5a1  2.z..;.\4....{..
+00000ec0: 091b 274d 08a3 0f32 24f2 ec60 ba97 279a  ..'M...2$..`..'.
+00000ed0: 105a ceaf 3aa9 7cdb 48ee 9aaa cccd 33d1  .Z..:.|.H.....3.
+00000ee0: 14f4 2ce9 64b1 f7eb 73a8 8a8a deb6 e8ec  ..,.d...s.......
+00000ef0: 1236 e743 96ce 8358 1a21 9fe5 7d6b 26d5  .6.C...X.!..}k&.
+00000f00: b4e8 6ca1 4f84 0725 92bc f99b 0805 dd69  ..l.O..%.......i
+00000f10: 7ebb 80ff 291c ba3c bb04 7c26 84da 3e40  ~...)..<..|&..>@
+00000f20: c76b edfe f9b4 ff03 0000 ffff 0300 504b  .k............PK
 00000f30: 0304 1400 0600 0800 0000 2100 13c4 2c13  ..........!...,.
 00000f40: c200 0000 4201 0000 2300 0000 786c 2f77  ....B...#...xl/w
 00000f50: 6f72 6b73 6865 6574 732f 5f72 656c 732f  orksheets/_rels/
 00000f60: 7368 6565 7432 2e78 6d6c 2e72 656c 7384  sheet2.xml.rels.
 00000f70: 8fc1 6ac3 3010 44ef 85fc 83d8 7b24 3b87  ..j.0.D.....{$;.
 00000f80: 508a 255f 4a21 d726 fd00 455e dba2 f64a  P.%_J!.&..E^...J
 00000f90: 68b7 25f9 fbe8 d884 428e c363 de30 5d7f  h.%.....B..c.0].
@@ -270,1787 +270,1793 @@
 000010d0: 0bb1 8551 24fd 18c3 7ec4 d9b1 8e09 a990  ...Q$...~.......
 000010e0: 3ee6 d949 8979 30c9 f98b 1bd0 acaa 6a6d  >..I.y0.......jm
 000010f0: f25f 07b4 2f4e b5ef 2ce4 7d57 833a 3d52  ._../N..,.}W.:=R
 00001100: 59fe ec8e 7d1f 3c6e a3bf ce48 f2cf 8449  Y...}.<n...H...I
 00001110: 3990 603e a248 39c8 45ed f280 6241 eb77  9.`>.H9.E...bA.w
 00001120: f69e 6b7d 0e04 a66d cccb f3f6 0900 00ff  ..k}...m........
 00001130: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
-00001140: 000b b47d 7d3f 0600 0075 2000 0018 0000  ...}}?...u .....
+00001140: 00d9 5b05 0c59 0600 0000 2100 0018 0000  ..[..Y....!.....
 00001150: 0078 6c2f 776f 726b 7368 6565 7473 2f73  .xl/worksheets/s
-00001160: 6865 6574 322e 786d 6c94 5adf 739b 3810  heet2.xml.Z.s.8.
-00001170: 7ebf 99fb 1f18 de1b 8c04 8ee3 89d3 699d  ~.............i.
-00001180: e95c 1f6e e6a6 bd1f cf04 cb31 53b0 3820  .\.n.......1S.8 
-00001190: 49db bffe 7685 0dab 059d ad87 d636 fbb1  I...v........6..
-000011a0: ab95 f6fb 56a0 dcbf ff5e 95c1 ab6a da42  ....V....^...j.B
-000011b0: 1f37 617c b308 0375 ccf5 ae38 3e6f c2bf  .7a|...u...8>o..
-000011c0: fefc f46e 1506 6d97 1d77 59a9 8f6a 13fe  ...n..m..wY..j..
-000011d0: 506d f8fe e1d7 5fee df74 f3ad 3d28 d505  Pm...._..t..=(..
-000011e0: e0e1 d86e c243 d7d5 eb28 6af3 83aa b2f6  ...n.C...(j.....
-000011f0: 46d7 ea08 96bd 6eaa ac83 9fcd 73d4 d68d  F.....n.....s...
-00001200: ca76 e6a6 aa8c c462 b18c aaac 3886 bd87  .v.....b....8...
-00001210: 7573 8d0f bddf 17b9 7ad4 f94b a58e 5def  us......z..K..].
-00001220: a451 65d6 c1f8 db43 51b7 676f 557e 8dbb  .Qe....CQ.goU~..
-00001230: 2a6b bebd d4ef 725d d5e0 e2a9 288b ee87  *k....r]....(...
-00001240: 711a 0655 befe fc7c d44d f654 42de dfe3  q..U...|.M.TB...
-00001250: 24cb cfbe cd8f 89fb aac8 1bdd ea7d 7703  $............}w.
-00001260: eea2 7ea0 d39c efa2 bb08 3c3d dcef 0ac8  ..~.......<=....
-00001270: 00a7 3d68 d47e 137e 88d7 dbe5 2a8c 1eee  ..=h.~.~....*...
-00001280: cd04 fd5d a8b7 967c 0f70 be9f b4fe 8686  ...]...|.p......
-00001290: cfbb 4db8 0017 ad2a 558e 9907 197c bcaa  ..M....*U....|..
-000012a0: ad2a cb4d f851 c022 b6ff 1aaf f81d 5c46  .*.M.Q."......\F
-000012b0: 834f fafd ecff 9359 a33f 9a60 a7f6 d94b  .O.....Y.?.`...K
-000012c0: d97d d16f bfa9 e2f9 d041 41a4 9033 a6be  .}.o.....AA..3..
-000012d0: defd 7854 6d0e 730e a16f 448a 5e73 5d82  ..xTm.s..oD.^s].
-000012e0: 0bf8 3fa8 0a2c 1e98 b3ec bbf9 7c2b 76dd  ..?..,......|+v.
-000012f0: 6113 ae16 37b7 f1e2 4ede 8297 fca5 ed74  a...7...N......t
-00001300: f54f 6f88 4fb7 f737 8ad3 8df0 79ba 31b9  .Oo.O..7....y.1.
-00001310: ee46 798e 08a1 4f77 8aff bd33 ea87 6c66  .Fy...Ow...3..lf
-00001320: e331 ebb2 87fb 46bf 0550 78e0 a0ad 332c  .1....F..Px...3,
-00001330: e378 0d5e e753 865c 11fb 01c1 e616 988b  .x.^.S.\........
-00001340: 1696 e1f5 410a 711f bdc2 dce6 f00f 5c0e  ....A.q.......\.
-00001350: 7e21 a5eb fd02 78f0 18af 5683 4713 f5a3  ~!....x...V.G...
-00001360: 6dbd 9b8f 97f8 c443 30cf 2399 f70b 0b78  m......C0.#....x
-00001370: 7d1e 001e f3b8 5bb0 3c6c 6b3c 1f6f e913  }.....[.<lk<.o..
-00001380: 0fc0 24de b812 fdbc d956 391f efd6 271e  ..$......V9...'.
-00001390: 8049 bc71 c6fa 78b6 359d 8f87 aa7a 75bd  .I.q..x.5....zu.
-000013a0: 0198 c45b b2f9 b4ad b7f3 f1ee 7ce2 0198  ...[........|...
-000013b0: c4e3 7568 5b1d 7518 a304 5d4f 2840 0f11  ..uh[.u...]O(@..
-000013c0: a12f b00c d119 313b 4a26 f6e3 30a0 894f  ./....1;J&..0..O
-000013d0: 5e34 e88c 981d 5513 7bd1 1bd1 83cf 649a  ^4....U.{.....d.
-000013e0: a56d 7665 09ea e431 b180 1e43 0a5e aab1  .mve...1...C.^..
-000013f0: 6d76 85f4 223f 760c 5015 ca72 29c6 f9eb  mv.."?v.P..r)...
-00001400: 3972 0249 d306 5053 b7f4 8aa5 a0b1 9714  9r.I..PS........
-00001410: 18f4 26a4 79c9 78e4 e029 3aba e420 46ab  ..&.y.x..):.. F.
-00001420: ede0 09db 2795 f498 6a05 acd9 855e 41e5  ....'...j....^A.
-00001430: 402c 262b 609b 1d6a 1153 b9b8 1c92 2a82  @,&+`..j.S....*.
-00001440: 5870 bd40 67a4 b41d 8211 53c5 b81c 928a  Xp.@g.....S.....
-00001450: 8258 70c9 4067 24a4 4333 ccb6 e5ac 1917  .Xp.@g$.C3......
-00001460: 4322 9a94 3627 3033 3b08 2c28 812f 8744  C"..6'03;.,(./.D
-00001470: 346b 98d2 950c e5e9 65cf b460 45cc 0550  4k......e..`E..P
-00001480: d866 074f 056d fe97 4302 7a5c 9378 327f  .f.O.m..C.z\.x2.
-00001490: b6d9 357f 541a 2e87 a4a2 2062 ce05 d854  ..5.T..... b...T
-000014a0: d211 39b8 20bc e867 d07c 8fe3 f2ec c532  ..9. ..g.|.....2
-000014b0: 4169 2457 e39a 9c76 6b16 cbe2 9184 f6f6  Ai$W...vk.......
-000014c0: d08b 6582 d248 ae26 4b66 b12c 7610 5bd2  ..e..H.&Kf.,v.[.
-000014d0: ce7c 71c9 103d 5489 5c71 1db7 cc22 1e79  .|q..=T.\q...".y
-000014e0: 6f65 2969 67be 1c92 b65e b9e2 5582 ce48  oe)ig....^..U..H
-000014f0: dd3a e827 bd88 8d68 9225 ef17 9659 8891  .:.'...h.%...Y..
-00001500: 9d76 965e 9d59 5a2d 6ac5 45da 320b e160  .v.^.YZ-j.E.2..`
-00001510: bcf4 daee 237a 9c39 f2c4 d257 2c33 3b18  ....#z.9...W,3;.
-00001520: 2fbd 3603 8826 2127 6b69 9b1d bc94 5e3b  /.6..&!'ki....^;
-00001530: 0044 9390 9389 b5cd 2e92 783d 0f48 44f3  .D........x=.HD.
-00001540: fdc4 842a 7320 3621 dbc1 13df 7448 af07  ...*s 6!....tH..
-00001550: 0644 937a e6ed c432 0be1 62ad d733 83b4  .D.z...2..b..3..
-00001560: c447 8cb4 3c15 9765 960e 0a25 5e4f 0d88  .G..<..e...%^O..
-00001570: 1e57 5a72 0566 66c7 037a e2f5 d480 e871  .WZr.ff..z.....q
-00001580: 626f 7996 9659 4807 8512 aa4d 175f 3620  boy..YH....M._6 
-00001590: 9a84 e45b 2bcb 2ca4 e3f1 3df1 d226 4493  ...[+.,...=..&D.
-000015a0: 89e5 72c8 cc8e d696 f8bd 8ab0 b449 8eb4  ..r..........I..
-000015b0: eccb 079d 9111 392a 36f1 d226 4493 899d  ......9*6..&D...
-000015c0: 84b4 b4c9 b5cd 4bbc b4c9 a06d a110 0967  ......K....m...g
-000015d0: e72c 8815 f776 0071 a148 bc94 cba0 b972  .,...v.q.H.....r
-000015e0: 4d88 34a7 5c6c f3b1 1d3c 4d06 e4a5 5c89  M.4.\l...<M...\.
-000015f0: b56d 4af8 1687 995d 04f3 52ae c492 a684  .mJ....]..R.....
-00001600: f728 6676 f4a8 d44b b910 3d96 5ec2 4bcf  .(fv...K..=.^.K.
-00001610: 328b c441 b0d4 4bb9 104d 4272 19b1 cc82  2..A..K..MBr....
-00001620: 8cc8 dae2 a45e 3262 d07c efed 4ac6 4b2d  .....^2b.|..J.K-
-00001630: 524b 0e92 4932 b6d9 b145 4cfd de69 5a72  RK..I2...EL..iZr
-00001640: 904e 5e6a da66 c77e 2df5 520b 4493 259b  .N^j.f.~-.R.D.%.
-00001650: 84b4 7632 a9a3 bfa5 5e7a 80e8 5167 53be  ..v2....^z..QgS.
-00001660: 8761 66d7 bb62 2fc6 a794 f149 3c09 699b  .af..b/....I<.i.
-00001670: 5d21 bd18 9f5a 8c4f 797f 6366 47c5 2ebd  ]!...Z.Oy.cfG...
-00001680: 188f 6832 b19c f1cc ece8 6f4b 2fc6 1b34  ..h2......oK/..4
-00001690: 6a3b 9ed4 e03b b68f 932b 5b7a c562 fad2  j;...;...+[z.b..
-000016a0: 6b8f 62d0 fc9d df24 c7fe ed09 79e7 77ba  k.b....$....y.w.
-000016b0: cd5c b1a3 7be9 cc12 d1ac aba6 7c6b 3607  .\..{.......|k6.
-000016c0: 5a32 4a6d 0710 6f62 4b2f 7932 68d6 5527  Z2Jm..obK/y2h.U'
-000016d0: 7d65 16c4 4a71 3b80 2603 f212 af65 ff4e  }e..Jq;.&....e.N
-000016e0: d67a e44c 27eb 3307 62d2 ba1d 3c4d 06e4  .z.L'.3.b...<M..
-000016f0: 7762 33f3 0676 ba64 33a0 e992 9d41 9301  wb3..v.d3....A..
-00001700: 7909 dff2 bcc7 19c9 c2af 6c29 c62e 572f  y.........l)..W/
-00001710: c183 43de be5c c750 fc0a 1e04 0f98 3e54  ..C..\.P......>T
-00001720: 7f82 db9f 59d6 d9b3 fa3d 6b9e 8b63 1b94  ....Y....=k..c..
-00001730: 6a0f ba02 879e b07a 4d7f 66db ffe8 746d  j......zM.f...tm
-00001740: 7aef 93ee e0dc d57c 3dc0 e9bb 0221 58dc  z......|=....!X.
-00001750: 0078 af75 77fe 0123 419f 5f55 f752 0775  .x.uw..#A._U.R.u
-00001760: 56ab e66b f113 0ebd 4127 7553 c099 af39  V..k....A'uS...9
-00001770: 5edf 84b5 6eba 262b ba30 38c0 f59f 1a0c  ^...n.&+.08.....
-00001780: e563 5d40 a92f 40df e0af 08ba 223f 5d81  .c]@./@....."?].
-00001790: dfcd bad8 6dc2 e6f3 ce9c f646 c31f 0c3c  ....m......F...<
-000017a0: fc07 0000 ffff 0300 504b 0304 1400 0600  ........PK......
-000017b0: 0800 0000 2100 8112 9d2b 9402 0000 f308  ....!....+......
-000017c0: 0000 1800 0000 786c 2f77 6f72 6b73 6865  ......xl/workshe
-000017d0: 6574 732f 7368 6565 7433 2e78 6d6c 9456  ets/sheet3.xml.V
-000017e0: cb8e a330 10bc afb4 ff80 7c9f 18f2 4e14  ...0......|...N.
-000017f0: 18cd 281a ed1c 565a adf6 7176 8c01 2b18  ..(...VZ..qv..+.
-00001800: 23db 79cc df6f 1b92 0c38 6105 9710 54dd  #.y..o...8a...T.
-00001810: 55ee a6e8 66f3 7c16 b977 644a 7359 8428  U...f.|..wdJsY.(
-00001820: 18f9 c863 0595 312f d210 fdfe f5f6 b444  ...c..1/.......D
-00001830: 9e36 a488 492e 0b16 a20f a6d1 73f4 f5cb  .6..I.......s...
-00001840: e624 d55e 678c 190f 180a 1da2 cc98 728d  .$.^g.........r.
-00001850: b1a6 1913 448f 64c9 0a40 12a9 0431 70ab  ....D.d..@...1p.
-00001860: 52ac 4bc5 485c 2589 1c8f 7d7f 8e05 e105  R.K.H\%...}.....
-00001870: aa19 d6aa 0f87 4c12 4ed9 56d2 8360 85a9  ......L.N.V..`..
-00001880: 4914 cb89 81f3 eb8c 97fa ca26 681f 3a41  I..........&h.:A
-00001890: d4fe 503e 5129 4aa0 d8f1 9c9b 8f8a 1479  ..P>Q)J........y
-000018a0: 82ae dfd3 422a b2cb a1ee 7330 25f4 ca5d  ....B*....s0%..]
-000018b0: dddc d10b 4e95 d432 3123 a0c3 f541 ef6b  ....N..21#...A.k
-000018c0: 5ee1 1506 a668 1373 a8c0 b6dd 532c 09d1  ^....h.s....S,..
-000018d0: 4bb0 7e0d 2608 479b aa41 7f38 3be9 c67f  K.~.&.G..A.8;...
-000018e0: cff6 7b27 e5de 02ef 7188 7c1b 8aef 62df  ..{'....q.|...b.
-000018f0: aa7e ff50 5ecc 1272 c8cd 4f79 fac6 789a  .~.P^..r..Oy..x.
-00001900: 1978 b833 38bf 2d63 1d7f 6c99 a6d0 3fa0  .x.38.-c..l...?.
-00001910: 198d 6796 89ca 1ce4 e0d7 13dc 1a01 ea27  ..g............'
-00001920: e7ea 7ae2 b1c9 42b4 f447 8bc0 5f4d 16c0  ..z...B..G.._M..
-00001930: 420f da48 f1b7 0682 4b7a 9d38 be24 c2f5  B..H....Kz.8.$..
-00001940: 9238 ed97 38b9 24c2 f592 38fe 6f22 ae4f  .8..8.$...8.o".O
-00001950: 5c35 604b 0c89 364a 9e3c f010 1c5d 97c4  \5`K..6J.<...]..
-00001960: 3a32 58c3 291e 570c a5da d817 0886 2668  :2X.).W.......&h
-00001970: 781c c768 3c0f 36f8 084d a517 f4b5 8d8e  x..h<.6..M......
-00001980: 6f28 06a9 9b1e 68f4 d783 e086 dec4 d16b  o(....h........k
-00001990: a3d3 c77a d0a0 fe7a 10dc d09b 397a 6d74  ...z...z....9zmt
-000019a0: fe58 6f3a 440f 821b 7a0b 47af 8d2e 1feb  .Xo:D...z.G.....
-000019b0: 81bf fad7 07c1 0dbd 95a3 d742 17fe 63bd  ...........B..c.
-000019c0: f910 3d08 fed4 5bb8 7e69 a31d 7e59 0cd1  ..=...[.~i..~Y..
-000019d0: 83e0 869e eb97 36da e117 3bc0 7bbf 0f10  ......6...;.{...
-000019e0: dcd0 73fd d246 3bfc b21a a207 c10d 3dd7  ..s..F;.......=.
-000019f0: 2f6d b4c3 2f01 acac 012f 3c44 3714 5dc7  /m../..../<D7.].
-00001a00: 58b2 4f78 d961 9960 d88c 698d 91e5 dd90  X.Ox.a.`..i.....
-00001a10: 69c3 1dae 0906 8d19 1bdd 28c3 f58d 0377  i.........(....w
-00001a20: 1807 b6d1 90c6 b686 c9d2 b58e 256b 9cc8  ............%k..
-00001a30: f54e bdc8 ea39 5e92 947d 272a e585 f672  .N...9^..}'*...r
-00001a40: 9654 4bca 6e1d 55af 31d8 0af6 bd96 6535  .TK.n.U.1.....e5
-00001a50: ea77 d2c0 2aaa fe66 f071 c160 a8fb 23c0  .w..*..f.q.`..#.
-00001a60: 1329 cdf5 c62e cadb e74a f40f 0000 ffff  .).......J......
-00001a70: 0300 504b 0304 1400 0600 0800 0000 2100  ..PK..........!.
-00001a80: f24d a6d1 562b 0000 182f 0100 1800 0000  .M..V+.../......
-00001a90: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
-00001aa0: 6565 7431 2e78 6d6c 9cdd 5973 1b47 a267  eet1.xml..Ys.G.g
-00001ab0: f1f7 8998 efa0 e0fb 5804 7739 2cdf 2862  ........X.w9,.(b
-00001ac0: e1be ef7c 6353 b4cd 6849 d490 6cbb 7b3e  ...|cS..hI..l.{>
-00001ad0: fdfc 8b14 89aa fc15 4ca1 1fee 6d3b eb00  ........L...m;..
-00001ae0: 05e0 6465 8294 8fea 97ff f9f7 97cf effe  ..de............
-00001af0: bcb9 7fb8 bdfb fa71 a6f7 d3ec ccbb 9baf  .......q........
-00001b00: d777 9f6e bffe fe71 e6e4 78f4 7f56 66de  .w.n...q..x..Vf.
-00001b10: 3d3c 5e7d fd74 f5f9 eeeb cdc7 99ff dc3c  =<^}.t.........<
-00001b20: ccfc cfaf fffb 7ffd f2d7 ddfd 3f1f feb8  ............?...
-00001b30: b979 7c97 67f8 faf0 71e6 8fc7 c76f 3fbf  .y|.g...q....o?.
-00001b40: 7fff 70fd c7cd 97ab 879f eebe dd7c cd91  ..p..........|..
-00001b50: dfee eebf 5c3d e65f ef7f 7fff f0ed fee6  ....\=._........
-00001b60: ead3 d383 be7c 7e3f 373b bbf4 fecb d5ed  .....|~?7;......
-00001b70: d799 e767 f8f9 fe47 9ee3 eeb7 df6e af6f  ...g...G.....n.o
-00001b80: 0677 d7ff fa72 f3f5 f1f9 49ee 6f3e 5f3d  .w...r....I.o>_=
-00001b90: e6f5 3ffc 71fb ede1 e5d9 be5c ffc8 d37d  ..?.q......\...}
-00001ba0: b9ba ffe7 bfbe fd9f ebbb 2fdf f214 ffb8  ........../.....
-00001bb0: fd7c fbf8 9fa7 279d 79f7 e5fa e78d dfbf  .|....'.y.......
-00001bc0: dedd 5ffd e373 def7 bf7b 0b57 d72f cffd  .._..s...{.W./..
-00001bd0: f42f 3cfd 97db ebfb bb87 bbdf 1e7f cad3  ./<.............
-00001be0: bd7f 7ea1 bee7 0fef 3fbc cf33 fdfa cba7  ..~.....?..3....
-00001bf0: dbbc 83fa 637f 777f f3db c799 aaf7 73d5  ....c.w.......s.
-00001c00: dfef 2d2c cfbc fff5 97a7 cfe8 f4f6 e6af  ..-,............
-00001c10: 87c6 3fbf 7bbc fac7 d1cd e79b ebc7 9b4f  ..?.{..........O
-00001c20: 5135 f3ee f1ee dbf6 cd6f 8ffd 9bcf 9feb  Q5.......o......
-00001c30: c7f7 a2aa b6f2 8fbb bb7f d68f dd08 359b  ..............5.
-00001c40: 133d 3c3d a63e d1d5 f5e3 ed9f 372f fcfc  .=<=.>......7/..
-00001c50: 72d4 fedf ef27 9f5f feb9 eacd afd4 277f  r....'._......'.
-00001c60: ff7a f6e6 3fbf bc92 d193 d0fd fb77 9f6e  .z..?........w.n
-00001c70: 7ebb fad7 e7c7 c3bb bfd6 6f6e 7fff e331  ~.........on...1
-00001c80: 2f69 311f 50fd 39fd fce9 3f83 9b87 eb08  /i1.P.9...?.....
-00001c90: ca2b f869 6eb1 7ed6 ebbb cf79 8afc ff77  .+.in.~....y...w
-00001ca0: 5f6e eb99 960f f8ea df4f fffb d7ed a7c7  _n.......O......
-00001cb0: 3f3e ceac ccfe b4dc 9bfd 30bf 9c67 b9fe  ?>........0..g..
-00001cc0: d7c3 e3dd 97b3 e703 bdef 0f7f 7ee0 dcf7  ............~...
-00001cd0: 07e6 7fbf 3f70 e1c7 1e38 fffd 81cb cb99  ....?p...8......
-00001ce0: e3df 1f3a f7b7 0f7d fffc 9a9f 3e8e c1d5  ...:...}....>...
-00001cf0: e3d5 afbf dcdf fdf5 2ed3 342f fee1 db55  ..........4/...U
-00001d00: 3de9 7b3f e769 9fde fbca 4ff5 0bef 78fb  =.{?.i....O...x.
-00001d10: f351 705d 3faa aa1f f671 262f 3c1f cb43  .Qp]?....q&/<..C
-00001d20: 46ff fc75 7eae f7cb fb3f f331 5fe7 fff2  F..u~....?.1_...
-00001d30: e4af 6708 d43c 43f7 a7fa f2bc cd67 9c7d  ..g..<C......g.}
-00001d40: 7dbe a773 ae36 8f4d 3857 dec1 8f9f 2bf0  }..s.6.M8W....+.
-00001d50: ebab 9f2b ced5 3c36 dffd be16 a639 570d  ...+..<6.....9W.
-00001d60: 7f9c 693e eb42 7146 89c5 36d1 7f21 ea79  ..i>.BqF..6..!.y
-00001d70: ddfc 8097 fe3b 85f5 c33e cee4 49c7 0ae7  .....;...>..I...
-00001d80: 97bb df6a 7d75 3526 c9df 2b0c fcfa 8cbd  ...j}u5&..+.....
-00001d90: b1a7 6787 ad83 e30f bdf5 7eea 65fa 87cf  ..g.......~.e...
-00001da0: 1678 7cb6 b1a9 e7b3 b50e 8e3f f0d6 d93e  .x|........?...>
-00001db0: 4c73 b6c0 e3b3 157e 565b 0797 ba3f c95e  Ls.....~V[...?.^
-00001dc0: 2ed8 1f7f 7335 3d3e df58 cef3 bb6b 1f5d  ....s5=>.X...k.]
-00001dd0: 9970 c2e2 02ff 7b77 bd7a 297e b9a2 7b1f  .p....{w.z)~..{.
-00001de0: 8a29 da3a 3a37 be3c 5b9f 676f aaeb bda6  .).::7.<[.go....
-00001df0: c717 6139 5bda 4727 4c97 de54 177d 4d8f  ..a9[.G'L..T.}M.
-00001e00: 27fc 6279 ddb7 0ecf 4db8 f27b 535d fa35  '.by....M..{S].5
-00001e10: 3d7e 8be5 65df 3e3a 9e52 edcf 34cb f114  =~..e.>:.R..4...
-00001e20: b326 f4f8 84e3 89f8 7dd6 b48e 4eb8 e07b  .&......}...N..{
-00001e30: c59a f2c6 ac09 ddf8 4cb1 d83c 3c37 699e  ........L..<<7i.
-00001e40: 36d7 984c 8a37 ced8 5c47 e617 3863 f3f0  6..L.7..\G..8c..
-00001e50: dc78 1ab7 3fd4 e63a f3f6 199b 6bc9 fc02  .x..?..:....k...
-00001e60: 9f6a ebf0 a44b a3b9 d6bc 7dc6 e67a 32cf  .j...K....}..z2.
-00001e70: 5b6c 1d9d 7069 cc35 579b 374f 58d3 8dbd  [l..pi.5W.7OX...
-00001e80: a0dc 7d5b 4727 2ca6 73cd d5e6 ed13 3657  ..}[G',.s.....6W
-00001e90: 9bf9 7239 ad9f 6bfc 7226 aca7 73cd d5e6  ..r9..k.r&..s...
-00001ea0: ed13 b6be b094 eb69 fd5c e313 4e98 a773  .......i.\..N..s
-00001eb0: cdd5 e6ed 13b6 569b 723d ad9f ebf5 840b  ......V.r=......
-00001ec0: 1326 cd5c 73b1 79fb 84cd c586 eba2 7eae  .&.\s.y.......~.
-00001ed0: f109 274d 9ae6 62f3 f609 9bcb c942 b901  ..'M..b......B..
-00001ee0: e7fb 72e3 8493 264d 73b1 79fb 84cd d564  ..r...&Ms.y....d
-00001ef0: 8149 d33a 3a69 d24c b5d6 cc35 1793 0526  .I.::i.L...5...&
-00001f00: 4deb e8a4 4933 d552 33d7 5c4b 1698 34cd  M...I3.R3.\K..4.
-00001f10: a38b 9326 cd54 2bcd 5c73 2d59 2c57 9af6  ...&.T+.\s-Y,W..
-00001f20: d109 9366 7eaa 95a6 a65f e7e1 6239 69da  ...f~...._..b9i.
-00001f30: 4727 4c9a f9a9 569a 9a1e 9fb0 9c34 eda3  G'L...V......4..
-00001f40: 1326 cdfc 542b 4d4d 8f4f 584e 9af6 d109  .&..T+MM.OXN....
-00001f50: 9366 7eaa 95a6 a6c7 272c 274d ebe8 d284  .f~.....','M....
-00001f60: 4933 3fd5 4a53 d3af 275c 2a27 4dfb e8a4  I3?.JS..'\*'M...
-00001f70: 4933 d54a 33df 5c4b f2a3 75f9 135b fbf0  I3.J3.\K..u..[..
-00001f80: a469 33d5 5a33 dffa 62b3 5c6e faed c32b  .i3.Z3..b.\n...+
-00001f90: 13be 4b3d fd6e e2e5 e799 3797 b79a 1e6f  ..K=.n....7....o
-00001fa0: 423d 664e fbf0 a4a9 33d5 7a93 5f95 344e  B=fN....3.z._.4N
-00001fb0: b9cc e5d8 3adc f8a1 a0f5 6d6a 7eaa 15a7  ....:.....mj~...
-00001fc0: a61b df18 3965 fbcb cd84 f9ba 30d5 9af3  ....9e......0...
-00001fd0: 447f 9c69 195d 2aaf 93ef 50eb 435e 9e74  D..i.]*...P.C^.t
-00001fe0: faa9 56a0 85e7 df98 b427 5479 d57c 87da  ..V......'Ty.|..
-00001ff0: a79f 70f1 2c4c b51e d5f4 f803 ffc0 2f1f  ..p.,L......../.
-00002000: da5f 7d26 4cab 85a9 56a4 9a6e 9cb2 bc5e  ._}&L...V..n...^
-00002010: 8bc3 933e e4a9 d6a4 85d6 6f33 3e94 d76b  ...>......o3>..k
-00002020: fbf0 ca84 9f0b 16a6 5a95 6aba f12e cbeb  ........Z.j.....
-00002030: b538 3ce1 d756 0b53 ad4a 35dd 38e5 58d6  .8<..V.S.J5.8.X.
-00002040: f30f 78c5 e149 d367 aaef 40f9 556e f394  ..x..I.g..@.Un..
-00002050: 5c36 edc3 937e 61d6 5c22 f21e 7ef4 778d  \6...~a.\"..~.w.
-00002060: 0bf5 e38a df54 2d4c 785b 8bcd 3521 e7f8  .....T-Lx[..5!..
-00002070: fb1f 236b 7abc 8795 33b4 7d74 c2d7 82c5  ..#kz...3.}t....
-00002080: e62a f0f6 099b df43 96ca c952 3fd7 f8e5  .*.....C...R?...
-00002090: 4cb8 0817 9bd7 fddb 276c 5ed8 2c77 f573  L.......'l^.,w.s
-000020a0: bd9e 70d2 3ab7 d8bc eadf 3e61 f3aa 5f2e  ..p.:.....>a.._.
-000020b0: 17b8 fab9 c627 9ce4 b079 014e 314f 16eb  .....'...y.N1O..
-000020c0: c7b5 e7c9 d284 a9b8 d8bc e0de 7e4f cd0b  ............~O..
-000020d0: aef1 94cf d75b fd5c 636b 13be 772c 3677  .....[.\ck..w,6w
-000020e0: e469 de53 fdb8 f2b7 b493 6646 717d bd31  .i.S......fFq}.1
-000020f0: f79b 7b2c 9bfe 62eb e884 37b5 34d5 c556  ..{,..b...7.4..V
-00002100: d363 f7e5 c5d6 3e3a e162 5b9a ea62 7ba2  .c....>:.b[..b{.
-00002110: dbbf 745f 2e2f b92e a658 50fb af4c fd47  ..t_./...XP..L.G
-00002120: 3ff5 9f7e 0c18 1932 326a 8eb4 7f5d 3fd5  ?..~...22j...]?.
-00002130: 05bc 54d3 c59b 2897 df0e 66a5 f8c3 93fe  ..T...(...f.....
-00002140: 2b33 7e13 2fcf fc32 3284 1935 47da 6f62  +3~./..22..5G.ob
-00002150: aa45 61a9 a6eb 37f1 72aa 5546 fa8c 0c18  .Ea...7.r.UF....
-00002160: 1932 326a 8eb4 5f60 f38b c314 17dc d2f3  .22j.._`........
-00002170: 9fb2 b4be 4834 7e67 f97c c97f 87c6 efa7  ....H4~g.|......
-00002180: cfc8 8091 2123 a3e6 48fb d537 97c0 a73f  ....!#..H..7...?
-00002190: e5fb fb8b 79e9 79e9 6bae ae1f ca2f d55d  ....y.y.k..../.]
-000021a0: 4cf1 3db0 ffca 8c67 c9cb 338f 6749 3932  L.=....g..3.gI92
-000021b0: 6a3e aafd 369a cbec 8fbc 8d9a 6f4f f60f  j>..6.......oO..
-000021c0: 2c14 1d4c f145 afbf f4c2 8cdf 4639 3284  ,..L.E......F92.
-000021d0: 1931 b2c6 c83a 231b 8c6c 32b2 c5c8 3623  .1...:#..l2...6#
-000021e0: 3b8c ec32 b2c7 c83e 2307 8c1c 3272 c4c8  ;..2...>#...2r..
-000021f0: 3123 278c 9c32 72c6 c839 2317 8c5c 3252  1#'..2r..9#..\2R
-00002200: 550e ad3a a4d6 6a20 a5d8 4ab3 956a 2bdd  U..:..j ..J..j+.
-00002210: 56ca adb4 5ba9 b7d2 6fa5 e04a c395 8a2b  V...[...o..J...+
-00002220: 1d57 4aae b45c a9b9 d273 a5e8 4ad3 95aa  .WJ..\...s..J...
-00002230: 2b5d 57ca aeb4 bdaa ed55 6daf 6a7b 55db  +]W......Um.j{U.
-00002240: abda 5ed5 f6aa b657 b5bd aaed 556d af6a  ..^....W....Um.j
-00002250: 7b55 dbab da5e d5f6 aab6 57b5 bdaa ed55  {U...^....W....U
-00002260: 6daf 6a7b 55db abda 5ed5 f6aa b657 b5bd  m.j{U...^....W..
-00002270: aaed 556d f7b5 ddd7 765f db7d 6df7 b5dd  ..Um....v_.}m...
-00002280: d776 5fdb 7d6d f7b5 ddd7 765f db7d 6df7  .v_.}m....v_.}m.
-00002290: b5dd d776 5fdb 7d6d f7b5 ddd7 765f db7d  ...v_.}m....v_.}
-000022a0: 6df7 b5dd d776 5fdb 7d6d f7b5 ddd7 f640  m....v_.}m.....@
-000022b0: db03 6d0f 3a36 686d 0fb4 3dd0 f640 db03  ..m.:6hm..=..@..
-000022c0: 6d0f b43d d0f6 40db 036d 0fb4 3dd0 f640  m..=..@..m..=..@
-000022d0: db03 6d0f b43d d0f6 40db 036d 0fb4 3dd0  ..m..=..@..m..=.
-000022e0: f640 db03 6d0f b43d d0f6 50db 436d 0fb5  .@..m..=..P.Cm..
-000022f0: 3dd4 f650 db43 6d0f b53d d4f6 50db 436d  =..P.Cm..=..P.Cm
-00002300: 0fb5 3dd4 f650 db43 6d0f b53d d4f6 50db  ..=..P.Cm..=..P.
-00002310: 436d 0fb5 3dd4 f650 db43 6d0f b53d d4f6  Cm..=..P.Cm..=..
-00002320: 50db 436d 8fb4 3dd2 f648 db23 6d8f 3abe  P.Cm..=..H.#m.:.
-00002330: 7e6b 7ba4 ed91 b647 da1e 697b a4ed 91b6  ~k{....G..i{....
-00002340: 47da 1e69 7ba4 ed91 b647 da1e 697b a4ed  G..i{....G..i{..
-00002350: 91b6 47da 1e69 7ba4 ed91 b647 da1e 697b  ..G..i{....G..i{
-00002360: 4ddb 6bda 5ed3 f69a b6d7 b4bd d6f1 d396  M.k.^...........
-00002370: b6d7 b4bd a6ed 356d af69 7b4d db6b da5e  ......5m.i{M.k.^
-00002380: d3f6 9ab6 d7b4 bda6 ed35 6daf 697b 4ddb  .........5m.i{M.
-00002390: 6bda 5ed3 f69a b6d7 b4bd a6ed 356d af6b  k.^.........5m.k
-000023a0: 7b5d dbeb da5e d7f6 bab6 d7b5 bdae ed75  {]...^.........u
-000023b0: 6daf 6b7b 5ddb ebda 5ed7 f6ba b6d7 b5bd  m.k{]...^.......
-000023c0: aeed 756d af6b 7b5d dbeb da5e d7f6 bab6  ..um.k{]...^....
-000023d0: d7b5 bdae ed75 6daf 6b7b 5ddb 1bda ded0  .....um.k{].....
-000023e0: f686 b637 b4bd a1ed 0d6d 6f68 7b43 db1b  ...7.....moh{C..
-000023f0: dade d0f6 86b6 37b4 bda1 ed0d 6d6f 687b  ......7.....moh{
-00002400: 43db 1bda ded0 f686 b637 b4bd a1ed 0d6d  C........7.....m
-00002410: 6f68 7b43 db1b dade d0f6 a6b6 37b5 bda9  oh{C........7...
-00002420: ed4d 6d6f 6a7b 53db 9bda ded4 f6a6 b637  .Mmoj{S........7
-00002430: b5bd a9ed 4d6d 6f6a 7b53 db9b dade d4f6  ....Mmoj{S......
-00002440: a6b6 37b5 bda9 ed4d 6d6f 6a7b 53db 9bda  ..7....Mmoj{S...
-00002450: ded4 f6a6 b637 b5bd a5ed 2d6d 6f69 7b4b  .....7....-moi{K
-00002460: db5b dade d2f6 96b6 b7b4 bda5 ed2d 6d6f  .[...........-mo
-00002470: 697b 4bdb 5bda ded2 f696 b6b7 b4bd a5ed  i{K.[...........
-00002480: 2d6d 6f69 7b4b db5b dade d2f6 96b6 b7b4  -moi{K.[........
-00002490: bda5 ed2d 6d6f 6b7b 5bdb dbda ded6 f6b6  ...-mok{[.......
-000024a0: b6b7 b5bd aded 6d6d 6f6b 7b5b dbdb 1dbf  ......mmok{[....
-000024b0: 18d7 f6b6 b6b7 b5bd aded 6d6d 6f6b 7b5b  ..........mmok{[
-000024c0: dbdb dade d6f6 b6b6 b7b5 bdad ed6d 6d6f  .............mmo
-000024d0: 6b7b 5bdb 3bda ded1 f68e b677 b4bd a3ed  k{[.;......w....
-000024e0: 1d6d ef68 7b47 db3b dade d1f6 8eb6 773a  .m.h{G.;......w:
-000024f0: fe1c 44db 3bda ded1 f68e b677 b4bd a3ed  ..D.;......w....
-00002500: 1d6d ef68 7b47 db3b dade d1f6 8eb6 77b4  .m.h{G.;......w.
-00002510: bda3 ed5d 6def 6a7b 57db bbda ded5 f6ae  ...]m.j{W.......
-00002520: b677 b5bd abed 5d6d ef6a 7b57 dbbb dade  .w....]m.j{W....
-00002530: edf8 632f 6def 6a7b 57db bbda ded5 f6ae  ..c/m.j{W.......
-00002540: b677 b5bd abed 5d6d ef6a 7b57 dbbb dade  .w....]m.j{W....
-00002550: d5f6 9eb6 f7b4 bda7 ed3d 6def 697b 4fdb  .........=m.i{O.
-00002560: 7bda ded3 f69e b6f7 b4bd a7ed 3d6d ef69  {...........=m.i
-00002570: 7baf e34f 39b5 bda7 ed3d 6def 697b 4fdb  {..O9....=m.i{O.
-00002580: 7bda ded3 f69e b6f7 b4bd a7ed 3d6d ef69  {...........=m.i
-00002590: 7b5f dbfb dade d7f6 beb6 f7b5 bdaf ed7d  {_.............}
-000025a0: 6def 6b7b 5fdb fbda ded7 f6be b6f7 b5bd  m.k{_...........
-000025b0: afed 7d6d ef6b 7b5f dbfb dade d7f6 beb6  ..}m.k{_........
-000025c0: f7b5 bdaf ed7d 6def 6b7b 5fdb fbda 3ed0  .....}m.k{_...>.
-000025d0: f681 b60f b47d a0ed 036d 1f68 fb40 db07  .....}...m.h.@..
-000025e0: da3e d0f6 81b6 0fb4 7da0 ed03 6d1f 68fb  .>......}...m.h.
-000025f0: 40db 07da 3ed0 f681 b60f b47d a0ed 036d  @...>......}...m
-00002600: 1f68 fb40 db07 da3e d0f6 81b6 0fb5 7da8  .h.@...>......}.
-00002610: ed43 6d1f 6afb 50db 87da 3ed4 f6a1 b60f  .Cm.j.P...>.....
-00002620: b57d a8ed 436d 1f6a fb50 db87 da3e d4f6  .}..Cm.j.P...>..
-00002630: a1b6 0fb5 7da8 ed43 6d1f 6afb 50db 87da  ....}..Cm.j.P...
-00002640: 3ed4 f6a1 b60f b57d a8ed 236d 1f69 fb48  >......}..#m.i.H
-00002650: db47 da3e d2f6 91b6 8fb4 7da4 ed23 6d1f  .G.>......}..#m.
-00002660: 69fb 48db 47da 3ed2 f691 b68f b47d a4ed  i.H.G.>......}..
-00002670: 236d 1f69 fb48 db47 da3e d2f6 91b6 8fb4  #m.i.H.G.>......
-00002680: 7da4 ed23 6d1f 69fb 58db c7da 3ed6 f6b1  }..#m.i.X...>...
-00002690: b68f b57d aced 636d 1f6b fb58 dbc7 da3e  ...}..cm.k.X...>
-000026a0: d6f6 b1b6 8fb5 7dac ed63 6d1f 6bfb 58db  ......}..cm.k.X.
-000026b0: c7da 3ed6 f6b1 b68f b57d aced 636d 1f6b  ..>......}..cm.k
-000026c0: fb58 dbc7 da3e d1f6 89b6 4fb4 7da2 ed13  .X...>....O.}...
-000026d0: 6d9f 68fb 44db 27da 3ed1 f689 b64f b47d  m.h.D.'.>....O.}
-000026e0: a2ed 136d 9f68 fb44 db27 da3e d1f6 89b6  ...m.h.D.'.>....
-000026f0: 4fb4 7da2 ed13 6d9f 68fb 44db 27da 3ed1  O.}...m.h.D.'.>.
-00002700: f689 b64f b57d aaed 536d 9f6a fb54 dba7  ...O.}..Sm.j.T..
-00002710: da3e d5f6 a9b6 4fb5 7daa ed53 6d9f 6afb  .>....O.}..Sm.j.
-00002720: 54db a7da 3ed5 f6a9 b64f b57d aaed 536d  T...>....O.}..Sm
-00002730: 9f6a fb54 dba7 da3e d5f6 a9b6 4fb5 7daa  .j.T...>....O.}.
-00002740: ed33 6d9f 69fb 4cdb 67da 3ed3 f699 b6cf  .3m.i.L.g.>.....
-00002750: b47d a6ed 336d 9f69 fb4c db67 da3e d3f6  .}..3m.i.L.g.>..
-00002760: 99b6 cfb4 7da6 ed33 6d9f 69fb 4cdb 67da  ....}..3m.i.L.g.
-00002770: 3ed3 f699 b6cf b47d a6ed 336d 9f69 fb5c  >......}..3m.i.\
-00002780: dbe7 da3e d7f6 b9b6 cfb5 7dae ed73 6d9f  ...>......}..sm.
-00002790: 6bfb 5cdb e7da 3ed7 f6b9 b6cf b57d aeed  k.\...>......}..
-000027a0: 736d 9f6b fb5c dbe7 da3e d7f6 b9b6 cfb5  sm.k.\...>......
-000027b0: 7dae ed73 6d9f 6bfb 5cdb e7da bed0 f685  }..sm.k.\.......
-000027c0: b62f b47d a1ed 0b6d 5f68 fb42 db17 dabe  ./.}...m_h.B....
-000027d0: d0f6 85b6 2fb4 7da1 ed0b 6d5f 68fb 42db  ..../.}...m_h.B.
-000027e0: 17da bed0 f685 b62f b47d a1ed 0b6d 5f68  ......./.}...m_h
-000027f0: fb42 db17 dabe d0f6 85b6 2fb5 7da9 ed4b  .B......../.}..K
-00002800: 6d5f 6afb 52db 97da bed4 f6a5 b62f b57d  m_j.R......../.}
-00002810: a9ed 4b6d 5f6a fb52 db97 dabe d4f6 a5b6  ..Km_j.R........
-00002820: 2fb5 7da9 ed4b 6d5f 6afb 52db 97da bed4  /.}..Km_j.R.....
-00002830: f6a5 b62f b57d a9ed aa2b 16a9 f45d 550a  .../.}...+...]U.
-00002840: afba 7a91 4ae5 5557 31d2 958c 7435 235d  ..z.J.UW1...t5#]
-00002850: d148 5735 d295 8d74 7523 5de1 4857 39d2  .HW5...tu#].HW9.
-00002860: 958e 74b5 235d f148 573d d295 8f74 f523  ..t.#].HW=...t.#
-00002870: 5d01 49e5 1ca8 ba12 92ae 86a4 2b22 e9a8  ].I.........+"..
-00002880: 48aa 8e8c a4ea e848 aa8e 90a4 ea28 49aa  H......H.....(I.
-00002890: 8e94 a4ea 6849 aa8e 98a4 eaa8 49aa 8e9c  ....hI......I...
-000028a0: a4ea e849 aa8e a0a4 ea28 4aaa 8ea4 a4ea  ...I.....(J.....
-000028b0: 684a aa8e a8a4 eaa8 4aaa 8eac a4ea e84a  hJ......J......J
-000028c0: aa8e b0a4 ea28 4baa 8eb4 a45a ed98 071d  .....(K....Z....
-000028d0: 7149 d551 9754 1d79 49d5 d197 541d 8149  qI.Q.T.yI...T..I
-000028e0: d551 9854 1d89 49d5 d198 541d 9149 d551  .Q.T..I...T..I.Q
-000028f0: 9954 1d99 49d5 d199 541d a149 d551 9a54  .T..I...T..I.Q.T
-00002900: 1da9 49d5 d19a 541d b149 d551 9b54 1db9  ..I...T..I.Q.T..
-00002910: 49fe 52de 662f d74e 359b 7f1f c48f a49a  I.R.f/.N5.......
-00002920: 355f a49a c4d5 1d0c 71f5 0b33 4e35 cb91  5_......q..3N5..
-00002930: e152 3932 6264 8d91 7546 3618 d964 648b  .R92bd..uF6..dd.
-00002940: 916d 4676 18d9 6564 8f91 7d46 0e18 3964  .mFv..ed..}F..9d
-00002950: e488 9163 464e 1839 65e4 8c91 7346 2e18  ...cFN.9e...sF..
-00002960: b964 24bb 6f29 239b 2f43 7d87 060e 2936  .d$.o)#./C}...)6
-00002970: 1b2f cfa5 da6c bb50 cacd a60b a5de 6cb9  ./...l.P......l.
-00002980: 500a ce86 0ba5 e26c b750 4ace 660b a5e6  P......l.PJ.f...
-00002990: 6cb5 508a ce46 0ba5 ea6c b350 cace 265b  l.P..F...l.P..&[
-000029a0: 52d9 6319 d276 7658 286d 677f 85d2 7676  R.c..vvX(mg...vv
-000029b0: 5728 6d67 6f85 d276 7656 286d 675f 85d2  W(mgo..vvV(mg_..
-000029c0: 7676 5528 6d67 4f85 d276 7654 286d 673f  vvU(mgO..vvT(mg?
-000029d0: 85d2 7676 5328 6d67 2f85 d276 76d2 92ca  ..vvS(mg/..vv...
-000029e0: 46ca 90b6 b38d 4269 3b9b 2894 b6b3 8542  F.....Bi;.(....B
-000029f0: 693b 1b28 94b6 b37d 4269 3b9b 2794 b6b3  i;.(...}Bi;.'...
-00002a00: 7542 693b a926 94b6 936a 4269 bbaf eda4  uBi;.&...jBi....
-00002a10: 9a3c 50db 4935 a1b4 9d54 b3a4 926a 32a4  .<P.I5...T...j2.
-00002a20: ed81 b693 6af2 406d 27d5 84d2 7652 4d28  ....j.@m'...vRM(
-00002a30: 6d27 d584 d276 524d 286d 27d5 84d2 7652  m'...vRM(m'...vR
-00002a40: 4d28 6d27 d584 d276 524d 286d 27d5 84d2  M(m'...vRM(m'...
-00002a50: 7652 4d28 6d27 d52c a9a4 9a0c 693b a926  vRM(m'.,....i;.&
-00002a60: 94b6 936a 4269 3ba9 2694 b693 6a42 693b  ...jBi;.&...jBi;
-00002a70: a926 94b6 936a 4269 3ba9 2694 b693 6a42  .&...jBi;.&...jB
-00002a80: 693b a926 94b6 87da 4eaa c903 b59d 5413  i;.&....N.....T.
-00002a90: 4adb 4935 4b2a a926 43da 4eaa 09d5 f1f5  J.I5K*.&C.N.....
-00002aa0: 5bdb 4935 79a0 b693 6a42 693b a926 94b6  [.I5y...jBi;.&..
-00002ab0: 936a 4269 3ba9 2694 b693 6a42 693b a926  .jBi;.&...jBi;.&
-00002ac0: 94b6 936a 4269 3ba9 2694 b693 6a42 693b  ...jBi;.&...jBi;
-00002ad0: a966 4925 d564 48db 4935 a1b4 9d54 134a  .fI%.dH.I5...T.J
-00002ae0: db49 35a1 b49d 5413 4adb 4935 a1b4 9d54  .I5...T.J.I5...T
-00002af0: 134a db49 35a1 b49d 5413 4adb 4935 a1b4  .J.I5...T.J.I5..
-00002b00: bda6 eda4 9a3c 50db 4935 a1b4 9d54 b3a4  .....<P.I5...T..
-00002b10: 926a 32a4 eda4 9a50 da4e aa09 d5f1 c3b5  .j2....P.N......
-00002b20: b693 6af2 406d 27d5 84d2 7652 4d28 6d27  ..j.@m'...vRM(m'
-00002b30: d584 d276 524d 286d 27d5 84d2 7652 4d28  ...vRM(m'...vRM(
-00002b40: 6d27 d584 d276 524d 286d 27d5 2ca9 a49a  m'...vRM(m'.,...
-00002b50: 0c69 3ba9 2694 b693 6a42 693b a926 94b6  .i;.&...jBi;.&..
-00002b60: 936a 4269 3ba9 2694 b693 6a42 693b a926  .jBi;.&...jBi;.&
-00002b70: 94b6 936a 4269 3ba9 2694 b637 b49d 5493  ...jBi;.&..7..T.
-00002b80: 076a 3ba9 2694 b693 6a96 5452 4d86 b49d  .j;.&...j.TRM...
-00002b90: 5413 4adb 4935 a1b4 9d54 134a db49 35a1  T.J.I5...T.J.I5.
-00002ba0: b49d 5413 4adb 4935 a1b4 9d54 134a db49  ..T.J.I5...T.J.I
-00002bb0: 35a1 b49d 5413 4adb 9bda 4eaa c903 b59d  5...T.J...N.....
-00002bc0: 5413 4adb 4935 4b2a a926 43da 4eaa 09a5  T.J.I5K*.&C.N...
-00002bd0: eda4 9a50 da4e aa09 a5ed a49a 50da 4eaa  ...P.N......P.N.
-00002be0: 09a5 eda4 9a50 da4e aa09 a5ed a49a 50da  .....P.N......P.
-00002bf0: 4eaa 09a5 ed2d 6d27 d5e4 81da 4eaa 09a5  N....-m'....N...
-00002c00: eda4 9a25 9554 9321 6d27 d584 d276 524d  ...%.T.!m'...vRM
-00002c10: 286d 27d5 84d2 7652 4da8 8e5f 8c6b 3ba9  (m'...vRM.._.k;.
-00002c20: 260f d476 524d 286d 27d5 84d2 7652 4d28  &..vRM(m'...vRM(
-00002c30: 6d27 d584 d276 524d 286d 27d5 84d2 7652  m'...vRM(m'...vR
-00002c40: cd92 4aaa c990 b693 6a42 693b a926 94b6  ..J.....jBi;.&..
-00002c50: 936a 4269 3ba9 2694 b693 6a42 693b a926  .jBi;.&...jBi;.&
-00002c60: 94b6 936a 4269 3ba9 2694 b693 6a42 693b  ...jBi;.&...jBi;
-00002c70: a926 94b6 936a 4269 3ba9 6649 25d5 6448  .&...jBi;.fI%.dH
-00002c80: db49 35a1 b49d 5413 4adb 4935 a1b4 9d54  .I5...T.J.I5...T
-00002c90: 134a db49 35a1 b49d 5413 4adb 4935 a1b4  .J.I5...T.J.I5..
-00002ca0: 9d54 134a db49 35a1 b49d 5413 4adb 4935  .T.J.I5...T.J.I5
-00002cb0: a1b4 9d54 134a db49 354b 2aa9 2643 da4e  ...T.J.I5K*.&C.N
-00002cc0: aa09 a5ed a49a 50da 4eaa 09a5 eda4 9a50  ......P.N......P
-00002cd0: da4e aa09 a5ed a49a 50da 4eaa 09a5 eda4  .N......P.N.....
-00002ce0: 9a50 da4e aa09 a5ed a49a 50da 4eaa 09a5  .P.N......P.N...
-00002cf0: eda4 9a25 9554 9321 6d27 d584 d276 524d  ...%.T.!m'...vRM
-00002d00: 286d 27d5 84d2 7652 4d28 6d27 d584 d276  (m'...vRM(m'...v
-00002d10: 524d 286d 27d5 84d2 7652 4d28 6d27 d584  RM(m'...vRM(m'..
-00002d20: d276 524d 286d 27d5 84d2 7652 4d28 6d27  .vRM(m'...vRM(m'
-00002d30: d52c a9a4 9a0c 693b a926 94b6 936a 4269  .,....i;.&...jBi
-00002d40: 3ba9 2694 b693 6a42 693b a926 94b6 936a  ;.&...jBi;.&...j
-00002d50: 4269 3ba9 2694 b693 6a42 693b a926 94b6  Bi;.&...jBi;.&..
-00002d60: 0fb4 9d54 9307 6a3b a926 94b6 936a 9654  ...T..j;.&...j.T
-00002d70: 524d 86b4 9d54 134a db49 35a1 b49d 5413  RM...T.J.I5...T.
-00002d80: 4adb 4935 a1b4 9d54 134a db49 35a1 b49d  J.I5...T.J.I5...
-00002d90: 5413 4adb 4935 a1b4 9d54 134a db87 da4e  T.J.I5...T.J...N
-00002da0: aac9 03b5 9d54 134a db49 354b 2aa9 2643  .....T.J.I5K*.&C
-00002db0: da4e aa09 a5ed a49a 50da 4eaa 09a5 eda4  .N......P.N.....
-00002dc0: 9a50 da4e aa09 a5ed a49a 50da 4eaa 09a5  .P.N......P.N...
-00002dd0: eda4 9a50 da4e aa09 a5ed a49a 50da 4eaa  ...P.N......P.N.
-00002de0: 09a5 eda4 9a25 9554 9321 6d27 d584 d276  .....%.T.!m'...v
-00002df0: 524d 286d 27d5 84d2 7652 4d28 6d27 d584  RM(m'...vRM(m'..
-00002e00: d276 524d 286d 27d5 84d2 7652 4d28 6d27  .vRM(m'...vRM(m'
-00002e10: d584 d276 524d 286d 27d5 84d2 7652 4d28  ...vRM(m'...vRM(
-00002e20: 6d27 d52c a9a4 9a0c 693b a926 94b6 936a  m'.,....i;.&...j
-00002e30: 4269 3ba9 2694 b693 6a42 693b a926 94b6  Bi;.&...jBi;.&..
-00002e40: 936a 4269 3ba9 2694 b693 6a42 693b a926  .jBi;.&...jBi;.&
-00002e50: 94b6 936a 4269 3ba9 2694 b693 6a96 5452  ...jBi;.&...j.TR
-00002e60: 4d86 b49d 5413 4adb 4935 a1b4 9d54 134a  M...T.J.I5...T.J
-00002e70: db49 35a1 b49d 5413 4adb 4935 a1b4 9d54  .I5...T.J.I5...T
-00002e80: 134a db49 35a1 b49d 5413 4adb 4935 a1b4  .J.I5...T.J.I5..
-00002e90: 9d54 134a db49 35a1 b49d 54b3 a492 6a32  .T.J.I5...T...j2
-00002ea0: a4ed a49a 50da 4eaa 09a5 eda4 9a50 da4e  ....P.N......P.N
-00002eb0: aa09 a5ed a49a 50da 4eaa 09a5 eda4 9a50  ......P.N......P
-00002ec0: da4e aa09 a5ed a49a 50da 4eaa 09a5 eda4  .N......P.N.....
-00002ed0: 9a50 da4e aa59 5249 3519 d276 524d 286d  .P.N.YRI5..vRM(m
-00002ee0: 27d5 84d2 7652 4d28 6d27 d584 d276 524d  '...vRM(m'...vRM
-00002ef0: 286d 27d5 84d2 7652 4d28 6d27 d584 d276  (m'...vRM(m'...v
-00002f00: 524d 286d 27d5 84d2 7652 4d28 6d27 d584  RM(m'...vRM(m'..
-00002f10: d276 52cd 924a aac9 90b6 936a 4269 3ba9  .vR..J.....jBi;.
-00002f20: 2694 b693 6a42 693b a926 94b6 936a 4269  &...jBi;.&...jBi
-00002f30: 3ba9 2694 b693 6a42 693b a926 94b6 936a  ;.&...jBi;.&...j
-00002f40: 4269 3ba9 2694 b693 6a42 693b a966 4925  Bi;.&...jBi;.fI%
-00002f50: d564 48db 4935 a1b4 9d54 134a db49 35a1  .dH.I5...T.J.I5.
-00002f60: b49d 5413 4adb 4935 a1b4 9d54 134a db49  ..T.J.I5...T.J.I
-00002f70: 35a1 b49d 5413 4adb 4935 a1b4 9d54 134a  5...T.J.I5...T.J
-00002f80: db49 35a1 b49d 5413 4adb 75aa 5962 5557  .I5...T.J.u.YbUW
-00002f90: 2d92 5453 4ee3 5552 4d39 9d57 4935 e5b4  -.TSN.URM9.WI5..
-00002fa0: 5e25 d594 d37b 9554 534e f355 524d 39dd  ^%...{.TSN.URM9.
-00002fb0: 5749 35e5 b45f 25d5 94d3 7f95 5453 ce19  WI5.._%.....TS..
-00002fc0: 5025 d594 730e d4a9 a69c b3a0 4aaa 29d7  P%..s.......J.).
-00002fd0: 310f 3a32 923a d5e4 b11d 2149 9d6a ca75  1.:2.:....!I.j.u
-00002fe0: cc83 a49a 721d f320 a9a6 5cc7 3c48 aa29  ....r.. ..\.<H.)
-00002ff0: d731 0f92 6aca 75cc 83a4 9a72 1df3 20a9  .1..j.u....r.. .
-00003000: a65c c73c 48aa 29d7 310f 926a ca75 cc83  .\.<H.).1..j.u..
-00003010: a49a 721d f320 a9a6 5cc7 3c48 aa09 d711  ..r.. ..\.<H....
-00003020: 98d4 a9a6 5cc7 7ad0 d198 d4a9 a68f ed98  ....\.z.........
-00003030: 0749 35e5 3ae6 4152 4db9 8e79 9054 53ae  .I5.:.ARM..y.TS.
-00003040: 631e 24d5 94eb 9807 4935 e55a f3a0 9d6a  c.$.....I5.Z...j
-00003050: 36ef 25fc 23a9 e6f3 3d84 9b77 5f2d 47fa  6.%.#...=..w_-G.
-00003060: 4be5 c880 9121 2323 46d6 1859 6764 8391  K....!##F..Ygd..
-00003070: 4d46 b618 d966 6487 915d 46f6 18d9 67e4  MF...fd..]F...g.
-00003080: 8091 4346 8e18 3966 e484 9153 46ce 1839  ..CF..9f...SF..9
-00003090: 67e4 8291 4b46 b2b3 96c2 b2b1 32a4 d6fc  g...KF......2...
-000030a0: 0d08 508a 4d86 09a5 da64 9850 ca4d 8609  ..P.M....d.P.M..
-000030b0: a5de 6498 500a 4e86 09a5 e264 9850 4a4e  ..d.P.N....d.PJN
-000030c0: 8609 a5e6 6498 508a 4e86 09a5 ea64 9850  ....d.P.N....d.P
-000030d0: ca4e 86c9 f5aa ed6c 9f50 dace e609 a5ed  .N.....l.P......
-000030e0: 6c9d 50da cec6 09a5 ed6c 9b50 dace a609  l.P......l.P....
-000030f0: a5ed 6c99 50da ce86 09a5 ed6c 9750 dace  ..l.P......l.P..
-00003100: 6609 a5ed 6c95 50da ce46 09a5 ed6c 9325  f...l.P..F...l.%
-00003110: 955d 9221 6de7 af33 80d2 7676 4828 6d67  .].!m..3..vvH(mg
-00003120: 7f84 d276 7647 286d 676f 84d2 7676 4628  ...vvG(mgo..vvF(
-00003130: 6d67 5f84 d276 ee98 09a5 eddc 3113 4adb  mg_..v......1.J.
-00003140: b963 2694 b693 6142 693b 1926 94b6 9361  .c&...aBi;.&...a
-00003150: 9654 324c 863a 3668 6d27 c3e4 81da 4e86  .T2L.:6hm'....N.
-00003160: 09a5 ed64 9850 da4e 8609 a5ed 6498 50da  ...d.P.N....d.P.
-00003170: 4e86 09a5 ed64 9850 da4e 8609 a5ed 6498  N....d.P.N....d.
-00003180: 50da 4e86 09a5 ed64 9850 da4e 8659 52c9  P.N....d.P.N.YR.
-00003190: 3019 d276 324c 286d 27c3 84d2 7632 4c28  0..v2L(m'...v2L(
-000031a0: 6d27 c384 d276 324c 286d 27c3 84d2 7632  m'...v2L(m'...v2
-000031b0: 4c28 6d27 c384 d276 324c 286d 27c3 84d2  L(m'...v2L(m'...
-000031c0: 76ee 9809 a5ed dc31 b3a4 9261 32a4 eddc  v......1...a2...
-000031d0: 3113 4adb b963 2694 b693 6142 693b 1926  1.J..c&...aBi;.&
-000031e0: 94b6 9361 4269 3b19 2694 b693 6142 693b  ...aBi;.&...aBi;
-000031f0: 1926 94b6 9361 4269 3b19 2694 b693 6142  .&...aBi;.&...aB
-00003200: 693b 1926 94b6 9361 9654 324c 86b4 9d0c  i;.&...a.T2L....
-00003210: 134a dbc9 30a1 b49d 0c13 4adb c930 a1b4  .J..0.....J..0..
-00003220: 9d0c 134a dbc9 30a1 b49d 0c13 4adb c930  ...J..0.....J..0
-00003230: a1b4 9d0c 134a dbc9 30a1 b49d 3b66 4269  .....J..0...;fBi
-00003240: 3b77 cc2c a964 980c 693b 77cc 84d2 76ee  ;w.,.d..i;w...v.
-00003250: 9809 a5ed dc31 134a dbc9 30a1 b49d 0c13  .....1.J..0.....
-00003260: 4adb c930 a1b4 9d0c 134a dbc9 30a1 b49d  J..0.....J..0...
-00003270: 0c13 4adb c930 a1b4 9d0c 134a dbc9 30a1  ..J..0.....J..0.
-00003280: b49d 0cb3 a492 6132 a4ed 6498 50da 4e86  ......a2..d.P.N.
-00003290: 09a5 ed64 9850 da4e 8609 a5ed 6498 50da  ...d.P.N....d.P.
-000032a0: 4e86 09a5 ed64 9850 da4e 8609 a5ed 6498  N....d.P.N....d.
-000032b0: 50da 4e86 09a5 eddc 3113 4adb b963 6649  P.N.....1.J..cfI
-000032c0: 25c3 6448 dbb9 6326 94b6 73c7 4c28 6de7  %.dH..c&..s.L(m.
-000032d0: 8e99 50da ce1d 33a1 b49d 3b66 4269 3b77  ..P...3...;fBi;w
+00001160: 6865 6574 322e 786d 6c94 5adb 6ee3 3610  heet2.xml.Z.n.6.
+00001170: 7d2f d07f 10f4 beb1 495d 621b 7116 1b07  }/......I]b.q...
+00001180: 4103 b440 d1ed ed55 91e9 5888 64a9 9272  A..@...U..X.d..r
+00001190: d9fd fa9d 916c 6938 146b f361 37b6 e668  .....li8.k.a7..h
+000011a0: 8e48 ce9c 1991 bef9 fc51 e4de 9baa 9bac  .H.......Q......
+000011b0: 3cac 7d71 35f7 3d75 48cb 6d76 785e fb7f  <.}q5.=uH.mvx^..
+000011c0: fdf9 f069 e17b 4d9b 1cb6 495e 1ed4 daff  ...i.{M...I^....
+000011d0: a61a fff3 edcf 3fdd bc97 f54b b357 aaf5  ......?....K.W..
+000011e0: c0c3 a159 fbfb b6ad 56b3 5993 ee55 9134  ...Y....V.Y..U.4
+000011f0: 5765 a50e 60d9 9575 91b4 f0b5 7e9e 3555  We..`..u....~.5U
+00001200: ad92 6d77 5391 cfe4 7c1e cf8a 243b f8bd  ..mwS...|...$;..
+00001210: 8755 7d89 8f72 b7cb 5275 5fa6 af85 3ab4  .U}..r..Ru_...:.
+00001220: bd93 5ae5 490b cfdf ecb3 aa39 792b d24b  ..Z.I......9y+.K
+00001230: dc15 49fd f25a 7d4a cba2 0217 4f59 9eb5  ..I..Z}J....OY..
+00001240: df3a a7be 57a4 abc7 e743 5927 4f39 8cfb  .:..W....CY'O9..
+00001250: 4384 497a f2dd 7d31 dc17 595a 974d b96b  C.Iz..}1..YZ.M.k
+00001260: afc0 ddac 7f50 73cc cbd9 7206 9e6e 6fb6  .....Ps...r..no.
+00001270: 198c 00a7 ddab d56e ed7f 11ab 4dbc f467  .......n....M..g
+00001280: b737 dd04 fd9d a9f7 867c f6da b2fa 55ed  .7.......|....U.
+00001290: da8d ca73 0087 b04e b802 4f65 f982 d0c7  ...s...N..Oe....
+000012a0: edda 9f83 d346 e52a c5b9 f012 f8f3 a68e  .....F.*........
+000012b0: f058 c02a fed7 f3c4 62f5 efc3 3d5c 01aa  .X.*....b...=\..
+000012c0: d9c0 453f 9f78 1fba b5fb bdf6 b66a 97bc  ..E?.x.......j..
+000012d0: e6ed 1fe5 fb2f 2a7b deb7 1028 11cc 054e  ...../*{...(...N
+000012e0: c96a fbed 5e35 29ac 053c c095 8cd0 6b5a  .j..^5)..<....kZ
+000012f0: e6e0 02fe f78a 0c83 0ae6 32f9 e8fe be67  ..........2....g
+00001300: db76 bff6 17f3 ab6b 315f 06d7 e025 7d6d  .v.....k1_...%}m
+00001310: dab2 f8a7 3774 0f35 dc28 8f37 c2df e38d  ....7t.5.(.7....
+00001320: e165 3706 2746 a03e de29 fff7 ce59 ffc8  .e7.'F.>.)...Y..
+00001330: dd6c dc27 6d72 7b53 97ef 1e04 24ce 5b95  .l.'mr{S....$.[.
+00001340: 6078 8b15 789d 1e32 8c15 b15f 10dc dd02  `x..x..2..._....
+00001350: 73d1 c062 bcdd 0652 decc de60 6e53 f807  s..b...R...`nS..
+00001360: 2e07 bf30 a4cb fd02 78f0 2816 8bc1 63c7  ...0....x.(...c.
+00001370: 7aa7 5b97 d37c a10b 1f82 f938 c269 bfb0  z.[..|.....8.i..
+00001380: 8097 8f03 c0e3 3896 7336 0edd 2aa6 f962  ......8.s6..*..b
+00001390: 173e 0013 be71 25fa 79d3 adc1 34df b50b  .>...q%.y...4...
+000013a0: 1f80 09df 3863 3d9f 6e8d a6f9 506d 2f8e  ....8c=.n...Pm/.
+000013b0: 3700 13be 98cd a76e bd9e e65b baf0 0198  7......n...[....
+000013c0: f0f1 38d4 ad96 3814 a05b 0e09 05e8 8111  ..8...8..[......
+000013d0: ea05 1b21 3a23 664b c808 b71c 0634 f1c9  ...!:#fK.....4..
+000013e0: 8306 9d11 b325 6a84 537a 237a 548c e538  .....%j.Sz#zT..8
+000013f0: 737d dc68 e690 4c82 2628 02d4 c961 6201  s}.h..L.&(...ab.
+00001400: 3d50 8672 1cc6 9152 378f f3ae 533a 253f  =P.r...R7...S:%?
+00001410: 560c 5015 9ae5 8149 dc83 82ae 8aa0 a66e  V.P....I.......n
+00001420: 8eb7 7557 7476 2729 1088 5efb 745c 8118  ..uWtv')..^.t\..
+00001430: 73f0 38ec 2910 4bab cde0 09cb 2795 7441  s.8.).K.....'.tA
+00001440: b502 96f4 4cad a072 20e7 5c2c d019 8933  ....L..r .\,...3
+00001450: 8b5a 082a 17e7 29a9 22c8 39d7 0b74 4628  .Z.*..).".9..tF(
+00001460: 2d82 21a8 629c a7a4 a220 e75c 32d0 19a1  -.!.b.... .\2...
+00001470: b468 86a4 9a71 9612 d124 b447 5138 564b  .h...q...$.GQ8VK
+00001480: dd6c 2bcf 3481 cf53 229a 15cc c036 189a  .l+.4..S"....6..
+00001490: a7e7 3dd3 8095 820b a0d4 cd16 0194 b4f8  ..=.............
+000014a0: 9fa7 04f4 b826 820b 203a 2366 8b00 421f  .....&.. :#f..B.
+000014b0: 38aa d179 4a2a 0a52 f05c 4067 84d2 920b  8..yJ*.R.\@g....
+000014c0: d229 fd3a 34ef 716c 9e9d b24c d234 0a16  .).:4.ql...L.4..
+000014d0: c692 6959 26c6 24d4 db43 a72c 9334 8d82  ..iY&.$..C.,.4..
+000014e0: 8511 f25a 9609 4b62 074e 5986 e8b1 662d  ...Z..Kb.NY...f-
+000014f0: 7894 6866 29c6 bcd7 4619 d0ca 7c36 4a10  x.hf)...F...|6J.
+00001500: 4d28 79cd d2cc 5258 d22f 704a 6c44 134a  M(y...RX./pJlD.J
+00001510: 1e98 9a59 4a4b 990c 9c2a 33a2 0925 2f51  ...YJK...*3..%/Q
+00001520: 9a59 4a4b c607 4eed 3ea2 c7fc 226f 2cbd  .YJK..N.>..."o,.
+00001530: 6232 b325 e303 a766 00d1 84d2 9858 dd6c  b2.%...f.....X.l
+00001540: c9cb c0a9 0340 34a1 e4d5 8f99 6d49 e2f4  .....@4.....mI..
+00001550: 3e10 209a 371d 46dc 4e81 d884 6c06 4fbc  >. .7.F.N...l.O.
+00001560: e908 9c5e 1810 3d06 d735 ef34 35b3 94b6  ...^..=..5.45...
+00001570: ac75 7a67 0834 f191 06a5 660e 2c29 84bb  .uzg.4....f.,)..
+00001580: 1d97 37b7 881e 573a e072 c8cc 960e 2074  ..7...W:.r.... t
+00001590: 7a6b 4034 9958 dee7 6866 1958 5228 747a  zk@4.X..hf.XR(tz
+000015a0: 6b40 34a1 1c03 b6cf 5acd 2c03 cbeb 7be8  k@4.....Z.,...{.
+000015b0: a44d 8826 13cb b589 992d a52d 74db 8ad0  .M.&.....-.-t...
+000015c0: b429 3046 a99b 2d11 1b3a 6913 a2c9 c472  .)0F..-..:i....r
+000015d0: a1d0 ccd2 d6e6 854e dad4 a175 a190 21ef  .......N...u..!.
+000015e0: 1c26 412c b837 0388 0b45 e8a4 5c1d 9a2b  .&A,.7...E..\..+
+000015f0: 9791 4853 cac5 3a81 cde0 c978 2027 e50a  ..HS..:....x '..
+00001600: b5b6 29e4 fd06 33db 12cc 49b9 424d 9a42  ..)...3...I.BM.B
+00001610: 5ea3 98d9 52a3 2227 e542 f418 7a21 8f76  ^...R."'.B..z!.v
+00001620: cd2c 434b 8245 4eca 8568 42c9 954b 334b  .,CK.EN..hB..K3K
+00001630: f244 5a23 1739 c948 87e6 bdb7 6d30 4e6a  .DZ#.9.H....m0Nj
+00001640: 1169 7210 1a83 d1cd 9616 3172 dbd3 d45a  .ir.......1r...Z
+00001650: 95c8 d8d4 d4cd 967e 2d72 520b 4493 2533  .......~-rR.D.%3
+00001660: 28b5 4627 b2d4 b7c8 490f 103d 2a7f c47b  (.F'....I..=*..{
+00001670: 1866 b6ed 153b 657c 4433 3e34 de43 99d9  .f...;e|D3>4.C..
+00001680: 92f1 9153 c623 9a8c 92d7 3766 b644 6cec  ...S.#....7f.Dl.
+00001690: 94f1 8826 943c e399 d952 dfba d39d 8b77  ...&.<...R.....w
+000016a0: 8d11 3d50 86d2 a0d4 cd36 4aa7 5e25 ee37  ..=P.....6J.^%.7
+000016b0: 48c6 6dbd 3be3 ca86 5ed1 c425 7612 970e  H.m.;...^..%v...
+000016c0: cdb7 198d 31a2 4b2c 6f78 58d5 6d33 1e6f  ....1.K,oxX.m3.o
+000016d0: 33b7 1963 2701 ead0 ac90 47bc e79d 02c5  3..c'.....G.....
+000016e0: 2c8b 3703 88d7 cdd8 499e 3a34 2be4 4629  ,.7.....I.:4+.F)
+000016f0: 9b04 b1e8 df0c 20e3 81dc ce64 26f6 5823  ...... ....d&.X#
+00001700: 637d a640 4ccd 37f1 0964 3c90 93b4 c513  c}.@L.7..d<.....
+00001710: 5d8c b964 1320 73c9 4e20 e381 9c84 2f46  ]..d. s.N ..../F
+00001720: 340d ce3b e3ca 865e d193 c549 f0e0 bc99  4..;...^...I....
+00001730: 53f1 2b78 263d 607a aafe d0b8 3f26 ad92  S.+x&=`z....?&..
+00001740: 67f5 5b52 3f67 87c6 cbe1 781a 0f81 f154  g.[R?g....x....T
+00001750: b7ee 8f89 fb2f 7074 dd95 fba7 b285 a3de  ...../pt........
+00001760: eee3 1e7e 08a0 607f 7f7e 05e0 5d59 b6a7  ...~..`..~..]Y..
+00001770: 2f30 77e8 f3ab 6a5f 2baf 4a2a 557f cdbe  /0w...j_+.J*U...
+00001780: c3f9 3b3c 4559 6770 ccdc 9df4 affd aaac  ..;<EYgp........
+00001790: db3a c95a dfdb c3f5 ef25 18f2 fb2a 8379  .:.Z.....%...*.y
+000017a0: 9b83 a4c2 0f1a da2c 3d5e 81ef f52a dbae  .......,=^...*..
+000017b0: fdfa 71db 9f7a 0fbf 5db8 fd01 0000 ffff  ..q..z..].......
+000017c0: 0300 504b 0304 1400 0600 0800 0000 2100  ..PK..........!.
+000017d0: 8112 9d2b 9402 0000 f308 0000 1800 0000  ...+............
+000017e0: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
+000017f0: 6565 7433 2e78 6d6c 9456 cb8e a330 10bc  eet3.xml.V...0..
+00001800: afb4 ff80 7c9f 18f2 4e14 18cd 281a ed1c  ....|...N...(...
+00001810: 565a adf6 7176 8c01 2b18 23db 79cc df6f  VZ..qv..+.#.y..o
+00001820: 1b92 0c38 6105 9710 54dd 55ee a6e8 66f3  ...8a...T.U...f.
+00001830: 7c16 b977 644a 7359 8428 18f9 c863 0595  |..wdJsY.(...c..
+00001840: 312f d210 fdfe f5f6 b444 9e36 a488 492e  1/.......D.6..I.
+00001850: 0b16 a20f a6d1 73f4 f5cb e624 d55e 678c  ......s....$.^g.
+00001860: 190f 180a 1da2 cc98 728d b1a6 1913 448f  ........r.....D.
+00001870: 64c9 0a40 12a9 0431 70ab 52ac 4bc5 485c  d..@...1p.R.K.H\
+00001880: 2589 1c8f 7d7f 8e05 e105 aa19 d6aa 0f87  %...}...........
+00001890: 4c12 4ed9 56d2 8360 85a9 4914 cb89 81f3  L.N.V..`..I.....
+000018a0: eb8c 97fa ca26 681f 3a41 d4fe 503e 5129  .....&h.:A..P>Q)
+000018b0: 4aa0 d8f1 9c9b 8f8a 1479 82ae dfd3 422a  J........y....B*
+000018c0: b2cb a1ee 7330 25f4 ca5d dddc d10b 4e95  ....s0%..]....N.
+000018d0: d432 3123 a0c3 f541 ef6b 5ee1 1506 a668  .21#...A.k^....h
+000018e0: 1373 a8c0 b6dd 532c 09d1 4bb0 7e0d 2608  .s....S,..K.~.&.
+000018f0: 479b aa41 7f38 3be9 c67f cff6 7b27 e5de  G..A.8;.....{'..
+00001900: 02ef 7188 7c1b 8aef 62df aa7e ff50 5ecc  ..q.|...b..~.P^.
+00001910: 1272 c8cd 4f79 fac6 789a 1978 b833 38bf  .r..Oy..x..x.38.
+00001920: 2d63 1d7f 6c99 a6d0 3fa0 198d 6796 89ca  -c..l...?...g...
+00001930: 1ce4 e0d7 13dc 1a01 ea27 e7ea 7ae2 b1c9  .........'..z...
+00001940: 42b4 f447 8bc0 5f4d 16c0 420f da48 f1b7  B..G.._M..B..H..
+00001950: 0682 4b7a 9d38 be24 c2f5 9238 ed97 38b9  ..Kz.8.$...8..8.
+00001960: 24c2 f592 38fe 6f22 ae4f 5c35 604b 0c89  $...8.o".O\5`K..
+00001970: 364a 9e3c f010 1c5d 97c4 3a32 58c3 291e  6J.<...]..:2X.).
+00001980: 570c a5da d817 0886 2668 781c c768 3c0f  W.......&hx..h<.
+00001990: 36f8 084d a517 f4b5 8d8e 6f28 06a9 9b1e  6..M......o(....
+000019a0: 68f4 d783 e086 dec4 d16b a3d3 c77a d0a0  h........k...z..
+000019b0: fe7a 10dc d09b 397a 6d74 fe58 6f3a 440f  .z....9zmt.Xo:D.
+000019c0: 821b 7a0b 47af 8d2e 1feb 81bf fad7 07c1  ..z.G...........
+000019d0: 0dbd 95a3 d742 17fe 63bd f910 3d08 fed4  .....B..c...=...
+000019e0: 5bb8 7e69 a31d 7e59 0cd1 83e0 869e eb97  [.~i..~Y........
+000019f0: 36da e117 3bc0 7bbf 0f10 dcd0 73fd d246  6...;.{.....s..F
+00001a00: 3bfc b21a a207 c10d 3dd7 2f6d b4c3 2f01  ;.......=./m../.
+00001a10: acac 012f 3c44 3714 5dc7 58b2 4f78 d961  .../<D7.].X.Ox.a
+00001a20: 9960 d88c 698d 91e5 dd90 69c3 1dae 0906  .`..i.....i.....
+00001a30: 8d19 1bdd 28c3 f58d 0377 1807 b6d1 90c6  ....(....w......
+00001a40: b686 c9d2 b58e 256b 9cc8 f54e bdc8 ea39  ......%k...N...9
+00001a50: 5e92 947d 272a e585 f672 9654 4bca 6e1d  ^..}'*...r.TK.n.
+00001a60: 55af 31d8 0af6 bd96 6535 ea77 d2c0 2aaa  U.1.....e5.w..*.
+00001a70: fe66 f071 c160 a8fb 23c0 1329 cdf5 c62e  .f.q.`..#..)....
+00001a80: cadb e74a f40f 0000 ffff 0300 504b 0304  ...J........PK..
+00001a90: 1400 0600 0800 0000 2100 e628 743d 522b  ........!..(t=R+
+00001aa0: 0000 102f 0100 1800 0000 786c 2f77 6f72  .../......xl/wor
+00001ab0: 6b73 6865 6574 732f 7368 6565 7431 2e78  ksheets/sheet1.x
+00001ac0: 6d6c 9cdd 5973 1b47 a267 f1f7 8998 efa0  ml..Ys.G.g......
+00001ad0: e0fb 5802 c14d 0ecb 378a 58b8 ef3b dfd8  ..X..M..7.X..;..
+00001ae0: 126d 335a 1235 24db ee9e 4f3f ff22 45a2  .m3Z.5$...O?."E.
+00001af0: 2a7f 0553 e887 7bdb ce3a 4001 3859 9920  *..S..{..:@.8Y. 
+00001b00: e5a3 fae5 7ffe fde5 f39b 3faf efee 6f6e  ..........?...on
+00001b10: bf7e 98eb fdf4 6eee cdf5 d78f b79f 6ebe  .~....n.......n.
+00001b20: fefe 61ee e478 fc7f 56e6 dedc 3f5c 7dfd  ..a..x..V...?\}.
+00001b30: 74f5 f9f6 ebf5 87b9 ff5c dfcf fdcf afff  t........\......
+00001b40: fb7f fdf2 d7ed dd3f efff b8be 7e78 9367  .......?....~x.g
+00001b50: f87a ff61 ee8f 8787 6f3f bf7d 7bff f18f  .z.a....o?.}{...
+00001b60: eb2f 57f7 3fdd 7ebb fe9a 23bf ddde 7db9  ./W.?.~...#...}.
+00001b70: 7ac8 bfde fdfe f6fe dbdd f5d5 a7c7 077d  z..............}
+00001b80: f9fc 76fe ddbb a5b7 5fae 6ebe ce3d 3dc3  ..v....._.n..==.
+00001b90: cf77 3ff2 1cb7 bffd 76f3 f17a 78fb f15f  .w?.....v..zx.._
+00001ba0: 5fae bf3e 3c3d c9dd f5e7 ab87 bcfe fb3f  _..><=.........?
+00001bb0: 6ebe dd3f 3fdb 978f 3ff2 745f aeee fef9  n..??...?.t_....
+00001bc0: af6f ffe7 e3ed 976f 798a 7fdc 7cbe 79f8  .o.....oy...|.y.
+00001bd0: cfe3 93ce bdf9 f2f1 e78d dfbf dede 5dfd  ..............].
+00001be0: e373 def7 bf7b 0b57 1f9f 9ffb f15f 78fa  .s...{.W....._x.
+00001bf0: 2f37 1fef 6eef 6f7f 7bf8 294f f7f6 e985  /7..n.o.{.)O....
+00001c00: fa9e dfbf 7dff 36cf f4eb 2f9f 6ef2 0eea  ....}.6.../.n...
+00001c10: 8ffd cddd f56f 1fe6 aade cfd5 60bf b7b0  .....o......`...
+00001c20: 3cf7 f6d7 5f1e 3fa3 d39b ebbf ee1b fffc  <..._.?.........
+00001c30: e6e1 ea1f 47d7 9faf 3f3e 5c7f 8aaa b937  ....G...?>\....7
+00001c40: 0fb7 dfb6 af7f 7b18 5c7f fe9c c7cf 67a4  ......{.\.....g.
+00001c50: 96f2 8fdb db7f d60f dd08 f42e e7b9 7f7c  ...............|
+00001c60: 487d 9eab 8f0f 377f 5e3f e1ab fda5 88fd  H}....7.^?......
+00001c70: bf8f a7ae ff39 277d fb72 d6e6 3f3f bf82  .....9'}.r..??..
+00001c80: f1a3 c8fd bb37 9fae 7fbb fad7 e787 c3db  .....7..........
+00001c90: bfd6 af6f 7eff e321 2f65 311f 4cfd f9fc  ...o~..!/e1.L...
+00001ca0: fce9 3fc3 ebfb 8f11 9353 ff34 bf58 3feb  ..?......S.4.X?.
+00001cb0: c7db cf79 8afc ff37 5f6e ea19 960f f6ea  ...y...7_n......
+00001cc0: df8f fffb d7cd a787 3f3e ccad bcfb 69b9  ........?>....i.
+00001cd0: f7ee 7d7f 39cf f2f1 5ff7 0fb7 5fce 9e0e  ..}.9..._..._...
+00001ce0: f4be 3ffc e981 f3df 1f98 fffd fec0 851f  ..?.............
+00001cf0: 7b60 fffb 0397 9733 b7bf 3f74 fe6f 1ffa  {`.....3..?t.o..
+00001d00: f6e9 353f 7e1c c3ab 87ab 5f7f b9bb fdeb  ..5?~....._.....
+00001d10: 4da6 675e fcfd b7ab 7ab2 f77e ced3 3ebe  M.g^....z..~..>.
+00001d20: f795 9fea 17de f1f6 fbf9 ec3f d68f aaea  ...........?....
+00001d30: 877d 98cb 0bcf c772 9fd1 3f7f edcf f77e  .}.....r..?....~
+00001d40: 79fb 673e e68f f9bf 3cf9 cb19 0235 cfd0  y.g>....<....5..
+00001d50: fda9 3e3f 6ff3 19df bd3c dfe3 3957 9bc7  ..>?o....<..9W..
+00001d60: a69c 2bef e0c7 cf15 f8e5 d5cf 17e7 6a1e  ..+...........j.
+00001d70: eb77 bfaf 8559 ce55 c31f e69a cfba 509c  .w...Y.U......P.
+00001d80: 5162 b14d 0c9e 897a 5e37 3fe0 7ad6 ff17  Qb.M...z^7?.z...
+00001d90: 0aeb 877d 98cb 934e 14f6 97bb dfea f22c  ...}...N.......,
+00001da0: 6f35 f0cb 33f6 269e 9e1c b60e 4e3e f4d6  o5..3.&.....N>..
+00001db0: fba9 97e7 c6fb f9fb 0913 7872 b689 a9a7  ..........xr....
+00001dc0: b3b5 0e4e 3ef0 d6d9 decf 72b6 c093 b315  ...N>.....r.....
+00001dd0: 7e56 5b07 97ba 3fc9 5e2e d81f 7f73 353d  ~V[...?.^....s5=
+00001de0: 39df 44ce d3bb 6b1f 5d99 72c2 e202 fffb  9.D...k.].r.....
+00001df0: 4fb3 572f c1cf 5774 ef7d 3145 5b47 e727  O.W/..Wt.}1E[G.'
+00001e00: 9767 ebf3 eccd 74bd d7f4 e422 2c67 4bfb  .g....t....",gK.
+00001e10: e894 e9d2 9be9 a2af e9c9 845f 2caf fbd6  ..........._,...
+00001e20: e1f9 2957 7e6f a64b bfa6 276f b1bc ecdb  ..)W~o.K..'o....
+00001e30: 4727 53aa fd99 6639 9e61 d684 9e9c 7032  G'S...f9.a....p2
+00001e40: 11bf cf9a d6d1 2917 7caf 5853 5e99 35a1  ......).|.XS^.5.
+00001e50: 1b9f 2916 9b87 e7a7 cdd3 e61a 9349 f1ca  ..)..........I..
+00001e60: 199b eb48 7f81 3336 0fcf 4fa6 71fb 436d  ...H..36..O.q.Cm
+00001e70: ae33 af9f b1b9 96f4 17f8 545b 87a7 5d1a  .3........T[..].
+00001e80: cdb5 e6f5 3336 d793 3e6f b175 74ca a531  ....36..>o.ut..1
+00001e90: df5c 6d5e 3d61 4d37 f682 72f7 6d1d 9db2  .\m^=aM7..r.m...
+00001ea0: 98d6 5fd8 5e26 eaeb 276c ae36 fd72 39ad  .._.^&..'l.6.r9.
+00001eb0: 9f6b f272 a6ac a7f3 cdd5 e6f5 13b6 beb0  .k.r............
+00001ec0: 94eb 69fd 5c93 134e 99a7 f3cd d5e6 f513  ..i.\..N........
+00001ed0: b656 9b72 3dad 9feb e584 0b53 26cd 7c73  .V.r=......S&.|s
+00001ee0: b179 fd84 cdc5 86eb a27e aec9 09a7 4d9a  .y.......~....M.
+00001ef0: e662 f3fa 099b cbc9 42b9 01e7 fb72 e384  .b......B....r..
+00001f00: d326 4d73 b179 fd84 cdd5 6481 49d3 3a3a  .&Ms.y....d.I.::
+00001f10: 6dd2 ccb4 d6cc 3717 9305 264d ebe8 b449  m.....7...&M...I
+00001f20: 33d3 5233 df5c 4b16 9834 cda3 8bd3 26cd  3.R3.\K..4....&.
+00001f30: 4c2b cd7c 732d 592c 579a f6d1 2993 a63f  L+.|s-Y,W...)..?
+00001f40: d34a 53d3 2ff3 70b1 9c34 eda3 5326 4d7f  .JS./.p..4..S&M.
+00001f50: a695 a6a6 2727 2c27 4dfb e894 49d3 9f69  ....'','M...I..i
+00001f60: a5a9 e9c9 09cb 49d3 3e3a 65d2 f467 5a69  ......I.>:e..gZi
+00001f70: 6a7a 72c2 72d2 b48e 2e4d 9934 fd99 569a  jzr.r....M.4..V.
+00001f80: 9a7e 39e1 5239 69da 47a7 4d9a 9956 9a7e  .~9.R9i.G.M..V.~
+00001f90: 732d e92f 975f a45a 8717 a66d fa8f bf22  s-./._.Z...m..."
+00001fa0: 78fe e1e2 d5b5 a6a6 273b c232 f3a6 7578  x.......';.2..ux
+00001fb0: 65da c499 69b5 e9b7 bed9 f498 39ed c3d3  e...i.......9...
+00001fc0: a6ce 4ceb 4dbf f5dd 6599 cbb1 75b8 f143  ..L.M...e...u..C
+00001fd0: 41eb db54 7fa6 15a7 a61b df18 3965 fbcb  A..T........9e..
+00001fe0: cd94 f9ba 30d3 9af3 487f 986b 295b 2aaf  ....0...H..k)[*.
+00001ff0: 93ef 50eb 435e 9e76 fa99 56a0 85a7 df98  ..P.C^.v..V.....
+00002000: b427 5479 d57c 87da a79f 72f1 2ccc b41e  .'Ty.|....r.,...
+00002010: d5f4 e403 7f5f 7ee0 edc3 2b53 7e2a 5898  ....._~...+S~*X.
+00002020: 6945 aae9 c629 f97d 47eb f0ca 942f e90b  iE...).}G..../..
+00002030: 33ad 4935 dd38 6579 bdb6 0faf 4cb9 7816  3.I5.8ey....L.x.
+00002040: 665a 956a ba71 caf2 e782 e2f0 b4a9 34d3  fZ.j.q........4.
+00002050: 37a0 85d6 247a 5f2e 11c5 e129 bf29 cb2f  7...$z_....).)./
+00002060: 6567 f8a6 5ed3 8d77 39f9 e49e 7ea6 2c0e  eg..^..w9...~.,.
+00002070: 4f9b b1cd 2522 efe1 477f d7b8 503f aef8  O...%"..G...P?..
+00002080: 4dd5 c294 732c 36d7 849c e3ef 7f8c ace9  M...s,6.........
+00002090: c91e 564e 97f6 d129 abfb 6273 1578 fd84  ..VN...)..bs.x..
+000020a0: cdef 214b a5b9 fab9 262f 67ca f45c 6c5e  ..!K....&/g..\l^
+000020b0: f7af 9fb0 79dd b3dc d5cf f572 c269 ebdc  ....y......r.i..
+000020c0: 62f3 aa7f fd84 cdcb 7ab9 5ce0 eae7 9a9c  b.......z.\.....
+000020d0: 709a c3e6 0538 c33c 59ac 1fd7 9e27 4b53  p....8.<Y....'KS
+000020e0: 7e83 b3d8 bce0 5e7f 4fcd 0bae f194 4f93  ~.....^.O.....O.
+000020f0: bf7e ae89 b529 5f57 179b 3bf2 2cef a97e  .~...)_W..;.,..~
+00002100: 5cf9 5bda 6933 a3b8 be5e 99fb cd3d 964d  \.[.i3...^...=.M
+00002110: 7fb1 7574 ca9b 5a9a e962 abe9 89fb f262  ..ut..Z..b.....b
+00002120: 6b1f 9d72 b12d cd74 b13d d2ed 5fba 2f97  k..r.-.t.=.._./.
+00002130: 975c 1753 ac6e 8317 a6fe a39f fa4f 3f86  .\.S.n.......O?.
+00002140: 8c8c 1819 3747 dabf ae9f e902 5eaa e9e2  ....7G......^...
+00002150: 4d94 df5a 3a98 95e2 0f4f 062f cce4 4d3c  M..Z:....O./..M<
+00002160: 3ff3 f3c8 0866 dc1c 69bf 8999 1685 a59a  ?....f..i.......
+00002170: aedf c4f3 a956 1919 3032 6464 c4c8 b839  .....V..02dd...9
+00002180: d27e 81cd 2f0e 335c 704b 4f7f cad2 fa22  .~../.3\pKO...."
+00002190: d1f8 9de5 d325 ff1d 9abc 9f01 2343 4646  .....%......#CFF
+000021a0: 8c8c 9b23 ed57 df5c 021f ff94 efef 2fe6  ...#.W.\....../.
+000021b0: a5a7 a5af b9ba f21d af8b 29be 940d 5e98  ..........)...^.
+000021c0: c92c 797e e6c9 2c29 47c6 cd47 b5df 4673  .,y~..,)G..G..Fs
+000021d0: 99fd 91b7 51f3 edc9 fe9e 85a2 8329 be75  ....Q........).u
+000021e0: 0d96 9e99 c9db 2847 4630 6346 d618 5967  ......(GF0cF..Yg
+000021f0: 6483 914d 46b6 18d9 6664 8791 5d46 f618  d..MF...fd..]F..
+00002200: d967 e480 9143 468e 1839 66e4 8491 5346  .g...CF..9f...SF
+00002210: ce18 3967 e482 914b 46aa caa1 5587 d45a  ..9g...KF...U..Z
+00002220: 0da5 145b 69b6 526d a5db 4ab9 9576 2bf5  ...[i.Rm..J..v+.
+00002230: 56fa ad14 5c69 b852 71a5 e34a c995 962b  V...\i.Rq..J...+
+00002240: 3557 7aae 145d 69ba 5275 a5eb 4ad9 95b6  5Wz..]i.Ru..J...
+00002250: 57b5 bdaa ed55 6daf 6a7b 55db abda 5ed5  W....Um.j{U...^.
+00002260: f6aa b657 b5bd aaed 556d af6a 7b55 dbab  ...W....Um.j{U..
+00002270: da5e d5f6 aab6 57b5 bdaa ed55 6daf 6a7b  .^....W....Um.j{
+00002280: 55db abda 5ed5 f6aa b657 b5bd aaed 81b6  U...^....W......
+00002290: 07da 1e68 7ba0 ed81 b607 da1e 687b a0ed  ...h{.......h{..
+000022a0: 81b6 07da 1e68 7ba0 ed81 b607 da1e 687b  .....h{.......h{
+000022b0: a0ed 81b6 07da 1e68 7ba0 ed81 b607 da1e  .......h{.......
+000022c0: 687b a0ed 81b6 07da 1e6a 7ba8 ed61 c706  h{.......j{..a..
+000022d0: aded a1b6 87da 1e6a 7ba8 eda1 b687 da1e  .......j{.......
+000022e0: 6a7b a8ed a1b6 87da 1e6a 7ba8 eda1 b687  j{.......j{.....
+000022f0: da1e 6a7b a8ed a1b6 87da 1e6a 7ba8 eda1  ..j{.......j{...
+00002300: b687 da1e 697b a4ed 91b6 47da 1e69 7ba4  ....i{....G..i{.
+00002310: ed91 b647 da1e 697b a4ed 91b6 47da 1e69  ...G..i{....G..i
+00002320: 7ba4 ed91 b647 da1e 697b a4ed 91b6 47da  {....G..i{....G.
+00002330: 1e69 7ba4 ed91 b647 da1e 697b a4ed b1b6  .i{....G..i{....
+00002340: c7da 1e6b 7bac ed71 c7d7 6f6d 8fb5 3dd6  ...k{..q..om..=.
+00002350: f658 db63 6d8f b53d d6f6 58db 636d 8fb5  .X.cm..=..X.cm..
+00002360: 3dd6 f658 db63 6d8f b53d d6f6 58db 636d  =..X.cm..=..X.cm
+00002370: 8fb5 3dd6 f658 db63 6daf 697b 4ddb 6bda  ..=..X.cm.i{M.k.
+00002380: 5ed3 f69a b6d7 3a7e dad2 f69a b6d7 b4bd  ^.....:~........
+00002390: a6ed 356d af69 7b4d db6b da5e d3f6 9ab6  ..5m.i{M.k.^....
+000023a0: d7b4 bda6 ed35 6daf 697b 4ddb 6bda 5ed3  .....5m.i{M.k.^.
+000023b0: f69a b6d7 b4bd a6ed 756d af6b 7b5d dbeb  ........um.k{]..
+000023c0: da5e d7f6 bab6 d7b5 bdae ed75 6daf 6b7b  .^.........um.k{
+000023d0: 5ddb ebda 5ed7 f6ba b6d7 b5bd aeed 756d  ]...^.........um
+000023e0: af6b 7b5d dbeb da5e d7f6 bab6 d7b5 bdae  .k{]...^........
+000023f0: ed75 6daf 6b7b 43db 1bda ded0 f686 b637  .um.k{C........7
+00002400: b4bd a1ed 0d6d 6f68 7b43 db1b dade d0f6  .....moh{C......
+00002410: 86b6 37b4 bda1 ed0d 6d6f 687b 43db 1bda  ..7.....moh{C...
+00002420: ded0 f686 b637 b4bd a1ed 0d6d 6f68 7b43  .....7.....moh{C
+00002430: db1b dade d4f6 a6b6 37b5 bda9 ed4d 6d6f  ........7....Mmo
+00002440: 6a7b 53db 9bda ded4 f6a6 b637 b5bd a9ed  j{S........7....
+00002450: 4d6d 6f6a 7b53 db9b dade d4f6 a6b6 37b5  Mmoj{S........7.
+00002460: bda9 ed4d 6d6f 6a7b 53db 9bda ded4 f6a6  ...Mmoj{S.......
+00002470: b6b7 b4bd a5ed 2d6d 6f69 7b4b db5b dade  ......-moi{K.[..
+00002480: d2f6 96b6 b7b4 bda5 ed2d 6d6f 697b 4bdb  .........-moi{K.
+00002490: 5bda ded2 f696 b6b7 b4bd a5ed 2d6d 6f69  [...........-moi
+000024a0: 7b4b db5b dade d2f6 96b6 b7b4 bda5 ed6d  {K.[...........m
+000024b0: 6d6f 6b7b 5bdb dbda ded6 f6b6 b6b7 b5bd  mok{[...........
+000024c0: aded 6d6d 6f6b 7bbb e317 e3da ded6 f6b6  ..mmok{.........
+000024d0: b6b7 b5bd aded 6d6d 6f6b 7b5b dbdb dade  ......mmok{[....
+000024e0: d6f6 b6b6 b7b5 bdad ed6d 6d6f 6b7b 47db  .........mmok{G.
+000024f0: 3bda ded1 f68e b677 b4bd a3ed 1d6d ef68  ;......w.....m.h
+00002500: 7b47 db3b dade d1f6 4ec7 9f83 687b 47db  {G.;....N...h{G.
+00002510: 3bda ded1 f68e b677 b4bd a3ed 1d6d ef68  ;......w.....m.h
+00002520: 7b47 db3b dade d1f6 8eb6 77b4 bdab ed5d  {G.;......w....]
+00002530: 6def 6a7b 57db bbda ded5 f6ae b677 b5bd  m.j{W........w..
+00002540: abed 5d6d ef6a 7b57 dbbb 1d7f eca5 ed5d  ..]m.j{W.......]
+00002550: 6def 6a7b 57db bbda ded5 f6ae b677 b5bd  m.j{W........w..
+00002560: abed 5d6d ef6a 7b57 dbbb dade d3f6 9eb6  ..]m.j{W........
+00002570: f7b4 bda7 ed3d 6def 697b 4fdb 7bda ded3  .....=m.i{O.{...
+00002580: f69e b6f7 b4bd a7ed 3d6d ef75 fc29 a7b6  ........=m.u.)..
+00002590: f7b4 bda7 ed3d 6def 697b 4fdb 7bda ded3  .....=m.i{O.{...
+000025a0: f69e b6f7 b4bd a7ed 3d6d ef6b 7b5f dbfb  ........=m.k{_..
+000025b0: dade d7f6 beb6 f7b5 bdaf ed7d 6def 6b7b  ...........}m.k{
+000025c0: 5fdb fbda ded7 f6be b6f7 b5bd afed 7d6d  _.............}m
+000025d0: ef6b 7b5f dbfb dade d7f6 beb6 f7b5 bdaf  .k{_............
+000025e0: ed7d 6def 6b7b 5fdb 07da 3ed0 f681 b60f  .}m.k{_...>.....
+000025f0: b47d a0ed 036d 1f68 fb40 db07 da3e d0f6  .}...m.h.@...>..
+00002600: 81b6 0fb4 7da0 ed03 6d1f 68fb 40db 07da  ....}...m.h.@...
+00002610: 3ed0 f681 b60f b47d a0ed 036d 1f68 fb40  >......}...m.h.@
+00002620: db07 da3e d0f6 a1b6 0fb5 7da8 ed43 6d1f  ...>......}..Cm.
+00002630: 6afb 50db 87da 3ed4 f6a1 b60f b57d a8ed  j.P...>......}..
+00002640: 436d 1f6a fb50 db87 da3e d4f6 a1b6 0fb5  Cm.j.P...>......
+00002650: 7da8 ed43 6d1f 6afb 50db 87da 3ed4 f6a1  }..Cm.j.P...>...
+00002660: b60f b57d a4ed 236d 1f69 fb48 db47 da3e  ...}..#m.i.H.G.>
+00002670: d2f6 91b6 8fb4 7da4 ed23 6d1f 69fb 48db  ......}..#m.i.H.
+00002680: 47da 3ed2 f691 b68f b47d a4ed 236d 1f69  G.>......}..#m.i
+00002690: fb48 db47 da3e d2f6 91b6 8fb4 7da4 ed23  .H.G.>......}..#
+000026a0: 6d1f 6bfb 58db c7da 3ed6 f6b1 b68f b57d  m.k.X...>......}
+000026b0: aced 636d 1f6b fb58 dbc7 da3e d6f6 b1b6  ..cm.k.X...>....
+000026c0: 8fb5 7dac ed63 6d1f 6bfb 58db c7da 3ed6  ..}..cm.k.X...>.
+000026d0: f6b1 b68f b57d aced 636d 1f6b fb58 db27  .....}..cm.k.X.'
+000026e0: da3e d1f6 89b6 4fb4 7da2 ed13 6d9f 68fb  .>....O.}...m.h.
+000026f0: 44db 27da 3ed1 f689 b64f b47d a2ed 136d  D.'.>....O.}...m
+00002700: 9f68 fb44 db27 da3e d1f6 89b6 4fb4 7da2  .h.D.'.>....O.}.
+00002710: ed13 6d9f 68fb 44db 27da 3ed1 f6a9 b64f  ..m.h.D.'.>....O
+00002720: b57d aaed 536d 9f6a fb54 dba7 da3e d5f6  .}..Sm.j.T...>..
+00002730: a9b6 4fb5 7daa ed53 6d9f 6afb 54db a7da  ..O.}..Sm.j.T...
+00002740: 3ed5 f6a9 b64f b57d aaed 536d 9f6a fb54  >....O.}..Sm.j.T
+00002750: dba7 da3e d5f6 a9b6 4fb5 7da6 ed33 6d9f  ...>....O.}..3m.
+00002760: 69fb 4cdb 67da 3ed3 f699 b6cf b47d a6ed  i.L.g.>......}..
+00002770: 336d 9f69 fb4c db67 da3e d3f6 99b6 cfb4  3m.i.L.g.>......
+00002780: 7da6 ed33 6d9f 69fb 4cdb 67da 3ed3 f699  }..3m.i.L.g.>...
+00002790: b6cf b47d a6ed 336d 9f6b fb5c dbe7 da3e  ...}..3m.k.\...>
+000027a0: d7f6 b9b6 cfb5 7dae ed73 6d9f 6bfb 5cdb  ......}..sm.k.\.
+000027b0: e7da 3ed7 f6b9 b6cf b57d aeed 736d 9f6b  ..>......}..sm.k
+000027c0: fb5c dbe7 da3e d7f6 b9b6 cfb5 7dae ed73  .\...>......}..s
+000027d0: 6d9f 6bfb 5cdb 17da bed0 f685 b62f b47d  m.k.\......../.}
+000027e0: a1ed 0b6d 5f68 fb42 db17 dabe d0f6 85b6  ...m_h.B........
+000027f0: 2fb4 7da1 ed0b 6d5f 68fb 42db 17da bed0  /.}...m_h.B.....
+00002800: f685 b62f b47d a1ed 0b6d 5f68 fb42 db17  .../.}...m_h.B..
+00002810: dabe d0f6 a5b6 2fb5 7da9 ed4b 6d5f 6afb  ....../.}..Km_j.
+00002820: 52db 97da bed4 f6a5 b62f b57d a9ed 4b6d  R......../.}..Km
+00002830: 5f6a fb52 db97 dabe d4f6 a5b6 2fb5 7da9  _j.R......../.}.
+00002840: ed4b 6d5f 6afb 52db 97da bed4 f6a5 b62f  .Km_j.R......../
+00002850: b55d 75c5 2295 beab 4ae1 5557 2f52 a9bc  .]u."...J.UW/R..
+00002860: ea2a 46ba 9291 ae66 a42b 1ae9 aa46 bab2  .*F....f.+...F..
+00002870: 91ae 6ea4 2b1c e92a 47ba d291 ae76 a42b  ..n.+..*G....v.+
+00002880: 1ee9 aa47 baf2 91ae 7ea4 2b20 a99c 0355  ...G....~.+ ...U
+00002890: 5742 d2d5 9074 4524 1d15 49d5 9191 541d  WB...tE$..I...T.
+000028a0: 1d49 d511 9254 1d25 49d5 9192 541d 2d49  .I...T.%I...T.-I
+000028b0: d511 9354 1d35 49d5 9193 541d 3d49 d511  ...T.5I...T.=I..
+000028c0: 9454 1d45 49d5 9194 541d 4d49 d511 9554  .T.EI...T.MI...T
+000028d0: 1d55 49d5 9195 541d 5d49 d511 9654 1d65  .UI...T.]I...T.e
+000028e0: 49d5 9196 54ab 1df3 a023 2ea9 3aea 92aa  I...T....#..:...
+000028f0: 232f a93a fa92 aa23 30a9 3a0a 93aa 2331  #/.:...#0.:...#1
+00002900: a93a 1a93 aa23 32a9 3a2a 93aa 2333 a93a  .:...#2.:*..#3.:
+00002910: 3a93 aa23 34a9 3a4a 93aa 2335 a93a 5a93  :..#4.:J..#5.:Z.
+00002920: aa23 36a9 3a6a 93aa 2337 c95f c6db ece5  .#6.:j..#7._....
+00002930: daa9 66f3 ef83 f891 54b3 e68b 5493 b8ba  ..f.....T...T...
+00002940: 8321 ae7e 6626 a966 3932 5a2a 47c6 8cac  .!.~f&.f92Z*G...
+00002950: 31b2 cec8 0623 9b8c 6c31 b2cd c80e 23bb  1....#..l1....#.
+00002960: 8cec 31b2 cfc8 0123 878c 1c31 72cc c809  ..1....#...1r...
+00002970: 23a7 8c9c 3172 cec8 0523 978c 64f7 2d65  #...1r...#..d.-e
+00002980: 64f3 6568 e0d0 d021 c566 e3e5 b954 9b6d  d.eh...!.f...T.m
+00002990: 174a b9d9 74a1 d49b 2d17 4ac1 d970 a154  .J..t...-.J..p.T
+000029a0: 9ced 164a c9d9 6ca1 d49c ad16 4ad1 d968  ...J..l.....J..h
+000029b0: a154 9d6d 164a d9d9 644b 2a7b 2c43 dace  .T.m.J..dK*{,C..
+000029c0: 0e0b a5ed ecaf 50da ceee 0aa5 edec ad50  ......P........P
+000029d0: dace ce0a a5ed ecab 50da ceae 0aa5 edec  ........P.......
+000029e0: a950 dace 8e0a a5ed eca7 50da ce6e 0aa5  .P........P..n..
+000029f0: edec a550 dace 4e5a 52d9 4819 d276 b651  ...P..NZR.H..v.Q
+00002a00: 286d 6713 85d2 76b6 5028 6d67 0385 d276  (mg...v.P(mg...v
+00002a10: b64f 286d 67f3 84d2 76b6 4e28 6d27 d584  .O(mg...v.N(m'..
+00002a20: d276 524d 286d 0fb4 9d54 9307 6a3b a926  .vRM(m...T..j;.&
+00002a30: 94b6 936a 9654 524d 86b4 3dd4 7652 4d1e  ...j.TRM..=.vRM.
+00002a40: a8ed a49a 50da 4eaa 09a5 eda4 9a50 da4e  ....P.N......P.N
+00002a50: aa09 a5ed a49a 50da 4eaa 09a5 eda4 9a50  ......P.N......P
+00002a60: da4e aa09 a5ed a49a 50da 4eaa 09a5 eda4  .N......P.N.....
+00002a70: 9a25 9554 9321 6d27 d584 d276 524d 286d  .%.T.!m'...vRM(m
+00002a80: 27d5 84d2 7652 4d28 6d27 d584 d276 524d  '...vRM(m'...vRM
+00002a90: 286d 27d5 84d2 7652 4d28 6d27 d584 d2f6  (m'...vRM(m'....
+00002aa0: 48db 4935 79a0 b693 6a42 693b a966 4925  H.I5y...jBi;.fI%
+00002ab0: d564 48db 4935 a13a be7e 6b3b a926 0fd4  .dH.I5.:.~k;.&..
+00002ac0: 7652 4d28 6d27 d584 d276 524d 286d 27d5  vRM(m'...vRM(m'.
+00002ad0: 84d2 7652 4d28 6d27 d584 d276 524d 286d  ..vRM(m'...vRM(m
+00002ae0: 27d5 84d2 7652 4d28 6d27 d52c a9a4 9a0c  '...vRM(m'.,....
+00002af0: 693b a926 94b6 936a 4269 3ba9 2694 b693  i;.&...jBi;.&...
+00002b00: 6a42 693b a926 94b6 936a 4269 3ba9 2694  jBi;.&...jBi;.&.
+00002b10: b693 6a42 693b a926 94b6 d7b4 9d54 9307  ..jBi;.&.....T..
+00002b20: 6a3b a926 94b6 936a 9654 524d 86b4 9d54  j;.&...j.TRM...T
+00002b30: 134a db49 35a1 3a7e b8d6 7652 4d1e a8ed  .J.I5.:~..vRM...
+00002b40: a49a 50da 4eaa 09a5 eda4 9a50 da4e aa09  ..P.N......P.N..
+00002b50: a5ed a49a 50da 4eaa 09a5 eda4 9a50 da4e  ....P.N......P.N
+00002b60: aa09 a5ed a49a 2595 5493 216d 27d5 84d2  ......%.T.!m'...
+00002b70: 7652 4d28 6d27 d584 d276 524d 286d 27d5  vRM(m'...vRM(m'.
+00002b80: 84d2 7652 4d28 6d27 d584 d276 524d 286d  ..vRM(m'...vRM(m
+00002b90: 27d5 84d2 f686 b693 6af2 406d 27d5 84d2  '.......j.@m'...
+00002ba0: 7652 cd92 4aaa c990 b693 6a42 693b a926  vR..J.....jBi;.&
+00002bb0: 94b6 936a 4269 3ba9 2694 b693 6a42 693b  ...jBi;.&...jBi;
+00002bc0: a926 94b6 936a 4269 3ba9 2694 b693 6a42  .&...jBi;.&...jB
+00002bd0: 697b 53db 4935 79a0 b693 6a42 693b a966  i{S.I5y...jBi;.f
+00002be0: 4925 d564 48db 4935 a1b4 9d54 134a db49  I%.dH.I5...T.J.I
+00002bf0: 35a1 b49d 5413 4adb 4935 a1b4 9d54 134a  5...T.J.I5...T.J
+00002c00: db49 35a1 b49d 5413 4adb 4935 a1b4 bda5  .I5...T.J.I5....
+00002c10: eda4 9a3c 50db 4935 a1b4 9d54 b3a4 926a  ...<P.I5...T...j
+00002c20: 32a4 eda4 9a50 da4e aa09 a5ed a49a 50da  2....P.N......P.
+00002c30: 4eaa 09d5 f18b 716d 27d5 e481 da4e aa09  N.....qm'....N..
+00002c40: a5ed a49a 50da 4eaa 09a5 eda4 9a50 da4e  ....P.N......P.N
+00002c50: aa09 a5ed a49a 50da 4eaa 5952 4935 19d2  ......P.N.YRI5..
+00002c60: 7652 4d28 6d27 d584 d276 524d 286d 27d5  vRM(m'...vRM(m'.
+00002c70: 84d2 7652 4d28 6d27 d584 d276 524d 286d  ..vRM(m'...vRM(m
+00002c80: 27d5 84d2 7652 4d28 6d27 d584 d276 524d  '...vRM(m'...vRM
+00002c90: 286d 27d5 2ca9 a49a 0c69 3ba9 2694 b693  (m'.,....i;.&...
+00002ca0: 6a42 693b a926 94b6 936a 4269 3ba9 2694  jBi;.&...jBi;.&.
+00002cb0: b693 6a42 693b a926 94b6 936a 4269 3ba9  ..jBi;.&...jBi;.
+00002cc0: 2694 b693 6a42 693b a926 94b6 936a 4269  &...jBi;.&...jBi
+00002cd0: 3ba9 6649 25d5 6448 db49 35a1 b49d 5413  ;.fI%.dH.I5...T.
+00002ce0: 4adb 4935 a1b4 9d54 134a db49 35a1 b49d  J.I5...T.J.I5...
+00002cf0: 5413 4adb 4935 a1b4 9d54 134a db49 35a1  T.J.I5...T.J.I5.
+00002d00: b49d 5413 4adb 4935 a1b4 9d54 b3a4 926a  ..T.J.I5...T...j
+00002d10: 32a4 eda4 9a50 da4e aa09 a5ed a49a 50da  2....P.N......P.
+00002d20: 4eaa 09a5 eda4 9a50 da4e aa09 a5ed a49a  N......P.N......
+00002d30: 50da 4eaa 09a5 eda4 9a50 da4e aa09 a5ed  P.N......P.N....
+00002d40: a49a 50da 4eaa 09a5 eda4 9a25 9554 9321  ..P.N......%.T.!
+00002d50: 6d27 d584 d276 524d 286d 27d5 84d2 7652  m'...vRM(m'...vR
+00002d60: 4d28 6d27 d584 d276 524d 286d 27d5 84d2  M(m'...vRM(m'...
+00002d70: 7652 4d28 6d27 d584 d2f6 81b6 936a f240  vRM(m'.......j.@
+00002d80: 6d27 d584 d276 52cd 924a aac9 90b6 936a  m'...vR..J.....j
+00002d90: 4269 3ba9 2694 b693 6a42 693b a926 94b6  Bi;.&...jBi;.&..
+00002da0: 936a 4269 3ba9 2694 b693 6a42 693b a926  .jBi;.&...jBi;.&
+00002db0: 94b6 936a 4269 fb50 db49 3579 a0b6 936a  ...jBi.P.I5y...j
+00002dc0: 4269 3ba9 6649 25d5 6448 db49 35a1 b49d  Bi;.fI%.dH.I5...
+00002dd0: 5413 4adb 4935 a1b4 9d54 134a db49 35a1  T.J.I5...T.J.I5.
+00002de0: b49d 5413 4adb 4935 a1b4 9d54 134a db49  ..T.J.I5...T.J.I
+00002df0: 35a1 b49d 5413 4adb 4935 a1b4 9d54 b3a4  5...T.J.I5...T..
+00002e00: 926a 32a4 eda4 9a50 da4e aa09 a5ed a49a  .j2....P.N......
+00002e10: 50da 4eaa 09a5 eda4 9a50 da4e aa09 a5ed  P.N......P.N....
+00002e20: a49a 50da 4eaa 09a5 eda4 9a50 da4e aa09  ..P.N......P.N..
+00002e30: a5ed a49a 50da 4eaa 09a5 eda4 9a25 9554  ....P.N......%.T
+00002e40: 9321 6d27 d584 d276 524d 286d 27d5 84d2  .!m'...vRM(m'...
+00002e50: 7652 4d28 6d27 d584 d276 524d 286d 27d5  vRM(m'...vRM(m'.
+00002e60: 84d2 7652 4d28 6d27 d584 d276 524d 286d  ..vRM(m'...vRM(m
+00002e70: 27d5 84d2 7652 cd92 4aaa c990 b693 6a42  '...vR..J.....jB
+00002e80: 693b a926 94b6 936a 4269 3ba9 2694 b693  i;.&...jBi;.&...
+00002e90: 6a42 693b a926 94b6 936a 4269 3ba9 2694  jBi;.&...jBi;.&.
+00002ea0: b693 6a42 693b a926 94b6 936a 4269 3ba9  ..jBi;.&...jBi;.
+00002eb0: 2694 b693 6a96 5452 4d86 b49d 5413 4adb  &...j.TRM...T.J.
+00002ec0: 4935 a1b4 9d54 134a db49 35a1 b49d 5413  I5...T.J.I5...T.
+00002ed0: 4adb 4935 a1b4 9d54 134a db49 35a1 b49d  J.I5...T.J.I5...
+00002ee0: 5413 4adb 4935 a1b4 9d54 134a db49 354b  T.J.I5...T.J.I5K
+00002ef0: 2aa9 2643 da4e aa09 a5ed a49a 50da 4eaa  *.&C.N......P.N.
+00002f00: 09a5 eda4 9a50 da4e aa09 a5ed a49a 50da  .....P.N......P.
+00002f10: 4eaa 09a5 eda4 9a50 da4e aa09 a5ed a49a  N......P.N......
+00002f20: 50da 4eaa 09a5 eda4 9a50 da4e aa59 5249  P.N......P.N.YRI
+00002f30: 3519 d276 524d 286d 27d5 84d2 7652 4d28  5..vRM(m'...vRM(
+00002f40: 6d27 d584 d276 524d 286d 27d5 84d2 7652  m'...vRM(m'...vR
+00002f50: 4d28 6d27 d584 d276 524d 286d 27d5 84d2  M(m'...vRM(m'...
+00002f60: 7652 4d28 6d27 d52c a9a4 9a0c 693b a926  vRM(m'.,....i;.&
+00002f70: 94b6 936a 4269 3ba9 2694 b693 6a42 693b  ...jBi;.&...jBi;
+00002f80: a926 94b6 936a 4269 3ba9 2694 b693 6a42  .&...jBi;.&...jB
+00002f90: 693b a926 94b6 936a 4269 3ba9 2694 b693  i;.&...jBi;.&...
+00002fa0: 6a42 69bb 4e35 4bac eaaa 4592 6aca 69bc  jBi.N5K...E.j.i.
+00002fb0: 4aaa 29a7 f32a a9a6 9cd6 aba4 9a72 7aaf  J.)..*.......rz.
+00002fc0: 926a ca69 be4a aa29 a7fb 2aa9 a69c f6ab  .j.i.J.)..*.....
+00002fd0: a49a 72fa af92 6aca 3903 aaa4 9a72 ce81  ..r...j.9....r..
+00002fe0: 3ad5 9473 1654 4935 e53a e641 4746 52a7  :..s.TI5.:.AGFR.
+00002ff0: 9a3c b623 24a9 534d b98e 7990 5453 ae63  .<.#$.SM..y.TS.c
+00003000: 1e24 d594 eb98 0749 35e5 3ae6 4152 4db9  .$.....I5.:.ARM.
+00003010: 8e79 9054 53ae 631e 24d5 94eb 9807 4935  .y.TS.c.$.....I5
+00003020: e53a e641 524d b98e 7990 5453 ae63 1e24  .:.ARM..y.TS.c.$
+00003030: d594 eb98 0749 35e1 3a02 933a d594 eb58  .....I5.:..:...X
+00003040: 0f3a 1a93 3ad5 f4b1 1df3 20a9 a65c c73c  .:..:..... ..\.<
+00003050: 48aa 29d7 310f 926a ca75 cc83 a49a 721d  H.).1..j.u....r.
+00003060: f320 a9a6 5c6b 1eb4 53cd e6bd 847f 24d5  . ..\k..S.....$.
+00003070: 7cba 8770 f3ee abe5 c860 a91c 1932 3262  |..p.....`...22b
+00003080: 64cc c81a 23eb 8c6c 30b2 c9c8 1623 db8c  d...#..l0....#..
+00003090: ec30 b2cb c81e 23fb 8c1c 3072 c8c8 1123  .0....#...0r...#
+000030a0: c78c 9c30 72ca c819 23e7 8c5c 3072 c948  ...0r...#..\0r.H
+000030b0: 76d6 5258 3656 86d4 9abf 0101 4ab1 c930  v.RX6V......J..0
+000030c0: a154 9b0c 134a b9c9 30a1 d49b 0c13 4ac1  .T...J..0.....J.
+000030d0: c930 a154 9c0c 134a c9c9 30a1 d49c 0c13  .0.T...J..0.....
+000030e0: 4ad1 c930 a154 9d0c 134a d9c9 30b9 5eb5  J..0.T...J..0.^.
+000030f0: 9ded 134a dbd9 3ca1 b49d ad13 4adb d938  ...J..<.....J..8
+00003100: a1b4 9d6d 134a dbd9 34a1 b49d 2d13 4adb  ...m.J..4...-.J.
+00003110: d930 a1b4 9ded 124a dbd9 2ca1 b49d ad12  .0.....J..,.....
+00003120: 4adb d928 a1b4 9d6d b2a4 b24b 32a4 edfc  J..(...m...K2...
+00003130: 7506 50da ce0e 09a5 edec 8f50 dace ee08  u.P........P....
+00003140: a5ed ec8d 50da cece 08a5 edec 8b50 dace  ....P........P..
+00003150: 1d33 a1b4 9d3b 6642 693b 77cc 84d2 7632  .3...;fBi;w...v2
+00003160: 4c28 6d27 c384 d276 32cc 924a 86c9 50c7  L(m'...v2..J..P.
+00003170: 06ad ed64 983c 50db c930 a1b4 9d0c 134a  ...d.<P..0.....J
+00003180: dbc9 30a1 b49d 0c13 4adb c930 a1b4 9d0c  ..0.....J..0....
+00003190: 134a dbc9 30a1 b49d 0c13 4adb c930 a1b4  .J..0.....J..0..
+000031a0: 9d0c 134a dbc9 304b 2a19 2643 da4e 8609  ...J..0K*.&C.N..
+000031b0: a5ed 6498 50da 4e86 09a5 ed64 9850 da4e  ..d.P.N....d.P.N
+000031c0: 8609 a5ed 6498 50da 4e86 09a5 ed64 9850  ....d.P.N....d.P
+000031d0: da4e 8609 a5ed 6498 50da ce1d 33a1 b49d  .N....d.P...3...
+000031e0: 3b66 9654 324c 86b4 9d3b 6642 693b 77cc  ;f.T2L...;fBi;w.
+000031f0: 84d2 7632 4c28 6d27 c384 d276 324c 286d  ..v2L(m'...v2L(m
+00003200: 27c3 84d2 7632 4c28 6d27 c384 d276 324c  '...v2L(m'...v2L
+00003210: 286d 27c3 84d2 7632 4c28 6d27 c384 d276  (m'...v2L(m'...v
+00003220: 32cc 924a 86c9 90b6 9361 4269 3b19 2694  2..J.....aBi;.&.
+00003230: b693 6142 693b 1926 94b6 9361 4269 3b19  ..aBi;.&...aBi;.
+00003240: 2694 b693 6142 693b 1926 94b6 9361 4269  &...aBi;.&...aBi
+00003250: 3b19 2694 b673 c74c 286d e78e 9925 950c  ;.&..s.L(m...%..
+00003260: 9321 6de7 8e99 50da ce1d 33a1 b49d 3b66  .!m...P...3...;f
+00003270: 4269 3b19 2694 b693 6142 693b 1926 94b6  Bi;.&...aBi;.&..
+00003280: 9361 4269 3b19 2694 b693 6142 693b 1926  .aBi;.&...aBi;.&
+00003290: 94b6 9361 4269 3b19 2694 b693 6196 5432  ...aBi;.&...a.T2
+000032a0: 4c86 b49d 0c13 4adb c930 a1b4 9d0c 134a  L.....J..0.....J
+000032b0: dbc9 30a1 b49d 0c13 4adb c930 a1b4 9d0c  ..0.....J..0....
+000032c0: 134a dbc9 30a1 b49d 0c13 4adb c930 a1b4  .J..0.....J..0..
+000032d0: 9d3b 6642 693b 77cc 2ca9 6498 0c69 3b77  .;fBi;w.,.d..i;w
 000032e0: cc84 d276 ee98 09a5 eddc 3113 4adb b963  ...v......1.J..c
-000032f0: 2694 b673 c74c 286d 27c3 84d2 7632 4c28  &..s.L(m'...v2L(
-00003300: 6d27 c32c a964 980c 693b 1926 94b6 9361  m'.,.d..i;.&...a
-00003310: 4269 3b19 2694 b693 6142 693b 1926 94b6  Bi;.&...aBi;.&..
-00003320: 9361 4269 3b19 2694 b693 6142 693b 1926  .aBi;.&...aBi;.&
-00003330: 94b6 9361 4269 3b77 cc84 d276 ee98 5952  ...aBi;w...v..YR
-00003340: c930 19d2 76ee 9809 a5ed dc31 134a dbb9  .0..v......1.J..
-00003350: 6326 94b6 73c7 4c28 6de7 8e99 50da 4e86  c&..s.L(m...P.N.
-00003360: 09a5 ed64 9850 da4e 8609 a5ed 6498 50da  ...d.P.N....d.P.
-00003370: 4e86 09a5 ed64 9850 da4e 8609 a5ed 6498  N....d.P.N....d.
-00003380: 2595 0c93 216d 27c3 84d2 7632 4c28 6d27  %...!m'...v2L(m'
-00003390: c384 d276 324c 286d 27c3 84d2 7632 4c28  ...v2L(m'...v2L(
-000033a0: 6d27 c384 d276 324c 286d 27c3 84d2 7632  m'...v2L(m'...v2
-000033b0: 4c28 6d27 c384 d276 32cc 924a 86c9 90b6  L(m'...v2..J....
-000033c0: 9361 4269 3b19 2694 b693 6142 693b 1926  .aBi;.&...aBi;.&
-000033d0: 94b6 9361 4269 3b19 2694 b693 6142 693b  ...aBi;.&...aBi;
-000033e0: 1926 94b6 9361 4269 3b19 2694 b693 6142  .&...aBi;.&...aB
-000033f0: 693b 1926 94b6 9361 9654 324c 86b4 9d0c  i;.&...a.T2L....
-00003400: 134a dbc9 30a1 b49d 0c13 4adb c930 a1b4  .J..0.....J..0..
-00003410: 9d0c 134a dbc9 30a1 b49d 0c13 4adb c930  ...J..0.....J..0
-00003420: a1b4 9d0c 134a dbc9 30a1 b49d 0c13 4adb  .....J..0.....J.
-00003430: c930 4b2a 1926 43da 4e86 09a5 ed64 9850  .0K*.&C.N....d.P
-00003440: da4e 8609 a5ed 6498 50da 4e86 09a5 ed64  .N....d.P.N....d
-00003450: 9850 da4e 8609 a5ed 6498 50da 4e86 09a5  .P.N....d.P.N...
-00003460: ed64 9850 da4e 8609 a5ed 6498 50da 4e86  .d.P.N....d.P.N.
-00003470: 5952 c930 19d2 7632 4c28 6d27 c384 d276  YR.0..v2L(m'...v
-00003480: 324c 286d 27c3 84d2 7632 4c28 6d27 c384  2L(m'...v2L(m'..
-00003490: d276 324c 286d 27c3 84d2 7632 4c28 6d27  .v2L(m'...v2L(m'
-000034a0: c384 d276 ee98 09a5 eddc 31b3 a492 6132  ...v......1...a2
-000034b0: a4ed dc31 134a dbb9 6326 94b6 73c7 4c28  ...1.J..c&..s.L(
-000034c0: 6de7 8e99 50da ce1d 33a1 b49d 3b66 4269  m...P...3...;fBi
+000032f0: 2694 b673 c74c 286d e78e 9950 dace 1d33  &..s.L(m...P...3
+00003300: a1b4 9d3b 6642 693b 77cc 84d2 76ee 9809  ...;fBi;w...v...
+00003310: a5ed 6498 50da 4e86 09a5 ed64 9825 950c  ..d.P.N....d.%..
+00003320: 9321 6d27 c384 d276 324c 286d 27c3 84d2  .!m'...v2L(m'...
+00003330: 7632 4c28 6d27 c384 d276 324c 286d 27c3  v2L(m'...v2L(m'.
+00003340: 84d2 7632 4c28 6d27 c384 d276 324c 286d  ..v2L(m'...v2L(m
+00003350: e78e 9950 dace 1d33 4b2a 1926 43da ce1d  ...P...3K*.&C...
+00003360: 33a1 b49d 3b66 4269 3b77 cc84 d276 ee98  3...;fBi;w...v..
+00003370: 09a5 eddc 3113 4adb c930 a1b4 9d0c 134a  ....1.J..0.....J
+00003380: dbc9 30a1 b49d 0c13 4adb c930 a1b4 9d0c  ..0.....J..0....
+00003390: 134a dbc9 30a1 b49d 0cb3 a492 6132 a4ed  .J..0.......a2..
+000033a0: 6498 50da 4e86 09a5 ed64 9850 da4e 8609  d.P.N....d.P.N..
+000033b0: a5ed 6498 50da 4e86 09a5 ed64 9850 da4e  ..d.P.N....d.P.N
+000033c0: 8609 a5ed 6498 50da 4e86 09a5 ed64 9850  ....d.P.N....d.P
+000033d0: da4e 8659 52c9 3019 d276 324c 286d 27c3  .N.YR.0..v2L(m'.
+000033e0: 84d2 7632 4c28 6d27 c384 d276 324c 286d  ..v2L(m'...v2L(m
+000033f0: 27c3 84d2 7632 4c28 6d27 c384 d276 324c  '...v2L(m'...v2L
+00003400: 286d 27c3 84d2 7632 4c28 6d27 c384 d276  (m'...v2L(m'...v
+00003410: 32cc 924a 86c9 90b6 9361 4269 3b19 2694  2..J.....aBi;.&.
+00003420: b693 6142 693b 1926 94b6 9361 4269 3b19  ..aBi;.&...aBi;.
+00003430: 2694 b693 6142 693b 1926 94b6 9361 4269  &...aBi;.&...aBi
+00003440: 3b19 2694 b693 6142 693b 1966 4925 c364  ;.&...aBi;.fI%.d
+00003450: 48db c930 a1b4 9d0c 134a dbc9 30a1 b49d  H..0.....J..0...
+00003460: 0c13 4adb c930 a1b4 9d0c 134a dbc9 30a1  ..J..0.....J..0.
+00003470: b49d 0c13 4adb c930 a1b4 9d0c 134a dbc9  ....J..0.....J..
+00003480: 30a1 b49d 0c13 4adb c930 4b2a 1926 43da  0.....J..0K*.&C.
+00003490: 4e86 09a5 ed64 9850 da4e 8609 a5ed 6498  N....d.P.N....d.
+000034a0: 50da 4e86 09a5 ed64 9850 da4e 8609 a5ed  P.N....d.P.N....
+000034b0: 6498 50da 4e86 09a5 ed64 9850 dace 1d33  d.P.N....d.P...3
+000034c0: a1b4 9d3b 6696 5432 4c86 b49d 3b66 4269  ...;f.T2L...;fBi
 000034d0: 3b77 cc84 d276 ee98 09a5 eddc 3113 4adb  ;w...v......1.J.
-000034e0: b963 2694 b693 6142 693b 1926 94b6 9361  .c&...aBi;.&...a
-000034f0: 9654 324c 86b4 9d0c 134a dbc9 30a1 b49d  .T2L.....J..0...
-00003500: 0c13 4adb c930 a1b4 9d0c 134a dbc9 30a1  ..J..0.....J..0.
-00003510: b49d 0c13 4adb c930 a1b4 9d0c 134a dbc9  ....J..0.....J..
-00003520: 30a1 b49d 0c13 4adb c930 4b2a 1926 43da  0.....J..0K*.&C.
-00003530: 4e86 09a5 ed64 9850 da4e 8609 a5ed 6498  N....d.P.N....d.
-00003540: 50da 4e86 09a5 ed64 9850 da4e 8609 a5ed  P.N....d.P.N....
-00003550: 6498 50da 4e86 09a5 ed64 9850 da4e 8609  d.P.N....d.P.N..
-00003560: a5ed 6498 50da 4e86 5952 c930 19d2 7632  ..d.P.N.YR.0..v2
-00003570: 4c28 6d27 c384 d276 324c 286d 27c3 84d2  L(m'...v2L(m'...
-00003580: 7632 4c28 6d27 c384 d276 324c 286d 27c3  v2L(m'...v2L(m'.
-00003590: 84d2 7632 4c28 6d27 c384 d276 324c 286d  ..v2L(m'...v2L(m
-000035a0: 27c3 2ca9 6498 0c69 3b19 2694 b693 6142  '.,.d..i;.&...aB
-000035b0: 693b 1926 94b6 9361 4269 3b19 2694 b693  i;.&...aBi;.&...
-000035c0: 6142 693b 1926 94b6 9361 4269 3b19 2694  aBi;.&...aBi;.&.
-000035d0: b693 6142 693b 1926 94b6 9361 4269 3b19  ..aBi;.&...aBi;.
-000035e0: 6649 25c3 6448 dbc9 30a1 b49d 0c13 4adb  fI%.dH..0.....J.
-000035f0: c930 a1b4 9d0c 134a dbc9 30a1 b49d 0c13  .0.....J..0.....
-00003600: 4adb c930 a1b4 9d0c 134a dbc9 30a1 b49d  J..0.....J..0...
-00003610: 0c13 4adb c930 a1b4 9d0c b3a4 9261 32a4  ..J..0.......a2.
-00003620: ed64 9850 da4e 8609 a5ed 6498 50da 4e86  .d.P.N....d.P.N.
-00003630: 09a5 ed64 9850 da4e 8609 a5ed 6498 50da  ...d.P.N....d.P.
-00003640: 4e86 09a5 ed64 9850 da4e 8609 a5ed 6498  N....d.P.N....d.
-00003650: 50da 4e86 09a5 ed64 9825 950c 9321 6d27  P.N....d.%...!m'
-00003660: c384 d276 324c 286d 27c3 84d2 7632 4c28  ...v2L(m'...v2L(
-00003670: 6d27 c384 d276 324c 286d 27c3 84d2 7632  m'...v2L(m'...v2
-00003680: 4c28 6d27 c384 d276 324c 286d 27c3 84d2  L(m'...v2L(m'...
-00003690: 7632 cc92 4a86 c990 b693 6142 693b 1926  v2..J.....aBi;.&
-000036a0: 94b6 9361 4269 3b19 2694 b693 6142 693b  ...aBi;.&...aBi;
-000036b0: 1926 94b6 9361 4269 3b19 2694 b693 6142  .&...aBi;.&...aB
-000036c0: 693b 1926 94b6 9361 4269 3b19 2694 b6eb  i;.&...aBi;.&...
-000036d0: 0cb3 c4ea 0cd3 3185 d777 cc94 5379 7dc7  ......1..w..Sy}.
-000036e0: 4c39 a557 5dcd 4832 4c1f abf7 3ac3 94d3  L9.W].H2L...:...
-000036f0: 7c9d 61ca e9be ce30 e5b4 5f67 9872 faaf  |.a....0.._g.r..
-00003700: 334c 3967 409d 61ca 3907 ea0c 53ce 5950  3L9g@.a.9...S.YP
-00003710: 6798 721d f320 1926 5c47 4752 df31 53ae  g.r.. .&\GGR.1S.
-00003720: 631e e48e 5e72 1df3 20f7 f492 f3ea afef  c...^r.. .......
-00003730: 9829 d731 0f72 5f2f b98e 7990 3b7b c975  .).1.r_/..y.;{.u
-00003740: cc83 dcdb 4bae 631e e4ee 5e72 1df3 20f7  ....K.c...^r.. .
-00003750: f792 eb98 07b9 c397 5cc7 3cc8 3dbe e43a  ........\.<.=..:
-00003760: e641 eef2 25d7 310f 3a02 933a c3e4 b11d  .A..%.1.:..:....
-00003770: 8949 7dc7 4cb9 8e79 909b 7dc9 75cc 83dc  .I}.L..y..}.u...
-00003780: ee4b ae63 1ee4 865f 721d f320 b7fc 92eb  .K.c..._r.. ....
-00003790: 9807 b9e9 975c c73c c86d bf1a 5c3b c3fc  .....\.<.m..\;..
-000037a0: 903b 607e bbfa 9abb 60f6 7e7e ca30 ff78  .;`~....`.~~.0.x
-000037b0: cc3f aefc b4bc 38f3 eedf bd85 abeb 9f3f  .?....8........?
-000037c0: fd67 70f3 707d f335 e3b3 3fcd cffc facb  .gp.p}.5..?.....
-000037d0: f5bb fb8f 33d5 52fd c88f 330b 33ef 72e0  ....3.R...3.3.r.
-000037e0: 21c3 7ffe 3a3f 3ff7 cbfb 3f7f fde5 fdf5  !...:??...?.....
-000037f0: 7768 f53b 34ae 36fb 8c0c 1819 3232 6264  wh.;4.6.....22bd
-00003800: 8d91 7546 3618 d964 648b 916d 4676 18d9  ..uF6..dd..mFv..
-00003810: 6564 8f91 7d46 0e18 3964 e488 9163 464e  ed..}F..9d...cFN
-00003820: 1839 65e4 8c91 7346 2e18 b964 24db eeb3  .9e...sF...d$...
-00003830: e7b1 c2ec ba0c a935 7b2e 9462 b3e3 42a9  .......5{..b..B.
-00003840: 36fb 2d94 72d3 6842 a937 8d26 9482 d368  6.-.r.hB.7.&...h
-00003850: 42a9 388d 2694 92d3 6842 a939 8d26 94a2  B.8.&...hB.9.&..
-00003860: d368 42a9 3a8d 2694 b2d3 6896 5436 5786  .hB.:.&...h.T6W.
-00003870: b49d ad15 4adb d958 a1b4 9d6d 154a dbd9  ....J..X...m.J..
-00003880: 54a1 b49d 2d15 4adb d950 a1b4 9ded 144a  T...-.J..P.....J
-00003890: dbd9 4ca1 b49d ad14 4adb d948 a1b4 9d6d  ..L.....J..H...m
-000038a0: 144a dbd9 44a1 b49d 2db4 a4b2 8332 a4ed  .J..D...-....2..
-000038b0: ec9f 50da ceee 09a5 edec 9d50 dace ce09  ..P........P....
-000038c0: a5ed ec9b 50da ceae 09a5 edec 9950 dace  ....P........P..
-000038d0: ad32 a1b4 9d5b 6542 693b b7ca 84d2 765f  .2...[eBi;....v_
-000038e0: db69 3479 a0b6 d368 9654 1a4d 863a 3668  .i4y...h.T.M.:6h
-000038f0: 6da7 d1e4 81da 4ea3 09a5 ed34 9a50 da4e  m.....N....4.P.N
-00003900: a309 a5ed 349a 50da 4ea3 09a5 ed34 9a50  ....4.P.N....4.P
-00003910: da4e a309 a5ed 349a 50da 4ea3 09a5 ed34  .N....4.P.N....4
-00003920: 9a50 da4e a359 5269 3419 d276 1a4d 286d  .P.N.YRi4..v.M(m
-00003930: a7d1 84d2 761a 4d28 6da7 d184 d276 1a4d  ....v.M(m....v.M
-00003940: 286d a7d1 84d2 761a 4d28 6da7 d184 d276  (m....v.M(m....v
-00003950: 1a4d 286d a7d1 84d2 761a 4d28 6da7 d12c  .M(m....v.M(m..,
-00003960: a934 9a0c 693b 8d26 94b6 d368 4269 3b8d  .4..i;.&...hBi;.
-00003970: 2694 b6d3 6842 693b 8d26 94b6 d368 4269  &...hBi;.&...hBi
-00003980: 3b8d 2694 b6d3 6842 693b 8d26 94b6 d368  ;.&...hBi;.&...h
-00003990: 4269 3b8d 2694 b6d3 6842 693b 8d66 49a5  Bi;.&...hBi;.fI.
-000039a0: d164 48db 6934 a1b4 9d46 134a db69 34a1  .dH.i4...F.J.i4.
-000039b0: b49d 4613 4adb 6934 a1b4 9d46 134a db69  ..F.J.i4...F.J.i
-000039c0: 34a1 b49d 4613 4adb 6934 a1b4 9d46 134a  4...F.J.i4...F.J
-000039d0: db69 34a1 b49d 46b3 a4d2 6832 a4ed 349a  .i4...F...h2..4.
-000039e0: 50da 4ea3 09a5 ed34 9a50 da4e a309 a5ed  P.N....4.P.N....
-000039f0: 349a 50da 4ea3 09a5 ed34 9a50 da4e a309  4.P.N....4.P.N..
-00003a00: a5ed 349a 50da 4ea3 09a5 ed34 9a50 da4e  ..4.P.N....4.P.N
-00003a10: a309 a5ed 349a 2595 4693 216d a7d1 84d2  ....4.%.F.!m....
-00003a20: 761a 4d28 6da7 d184 d276 1a4d 286d a7d1  v.M(m....v.M(m..
-00003a30: 84d2 761a 4d28 6da7 d184 d276 1a4d 286d  ..v.M(m....v.M(m
-00003a40: a7d1 84d2 761a 4d28 6da7 d184 d276 1acd  ....v.M(m....v..
-00003a50: 924a a3c9 90b6 d368 4269 3b8d 2694 b6d3  .J.....hBi;.&...
-00003a60: 6842 693b 8d26 94b6 d368 4269 3b8d 2694  hBi;.&...hBi;.&.
-00003a70: b6d3 6842 693b 8d26 94b6 d368 4269 3b8d  ..hBi;.&...hBi;.
-00003a80: 2694 b6d3 6842 693b 8d26 94b6 d368 9654  &...hBi;.&...h.T
-00003a90: 1a4d 86b4 9d46 134a db69 34a1 b49d 4613  .M...F.J.i4...F.
-00003aa0: 4adb 6934 a1b4 9d46 134a db69 34a1 b49d  J.i4...F.J.i4...
-00003ab0: 4613 4adb 6934 a1b4 9d46 134a db69 34a1  F.J.i4...F.J.i4.
-00003ac0: b49d 4613 4adb 6934 4b2a 8d26 43da 4ea3  ..F.J.i4K*.&C.N.
-00003ad0: 09a5 ed34 9a50 da4e a309 a5ed 349a 50da  ...4.P.N....4.P.
-00003ae0: 4ea3 09a5 ed34 9a50 da4e a309 a5ed 349a  N....4.P.N....4.
-00003af0: 50da 4ea3 09a5 ed34 9a50 da4e a309 a5ed  P.N....4.P.N....
-00003b00: 349a 50da 4ea3 5952 6934 19d2 761a 4d28  4.P.N.YRi4..v.M(
-00003b10: 6da7 d184 d276 1a4d 286d a7d1 84d2 761a  m....v.M(m....v.
-00003b20: 4d28 6da7 d184 d276 1a4d 286d a7d1 84d2  M(m....v.M(m....
-00003b30: 761a 4d28 6da7 d184 d276 1a4d 286d a7d1  v.M(m....v.M(m..
-00003b40: 2ca9 349a 0c69 3b8d 2694 b6d3 6842 693b  ,.4..i;.&...hBi;
-00003b50: 8d26 94b6 d368 4269 3b8d 2694 b6d3 6842  .&...hBi;.&...hB
-00003b60: 693b 8d26 94b6 d368 4269 3b8d 2694 b6d3  i;.&...hBi;.&...
-00003b70: 6842 693b 8d26 94b6 d368 4269 3b8d 6649  hBi;.&...hBi;.fI
-00003b80: a5d1 6448 db69 34a1 b49d 4613 4adb 6934  ..dH.i4...F.J.i4
-00003b90: a1b4 9d46 134a db69 34a1 b49d 4613 4adb  ...F.J.i4...F.J.
-00003ba0: 6934 a1b4 9d46 134a db69 34a1 b49d 4613  i4...F.J.i4...F.
-00003bb0: 4adb 6934 a1b4 9d46 b3a4 d268 32a4 ed34  J.i4...F...h2..4
-00003bc0: 9a50 da4e a309 a5ed 349a 50da 4ea3 09a5  .P.N....4.P.N...
-00003bd0: ed34 9a50 da4e a309 a5ed 349a 50da 4ea3  .4.P.N....4.P.N.
-00003be0: 09a5 ed34 9a50 da4e a309 a5ed 349a 50da  ...4.P.N....4.P.
-00003bf0: 4ea3 09a5 ed34 9a25 9546 9321 6da7 d184  N....4.%.F.!m...
-00003c00: d276 1a4d 286d a7d1 84d2 761a 4d28 6da7  .v.M(m....v.M(m.
-00003c10: d184 d276 1a4d 286d a7d1 84d2 761a 4d28  ...v.M(m....v.M(
-00003c20: 6da7 d184 d276 1a4d 286d a7d1 84d2 761a  m....v.M(m....v.
-00003c30: cd92 4aa3 c990 b6d3 6842 693b 8d26 94b6  ..J.....hBi;.&..
-00003c40: d368 4269 3b8d 2694 b6d3 6842 693b 8d26  .hBi;.&...hBi;.&
-00003c50: 94b6 d368 4269 3b8d 2694 b6d3 6842 693b  ...hBi;.&...hBi;
-00003c60: 8d26 94b6 d368 4269 3b8d 2694 b6d3 6896  .&...hBi;.&...h.
-00003c70: 541a 4d86 b49d 4613 4adb 6934 a1b4 9d46  T.M...F.J.i4...F
-00003c80: 134a db69 34a1 b49d 4613 4adb 6934 a1b4  .J.i4...F.J.i4..
-00003c90: 9d46 134a db69 34a1 b49d 4613 4adb 6934  .F.J.i4...F.J.i4
-00003ca0: a1b4 9d46 134a db69 344b 2a8d 2643 da4e  ...F.J.i4K*.&C.N
-00003cb0: a309 a5ed 349a 50da 4ea3 09a5 ed34 9a50  ....4.P.N....4.P
-00003cc0: da4e a309 a5ed 349a 50da 4ea3 09a5 ed34  .N....4.P.N....4
-00003cd0: 9a50 da4e a309 a5ed 349a 50da 4ea3 09a5  .P.N....4.P.N...
-00003ce0: ed34 9a50 da4e a359 5269 3419 d276 1a4d  .4.P.N.YRi4..v.M
-00003cf0: 286d a7d1 84d2 761a 4d28 6da7 d184 d276  (m....v.M(m....v
-00003d00: 1a4d 286d a7d1 84d2 761a 4d28 6da7 d184  .M(m....v.M(m...
-00003d10: d276 1a4d 286d a7d1 84d2 761a 4d28 6da7  .v.M(m....v.M(m.
-00003d20: d12c a934 9a0c 693b 8d26 94b6 d368 4269  .,.4..i;.&...hBi
-00003d30: 3b8d 2694 b6d3 6842 693b 8d26 94b6 d368  ;.&...hBi;.&...h
-00003d40: 4269 3b8d 2694 b6d3 6842 693b 8d26 94b6  Bi;.&...hBi;.&..
-00003d50: d368 4269 3b8d 2694 b6d3 6842 693b 8d66  .hBi;.&...hBi;.f
-00003d60: 49a5 d164 48db 6934 a1b4 9d46 134a db69  I..dH.i4...F.J.i
-00003d70: 34a1 b49d 4613 4adb 6934 a1b4 9d46 134a  4...F.J.i4...F.J
-00003d80: db69 34a1 b49d 4613 4adb 6934 a1b4 9d46  .i4...F.J.i4...F
-00003d90: 134a db69 34a1 b49d 46b3 a4d2 6832 a4ed  .J.i4...F...h2..
-00003da0: 349a 50da 4ea3 09a5 ed34 9a50 da4e a309  4.P.N....4.P.N..
-00003db0: a5ed 349a 50da 4ea3 09a5 ed34 9a50 da4e  ..4.P.N....4.P.N
-00003dc0: a309 a5ed 349a 50da 4ea3 09a5 ed34 9a50  ....4.P.N....4.P
-00003dd0: da4e a309 a5ed 349a 2595 4693 216d a7d1  .N....4.%.F.!m..
-00003de0: 84d2 761a 4d28 6da7 d184 d276 1a4d 286d  ..v.M(m....v.M(m
-00003df0: a7d1 84d2 761a 4d28 6da7 d184 d276 1a4d  ....v.M(m....v.M
-00003e00: 286d a7d1 84d2 761a 4d28 6da7 d184 d276  (m....v.M(m....v
-00003e10: 1acd 924a a3c9 90b6 d368 4269 3b8d 2694  ...J.....hBi;.&.
-00003e20: b6d3 6842 693b 8d26 94b6 d368 4269 3b8d  ..hBi;.&...hBi;.
-00003e30: 2694 b6d3 6842 693b 8d26 94b6 d368 4269  &...hBi;.&...hBi
-00003e40: 3b8d 2694 b6d3 6842 693b 8d26 94b6 eb46  ;.&...hBi;.&...F
-00003e50: b3c4 ea46 d331 85d7 8da6 9cca eb46 534e  ...F.1.......FSN
-00003e60: e975 a329 a7f6 aaab 1a49 a3e9 6335 5f37  .u.).....I..c5_7
-00003e70: 9a72 baaf 1b4d 39ed d78d a69c feeb 4653  .r...M9.......FS
-00003e80: ce19 5037 9a72 ce81 bad1 9473 16d4 8da6  ..P7.r.....s....
-00003e90: 5cc7 3ce8 c848 ea5b 65f2 d88e 90a4 be55  \.<..H.[e......U
-00003ea0: a65c c73c c8fd bee4 3ae6 41ee f825 d731  .\.<....:.A..%.1
-00003eb0: 0f72 cf2f b98e 7990 bb7e c975 cc83 dcf7  .r./..y..~.u....
-00003ec0: 4bae 631e e4ce 5f72 1df3 20f7 fe92 eb98  K.c..._r.. .....
-00003ed0: 07b9 fb97 5cc7 3cc8 fdbf e43a e641 ee00  ....\.<....:.A..
-00003ee0: 26d7 310f 720f 30b8 8ec0 a46e 34e5 3ad6  &.1.r.0....n4.:.
-00003ef0: 838e c6a4 be55 a68f ed98 07b9 1598 5cc7  .....U........\.
-00003f00: 3cc8 cdc0 e43a e641 6e07 26d7 310f 7243  <....:.An.&.1.rC
-00003f10: 30b9 8e79 905b 82c9 b5e6 41ab d15c 9e2d  0..y.[....A..\.-
-00003f20: 1bcd 8e30 736e f1b5 cc7c e23f cecc 37ca  ...0sn...|.?..7.
-00003f30: cc95 e522 ccec 6256 da4c ff95 79ff 3de7  ..."..bV.L..y.=.
-00003f40: 1c30 3264 64d4 1c69 bf8d de94 6fa3 e68b  .02dd..i....o...
-00003f50: b7f1 a17c 1b32 1f66 cbb7 f1c2 8cdf 4639  ...|.2.f......F9
-00003f60: 325c 2e47 46cd 91f6 db98 9bf2 6dd4 7cfb  2\.GF.......m.|.
-00003f70: 6d7c e895 6fa3 8329 52da fef2 0b33 7e1b  m|..o..)R....3~.
-00003f80: e5c8 1066 d41c 69bf 8d4c 8f76 f8fb c6a4  ...f..i..L.v....
-00003f90: aaf9 fa6d bc9c 7e75 b91c e933 3260 64c8  ...m..~u...32`d.
-00003fa0: c8a8 39d2 7e89 698b ffbb 3679 b97e 64d9  ..9.~.i...6y.~d.
-00003fb0: 262f 941f fa33 d468 93bf 3f6c 3c32 6064  &/...3.h..?l<2`d
-00003fc0: c8c8 a839 d27e fd49 a8a7 fa88 6bbe 9829  ...9.~.I....k..)
-00003fd0: 4c78 99de 2c33 fe05 1a4f 9572 6458 f7dd  Lx..,3...O.rdX..
-00003fe0: 2d9f a3e6 48fb 7d2c 4df9 3e6a befd 3e7a  -...H.},M.>j..>z
-00003ff0: b34c f92e 8839 ff02 8ddf 4839 325c 2e47  .L...9....H92\.G
-00004000: 46cd 91f6 1ba9 6f50 dc8a dddf 98f3 e50d  F.....oP........
-00004010: 8d57 97cb 913e 2303 4686 8c8c 9a23 ed97  .W...>#.F....#..
-00004020: 5887 faff 558f bffc 9cf8 b77b fcc5 72ce  X...U......{..r.
-00004030: 977f 5f40 fffb c39a 73be 6486 30a3 e648  .._@....s.d.0..H
-00004040: fbf5 d71b db34 1ff1 cb46 38fe 5b04 7ab3  .....4...F8.[.z.
-00004050: f3e5 abee 828a cbb9 bf5c 6ea9 0346 868c  .........\n..F..
-00004060: 8c9a 23ad 37b2 32e5 a6fb c497 93be fcf8  ..#.7.2.........
-00004070: 3ba1 a562 bf7a 855e 273d 2343 4646 cd91  ;..b.z.^'=#CFF..
-00004080: f61b 696e bbb9 56fe 7eca afb8 a1f6 66cb  ..in..V.~.....f.
-00004090: 2f0f 9d50 f9ed e115 1abf 0db6 5d98 5173  /..P........].Qs
-000040a0: a4fd 369a dbee db6f c30d b537 5bae a52b  ..6....o...7[..+
-000040b0: 1d50 af5c 4b5f a1f1 db60 db85 1935 47da  .P.\K_...`...5G.
-000040c0: 6fa3 b9ed befd 365e b6d8 c6d5 d12b 57d2  o.....6^.....+W.
-000040d0: 952e a85c 495f a1f1 db28 b7ef 21cc a839  ...\I_...(..!..9
-000040e0: d27e 1bcd adf9 edb7 f1b2 d336 df46 7991  .~.........6.Fy.
-000040f0: af74 41e5 45fe 0a8d df46 b98b 0f61 46cd  .tA.E....F...aF.
-00004100: 91f6 db68 eed0 6fbd 8dfe 0adb 2a23 4346  ...h..o.....*#CF
-00004110: 46cd 91f6 c99b db6a fef9 47ff e295 95e7  F......j..G.....
-00004120: 0daf bdd0 b388 b073 7e7f d878 a11f 3232  .......s~..x..22
-00004130: 6a8e b45f 6b73 e77c db77 e8d7 bf14 a6d7  j.._ks.|.w......
-00004140: 6315 6c1f e6a5 977b ec60 a51c 1932 326a  c.l....{.`...22j
-00004150: 8eb4 5f7a 7347 7dfb a587 6ebc 7456 bef6  .._zsG}...n.tV..
-00004160: 61d6 bc72 eb1c acb0 9932 326a 8eb4 5f7a  a..r.....22j.._z
-00004170: 7333 7dfb a587 6ebc 7456 bbd6 e139 d639  s3}...n.tV...9.9
-00004180: b6cf 9572 64c8 c8a8 39d2 7ae9 1f9a dbe7  ...rd...9.z.....
-00004190: 9b2f bda6 c72f 7dae 5ce1 8ac3 e5da f674  ./.../}.\......t
-000041a0: aee6 8f26 0346 868c 8c9a 23ed 973e d586  ...&.F....#..>..
-000041b0: f921 74e3 a597 ab5a 71b8 5ccf eac3 ad6f  .!t....Zq.\....o
-000041c0: e103 4686 8c8c 9a23 ed97 3ed5 26f9 2174  ..F....#..>.&.!t
-000041d0: e3a5 9797 6971 787c 99b6 4f39 d586 f6a1  ....iqx|..O9....
-000041e0: f94b 89de 5c79 7915 87c7 9757 fb94 536d  .K..\yy....W..Sm
-000041f0: 3e1f 9a0b 656f aebc 2cda 87e7 c797 45fb  >...eo..,.....E.
-00004200: 94d3 6c14 d587 d0e3 0f76 9ee9 dc3e 3c9e  ..l......v...><.
-00004210: ceed 5316 dbc3 df7f 6ffb 10ba 714a a661  ..S.....o...qJ.a
-00004220: fbf0 781a b64f d95c e533 39de 3865 6b19  ..x..O.\.39.8ek.
-00004230: 9f67 fab4 0f4f 9a3e cdd5 f9ed 53b6 96df  .g...O.>....S...
-00004240: 79a6 4ffb f0a4 e9d3 5c55 df3e 656b d99c  y.O.....\U.>ek..
-00004250: 67fa b40e 2f4c 983e f911 bdf1 63d1 9be7  g.../L.>....c...
-00004260: 7cc2 c736 17ca 0954 1e9f 3083 7ab3 cde5  |..6...T..0.z...
-00004270: 20ff fca3 df30 9e1f 58fe fe64 fc2a 5a93   ....0..X..d.*Z.
-00004280: 263f ae4d f7de 5a4b c042 3953 9f9e aef1  &?.M..ZK.B9S....
-00004290: de27 4cd5 de6c 7311 f881 4fb4 b50a 2c94  .'L..ls...O...,.
-000042a0: 93f5 e9e9 1a67 9d30 5b7b b3cd 75e0 07ce  .....g.0[{..u...
-000042b0: fafc 8db1 57ff d2ac f8d0 9a57 f754 6a3a  ....W......W.Tj:
-000042c0: befd 3516 b5e2 2c53 5dd0 f941 aff9 2b63  ..5...,S]..A..+c
-000042d0: 675d ebf0 c449 37d5 15dd 9b6d 5eb3 2bce  g]...I7....m^.+.
-000042e0: 86d6 e189 9361 aa4b 3a3f 0936 dfa7 73a1  .....a.K:?.6..s.
-000042f0: 7578 d254 e84d 7749 d7f8 f82f 4a5c e4a4  ux.T.MwI.../J\..
-00004300: c5f1 49ef b4f7 df5e d24f 0f2c 2fe9 49cb  ..I....^.O.,/.I.
-00004310: 556f ba4b bac6 c717 cf62 f1d5 72b5 571c  Uo.K.....b..r.W.
-00004320: 9fb4 90f4 a6bb a46b bc71 d6f2 af9e ec15  .......k.q......
-00004330: c7c7 53ab 7d8d f4a6 bba4 6bbc 71d6 f297  ..S.}.....k.q...
-00004340: caf9 69a7 757c ecb9 386b 71fd fffd 56db  ..i.u|..8kq...V.
-00004350: ebb5 f6ef c5e2 47a6 7cc2 ede3 e38d b138  ......G.|......8
-00004360: eb74 eb41 afb5 852f 163f ede4 aced e3e3  .t.A.../.?......
-00004370: bdb1 38eb 742b 42af 79c9 2ff4 ca1d b7d7  ..8.t+B.y./.....
-00004380: 3ede f841 a638 eb74 6b42 afb5 912f 3987  >..A.8.tkB.../9.
-00004390: dbc7 27cd e1b9 e956 851a 1fcf a625 e670  ..'....V.....%.p
-000043a0: 717c d21c 9e6b fec8 f2f6 b654 e38d b332  q|...k.....T...2
-000043b0: 878b e393 e6f0 5cb1 16bd 3187 6bbc 7156  ......\...1.k.qV
-000043c0: e670 717c d21c 9e9b 6e6d aaf1 c659 99c3  .pq|....nm...Y..
-000043d0: c5f1 4973 786e bab5 a9c6 c767 5d66 3615  ..Isxn.....g]f6.
-000043e0: c727 cea6 e9d6 a6fc 1970 f3ac cea6 f6f1  .'.......p......
-000043f0: 89b3 69ba b569 aeb5 f62c 3b9b dac7 27ce  ..i..i...,;...'.
-00004400: a6e9 d6a6 b9d6 dab3 ec6c 6a1f 9f38 9ba6  .........lj..8..
-00004410: 5b9b e65a 3f61 2c3b 9bda c727 cea6 e9d6  [..Z?a,;...'....
-00004420: a6b9 d6da b3e2 6c6a 1f9f 349b e6a7 5b9b  ......lj..4...[.
-00004430: 6a7c fc8d 6589 af83 c5f1 49df 07e7 a75b  j|..e.....I....[
-00004440: 9b6a bc71 56be 1016 c727 7d4f 9a9f 6e6d  .j.qV....'}O..nm
-00004450: aaf1 c659 f976 561c 9ff4 9d70 7eba b5a9  ...Y.vV....p~...
-00004460: c65f cfba c0ef 497b c5f1 8967 9d6e 6d9a  ._....I{...g.nm.
-00004470: 6fae 4d0b bdf2 87e8 5e71 7cc2 4fd1 bdf9  o.M.....^q|.O...
-00004480: e9d6 a61a 6f7c c29e b57d 7ce2 59a7 5b9b  ....o|...}|.Y.[.
-00004490: e65b 6bcf 0a2b 6271 7cd2 8a38 3fdd da54  .[k..+bq|..8?..T
-000044a0: e363 af73 ac4d ade3 bd95 8973 78ba b569  .c.s.M.....sx..i
-000044b0: bef5 bd89 dfad f55a c77b 2b93 d6e1 f9e9  .......Z.{+.....
-000044c0: d6a6 1a1f 7bf5 c7f9 d6f1 deca a439 bc30  ....{........9.0
-000044d0: ddda 54e3 8d4f 98eb b575 bcd7 f8af 9fda  ..T..O...u......
-000044e0: df11 17fe db9f a69e 1e58 fe34 c55a f59d  .........X.4.Z..
-000044f0: 7afa 2397 e2c4 d32d 140b fe11 1f93 aa83  z.#....-........
-00004500: 99b4 e92d 4cb7 603c e1ed 3fda 9ef7 87bc  ...-L.`<..?.....
-00004510: 0eaa b730 f115 4cb7 782c bcfc c95b e3eb  ...0..L.x,...[..
-00004520: cd02 9b6f 2735 690b 5e98 6e21 79c2 8bff  ...o'5i.^.n!y...
-00004530: 18ad f8af 147a 1dcc c4b3 4fb7 a02c bcfc  .....z....O..,..
-00004540: 0158 f352 e307 a30e aaf1 c7d9 cf13 f0fd  .X.R............
-00004550: c31f 3737 8f83 abc7 ab5f 7ff9 76f5 fbcd  ..77....._..v...
-00004560: ced5 fdef b75f 1fde 7dbe f92d d7d3 ecd3  ....._..}..-....
-00004570: 6d1f ee6f 7faf 7f53 f8fc 2f8f 77df 723f  m..o...S../.w.r?
-00004580: 8899 77ff b87b 7cbc fbf2 f48f 7fdc 5c7d  ..w..{|.......\}
-00004590: bac9 2d20 667f 8a96 dfee ee1e 5ffe 25bf  ..- f......._.%.
-000045a0: e5aa 9ff3 e8e6 f15f dfde 7dbb fa76 737f  ......._..}..vs.
-000045b0: 74fb ff6e 3ece 6489 b8bb bfcd 1d24 ae1e  t..n>.d......$..
-000045c0: 6fef be7e 9cf9 7677 ff78 7f75 fb38 f3ee  o..~..vw.x.u.8..
-000045d0: cf9b fbc7 dbeb abcf 836f b779 be99 77f7  .........o.y..w.
-000045e0: 3fdf 7efa 3873 bff1 e9f9 5766 7fdd ddff  ?.~.8s....Wf....
-000045f0: f3e9 05ff faff 0500 0000 ffff 0300 504b  ..............PK
-00004600: 0304 1400 0600 0800 0000 2100 e9a6 25b8  ..........!...%.
-00004610: 6606 0000 531b 0000 1300 0000 786c 2f74  f...S.......xl/t
-00004620: 6865 6d65 2f74 6865 6d65 312e 786d 6cec  heme/theme1.xml.
-00004630: 59cd 6e1b 3710 be17 e83b 107b 4f2c d992  Y.n.7....;.{O,..
-00004640: 6219 9103 4b96 e236 7162 d84a 8a1c a95d  b...K..6qb.J...]
-00004650: 6a97 1177 b920 293b ba15 c9b1 4081 a269  j..w. );....@..i
-00004660: d14b 81de 7a28 da06 4880 5ed2 a771 9ba2  .K..z(..H.^..q..
-00004670: 4d81 bc42 87e4 4a5a 5a54 6c27 06fa 171d  M..B..JZZTl'....
-00004680: 6c2d f7e3 fccf 7086 ba7a ed41 cad0 2111  l-....p..z.A..!.
-00004690: 92f2 ac15 542f 5702 44b2 9047 348b 5bc1  ....T/W.D..G4.[.
-000046a0: 9d7e efd2 7a80 a4c2 5984 19cf 482b 9810  .~..z...Y...H+..
-000046b0: 195c db7c ffbd ab78 4325 2425 08f6 6772  .\.|...xC%$%..gr
-000046c0: 03b7 8244 a97c 6365 4586 b08c e565 9e93  ...D.|ceE....e..
-000046d0: 0cde 0db9 48b1 8247 11af 4402 1f01 dd94  ....H..G..D.....
-000046e0: adac 562a 8d95 14d3 2c40 194e 81ec ede1  ..V*....,@.N....
-000046f0: 9086 04f5 35c9 6073 4abc cbe0 3153 522f  ....5.`sJ...1SR/
-00004700: 844c 1c68 d2c4 d961 b0d1 a8aa 1172 223b  .L.h...a.....r";
-00004710: 4ca0 43cc 5a01 f089 f851 9f3c 5001 6258  L.C.Z....Q.<P.bX
-00004720: 2a78 d10a 2ae6 13ac 6c5e 5dc1 1bc5 26a6  *x..*...l^]...&.
-00004730: 96ec 2ded eb99 4fb1 afd8 108d 560d 4f11  ..-...O.....V.O.
-00004740: 0f66 4cab bd5a f3ca f68c be01 30b5 88eb  .fL..Z......0...
-00004750: 76bb 9d6e 7546 cf00 7018 82a6 5696 32cd  v..nuF..p...V.2.
-00004760: 5a6f bdda 9ed2 2c81 ecd7 45da 9d4a bd52  Zo....,...E..J.R
-00004770: 73f1 25fa 6b0b 3237 dbed 76bd 59c8 6289  s.%.k.27..v.Y.b.
-00004780: 1a90 fd5a 5bc0 af57 1ab5 ad55 076f 4016  ...Z[..W...U.o@.
-00004790: 5f5f c0d7 da5b 9d4e c3c1 1b90 c537 16f0  __...[.N.....7..
-000047a0: bd2b cd46 cdc5 1b50 c268 365a 406b 87f6  .+.F...P.h6Z@k..
-000047b0: 7a05 f519 64c8 d98e 17be 0ef0 f54a 019f  z...d........J..
-000047c0: a320 1a66 d1a5 590c 79a6 96c5 5a8a ef73  . .f..Y.y...Z..s
-000047d0: d103 8006 32ac 6886 d424 2743 1c42 1477  ....2.h..$'C.B.w
-000047e0: 703a 1014 6b06 7883 e0d2 1bbb 14ca 8525  p:..k.x........%
-000047f0: cd0b c950 d05c b582 0f73 0c19 31a7 f7ea  ...P.\...s..1...
-00004800: f9f7 af9e 3f45 af9e 3f39 7ef8 ecf8 e14f  ....?E..?9~....O
-00004810: c78f 1e1d 3ffc d1d2 7236 eee0 2c2e 6f7c  ....?...r6..,.o|
-00004820: f9ed 677f 7efd 31fa e3e9 372f 1f7f e1c7  ..g.~.1...7/....
-00004830: cb32 fed7 1f3e f9e5 e7cf fd40 c8a0 b944  .2...>.....@...D
-00004840: 2fbe 7cf2 dbb3 272f befa f4f7 ef1e 7be0  /.|...'/......{.
-00004850: 5b02 0fca f03e 4d89 44b7 c811 dae7 29e8  [....>M.D.....).
-00004860: 660c e34a 4e06 e27c 3bfa 09a6 ce0e 9c00  f..JN..|;.......
-00004870: 6d0f e9ae 4a1c e0ad 0966 3e5c 9bb8 c6bb  m...J....f>\....
-00004880: 2ba0 78f8 80d7 c7f7 1d59 0f12 3156 d4c3  +.x......Y..1V..
-00004890: f946 923a c05d ce59 9b0b af01 6e68 5e25  .F.:.].Y....nh^%
-000048a0: 0bf7 c759 ec67 2ec6 65dc 3ec6 873e de1d  ...Y.g..e.>..>..
-000048b0: 9c39 aeed 8e73 a89a d3a0 746c df49 8823  .9...s....tl.I.#
-000048c0: e61e c399 c231 c988 42fa 1d1f 11e2 d1ee  .....1..B.......
-000048d0: 1ea5 8e5d 7769 28b8 e443 85ee 51d4 c6d4  ...]wi(..C..Q...
-000048e0: 6b92 3e1d 3881 34df b443 53f0 cbc4 a733  k.>.8.4..CS....3
-000048f0: b8da b1cd ee5d d4e6 cca7 f536 3974 9190  .....].....69t..
-00004900: 1098 7984 ef13 e698 f13a 1e2b 9cfa 48f6  ..y......:.+..H.
-00004910: 71ca ca06 bf89 55e2 13f2 6022 c232 ae2b  q.....U...`".2.+
-00004920: 1578 3a26 8ca3 6e44 a4f4 edb9 2d40 df92  .x:&..nD....-@..
-00004930: d36f 60a8 575e b7ef b249 ea22 85a2 231f  .o`.W^...I."..#.
-00004940: cd9b 98f3 3272 9b8f 3a09 4e73 afcc 344b  ....2r..:.Ns..4K
-00004950: cad8 0fe4 0842 14a3 3dae 7cf0 5dee 6688  .....B..=.|.].f.
-00004960: 7e06 3fe0 6ca9 bbef 52e2 b8fb f442 7087  ~.?.l...R....Bp.
-00004970: c68e 48f3 00d1 6fc6 a2a8 da4e fd4d 69f6  ..H...o....N.Mi.
-00004980: ba62 cc28 54e3 77c5 787a 3a6d c1d1 e44b  .b.(T.w.xz:m...K
-00004990: 899d 1325 7819 ee5f 5878 b7f1 38db 2310  ...%x.._Xx..8.#.
-000049a0: eb8b 07cf bbba fbae ee06 fff9 babb 2c97  ..............,.
-000049b0: cf5a 6de7 0516 9ae4 795f 6cba e474 6993  .Zm.....y_l..ti.
-000049c0: 3ca4 8c1d a809 2337 a5e9 9325 1c16 510f  <.....#7...%..Q.
-000049d0: 164d 036f a6b8 d9d0 9427 f0b5 28ee 0e2e  .M.o.....'..(...
-000049e0: 16d8 ec41 82ab 8fa8 4a0e 129c 438f 5d35  ...A....J...C.]5
-000049f0: 235f 2c0b d2b1 4439 9730 db99 6533 7c92  #_,...D9.0..e3|.
-00004a00: 13b4 cd38 49a1 cd36 9361 5dcf 0cb6 1e48  ...8I..6.a]....H
-00004a10: ac76 7964 97d7 cab3 e18c 8c99 1463 337f  .vyd.........c3.
-00004a20: 4e19 ad69 0267 65b6 76e5 ed98 55ad 544b  N..i.ge.v...U.TK
-00004a30: cde6 aa56 35a2 9952 e7a8 3653 197c b8a8  ...V5..R..6S.|..
-00004a40: 1a2c ceac 095d 0882 de05 acdc 8011 5dcb  .,...]........].
-00004a50: 0eb3 0966 24d2 76b7 73f3 d42d 9af5 85ba  ...f$.v.s..-....
-00004a60: 4826 3822 858f b4de 8b3e aa1a 274d 6365  H&8".....>..'Mce
-00004a70: 1a46 1e1f e939 ef14 1f95 b835 35d9 b7e0  .F...9.....55...
-00004a80: 7616 2795 d9d5 96b0 9b7a ef6d bc34 1d6e  v.'......z.m.4.n
-00004a90: e75e d279 7b22 1d59 564e 4e96 a1a3 56d0  .^.y{".YVNN...V.
-00004aa0: acaf d603 14e2 bc15 0c61 ac85 af69 0e5e  .........a...i.^
-00004ab0: 97ba f1c3 2c86 bba1 5009 1bf6 a726 b309  ....,...P....&..
-00004ac0: d7b9 379b feb0 acc2 4d85 b5fb 82c2 4e1d  ..7.....M.....N.
-00004ad0: c885 54db 5826 3634 ccab 2204 5866 8670  ..T.X&64..".Xf.p
-00004ae0: 23ff 6a1d cc7a 510a d848 7f03 29d6 d621  #.j..zQ..H..)..!
-00004af0: 18fe 3629 c08e ae6b c970 4842 5576 7669  ..6)...k.pHBUvvi
-00004b00: c5dc 5118 4051 4af9 5811 7190 4447 68c0  ..Q.@QJ.X.q.DGh.
-00004b10: c662 1f83 fb75 a882 3e11 9570 3b61 2a82  .b...u..>..p;a*.
-00004b20: 7e80 ab34 6d6d f3ca 2dce 45d2 952f b00c  ~..4mm..-.E../..
-00004b30: ceae 6396 27b8 28b7 3a45 a799 6ce1 268f  ..c.'.(.:E..l.&.
-00004b40: 6732 9827 2bad 110f 74f3 ca6e 943b bf2a  g2.'+...t..n.;.*
-00004b50: 26e5 2f48 9572 18ff cf54 d1e7 095c 17ac  &./H.r...T...\..
-00004b60: 45da 0321 dce4 0a8c 74be b602 2e54 c2a1  E..!....t....T..
-00004b70: 0ae5 090d 7b02 2eb9 4ced 8068 81eb 5878  ....{...L..h..Xx
-00004b80: 0d41 05f7 c9e6 bf20 87fa bfcd 394b c3a4  .A..... ....9K..
-00004b90: 354c 7d6a 9fc6 4850 388f 5422 08d9 83b2  5L}j..HP8.T"....
-00004ba0: 64a2 ef14 62d5 e2ec b224 5941 c844 5449  d...b....$YA.DTI
-00004bb0: 5c99 5bb1 07e4 90b0 beae 810d 7db6 0728  \.[.........}..(
-00004bc0: 8150 37d5 a428 0306 7732 fedc e722 8306  .P7..(..w2..."..
-00004bd0: b16e 72fe a99d 8f4d e6f3 b607 ba3b b02d  .nr....M.....;.-
-00004be0: 96dd 7fc6 5ea4 562a faa5 a3a0 e93d fb4c  ....^.V*.....=.L
-00004bf0: 4f35 2b07 af39 d8cf 79d4 da8a b5a0 f16a  O5+..9..y......j
-00004c00: fdcc 476d 0e97 3e48 ff81 f38f 8a90 d91f  ..Gm..>H........
-00004c10: 27f4 81da e7fb 505b 11fc d660 db2b 0451  '.....P[...`.+.Q
-00004c20: 7dc9 361e 4817 485b 1e07 d038 d945 1b4c  }.6.H.H[...8.E.L
-00004c30: 9a94 6d58 8aee f6c2 db28 b891 2e3a dd19  ..mX.....(...:..
-00004c40: 5fc8 d237 e974 cf69 ec59 73e6 b273 72f1  _..7.t.i.Ys..sr.
-00004c50: f5dd e7f9 8c5d 58d8 b175 b9d3 f598 1a92  .....]X..u......
-00004c60: f664 8aea f668 3ac8 18c7 985f b5ca 3f3c  .d...h:...._..?<
-00004c70: f1c1 7d70 f436 5cf1 8f99 92f6 6aff 015c  ..}p.6\.....j..\
-00004c80: f1c1 9461 7f24 80e4 b7ce 355b 37ff 0200  ...a.$....5[7...
-00004c90: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
-00004ca0: 0021 0037 b198 f114 0300 0090 0a00 000d  .!.7............
-00004cb0: 0000 0078 6c2f 7374 796c 6573 2e78 6d6c  ...xl/styles.xml
-00004cc0: c456 db6e db30 0c7d 1fb0 7f10 f4ee fad2  .V.n.0.}........
-00004cd0: 384b 02db 45d3 d440 816d 18d0 0cd8 ab62  8K..E..@.m.....b
-00004ce0: cb89 505d 0c59 699d 0dfb f751 be24 2eda  ..P].Yi....Q.$..
-00004cf0: ae69 d7a1 2f96 4453 87a4 0e49 293a ab05  .i../.DS...I):..
-00004d00: 47b7 5457 4cc9 18fb 271e 4654 662a 6772  G.TWL...'.FTf*gr
-00004d10: 1de3 efcb d499 6054 1922 73c2 95a4 31de  ......`T."s...1.
-00004d20: d10a 9f25 1f3f 4495 d971 7abd a1d4 2080  ...%.?D..qz... .
-00004d30: 9055 8c37 c694 33d7 adb2 0d15 a43a 5125  .U.7..3......:Q%
-00004d40: 95f0 a750 5a10 034b bd76 ab52 5392 5776  ...PZ..K.v.RS.Wv
-00004d50: 93e0 6ee0 7963 5710 2671 8b30 13d9 3120  ..n.ycW.&q.0..1 
-00004d60: 82e8 9b6d e964 4a94 c4b0 15e3 ccec 1a2c  ...m.dJ........,
-00004d70: 8c44 36bb 5a4b a5c9 8a83 abb5 3f22 19aa  .D6.ZK......?"..
-00004d80: fdb1 0e7a 0b8d e881 11c1 32ad 2a55 9813  ...z......2.*U..
-00004d90: 0075 5551 b08c 3ef4 75ea 4e5d 921d 9000  .uUQ..>.u.N]....
-00004da0: f675 487e e87a 411b 7812 154a 9a0a 656a  .uH~.zA.x..J..ej
-00004db0: 2b4d 8c43 40b7 4ecf 6ea4 ba93 a9fd 059c  +M.C@.N.n.......
-00004dc0: e056 2b89 aa9f e896 7090 f8d8 4da2 4c71  .V+.....p...M.Lq
-00004dd0: a591 81c3 8658 1b89 2482 b61a 1784 b395  .....X..$.......
-00004de0: 6656 ad20 82f1 5d2b 0eac a0e1 a7d3 130c  fV. ..]+........
-00004df0: 4ecb 0a5d eb47 6f67 65b5 dec3 d6e8 ffc6  N..].Goge.......
-00004e00: f57e 311d c74c 4742 3354 4006 e37c 9f1a  .~1..LGB3T@..|..
-00004e10: 81cd 0210 2411 64bd a15a a6b0 40dd 7cb9  ....$.d..Z..@.|.
-00004e20: 2b21 0724 1468 cb65 a3f7 8cf6 5a93 9d1f  +!.$.h.e....Z...
-00004e30: 8483 0d6e 6330 8956 4ae7 d010 faa4 b4f9  ...nc0.VJ.......
-00004e40: d78a 9288 d3c2 4072 68b6 ded8 d1a8 12be  ......@rh.......
-00004e50: 2b65 0cd4 4d12 e58c ac95 24dc e653 bfa3  +e..M.....$..S..
-00004e60: 9b40 3819 e5fc da36 8d1f c53d ecba 4072  .@8....6...=..@r
-00004e70: 2b52 61ae f218 43fb b199 d84f 2190 6eda  +Ra...C....O!.n.
-00004e80: e2b5 0b8b 3f44 6bb1 87b0 1ef8 fc72 5c54  ....?Dk......r\T
-00004e90: 177b 034f edf6 c1c1 c7bd daef 46a4 2cf9  .{.O........F.,.
-00004ea0: ce56 6f57 974f 6141 5b7a 332c 7b70 c7f9  .VoW.OaA[z3,{p..
-00004eb0: 055a 6fed 5717 f1f3 c82f 3ebd a391 8f8f  .Zo.W..../>.....
-00004ec0: bfe3 e568 e4d3 97b2 7434 f2e8 3df8 3fe7  ...h....t4..=.?.
-00004ed0: 6c2d 056d 9333 89e0 a268 97e8 4e93 7249  l-.m.3...h..N.rI
-00004ee0: eb3e 69dd bae8 ca0c 0a6b 50bd f76a 775f  .>i......kP..jw_
-00004ef0: 85c8 76b8 187f b597 3d87 5bac 2b24 b4da  ..v.....=.[.+$..
-00004f00: 326e 987c a46e 0133 af0f 9dc0 b38d c8d8  2n.|.n.3........
-00004f10: 8bbb e911 7b2b c06b 4e0b b2e5 66b9 ff19  ....{+.kN...f...
-00004f20: e3c3 fc0b cdd9 564c f75a dfd8 ad32 0d44  ......VL.Z...2.D
-00004f30: 8c0f f3cf b661 f963 6b03 22fc 5cc1 5507  .....a.ck.".\.U.
-00004f40: 23da 6a16 e35f 97f3 4fd3 c565 1a38 136f  #.j.._..O..e.8.o
-00004f50: 3e71 46a7 3474 a6e1 7ce1 84a3 8bf9 6291  >qF.4t..|.....b.
-00004f60: 4ebd c0bb f83d 7841 fcc3 fba1 79ed 406b  N....=xA....y.@k
-00004f70: f247 b38a c32b 4377 c176 215e 1f64 311e  .G...+Cw.v!^.d1.
-00004f80: 2c5a f79b 560d 6e0f 7d9f 0663 ef3c f43d  ,Z..V.n.}..c.<.=
-00004f90: 273d f57c 6734 2613 6732 3e0d 9d34 f483  '=.|g4&.g2>..4..
-00004fa0: c578 34bf 0cd3 70e0 7bf8 ca17 8be7 fa7e  .x4...p.{......~
-00004fb0: ff62 a9fd 7066 98a0 9cc9 9eab 9ea1 a114  .b..pf..........
-00004fc0: 4882 e55f 8270 7b26 dcc3 5332 f903 0000  H.._.p{&..S2....
-00004fd0: ffff 0300 504b 0304 1400 0600 0800 0000  ....PK..........
-00004fe0: 2100 1b27 16c6 e51f 0000 f96a 0000 1400  !..'.......j....
-00004ff0: 0000 786c 2f73 6861 7265 6453 7472 696e  ..xl/sharedStrin
-00005000: 6773 2e78 6d6c b45d 6d73 db46 92fe 7e55  gs.xml.]ms.F..~U
-00005010: f71f a658 75bb 542c 52a4 ecec e5ec 285b  ...Xu.T,R.....([
-00005020: d69b ad9c a4c8 129d c4e5 4b50 1008 9258  ..........KP...X
-00005030: 8300 0380 7ac9 a7fd 2177 7f6e 7fc9 3ddd  ....z...!w.n..=.
-00005040: 3d83 b719 5092 e37c d88d 4d0c 661a 333d  =...P..|..M.f.3=
-00005050: 3ddd 4f3f 3dfe f6ef 77cb 58dd 8459 1ea5  =.O?=...w.X..Y..
-00005060: c95e 6f3c 1cf5 5498 04e9 344a e67b bdf7  .^o<..T...4J.{..
-00005070: 93e3 c137 3d95 177e 32f5 e334 09f7 7af7  ...7=..~2..4..z.
-00005080: 61de fbfb 77ff fe6f dfe6 79a1 f06e 92ef  a...w..o..y..n..
-00005090: f516 45b1 7ab9 b393 078b 70e9 e7c3 7415  ..E.z.....p...t.
-000050a0: 2678 324b b3a5 5fe0 afd9 7c27 5f65 a13f  &x2K.._...|'_e.?
-000050b0: cd17 6158 2ce3 9ddd d1e8 6f3b 4b3f 4a7a  ..aX,.....o;K?Jz
-000050c0: 2a48 d749 b1d7 7bf1 e2eb 9e5a 27d1 6feb  *H.I..{....Z'.o.
-000050d0: f040 ffb2 fb4d efbb 6ff3 e8bb 6f8b ef4e  .@...M..o...o..N
-000050e0: 92a8 88fc 5815 e172 1566 7eb1 ce42 f5f1  ....X..r.f~..B..
-000050f0: bf7f f976 a7f8 eedb 1d6a 22cd 26a3 51fb  ...v.....j".&.Q.
-00005100: a733 7f9e 8445 14a8 384c e6c5 427d 5c5a  .3...E..8L..B}\Z
-00005110: 6fc5 de92 1bb5 5f35 8306 eb2c 0b93 427d  o....._5...,..B}
-00005120: 7c6d bd7a 620f 7815 c633 b55c 176b 881b  |m.zb.x..3.\.k..
-00005130: 25d3 7580 a90b 4285 89c8 a23b f5f1 ed8e  %.u...B....;....
-00005140: 2dc0 99b7 6c8f 7da0 c78c c39b 30ce 955f  -...l.}.....0.._
-00005150: a8db 4514 2c54 b108 d534 9acd 4292 8866  ..E.,T...4..B..f
-00005160: a436 4494 abf0 c68f d77e 114e 5dc2 ce4e  .6D......~.N]..N
-00005170: bd93 f638 f8ed b4fd db61 388b 9290 870a  ...8.....a8.....
-00005180: d228 5679 1814 d00d 4880 5155 e843 8c79  .(Vy....H.QU.C.y
-00005190: 96ae 572a 9da9 c0bf 8ec3 5c61 e838 0d68  ..W*......\a.8.h
-000051a0: e076 676f a8e5 243d 4047 57d2 4fbb c545  .vgo..$=@GW.O..E
-000051b0: 1afb 5954 dc53 77f4 7966 baa3 a435 565e  ..YT.Sw.yf...5V^
-000051c0: 64d0 c2bc fdfe 4ade 8fc2 dc8b 121e aedd  d.....J.........
-000051d0: e27c bdbc 0e33 ea7f e1c7 b301 b427 81c8  .|...3.......'..
-000051e0: f5ee db6f 2493 ee3e b418 6507 3c05 ea3a  ...o$..>..e.<..:
-000051f0: c4ee 9863 cfa8 2255 be5a f919 946e 8d2f  ...c.."U.Z...n./
-00005200: 93b9 b206 b892 8fe9 1259 6b2b 44e6 f926  .........Yk+D..&
-00005210: b915 c94d faab fad3 70e6 afe3 62cf 68ee  ...M....p...b.h.
-00005220: 56bb 7b7e d0d5 b77c 00d4 c85f 8605 e6c5  V.{~...|..._....
-00005230: b125 a69d 7339 f3ae 0e3c e9a1 abff 23a8  .%..s9...<....#.
-00005240: 2734 e606 2a84 05cb c9b4 842a 0bf3 28c7  '4..*......*..(.
-00005250: 8fb4 d098 1c3d 74f9 2563 eb13 665e 967a  .....=t.%c..f^.z
-00005260: e16c d635 ca71 14a3 136c cbe2 161d 0f56  .l.5.q...l.....V
-00005270: 5101 bd74 7cca e9ca ebec e3f2 f2d2 3b58  Q..t|.........;X
-00005280: 778d 7075 50dc afc2 cea7 934d 4f27 78b3  w.puP......MO'x.
-00005290: dc1f 5095 1caa c09b a83f de7b 331e 6dab  ..P......?.{3.m.
-000052a0: ddbd 4ffe aa48 13eb bbab b6d4 47d7 e8a6  ..O..H......G...
-000052b0: ff59 14c7 a2da 3769 34cd a186 c56d 1826  .Y....7i4....m.&
-000052c0: ca9f fec3 0f68 768c b6b6 c7dd 56cf f716  .....hv.....V...
-000052d0: 611c ad97 dbea c51e bdec 9004 da91 f8f1  a...............
-000052e0: 8fd4 f31f 11c6 c880 dd5b 9f8a d8c7 5192  .........[....Q.
-000052f0: e5ea 3344 0bef 1e29 dab5 0f93 253b f436  ..3D...)....%;.6
-00005300: 9aba edff ed3e 1a75 4d34 77e0 4387 fdb9  .....>.uM4w.C...
-00005310: e968 1146 f305 8e03 db90 2f36 f554 5382  .h.F....../6.TS.
-00005320: 02b6 fc53 12e6 6c85 c8e6 896c d328 d3a6  ...S..l....l.(..
-00005330: d6d1 f7ed 49d2 b929 3775 ada5 ddd8 f762  ....I..)7u.....b
-00005340: 43df 62a8 1eb1 cb3a a53b c8d2 3c1f 0469  C.b....:.;..<..i
-00005350: 52f8 41a1 0d01 9f89 1f7f 58d8 7378 e905  R.A.......X.sx..
-00005360: 9d4a 1f8c bcf3 eb49 e42d 0ad3 c4e9 05d8  .J.....I.-......
-00005370: cdda f671 3fd8 b57b 9a58 c7bb a359 bba7  ...q?..{.X...Y..
-00005380: 60ec 9d04 d297 3e7d 5c47 afdd caea 67d7  `.....>}\G....g.
-00005390: d1cf 8e2d 1204 6f8d d7ee 69c2 9fff fc0a  ...-..o...i.....
-000053a0: 6785 c343 320f bbe6 583e 99df ee9a 0f3c  g..C2...X>.....<
-000053b0: ec7a fb7b 9a0a 3c1f 6112 be9a fc3a 1a7e  .z.{..<.a....:.~
-000053c0: bdb3 fc75 f717 b5ef e7f0 49e0 43e4 8b34  ...u......I.C..4
-000053d0: 2b06 b9bf 5cc5 f089 423f 8727 4756 dc3a  +...\...B?.'GV.:
-000053e0: d5cb 9e3a 4f99 187b 258b 02f8 4069 3615  ...:O..{%...@i6.
-000053f0: 1b48 5ba9 3c2a ad2e c3d8 e396 1e35 f1d8  .H[.<*.......5..
-00005400: 0bb0 5dbe 208e 12b1 d495 7773 1bc1 70e0  ..]. .....ws..p.
-00005410: 005b 6144 3ade 7f56 fe1d 3c9e 7e94 04f1  .[aD:..V..<.~...
-00005420: 9afc 6439 e8c4 dd85 a794 2bfc 512d a32c  ..d9......+.Q-.,
-00005430: c37f c8e8 6569 c17d 5a26 d68f 570b 3f3f  ....ei.}Z&..W.??
-00005440: 3c7a d316 e492 de30 06e7 fa1e 1e45 1066  <z.....0.....E.f
-00005450: 051c 66f4 37c7 d47d 9c86 734b 5dcd 30de  ..f.7..}..sK].0.
-00005460: 359c b14f ed2e cf44 1e31 86e4 cb43 6ccc  5..O...D.1...Cl.
-00005470: d775 44fe 1d04 c5f7 4645 ae7e 5bfb 531c  .uD.....FE.~[.S.
-00005480: db85 ea8f f692 745b 8df7 60a5 2dc1 e5e3  ......t[..`.-...
-00005490: 9e34 d007 3d6b 0f77 fbc1 ddef 4932 8d02  .4..=k.w....I2..
-000054a0: 389b c64f 14d7 33bc 0b16 9813 5a85 4548  8..O..3.....Z.EH
-000054b0: 7e32 2d56 7420 d6e6 357d e64f 64f8 bd09  ~2-Vt ..5}.Od...
-000054c0: dcb2 f2a3 cb13 2154 7934 0ddb 53e5 78fd  ......!Ty4..S.x.
-000054d0: 384b 2d27 fd8f 0944 3dfe 2191 26a9 adbe  8K-'...D=.!.&...
-000054e0: 9f37 436f f944 734d 51e2 4389 6f1f 9e24  .7Co.DsMQ.C.o..$
-000054f0: ddc3 979c a55a 97d6 343d 51ac 0767 aa16  .....Z..4=Q..g..
-00005500: 1714 0b28 1179 0d79 c89b 1d01 6902 cf92  ...(.y.y....i...
-00005510: 7e54 7338 b589 2aa2 a5ad 3157 053c fe77  ~Ts8..*...1W.<.w
-00005520: dcd6 32c8 685f 4570 eccf e721 592f 98c4  ..2.h_Ep...!Y/..
-00005530: 7260 ec3b 1a07 eafd 31b7 3676 b1a1 7713  r`.;....1.6v..w.
-00005540: a556 1103 5bc1 1456 7695 3abd 1469 f936  .V..[..Vv.:..i.6
-00005550: 2dae d0c0 8b36 f47d c94e 3b9f d57a d3dd  -....6.}.N;..z..
-00005560: fad9 9283 9b6a 1b46 59b0 8e30 50c7 612e  .....j.FY..0P.a.
-00005570: 8f2d fbd6 e839 808e c1d1 323b 7b95 dec2  .-...9....2;{...
-00005580: 9ee7 ebd5 2abe efec 575e 69f7 7b9c 6610  ....*...W^i.{.f.
-00005590: 71aa 6ed2 b820 8f6d 9aa5 1ca7 fa08 77d2  q.n.. .m......w.
-000055a0: 295c f20c 46ef 3e43 c480 3fc1 9a72 c0b9  )\..F.>C..?..r..
-000055b0: 69f4 1fad c578 3ff5 b4bc ce85 4694 2cdd  i....x?.....F.,.
-000055c0: 36be 02c7 450e cb84 05c6 3138 9bf1 a950  6...E.....18...P
-000055d0: 1fbb f11c 27b7 4307 bc8b 83f6 80a7 ef27  ....'.C........'
-000055e0: c04f 9222 4b63 1c5b 7355 1f72 5b4d 48ef  .O."Kc.[sU.r[MH.
-000055f0: 3a7a f2f0 ead3 7a33 8884 0b05 8168 ae0e  :z....z3.....h..
-00005600: 5980 723e c224 cce6 f703 b8ee 19fc 4002  Y.r>.$........@.
-00005610: 14f2 fb1c 800e 8107 38c8 e773 a00b c02d  ........8..s...-
-00005620: 1c5f 7e74 b459 7d68 223b 7bef d0cb a323  ._~t.Y}h";{....#
-00005630: af1c 74f3 3a1e 9c9e bc7b b4a8 d4b8 dddd  ..t.:....{......
-00005640: 61e9 d6eb 4d14 d18a 0119 c2e7 1ab0 83cf  a...M...........
-00005650: b090 fd06 568b 459a 438d 7868 2cf0 2c9a  ....V.E.C.xh,.,.
-00005660: af81 7a61 ceda 7d97 6ebd 5e1e d7f8 15fc  ..za..}.n.^.....
-00005670: c1fd 0164 b3dd adc4 f5a2 0cbf f033 3e5d  ...d.........3>]
-00005680: cd96 fae8 d812 16ec 76e0 affc 2012 e84b  ........v... ..K
-00005690: 7fb5 f426 bf63 f35d fbc9 27f5 f1d8 da5e  ...&.c.]..'....^
-000056a0: 9692 db46 887b 8a09 4eec b00e 0146 d9bc  ...F.{..N....F..
-000056b0: a8ef de3e 7a49 dfbd 6d77 75d0 9e12 fd85  ...>zI..mwu.....
-000056c0: e894 46c6 7797 dfe7 9a2b cfd1 a33d 5d8e  ..F.w....+...=].
-000056d0: ce1c 93e5 e8ab c368 cb7c 5592 2228 8f56  .......h.|U."(.V
-000056e0: b08a c06c b1c0 7035 37db 7132 fc8e c1d8  ...l..p57.q2....
-000056f0: b732 769b 2695 7b75 85af 8e97 e584 7fcc  .2v.&.{u........
-00005700: db0b c7db 9332 882e b755 89b2 10b4 0015  .....2...U......
-00005710: d360 4829 17f9 e20c 69d6 0266 69ea 9098  .`H)....i..fi...
-00005720: e2d9 dc35 ae86 7680 e886 1941 b05f 6078  ...5..v....A._`x
-00005730: 8140 5e75 a342 1a6b 72ca f379 f320 e00f  .@^u.B.kr..y. ..
-00005740: b6a1 1b14 315f efbd b57c 1d83 3d7d de04  ....1_...|..=}..
-00005750: d4c7 7dca 673b 0439 1548 bfad d34e 88df  ..}.g;.9.H...N..
-00005760: de73 c7e6 18c2 fba5 8604 29a0 1ed8 6584  .s........)...e.
-00005770: 5c14 4dd0 a18a dc07 595e c47b 099c aa83  \.M.....Y^.{....
-00005780: f560 0528 2fb4 e1b2 9943 575a 1182 1906  .`.(/....CWZ....
-00005790: 40bd 2b6a a942 5777 0063 8529 efde 7a45  @.+j.BWw.c.)..zE
-000057a0: fa16 d1ec 04d0 b0f7 08e7 bb36 8253 824a  ...........6.S.J
-000057b0: c047 8640 5153 04db d166 1f60 46a1 4e95  .G.@QS...f.`F.N.
-000057c0: c0f0 013d 43ef 9094 5918 37b5 9ed8 4148  ...=C...Y.7...AH
-000057d0: 4fc8 b9b8 08e4 56e7 4305 bf4e 90f0 7a46  O.....V.C..N..zF
-000057e0: 621b e656 9a4a b6e2 817e b5bb b700 7a17  b..V.J...~....z.
-000057f0: 0231 9e45 613c d5f8 e88e 0484 2ee7 c3ed  .1.Ea<..........
-00005800: d31b af5b 4707 75f1 cd30 0f7d 9a03 9d89  ...[G.u..0.}....
-00005810: 24cd 2543 4e90 eb6a afb8 59eb 490a cdd2  $.%CN..j..Y.I...
-00005820: a9a5 7d57 b07f 0480 3499 4291 1169 3c3d  ..}W....4.B..i<=
-00005830: 1dd5 eadc 4e4f 8984 6a8a fc81 b872 c639  ....NO..j....r.9
-00005840: 2816 c049 1629 26d6 e126 e4d1 f2f9 a1b7  (..I.)&..&......
-00005850: 9e98 36ed afbb c272 d28e 9bc1 3fc4 7a13  ..6....r....?.z.
-00005860: 8812 a429 ff04 d405 7e11 d289 4847 4570  ...)....~...HGEp
-00005870: 1c06 0a11 3ecd 00da 4cd3 5bf8 928e 305e  ....>...L.[...0^
-00005880: c69b 79ba 138f 1a7e a131 91fd 7acc 886b  ..y....~.1..z..k
-00005890: 6b05 3ff3 1be1 1f03 727e cc90 7138 2bbe  k.?.....r~..q8+.
-000058a0: d047 5257 8f1a 93a5 7bc4 a01c 9912 48a3  .GRW....{.....H.
-000058b0: 8d0f d027 7d44 0b4e 5f2e 6933 53d0 ee59  ...'}D.N_.i3S..Y
-000058c0: afeb d11d 6d03 0be6 73cc 308d 6bd4 87b2  ....m...s.0.k...
-000058d0: a76b ca75 9763 c3c1 164d 429e b544 8880  .k.u.c...MB..D..
-000058e0: c8c3 8328 1ff1 34a8 fefb c3c1 e02f f3e2  ...(..4....../..
-000058f0: d5fb d5ce 2194 c982 c54a c9de 1f3e 723a  ....!....J...>r:
-00005900: 9e28 9600 1f0e c94e 2f45 b253 acd9 ce25  .(.....N/E.S...%
-00005910: 694b b770 a797 6de1 ce60 7996 eba5 ca57  iK.p..m..`y....W
-00005920: 30bb d863 4b6c 627c f2ef e176 1924 a73e  0..cKlb|...v.$.>
-00005930: d278 037e 40c9 4d57 fa43 be7e 1925 1ef2  .x.~@.MW.C.~.%..
-00005940: 8701 bff0 f481 28f7 fc84 61a8 79d7 2049  ......(...a.y. I
-00005950: 99f7 4d10 fb57 295f ca47 d10c 0d4c 665b  ..M..W)_.G...Lf[
-00005960: 3e68 60c5 22d5 0771 0717 6146 d910 7af5  >h`."..q..aF..z.
-00005970: 0253 f0d4 6161 903f 63c4 23a4 bc5d a3b5  .S..aa.?c.#..]..
-00005980: 5c8b 1a82 c508 28cd 0b30 685a c78f 5d1f  \.....(..0hZ..].
-00005990: 164d ef8e a9d9 195a 9993 c58a 7500 ce57  .M.....Z....u..W
-000059a0: e07a fd9c 9bfb eb3c 8ffc 8462 0878 fdd7  .z.....<...b.x..
-000059b0: 6b3a b0a1 2fc3 7008 2022 0761 a3e4 0cd0  k:../.p. ".a....
-000059c0: fed3 2725 bc29 1ce8 ddda 3359 ade3 3cf4  ..'%.)....3Y..<.
-000059d0: f20b dd43 5b9e 8bd0 ffd4 a081 68ef cf29  ...C[.......h..)
-000059e0: 8d2b 0322 6baa 8759 a137 0b07 69c4 348f  .+."k..Y.7..i.4.
-000059f0: fde2 ddaf f268 bef4 1ffc 30ce f4b5 3fea  .....h....0...?.
-00005a00: 5047 f726 94f0 b11b 99c5 f1e6 e4d8 8588  PG.&............
-00005a10: c837 4cf5 5b68 d461 2163 7fee e548 5e1e  .7L.[h.a!c...H^.
-00005a20: 137e 105a 9652 5b2b d36a 733f 3f46 3928  .~.Z.R[+.js??F9(
-00005a30: 2d30 096f c214 bc81 ecfe b965 e26a fd5d  -0.o.......e.j.]
-00005a40: 61d4 ee86 ec14 fe28 6907 669b b0b2 0c15  a......(i.f.....
-00005a50: f45c 8801 b95a 53c2 08a7 fe9c 801d 4a85  .\...ZS.......J.
-00005a60: b00d 2744 eb86 df1b aa23 22a2 50b8 1903  ..'D.....#".P...
-00005a70: a885 16c8 6ecf e194 90ee c396 3350 8b7c  ....n.......3P.|
-00005a80: 4082 73ff a59a 4519 f84a c05d 9934 4098  @.s...E..J.].4@.
-00005a90: 1394 92b5 91db 6d13 cd05 0741 bb05 81bd  ......m....A....
-00005aa0: 6816 aec4 1072 8281 3adc c6fb 1180 c656  h....r..:......V
-00005ab0: 87d8 e3dc dd50 9d14 6001 6144 ce7b 52de  .....P..`.aD.{R.
-00005ac0: 460b 48a2 ea97 72b4 880b fa00 faf1 f950  F.H...r........P
-00005ad0: bd4e ee45 e855 0a8c 48f9 d788 4654 b137  .N.E.U..H...FT.7
-00005ae0: 1e8d 462a c797 c431 0e2d 15cd 9314 31ca  ..F*...1.-....1.
-00005af0: b0bd e824 aa27 b3e3 31c5 c25a f0cb 9089  ...$.'..1..Z....
-00005b00: 43a0 23d5 4836 973f fc7c 7244 c068 4a67  C.#.H6.?.|rD.hJg
-00005b10: 91ca d359 8160 1fc8 a183 ee94 8533 eb5c  ...Y.`.......3.\
-00005b20: 4356 2c9a dd13 3b88 dfa7 6915 3e55 1468  CV,...;...i.>U.h
-00005b30: 1f7b e9af 30fd c413 926c bcf6 d989 0c60  .{..0....l.....`
-00005b40: 1268 5196 2683 fbf4 1380 3c66 8fa8 fede  .hQ.&.....<f....
-00005b50: 184b b29e cd40 9aea fd84 9cce 095a f4b6  .K...@.......Z..
-00005b60: 48ce 04b0 767f 0f1c 0af3 f83c 9587 6dd1  H...v......<..m.
-00005b70: 66d0 6c7a f2e7 88ac 6934 ec60 4b2c d125  f.lz....i4.`K,.%
-00005b80: 3a51 c28e 29da e894 bfd6 c2f5 11e5 e3f6  :Q..)...........
-00005b90: c353 d674 280f 8255 edaf 5092 105b 4747  .S.t(..U..P..[GG
-00005ba0: 215d 2bd1 ee48 dee7 eeac 1320 8dd7 4b84  !]+..H..... ..K.
-00005bb0: bf5a 9139 dd89 3546 1214 bafe a134 f59c  .Z.9..5F.....4..
-00005bc0: 1090 e406 539b 2a09 cce2 f7cd a990 eb44  ....S.*........D
-00005bd0: 0a64 5c2e 2d37 2590 f17e fef0 4841 cc27  .d\.-7%..~..HA.'
-00005be0: 42c5 28a0 d31f 6ec4 ab78 0fd8 baa4 9b50  B.(...n..x.....P
-00005bf0: 6122 cfd5 f600 c519 9b05 6f0d 2169 200c  a"........o.!i .
-00005c00: 34e9 127e ff6e ffde 3ab9 62e8 6dab a7fa  4..~.n..:.b.m...
-00005c10: d129 5963 16a4 41bb c34e d8da aee9 bdcd  .)Yc..A..N......
-00005c20: 9482 9a5f a0f3 b389 750e 9ccc 4c1a 8bbc  ..._....u...L...
-00005c30: 566c 9930 91ac 29cd 84bf 2e52 1c33 08c3  Vl.0..)....R.3..
-00005c40: eb11 b73e 4f49 ad07 bcc4 1697 b162 19b1  ...>OI.......b..
-00005c50: b094 48df e696 c699 b7be 01d6 b014 6417  ..H...........d.
-00005c60: 2e02 4c5b 9ca7 ea16 b43f 8891 a874 5dac  ..L[.....?...t].
-00005c70: d658 9ebb 82ed 84e4 7019 0737 f13d 323a  .X......p..7.=2:
-00005c80: 6036 86f9 2b32 bb98 2958 13ca 1bd0 e156  `6..+2..)X.....V
-00005c90: 2e79 bebe 9e21 f284 0deb fdc0 1dfe cf04  .y...!..........
-00005ca0: 1d82 2706 c2aa 652c c936 7825 7c50 05bc  ..'...e,.6x%|P..
-00005cb0: 67cc d36c af5d 253e acd2 e9d1 e1d1 44ac  g..l.]%>......D.
-00005cc0: 719c a69f 384e c547 e8e0 3dfa 5d90 0b11  q...8N.G..=.]...
-00005cd0: 91ec 3ef1 0622 28e7 142d 593c 1c6b 71ea  ..>.."(..-Y<.kq.
-00005ce0: 4f31 09c4 dfa4 2f5f 214d 85fc 3e38 8c32  O1..../_!M..>8.2
-00005cf0: e586 b42a 2a5d f2e5 f0f9 9190 24cd 0490  ...**]......$...
-00005d00: 2d24 b34b 8e3a e5be d163 7962 e287 925f  -$.K.:...cyb..._
-00005d10: 3772 6a8d 8753 9690 0262 7969 4443 8b6f  7rj..S...byiDC.o
-00005d20: 4d80 2013 38fe 0951 90dc e50d 689b a24d  M. .8..Q....h..M
-00005d30: 8cef e0bc d5eb 07bc 6602 fdaa 9e93 d997  ........f.......
-00005d40: 63b9 5cac de8f e66d b08b 8915 ecb2 7b40  c.\....m......{@
-00005d50: 6099 f78b 61d1 7ce3 a264 6bc9 bac1 0731  `...a.|..dk....1
-00005d60: d811 36e8 ccc7 09bc 84f3 8ff3 1f7f 846a  ..6............j
-00005d70: 90d1 8242 e464 316f ee55 1f67 2ce6 ff3f  ...B.d1o.U.g,..?
-00005d80: bffe 0ff9 f5f2 f599 4ac2 10c8 09f6 1c5c  ........J......\
-00005d90: 5a3e 6c68 9d9a 1f23 7ad7 bf3c 3af8 e1ec  Z>lh...#z..<:...
-00005da0: ece8 fcf0 e8d0 3dbf 34e8 1986 b74e 20ca  ......=.4....N .
-00005db0: 2d57 5cd7 2a34 69ec 7ca8 4b9c c27f 9943  -W\.*4i.|.K....C
-00005dc0: 8948 d306 401d 0a9a 71e5 07bf ad91 5582  .H..@...q.....U.
-00005dd0: 4631 8900 5456 bd8a bc33 86ea ccc7 494a  F1..TV...3....IJ
-00005de0: dc1a f172 aa39 211f 6140 eecc 8aba a51d  ...r.9!.a@......
-00005df0: 0448 8518 8448 7bcb 0436 5bb0 1ba6 4d2a  .H...H{..6[...M*
-00005e00: eb5c 430e e79a e984 a44e 486d 5c34 9a02  .\C......NHm\4..
-00005e10: a317 ec68 89f7 4272 61d1 64cf 60b3 2cb0  ...h..Bra.d.`.,.
-00005e20: cb31 0512 d294 0e19 7f81 0f7a 3156 9413  .1.........z1V..
-00005e30: 9f03 9d31 9644 2bbe 6f80 4cab 58a6 a3a3  ...1.D+.o.L.X...
-00005e40: 6d4e a6c9 df80 72ea dc1f 1ac9 4ff5 e8c4  mN....r.....O...
-00005e50: 1c21 5af9 2a90 d2ec a697 ea83 8312 c316  .!Z.*...........
-00005e60: a5b4 a970 b5e8 1c26 4ff7 4a4f b773 b6c8  ...p...&O.JO.s..
-00005e70: 3fb9 2242 bb33 bdc7 7d9e 24c0 a40b 3d9f  ?."B.3..}.$...=.
-00005e80: f9eb 64ca be84 e5dc 715b 023f 4282 26ae  ..d.....q[.?B.&.
-00005e90: d630 2838 70c3 a961 c0f3 5b4e 19de 8272  .0(8p..a..[N...r
-00005ea0: cf30 9bf5 5463 29de 4578 b7e9 99c7 3c1b  .0..Tc).Ex....<.
-00005eb0: 49e7 b4db 1d0b 98e7 67d7 11fc 822c 424a  I.......g....,BJ
-00005ec0: 3fd7 381f ef00 4a5f ebe0 91bc 6039 20d3  ?.8...J_....`9 .
-00005ed0: 419d 2f0c 1508 d215 be87 1c67 43fa aa37  A./........gC..7
-00005ee0: a868 c4db ce0e 4a3b cf26 58ef a9f3 93ab  .h....J;.&X.....
-00005ef0: c9b6 46a5 e944 a788 8175 b726 8d58 8717  ..F..D...u.&.X..
-00005f00: c3f1 d160 3c56 6038 7cb5 dc99 b0c1 0775  ...`<V`8|......u
-00005f10: 98fc 727b db9b 293b b340 96c6 2152 d00e  ..r{..);.@..!R..
-00005f20: 8593 0f56 52c0 2510 bc53 e110 a34c 0274  ...VR.%..S...L.t
-00005f30: 6909 129a dfca 3c8c e91a 7b3a d5b0 759d  i.....<...{:..u.
-00005f40: 95f9 52e5 bf65 459f c9ac bfee 3eeb 83f7  ..R..eE.....>...
-00005f50: 9cef ec6e fdba bbb5 63fe ace8 7389 c37f  ...n....c...s...
-00005f60: bbc7 cdea c458 1c6b 7861 4f3b b535 4e35  .....X.kxaO;.5N5
-00005f70: 1f39 9a0b 83b3 7bb3 dce2 04b6 1789 0487  .9....{.........
-00005f80: 07b3 5852 1906 b8a0 8a96 92d2 d0ba 2883  ..XR..........(.
-00005f90: 4026 d866 440b 9ad2 2df0 1ffd a4e5 c10c  @&.fD...-.......
-00005fa0: ad18 0776 bf4e ed67 3a9d c322 c012 8459  ...v.N.g:.."...Y
-00005fb0: 05de d173 847a d711 c5af 15ef 834d a920  ...s.z.......M. 
-00005fc0: 8f4c 5135 7050 e71c 3f78 9e92 6663 3345  .LQ5pP..?x..fc3E
-00005fd0: 7195 84f5 8440 3b21 96fa 0531 401e b488  q....@;!...1@...
-00005fe0: 4c63 d389 64ae 8ab0 b295 621f b119 08df  Lc..d.....b.....
-00005ff0: 27ef 80a8 447c 1430 7b09 cad3 a05c 2f51  '...D|.0{....\/Q
-00006000: 7b33 d7ac c6ca 869d a7ee 33cb f408 6855  {3........3...hU
-00006010: 9fa4 6f01 d9ea 84be e5d5 8a85 ba3a b0aa  ..o..........:..
-00006020: 481c fb5e 47bb f726 84a8 fc1a 7516 cdc4  H..^G..&....u...
-00006030: 63c7 1f3e c047 e714 1b29 3ad9 8893 e383  c..>.G...):.....
-00006040: 831d fcdf 6935 ff8e 7a81 72e3 4556 8cfa  ....i5..z.r.EV..
-00006050: 5459 724b 822b 9200 5ff9 4809 3a8c 7391  TYrK.+.._.H.:.s.
-00006060: aee8 5bf2 d733 e8b6 3bb1 2456 9c1a 62c8  ..[..3..;.$V..b.
-00006070: 4d0d 614d d815 368e 091d 9ae6 2c7d 7d7e  M.aM..6.....,}}~
-00006080: c813 573e eb55 ddb6 c6ef b113 2054 37c4  ..W>.U...... T7.
-00006090: 0734 dd21 7c0b 78db 543d 2046 96f6 2f6f  .4.!|.x.T= F../o
-000060a0: 2b12 9e3c 9195 44f2 da2a 9446 2bbc 5ba1  +..<..D..*.F+.[.
-000060b0: 428c eb92 60e5 1986 e4d3 1a1b 910a c8e0  B...`...........
-000060c0: f2f8 546c 2126 ee12 9e2c f26d caa7 b980  ..Tl!&...,.m....
-000060d0: e995 13b8 bd39 5a6f 38f6 ce67 4d42 6b6e  .....9Zo8..gMBkn
-000060e0: 9f36 0978 f9cb 4d02 f3fd 9e34 09b6 6e19  .6.x..M....4..n.
-000060f0: cdbf 5ca4 5757 ed29 3af3 ef4a 369c 0fe2  ..\.WW.):..J6...
-00006100: 1acc 2f2d f2c5 812b 43b7 f4ef 7e14 e69c  ../-...+C...~...
-00006110: 4d36 c37a e905 2764 e67e 4920 200c 3a95  M6.z..'d.~I  .:.
-00006120: 8281 980b 6f52 478e 4747 356a 4d44 446f  ....oRG.GG5jMDDo
-00006130: 42dc 60a0 faec 474b f710 02d8 9e38 6ff0  B.`...GK.....8o.
-00006140: 6399 0b85 9cfb a577 74f4 d589 e76f 3d6c  c......wt....o=l
-00006150: 698d 0054 f1c5 e3db 2cb1 c681 0b9e 39a1  i..T....,.....9.
-00006160: 692d 1692 369a 15fd e561 fb28 1dbd 0fda  i-..6....a.(....
-00006170: 13bd 5ffc ec5d fbc1 27f9 2afb 2958 cd9d  .._..]..'.*.)X..
-00006180: 4faf 1620 d932 cb0b 1b0d f953 76fa 0549  O.. .2.....Sv..I
-00006190: 83f3 8d5d 089c d06d 53a8 7107 bc4b 18ec  ...]...mS.q..K..
-000061a0: 6776 da8d 19b3 21a1 f007 8132 85d6 5664  gv....!....2..Vd
-000061b0: 4383 3a42 4446 40bf 7c80 4892 20ca e720  C.:BDF@.|.H. .. 
-000061c0: bf2d ca1b 031d fb98 c115 ea0e 1011 2d97  .-............-.
-000061d0: 7041 7f37 0750 2d58 d473 5cea dd06 1fdf  pA.7.P-X.s\.....
-000061e0: 04d8 97dc e9c6 e3bc c94f 70b2 1d9a 658e  .........Op...e.
-000061f0: 38ea 0b40 794c c6d7 058a 4d30 4897 febd  8..@yL....M0H...
-00006200: 545d c737 0621 5e2f b107 74a5 ec49 4250  T].7.!^/..t..IBP
-00006210: b9b3 32b2 e992 c22c 3c3f e470 3916 2881  ..2....,<?.p9.(.
-00006220: 82ea 9a44 3a5c a3d2 43b5 6ba1 ffac 1976  ...D:\..C.k....v
-00006230: 52e0 4a30 5c6c 7741 7bc9 eb65 0b24 eaae  R.J0\lwA{..e.$..
-00006240: 1220 feed 3914 6097 30ad f613 fa4d 1119  . ..9.`.0....M..
-00006250: ea25 0a13 14ff 0d66 8748 3bcd 20bd af01  .%.....f.H;. ...
-00006260: eeed ae6a d9ed dad9 0658 ac08 b6b8 067a  ...j.....X.....z
-00006270: 0dc3 8490 8d98 5865 efda 0785 79d2 7f02  ......Xe....y...
-00006280: 5e58 f1b6 8929 64aa 4a6b 2841 bf96 3872  ^X...)d.Jk(A..8r
-00006290: f5ff 7c0f 5358 0e51 4317 a0a5 0660 1149  ..|.SX.QC....`.I
-000062a0: 5e70 cb46 4a08 9f5c bda1 a7b3 f196 ce7a  ^p.FJ..\.......z
-000062b0: 58a7 2926 ce35 ab02 9761 7b18 004d c204  X.)&.5...a{..M..
-000062c0: 5a6f bd4a 066b 6bf7 28c8 1df5 7965 5e76  Zo.J.kk.(...ye^v
-000062d0: 0d60 c01e b2fa 2bc7 b29a af99 a4f4 b6ab  .`....+.........
-000062e0: 0740 e082 3a71 e9b1 8933 b874 c874 aafa  .@..:q...3.t.t..
-000062f0: daeb ddae 1501 d959 70dd 91b8 e5f9 c6b1  .......Yp.......
-00006300: d87b 9104 9219 0479 a73b ae5e ca5f aade  .{.....y.;.^._..
-00006310: f865 e251 9b1e 7f94 1cac e4ff 10ee 4279  .e.Q..........By
-00006320: 23d4 d1cc a14b 3d40 01d3 7e2d 3d43 60ec  #....K=@..~-=C`.
-00006330: dee8 2fe8 e755 fdd7 18bf 0e47 5f6f 95dd  ../..U.....G_o..
-00006340: a18f 0a6c 1d8f 18bc fa7a a496 c001 dd7d  ...l.....z.....}
-00006350: 0e47 a3b1 793b 4de0 8451 f77b e3a5 5dc0  .G..y;M..Q.{..].
-00006360: 63d4 8500 0ae7 249c fa28 6936 677a a56d  c.....$..(i6gz.m
-00006370: 7a01 555f 97f3 40fb 6841 f3e6 ee01 86cf  z.U_..@.hA......
-00006380: 14d8 4cc5 dc0d 5a41 dbb9 a1b5 20dc e280  ..L...ZA.... ...
-00006390: 5e40 f5a4 6b39 4eaa 9711 de6b a602 c3c1  ^@..k9N....k....
-000063a0: b428 2dab 528e 3c84 852c 6026 b4c1 14fc  .(-.R.<..,`&....
-000063b0: 98ce d635 9204 c8a2 f5d0 539f fed7 d4bd  ...5......S.....
-000063c0: adad 5e5b c7d1 e8f1 e2f9 77c4 a3f8 02d2  ..^[......w.....
-000063d0: f977 7d78 638f 90ce bfdb 249d 6176 5008  .w}xc.....$.avP.
-000063e0: 8cfe 84e5 4151 6a59 7b6a 654a e0dc a3f2  ....AQjY{jeJ....
-000063f0: 82f0 6a02 1a90 ec35 f8bc 7650 cccc c221  ..j....5..vP...!
-00006400: 6486 d075 0c2a f7b6 8aa3 25d5 8f11 d65b  d..u.*....%....[
-00006410: a260 30ca f715 49cf ba1c 00c2 c13d fdf9  .`0...I......=..
-00006420: 8373 d54b 7713 6109 690e 052a e6e8 c50a  .s.Kw.a.i..*....
-00006430: 6a6c 9691 d83a 4601 e754 1492 6b78 383f  jl...:F..T..kx8?
-00006440: e0e7 6a82 44ba a420 fb75 4bfa 57c8 9b2b  ..j.D.. .uK.W..+
-00006450: 24be b75a 3087 a5d3 f25d 94b5 10ec 17af  $..Z0....]......
-00006460: 1d9f bc01 d05a 407f 8d97 d5d6 1c3a 12c9  .....Z@......:..
-00006470: 0b7b d4f7 c9d4 61a7 603e 834f bcd7 4199  .{....a.`>.O..A.
-00006480: 2c60 3f1a 9e77 f571 68ca daee 740c 5927  ,`?..w.qh...t.Y'
-00006490: 9e30 ee4d 9447 4096 370c a65b f0cc 0700  .0.M.G@.7..[....
-000064a0: 8b51 cd2f f968 9e10 d7a7 03b8 945e 371d  .Q./.h.......^7.
-000064b0: 091c 0950 17ed 1eaa 7d49 5308 27cf 3acd  ...P....}IS.'.:.
-000064c0: aa7c b7e5 8459 f4ff 93eb 769b 09ca 88db  .|...Y....v.....
-000064d0: bf4d 27de b470 fc4e 0bf9 cef1 fb09 600b  .M'..p.N......`.
-000064e0: 6b6c 2018 f66f d622 4de9 dd43 5b02 fcfc  kl ..o."M..C[...
-000064f0: c1f9 736e ff6a 0721 ef5d 8475 cf45 1bc7  ..sn.j.!.].u.E..
-00006500: cd07 d59d 1c96 74ef 11a7 1329 0eb8 a837  ......t....)...7
-00006510: bd87 8f16 051b db9f 6c7c 7a8c e963 b268  ........l|z..c.h
-00006520: 46e6 5b17 9e96 e084 b873 dc66 ccbb ab71  F.[......s.f...q
-00006530: 9096 cd90 f703 dbf3 fe95 e296 bbb5 9665  ...............e
-00006540: 139c b344 10a5 d2d9 a17a cbed 4d4a adf6  ...D.....z..MJ..
-00006550: 4883 1726 7568 f02e b10f 36ab 023e 9371  H..&uh....6..>.q
-00006560: 5f26 6987 2a96 c92c 3299 9cdb e3c0 b2a4  _&i.*..,2.......
-00006570: 39b2 e9e9 56f0 32f7 d649 6533 7c0d ba66  9...V.2..Ie3|..f
-00006580: e4b6 46a5 6e14 99e9 0a33 728e 66aa 0f62  ..F.n....3r.f..b
-00006590: 0d79 ea70 9447 eab5 a380 37d1 1985 432a  .y.p.G....7...C*
-000065a0: 8c6b cb76 c479 6202 6ae9 da0e f834 032d  .k.v.yb.j....4.-
-000065b0: 0178 0035 7af6 43f9 c5ea 7d93 be68 0ff4  .x.5z.C...}..h..
-000065c0: 13f4 8c35 02d3 3c84 4f9f a700 9e70 e104  ...5..<.O....p..
-000065d0: aaab 8948 4685 d6d8 e68c 3450 2084 acdc  ...HF.....4P ...
-000065e0: 6890 802b 52b6 e3f0 08d4 7c03 49dc e36e  h..+R.....|.I..n
-000065f0: 8d43 342b 3fdf aa4d e240 8594 4e8f 6ddb  .C4+?..M.@..N.m.
-00006600: 4f83 436f bc22 a5f3 5611 e35a 1d47 e535  O.Co."..V..Z.G.5
-00006610: 0596 758c 8841 a8b9 4e5d 15ee 92b8 a991  ..u..A..N]......
-00006620: a22c 0b46 3ea6 45a3 b26c 0f67 9875 304c  .,.F>.E..l.g.u0L
-00006630: 9cbc 1f56 5ccf d06e c7f9 a1c1 19b8 3a1c  ...V\..n......:.
-00006640: 4d77 35bb aa92 8917 8bfb 3c0a f2ae 96a0  Mw5.......<.....
-00006650: f015 838b 2c05 7808 cef6 bcab 1942 ce5a  ....,.x......B.Z
-00006660: 9f1d c25d d44b 4275 86b1 fd01 d526 2446  ...].KBu.....&$F
-00006670: c7ee e1b3 f121 38ac 261d 6cad 72b3 39a4  .....!8.&.l.r.9.
-00006680: d8d0 16c5 b252 4edb 55a7 d007 194f 2a30  .....RN.U....O*0
-00006690: e92e 9af2 9bad 6d77 a0ab ac2a e8bb fd15  ......mw...*....
-000066a0: 7ad5 ab7b 9dec ade9 aea3 6cb7 abd5 2db6  z..{......l...-.
-000066b0: 1f69 fa3e e1fa c4f8 e232 4ceb f592 8cdd  .i.>.....2L.....
-000066c0: 2deb 850f 529d a0ce daaa 1343 3fbe a7cb  -...R......C?...
-000066d0: 3e92 5681 b335 ff27 ac97 0f2f 3dc3 5874  >.V..5.'.../=.Xt
-000066e0: 5758 6d81 0c24 4658 824f 776b 0923 0457  WXm..$FX.Owk.#.W
-000066f0: 164c 534e d993 43f1 8acc 09c1 514b 2862  .LSN..C.....QK(b
-00006700: 1530 536c cf3f 7380 c4cf 906f c0cd 5900  .0Sl.?s....o..Y.
-00006710: a8cb 38c7 5a38 b217 140d b532 4ba8 603a  ..8.Z8.....2K.`:
-00006720: bf1e 4c22 bad0 876f be10 d8fb 0a40 134c  ..L"...o.....@.L
-00006730: e75f 2156 4137 edec 0333 fe61 7777 8c04  ._!VA7...3.aww..
-00006740: da8b 7abb 7d5c 4881 1391 dbd9 ba52 aec0  ..z.}\H......R..
-00006750: 5c28 977c d945 2d69 d247 808e 0411 c579  \(.|.E-i.G.....y
-00006760: 5132 033d 8658 4d94 37e0 5485 d55f c9e0  Q2.=.XM.7.T.._..
-00006770: 64f8 050a afbb b572 3a0d 54c8 9fe2 9e22  d......r:.T...."
-00006780: becc c930 2139 f16e c888 4228 b23c 7b49  ...0!9.n..B(.<{I
-00006790: 86eb 5737 25c1 cb79 add2 7398 d383 354d  ..W7%..y..s...5M
-000067a0: e86b 24e7 9fef a13e 3d4a 98b2 8183 288c  .k$....>=J....(.
-000067b0: 6906 2969 bead bede db0f 0fd6 d667 be4f  i.)i.........g.O
-000067c0: 22ba 8903 956d 068b d5cc b001 386b 41ba  "....m......8kA.
-000067d0: 941c 85fa 685f 6fb2 e1cd 0f9b dfbc a4ec  ....h_o.........
-000067e0: 7d59 50d0 7541 1bd4 b47c 5432 30cd 0d6f  }YP.uA...|T20..o
-000067f0: 88cf 9214 ee51 f34e 3707 775b 1b7c cef5  .....Q.N7.w[.|..
-00006800: f0ae 0391 8aef 862b 3d36 4410 b8ff a3ba  .......+=6D.....
-00006810: 398c 6f3c d337 94d9 9cd0 cb4b 13e5 5709  9.o<.7.....K..W.
-00006820: d326 2809 b5d7 f7bc 39c4 3179 57c7 e630  .&(.....9.1yW..0
-00006830: c894 5c75 e6e2 a17f 1fd0 0ea9 2e04 4336  ..\u..........C6
-00006840: 8492 4504 3072 5e47 e3b6 7c9d 0a38 afa4  ..E.0r^G..|..8..
-00006850: e67c a720 8eb1 978a 2e1d cc71 eb60 385d  .|. .......q.`8]
-00006860: e643 5c8f 920c 83c5 ce34 0dd6 840a edec  .C\......4......
-00006870: be18 7f33 fee6 6fca 22f5 cf4c bae4 e6dd  ...3..o."..L....
-00006880: c6cb 0f74 d2b0 4e56 a80a cc34 5f84 785b  ...t..NV...4_.x[
-00006890: fe5c 085f b8a8 2f45 e96f 3dde a532 4261  .\._../E.o=..2Ba
-000068a0: 8b51 cd0b f395 4b3a 71c9 3a2c d143 cb49  .Q....K:q.:,.C.I
-000068b0: e0a0 83af 952b e89a 193f 7644 20ec 0c93  .....+...?vD ...
-000068c0: 0f85 dbf7 c406 6b9e 636d 7f73 2c29 5432  ......k.cm.s,)T2
-000068d0: a2e2 5260 8cbc 0c00 f192 40a4 82fc 864d  ..R`......@....M
-000068e0: 685b 861a a5fb 845f 797e 6868 dded a6ba  h[....._y~hh....
-000068f0: ccbc 210b ad18 f1db 4cf7 6d12 69a7 906e  ..!.....L.m.i..n
-00006900: 3944 ea4a 048f a85d b10c ec74 8e1a f726  9D.J...]...t...&
-00006910: cadd 43a6 ce39 0de0 d14a f6ad a28f 84ff  ..C..9...J......
-00006920: a51c 5019 97ad 15c8 d180 85e3 bece 42ef  ..P...........B.
-00006930: 496c 9467 e39d c1b8 3a12 6567 d621 7c89  Il.g....:.eg.!|.
-00006940: 3eae ef07 2b3f 278e 3b54 8470 d686 702f  >...+?'.;T.p..p/
-00006950: 15fa d013 09a0 4678 32b5 9b18 8184 941d  ......Fx2.......
-00006960: b867 8a46 d4f7 2de6 9b04 b78b c59b b3c4  .g.F..-.........
-00006970: b727 d492 de98 20b0 606c 5095 a7e8 d2e3  .'.... .`lP.....
-00006980: 973b e6c8 5474 186b d31c c8a4 ae39 6b4c  .;..Tt.k.....9kL
-00006990: f727 467c 1d88 b03e cd5c 9479 1b2a 2261  .'F|...>.\.y.*"a
-000069a0: ad26 bebd ce3b 56d6 4b5f 85c2 5c08 3ea7  .&...;V.K_..\.>.
-000069b0: 70ad 5ac8 4718 269a d915 158e 646c 14df  p.Z.G.&.....dl..
-000069c0: 4b55 d6c0 2f7f 9192 5390 372b 7797 4423  KU../...S.7+w.D#
-000069d0: b260 4370 aa1b e07b 6278 1111 1be1 1a93  .`Cp...{bx......
-000069e0: d1a6 eca5 eca8 fa44 7595 bad4 0b94 a53e  .......Du......>
-000069f0: 95d3 b765 0d11 69f0 8a60 3aa8 50f3 f6bf  ...e..i..`:.P...
-00006a00: 3afb 43ff b9ad 2694 3261 fe2d df8e 58bb  :.C...&.2a.-..X.
-00006a10: 4daf f3be c55a b9f4 e74b d3a6 b258 c751  M....Z...K...X.Q
-00006a20: 5dae c62d 7fdd 578e f111 c27e 449f 7d21  ]..-..W....~D.}!
-00006a30: e62c 9279 b5a3 d77a f0ba c529 a4ef 833d  .,.y...z...)...=
-00006a40: 434f e0a4 0f7b 736a 3f2d 8892 f70a ee87  CO...{sj?-......
-00006a50: 925f 0ede 1f9e a857 f03d f077 ba1d 4d7b  ._.....W.=.w..M{
-00006a60: 78ed 69e5 0bbd f41d 685d 1273 9bda 2598  x.i.....h].s..%.
-00006a70: 2c2f 5f93 62dc c15c 0f42 6723 655e 74ca  ,/_.b..\.Bg#e^t.
-00006a80: c2da ea76 bd2c 69e1 f741 7fb2 bdbf 455c  ...v.,i..A....E\
-00006a90: af44 b1e7 3920 d793 a769 436f 4c1d 645b  .D..9 ...iCoL.d[
-00006aa0: 53a7 d619 3ab8 71c2 883c 8abc 409d 17aa  S...:.q..<..@...
-00006ab0: cf42 da58 f079 3731 641a 8e25 39aa e4bf  .B.X.y71d..%9...
-00006ac0: 0b5b 5c68 adfa da25 ba3c 7516 05a8 44a4  .[\h...%.<u...D.
-00006ad0: 1446 8a0d 05b8 354f 11bb e2bf bcd1 d8a5  .F....5O........
-00006ae0: d055 dbe6 e6a4 f6f4 3447 23ea 8a19 4de7  .U......4G#...M.
-00006af0: f1cc 2d4f 7fc6 704c 6873 b2d7 fac4 23da  ..-O..pLhs....#.
-00006b00: 6a97 c210 3ecf e41b 2e7f e1fc 9690 e2da  j...>...........
-00006b10: 7d94 380c 6643 1802 74c1 3159 485d 0f2e  }.8.fC..t.1YH]..
-00006b20: e73b 57d6 d8d7 f136 e6c4 a44e a46e 45c6  .;W....6...N.nE.
-00006b30: 2ceb 70f2 9294 4af7 f639 47da 38e1 f446  ,.p...J..9G.8..F
-00006b40: 7535 2f19 69ca d096 d24b 3e42 dfcd ccf7  u5/.i....K>B....
-00006b50: c4a2 2c43 cdd6 89d4 93d7 a21c 7657 9802  ..,C........vW..
-00006b60: fbc0 e754 3282 96d2 66ce 931a a5d7 7c83  ...T2...f.....|.
-00006b70: 9e1c a7b8 d319 b7f9 5101 a06e ab4f 82ea  ........Q..n.O..
-00006b80: 18e1 fdc3 f11e 15ae 68d4 b259 c0d1 c848  ........h..Y...H
-00006b90: e096 3efa c2da 95c9 76cc 5be7 d0e8 9b30  ..>.....v.[....0
-00006ba0: 4c89 3bb6 a65e 90aa a2a1 3a7c fa5a 2e3a  L.;..^....:|.Z.:
-00006bb0: c6f8 082b e78c 6c1e d217 b52c 01a2 cccf  ...+..l....,....
-00006bc0: ee9b a992 c4da 11f6 3546 254e b635 aae5  ........5F%N.5..
-00006bd0: 0188 f5a0 4ba1 7541 becc 7293 dccb 8297  ....K.uA..r.....
-00006be0: a068 edfe c4e6 03a2 7cf3 d5b4 7c3b c997  .h......|...|;..
-00006bf0: 180a d712 a4eb b95c 9fcd 47af d473 1bcf  .......\..G..s..
-00006c00: 41aa 18fa 306a b335 2e19 07dd 98ae 1414  A...0j.5........
-00006c10: f27c edc4 32f5 2dbc c47c 6f8c 0d1d 7a3a  .|..2.-..|o...z:
-00006c20: 5ef0 7081 6519 f577 9d04 330f 34e2 f186  ^.p.e..w..3.4...
-00006c30: 2b88 b9c1 f387 1aec 6e68 f0c0 0078 fcc0  +.......nh...x..
-00006c40: db9b 463f e69a ca83 7549 bea5 6d7e 8bf4  ..F?....uI..m~..
-00006c50: f78e b65a 9ca2 32f7 34b0 6b47 d82d a8bf  ...Z..2.4.kG.-..
-00006c60: 1ca1 63f0 b609 81cf 4a45 985f b24b dc13  ..c.....JE._.K..
-00006c70: 843a cd2f d923 e436 4ea7 5495 fe49 9deb  .:./.#.6N.T..I..
-00006c80: 8ad4 3fa9 77a9 5ffd 929d eb08 b044 26e0  ..?.w._......D&.
-00006c90: 3d4b 69ae 5d85 9813 151d d509 4cff 61ca  =Ki.].......L.a.
-00006ca0: 1ba5 e5c9 9bd7 0180 a9ed f4ce 7b86 b57e  ............{..~
-00006cb0: 4ebe 901c ffe8 56ca 7dad 9899 6a00 8161  N.....V.}...j..a
-00006cc0: bb63 c226 e48b f80b a5b4 64d8 1bf4 06ae  .c.&......d.....
-00006cd0: 992f 2b74 fbba 988d 6a20 697c ba48 505f  ./+t....j i|.HP_
-00006ce0: bfaf d3e2 967d 3a07 ae5f e907 aa75 2aa8  .....}:.._...u*.
-00006cf0: 866a 63a9 24df 540d d315 ddf0 99da 5fc1  .jc.$.T......._.
-00006d00: 8ef9 24a5 ba7c 8f52 47d4 23fd c544 0ad6  ..$..|.RG.#..D..
-00006d10: 0bf5 21f5 cc69 dba6 4beb a817 8434 6b1c  ..!..i..K....4k.
-00006d20: 5044 b82a 6b89 6565 3cfe ed99 29a8 c51f  PD.*k.ee<...)...
-00006d30: ca83 c7d3 9728 3c63 2a09 6e7e 4725 f433  .....(<c*.n~G%.3
-00006d40: d51b c247 b488 1275 b145 0aca 2490 6c42  ...G...u.E..$.lB
-00006d50: 30b2 37bb 5549 56c5 6ca0 6850 7fc8 3d19  0.7.UIV.l.hP..=.
-00006d60: 1a78 6361 364d 99f1 97cb e5ee 1cb8 2c26  .xca6M........,&
-00006d70: 6afd 130b 860d 6850 ce3f 2a89 4140 ad85  j.....hP.?*.A@..
-00006d80: 1bef bd66 2da4 6f64 4de3 8fa4 db26 3481  ...f-.odM....&4.
-00006d90: 1ba8 6e19 e0a2 f801 1717 1916 5a7f 9ea6  ..n.........Z...
-00006da0: 54cf 82f3 d65c c080 58b0 5649 1847 2831  T....\..X.VI.G(1
-00006db0: a925 2cb6 8684 a9ea e1b8 3e4f 775e 2f7e  .%,.......>Ow^/~
-00006dc0: d594 fb40 8fc5 9254 2349 fd0d aa46 b5e3  ...@...T#I...F..
-00006dd0: 86d1 91dd b176 4043 1174 f072 86f2 f0d4  .....v@C.t.r....
-00006de0: c289 19dc 77d0 45c9 0d91 fd49 f3b0 a4e9  ....w.E....I....
-00006df0: 31d7 aff2 0c49 7d0c d3bf be58 b121 2505  1....I}....X.!%.
-00006e00: 8087 10d5 56f6 5eb7 7f0b 9a3b eac6 68b2  ....V.^....;..h.
-00006e10: c1a8 61cc 6f11 0271 35ea 82c0 930e b870  ..a.o..q5......p
-00006e20: fa52 d079 f285 e40a 1231 7ab2 edc9 9cf0  .R.y.....1z.....
-00006e30: 3cd7 abef cafb 93fe f5cf ff15 a880 5e44  <.............^D
-00006e40: 164d 062a ef4e fad7 3fff af1c 0edd 4bde  .M.*.N..?.....K.
-00006e50: 85e0 359d 7701 523b 7c18 8660 981e 9792  ..5.w.R;|..`....
-00006e60: 069f ceeb a358 585a 2915 d601 5e92 a170  .....XXZ)...^..p
-00006e70: b6bf bf0f a60a dded 79c3 17a4 d15d 1875  ........y....].u
-00006e80: 1986 a3b1 ea82 8edc 1fd9 9683 c1ce cdd7  ................
-00006e90: 424d 6e91 8027 062d ce12 ae43 a55a 19ba  BMn..'.-...C.Z..
-00006ea0: 8701 f6c4 57bb 0363 7975 a561 9f0f f01d  ....W..cyu.a....
-00006eb0: a94c 876b cdaf 728d 282a 3777 9290 b05d  .L.k..r.(*7w...]
-00006ec0: fd33 05d4 7462 6948 8ac2 9210 8810 a296  .3..tbiH........
-00006ed0: 1139 bd63 8b39 a0b1 d3f2 faa9 5388 45b7  .9.c.9......S.E.
-00006ee0: b958 6756 a314 7963 b9de 4749 8ffa f12f  .XgV..yc..GI.../
-00006ef0: ca3e 6cf5 bfe1 53e2 6b54 c16d ff43 3443  .>l...S.kT.m.C4C
-00006f00: 83c5 d64f e01a 2f8e 8e02 91e1 59cf a32a  ...O../.....Y..*
-00006f10: f033 feb7 6cda 15d2 5eef d9f9 b31e 75d6  .3..l...^.....u.
-00006f20: d345 65ae e379 a8ae c242 e3d2 5888 9216  .Ee..y...B..X...
-00006f30: 3712 dd85 e1e2 b89f b1fe 94d3 d27c cb1e  7............|..
-00006f40: d27b 80da b9ee 958b 4ed9 2738 dfb3 abed  .{......N.'8....
-00006f50: 5cf2 f199 c337 ffb4 27ba 367b 16f1 19f4  \....7..'.6{....
-00006f60: 4487 9752 6eb1 5a05 215d 0358 e2e7 b0a9  D..Rn.Z.!].X....
-00006f70: 13aa e3ad 7122 34e2 08e4 42c7 cdfb 11b2  ....q"4...B.....
-00006f80: c730 7484 59c6 fe2d e396 b489 2a20 a376  .0t.Y..-....* .v
-00006f90: 8942 1398 9790 76b5 0b3b 4f07 f8c6 809b  .B....v..;O.....
-00006fa0: 739a a686 409f fe75 7c1d aace b7c0 28dc  s...@..u|.....(.
-00006fb0: 6c05 8e2a 17a4 0339 acd6 1bdf 524d 0b62  l..*...9....RM.b
-00006fc0: c83f dc21 7f29 76c1 24bd 5c27 5b4f 90fe  .?.!.)v.$.\'[O..
-00006fd0: b115 108d 5564 71e9 c29c 87df dec1 3f5d  ....Udq.......?]
-00006fe0: f5dd ff0b 0000 00ff ff03 0050 4b03 0414  ...........PK...
-00006ff0: 0006 0008 0000 0021 00f1 5ae5 ae55 0100  .......!..Z..U..
-00007000: 006b 0200 0011 0008 0164 6f63 5072 6f70  .k.......docProp
-00007010: 732f 636f 7265 2e78 6d6c 20a2 0401 28a0  s/core.xml ...(.
-00007020: 0001 0000 0000 0000 0000 0000 0000 0000  ................
-00007030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000034e0: b963 2694 b673 c74c 286d e78e 9950 dace  .c&..s.L(m...P..
+000034f0: 1d33 a1b4 9d3b 6642 693b 77cc 84d2 7632  .3...;fBi;w...v2
+00003500: 4c28 6d27 c384 d276 32cc 924a 86c9 90b6  L(m'...v2..J....
+00003510: 9361 4269 3b19 2694 b693 6142 693b 1926  .aBi;.&...aBi;.&
+00003520: 94b6 9361 4269 3b19 2694 b693 6142 693b  ...aBi;.&...aBi;
+00003530: 1926 94b6 9361 4269 3b19 2694 b693 6142  .&...aBi;.&...aB
+00003540: 693b 1966 4925 c364 48db c930 a1b4 9d0c  i;.fI%.dH..0....
+00003550: 134a dbc9 30a1 b49d 0c13 4adb c930 a1b4  .J..0.....J..0..
+00003560: 9d0c 134a dbc9 30a1 b49d 0c13 4adb c930  ...J..0.....J..0
+00003570: a1b4 9d0c 134a dbc9 30a1 b49d 0c13 4adb  .....J..0.....J.
+00003580: c930 4b2a 1926 43da 4e86 09a5 ed64 9850  .0K*.&C.N....d.P
+00003590: da4e 8609 a5ed 6498 50da 4e86 09a5 ed64  .N....d.P.N....d
+000035a0: 9850 da4e 8609 a5ed 6498 50da 4e86 09a5  .P.N....d.P.N...
+000035b0: ed64 9850 da4e 8609 a5ed 6498 2595 0c93  .d.P.N....d.%...
+000035c0: 216d 27c3 84d2 7632 4c28 6d27 c384 d276  !m'...v2L(m'...v
+000035d0: 324c 286d 27c3 84d2 7632 4c28 6d27 c384  2L(m'...v2L(m'..
+000035e0: d276 324c 286d 27c3 84d2 7632 4c28 6d27  .v2L(m'...v2L(m'
+000035f0: c384 d276 324c 286d 27c3 2ca9 6498 0c69  ...v2L(m'.,.d..i
+00003600: 3b19 2694 b693 6142 693b 1926 94b6 9361  ;.&...aBi;.&...a
+00003610: 4269 3b19 2694 b693 6142 693b 1926 94b6  Bi;.&...aBi;.&..
+00003620: 9361 4269 3b19 2694 b693 6142 693b 1926  .aBi;.&...aBi;.&
+00003630: 94b6 9361 9654 324c 86b4 9d0c 134a dbc9  ...a.T2L.....J..
+00003640: 30a1 b49d 0c13 4adb c930 a1b4 9d0c 134a  0.....J..0.....J
+00003650: dbc9 30a1 b49d 0c13 4adb c930 a1b4 9d0c  ..0.....J..0....
+00003660: 134a dbc9 30a1 b49d 0c13 4adb c930 a1b4  .J..0.....J..0..
+00003670: 9d0c b3a4 9261 32a4 ed64 9850 da4e 8609  .....a2..d.P.N..
+00003680: a5ed 6498 50da 4e86 09a5 ed64 9850 da4e  ..d.P.N....d.P.N
+00003690: 8609 a5ed 6498 50da 4e86 09a5 ed64 9850  ....d.P.N....d.P
+000036a0: da4e 8609 a5ed 6498 50da 4e86 5952 c930  .N....d.P.N.YR.0
+000036b0: 19d2 7632 4c28 6d27 c384 d276 324c 286d  ..v2L(m'...v2L(m
+000036c0: 27c3 84d2 7632 4c28 6d27 c384 d276 324c  '...v2L(m'...v2L
+000036d0: 286d 27c3 84d2 7632 4c28 6d27 c384 d276  (m'...v2L(m'...v
+000036e0: 324c 286d 27c3 84d2 769d 6196 589d 613a  2L(m'...v.a.X.a:
+000036f0: a6f0 fa8e 9972 2aaf ef98 29a7 f4aa ab19  .....r*...).....
+00003700: 4986 e963 f55e 6798 729a af33 4c39 ddd7  I..c.^g.r..3L9..
+00003710: 19a6 9cf6 eb0c 534e ff75 8629 e70c a833  ......SN.u.)...3
+00003720: 4c39 e740 9d61 ca39 0bea 0c53 ae63 1e24  L9.@.a.9...S.c.$
+00003730: c384 ebe8 48ea 3b66 ca75 cc83 dcd1 4bae  ....H.;f.u....K.
+00003740: 631e e49e 5e72 5efd f51d 33e5 3ae6 41ee  c...^r^...3.:.A.
+00003750: eb25 d731 0f72 672f b98e 7990 7b7b c975  .%.1.rg/..y.{{.u
+00003760: cc83 dcdd 4bae 631e e4fe 5e72 1df3 2077  ....K.c...^r.. w
+00003770: f892 eb98 07b9 c797 5cc7 3cc8 5dbe e43a  ........\.<.]..:
+00003780: e641 4760 5267 983c b623 31a9 ef98 29d7  .AG`Rg.<.#1...).
+00003790: 310f 72b3 2fb9 8e79 90db 7dc9 75cc 83dc  1.r./..y..}.u...
+000037a0: f04b ae63 1ee4 965f 721d f320 37fd 92eb  .K.c..._r.. 7...
+000037b0: 9807 b9ed 5783 6b67 98ef 7307 cc6f 575f  ....W.kg..s..oW_
+000037c0: 7317 ccde cf8f 19e6 1f0f f9c7 959f 9617  s...............
+000037d0: e7de fcbb b770 f5f1 e74f ff19 5edf 7fbc  .....p...O..^...
+000037e0: fe9a f177 3ff5 e77e fde5 e39b bb0f 73d5  ...w?..~......s.
+000037f0: 52fd c80f 730b 736f 72e0 3ec3 7ffe daef  R...s.sor.>.....
+00003800: cfff f2f6 cf5f 7f79 fbf1 3bb4 fa1d 9a54  ....._.y..;....T
+00003810: 9b03 4686 8c8c 1819 33b2 c6c8 3a23 1b8c  ..F.....3...:#..
+00003820: 6c32 b2c5 c836 233b 8cec 32b2 c7c8 3e23  l2...6#;..2...>#
+00003830: 078c 1c32 72c4 c831 2327 8c9c 3272 c6c8  ...2r..1#'..2r..
+00003840: 3923 178c 5c32 926d f7c9 f344 6176 5d86  9#..\2.m...Dav].
+00003850: d49a 3d17 4ab1 d971 a154 9bfd 164a b969  ..=.J..q.T...J.i
+00003860: 34a1 d49b 4613 4ac1 6934 a154 9c46 134a  4...F.J.i4.T.F.J
+00003870: c969 34a1 d49c 4613 4ad1 6934 a154 9d46  .i4...F.J.i4.T.F
+00003880: 134a d969 344b 2a9b 2b43 dace d60a a5ed  .J.i4K*.+C......
+00003890: 6cac 50da ceb6 0aa5 ed6c aa50 dace 960a  l.P......l.P....
+000038a0: a5ed 6ca8 50da ce76 0aa5 ed6c a650 dace  ..l.P..v...l.P..
+000038b0: 560a a5ed 6ca4 50da ce36 0aa5 ed6c a250  V...l.P..6...l.P
+000038c0: dace 165a 52d9 4119 d276 f64f 286d 67f7  ...ZR.A..v.O(mg.
+000038d0: 84d2 76f6 4e28 6d67 e784 d276 f64d 286d  ..v.N(mg...v.M(m
+000038e0: 67d7 84d2 76f6 4c28 6de7 5699 50da cead  g...v.L(m.V.P...
+000038f0: 32a1 b49d 5b65 4269 7ba0 ed34 9a3c 50db  2...[eBi{..4.<P.
+00003900: 6934 4b2a 8d26 431d 1bb4 b6d3 68f2 406d  i4K*.&C.....h.@m
+00003910: a7d1 84d2 761a 4d28 6da7 d184 d276 1a4d  ....v.M(m....v.M
+00003920: 286d a7d1 84d2 761a 4d28 6da7 d184 d276  (m....v.M(m....v
+00003930: 1a4d 286d a7d1 84d2 761a 4d28 6da7 d12c  .M(m....v.M(m..,
+00003940: a934 9a0c 693b 8d26 94b6 d368 4269 3b8d  .4..i;.&...hBi;.
+00003950: 2694 b6d3 6842 693b 8d26 94b6 d368 4269  &...hBi;.&...hBi
+00003960: 3b8d 2694 b6d3 6842 693b 8d26 94b6 d368  ;.&...hBi;.&...h
+00003970: 4269 3b8d 2694 b6d3 6896 541a 4d86 b49d  Bi;.&...h.T.M...
+00003980: 4613 4adb 6934 a1b4 9d46 134a db69 34a1  F.J.i4...F.J.i4.
+00003990: b49d 4613 4adb 6934 a1b4 9d46 134a db69  ..F.J.i4...F.J.i
+000039a0: 34a1 b49d 4613 4adb 6934 a1b4 9d46 134a  4...F.J.i4...F.J
+000039b0: db69 34a1 b49d 46b3 a4d2 6832 a4ed 349a  .i4...F...h2..4.
+000039c0: 50da 4ea3 09a5 ed34 9a50 da4e a309 a5ed  P.N....4.P.N....
+000039d0: 349a 50da 4ea3 09a5 ed34 9a50 da4e a309  4.P.N....4.P.N..
+000039e0: a5ed 349a 50da 4ea3 09a5 ed34 9a50 da4e  ..4.P.N....4.P.N
+000039f0: a359 5269 3419 d276 1a4d 286d a7d1 84d2  .YRi4..v.M(m....
+00003a00: 761a 4d28 6da7 d184 d276 1a4d 286d a7d1  v.M(m....v.M(m..
+00003a10: 84d2 761a 4d28 6da7 d184 d276 1a4d 286d  ..v.M(m....v.M(m
+00003a20: a7d1 84d2 761a 4d28 6da7 d184 d276 1acd  ....v.M(m....v..
+00003a30: 924a a3c9 90b6 d368 4269 3b8d 2694 b6d3  .J.....hBi;.&...
+00003a40: 6842 693b 8d26 94b6 d368 4269 3b8d 2694  hBi;.&...hBi;.&.
+00003a50: b6d3 6842 693b 8d26 94b6 d368 4269 3b8d  ..hBi;.&...hBi;.
+00003a60: 2694 b6d3 6842 693b 8d66 49a5 d164 48db  &...hBi;.fI..dH.
+00003a70: 6934 a1b4 9d46 134a db69 34a1 b49d 4613  i4...F.J.i4...F.
+00003a80: 4adb 6934 a1b4 9d46 134a db69 34a1 b49d  J.i4...F.J.i4...
+00003a90: 4613 4adb 6934 a1b4 9d46 134a db69 34a1  F.J.i4...F.J.i4.
+00003aa0: b49d 4613 4adb 6934 4b2a 8d26 43da 4ea3  ..F.J.i4K*.&C.N.
+00003ab0: 09a5 ed34 9a50 da4e a309 a5ed 349a 50da  ...4.P.N....4.P.
+00003ac0: 4ea3 09a5 ed34 9a50 da4e a309 a5ed 349a  N....4.P.N....4.
+00003ad0: 50da 4ea3 09a5 ed34 9a50 da4e a309 a5ed  P.N....4.P.N....
+00003ae0: 349a 2595 4693 216d a7d1 84d2 761a 4d28  4.%.F.!m....v.M(
+00003af0: 6da7 d184 d276 1a4d 286d a7d1 84d2 761a  m....v.M(m....v.
+00003b00: 4d28 6da7 d184 d276 1a4d 286d a7d1 84d2  M(m....v.M(m....
+00003b10: 761a 4d28 6da7 d184 d276 1a4d 286d a7d1  v.M(m....v.M(m..
+00003b20: 2ca9 349a 0c69 3b8d 2694 b6d3 6842 693b  ,.4..i;.&...hBi;
+00003b30: 8d26 94b6 d368 4269 3b8d 2694 b6d3 6842  .&...hBi;.&...hB
+00003b40: 693b 8d26 94b6 d368 4269 3b8d 2694 b6d3  i;.&...hBi;.&...
+00003b50: 6842 693b 8d26 94b6 d368 9654 1a4d 86b4  hBi;.&...h.T.M..
+00003b60: 9d46 134a db69 34a1 b49d 4613 4adb 6934  .F.J.i4...F.J.i4
+00003b70: a1b4 9d46 134a db69 34a1 b49d 4613 4adb  ...F.J.i4...F.J.
+00003b80: 6934 a1b4 9d46 134a db69 34a1 b49d 4613  i4...F.J.i4...F.
+00003b90: 4adb 6934 a1b4 9d46 b3a4 d268 32a4 ed34  J.i4...F...h2..4
+00003ba0: 9a50 da4e a309 a5ed 349a 50da 4ea3 09a5  .P.N....4.P.N...
+00003bb0: ed34 9a50 da4e a309 a5ed 349a 50da 4ea3  .4.P.N....4.P.N.
+00003bc0: 09a5 ed34 9a50 da4e a309 a5ed 349a 50da  ...4.P.N....4.P.
+00003bd0: 4ea3 5952 6934 19d2 761a 4d28 6da7 d184  N.YRi4..v.M(m...
+00003be0: d276 1a4d 286d a7d1 84d2 761a 4d28 6da7  .v.M(m....v.M(m.
+00003bf0: d184 d276 1a4d 286d a7d1 84d2 761a 4d28  ...v.M(m....v.M(
+00003c00: 6da7 d184 d276 1a4d 286d a7d1 84d2 761a  m....v.M(m....v.
+00003c10: cd92 4aa3 c990 b6d3 6842 693b 8d26 94b6  ..J.....hBi;.&..
+00003c20: d368 4269 3b8d 2694 b6d3 6842 693b 8d26  .hBi;.&...hBi;.&
+00003c30: 94b6 d368 4269 3b8d 2694 b6d3 6842 693b  ...hBi;.&...hBi;
+00003c40: 8d26 94b6 d368 4269 3b8d 6649 a5d1 6448  .&...hBi;.fI..dH
+00003c50: db69 34a1 b49d 4613 4adb 6934 a1b4 9d46  .i4...F.J.i4...F
+00003c60: 134a db69 34a1 b49d 4613 4adb 6934 a1b4  .J.i4...F.J.i4..
+00003c70: 9d46 134a db69 34a1 b49d 4613 4adb 6934  .F.J.i4...F.J.i4
+00003c80: a1b4 9d46 134a db69 344b 2a8d 2643 da4e  ...F.J.i4K*.&C.N
+00003c90: a309 a5ed 349a 50da 4ea3 09a5 ed34 9a50  ....4.P.N....4.P
+00003ca0: da4e a309 a5ed 349a 50da 4ea3 09a5 ed34  .N....4.P.N....4
+00003cb0: 9a50 da4e a309 a5ed 349a 50da 4ea3 09a5  .P.N....4.P.N...
+00003cc0: ed34 9a25 9546 9321 6da7 d184 d276 1a4d  .4.%.F.!m....v.M
+00003cd0: 286d a7d1 84d2 761a 4d28 6da7 d184 d276  (m....v.M(m....v
+00003ce0: 1a4d 286d a7d1 84d2 761a 4d28 6da7 d184  .M(m....v.M(m...
+00003cf0: d276 1a4d 286d a7d1 84d2 761a 4d28 6da7  .v.M(m....v.M(m.
+00003d00: d12c a934 9a0c 693b 8d26 94b6 d368 4269  .,.4..i;.&...hBi
+00003d10: 3b8d 2694 b6d3 6842 693b 8d26 94b6 d368  ;.&...hBi;.&...h
+00003d20: 4269 3b8d 2694 b6d3 6842 693b 8d26 94b6  Bi;.&...hBi;.&..
+00003d30: d368 4269 3b8d 2694 b6d3 6896 541a 4d86  .hBi;.&...h.T.M.
+00003d40: b49d 4613 4adb 6934 a1b4 9d46 134a db69  ..F.J.i4...F.J.i
+00003d50: 34a1 b49d 4613 4adb 6934 a1b4 9d46 134a  4...F.J.i4...F.J
+00003d60: db69 34a1 b49d 4613 4adb 6934 a1b4 9d46  .i4...F.J.i4...F
+00003d70: 134a db69 34a1 b49d 46b3 a4d2 6832 a4ed  .J.i4...F...h2..
+00003d80: 349a 50da 4ea3 09a5 ed34 9a50 da4e a309  4.P.N....4.P.N..
+00003d90: a5ed 349a 50da 4ea3 09a5 ed34 9a50 da4e  ..4.P.N....4.P.N
+00003da0: a309 a5ed 349a 50da 4ea3 09a5 ed34 9a50  ....4.P.N....4.P
+00003db0: da4e a359 5269 3419 d276 1a4d 286d a7d1  .N.YRi4..v.M(m..
+00003dc0: 84d2 761a 4d28 6da7 d184 d276 1a4d 286d  ..v.M(m....v.M(m
+00003dd0: a7d1 84d2 761a 4d28 6da7 d184 d276 1a4d  ....v.M(m....v.M
+00003de0: 286d a7d1 84d2 761a 4d28 6da7 d184 d276  (m....v.M(m....v
+00003df0: 1acd 924a a3c9 90b6 d368 4269 3b8d 2694  ...J.....hBi;.&.
+00003e00: b6d3 6842 693b 8d26 94b6 d368 4269 3b8d  ..hBi;.&...hBi;.
+00003e10: 2694 b6d3 6842 693b 8d26 94b6 d368 4269  &...hBi;.&...hBi
+00003e20: 3b8d 2694 b6d3 6842 693b 8d66 49a5 d164  ;.&...hBi;.fI..d
+00003e30: 48db 6934 a1b4 9d46 134a db69 34a1 b49d  H.i4...F.J.i4...
+00003e40: 4613 4adb 6934 a1b4 9d46 134a db69 34a1  F.J.i4...F.J.i4.
+00003e50: b49d 4613 4adb 6934 a1b4 9d46 134a db69  ..F.J.i4...F.J.i
+00003e60: 34a1 b49d 4613 4adb 75a3 5962 75a3 e998  4...F.J.u.Ybu...
+00003e70: c2eb 4653 4ee5 75a3 29a7 f4ba d194 537b  ..FSN.u.).....S{
+00003e80: d555 8da4 d1f4 b19a af1b 4d39 ddd7 8da6  .U........M9....
+00003e90: 9cf6 eb46 534e ff75 a329 e70c a81b 4d39  ...FSN.u.)....M9
+00003ea0: e740 dd68 ca39 0bea 4653 ae63 1e74 6424  .@.h.9..FS.c.td$
+00003eb0: f5ad 3279 6c47 4852 df2a 53ae 631e e47e  ..2ylGHR.*S.c..~
+00003ec0: 5f72 1df3 2077 fc92 eb98 07b9 e797 5cc7  _r.. w........\.
+00003ed0: 3cc8 5dbf e43a e641 eefb 25d7 310f 72e7  <.]..:.A..%.1.r.
+00003ee0: 2fb9 8e79 907b 7fc9 75cc 83dc fd4b ae63  /..y.{..u....K.c
+00003ef0: 1ee4 fe5f 721d f320 7700 93eb 9807 b907  ..._r.. w.......
+00003f00: 185c 4760 5237 9a72 1deb 4147 6352 df2a  .\G`R7.r..AGcR.*
+00003f10: d3c7 76cc 83dc 0a4c ae63 1ee4 6660 721d  ..v....L.c..f`r.
+00003f20: f320 b703 93eb 9807 b921 985c c73c c82d  . .......!.\.<.-
+00003f30: c1e4 5af3 a0d5 682e bf2b 1bcd 8e30 737e  ..Z...h..+...0s~
+00003f40: f1a5 cc7c e43f ccf5 1b65 e6ca 7211 6676  ...|.?...e..r.fv
+00003f50: 312b 6d66 f0c2 bcfd 9e73 0e19 1931 326e  1+mf.....s...12n
+00003f60: 8eb4 df46 6fc6 b751 f3c5 db78 5fbe 0d99  ...Fo..Q...x_...
+00003f70: f7ef cab7 f1cc 4cde 4639 325a 2e47 c6cd  ......L.F92Z.G..
+00003f80: 91f6 db98 9ff1 6dd4 7cfb 6dbc ef95 6fa3  ......m.|.m...o.
+00003f90: 8329 52da c1f2 3333 791b e5c8 0866 dc1c  .)R...33y....f..
+00003fa0: 69bf 8d4c 8f76 f8fb caa4 aaf9 fa6d 3c9f  i..L.v.......m<.
+00003fb0: 7e75 b91c 1930 3264 64c4 c8b8 39d2 7e89  ~u...02dd...9.~.
+00003fc0: 698b ffbb 3679 b97e 64d9 262f 941f fa13  i...6y.~d.&/....
+00003fd0: d468 93bf 3f6c 3232 6464 c4c8 b839 d27e  .h..?l22dd...9.~
+00003fe0: fd49 a867 fa88 6bbe 9829 4c78 99de 3b66  .I.g..k..)Lx..;f
+00003ff0: fc33 3499 2ae5 c8a8 eebb 5b3e c7cd 91f6  .34.*.....[>....
+00004000: fb58 9af1 7dd4 7cfb 7df4 de31 e5bb 20e6  .X..}.|.}..1.. .
+00004010: fc33 3479 23e5 c868 b91c 1937 47da 6fa4  .34y#..h...7G.o.
+00004020: be41 712b 767f 65ce 9737 345e 5d2e 4706  .Aq+v.e..74^].G.
+00004030: 8c0c 1919 3132 6e8e b45f 621d eaff 573d  ....12n.._b...W=
+00004040: fef2 53e2 dfee f117 cb39 5ffe 7d01 83ef  ..S......9_.}...
+00004050: 0f6b cef9 9219 c18c 9b23 edd7 5f6f 6cb3  .k.......#.._ol.
+00004060: 7cc4 cf1b e1e4 6f11 e8bd eb97 afba 0b2a  |.....o........*
+00004070: 2ee7 c172 b9a5 0e19 1931 326e 8eb4 dec8  ...r.....12n....
+00004080: ca8c 9bee 235f 4efa f2e3 ef84 968a fdea  ....#_N.........
+00004090: 057a 99f4 8c8c 1819 3747 da6f a4b9 ede6  .z......7G.o....
+000040a0: 5af9 fb29 bfe2 86da 7b57 7e79 e884 ca6f  Z..)....{W~y...o
+000040b0: 0f2f d0e4 6db0 edc2 8c9b 23ed b7d1 dc76  ./..m.....#....v
+000040c0: 5f7f 1b6e a8bd 77e5 5aba d201 f5ca b5f4  _..n..w.Z.......
+000040d0: 059a bc0d b65d 9871 73a4 fd36 9adb eeeb  .....].qs..6....
+000040e0: 6fe3 798b 6d5c 1dbd 7225 5de9 82ca 95f4  o.y.m\..r%].....
+000040f0: 059a bc8d 72fb 1ec1 8c9b 23ed b7d1 dc9a  ....r.....#.....
+00004100: 5f7f 1bcf 3b6d f36d 9417 f94a 1754 5ee4  _...;m.m...J.T^.
+00004110: 2fd0 e46d 94bb f808 66dc 1c69 bf8d e60e  /..m....f..i....
+00004120: fdda db18 acb0 ad32 3262 64dc 1c69 9fbc  .......22bd..i..
+00004130: b9ad e69f 7ff4 2f5e 5979 daf0 da0b 3d8b  ....../^Yy....=.
+00004140: 083b e7f7 874d 16fa 1123 e3e6 48fb b536  .;...M...#..H..6
+00004150: 77ce d77d 877e f94b 617a 3d56 c1f6 615e  w..}.~.Kaz=V..a^
+00004160: 7ab9 c70e 57ca 9111 23e3 e648 fba5 3777  z...W...#..H..7w
+00004170: d4d7 5f7a e8c6 4b67 e56b 1f66 cd2b b7ce  .._z..Kg.k.f.+..
+00004180: e10a 9b29 23e3 e648 fba5 3737 d3d7 5f7a  ...)#..H..77.._z
+00004190: e8c6 4b67 b56b 1d9e 679d 63fb 5c29 4746  ..Kg.k..g.c.\)GF
+000041a0: 8c8c 9b23 ad97 febe b97d befa d26b 7af2  ...#.....}...kz.
+000041b0: d2e7 cb15 ae38 5cae 6d8f e76a fe68 3264  .....8\.m..j.h2d
+000041c0: 64c4 c8b8 39d2 7ee9 336d 98ef 4337 5e7a  d...9.~.3m..C7^z
+000041d0: b9aa 1587 cbf5 ac3e dcfa 163e 6464 c4c8  .......>...>dd..
+000041e0: b839 d27e e933 6d92 ef43 375e 7a79 9916  .9.~.3m..C7^zy..
+000041f0: 8727 9769 fb94 336d 68ef 9bbf 94e8 cd97  .'.i..3mh.......
+00004200: 9757 7178 7279 b54f 39d3 e6f3 beb9 50f6  .Wqxry.O9.....P.
+00004210: e6cb cba2 7db8 3fb9 2cda a79c 65a3 a8de  ....}.?.,...e...
+00004220: 879e 7cb0 7da6 73fb f064 3ab7 4f59 6c0f  ..|.}.s..d:.OYl.
+00004230: 7fff bded 7de8 c629 9986 edc3 9369 d83e  ....}..).....i.>
+00004240: 6573 95cf e478 e594 ad65 bccf f469 1f9e  es...x...e...i..
+00004250: 367d 9aab f3eb a76c 2dbf 7da6 4ffb f0b4  6}.....l-.}.O...
+00004260: e9d3 5c55 5f3f 656b d9ec 337d 5a87 17a6  ..\U_?ek..3}Z...
+00004270: 4c9f fc88 def8 b1e8 d573 3ee2 139b 0be5  L........s>.....
+00004280: 042a 8f4f 9941 bd77 cde5 20ff fca3 df30  .*.O.A.w.. ....0
+00004290: 9e1e 58fe fe64 f22a 5a93 263f aecd f6de  ..X..d.*Z.&?....
+000042a0: 5a4b c042 3953 1f9f aef1 dea7 4cd5 debb  ZK.B9S......L...
+000042b0: e622 f003 9f68 6b15 5828 27eb e3d3 35ce  ."...hk.X('...5.
+000042c0: 3a65 b6f6 de35 d781 1f38 ebd3 37c6 5efd  :e...5...8..7.^.
+000042d0: 4bb3 e243 6b5e dd33 a9e9 f8f6 d758 d48a  K..Ck^.3.....X..
+000042e0: b3cc 7441 e707 bde6 af8c 9d75 adc3 5327  ..tA.......u..S'
+000042f0: dd4c 5774 ef5d f39a 5d71 36b4 0e4f 9d0c  .LWt.]..]q6..O..
+00004300: 335d d2f9 49b0 f93e 9d0b adc3 d3a6 426f  3]..I..>......Bo
+00004310: b64b bac6 277f 51e2 2227 2d8e 4f7b a7bd  .K..'.Q."'-.O{..
+00004320: fff6 927e 7c60 7949 4f5b ae7a b35d d235  ...~|`yIO[.z.].5
+00004330: 3eb9 7816 8baf 96ab bde2 f8b4 85a4 37db  >.x...........7.
+00004340: 255d e38d b396 7ff5 64af 383e 995a ed6b  %]......d.8>.Z.k
+00004350: a437 db25 5de3 8db3 96bf 54ce 4f3b ade3  .7.%].....T.O;..
+00004360: 13cf c559 8beb ffef b7da 5eaf b57f 2f16  ...Y......^.../.
+00004370: 3f32 e513 6e1f 9f6c 8cc5 5967 5b0f 7aad  ?2..n..l..Yg[.z.
+00004380: 2d7c b1f8 6927 676d 1f9f ec8d c559 675b  -|..i'gm.....Yg[
+00004390: 117a cd4b 7ea1 e759 dbc7 a79e 75b6 35a1  .z.K~..Y....u.5.
+000043a0: d7da c897 9cc3 ede3 d3e6 f0fc 6cab 428d  ............l.B.
+000043b0: 4f66 d312 73b8 383e 6d0e cf37 7f64 797d  Of..s.8>m..7.dy}
+000043c0: 5baa f1c6 5999 c3c5 f169 7378 be58 8b5e  [...Y....isx.X.^
+000043d0: 99c3 35de 382b 73b8 383e 6d0e cfcf b636  ..5.8+s.8>m....6
+000043e0: d578 e3ac cca6 e2f8 b4d9 343f dbda 54e3  .x........4?..T.
+000043f0: 93b3 2e33 9b8a e353 67d3 6c6b 53fe 0cb8  ...3...Sg.lkS...
+00004400: 7956 6753 fbf8 d4d9 34db da34 df5a 7b96  yVgS....4..4.Z{.
+00004410: 9d4d ede3 5367 d36c 6bd3 7c6b ed59 7636  .M..Sg.lk.|k.Yv6
+00004420: b58f 4f9d 4db3 ad4d f3ad 9f30 969d 4ded  ..O.M..M...0..M.
+00004430: e353 67d3 6c6b d37c 6bed 5971 36b5 8f4f  .Sg.lk.|k.Yq6..O
+00004440: 9b4d fdd9 d6a6 1a9f 7c63 59e2 eb60 717c  .M......|cY..`q|
+00004450: daf7 c1fe 6c6b 538d 37ce ca17 c2e2 f8b4  ....lkS.7.......
+00004460: ef49 fdd9 d6a6 1a6f 9c95 6f67 c5f1 69df  .I.....o..og..i.
+00004470: 09fb b3ad 4d35 fe72 d685 1e57 4e71 7cda  ....M5.r...WNq|.
+00004480: 95d3 9f6d 6daa f1c6 59b9 728a e3d3 ae9c  ...mm...Y.r.....
+00004490: fe6c 6b53 8d37 3ee1 f247 f75e 717c cacf  .lkS.7>..G.^q|..
+000044a0: eebd fe6c 6b53 8d4f d6e1 1556 c4e2 f8b4  ...lkS.O...V....
+000044b0: 15b1 3fdb da54 e393 4f78 ded9 d45a 9b56  ..?..T..Ox...Z.V
+000044c0: a6ce e1d9 d6a6 7eeb 7bd1 bc5e 5b6b d3ca  ......~.{..^[k..
+000044d0: d4d9 34db dad4 6fae 3d7d 7f9c 6f1d efad  ..4...o.=}..o...
+000044e0: 4cbb 7216 665b 9b6a bcf1 0973 e5b4 8ef7  L.r.f[.j...s....
+000044f0: 1aff f553 fb9b e9c2 7ffb d3d4 e303 cb9f  ...S............
+00004500: a658 abbe 538f 7fe4 529c 78b6 8562 c13f  .X..S...R.x..b.?
+00004510: e243 6f07 33ed d25d 986d c178 c4db 7fb4  .Co.3..].m.x....
+00004520: ddf7 87bc 0eaa b730 f515 ccb6 782c 3cff  .......0....x,<.
+00004530: c95b e362 5e60 f3ed a4a6 6dc1 0bb3 2d24  .[.b^`....m...-$
+00004540: 8f78 f11f a315 ff95 42af 8399 7af6 d916  .x......B...z...
+00004550: 9485 1a2f 0c2c 94bf 8acc a7dd f1df ddbc  .../.,..........
+00004560: bcc8 a709 f8f6 fe8f ebeb 87e1 d5c3 d5af  ................
+00004570: bf7c bbfa fd7a e7ea eef7 9baf f76f 3e5f  .|...z.......o>_
+00004580: ff96 ebe9 dde3 6d1f ee6e 7eaf 7f53 f8f4  ......m..n~..S..
+00004590: 2f0f b7df 723f 88b9 37ff b87d 78b8 fdf2  /...r?..7..}x...
+000045a0: f88f 7f5c 5f7d bace 2d20 defd 142d bfdd  ...\_}..- ...-..
+000045b0: de3e 3cff 4b7e cb55 3fe7 d1f5 c3bf bebd  .><.K~.U?.......
+000045c0: f976 f5ed faee e8e6 ff5d 7f98 cb12 717b  .v.......]....q{
+000045d0: 7793 3b48 5c3d dcdc 7efd 30f7 edf6 eee1  w.;H\=..~.0.....
+000045e0: eeea e661 eecd 9fd7 770f 371f af3e 0fbf  ...a....w.7..>..
+000045f0: dde4 f9e6 dedc fd7c f3e9 c3dc ddc6 a7a7  .......|........
+00004600: 5f99 fd75 7bf7 cfc7 17fc ebff 1700 0000  _..u{...........
+00004610: ffff 0300 504b 0304 1400 0600 0800 0000  ....PK..........
+00004620: 2100 e9a6 25b8 6606 0000 531b 0000 1300  !...%.f...S.....
+00004630: 0000 786c 2f74 6865 6d65 2f74 6865 6d65  ..xl/theme/theme
+00004640: 312e 786d 6cec 59cd 6e1b 3710 be17 e83b  1.xml.Y.n.7....;
+00004650: 107b 4f2c d992 6219 9103 4b96 e236 7162  .{O,..b...K..6qb
+00004660: d84a 8a1c a95d 6a97 1177 b920 293b ba15  .J...]j..w. );..
+00004670: c9b1 4081 a269 d14b 81de 7a28 da06 4880  ..@..i.K..z(..H.
+00004680: 5ed2 a771 9ba2 4d81 bc42 87e4 4a5a 5a54  ^..q..M..B..JZZT
+00004690: 6c27 06fa 171d 6c2d f7e3 fccf 7086 ba7a  l'....l-....p..z
+000046a0: ed41 cad0 2111 92f2 ac15 542f 5702 44b2  .A..!.....T/W.D.
+000046b0: 9047 348b 5bc1 9d7e efd2 7a80 a4c2 5984  .G4.[..~..z...Y.
+000046c0: 19cf 482b 9810 195c db7c ffbd ab78 4325  ..H+...\.|...xC%
+000046d0: 2425 08f6 6772 03b7 8244 a97c 6365 4586  $%..gr...D.|ceE.
+000046e0: b08c e565 9e93 0cde 0db9 48b1 8247 11af  ...e......H..G..
+000046f0: 4402 1f01 dd94 adac 562a 8d95 14d3 2c40  D.......V*....,@
+00004700: 194e 81ec ede1 9086 04f5 35c9 6073 4abc  .N........5.`sJ.
+00004710: cbe0 3153 522f 844c 1c68 d2c4 d961 b0d1  ..1SR/.L.h...a..
+00004720: a8aa 1172 223b 4ca0 43cc 5a01 f089 f851  ...r";L.C.Z....Q
+00004730: 9f3c 5001 6258 2a78 d10a 2ae6 13ac 6c5e  .<P.bX*x..*...l^
+00004740: 5dc1 1bc5 26a6 96ec 2ded eb99 4fb1 afd8  ]...&...-...O...
+00004750: 108d 560d 4f11 0f66 4cab bd5a f3ca f68c  ..V.O..fL..Z....
+00004760: be01 30b5 88eb 76bb 9d6e 7546 cf00 7018  ..0...v..nuF..p.
+00004770: 82a6 5696 32cd 5a6f bdda 9ed2 2c81 ecd7  ..V.2.Zo....,...
+00004780: 45da 9d4a bd52 73f1 25fa 6b0b 3237 dbed  E..J.Rs.%.k.27..
+00004790: 76bd 59c8 6289 1a90 fd5a 5bc0 af57 1ab5  v.Y.b....Z[..W..
+000047a0: ad55 076f 4016 5f5f c0d7 da5b 9d4e c3c1  .U.o@.__...[.N..
+000047b0: 1b90 c537 16f0 bd2b cd46 cdc5 1b50 c268  ...7...+.F...P.h
+000047c0: 365a 406b 87f6 7a05 f519 64c8 d98e 17be  6Z@k..z...d.....
+000047d0: 0ef0 f54a 019f a320 1a66 d1a5 590c 79a6  ...J... .f..Y.y.
+000047e0: 96c5 5a8a ef73 d103 8006 32ac 6886 d424  ..Z..s....2.h..$
+000047f0: 2743 1c42 1477 703a 1014 6b06 7883 e0d2  'C.B.wp:..k.x...
+00004800: 1bbb 14ca 8525 cd0b c950 d05c b582 0f73  .....%...P.\...s
+00004810: 0c19 31a7 f7ea f9f7 af9e 3f45 af9e 3f39  ..1.......?E..?9
+00004820: 7ef8 ecf8 e14f c78f 1e1d 3ffc d1d2 7236  ~....O....?...r6
+00004830: eee0 2c2e 6f7c f9ed 677f 7efd 31fa e3e9  ..,.o|..g.~.1...
+00004840: 372f 1f7f e1c7 cb32 fed7 1f3e f9e5 e7cf  7/.....2...>....
+00004850: fd40 c8a0 b944 2fbe 7cf2 dbb3 272f befa  .@...D/.|...'/..
+00004860: f4f7 ef1e 7be0 5b02 0fca f03e 4d89 44b7  ....{.[....>M.D.
+00004870: c811 dae7 29e8 660c e34a 4e06 e27c 3bfa  ....).f..JN..|;.
+00004880: 09a6 ce0e 9c00 6d0f e9ae 4a1c e0ad 0966  ......m...J....f
+00004890: 3e5c 9bb8 c6bb 2ba0 78f8 80d7 c7f7 1d59  >\....+.x......Y
+000048a0: 0f12 3156 d4c3 f946 923a c05d ce59 9b0b  ..1V...F.:.].Y..
+000048b0: af01 6e68 5e25 0bf7 c759 ec67 2ec6 65dc  ..nh^%...Y.g..e.
+000048c0: 3ec6 873e de1d 9c39 aeed 8e73 a89a d3a0  >..>...9...s....
+000048d0: 746c df49 8823 e61e c399 c231 c988 42fa  tl.I.#.....1..B.
+000048e0: 1d1f 11e2 d1ee 1ea5 8e5d 7769 28b8 e443  .........]wi(..C
+000048f0: 85ee 51d4 c6d4 6b92 3e1d 3881 34df b443  ..Q...k.>.8.4..C
+00004900: 53f0 cbc4 a733 b8da b1cd ee5d d4e6 cca7  S....3.....]....
+00004910: f536 3974 9190 1098 7984 ef13 e698 f13a  .69t....y......:
+00004920: 1e2b 9cfa 48f6 71ca ca06 bf89 55e2 13f2  .+..H.q.....U...
+00004930: 6022 c232 ae2b 1578 3a26 8ca3 6e44 a4f4  `".2.+.x:&..nD..
+00004940: edb9 2d40 df92 d36f 60a8 575e b7ef b249  ..-@...o`.W^...I
+00004950: ea22 85a2 231f cd9b 98f3 3272 9b8f 3a09  ."..#.....2r..:.
+00004960: 4e73 afcc 344b cad8 0fe4 0842 14a3 3dae  Ns..4K.....B..=.
+00004970: 7cf0 5dee 6688 7e06 3fe0 6ca9 bbef 52e2  |.].f.~.?.l...R.
+00004980: b8fb f442 7087 c68e 48f3 00d1 6fc6 a2a8  ...Bp...H...o...
+00004990: da4e fd4d 69f6 ba62 cc28 54e3 77c5 787a  .N.Mi..b.(T.w.xz
+000049a0: 3a6d c1d1 e44b 899d 1325 7819 ee5f 5878  :m...K...%x.._Xx
+000049b0: b7f1 38db 2310 eb8b 07cf bbba fbae ee06  ..8.#...........
+000049c0: fff9 babb 2c97 cf5a 6de7 0516 9ae4 795f  ....,..Zm.....y_
+000049d0: 6cba e474 6993 3ca4 8c1d a809 2337 a5e9  l..ti.<.....#7..
+000049e0: 9325 1c16 510f 164d 036f a6b8 d9d0 9427  .%..Q..M.o.....'
+000049f0: f0b5 28ee 0e2e 16d8 ec41 82ab 8fa8 4a0e  ..(......A....J.
+00004a00: 129c 438f 5d35 235f 2c0b d2b1 4439 9730  ..C.]5#_,...D9.0
+00004a10: db99 6533 7c92 13b4 cd38 49a1 cd36 9361  ..e3|....8I..6.a
+00004a20: 5dcf 0cb6 1e48 ac76 7964 97d7 cab3 e18c  ]....H.vyd......
+00004a30: 8c99 1463 337f 4e19 ad69 0267 65b6 76e5  ...c3.N..i.ge.v.
+00004a40: ed98 55ad 544b cde6 aa56 35a2 9952 e7a8  ..U.TK...V5..R..
+00004a50: 3653 197c b8a8 1a2c ceac 095d 0882 de05  6S.|...,...]....
+00004a60: acdc 8011 5dcb 0eb3 0966 24d2 76b7 73f3  ....]....f$.v.s.
+00004a70: d42d 9af5 85ba 4826 3822 858f b4de 8b3e  .-....H&8".....>
+00004a80: aa1a 274d 6365 1a46 1e1f e939 ef14 1f95  ..'Mce.F...9....
+00004a90: b835 35d9 b7e0 7616 2795 d9d5 96b0 9b7a  .55...v.'......z
+00004aa0: ef6d bc34 1d6e e75e d279 7b22 1d59 564e  .m.4.n.^.y{".YVN
+00004ab0: 4e96 a1a3 56d0 acaf d603 14e2 bc15 0c61  N...V..........a
+00004ac0: ac85 af69 0e5e 97ba f1c3 2c86 bba1 5009  ...i.^....,...P.
+00004ad0: 1bf6 a726 b309 d7b9 379b feb0 acc2 4d85  ...&....7.....M.
+00004ae0: b5fb 82c2 4e1d c885 54db 5826 3634 ccab  ....N...T.X&64..
+00004af0: 2204 5866 8670 23ff 6a1d cc7a 510a d848  ".Xf.p#.j..zQ..H
+00004b00: 7f03 29d6 d621 18fe 3629 c08e ae6b c970  ..)..!..6)...k.p
+00004b10: 4842 5576 7669 c5dc 5118 4051 4af9 5811  HBUvvi..Q.@QJ.X.
+00004b20: 7190 4447 68c0 c662 1f83 fb75 a882 3e11  q.DGh..b...u..>.
+00004b30: 9570 3b61 2a82 7e80 ab34 6d6d f3ca 2dce  .p;a*.~..4mm..-.
+00004b40: 45d2 952f b00c ceae 6396 27b8 28b7 3a45  E../....c.'.(.:E
+00004b50: a799 6ce1 268f 6732 9827 2bad 110f 74f3  ..l.&.g2.'+...t.
+00004b60: ca6e 943b bf2a 26e5 2f48 9572 18ff cf54  .n.;.*&./H.r...T
+00004b70: d1e7 095c 17ac 45da 0321 dce4 0a8c 74be  ...\..E..!....t.
+00004b80: b602 2e54 c2a1 0ae5 090d 7b02 2eb9 4ced  ...T......{...L.
+00004b90: 8068 81eb 5878 0d41 05f7 c9e6 bf20 87fa  .h..Xx.A..... ..
+00004ba0: bfcd 394b c3a4 354c 7d6a 9fc6 4850 388f  ..9K..5L}j..HP8.
+00004bb0: 5422 08d9 83b2 64a2 ef14 62d5 e2ec b224  T"....d...b....$
+00004bc0: 5941 c844 5449 5c99 5bb1 07e4 90b0 beae  YA.DTI\.[.......
+00004bd0: 810d 7db6 0728 8150 37d5 a428 0306 7732  ..}..(.P7..(..w2
+00004be0: fedc e722 8306 b16e 72fe a99d 8f4d e6f3  ..."...nr....M..
+00004bf0: b607 ba3b b02d 96dd 7fc6 5ea4 562a faa5  ...;.-....^.V*..
+00004c00: a3a0 e93d fb4c 4f35 2b07 af39 d8cf 79d4  ...=.LO5+..9..y.
+00004c10: da8a b5a0 f16a fdcc 476d 0e97 3e48 ff81  .....j..Gm..>H..
+00004c20: f38f 8a90 d91f 27f4 81da e7fb 505b 11fc  ......'.....P[..
+00004c30: d660 db2b 0451 7dc9 361e 4817 485b 1e07  .`.+.Q}.6.H.H[..
+00004c40: d038 d945 1b4c 9a94 6d58 8aee f6c2 db28  .8.E.L..mX.....(
+00004c50: b891 2e3a dd19 5fc8 d237 e974 cf69 ec59  ...:.._..7.t.i.Y
+00004c60: 73e6 b273 72f1 f5dd e7f9 8c5d 58d8 b175  s..sr......]X..u
+00004c70: b9d3 f598 1a92 f664 8aea f668 3ac8 18c7  .......d...h:...
+00004c80: 985f b5ca 3f3c f1c1 7d70 f436 5cf1 8f99  ._..?<..}p.6\...
+00004c90: 92f6 6aff 015c f1c1 9461 7f24 80e4 b7ce  ..j..\...a.$....
+00004ca0: 355b 37ff 0200 00ff ff03 0050 4b03 0414  5[7........PK...
+00004cb0: 0006 0008 0000 0021 0037 b198 f114 0300  .......!.7......
+00004cc0: 0090 0a00 000d 0000 0078 6c2f 7374 796c  .........xl/styl
+00004cd0: 6573 2e78 6d6c c456 db6e db30 0c7d 1fb0  es.xml.V.n.0.}..
+00004ce0: 7f10 f4ee fad2 384b 02db 45d3 d440 816d  ......8K..E..@.m
+00004cf0: 18d0 0cd8 ab62 cb89 505d 0c59 699d 0dfb  .....b..P].Yi...
+00004d00: f751 be24 2eda ae69 d7a1 2f96 4453 87a4  .Q.$...i../.DS..
+00004d10: 0e49 293a ab05 47b7 5457 4cc9 18fb 271e  .I):..G.TWL...'.
+00004d20: 4654 662a 6772 1de3 efcb d499 6054 1922  FTf*gr......`T."
+00004d30: 73c2 95a4 31de d10a 9f25 1f3f 4495 d971  s...1....%.?D..q
+00004d40: 7abd a1d4 2080 9055 8c37 c694 33d7 adb2  z... ..U.7..3...
+00004d50: 0d15 a43a 5125 95f0 a750 5a10 034b bd76  ...:Q%...PZ..K.v
+00004d60: ab52 5392 5776 93e0 6ee0 7963 5710 2671  .RS.Wv..n.ycW.&q
+00004d70: 8b30 13d9 3120 82e8 9b6d e964 4a94 c4b0  .0..1 ...m.dJ...
+00004d80: 15e3 ccec 1a2c 8c44 36bb 5a4b a5c9 8a83  .....,.D6.ZK....
+00004d90: abb5 3f22 19aa fdb1 0e7a 0b8d e881 11c1  ..?".....z......
+00004da0: 32ad 2a55 9813 0075 5551 b08c 3ef4 75ea  2.*U...uUQ..>.u.
+00004db0: 4e5d 921d 9000 f675 487e e87a 411b 7812  N].....uH~.zA.x.
+00004dc0: 154a 9a0a 656a 2b4d 8c43 40b7 4ecf 6ea4  .J..ej+M.C@.N.n.
+00004dd0: ba93 a9fd 059c e056 2b89 aa9f e896 7090  .......V+.....p.
+00004de0: f8d8 4da2 4c71 a591 81c3 8658 1b89 2482  ..M.Lq.....X..$.
+00004df0: b61a 1784 b395 6656 ad20 82f1 5d2b 0eac  ......fV. ..]+..
+00004e00: a0e1 a7d3 130c 4ecb 0a5d eb47 6f67 65b5  ......N..].Goge.
+00004e10: dec3 d6e8 ffc6 f57e 311d c74c 4742 3354  .......~1..LGB3T
+00004e20: 4006 e37c 9f1a 81cd 0210 2411 64bd a15a  @..|......$.d..Z
+00004e30: a6b0 40dd 7cb9 2b21 0724 1468 cb65 a3f7  ..@.|.+!.$.h.e..
+00004e40: 8cf6 5a93 9d1f 8483 0d6e 6330 8956 4ae7  ..Z......nc0.VJ.
+00004e50: d010 faa4 b4f9 d78a 9288 d3c2 4072 68b6  ............@rh.
+00004e60: ded8 d1a8 12be 2b65 0cd4 4d12 e58c ac95  ......+e..M.....
+00004e70: 24dc e653 bfa3 9b40 3819 e5fc da36 8d1f  $..S...@8....6..
+00004e80: c53d ecba 4072 2b52 61ae f218 43fb b199  .=..@r+Ra...C...
+00004e90: d84f 2190 6eda e2b5 0b8b 3f44 6bb1 87b0  .O!.n.....?Dk...
+00004ea0: 1ef8 fc72 5c54 177b 034f edf6 c1c1 c7bd  ...r\T.{.O......
+00004eb0: daef 46a4 2cf9 ce56 6f57 974f 6141 5b7a  ..F.,..VoW.OaA[z
+00004ec0: 332c 7b70 c7f9 055a 6fed 5717 f1f3 c82f  3,{p...Zo.W..../
+00004ed0: 3ebd a391 8f8f bfe3 e568 e4d3 97b2 7434  >........h....t4
+00004ee0: f2e8 3df8 3fe7 6c2d 056d 9333 89e0 a268  ..=.?.l-.m.3...h
+00004ef0: 97e8 4e93 7249 eb3e 69dd bae8 ca0c 0a6b  ..N.rI.>i......k
+00004f00: 50bd f76a 775f 85c8 76b8 187f b597 3d87  P..jw_..v.....=.
+00004f10: 5bac 2b24 b4da 326e 987c a46e 0133 af0f  [.+$..2n.|.n.3..
+00004f20: 9dc0 b38d c8d8 8bbb e911 7b2b c06b 4e0b  ..........{+.kN.
+00004f30: b2e5 66b9 ff19 e3c3 fc0b cdd9 564c f75a  ..f.........VL.Z
+00004f40: dfd8 ad32 0d44 8c0f f3cf b661 f963 6b03  ...2.D.....a.ck.
+00004f50: 22fc 5cc1 5507 23da 6a16 e35f 97f3 4fd3  ".\.U.#.j.._..O.
+00004f60: c565 1a38 136f 3e71 46a7 3474 a6e1 7ce1  .e.8.o>qF.4t..|.
+00004f70: 84a3 8bf9 6291 4ebd c0bb f83d 7841 fcc3  ....b.N....=xA..
+00004f80: fba1 79ed 406b f247 b38a c32b 4377 c176  ..y.@k.G...+Cw.v
+00004f90: 215e 1f64 311e 2c5a f79b 560d 6e0f 7d9f  !^.d1.,Z..V.n.}.
+00004fa0: 0663 ef3c f43d 273d f57c 6734 2613 6732  .c.<.='=.|g4&.g2
+00004fb0: 3e0d 9d34 f483 c578 34bf 0cd3 70e0 7bf8  >..4...x4...p.{.
+00004fc0: ca17 8be7 fa7e ff62 a9fd 7066 98a0 9cc9  .....~.b..pf....
+00004fd0: 9eab 9ea1 a114 4882 e55f 8270 7b26 dcc3  ......H.._.p{&..
+00004fe0: 5332 f903 0000 ffff 0300 504b 0304 1400  S2........PK....
+00004ff0: 0600 0800 0000 2100 6fc5 cb0e 3420 0000  ......!.o...4 ..
+00005000: 176c 0000 1400 0000 786c 2f73 6861 7265  .l......xl/share
+00005010: 6453 7472 696e 6773 2e78 6d6c b45d 6d73  dStrings.xml.]ms
+00005020: db46 92fe 7e55 f71f a658 75bb 542c 4a94  .F..~U...Xu.T,J.
+00005030: ecec e6ec 285b d69b ad9c a4c8 129d c4e5  ....([..........
+00005040: 4b50 1008 9238 8300 4380 7ac9 a7fd 2177  KP...8..C.z...!w
+00005050: 7f6e 7fc9 3ddd 3d33 7899 0125 39ce 87dd  .n..=.=3x..%9...
+00005060: d8c4 60a6 31d3 d3d3 fdf4 d3e3 6fff 7137  ..`.1.......o.q7
+00005070: 4fd5 4dbc 2c92 3cdb ebed 6c0d 7b2a cea2  O.M.,.<...l.{*..
+00005080: 7c9c 64d3 bdde fbd1 f1e0 9b9e 2aca 301b  |.d.........*.0.
+00005090: 8769 9ec5 7bbd fbb8 e8fd e3bb 7fff b76f  .i..{..........o
+000050a0: 8ba2 5478 372b f67a b3b2 5cbc dcde 2ea2  ..Tx7+.z..\.....
+000050b0: 593c 0f8b ad7c 1167 7832 c997 f3b0 c45f  Y<...|.gx2....._
+000050c0: 97d3 ed62 b18c c371 318b e372 9e6e ef0e  ...b...q1..r.n..
+000050d0: 877f db9e 8749 d653 51be caca bdde 8b17  .....I.SQ.......
+000050e0: 7fef a955 96fc b68a 0ff4 2fcf 87bd efbe  ...U....../.....
+000050f0: 2d92 efbe 2dbf 3bc9 9232 0953 55c6 f345  -...-.;..2.SU..E
+00005100: bc0c cbd5 3256 1fff eb97 6fb7 cbef bedd  ....2V....o.....
+00005110: a626 d26c 341c b67f 3a0b a759 5c26 914a  .&.l4...:..Y\&.J
+00005120: e36c 5ace d4c7 b9f3 561a ccb9 51fb 5533  .lZ.....V...Q.U3
+00005130: 68b4 5a2e e3ac 541f 5f3b af9e b803 5ec5  h.Z...T._;....^.
+00005140: e944 cd57 e50a e226 d978 1561 eaa2 5861  .D.W...&.x.a..Xa
+00005150: 2296 c99d faf8 76db 15e0 2c98 b7c7 3ed0  ".....v...,...>.
+00005160: 63a6 f14d 9c16 2a2c d5ed 2c89 66aa 9cc5  c..M..*,..,.f...
+00005170: 6a9c 4c26 3149 4433 521b 2229 547c 13a6  j.L&1ID3R.")T|..
+00005180: abb0 8cc7 3e61 27a7 c149 7b1c fc76 dafe  ....>a'..I{..v..
+00005190: ed30 9e24 59cc 4345 7992 aa22 8e4a e806  .0.$Y.CEy..".J..
+000051a0: 24c0 a82a 0e21 c674 99af 162a 9fa8 28bc  $..*.!.t...*..(.
+000051b0: 4ee3 4261 e834 8f68 e076 676f a8e5 283f  N.Ba.4.h.vgo..(?
+000051c0: 4047 57d2 4fbb c545 9e86 cba4 bca7 eee8  @GW.O..E........
+000051d0: f3cc 7427 596b aca2 5c42 0b8b f6fb 0b79  ..t'Yk..\B.....y
+000051e0: 3f89 8b20 c978 b876 8bf3 d5fc 3a5e 52ff  ?.. .x.v....:^R.
+000051f0: b330 9d0c a03d 1944 ae77 df7e 231b 75f7  .0...=.D.w.~#.u.
+00005200: a1c5 b01d f014 a8eb 18bb 638a 3da3 ca5c  ..........c.=..\
+00005210: 856a 112e a174 2b7c 99cc 9533 c095 7c4c  .j...t+|...3..|L
+00005220: 97c8 5a5b 2132 cf37 c9ad 486e d25f d51f  ..Z[!2.7..Hn._..
+00005230: c793 7095 967b 4673 37da ddf3 83ae bee5  ..p..{Fs7.......
+00005240: 03a0 46e1 3c2e 312f 9e2d 31ee 9ccb 4970  ..F.<.1/.-1...Ip
+00005250: 7510 480f 5dfd 1f41 3da1 3137 5021 2c58  u.H.]..A=.17P!,X
+00005260: 41a6 2556 cbb8 480a fc48 0b8d c9d1 43db  A.%V..H..H....C.
+00005270: 2fd9 713e 6112 2cf3 209e 4cba 4639 4e52  /.q>a.,. .L.F9NR
+00005280: 7482 6d59 dea2 e3c1 2229 a197 9e4f 395d  t.mY....")...O9]
+00005290: 049d 7d5c 5e5e 0607 abae 11ae 0eca fb45  ..}\^^.........E
+000052a0: dcf9 74b4 eee9 086f dafd 0155 29a0 0abc  ..t....o...U)...
+000052b0: 89fa 3b7b 6f76 869b 6a77 ef53 b828 f3cc  ..;{ov..jw.S.(..
+000052c0: f9ee aa2d f5d1 35ba e97f 92a4 a9a8 f64d  ...-..5........M
+000052d0: 9e8c 0ba8 6179 1bc7 990a c7ff 1346 343b  ....ay.......F4;
+000052e0: 465b dbe3 6eaa e77b b338 4d56 f34d f562  F[..n..{.8MV.M.b
+000052f0: 8f5e f648 02ed c8c2 f447 eaf9 8f08 6364  .^.H.....G....cd
+00005300: c0ee ad4f 451a e228 5916 ea33 448b ef1e  ...OE..(Y..3D...
+00005310: 29da 7508 9325 3bf4 3619 fbed ffed 3e1a  ).u..%;.6.....>.
+00005320: 754d 3477 1042 87c3 a9e9 6816 27d3 198e  uM4w.B....h.'...
+00005330: 03d7 90cf d6f5 5453 8212 b6fc 5316 176c  ......TS....S..l
+00005340: 85c8 e689 6ce3 64a9 4dad a7ef db93 ac73  ....l.d.M......s
+00005350: 53ae eb5a 4bbb b6ef d99a bec5 503d 6297  S..ZK.......P=b.
+00005360: 754a 77b0 cc8b 6210 e559 1946 a536 047c  uJw...b..Y.F.6.|
+00005370: 267e fc61 e6ce e165 1075 2a7d 340c ceaf  &~.a...e.u*}4...
+00005380: 4749 302b 4d13 af17 e036 6bdb c7fd 68d7  GI0+M....6k...h.
+00005390: ed69 e41c ef9e 66ed 9ea2 9de0 2492 bef4  .i....f.....$...
+000053a0: e9e3 3b7a dd56 4e3f bb9e 7eb6 5d91 2078  ..;z.VN?..~.]. x
+000053b0: 6bbc 764f 23fe fce7 5738 2b3c 1e92 79d8  k.vO#...W8+<..y.
+000053c0: 35c7 f2c9 fc76 d77c e061 d7db dfd3 54e0  5....v.|.a....T.
+000053d0: f910 93f0 d5e8 d7e1 d6d7 dbf3 5f77 7f51  ............_w.Q
+000053e0: fb61 019f 043e 4431 cb97 e5a0 08e7 8b14  .a...>D1........
+000053f0: 3e51 1c16 f0e4 c88a 3ba7 baed a9f3 9449  >Q......;......I
+00005400: b157 9649 041f 285f 8ec5 06d2 56b2 47a5  .W.I..(_....V.G.
+00005410: d365 9c06 dc32 a026 017b 01ae cb17 a549  .e...2.&.{.....I
+00005420: 2696 baf2 6e6e 1318 0e1c 600b 8c48 c7fb  &...nn....`..H..
+00005430: cf2a bc83 c7d3 4fb2 285d 919f 2c07 9db8  .*....O.(]..,...
+00005440: bbf0 940a 853f aa79 b25c e23f 64f4 9679  .....?.y.\.?d..y
+00005450: c97d 3a26 364c 17b3 b038 3c7a d316 e492  .}:&6L...8<z....
+00005460: de30 06e7 fa1e 1e45 142f 4b38 cce8 6f8a  .0.....E./K8..o.
+00005470: a9fb 388e a78e ba9a 6182 6b38 639f da5d  ..8.....a.k8c..]
+00005480: 9e89 3c62 0cc9 9787 d898 afeb 84fc 3b08  ..<b..........;.
+00005490: 8aef 4dca 42fd b60a c738 b64b d51f ee65  ..M.B....8.K...e
+000054a0: f9a6 dad9 8395 7604 978f 7bd2 401f f4ac  ......v...{.@...
+000054b0: 3ddc ed07 7fbf 27d9 3889 e06c 1a3f 515c  =.....'.8..l.?Q\
+000054c0: cff8 2e9a 614e 6815 6631 f9c9 b458 c981  ....aNh.f1...X..
+000054d0: 589b d7f4 993f 91e1 0f46 70cb ec47 db13  X....?...Fp..G..
+000054e0: 2156 4532 8edb 53e5 79fd 7899 3b4e fa1f  !VE2..S.y.x.;N..
+000054f0: 1388 7afc 4322 8d72 577d 3f6f 86de f289  ..z.C".rW}?o....
+00005500: e69b a22c 8412 df3e 3c49 ba87 2f39 4bb5  ...,...><I../9K.
+00005510: 2e9d 697a a258 0fce 542d 2e28 6750 22f2  ..iz.X..T-.(gP".
+00005520: 1a8a 9837 3b02 d20c 9e25 fda8 a670 6a33  ...7;....%...pj3
+00005530: 5526 7357 63ae 4a78 fcef b8ad 6390 d1be  U&sWc.Jx....c...
+00005540: 8ae0 d89f 2f62 b25e 3089 7660 ec3b 1a07  ..../b.^0.v`.;..
+00005550: eafd b170 3676 b9a6 7713 a556 1103 5bc1  ...p6v..w..V..[.
+00005560: 1c56 7691 7bbd 1469 f936 2faf d020 48d6  .Vv.{..i.6/.. H.
+00005570: f47d c94e 3b9f d57a d3dd 86cb 3907 37d5  .}.N;..z....9.7.
+00005580: 364c 96d1 2ac1 401d 87b9 3c76 ec5b a3e7  6L..*.@...<v.[..
+00005590: 083a 0647 cbec ec45 7e0b 7b5e ac16 8bf4  .:.G...E~.{^....
+000055a0: beb3 5f79 a5dd ef71 be84 8863 7593 a725  .._y...q...cu..%
+000055b0: 796c e365 ce71 6a88 7027 1fc3 255f c2e8  yl.e.qj.p'..%_..
+000055c0: dd2f 1131 e04f b0a6 1c70 ae1b fd47 6731  ./.1.O...p...Gg1
+000055d0: de8f 032d af77 a111 254b b78d afc0 7151  ...-.w..%K....qQ
+000055e0: c032 6181 710c 4e26 7c2a d4c7 6e3c c7c9  .2a.q.N&|*..n<..
+000055f0: edd1 81e0 e2a0 3de0 e9fb 11f0 93ac 5ce6  ......=.......\.
+00005600: 298e ada9 aa0f b9a9 46a4 771d 3d05 78f5  ).......F.w.=.x.
+00005610: 69bd 1944 c287 8240 345f 872c 809d 8f38  i..D...@4_.,...8
+00005620: 8b97 d3fb 015c f725 fc40 0214 8afb 0280  .....\.%.@......
+00005630: 0e81 0738 c8a7 53a0 0bc0 2d3c 5f7e 74b4  ...8..S...-<_~t.
+00005640: 5e7d 6822 3b7b efd0 cba3 a3c0 0eba 7e1d  ^}h";{........~.
+00005650: 0f4e 4fde 3d5a 546a dcee eed0 baf5 7a13  .NO.=ZTj......z.
+00005660: 25b4 6240 86f0 b906 ece0 332c 66bf 81d5  %.b@......3,f...
+00005670: 6296 1750 231e 1a0b 3c49 a62b a05e 98b3  b..P#...<I.+.^..
+00005680: 76df d6ad d7cb e31b bf82 3fb8 3f80 6cae  v.........?.?.l.
+00005690: bb95 f95e 94e1 67e1 924f 57b3 a53e 7ab6  ...^..g..OW..>z.
+000056a0: 8403 bb1d 848b 304a 04fa d25f 2dbd c9ef  ......0J..._-...
+000056b0: d87c d761 f649 7d3c 76b6 97a3 e4ae 11e2  .|.a.I}<v.......
+000056c0: 9e52 8213 3bac 4384 51d6 2fea bbb7 8f5e  .R..;.C.Q./....^
+000056d0: d277 6fdb 5d1d b4a7 447f 213a a591 f1dd  .wo.]...D.!:....
+000056e0: f6fb 7c73 1578 7a74 a7cb d399 67b2 3c7d  ..|s.xzt....g.<}
+000056f0: 7518 6d99 af4a 5204 e5c9 0256 1198 2d16  u.m..JR....V..-.
+00005700: 18ae e67a 3b4e 86df 3318 fb56 c66e d3a4  ...z;N..3..V.n..
+00005710: 72af bef0 d5f3 b29c f08f 797b e679 7b64  r.........y{.y{d
+00005720: 8368 bbad 2cca 42d0 0254 4c83 2156 2ef2  .h..,.B..TL.!V..
+00005730: c519 d2ac 05cc d2d4 2331 c5b3 856f 5c0d  ........#1...o\.
+00005740: ed00 d18d 9704 c17e 81e1 0502 79d5 8d0a  .......~....y...
+00005750: 69ac c92b cfe7 cd83 803f d886 7e50 c47c  i..+.....?..~P.|
+00005760: 7df0 d6f1 750c f6f4 7913 501f f729 9fed  }...u...y.P..)..
+00005770: 11e4 5420 fdb6 4e7b 217e 77cf 1d9b 6308  ..T ..N{!~w...c.
+00005780: ef5b 0d89 7240 3db0 cb08 b928 9aa0 4315  .[..r@=....(..C.
+00005790: b90f b2bc 88f7 3238 5507 abc1 0250 5eec  ......28U....P^.
+000057a0: c265 138f aeb4 2204 330c 807a 5fd4 5285  .e....".3..z_.R.
+000057b0: aefe 00c6 0953 debd 0dca fc2d a2d9 11a0  .....S.....-....
+000057c0: e1e0 11ce 776d 04af 0495 808f 0c81 92a6  ....wm..........
+000057d0: 08ae a3cd 3ec0 8442 9d2a 8111 027a 86de  ....>..B.*...z..
+000057e0: 2129 3333 6e6a 3db1 8390 9e90 7371 11c8  !)33nj=.....sq..
+000057f0: ad2e b614 fc3a 41c2 eb19 894d 985b 692a  .....:A....M.[i*
+00005800: d98a 07fa d5ee de0c e85d 0cc4 7892 c4e9  .........]..x...
+00005810: 58e3 a3db 1210 fa9c 0fbf 4f6f bc6e 1d1d  X.........Oo.n..
+00005820: d4c5 37c3 3cf4 691e 7426 9134 970c 3942  ..7.<.i.t&.4..9B
+00005830: aeab bde2 66ad 4739 344b a796 f67d c1fe  ....f.G94K...}..
+00005840: 1100 d26c 0c45 46a4 f1f4 7454 ab73 373d  ...l.EF...tT.s7=
+00005850: 2512 aa31 f207 e2ca 19e7 a09c 0127 99e5  %..1.........'..
+00005860: 9858 8f9b 5024 f3e7 87c1 6a64 dab4 bfee  .X..P$....jd....
+00005870: 0acb 493b 6e02 ff10 eb4d 204a 94e7 fc13  ..I;n....M J....
+00005880: 5017 f845 4827 221d 95c0 7118 2844 f834  P..EH'"...q.(D.4
+00005890: 0368 33ce 6fe1 4b7a c278 196f 12e8 4e02  .h3.o.Kz.x.o..N.
+000058a0: 6af8 85c6 44f6 eb31 23ae 9c15 fccc 6f84  j...D..1#.....o.
+000058b0: 7f0c c8f9 3143 a6f1 a4fc 421f 495d 3d6a  ....1C....B.I]=j
+000058c0: 4c96 ee11 8372 644a 208d 363e 409f f411  L....rdJ .6>@...
+000058d0: 2d38 bd5d d266 a6a0 ddb3 5ed7 a33b da06  -8.].f....^..;..
+000058e0: 0ecc e799 611a d7a8 0f65 4f57 94eb b663  ....a....eOW...c
+000058f0: c3c1 164d 429e d522 4440 e4e1 41d8 473c  ...MB.."D@..A.G<
+00005900: 0daa fffe 7030 f8cb b47c f57e b17d 0865  ....p0...|.~.}.e
+00005910: 7260 312b d9fb c347 4ec7 13c5 12e0 c323  r`1+...GN......#
+00005920: d9e9 a548 768a 35db be24 6de9 16ee f4b2  ...Hv.5..$m.....
+00005930: 2ddc 192c cf7c 3557 c502 6617 7b6c 8e4d  -..,.|5W..f.{l.M
+00005940: 8c4f fe3d deb4 4172 1e22 8d37 e007 94dc  .O.=..Ar.".7....
+00005950: f4a5 3fe4 ebe7 4916 207f 18f1 0b4f 1f88  ..?...I. ....O..
+00005960: 72cf 4f18 869a 770d 92d9 bc6f 86d8 bf4a  r.O...w....o...J
+00005970: f952 3e8a 6668 6032 dbf2 4103 2716 a93e  .R>.fh`2..A.'..>
+00005980: 883b b888 9794 0da1 572f 3005 4f1d 1606  .;......W/0.O...
+00005990: f933 463c 42ca db37 5acb b5a8 2158 8c80  .3F<B..7Z...!X..
+000059a0: d2bc 0083 a675 fcd8 f561 c9f8 ee98 9a9d  .....u...a......
+000059b0: a195 3959 9c58 07e0 7c05 aed7 cfb9 69b8  ..9Y.X..|.....i.
+000059c0: 2a8a 24cc 2886 80d7 7fbd a203 1bfa b215  *.$.(...........
+000059d0: 6f01 8828 40d8 b09c 01da 7ffa a484 3785  o..(@.........7.
+000059e0: 03bd 5b7b 468b 555a c441 71a1 7b68 cb73  ..[{F.UZ.Aq.{h.s
+000059f0: 1187 9f1a 3410 edfd 79a5 f165 4064 4df5  ....4...y..e@dM.
+00005a00: 300b f4e6 e020 8d98 e6b1 5fbc fb55 914c  0.... ...._..U.L
+00005a10: e7e1 831f c699 bef6 471d eae8 de84 1221  ........G......!
+00005a20: 7623 b338 de9c 1cfb 1011 f986 b17e 0b8d  v#.8.........~..
+00005a30: 3a2c 641a 4e83 02c9 cb63 c20f 62c7 526a  :,d.N....c..b.Rj
+00005a40: 6b65 5aad efe7 c7a4 00a5 0526 e14d 9c83  keZ........&.M..
+00005a50: 37b0 bc7f ee98 b85a 7f57 18b5 bb21 3b85  7......Z.W...!;.
+00005a60: 3f4a da81 d926 ac2c 5b0a 7a2e c480 42ad  ?J...&.,[.z...B.
+00005a70: 2861 8453 7f4a c00e a542 d886 13a2 75c3  (a.S.J...B....u.
+00005a80: ef6d a923 22a2 50b8 9902 a885 16c8 6e2f  .m.#".P.......n/
+00005a90: e094 90ee c396 3350 8b7c 4086 73ff a59a  ......3P.|@.s...
+00005aa0: 244b f095 80bb 3269 8030 2728 256b 23b7  $K....2i.0'(%k#.
+00005ab0: db24 9a0b 0e82 760b 027b d12c 5e88 21e4  .$....v..{.,^.!.
+00005ac0: 0403 75b8 89f7 1300 8dad 0eb1 c7b9 bb2d  ..u............-
+00005ad0: 7552 8205 8411 39ef 4979 1b2d 2089 aa5f  uR....9.Iy.- .._
+00005ae0: 2ad0 222d e903 e8c7 e75b ea75 762f 422f  *."-.....[.uv/B/
+00005af0: 7260 442a bc46 34a2 cabd 9de1 70a8 0a7c  r`D*.F4.....p..|
+00005b00: 499a e2d0 52c9 34cb 11a3 6cb5 179d 440d  I...R.4...l...D.
+00005b10: 6476 02a6 5838 0b7e 1933 7108 74a4 1ac9  dv..X8.~.3q.t...
+00005b20: e6f2 879f 4f8e 0818 cde9 2c52 453e 2911  ....O.....,RE>).
+00005b30: ec03 39f4 d09d 96f1 c439 d790 154b 26f7  ..9......9...K&.
+00005b40: c40e e2f7 695a 854f 9544 dac7 9e87 0b4c  ....iZ.O.D.....L
+00005b50: 3ff1 8424 1baf 7d76 2203 9804 5ab2 ccb3  ?..$..}v"...Z...
+00005b60: c17d fe09 401e b347 547f 6f07 4bb2 9a4c  .}..@..GT.o.K..L
+00005b70: 409a eafd 849c ce09 5af4 3648 ce0c b076  @.......Z.6H...v
+00005b80: 7f0f 1c0a f3f8 3c97 876d d126 d06c 7af2  ......<..m.&.lz.
+00005b90: e788 ac69 34ec 604b 2cd1 253a 51c2 8e29  ...i4.`K,.%:Q..)
+00005ba0: dae8 94bf d6c2 f711 f671 fbe1 296b 3a94  .........q..)k:.
+00005bb0: 07c1 aaf6 5728 4988 ada3 a390 ae95 6877  ....W(I.......hw
+00005bc0: 24ef 7377 ce09 90a7 ab39 c25f adc8 9cee  $.sw.....9._....
+00005bd0: c41a 2309 0a5d ff60 4d3d 2704 24b9 c1d4  ..#..].`M='.$...
+00005be0: a64a 02b3 f87d 732a 143a 9102 19e7 73c7  .J...}s*.:....s.
+00005bf0: 4d89 64bc 9f3f 3c52 10f3 8950 310a e8f4  M.d..?<R...P1...
+00005c00: 871b f12a de03 b62e e926 5498 c873 b53d  ...*.....&T..s.=
+00005c10: 4071 c67a c15b 4348 1a08 038d ba84 dfbf  @q.z.[CH........
+00005c20: dbbf 774e ae14 7adb eaa9 7e74 4ad6 9805  ..wN..z...~tJ...
+00005c30: 69d0 eeb0 1336 366b 7aef 32a5 a0e6 17e8  i....66kz.2.....
+00005c40: fc6c e49c 0327 1393 c622 af15 5b26 ce24  .l...'..."..[&.$
+00005c50: 6b4a 3311 aeca 1cc7 0cc2 f07a c4ad cf53  kJ3........z...S
+00005c60: 52eb 012f b1c3 65ac 5846 2c2c 25d2 37b9  R../..e.XF,,%.7.
+00005c70: a571 e69d 6f80 35b4 82ec c245 8069 4b8b  .q..o.5....E.iK.
+00005c80: 5cdd 82f6 0731 3295 afca c50a cb73 57b2  \....12......sW.
+00005c90: 9d90 1c2e e3e0 26be 4746 07cc c6b8 7845  ......&.GF....xE
+00005ca0: 6617 3305 6b42 7903 3adc ec92 17ab eb09  f.3.kBy.:.......
+00005cb0: 224f d8b0 de0f dce1 7f8f d021 7862 20ac  "O.........!xb .
+00005cc0: 3ac6 926c 4360 e183 2ae0 3d63 9e66 7bed  :..lC`..*.=c.f{.
+00005cd0: 2af1 6195 4e8f 0e8f 4662 8dd3 3cff c471  *.a.N...Fb..<..q
+00005ce0: 2a3e 4207 efc9 ef82 5c88 8864 f789 3790  *>B.....\..d..7.
+00005cf0: 4039 c768 c9e2 e158 4bf3 708c 4920 fe26  @9.h...XK.p.I .&
+00005d00: 7df9 0269 2ae4 f7c1 6194 2937 a455 5169  }..i*...a.)7.UQi
+00005d10: cb97 c3e7 2742 9234 1340 b690 cc2e 39ea  ....'B.4.@....9.
+00005d20: 94fb 468f f6c4 c40f 965f 37f4 6a4d 8053  ..F......_7.jM.S
+00005d30: 9690 0262 7969 4443 8bef 4c80 2013 38fe  ...byiDC..L. .8.
+00005d40: 0951 90dc e50d 689b a24d 8cef e0bc d5eb  .Q....h..M......
+00005d50: 07bc 6604 fdaa 9e93 d997 63d9 2e56 ef47  ..f.......c..V.G
+00005d60: f336 d8c5 c40a f6d9 3d20 b0cc fbc5 b068  .6......= .....h
+00005d70: be76 5196 2bc9 bac1 0731 d811 36e8 24c4  .vQ.+....1..6.$.
+00005d80: 093c 87f3 8ff3 1f7f 846a 90d1 8242 1464  .<.......j...B.d
+00005d90: 316f ee55 1f67 2ce6 ffef 5fff 87fc 7af9  1o.U.g,..._...z.
+00005da0: fa4c 6571 0ce4 047b 0e2e 2d1f 36b4 4ecd  .Leq...{..-.6.N.
+00005db0: 8f11 bdeb 5f1e 1dfc 7076 7674 7e78 74e8  ...._...pvvt~xt.
+00005dc0: 9f5f 1af4 0cc3 3b27 10e5 962b ae6b 159a  ._....;'...+.k..
+00005dd0: 3476 3ed4 25cd e1bf 4ca1 44a4 6903 a00e  4v>.%...L.D.i...
+00005de0: 25cd b80a a3df 56c8 2a41 a398 4400 2aab  %.....V.*A..D.*.
+00005df0: 5e45 de19 5bea 2cc4 494a dc1a f172 aa39  ^E..[.,.IJ...r.9
+00005e00: 211f 6140 eecc 82ba a51d 0448 8518 8448  !.a@.......H...H
+00005e10: 7bcb 0436 5bb0 1ba6 4d2a eb5c 430e ef9a  {..6[...M*.\C...
+00005e20: e984 a44e 48ad 5d34 9a02 a317 ec68 89f7  ...NH.]4.....h..
+00005e30: 4272 61d1 64cf 60b3 ccb0 cb31 0512 d258  Bra.d.`....1...X
+00005e40: 878c bf20 04bd 182b ca89 cf81 ce18 4ba2  ... ...+......K.
+00005e50: 15df 3740 a655 2cd3 d1d1 2627 d3e4 6f40  ..7@.U,...&'..o@
+00005e60: 3975 ee0f 8de4 a77a 7462 8e10 ad7c 1548  9u.....ztb...|.H
+00005e70: 6976 d34b f5c1 4389 618b 626d 2a5c 2d3a  iv.K..C.a.bm*\-:
+00005e80: 87c9 d3bd d2d3 ed9d 2df2 4fae 88d0 ee4d  ........-.O....M
+00005e90: ef71 9f27 1930 e952 cf67 f13a 1bb3 2fe1  .q.'.0.R.g.:../.
+00005ea0: 3877 dc96 c08f 98a0 89ab 150c 0a0e dc78  8w.............x
+00005eb0: 6c18 f0fc 9657 86b7 a0dc 33cc e63c d558  l....W....3..<.X
+00005ec0: 4a70 11df ad7b 1630 cf46 d239 ed76 c702  Jp...{.0.F.9.v..
+00005ed0: e685 cbeb 047e c132 414a bfd0 381f ef00  .....~.2AJ..8...
+00005ee0: 4a5f ebe0 91bc 6039 20f3 419d 2f0c 1588  J_....`9 .A./...
+00005ef0: f205 be87 1c67 43fa aa37 a868 c49b de0e  .....gC..7.h....
+00005f00: ac9d 6713 acf7 d4f9 c9d5 6853 a3d2 74a2  ..g.......hS..t.
+00005f10: 53c4 c0ba 5b93 46ac c38b ad9d a3c1 ce8e  S...[.F.........
+00005f20: 02c3 e1ab f9f6 880d 3ea8 c3e4 97bb dbde  ........>.......
+00005f30: 4cd9 9903 b234 0e91 9276 289c 7cb0 9222  L....4...v(.|.."
+00005f40: 2e81 e09d 0a87 1865 12a0 4b4b 90d0 fc56  .......e..KK...V
+00005f50: e661 8c57 d8d3 b986 adeb accc 97aa f86d  .a.W...........m
+00005f60: 59f6 99cc faeb eeb3 3e78 cfc5 f6ee c6af  Y.......>x......
+00005f70: bb1b dbe6 cf8a 3e97 38fc b77b dcac 4e8c  ......>.8..{..N.
+00005f80: c5b1 8617 f6b4 535b e354 f391 a3b9 3038  ......S[.T....08
+00005f90: bbd7 cb2d 4e60 7b91 4870 7830 b339 9561  ...-N`{.Hpx0.9.a
+00005fa0: 800b aa68 2929 0dad 8b32 0864 826d 46b4  ...h))...2.d.mF.
+00005fb0: a029 dd02 ffd1 4f5a 1ecc d082 7160 ffeb  .)....OZ....q`..
+00005fc0: d47e a2d3 392c 022c 41bc acc0 3b7a 8e50  .~..9,.,A...;z.P
+00005fd0: ef3a a1f8 b5e2 7db0 2915 e491 29aa 060e  .:....}.)...)...
+00005fe0: ea9c e307 cf53 d26c 6ca6 24ad 92b0 8110  .....S.ll.$.....
+00005ff0: 6847 c452 bf20 06c8 8316 9169 6c3a 91cc  hG.R. .....il:..
+00006000: 5511 4eb6 52ec 2336 03e1 fbe4 1d10 9588  U.N.R.#6........
+00006010: 8f02 662f 4179 1a94 eb39 6a6f a69a d558  ..f/Ay...9jo...X
+00006020: d9b0 f3dc 7f66 991e 01ad ea93 f42d 205b  .....f.......- [
+00006030: 9dd0 77bc 5ab1 5057 074e 1589 67df eb68  ..w.Z.PW.N..g..h
+00006040: f7de 8410 955f a3ce 9289 78ec f8c3 07f8  ....._....x.....
+00006050: e89c 6223 4527 1b71 727c 70b0 8dff 3bad  ..b#E'.qr|p...;.
+00006060: e6df 532f 6037 5ee2 c4a8 4f95 a570 24b8  ..S/`7^...O..p$.
+00006070: 2209 f095 8f94 a0c3 3897 f982 bea5 783d  ".......8.....x=
+00006080: 816e fb13 4b62 c5a9 2186 5cd7 10d6 845d  .n..Kb..!.\....]
+00006090: 61e3 98d0 a169 ced2 d7e7 873c 71f6 59af  a....i.....<q.Y.
+000060a0: eab6 357e 8f9d 00a1 ba21 3ea0 e98e e15b  ..5~.....!>....[
+000060b0: c0db a6ea 0131 b2b4 7f79 5b91 f0e4 892c  .....1...y[....,
+000060c0: 2492 d756 c11a adf8 6e81 0a31 ae4b 8295  $..V....n..1.K..
+000060d0: 6718 924f 6b6c 442a 2083 cb13 52b1 8598  g..OklD* ...R...
+000060e0: b84b 78b2 c8b7 a990 e602 a657 4ee0 f6e6  .Kx........WN...
+000060f0: 68bd e1d9 3b9f 3509 adb9 7dda 24e0 e52f  h...;.5...}.$../
+00006100: 3709 ccf7 7bd2 24b8 ba65 34ff 7296 5f5d  7...{.$..e4.r._]
+00006110: b5a7 e82c bcb3 6cb8 10c4 3598 5f5a e48b  ...,..l...5._Z..
+00006120: 035f 866e 1ede fd28 cc39 976c 86f5 d20b  ._.n...(.9.l....
+00006130: 4ec8 ccfd 9c40 4018 742a 0503 3117 dea4  N....@@.t*..1...
+00006140: 8e1c 8f8e 6ad4 9a84 88de 84b8 c140 f5d9  ....j........@..
+00006150: 8f96 ee21 04b0 3d71 dee0 c732 170a 39f7  ...!..=q...2..9.
+00006160: cbe0 e8e8 ab93 20dc 78d8 d21a 01a8 e28b  ...... .x.......
+00006170: c777 5962 8d03 173c 7342 d35a 2c24 6d34  .wYb...<sB.Z,$m4
+00006180: 2bfa cbc3 f651 3a7a 1fb5 277a bffc 39b8  +....Q:z..'z..9.
+00006190: 0ea3 4ff2 55ee 53b0 9a3b 9f5e cd40 b265  ..O.U.S..;.^.@.e
+000061a0: 9617 361a f2a7 ecf4 0b92 06e7 1bbb 1038  ..6............8
+000061b0: a1df a650 e30e 7897 30d8 cfec b41b 3366  ...P..x.0.....3f
+000061c0: 4342 e10f 0265 0aad 9dc8 8606 f584 888c  CB...e..........
+000061d0: 807e f900 9124 4194 cf41 7e5b 9437 063a  .~...$A..A~[.7.:
+000061e0: 0e31 830b d41d 2022 9acf e182 fe6e 0ea0  .1.... ".....n..
+000061f0: 5ab0 a8e7 d8ea dd1a 1fdf 04d8 97dc e9da  Z...............
+00006200: e3bc c94f f0b2 1d9a 658e 38ea 4b40 794c  ...O....e.8.K@yL
+00006210: c6d7 058a 4d30 4897 febd 545d c737 0621  ....M0H...T].7.!
+00006220: 5e2f b107 74a5 ec49 4650 b9b7 32b2 e992  ^/..t..IFP..2...
+00006230: c22c 3c3f e470 3915 2881 82ea 9a44 3a5c  .,<?.p9.(....D:\
+00006240: a3d2 43b5 eba0 ffac 196e 52e0 4a30 5c6c  ..C......nR.J0\l
+00006250: 7741 7bc9 eb65 0b24 eaae 3220 feed 3914  wA{..e.$..2 ..9.
+00006260: 6097 30ad f613 fa4d 1119 ea25 0a13 14ff  `.0....M...%....
+00006270: 0d66 8748 3bcd 20bd af01 eecd ae6a d9cd  .f.H;. ......j..
+00006280: dad9 0658 ac8c 36b8 067a 05c3 8490 8d98  ...X..6..z......
+00006290: 58b6 77ed 83c2 3ce9 3f01 2fac 78db c414  X.w...<.?./.x...
+000062a0: 3255 a535 94a0 5f4b 1cf9 fa7f be87 29b4  2U.5.._K......).
+000062b0: 43d4 d005 68a9 0158 4492 17dc b291 12c2  C...h..XD.......
+000062c0: 2757 6fe8 e96c bca5 b31e ce69 8a89 f3cd  'Wo..l.....i....
+000062d0: aac0 65d8 1e06 4093 3081 d65b af92 c1da  ..e...@.0..[....
+000062e0: da3d 0a72 477d 5e99 977d 0318 b087 acfe  .=.rG}^..}......
+000062f0: c2b3 ace6 6b46 39bd edeb 0110 b8a0 4e5c  ....kF9.......N\
+00006300: 7a6c e20c 2e1d 329d aabe f67a 376b 4540  zl....2....z7kE@
+00006310: 6e16 5c77 246e 79b1 762c f65e 2481 6406  n.\w$ny.v,.^$.d.
+00006320: 41de e98e ab97 8a97 aab7 f332 0ba8 4d8f  A..........2..M.
+00006330: 3f4a 0e56 f27f 0877 a1bc 11ea 68a6 d0a5  ?J.V...w....h...
+00006340: 1ea0 8071 bf96 9e21 3076 6ff8 17f4 f3aa  ...q...!0vo.....
+00006350: fe6b 8a5f b786 5f6f d8ee d047 05b6 ee0c  .k._.._o...G....
+00006360: 19bc fa7a a8e6 c001 fd7d 6e0d 873b e6ed  ...z.....}n..;..
+00006370: 3c83 1346 ddef edcc dd02 1ea3 2e04 5078  <..F..........Px
+00006380: 27e1 3444 49b3 39d3 2b6d d30b a8fa ba9c  '.4DI.9.+m......
+00006390: 07da 470b 5a34 770f 307c a6c0 2e55 cadd  ..G.Z4w.0|...U..
+000063a0: a015 b49d 1b3a 0bc2 2d0e e805 544f fa96  .....:..-...TO..
+000063b0: e3a4 7a19 e1bd 662a 301c 4c8b d2b2 2a76  ..z...f*0.L...*v
+000063c0: e42d 58c8 1266 421b 4cc1 8fe9 6c5d 2149  .-X..fB.L...l]!I
+000063d0: 802c 5a0f 3df5 e97f 4ddd dbd8 e8b5 751c  .,Z.=...M.....u.
+000063e0: 8d1e 2f5e 7847 3c8a 2f20 5d78 d787 37f6  ../^xG<./ ]x..7.
+000063f0: 08e9 c2bb 75d2 1966 0785 c0e8 4f58 1e14  ....u..f....OX..
+00006400: a5da da53 2753 02e7 1e95 1784 5713 d080  ...S'S......W...
+00006410: 64af c1e7 b583 6266 160e 2133 84ae 5350  d.....bf..!3..SP
+00006420: b937 559a cca9 7e8c b05e 8b82 c128 df57  .7U...~..^...(.W
+00006430: 243d e772 0008 07f7 f4e7 0fde 55b7 ee26  $=.r........U..&
+00006440: c212 d21c 0a54 ccd1 8b15 d4d8 2c23 b175  .....T......,#.u
+00006450: 8c02 cea9 2824 d7f0 707e 202c d408 8974  ....($..p~ ,...t
+00006460: 4941 f6eb 96f4 af90 b750 487c 6fb4 600e  IA.......PH|o.`.
+00006470: 47a7 e5bb 286b 21d8 2f5e 3b3e 7903 a0b5  G...(k!./^;>y...
+00006480: 84fe 1a2f abad 3974 2492 17f6 a8ef 93a9  .../..9t$.......
+00006490: c34e c17c 469f 78af 8332 59c2 7e34 3cef  .N.|F.x..2Y.~4<.
+000064a0: eae3 d094 b5dd eb18 b24e 3c61 dc9b a448  .........N<a...H
+000064b0: 802c af19 4cb7 e099 8f00 16a3 9a5f f2d1  .,..L........_..
+000064c0: 3c21 be4f 0770 29bd ae3b 1238 12a0 2eda  <!.O.p)..;.8....
+000064d0: 3d54 fb92 a610 4e9e 739a 55f9 6ec7 0973  =T....N.s.U.n..s
+000064e0: e8ff 27d7 ed36 2394 11b7 7f1b 8f82 71e9  ..'..6#.......q.
+000064f0: f99d 16f2 9de7 f713 c016 ced8 4030 dcdf  ............@0..
+00006500: 9c45 1ad3 bb87 ae04 f8f9 83f7 e7c2 fdd5  .E..............
+00006510: 0d42 defb 08eb 818f 368e 9b0f aa3b 391c  .B......6....;9.
+00006520: e9de 234e 2752 1c70 d160 7c0f 1f2d 89d6  ..#N'R.p.`|..-..
+00006530: b63f 59fb f418 d3c7 64d1 2599 6f5d 786a  .?Y.....d.%.o]xj
+00006540: c109 71e7 b8cd 0eef aec6 416a 9b21 ef07  ..q.......Aj.!..
+00006550: b6e7 fd2b c52d 776b 2d6d 139c b344 10a5  ...+.-wk-m...D..
+00006560: d2d9 2df5 96db 9b94 5aed 9106 2f4c ead0  ..-.....Z.../L..
+00006570: e05d 621f 5c56 057c 26e3 be8c f20e 55b4  .]b.\V.|&.....U.
+00006580: c92c 3299 9cdb e3c0 d2d2 1cd9 f474 2bb8  .,2..........t+.
+00006590: cdbd 7552 d90c 5f83 ae19 b9ad 51a9 1b45  ..uR.._.....Q..E
+000065a0: 66ba c28c 9ca3 89ea 8358 439e 3a1c e5a1  f........XC.:...
+000065b0: 7aed 29e0 cd74 46e1 900a e3da b21d 719e  z.)..tF.......q.
+000065c0: 9880 5aba b603 3ecd 404b 001e 408d 9efd  ..Z...>.@K..@...
+000065d0: 507e b17a dfa4 2fda 03fd 043d 638d c034  P~.z../....=c..4
+000065e0: 6fc1 a72f 7200 4fb8 7002 d5d5 4424 a342  o../r.O.p...D$.B
+000065f0: 6b6c 7346 1a28 1042 566e 38c8 c015 b1ed  klsF.(.BVn8.....
+00006600: 383c 0235 df40 12f7 b85b e310 cdec e73b  8<.5.@...[.....;
+00006610: b549 1ca8 90d2 e9b1 5dfb 6970 e8b5 57a4  .I......].ip..W.
+00006620: 74de 2a62 5cab e3c4 5e53 e058 c784 1884  t.*b\...^S.X....
+00006630: 9aeb d455 e12e 899b 1a29 cab1 60e4 633a  ...U.....)..`.c:
+00006640: 342a c7f6 7086 5907 c3c4 c9fb 61c1 f50c  4*..p.Y.....a...
+00006650: ed76 9c1f 1a9c 81ab c3d1 7457 b3ab 2a99  .v........tW..*.
+00006660: 7831 bb2f 92a8 e86a 090a 5f39 b858 e600  x1./...j.._9.X..
+00006670: 0fc1 d99e 7635 43c8 59eb b343 b88b 7a49  ....v5C.Y..C..zI
+00006680: a8ce 30b6 3fa0 da84 c4e8 d83d 7cb6 7308  ..0.?......=|.s.
+00006690: 0eab 4907 3bab dc6c 0e29 d6b4 45b1 ac94  ..I.;..l.)..E...
+000066a0: d376 d529 f441 c693 0a4c ba8b c67e b3b3  .v.).A...L...~..
+000066b0: ed0e 7495 5505 7db7 bf42 af7a 75af 93bb  ..t.U.}..B.zu...
+000066c0: 35fd 7594 ed76 b5ba c5f6 234d df27 5c9f  5.u..v....#M.'\.
+000066d0: 185f 5c86 e9bc 6ec9 d8dd b25e 8420 d509  ._\...n....^. ..
+000066e0: eaac ad3a 31f4 d37b baec 236b 1538 3bf3  ...:1..{..#k.8;.
+000066f0: 7fc2 7af9 f0d2 338c 4577 85d5 16c8 4062  ..z...3.Ew....@b
+00006700: 8425 8474 b796 3042 7065 c138 e794 3d39  .%.t..0Bpe.8..=9
+00006710: 14af c89c 101c 3587 2256 0133 c5f6 fc33  ......5."V.3...3
+00006720: 0748 fc0c f906 dc9c 0580 dac6 39ce c291  .H..........9...
+00006730: bda0 68a8 9559 4205 d3f9 f560 94d0 853e  ..h..YB....`...>
+00006740: 7cf3 85c0 de57 009a 603a ff0a b14a ba69  |....W..`:...J.i
+00006750: 671f 98f1 0fbb bb3b 48a0 bda8 b7db c785  g......;H.......
+00006760: 1438 11b9 9dab 2b76 05a6 42b9 e4cb 2e6a  .8....+v..B....j
+00006770: 4993 3e02 7424 8828 ce4b b209 e831 c46a  I.>.t$.(.K...1.j
+00006780: a2bc 01a7 2a9c fe2c 8393 e117 28bc eed6  ....*..,....(...
+00006790: c9e9 3450 a170 8c7b 8af8 3227 c384 e4c4  ..4P.p.{..2'....
+000067a0: bb21 230a a1c8 f1ec 2519 ae5f 5d97 04b7  .!#.....%.._]...
+000067b0: f35a a5e7 30a7 072b 9ad0 d748 ce3f df43  .Z..0..+...H.?.C
+000067c0: 7d7a 9231 6503 0751 9cd2 0c52 d27c 537d  }z.1e..Q...R.|S}
+000067d0: bdb7 1f1f ac9c cf7c 9f25 7413 072a db0c  .......|.%t..*..
+000067e0: 16ab 9961 0370 d6a2 7c2e 390a f5d1 bdde  ...a.p..|.9.....
+000067f0: 64cd 9b1f d6bf 7949 d97b 5b50 d075 411b  d.....yI.{[P.uA.
+00006800: d4d4 3eb2 0c4c 73c3 1be2 b32c 877b d4bc  ..>..Ls....,.{..
+00006810: d3cd c3dd d606 9f73 3dbc eb40 a4e2 bbe1  .......s=..@....
+00006820: acc7 8608 02f7 7f54 3787 f18d 67fa 8632  .......T7...g..2
+00006830: 9713 7a79 69a2 fc2a 61da 0425 a1f6 fa9e  ..zyi..*a..%....
+00006840: 378f 3826 efea d91c 0699 92ab ce7c 3cf4  7.8&.........|<.
+00006850: ef23 da21 d585 60c8 8650 b288 0046 ceeb  .#.!..`..P...F..
+00006860: 68dc 96af 5301 e795 d49c ef14 c431 f652  h...S........1.R
+00006870: d1a5 8305 6e1d 8cc7 f362 0bd7 a364 5bd1  ....n....b...d[.
+00006880: 6c7b 9c47 2b42 85b6 775f ec7c b3f3 cddf  l{.G+B..w_.|....
+00006890: 9443 ea9f 9874 c9cd bbb5 971f e8a4 619d  .C...t........a.
+000068a0: ac50 1598 69be 08f1 b6c2 a910 be70 515f  .P..i........pQ_
+000068b0: 8ed2 df7a bc4b 6584 c216 a39a 17e6 2b5b  ...z.Ke.......+[
+000068c0: 3ab1 651d 5af4 d071 1238 e8e0 6be5 4aba  :.e.Z..q.8..k.J.
+000068d0: 6626 4c3d 1108 3bc3 e443 e1f6 3db1 c19a  f&L=..;..C..=...
+000068e0: e758 dbdf 1c4b 0a95 8ca8 b814 1823 2f03  .X...K.......#/.
+000068f0: 40dc 1288 5454 dcb0 096d cb50 a374 9ff0  @...TT...m.P.t..
+00006900: 2bcf 0f0d adbb dd54 9799 3764 a115 237e  +......T..7d..#~
+00006910: 9be9 be4d 22ed 14d2 2f87 485d 8910 10b5  ...M".../.H]....
+00006920: 2b95 81bd ce51 e3de 44b9 7bc8 d439 e711  +....Q..D.{..9..
+00006930: 3c5a c9be 55f4 91f8 3f95 072a e3b2 b512  <Z..U...?..*....
+00006940: 391a b070 fcd7 59e8 3d89 8df2 6c67 7bb0  9..p..Y.=...lg{.
+00006950: 531d 89b2 33eb 10be 441f d7f7 8345 5810  S...3...D....EX.
+00006960: c71d 2a42 386b 43b8 970a 7de8 8904 5023  ..*B8kC...}...P#
+00006970: 3c99 da4d 8c40 426c 07fe 99a2 11f5 7d8b  <..M.@Bl......}.
+00006980: c53a c1dd 62f1 e62c f1ed 09b5 a437 2608  .:..b..,.....7&.
+00006990: 2c18 1754 e529 ba0c f8e5 8e39 3215 1dc6  ,..T.).....92...
+000069a0: da34 0732 a96b ce1a d3fd 8909 5f07 22ac  .4.2.k......_.".
+000069b0: 4f33 1736 6f43 4524 acd5 c4b7 d779 c7ca  O3.6oCE$.....y..
+000069c0: 7ae9 ab50 980b c1e7 14ae 558b f908 c344  z..P......U....D
+000069d0: 33bb a2c2 918c 8de2 7ba9 6c0d fcfc 1729  3.......{.l....)
+000069e0: 3905 79b3 7277 4934 220b 3604 a7ba 01be  9.y.rwI4".6.....
+000069f0: 2786 1711 b111 ae31 19ae cb5e ca8e aa4f  '......1...^...O
+00006a00: 5457 a94b bd40 59ea 5339 7d6b 6b88 4883  TW.K.@Y.S9}kk.H.
+00006a10: 1704 d341 859a b7ff d5d9 1ffa cf6d 35a1  ...A.........m5.
+00006a20: 9409 f36f f976 c4da 6d7a 9df7 2dd6 caa5  ...o.v..mz..-...
+00006a30: 3f5f 9a36 95c5 398e ea72 356e f9eb be72  ?_.6..9..r5n...r
+00006a40: 8c8f 10f6 23fa ec0b 3167 91cc ab1b bdd6  ....#...1g......
+00006a50: 83d7 0d4e 217d 1fed 197a 0227 7dd8 9b53  ...N!}...z.'}..S
+00006a60: fb79 4994 bc57 703f 94fc 72f0 fef0 44bd  .yI..Wp?..r...D.
+00006a70: 82ef 81bf d3ed 68da c36b 4f2b 5fe8 55bb  ......h..kO+_.U.
+00006a80: e092 65e1 2b50 8cab 57e8 0ee8 dca3 ac8a  ..e.+P..W.......
+00006a90: 4e47 38db d8ad 8525 0dfb 3eea 8f36 f737  NG8....%..>..6.7
+00006aa0: 88c7 9529 f62a 07e4 56f2 14ac e98d 6981  ...).*..V.....i.
+00006ab0: 6c47 eab4 3943 f536 0e16 1143 81f9 d739  lG..9C.6...C...9
+00006ac0: 9ffa 9ca3 4d03 7f76 1dfb a5e1 3492 134a  ....M..v....4..J
+00006ad0: beb9 30c1 85b2 aaaf 54a2 8b51 2749 842a  ..0.....T..Q'I.*
+00006ae0: 434a 4fe4 d82c 8052 8b1c 7129 fecb 9b88  CJO..,.R..q)....
+00006af0: dd05 5d91 6d6e 456a 4f4f 7334 a2a5 98d1  ..].mnEjOOs4....
+00006b00: 748e cedc e0f4 670c c764 352f 33ad 4f1c  t.....g..d5/3.O.
+00006b10: a18d 7699 0b61 ef4c ace1 d216 ce5d 09e1  ..v..a.L.....]..
+00006b20: addd 87c5 5830 1b92 fda7 cb8b c9fa e95a  ....X0.........Z
+00006b30: 6f39 bbb9 6ac6 bd6a b731 2726 2d22 3529  o9..j..j.1'&-"5)
+00006b40: 32a6 adb1 292c e194 eee4 f38e b476 c2e9  2...),.......v..
+00006b50: 8dea da5d 32c0 947d b5d2 4bae 41df bbcc  ...]2..}..K.A...
+00006b60: 77c0 a2e4 424d 5699 d48a d722 1876 4598  w...BMV....".vE.
+00006b70: defa c0e7 5432 8272 d266 c593 1ae5 d77c  ....T2.r.f.....|
+00006b80: 3b9e 1c95 b8af 1937 f551 719f 6eab ad7c  ;......7.Qq.n..|
+00006b90: 7544 f0fe e158 8e8a 5234 22d9 2cce 6864  uD...X..R4".,.hd
+00006ba0: 1b70 031f 7d61 ed3a 6437 9ead f363 f42d  .p..}a.:d7...c.-
+00006bb0: 17a6 7c1d 5b53 2f48 55ad 501d 2c7d 2d17  ..|.[S/HU.P.,}-.
+00006bc0: 1d51 7c3c d939 237b 86d4 442d 0380 08f2  .Q|<.9#{..D-....
+00006bd0: b3fb 661a 2431 7284 598d 5189 6fed 8cea  ..f.$1r.Y.Q.o...
+00006be0: 9cee 623d e8c2 675d 6c2f b3dc 24ee b2e0  ..b=..g]l/..$...
+00006bf0: 16f0 acdd 8dd8 7c40 746e be76 966f 1ef9  ......|@tn.v.o..
+00006c00: 1243 e1ca 817c 3595 abb1 f958 955a 6de3  .C...|5....X.Zm.
+00006c10: 1548 8542 1f46 6db2 c205 e2a0 12d3 7581  .H.B.Fm.......u.
+00006c20: 428c af9d 46a6 7685 9798 ef84 7161 c140  B...F.v.....qa.@
+00006c30: c702 012e a7b4 117d d7b9 3409 4011 de59  .......}..4.@..Y
+00006c40: 73bd 3037 78fe 5083 dd35 0d1e 1800 8f1f  s.07x.P..5......
+00006c50: 787b dde8 c75c 2f79 b0b2 c45a dae6 b748  x{...\/y...Z...H
+00006c60: 6d6f 6bab c5e9 2773 0703 bb6d 84cb 82d6  mok...'s...m....
+00006c70: cbd1 3706 6f9b 10f8 a354 60f9 25bb c41d  ..7.o....T`.%...
+00006c80: 40a8 c1fc 923d 426e e350 4ac5 e89f d4b9  @....=Bn.PJ.....
+00006c90: ae36 fd93 7a97 dad4 2fd9 b98e ee2c ea00  .6..z.../....,..
+00006ca0: cf58 ca6e dd0a c382 68e6 a83c 606a 0fd3  .X.n....h..<`j..
+00006cb0: d928 e54e 9eba 76ee 4ddd 6670 de33 8cf4  .(.N..v.M.fp.3..
+00006cc0: 73f2 85e4 f847 b752 caeb c4c3 54df 077c  s....G.R....T..|
+00006cd0: da1f ef35 e15c c456 2893 25c3 dea0 2e70  ...5.\.V(.%....p
+00006ce0: 3dbc adbe edeb 4235 aa6f a4f1 e992 407d  =.....B5.o....@}
+00006cf0: b5be 4e79 3bf6 e91c 987d a51f a8c4 a960  ..Ny;....}.....`
+00006d00: 18aa 7ba5 727b 5311 4cd7 6fc3 676a 7f05  ..{.r{S.L.o.gj..
+00006d10: 3bdd a39c 6aee 034a 0b51 8ff4 1713 0538  ;...j..J.Q.....8
+00006d20: 2fd4 87d4 33a7 6d9b 2e9b a35e 10ae ac70  /...3.m....^...p
+00006d30: 4011 99ca d609 cbca 04fc db33 532c 8b3f  @..........3S,.?
+00006d40: d883 27d0 1724 3c63 9a08 6e75 4795 f333  ..'..$<c..nuG..3
+00006d50: d5db 828f e890 20ea 628b 1494 2520 d984  ...... .b...% ..
+00006d60: 3ce4 6e76 a74a ac8a c740 bfa0 fe90 5732  <.nv.J...@....W2
+00006d70: 14ef c6c2 ac9b 32e3 2fdb e5ee 1cd8 160a  ......2./.......
+00006d80: b5fe f904 c3f4 3308 e61f 95c4 a09b cec2  ......3.........
+00006d90: edec bd66 2da4 6f64 4de3 8fa4 9b24 3439  ...f-.odM....$49
+00006da0: 1b88 ad0d 5e51 d880 4b89 0cc3 ac3f cd73  ....^Q..K....?.s
+00006db0: aa55 c179 6b2e 5740 9c57 ab12 4c13 948f  .U.yk.W@.W..L...
+00006dc0: d492 111b 5b84 97ea e1b8 f64e 775e 2f6c  ....[......Nw^/l
+00006dd0: d574 fa48 8fc5 9254 2349 6d0d 2a42 b5e3  .t.H...T#Im.*B..
+00006de0: 86d1 91b9 7176 4043 1174 f072 86d2 efdc  ....qv@C.t.r....
+00006df0: c180 19b8 f750 41c9 0d91 fd49 f330 a7e9  .....PA....I.0..
+00006e00: 3157 abf2 0c49 ed0b 53bb be58 2121 01fe  1W...I..S..X!!..
+00006e10: c03a 8846 2b7b afdb bf05 851d 3561 34d9  .:.F+{......5a4.
+00006e20: 60cb 309e 378b 81a6 1a75 4150 4907 5c3c  `.0.7....uAPI.\<
+00006e30: 7e29 c83b f942 72bd 8818 3dd9 f664 4e78  ~).;.Br...=..dNx
+00006e40: 9eeb 9575 f66e a47f fdf3 7f05 06a0 1791  ...u.n..........
+00006e50: 2193 81ec bd48 fffa e7ff d9e1 d0bd e454  !....H.........T
+00006e60: 083a d339 15a0 b05b 0f43 0c0c c1e3 c2d1  .:.9...[.C......
+00006e70: e8d3 797d 1407 27b3 5261 1de0 2519 7a66  ..y}..'.Ra..%.zf
+00006e80: fbfb fb60 a1d0 bd9d 377c f919 dd73 5197  ...`....7|...sQ.
+00006e90: 616b b8a3 ba60 21ff 47b6 e560 2073 fd95  ak...`!.G..` s..
+00006ea0: 4fa3 5b24 d789 1d8b b384 6b4c a90e 86ee  O.[$......kL....
+00006eb0: 5880 3d09 d5ee c058 5e5d 45d8 e703 7c5b  X.=....X^]E...|[
+00006ec0: aace e15a f3ab 5cff 89aa cced 2c26 dc56  ...Z..\.....,&.V
+00006ed0: ff4c 0135 9d58 1a6e a2b0 2406 da83 a865  .L.5.X.n..$....e
+00006ee0: 484e ef8e c30a d0b8 a8bd 5aea 1462 d14d  HN........Z..b.M
+00006ef0: 2dce 99d5 2833 5e5b 8af7 5152 9f61 fa8b  -...(3^[..QR.a..
+00006f00: 720f 5bfd eff3 58ec 8caa b3dd 7f64 66cb  r.[...X......df.
+00006f10: e0ac f513 b8c6 79a3 a340 6478 d60b a8c2  ......y..@dx....
+00006f20: fb8c ff9d 9a76 f573 d07b 76fe ac47 9df5  .....v.s.{v..G..
+00006f30: 74c1 98ef 78de 5257 71a9 3167 2c84 a5bc  t...x.RWq.1g,...
+00006f40: 0d45 7761 b838 ee67 1c3f e794 33df a087  .Ewa.8.g.?..3...
+00006f50: d41d 6074 ae69 e582 52f6 09ce f7dc 4a3a  ..`t.i..R.....J:
+00006f60: 9f7c 7ce6 f0ad 3eed 89ae cd9e 436a 06f5  .||...>.....Cj..
+00006f70: d0e3 a5d8 2d56 ab0e a42b fe2c 360e 9b3a  ....-V...+.,6..:
+00006f80: a21a dd1a df41 a389 402e 74dc bc9f 2033  .....A..@.t... 3
+00006f90: 0c43 4778 641a de32 2649 9ba8 0232 6a17  .CGxd..2&I...2j.
+00006fa0: 2434 4177 0969 17bb b0f3 7480 af0d b839  $4Aw.i....t....9
+00006fb0: 5f69 ea03 f4e9 5fc7 cea1 ea7c c38b c2ad  _i...._....|....
+00006fc0: 55e0 9f72 b139 50c1 6abd f12d d5b4 2086  U..r.9P.j..-.. .
+00006fd0: fcc3 1df2 9762 178c f2cb 55b6 f104 e91f  .....b....U.....
+00006fe0: 5bdd d058 4516 972e c3f9 acb7 39d8 b7cb  [..XE.......9...
+00006ff0: a883 7d2f 19df 9fc5 af21 2416 7db0 97b1  ..}/.....!$.}...
+00007000: 3412 29bc ece2 5f51 6e85 2fa4 d0cb 5591  4.)..._Qn./...U.
+00007010: c4a5 308a a068 b989 b07d 2984 e5c7 d375  ..0..h...})....u
+00007020: 1694 b079 8865 237a c5fc 8d9f 800b 1e18  ...y.e#z........
+00007030: 85cd a6fa 926f e78a 2386 29e5 9f6a 70e3  .....o..#.)..jp.
+00007040: d76d fcc3 5edf fdbf 0000 0000 ffff 0300  .m..^...........
+00007050: 504b 0304 1400 0600 0800 0000 2100 d6d1  PK..........!...
+00007060: 18e7 5501 0000 6b02 0000 1100 0801 646f  ..U...k.......do
+00007070: 6350 726f 7073 2f63 6f72 652e 786d 6c20  cProps/core.xml 
+00007080: a204 0128 a000 0100 0000 0000 0000 0000  ...(............
 00007090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000070a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000070b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000070c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000070d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000070e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000070f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007120: 0000 7c92 dd4b c330 14c5 df05 ff87 92f7  ..|..K.0........
-00007130: 3649 eba6 84ae 033f f6a4 203a 517c 0bc9  6I.....?.. :Q|..
-00007140: dd16 6cd2 9064 5fff bd69 b7d5 0ec5 c7dc  ..l..d_..i......
-00007150: 73ee 8f73 2e29 a73b 5d27 1b70 5e35 6682  s..s.).;]'.p^5f.
-00007160: 6846 5002 4634 5299 e504 bdcd 67e9 0d4a  hFP.F4R.....g..J
-00007170: 7ce0 46f2 ba31 3041 7bf0 685a 5d5e 94c2  |.F..10A{.hZ]^..
-00007180: 32d1 3878 768d 0517 14f8 2492 8c67 c24e  2.8xv.....$..g.N
-00007190: d02a 04cb 30f6 6205 9afb 2c3a 4c14 178d  .*..0.b...,:L...
-000071a0: d33c c4a7 5b62 cbc5 175f 02ce 0919 630d  .<..[b..._....c.
-000071b0: 814b 1e38 6e81 a9ed 89e8 8894 a247 dab5  .K.8n........G..
-000071c0: ab3b 8014 186a d060 82c7 34a3 f8c7 1bc0  .;...j.`..4.....
-000071d0: 69ff e742 a70c 9c5a 85bd 8d9d 8e71 876c  i..B...Z.....q.l
-000071e0: 290e 62ef de79 d51b b7db 6db6 2dba 1831  ).b..y....m.-..1
-000071f0: 3fc5 1f4f 8faf 5dd5 5499 f656 0250 554a  ?..O..].T..V.PUJ
-00007200: c184 031e 1a57 b5fd ed7e 5797 7830 6c0f  .....W...~W.x0l.
-00007210: 5873 1f9e e2ad 170a e4ed be7a d09a 9b75  Xs.........z...u
-00007220: ac95 bcf0 0d57 4dad 4afc db15 c95d 9103  .....WM.J....]..
-00007230: 1e64 12a3 b143 9193 f25e dcdd cf67 a8ca  .d...C...^...g..
-00007240: 494e 5352 a464 34a7 6346 c6ac b8fe 6c43  INSR.d4.cF....lC
-00007250: 9ced b751 0f03 7d8c f23f 314f 2949 c9d5  ...Q..}..?1O)I..
-00007260: 9ce6 8c8c 18cd 07c4 13a0 ea72 9f7f 8fea  ...........r....
-00007270: 1b00 00ff ff03 0050 4b03 0414 0006 0008  .......PK.......
-00007280: 0000 0021 00e8 b39b c699 0100 0000 2800  ...!..........(.
-00007290: 0027 0000 0078 6c2f 7072 696e 7465 7253  .'...xl/printerS
-000072a0: 6574 7469 6e67 732f 7072 696e 7465 7253  ettings/printerS
-000072b0: 6574 7469 6e67 7332 2e62 696e ec9a 314f  ettings2.bin..1O
-000072c0: c240 14c7 ffd7 5629 61c0 c59d c144 1c48  .@....V)a....D.H
-000072d0: d074 7223 4ae2 6820 266e c658 131b 8983  .tr#J.h &n.X....
-000072e0: d1c4 b1ee 0cce ec7e 18bf 8389 7e14 df15  .......~....~...
-000072f0: 2aad 9686 a65c 10f9 1f1c 47af f0ee f577  *....\....G....w
-00007300: f75e df3d 38c1 292e d045 1f3d 34d0 c43d  .^.=8.)..E.=4..=
-00007310: aee1 2388 da2b 3c44 470d ec63 0fd9 4539  ..#..+<DG..c..E9
-00007320: 70de b1b3 5bff 78b6 15aa 18d5 3cd7 8742  p...[.x.....<..B
-00007330: 05e7 9625 2d60 cb6b 07de 8cef 97e9 d6d2  ...%-`.k........
-00007340: ad1c 01fd eed1 b181 6127 22f5 e83f 4b56  ........a'"..?KV
-00007350: 9f39 0d28 7915 0854 394d 2430 83c0 9621  .9.(y..T9M$0...!
-00007360: 32f6 4a10 7f42 4bf4 ecc8 bd26 c025 0625  2.J..BK....&.%.%
-00007370: 751e fbde 300c 45ce 0b1d 316d 4e13 28b2  u...0.E...1mN.(.
-00007380: 0ece 7027 014f 2075 1085 3dcb 26d8 c621  ..p'.O u..=.&..!
-00007390: d235 4fa3 f84a 7d03 6aeb 20eb e0d7 e37f  .5O..J}.j. .....
-000073a0: d958 d910 951e 2737 169f 7355 0ac5 7afc  .X....'7..sU..z.
-000073b0: 51e5 cb4e 4449 9d3e 33e3 fd34 79a5 a646  Q..NDI.>3..4y..F
-000073c0: 3fef 9c28 5da2 61ad ef77 4bb6 fe8a 8c2f  ?..(].a..wK..../
-000073d0: 9163 bad1 c79e abb7 58a3 5a42 bf8d 4d27  .c......X.ZB..M'
-000073e0: ea56 d10c e893 6eeb edb6 90ef e3dd 8204  .V....n.........
-000073f0: 4880 0448 8004 4880 0448 8004 8a10 e0ee  H..H..H..H......
-00007400: 67ed d78b 89c4 038d 70ad 0868 2f32 4ee0  g.......p..h/2N.
-00007410: 2eec b2cb 6797 958b e170 c895 4802 3181  ....g....p..H.1.
-00007420: 4486 8950 4880 0448 c018 8149 5eda 20e1  D..PH..H...I^. .
-00007430: 57eb 733b 5917 3194 c223 6ee4 c7ab 76e2  W.s;Y.1..#n...v.
-00007440: 7f3f aaa9 2573 a340 6321 81bf 43e0 0b00  .?..%s.@c!..C...
-00007450: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
-00007460: 0021 0072 de72 2498 0100 0052 0300 0010  .!.r.r$....R....
-00007470: 0008 0164 6f63 5072 6f70 732f 6170 702e  ...docProps/app.
-00007480: 786d 6c20 a204 0128 a000 0100 0000 0000  xml ...(........
-00007490: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000074a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000074b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000074c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000074d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000074e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007120: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007150: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007160: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007170: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007180: 0000 0000 0000 007c 924b 4fc3 3010 84ef  .......|.KO.0...
+00007190: 48fc 87c8 f7c4 79d0 0256 924a 3c7a a212  H.....y..V.J<z..
+000071a0: 8220 1037 cbde b616 b163 d9ee 23ff 1e27  . .7.....c..#..'
+000071b0: 6943 2b10 47ef cc7e 9a59 399f ed65 1d6c  iC+.G..~.Y9..e.l
+000071c0: c158 d1a8 0225 518c 0250 ace1 42ad 0af4  .X...%Q..P..B...
+000071d0: 56cd c31b 1458 4715 a775 a3a0 402d 5834  V....XG..u..@-X4
+000071e0: 2b2f 2f72 a609 6b0c 3c9b 4683 7102 6ce0  +//r..k.<.F.q.l.
+000071f0: 49ca 12a6 0bb4 764e 138c 2d5b 83a4 36f2  I.....vN..-[..6.
+00007200: 0ee5 c565 6324 75fe 6956 5853 f645 5780  ...ec$u.iVXS.EW.
+00007210: d338 9e62 098e 72ea 28ee 80a1 1e89 e880  .8.b..r.(.......
+00007220: e46c 44ea 8da9 7b00 6718 6a90 a09c c549  .lD...{.g.j....I
+00007230: 94e0 1faf 0323 ed9f 0bbd 72e2 94c2 b5da  .....#....r.....
+00007240: 773a c43d 6573 3688 a37b 6fc5 68dc ed76  w:.=es6..{o.h..v
+00007250: d12e eb63 f8fc 09fe 583c bdf6 5543 a1ba  ...c....X<..UC..
+00007260: 5b31 4065 ce19 6106 a86b 4cd9 f5d7 edbe  [1@e..a..kL.....
+00007270: cef1 c9b0 3b60 4dad 5bf8 5b2f 05f0 bbb6  ....;`M.[.[/....
+00007280: 7c94 92aa 8daf 15bc d02d 154d 2d72 fcdb  |........-.M-r..
+00007290: e5c9 7d91 010f 3cf0 d1c8 50e4 a8bc 67f7  ..}...<...P...g.
+000072a0: 0fd5 1c95 699c 2661 9c85 f1a4 4aa6 249e  ....i.&a....J.$.
+000072b0: 92ec fab3 0b71 b6df 451d 06f2 10e5 7f62  .....q..E......b
+000072c0: 870b d349 15df 926c 42b2 ab13 e211 50f6  ...I...lB.....P.
+000072d0: b9cf bf47 f90d 0000 ffff 0300 504b 0304  ...G........PK..
+000072e0: 1400 0600 0800 0000 2100 1498 7b03 9901  ........!...{...
+000072f0: 0000 0028 0000 2700 0000 786c 2f70 7269  ...(..'...xl/pri
+00007300: 6e74 6572 5365 7474 696e 6773 2f70 7269  nterSettings/pri
+00007310: 6e74 6572 5365 7474 696e 6773 322e 6269  nterSettings2.bi
+00007320: 6eec 9abf 4bc3 4014 c7bf 9744 9bd0 a12e  n...K.@....D....
+00007330: ee1d 04eb 5028 2593 5bd1 82a3 5804 3711  ....P(%.[...X.7.
+00007340: 2358 280e a2e0 18f7 0e82 5b57 f1bf 12f4  #X(.......[W....
+00007350: 4ff1 ddf5 57aa 6968 488f 5afb bdf6 7acd  O...W.ihH.Z...z.
+00007360: a57d f7f2 b97b 2fef 5e7b 8253 5ca2 8d0e  .}...{/.^{.S\...
+00007370: ce50 450d f7b8 4184 ae69 aff1 608e aa68  .PE...A..i..`..h
+00007380: e200 e945 79f0 3eb0 b75f f97c 7615 020c  ...Ey.>.._.|v...
+00007390: caa1 1f41 a184 0bc7 9116 70e5 b585 70ce  ...A......p...p.
+000073a0: f78b 746b e94e 8680 4efb e8d8 c2b0 2391  ..tk.N..N.....#.
+000073b0: 7af4 9f25 adcf 9e06 94bc 0e04 024e 1309  z..%.........N..
+000073c0: cc21 b063 898c bb16 c49f 5017 3d5b 72af  .!.c......P.=[r.
+000073d0: e9e2 0abd 823a 0f7d 6f1c c722 e785 8e98  .....:.}o.."....
+000073e0: 36a7 09e4 5907 e7b8 9380 a72b b567 c29e  6...Y......+.g..
+000073f0: 5513 6ce0 10b3 354b a3f1 9546 16d4 d641  U.l...5K...F...A
+00007400: 56f3 d7e3 7fd9 58d1 1095 1e27 3316 5f70  V.....X....'3._p
+00007410: 550a c5ca f8a3 2a92 9d88 923a 7da6 c6fb  U.....*....:}...
+00007420: b3e4 959a 1afd a273 a274 31c3 3a93 772b  .......s.t1.:.w+
+00007430: b6fe 928c 2f91 e36c a38f 435f 6fb1 06e5  ..../..l..C_o...
+00007440: 847e 5bdb 9ee9 5666 06f4 c9a0 fef6 9acb  .~[...Vf........
+00007450: f7f1 6e41 0224 4002 2440 0224 4002 2440  ..nA.$@.$@.$@.$@
+00007460: 0279 0870 f7b3 f1eb c546 e281 46b8 5104  .y.p.....F..F.Q.
+00007470: b417 1926 7097 76d9 c5b3 cbca 47bf dfe7  ...&p.v.....G...
+00007480: 4a24 8131 8144 8689 5048 8004 48c0 1a81  J$.1.D..PH..H...
+00007490: 515e da22 e177 e76b 3759 9731 94c2 236e  Q^.".w.k7Y.1..#n
+000074a0: e5c7 ab46 e27f 3faa a625 73a3 4063 2181  ...F..?..%s.@c!.
+000074b0: bf43 e01b 0000 ffff 0300 504b 0304 1400  .C........PK....
+000074c0: 0600 0800 0000 2100 72de 7224 9801 0000  ......!.r.r$....
+000074d0: 5203 0000 1000 0801 646f 6350 726f 7073  R.......docProps
+000074e0: 2f61 7070 2e78 6d6c 20a2 0401 28a0 0001  /app.xml ...(...
 000074f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007500: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007510: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007520: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007530: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007540: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007550: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007560: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007570: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007580: 0000 0000 0000 0000 0000 009c 9351 6bdb  .............Qk.
-00007590: 3010 c7df 07fb 0e46 ef8d dc2e 9411 6495  0......F......d.
-000075a0: d16e 74b0 d140 d2ec 5995 cfb1 a822 09e9  .nt..@..Y...."..
-000075b0: 6292 7dfa 9d6c eada edf6 b2b7 bbfb 9ffe  b.}..l..........
-000075c0: fc74 2789 9bd3 c116 1dc4 64bc abd8 e5a2  .t'.......d.....
-000075d0: 6405 38ed 6be3 f615 7bdc 7ebb f8cc 8a84  d.8.k...{.~.....
-000075e0: cad5 ca7a 0715 3b43 6237 f2e3 07b1 8e3e  ...z..;Cb7.....>
-000075f0: 4044 03a9 200b 972a d622 8615 e749 b770  @D.. ..*."...I.p
-00007600: 5069 41b2 23a5 f1f1 a090 d2b8 e7be 698c  PiA.#.........i.
-00007610: 863b af8f 0770 c8af caf2 9ac3 09c1 d550  .;...p.........P
-00007620: 5f84 d190 0d8e ab0e ffd7 b4f6 3af3 a5dd  _...........:...
-00007630: f61c 0858 8a2f 2158 a315 d22d e54f a3a3  ...X./!X...-.O..
-00007640: 4fbe c1e2 eb49 8315 7c2a 0aa2 db80 3e46  O....I..|*....>F
-00007650: 8367 590a 3e4d c546 2b0b b764 2c1b 6513  .gY.>M.F+..d,.e.
-00007660: 08fe 5a10 f7a0 f2d0 d6ca c424 4587 ab0e  ..Z........$E...
-00007670: 34fa 5824 f39b c676 c58a 2795 20e3 54ac  4.X$...v..'. .T.
-00007680: 53d1 2887 8495 db86 a48f 6d48 18e5 2f1f  S.(.......mH../.
-00007690: 9f53 0b80 4970 6a18 8a7d 38ed 9dc6 6629  .S..Ipj..}8...f)
-000076a0: 977d 0305 f3c6 6c30 8090 3047 dc1a b490  .}....l0..0G....
-000076b0: 1e9a b58a f817 e2e5 94b8 6718 7807 9cef  ..........g.x...
-000076c0: 2e1c e77c 23e9 43c8 539e b18f dada fa7f  ...|#.C.S.......
-000076d0: 9cda e531 3c11 d0bb 3bf7 6324 fa37 bc3f  ...1<...;.c$.7.?
-000076e0: 8c7b 4e8f 61eb ef14 c2cb 3ee6 45b1 6955  .{N.a.....>.E.iU
-000076f0: 849a 5638 ee6b 2c88 7b5a 45b4 d9e4 b655  ..V8.k,.{ZE....U
-00007700: 6e0f f54b cf7b 21bf 9edd f045 e4e5 f5a2  n..K.{!....E....
-00007710: fc54 d2c3 98d4 047f fd0c f20f 0000 00ff  .T..............
-00007720: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
-00007730: 00e6 737a 775e 0400 00f0 1100 0027 0000  ..szw^.......'..
-00007740: 0078 6c2f 7072 696e 7465 7253 6574 7469  .xl/printerSetti
-00007750: 6e67 732f 7072 696e 7465 7253 6574 7469  ngs/printerSetti
-00007760: 6e67 7331 2e62 696e ec57 6d4f 5c45 143e  ngs1.bin.WmO\E.>
-00007770: e799 d9b9 7717 9665 d92d 5d5a 5e96 ad85  ....w..e.-]Z^...
-00007780: 1685 420b 1595 b6bb 2eb4 6091 625b 1593  ..B.......`.b[..
-00007790: c684 78d1 3431 60b4 fd66 e2a6 8989 d12f  ..x.41`..f...../
-000077a0: c68f fd15 fe06 3ff9 234c fc1b 26c6 e033  ......?.#L..&..3
-000077b0: f7ee b2d4 d715 37a4 9ace 64ee bc9f f3cc  ......7...d.....
-000077c0: 7999 39f7 9edc 93ba acc8 6dd9 904d 7ed7  y.9.......m..M~.
-000077d0: 58df e548 8df5 2d96 9983 59df 5ae5 ea4b  X..H..-...Y.Z..K
-000077e0: 322b d3b2 2017 c527 b519 fc20 c5bc f951  2+.. ..'... ...Q
-000077f0: 4525 2d8f 7be6 c388 ad40 b600 0157 58f6  E%-.{....@...WX.
-00007800: 6a32 1faf eeee 4749 ce73 68d5 bfa5 5edf  j2....GI.sh...^.
-00007810: dedd dbe5 e017 c5e6 0c17 fab5 2927 f28b  ............)'..
-00007820: 2d84 82b4 fdb2 5097 6dd9 953d 96b2 dc90  -.....P.m..=....
-00007830: 1dd6 3bf2 b1dc 97f7 d8df 940f e5a1 7c12  ..;...........|.
-00007840: b7ea b22e 97ff f000 1ec3 7e20 f295 f994  ..........~ ....
-00007850: 4d8d d440 8db1 48c1 45aa 6ce7 6c3f 7906  M..@..H.E.l.l?y.
-00007860: 873b a149 6b46 7bd0 8b2c fa90 3392 f1b3  .;.IkF{..,..3...
-00007870: 3088 b721 4088 b427 e447 d44f 8274 d46a  0..!@..'.G.O.t.j
-00007880: 2a43 9a01 0213 7061 5826 e79e df6d 9462  *C....paX&...m.b
-00007890: a459 8422 86c5 b2a4 caae 1c94 251b 136c  .Y."........%..l
-000078a0: 3250 e96b d147 4a9d 6d04 b61a daaa e4fc  2P.k.GJ.m.......
-000078b0: 6858 3661 d93e c188 8cfb 020d 8df4 27db  hX6a.>........'.
-000078c0: 3c16 75ca a170 200d c913 850c 441a 9661  <.u..p .....D..a
-000078d0: a4e0 e1da 8a09 2bb2 1351 1e6d 4670 e00e  ......+..Q.mFp..
-000078e0: a491 01cf 6eb2 daa7 39d3 8fbc 0e68 418b  ....n...9....hA.
-000078f0: 3881 419c 44c9 0ce1 144e 6318 2318 c518  8.A.D....Nc.#...
-00007900: ca18 4705 67f0 1cce 6202 9338 87f3 98c2  ..G.g...b..8....
-00007910: f3fa 824e eb8c 5ed0 599d d38b 7a49 e775  ...N..^.Y...zI.u
-00007920: 412f eb8b 58d4 97f0 325e c112 aee0 2aae  A/..X...2^....*.
-00007930: a18a 9abe 8aba 2e87 8d15 5cc7 0dac 628d  ..........\...b.
-00007940: b6e9 51b9 58e0 b642 585e e236 6309 cb56  ..Q.X..BX^.6c..V
-00007950: b3a6 cfe4 b45f f366 0005 14b5 890b 312e  ....._.f......1.
-00007960: 3b6c 47ec a81d 73c4 a515 3da3 4d5c 7a4e  ;lG...s...=.M\zN
-00007970: cfeb 9412 17a6 a399 e842 348b 2770 e922  .........B4.'p."
-00007980: 625c 6649 afe8 55bd a655 6de2 c28a 6bc1  b\fI..U..Um...k.
-00007990: 7acd dec4 3a5e c706 6e61 136f e076 58b9  z...:^..na.o.vX.
-000079a0: 83bb 7813 6fe1 6d6c e11d 8849 ecab 2d7f  ..x.o.ml...I..-.
-000079b0: 8d2d 497b 3596 a647 9d48 d39d 7083 eea4  .-I{5..G.H..p...
-000079c0: 2b05 43c1 293d adc3 3aa2 a33a 66a2 03d8  +.C.)=..:..:f...
-000079d0: 5a3c abc5 092d 4e6a 51a8 ec70 1c61 5e52  Z<...-NjQ..p.a^R
-000079e0: 4df5 7ad5 0a6d 0d34 c1b0 df86 fd89 fd1a  M.z..m.4........
-000079f0: 1ab6 4999 585e 2a61 62d2 caa1 70dc b9c0  ..I.X^*ab...p...
-00007a00: 852e ed32 aec7 f5ba acf3 664d d562 c015  ...2......fM.b..
-00007a10: 8cd0 9849 294b 7187 4389 ad3b 4337 a412  ...I)Kq.C..;C7..
-00007a20: 5aee 6268 4e5e 0b1a 1b07 8fe3 27c9 3ce1  Z.bhN^......'.<.
-00007a30: 4e5f f2b6 7670 d6d1 ac8e 26a2 e082 9a87  N_..vp....&.....
-00007a40: ef1d ed90 50bc a7de 5c94 32af a5aa 653b  ....P...\.2...e;
-00007a50: cd3c 4f5f 78dc 23b2 c4fe 14cb 4f74 da8f  .<O_x.#.....Ot..
-00007a60: d89f fbfc af67 6bef 3ee2 75f6 ad85 944a  .....gk.>.u....J
-00007a70: fe02 89e2 6b80 543d e11c bbb4 7d9f 7d22  ....k.T=....}.}"
-00007a80: b938 7ded bbb5 f826 d9e6 2d72 b444 7c94  .8}....&..-r.D|.
-00007a90: 112f d28e d267 221b 7bbb 3b32 b730 b356  ./...g".{.;2.0.V
-00007aa0: af77 ceb1 bbfb a094 46a7 908f 2897 ae6e  .w......F...(..n
-00007ab0: f38a 4ab3 ecef 3f0d 689e 0a0c df10 453d  ..J...?.h.....E=
-00007ac0: 7eff af33 2258 667c e0a3 8235 daf3 7ac7  ~..3"Xf|...5..z.
-00007ad0: f8fe edfe d526 a7ae 3852 a3d1 3800 fe1d  .....&..8R..8...
-00007ae0: edb3 9902 c629 01bd 38f6 b34e 4eb6 cce0  .....)..8..NN...
-00007af0: e07d 060c 0fe9 d20f 1816 dc61 ff01 f37d  .}.........a...}
-00007b00: 860d 1f30 50f8 bb74 c0f9 78d4 cc4b b454  ...0P..t..x..K.T
-00007b10: da82 f432 2cc1 a3f8 b031 e39f f77d 16f9  ...2,....1...}..
-00007b20: 3eb9 5952 b100 d84e 3341 93eb edcf 10d2  >.YR...N3A......
-00007b30: bda3 48cc 335f a104 12f1 35e2 aa03 d576  ..H.3_....5....v
-00007b40: 57fb 01d9 2714 5bf1 add7 493c 924f aad6  W...'.[...I<.O..
-00007b50: 9bf4 cf74 e51f b5c3 a9e8 9fb7 d659 bba7  ...t.........Y..
-00007b60: 76d2 6cbd 6bbe 3e5c 0aec 7b14 2db6 edf7  v.l.k.>\..{.-...
-00007b70: 8f4f 95f8 929c f498 bda9 7b67 ff1f 534a  .O........{g..SJ
-00007b80: 79b5 f9ff 3fff df67 a8d6 76cc 96d5 9c8f  y...?..g..v.....
-00007b90: 96f5 ac4e e864 335a 1e94 cef2 7f51 621d  ...N.d3Z.....Qb.
-00007ba0: 866d 9d1d 2df9 993e 7e31 347d acfd 661e  .m..-..>~14}..f.
-00007bb0: 1182 ca3e 733b 2963 f167 e9d8 25f0 2b00  ...>s;)c.g..%.+.
-00007bc0: 0000 ffff 0300 504b 0102 2d00 1400 0600  ......PK..-.....
-00007bd0: 0800 0000 2100 6c04 da6e 7e01 0000 9c06  ....!.l..n~.....
-00007be0: 0000 1300 0000 0000 0000 0000 0000 0000  ................
-00007bf0: 0000 0000 5b43 6f6e 7465 6e74 5f54 7970  ....[Content_Typ
-00007c00: 6573 5d2e 786d 6c50 4b01 022d 0014 0006  es].xmlPK..-....
-00007c10: 0008 0000 0021 00b5 5530 23f4 0000 004c  .....!..U0#....L
-00007c20: 0200 000b 0000 0000 0000 0000 0000 0000  ................
-00007c30: 00b7 0300 005f 7265 6c73 2f2e 7265 6c73  ....._rels/.rels
-00007c40: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
-00007c50: 815b b8c9 0b01 0000 6104 0000 1a00 0000  .[......a.......
-00007c60: 0000 0000 0000 0000 0000 dc06 0000 786c  ..............xl
-00007c70: 2f5f 7265 6c73 2f77 6f72 6b62 6f6f 6b2e  /_rels/workbook.
-00007c80: 786d 6c2e 7265 6c73 504b 0102 2d00 1400  xml.relsPK..-...
-00007c90: 0600 0800 0000 2100 02b9 e3e1 1302 0000  ......!.........
-00007ca0: 6504 0000 0f00 0000 0000 0000 0000 0000  e...............
-00007cb0: 0000 2709 0000 786c 2f77 6f72 6b62 6f6f  ..'...xl/workboo
-00007cc0: 6b2e 786d 6c50 4b01 022d 0014 0006 0008  k.xmlPK..-......
-00007cd0: 0000 0021 0026 7b5a 8391 0300 003e 0d00  ...!.&{Z.....>..
-00007ce0: 0018 0000 0000 0000 0000 0000 0000 0067  ...............g
-00007cf0: 0b00 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
-00007d00: 2f73 6865 6574 342e 786d 6c50 4b01 022d  /sheet4.xmlPK..-
-00007d10: 0014 0006 0008 0000 0021 0013 c42c 13c2  .........!...,..
-00007d20: 0000 0042 0100 0023 0000 0000 0000 0000  ...B...#........
-00007d30: 0000 0000 002e 0f00 0078 6c2f 776f 726b  .........xl/work
-00007d40: 7368 6565 7473 2f5f 7265 6c73 2f73 6865  sheets/_rels/she
-00007d50: 6574 322e 786d 6c2e 7265 6c73 504b 0102  et2.xml.relsPK..
-00007d60: 2d00 1400 0600 0800 0000 2100 3b6d 324b  -.........!.;m2K
-00007d70: c100 0000 4201 0000 2300 0000 0000 0000  ....B...#.......
-00007d80: 0000 0000 0000 3110 0000 786c 2f77 6f72  ......1...xl/wor
-00007d90: 6b73 6865 6574 732f 5f72 656c 732f 7368  ksheets/_rels/sh
-00007da0: 6565 7431 2e78 6d6c 2e72 656c 7350 4b01  eet1.xml.relsPK.
-00007db0: 022d 0014 0006 0008 0000 0021 000b b47d  .-.........!...}
-00007dc0: 7d3f 0600 0075 2000 0018 0000 0000 0000  }?...u .........
-00007dd0: 0000 0000 0000 0033 1100 0078 6c2f 776f  .......3...xl/wo
-00007de0: 726b 7368 6565 7473 2f73 6865 6574 322e  rksheets/sheet2.
-00007df0: 786d 6c50 4b01 022d 0014 0006 0008 0000  xmlPK..-........
-00007e00: 0021 0081 129d 2b94 0200 00f3 0800 0018  .!....+.........
-00007e10: 0000 0000 0000 0000 0000 0000 00a8 1700  ................
-00007e20: 0078 6c2f 776f 726b 7368 6565 7473 2f73  .xl/worksheets/s
-00007e30: 6865 6574 332e 786d 6c50 4b01 022d 0014  heet3.xmlPK..-..
-00007e40: 0006 0008 0000 0021 00f2 4da6 d156 2b00  .......!..M..V+.
-00007e50: 0018 2f01 0018 0000 0000 0000 0000 0000  ../.............
-00007e60: 0000 0072 1a00 0078 6c2f 776f 726b 7368  ...r...xl/worksh
-00007e70: 6565 7473 2f73 6865 6574 312e 786d 6c50  eets/sheet1.xmlP
-00007e80: 4b01 022d 0014 0006 0008 0000 0021 00e9  K..-.........!..
-00007e90: a625 b866 0600 0053 1b00 0013 0000 0000  .%.f...S........
-00007ea0: 0000 0000 0000 0000 00fe 4500 0078 6c2f  ..........E..xl/
-00007eb0: 7468 656d 652f 7468 656d 6531 2e78 6d6c  theme/theme1.xml
-00007ec0: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
-00007ed0: 37b1 98f1 1403 0000 900a 0000 0d00 0000  7...............
-00007ee0: 0000 0000 0000 0000 0000 954c 0000 786c  ...........L..xl
-00007ef0: 2f73 7479 6c65 732e 786d 6c50 4b01 022d  /styles.xmlPK..-
-00007f00: 0014 0006 0008 0000 0021 001b 2716 c6e5  .........!..'...
-00007f10: 1f00 00f9 6a00 0014 0000 0000 0000 0000  ....j...........
-00007f20: 0000 0000 00d4 4f00 0078 6c2f 7368 6172  ......O..xl/shar
-00007f30: 6564 5374 7269 6e67 732e 786d 6c50 4b01  edStrings.xmlPK.
-00007f40: 022d 0014 0006 0008 0000 0021 00f1 5ae5  .-.........!..Z.
-00007f50: ae55 0100 006b 0200 0011 0000 0000 0000  .U...k..........
-00007f60: 0000 0000 0000 00eb 6f00 0064 6f63 5072  ........o..docPr
-00007f70: 6f70 732f 636f 7265 2e78 6d6c 504b 0102  ops/core.xmlPK..
-00007f80: 2d00 1400 0600 0800 0000 2100 e8b3 9bc6  -.........!.....
-00007f90: 9901 0000 0028 0000 2700 0000 0000 0000  .....(..'.......
-00007fa0: 0000 0000 0000 7772 0000 786c 2f70 7269  ......wr..xl/pri
-00007fb0: 6e74 6572 5365 7474 696e 6773 2f70 7269  nterSettings/pri
-00007fc0: 6e74 6572 5365 7474 696e 6773 322e 6269  nterSettings2.bi
-00007fd0: 6e50 4b01 022d 0014 0006 0008 0000 0021  nPK..-.........!
-00007fe0: 0072 de72 2498 0100 0052 0300 0010 0000  .r.r$....R......
-00007ff0: 0000 0000 0000 0000 0000 0055 7400 0064  ...........Ut..d
-00008000: 6f63 5072 6f70 732f 6170 702e 786d 6c50  ocProps/app.xmlP
-00008010: 4b01 022d 0014 0006 0008 0000 0021 00e6  K..-.........!..
-00008020: 737a 775e 0400 00f0 1100 0027 0000 0000  szw^.......'....
-00008030: 0000 0000 0000 0000 0023 7700 0078 6c2f  .........#w..xl/
-00008040: 7072 696e 7465 7253 6574 7469 6e67 732f  printerSettings/
-00008050: 7072 696e 7465 7253 6574 7469 6e67 7331  printerSettings1
-00008060: 2e62 696e 504b 0506 0000 0000 1100 1100  .binPK..........
-00008070: 9e04 0000 c67b 0000 0000                 .....{....
+00007580: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007590: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000075a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000075b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000075c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000075d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000075e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000075f0: 9c93 516b db30 10c7 df07 fb0e 46ef 8ddc  ..Qk.0......F...
+00007600: 2e94 1164 95d1 6e74 b0d1 40d2 ec59 95cf  ...d..nt..@..Y..
+00007610: b1a8 2209 e962 927d fa9d 6cea daed f6b2  .."..b.}..l.....
+00007620: b7bb fb9f fefc 7427 899b d3c1 161d c464  ......t'.......d
+00007630: bcab d8e5 a264 0538 ed6b e3f6 157b dc7e  .....d.8.k...{.~
+00007640: bbf8 cc8a 84ca d5ca 7a07 153b 4362 37f2  ........z..;Cb7.
+00007650: e307 b18e 3e40 4403 a920 0b97 2ad6 2286  ....>@D.. ..*.".
+00007660: 15e7 49b7 7050 6941 b223 a5f1 f1a0 90d2  ..I.pPiA.#......
+00007670: b8e7 be69 8c86 3baf 8f07 70c8 afca f29a  ...i..;...p.....
+00007680: c309 c1d5 505f 84d1 900d 8eab 0eff d7b4  ....P_..........
+00007690: f63a f3a5 ddf6 1c08 588a 2f21 58a3 15d2  .:......X./!X...
+000076a0: 2de5 4fa3 a34f bec1 e2eb 4983 157c 2a0a  -.O..O....I..|*.
+000076b0: a2db 803e 4683 6759 0a3e 4dc5 462b 0bb7  ...>F.gY.>M.F+..
+000076c0: 642c 1b65 1308 fe5a 10f7 a0f2 d0d6 cac4  d,.e...Z........
+000076d0: 2445 87ab 0e34 fa58 24f3 9bc6 76c5 8a27  $E...4.X$...v..'
+000076e0: 9520 e354 ac53 d128 8784 95db 86a4 8f6d  . .T.S.(.......m
+000076f0: 4818 e52f 1f9f 530b 8049 706a 188a 7d38  H../..S..Ipj..}8
+00007700: ed9d c666 2997 7d03 05f3 c66c 3080 9030  ...f).}....l0..0
+00007710: 47dc 1ab4 901e 9ab5 8af8 17e2 e594 b867  G..............g
+00007720: 1878 079c ef2e 1ce7 7c23 e943 c853 9eb1  .x......|#.C.S..
+00007730: 8fda dafa 7f9c dae5 313c 11d0 bb3b f763  ........1<...;.c
+00007740: 24fa 37bc 3f8c 7b4e 8f61 ebef 14c2 cb3e  $.7.?.{N.a.....>
+00007750: e645 b169 5584 9a56 38ee 6b2c 887b 5a45  .E.iU..V8.k,.{ZE
+00007760: b4d9 e4b6 556e 0ff5 4bcf 7b21 bf9e ddf0  ....Un..K.{!....
+00007770: 45e4 e5f5 a2fc 54d2 c398 d404 7ffd 0cf2  E.....T.........
+00007780: 0f00 0000 ffff 0300 504b 0304 1400 0600  ........PK......
+00007790: 0800 0000 2100 e673 7a77 5e04 0000 f011  ....!..szw^.....
+000077a0: 0000 2700 0000 786c 2f70 7269 6e74 6572  ..'...xl/printer
+000077b0: 5365 7474 696e 6773 2f70 7269 6e74 6572  Settings/printer
+000077c0: 5365 7474 696e 6773 312e 6269 6eec 576d  Settings1.bin.Wm
+000077d0: 4f5c 4514 3ee7 99d9 b977 1796 65d9 2d5d  O\E.>....w..e.-]
+000077e0: 5a5e 96ad 8516 8542 0b15 95b6 bb2e b460  Z^.....B.......`
+000077f0: 9162 5b15 93c6 8478 d134 3160 b4fd 66e2  .b[....x.41`..f.
+00007800: a689 89d1 2fc6 8ffd 15fe 063f f923 4cfc  ..../......?.#L.
+00007810: 1b26 c6e0 33f7 eeb2 d4d7 1537 a49a ce64  .&..3......7...d
+00007820: eebc 9ff3 cc79 9939 f79e dc93 baac c86d  .....y.9.......m
+00007830: d990 4d7e d758 dfe5 488d f52d 9699 8359  ..M~.X..H..-...Y
+00007840: df5a e5ea 4b32 2bd3 b220 17c5 27b5 19fc  .Z..K2+.. ..'...
+00007850: 20c5 bcf9 5145 252d 8f7b e6c3 88ad 40b6   ...QE%-.{....@.
+00007860: 0001 5758 f66a 321f afee ee47 49ce 7368  ..WX.j2....GI.sh
+00007870: d5bf a55e dfde dddb e5e0 17c5 e60c 17fa  ...^............
+00007880: b529 27f2 8b2d 8482 b4fd b250 976d d995  .)'..-.....P.m..
+00007890: 3d96 b2dc 901d d63b f2b1 dc97 f7d8 df94  =......;........
+000078a0: 0fe5 a17c 12b7 eab2 2e97 fff0 001e c37e  ...|...........~
+000078b0: 20f2 95f9 944d 8dd4 408d b148 c145 aa6c   ....M..@..H.E.l
+000078c0: e76c 3f79 0687 3ba1 496b 467b d08b 2cfa  .l?y..;.IkF{..,.
+000078d0: 9033 92f1 b330 88b7 2140 88b4 27e4 47d4  .3...0..!@..'.G.
+000078e0: 4f82 74d4 6a2a 439a 0102 1370 6158 26e7  O.t.j*C....paX&.
+000078f0: 9edf 6d94 62a4 5984 2286 c5b2 a4ca ae1c  ..m.b.Y.".......
+00007900: 9425 1b13 6c32 50e9 6bd1 474a 9d6d 04b6  .%..l2P.k.GJ.m..
+00007910: 1ada aae4 fc68 5836 61d9 3ec1 888c fb02  .....hX6a.>.....
+00007920: 0d8d f427 db3c 1675 caa1 7020 0dc9 1385  ...'.<.u..p ....
+00007930: 0c44 1a96 61a4 e0e1 da8a 092b b213 511e  .D..a......+..Q.
+00007940: 6d46 70e0 0ea4 9101 cf6e b2da a739 d38f  mFp......n...9..
+00007950: bc0e 6841 8b38 8141 9c44 c90c e114 4e63  ..hA.8.A.D....Nc
+00007960: 1823 18c5 18ca 1847 0567 f01c ce62 0293  .#.....G.g...b..
+00007970: 3887 f398 c2f3 fa82 4eeb 8c5e d059 9dd3  8.......N..^.Y..
+00007980: 8b7a 49e7 7541 2feb 8b58 d497 f032 5ec1  .zI.uA/..X...2^.
+00007990: 12ae e02a aea1 8a9a be8a ba2e 878d 155c  ...*...........\
+000079a0: c70d ac62 8db6 e951 b958 e0b6 4258 5ee2  ...b...Q.X..BX^.
+000079b0: 3663 09cb 56b3 a6cf e4b4 5ff3 6600 0514  6c..V....._.f...
+000079c0: b589 0b31 2e3b 6c47 eca8 1d73 c4a5 153d  ...1.;lG...s...=
+000079d0: a34d 5c7a 4ecf eb94 1217 a6a3 99e8 4234  .M\zN.........B4
+000079e0: 8b27 70e9 2262 5c66 49af e855 bda6 556d  .'p."b\fI..U..Um
+000079f0: e2c2 8a6b c17a cdde c43a 5ec7 066e 6113  ...k.z...:^..na.
+00007a00: 6fe0 7658 b983 bb78 136f e16d 6ce1 1d88  o.vX...x.o.ml...
+00007a10: 49ec ab2d 7f8d 2d49 7b35 96a6 479d 48d3  I..-..-I{5..G.H.
+00007a20: 9d70 83ee a42b 0543 c129 3dad c33a a2a3  .p...+.C.)=..:..
+00007a30: 3a66 a203 d85a 3cab c509 2d4e 6a51 a8ec  :f...Z<...-NjQ..
+00007a40: 701c 615e 524d f57a d50a 6d0d 34c1 b0df  p.a^RM.z..m.4...
+00007a50: 86fd 89fd 1a1a b649 9958 5e2a 6162 d2ca  .......I.X^*ab..
+00007a60: a170 dcb9 c085 2eed 32ae c7f5 baac f366  .p......2......f
+00007a70: 4dd5 62c0 158c d098 4929 4b71 8743 89ad  M.b.....I)Kq.C..
+00007a80: 3b43 37a4 125a ee62 684e 5e0b 1a1b 078f  ;C7..Z.bhN^.....
+00007a90: e327 c93c e14e 5ff2 b676 70d6 d1ac 8e26  .'.<.N_..vp....&
+00007aa0: a2e0 829a 87ef 1ded 9050 bca7 de5c 9432  .........P...\.2
+00007ab0: afa5 aa65 3bcd 3c4f 5f78 dc23 b2c4 fe14  ...e;.<O_x.#....
+00007ac0: cb4f 74da 8fd8 9ffb fcaf 676b ef3e e275  .Ot.......gk.>.u
+00007ad0: f6ad 8594 4afe 0289 e26b 8054 3de1 1cbb  ....J....k.T=...
+00007ae0: b47d 9f7d 22b9 387d edbb b5f8 26d9 e62d  .}.}".8}....&..-
+00007af0: 72b4 447c 9411 2fd2 8ed2 6722 1b7b bb3b  r.D|../...g".{.;
+00007b00: 32b7 30b3 56af 77ce b1bb fba0 9446 a790  2.0.V.w......F..
+00007b10: 8f28 97ae 6ef3 8a4a b3ec ef3f 0d68 9e0a  .(..n..J...?.h..
+00007b20: 0cdf 1045 3d7e ffaf 3322 5866 7ce0 a382  ...E=~..3"Xf|...
+00007b30: 35da f37a c7f8 feed fed5 26a7 ae38 52a3  5..z......&..8R.
+00007b40: d138 00fe 1ded b399 02c6 2901 bd38 f6b3  .8........)..8..
+00007b50: 4e4e b6cc e0e0 7d06 0c0f e9d2 0f18 16dc  NN....}.........
+00007b60: 61ff 01f3 7d86 0d1f 3050 f8bb 74c0 f978  a...}...0P..t..x
+00007b70: d4cc 4bb4 54da 82f4 322c c1a3 f8b0 31e3  ..K.T...2,....1.
+00007b80: 9ff7 7d16 f93e b959 52b1 00d8 4e33 4193  ..}..>.YR...N3A.
+00007b90: ebed cf10 d2bd a348 cc33 5fa1 0412 f135  .......H.3_....5
+00007ba0: e2aa 03d5 7657 fb01 d927 145b f1ad d749  ....vW...'.[...I
+00007bb0: 3c92 4faa d69b f4cf 74e5 1fb5 c3a9 e89f  <.O.....t.......
+00007bc0: b7d6 59bb a776 d26c bd6b be3e 5c0a ec7b  ..Y..v.l.k.>\..{
+00007bd0: 142d b6ed f78f 4f95 f892 9cf4 98bd a97b  .-....O........{
+00007be0: 67ff 1f53 4a79 b5f9 ff3f ffdf 67a8 d676  g..SJy...?..g..v
+00007bf0: cc96 d59c 8f96 f5ac 4ee8 6433 5a1e 94ce  ........N.d3Z...
+00007c00: f27f 5162 1d86 6d9d 1d2d f999 3e7e 3134  ..Qb..m..-..>~14
+00007c10: 7dac fd66 1e11 82ca 3e73 3b29 63f1 67e9  }..f....>s;)c.g.
+00007c20: d825 f02b 0000 00ff ff03 0050 4b01 022d  .%.+.......PK..-
+00007c30: 0014 0006 0008 0000 0021 006c 04da 6e7e  .........!.l..n~
+00007c40: 0100 009c 0600 0013 0000 0000 0000 0000  ................
+00007c50: 0000 0000 0000 0000 005b 436f 6e74 656e  .........[Conten
+00007c60: 745f 5479 7065 735d 2e78 6d6c 504b 0102  t_Types].xmlPK..
+00007c70: 2d00 1400 0600 0800 0000 2100 b555 3023  -.........!..U0#
+00007c80: f400 0000 4c02 0000 0b00 0000 0000 0000  ....L...........
+00007c90: 0000 0000 0000 b703 0000 5f72 656c 732f  .........._rels/
+00007ca0: 2e72 656c 7350 4b01 022d 0014 0006 0008  .relsPK..-......
+00007cb0: 0000 0021 0081 5bb8 c90b 0100 0061 0400  ...!..[......a..
+00007cc0: 001a 0000 0000 0000 0000 0000 0000 00dc  ................
+00007cd0: 0600 0078 6c2f 5f72 656c 732f 776f 726b  ...xl/_rels/work
+00007ce0: 626f 6f6b 2e78 6d6c 2e72 656c 7350 4b01  book.xml.relsPK.
+00007cf0: 022d 0014 0006 0008 0000 0021 0002 b9e3  .-.........!....
+00007d00: e113 0200 0065 0400 000f 0000 0000 0000  .....e..........
+00007d10: 0000 0000 0000 0027 0900 0078 6c2f 776f  .......'...xl/wo
+00007d20: 726b 626f 6f6b 2e78 6d6c 504b 0102 2d00  rkbook.xmlPK..-.
+00007d30: 1400 0600 0800 0000 2100 c795 eaa5 9103  ........!.......
+00007d40: 0000 3e0d 0000 1800 0000 0000 0000 0000  ..>.............
+00007d50: 0000 0000 670b 0000 786c 2f77 6f72 6b73  ....g...xl/works
+00007d60: 6865 6574 732f 7368 6565 7434 2e78 6d6c  heets/sheet4.xml
+00007d70: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
+00007d80: 13c4 2c13 c200 0000 4201 0000 2300 0000  ..,.....B...#...
+00007d90: 0000 0000 0000 0000 0000 2e0f 0000 786c  ..............xl
+00007da0: 2f77 6f72 6b73 6865 6574 732f 5f72 656c  /worksheets/_rel
+00007db0: 732f 7368 6565 7432 2e78 6d6c 2e72 656c  s/sheet2.xml.rel
+00007dc0: 7350 4b01 022d 0014 0006 0008 0000 0021  sPK..-.........!
+00007dd0: 003b 6d32 4bc1 0000 0042 0100 0023 0000  .;m2K....B...#..
+00007de0: 0000 0000 0000 0000 0000 0031 1000 0078  ...........1...x
+00007df0: 6c2f 776f 726b 7368 6565 7473 2f5f 7265  l/worksheets/_re
+00007e00: 6c73 2f73 6865 6574 312e 786d 6c2e 7265  ls/sheet1.xml.re
+00007e10: 6c73 504b 0102 2d00 1400 0600 0800 0000  lsPK..-.........
+00007e20: 2100 d95b 050c 5906 0000 0021 0000 1800  !..[..Y....!....
+00007e30: 0000 0000 0000 0000 0000 0000 3311 0000  ............3...
+00007e40: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
+00007e50: 6565 7432 2e78 6d6c 504b 0102 2d00 1400  eet2.xmlPK..-...
+00007e60: 0600 0800 0000 2100 8112 9d2b 9402 0000  ......!....+....
+00007e70: f308 0000 1800 0000 0000 0000 0000 0000  ................
+00007e80: 0000 c217 0000 786c 2f77 6f72 6b73 6865  ......xl/workshe
+00007e90: 6574 732f 7368 6565 7433 2e78 6d6c 504b  ets/sheet3.xmlPK
+00007ea0: 0102 2d00 1400 0600 0800 0000 2100 e628  ..-.........!..(
+00007eb0: 743d 522b 0000 102f 0100 1800 0000 0000  t=R+.../........
+00007ec0: 0000 0000 0000 0000 8c1a 0000 786c 2f77  ............xl/w
+00007ed0: 6f72 6b73 6865 6574 732f 7368 6565 7431  orksheets/sheet1
+00007ee0: 2e78 6d6c 504b 0102 2d00 1400 0600 0800  .xmlPK..-.......
+00007ef0: 0000 2100 e9a6 25b8 6606 0000 531b 0000  ..!...%.f...S...
+00007f00: 1300 0000 0000 0000 0000 0000 0000 1446  ...............F
+00007f10: 0000 786c 2f74 6865 6d65 2f74 6865 6d65  ..xl/theme/theme
+00007f20: 312e 786d 6c50 4b01 022d 0014 0006 0008  1.xmlPK..-......
+00007f30: 0000 0021 0037 b198 f114 0300 0090 0a00  ...!.7..........
+00007f40: 000d 0000 0000 0000 0000 0000 0000 00ab  ................
+00007f50: 4c00 0078 6c2f 7374 796c 6573 2e78 6d6c  L..xl/styles.xml
+00007f60: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
+00007f70: 6fc5 cb0e 3420 0000 176c 0000 1400 0000  o...4 ...l......
+00007f80: 0000 0000 0000 0000 0000 ea4f 0000 786c  ...........O..xl
+00007f90: 2f73 6861 7265 6453 7472 696e 6773 2e78  /sharedStrings.x
+00007fa0: 6d6c 504b 0102 2d00 1400 0600 0800 0000  mlPK..-.........
+00007fb0: 2100 d6d1 18e7 5501 0000 6b02 0000 1100  !.....U...k.....
+00007fc0: 0000 0000 0000 0000 0000 0000 5070 0000  ............Pp..
+00007fd0: 646f 6350 726f 7073 2f63 6f72 652e 786d  docProps/core.xm
+00007fe0: 6c50 4b01 022d 0014 0006 0008 0000 0021  lPK..-.........!
+00007ff0: 0014 987b 0399 0100 0000 2800 0027 0000  ...{......(..'..
+00008000: 0000 0000 0000 0000 0000 00dc 7200 0078  ............r..x
+00008010: 6c2f 7072 696e 7465 7253 6574 7469 6e67  l/printerSetting
+00008020: 732f 7072 696e 7465 7253 6574 7469 6e67  s/printerSetting
+00008030: 7332 2e62 696e 504b 0102 2d00 1400 0600  s2.binPK..-.....
+00008040: 0800 0000 2100 72de 7224 9801 0000 5203  ....!.r.r$....R.
+00008050: 0000 1000 0000 0000 0000 0000 0000 0000  ................
+00008060: ba74 0000 646f 6350 726f 7073 2f61 7070  .t..docProps/app
+00008070: 2e78 6d6c 504b 0102 2d00 1400 0600 0800  .xmlPK..-.......
+00008080: 0000 2100 e673 7a77 5e04 0000 f011 0000  ..!..szw^.......
+00008090: 2700 0000 0000 0000 0000 0000 0000 8877  '..............w
+000080a0: 0000 786c 2f70 7269 6e74 6572 5365 7474  ..xl/printerSett
+000080b0: 696e 6773 2f70 7269 6e74 6572 5365 7474  ings/printerSett
+000080c0: 696e 6773 312e 6269 6e50 4b05 0600 0000  ings1.binPK.....
+000080d0: 0011 0011 009e 0400 002b 7c00 0000 00    .........+|....
```

### Comparing `steam-sdk-2023.5.4/steam_sdk/configs/tools_defaults/ToolDefaultReader.py` & `steam-sdk-2023.6.0/steam_sdk/configs/tools_defaults/ToolDefaultReader.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/data/DataAnalysis.py` & `steam-sdk-2023.6.0/steam_sdk/data/DataAnalysis.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/data/DataConductor.py` & `steam-sdk-2023.6.0/steam_sdk/data/DataConductor.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,20 +95,18 @@
     th_insulation_along_height: float = None
     # Fractions given with respect to the insulated conductor
     f_superconductor: float = None
     f_stabilizer: float = None  # (related to CuFraction in ProteCCT)
     f_insulation: float = None
     f_inner_voids: float = None
     f_outer_voids: float = None
-    f_core: float = None
     # Available materials depend on the component and on the selected program
     material_insulation: str = None
     material_inner_voids: str = None
     material_outer_voids: str = None
-    material_core: str = None
 
 
 class Rutherford(BaseModel):
     """
         Rutherford cable type: for example LHC MB magnet cable
     """
     type: Literal['Rutherford']
```

### Comparing `steam-sdk-2023.5.4/steam_sdk/data/DataDakota.py` & `steam-sdk-2023.6.0/steam_sdk/data/DataDakota.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/data/DataEventCircuit.py` & `steam-sdk-2023.6.0/steam_sdk/data/DataEventCircuit.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/data/DataEventMagnet.py` & `steam-sdk-2023.6.0/steam_sdk/data/DataEventMagnet.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/data/DataFiQuS.py` & `steam-sdk-2023.6.0/steam_sdk/data/DataFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/data/DataLEDET.py` & `steam-sdk-2023.6.0/steam_sdk/data/DataLEDET.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     Tc0_NbTi_ht_inGroup: np.ndarray = np.array([])
     Bc2_NbTi_ht_inGroup: np.ndarray = np.array([])
     c1_Ic_NbTi_inGroup: np.ndarray = np.array([])
     c2_Ic_NbTi_inGroup: np.ndarray = np.array([])
     Tc0_Nb3Sn_inGroup: np.ndarray = np.array([])
     Bc2_Nb3Sn_inGroup: np.ndarray = np.array([])
     Jc_Nb3Sn0_inGroup: np.ndarray = np.array([])
-    alpha_Nb3Sn0_inGroup: np.ndarray = np.array([])
+    alpha_Nb3Sn_inGroup: np.ndarray = np.array([])
     f_scaling_Jc_BSCCO2212_inGroup: np.ndarray = np.array([])
     df_inGroup: np.ndarray = np.array([])
     selectedFit_inGroup: np.ndarray = np.array([])
     fitParameters_inGroup: np.ndarray = np.array([])
     overwrite_f_internalVoids_inGroup: np.ndarray = np.array([])
     overwrite_f_externalVoids_inGroup: np.ndarray = np.array([])
     alphasDEG: np.ndarray = np.array([])
@@ -177,14 +177,15 @@
     flag_showFigures: int = None
     flag_saveFigures: int = None
     flag_saveMatFile: int = None
     flag_saveTxtFiles: int = None
     flag_saveResultsToMesh: int = None
     flag_generateReport: int = None
     flag_hotSpotTemperatureInEachGroup: int = None
+    flag_importFieldWhenCalculatingHotSpotT: int = None
     flag_3D: int = None
     flag_adaptiveTimeStepping: int = None
     sim3D_flag_Import3DGeometry: int = None
     sim3D_import3DGeometry_modelNumber: int = None
 
 @dataclass
 class LEDETPlots:
```

### Comparing `steam-sdk-2023.5.4/steam_sdk/data/DataModelCircuit.py` & `steam-sdk-2023.6.0/steam_sdk/data/DataModelCircuit.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/data/DataModelConductor.py` & `steam-sdk-2023.6.0/steam_sdk/data/DataModelConductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/data/DataModelMagnet.py` & `steam-sdk-2023.6.0/steam_sdk/data/DataModelMagnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -390,30 +390,27 @@
     DistMax: float = None
 
 
 class MultipoleGeometry(BaseModel):
     """
         Level 2: Class for FiQuS Multipole
     """
+    simplified_coil: bool = None
     with_iron_yoke: bool = None
     with_wedges: bool = None
 
 
 class MultipoleMesh(BaseModel):
     """
         Level 2: Class for FiQuS Multipole
     """
     default_mesh: bool = None
     mesh_iron: Threshold = Threshold()
     mesh_coil: Threshold = Threshold()
-    MeshSizeMin: float = None  # sets gmsh Mesh.MeshSizeMin
-    MeshSizeMax: float = None  # sets gmsh Mesh.MeshSizeMax
-    MeshSizeFromCurvature: float = None  # sets gmsh Mesh.MeshSizeFromCurvature
     Algorithm: int = None  # sets gmsh Mesh.Algorithm
-    AngleToleranceFacetOverlap: float = None  # sets gmsh Mesh.AngleToleranceFacetOverlap
     ElementOrder: int = None  # sets gmsh Mesh.ElementOrder
     Optimize: int = None  # sets gmsh Mesh.Optimize
 
 
 class MultipoleSolve(BaseModel):
     """
         Level 2: Class for FiQuS Multipole
@@ -714,14 +711,15 @@
     flag_saveMatFile: int = None
     flag_saveTxtFiles: int = None
     flag_generateReport: int = None
     flag_saveResultsToMesh: int = None
     tQuench: List[float] = []
     initialQuenchTemp: List[float] = []
     flag_hotSpotTemperatureInEachGroup: int = None
+    flag_importFieldWhenCalculatingHotSpotT: int = None
 
 
 class Simulation3DLEDET(BaseModel):
     """
         Level 2: Class for 3D simulation parameters and options in lEDET
     """
     # Variables in the "Options" sheet
```

### Comparing `steam-sdk-2023.5.4/steam_sdk/data/DataParsimConductor.py` & `steam-sdk-2023.6.0/steam_sdk/data/DataParsimConductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/data/DataProteCCT.py` & `steam-sdk-2023.6.0/steam_sdk/data/DataProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/data/DataPyBBQ.py` & `steam-sdk-2023.6.0/steam_sdk/data/DataPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/data/DataRoxieParser.py` & `steam-sdk-2023.6.0/steam_sdk/data/DataRoxieParser.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,17 +258,17 @@
 
 
 class Corner(BaseModel):
     """
         Class for corner positions
     """
     iH: Coord = Coord()  # inner left
-    iLA: Coord = Coord()  # inner right
+    iL: Coord = Coord()  # inner right
     oH: Coord = Coord()  # outer left
-    oLA: Coord = Coord()  # outer right
+    oL: Coord = Coord()  # outer right
 
 
 class HalfTurnCorner(BaseModel):
     """
         Class for corner type
     """
     insulated: Corner = Corner()
@@ -279,36 +279,51 @@
     """
         Class for half-turn data
     """
     corners: HalfTurnCorner = HalfTurnCorner()
     strand_groups: Dict[int, StrandGroup] = {}
 
 
+class Order(BaseModel):
+    """
+        Class for electrical order (block location)
+    """
+    coil: int = None
+    pole: int = None
+    layer: int = None
+    winding: int = None
+    block: int = None
+
+
 class CenterShift(BaseModel):
     """
         Class for bore center shift
     """
     inner: Coord = Coord()
     outer: Coord = Coord()
 
 
 class Wedge(BaseModel):
     """
         Class for wedge positions
     """
     corners: Corner = Corner()
+    corners_ins: Corner = Corner()
     corrected_center: CenterShift = CenterShift()
-    coil: int = None
+    corrected_center_ins: CenterShift = CenterShift()
+    order_l: Order = Order()
+    order_h: Order = Order()
 
 
 class BlockData(BaseModel):
     """
         Class for block data
     """
     block_corners: Corner = Corner()
+    block_corners_ins: Corner = Corner()
     current_sign: int = None
     half_turns: Dict[int, HalfTurn] = {}
 
 
 class WindingData(BaseModel):
     """
         Class for winding data
@@ -336,25 +351,14 @@
     """
         Class for poles
     """
     poles: Dict[int, Layer] = {}
     bore_center: Coord = Coord()
 
 
-class Order(BaseModel):
-    """
-        Class for electrical order (block location)
-    """
-    coil: int = None
-    pole: int = None
-    layer: int = None
-    winding: int = None
-    block: int = None
-
-
 class CoilData(BaseModel):
     """
         Class for coils
     """
     coils: Dict[int, Pole] = {}
     physical_order: List[Order] = []
```

### Comparing `steam-sdk-2023.5.4/steam_sdk/data/DataSIGMA.py` & `steam-sdk-2023.6.0/steam_sdk/data/DataSIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/data/DataSettings.py` & `steam-sdk-2023.6.0/steam_sdk/data/DataSettings.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,26 @@
         Dataclass of settings for STEAM analyses
         This will be populated either form a local settings file (if flag_permanent_settings=False)
         or from the keys in the input analysis file (if flag_permanent_settings=True)
     """
     comsolexe_path:       str = None  # full path to comsol.exe, only COMSOL53a is supported
     JAVA_jdk_path:        str = None  # full path to folder with java jdk
     CFunLibPath:          str = None  # path to dll files with material properties
+    ANSYS_path:           str = None
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
+    local_COSIM_folder:   str = None  #
     local_Dakota_path:    str = None  # full path to local Dakota folder
     local_FiQuS_folder:   str = None  # full path to local FiQuS folder
     local_LEDET_folder:   str = None  # full path to local LEDET folder
     local_PyBBQ_folder:   str = None  # full path to local PyBBQ folder
     local_PSPICE_folder:  str = None  # full path to local PSPICE folder
     local_SIGMA_folder:   str = None  # full path to local SIGMA folder
     local_XYCE_folder:    str = None  # full path to local PSPICE folder
```

### Comparing `steam-sdk-2023.5.4/steam_sdk/data/DataSignal.py` & `steam-sdk-2023.6.0/steam_sdk/data/DataSignal.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/data/DictionaryLEDET.py` & `steam-sdk-2023.6.0/steam_sdk/data/DictionaryLEDET.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         # 'Conductor.material_properties.fit_Nb3Sn_cable.fit': '',
         # 'Conductor.material_properties.fit_Nb3Sn_cable.Tc0_Summers': 'Tc0_Nb3Sn_inGroup',
         # 'Conductor.material_properties.fit_Nb3Sn_cable.Bc20_Summers': 'Bc2_Nb3Sn_inGroup',
         # 'Conductor.material_properties.fit_Nb3Sn_cable.Jc0_Summers': 'Jc_Nb3Sn0_inGroup',
         # 'Conductor.material_properties.fit_Nb3Sn_cable.Tc0_Bordini': '',  # TODO: how to deal with the fact that Tc0_Nb3Sn_inGroup changes meaning in LEDET depending on the fit type?
         # 'Conductor.material_properties.fit_Nb3Sn_cable.Bc20_Bordini': '',  # TODO: how to deal with the fact that Bc2_Nb3Sn_inGroup changes meaning in LEDET depending on the fit type?
         # 'Conductor.material_properties.fit_Nb3Sn_cable.C0_Bordini': '',  # TODO: how to deal with the fact that Jc_Nb3Sn0_inGroup changes meaning in LEDET depending on the fit type?
-        # 'Conductor.material_properties.fit_Nb3Sn_cable.alpha_Bordini': 'alpha_Nb3Sn0_inGroup',
+        # 'Conductor.material_properties.fit_Nb3Sn_cable.alpha_Bordini': 'alpha_Nb3Sn_inGroup',
         # 'Conductor.material_properties.fit_Bi2212_cable.fit': '',
         # 'Conductor.material_properties.fit_Bi2212_cable.f_scaling_Jc_BSCCO2212': '',
 
         'Circuit.R_circuit': 'R_circuit',
         'Circuit.L_circuit': '',
         'Circuit.R_parallel': '',
 
@@ -224,14 +224,15 @@
         'Options_LEDET.post_processing.flag_saveMatFile': 'flag_saveMatFile',
         'Options_LEDET.post_processing.flag_saveTxtFiles': 'flag_saveTxtFiles',
         'Options_LEDET.post_processing.flag_saveResultsToMesh': 'flag_saveResultsToMesh',
         'Options_LEDET.post_processing.flag_generateReport': 'flag_generateReport',
         'Options_LEDET.post_processing.tQuench': 'tQuench',
         'Options_LEDET.post_processing.initialQuenchTemp': 'initialQuenchTemp',
         'Options_LEDET.post_processing.flag_hotSpotTemperatureInEachGroup': 'flag_hotSpotTemperatureInEachGroup',
+        'Options_LEDET.post_processing.flag_importFieldWhenCalculatingHotSpotT': 'flag_importFieldWhenCalculatingHotSpotT',
 
         'Options_LEDET.simulation_3D.flag_3D': 'flag_3D',
         'Options_LEDET.simulation_3D.flag_adaptiveTimeStepping': 'flag_adaptiveTimeStepping',
         'Options_LEDET.simulation_3D.sim3D_flag_Import3DGeometry': 'sim3D_flag_Import3DGeometry',
         'Options_LEDET.simulation_3D.sim3D_import3DGeometry_modelNumber': 'sim3D_import3DGeometry_modelNumber',
         'Options_LEDET.simulation_3D.sim3D_uThreshold': 'sim3D_uThreshold',
         'Options_LEDET.simulation_3D.sim3D_f_cooling_down': 'sim3D_f_cooling_down',
```

### Comparing `steam-sdk-2023.5.4/steam_sdk/data/DictionaryProteCCT.py` & `steam-sdk-2023.6.0/steam_sdk/data/DictionaryProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/data/DictionaryPyBBQ.py` & `steam-sdk-2023.6.0/steam_sdk/data/DictionaryPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/data/TemplateLEDET.py` & `steam-sdk-2023.6.0/steam_sdk/data/TemplateLEDET.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         ['Tc0_NbTi_ht_inGroup', None, 'Tc0_NbTi_ht_inGroup [K]'],
         ['Bc2_NbTi_ht_inGroup', None, 'Bc2_NbTi_ht_inGroup [T]'],
         ['c1_Ic_NbTi_inGroup', None, 'c1_Ic_NbTi_inGroup [A]'],
         ['c2_Ic_NbTi_inGroup', None, 'c2_Ic_NbTi_inGroup [A/T]'],
         ['Tc0_Nb3Sn_inGroup', None, 'Tc0_Nb3Sn [K]'],
         ['Bc2_Nb3Sn_inGroup', None, 'Bc2_Nb3Sn [T]'],
         ['Jc_Nb3Sn0_inGroup', None, 'Jc_Nb3Sn0 [A*T^0.5/m^2] Based on short-sample measurements'],
-        ['alpha_Nb3Sn0_inGroup', None, 'alpha parameter used when Bordini\'s Nb3Sn fit is selected'],
+        ['alpha_Nb3Sn_inGroup', None, 'alpha parameter used when Bordini\'s Nb3Sn fit is selected'],
         ['f_scaling_Jc_BSCCO2212_inGroup', None, 'scaling factor for the Jc(T,B) when BSCCO-2212 fit is selected'],
         ['df_inGroup', None, 'filament diameter [m]'],
         ['selectedFit_inGroup', None, 'Jc fit type (only used for persistent-current calculation): 1= Jc=constant; 2= Nb-Ti Bottura; 3= Nb-Ti CUDI ; 4= Nb3Sn Summers'],
         ['fitParameters_inGroup', None, 'Jc fit parameters [consult this report for more information: https://edms.cern.ch/document/2418186 ]'],
         ['overwrite_f_internalVoids_inGroup', None, 'Fraction of cable cross-section occupied by voids between strands and strands'],
         ['overwrite_f_externalVoids_inGroup', None, 'Fraction of cable cross-section occupied by voids between strands and insulation layers'],
         ['f_RRR1_Cu_inGroup', None, 'First Cu fraction of wire/strand in conductor with non-uniform RRR'],
@@ -217,14 +217,15 @@
         ['flag_showFigures', None, 'Show figures showing the main results'],
         ['flag_saveFigures', None, 'Save figures showing the main results'],
         ['flag_saveMatFile', None, 'Save main simulation results in a mat file (0=do not save; 1=save most variables; 2=save only most relevant variables)'],
         ['flag_saveTxtFiles', None, 'Save selected variables in a txt files. The variables are defined in the "Variables" sheet'],
         ['flag_saveResultsToMesh', None, 'Save selected variables and assign them to a given mesh of elements. The variables are defined in the "Variables" sheet  (default: No)'],
         ['flag_generateReport', None, 'Generate a report summarizing the simulation results (default: Yes)'],
         ['flag_hotSpotTemperatureInEachGroup', None, 'Calculate the hot-spot temperature in each group instead of in each coil section (default: No)'],
+        ['flag_importFieldWhenCalculatingHotSpotT', None, 'If set to 1, when calculating the hot-spot temperature during post-processing the magnetic field will be imported from the simulated field of the half-turn with the highest magnetic field in the field map (default=0)'],
         [None, None, None],
         [None, None, '3D Simulation Options'],
         ['flag_3D', None, 'If set to 1, the 3D model will run instead of the default 2D'],
         ['flag_adaptiveTimeStepping', None, 'If set to 1, adaptive time stepping will be enabled'],
         ['sim3D_flag_Import3DGeometry', None, 'Flag indicating that the 3D geometry and field map are imported from a csv file'],
         ['sim3D_import3DGeometry_modelNumber', None, 'Number indicating the input csv file containing the 3D geometry and field map'],
     ]
```

### Comparing `steam-sdk-2023.5.4/steam_sdk/data/TemplateProteCCT.py` & `steam-sdk-2023.6.0/steam_sdk/data/TemplateProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/drivers/DriverAnalysis.py` & `steam-sdk-2023.6.0/steam_sdk/drivers/DriverAnalysis.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/drivers/DriverDakota.py` & `steam-sdk-2023.6.0/steam_sdk/drivers/DriverDakota.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/drivers/DriverFiQuS.py` & `steam-sdk-2023.6.0/steam_sdk/drivers/DriverFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/drivers/DriverLEDET.py` & `steam-sdk-2023.6.0/steam_sdk/drivers/DriverLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/drivers/DriverPSPICE.py` & `steam-sdk-2023.6.0/steam_sdk/drivers/DriverPSPICE.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/drivers/DriverProteCCT.py` & `steam-sdk-2023.6.0/steam_sdk/drivers/DriverProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/drivers/DriverPyBBQ.py` & `steam-sdk-2023.6.0/steam_sdk/drivers/DriverPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/drivers/DriverSIGMA.py` & `steam-sdk-2023.6.0/steam_sdk/drivers/DriverSIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/drivers/DriverXYCE.py` & `steam-sdk-2023.6.0/steam_sdk/drivers/DriverXYCE.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/parsers/CSD_Reader.py` & `steam-sdk-2023.6.0/steam_sdk/parsers/CSD_Reader.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/parsers/ParserCond2d.py` & `steam-sdk-2023.6.0/steam_sdk/parsers/ParserCond2d.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/parsers/ParserCsd.py` & `steam-sdk-2023.6.0/steam_sdk/parsers/ParserCsd.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,13 +12,13 @@
     :return: dataframe with the selected signals
     '''
 
     if type(list_signals) == str: list_signals = [list_signals]           # If only one signal is passed as an argument, make it a list
     csd=CSD_read(full_name_file).data_dict
     csd['time'] = csd['Time']
     del csd['Time']
-    print(csd)
+    # print(csd)
     all_signals_df = pd.DataFrame.from_dict(csd) # read file into a dataframe
-    print(all_signals_df)
+    # print(all_signals_df)
     all_signals_df.columns = all_signals_df.columns.str.replace(' ', '')  # eliminate whitespaces from the column names
     list_signals = [x.replace(' ', '') for x in list_signals]             # eliminate whitespaces from the signal names
     return all_signals_df[list_signals]
```

### Comparing `steam-sdk-2023.5.4/steam_sdk/parsers/ParserCsv.py` & `steam-sdk-2023.6.0/steam_sdk/parsers/ParserCsv.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/parsers/ParserDakota.py` & `steam-sdk-2023.6.0/steam_sdk/parsers/ParserDakota.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/parsers/ParserDatToCsv.py` & `steam-sdk-2023.6.0/steam_sdk/parsers/ParserDatToCsv.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/parsers/ParserExcel.py` & `steam-sdk-2023.6.0/steam_sdk/parsers/ParserExcel.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/parsers/ParserFiQuS.py` & `steam-sdk-2023.6.0/steam_sdk/parsers/ParserFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/parsers/ParserLEDET.py` & `steam-sdk-2023.6.0/steam_sdk/parsers/ParserLEDET.py`

 * *Files 0% similar despite different names*

```diff
@@ -822,15 +822,15 @@
 #######################  Methods for consistency checks of LEDET input files - END  #######################
 
 
 #######################  Helper functions - START  #######################
 def _getOptionalVariables_input():
     # Define optional variables, which will be written only if present in the dataclass
     optional_variables_input_sheet = [
-        'alpha_Nb3Sn0_inGroup',
+        'alpha_Nb3Sn_inGroup',
         'f_scaling_Jc_BSCCO2212_inGroup',
         'overwrite_f_internalVoids_inGroup', 'overwrite_f_externalVoids_inGroup',
         'f_RRR1_Cu_inGroup', 'f_RRR2_Cu_inGroup', 'f_RRR3_Cu_inGroup',
         'RRR1_Cu_inGroup', 'RRR2_Cu_inGroup', 'RRR3_Cu_inGroup',
         ]
     return optional_variables_input_sheet
```

### Comparing `steam-sdk-2023.5.4/steam_sdk/parsers/ParserMap2d.py` & `steam-sdk-2023.6.0/steam_sdk/parsers/ParserMap2d.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/parsers/ParserMat.py` & `steam-sdk-2023.6.0/steam_sdk/parsers/ParserMat.py`

 * *Files 18% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     :param full_name_file: full path to the mat file
     :param list_signals: list of signals to read
     :return: dataframe with the selected signals
     '''
 
     with h5py.File(full_name_file, 'r') as simulationSignals:
         df_signals = pd.DataFrame()
-        number_of_time_steps = len(simulationSignals['time_vector'])
+        number_of_time_steps = len(simulationSignals['time_vector'])  #TODO it is bad to hard-code this logic!
         for label_signal in list_signals:
             if ('(' in label_signal) and (')' in label_signal):
                 # Special case: Only certain columns will be read
                 label_signal_split = label_signal.split('(')
                 signal        = label_signal_split[0]
                 rows_columns  = label_signal_split[1].rstrip(')').split(',')
                 label_rows    = rows_columns[0]
@@ -151,14 +151,77 @@
 
             simulationSignal = simulationSignal.flatten()
             df = pd.DataFrame({label_signal: simulationSignal})
             df_signals = pd.concat([df_signals, df], axis=1)
     return df_signals
 
 
+def get_signals_from_mat_to_dict(full_name_file: str, list_signals, bool_transpose: bool = True):
+    '''
+    Reads a mat file and returns a dataframe with the selected signals
+
+    Note: The selected signals can also be define with a special syntax that allows accessing one certain row or column (1-indexed).
+          Example: U_CoilSections(:,2) allows reading the 2nd column of the variable named U_CoilSections
+          Example: U_CoilSections(3,:) allows reading the 3rd row of the variable named U_CoilSections
+          Multiple columns/rows selection not currently supported  #TODO it would be nice to add
+
+    :param full_name_file: full path to the mat file
+    :param list_signals: list of signals to read
+    :return: dict with the selected signals
+    '''
+
+    with h5py.File(full_name_file, 'r') as simulationSignals:
+        dict_signals = {}
+        number_of_time_steps = len(simulationSignals['time_vector'])  #TODO it is bad to hard-code this logic!
+        for label_signal in list_signals:
+            if ('(' in label_signal) and (')' in label_signal):
+                # Special case: Only certain columns will be read
+                label_signal_split = label_signal.split('(')
+                signal        = label_signal_split[0]
+                rows_columns  = label_signal_split[1].rstrip(')').split(',')
+                label_rows    = rows_columns[0]
+                label_columns = rows_columns[1]
+
+
+                # Find slice of selected rows
+                if label_rows == ':':
+                    rows = slice(0, simulationSignals[signal].shape[1])
+                elif ':' in label_rows:
+                    raise Exception('Multiple rows selection not currently supported.')
+                    # label_rows_split = label_rows.split(':')
+                    # rows = slice(int(label_rows_split[0]) - 1, int(label_rows_split[1]) - 1)
+                else:
+                    rows = int(label_rows)
+
+                # Find slice of selected columns
+                if label_columns == ':':
+                    columns = slice(0, simulationSignals[signal].shape[0])
+                elif ':' in label_columns:
+                    raise Exception('Multiple columns selection not currently supported.')
+                    # label_columns_split = label_columns.split(':')
+                    # columns = slice(int(label_columns_split[0])-1, int(label_columns_split[1])-1)
+                else:
+                    columns = int(label_columns)-1
+
+                # Apply slices
+                if bool_transpose:
+                    simulationSignal = np.array(simulationSignals[signal][columns, rows])
+                else:
+                    simulationSignal = np.array(simulationSignals[signal][rows, columns])
+            else:
+                # Regular case: One-column signal is read
+                if bool_transpose:
+                    simulationSignal = np.array(simulationSignals[label_signal]).T
+                else:
+                    simulationSignal = np.array(simulationSignals[label_signal])
+
+            dict_signals[label_signal] = simulationSignal
+    return dict_signals
+
+
 def print_shapes_of_entries(simulationSignals):
     shapes_dict = {}
     for key, value in simulationSignals.items():
         # Check if the value is a dataset
         if isinstance(value, h5py.Dataset):
             # Check the shape of the dataset
             shape = value.shape
```

### Comparing `steam-sdk-2023.5.4/steam_sdk/parsers/ParserPSPICE.py` & `steam-sdk-2023.6.0/steam_sdk/parsers/ParserPSPICE.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,14 +257,29 @@
                     new_Component = Component()
                     new_Component.type = 'controlled-source component'
                     new_Component.nodes = nodes
                     new_Component.value = str(value)
                     self.circuit_data.Netlist.__setattr__(name, new_Component)
                     continue
 
+                # Special case: Diode component
+                if ('d' in line and line[0] == 'd') or ('D' in line and line[0] == 'D'):
+                    line_before, _, line_after = line.rstrip('\n').partition('(')  # Take the part of the string before and after the first "(" char
+                    name = str(line_before.strip(' '))
+                    line_before, _, line_after = line_after.rstrip(' ').partition(')')  # Take the part of the string before and after the first ")" char
+                    nodes = line_before.split(' ')
+                    value = line_after.strip(' { } ')  # Strip spaces and bracket at the extremities
+                    self.name_last_component = name
+                    new_Component = Component()
+                    new_Component.type = 'Diode component'
+                    new_Component.nodes = nodes
+                    new_Component.value = str(value)
+                    self.circuit_data.Netlist.__setattr__(self.name_last_component, new_Component)
+                    continue
+
                 # Special case: Parametrized component
                 if ('x' in line and line[0] == 'x') or ('X' in line and line[0] == 'X'):
                     self.flag_read_parametrized_component = True
                     line_before, _, line_after = line.rstrip('\n').partition('(')  # Take the part of the string before and after the first "(" char
                     name = str(line_before.strip(' '))
                     line_before, _, line_after = line_after.rstrip(' ').partition(')')  # Take the part of the string before and after the first ")" char
                     nodes = line_before.split(' ')
@@ -369,15 +384,15 @@
         :return:
         '''
 
         # Prepare header
         time_start = datetime.datetime.now()
         rows_header = [
             add_comment('PSPICE Netlist Simulation File'),
-            add_comment('Generated at {} at CERN using STEAM_SDK'.format(time_start)),
+            add_comment(f'Generated at {time_start} at CERN using STEAM_SDK'),
             add_comment('Authors: STEAM Team'),
         ]
 
         # Prepare stimuli
         rows_stimuli = []
         rows_stimuli.append(add_comment('**** Stimulus files ****'))  # Add header of this section
         if self.circuit_data.Stimuli.stimulus_files:
@@ -422,14 +437,15 @@
             # name, nodes, value, parameters, type = component.name, component.nodes, component.value, component.parameters, component.type
 
             # Check inputs
             if not type:
                 raise Exception('At least one netlist entry of known type must be added. Supported component types:\n' +
                                 '- comment\n' +
                                 '- standard component\n'
+                                '- Diode component\n'
                                 '- stimulus-controlled component\n'
                                 '- controlled-source component\n'
                                 '- pulsed-source component\n'
                                 '- parametrized component\n'
                                 '- transient-source component\n'
                                 'Netlist cannot be generated.')
 
@@ -438,14 +454,19 @@
                 if verbose: print('Netlist entry {} in position #{} is treated as a comment.'.format(name, s + 1))
                 rows_netlist.append(add_comment(value))
             elif type == 'standard component':
                 if name == None or nodes == None or value == None:
                     raise Exception('Netlist component in position #{} is of type {} and requires name, nodes, and value.'.format(s+1, type))
                 if verbose: print('Netlist entry {} in position #{} is treated as a standard component.'.format(name, s + 1))
                 rows_netlist.append(add_standard_component(name, nodes, value))
+            elif type == 'Diode component':
+                if name == None or nodes == None or value == None:
+                    raise Exception('Netlist component in position #{} is of type {} and requires name, nodes, and value.'.format(s+1, type))
+                if verbose: print('Netlist entry {} in position #{} is treated as a standard component.'.format(name, s + 1))
+                rows_netlist.append(add_Diode_component(name, nodes, value))
             elif type == 'stimulus-controlled component':
                 if name == None or nodes == None or value == None:
                     raise Exception('Netlist component in position #{} is of type {} and requires name, nodes, and value.'.format(s+1, type))
                 if verbose: print('Netlist entry {} in position #{} is treated as a stimulus-controlled component.'.format(name, s + 1))
                 rows_netlist.append(add_stimulus_controlled_component(name, nodes, value))
             elif type == 'pulsed-source component':
                 if name == None or nodes == None or value == None:
@@ -685,14 +706,20 @@
 
 def add_standard_component(name: str, nodes: list, value: str):
     ''' Format standard component netlist row '''
     str_nodes = " ".join(nodes)  # string with space-separated nodes
     formatted_text = name + ' (' + str_nodes + ') ' + '{' + str(value) + '}'
     return formatted_text
 
+def add_Diode_component(name: str, nodes: list, value: str):
+    ''' Format Diode component netlist row '''
+    str_nodes = " ".join(nodes)  # string with space-separated nodes
+    formatted_text = name + ' (' + str_nodes + ') ' + str(value)
+    return formatted_text
+
 def add_stimulus_controlled_component(name: str, nodes: list, value: str):
     ''' Format stimulus-controlled component netlist row '''
     str_nodes = " ".join(nodes)  # string with space-separated nodes
     str_stimulus = 'STIMULUS = ' + value
     formatted_text = name + ' (' + str_nodes + ') ' + str_stimulus
     return formatted_text
```

### Comparing `steam-sdk-2023.5.4/steam_sdk/parsers/ParserPdf.py` & `steam-sdk-2023.6.0/steam_sdk/parsers/ParserPdf.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/parsers/ParserProteCCT.py` & `steam-sdk-2023.6.0/steam_sdk/parsers/ParserProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/parsers/ParserProtePyBBQ.py` & `steam-sdk-2023.6.0/steam_sdk/parsers/ParserProtePyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/parsers/ParserRoxie.py` & `steam-sdk-2023.6.0/steam_sdk/parsers/ParserRoxie.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,47 +1,56 @@
-import os
+# import os
 from pathlib import Path
 import math
 from math import *
 import numpy as np
 import yaml
-from pydantic import BaseModel, PrivateAttr
-from typing import (Deque, Dict, FrozenSet, List, Optional, Sequence, Set, Tuple, Union, Type)
+from typing import Dict
 
 from steam_sdk.builders import geometricFunctions as gf
 from steam_sdk.data import DataRoxieParser as pd
 # import matplotlib.pyplot as plt
 # import matplotlib.lines as lines
 # import matplotlib.patches as patches
 
 
-def arcCenter(C, iH, oH, iLA, oLA, diff_radius=None):
+def arc_angle_between_point_and_abscissa(p, c):
+    """
+        Returns the angle of an arc with center c and endpoints at (cx + radius, cy) and (px, py)
+        :param p: list of x and y coordinates of a point
+        :param c: list of x and y coordinates of the arc center
+    """
+    theta = np.arctan2(p[1] - c[1], p[0] - c[0])
+    return theta + (2 * np.pi if theta < 0 else 0)
+
+
+def arcCenter(C, iH, oH, iL, oL, diff_radius=None):
     inner_radius = (np.sqrt(np.square(iH.x - C.x) + np.square(iH.y - C.y)) +
-                    np.sqrt(np.square(iLA.x - C.x) + np.square(iLA.y - C.y))) / 2
+                    np.sqrt(np.square(iL.x - C.x) + np.square(iL.y - C.y))) / 2
     if diff_radius:
         outer_radius = inner_radius + diff_radius
     else:
         outer_radius = (np.sqrt(np.square(oH.x - C.x) + np.square(oH.y - C.y)) +
-                        np.sqrt(np.square(oLA.x - C.x) + np.square(oLA.y - C.y))) / 2
-    d_inner = [0.5 * abs((iLA.x - iH.x)), 0.5 * abs((iH.y - iLA.y))]
-    d_outer = [0.5 * abs((oLA.x - oH.x)), 0.5 * abs((oH.y - oLA.y))]
+                        np.sqrt(np.square(oL.x - C.x) + np.square(oL.y - C.y))) / 2
+    d_inner = [0.5 * abs((iL.x - iH.x)), 0.5 * abs((iH.y - iL.y))]
+    d_outer = [0.5 * abs((oL.x - oH.x)), 0.5 * abs((oH.y - oL.y))]
     aa = [np.sqrt(np.square(d_inner[0]) + np.square(d_inner[1])),
           np.sqrt(np.square(d_outer[0]) + np.square(d_outer[1]))]
     bb = [np.sqrt(np.square(inner_radius) - np.square(aa[0])), np.sqrt(np.square(outer_radius) - np.square(aa[1]))]
-    if iLA.y < iH.y:
-        M_inner = [iH.x + d_inner[0], iLA.y + d_inner[1]]
-        M_outer = [oH.x + d_outer[0], oLA.y + d_outer[1]]
-        if iLA.y >= 0.:
+    if iL.y < iH.y:
+        M_inner = [iH.x + d_inner[0], iL.y + d_inner[1]]
+        M_outer = [oH.x + d_outer[0], oL.y + d_outer[1]]
+        if iL.y >= 0.:
             sign = [-1, -1]
         else:
             sign = [1, 1]
     else:
         M_inner = [iH.x + d_inner[0], iH.y + d_inner[1]]
         M_outer = [oH.x + d_outer[0], oH.y + d_outer[1]]
-        if iLA.y >= 0.:
+        if iL.y >= 0.:
             sign = [1, -1]
         else:
             sign = [-1, 1]
     inner = [M_inner[0] + sign[0] * bb[0] * d_inner[1] / aa[0], M_inner[1] + sign[1] * bb[0] * d_inner[0] / aa[0]]
     outer = [M_outer[0] + sign[0] * bb[1] * d_outer[1] / aa[1], M_outer[1] + sign[1] * bb[1] * d_outer[0] / aa[1]]
     return inner, outer
 
@@ -87,18 +96,18 @@
         for eo in roxie_data.coil.physical_order:
             winding = roxie_data.coil.coils[eo.coil].poles[eo.pole].layers[eo.layer].windings[eo.winding]
             block = winding.blocks[eo.block]
             for halfTurn_nr, halfTurn in block.half_turns.items():
                 self.idx_half_turn = self.idx_half_turn + 1
                 insulated = halfTurn.corners.insulated
                 bare = halfTurn.corners.bare
-                self.x_insulated.append([insulated.iH.x, insulated.oH.x, insulated.oLA.x, insulated.iLA.x])
-                self.y_insulated.append([insulated.iH.y, insulated.oH.y, insulated.oLA.y, insulated.iLA.y])
-                self.x_bare.append([bare.iH.x, bare.oH.x, bare.oLA.x, bare.iLA.x])
-                self.y_bare.append([bare.iH.y, bare.oH.y, bare.oLA.y, bare.iLA.y])
+                self.x_insulated.append([insulated.iH.x, insulated.oH.x, insulated.oL.x, insulated.iL.x])
+                self.y_insulated.append([insulated.iH.y, insulated.oH.y, insulated.oL.y, insulated.iL.y])
+                self.x_bare.append([bare.iH.x, bare.oH.x, bare.oL.x, bare.iL.x])
+                self.y_bare.append([bare.iH.y, bare.oH.y, bare.oL.y, bare.iL.y])
                 self.i_conductor.append(block.current_sign)
 
                 for strand_gr_nr, strand_gr in halfTurn.strand_groups.items():
                     for strand_nr, strand in strand_gr.strand_positions.items():
                         self.x_strand.append(strand.x)
                         self.y_strand.append(strand.y)
                         self.i_strand.append(block.current_sign)
@@ -583,14 +592,18 @@
             nRowsParameters = int(firstRow[5:])
             if verbose:
                 print('{} definition parameters have {} row(s)'.format(key, nRowsParameters))
 
             # Separate part of the data with group definition information
             parameters = fileContentByRow[keywords[key]['index'] + 1:keywords[key]['index'] + 1 + nRowsParameters]
 
+            if key == 'block':
+                self.layer_radius = list(set([float(row.split()[3]) for row in parameters]))
+                self.layer_radius.sort()
+
             # Assign parameters to a list of parameters objects
             for row in parameters:
                 rowSplitStr = row.split()
 
                 if key == 'group':
                     data.groups[rowSplitStr[0]] = pd.Group(symm=int(rowSplitStr[1]), typexy=int(rowSplitStr[2]),
                                                            blocks=list(map(int, rowSplitStr[3:-1])))
@@ -638,19 +651,15 @@
                                             '.data file.')
                         else:
                             if group_nr not in groups_list and block_nr not in trans_blocks_list:
                                 raise Exception('The current block is not transformed or belongs to a group that is not'
                                                 'transformed: check "BCS" under "EULER" in the .data file.')
 
                     radius = float(rowSplitStr[3])
-                    if radius not in self.layer_radius:
-                        self.layer_radius = self.layer_radius + [radius]
-                        layer = len(self.layer_radius)
-                    else:
-                        layer = self.layer_radius.index(radius) + 1
+                    layer = self.layer_radius.index(radius) + 1
 
                     turn = float(rowSplitStr[11])
                     if 'symm' in locals():
                         pole = floor(turn * symm / 360 + 1)
                     else:
                         pole = block_nr
 
@@ -1299,32 +1308,32 @@
                 # Apply shift2 cartesian shift transformation
                 xBareCable[i], yBareCable[i] = xBareCable[i] + shiftX, yBareCable[i] + shiftY
                 xCable[i], yCable[i] = xCable[i] + shiftX, yCable[i] + shiftY
 
             # Store cable positions
             block.half_turns[ht_nr].corners.insulated = pd.Corner(iH=pd.Coord(x=sigDig(xCable[0 if self.block.imag == 0 else 1]),
                                                                               y=sigDig(yCable[0 if self.block.imag == 0 else 1])),
-                                                                  iLA=pd.Coord(x=sigDig(xCable[1 if self.block.imag == 0 else 0]),
+                                                                  iL=pd.Coord(x=sigDig(xCable[1 if self.block.imag == 0 else 0]),
                                                                                y=sigDig(yCable[1 if self.block.imag == 0 else 0])),
-                                                                  oLA=pd.Coord(x=sigDig(xCable[2 if self.block.imag == 0 else 3]),
+                                                                  oL=pd.Coord(x=sigDig(xCable[2 if self.block.imag == 0 else 3]),
                                                                                y=sigDig(yCable[2 if self.block.imag == 0 else 3])),
                                                                   oH=pd.Coord(x=sigDig(xCable[3 if self.block.imag == 0 else 2]),
                                                                               y=sigDig(yCable[3 if self.block.imag == 0 else 2])))
             block.half_turns[ht_nr].corners.bare = pd.Corner(
                 iH=pd.Coord(x=sigDig(xBareCable[0 if self.block.imag == 0 else 1]), y=sigDig(yBareCable[0 if self.block.imag == 0 else 1])),
-                iLA=pd.Coord(x=sigDig(xBareCable[1 if self.block.imag == 0 else 0]), y=sigDig(yBareCable[1 if self.block.imag == 0 else 0])),
-                oLA=pd.Coord(x=sigDig(xBareCable[2 if self.block.imag == 0 else 3]), y=sigDig(yBareCable[2 if self.block.imag == 0 else 3])),
+                iL=pd.Coord(x=sigDig(xBareCable[1 if self.block.imag == 0 else 0]), y=sigDig(yBareCable[1 if self.block.imag == 0 else 0])),
+                oL=pd.Coord(x=sigDig(xBareCable[2 if self.block.imag == 0 else 3]), y=sigDig(yBareCable[2 if self.block.imag == 0 else 3])),
                 oH=pd.Coord(x=sigDig(xBareCable[3 if self.block.imag == 0 else 2]), y=sigDig(yBareCable[3 if self.block.imag == 0 else 2])))
 
             # if c == self.block.nco - 1:
             #     block.block_corners.iH = pd.Coord(x=sigDig(xCable[0]), y=sigDig(yCable[0]))  # 1
             #     block.block_corners.oH = pd.Coord(x=sigDig(xCable[3]), y=sigDig(yCable[3]))  # 4
             # elif c == 0:
-            #     block.block_corners.iLA = pd.Coord(x=sigDig(xCable[1]), y=sigDig(yCable[1]))  # 2
-            #     block.block_corners.oLA = pd.Coord(x=sigDig(xCable[2]), y=sigDig(yCable[2]))  # 3
+            #     block.block_corners.iL = pd.Coord(x=sigDig(xCable[1]), y=sigDig(yCable[1]))  # 2
+            #     block.block_corners.oL = pd.Coord(x=sigDig(xCable[2]), y=sigDig(yCable[2]))  # 3
             # else:
             #     pass
 
             if c == self.block.nco and c == 1:
                 corner0 = [xCable[0], yCable[0]]  # 1
                 corner3 = [xCable[3], yCable[3]]  # 4
                 corner1 = [xCable[1], yCable[1]]  # 2
@@ -1389,16 +1398,20 @@
         # self.ax.add_line(lines.Line2D([corner3[0], corner2[0]], [corner3[1], corner2[1]], color='red'))
         # self.ax.add_line(lines.Line2D([corner2[0], corner1[0]], [corner2[1], corner1[1]], color='red'))
         # self.ax.add_line(lines.Line2D([corner1[0], corner0[0]], [corner1[1], corner0[1]], color='red'))
         # plt.show()
         if self.block.type == 2 or self.block.nco == 1:
             block.block_corners.iH = pd.Coord(x=sigDig(corner0[0]), y=sigDig(corner0[1]))  # 1
             block.block_corners.oH = pd.Coord(x=sigDig(corner3[0]), y=sigDig(corner3[1]))  # 4
-            block.block_corners.iLA = pd.Coord(x=sigDig(corner1[0]), y=sigDig(corner1[1]))  # 2
-            block.block_corners.oLA = pd.Coord(x=sigDig(corner2[0]), y=sigDig(corner2[1]))  # 3
+            block.block_corners.iL = pd.Coord(x=sigDig(corner1[0]), y=sigDig(corner1[1]))  # 2
+            block.block_corners.oL = pd.Coord(x=sigDig(corner2[0]), y=sigDig(corner2[1]))  # 3
+            block.block_corners_ins.iH = pd.Coord(x=sigDig(corner0[0]), y=sigDig(corner0[1]))  # 1
+            block.block_corners_ins.oH = pd.Coord(x=sigDig(corner3[0]), y=sigDig(corner3[1]))  # 4
+            block.block_corners_ins.iL = pd.Coord(x=sigDig(corner1[0]), y=sigDig(corner1[1]))  # 2
+            block.block_corners_ins.oL = pd.Coord(x=sigDig(corner2[0]), y=sigDig(corner2[1]))  # 3
         else:
             new_corners_inner = gf.intersectLineCircle(gf.findLineThroughTwoPoints(corner0, corner3),
                                                        [radius, coil.bore_center.x, coil.bore_center.y])
             if min(abs(new_corners_inner[0][0] - corner0[0]),
                    abs(new_corners_inner[1][0] - corner0[0])) == abs(new_corners_inner[0][0] - corner0[0]):
                 new_inner = new_corners_inner[0]
             else:
@@ -1447,21 +1460,29 @@
             #     mid_outer_beg = new_corners_outer_mid[0]
             # else:
             #     mid_outer_beg = new_corners_outer_mid[1]
 
             if self.block.imag == 0:
                 block.block_corners.iH = pd.Coord(x=sigDig(mid_inner_end[0]), y=sigDig(mid_inner_end[1]))  # 1
                 block.block_corners.oH = pd.Coord(x=sigDig(mid_outer_end[0]), y=sigDig(mid_outer_end[1]))  # 4
-                block.block_corners.iLA = pd.Coord(x=sigDig(mid_inner_beg[0]), y=sigDig(mid_inner_beg[1]))  # 2
-                block.block_corners.oLA = pd.Coord(x=sigDig(mid_outer_beg[0]), y=sigDig(mid_outer_beg[1]))  # 3
+                block.block_corners.iL = pd.Coord(x=sigDig(mid_inner_beg[0]), y=sigDig(mid_inner_beg[1]))  # 2
+                block.block_corners.oL = pd.Coord(x=sigDig(mid_outer_beg[0]), y=sigDig(mid_outer_beg[1]))  # 3
+                block.block_corners_ins.iH = pd.Coord(x=sigDig(corner0[0]), y=sigDig(corner0[1]))  # 1
+                block.block_corners_ins.oH = pd.Coord(x=sigDig(corner3[0]), y=sigDig(corner3[1]))  # 4
+                block.block_corners_ins.iL = pd.Coord(x=sigDig(corner1[0]), y=sigDig(corner1[1]))  # 2
+                block.block_corners_ins.oL = pd.Coord(x=sigDig(corner2[0]), y=sigDig(corner2[1]))  # 3
             else:
-                block.block_corners.iLA = pd.Coord(x=sigDig(mid_inner_end[0]), y=sigDig(mid_inner_end[1]))
-                block.block_corners.oLA = pd.Coord(x=sigDig(mid_outer_end[0]), y=sigDig(mid_outer_end[1]))
+                block.block_corners.iL = pd.Coord(x=sigDig(mid_inner_end[0]), y=sigDig(mid_inner_end[1]))
+                block.block_corners.oL = pd.Coord(x=sigDig(mid_outer_end[0]), y=sigDig(mid_outer_end[1]))
                 block.block_corners.iH = pd.Coord(x=sigDig(mid_inner_beg[0]), y=sigDig(mid_inner_beg[1]))
                 block.block_corners.oH = pd.Coord(x=sigDig(mid_outer_beg[0]), y=sigDig(mid_outer_beg[1]))
+                block.block_corners_ins.iL = pd.Coord(x=sigDig(corner0[0]), y=sigDig(corner0[1]))  # 1
+                block.block_corners_ins.oL = pd.Coord(x=sigDig(corner3[0]), y=sigDig(corner3[1]))  # 4
+                block.block_corners_ins.iH = pd.Coord(x=sigDig(corner1[0]), y=sigDig(corner1[1]))  # 2
+                block.block_corners_ins.oH = pd.Coord(x=sigDig(corner2[0]), y=sigDig(corner2[1]))  # 3
 
             # new_corners_inner = gf.intersectLineCircle(
             #     gf.findLineThroughTwoPoints(corner0, corner3),
             #     [radius, coil.bore_center.x, coil.bore_center.y])
             # if min(abs(new_corners_inner[0][0] - corner0[0]),
             #        abs(new_corners_inner[1][0] - corner0[0])) == abs(new_corners_inner[0][0] - corner0[0]):
             #     new_inner = new_corners_inner[0]
@@ -1476,19 +1497,19 @@
             #        abs(new_corners_outer[1][0] - corner0[0])) == abs(new_corners_outer[0][0] - corner0[0]):
             #     new_outer = new_corners_outer[0]
             # else:
             #     new_outer = new_corners_outer[1]
             # if corner0[0] < corner1[0]:
             #     block.block_corners.iH = pd.Coord(x=sigDig(new_inner[0]), y=sigDig(new_inner[1]))  # 1
             #     block.block_corners.oH = pd.Coord(x=sigDig(new_outer[0]), y=sigDig(new_outer[1]))  # 4
-            #     block.block_corners.iLA = pd.Coord(x=sigDig(corner1[0]), y=sigDig(corner1[1]))  # 2
-            #     block.block_corners.oLA = pd.Coord(x=sigDig(corner2[0]), y=sigDig(corner2[1]))  # 3
+            #     block.block_corners.iL = pd.Coord(x=sigDig(corner1[0]), y=sigDig(corner1[1]))  # 2
+            #     block.block_corners.oL = pd.Coord(x=sigDig(corner2[0]), y=sigDig(corner2[1]))  # 3
             # else:
-            #     block.block_corners.iLA = pd.Coord(x=sigDig(new_inner[0]), y=sigDig(new_inner[1]))
-            #     block.block_corners.oLA = pd.Coord(x=sigDig(new_outer[0]), y=sigDig(new_outer[1]))
+            #     block.block_corners.iL = pd.Coord(x=sigDig(new_inner[0]), y=sigDig(new_inner[1]))
+            #     block.block_corners.oL = pd.Coord(x=sigDig(new_outer[0]), y=sigDig(new_outer[1]))
             #     block.block_corners.iH = pd.Coord(x=sigDig(corner1[0]), y=sigDig(corner1[1]))
             #     block.block_corners.oH = pd.Coord(x=sigDig(corner2[0]), y=sigDig(corner2[1]))
 
         # ((block.pole % 2 == 0) * np.sign(-I[0]) +
         #  (block.pole % 2 != 0) * np.sign(I[0])) * block.radius / 1e3]
 
         return self.data.coil
@@ -1509,24 +1530,27 @@
             :return: list
         """
         blockTypes = {1: 'Cos-theta', 2: 'Block-coil'}
 
         if blocks:
             self.roxieData.coil.blocks = blocks
 
+        for no, blk in self.roxieData.coil.blocks.items():
+            self.data.coil.physical_order.append(pd.Order(coil=blk.coil, pole=blk.pole, layer=blk.layer,
+                                                          winding=blk.winding, block=int(no)))
+
+        blk_layers = [[no, blk.layer] for no, blk in self.roxieData.coil.blocks.items()]
+        blk_layers.sort(key=lambda x: x[1])
         # plt.figure(figsize=(10, 10))
         # self.ax = plt.axes()
         # self.ax.set_xlim(-0.2, 0.2)
         # self.ax.set_ylim(-0.2, 0.2)
-        for no in self.roxieData.coil.blocks:
-            self.no = int(no)
-            self.block = self.roxieData.coil.blocks[no]
-            self.data.coil.physical_order.append(
-                pd.Order(coil=self.block.coil, pole=self.block.pole, layer=self.block.layer, winding=self.block.winding,
-                         block=self.no))
+        for pair in blk_layers:
+            self.no = int(pair[0])
+            self.block = self.roxieData.coil.blocks[pair[0]]
 
             # Get desired conductor data
             self.cond_name = self.block.condname
             self.getConductorFromCableDatabase(cadata=cadata)
 
             # Calculate x/y positions of the conductor corners and strands
             if verbose:
@@ -1568,51 +1592,64 @@
                             blocks = list(winding.blocks.keys())
                             adj_blocks = list(adj_winding.blocks.keys())
 
                             for block_key, block in winding.blocks.items():
                                 wedge_no += 1
                                 self.data.wedges[wedge_no] = pd.Wedge()
                                 wedge = self.data.wedges[wedge_no]
-                                wedge.coil = coil_nr
 
                                 if blocks.index(block_key) == 0:
-                                    wedge.corners = pd.Corner(iH=adj_winding.blocks[adj_blocks[0]].block_corners.iLA, iLA=block.block_corners.iH,
-                                                              oH=adj_winding.blocks[adj_blocks[0]].block_corners.oLA, oLA=block.block_corners.oH)
+                                    wedge.corners = pd.Corner(iH=adj_winding.blocks[adj_blocks[0]].block_corners.iL, iL=block.block_corners.iH,
+                                                              oH=adj_winding.blocks[adj_blocks[0]].block_corners.oL, oL=block.block_corners.oH)
+                                    wedge.corners_ins = pd.Corner(iH=adj_winding.blocks[adj_blocks[0]].block_corners_ins.iL, iL=block.block_corners_ins.iH,
+                                                                  oH=adj_winding.blocks[adj_blocks[0]].block_corners_ins.oL, oL=block.block_corners_ins.oH)
+                                    wedge.order_l = pd.Order(coil=coil_nr, pole=pole_nr, layer=layer_nr, winding=winding_key, block=block_key)
+                                    wedge.order_h = pd.Order(coil=coil_nr, pole=pole_nr, layer=layer_nr, winding=winding_key + 1, block=adj_blocks[0])
                                 else:
-                                    wedge.corners = pd.Corner(iH=block.block_corners.iLA, iLA=adj_winding.blocks[adj_blocks[blocks.index(block_key)]].block_corners.iH,
-                                                              oH=block.block_corners.oLA, oLA=adj_winding.blocks[adj_blocks[blocks.index(block_key)]].block_corners.oH)
+                                    wedge.corners = pd.Corner(iH=block.block_corners.iL, iL=adj_winding.blocks[adj_blocks[blocks.index(block_key)]].block_corners.iH,
+                                                              oH=block.block_corners.oL, oL=adj_winding.blocks[adj_blocks[blocks.index(block_key)]].block_corners.oH)
+                                    wedge.corners_ins = pd.Corner(iH=block.block_corners_ins.iL, iL=adj_winding.blocks[adj_blocks[blocks.index(block_key)]].block_corners_ins.iH,
+                                                                  oH=block.block_corners_ins.oL, oL=adj_winding.blocks[adj_blocks[blocks.index(block_key)]].block_corners_ins.oH)
+                                    wedge.order_h = pd.Order(coil=coil_nr, pole=pole_nr, layer=layer_nr, winding=winding_key, block=block_key)
+                                    wedge.order_l = pd.Order(coil=coil_nr, pole=pole_nr, layer=layer_nr, winding=winding_key + 1, block=adj_blocks[blocks.index(block_key)])
+
                                 # ax.text(wedge.corners.iH.x, wedge.corners.iH.y, 'iH', style='italic', bbox={'facecolor': 'red', 'pad': 2})
                                 # ax.text(wedge.corners.oH.x, wedge.corners.oH.y, 'oH', style='italic', bbox={'facecolor': 'red', 'pad': 2})
-                                # ax.text(wedge.corners.iLA.x, wedge.corners.iLA.y, 'iLA', style='italic', bbox={'facecolor': 'red', 'pad': 2})
-                                # ax.text(wedge.corners.oLA.x, wedge.corners.oLA.y, 'oLA', style='italic', bbox={'facecolor': 'red', 'pad': 2})
+                                # ax.text(wedge.corners.iL.x, wedge.corners.iL.y, 'iL', style='italic', bbox={'facecolor': 'red', 'pad': 2})
+                                # ax.text(wedge.corners.oL.x, wedge.corners.oL.y, 'oL', style='italic', bbox={'facecolor': 'red', 'pad': 2})
                                 # if blocks.index(block_key) == 0:
                                 #     corners1 = block.block_corners
                                 #     corners2 = adj_winding.blocks[adj_blocks[0]].block_corners
                                 # else:
                                 #     corners2 = block.block_corners
                                 #     corners1 = adj_winding.blocks[adj_blocks[blocks.index(block_key)]].block_corners
                                 #
-                                # if corners1.iLA.y >= 0.:
-                                #     wedge.corners = pd.Corner(iH=corners2.iLA, iLA=corners1.iH,
-                                #                               oH=corners2.oLA, oLA=corners1.oH)
+                                # if corners1.iL.y >= 0.:
+                                #     wedge.corners = pd.Corner(iH=corners2.iL, iL=corners1.iH,
+                                #                               oH=corners2.oL, oL=corners1.oH)
                                 # else:
-                                #     wedge.corners = pd.Corner(iH=corners1.iLA, iLA=corners2.iH,
-                                #                               oH=corners1.oLA, oLA=corners2.oH)
+                                #     wedge.corners = pd.Corner(iH=corners1.iL, iL=corners2.iH,
+                                #                               oH=corners1.oL, oL=corners2.oH)
 
                                 wedge.corrected_center = pd.CenterShift()
-                                if wedge.corners.iLA.y >= 0.:
-                                    inner, outer = arcCenter(C=coil.bore_center, iH=wedge.corners.iH, iLA=wedge.corners.iLA,
-                                                             oH=wedge.corners.oH, oLA=wedge.corners.oLA)
+                                wedge.corrected_center_ins = pd.CenterShift()
+                                if wedge.corners.iL.y >= 0.:
+                                    inner, outer = arcCenter(C=coil.bore_center, iH=wedge.corners.iH, iL=wedge.corners.iL,
+                                                             oH=wedge.corners.oH, oL=wedge.corners.oL)
+                                    inner_ins, outer_ins = arcCenter(C=coil.bore_center, iH=wedge.corners_ins.iH, iL=wedge.corners_ins.iL,
+                                                                     oH=wedge.corners_ins.oH, oL=wedge.corners_ins.oL)
                                 else:
-                                    inner, outer = arcCenter(C=coil.bore_center, iH=wedge.corners.iLA, iLA=wedge.corners.iH,
-                                                             oH=wedge.corners.oLA, oLA=wedge.corners.oH)
-                                wedge.corrected_center.inner = pd.Coord(x=float(sigDig(inner[0])),
-                                                                        y=float(sigDig(inner[1])))
-                                wedge.corrected_center.outer = pd.Coord(x=float(sigDig(outer[0])),
-                                                                        y=float(sigDig(outer[1])))
+                                    inner, outer = arcCenter(C=coil.bore_center, iH=wedge.corners.iL, iL=wedge.corners.iH,
+                                                             oH=wedge.corners.oL, oL=wedge.corners.oH)
+                                    inner_ins, outer_ins = arcCenter(C=coil.bore_center, iH=wedge.corners_ins.iL, iL=wedge.corners_ins.iH,
+                                                                     oH=wedge.corners_ins.oL, oL=wedge.corners_ins.oH)
+                                wedge.corrected_center.inner = pd.Coord(x=float(sigDig(inner[0])), y=float(sigDig(inner[1])))
+                                wedge.corrected_center.outer = pd.Coord(x=float(sigDig(outer[0])), y=float(sigDig(outer[1])))
+                                wedge.corrected_center_ins.inner = pd.Coord(x=float(sigDig(inner_ins[0])), y=float(sigDig(inner_ins[1])))
+                                wedge.corrected_center_ins.outer = pd.Coord(x=float(sigDig(outer_ins[0])), y=float(sigDig(outer_ins[1])))
                                 # ax.text(wedge.corrected_center.inner.x, wedge.corrected_center.inner.y, 'i' + str(wedge_no), style='italic', bbox={'facecolor': 'blue', 'pad': 2})
                                 # ax.text(wedge.corrected_center.outer.x, wedge.corrected_center.outer.y, 'o' + str(wedge_no), style='italic', bbox={'facecolor': 'blue', 'pad': 2})
 
         return self.data if coil else self.data.wedges
 
     def getData(self, dir_iron: Path = None, dir_data: Path = None, dir_cadata: Path = None,
                 dump_yamls: bool = False, verbose: bool = False):
```

### Comparing `steam-sdk-2023.5.4/steam_sdk/parsers/ParserSIGMA.py` & `steam-sdk-2023.6.0/steam_sdk/parsers/ParserSIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/parsers/ParserTdms.py` & `steam-sdk-2023.6.0/steam_sdk/parsers/ParserTdms.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/parsers/ParserXYCE.py` & `steam-sdk-2023.6.0/steam_sdk/parsers/ParserXYCE.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/parsers/ParserYAML.py` & `steam-sdk-2023.6.0/steam_sdk/parsers/ParserYAML.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,8 +89,11 @@
     data_dict = list_single_row_recursively(data_dict, list_exceptions=list_exceptions)
 
     # Make sure the target folder exists
     make_folder_if_not_existing(os.path.dirname(name_output_file), verbose=False)
 
     # Write yaml file
     with open(name_output_file, 'w') as yaml_file:
-        ruamel_yaml.dump(data_dict, yaml_file)
+        if with_comments:
+            ruamel.yaml.round_trip_dump(data_dict, yaml_file)
+        else:
+            ruamel_yaml.dump(data_dict, yaml_file)
```

### Comparing `steam-sdk-2023.5.4/steam_sdk/parsims/ParsimConductor.py` & `steam-sdk-2023.6.0/steam_sdk/parsims/ParsimConductor.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
             dict_attribute_to_column = yaml.safe_load(file)
 
         # set magnet name to local model
         rsetattr(self.data_parsim_conductor, 'GeneralParameters.magnet_name', magnet_name)
 
         # get column name of coil and magnet
         parsed_columns = []  # list containing the column names that were parsed
-        column_name_magnets, column_name_coils = self.__get_and_check_main_column_names(df_coils, parsed_columns, dict_attribute_to_column['MainColumnNames'])
+        column_name_magnets, column_name_coils = self.__read_and_check_main_column_names(df_coils, parsed_columns, dict_attribute_to_column['MainColumnNames'])
 
         # delete all rows of dataframe that don't belong to the magnet
         mask = df_coils[column_name_magnets] != magnet_name  # create a boolean mask for the rows that do not have the value in the column
         df_coils = df_coils.drop(df_coils[mask].index)  # drop the rows that do not have the value in the column
 
         # Assign the content to a dataclass structure - loop over all the coils of the magnet in the database
         for _, row in df_coils.iterrows():
@@ -158,15 +158,15 @@
         with open(path_output_file, 'w', newline='') as csv_file:
             writer = csv.DictWriter(csv_file, fieldnames=dict_sweeper.keys())
             writer.writeheader()
             writer.writerow(dict_sweeper)
 
     ################ HELPERS
 
-    def __get_and_check_main_column_names(self, df_coils: pd.DataFrame, parsed_columns: List[str], dict_attr_to_colname: Dict[str, List[str]]):
+    def __read_and_check_main_column_names(self, df_coils: pd.DataFrame, parsed_columns: List[str], dict_attr_to_colname: Dict[str, List[str]]):
         '''
         function checking the main columns "magnet name" and "coil name" and returning their column name
 
         :param df_coils: dataframe where every row represents one coil
         :param parsed_columns: A list of column names that have already been parsed (parsed columns are added)
         :param dict_attr_to_colname: A dictionary mapping attribute names of the coil (key) to possible column names (values)
         '''
@@ -376,15 +376,15 @@
             if not coil.coil_resistance_room_T:
                 warnings.warn(f'No room temperature resistance measurement for coil "{coil_name}" was found in database. Using default value for half_turn_length from modelData.')
                 continue
             original_conductor = self.model_data.Conductors[self.dict_coilName_to_conductorIndex[coil_name]]
             # calculate the optimized coil length for every group in the conductor sample separately
             for sample in coil.conductorSamples:
                 # optimize the length for this coil with one conductor
-                L = self.__optimize_coil_length_with_resistance_meas(sample, coil_name, original_conductor, coil)
+                L = self.__calculate_coil_length_with_resistance_meas(sample, coil_name, original_conductor, coil)
                 # for every conductorSamples add the optimized lengths together (to later make the average)
                 for group_number in self.groups_to_coils[coil_name]:
                     ht_len[group_number - 1] = ht_len[group_number - 1] + L
             # divide the sum of all the length with the number of conductorSamples do get the average value
             for index in self.groups_to_coils[coil_name]:
                 ht_len[index-1] = ht_len[index-1] / len(coil.conductorSamples)
 
@@ -397,15 +397,15 @@
         # if some values could not be calculated or been taken from modeldata, inform the user that calculation was skipped
         if any(l in [None, 0.0] for l in ht_len):
             warnings.warn(f'Length optimization was skipped. Not all ht lengths could be calculated from measurements or read from modelData.')
         else:
             # add the list to the sweeper dict as a string
             dict_sweeper[f'CoilWindings.half_turn_length'] = '[' + ', '.join(str(x) for x in ht_len) + ']'
 
-    def __optimize_coil_length_with_resistance_meas(self, conductor_sample: ConductorSample, coil_name: str,
+    def __calculate_coil_length_with_resistance_meas(self, conductor_sample: ConductorSample, coil_name: str,
                                                     original_conductor: Conductor, coil: Coil):
         """
         Optimizes the coil length using the room temperature resistance measurements using the formula:
         R_RT = rho * L / (fCu * A_cond) * f_twist_pitch -> solving for length L
 
         :param conductor_sample: A ConductorSample object containing sample data for the conductor
         :param coil_name: The name of the coil
@@ -526,15 +526,15 @@
                     # append value to sweeper dict
                     dict_sweeper[sweeper_cond_name + conductor_attribute_name] = val
 
             # insert Jc fit value(s) depending on their fitting function (usual Bottura, CUDI1, CUDI3 for NbTi and Summers, Bordini for Nb3Sn)
             Jc_dict_list = []
             for conductor_sample in coil.conductorSamples:
                 # calculate the parameters for Jc fit for every conductor sample of this coil
-                Jc_dict = self.__get_Jc_fit_params(original_conductor=self.model_data.Conductors[idx], coil_name=coil_name,
+                Jc_dict = self.__calculate_Jc_fit_params(original_conductor=self.model_data.Conductors[idx], coil_name=coil_name,
                                   strand_geometry=conductor_sample.strand_geometry, Bc20=conductor_sample.Bc20,
                                   Ic_measurements=conductor_sample.Ic_measurements, Tc0=conductor_sample.Tc0,
                                   n_strand=conductor_sample.number_of_strands, Cu_nCu=conductor_sample.Cu_noCu)
                 Jc_dict_list.append(Jc_dict)
             # Calculate the average of values for each key across all dictionaries in the list
             Jc_avg_dict = average_dicts(Jc_dict_list)
             for name, val in Jc_avg_dict.items():
@@ -545,19 +545,19 @@
                 # check if RT measurement is defined
                 if not coil.coil_resistance_room_T:
                     warnings.warn(f'No room temperature resistance measurement for coil "{coil_name}" was found in database. Not optimizing fraction of copper.')
                     continue
                 # calculate Cu_noCu for every conductor sample and use mean value
                 list_optimized_Cu_noCu = []
                 for sample in coil.conductorSamples:
-                    list_optimized_Cu_noCu.append(self.__optimize_fCu_with_resistance_meas(sample, coil_name, self.model_data.Conductors[idx], coil))
+                    list_optimized_Cu_noCu.append(self.__calculate_fCu_with_resistance_meas(sample, coil_name, self.model_data.Conductors[idx], coil))
                 # if the Cu no Cu ratio could be parsed directly from a column, overwrite it with optimized value
                 dict_sweeper[sweeper_cond_name + 'strand.Cu_noCu_in_strand'] = np.mean(list_optimized_Cu_noCu)
 
-    def __optimize_fCu_with_resistance_meas(self, conductor_sample: ConductorSample, coil_name: str,
+    def __calculate_fCu_with_resistance_meas(self, conductor_sample: ConductorSample, coil_name: str,
                                             original_conductor: Conductor, coil: Coil):
         """
         Optimizes the fraction of copper (fCu) using the room temperature resistance measurements using the formula:
         R_RT = rho * L / (fCu * A_cond) * f_twist_pitch -> solving for fCu
 
         :param conductor_sample: A ConductorSample object containing sample data for the conductor
         :param coil_name: The name of the coil
@@ -609,15 +609,15 @@
         if not Cu_noCu_old: Cu_noCu_old = conductor_sample.Cu_noCu
         if not Cu_noCu_old: Cu_noCu_old = original_conductor.strand.Cu_noCu_in_strand
         if self.verbose: print(f'Copper-non-Copper-ratio optimized form {Cu_noCu_old} to {Cu_noCu_new}.')
 
         # calculate fCu
         return Cu_noCu_new
     
-    def __get_Jc_fit_params(self, original_conductor: Conductor, strand_geometry: StrandGeometry, n_strand: int,
+    def __calculate_Jc_fit_params(self, original_conductor: Conductor, strand_geometry: StrandGeometry, n_strand: int,
                             Cu_nCu: float, Tc0: float, Bc20: float, Ic_measurements: List[IcMeasurement], coil_name: str):
         """
         Calculate Jc fit parameters for a coil based using the variables to change, the original conductor's properties
         and the provided critical current measurements.
 
         :param original_conductor: The original conductor object, needed for getting parameters if they are not being changed, meaning not present in conductor_sample
         :param strand_geometry: geometry of the conductor sample
```

### Comparing `steam-sdk-2023.5.4/steam_sdk/parsims/ParsimDakota.py` & `steam-sdk-2023.6.0/steam_sdk/parsims/ParsimDakota.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/parsims/ParsimEventCircuit.py` & `steam-sdk-2023.6.0/steam_sdk/parsims/ParsimEventCircuit.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/parsims/ParsimEventMagnet.py` & `steam-sdk-2023.6.0/steam_sdk/parsims/ParsimEventMagnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,29 +203,29 @@
             # Look into the tdms test campaign folders and search for files containing timestamp
             campaign_name_tdms, name_file_found_tdms = search_file_in_subfolders(timestamp, path_tdms_files, '.tdms')
 
             # if a tdms file could be found, append remaining values to dataframe - this event is finished
             if campaign_name_tdms and name_file_found_tdms:
                 new_row["Test name"] = name_file_found_tdms
                 new_row["Test campaign"] = campaign_name_tdms
-                new_row["Configuration"] = get_config_tdms(path_tdms_files, campaign_name_tdms, name_file_found_tdms,
+                new_row["Configuration"] = self.__get_config_tdms(path_tdms_files, campaign_name_tdms, name_file_found_tdms,
                                                            dict_configs_with_signals, self.verbose)
                 new_row["flag_convert_meas_csv"] = '1'  # csv will be generated by viewer if not present
                 df = pd.concat([df, pd.DataFrame([new_row])], ignore_index=True)  # Append the new row to the DataFrame
                 continue
 
 
             # if no tdms file present, search for csv file containing the timestamp
             campaign_name_csv, name_file_found_csv = search_file_in_subfolders(timestamp, path_output_measurement_files,'.csv')
 
             # if a csv file could be found, append remaining values to dataframe - this event is finished
             if campaign_name_csv and name_file_found_csv:
                 new_row["Test name"] = name_file_found_csv
                 new_row["Test campaign"] = campaign_name_csv
-                new_row["Configuration"] = get_config_csv(path_output_measurement_files, campaign_name_csv,
+                new_row["Configuration"] = self.__get_config_csv(path_output_measurement_files, campaign_name_csv,
                                                           name_file_found_csv, dict_configs_with_signals, self.verbose)
                 new_row["flag_convert_meas_csv"] = '0'  # Viewer will not try to convert data
                 df = pd.concat([df, pd.DataFrame([new_row])], ignore_index=True)  # Append the new row to the DataFrame
                 continue
 
 
             # if neither tdms nor csv is found, no measurement data is attached - Viewer shows only simulation results
@@ -405,15 +405,15 @@
 
     def __calculate_QH_R_cold(self):  # TODO: put it in BuilderModel?
         f_SS = self.ref_model.model_data.Options_LEDET.physics.fScaling_RhoSS
         w_QH = self.ref_model.model_data.Quench_Protection.Quench_Heaters.w
         h_QH = self.ref_model.model_data.Quench_Protection.Quench_Heaters.h
         l_QH = self.ref_model.model_data.Quench_Protection.Quench_Heaters.l
         f_QH = self.ref_model.model_data.Quench_Protection.Quench_Heaters.f_cover
-        rhoSS = 5.00E-07 * f_SS  # in [Ohm m]
+        rhoSS = 5.00E-07 * f_SS  # in [Ohm m]  # TODO use cfun?
         return [rhoSS / (w_QH[qh] * h_QH[qh]) * l_QH[qh] * f_QH[qh] for qh in range(len(w_QH))]
 
 
     def __read_general_parameters(self, event_info: pd.Series, new_event: DataEventMagnet, dict_attribute_to_column: Dict):
         '''
         Function to set GeneralParameters keys from data series into local DataEventMagnet class
 
@@ -545,15 +545,15 @@
             else:
                 list_values = [float(num_as_str.strip(' ')) for num_as_str in event_info[param].split(';')]
             if len(list_QH_circuits) != len(list_values):
                 raise Exception(f'The key "{key_QH_names}" has {len(list_QH_circuits)} values, while the key "{param}" has {len(list_values)} values.')
             for qh, qh_unit in enumerate(list_QH_circuits):
                 rsetattr(dict_QH[qh_unit], dict_params[param], list_values[qh])
 
-        # correct the measured trigger time by interpolating the discharge curve (U(t) = U * e^((t+T)/tau)) back in time
+        # correct the measured trigger time by interpolating the discharge curve (U(t) = U * e^(-(t+T)/tau)) back in time
         # to measure the start time, a threshold is used. The real trigger time is therefore earlier.
         if rel_quench_heater_trip_threshold is not None:
             for QH_name, QH in dict_QH.items():
                 # Calculate the time constant for the discharge
                 tau = QH.C * QH.R_total
                 # Calculate the corrected voltage based on the relative trip threshold
                 U_corrected = QH.U0 / rel_quench_heater_trip_threshold
@@ -611,14 +611,112 @@
         # check if config has been read correctly (at least one configuration has a list of measurement names)
         if all(value == [] for value in dict_configs_with_signals.values()):
             raise Exception(f'No valid configuration found in configurations file {path_config_file}')
 
         return dict_configs_with_signals
     
 
+
+    def __get_config_tdms(self, path_tdms_files, campaign_name, file_name, dict_configs_with_signals, verbose):
+        """
+        Read the TDMS file specified by the `path_tdms_files`, `campaign_name` and `file_name` arguments
+        using the ParserTdms class to make a list of all the measurement signal names present in the TDMS file.
+        The function returns the most advanced configuration by using the get_most_advanced_viewer_config function.
+
+        :param path_tdms_files: A string representing the path to the TDMS folder.
+        :param campaign_name: A string representing the name of the campaign.
+        :param file_name: A string representing the name of the TDMS file to be found.
+        :param dict_configs_with_signals: A dictionary holding all configurations (keys) and their needed signals (values).
+        :param verbose: A boolean indicating whether to print verbose output.
+        :return: name of the most advanced viewer configuration.
+        """
+        # define full path
+        full_path = Path(os.path.join(path_tdms_files, campaign_name, file_name + '.tdms')).resolve()
+
+        # init list
+        list_meas_signals = []
+
+        # for each group (LF, MF, HF) there can be different signals, dict keys are groups and values respective signals
+        dict_meas_signals_with_groups = ParserTdms(Path(full_path)).getNames()[2]
+
+        # loop through the dict
+        for group, signal_list in dict_meas_signals_with_groups.items():
+            # append the group name with the signal name and a . in between, as in the tdms files
+            for signal in signal_list:
+                list_meas_signals.append(group + '.' + signal)
+            # the time is not in signal list from the .getNames() function and has to be added here
+            list_meas_signals.append(group + '.Time [s]')
+
+        return self.__get_most_advanced_viewer_config(dict_configs_with_signals, list_meas_signals, file_name, verbose=verbose)
+
+    def __get_config_csv(self, path_parent_dir, campaign_name, file_name, dict_configs_with_signals, verbose):
+        """
+        Read all the signals present in a csv measurement file and return the most advanced configuration
+        by using the get_most_advanced_viewer_config function.
+
+        :param path_parent_dir: A string representing the path to the folder with all the campaigns in it.
+        :param campaign_name: A string representing the name of the campaign to look for csv files.
+        :param file_name: A string representing the name of the csv file.
+        :param dict_configs_with_signals: A dictionary containing the configurations with signals.
+        :param verbose: A boolean indicating whether to print verbose output.
+        :return: name of the most advanced viewer configuration.
+        """
+        # Initialization of list to store measurement signals
+        list_meas_signals = []
+
+        # Loop over campaign names and file names to get full path of csv file and extract signal names
+        for suffix in ["MF", "HF", "LF"]:
+            full_path = Path(os.path.join(path_parent_dir, campaign_name, file_name + '_' + suffix + '.csv')).resolve()
+            if os.path.isfile(full_path):
+                # read all the names of the columns (=names of the present signals)
+                csv_header = pd.read_csv(full_path, nrows=1).columns.tolist()
+
+                # Append the suffix to the header names
+                csv_header = [suffix + '.' + header_name for header_name in csv_header]
+
+                # Append the signal names to the list
+                list_meas_signals = list_meas_signals + csv_header
+
+        # Call the function to get the most advanced configuration
+        return self.__get_most_advanced_viewer_config(dict_configs_with_signals, list_meas_signals, file_name, verbose=verbose)
+
+
+    def __get_most_advanced_viewer_config(self, dict_configs_with_signals, list_meas_signals, filename, verbose):
+        """
+        Return the configuration name of the first dict where all signal names in its list of values are present in `list_meas_signals`.
+
+        :param dict_configs_with_signals: A dictionary with configuration names as keys and lists of signal names as values - Ordered from most advanced to least advanced.
+        :param list_meas_signals: A list of signal names found in tdms/csv measurement files.
+        :param filename: A string representing the name of the measurement file.
+        :param verbose: A boolean indicating whether to print verbose output.
+        :return: A string representing the most advanced viewer configuration.
+        """
+        #
+        if dict_configs_with_signals == {}: raise Exception(f'No configurations specified.')
+
+        # check for the configurations if all the needed signals are present and return the most advanced one
+        for config_name, signal_list in dict_configs_with_signals.items():
+            # check whether all the signal names in the configuration's list are present in the measurement signal list
+            if set(signal_list).issubset(set(list_meas_signals)):
+                # if all the signal names are present, return the configuration name
+                if verbose: print(f'{filename}: configuration {config_name} is used.')
+                return config_name
+            else:
+                # print missing signals and skip to the next configuration
+                missing_signals = set(signal_list).difference(set(list_meas_signals))
+                if verbose: print(f'{filename}: configuration {config_name} skipped. Could not find {missing_signals}')
+
+        # if no valid configuration could be found, raise an exception with an error message indicating the missing signals for the simplest configuration
+        if config_name and missing_signals:
+            raise Exception(f'No valid configuration could be found for measurement {filename}.\n'
+                            f'Missing signals for simplest configuration {config_name}: {missing_signals}')
+        else:
+            raise Exception(f'No valid configuration could be found for measurement {filename}.')
+
+
 def remove_frequency_suffix(name_file_found_csv):
     """
     Removes a frequency suffix ("_MF", "_HF", "_LF") from the end of a file name if existing
     """
     for suffix in ["_MF", "_HF", "_LF"]:
         if name_file_found_csv.endswith(suffix):
             name_file_found_csv = name_file_found_csv[:-len(suffix)]
@@ -681,105 +779,7 @@
                 campaign_name, name_file_found = list_campaign_names[0], list_file_names[0]
             else:
                 raise Exception(
                     f'More then one then one csv file with the specified timestamp found: {list_file_names}')
 
     # return tuple with lists of subfolder and file names
     return campaign_name, name_file_found
-
-
-def get_config_tdms(path_tdms_files, campaign_name, file_name, dict_configs_with_signals, verbose):
-    """
-    Read the TDMS file specified by the `path_tdms_files`, `campaign_name` and `file_name` arguments
-    using the ParserTdms class to make a list of all the measurement signal names present in the TDMS file.
-    The function returns the most advanced configuration by using the get_most_advanced_viewer_config function.
-
-    :param path_tdms_files: A string representing the path to the TDMS folder.
-    :param campaign_name: A string representing the name of the campaign.
-    :param file_name: A string representing the name of the TDMS file to be found.
-    :param dict_configs_with_signals: A dictionary holding all configurations (keys) and their needed signals (values).
-    :param verbose: A boolean indicating whether to print verbose output.
-    :return: name of the most advanced viewer configuration.
-    """
-    # define full path
-    full_path = Path(os.path.join(path_tdms_files, campaign_name, file_name + '.tdms')).resolve()
-
-    # init list
-    list_meas_signals = []
-
-    # for each group (LF, MF, HF) there can be different signals, dict keys are groups and values respective signals
-    dict_meas_signals_with_groups = ParserTdms(Path(full_path)).getNames()[2]
-
-    # loop through the dict
-    for group, signal_list in dict_meas_signals_with_groups.items():
-        # append the group name with the signal name and a . in between, as in the tdms files
-        for signal in signal_list:
-            list_meas_signals.append(group + '.' + signal)
-        # the time is not in signal list from the .getNames() function and has to be added here
-        list_meas_signals.append(group + '.Time [s]')
-
-    return get_most_advanced_viewer_config(dict_configs_with_signals, list_meas_signals, file_name, verbose=verbose)
-
-
-def get_config_csv(path_parent_dir, campaign_name, file_name, dict_configs_with_signals, verbose):
-    """
-    Read all the signals present in a csv measurement file and return the most advanced configuration
-    by using the get_most_advanced_viewer_config function.
-
-    :param path_parent_dir: A string representing the path to the folder with all the campaigns in it.
-    :param campaign_name: A string representing the name of the campaign to look for csv files.
-    :param file_name: A string representing the name of the csv file.
-    :param dict_configs_with_signals: A dictionary containing the configurations with signals.
-    :param verbose: A boolean indicating whether to print verbose output.
-    :return: name of the most advanced viewer configuration.
-    """
-    # Initialization of list to store measurement signals
-    list_meas_signals = []
-
-    # Loop over campaign names and file names to get full path of csv file and extract signal names
-    for suffix in ["MF", "HF", "LF"]:
-        full_path = Path(os.path.join(path_parent_dir, campaign_name, file_name + '_' + suffix + '.csv')).resolve()
-        if os.path.isfile(full_path):
-            # read all the names of the columns (=names of the present signals)
-            csv_header = pd.read_csv(full_path, nrows=1).columns.tolist()
-
-            # Append the suffix to the header names
-            csv_header = [suffix + '.' + header_name for header_name in csv_header]
-
-            # Append the signal names to the list
-            list_meas_signals = list_meas_signals + csv_header
-
-    # Call the function to get the most advanced configuration
-    return get_most_advanced_viewer_config(dict_configs_with_signals, list_meas_signals, file_name, verbose=verbose)
-
-
-def get_most_advanced_viewer_config(dict_configs_with_signals, list_meas_signals, filename, verbose):
-    """
-    Return the configuration name of the first dict where all signal names in its list of values are present in `list_meas_signals`.
-
-    :param dict_configs_with_signals: A dictionary with configuration names as keys and lists of signal names as values - Ordered from most advanced to least advanced.
-    :param list_meas_signals: A list of signal names found in tdms/csv measurement files.
-    :param filename: A string representing the name of the measurement file.
-    :param verbose: A boolean indicating whether to print verbose output.
-    :return: A string representing the most advanced viewer configuration.
-    """
-    #
-    if dict_configs_with_signals == {}: raise Exception(f'No configurations specified.')
-
-    # check for the configurations if all the needed signals are present and return the most advanced one
-    for config_name, signal_list in dict_configs_with_signals.items():
-        # check whether all the signal names in the configuration's list are present in the measurement signal list
-        if set(signal_list).issubset(set(list_meas_signals)):
-            # if all the signal names are present, return the configuration name
-            if verbose: print(f'{filename}: configuration {config_name} is used.')
-            return config_name
-        else:
-            # print missing signals and skip to the next configuration
-            missing_signals = set(signal_list).difference(set(list_meas_signals))
-            if verbose: print(f'{filename}: configuration {config_name} skipped. Could not find {missing_signals}')
-
-    # if no valid configuration could be found, raise an exception with an error message indicating the missing signals for the simplest configuration
-    if config_name and missing_signals:
-        raise Exception(f'No valid configuration could be found for measurement {filename}.\n'
-                        f'Missing signals for simplest configuration {config_name}: {missing_signals}')
-    else:
-        raise Exception(f'No valid configuration could be found for measurement {filename}.')
```

### Comparing `steam-sdk-2023.5.4/steam_sdk/parsims/ParsimSweep.py` & `steam-sdk-2023.6.0/steam_sdk/parsims/ParsimSweep.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/plotters/PlotterAnalysis.py` & `steam-sdk-2023.6.0/steam_sdk/plotters/PlotterAnalysis.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/plotters/PlotterMap2d.py` & `steam-sdk-2023.6.0/steam_sdk/plotters/PlotterMap2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -410,18 +410,18 @@
         for pole_nr, pole in coil.poles.items():
             for layer_nr, layer in pole.layers.items():
                 for winding_key, winding in layer.windings.items():
                     for block_key, block in winding.blocks.items():
                         for halfTurn_nr, halfTurn in block.half_turns.items():
                             insu = halfTurn.corners.insulated
                             bare = halfTurn.corners.bare
-                            xPos.append([insu.iH.x, insu.oH.x, insu.oLA.x, insu.iLA.x])
-                            yPos.append([insu.iH.y, insu.oH.y, insu.oLA.y, insu.iLA.y])
-                            xBarePos.append([bare.iH.x, bare.oH.x, bare.oLA.x, bare.iLA.x])
-                            yBarePos.append([bare.iH.y, bare.oH.y, bare.oLA.y, bare.iLA.y])
+                            xPos.append([insu.iH.x, insu.oH.x, insu.oL.x, insu.iL.x])
+                            yPos.append([insu.iH.y, insu.oH.y, insu.oL.y, insu.iL.y])
+                            xBarePos.append([bare.iH.x, bare.oH.x, bare.oL.x, bare.iL.x])
+                            yBarePos.append([bare.iH.y, bare.oH.y, bare.oL.y, bare.iL.y])
                             iPos.append(block.current_sign)
     return (xPos, yPos, xBarePos, yBarePos, iPos)
 
 def plotEdges(xPos, yPos, xBarePos, yBarePos, iPos, ax):
     # Plot edges
     for c, (cXPos, cYPos) in enumerate(zip(xPos, yPos)):
         pt1, pt2, pt3, pt4 = [cXPos[0]*1000, cYPos[0]*1000], [cXPos[1]*1000, cYPos[1]*1000], [cXPos[2]*1000, cYPos[2]*1000], [cXPos[3]*1000, cYPos[3]*1000]
```

### Comparing `steam-sdk-2023.5.4/steam_sdk/plotters/PlotterModel.py` & `steam-sdk-2023.6.0/steam_sdk/plotters/PlotterModel.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/plotters/PlotterParametric.py` & `steam-sdk-2023.6.0/steam_sdk/plotters/PlotterParametric.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/plotters/PlotterRoxie.py` & `steam-sdk-2023.6.0/steam_sdk/plotters/PlotterRoxie.py`

 * *Files 3% similar despite different names*

```diff
@@ -168,15 +168,15 @@
     for eo in roxie_data.coil.physical_order:
         winding = roxie_data.coil.coils[eo.coil].poles[eo.pole].layers[eo.layer].windings[eo.winding]
         block = winding.blocks[eo.block]
         for halfTurn_nr, halfTurn in block.half_turns.items():
             insu = halfTurn.corners.insulated
             bare = halfTurn.corners.bare
 
-            xPos.append([insu.iH.x, insu.oH.x, insu.oLA.x, insu.iLA.x])
-            yPos.append([insu.iH.y, insu.oH.y, insu.oLA.y, insu.iLA.y])
-            xBarePos.append([bare.iH.x, bare.oH.x, bare.oLA.x, bare.iLA.x])
-            yBarePos.append([bare.iH.y, bare.oH.y, bare.oLA.y, bare.iLA.y])
+            xPos.append([insu.iH.x, insu.oH.x, insu.oL.x, insu.iL.x])
+            yPos.append([insu.iH.y, insu.oH.y, insu.oL.y, insu.iL.y])
+            xBarePos.append([bare.iH.x, bare.oH.x, bare.oL.x, bare.iL.x])
+            yBarePos.append([bare.iH.y, bare.oH.y, bare.oL.y, bare.iL.y])
             iPos.append(block.current_sign)
     plotEdges(xPos, yPos, xBarePos, yBarePos, iPos, selectedFont)
 
     displayWaitAndClose(waitTimeBeforeMessage=.1, waitTimeAfterMessage=10)
```

### Comparing `steam-sdk-2023.5.4/steam_sdk/postprocs/PostprocsMetrics.py` & `steam-sdk-2023.6.0/steam_sdk/postprocs/PostprocsMetrics.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/utils/MTF_reading_functions.py` & `steam-sdk-2023.6.0/steam_sdk/utils/MTF_reading_functions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/utils/ModifyModelData.py` & `steam-sdk-2023.6.0/steam_sdk/utils/ModifyModelData.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/utils/ModifyModelDataMagnet.py` & `steam-sdk-2023.6.0/steam_sdk/utils/ModifyModelDataMagnet.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import os
 from pathlib import Path
 import yaml
+import ruamel.yaml
 from steam_sdk.data.DataModelMagnet import DataModelMagnet
 from steam_sdk.parsers.ParserYAML import dict_to_yaml
 
 if __name__ == "__main__":
     path_models = Path.joinpath(Path(__file__).parent.parent.parent, 'C:\\Users\emm\cernbox\SWAN_projects\steam_models\magnets')
-    path_models = Path.joinpath(Path(__file__).parent.parent.parent, r'C:\Users\jlidholm\cernbox\Git-projects\steam_models\magnets')
-    #path_models = Path.joinpath(Path(__file__).parent.parent.parent, 'tests/builders/model_library/magnets')
+    # path_models = Path.joinpath(Path(__file__).parent.parent.parent, r'E:\Python\steam_models\magnets')
+    # path_models = Path.joinpath(Path(__file__).parent.parent.parent, 'tests/builders/model_library/magnets')
     models = [x.parts[-1] for x in Path(path_models).iterdir() if x.is_dir()]
-    #models = ['MQXA']
+    #models = ['MCBRD']
 
     for mm in models:
         # Read file
         file_model_data = Path.joinpath(path_models, mm, 'input', 'modelData_' + mm + '.yaml')
         if os.path.isfile(file_model_data):
             # Load yaml keys into DataAnalysis dataclass
             with open(file_model_data, "r") as stream:
@@ -23,14 +24,15 @@
 
             # Note: Obsolete keys in yaml file will automatically be deleted
 
             # Note: New keys added to DataModelMagnet will automatically be added to the yaml file (UNLESS A VALUE IS ASSIGNED BELOW, THEIR VALUES WILL BE INITIALIZED TO DEFAULT)
 
             # Example to assign value to new keys in model data
             # model_data.Options_LEDET.magnet_inductance.flag_calculate_inductance = True
+            model_data.Options_LEDET.post_processing.flag_importFieldWhenCalculatingHotSpotT = 0
 
             # Example to change positions of key keeping its value (IF THIS IS NOT DONE THE INFOMRATION IN THE ORIGINAL YAML FILE WILL BE LOST!)
             # Note: The following will raise an exception if the keys do not exist in the original yaml file
             # model_data.Options_LEDET.magnet_inductance.LUT_DifferentialInductance_current = dictionary_yaml['GeneralParameters']['magnet_inductance']['fL_I']
             # model_data.Options_LEDET.magnet_inductance.LUT_DifferentialInductance_inductance = dictionary_yaml['GeneralParameters']['magnet_inductance']['fL_L']
             #
             # model_data.Options_LEDET.heat_exchange.heat_exchange_max_distance = dictionary_yaml['CoilWindings']['heat_exchange']['heat_exchange_max_distance']
@@ -40,15 +42,14 @@
             # model_data.Options_LEDET.heat_exchange.iContactAlongHeight_pairs_to_remove = dictionary_yaml['CoilWindings']['heat_exchange']['iContactAlongHeight_pairs_to_remove']
             # model_data.Options_LEDET.heat_exchange.th_insulationBetweenLayers = dictionary_yaml['CoilWindings']['heat_exchange']['th_insulationBetweenLayers']
             #
             # model_data.Options_LEDET.conductor_geometry_used_for_ISCL.alphaDEG_ht = dictionary_yaml['CoilWindings']['multipole']['alphaDEG_ht']
             # model_data.Options_LEDET.conductor_geometry_used_for_ISCL.rotation_ht = dictionary_yaml['CoilWindings']['multipole']['rotation_ht']
             # model_data.Options_LEDET.conductor_geometry_used_for_ISCL.mirror_ht = dictionary_yaml['CoilWindings']['multipole']['mirror_ht']
             # model_data.Options_LEDET.conductor_geometry_used_for_ISCL.mirrorY_ht = dictionary_yaml['CoilWindings']['multipole']['mirrorY_ht']
-            model_data.Quench_Protection.Quench_Heaters.turns_sides = ["O"] * len(model_data.Quench_Protection.Quench_Heaters.iQH_toHalfTurn_From)
 
             # Check and reformat the key values
             model_data = DataModelMagnet(**model_data.dict())
 
             # Write file
             # file_model_data_output = Path.joinpath(path_models, mm, 'input', 'modelData_' + mm + '_MODIFIED.yaml')  # use this line if you wish to test the results of this script
             file_model_data_output = file_model_data  # use this line if you wish to really update all yaml input files
```

### Comparing `steam-sdk-2023.5.4/steam_sdk/utils/ModifyModelDataconductor.py` & `steam-sdk-2023.6.0/steam_sdk/utils/ModifyModelDataconductor.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import yaml
 
 from steam_sdk.data.DataModelConductor import DataModelConductor
 from steam_sdk.parsers.ParserYAML import dict_to_yaml
 
 if __name__ == "__main__":
     path_models = Path.joinpath(Path(__file__).parent.parent.parent, 'C:\\Users\emm\cernbox\SWAN_projects\steam_models\conductors')
-    path_models = Path.joinpath(Path(__file__).parent.parent.parent, 'tests/builders/model_library/conductors')
+    # path_models = Path.joinpath(Path(__file__).parent.parent.parent, 'tests/builders/model_library/conductors')
     models = [x.parts[-1] for x in Path(path_models).iterdir() if x.is_dir()]
 
     for mm in models:
         # Read file
         file_model_data = Path.joinpath(path_models, mm, 'input', 'modelData_' + mm + '.yaml')
         if os.path.isfile(file_model_data):
             # Load yaml keys into DataAnalysis dataclass
```

### Comparing `steam-sdk-2023.5.4/steam_sdk/utils/clean_NaN_from_signal.py` & `steam-sdk-2023.6.0/steam_sdk/utils/clean_NaN_from_signal.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/utils/compare_two_parameters.py` & `steam-sdk-2023.6.0/steam_sdk/utils/compare_two_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/utils/create_coordinate_file_SIGMA.py` & `steam-sdk-2023.6.0/steam_sdk/utils/create_coordinate_file_SIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/utils/get_attribute_type.py` & `steam-sdk-2023.6.0/steam_sdk/utils/get_attribute_type.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/utils/misc.py` & `steam-sdk-2023.6.0/steam_sdk/utils/misc.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/utils/parse_str_to_list.py` & `steam-sdk-2023.6.0/steam_sdk/utils/parse_str_to_list.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/utils/tic_toc.py` & `steam-sdk-2023.6.0/steam_sdk/utils/tic_toc.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/utils/utils_PC.py` & `steam-sdk-2023.6.0/steam_sdk/utils/utils_PC.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/viewers/Viewer.py` & `steam-sdk-2023.6.0/steam_sdk/viewers/Viewer.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/viewers/ViewerMeas.py` & `steam-sdk-2023.6.0/steam_sdk/viewers/ViewerMeas.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/viewers/ViewerSim.py` & `steam-sdk-2023.6.0/steam_sdk/viewers/ViewerSim.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk/wrappers/wrapper_yaml.py` & `steam-sdk-2023.6.0/steam_sdk/wrappers/wrapper_yaml.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk.egg-info/PKG-INFO` & `steam-sdk-2023.6.0/steam_sdk.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: steam-sdk
-Version: 2023.5.4
+Version: 2023.6.0
 Summary: Source code for APIs for STEAM tools.
 Home-page: https://gitlab.cern.ch/steam/steam_sdk
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: STEAM,CERN,API,SDK
+Keywords: CERN,STEAM,SDK,API
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM_SDK
```

### Comparing `steam-sdk-2023.5.4/steam_sdk.egg-info/SOURCES.txt` & `steam-sdk-2023.6.0/steam_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.4/steam_sdk.egg-info/requires.txt` & `steam-sdk-2023.6.0/steam_sdk.egg-info/requires.txt`

 * *Files identical despite different names*

