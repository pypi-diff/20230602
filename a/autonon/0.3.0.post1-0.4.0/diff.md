# Comparing `tmp/autonon-0.3.0.post1.tar.gz` & `tmp/autonon-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autonon-0.3.0.post1.tar", last modified: Wed Mar  8 15:08:47 2023, max compression
+gzip compressed data, was "autonon-0.4.0.tar", last modified: Fri Jun  2 14:56:15 2023, max compression
```

## Comparing `autonon-0.3.0.post1.tar` & `autonon-0.4.0.tar`

### file list

```diff
@@ -1,787 +1,868 @@
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.671968 autonon-0.3.0.post1/
--rw-rw-rw-   0        0        0     1103 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/LICENSE
--rw-rw-rw-   0        0        0      189 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/MANIFEST.in
--rw-rw-rw-   0        0        0     2704 2023-03-08 15:08:47.670971 autonon-0.3.0.post1/PKG-INFO
--rw-rw-rw-   0        0        0     2203 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.293971 autonon-0.3.0.post1/autonon.egg-info/
--rw-rw-rw-   0        0        0     2704 2023-03-08 15:08:47.000000 autonon-0.3.0.post1/autonon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    35189 2023-03-08 15:08:47.000000 autonon-0.3.0.post1/autonon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-08 15:08:47.000000 autonon-0.3.0.post1/autonon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      325 2023-03-08 15:08:47.000000 autonon-0.3.0.post1/autonon.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-03-08 15:08:47.000000 autonon-0.3.0.post1/autonon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1231 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/cython_setup.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.293971 autonon-0.3.0.post1/organon/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.293971 autonon-0.3.0.post1/organon/afe/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.293971 autonon-0.3.0.post1/organon/afe/core/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.293971 autonon-0.3.0.post1/organon/afe/core/businessobjects/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/core/businessobjects/__init__.py
--rw-rw-rw-   0        0        0     2399 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/core/businessobjects/afe_static_objects.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.293971 autonon-0.3.0.post1/organon/afe/data/
--rw-rw-rw-   0        0        0      913 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/data/__init__.py
--rw-rw-rw-   0        0        0      305 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/data/base_df.zip
--rw-rw-rw-   0        0        0     9969 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/data/cash_df.zip
--rw-rw-rw-   0        0        0      271 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/data/score_df.zip
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.293971 autonon-0.3.0.post1/organon/afe/dataaccess/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/dataaccess/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.309584 autonon-0.3.0.post1/organon/afe/dataaccess/services/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/dataaccess/services/__init__.py
--rw-rw-rw-   0        0        0     1456 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/dataaccess/services/base_record_reader.py
--rw-rw-rw-   0        0        0      304 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/dataaccess/services/i_sample_data_service.py
--rw-rw-rw-   0        0        0     5474 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/dataaccess/services/sample_data_service.py
--rw-rw-rw-   0        0        0     4089 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/dataaccess/services/sample_data_service_helper.py
--rw-rw-rw-   0        0        0     9013 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/dataaccess/services/target_file_record_repository.py
--rw-rw-rw-   0        0        0    22930 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/dataaccess/services/transaction_file_record_reader.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.309584 autonon-0.3.0.post1/organon/afe/domain/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.309584 autonon-0.3.0.post1/organon/afe/domain/common/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/common/__init__.py
--rw-rw-rw-   0        0        0     3021 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/common/afe_date_helper.py
--rw-rw-rw-   0        0        0     7855 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/common/base_execution_plan_service.py
--rw-rw-rw-   0        0        0     9568 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/common/persist_helper.py
--rw-rw-rw-   0        0        0     4508 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/common/reader_helper.py
--rw-rw-rw-   0        0        0     3135 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/common/runtime_stats_service.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.319343 autonon-0.3.0.post1/organon/afe/domain/enums/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/enums/__init__.py
--rw-rw-rw-   0        0        0      447 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/enums/afe_date_column_encoding_type.py
--rw-rw-rw-   0        0        0      268 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/enums/afe_date_column_type.py
--rw-rw-rw-   0        0        0      261 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/enums/afe_learning_type.py
--rw-rw-rw-   0        0        0      980 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/enums/afe_operator.py
--rw-rw-rw-   0        0        0      252 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/enums/afe_target_column_type.py
--rw-rw-rw-   0        0        0      286 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/enums/binary_target_class.py
--rw-rw-rw-   0        0        0      273 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/enums/date_resolution.py
--rw-rw-rw-   0        0        0      216 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/enums/record_source_type.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.320340 autonon-0.3.0.post1/organon/afe/domain/modelling/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/modelling/__init__.py
--rw-rw-rw-   0        0        0    36067 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/modelling/abstract_modelling_service.py
--rw-rw-rw-   0        0        0     6903 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/modelling/auto_column_type_decider_service.py
--rw-rw-rw-   0        0        0     7224 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/modelling/base_modelling_service.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.328641 autonon-0.3.0.post1/organon/afe/domain/modelling/businessobjects/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/modelling/businessobjects/__init__.py
--rw-rw-rw-   0        0        0     4335 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/modelling/businessobjects/afe_column.py
--rw-rw-rw-   0        0        0      293 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/modelling/businessobjects/afe_feature.py
--rw-rw-rw-   0        0        0      444 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/modelling/businessobjects/base_afe_feature.py
--rw-rw-rw-   0        0        0     4765 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/modelling/businessobjects/bin_info.py
--rw-rw-rw-   0        0        0    29362 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/modelling/businessobjects/data_frame_builder.py
--rw-rw-rw-   0        0        0     3746 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/modelling/businessobjects/multi_target_entity_container.py
--rw-rw-rw-   0        0        0      503 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/modelling/businessobjects/target_file_record.py
--rw-rw-rw-   0        0        0     4584 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/modelling/businessobjects/target_file_record_collection.py
--rw-rw-rw-   0        0        0     1081 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/modelling/businessobjects/transaction_file_record.py
--rw-rw-rw-   0        0        0     4210 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/modelling/businessobjects/transaction_file_record_collection.py
--rw-rw-rw-   0        0        0     1546 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/modelling/businessobjects/transaction_file_stats.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.328641 autonon-0.3.0.post1/organon/afe/domain/modelling/helper/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/modelling/helper/__init__.py
--rw-rw-rw-   0        0        0    30343 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/modelling/helper/data_frame_builder_helper.pyx
--rw-rw-rw-   0        0        0     3059 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/modelling/helper/trx_reader_helper.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.328641 autonon-0.3.0.post1/organon/afe/domain/modelling/supervised/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/modelling/supervised/__init__.py
--rw-rw-rw-   0        0        0     1119 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/modelling/supervised/afe_supervised_algorithm_settings.py
--rw-rw-rw-   0        0        0     2336 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/modelling/supervised/multi_target_entity_container_service.py
--rw-rw-rw-   0        0        0    13567 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/modelling/supervised/multi_target_modelling_helper.py
--rw-rw-rw-   0        0        0     2812 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/modelling/supervised/multi_target_modelling_service.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.328641 autonon-0.3.0.post1/organon/afe/domain/modelling/unsupervised/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/modelling/unsupervised/__init__.py
--rw-rw-rw-   0        0        0      895 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/modelling/unsupervised/afe_unsupervised_algorithm_settings.py
--rw-rw-rw-   0        0        0     1331 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/modelling/unsupervised/unsupervised_feature_extraction_service.py
--rw-rw-rw-   0        0        0     1270 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/modelling/unsupervised/unsupervised_modelling_helper.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.328641 autonon-0.3.0.post1/organon/afe/domain/reporting/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/reporting/__init__.py
--rw-rw-rw-   0        0        0     7776 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/reporting/abstract_report_helper.py
--rw-rw-rw-   0        0        0      517 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/reporting/afe_column_dto.py
--rw-rw-rw-   0        0        0     2873 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/reporting/afe_matplotlib_report_helper.py
--rw-rw-rw-   0        0        0      322 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/reporting/afe_model_output.py
--rw-rw-rw-   0        0        0      334 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/reporting/afe_output_report.py
--rw-rw-rw-   0        0        0     2499 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/reporting/afe_plotly_report_helper.py
--rw-rw-rw-   0        0        0     1570 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/reporting/base_afe_model_output.py
--rw-rw-rw-   0        0        0     1567 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/reporting/base_afe_output_report.py
--rw-rw-rw-   0        0        0     1554 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/reporting/base_report_helper.py
--rw-rw-rw-   0        0        0     8397 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/reporting/dashboard_helper.py
--rw-rw-rw-   0        0        0    16863 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/reporting/matplotlib_common_functions.py
--rw-rw-rw-   0        0        0     6433 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/reporting/plotly_common_functions.py
--rw-rw-rw-   0        0        0     7667 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/reporting/plotly_dashboard_helper.py
--rw-rw-rw-   0        0        0      487 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/reporting/runtime_statistics.py
--rw-rw-rw-   0        0        0     2668 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/reporting/transformation.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.344264 autonon-0.3.0.post1/organon/afe/domain/scoring/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/scoring/__init__.py
--rw-rw-rw-   0        0        0    17479 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/scoring/afe_scoring_service.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.359887 autonon-0.3.0.post1/organon/afe/domain/settings/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/settings/__init__.py
--rw-rw-rw-   0        0        0      552 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/settings/afe_algorithm_settings.py
--rw-rw-rw-   0        0        0      683 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/settings/afe_data_settings.py
--rw-rw-rw-   0        0        0     1049 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/settings/afe_date_column.py
--rw-rw-rw-   0        0        0      661 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/settings/afe_modelling_settings.py
--rw-rw-rw-   0        0        0     1852 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/settings/afe_output_settings.py
--rw-rw-rw-   0        0        0      728 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/settings/afe_process_settings.py
--rw-rw-rw-   0        0        0      448 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/settings/afe_reading_settings.py
--rw-rw-rw-   0        0        0      465 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/settings/afe_scoring_settings.py
--rw-rw-rw-   0        0        0     1847 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/settings/afe_settings_reader.py
--rw-rw-rw-   0        0        0    11298 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/settings/afe_settings_type_validators.py
--rw-rw-rw-   0        0        0    35269 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/settings/afe_settings_validator.py
--rw-rw-rw-   0        0        0      806 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/settings/afe_target_column.py
--rw-rw-rw-   0        0        0     1066 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/settings/auto_column_decider_settings.py
--rw-rw-rw-   0        0        0     2165 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/settings/base_afe_data_settings.py
--rw-rw-rw-   0        0        0     2847 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/settings/base_afe_modelling_settings.py
--rw-rw-rw-   0        0        0     1383 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/settings/base_afe_scoring_settings.py
--rw-rw-rw-   0        0        0      306 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/settings/base_afe_settings.py
--rw-rw-rw-   0        0        0    26922 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/settings/base_afe_settings_reader.py
--rw-rw-rw-   0        0        0     1064 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/settings/base_trx_descriptor.py
--rw-rw-rw-   0        0        0     1025 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/settings/binary_target.py
--rw-rw-rw-   0        0        0      815 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/settings/db_object_input.py
--rw-rw-rw-   0        0        0     1628 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/settings/feature_generation_settings.py
--rw-rw-rw-   0        0        0      589 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/settings/model_settings.py
--rw-rw-rw-   0        0        0      814 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/settings/modelling_reduction_settings.py
--rw-rw-rw-   0        0        0     1374 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/settings/record_source.py
--rw-rw-rw-   0        0        0     1119 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/settings/target_descriptor.py
--rw-rw-rw-   0        0        0      539 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/settings/temporal_grid.py
--rw-rw-rw-   0        0        0     1179 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/settings/trx_descriptor.py
--rw-rw-rw-   0        0        0     3391 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/domain/settings/validation_helper.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.359887 autonon-0.3.0.post1/organon/afe/services/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/services/__init__.py
--rw-rw-rw-   0        0        0     2153 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/services/afe_application_operations.py
--rw-rw-rw-   0        0        0    36446 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/afe/services/afe_executor.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.359887 autonon-0.3.0.post1/organon/fl/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.359887 autonon-0.3.0.post1/organon/fl/core/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.359887 autonon-0.3.0.post1/organon/fl/core/businessobjects/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/businessobjects/__init__.py
--rw-rw-rw-   0        0        0     2676 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/businessobjects/data_partition.py
--rw-rw-rw-   0        0        0     2690 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/businessobjects/dataframe.py
--rw-rw-rw-   0        0        0     4940 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/businessobjects/date_interval.py
--rw-rw-rw-   0        0        0     3151 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/businessobjects/dict_dataframe.py
--rw-rw-rw-   0        0        0     1115 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/businessobjects/fl_core_static_objects.py
--rw-rw-rw-   0        0        0     8893 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/businessobjects/histogram_16.py
--rw-rw-rw-   0        0        0     1680 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/businessobjects/idata_partition.py
--rw-rw-rw-   0        0        0     2080 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/businessobjects/idataframe.py
--rw-rw-rw-   0        0        0     5123 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/businessobjects/np2d_dataframe.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.359887 autonon-0.3.0.post1/organon/fl/core/collections/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/collections/__init__.py
--rw-rw-rw-   0        0        0      946 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/collections/pair.py
--rw-rw-rw-   0        0        0     1252 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/collections/sorted_dict.py
--rw-rw-rw-   0        0        0      815 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/collections/sorted_list.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.359887 autonon-0.3.0.post1/organon/fl/core/enums/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/enums/__init__.py
--rw-rw-rw-   0        0        0      290 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/enums/column_measurement_type.py
--rw-rw-rw-   0        0        0      278 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/enums/column_native_type.py
--rw-rw-rw-   0        0        0      268 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/enums/date_interval_type.py
--rw-rw-rw-   0        0        0      256 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/enums/datetime_token.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.375511 autonon-0.3.0.post1/organon/fl/core/exceptionhandling/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/exceptionhandling/__init__.py
--rw-rw-rw-   0        0        0      170 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/exceptionhandling/known_exception.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.375511 autonon-0.3.0.post1/organon/fl/core/executionutil/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/executionutil/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.375511 autonon-0.3.0.post1/organon/fl/core/executionutil/objects/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/executionutil/objects/__init__.py
--rw-rw-rw-   0        0        0      413 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/executionutil/objects/locked_iterator.py
--rw-rw-rw-   0        0        0     1471 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/executionutil/objects/stopwatch.py
--rw-rw-rw-   0        0        0     2785 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/executionutil/parallel_execution_helper.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.375511 autonon-0.3.0.post1/organon/fl/core/extensions/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/extensions/__init__.py
--rw-rw-rw-   0        0        0     3730 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/extensions/string_extensions.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.375511 autonon-0.3.0.post1/organon/fl/core/fileoperations/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/fileoperations/__init__.py
--rw-rw-rw-   0        0        0      783 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/fileoperations/directory_helper.py
--rw-rw-rw-   0        0        0     2885 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/fileoperations/file_io_helper.py
--rw-rw-rw-   0        0        0      186 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/fileoperations/file_read_options.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.375511 autonon-0.3.0.post1/organon/fl/core/helpers/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/helpers/__init__.py
--rw-rw-rw-   0        0        0      586 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/helpers/boolean_helper.py
--rw-rw-rw-   0        0        0     6745 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/helpers/data_frame_helper.py
--rw-rw-rw-   0        0        0     5252 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/helpers/date_helper.py
--rw-rw-rw-   0        0        0     1119 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/helpers/dict_helper.py
--rw-rw-rw-   0        0        0      818 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/helpers/enums_helpers.py
--rw-rw-rw-   0        0        0     4309 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/helpers/environment_info_helper.py
--rw-rw-rw-   0        0        0     1111 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/helpers/float_helper.py
--rw-rw-rw-   0        0        0      657 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/helpers/function_helper.py
--rw-rw-rw-   0        0        0      525 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/helpers/guid_helper.py
--rw-rw-rw-   0        0        0     1107 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/helpers/list_helper.py
--rw-rw-rw-   0        0        0     2006 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/helpers/object_helper.py
--rw-rw-rw-   0        0        0     1585 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/helpers/process_info_helper.py
--rw-rw-rw-   0        0        0     6339 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/helpers/string_helper.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.375511 autonon-0.3.0.post1/organon/fl/core/iocutil/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/iocutil/__init__.py
--rw-rw-rw-   0        0        0     2528 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/iocutil/ioc_helper.py
--rw-rw-rw-   0        0        0      402 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/core/iocutil/ioc_registration_item.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.391134 autonon-0.3.0.post1/organon/fl/generic/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/generic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.391134 autonon-0.3.0.post1/organon/fl/generic/datadtos/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/generic/datadtos/__init__.py
--rw-rw-rw-   0        0        0      289 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/generic/datadtos/environment_info_dto.py
--rw-rw-rw-   0        0        0      291 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/generic/datadtos/process_info_dto.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.391134 autonon-0.3.0.post1/organon/fl/generic/enums/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/generic/enums/__init__.py
--rw-rw-rw-   0        0        0      225 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/generic/enums/os_type_id.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.391134 autonon-0.3.0.post1/organon/fl/generic/interaction/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/generic/interaction/__init__.py
--rw-rw-rw-   0        0        0     1229 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/generic/interaction/fl_initializer.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.391134 autonon-0.3.0.post1/organon/fl/logging/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/logging/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.391134 autonon-0.3.0.post1/organon/fl/logging/helpers/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/logging/helpers/__init__.py
--rw-rw-rw-   0        0        0    11191 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/logging/helpers/log_helper.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.391134 autonon-0.3.0.post1/organon/fl/mathematics/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/mathematics/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.391134 autonon-0.3.0.post1/organon/fl/mathematics/businessobjects/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/mathematics/businessobjects/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.391134 autonon-0.3.0.post1/organon/fl/mathematics/businessobjects/sets/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/mathematics/businessobjects/sets/__init__.py
--rw-rw-rw-   0        0        0     3977 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/mathematics/businessobjects/sets/interval.py
--rw-rw-rw-   0        0        0     1489 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/mathematics/businessobjects/sets/sum_triple.py
--rw-rw-rw-   0        0        0     1549 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/mathematics/businessobjects/tuple_generic_collection.py
--rw-rw-rw-   0        0        0      259 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/mathematics/constants.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.391134 autonon-0.3.0.post1/organon/fl/mathematics/enums/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/mathematics/enums/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.391134 autonon-0.3.0.post1/organon/fl/mathematics/enums/sets/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/mathematics/enums/sets/__init__.py
--rw-rw-rw-   0        0        0      235 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/mathematics/enums/sets/interval_type.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.391134 autonon-0.3.0.post1/organon/fl/mathematics/helpers/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/mathematics/helpers/__init__.py
--rw-rw-rw-   0        0        0      967 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/mathematics/helpers/dask_dataframe_operations.py
--rw-rw-rw-   0        0        0      931 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/mathematics/helpers/dataframe_operations_factory.py
--rw-rw-rw-   0        0        0     2337 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/mathematics/helpers/dict_dataframe_operations.py
--rw-rw-rw-   0        0        0     3266 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/mathematics/helpers/idataframe_operations.py
--rw-rw-rw-   0        0        0     4863 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/mathematics/helpers/pandas_dataframe_operations.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.406758 autonon-0.3.0.post1/organon/fl/mathematics/linearalgebra/
--rw-rw-rw-   0        0        0    16750 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/mathematics/linearalgebra/IBlas.py
--rw-rw-rw-   0        0        0    75446 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/mathematics/linearalgebra/MklFunctions.py
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/mathematics/linearalgebra/__init__.py
--rw-rw-rw-   0        0        0      969 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/mathematics/linearalgebra/blas_service_factory.py
--rw-rw-rw-   0        0        0      179 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/mathematics/linearalgebra/blas_service_type.py
--rw-rw-rw-   0        0        0     1583 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/mathematics/linearalgebra/enums.py
--rw-rw-rw-   0        0        0    16853 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/mathematics/linearalgebra/scipy_blas_service.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.406758 autonon-0.3.0.post1/organon/fl/mathematics/sweep/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/mathematics/sweep/__init__.py
--rw-rw-rw-   0        0        0     6638 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/mathematics/sweep/covariance_generator.py
--rw-rw-rw-   0        0        0     5050 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/mathematics/sweep/covariance_info.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.406758 autonon-0.3.0.post1/organon/fl/mathematics/sweep/data_classes/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/mathematics/sweep/data_classes/__init__.py
--rw-rw-rw-   0        0        0      758 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/mathematics/sweep/data_classes/linear_regression_algorithm_settings.py
--rw-rw-rw-   0        0        0      396 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/mathematics/sweep/data_classes/linear_regression_parameter.py
--rw-rw-rw-   0        0        0     2541 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/mathematics/sweep/data_classes/linear_regression_results.py
--rw-rw-rw-   0        0        0      847 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/mathematics/sweep/data_classes/linear_regression_step.py
--rw-rw-rw-   0        0        0     1378 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/mathematics/sweep/data_classes/selected_attribute.py
--rw-rw-rw-   0        0        0      336 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/mathematics/sweep/data_classes/swept_attribute.py
--rw-rw-rw-   0        0        0      355 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/mathematics/sweep/data_classes/transformation.py
--rw-rw-rw-   0        0        0      597 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/mathematics/sweep/enums.py
--rw-rw-rw-   0        0        0    25509 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/mathematics/sweep/fast_model_builder.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.406758 autonon-0.3.0.post1/organon/fl/mathematics/sweep/matrices/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/mathematics/sweep/matrices/__init__.py
--rw-rw-rw-   0        0        0     4895 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/mathematics/sweep/matrices/csc_matrix.py
--rw-rw-rw-   0        0        0     1682 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/mathematics/sweep/matrices/dense_matrix.py
--rw-rw-rw-   0        0        0      971 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/mathematics/sweep/matrices/i_matrix.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.406758 autonon-0.3.0.post1/organon/fl/mathematics/sweep/pyx_files/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/mathematics/sweep/pyx_files/__init__.py
--rw-rw-rw-   0        0        0     7951 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/mathematics/sweep/pyx_files/sweep_helper.pyx
--rw-rw-rw-   0        0        0    14453 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/mathematics/sweep/sweep_operator.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.406758 autonon-0.3.0.post1/organon/fl/security/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/security/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.406758 autonon-0.3.0.post1/organon/fl/security/helpers/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/security/helpers/__init__.py
--rw-rw-rw-   0        0        0     3637 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/security/helpers/encryption_helper.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.406758 autonon-0.3.0.post1/organon/fl/serialization/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/serialization/__init__.py
--rw-rw-rw-   0        0        0     1538 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/fl/serialization/serialization_helper.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.406758 autonon-0.3.0.post1/organon/idq/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.422381 autonon-0.3.0.post1/organon/idq/core/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/core/__init__.py
--rw-rw-rw-   0        0        0     1890 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/core/dq_constants.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.422381 autonon-0.3.0.post1/organon/idq/core/enums/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/core/enums/__init__.py
--rw-rw-rw-   0        0        0      162 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/core/enums/data_entity_type.py
--rw-rw-rw-   0        0        0     2520 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/core/enums/dq_comparison_result_code.py
--rw-rw-rw-   0        0        0      263 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/core/enums/dq_task_type.py
--rw-rw-rw-   0        0        0     1100 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/core/enums/dq_test_type.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.422381 autonon-0.3.0.post1/organon/idq/core/helpers/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/core/helpers/__init__.py
--rw-rw-rw-   0        0        0      413 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/core/helpers/formatting_helper.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.422381 autonon-0.3.0.post1/organon/idq/dataaccess/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/dataaccess/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.422381 autonon-0.3.0.post1/organon/idq/dataaccess/abstractions/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/dataaccess/abstractions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.422381 autonon-0.3.0.post1/organon/idq/dataaccess/helpers/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/dataaccess/helpers/__init__.py
--rw-rw-rw-   0        0        0     6807 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/dataaccess/helpers/record_source_filter_helper.py
--rw-rw-rw-   0        0        0     7873 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/dataaccess/record_source_reader.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.422381 autonon-0.3.0.post1/organon/idq/domain/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.422381 autonon-0.3.0.post1/organon/idq/domain/algorithms/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/algorithms/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.422381 autonon-0.3.0.post1/organon/idq/domain/algorithms/objects/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/algorithms/objects/__init__.py
--rw-rw-rw-   0        0        0      570 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/algorithms/objects/base_comparison_input.py
--rw-rw-rw-   0        0        0      584 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/algorithms/objects/mean_ci_comparison_input.py
--rw-rw-rw-   0        0        0      787 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/algorithms/objects/time_series_comparison_input.py
--rw-rw-rw-   0        0        0      616 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/algorithms/objects/traffic_light_comparison_input.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.422381 autonon-0.3.0.post1/organon/idq/domain/businessobjects/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/businessobjects/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.438004 autonon-0.3.0.post1/organon/idq/domain/businessobjects/data_column/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/businessobjects/data_column/__init__.py
--rw-rw-rw-   0        0        0      757 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/businessobjects/data_column/dq_data_column.py
--rw-rw-rw-   0        0        0      360 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/businessobjects/data_column/dq_df_data_column.py
--rw-rw-rw-   0        0        0      356 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/businessobjects/data_column/dq_file_data_column.py
--rw-rw-rw-   0        0        0      528 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/businessobjects/dq_calculation_output.py
--rw-rw-rw-   0        0        0      782 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/businessobjects/dq_calculation_result.py
--rw-rw-rw-   0        0        0     2066 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/businessobjects/dq_comparison_result.py
--rw-rw-rw-   0        0        0     2131 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/businessobjects/dq_control_parameters.py
--rw-rw-rw-   0        0        0     1852 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/businessobjects/dq_data_column_collection.py
--rw-rw-rw-   0        0        0      278 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/businessobjects/dq_data_source.py
--rw-rw-rw-   0        0        0      172 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/businessobjects/dq_settings.py
--rw-rw-rw-   0        0        0      312 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/businessobjects/dq_test_group.py
--rw-rw-rw-   0        0        0      266 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/businessobjects/main_sample_results.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.438004 autonon-0.3.0.post1/organon/idq/domain/businessobjects/record_sources/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/businessobjects/record_sources/__init__.py
--rw-rw-rw-   0        0        0      805 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/businessobjects/record_sources/dq_base_record_source.py
--rw-rw-rw-   0        0        0      663 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/businessobjects/record_sources/dq_df_record_source.py
--rw-rw-rw-   0        0        0      586 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/businessobjects/record_sources/dq_file_record_source.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.438004 autonon-0.3.0.post1/organon/idq/domain/businessobjects/statistics/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/businessobjects/statistics/__init__.py
--rw-rw-rw-   0        0        0      329 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/businessobjects/statistics/data_source_statistics.py
--rw-rw-rw-   0        0        0      250 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/businessobjects/statistics/dq_base_statistics.py
--rw-rw-rw-   0        0        0     1360 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/businessobjects/statistics/dq_categorical_statistics.py
--rw-rw-rw-   0        0        0      889 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/businessobjects/statistics/dq_population_numerical_statistics.py
--rw-rw-rw-   0        0        0     2442 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/businessobjects/statistics/dq_sample_numerical_statistics.py
--rw-rw-rw-   0        0        0      547 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/businessobjects/statistics/population_statistics.py
--rw-rw-rw-   0        0        0      510 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/businessobjects/statistics/sample_statistics.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.453627 autonon-0.3.0.post1/organon/idq/domain/controls/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/controls/__init__.py
--rw-rw-rw-   0        0        0     2267 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/controls/base_dq_control.py
--rw-rw-rw-   0        0        0     7345 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/controls/base_psi_signal_control.py
--rw-rw-rw-   0        0        0     7491 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/controls/column_mean_control.py
--rw-rw-rw-   0        0        0     4030 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/controls/data_source_stats_time_series_control.py
--rw-rw-rw-   0        0        0     4221 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/controls/data_source_stats_traffic_light_control.py
--rw-rw-rw-   0        0        0     3282 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/controls/duplicate_keys_control.py
--rw-rw-rw-   0        0        0     1958 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/controls/empty_table_control.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.453627 autonon-0.3.0.post1/organon/idq/domain/controls/helpers/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/controls/helpers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.453627 autonon-0.3.0.post1/organon/idq/domain/controls/helpers/algorithms/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/controls/helpers/algorithms/__init__.py
--rw-rw-rw-   0        0        0     1768 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/controls/helpers/algorithms/base_predictor.py
--rw-rw-rw-   0        0        0      311 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/controls/helpers/algorithms/prediction_result.py
--rw-rw-rw-   0        0        0      595 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/controls/helpers/algorithms/predictor_factory.py
--rw-rw-rw-   0        0        0     1828 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/controls/helpers/algorithms/random_forest_predictor.py
--rw-rw-rw-   0        0        0     1660 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/controls/helpers/column_values_comparer.py
--rw-rw-rw-   0        0        0     2138 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/controls/helpers/comparison_helper_functions.py
--rw-rw-rw-   0        0        0     1213 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/controls/helpers/psi_comparer.py
--rw-rw-rw-   0        0        0    19586 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/controls/helpers/traffic_light_comparer.py
--rw-rw-rw-   0        0        0     5023 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/controls/psi_nominal_signal_control.py
--rw-rw-rw-   0        0        0     9512 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/controls/psi_numeric_signal_control.py
--rw-rw-rw-   0        0        0    13421 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/controls/stable_column_control.py
--rw-rw-rw-   0        0        0     8096 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/controls/table_columns_control.py
--rw-rw-rw-   0        0        0     4365 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/controls/unexpected_nominal_values_control.py
--rw-rw-rw-   0        0        0     5416 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/controls/unexpected_numerical_values_control.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.453627 autonon-0.3.0.post1/organon/idq/domain/enums/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/enums/__init__.py
--rw-rw-rw-   0        0        0      520 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/enums/dq_control_type.py
--rw-rw-rw-   0        0        0      200 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/enums/dq_pred_algorithm_type.py
--rw-rw-rw-   0        0        0      223 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/enums/dq_record_source_type.py
--rw-rw-rw-   0        0        0      215 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/enums/dq_run_type.py
--rw-rw-rw-   0        0        0      354 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/enums/dq_test_group_type.py
--rw-rw-rw-   0        0        0      185 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/enums/signal_type.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.453627 autonon-0.3.0.post1/organon/idq/domain/helpers/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/helpers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.453627 autonon-0.3.0.post1/organon/idq/domain/helpers/statistics/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/helpers/statistics/__init__.py
--rw-rw-rw-   0        0        0     5986 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/helpers/statistics/dq_statistical_functions.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.453627 autonon-0.3.0.post1/organon/idq/domain/reporting/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/reporting/__init__.py
--rw-rw-rw-   0        0        0     5309 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/reporting/base_dq_report_helper.py
--rw-rw-rw-   0        0        0    14789 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/reporting/base_multiple_calculation_report_helper.py
--rw-rw-rw-   0        0        0     6963 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/reporting/dq_reporting_executor.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.453627 autonon-0.3.0.post1/organon/idq/domain/reporting/enum/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/reporting/enum/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.469250 autonon-0.3.0.post1/organon/idq/domain/reporting/helpers/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/reporting/helpers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.469250 autonon-0.3.0.post1/organon/idq/domain/reporting/objects/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/reporting/objects/__init__.py
--rw-rw-rw-   0        0        0      960 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/reporting/objects/base_alert_info.py
--rw-rw-rw-   0        0        0      622 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/reporting/objects/base_dq_output_report.py
--rw-rw-rw-   0        0        0     1036 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/reporting/objects/base_dq_report_helper_params.py
--rw-rw-rw-   0        0        0     1199 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/reporting/objects/base_multiple_calculation_report_helper_params.py
--rw-rw-rw-   0        0        0     1182 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/reporting/objects/dq_comparison_sample_report_input.py
--rw-rw-rw-   0        0        0      883 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/reporting/objects/nominal_column_control_details.py
--rw-rw-rw-   0        0        0      886 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/reporting/objects/numeric_column_control_details.py
--rw-rw-rw-   0        0        0      581 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/reporting/objects/signal_details.py
--rw-rw-rw-   0        0        0      213 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/reporting/objects/single_source_alert_info.py
--rw-rw-rw-   0        0        0      269 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/reporting/objects/single_source_report_helper_params.py
--rw-rw-rw-   0        0        0      239 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/reporting/objects/single_source_report_output.py
--rw-rw-rw-   0        0        0      820 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/reporting/objects/source_with_partitions_alert_info.py
--rw-rw-rw-   0        0        0      527 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/reporting/objects/source_with_partitions_dq_report_output.py
--rw-rw-rw-   0        0        0     1069 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/reporting/objects/source_with_partitions_report_helper_params.py
--rw-rw-rw-   0        0        0      753 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/reporting/objects/table_control_details.py
--rw-rw-rw-   0        0        0     3085 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/reporting/single_source_report_helper.py
--rw-rw-rw-   0        0        0     3786 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/reporting/source_with_partitions_report_helper.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.469250 autonon-0.3.0.post1/organon/idq/domain/services/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/services/__init__.py
--rw-rw-rw-   0        0        0    20865 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/services/base_user_input_service.py
--rw-rw-rw-   0        0        0     8866 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/services/base_user_input_validation_service.py
--rw-rw-rw-   0        0        0     8121 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/services/dq_full_process_executor.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.469250 autonon-0.3.0.post1/organon/idq/domain/services/output/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/services/output/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.484875 autonon-0.3.0.post1/organon/idq/domain/services/output/calculation/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/services/output/calculation/__init__.py
--rw-rw-rw-   0        0        0      187 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/services/output/calculation/db_source_stats_output_service.py
--rw-rw-rw-   0        0        0      187 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/services/output/calculation/df_source_stats_output_service.py
--rw-rw-rw-   0        0        0      189 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/services/output/calculation/file_source_stats_output_service.py
--rw-rw-rw-   0        0        0      233 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/services/output/calculation/stats_output_service.py
--rw-rw-rw-   0        0        0      914 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/services/output/dq_output_persistence_service.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.484875 autonon-0.3.0.post1/organon/idq/domain/services/statistics/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/services/statistics/__init__.py
--rw-rw-rw-   0        0        0     7565 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/services/statistics/dq_statistics_domain_service.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.484875 autonon-0.3.0.post1/organon/idq/domain/services/statistics/source_statistics/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/services/statistics/source_statistics/__init__.py
--rw-rw-rw-   0        0        0     3879 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/services/statistics/source_statistics/df_source_stats_service.py
--rw-rw-rw-   0        0        0     8660 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/services/statistics/source_statistics/dq_source_stats_base_service.py
--rw-rw-rw-   0        0        0     4783 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/services/statistics/source_statistics/file_source_stats_service.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.484875 autonon-0.3.0.post1/organon/idq/domain/services/task_executor/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/services/task_executor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.492201 autonon-0.3.0.post1/organon/idq/domain/services/task_executor/calculation/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/services/task_executor/calculation/__init__.py
--rw-rw-rw-   0        0        0     5953 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/services/task_executor/calculation/dq_calculation_task_executor.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.493199 autonon-0.3.0.post1/organon/idq/domain/services/task_executor/comparison/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/services/task_executor/comparison/__init__.py
--rw-rw-rw-   0        0        0     5237 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/services/task_executor/comparison/dq_comparison_task_executor.py
--rw-rw-rw-   0        0        0     1885 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/services/user_input_service.py
--rw-rw-rw-   0        0        0     1322 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/services/user_input_validation_service.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.497183 autonon-0.3.0.post1/organon/idq/domain/settings/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/settings/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.498699 autonon-0.3.0.post1/organon/idq/domain/settings/abstractions/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/settings/abstractions/__init__.py
--rw-rw-rw-   0        0        0     1213 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/settings/abstractions/dq_base_calculation_parameters.py
--rw-rw-rw-   0        0        0      998 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/settings/abstractions/dq_base_comparison_parameters.py
--rw-rw-rw-   0        0        0      951 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/settings/abstractions/dq_base_input_source_settings.py
--rw-rw-rw-   0        0        0     1003 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/settings/abstractions/dq_full_process_input.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.503039 autonon-0.3.0.post1/organon/idq/domain/settings/calculation/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/settings/calculation/__init__.py
--rw-rw-rw-   0        0        0      425 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/settings/calculation/dq_df_calculation_parameters.py
--rw-rw-rw-   0        0        0      428 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/settings/calculation/dq_file_calculation_parameters.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.504350 autonon-0.3.0.post1/organon/idq/domain/settings/comparison/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/settings/comparison/__init__.py
--rw-rw-rw-   0        0        0      417 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/settings/comparison/dq_df_comparison_parameters.py
--rw-rw-rw-   0        0        0      422 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/settings/comparison/dq_file_comparison_parameters.py
--rw-rw-rw-   0        0        0      937 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/settings/date_value_definition.py
--rw-rw-rw-   0        0        0      282 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/settings/dq_column_metadata.py
--rw-rw-rw-   0        0        0      284 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/settings/dq_comparison_column_info.py
--rw-rw-rw-   0        0        0      324 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/settings/dq_notification_settings.py
--rw-rw-rw-   0        0        0      187 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/settings/dq_output_settings.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.504350 autonon-0.3.0.post1/organon/idq/domain/settings/full_process/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/settings/full_process/__init__.py
--rw-rw-rw-   0        0        0      527 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/settings/full_process/dq_df_full_process_input.py
--rw-rw-rw-   0        0        0      536 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/settings/full_process/dq_file_full_process_input.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.504350 autonon-0.3.0.post1/organon/idq/domain/settings/input_source/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/settings/input_source/__init__.py
--rw-rw-rw-   0        0        0      489 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/settings/input_source/dq_df_input_source_settings.py
--rw-rw-rw-   0        0        0      656 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/settings/input_source/dq_file_input_source_settings.py
--rw-rw-rw-   0        0        0      266 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/settings/mail_notification_settings.py
--rw-rw-rw-   0        0        0     1750 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/domain/settings/partition_info.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.504350 autonon-0.3.0.post1/organon/idq/services/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/services/__init__.py
--rw-rw-rw-   0        0        0     5751 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/services/base_idq_executor.py
--rw-rw-rw-   0        0        0     1608 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/services/idq_application_operations.py
--rw-rw-rw-   0        0        0     1692 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/services/idq_executor.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.504350 autonon-0.3.0.post1/organon/idq/services/user_settings/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/services/user_settings/__init__.py
--rw-rw-rw-   0        0        0    14301 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/services/user_settings/base_dq_user_input.py
--rw-rw-rw-   0        0        0      696 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/services/user_settings/base_user_calculation_params.py
--rw-rw-rw-   0        0        0     1862 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/services/user_settings/dq_user_input.py
--rw-rw-rw-   0        0        0      689 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/services/user_settings/user_calculation_params.py
--rw-rw-rw-   0        0        0      274 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/services/user_settings/user_date_value_definition.py
--rw-rw-rw-   0        0        0      318 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/services/user_settings/user_db_obj_locator.py
--rw-rw-rw-   0        0        0      458 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/services/user_settings/user_existing_calculation_params.py
--rw-rw-rw-   0        0        0      718 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/services/user_settings/user_input_source_settings.py
--rw-rw-rw-   0        0        0      705 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/services/user_settings/user_multi_partition_calculation_params.py
--rw-rw-rw-   0        0        0      416 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/idq/services/user_settings/user_partition_info.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.504350 autonon-0.3.0.post1/organon/ml/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.504350 autonon-0.3.0.post1/organon/ml/common/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.504350 autonon-0.3.0.post1/organon/ml/common/enums/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/common/enums/__init__.py
--rw-rw-rw-   0        0        0      190 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/common/enums/classification_type.py
--rw-rw-rw-   0        0        0      296 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/common/enums/pretrained_model_type.py
--rw-rw-rw-   0        0        0      193 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/common/enums/target_type.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.504350 autonon-0.3.0.post1/organon/ml/common/helpers/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/common/helpers/__init__.py
--rw-rw-rw-   0        0        0     3393 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/common/helpers/df_ops_helper.py
--rw-rw-rw-   0        0        0      359 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/common/helpers/parameter_helper.py
--rw-rw-rw-   0        0        0      847 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/common/helpers/user_input_service_helper.py
--rw-rw-rw-   0        0        0      970 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/common/helpers/validation_helper.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.504350 autonon-0.3.0.post1/organon/ml/common/objects/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/common/objects/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.504350 autonon-0.3.0.post1/organon/ml/feature_reduction/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_reduction/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.519973 autonon-0.3.0.post1/organon/ml/feature_reduction/domain/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_reduction/domain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.519973 autonon-0.3.0.post1/organon/ml/feature_reduction/domain/enums/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_reduction/domain/enums/__init__.py
--rw-rw-rw-   0        0        0      296 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_reduction/domain/enums/feature_reduction_types.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.519973 autonon-0.3.0.post1/organon/ml/feature_reduction/domain/objects/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_reduction/domain/objects/__init__.py
--rw-rw-rw-   0        0        0      391 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_reduction/domain/objects/feature_reduction_output.py
--rw-rw-rw-   0        0        0      826 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_reduction/domain/objects/numeric_column_stats.py
--rw-rw-rw-   0        0        0      464 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_reduction/domain/objects/univariate_performance_reduction_output.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.519973 autonon-0.3.0.post1/organon/ml/feature_reduction/domain/reductions/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_reduction/domain/reductions/__init__.py
--rw-rw-rw-   0        0        0     1369 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_reduction/domain/reductions/base_feature_reduction.py
--rw-rw-rw-   0        0        0     5892 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_reduction/domain/reductions/high_correlated_feature_reduction.py
--rw-rw-rw-   0        0        0     2017 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_reduction/domain/reductions/null_feature_reduction.py
--rw-rw-rw-   0        0        0     7466 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_reduction/domain/reductions/similar_distribution_feature_reduction.py
--rw-rw-rw-   0        0        0     1183 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_reduction/domain/reductions/stability_feature_reduction.py
--rw-rw-rw-   0        0        0     4365 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_reduction/domain/reductions/univariate_performance_feature_reduction.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.519973 autonon-0.3.0.post1/organon/ml/feature_reduction/domain/services/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_reduction/domain/services/__init__.py
--rw-rw-rw-   0        0        0     4021 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_reduction/domain/services/feature_reduction_service.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.519973 autonon-0.3.0.post1/organon/ml/feature_reduction/services/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_reduction/services/__init__.py
--rw-rw-rw-   0        0        0     3607 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_reduction/services/feature_reduction.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.519973 autonon-0.3.0.post1/organon/ml/feature_reduction/settings/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_reduction/settings/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.519973 autonon-0.3.0.post1/organon/ml/feature_reduction/settings/enums/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_reduction/settings/enums/__init__.py
--rw-rw-rw-   0        0        0    11831 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_reduction/settings/feature_reduction_user_input_service.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.535596 autonon-0.3.0.post1/organon/ml/feature_reduction/settings/objects/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_reduction/settings/objects/__init__.py
--rw-rw-rw-   0        0        0      230 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_reduction/settings/objects/base_feature_reduction_settings.py
--rw-rw-rw-   0        0        0      694 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_reduction/settings/objects/high_correlated_feature_reduction_settings.py
--rw-rw-rw-   0        0        0      370 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_reduction/settings/objects/null_feature_reduction_settings.py
--rw-rw-rw-   0        0        0      693 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_reduction/settings/objects/similar_distribution_feature_reduction_settings.py
--rw-rw-rw-   0        0        0      344 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_reduction/settings/objects/stability_feature_reduction_settings.py
--rw-rw-rw-   0        0        0      613 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_reduction/settings/objects/univariate_performance_feature_reduction_settings.py
--rw-rw-rw-   0        0        0      569 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_reduction/settings/objects/user_feature_reduction_settings.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.535596 autonon-0.3.0.post1/organon/ml/feature_selection/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_selection/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.535596 autonon-0.3.0.post1/organon/ml/feature_selection/domain/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_selection/domain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.535596 autonon-0.3.0.post1/organon/ml/feature_selection/domain/enums/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_selection/domain/enums/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.535596 autonon-0.3.0.post1/organon/ml/feature_selection/domain/objects/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_selection/domain/objects/__init__.py
--rw-rw-rw-   0        0        0      229 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_selection/domain/objects/base_selection_output.py
--rw-rw-rw-   0        0        0      227 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_selection/domain/objects/cfs_selection_output.py
--rw-rw-rw-   0        0        0      271 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_selection/domain/objects/feature_similarity_selection_output.py
--rw-rw-rw-   0        0        0      233 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_selection/domain/objects/lasso_selection_output.py
--rw-rw-rw-   0        0        0     1372 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_selection/domain/objects/priority_queue.py
--rw-rw-rw-   0        0        0      235 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_selection/domain/objects/rf_selection_output.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.535596 autonon-0.3.0.post1/organon/ml/feature_selection/domain/objects/settings/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_selection/domain/objects/settings/__init__.py
--rw-rw-rw-   0        0        0      259 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_selection/domain/objects/settings/base_feature_selection_settings.py
--rw-rw-rw-   0        0        0      649 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_selection/domain/objects/settings/base_supervised_feature_selection_settings.py
--rw-rw-rw-   0        0        0      349 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_selection/domain/objects/settings/base_unsupervised_feature_selection_settings.py
--rw-rw-rw-   0        0        0      722 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_selection/domain/objects/settings/cfs_selection_settings.py
--rw-rw-rw-   0        0        0      652 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_selection/domain/objects/settings/feature_similarity_selection_settings.py
--rw-rw-rw-   0        0        0      683 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_selection/domain/objects/settings/lasso_selection_settings.py
--rw-rw-rw-   0        0        0      855 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_selection/domain/objects/settings/rf_selection_settings.py
--rw-rw-rw-   0        0        0      685 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_selection/domain/objects/settings/sweep_selection_settings.py
--rw-rw-rw-   0        0        0      233 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_selection/domain/objects/sweep_selection_output.py
--rw-rw-rw-   0        0        0     8164 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_selection/domain/objects/unsupervised_feature_extractor.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.553830 autonon-0.3.0.post1/organon/ml/feature_selection/domain/services/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_selection/domain/services/__init__.py
--rw-rw-rw-   0        0        0     5980 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_selection/domain/services/base_feature_selection_service.py
--rw-rw-rw-   0        0        0     1811 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_selection/domain/services/base_supervised_feature_selection_service.py
--rw-rw-rw-   0        0        0     1158 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_selection/domain/services/base_unsupervised_feature_selection_service.py
--rw-rw-rw-   0        0        0     4985 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_selection/domain/services/cfs_selection_service.py
--rw-rw-rw-   0        0        0     5701 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_selection/domain/services/feature_similarity_selection_service.py
--rw-rw-rw-   0        0        0     1913 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_selection/domain/services/lasso_selection_service.py
--rw-rw-rw-   0        0        0     2020 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_selection/domain/services/rf_selection_service.py
--rw-rw-rw-   0        0        0     1812 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_selection/domain/services/sweep_selection_service.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.556987 autonon-0.3.0.post1/organon/ml/feature_selection/services/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_selection/services/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.583096 autonon-0.3.0.post1/organon/ml/feature_selection/services/abstractions/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_selection/services/abstractions/__init__.py
--rw-rw-rw-   0        0        0      436 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_selection/services/abstractions/base_feature_selecter.py
--rw-rw-rw-   0        0        0      769 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_selection/services/abstractions/base_supervised_feature_selecter.py
--rw-rw-rw-   0        0        0      326 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_selection/services/abstractions/base_unsupervised_feature_selecter.py
--rw-rw-rw-   0        0        0     1545 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_selection/services/cfs.py
--rw-rw-rw-   0        0        0     1435 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_selection/services/feature_similarity_selection.py
--rw-rw-rw-   0        0        0     1400 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_selection/services/lasso_selection.py
--rw-rw-rw-   0        0        0     1582 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_selection/services/rf_selection.py
--rw-rw-rw-   0        0        0     1282 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/feature_selection/services/sweep_selection.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.583096 autonon-0.3.0.post1/organon/ml/modelling/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.583096 autonon-0.3.0.post1/organon/ml/modelling/algorithms/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/algorithms/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.583096 autonon-0.3.0.post1/organon/ml/modelling/algorithms/classifiers/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/algorithms/classifiers/__init__.py
--rw-rw-rw-   0        0        0     6115 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/algorithms/classifiers/gam_classifier.py
--rw-rw-rw-   0        0        0      433 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/algorithms/classifiers/gbm_classifier.py
--rw-rw-rw-   0        0        0      375 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/algorithms/classifiers/lightgbm_classifier.py
--rw-rw-rw-   0        0        0      435 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/algorithms/classifiers/logistic_regression_classifier.py
--rw-rw-rw-   0        0        0      421 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/algorithms/classifiers/multi_layer_perceptron_classifier.py
--rw-rw-rw-   0        0        0      415 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/algorithms/classifiers/rf_classifier.py
--rw-rw-rw-   0        0        0      563 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/algorithms/classifiers/stacking_ensemble_classifier.py
--rw-rw-rw-   0        0        0     2252 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/algorithms/classifiers/voting_ensemble_classifier.py
--rw-rw-rw-   0        0        0      372 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/algorithms/classifiers/xgboost_classifier.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.583096 autonon-0.3.0.post1/organon/ml/modelling/algorithms/core/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/algorithms/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.598718 autonon-0.3.0.post1/organon/ml/modelling/algorithms/core/abstractions/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/algorithms/core/abstractions/__init__.py
--rw-rw-rw-   0        0        0     1935 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/algorithms/core/abstractions/base_classifier.py
--rw-rw-rw-   0        0        0     6296 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/algorithms/core/abstractions/base_modeller.py
--rw-rw-rw-   0        0        0      842 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/algorithms/core/abstractions/base_regressor.py
--rw-rw-rw-   0        0        0     1979 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/algorithms/core/abstractions/base_sklearn_classifier.py
--rw-rw-rw-   0        0        0     1718 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/algorithms/core/abstractions/base_sklearn_regressor.py
--rw-rw-rw-   0        0        0     6220 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/algorithms/core/abstractions/gam_mixin.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.598718 autonon-0.3.0.post1/organon/ml/modelling/algorithms/core/enums/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/algorithms/core/enums/__init__.py
--rw-rw-rw-   0        0        0     1132 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/algorithms/core/enums/modeller.py
--rw-rw-rw-   0        0        0      174 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/algorithms/core/enums/modeller_type.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.598718 autonon-0.3.0.post1/organon/ml/modelling/algorithms/helpers/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/algorithms/helpers/__init__.py
--rw-rw-rw-   0        0        0     2217 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/algorithms/helpers/ensembling_helper.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.598718 autonon-0.3.0.post1/organon/ml/modelling/algorithms/regressors/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/algorithms/regressors/__init__.py
--rw-rw-rw-   0        0        0     2688 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/algorithms/regressors/gam_regressor.py
--rw-rw-rw-   0        0        0      423 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/algorithms/regressors/gbm_regressor.py
--rw-rw-rw-   0        0        0      359 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/algorithms/regressors/lasso_regressor.py
--rw-rw-rw-   0        0        0      369 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/algorithms/regressors/lightgbm_regressor.py
--rw-rw-rw-   0        0        0      411 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/algorithms/regressors/multi_layer_perceptron_regressor.py
--rw-rw-rw-   0        0        0      405 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/algorithms/regressors/rf_regressor.py
--rw-rw-rw-   0        0        0      358 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/algorithms/regressors/ridge_regressor.py
--rw-rw-rw-   0        0        0      553 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/algorithms/regressors/stacking_ensemble_regressor.py
--rw-rw-rw-   0        0        0     1614 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/algorithms/regressors/voting_ensemble_regressor.py
--rw-rw-rw-   0        0        0      362 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/algorithms/regressors/xgboost_regressor.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.598718 autonon-0.3.0.post1/organon/ml/modelling/algorithms/services/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/algorithms/services/__init__.py
--rw-rw-rw-   0        0        0     2469 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/algorithms/services/algorithm_service.py
--rw-rw-rw-   0        0        0     5915 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/algorithms/services/ml_application_operations.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.598718 autonon-0.3.0.post1/organon/ml/modelling/model_selection/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/model_selection/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.598718 autonon-0.3.0.post1/organon/ml/modelling/model_selection/domain/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/model_selection/domain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.614342 autonon-0.3.0.post1/organon/ml/modelling/model_selection/domain/objects/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/model_selection/domain/objects/__init__.py
--rw-rw-rw-   0        0        0      471 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/model_selection/domain/objects/cross_validation_output.py
--rw-rw-rw-   0        0        0      400 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/model_selection/domain/objects/hpo_output.py
--rw-rw-rw-   0        0        0      590 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/model_selection/domain/objects/selecter_output.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.614342 autonon-0.3.0.post1/organon/ml/modelling/model_selection/domain/services/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/model_selection/domain/services/__init__.py
--rw-rw-rw-   0        0        0     3770 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/model_selection/domain/services/cross_validation_service.py
--rw-rw-rw-   0        0        0    10000 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/model_selection/domain/services/hpo_service.py
--rw-rw-rw-   0        0        0    14376 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/model_selection/domain/services/selection_service.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.614342 autonon-0.3.0.post1/organon/ml/modelling/model_selection/services/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/model_selection/services/__init__.py
--rw-rw-rw-   0        0        0     1490 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/model_selection/services/cross_validation.py
--rw-rw-rw-   0        0        0     2360 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/model_selection/services/hp_optimizer.py
--rw-rw-rw-   0        0        0     1773 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/model_selection/services/selecter.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.614342 autonon-0.3.0.post1/organon/ml/modelling/model_selection/services/user_settings/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/model_selection/services/user_settings/__init__.py
--rw-rw-rw-   0        0        0      595 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/model_selection/services/user_settings/user_hp_optimization_settings.py
--rw-rw-rw-   0        0        0      647 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/model_selection/services/user_settings/user_selection_settings.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.614342 autonon-0.3.0.post1/organon/ml/modelling/model_selection/settings/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/model_selection/settings/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.614342 autonon-0.3.0.post1/organon/ml/modelling/model_selection/settings/enums/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/model_selection/settings/enums/__init__.py
--rw-rw-rw-   0        0        0      219 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/model_selection/settings/enums/search_type.py
--rw-rw-rw-   0        0        0     5849 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/model_selection/settings/model_selection_user_input_service.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.629966 autonon-0.3.0.post1/organon/ml/modelling/model_selection/settings/objects/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/model_selection/settings/objects/__init__.py
--rw-rw-rw-   0        0        0      489 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/model_selection/settings/objects/cross_validation_settings.py
--rw-rw-rw-   0        0        0      750 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/model_selection/settings/objects/hp_optimization_settings.py
--rw-rw-rw-   0        0        0      733 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/modelling/model_selection/settings/objects/selection_settings.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.629966 autonon-0.3.0.post1/organon/ml/object_classification/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/object_classification/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.629966 autonon-0.3.0.post1/organon/ml/object_classification/domain/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/object_classification/domain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.637675 autonon-0.3.0.post1/organon/ml/object_classification/domain/objects/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/object_classification/domain/objects/__init__.py
--rw-rw-rw-   0        0        0      405 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/object_classification/domain/objects/fine_tuning_settings.py
--rw-rw-rw-   0        0        0     2004 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/object_classification/domain/objects/object_clf_settings.py
--rw-rw-rw-   0        0        0      448 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/object_classification/domain/objects/pretrained_model_settings.py
--rw-rw-rw-   0        0        0      432 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/object_classification/domain/objects/transfer_learning_settings.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.638676 autonon-0.3.0.post1/organon/ml/object_classification/domain/services/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/object_classification/domain/services/__init__.py
--rw-rw-rw-   0        0        0      556 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/object_classification/domain/services/object_classification_service.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.639668 autonon-0.3.0.post1/organon/ml/object_classification/services/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/object_classification/services/__init__.py
--rw-rw-rw-   0        0        0     3998 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/object_classification/services/object_classifier.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.640664 autonon-0.3.0.post1/organon/ml/preprocessing/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/preprocessing/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.640664 autonon-0.3.0.post1/organon/ml/preprocessing/domain/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/preprocessing/domain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.641660 autonon-0.3.0.post1/organon/ml/preprocessing/domain/objects/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/preprocessing/domain/objects/__init__.py
--rw-rw-rw-   0        0        0      406 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/preprocessing/domain/objects/coarse_class_fit_output.py
--rw-rw-rw-   0        0        0      559 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/preprocessing/domain/objects/imputation_fit_output.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.643654 autonon-0.3.0.post1/organon/ml/preprocessing/domain/services/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/preprocessing/domain/services/__init__.py
--rw-rw-rw-   0        0        0    32236 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/preprocessing/domain/services/coarse_class_service.py
--rw-rw-rw-   0        0        0     7245 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/preprocessing/domain/services/imputation_service.py
--rw-rw-rw-   0        0        0     5659 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/preprocessing/domain/services/one_hot_encoding_service.py
--rw-rw-rw-   0        0        0     2549 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/preprocessing/domain/services/scaling_service.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.644650 autonon-0.3.0.post1/organon/ml/preprocessing/helpers/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/preprocessing/helpers/__init__.py
--rw-rw-rw-   0        0        0     1476 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/preprocessing/helpers/preprocessing_input_helper.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.648637 autonon-0.3.0.post1/organon/ml/preprocessing/services/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/preprocessing/services/__init__.py
--rw-rw-rw-   0        0        0     6312 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/preprocessing/services/preprocessor.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.650683 autonon-0.3.0.post1/organon/ml/preprocessing/services/user_settings/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/preprocessing/services/user_settings/__init__.py
--rw-rw-rw-   0        0        0      569 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/preprocessing/services/user_settings/coarse_input_dto.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.650683 autonon-0.3.0.post1/organon/ml/preprocessing/settings/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/preprocessing/settings/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.650683 autonon-0.3.0.post1/organon/ml/preprocessing/settings/enums/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/preprocessing/settings/enums/__init__.py
--rw-rw-rw-   0        0        0      178 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/preprocessing/settings/enums/imputer_type.py
--rw-rw-rw-   0        0        0      175 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/preprocessing/settings/enums/scaler_type.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.650683 autonon-0.3.0.post1/organon/ml/preprocessing/settings/objects/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/preprocessing/settings/objects/__init__.py
--rw-rw-rw-   0        0        0      625 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/preprocessing/settings/objects/coarse_class_settings.py
--rw-rw-rw-   0        0        0      668 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/preprocessing/settings/objects/imputation_settings.py
--rw-rw-rw-   0        0        0      217 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/preprocessing/settings/objects/one_hot_encoding_settings.py
--rw-rw-rw-   0        0        0      258 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/preprocessing/settings/objects/scaling_settings.py
--rw-rw-rw-   0        0        0     5911 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/preprocessing/settings/preprocessing_user_input_service.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.650683 autonon-0.3.0.post1/organon/ml/reporting/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/reporting/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.650683 autonon-0.3.0.post1/organon/ml/reporting/domain/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/reporting/domain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.650683 autonon-0.3.0.post1/organon/ml/reporting/domain/objects/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/reporting/domain/objects/__init__.py
--rw-rw-rw-   0        0        0      114 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/reporting/domain/objects/base_report.py
--rw-rw-rw-   0        0        0      426 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/reporting/domain/objects/binary_report.py
--rw-rw-rw-   0        0        0      396 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/reporting/domain/objects/multiclass_report.py
--rw-rw-rw-   0        0        0      339 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/reporting/domain/objects/regression_report.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.650683 autonon-0.3.0.post1/organon/ml/reporting/domain/services/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/reporting/domain/services/__init__.py
--rw-rw-rw-   0        0        0      709 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/reporting/domain/services/base_reporter_service.py
--rw-rw-rw-   0        0        0    13318 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/reporting/domain/services/binary_reporter_service.py
--rw-rw-rw-   0        0        0     3562 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/reporting/domain/services/multiclass_reporter_service.py
--rw-rw-rw-   0        0        0     6896 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/reporting/domain/services/regression_reporter_service.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.650683 autonon-0.3.0.post1/organon/ml/reporting/services/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/reporting/services/__init__.py
--rw-rw-rw-   0        0        0     2053 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/reporting/services/reporter.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.650683 autonon-0.3.0.post1/organon/ml/reporting/settings/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/reporting/settings/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.650683 autonon-0.3.0.post1/organon/ml/reporting/settings/objects/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/reporting/settings/objects/__init__.py
--rw-rw-rw-   0        0        0      414 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/reporting/settings/objects/reporter_settings.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.650683 autonon-0.3.0.post1/organon/ml/sampling/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/sampling/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.650683 autonon-0.3.0.post1/organon/ml/sampling/domain/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/sampling/domain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.650683 autonon-0.3.0.post1/organon/ml/sampling/domain/objects/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/sampling/domain/objects/__init__.py
--rw-rw-rw-   0        0        0      242 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/sampling/domain/objects/sampling_output.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.650683 autonon-0.3.0.post1/organon/ml/sampling/domain/services/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/sampling/domain/services/__init__.py
--rw-rw-rw-   0        0        0     1253 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/sampling/domain/services/sampling_preprocessing_service.py
--rw-rw-rw-   0        0        0    10475 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/sampling/domain/services/sampling_service.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.650683 autonon-0.3.0.post1/organon/ml/sampling/services/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/sampling/services/__init__.py
--rw-rw-rw-   0        0        0     1390 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/sampling/services/sampler.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.667981 autonon-0.3.0.post1/organon/ml/sampling/services/user_settings/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/sampling/services/user_settings/__init__.py
--rw-rw-rw-   0        0        0      470 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/sampling/services/user_settings/user_sampling_settings.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.668980 autonon-0.3.0.post1/organon/ml/sampling/settings/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/sampling/settings/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.669975 autonon-0.3.0.post1/organon/ml/sampling/settings/enums/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/sampling/settings/enums/__init__.py
--rw-rw-rw-   0        0        0      202 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/sampling/settings/enums/sampling_strategy.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:08:47.670971 autonon-0.3.0.post1/organon/ml/sampling/settings/objects/
--rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/sampling/settings/objects/__init__.py
--rw-rw-rw-   0        0        0      624 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/sampling/settings/objects/sampling_settings.py
--rw-rw-rw-   0        0        0     2636 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/organon/ml/sampling/settings/sampling_user_input_service.py
--rw-rw-rw-   0        0        0       84 2022-12-22 11:40:42.000000 autonon-0.3.0.post1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-08 15:08:47.671968 autonon-0.3.0.post1/setup.cfg
--rw-rw-rw-   0        0        0     1817 2023-03-08 15:08:05.000000 autonon-0.3.0.post1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:15.130598 autonon-0.4.0/
+-rw-rw-rw-   0        0        0     1103 2022-12-22 11:40:42.000000 autonon-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0      189 2022-12-22 11:40:42.000000 autonon-0.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3744 2023-06-02 14:56:15.130598 autonon-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3249 2023-06-02 14:50:05.000000 autonon-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.128027 autonon-0.4.0/autonon.egg-info/
+-rw-rw-rw-   0        0        0     3744 2023-06-02 14:56:12.000000 autonon-0.4.0/autonon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    39035 2023-06-02 14:56:13.000000 autonon-0.4.0/autonon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 14:56:12.000000 autonon-0.4.0/autonon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      431 2023-06-02 14:56:12.000000 autonon-0.4.0/autonon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-02 14:56:12.000000 autonon-0.4.0/autonon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1231 2022-12-22 11:40:42.000000 autonon-0.4.0/cython_setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.128027 autonon-0.4.0/organon/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.128027 autonon-0.4.0/organon/afe/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.128027 autonon-0.4.0/organon/afe/core/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.143674 autonon-0.4.0/organon/afe/core/businessobjects/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/core/businessobjects/__init__.py
+-rw-rw-rw-   0        0        0     2399 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/core/businessobjects/afe_static_objects.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.163095 autonon-0.4.0/organon/afe/data/
+-rw-rw-rw-   0        0        0      913 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/data/__init__.py
+-rw-rw-rw-   0        0        0      289 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/afe/data/base_df.zip
+-rw-rw-rw-   0        0        0     8119 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/afe/data/cash_df.zip
+-rw-rw-rw-   0        0        0      266 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/afe/data/score_df.zip
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.163095 autonon-0.4.0/organon/afe/dataaccess/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/dataaccess/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.163095 autonon-0.4.0/organon/afe/dataaccess/helpers/
+-rw-rw-rw-   0        0        0        0 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/afe/dataaccess/helpers/__init__.py
+-rw-rw-rw-   0        0        0      571 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/afe/dataaccess/helpers/record_source_helper.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.178744 autonon-0.4.0/organon/afe/dataaccess/services/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/dataaccess/services/__init__.py
+-rw-rw-rw-   0        0        0     1456 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/dataaccess/services/base_record_reader.py
+-rw-rw-rw-   0        0        0      304 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/dataaccess/services/i_sample_data_service.py
+-rw-rw-rw-   0        0        0     5474 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/dataaccess/services/sample_data_service.py
+-rw-rw-rw-   0        0        0     4089 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/dataaccess/services/sample_data_service_helper.py
+-rw-rw-rw-   0        0        0     9197 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/afe/dataaccess/services/target_file_record_repository.py
+-rw-rw-rw-   0        0        0    23096 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/afe/dataaccess/services/transaction_file_record_reader.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.178744 autonon-0.4.0/organon/afe/domain/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.210001 autonon-0.4.0/organon/afe/domain/common/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/common/__init__.py
+-rw-rw-rw-   0        0        0     3021 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/common/afe_date_helper.py
+-rw-rw-rw-   0        0        0     7855 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/common/base_execution_plan_service.py
+-rw-rw-rw-   0        0        0     9568 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/common/persist_helper.py
+-rw-rw-rw-   0        0        0     4508 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/common/reader_helper.py
+-rw-rw-rw-   0        0        0     3135 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/common/runtime_stats_service.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.241222 autonon-0.4.0/organon/afe/domain/enums/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/enums/__init__.py
+-rw-rw-rw-   0        0        0      447 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/enums/afe_date_column_encoding_type.py
+-rw-rw-rw-   0        0        0      268 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/enums/afe_date_column_type.py
+-rw-rw-rw-   0        0        0      261 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/enums/afe_learning_type.py
+-rw-rw-rw-   0        0        0      980 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/enums/afe_operator.py
+-rw-rw-rw-   0        0        0      252 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/enums/afe_target_column_type.py
+-rw-rw-rw-   0        0        0      286 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/enums/binary_target_class.py
+-rw-rw-rw-   0        0        0      273 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/enums/date_resolution.py
+-rw-rw-rw-   0        0        0      216 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/enums/record_source_type.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.256875 autonon-0.4.0/organon/afe/domain/modelling/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/modelling/__init__.py
+-rw-rw-rw-   0        0        0    36067 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/modelling/abstract_modelling_service.py
+-rw-rw-rw-   0        0        0     6903 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/modelling/auto_column_type_decider_service.py
+-rw-rw-rw-   0        0        0     7224 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/modelling/base_modelling_service.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.327782 autonon-0.4.0/organon/afe/domain/modelling/businessobjects/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/modelling/businessobjects/__init__.py
+-rw-rw-rw-   0        0        0     4335 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/modelling/businessobjects/afe_column.py
+-rw-rw-rw-   0        0        0      293 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/modelling/businessobjects/afe_feature.py
+-rw-rw-rw-   0        0        0      444 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/modelling/businessobjects/base_afe_feature.py
+-rw-rw-rw-   0        0        0     4765 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/modelling/businessobjects/bin_info.py
+-rw-rw-rw-   0        0        0    29362 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/modelling/businessobjects/data_frame_builder.py
+-rw-rw-rw-   0        0        0     3746 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/modelling/businessobjects/multi_target_entity_container.py
+-rw-rw-rw-   0        0        0      503 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/modelling/businessobjects/target_file_record.py
+-rw-rw-rw-   0        0        0     4584 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/modelling/businessobjects/target_file_record_collection.py
+-rw-rw-rw-   0        0        0     1081 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/modelling/businessobjects/transaction_file_record.py
+-rw-rw-rw-   0        0        0     4210 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/modelling/businessobjects/transaction_file_record_collection.py
+-rw-rw-rw-   0        0        0     1546 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/modelling/businessobjects/transaction_file_stats.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.334036 autonon-0.4.0/organon/afe/domain/modelling/helper/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/modelling/helper/__init__.py
+-rw-rw-rw-   0        0        0    30343 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/modelling/helper/data_frame_builder_helper.pyx
+-rw-rw-rw-   0        0        0     3059 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/modelling/helper/trx_reader_helper.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.353900 autonon-0.4.0/organon/afe/domain/modelling/supervised/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/modelling/supervised/__init__.py
+-rw-rw-rw-   0        0        0     1119 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/modelling/supervised/afe_supervised_algorithm_settings.py
+-rw-rw-rw-   0        0        0     2336 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/modelling/supervised/multi_target_entity_container_service.py
+-rw-rw-rw-   0        0        0    13567 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/modelling/supervised/multi_target_modelling_helper.py
+-rw-rw-rw-   0        0        0     2812 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/modelling/supervised/multi_target_modelling_service.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.353900 autonon-0.4.0/organon/afe/domain/modelling/unsupervised/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/modelling/unsupervised/__init__.py
+-rw-rw-rw-   0        0        0      964 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/afe/domain/modelling/unsupervised/afe_unsupervised_algorithm_settings.py
+-rw-rw-rw-   0        0        0     1331 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/modelling/unsupervised/unsupervised_feature_extraction_service.py
+-rw-rw-rw-   0        0        0     1330 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/afe/domain/modelling/unsupervised/unsupervised_modelling_helper.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.432032 autonon-0.4.0/organon/afe/domain/reporting/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/reporting/__init__.py
+-rw-rw-rw-   0        0        0     7776 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/reporting/abstract_report_helper.py
+-rw-rw-rw-   0        0        0      517 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/reporting/afe_column_dto.py
+-rw-rw-rw-   0        0        0     2873 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/reporting/afe_matplotlib_report_helper.py
+-rw-rw-rw-   0        0        0      322 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/reporting/afe_model_output.py
+-rw-rw-rw-   0        0        0      334 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/reporting/afe_output_report.py
+-rw-rw-rw-   0        0        0     2499 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/reporting/afe_plotly_report_helper.py
+-rw-rw-rw-   0        0        0     1570 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/reporting/base_afe_model_output.py
+-rw-rw-rw-   0        0        0     1567 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/reporting/base_afe_output_report.py
+-rw-rw-rw-   0        0        0     1554 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/reporting/base_report_helper.py
+-rw-rw-rw-   0        0        0     8397 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/reporting/dashboard_helper.py
+-rw-rw-rw-   0        0        0    16863 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/reporting/matplotlib_common_functions.py
+-rw-rw-rw-   0        0        0     6433 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/reporting/plotly_common_functions.py
+-rw-rw-rw-   0        0        0     7667 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/reporting/plotly_dashboard_helper.py
+-rw-rw-rw-   0        0        0      487 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/reporting/runtime_statistics.py
+-rw-rw-rw-   0        0        0     2668 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/reporting/transformation.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.432032 autonon-0.4.0/organon/afe/domain/scoring/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/scoring/__init__.py
+-rw-rw-rw-   0        0        0    17479 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/scoring/afe_scoring_service.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.570474 autonon-0.4.0/organon/afe/domain/settings/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/settings/__init__.py
+-rw-rw-rw-   0        0        0      552 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/settings/afe_algorithm_settings.py
+-rw-rw-rw-   0        0        0      683 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/settings/afe_data_settings.py
+-rw-rw-rw-   0        0        0     1049 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/settings/afe_date_column.py
+-rw-rw-rw-   0        0        0      661 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/settings/afe_modelling_settings.py
+-rw-rw-rw-   0        0        0     1852 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/settings/afe_output_settings.py
+-rw-rw-rw-   0        0        0      728 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/settings/afe_process_settings.py
+-rw-rw-rw-   0        0        0      448 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/settings/afe_reading_settings.py
+-rw-rw-rw-   0        0        0      465 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/settings/afe_scoring_settings.py
+-rw-rw-rw-   0        0        0     1397 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/afe/domain/settings/afe_settings_reader.py
+-rw-rw-rw-   0        0        0    11298 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/settings/afe_settings_type_validators.py
+-rw-rw-rw-   0        0        0    35269 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/settings/afe_settings_validator.py
+-rw-rw-rw-   0        0        0      806 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/settings/afe_target_column.py
+-rw-rw-rw-   0        0        0     1066 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/settings/auto_column_decider_settings.py
+-rw-rw-rw-   0        0        0     2165 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/settings/base_afe_data_settings.py
+-rw-rw-rw-   0        0        0     2847 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/settings/base_afe_modelling_settings.py
+-rw-rw-rw-   0        0        0     1383 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/settings/base_afe_scoring_settings.py
+-rw-rw-rw-   0        0        0      306 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/settings/base_afe_settings.py
+-rw-rw-rw-   0        0        0    26957 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/afe/domain/settings/base_afe_settings_reader.py
+-rw-rw-rw-   0        0        0     1064 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/settings/base_trx_descriptor.py
+-rw-rw-rw-   0        0        0     1025 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/settings/binary_target.py
+-rw-rw-rw-   0        0        0      815 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/settings/db_object_input.py
+-rw-rw-rw-   0        0        0     1507 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/afe/domain/settings/feature_generation_settings.py
+-rw-rw-rw-   0        0        0      589 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/settings/model_settings.py
+-rw-rw-rw-   0        0        0      814 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/settings/modelling_reduction_settings.py
+-rw-rw-rw-   0        0        0     1374 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/settings/record_source.py
+-rw-rw-rw-   0        0        0     1119 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/settings/target_descriptor.py
+-rw-rw-rw-   0        0        0      539 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/settings/temporal_grid.py
+-rw-rw-rw-   0        0        0     1179 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/settings/trx_descriptor.py
+-rw-rw-rw-   0        0        0     3391 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/domain/settings/validation_helper.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.570474 autonon-0.4.0/organon/afe/services/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/afe/services/__init__.py
+-rw-rw-rw-   0        0        0     1196 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/afe/services/afe_application_operations.py
+-rw-rw-rw-   0        0        0    36491 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/afe/services/afe_executor.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.570474 autonon-0.4.0/organon/common/
+-rw-rw-rw-   0        0        0        0 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.570474 autonon-0.4.0/organon/common/helpers/
+-rw-rw-rw-   0        0        0        0 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/common/helpers/__init__.py
+-rw-rw-rw-   0        0        0      884 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/common/helpers/dev_mode_helper.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.570474 autonon-0.4.0/organon/fl/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.570474 autonon-0.4.0/organon/fl/core/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.632975 autonon-0.4.0/organon/fl/core/businessobjects/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/businessobjects/__init__.py
+-rw-rw-rw-   0        0        0     1212 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/fl/core/businessobjects/dask_dataframe.py
+-rw-rw-rw-   0        0        0     2676 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/businessobjects/data_partition.py
+-rw-rw-rw-   0        0        0     2690 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/businessobjects/dataframe.py
+-rw-rw-rw-   0        0        0     4940 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/businessobjects/date_interval.py
+-rw-rw-rw-   0        0        0     3151 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/businessobjects/dict_dataframe.py
+-rw-rw-rw-   0        0        0     1115 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/businessobjects/fl_core_static_objects.py
+-rw-rw-rw-   0        0        0     8893 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/businessobjects/histogram_16.py
+-rw-rw-rw-   0        0        0     1680 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/businessobjects/idata_partition.py
+-rw-rw-rw-   0        0        0     2080 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/businessobjects/idataframe.py
+-rw-rw-rw-   0        0        0     5123 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/businessobjects/np2d_dataframe.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.632975 autonon-0.4.0/organon/fl/core/collections/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/collections/__init__.py
+-rw-rw-rw-   0        0        0      946 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/collections/pair.py
+-rw-rw-rw-   0        0        0     1252 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/collections/sorted_dict.py
+-rw-rw-rw-   0        0        0      815 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/collections/sorted_list.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.664224 autonon-0.4.0/organon/fl/core/enums/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/enums/__init__.py
+-rw-rw-rw-   0        0        0      290 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/enums/column_measurement_type.py
+-rw-rw-rw-   0        0        0      278 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/enums/column_native_type.py
+-rw-rw-rw-   0        0        0      268 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/enums/date_interval_type.py
+-rw-rw-rw-   0        0        0      256 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/enums/datetime_token.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.664224 autonon-0.4.0/organon/fl/core/exceptionhandling/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/exceptionhandling/__init__.py
+-rw-rw-rw-   0        0        0      170 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/exceptionhandling/known_exception.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.676429 autonon-0.4.0/organon/fl/core/executionutil/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/executionutil/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.684316 autonon-0.4.0/organon/fl/core/executionutil/objects/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/executionutil/objects/__init__.py
+-rw-rw-rw-   0        0        0      413 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/executionutil/objects/locked_iterator.py
+-rw-rw-rw-   0        0        0     1471 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/executionutil/objects/stopwatch.py
+-rw-rw-rw-   0        0        0     2785 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/executionutil/parallel_execution_helper.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.684316 autonon-0.4.0/organon/fl/core/extensions/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/extensions/__init__.py
+-rw-rw-rw-   0        0        0     3730 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/extensions/string_extensions.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.699346 autonon-0.4.0/organon/fl/core/fileoperations/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/fileoperations/__init__.py
+-rw-rw-rw-   0        0        0     1424 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/fl/core/fileoperations/directory_helper.py
+-rw-rw-rw-   0        0        0     2885 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/fileoperations/file_io_helper.py
+-rw-rw-rw-   0        0        0      186 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/fileoperations/file_read_options.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.762445 autonon-0.4.0/organon/fl/core/helpers/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/helpers/__init__.py
+-rw-rw-rw-   0        0        0      586 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/helpers/boolean_helper.py
+-rw-rw-rw-   0        0        0     6745 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/helpers/data_frame_helper.py
+-rw-rw-rw-   0        0        0     5252 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/helpers/date_helper.py
+-rw-rw-rw-   0        0        0     1119 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/helpers/dict_helper.py
+-rw-rw-rw-   0        0        0      818 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/helpers/enums_helpers.py
+-rw-rw-rw-   0        0        0     4309 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/helpers/environment_info_helper.py
+-rw-rw-rw-   0        0        0     1111 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/helpers/float_helper.py
+-rw-rw-rw-   0        0        0      657 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/helpers/function_helper.py
+-rw-rw-rw-   0        0        0      525 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/helpers/guid_helper.py
+-rw-rw-rw-   0        0        0     1107 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/helpers/list_helper.py
+-rw-rw-rw-   0        0        0     2787 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/fl/core/helpers/object_helper.py
+-rw-rw-rw-   0        0        0     1585 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/helpers/process_info_helper.py
+-rw-rw-rw-   0        0        0     6339 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/helpers/string_helper.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.762445 autonon-0.4.0/organon/fl/core/iocutil/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/iocutil/__init__.py
+-rw-rw-rw-   0        0        0     2528 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/iocutil/ioc_helper.py
+-rw-rw-rw-   0        0        0      402 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/core/iocutil/ioc_registration_item.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.762445 autonon-0.4.0/organon/fl/generic/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/generic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.778061 autonon-0.4.0/organon/fl/generic/datadtos/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/generic/datadtos/__init__.py
+-rw-rw-rw-   0        0        0      289 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/generic/datadtos/environment_info_dto.py
+-rw-rw-rw-   0        0        0      291 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/generic/datadtos/process_info_dto.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.778061 autonon-0.4.0/organon/fl/generic/enums/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/generic/enums/__init__.py
+-rw-rw-rw-   0        0        0      225 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/generic/enums/os_type_id.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.778061 autonon-0.4.0/organon/fl/generic/interaction/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/generic/interaction/__init__.py
+-rw-rw-rw-   0        0        0     1043 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/fl/generic/interaction/fl_initializer.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.778061 autonon-0.4.0/organon/fl/logging/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/logging/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.778061 autonon-0.4.0/organon/fl/logging/helpers/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/logging/helpers/__init__.py
+-rw-rw-rw-   0        0        0    11888 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/fl/logging/helpers/log_helper.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.793656 autonon-0.4.0/organon/fl/mathematics/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/mathematics/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.793656 autonon-0.4.0/organon/fl/mathematics/businessobjects/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/mathematics/businessobjects/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.809311 autonon-0.4.0/organon/fl/mathematics/businessobjects/sets/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/mathematics/businessobjects/sets/__init__.py
+-rw-rw-rw-   0        0        0     3977 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/mathematics/businessobjects/sets/interval.py
+-rw-rw-rw-   0        0        0     1489 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/mathematics/businessobjects/sets/sum_triple.py
+-rw-rw-rw-   0        0        0     1549 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/mathematics/businessobjects/tuple_generic_collection.py
+-rw-rw-rw-   0        0        0      259 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/mathematics/constants.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.809311 autonon-0.4.0/organon/fl/mathematics/enums/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/mathematics/enums/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.809311 autonon-0.4.0/organon/fl/mathematics/enums/sets/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/mathematics/enums/sets/__init__.py
+-rw-rw-rw-   0        0        0      235 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/mathematics/enums/sets/interval_type.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.824931 autonon-0.4.0/organon/fl/mathematics/helpers/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/mathematics/helpers/__init__.py
+-rw-rw-rw-   0        0        0     2323 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/fl/mathematics/helpers/dask_dataframe_operations.py
+-rw-rw-rw-   0        0        0     1192 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/fl/mathematics/helpers/dataframe_operations_factory.py
+-rw-rw-rw-   0        0        0     2337 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/mathematics/helpers/dict_dataframe_operations.py
+-rw-rw-rw-   0        0        0     3266 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/mathematics/helpers/idataframe_operations.py
+-rw-rw-rw-   0        0        0     4863 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/mathematics/helpers/pandas_dataframe_operations.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.860215 autonon-0.4.0/organon/fl/mathematics/linearalgebra/
+-rw-rw-rw-   0        0        0    16750 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/mathematics/linearalgebra/IBlas.py
+-rw-rw-rw-   0        0        0    75446 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/mathematics/linearalgebra/MklFunctions.py
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/mathematics/linearalgebra/__init__.py
+-rw-rw-rw-   0        0        0      969 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/mathematics/linearalgebra/blas_service_factory.py
+-rw-rw-rw-   0        0        0      179 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/mathematics/linearalgebra/blas_service_type.py
+-rw-rw-rw-   0        0        0     1583 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/mathematics/linearalgebra/enums.py
+-rw-rw-rw-   0        0        0    16853 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/mathematics/linearalgebra/scipy_blas_service.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.891496 autonon-0.4.0/organon/fl/mathematics/sweep/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/mathematics/sweep/__init__.py
+-rw-rw-rw-   0        0        0     6638 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/mathematics/sweep/covariance_generator.py
+-rw-rw-rw-   0        0        0     5050 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/mathematics/sweep/covariance_info.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.922715 autonon-0.4.0/organon/fl/mathematics/sweep/data_classes/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/mathematics/sweep/data_classes/__init__.py
+-rw-rw-rw-   0        0        0      758 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/mathematics/sweep/data_classes/linear_regression_algorithm_settings.py
+-rw-rw-rw-   0        0        0      396 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/mathematics/sweep/data_classes/linear_regression_parameter.py
+-rw-rw-rw-   0        0        0     2541 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/mathematics/sweep/data_classes/linear_regression_results.py
+-rw-rw-rw-   0        0        0      847 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/mathematics/sweep/data_classes/linear_regression_step.py
+-rw-rw-rw-   0        0        0     1378 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/mathematics/sweep/data_classes/selected_attribute.py
+-rw-rw-rw-   0        0        0      336 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/mathematics/sweep/data_classes/swept_attribute.py
+-rw-rw-rw-   0        0        0      355 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/mathematics/sweep/data_classes/transformation.py
+-rw-rw-rw-   0        0        0      597 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/mathematics/sweep/enums.py
+-rw-rw-rw-   0        0        0    25509 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/mathematics/sweep/fast_model_builder.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.938367 autonon-0.4.0/organon/fl/mathematics/sweep/matrices/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/mathematics/sweep/matrices/__init__.py
+-rw-rw-rw-   0        0        0     4895 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/mathematics/sweep/matrices/csc_matrix.py
+-rw-rw-rw-   0        0        0     1682 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/mathematics/sweep/matrices/dense_matrix.py
+-rw-rw-rw-   0        0        0      971 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/mathematics/sweep/matrices/i_matrix.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.938367 autonon-0.4.0/organon/fl/mathematics/sweep/pyx_files/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/mathematics/sweep/pyx_files/__init__.py
+-rw-rw-rw-   0        0        0     7951 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/mathematics/sweep/pyx_files/sweep_helper.pyx
+-rw-rw-rw-   0        0        0    14453 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/mathematics/sweep/sweep_operator.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.938367 autonon-0.4.0/organon/fl/modelling/
+-rw-rw-rw-   0        0        0        0 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/fl/modelling/__init__.py
+-rw-rw-rw-   0        0        0     8259 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/fl/modelling/unsupervised_feature_extractor.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.938367 autonon-0.4.0/organon/fl/security/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/security/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.938367 autonon-0.4.0/organon/fl/security/helpers/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/security/helpers/__init__.py
+-rw-rw-rw-   0        0        0     3637 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/security/helpers/encryption_helper.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.953966 autonon-0.4.0/organon/fl/serialization/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/serialization/__init__.py
+-rw-rw-rw-   0        0        0     1538 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/fl/serialization/serialization_helper.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.953966 autonon-0.4.0/organon/idq/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.953966 autonon-0.4.0/organon/idq/core/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/core/__init__.py
+-rw-rw-rw-   0        0        0     1890 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/core/dq_constants.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.969591 autonon-0.4.0/organon/idq/core/enums/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/core/enums/__init__.py
+-rw-rw-rw-   0        0        0      162 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/core/enums/data_entity_type.py
+-rw-rw-rw-   0        0        0     2520 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/core/enums/dq_comparison_result_code.py
+-rw-rw-rw-   0        0        0      263 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/core/enums/dq_task_type.py
+-rw-rw-rw-   0        0        0     1100 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/core/enums/dq_test_type.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.985217 autonon-0.4.0/organon/idq/core/helpers/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/core/helpers/__init__.py
+-rw-rw-rw-   0        0        0      413 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/core/helpers/formatting_helper.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.985217 autonon-0.4.0/organon/idq/dataaccess/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/dataaccess/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:13.985217 autonon-0.4.0/organon/idq/dataaccess/abstractions/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/dataaccess/abstractions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.000865 autonon-0.4.0/organon/idq/dataaccess/helpers/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/dataaccess/helpers/__init__.py
+-rw-rw-rw-   0        0        0     6807 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/dataaccess/helpers/record_source_filter_helper.py
+-rw-rw-rw-   0        0        0     7873 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/dataaccess/record_source_reader.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.000865 autonon-0.4.0/organon/idq/domain/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.000865 autonon-0.4.0/organon/idq/domain/algorithms/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/algorithms/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.016465 autonon-0.4.0/organon/idq/domain/algorithms/objects/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/algorithms/objects/__init__.py
+-rw-rw-rw-   0        0        0      570 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/algorithms/objects/base_comparison_input.py
+-rw-rw-rw-   0        0        0      584 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/algorithms/objects/mean_ci_comparison_input.py
+-rw-rw-rw-   0        0        0      787 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/algorithms/objects/time_series_comparison_input.py
+-rw-rw-rw-   0        0        0      616 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/algorithms/objects/traffic_light_comparison_input.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.051763 autonon-0.4.0/organon/idq/domain/businessobjects/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/businessobjects/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.067388 autonon-0.4.0/organon/idq/domain/businessobjects/data_column/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/businessobjects/data_column/__init__.py
+-rw-rw-rw-   0        0        0      757 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/businessobjects/data_column/dq_data_column.py
+-rw-rw-rw-   0        0        0      360 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/businessobjects/data_column/dq_df_data_column.py
+-rw-rw-rw-   0        0        0      356 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/businessobjects/data_column/dq_file_data_column.py
+-rw-rw-rw-   0        0        0      528 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/businessobjects/dq_calculation_output.py
+-rw-rw-rw-   0        0        0      824 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/idq/domain/businessobjects/dq_calculation_result.py
+-rw-rw-rw-   0        0        0     2066 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/businessobjects/dq_comparison_result.py
+-rw-rw-rw-   0        0        0     2131 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/businessobjects/dq_control_parameters.py
+-rw-rw-rw-   0        0        0     1852 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/businessobjects/dq_data_column_collection.py
+-rw-rw-rw-   0        0        0      278 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/businessobjects/dq_data_source.py
+-rw-rw-rw-   0        0        0      172 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/businessobjects/dq_settings.py
+-rw-rw-rw-   0        0        0      312 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/businessobjects/dq_test_group.py
+-rw-rw-rw-   0        0        0      266 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/businessobjects/main_sample_results.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.083013 autonon-0.4.0/organon/idq/domain/businessobjects/record_sources/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/businessobjects/record_sources/__init__.py
+-rw-rw-rw-   0        0        0      805 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/businessobjects/record_sources/dq_base_record_source.py
+-rw-rw-rw-   0        0        0      663 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/businessobjects/record_sources/dq_df_record_source.py
+-rw-rw-rw-   0        0        0      586 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/businessobjects/record_sources/dq_file_record_source.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.114262 autonon-0.4.0/organon/idq/domain/businessobjects/statistics/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/businessobjects/statistics/__init__.py
+-rw-rw-rw-   0        0        0      329 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/businessobjects/statistics/data_source_statistics.py
+-rw-rw-rw-   0        0        0      250 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/businessobjects/statistics/dq_base_statistics.py
+-rw-rw-rw-   0        0        0     1360 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/businessobjects/statistics/dq_categorical_statistics.py
+-rw-rw-rw-   0        0        0      889 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/businessobjects/statistics/dq_population_numerical_statistics.py
+-rw-rw-rw-   0        0        0     2442 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/businessobjects/statistics/dq_sample_numerical_statistics.py
+-rw-rw-rw-   0        0        0      547 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/businessobjects/statistics/population_statistics.py
+-rw-rw-rw-   0        0        0      510 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/businessobjects/statistics/sample_statistics.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.177126 autonon-0.4.0/organon/idq/domain/controls/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/controls/__init__.py
+-rw-rw-rw-   0        0        0     2267 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/controls/base_dq_control.py
+-rw-rw-rw-   0        0        0     7345 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/controls/base_psi_signal_control.py
+-rw-rw-rw-   0        0        0     7491 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/controls/column_mean_control.py
+-rw-rw-rw-   0        0        0     4030 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/controls/data_source_stats_time_series_control.py
+-rw-rw-rw-   0        0        0     4221 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/controls/data_source_stats_traffic_light_control.py
+-rw-rw-rw-   0        0        0     3282 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/controls/duplicate_keys_control.py
+-rw-rw-rw-   0        0        0     1958 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/controls/empty_table_control.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.208440 autonon-0.4.0/organon/idq/domain/controls/helpers/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/controls/helpers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.211560 autonon-0.4.0/organon/idq/domain/controls/helpers/algorithms/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/controls/helpers/algorithms/__init__.py
+-rw-rw-rw-   0        0        0     1768 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/controls/helpers/algorithms/base_predictor.py
+-rw-rw-rw-   0        0        0      311 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/controls/helpers/algorithms/prediction_result.py
+-rw-rw-rw-   0        0        0      595 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/controls/helpers/algorithms/predictor_factory.py
+-rw-rw-rw-   0        0        0     1828 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/controls/helpers/algorithms/random_forest_predictor.py
+-rw-rw-rw-   0        0        0     1660 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/controls/helpers/column_values_comparer.py
+-rw-rw-rw-   0        0        0     2138 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/controls/helpers/comparison_helper_functions.py
+-rw-rw-rw-   0        0        0     1213 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/controls/helpers/psi_comparer.py
+-rw-rw-rw-   0        0        0    19586 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/controls/helpers/traffic_light_comparer.py
+-rw-rw-rw-   0        0        0     5023 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/controls/psi_nominal_signal_control.py
+-rw-rw-rw-   0        0        0     9512 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/controls/psi_numeric_signal_control.py
+-rw-rw-rw-   0        0        0    13421 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/controls/stable_column_control.py
+-rw-rw-rw-   0        0        0     8096 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/controls/table_columns_control.py
+-rw-rw-rw-   0        0        0     4365 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/controls/unexpected_nominal_values_control.py
+-rw-rw-rw-   0        0        0     5416 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/controls/unexpected_numerical_values_control.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.242840 autonon-0.4.0/organon/idq/domain/enums/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/enums/__init__.py
+-rw-rw-rw-   0        0        0      520 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/enums/dq_control_type.py
+-rw-rw-rw-   0        0        0      200 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/enums/dq_pred_algorithm_type.py
+-rw-rw-rw-   0        0        0      223 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/enums/dq_record_source_type.py
+-rw-rw-rw-   0        0        0      215 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/enums/dq_run_type.py
+-rw-rw-rw-   0        0        0      354 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/enums/dq_test_group_type.py
+-rw-rw-rw-   0        0        0      185 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/enums/signal_type.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.242840 autonon-0.4.0/organon/idq/domain/helpers/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/helpers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.258436 autonon-0.4.0/organon/idq/domain/helpers/statistics/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/helpers/statistics/__init__.py
+-rw-rw-rw-   0        0        0     5986 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/helpers/statistics/dq_statistical_functions.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.274062 autonon-0.4.0/organon/idq/domain/reporting/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/reporting/__init__.py
+-rw-rw-rw-   0        0        0     5309 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/reporting/base_dq_report_helper.py
+-rw-rw-rw-   0        0        0    14789 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/reporting/base_multiple_calculation_report_helper.py
+-rw-rw-rw-   0        0        0     6963 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/reporting/dq_reporting_executor.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.274062 autonon-0.4.0/organon/idq/domain/reporting/enum/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/reporting/enum/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.274062 autonon-0.4.0/organon/idq/domain/reporting/helpers/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/reporting/helpers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.352187 autonon-0.4.0/organon/idq/domain/reporting/objects/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/reporting/objects/__init__.py
+-rw-rw-rw-   0        0        0      960 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/reporting/objects/base_alert_info.py
+-rw-rw-rw-   0        0        0      622 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/reporting/objects/base_dq_output_report.py
+-rw-rw-rw-   0        0        0     1036 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/reporting/objects/base_dq_report_helper_params.py
+-rw-rw-rw-   0        0        0     1199 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/reporting/objects/base_multiple_calculation_report_helper_params.py
+-rw-rw-rw-   0        0        0     1182 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/reporting/objects/dq_comparison_sample_report_input.py
+-rw-rw-rw-   0        0        0      883 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/reporting/objects/nominal_column_control_details.py
+-rw-rw-rw-   0        0        0      886 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/reporting/objects/numeric_column_control_details.py
+-rw-rw-rw-   0        0        0      581 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/reporting/objects/signal_details.py
+-rw-rw-rw-   0        0        0      213 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/reporting/objects/single_source_alert_info.py
+-rw-rw-rw-   0        0        0      269 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/reporting/objects/single_source_report_helper_params.py
+-rw-rw-rw-   0        0        0      239 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/reporting/objects/single_source_report_output.py
+-rw-rw-rw-   0        0        0      820 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/reporting/objects/source_with_partitions_alert_info.py
+-rw-rw-rw-   0        0        0      527 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/reporting/objects/source_with_partitions_dq_report_output.py
+-rw-rw-rw-   0        0        0     1069 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/reporting/objects/source_with_partitions_report_helper_params.py
+-rw-rw-rw-   0        0        0      753 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/reporting/objects/table_control_details.py
+-rw-rw-rw-   0        0        0     3085 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/reporting/single_source_report_helper.py
+-rw-rw-rw-   0        0        0     3786 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/reporting/source_with_partitions_report_helper.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.381838 autonon-0.4.0/organon/idq/domain/services/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/services/__init__.py
+-rw-rw-rw-   0        0        0    20865 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/services/base_user_input_service.py
+-rw-rw-rw-   0        0        0     8866 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/services/base_user_input_validation_service.py
+-rw-rw-rw-   0        0        0     8049 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/idq/domain/services/dq_full_process_executor.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.387273 autonon-0.4.0/organon/idq/domain/services/output/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/services/output/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.402929 autonon-0.4.0/organon/idq/domain/services/output/calculation/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/services/output/calculation/__init__.py
+-rw-rw-rw-   0        0        0      187 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/services/output/calculation/db_source_stats_output_service.py
+-rw-rw-rw-   0        0        0      187 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/services/output/calculation/df_source_stats_output_service.py
+-rw-rw-rw-   0        0        0      189 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/services/output/calculation/file_source_stats_output_service.py
+-rw-rw-rw-   0        0        0      233 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/services/output/calculation/stats_output_service.py
+-rw-rw-rw-   0        0        0      914 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/services/output/dq_output_persistence_service.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.402929 autonon-0.4.0/organon/idq/domain/services/statistics/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/services/statistics/__init__.py
+-rw-rw-rw-   0        0        0     7565 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/services/statistics/dq_statistics_domain_service.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.418527 autonon-0.4.0/organon/idq/domain/services/statistics/source_statistics/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/services/statistics/source_statistics/__init__.py
+-rw-rw-rw-   0        0        0     3879 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/services/statistics/source_statistics/df_source_stats_service.py
+-rw-rw-rw-   0        0        0     8784 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/idq/domain/services/statistics/source_statistics/dq_source_stats_base_service.py
+-rw-rw-rw-   0        0        0     4783 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/services/statistics/source_statistics/file_source_stats_service.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.418527 autonon-0.4.0/organon/idq/domain/services/task_executor/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/services/task_executor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.418527 autonon-0.4.0/organon/idq/domain/services/task_executor/calculation/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/services/task_executor/calculation/__init__.py
+-rw-rw-rw-   0        0        0     6236 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/idq/domain/services/task_executor/calculation/dq_calculation_task_executor.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.418527 autonon-0.4.0/organon/idq/domain/services/task_executor/comparison/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/services/task_executor/comparison/__init__.py
+-rw-rw-rw-   0        0        0     5237 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/services/task_executor/comparison/dq_comparison_task_executor.py
+-rw-rw-rw-   0        0        0     1885 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/services/user_input_service.py
+-rw-rw-rw-   0        0        0     1322 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/services/user_input_validation_service.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.449777 autonon-0.4.0/organon/idq/domain/settings/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/settings/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.465400 autonon-0.4.0/organon/idq/domain/settings/abstractions/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/settings/abstractions/__init__.py
+-rw-rw-rw-   0        0        0     1213 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/settings/abstractions/dq_base_calculation_parameters.py
+-rw-rw-rw-   0        0        0      998 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/settings/abstractions/dq_base_comparison_parameters.py
+-rw-rw-rw-   0        0        0      951 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/settings/abstractions/dq_base_input_source_settings.py
+-rw-rw-rw-   0        0        0     1120 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/idq/domain/settings/abstractions/dq_full_process_input.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.481027 autonon-0.4.0/organon/idq/domain/settings/calculation/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/settings/calculation/__init__.py
+-rw-rw-rw-   0        0        0      425 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/settings/calculation/dq_df_calculation_parameters.py
+-rw-rw-rw-   0        0        0      428 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/settings/calculation/dq_file_calculation_parameters.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.496651 autonon-0.4.0/organon/idq/domain/settings/comparison/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/settings/comparison/__init__.py
+-rw-rw-rw-   0        0        0      417 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/settings/comparison/dq_df_comparison_parameters.py
+-rw-rw-rw-   0        0        0      422 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/settings/comparison/dq_file_comparison_parameters.py
+-rw-rw-rw-   0        0        0      230 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/idq/domain/settings/dask_settings.py
+-rw-rw-rw-   0        0        0      937 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/settings/date_value_definition.py
+-rw-rw-rw-   0        0        0      282 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/settings/dq_column_metadata.py
+-rw-rw-rw-   0        0        0      284 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/settings/dq_comparison_column_info.py
+-rw-rw-rw-   0        0        0      324 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/settings/dq_notification_settings.py
+-rw-rw-rw-   0        0        0      187 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/settings/dq_output_settings.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.496651 autonon-0.4.0/organon/idq/domain/settings/full_process/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/settings/full_process/__init__.py
+-rw-rw-rw-   0        0        0      527 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/settings/full_process/dq_df_full_process_input.py
+-rw-rw-rw-   0        0        0      536 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/settings/full_process/dq_file_full_process_input.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.512276 autonon-0.4.0/organon/idq/domain/settings/input_source/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/settings/input_source/__init__.py
+-rw-rw-rw-   0        0        0      489 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/settings/input_source/dq_df_input_source_settings.py
+-rw-rw-rw-   0        0        0      656 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/settings/input_source/dq_file_input_source_settings.py
+-rw-rw-rw-   0        0        0      266 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/settings/mail_notification_settings.py
+-rw-rw-rw-   0        0        0     1750 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/domain/settings/partition_info.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.512276 autonon-0.4.0/organon/idq/services/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/services/__init__.py
+-rw-rw-rw-   0        0        0     6008 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/idq/services/base_idq_executor.py
+-rw-rw-rw-   0        0        0      911 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/idq/services/idq_application_operations.py
+-rw-rw-rw-   0        0        0     1692 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/services/idq_executor.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.563021 autonon-0.4.0/organon/idq/services/user_settings/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/services/user_settings/__init__.py
+-rw-rw-rw-   0        0        0    14301 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/services/user_settings/base_dq_user_input.py
+-rw-rw-rw-   0        0        0      696 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/services/user_settings/base_user_calculation_params.py
+-rw-rw-rw-   0        0        0     1862 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/services/user_settings/dq_user_input.py
+-rw-rw-rw-   0        0        0      689 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/services/user_settings/user_calculation_params.py
+-rw-rw-rw-   0        0        0      274 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/services/user_settings/user_date_value_definition.py
+-rw-rw-rw-   0        0        0      318 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/services/user_settings/user_db_obj_locator.py
+-rw-rw-rw-   0        0        0      458 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/services/user_settings/user_existing_calculation_params.py
+-rw-rw-rw-   0        0        0      718 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/services/user_settings/user_input_source_settings.py
+-rw-rw-rw-   0        0        0      705 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/services/user_settings/user_multi_partition_calculation_params.py
+-rw-rw-rw-   0        0        0      416 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/idq/services/user_settings/user_partition_info.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.563021 autonon-0.4.0/organon/ml/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.563021 autonon-0.4.0/organon/ml/common/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.578647 autonon-0.4.0/organon/ml/common/enums/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/common/enums/__init__.py
+-rw-rw-rw-   0        0        0      190 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/common/enums/classification_type.py
+-rw-rw-rw-   0        0        0      177 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/common/enums/color_type.py
+-rw-rw-rw-   0        0        0      297 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/common/enums/optimizer_type.py
+-rw-rw-rw-   0        0        0      296 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/common/enums/pretrained_model_type.py
+-rw-rw-rw-   0        0        0      223 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/common/enums/random_flip_type.py
+-rw-rw-rw-   0        0        0      193 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/common/enums/target_type.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.594273 autonon-0.4.0/organon/ml/common/helpers/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/common/helpers/__init__.py
+-rw-rw-rw-   0        0        0     3421 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/common/helpers/df_ops_helper.py
+-rw-rw-rw-   0        0        0      359 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/common/helpers/parameter_helper.py
+-rw-rw-rw-   0        0        0      864 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/common/helpers/user_input_service_helper.py
+-rw-rw-rw-   0        0        0      970 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/common/helpers/validation_helper.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.594273 autonon-0.4.0/organon/ml/common/objects/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/common/objects/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.594273 autonon-0.4.0/organon/ml/feature_reduction/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_reduction/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.594273 autonon-0.4.0/organon/ml/feature_reduction/domain/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_reduction/domain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.609902 autonon-0.4.0/organon/ml/feature_reduction/domain/enums/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_reduction/domain/enums/__init__.py
+-rw-rw-rw-   0        0        0      296 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_reduction/domain/enums/feature_reduction_types.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.609902 autonon-0.4.0/organon/ml/feature_reduction/domain/helpers/
+-rw-rw-rw-   0        0        0        0 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/feature_reduction/domain/helpers/__init__.py
+-rw-rw-rw-   0        0        0     4282 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/feature_reduction/domain/helpers/univariate_performance_helper.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.625527 autonon-0.4.0/organon/ml/feature_reduction/domain/objects/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_reduction/domain/objects/__init__.py
+-rw-rw-rw-   0        0        0      391 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_reduction/domain/objects/feature_reduction_output.py
+-rw-rw-rw-   0        0        0      423 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/feature_reduction/domain/objects/high_corr_reduction_output.py
+-rw-rw-rw-   0        0        0      826 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_reduction/domain/objects/numeric_column_stats.py
+-rw-rw-rw-   0        0        0      433 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/feature_reduction/domain/objects/similar_dist_reduction_output.py
+-rw-rw-rw-   0        0        0      464 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_reduction/domain/objects/univariate_performance_reduction_output.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.625527 autonon-0.4.0/organon/ml/feature_reduction/domain/reductions/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_reduction/domain/reductions/__init__.py
+-rw-rw-rw-   0        0        0     1770 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/feature_reduction/domain/reductions/base_feature_reduction.py
+-rw-rw-rw-   0        0        0     6695 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/feature_reduction/domain/reductions/high_correlated_feature_reduction.py
+-rw-rw-rw-   0        0        0     2257 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/feature_reduction/domain/reductions/null_feature_reduction.py
+-rw-rw-rw-   0        0        0     6006 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/feature_reduction/domain/reductions/similar_distribution_feature_reduction.py
+-rw-rw-rw-   0        0        0     1312 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/feature_reduction/domain/reductions/stability_feature_reduction.py
+-rw-rw-rw-   0        0        0     2733 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/feature_reduction/domain/reductions/univariate_performance_feature_reduction.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.625527 autonon-0.4.0/organon/ml/feature_reduction/domain/services/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_reduction/domain/services/__init__.py
+-rw-rw-rw-   0        0        0     5162 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/feature_reduction/domain/services/feature_reduction_service.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.625527 autonon-0.4.0/organon/ml/feature_reduction/services/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_reduction/services/__init__.py
+-rw-rw-rw-   0        0        0     3923 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/feature_reduction/services/feature_reduction.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.625527 autonon-0.4.0/organon/ml/feature_reduction/settings/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_reduction/settings/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.625527 autonon-0.4.0/organon/ml/feature_reduction/settings/enums/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_reduction/settings/enums/__init__.py
+-rw-rw-rw-   0        0        0    13494 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/feature_reduction/settings/feature_reduction_user_input_service.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.625527 autonon-0.4.0/organon/ml/feature_reduction/settings/objects/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_reduction/settings/objects/__init__.py
+-rw-rw-rw-   0        0        0      365 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/feature_reduction/settings/objects/base_feature_reduction_settings.py
+-rw-rw-rw-   0        0        0     1337 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/feature_reduction/settings/objects/high_correlated_feature_reduction_settings.py
+-rw-rw-rw-   0        0        0      601 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/feature_reduction/settings/objects/null_feature_reduction_settings.py
+-rw-rw-rw-   0        0        0     1318 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/feature_reduction/settings/objects/similar_distribution_feature_reduction_settings.py
+-rw-rw-rw-   0        0        0      295 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/feature_reduction/settings/objects/stability_feature_reduction_settings.py
+-rw-rw-rw-   0        0        0     1199 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/feature_reduction/settings/objects/univariate_performance_feature_reduction_settings.py
+-rw-rw-rw-   0        0        0      607 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/feature_reduction/settings/objects/user_feature_reduction_settings.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.625527 autonon-0.4.0/organon/ml/feature_selection/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_selection/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.641148 autonon-0.4.0/organon/ml/feature_selection/domain/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_selection/domain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.641148 autonon-0.4.0/organon/ml/feature_selection/domain/enums/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_selection/domain/enums/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.656776 autonon-0.4.0/organon/ml/feature_selection/domain/objects/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_selection/domain/objects/__init__.py
+-rw-rw-rw-   0        0        0      229 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_selection/domain/objects/base_selection_output.py
+-rw-rw-rw-   0        0        0      227 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_selection/domain/objects/cfs_selection_output.py
+-rw-rw-rw-   0        0        0      271 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_selection/domain/objects/feature_similarity_selection_output.py
+-rw-rw-rw-   0        0        0      233 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_selection/domain/objects/lasso_selection_output.py
+-rw-rw-rw-   0        0        0     1372 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_selection/domain/objects/priority_queue.py
+-rw-rw-rw-   0        0        0      235 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_selection/domain/objects/rf_selection_output.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.703650 autonon-0.4.0/organon/ml/feature_selection/domain/objects/settings/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_selection/domain/objects/settings/__init__.py
+-rw-rw-rw-   0        0        0      259 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_selection/domain/objects/settings/base_feature_selection_settings.py
+-rw-rw-rw-   0        0        0      649 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_selection/domain/objects/settings/base_supervised_feature_selection_settings.py
+-rw-rw-rw-   0        0        0      349 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_selection/domain/objects/settings/base_unsupervised_feature_selection_settings.py
+-rw-rw-rw-   0        0        0      722 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_selection/domain/objects/settings/cfs_selection_settings.py
+-rw-rw-rw-   0        0        0      652 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_selection/domain/objects/settings/feature_similarity_selection_settings.py
+-rw-rw-rw-   0        0        0      683 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_selection/domain/objects/settings/lasso_selection_settings.py
+-rw-rw-rw-   0        0        0      855 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_selection/domain/objects/settings/rf_selection_settings.py
+-rw-rw-rw-   0        0        0      753 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/feature_selection/domain/objects/settings/sweep_selection_settings.py
+-rw-rw-rw-   0        0        0      233 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_selection/domain/objects/sweep_selection_output.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.736515 autonon-0.4.0/organon/ml/feature_selection/domain/services/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_selection/domain/services/__init__.py
+-rw-rw-rw-   0        0        0     5879 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/feature_selection/domain/services/base_feature_selection_service.py
+-rw-rw-rw-   0        0        0     1811 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_selection/domain/services/base_supervised_feature_selection_service.py
+-rw-rw-rw-   0        0        0     1158 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_selection/domain/services/base_unsupervised_feature_selection_service.py
+-rw-rw-rw-   0        0        0     4985 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_selection/domain/services/cfs_selection_service.py
+-rw-rw-rw-   0        0        0     5701 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_selection/domain/services/feature_similarity_selection_service.py
+-rw-rw-rw-   0        0        0     1913 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_selection/domain/services/lasso_selection_service.py
+-rw-rw-rw-   0        0        0     2020 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_selection/domain/services/rf_selection_service.py
+-rw-rw-rw-   0        0        0     1923 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/feature_selection/domain/services/sweep_selection_service.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.754412 autonon-0.4.0/organon/ml/feature_selection/services/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_selection/services/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.770037 autonon-0.4.0/organon/ml/feature_selection/services/abstractions/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_selection/services/abstractions/__init__.py
+-rw-rw-rw-   0        0        0      436 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_selection/services/abstractions/base_feature_selecter.py
+-rw-rw-rw-   0        0        0      769 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_selection/services/abstractions/base_supervised_feature_selecter.py
+-rw-rw-rw-   0        0        0      326 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_selection/services/abstractions/base_unsupervised_feature_selecter.py
+-rw-rw-rw-   0        0        0     1545 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_selection/services/cfs.py
+-rw-rw-rw-   0        0        0     1435 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_selection/services/feature_similarity_selection.py
+-rw-rw-rw-   0        0        0     1400 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_selection/services/lasso_selection.py
+-rw-rw-rw-   0        0        0     1582 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/feature_selection/services/rf_selection.py
+-rw-rw-rw-   0        0        0     1335 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/feature_selection/services/sweep_selection.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.770037 autonon-0.4.0/organon/ml/modelling/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.770037 autonon-0.4.0/organon/ml/modelling/algorithms/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/algorithms/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.801285 autonon-0.4.0/organon/ml/modelling/algorithms/classifiers/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/algorithms/classifiers/__init__.py
+-rw-rw-rw-   0        0        0     6115 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/algorithms/classifiers/gam_classifier.py
+-rw-rw-rw-   0        0        0      433 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/algorithms/classifiers/gbm_classifier.py
+-rw-rw-rw-   0        0        0      375 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/algorithms/classifiers/lightgbm_classifier.py
+-rw-rw-rw-   0        0        0      435 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/algorithms/classifiers/logistic_regression_classifier.py
+-rw-rw-rw-   0        0        0      421 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/algorithms/classifiers/multi_layer_perceptron_classifier.py
+-rw-rw-rw-   0        0        0      415 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/algorithms/classifiers/rf_classifier.py
+-rw-rw-rw-   0        0        0      563 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/algorithms/classifiers/stacking_ensemble_classifier.py
+-rw-rw-rw-   0        0        0     2252 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/algorithms/classifiers/voting_ensemble_classifier.py
+-rw-rw-rw-   0        0        0      372 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/algorithms/classifiers/xgboost_classifier.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.801285 autonon-0.4.0/organon/ml/modelling/algorithms/core/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/algorithms/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.832537 autonon-0.4.0/organon/ml/modelling/algorithms/core/abstractions/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/algorithms/core/abstractions/__init__.py
+-rw-rw-rw-   0        0        0     1935 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/algorithms/core/abstractions/base_classifier.py
+-rw-rw-rw-   0        0        0     6296 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/algorithms/core/abstractions/base_modeller.py
+-rw-rw-rw-   0        0        0      842 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/algorithms/core/abstractions/base_regressor.py
+-rw-rw-rw-   0        0        0     1979 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/algorithms/core/abstractions/base_sklearn_classifier.py
+-rw-rw-rw-   0        0        0     1718 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/algorithms/core/abstractions/base_sklearn_regressor.py
+-rw-rw-rw-   0        0        0     6150 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/modelling/algorithms/core/abstractions/gam_mixin.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.848161 autonon-0.4.0/organon/ml/modelling/algorithms/core/enums/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/algorithms/core/enums/__init__.py
+-rw-rw-rw-   0        0        0     1132 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/algorithms/core/enums/modeller.py
+-rw-rw-rw-   0        0        0      174 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/algorithms/core/enums/modeller_type.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.848161 autonon-0.4.0/organon/ml/modelling/algorithms/helpers/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/algorithms/helpers/__init__.py
+-rw-rw-rw-   0        0        0     2217 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/algorithms/helpers/ensembling_helper.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.899407 autonon-0.4.0/organon/ml/modelling/algorithms/regressors/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/algorithms/regressors/__init__.py
+-rw-rw-rw-   0        0        0     2688 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/algorithms/regressors/gam_regressor.py
+-rw-rw-rw-   0        0        0      423 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/algorithms/regressors/gbm_regressor.py
+-rw-rw-rw-   0        0        0      359 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/algorithms/regressors/lasso_regressor.py
+-rw-rw-rw-   0        0        0      369 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/algorithms/regressors/lightgbm_regressor.py
+-rw-rw-rw-   0        0        0      411 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/algorithms/regressors/multi_layer_perceptron_regressor.py
+-rw-rw-rw-   0        0        0      405 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/algorithms/regressors/rf_regressor.py
+-rw-rw-rw-   0        0        0      358 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/algorithms/regressors/ridge_regressor.py
+-rw-rw-rw-   0        0        0      553 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/algorithms/regressors/stacking_ensemble_regressor.py
+-rw-rw-rw-   0        0        0     1614 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/algorithms/regressors/voting_ensemble_regressor.py
+-rw-rw-rw-   0        0        0      362 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/algorithms/regressors/xgboost_regressor.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.905193 autonon-0.4.0/organon/ml/modelling/algorithms/services/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/algorithms/services/__init__.py
+-rw-rw-rw-   0        0        0     2469 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/algorithms/services/algorithm_service.py
+-rw-rw-rw-   0        0        0     5658 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/modelling/algorithms/services/ml_application_operations.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.906216 autonon-0.4.0/organon/ml/modelling/model_selection/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/model_selection/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.906216 autonon-0.4.0/organon/ml/modelling/model_selection/domain/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/model_selection/domain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.908440 autonon-0.4.0/organon/ml/modelling/model_selection/domain/objects/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/model_selection/domain/objects/__init__.py
+-rw-rw-rw-   0        0        0      471 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/model_selection/domain/objects/cross_validation_output.py
+-rw-rw-rw-   0        0        0      400 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/model_selection/domain/objects/hpo_output.py
+-rw-rw-rw-   0        0        0      590 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/model_selection/domain/objects/selecter_output.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.924088 autonon-0.4.0/organon/ml/modelling/model_selection/domain/services/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/model_selection/domain/services/__init__.py
+-rw-rw-rw-   0        0        0     3770 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/model_selection/domain/services/cross_validation_service.py
+-rw-rw-rw-   0        0        0    10000 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/model_selection/domain/services/hpo_service.py
+-rw-rw-rw-   0        0        0    14376 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/model_selection/domain/services/selection_service.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.939714 autonon-0.4.0/organon/ml/modelling/model_selection/services/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/model_selection/services/__init__.py
+-rw-rw-rw-   0        0        0     1490 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/model_selection/services/cross_validation.py
+-rw-rw-rw-   0        0        0     2360 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/model_selection/services/hp_optimizer.py
+-rw-rw-rw-   0        0        0     1773 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/model_selection/services/selecter.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.955316 autonon-0.4.0/organon/ml/modelling/model_selection/services/user_settings/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/model_selection/services/user_settings/__init__.py
+-rw-rw-rw-   0        0        0      595 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/model_selection/services/user_settings/user_hp_optimization_settings.py
+-rw-rw-rw-   0        0        0      647 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/model_selection/services/user_settings/user_selection_settings.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.955316 autonon-0.4.0/organon/ml/modelling/model_selection/settings/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/model_selection/settings/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.970964 autonon-0.4.0/organon/ml/modelling/model_selection/settings/enums/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/model_selection/settings/enums/__init__.py
+-rw-rw-rw-   0        0        0      219 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/model_selection/settings/enums/search_type.py
+-rw-rw-rw-   0        0        0     5849 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/model_selection/settings/model_selection_user_input_service.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.986589 autonon-0.4.0/organon/ml/modelling/model_selection/settings/objects/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/model_selection/settings/objects/__init__.py
+-rw-rw-rw-   0        0        0      489 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/model_selection/settings/objects/cross_validation_settings.py
+-rw-rw-rw-   0        0        0      750 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/model_selection/settings/objects/hp_optimization_settings.py
+-rw-rw-rw-   0        0        0      733 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/modelling/model_selection/settings/objects/selection_settings.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.986589 autonon-0.4.0/organon/ml/object_classification/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/object_classification/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.986589 autonon-0.4.0/organon/ml/object_classification/common/
+-rw-rw-rw-   0        0        0        0 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/object_classification/common/__init__.py
+-rw-rw-rw-   0        0        0      512 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/object_classification/common/helpers.py
+-rw-rw-rw-   0        0        0      373 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/object_classification/common/object_classification_constants.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.986589 autonon-0.4.0/organon/ml/object_classification/domain/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/object_classification/domain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.986589 autonon-0.4.0/organon/ml/object_classification/domain/common/
+-rw-rw-rw-   0        0        0        0 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/object_classification/domain/common/__init__.py
+-rw-rw-rw-   0        0        0     4804 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/object_classification/domain/common/base_model_generator.py
+-rw-rw-rw-   0        0        0      722 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/object_classification/domain/common/helpers.py
+-rw-rw-rw-   0        0        0     2648 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/object_classification/domain/common/object_clf_settings_validator.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:14.986589 autonon-0.4.0/organon/ml/object_classification/domain/data_sources/
+-rw-rw-rw-   0        0        0        0 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/object_classification/domain/data_sources/__init__.py
+-rw-rw-rw-   0        0        0     2568 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/object_classification/domain/data_sources/base_data_source_handler.py
+-rw-rw-rw-   0        0        0     2130 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/object_classification/domain/data_sources/data_source_handler_factory.py
+-rw-rw-rw-   0        0        0     3099 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/object_classification/domain/data_sources/labeled_dir_data_source_handler.py
+-rw-rw-rw-   0        0        0     1233 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/object_classification/domain/data_sources/tf_dataset_data_source_handler.py
+-rw-rw-rw-   0        0        0     1369 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/object_classification/domain/data_sources/unlabeled_dir_data_source_handler.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:15.002218 autonon-0.4.0/organon/ml/object_classification/domain/objects/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/object_classification/domain/objects/__init__.py
+-rw-rw-rw-   0        0        0      544 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/object_classification/domain/objects/data_augmentation_settings.py
+-rw-rw-rw-   0        0        0      799 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/object_classification/domain/objects/data_source_settings.py
+-rw-rw-rw-   0        0        0      653 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/object_classification/domain/objects/fine_tuning_settings.py
+-rw-rw-rw-   0        0        0     2333 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/object_classification/domain/objects/object_clf_settings.py
+-rw-rw-rw-   0        0        0      448 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/object_classification/domain/objects/pretrained_model_settings.py
+-rw-rw-rw-   0        0        0      589 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/object_classification/domain/objects/transfer_learning_settings.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:15.002218 autonon-0.4.0/organon/ml/object_classification/domain/services/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/object_classification/domain/services/__init__.py
+-rw-rw-rw-   0        0        0    14769 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/object_classification/domain/services/base_object_classification_service.py
+-rw-rw-rw-   0        0        0     2437 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/object_classification/domain/services/binary_object_classificion_service.py
+-rw-rw-rw-   0        0        0     2786 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/object_classification/domain/services/multiclass_object_classification_service.py
+-rw-rw-rw-   0        0        0     1916 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/object_classification/domain/services/object_classification_service_factory.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:15.002218 autonon-0.4.0/organon/ml/object_classification/services/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/object_classification/services/__init__.py
+-rw-rw-rw-   0        0        0     6381 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/object_classification/services/object_classifier.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:15.002218 autonon-0.4.0/organon/ml/object_detection/
+-rw-rw-rw-   0        0        0        0 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/object_detection/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:15.002218 autonon-0.4.0/organon/ml/object_detection/domain/
+-rw-rw-rw-   0        0        0        0 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/object_detection/domain/__init__.py
+-rw-rw-rw-   0        0        0     6736 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/object_detection/domain/object_detection_training_service.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:15.002218 autonon-0.4.0/organon/ml/object_detection/services/
+-rw-rw-rw-   0        0        0        0 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/object_detection/services/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:15.002218 autonon-0.4.0/organon/ml/object_detection/services/enums/
+-rw-rw-rw-   0        0        0        0 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/object_detection/services/enums/__init__.py
+-rw-rw-rw-   0        0        0      190 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/object_detection/services/enums/map_metric.py
+-rw-rw-rw-   0        0        0      233 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/object_detection/services/enums/model_type.py
+-rw-rw-rw-   0        0        0    12768 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/object_detection/services/object_detection_trainer.py
+-rw-rw-rw-   0        0        0     6589 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/object_detection/services/object_detector.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:15.002218 autonon-0.4.0/organon/ml/object_detection/services/objects/
+-rw-rw-rw-   0        0        0        0 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/object_detection/services/objects/__init__.py
+-rw-rw-rw-   0        0        0      358 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/object_detection/services/objects/detection_info.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:15.002218 autonon-0.4.0/organon/ml/preprocessing/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/preprocessing/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:15.002218 autonon-0.4.0/organon/ml/preprocessing/domain/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/preprocessing/domain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:15.017816 autonon-0.4.0/organon/ml/preprocessing/domain/objects/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/preprocessing/domain/objects/__init__.py
+-rw-rw-rw-   0        0        0      406 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/preprocessing/domain/objects/coarse_class_fit_output.py
+-rw-rw-rw-   0        0        0      559 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/preprocessing/domain/objects/imputation_fit_output.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:15.017816 autonon-0.4.0/organon/ml/preprocessing/domain/services/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/preprocessing/domain/services/__init__.py
+-rw-rw-rw-   0        0        0    33942 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/preprocessing/domain/services/coarse_class_service.py
+-rw-rw-rw-   0        0        0     9325 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/preprocessing/domain/services/imputation_service.py
+-rw-rw-rw-   0        0        0    10037 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/preprocessing/domain/services/one_hot_encoding_service.py
+-rw-rw-rw-   0        0        0     2549 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/preprocessing/domain/services/scaling_service.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:15.033465 autonon-0.4.0/organon/ml/preprocessing/helpers/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/preprocessing/helpers/__init__.py
+-rw-rw-rw-   0        0        0     1476 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/preprocessing/helpers/preprocessing_input_helper.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:15.033465 autonon-0.4.0/organon/ml/preprocessing/services/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/preprocessing/services/__init__.py
+-rw-rw-rw-   0        0        0     5770 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/preprocessing/services/preprocessor.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:15.033465 autonon-0.4.0/organon/ml/preprocessing/services/user_settings/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/preprocessing/services/user_settings/__init__.py
+-rw-rw-rw-   0        0        0      410 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/preprocessing/services/user_settings/coarse_input_dto.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:15.033465 autonon-0.4.0/organon/ml/preprocessing/settings/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/preprocessing/settings/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:15.049066 autonon-0.4.0/organon/ml/preprocessing/settings/enums/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/preprocessing/settings/enums/__init__.py
+-rw-rw-rw-   0        0        0      178 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/preprocessing/settings/enums/imputer_type.py
+-rw-rw-rw-   0        0        0      175 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/preprocessing/settings/enums/scaler_type.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:15.049066 autonon-0.4.0/organon/ml/preprocessing/settings/objects/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/preprocessing/settings/objects/__init__.py
+-rw-rw-rw-   0        0        0      462 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/preprocessing/settings/objects/coarse_class_settings.py
+-rw-rw-rw-   0        0        0      615 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/preprocessing/settings/objects/imputation_settings.py
+-rw-rw-rw-   0        0        0      217 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/preprocessing/settings/objects/one_hot_encoding_settings.py
+-rw-rw-rw-   0        0        0      258 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/preprocessing/settings/objects/scaling_settings.py
+-rw-rw-rw-   0        0        0     4764 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/preprocessing/settings/preprocessing_user_input_service.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:15.049066 autonon-0.4.0/organon/ml/reporting/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/reporting/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:15.049066 autonon-0.4.0/organon/ml/reporting/domain/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/reporting/domain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:15.078264 autonon-0.4.0/organon/ml/reporting/domain/objects/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/reporting/domain/objects/__init__.py
+-rw-rw-rw-   0        0        0      114 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/reporting/domain/objects/base_report.py
+-rw-rw-rw-   0        0        0      426 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/reporting/domain/objects/binary_report.py
+-rw-rw-rw-   0        0        0      465 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/reporting/domain/objects/multiclass_report.py
+-rw-rw-rw-   0        0        0      339 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/reporting/domain/objects/regression_report.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:15.085302 autonon-0.4.0/organon/ml/reporting/domain/services/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/reporting/domain/services/__init__.py
+-rw-rw-rw-   0        0        0      709 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/reporting/domain/services/base_reporter_service.py
+-rw-rw-rw-   0        0        0    13326 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/reporting/domain/services/binary_reporter_service.py
+-rw-rw-rw-   0        0        0     9037 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/reporting/domain/services/multiclass_reporter_service.py
+-rw-rw-rw-   0        0        0     7160 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/reporting/domain/services/regression_reporter_service.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:15.085302 autonon-0.4.0/organon/ml/reporting/services/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/reporting/services/__init__.py
+-rw-rw-rw-   0        0        0     2704 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/reporting/services/reporter.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:15.085302 autonon-0.4.0/organon/ml/reporting/settings/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/reporting/settings/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:15.085302 autonon-0.4.0/organon/ml/reporting/settings/objects/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/reporting/settings/objects/__init__.py
+-rw-rw-rw-   0        0        0      420 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/reporting/settings/objects/multiclass_reporter_settings.py
+-rw-rw-rw-   0        0        0      409 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/reporting/settings/objects/reporter_settings.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:15.085302 autonon-0.4.0/organon/ml/sampling/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/sampling/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:15.085302 autonon-0.4.0/organon/ml/sampling/domain/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/sampling/domain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:15.085302 autonon-0.4.0/organon/ml/sampling/domain/objects/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/sampling/domain/objects/__init__.py
+-rw-rw-rw-   0        0        0      242 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/sampling/domain/objects/sampling_output.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:15.099339 autonon-0.4.0/organon/ml/sampling/domain/services/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/sampling/domain/services/__init__.py
+-rw-rw-rw-   0        0        0     1253 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/sampling/domain/services/sampling_preprocessing_service.py
+-rw-rw-rw-   0        0        0    10475 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/sampling/domain/services/sampling_service.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:15.099339 autonon-0.4.0/organon/ml/sampling/services/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/sampling/services/__init__.py
+-rw-rw-rw-   0        0        0     1390 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/sampling/services/sampler.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:15.115002 autonon-0.4.0/organon/ml/sampling/services/user_settings/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/sampling/services/user_settings/__init__.py
+-rw-rw-rw-   0        0        0      470 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/sampling/services/user_settings/user_sampling_settings.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:15.115002 autonon-0.4.0/organon/ml/sampling/settings/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/sampling/settings/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:15.115002 autonon-0.4.0/organon/ml/sampling/settings/enums/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/sampling/settings/enums/__init__.py
+-rw-rw-rw-   0        0        0      202 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/sampling/settings/enums/sampling_strategy.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:15.115002 autonon-0.4.0/organon/ml/sampling/settings/objects/
+-rw-rw-rw-   0        0        0        0 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/sampling/settings/objects/__init__.py
+-rw-rw-rw-   0        0        0      624 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/sampling/settings/objects/sampling_settings.py
+-rw-rw-rw-   0        0        0     2636 2022-12-22 11:40:42.000000 autonon-0.4.0/organon/ml/sampling/settings/sampling_user_input_service.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:15.130598 autonon-0.4.0/organon/ml/text_classification/
+-rw-rw-rw-   0        0        0      155 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/text_classification/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:15.130598 autonon-0.4.0/organon/ml/text_classification/domain/
+-rw-rw-rw-   0        0        0        0 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/text_classification/domain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:15.130598 autonon-0.4.0/organon/ml/text_classification/domain/enums/
+-rw-rw-rw-   0        0        0        0 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/text_classification/domain/enums/__init__.py
+-rw-rw-rw-   0        0        0      197 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/text_classification/domain/enums/classification_languages.py
+-rw-rw-rw-   0        0        0      326 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/text_classification/domain/enums/model_checkpoints.py
+-rw-rw-rw-   0        0        0      190 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/text_classification/domain/enums/model_run_type.py
+-rw-rw-rw-   0        0        0      256 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/text_classification/domain/enums/selection_metrics.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:15.130598 autonon-0.4.0/organon/ml/text_classification/domain/objects/
+-rw-rw-rw-   0        0        0        0 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/text_classification/domain/objects/__init__.py
+-rw-rw-rw-   0        0        0     1475 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/text_classification/domain/objects/grid_search_settings.py
+-rw-rw-rw-   0        0        0      358 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/text_classification/domain/objects/model_parameter_settings.py
+-rw-rw-rw-   0        0        0      538 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/text_classification/domain/objects/optimizer_settings.py
+-rw-rw-rw-   0        0        0     2188 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/text_classification/domain/objects/text_classification_settings.py
+-rw-rw-rw-   0        0        0      348 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/text_classification/domain/objects/tokenizer_settings.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:15.130598 autonon-0.4.0/organon/ml/text_classification/domain/services/
+-rw-rw-rw-   0        0        0        0 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/text_classification/domain/services/__init__.py
+-rw-rw-rw-   0        0        0    32705 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/text_classification/domain/services/text_classification_service.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:56:15.130598 autonon-0.4.0/organon/ml/text_classification/services/
+-rw-rw-rw-   0        0        0        0 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/text_classification/services/__init__.py
+-rw-rw-rw-   0        0        0     7132 2023-06-02 14:50:05.000000 autonon-0.4.0/organon/ml/text_classification/services/text_classifier.py
+-rw-rw-rw-   0        0        0       84 2022-12-22 11:40:42.000000 autonon-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-02 14:56:15.130598 autonon-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     2015 2023-06-02 14:50:05.000000 autonon-0.4.0/setup.py
```

### Comparing `autonon-0.3.0.post1/LICENSE` & `autonon-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/PKG-INFO` & `autonon-0.4.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,12 @@
-Metadata-Version: 2.1
-Name: autonon
-Version: 0.3.0.post1
-Summary: Organon Automated ML Platform
-Home-page: https://gitlab.com/organon-os/autonon
-Author: Organon Analytics
-Author-email: support@organonanalytics.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Autonon
 
-Autonon is a library to server a end to end machine learning pipeline. We are developing modules one by one. Currently, we developed feature extraction(AFE) and data quality modules(IDQ). There are more to come...
+AUTONON is a groundbreaking library developed by Organon Analytics, revolutionizing the world of Machine Learning. With its advanced capabilities, AUTONON automates and accelerates the entire Machine Learning process(MLops), enabling swift application to real-life challenges. As a versatile Python library available in both private and public clouds, AUTONON offers open source and commercial versions, catering to diverse user needs. Featuring four powerful modules, AUTONON empowers users with unparalleled capabilities. The feature extraction module enables efficient extraction of relevant information from datasets, while the data quality module ensures the integrity and reliability of input data. The machine learning module facilitates seamless model development and optimization, while the deep learning module opens doors to cutting-edge neural network architectures. By leveraging AUTONON, data scientists and practitioners can unlock new levels of efficiency, productivity, and accuracy in their Machine Learning endeavors. Whether it's accelerating research projects, developing innovative solutions, or tackling complex business problems, AUTONON empowers users to achieve exceptional results and stay at the forefront of the rapidly evolving field of Machine Learning
 
-- [Documentation](https://organonanalytics.atlassian.net/wiki/spaces/AOT/pages/2095546790/Getting+started)
+- [Documentation](https://organonanalytics.atlassian.net/wiki/spaces/AOT/overview)
 - [Code of Conduct](https://gitlab.com/organon-os/autonon/-/blob/main/CODE_OF_CONDUCT.md)
 - [Contribution](https://gitlab.com/organon-os/autonon/-/blob/main/CONTRIBUTING.md) 
 - Bug reports:  You can use GitLab issues.
 - Contact: support@organonanalytics.com
 - Company website: [Organon Analytics](http://www.organonanalytics.com/) 
 
 ## Installation
@@ -64,9 +48,7 @@
   coverage run --omit='*orgenv*' -m unittest organon/all_tests.py
   ```
 * Run command to get coverage report:  `coverage report`
 
 ### License
 
 This project is licensed under the terms of the [MIT License](LICENSE)
-
-
```

### Comparing `autonon-0.3.0.post1/autonon.egg-info/PKG-INFO` & `autonon-0.4.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autonon
-Version: 0.3.0.post1
+Version: 0.4.0
 Summary: Organon Automated ML Platform
 Home-page: https://gitlab.com/organon-os/autonon
 Author: Organon Analytics
 Author-email: support@organonanalytics.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -12,17 +12,17 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Autonon
 
-Autonon is a library to server a end to end machine learning pipeline. We are developing modules one by one. Currently, we developed feature extraction(AFE) and data quality modules(IDQ). There are more to come...
+AUTONON is a groundbreaking library developed by Organon Analytics, revolutionizing the world of Machine Learning. With its advanced capabilities, AUTONON automates and accelerates the entire Machine Learning process(MLops), enabling swift application to real-life challenges. As a versatile Python library available in both private and public clouds, AUTONON offers open source and commercial versions, catering to diverse user needs. Featuring four powerful modules, AUTONON empowers users with unparalleled capabilities. The feature extraction module enables efficient extraction of relevant information from datasets, while the data quality module ensures the integrity and reliability of input data. The machine learning module facilitates seamless model development and optimization, while the deep learning module opens doors to cutting-edge neural network architectures. By leveraging AUTONON, data scientists and practitioners can unlock new levels of efficiency, productivity, and accuracy in their Machine Learning endeavors. Whether it's accelerating research projects, developing innovative solutions, or tackling complex business problems, AUTONON empowers users to achieve exceptional results and stay at the forefront of the rapidly evolving field of Machine Learning
 
-- [Documentation](https://organonanalytics.atlassian.net/wiki/spaces/AOT/pages/2095546790/Getting+started)
+- [Documentation](https://organonanalytics.atlassian.net/wiki/spaces/AOT/overview)
 - [Code of Conduct](https://gitlab.com/organon-os/autonon/-/blob/main/CODE_OF_CONDUCT.md)
 - [Contribution](https://gitlab.com/organon-os/autonon/-/blob/main/CONTRIBUTING.md) 
 - Bug reports:  You can use GitLab issues.
 - Contact: support@organonanalytics.com
 - Company website: [Organon Analytics](http://www.organonanalytics.com/) 
 
 ## Installation
```

### Comparing `autonon-0.3.0.post1/autonon.egg-info/SOURCES.txt` & `autonon-0.4.0/autonon.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 organon/afe/core/businessobjects/__init__.py
 organon/afe/core/businessobjects/afe_static_objects.py
 organon/afe/data/__init__.py
 organon/afe/data/base_df.zip
 organon/afe/data/cash_df.zip
 organon/afe/data/score_df.zip
 organon/afe/dataaccess/__init__.py
+organon/afe/dataaccess/helpers/__init__.py
+organon/afe/dataaccess/helpers/record_source_helper.py
 organon/afe/dataaccess/services/__init__.py
 organon/afe/dataaccess/services/base_record_reader.py
 organon/afe/dataaccess/services/i_sample_data_service.py
 organon/afe/dataaccess/services/sample_data_service.py
 organon/afe/dataaccess/services/sample_data_service_helper.py
 organon/afe/dataaccess/services/target_file_record_repository.py
 organon/afe/dataaccess/services/transaction_file_record_reader.py
@@ -117,17 +119,21 @@
 organon/afe/domain/settings/target_descriptor.py
 organon/afe/domain/settings/temporal_grid.py
 organon/afe/domain/settings/trx_descriptor.py
 organon/afe/domain/settings/validation_helper.py
 organon/afe/services/__init__.py
 organon/afe/services/afe_application_operations.py
 organon/afe/services/afe_executor.py
+organon/common/__init__.py
+organon/common/helpers/__init__.py
+organon/common/helpers/dev_mode_helper.py
 organon/fl/__init__.py
 organon/fl/core/__init__.py
 organon/fl/core/businessobjects/__init__.py
+organon/fl/core/businessobjects/dask_dataframe.py
 organon/fl/core/businessobjects/data_partition.py
 organon/fl/core/businessobjects/dataframe.py
 organon/fl/core/businessobjects/date_interval.py
 organon/fl/core/businessobjects/dict_dataframe.py
 organon/fl/core/businessobjects/fl_core_static_objects.py
 organon/fl/core/businessobjects/histogram_16.py
 organon/fl/core/businessobjects/idata_partition.py
@@ -222,14 +228,16 @@
 organon/fl/mathematics/sweep/data_classes/transformation.py
 organon/fl/mathematics/sweep/matrices/__init__.py
 organon/fl/mathematics/sweep/matrices/csc_matrix.py
 organon/fl/mathematics/sweep/matrices/dense_matrix.py
 organon/fl/mathematics/sweep/matrices/i_matrix.py
 organon/fl/mathematics/sweep/pyx_files/__init__.py
 organon/fl/mathematics/sweep/pyx_files/sweep_helper.pyx
+organon/fl/modelling/__init__.py
+organon/fl/modelling/unsupervised_feature_extractor.py
 organon/fl/security/__init__.py
 organon/fl/security/helpers/__init__.py
 organon/fl/security/helpers/encryption_helper.py
 organon/fl/serialization/__init__.py
 organon/fl/serialization/serialization_helper.py
 organon/idq/__init__.py
 organon/idq/core/__init__.py
@@ -358,14 +366,15 @@
 organon/idq/domain/services/statistics/source_statistics/file_source_stats_service.py
 organon/idq/domain/services/task_executor/__init__.py
 organon/idq/domain/services/task_executor/calculation/__init__.py
 organon/idq/domain/services/task_executor/calculation/dq_calculation_task_executor.py
 organon/idq/domain/services/task_executor/comparison/__init__.py
 organon/idq/domain/services/task_executor/comparison/dq_comparison_task_executor.py
 organon/idq/domain/settings/__init__.py
+organon/idq/domain/settings/dask_settings.py
 organon/idq/domain/settings/date_value_definition.py
 organon/idq/domain/settings/dq_column_metadata.py
 organon/idq/domain/settings/dq_comparison_column_info.py
 organon/idq/domain/settings/dq_notification_settings.py
 organon/idq/domain/settings/dq_output_settings.py
 organon/idq/domain/settings/mail_notification_settings.py
 organon/idq/domain/settings/partition_info.py
@@ -401,29 +410,36 @@
 organon/idq/services/user_settings/user_input_source_settings.py
 organon/idq/services/user_settings/user_multi_partition_calculation_params.py
 organon/idq/services/user_settings/user_partition_info.py
 organon/ml/__init__.py
 organon/ml/common/__init__.py
 organon/ml/common/enums/__init__.py
 organon/ml/common/enums/classification_type.py
+organon/ml/common/enums/color_type.py
+organon/ml/common/enums/optimizer_type.py
 organon/ml/common/enums/pretrained_model_type.py
+organon/ml/common/enums/random_flip_type.py
 organon/ml/common/enums/target_type.py
 organon/ml/common/helpers/__init__.py
 organon/ml/common/helpers/df_ops_helper.py
 organon/ml/common/helpers/parameter_helper.py
 organon/ml/common/helpers/user_input_service_helper.py
 organon/ml/common/helpers/validation_helper.py
 organon/ml/common/objects/__init__.py
 organon/ml/feature_reduction/__init__.py
 organon/ml/feature_reduction/domain/__init__.py
 organon/ml/feature_reduction/domain/enums/__init__.py
 organon/ml/feature_reduction/domain/enums/feature_reduction_types.py
+organon/ml/feature_reduction/domain/helpers/__init__.py
+organon/ml/feature_reduction/domain/helpers/univariate_performance_helper.py
 organon/ml/feature_reduction/domain/objects/__init__.py
 organon/ml/feature_reduction/domain/objects/feature_reduction_output.py
+organon/ml/feature_reduction/domain/objects/high_corr_reduction_output.py
 organon/ml/feature_reduction/domain/objects/numeric_column_stats.py
+organon/ml/feature_reduction/domain/objects/similar_dist_reduction_output.py
 organon/ml/feature_reduction/domain/objects/univariate_performance_reduction_output.py
 organon/ml/feature_reduction/domain/reductions/__init__.py
 organon/ml/feature_reduction/domain/reductions/base_feature_reduction.py
 organon/ml/feature_reduction/domain/reductions/high_correlated_feature_reduction.py
 organon/ml/feature_reduction/domain/reductions/null_feature_reduction.py
 organon/ml/feature_reduction/domain/reductions/similar_distribution_feature_reduction.py
 organon/ml/feature_reduction/domain/reductions/stability_feature_reduction.py
@@ -450,15 +466,14 @@
 organon/ml/feature_selection/domain/objects/base_selection_output.py
 organon/ml/feature_selection/domain/objects/cfs_selection_output.py
 organon/ml/feature_selection/domain/objects/feature_similarity_selection_output.py
 organon/ml/feature_selection/domain/objects/lasso_selection_output.py
 organon/ml/feature_selection/domain/objects/priority_queue.py
 organon/ml/feature_selection/domain/objects/rf_selection_output.py
 organon/ml/feature_selection/domain/objects/sweep_selection_output.py
-organon/ml/feature_selection/domain/objects/unsupervised_feature_extractor.py
 organon/ml/feature_selection/domain/objects/settings/__init__.py
 organon/ml/feature_selection/domain/objects/settings/base_feature_selection_settings.py
 organon/ml/feature_selection/domain/objects/settings/base_supervised_feature_selection_settings.py
 organon/ml/feature_selection/domain/objects/settings/base_unsupervised_feature_selection_settings.py
 organon/ml/feature_selection/domain/objects/settings/cfs_selection_settings.py
 organon/ml/feature_selection/domain/objects/settings/feature_similarity_selection_settings.py
 organon/ml/feature_selection/domain/objects/settings/lasso_selection_settings.py
@@ -544,24 +559,53 @@
 organon/ml/modelling/model_selection/settings/enums/__init__.py
 organon/ml/modelling/model_selection/settings/enums/search_type.py
 organon/ml/modelling/model_selection/settings/objects/__init__.py
 organon/ml/modelling/model_selection/settings/objects/cross_validation_settings.py
 organon/ml/modelling/model_selection/settings/objects/hp_optimization_settings.py
 organon/ml/modelling/model_selection/settings/objects/selection_settings.py
 organon/ml/object_classification/__init__.py
+organon/ml/object_classification/common/__init__.py
+organon/ml/object_classification/common/helpers.py
+organon/ml/object_classification/common/object_classification_constants.py
 organon/ml/object_classification/domain/__init__.py
+organon/ml/object_classification/domain/common/__init__.py
+organon/ml/object_classification/domain/common/base_model_generator.py
+organon/ml/object_classification/domain/common/helpers.py
+organon/ml/object_classification/domain/common/object_clf_settings_validator.py
+organon/ml/object_classification/domain/data_sources/__init__.py
+organon/ml/object_classification/domain/data_sources/base_data_source_handler.py
+organon/ml/object_classification/domain/data_sources/data_source_handler_factory.py
+organon/ml/object_classification/domain/data_sources/labeled_dir_data_source_handler.py
+organon/ml/object_classification/domain/data_sources/tf_dataset_data_source_handler.py
+organon/ml/object_classification/domain/data_sources/unlabeled_dir_data_source_handler.py
 organon/ml/object_classification/domain/objects/__init__.py
+organon/ml/object_classification/domain/objects/data_augmentation_settings.py
+organon/ml/object_classification/domain/objects/data_source_settings.py
 organon/ml/object_classification/domain/objects/fine_tuning_settings.py
 organon/ml/object_classification/domain/objects/object_clf_settings.py
 organon/ml/object_classification/domain/objects/pretrained_model_settings.py
 organon/ml/object_classification/domain/objects/transfer_learning_settings.py
 organon/ml/object_classification/domain/services/__init__.py
-organon/ml/object_classification/domain/services/object_classification_service.py
+organon/ml/object_classification/domain/services/base_object_classification_service.py
+organon/ml/object_classification/domain/services/binary_object_classificion_service.py
+organon/ml/object_classification/domain/services/multiclass_object_classification_service.py
+organon/ml/object_classification/domain/services/object_classification_service_factory.py
 organon/ml/object_classification/services/__init__.py
 organon/ml/object_classification/services/object_classifier.py
+organon/ml/object_detection/__init__.py
+organon/ml/object_detection/domain/__init__.py
+organon/ml/object_detection/domain/object_detection_training_service.py
+organon/ml/object_detection/services/__init__.py
+organon/ml/object_detection/services/object_detection_trainer.py
+organon/ml/object_detection/services/object_detector.py
+organon/ml/object_detection/services/enums/__init__.py
+organon/ml/object_detection/services/enums/map_metric.py
+organon/ml/object_detection/services/enums/model_type.py
+organon/ml/object_detection/services/objects/__init__.py
+organon/ml/object_detection/services/objects/detection_info.py
 organon/ml/preprocessing/__init__.py
 organon/ml/preprocessing/domain/__init__.py
 organon/ml/preprocessing/domain/objects/__init__.py
 organon/ml/preprocessing/domain/objects/coarse_class_fit_output.py
 organon/ml/preprocessing/domain/objects/imputation_fit_output.py
 organon/ml/preprocessing/domain/services/__init__.py
 organon/ml/preprocessing/domain/services/coarse_class_service.py
@@ -596,14 +640,15 @@
 organon/ml/reporting/domain/services/binary_reporter_service.py
 organon/ml/reporting/domain/services/multiclass_reporter_service.py
 organon/ml/reporting/domain/services/regression_reporter_service.py
 organon/ml/reporting/services/__init__.py
 organon/ml/reporting/services/reporter.py
 organon/ml/reporting/settings/__init__.py
 organon/ml/reporting/settings/objects/__init__.py
+organon/ml/reporting/settings/objects/multiclass_reporter_settings.py
 organon/ml/reporting/settings/objects/reporter_settings.py
 organon/ml/sampling/__init__.py
 organon/ml/sampling/domain/__init__.py
 organon/ml/sampling/domain/objects/__init__.py
 organon/ml/sampling/domain/objects/sampling_output.py
 organon/ml/sampling/domain/services/__init__.py
 organon/ml/sampling/domain/services/sampling_preprocessing_service.py
@@ -613,8 +658,25 @@
 organon/ml/sampling/services/user_settings/__init__.py
 organon/ml/sampling/services/user_settings/user_sampling_settings.py
 organon/ml/sampling/settings/__init__.py
 organon/ml/sampling/settings/sampling_user_input_service.py
 organon/ml/sampling/settings/enums/__init__.py
 organon/ml/sampling/settings/enums/sampling_strategy.py
 organon/ml/sampling/settings/objects/__init__.py
-organon/ml/sampling/settings/objects/sampling_settings.py
+organon/ml/sampling/settings/objects/sampling_settings.py
+organon/ml/text_classification/__init__.py
+organon/ml/text_classification/domain/__init__.py
+organon/ml/text_classification/domain/enums/__init__.py
+organon/ml/text_classification/domain/enums/classification_languages.py
+organon/ml/text_classification/domain/enums/model_checkpoints.py
+organon/ml/text_classification/domain/enums/model_run_type.py
+organon/ml/text_classification/domain/enums/selection_metrics.py
+organon/ml/text_classification/domain/objects/__init__.py
+organon/ml/text_classification/domain/objects/grid_search_settings.py
+organon/ml/text_classification/domain/objects/model_parameter_settings.py
+organon/ml/text_classification/domain/objects/optimizer_settings.py
+organon/ml/text_classification/domain/objects/text_classification_settings.py
+organon/ml/text_classification/domain/objects/tokenizer_settings.py
+organon/ml/text_classification/domain/services/__init__.py
+organon/ml/text_classification/domain/services/text_classification_service.py
+organon/ml/text_classification/services/__init__.py
+organon/ml/text_classification/services/text_classifier.py
```

### Comparing `autonon-0.3.0.post1/cython_setup.py` & `autonon-0.4.0/cython_setup.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/core/businessobjects/afe_static_objects.py` & `autonon-0.4.0/organon/afe/core/businessobjects/afe_static_objects.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/data/__init__.py` & `autonon-0.4.0/organon/afe/data/__init__.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/dataaccess/services/base_record_reader.py` & `autonon-0.4.0/organon/afe/dataaccess/services/base_record_reader.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/dataaccess/services/sample_data_service.py` & `autonon-0.4.0/organon/afe/dataaccess/services/sample_data_service.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/dataaccess/services/sample_data_service_helper.py` & `autonon-0.4.0/organon/afe/dataaccess/services/sample_data_service_helper.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/dataaccess/services/target_file_record_repository.py` & `autonon-0.4.0/organon/afe/dataaccess/services/target_file_record_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from datetime import datetime
 from typing import Callable, List, Optional
 
 import numpy as np
 import pandas as pd
 
 from organon.afe.core.businessobjects.afe_static_objects import AfeStaticObjects
+from organon.afe.dataaccess.helpers.record_source_helper import validate_entity_column
 from organon.afe.dataaccess.services.base_record_reader import BaseRecordReader
 from organon.afe.domain.common import afe_date_helper
 from organon.afe.domain.enums.afe_date_column_type import AfeDateColumnType
 from organon.afe.domain.enums.afe_target_column_type import AfeTargetColumnType
 from organon.afe.domain.enums.binary_target_class import BinaryTargetClass
 from organon.afe.domain.modelling.businessobjects.target_file_record import TargetFileRecord
 from organon.afe.domain.modelling.businessobjects.target_file_record_collection import TargetFileRecordCollection
@@ -80,14 +81,15 @@
         Creates TargetFileRecords from a pandas DataFrame and stores in collection.
 
         :param TargetFileRecordCollection collection:
         :param pd.DataFrame data_frame:
         :param int initial_index: collection index to start adding data_frame rows
         """
         index = initial_index
+        validate_entity_column("target", data_frame, self._file_descriptor.entity_column_name)
         try:
             for row_iter in data_frame.iterrows():
                 frame_row = row_iter[1]
                 entity_id = frame_row[self._file_descriptor.entity_column_name]
                 target = None
                 if self._is_scoring:
                     if self._file_descriptor.target_column is not None and \
```

### Comparing `autonon-0.3.0.post1/organon/afe/dataaccess/services/transaction_file_record_reader.py` & `autonon-0.4.0/organon/afe/dataaccess/services/transaction_file_record_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from datetime import datetime
 from typing import Dict, Callable, Tuple, List, Optional
 
 import numpy as np
 import pandas as pd
 
 from organon.afe.core.businessobjects.afe_static_objects import AfeStaticObjects
+from organon.afe.dataaccess.helpers.record_source_helper import validate_entity_column
 from organon.afe.dataaccess.services.base_record_reader import BaseRecordReader
 from organon.afe.domain.common import afe_date_helper
 from organon.afe.domain.enums.record_source_type import RecordSourceType
 from organon.afe.domain.modelling.businessobjects.transaction_file_record_collection import \
     TransactionFileRecordCollection
 from organon.afe.domain.modelling.businessobjects.transaction_file_stats import TransactionFileStats
 from organon.afe.domain.settings.afe_date_column import AfeDateColumn
@@ -226,14 +227,15 @@
 
         :param set unique_entities_set: Set of unique entities to be read
         :param max_record_num: Maximum number of records to be created
         :param pd.DataFrame data_frame: DataFrame to be read
         :param TransactionFileRecordCollection collection: Collection to store records
         """
         trx_entity_column: str = self._trx_entity_column
+        validate_entity_column("transaction", data_frame, trx_entity_column)
         trx_date_columns = [date_column.column_name for date_column in self._date_columns.values()]
 
         columns_ordered = [trx_entity_column]
         if len(trx_date_columns) > 0:
             columns_ordered.extend(trx_date_columns)
 
         columns_ordered.extend(self._non_empty_q_cols)
```

### Comparing `autonon-0.3.0.post1/organon/afe/domain/common/afe_date_helper.py` & `autonon-0.4.0/organon/afe/domain/common/afe_date_helper.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/common/base_execution_plan_service.py` & `autonon-0.4.0/organon/afe/domain/common/base_execution_plan_service.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/common/persist_helper.py` & `autonon-0.4.0/organon/afe/domain/common/persist_helper.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/common/reader_helper.py` & `autonon-0.4.0/organon/afe/domain/common/reader_helper.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/common/runtime_stats_service.py` & `autonon-0.4.0/organon/afe/domain/common/runtime_stats_service.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/enums/afe_operator.py` & `autonon-0.4.0/organon/afe/domain/enums/afe_operator.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/modelling/abstract_modelling_service.py` & `autonon-0.4.0/organon/afe/domain/modelling/abstract_modelling_service.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/modelling/auto_column_type_decider_service.py` & `autonon-0.4.0/organon/afe/domain/modelling/auto_column_type_decider_service.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/modelling/base_modelling_service.py` & `autonon-0.4.0/organon/afe/domain/modelling/base_modelling_service.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/modelling/businessobjects/afe_column.py` & `autonon-0.4.0/organon/afe/domain/modelling/businessobjects/afe_column.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/modelling/businessobjects/bin_info.py` & `autonon-0.4.0/organon/afe/domain/modelling/businessobjects/bin_info.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/modelling/businessobjects/data_frame_builder.py` & `autonon-0.4.0/organon/afe/domain/modelling/businessobjects/data_frame_builder.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/modelling/businessobjects/multi_target_entity_container.py` & `autonon-0.4.0/organon/afe/domain/modelling/businessobjects/multi_target_entity_container.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/modelling/businessobjects/target_file_record_collection.py` & `autonon-0.4.0/organon/afe/domain/modelling/businessobjects/target_file_record_collection.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/modelling/businessobjects/transaction_file_record.py` & `autonon-0.4.0/organon/afe/domain/modelling/businessobjects/transaction_file_record.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/modelling/businessobjects/transaction_file_record_collection.py` & `autonon-0.4.0/organon/afe/domain/modelling/businessobjects/transaction_file_record_collection.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/modelling/businessobjects/transaction_file_stats.py` & `autonon-0.4.0/organon/afe/domain/modelling/businessobjects/transaction_file_stats.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/modelling/helper/data_frame_builder_helper.pyx` & `autonon-0.4.0/organon/afe/domain/modelling/helper/data_frame_builder_helper.pyx`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/modelling/helper/trx_reader_helper.py` & `autonon-0.4.0/organon/afe/domain/modelling/helper/trx_reader_helper.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/modelling/supervised/afe_supervised_algorithm_settings.py` & `autonon-0.4.0/organon/afe/domain/modelling/supervised/afe_supervised_algorithm_settings.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/modelling/supervised/multi_target_entity_container_service.py` & `autonon-0.4.0/organon/afe/domain/modelling/supervised/multi_target_entity_container_service.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/modelling/supervised/multi_target_modelling_helper.py` & `autonon-0.4.0/organon/afe/domain/modelling/supervised/multi_target_modelling_helper.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/modelling/supervised/multi_target_modelling_service.py` & `autonon-0.4.0/organon/afe/domain/modelling/supervised/multi_target_modelling_service.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/modelling/unsupervised/afe_unsupervised_algorithm_settings.py` & `autonon-0.4.0/organon/afe/domain/modelling/unsupervised/afe_unsupervised_algorithm_settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,20 +8,22 @@
 class AfeUnsupervisedAlgorithmSettings(AfeAlgorithmSettings):
     """
     Algorithm settings for Automated Feature Extraction with Unsupervised Learning type
     """
     ATTR_DICT = {
         "bin_count": int,
         "r_factor": float,
+        "random_state": int,
         "max_column_count": int,
         "is_logging": bool
     }
     ATTR_DICT.update(AfeAlgorithmSettings.ATTR_DICT)
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.bin_count: int = None
         self.r_factor: float = None
+        self.random_state: int = None
         self.max_column_count: int = None
         self.is_logging: bool = None
 
         get_values_from_kwargs(self, self.ATTR_DICT, kwargs)
```

### Comparing `autonon-0.3.0.post1/organon/afe/domain/modelling/unsupervised/unsupervised_feature_extraction_service.py` & `autonon-0.4.0/organon/afe/domain/modelling/unsupervised/unsupervised_feature_extraction_service.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/modelling/unsupervised/unsupervised_modelling_helper.py` & `autonon-0.4.0/organon/afe/domain/modelling/unsupervised/unsupervised_modelling_helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """Includes UnsupervisedModellingHelper and UnsupervisedFeatureExtractor classes."""
 from typing import List
 
 from organon.afe.domain.modelling.unsupervised.afe_unsupervised_algorithm_settings import \
     AfeUnsupervisedAlgorithmSettings
 from organon.fl.core.businessobjects.dict_dataframe import DictDataFrame
-from organon.ml.feature_selection.domain.objects.unsupervised_feature_extractor import UnsupervisedFeatureExtractor
+from organon.fl.modelling.unsupervised_feature_extractor import UnsupervisedFeatureExtractor
 
 
 class UnsupervisedModellingHelper:
     """
     Helper class for Unsupervised Feature Extraction Service
     """
 
     @staticmethod
     def get_selected_cols(num_threads: int,
                           algorithm_settings: AfeUnsupervisedAlgorithmSettings = None,
                           frame_with_all_columns: DictDataFrame = None) -> List[str]:
         """Selects best afe columns by unsupervised modelling"""
         input_frame = dict((k, frame_with_all_columns.get_value(k)) for k in frame_with_all_columns.get_column_names())
         extractor = UnsupervisedFeatureExtractor(input_frame, algorithm_settings.bin_count, algorithm_settings.r_factor,
-                                                 algorithm_settings.max_column_count, algorithm_settings.is_logging)
+                                                 algorithm_settings.random_state, algorithm_settings.max_column_count,
+                                                 algorithm_settings.is_logging)
         return extractor.execute(num_threads)
```

### Comparing `autonon-0.3.0.post1/organon/afe/domain/reporting/abstract_report_helper.py` & `autonon-0.4.0/organon/afe/domain/reporting/abstract_report_helper.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/reporting/afe_column_dto.py` & `autonon-0.4.0/organon/afe/domain/reporting/afe_column_dto.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/reporting/afe_matplotlib_report_helper.py` & `autonon-0.4.0/organon/afe/domain/reporting/afe_matplotlib_report_helper.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/reporting/afe_plotly_report_helper.py` & `autonon-0.4.0/organon/afe/domain/reporting/afe_plotly_report_helper.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/reporting/base_afe_model_output.py` & `autonon-0.4.0/organon/afe/domain/reporting/base_afe_model_output.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/reporting/base_afe_output_report.py` & `autonon-0.4.0/organon/afe/domain/reporting/base_afe_output_report.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/reporting/base_report_helper.py` & `autonon-0.4.0/organon/afe/domain/reporting/base_report_helper.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/reporting/dashboard_helper.py` & `autonon-0.4.0/organon/afe/domain/reporting/dashboard_helper.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/reporting/matplotlib_common_functions.py` & `autonon-0.4.0/organon/afe/domain/reporting/matplotlib_common_functions.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/reporting/plotly_common_functions.py` & `autonon-0.4.0/organon/afe/domain/reporting/plotly_common_functions.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/reporting/plotly_dashboard_helper.py` & `autonon-0.4.0/organon/afe/domain/reporting/plotly_dashboard_helper.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/reporting/transformation.py` & `autonon-0.4.0/organon/afe/domain/reporting/transformation.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/scoring/afe_scoring_service.py` & `autonon-0.4.0/organon/afe/domain/scoring/afe_scoring_service.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/settings/afe_algorithm_settings.py` & `autonon-0.4.0/organon/afe/domain/settings/afe_algorithm_settings.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/settings/afe_data_settings.py` & `autonon-0.4.0/organon/afe/domain/settings/afe_data_settings.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/settings/afe_date_column.py` & `autonon-0.4.0/organon/afe/domain/settings/afe_date_column.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/settings/afe_modelling_settings.py` & `autonon-0.4.0/organon/afe/domain/settings/afe_modelling_settings.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/settings/afe_output_settings.py` & `autonon-0.4.0/organon/afe/domain/settings/afe_output_settings.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/settings/afe_process_settings.py` & `autonon-0.4.0/organon/afe/domain/settings/afe_process_settings.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/settings/afe_settings_reader.py` & `autonon-0.4.0/organon/afe/domain/settings/afe_settings_reader.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 """
 This module includes AfeSettingsReader class.
 """
 from organon.afe.domain.common.reader_helper import setattr_if_none
 from organon.afe.domain.settings.afe_modelling_settings import AfeModellingSettings
 from organon.afe.domain.settings.afe_reading_settings import AfeDataReadingSettings
 from organon.afe.domain.settings.base_afe_settings_reader import BaseAfeSettingsReader
-from organon.afe.domain.enums.afe_operator import AfeOperator
+
 
 class AfeSettingsReader(BaseAfeSettingsReader[AfeModellingSettings]):
     """
     Class for static methods on reading AfeModellingSettings from a file
     """
 
     def _set_trx_descriptor_defaults(self, modelling_settings: AfeModellingSettings):
 
         feature_gen_settings = modelling_settings.data_source_settings.trx_descriptor.feature_gen_setting
 
         if feature_gen_settings.included_operators is None:
-            feature_gen_settings.included_operators = [AfeOperator.Density, AfeOperator.Sum, AfeOperator.Frequency,
-                                                       AfeOperator.TimeSinceFirst, AfeOperator.Ratio]
-        if feature_gen_settings.included_trend_operators is None:
-            feature_gen_settings.included_trend_operators = [AfeOperator.DensityTrend, AfeOperator.FrequencyTrend,
-                                                             AfeOperator.SumTrend]
+            feature_gen_settings.included_operators = self._get_default_included_afe_operators()
         if feature_gen_settings.date_offset is None:
             feature_gen_settings.date_offset = 0
         try:
             trx_descriptor = modelling_settings.data_source_settings.trx_descriptor
             if trx_descriptor.reading_settings is None:
                 trx_descriptor.reading_settings = AfeDataReadingSettings()
```

### Comparing `autonon-0.3.0.post1/organon/afe/domain/settings/afe_settings_type_validators.py` & `autonon-0.4.0/organon/afe/domain/settings/afe_settings_type_validators.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/settings/afe_settings_validator.py` & `autonon-0.4.0/organon/afe/domain/settings/afe_settings_validator.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/settings/afe_target_column.py` & `autonon-0.4.0/organon/afe/domain/settings/afe_target_column.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/settings/auto_column_decider_settings.py` & `autonon-0.4.0/organon/afe/domain/settings/auto_column_decider_settings.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/settings/base_afe_data_settings.py` & `autonon-0.4.0/organon/afe/domain/settings/base_afe_data_settings.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/settings/base_afe_modelling_settings.py` & `autonon-0.4.0/organon/afe/domain/settings/base_afe_modelling_settings.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/settings/base_afe_scoring_settings.py` & `autonon-0.4.0/organon/afe/domain/settings/base_afe_scoring_settings.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/settings/base_afe_settings_reader.py` & `autonon-0.4.0/organon/afe/domain/settings/base_afe_settings_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,14 @@
         self._set_algorithm_settings_defaults(modelling_settings)
 
         self._set_trx_descriptor_defaults(modelling_settings)
         self.__set_target_descriptor_defaults(modelling_settings)
 
         self._assign_base_afe_settings_defaults(modelling_settings)
 
-
     @classmethod
     def _get_default_values_dict(cls):
         return {
             "data_source_settings": {
                 "entity_table_existence": False,
                 "max_number_of_target_samples": 100000,
                 "max_number_of_transaction_samples": np.iinfo(np.int64).max,
@@ -251,15 +250,14 @@
                                        date_resolution: Union[DateResolution, str] = None,
                                        date_column_name: str = None,
                                        date_column_type: Union[str, AfeDateColumnType] = None,
                                        date_column_format: str = None,
                                        dimension_columns: List[str] = None,
                                        quantity_columns: List[str] = None,
                                        included_operators: List[Union[AfeOperator, str]] = None,
-                                       included_trend_operators: List[Union[AfeOperator, str]] = None,
                                        date_offset: int = None,
                                        max_observation_date: datetime = None
                                        ) -> FeatureGenerationSettings:
         """
         Generates FeatureGenerationSettings instance.
         """
 
@@ -271,15 +269,14 @@
 
         return FeatureGenerationSettings(temporal_grids=temporal_grids,
                                          date_resolution=date_resolution,
                                          date_column=date_column,
                                          dimension_columns=dimension_columns,
                                          quantity_columns=quantity_columns,
                                          included_operators=included_operators,
-                                         included_trend_operators=included_trend_operators,
                                          date_offset=date_offset,
                                          max_observation_date=max_observation_date
                                          )
 
     @staticmethod
     def get_auto_column_decider_settings(sampling_ratio: float,
                                          numeric_to_dimension: int,
@@ -501,7 +498,12 @@
         modelling_settings.scoring_raw_input_source = scoring_raw_input_source
         modelling_settings.scoring_target_source = scoring_target_source
         modelling_settings.algorithm_settings = algorithm_settings
         modelling_settings.process_settings = process_settings
         modelling_settings.output_settings = output_settings
         modelling_settings.afe_learning_type = afe_learning_type
         return modelling_settings
+
+    @classmethod
+    def _get_default_included_afe_operators(cls) -> List[AfeOperator]:
+        return [AfeOperator.Density, AfeOperator.Sum, AfeOperator.Frequency, AfeOperator.TimeSinceFirst,
+                AfeOperator.Ratio]
```

### Comparing `autonon-0.3.0.post1/organon/afe/domain/settings/base_trx_descriptor.py` & `autonon-0.4.0/organon/afe/domain/settings/base_trx_descriptor.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/settings/binary_target.py` & `autonon-0.4.0/organon/afe/domain/settings/binary_target.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/settings/db_object_input.py` & `autonon-0.4.0/organon/afe/domain/settings/db_object_input.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/settings/feature_generation_settings.py` & `autonon-0.4.0/organon/afe/domain/settings/feature_generation_settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,25 +16,23 @@
         "date_column": AfeDateColumn,
         "dimension_columns": List[str],
         "quantity_columns": List[str],
         "temporal_grids": List[TemporalGrid],
         "date_resolution": DateResolution,
         "horizon_list": List[int],
         "included_operators": List[AfeOperator],
-        "included_trend_operators": List[AfeOperator],
         "date_offset": int,
         "max_observation_date": datetime
     }
 
     def __init__(self, **kwargs):
         self.date_column: AfeDateColumn = None
         self.dimension_columns: List[str] = None
         self.quantity_columns: List[str] = None
         self.temporal_grids: List[TemporalGrid] = None
         self.date_resolution: DateResolution = None
         self.horizon_list: List[int] = None
         self.included_operators: List[AfeOperator] = None
-        self.included_trend_operators: List[AfeOperator] = None
         self.date_offset: int = None
         self.max_observation_date: datetime = None
 
         get_values_from_kwargs(self, self.ATTR_DICT, kwargs)
```

### Comparing `autonon-0.3.0.post1/organon/afe/domain/settings/model_settings.py` & `autonon-0.4.0/organon/afe/domain/settings/model_settings.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/settings/modelling_reduction_settings.py` & `autonon-0.4.0/organon/afe/domain/settings/modelling_reduction_settings.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/settings/record_source.py` & `autonon-0.4.0/organon/afe/domain/settings/record_source.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/settings/target_descriptor.py` & `autonon-0.4.0/organon/afe/domain/settings/target_descriptor.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/settings/temporal_grid.py` & `autonon-0.4.0/organon/afe/domain/settings/temporal_grid.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/settings/trx_descriptor.py` & `autonon-0.4.0/organon/afe/domain/settings/trx_descriptor.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/domain/settings/validation_helper.py` & `autonon-0.4.0/organon/afe/domain/settings/validation_helper.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/afe/services/afe_executor.py` & `autonon-0.4.0/organon/afe/services/afe_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 This module includes AfeExecutionHelper class.
 """
 from datetime import datetime
 from typing import Union, List, Dict, Optional, Tuple, TypeVar, Generic
 
 import pandas as pd
 
-
+import organon
 from organon.afe.core.businessobjects.afe_static_objects import AfeStaticObjects
 from organon.afe.domain.common.persist_helper import PersistHelper
 from organon.afe.domain.enums.afe_date_column_type import AfeDateColumnType
 from organon.afe.domain.enums.afe_learning_type import AfeLearningType
 from organon.afe.domain.enums.afe_operator import AfeOperator
 from organon.afe.domain.enums.afe_target_column_type import AfeTargetColumnType
 from organon.afe.domain.enums.date_resolution import DateResolution
@@ -32,35 +32,41 @@
 from organon.afe.domain.settings.auto_column_decider_settings import AutoColumnDeciderSettings
 from organon.afe.domain.settings.feature_generation_settings import FeatureGenerationSettings
 from organon.afe.domain.settings.record_source import RecordSource
 from organon.afe.domain.settings.target_descriptor import TargetDescriptor
 from organon.afe.domain.settings.temporal_grid import TemporalGrid
 from organon.afe.domain.settings.trx_descriptor import TrxDescriptor
 from organon.afe.services.afe_application_operations import AfeApplicationOperations
+from organon.common.helpers import dev_mode_helper
 from organon.fl.core.exceptionhandling.known_exception import KnownException
 from organon.fl.core.helpers import process_info_helper
 from organon.fl.logging.helpers.log_helper import LogHelper
 from organon.fl.serialization.serialization_helper import serialize_to_file, deserialize_from_file
 
 AfeModelOutputType = TypeVar("AfeModelOutputType", bound=BaseAfeModelOutput)
 
 
 class AFE(Generic[AfeModelOutputType]):
     """
     AfeExecutionHelper class
     """
 
-    def __init__(self, log_to_console: bool = False):
-        self._initialize_afe(log_to_console)
+    def __init__(self):
+        self._initialize_afe()
         self.model_output: Optional[AfeModelOutputType] = None
         self._settings_reader = self._get_afe_settings_reader()
 
     @classmethod
-    def _initialize_afe(cls, log_to_console: bool):
-        AfeApplicationOperations.initialize_app(log_to_console)
+    def init_dev_mode(cls, log_to_console: bool = True, log_file: str = "application.log"):
+        """Initializes development mode."""
+        dev_mode_helper.init_dev_mode(organon.afe.__name__, log_to_console=log_to_console, log_file=log_file)
+
+    @classmethod
+    def _initialize_afe(cls):
+        AfeApplicationOperations.initialize_app()
 
     @classmethod
     def _get_afe_settings_reader(cls):
         return AfeSettingsReader()
 
     @classmethod
     def _get_afe_settings_validator(cls):
@@ -294,15 +300,14 @@
                                        date_resolution: Union[DateResolution, str] = None,
                                        date_column_name: str = None,
                                        date_column_type: Union[str, AfeDateColumnType] = None,
                                        date_column_format: str = None,
                                        dimension_columns: List[str] = None,
                                        quantity_columns: List[str] = None,
                                        included_operators: List[Union[AfeOperator, str]] = None,
-                                       included_trend_operators: List[Union[AfeOperator, str]] = None,
                                        date_offset: int = None,
                                        max_observation_date: datetime = None,
                                        **kwargs
                                        ):
         """
         Generates FeatureGenerationSettings instance.
 
@@ -310,30 +315,28 @@
         :param date_resolution:
         :param date_column_name:
         :param date_column_type:
         :param date_column_format:
         :param dimension_columns:
         :param quantity_columns:
         :param included_operators:
-        :param included_trend_operators:
         :param date_offset:
         :param max_observation_date:
         :return:
         """
         # pylint: disable=too-many-arguments, unused-argument
         return cls._get_afe_settings_reader().get_feature_generation_setting(
             temporal_grids=temporal_grids,
             date_resolution=date_resolution,
             date_column_name=date_column_name,
             date_column_format=date_column_format,
             date_column_type=date_column_type,
             dimension_columns=dimension_columns,
             quantity_columns=quantity_columns,
             included_operators=included_operators,
-            included_trend_operators=included_trend_operators,
             date_offset=date_offset,
             max_observation_date=max_observation_date
         )
 
     @classmethod
     def get_auto_column_decider_setting(cls, sampling_ratio: float = None,
                                         numeric_to_dimension: int = None,
```

### Comparing `autonon-0.3.0.post1/organon/fl/core/businessobjects/data_partition.py` & `autonon-0.4.0/organon/fl/core/businessobjects/data_partition.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/core/businessobjects/dataframe.py` & `autonon-0.4.0/organon/fl/core/businessobjects/dataframe.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/core/businessobjects/date_interval.py` & `autonon-0.4.0/organon/fl/core/businessobjects/date_interval.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/core/businessobjects/dict_dataframe.py` & `autonon-0.4.0/organon/fl/core/businessobjects/dict_dataframe.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/core/businessobjects/fl_core_static_objects.py` & `autonon-0.4.0/organon/fl/core/businessobjects/fl_core_static_objects.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/core/businessobjects/histogram_16.py` & `autonon-0.4.0/organon/fl/core/businessobjects/histogram_16.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/core/businessobjects/idata_partition.py` & `autonon-0.4.0/organon/fl/core/businessobjects/idata_partition.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/core/businessobjects/idataframe.py` & `autonon-0.4.0/organon/fl/core/businessobjects/idataframe.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/core/businessobjects/np2d_dataframe.py` & `autonon-0.4.0/organon/fl/core/businessobjects/np2d_dataframe.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/core/collections/pair.py` & `autonon-0.4.0/organon/fl/core/collections/pair.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/core/collections/sorted_dict.py` & `autonon-0.4.0/organon/fl/core/collections/sorted_dict.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/core/collections/sorted_list.py` & `autonon-0.4.0/organon/fl/core/collections/sorted_list.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/core/executionutil/objects/stopwatch.py` & `autonon-0.4.0/organon/fl/core/executionutil/objects/stopwatch.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/core/executionutil/parallel_execution_helper.py` & `autonon-0.4.0/organon/fl/core/executionutil/parallel_execution_helper.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/core/extensions/string_extensions.py` & `autonon-0.4.0/organon/fl/core/extensions/string_extensions.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/core/fileoperations/file_io_helper.py` & `autonon-0.4.0/organon/fl/core/fileoperations/file_io_helper.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/core/helpers/boolean_helper.py` & `autonon-0.4.0/organon/fl/core/helpers/boolean_helper.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/core/helpers/data_frame_helper.py` & `autonon-0.4.0/organon/fl/core/helpers/data_frame_helper.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/core/helpers/date_helper.py` & `autonon-0.4.0/organon/fl/core/helpers/date_helper.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/core/helpers/dict_helper.py` & `autonon-0.4.0/organon/fl/core/helpers/dict_helper.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/core/helpers/enums_helpers.py` & `autonon-0.4.0/organon/fl/core/helpers/enums_helpers.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/core/helpers/environment_info_helper.py` & `autonon-0.4.0/organon/fl/core/helpers/environment_info_helper.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/core/helpers/float_helper.py` & `autonon-0.4.0/organon/fl/core/helpers/float_helper.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/core/helpers/function_helper.py` & `autonon-0.4.0/organon/fl/core/helpers/function_helper.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/core/helpers/guid_helper.py` & `autonon-0.4.0/organon/fl/core/helpers/guid_helper.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/core/helpers/list_helper.py` & `autonon-0.4.0/organon/fl/core/helpers/list_helper.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/core/helpers/process_info_helper.py` & `autonon-0.4.0/organon/fl/core/helpers/process_info_helper.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/core/helpers/string_helper.py` & `autonon-0.4.0/organon/fl/core/helpers/string_helper.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/core/iocutil/ioc_helper.py` & `autonon-0.4.0/organon/fl/core/iocutil/ioc_helper.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/generic/interaction/fl_initializer.py` & `autonon-0.4.0/organon/fl/generic/interaction/fl_initializer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 """
 This module keeps the functions that are used in Framework Library initialization.
 """
 import threading
 
 from organon.fl.core.businessobjects.fl_core_static_objects import FlCoreStaticObjects
-from organon.fl.logging.helpers.log_helper import LogHelper
 
 FL_INIT_LOCK = threading.Lock()
 
 
 class FlInitializer:
     """Class for fl application operations"""
+
     @classmethod
-    def application_initialize(cls, log_to_console: bool = False):
+    def application_initialize(cls):
         """
         Gives the signal for application initialization the application by passing True value to the
         application_initialize_called variable.
         :return: nothing
         """
         with FL_INIT_LOCK:
             if not FlCoreStaticObjects.application_initialize_called:
-                cls._on_init(log_to_console)
+                cls._on_init()
                 FlCoreStaticObjects.application_initialize_called = True
 
     @classmethod
-    def _on_init(cls, log_to_console: bool):
-        LogHelper.initialize(log_to_console=log_to_console)
+    def _on_init(cls):
         cls.register_types()
 
     @classmethod
     def register_types(cls):
         """
         Registers the IoC items according to its ioc key, abstract type and concrete type.
         :return:nothing
```

### Comparing `autonon-0.3.0.post1/organon/fl/logging/helpers/log_helper.py` & `autonon-0.4.0/organon/fl/logging/helpers/log_helper.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,36 @@
 """
 This module is for logging and includes LogHelper class.
 """
 import logging
 import sys
+import threading
+from enum import Enum, auto
 from typing import List, Dict, Any
 
 
-class Levels:
+class Levels(Enum):
     """Class for constant values of logging levels """
-    CRITICAL = logging.CRITICAL
-    ERROR = logging.ERROR
-    WARNING = logging.WARNING
-    INFO = logging.INFO
-    DEBUG = logging.DEBUG
-    NOTSET = logging.NOTSET
+    CRITICAL = auto()
+    ERROR = auto()
+    WARNING = auto()
+    INFO = auto()
+    DEBUG = auto()
+    NOTSET = auto()
+
+
+_LEVELS_MAP = {
+    Levels.CRITICAL: logging.CRITICAL,
+    Levels.ERROR: logging.ERROR,
+    Levels.WARNING: logging.WARNING,
+    Levels.INFO: logging.INFO,
+    Levels.DEBUG: logging.DEBUG,
+    Levels.NOTSET: logging.NOTSET
+}
+_REVERSE_LEVELS_MAP = {value: key for key, value in _LEVELS_MAP.items()}
 
 
 class LogCallerInfo:
     """Stores FrameInfo information"""
 
     def __init__(self):
         self.frame = None
@@ -53,16 +66,19 @@
         self._style._fmt = self.__get_format(record.levelno)
         result = super().format(record)
         self._style._fmt = original_fmt
         return result
 
     def __get_format(self, levelno: int):
         """Returns format corresponding to given level"""
-        if levelno in self.level_formats and self.level_formats[levelno] is not None:
-            return self.level_formats[levelno]
+        level = None
+        if levelno in _REVERSE_LEVELS_MAP:
+            level = _REVERSE_LEVELS_MAP[levelno]
+        if level in self.level_formats and self.level_formats[level] is not None:
+            return self.level_formats[level]
         return self.default_format
 
     def set_default_format(self, format_str: str):
         """Sets default format"""
         self.default_format = format_str
 
     def set_level_format(self, level, format_str: str):
@@ -75,87 +91,77 @@
             self.level_formats[level] = format_str
 
 
 class LogHelper:
     """
     Includes static methods for logging.
     """
-    Levels = Levels
     level = Levels.INFO
     default_format = "[%(asctime)s] [%(threadName)s] %(levelname)-8s %(module_name)s:%(line_number)s - %(message)s"
     default_file = "application.log"
     log_formatter = OrganonFormatter(default_format, "%Y-%m-%d %H:%M:%S")
     global_extras: Dict[str, Any] = {}
     handlers: List[logging.Handler] = []
 
+    INITIALIZED = False
+    __init_lock = threading.Lock()
+
     @staticmethod
-    def initialize(format_str: str = default_format, file_path: str = default_file, log_to_console: bool = True,
-                   log_level: int = Levels.INFO):
+    def initialize(root_logger_format_str: str = default_format, file_path: str = default_file,
+                   log_to_console: bool = True, root_logger_level: Levels = None, log_to_file: bool = False):
         """
         Adds file and console_apps handlers. Sets minimum log level and log format
-        :param format_str: Format of logs.
-        :type format_str: str
+        :param root_logger_format_str: Format of logs.
+        :type root_logger_format_str: str
         :param file_path: Path to log file.
         :type file_path: str
         :param log_to_console: Set to true if logs should be printed to console_apps
         :type log_to_console: bool
-        :param log_level: Minimum level of messages to be logged. (Default=LogHelper.Levels.INFO)
-        :type log_level: int
-        """
-        LogHelper.reset()
-        LogHelper.set_level(log_level)
-        LogHelper.set_default_format(format_str)
-        LogHelper.add_default_file_handler(file_path)
-        if log_to_console:
-            LogHelper.add_default_console_handler()
-
-    @staticmethod
-    def reset():
-        """Resets settings"""
-        LogHelper.handlers = []
-        LogHelper.set_default_format(LogHelper.default_format)
-        LogHelper.set_level(LogHelper.Levels.INFO)
-
-    @staticmethod
-    def set_level(level):
-        """
-        Sets level of loggers
-        :param level: logging levels (LogHelper.Levels.INFO, LogHelper.Levels.DEBUG etc.)
-        """
-        LogHelper.level = level
+        :param log_to_file: Set to true if logs should be printed to file (application.log by default)
+        :type log_to_file: bool
+        :param root_logger_level: Minimum level of messages to be logged for root logger.
+        :type root_logger_level: int
+        """
+        with LogHelper.__init_lock:
+            if LogHelper.INITIALIZED:
+                raise ValueError("LogHelper already initialized!")
+            if root_logger_level is not None:
+                LogHelper.set_logger_level(root_logger_level)
+            LogHelper.set_default_formatter_default_format_str(root_logger_format_str)
+            if log_to_file:
+                LogHelper.add_file_handler(file_path)
+            if log_to_console:
+                LogHelper.add_console_handler()
+            LogHelper.INITIALIZED = True
 
     @staticmethod
-    def add_default_file_handler(file_path: str):
+    def add_file_handler(file_path: str, logger_name: str = None):
         """
         Sets file where logs will appear
         :param file_path: path to log file
         :type file_path: str
         """
         file_handler = logging.FileHandler(file_path, encoding="utf-8")
-        if LogHelper.log_formatter:
-            file_handler.setFormatter(LogHelper.log_formatter)
-        LogHelper.add_handler(file_handler)
+        LogHelper._add_handler_to_logger(file_handler, logger_name)
 
     @staticmethod
-    def add_default_console_handler():
+    def add_console_handler(logger_name: str = None):
         """
         Add console_apps handler to loggers
         """
         stream_handler = logging.StreamHandler()
-        if LogHelper.log_formatter:
-            stream_handler.setFormatter(LogHelper.log_formatter)
-        LogHelper.add_handler(stream_handler)
+        LogHelper._add_handler_to_logger(stream_handler, logger_name)
 
     @staticmethod
-    def set_default_format(format_str: str):
-        """Sets default format of log formatter"""
+    def set_default_formatter_default_format_str(format_str: str):
+        """Sets default format of default log formatter"""
         LogHelper.log_formatter.set_default_format(format_str)
 
     @staticmethod
-    def set_level_format(level, format_str: str):
+    def set_default_formatter_format_str_for_level(level, format_str: str):
         """Sets format string of a level
         :param level: Level of which format string will be set (Levels.DEBUG, Levels.INFO etc)
         :param format_str: Format string to be set to given level
         :type format_str: str
         """
         LogHelper.log_formatter.set_level_format(level, format_str)
 
@@ -163,108 +169,112 @@
     def add_global_extra(key: str, value):
         """
         Adds a global extra, that is a global value to be logged with every log.
         """
         LogHelper.global_extras[key] = value
 
     @staticmethod
-    def add_handler(handler: logging.Handler, use_default_format: bool = True):
+    def _add_handler_to_logger(handler: logging.Handler, logger_name: str = None, use_default_format: bool = True):
         """Adds extra handlers to loggers"""
         if use_default_format:
             handler.setFormatter(LogHelper.log_formatter)
-        LogHelper.handlers.append(handler)
-        loggers = LogHelper.get_all_loggers()
-        for logger in loggers:
-            logger.addHandler(handler)
+        logger = LogHelper._get_logger(logger_name)
+        logger.addHandler(handler)
 
     @staticmethod
-    def get_all_loggers():
+    def _get_all_loggers():
         """Returns all loggers"""
         return [logging.getLogger(name) for name in logging.root.manager.loggerDict]  # pylint: disable=no-member
 
     @staticmethod
-    def __get_logger(name: str):
-        """Creates a logger"""
-        root_logger = logging.getLogger(name)
-        root_logger.setLevel(LogHelper.level)
-        if len(root_logger.handlers) == 0:
-            for handler in LogHelper.handlers:
-                root_logger.addHandler(handler)
+    def set_logger_level(level: Levels, logger_name: str = None):
+        """Sets logger level"""
+        logger = LogHelper._get_logger(logger_name)
+        logging_module_level = LogHelper._get_level_in_logging_module(level)
+        logger.setLevel(logging_module_level)
 
-        return root_logger
+    @staticmethod
+    def _get_root_logger():
+        return logging.getLogger(None)
+
+    @staticmethod
+    def _get_level_in_logging_module(level: Levels):
+        if level in _LEVELS_MAP:
+            return _LEVELS_MAP[level]
+        raise ValueError("Given level cannot be converted to a logging module level")
 
     @staticmethod
     def info(message: str):
         """
         Logs a message with level "INFO".
         :param message: Message to be logged.
         :type message: str
         """
         log_caller = get_log_caller_info()
-        logger = LogHelper.__get_logger(log_caller.module_name)
-        logger.info(message, extra=LogHelper.__get_extras(log_caller))
+        logger = LogHelper._get_logger(log_caller.module_name)
+        logger.info(message, extra=LogHelper._get_extras(log_caller))
 
     @staticmethod
     def debug(message):
         """
         Logs a message with level "DEBUG".
         :param message: Message to be logged.
         :type message: str
         """
         log_caller = get_log_caller_info()
-        logger = LogHelper.__get_logger(log_caller.module_name)
-        logger.debug(message, extra=LogHelper.__get_extras(log_caller))
+        logger = LogHelper._get_logger(log_caller.module_name)
+        logger.debug(message, extra=LogHelper._get_extras(log_caller))
 
     @staticmethod
     def warning(message):
         """
         Logs a message with level 'WARNING'.
         :param message: Message to be logged.
         :type message: str
         """
         log_caller = get_log_caller_info()
-        logger = LogHelper.__get_logger(log_caller.module_name)
-        logger.warning(message, extra=LogHelper.__get_extras(log_caller))
+        logger = LogHelper._get_logger(log_caller.module_name)
+        logger.warning(message, extra=LogHelper._get_extras(log_caller))
 
     @staticmethod
     def error(message):
         """
         Logs a message with level 'ERROR'.
         :param message: Message to be logged.
         :type message: str
         """
         log_caller = get_log_caller_info()
-        logger = LogHelper.__get_logger(log_caller.module_name)
-        logger.error(message, extra=LogHelper.__get_extras(log_caller))
+        logger = LogHelper._get_logger(log_caller.module_name)
+        logger.error(message, extra=LogHelper._get_extras(log_caller))
 
     @staticmethod
     def exception(message):
         """
         Logs a message with level 'ERROR' and also logs stack trace. Should only be called in an exception handler.
         :param message: Message to be logged.
         :type message: str
         """
         log_caller = get_log_caller_info()
-        logger = LogHelper.__get_logger(log_caller.module_name)
-        logger.exception(message, extra=LogHelper.__get_extras(log_caller))
+        logger = LogHelper._get_logger(log_caller.module_name)
+        logger.exception(message, extra=LogHelper._get_extras(log_caller))
         # message = ExceptionFormattingHelper.format_exception(exception)
 
     @staticmethod
     def critical(message):
         """
         Logs a message with level 'CRITICAL'.
         :param message: Message to be logged.
         :type message: str
         """
         log_caller = get_log_caller_info()
-        logger = LogHelper.__get_logger(log_caller.module_name)
-        logger.critical(message, extra=LogHelper.__get_extras(log_caller))
+        logger = LogHelper._get_logger(log_caller.module_name)
+        logger.critical(message, extra=LogHelper._get_extras(log_caller))
 
     @staticmethod
-    def __get_extras(log_caller_info: LogCallerInfo, except_list: List[str] = None):
+    def _get_extras(log_caller_info: LogCallerInfo, except_list: List[str] = None):
         """
         Adds extra values while logging to be used in format of log formatter
         :param log_caller_info:
         :param except_list: names of attributes in log_caller_info which should not exist in log message
         :return: dictionary of extra values
         """
         extras = {}
@@ -273,21 +283,22 @@
             if attr_val is not None:
                 if except_list is not None and attr in except_list:
                     extras[attr] = ""
                 else:
                     extras[attr] = attr_val
             else:
                 extras[attr] = ""
-
-        for key, value in LogHelper.global_extras.items():
-            # global_extras_str += "{0} ".format(str(value))
-            extras[key] = value
-
+        extras.update(LogHelper.global_extras)
         return extras
 
+    @staticmethod
+    def _get_logger(name: str = None):
+        """Creates a logger"""
+        return logging.getLogger(name)
+
 
 if hasattr(sys, '_getframe'):
     currentframe = lambda stack_index: sys._getframe(stack_index + 1)  # pylint: disable=protected-access
 else:
     def currentframe(stack_index):
         """Return the frame object for the caller's stack frame."""
         try:
```

### Comparing `autonon-0.3.0.post1/organon/fl/mathematics/businessobjects/sets/interval.py` & `autonon-0.4.0/organon/fl/mathematics/businessobjects/sets/interval.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/mathematics/businessobjects/sets/sum_triple.py` & `autonon-0.4.0/organon/fl/mathematics/businessobjects/sets/sum_triple.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/mathematics/businessobjects/tuple_generic_collection.py` & `autonon-0.4.0/organon/fl/mathematics/businessobjects/tuple_generic_collection.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/mathematics/helpers/dataframe_operations_factory.py` & `autonon-0.4.0/organon/fl/mathematics/helpers/dataframe_operations_factory.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 """This module includes DataFrameOperationsFactory class."""
+from organon.fl.core.businessobjects.dask_dataframe import DaskDataFrame
 from organon.fl.core.businessobjects.dataframe import DataFrame
 from organon.fl.core.businessobjects.dict_dataframe import DictDataFrame
 from organon.fl.core.businessobjects.idataframe import IDataFrame
+from organon.fl.mathematics.helpers.dask_dataframe_operations import DaskDataFrameOperations
 from organon.fl.mathematics.helpers.dict_dataframe_operations import DictDataFrameOperations
 from organon.fl.mathematics.helpers.pandas_dataframe_operations import PandasDataFrameOperations
 
 
 class DataFrameOperationsFactory:
     """Class for DataFrameOperationsFactory"""
 
     @staticmethod
     def get_dataframe_operations(df_obj: IDataFrame):
         """ check whether we have dask or not and return dask operations accordingly"""
         if isinstance(df_obj, DictDataFrame):
             return DictDataFrameOperations()
         if isinstance(df_obj, DataFrame):
             return PandasDataFrameOperations()
+        if isinstance(df_obj, DaskDataFrame):
+            return DaskDataFrameOperations()
         raise NotImplementedError
```

### Comparing `autonon-0.3.0.post1/organon/fl/mathematics/helpers/dict_dataframe_operations.py` & `autonon-0.4.0/organon/fl/mathematics/helpers/dict_dataframe_operations.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/mathematics/helpers/idataframe_operations.py` & `autonon-0.4.0/organon/fl/mathematics/helpers/idataframe_operations.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/mathematics/helpers/pandas_dataframe_operations.py` & `autonon-0.4.0/organon/fl/mathematics/helpers/pandas_dataframe_operations.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/mathematics/linearalgebra/IBlas.py` & `autonon-0.4.0/organon/fl/mathematics/linearalgebra/IBlas.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/mathematics/linearalgebra/MklFunctions.py` & `autonon-0.4.0/organon/fl/mathematics/linearalgebra/MklFunctions.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/mathematics/linearalgebra/blas_service_factory.py` & `autonon-0.4.0/organon/fl/mathematics/linearalgebra/blas_service_factory.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/mathematics/linearalgebra/enums.py` & `autonon-0.4.0/organon/fl/mathematics/linearalgebra/enums.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/mathematics/linearalgebra/scipy_blas_service.py` & `autonon-0.4.0/organon/fl/mathematics/linearalgebra/scipy_blas_service.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/mathematics/sweep/covariance_generator.py` & `autonon-0.4.0/organon/fl/mathematics/sweep/covariance_generator.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/mathematics/sweep/covariance_info.py` & `autonon-0.4.0/organon/fl/mathematics/sweep/covariance_info.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/mathematics/sweep/data_classes/linear_regression_algorithm_settings.py` & `autonon-0.4.0/organon/fl/mathematics/sweep/data_classes/linear_regression_algorithm_settings.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/mathematics/sweep/data_classes/linear_regression_results.py` & `autonon-0.4.0/organon/fl/mathematics/sweep/data_classes/linear_regression_results.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/mathematics/sweep/data_classes/linear_regression_step.py` & `autonon-0.4.0/organon/fl/mathematics/sweep/data_classes/linear_regression_step.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/mathematics/sweep/data_classes/selected_attribute.py` & `autonon-0.4.0/organon/fl/mathematics/sweep/data_classes/selected_attribute.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/mathematics/sweep/enums.py` & `autonon-0.4.0/organon/fl/mathematics/sweep/enums.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/mathematics/sweep/fast_model_builder.py` & `autonon-0.4.0/organon/fl/mathematics/sweep/fast_model_builder.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/mathematics/sweep/matrices/csc_matrix.py` & `autonon-0.4.0/organon/fl/mathematics/sweep/matrices/csc_matrix.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/mathematics/sweep/matrices/dense_matrix.py` & `autonon-0.4.0/organon/fl/mathematics/sweep/matrices/dense_matrix.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/mathematics/sweep/matrices/i_matrix.py` & `autonon-0.4.0/organon/fl/mathematics/sweep/matrices/i_matrix.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/mathematics/sweep/pyx_files/sweep_helper.pyx` & `autonon-0.4.0/organon/fl/mathematics/sweep/pyx_files/sweep_helper.pyx`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/mathematics/sweep/sweep_operator.py` & `autonon-0.4.0/organon/fl/mathematics/sweep/sweep_operator.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/security/helpers/encryption_helper.py` & `autonon-0.4.0/organon/fl/security/helpers/encryption_helper.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/fl/serialization/serialization_helper.py` & `autonon-0.4.0/organon/fl/serialization/serialization_helper.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/core/dq_constants.py` & `autonon-0.4.0/organon/idq/core/dq_constants.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/core/enums/dq_comparison_result_code.py` & `autonon-0.4.0/organon/idq/core/enums/dq_comparison_result_code.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/core/enums/dq_test_type.py` & `autonon-0.4.0/organon/idq/core/enums/dq_test_type.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/dataaccess/helpers/record_source_filter_helper.py` & `autonon-0.4.0/organon/idq/dataaccess/helpers/record_source_filter_helper.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/dataaccess/record_source_reader.py` & `autonon-0.4.0/organon/idq/dataaccess/record_source_reader.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/algorithms/objects/base_comparison_input.py` & `autonon-0.4.0/organon/idq/domain/algorithms/objects/base_comparison_input.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/algorithms/objects/mean_ci_comparison_input.py` & `autonon-0.4.0/organon/idq/domain/algorithms/objects/mean_ci_comparison_input.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/algorithms/objects/time_series_comparison_input.py` & `autonon-0.4.0/organon/idq/domain/algorithms/objects/time_series_comparison_input.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/algorithms/objects/traffic_light_comparison_input.py` & `autonon-0.4.0/organon/idq/domain/algorithms/objects/traffic_light_comparison_input.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/businessobjects/data_column/dq_data_column.py` & `autonon-0.4.0/organon/idq/domain/businessobjects/data_column/dq_data_column.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/businessobjects/dq_calculation_output.py` & `autonon-0.4.0/organon/idq/domain/businessobjects/dq_calculation_output.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/businessobjects/dq_calculation_result.py` & `autonon-0.4.0/organon/idq/domain/businessobjects/dq_calculation_result.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """todo"""
 from typing import Optional
 
 from organon.fl.core.businessobjects.dataframe import DataFrame
+from organon.idq.domain.businessobjects.statistics.data_source_statistics import DataSourceStatistics
 from organon.idq.domain.businessobjects.statistics.population_statistics import PopulationStatistics
 from organon.idq.domain.businessobjects.statistics.sample_statistics import SampleStatistics
-from organon.idq.domain.businessobjects.statistics.data_source_statistics import DataSourceStatistics
 
 
 class DqCalculationResult:
     """todo"""
 
     def __init__(self):
         self.calculation_name: str = None
         self.data_source_stats: Optional[DataSourceStatistics] = None
         self.sample_stats: Optional[SampleStatistics] = None
         self.population_stats: Optional[PopulationStatistics] = None
         self.sample_data: Optional[DataFrame] = None
+        self.column_metadata_list = None
```

### Comparing `autonon-0.3.0.post1/organon/idq/domain/businessobjects/dq_comparison_result.py` & `autonon-0.4.0/organon/idq/domain/businessobjects/dq_comparison_result.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/businessobjects/dq_control_parameters.py` & `autonon-0.4.0/organon/idq/domain/businessobjects/dq_control_parameters.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/businessobjects/dq_data_column_collection.py` & `autonon-0.4.0/organon/idq/domain/businessobjects/dq_data_column_collection.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/businessobjects/record_sources/dq_base_record_source.py` & `autonon-0.4.0/organon/idq/domain/businessobjects/record_sources/dq_base_record_source.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/businessobjects/record_sources/dq_df_record_source.py` & `autonon-0.4.0/organon/idq/domain/businessobjects/record_sources/dq_df_record_source.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/businessobjects/record_sources/dq_file_record_source.py` & `autonon-0.4.0/organon/idq/domain/businessobjects/record_sources/dq_file_record_source.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/businessobjects/statistics/dq_categorical_statistics.py` & `autonon-0.4.0/organon/idq/domain/businessobjects/statistics/dq_categorical_statistics.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/businessobjects/statistics/dq_population_numerical_statistics.py` & `autonon-0.4.0/organon/idq/domain/businessobjects/statistics/dq_population_numerical_statistics.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/businessobjects/statistics/dq_sample_numerical_statistics.py` & `autonon-0.4.0/organon/idq/domain/businessobjects/statistics/dq_sample_numerical_statistics.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/businessobjects/statistics/population_statistics.py` & `autonon-0.4.0/organon/idq/domain/businessobjects/statistics/population_statistics.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/controls/base_dq_control.py` & `autonon-0.4.0/organon/idq/domain/controls/base_dq_control.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/controls/base_psi_signal_control.py` & `autonon-0.4.0/organon/idq/domain/controls/base_psi_signal_control.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/controls/column_mean_control.py` & `autonon-0.4.0/organon/idq/domain/controls/column_mean_control.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/controls/data_source_stats_time_series_control.py` & `autonon-0.4.0/organon/idq/domain/controls/data_source_stats_time_series_control.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/controls/data_source_stats_traffic_light_control.py` & `autonon-0.4.0/organon/idq/domain/controls/data_source_stats_traffic_light_control.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/controls/duplicate_keys_control.py` & `autonon-0.4.0/organon/idq/domain/controls/duplicate_keys_control.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/controls/empty_table_control.py` & `autonon-0.4.0/organon/idq/domain/controls/empty_table_control.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/controls/helpers/algorithms/base_predictor.py` & `autonon-0.4.0/organon/idq/domain/controls/helpers/algorithms/base_predictor.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/controls/helpers/algorithms/predictor_factory.py` & `autonon-0.4.0/organon/idq/domain/controls/helpers/algorithms/predictor_factory.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/controls/helpers/algorithms/random_forest_predictor.py` & `autonon-0.4.0/organon/idq/domain/controls/helpers/algorithms/random_forest_predictor.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/controls/helpers/column_values_comparer.py` & `autonon-0.4.0/organon/idq/domain/controls/helpers/column_values_comparer.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/controls/helpers/comparison_helper_functions.py` & `autonon-0.4.0/organon/idq/domain/controls/helpers/comparison_helper_functions.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/controls/helpers/psi_comparer.py` & `autonon-0.4.0/organon/idq/domain/controls/helpers/psi_comparer.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/controls/helpers/traffic_light_comparer.py` & `autonon-0.4.0/organon/idq/domain/controls/helpers/traffic_light_comparer.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/controls/psi_nominal_signal_control.py` & `autonon-0.4.0/organon/idq/domain/controls/psi_nominal_signal_control.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/controls/psi_numeric_signal_control.py` & `autonon-0.4.0/organon/idq/domain/controls/psi_numeric_signal_control.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/controls/stable_column_control.py` & `autonon-0.4.0/organon/idq/domain/controls/stable_column_control.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/controls/table_columns_control.py` & `autonon-0.4.0/organon/idq/domain/controls/table_columns_control.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/controls/unexpected_nominal_values_control.py` & `autonon-0.4.0/organon/idq/domain/controls/unexpected_nominal_values_control.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/controls/unexpected_numerical_values_control.py` & `autonon-0.4.0/organon/idq/domain/controls/unexpected_numerical_values_control.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/enums/dq_control_type.py` & `autonon-0.4.0/organon/idq/domain/enums/dq_control_type.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/helpers/statistics/dq_statistical_functions.py` & `autonon-0.4.0/organon/idq/domain/helpers/statistics/dq_statistical_functions.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/reporting/base_dq_report_helper.py` & `autonon-0.4.0/organon/idq/domain/reporting/base_dq_report_helper.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/reporting/base_multiple_calculation_report_helper.py` & `autonon-0.4.0/organon/idq/domain/reporting/base_multiple_calculation_report_helper.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/reporting/dq_reporting_executor.py` & `autonon-0.4.0/organon/idq/domain/reporting/dq_reporting_executor.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/reporting/objects/base_alert_info.py` & `autonon-0.4.0/organon/idq/domain/reporting/objects/base_alert_info.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/reporting/objects/base_dq_output_report.py` & `autonon-0.4.0/organon/idq/domain/reporting/objects/base_dq_output_report.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/reporting/objects/base_dq_report_helper_params.py` & `autonon-0.4.0/organon/idq/domain/reporting/objects/base_dq_report_helper_params.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/reporting/objects/base_multiple_calculation_report_helper_params.py` & `autonon-0.4.0/organon/idq/domain/reporting/objects/base_multiple_calculation_report_helper_params.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/reporting/objects/dq_comparison_sample_report_input.py` & `autonon-0.4.0/organon/idq/domain/reporting/objects/dq_comparison_sample_report_input.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/reporting/objects/nominal_column_control_details.py` & `autonon-0.4.0/organon/idq/domain/reporting/objects/nominal_column_control_details.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/reporting/objects/numeric_column_control_details.py` & `autonon-0.4.0/organon/idq/domain/reporting/objects/numeric_column_control_details.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/reporting/objects/signal_details.py` & `autonon-0.4.0/organon/idq/domain/reporting/objects/signal_details.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/reporting/objects/source_with_partitions_alert_info.py` & `autonon-0.4.0/organon/idq/domain/reporting/objects/source_with_partitions_alert_info.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/reporting/objects/source_with_partitions_dq_report_output.py` & `autonon-0.4.0/organon/idq/domain/reporting/objects/source_with_partitions_dq_report_output.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/reporting/objects/source_with_partitions_report_helper_params.py` & `autonon-0.4.0/organon/idq/domain/reporting/objects/source_with_partitions_report_helper_params.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/reporting/objects/table_control_details.py` & `autonon-0.4.0/organon/idq/domain/reporting/objects/table_control_details.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/reporting/single_source_report_helper.py` & `autonon-0.4.0/organon/idq/domain/reporting/single_source_report_helper.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/reporting/source_with_partitions_report_helper.py` & `autonon-0.4.0/organon/idq/domain/reporting/source_with_partitions_report_helper.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/services/base_user_input_service.py` & `autonon-0.4.0/organon/idq/domain/services/base_user_input_service.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/services/base_user_input_validation_service.py` & `autonon-0.4.0/organon/idq/domain/services/base_user_input_validation_service.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/services/dq_full_process_executor.py` & `autonon-0.4.0/organon/idq/domain/services/dq_full_process_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,18 +103,17 @@
     def _get_run_type(self) -> DqRunType:
         # todo
         if len(self.dq_settings.calculation_parameters) == 1:
             return DqRunType.RUN_ONE_DATA_SOURCE
         return DqRunType.RUN_ONE_DATA_SOURCE_WITH_PARTITIONS
 
     def __decide_comparison_columns(self, t_calc_result: DqCalculationResult):
-        t_calc_params = self.dq_settings.calculation_parameters[-1]
         comp_cols_dict: Dict[str, DqComparisonColumnInfo] = \
             {col.column_name: col for col in self.dq_settings.comparison_parameters.comparison_columns}
-        meta_dict: Dict[str, DqColumnMetadata] = {col.column_name: col for col in t_calc_params.column_dq_metadata_list}
+        meta_dict: Dict[str, DqColumnMetadata] = {col.column_name: col for col in t_calc_result.column_metadata_list}
         duplicate_column_control_default = False
         bh_default = len(self.dq_settings.calculation_parameters) - 1
         for col in t_calc_result.data_source_stats.data_column_collection:
             if col.column_name in meta_dict and meta_dict[col.column_name].inclusion_flag:
                 if col.column_name in comp_cols_dict:
                     comp_col = comp_cols_dict[col.column_name]
                     comp_col.duplicate_column_control = duplicate_column_control_default \
```

### Comparing `autonon-0.3.0.post1/organon/idq/domain/services/output/dq_output_persistence_service.py` & `autonon-0.4.0/organon/idq/domain/services/output/dq_output_persistence_service.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/services/statistics/dq_statistics_domain_service.py` & `autonon-0.4.0/organon/idq/domain/services/statistics/dq_statistics_domain_service.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/services/statistics/source_statistics/df_source_stats_service.py` & `autonon-0.4.0/organon/idq/domain/services/statistics/source_statistics/df_source_stats_service.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/services/statistics/source_statistics/dq_source_stats_base_service.py` & `autonon-0.4.0/organon/idq/domain/services/statistics/source_statistics/dq_source_stats_base_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
                                           data_col_collection: DqDataColumnCollection) \
             -> Dict[str, DqCategoricalStatistics]:
         """Get statistics for nominal columns in data"""
 
         filtered_metadata = [col_meta for col_meta in self.calc_params.column_dq_metadata_list
                              if col_meta.inclusion_flag and col_meta.column_name in nominal_column_names]
         dq_columns = {col.column_name: col for col in data_col_collection
-                            if col.column_name in [meta.column_name for meta in filtered_metadata]}
+                      if col.column_name in [meta.column_name for meta in filtered_metadata]}
         all_stats = {}
         histograms = {}
         if len(dq_columns) > 0:
             histograms = self._get_histograms_for_columns(dq_columns)
         for col_meta in filtered_metadata:
             col_name = col_meta.column_name
             missing_values = col_meta.default_values
@@ -99,14 +99,15 @@
                 raise KnownException("Column not in dataframe")
             col_native_type = data_columns[col.column_name].column_native_type
             if col_native_type == ColumnNativeType.Numeric:
                 numerical_cols.append(col)
             elif col_native_type in self.calc_params.nominal_column_types:
                 categorical_cols.append(col)
         missing_values = {col.column_name: col.default_values for col in categorical_cols}
+
         stats = DqStatisticsDomainService.compute_categorical_statistics(data, missing_values)
         sample_stats = SampleStatistics()
         sample_stats.nominal_statistics = {col_name: stat for col_name, stat in stats.items()
                                            if stat.cardinality <= self.calc_params.max_nominal_cardinality_count}
         default_values_by_col = {col.column_name: self.__get_default_values(col.default_values)
                                  for col in numerical_cols}
         sample_stats.numerical_statistics = \
@@ -126,19 +127,19 @@
             if math.isnan(float_val):
                 nan_exists = True
             float_vals.append(float_val)
         if not nan_exists:
             float_vals.append(float("nan"))
         return float_vals
 
-    def update_calc_params(self, col_collection: DqDataColumnCollection):
+    def update_calc_params(self, col_collection: DqDataColumnCollection) -> List[DqColumnMetadata]:
         """Updates calculation metadata list using column info"""
-        self.__update_column_dq_metadata_list(col_collection)
+        return self.__update_column_dq_metadata_list(col_collection)
 
-    def __update_column_dq_metadata_list(self, col_collection: DqDataColumnCollection):
+    def __update_column_dq_metadata_list(self, col_collection: DqDataColumnCollection) -> List[DqColumnMetadata]:
         """Updates calculation metadata list using column info"""
         calc_params = self.calc_params
         col_meta_dict: Dict[str, DqColumnMetadata] = {col.column_name: col for col in
                                                       calc_params.column_dq_metadata_list}
         eligible_types = [ColumnNativeType.Numeric] + calc_params.nominal_column_types
         for col in col_collection:
             if col.column_native_type in eligible_types:
@@ -152,8 +153,10 @@
                     new_meta.column_name = col.column_name
                     new_meta.inclusion_flag = True
                     new_meta.default_values = []
                     col_meta_dict[col.column_name] = new_meta
             else:
                 if col.column_name in col_meta_dict:
                     col_meta_dict.pop(col.column_name)
-        self.calc_params.column_dq_metadata_list = list(col_meta_dict.values())
+        metadata_list = list(col_meta_dict.values())
+        self.calc_params.column_dq_metadata_list = metadata_list
+        return metadata_list
```

### Comparing `autonon-0.3.0.post1/organon/idq/domain/services/statistics/source_statistics/file_source_stats_service.py` & `autonon-0.4.0/organon/idq/domain/services/statistics/source_statistics/file_source_stats_service.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/services/task_executor/calculation/dq_calculation_task_executor.py` & `autonon-0.4.0/organon/idq/domain/services/task_executor/calculation/dq_calculation_task_executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from organon.idq.domain.services.statistics.source_statistics.df_source_stats_service import DfSourceStatsService
 from organon.idq.domain.services.statistics.source_statistics.dq_source_stats_base_service import \
     DqSourceStatsBaseService
 from organon.idq.domain.services.statistics.source_statistics.file_source_stats_service import FileSourceStatsService
 from organon.idq.domain.settings.abstractions.dq_base_calculation_parameters import DqBaseCalculationParameters
 from organon.idq.domain.settings.calculation.dq_df_calculation_parameters import DqDfCalculationParameters
 from organon.idq.domain.settings.calculation.dq_file_calculation_parameters import DqFileCalculationParameters
+from organon.idq.domain.settings.dq_column_metadata import DqColumnMetadata
 
 
 class DqCalculationTaskExecutor:
     """Executes dq calculations with given parameters"""
 
     def __init__(self, calculation_parameters: DqBaseCalculationParameters,
                  run_type: DqRunType, is_test_calculation: bool = False):
@@ -44,18 +45,20 @@
 
         sample_data = self._get_sample_data()
         data_col_collection = self._get_data_column_collection(sample_data)
         self._update_params_with_column_collection(data_col_collection)
         sample_stats = self._compute_sample_stats(sample_data, data_col_collection)
         filtered_columns = self._filter_high_cardinality_columns(data_col_collection)
         population_nominal_stats = self._get_population_nominal_stats(filtered_columns, data_col_collection)
+        columns_metadata_list = self._update_params_with_column_collection(data_col_collection)
 
         result.data_source_stats.data_column_collection = data_col_collection
         result.data_source_stats.row_count = sample_data.full_data_row_count
         result.sample_stats = sample_stats
+        result.column_metadata_list = columns_metadata_list
         result.population_stats.nominal_statistics = population_nominal_stats
 
         if self.is_test_calculation:
             result.sample_data = DataFrame()
             result.sample_data.data_frame = sample_data.sampled_data
 
         return result
@@ -76,16 +79,17 @@
         record_source_reader = RecordSourceReader(self.calculation_parameters.input_source_settings)
         return record_source_reader.read()
 
     def _compute_sample_stats(self, sample_data: DqDataSource, data_column_collection: DqDataColumnCollection) \
             -> SampleStatistics:
         return self.stats_service.get_sample_stats(sample_data.sampled_data, data_column_collection)
 
-    def _update_params_with_column_collection(self, data_column_collection: DqDataColumnCollection):
-        self.stats_service.update_calc_params(data_column_collection)
+    def _update_params_with_column_collection(self, data_column_collection: DqDataColumnCollection) \
+            -> List[DqColumnMetadata]:
+        return self.stats_service.update_calc_params(data_column_collection)
 
     def _filter_high_cardinality_columns(self, data_column_collection: DqDataColumnCollection) -> List[str]:
         return self.stats_service.filter_high_cardinality_columns(data_column_collection)
 
     def _get_population_nominal_stats(self, filtered_columns: List[str],
                                       data_column_collection: DqDataColumnCollection):
         return self.stats_service.get_population_nominal_statistics(filtered_columns, data_column_collection)
```

### Comparing `autonon-0.3.0.post1/organon/idq/domain/services/task_executor/comparison/dq_comparison_task_executor.py` & `autonon-0.4.0/organon/idq/domain/services/task_executor/comparison/dq_comparison_task_executor.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/services/user_input_service.py` & `autonon-0.4.0/organon/idq/domain/services/user_input_service.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/services/user_input_validation_service.py` & `autonon-0.4.0/organon/idq/domain/services/user_input_validation_service.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/settings/abstractions/dq_base_calculation_parameters.py` & `autonon-0.4.0/organon/idq/domain/settings/abstractions/dq_base_calculation_parameters.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/settings/abstractions/dq_base_comparison_parameters.py` & `autonon-0.4.0/organon/idq/domain/settings/abstractions/dq_base_comparison_parameters.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/settings/abstractions/dq_base_input_source_settings.py` & `autonon-0.4.0/organon/idq/domain/settings/abstractions/dq_base_input_source_settings.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/settings/abstractions/dq_full_process_input.py` & `autonon-0.4.0/organon/idq/domain/settings/abstractions/dq_full_process_input.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Includes DqFullProcessInput class."""
 from typing import List, TypeVar, Generic
 
 from organon.idq.domain.settings.abstractions.dq_base_calculation_parameters import DqBaseCalculationParameters
 from organon.idq.domain.settings.abstractions.dq_base_comparison_parameters import DqBaseComparisonParameters
+from organon.idq.domain.settings.dask_settings import DaskSettings
 from organon.idq.domain.settings.dq_notification_settings import DqNotificationSettings
 from organon.idq.domain.settings.dq_output_settings import DqOutputSettings
 
 T1 = TypeVar("T1", bound=DqBaseCalculationParameters)
 T2 = TypeVar("T2", bound=DqBaseComparisonParameters)
 
 
@@ -15,7 +16,8 @@
 
     def __init__(self):
         self.calculation_parameters: List[T1] = None
         self.comparison_parameters: T2 = None
         self.use_supplied_calcs_as_comp_inputs: bool = None
         self.notification_settings: DqNotificationSettings = None
         self.output_settings: DqOutputSettings = None
+        self.dask_settings: DaskSettings = None
```

### Comparing `autonon-0.3.0.post1/organon/idq/domain/settings/date_value_definition.py` & `autonon-0.4.0/organon/idq/domain/settings/date_value_definition.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/settings/full_process/dq_df_full_process_input.py` & `autonon-0.4.0/organon/idq/domain/settings/full_process/dq_df_full_process_input.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/settings/full_process/dq_file_full_process_input.py` & `autonon-0.4.0/organon/idq/domain/settings/full_process/dq_file_full_process_input.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/settings/input_source/dq_file_input_source_settings.py` & `autonon-0.4.0/organon/idq/domain/settings/input_source/dq_file_input_source_settings.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/domain/settings/partition_info.py` & `autonon-0.4.0/organon/idq/domain/settings/partition_info.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/services/base_idq_executor.py` & `autonon-0.4.0/organon/idq/services/base_idq_executor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Includes IDQ class."""
 import abc
 from typing import Optional, List, TypeVar, Generic, Dict
 
+import organon
+from organon.common.helpers import dev_mode_helper
 from organon.fl.core.exceptionhandling.known_exception import KnownException
 from organon.idq.core.dq_constants import DqConstants
 from organon.idq.domain.businessobjects.dq_calculation_output import DqCalculationOutput
 from organon.idq.domain.reporting.objects.base_dq_output_report import BaseDqOutputReport
 from organon.idq.domain.services.base_user_input_service import BaseUserInputService
 from organon.idq.domain.services.dq_full_process_executor import DqFullProcessExecutor
 from organon.idq.domain.settings.abstractions.dq_full_process_input import DqFullProcessInput
@@ -15,38 +17,43 @@
 UserInputServiceType = TypeVar("UserInputServiceType", bound=BaseUserInputService)
 DqUserInputType = TypeVar("DqUserInputType", bound=BaseDqUserInput)
 
 
 class BaseIDQ(Generic[UserInputServiceType, DqUserInputType], metaclass=abc.ABCMeta):
     """User service class for IDQ."""
 
-    def __init__(self, log_to_console: bool = False):
-        self._initialize_idq(log_to_console)
+    def __init__(self):
+        self._initialize_idq()
         self.results: Optional[BaseDqOutputReport] = None
         self.calculation_outputs: Optional[List[DqCalculationOutput]] = None
         self._user_settings: DqUserInputType = self._get_user_settings_instance()
 
     @abc.abstractmethod
     def _get_user_settings_instance(self) -> DqUserInputType:
         """Returns empty DqUserInput instance"""
 
     @classmethod
-    def _initialize_idq(cls, log_to_console: bool):
-        IdqApplicationOperations.initialize_app(log_to_console)
+    def _initialize_idq(cls):
+        IdqApplicationOperations.initialize_app()
 
     def execute(self) -> BaseDqOutputReport:
         """Executes idq and returns results"""
         helper = self._get_user_input_service()
         full_process_input = helper.convert_to_full_process_input()
         executor = self._get_dq_full_process_executor(full_process_input)
         results, calculation_results = executor.execute()
         self.results = results
         self.calculation_outputs = calculation_results
         return results
 
+    @classmethod
+    def init_dev_mode(cls, log_to_console: bool = True, log_file: str = "application.log"):
+        """Initializes development mode."""
+        dev_mode_helper.init_dev_mode(organon.idq.__name__, log_to_console=log_to_console, log_file=log_file)
+
     @abc.abstractmethod
     def _get_user_input_service(self) -> UserInputServiceType:
         """Returns UserInputService instance"""
 
     @classmethod
     def _get_dq_full_process_executor(cls, full_process_input: DqFullProcessInput) -> DqFullProcessExecutor:
         return DqFullProcessExecutor(full_process_input)
```

### Comparing `autonon-0.3.0.post1/organon/idq/services/idq_executor.py` & `autonon-0.4.0/organon/idq/services/idq_executor.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/services/user_settings/base_dq_user_input.py` & `autonon-0.4.0/organon/idq/services/user_settings/base_dq_user_input.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/services/user_settings/base_user_calculation_params.py` & `autonon-0.4.0/organon/idq/services/user_settings/base_user_calculation_params.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/services/user_settings/dq_user_input.py` & `autonon-0.4.0/organon/idq/services/user_settings/dq_user_input.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/services/user_settings/user_calculation_params.py` & `autonon-0.4.0/organon/idq/services/user_settings/user_calculation_params.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/services/user_settings/user_input_source_settings.py` & `autonon-0.4.0/organon/idq/services/user_settings/user_input_source_settings.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/idq/services/user_settings/user_multi_partition_calculation_params.py` & `autonon-0.4.0/organon/idq/services/user_settings/user_multi_partition_calculation_params.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/common/helpers/df_ops_helper.py` & `autonon-0.4.0/organon/ml/common/helpers/df_ops_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from organon.fl.core.helpers import list_helper
 
 
 def get_train_test_split(data: pd.DataFrame, test_ratio: float, strata_columns: List[str] = None, random_state=None):
     """Divides given data to two splits(train and test) using given ratio"""
     if test_ratio > 1.0:
         raise ValueError("test_ratio cannot be higher than 1.0")
-    test_indices = get_sample_indices(data, test_ratio, strata_columns, random_state)
+    test_indices = get_sample_indices(data, test_ratio, strata_columns=strata_columns, random_state=random_state)
     train_data = data.loc[data.index.difference(test_indices)]
     return train_data, data.loc[test_indices]
 
 
 def get_train_test_split_from_strata(data: pd.DataFrame, strata_data: pd.Series, test_ratio: float, random_state=None):
     """Divides given data to two splits(train and test) using given ratio"""
     if test_ratio > 1.0:
```

### Comparing `autonon-0.3.0.post1/organon/ml/common/helpers/user_input_service_helper.py` & `autonon-0.4.0/organon/ml/common/helpers/user_input_service_helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,16 @@
     return value if value is not None else default_value
 
 
 def get_enum(enum_str: str, enum_class: Type[T]) -> T:
     """Converts string to enum """
     if enum_str is None:
         return None
-    valid_values = [e.name for e in enum_class]
-    if enum_str not in valid_values:
-        raise KnownException(
-            f"Invalid value for enum '{enum_class.__name__}'."
-            f"Expected one of: {str(valid_values)} Got: '{enum_str}'")
-    value = enum_class[enum_str]
-    return value
+
+    valid_values = {e.name.upper(): e for e in enum_class}
+
+    if enum_str.upper() in valid_values:
+        return valid_values[enum_str.upper()]
+
+    raise KnownException(
+        f"Invalid value for enum '{enum_class.__name__}'."
+        f"Expected one of: {str(list(valid_values.keys()))} Got: '{enum_str}'")
```

### Comparing `autonon-0.3.0.post1/organon/ml/common/helpers/validation_helper.py` & `autonon-0.4.0/organon/ml/common/helpers/validation_helper.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/feature_reduction/domain/objects/numeric_column_stats.py` & `autonon-0.4.0/organon/ml/feature_reduction/domain/objects/numeric_column_stats.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/feature_reduction/domain/reductions/null_feature_reduction.py` & `autonon-0.4.0/organon/ml/feature_reduction/domain/reductions/null_feature_reduction.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,25 +9,34 @@
 from organon.ml.feature_reduction.settings.objects.null_feature_reduction_settings import NullFeatureReductionSettings
 
 
 class NullFeatureReduction(BaseFeatureReduction):
     """ NullFeatureReduction class"""
 
     def _execute_reduction(self, settings: NullFeatureReductionSettings) -> FeatureReductionOutput:
-        missing_df = self._calculate_null_ratio(data=settings.data)
-        reduced_columns = self._find_reduced_columns(missing_df, settings.null_ratio_threshold)
-        settings.data.drop(reduced_columns, axis=1, inplace=True)
         output = FeatureReductionOutput()
+        included_columns = self._get_included_columns(settings.data, settings.excluded_columns)
+        missing_df = self._calculate_null_ratio(settings.data, included_columns)
         output.feature_reduction_type = FeatureReductionType.NULL
+
+        if missing_df is None:
+            output.reduced_column_list = None
+            return output
+
+        reduced_columns = self._find_reduced_columns(missing_df, settings.null_ratio_threshold)
         output.reduced_column_list = reduced_columns
         return output
 
     @staticmethod
-    def _calculate_null_ratio(data: pd.DataFrame) -> pd.DataFrame:
-        na_columns = [col for col in data.columns if data[col].isnull().sum() > 0]
+    def _calculate_null_ratio(data: pd.DataFrame, included_columns: List[str] = None):
+
+        if not included_columns:
+            return None
+
+        na_columns = [col for col in included_columns if data[col].isnull().sum() > 0]
 
         ratio = (data[na_columns].isnull().sum() / data.shape[0])
         missing_df = pd.DataFrame(ratio)
         missing_df.reset_index(inplace=True)
         missing_df.columns = ["columns", "ratio"]
         return missing_df
```

### Comparing `autonon-0.3.0.post1/organon/ml/feature_reduction/domain/reductions/similar_distribution_feature_reduction.py` & `autonon-0.4.0/organon/ml/feature_reduction/domain/reductions/similar_distribution_feature_reduction.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 """ This module includes SimilarDistributionFeatureReduction"""
-from typing import List, Dict
+from typing import List, Dict, Tuple, Optional
 
 import pandas as pd
-from lightgbm import LGBMClassifier, LGBMRegressor
-from sklearn.model_selection import cross_val_score
 
 from organon.fl.core.enums.column_native_type import ColumnNativeType
 from organon.fl.core.helpers.data_frame_helper import get_column_native_type
-from organon.ml.common.enums.target_type import TargetType
 from organon.ml.feature_reduction.domain.enums.feature_reduction_types import FeatureReductionType
-from organon.ml.feature_reduction.domain.objects.feature_reduction_output import FeatureReductionOutput
+from organon.ml.feature_reduction.domain.helpers.univariate_performance_helper import \
+    get_reduced_columns_via_performance
 from organon.ml.feature_reduction.domain.objects.numeric_column_stats import NumericColumnStats
+from organon.ml.feature_reduction.domain.objects.similar_dist_reduction_output import SimilarDistReductionOutput
 from organon.ml.feature_reduction.domain.reductions.base_feature_reduction import BaseFeatureReduction
 from organon.ml.feature_reduction.settings.objects.similar_distribution_feature_reduction_settings import \
     SimilarDistributionFeatureReductionSettings
 
 
 class SimilarDistributionFeatureReduction(BaseFeatureReduction):
     """SimilarDistributionFeatureReduction class"""
 
-    def _execute_reduction(self, settings: SimilarDistributionFeatureReductionSettings) -> FeatureReductionOutput:
+    def _execute_reduction(self, settings: SimilarDistributionFeatureReductionSettings) -> SimilarDistReductionOutput:
         data = settings.data
-        numeric_columns = [col for col in data.columns if
+        output = SimilarDistReductionOutput()
+        output.feature_reduction_type = FeatureReductionType.SIMILAR_DISTRIBUTION
+        included_columns = self._get_included_columns(data, settings.excluded_columns)
+        numeric_columns = [col for col in included_columns if
                            (get_column_native_type(data, col) == ColumnNativeType.Numeric)
                            and (col != settings.target_column_name)
                            and (data[col].nunique() > settings.nunique_count)]
+        if not numeric_columns:
+            output.reduced_column_list = None
+            return output
         numeric_columns_stats = self._get_stats(data, numeric_columns)
         similar_distribution_columns = self._get_similar_distribution_columns(numeric_columns_stats)
-        reduced_columns = self._find_reduced_columns(settings, similar_distribution_columns)
-        settings.data.drop(reduced_columns, axis=1, inplace=True)
-        output = FeatureReductionOutput()
-        output.feature_reduction_type = FeatureReductionType.SIMILAR_DISTRIBUTION
+        reduced_columns, new_col_performances = self._find_reduced_columns(settings, similar_distribution_columns)
         output.reduced_column_list = reduced_columns
+        output.new_univariate_performance_results = new_col_performances
         return output
 
     @staticmethod
     def _get_stats(data: pd.DataFrame, numeric_columns: List[str]) -> List[NumericColumnStats]:
         """
         Return numeric column stats which includes mean,std, percentile 25, percentile 50, percentile 75.
         Parameters
@@ -78,95 +81,44 @@
             column_list = []
             column_list.append(numeric_columns_stats[count].column_name)
             for j in range(count + 1, len(numeric_columns_stats)):
 
                 if numeric_columns_stats[count] == numeric_columns_stats[j]:
                     column_list.append(numeric_columns_stats[j].column_name)
                     similar_distribution_columns_set.add(numeric_columns_stats[j].column_name)
-
-            similar_distribution_columns[numeric_columns_stats[count].column_name] = column_list
+            if len(column_list) > 1:
+                similar_distribution_columns[numeric_columns_stats[count].column_name] = column_list
         return similar_distribution_columns
 
-    def _find_reduced_columns(self, settings: SimilarDistributionFeatureReductionSettings,
-                              similar_distribution_columns: Dict[str, List[str]]) -> List[str]:
+    @staticmethod
+    def _find_reduced_columns(settings: SimilarDistributionFeatureReductionSettings,
+                              similar_distribution_columns: Dict[str, List[str]]) -> \
+            Tuple[List[str], Optional[Dict[str, float]]]:
         """
         Find reduced columns.
         Parameters
         ----------
         settings
         similar_distribution_columns
         numeric_columns_list
 
         Returns
         -------
         Returns columns list which reduced.
         """
+        if len(similar_distribution_columns) == 0:
+            return [], None
         reduced_columns = []
         if settings.target_column_name is not None and settings.target_type is not None:
-            reduced_columns = self._get_reduced_columns_via_performance(settings, similar_distribution_columns)
-            return reduced_columns
+            reduced_columns, new_col_performances = get_reduced_columns_via_performance(
+                settings.data, settings.target_column_name, settings.target_type, settings.performance_metric,
+                list(similar_distribution_columns.values()), settings.univariate_performance_result,
+                random_state=settings.random_state)
+            return reduced_columns, new_col_performances
 
         for column_list in similar_distribution_columns.values():
             column_list.sort()
             reduced_columns.extend(column_list[1:])
-        return reduced_columns
-
-    @staticmethod
-    def _get_reduced_columns_via_performance(
-            settings: SimilarDistributionFeatureReductionSettings,
-            similar_distribution_columns: Dict[str, List[str]]) -> List[str]:
-        """
-        Finds the reduced column using the univariate performance result.
-        Parameters
-        ----------
-        settings
-        similar_distribution_columns
-
-        Returns
-        -------
-        Returns columns list which reduced.
-
-        """
-        data = settings.data
-        target_type = settings.target_type.name
-        target_column_name = settings.target_column_name
-
-        model = SimilarDistributionFeatureReduction._get_model(target_type, settings.random_state)
-
-        reduced_columns = []
-        for column_list in similar_distribution_columns.values():
-            score_result = {}
-            if settings.univariate_performance_result is None:
-                for column in column_list:
-                    score = cross_val_score(model, data[[column]], data[target_column_name], cv=3,
-                                            scoring=settings.performance_metric).mean()
-                    score_result[column] = score
-            else:
-                for column in column_list:
-                    score_result[column] = settings.univariate_performance_result[column]
-            best_score_column = max(score_result, key=score_result.get)
-            for column in column_list:
-                if column != best_score_column:
-                    reduced_columns.append(column)
-        return reduced_columns
-
-    @staticmethod
-    def _get_model(target_type: str, random_state: int):
-        """
-        Return Model with using target type.
-        Parameters
-        ----------
-        target_type
-
-        Returns
-        -------
-        Returns Model object for LGBM
-        """
-
-        if target_type in (TargetType.BINARY.name, TargetType.MULTICLASS.name):
-            model = LGBMClassifier(random_state=random_state)
-        else:
-            model = LGBMRegressor(random_state=random_state)
-        return model
+        return reduced_columns, None
 
     def get_description(self) -> str:
         return "Similar Distribution Feature Reduction"
```

### Comparing `autonon-0.3.0.post1/organon/ml/feature_reduction/domain/reductions/stability_feature_reduction.py` & `autonon-0.4.0/organon/ml/feature_reduction/domain/reductions/stability_feature_reduction.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,17 +6,23 @@
     StabilityFeatureReductionSettings
 
 
 class StabilityFeatureReduction(BaseFeatureReduction):
     """StabilityFeatureReduction class"""
 
     def _execute_reduction(self, settings: StabilityFeatureReductionSettings) -> FeatureReductionOutput:
-        data = settings.data
-        reduced_columns = [col for col in data.columns if len(data[col].value_counts()) == 1]
-        settings.data.drop(reduced_columns, axis=1, inplace=True)
         output = FeatureReductionOutput()
         output.feature_reduction_type = FeatureReductionType.STABILITY
+
+        included_columns = self._get_included_columns(settings.data, settings.excluded_columns)
+
+        if not included_columns:
+            output.reduced_column_list = None
+            return output
+
+        reduced_columns = [col for col in included_columns if len(settings.data[col].value_counts()) == 1]
+
         output.reduced_column_list = reduced_columns
         return output
 
     def get_description(self) -> str:
         return "Stability Feature Reduction"
```

### Comparing `autonon-0.3.0.post1/organon/ml/feature_reduction/domain/reductions/univariate_performance_feature_reduction.py` & `autonon-0.4.0/organon/ml/feature_reduction/domain/services/feature_reduction_service.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,103 +1,87 @@
-""" This module includes UnivariatePerformanceFeatureReduction"""
-from typing import List
+"""Includes FeatureReductionService class"""
+from typing import List, Dict
 
-from lightgbm import LGBMRegressor, LGBMClassifier
-from sklearn.model_selection import cross_val_score
+import pandas as pd
 
-from organon.fl.core.enums.column_native_type import ColumnNativeType
-from organon.fl.core.helpers.data_frame_helper import get_column_native_type
-from organon.ml.common.enums.target_type import TargetType
-from organon.ml.feature_reduction.domain.enums.feature_reduction_types import FeatureReductionType
 from organon.ml.feature_reduction.domain.objects.feature_reduction_output import FeatureReductionOutput
+from organon.ml.feature_reduction.domain.objects.high_corr_reduction_output import HighCorrReductionOutput
+from organon.ml.feature_reduction.domain.objects.similar_dist_reduction_output import SimilarDistReductionOutput
 from organon.ml.feature_reduction.domain.objects.univariate_performance_reduction_output import \
     UnivariatePerformanceFeatureReductionOutput
-from organon.ml.feature_reduction.domain.reductions.base_feature_reduction import BaseFeatureReduction
-
+from organon.ml.feature_reduction.domain.reductions.high_correlated_feature_reduction import \
+    HighCorrelatedFeatureReduction
+from organon.ml.feature_reduction.domain.reductions.null_feature_reduction import NullFeatureReduction
+from organon.ml.feature_reduction.domain.reductions.similar_distribution_feature_reduction import \
+    SimilarDistributionFeatureReduction
+from organon.ml.feature_reduction.domain.reductions.stability_feature_reduction import StabilityFeatureReduction
+from organon.ml.feature_reduction.domain.reductions.univariate_performance_feature_reduction import \
+    UnivariatePerformanceFeatureReduction
+from organon.ml.feature_reduction.settings.objects.base_feature_reduction_settings import BaseFeatureReductionSettings
+from organon.ml.feature_reduction.settings.objects.high_correlated_feature_reduction_settings import \
+    HighCorrelatedFeatureReductionSettings
+from organon.ml.feature_reduction.settings.objects.null_feature_reduction_settings import NullFeatureReductionSettings
+from organon.ml.feature_reduction.settings.objects.similar_distribution_feature_reduction_settings import \
+    SimilarDistributionFeatureReductionSettings
+from organon.ml.feature_reduction.settings.objects.stability_feature_reduction_settings import \
+    StabilityFeatureReductionSettings
 from organon.ml.feature_reduction.settings.objects.univariate_performance_feature_reduction_settings import \
     UnivariatePerformanceFeatureReductionSettings
 
 
-class UnivariatePerformanceFeatureReduction(BaseFeatureReduction):
-    """UnivariatePerformanceFeatureReduction class"""
-
-    def _execute_reduction(self, settings: UnivariatePerformanceFeatureReductionSettings) -> FeatureReductionOutput:
-        data = settings.data
-        numeric_columns = [col for col in data.columns if
-                           (get_column_native_type(data, col) == ColumnNativeType.Numeric)
-                           and (col != settings.target_column_name)]
-
-        output = self._find_reduced_columns(settings, numeric_columns)
-        settings.data.drop(output.reduced_column_list, axis=1, inplace=True)
-        return output
-
-    @staticmethod
-    def _find_reduced_columns(settings: UnivariatePerformanceFeatureReductionSettings,
-                              numeric_columns_list: List[str]) -> UnivariatePerformanceFeatureReductionOutput:
-        """
-        Find reduced columns with using numeric column univariate performance result
-        Parameters
-        ----------
-        settings
-        numeric_columns_list
-
-        Returns
-        -------
-        Return UnivariatePerformanceFeatureReductionOutput
-        """
-        data = settings.data
-        target_type = settings.target_type.name
-        target_column_name = settings.target_column_name
-
-        model = UnivariatePerformanceFeatureReduction._get_model(target_type, settings.random_state)
-        reduced_columns = []
-        score_result = {}
-        for column in numeric_columns_list:
-            score = cross_val_score(model, data[[column]], data[target_column_name], cv=3,
-                                    scoring=settings.performance_metric).mean()
-            score_result[column] = score
-            if score < settings.univariate_performance_threshold:
-                reduced_columns.append(column)
-        output = UnivariatePerformanceFeatureReduction._get_output(reduced_columns, score_result)
-        return output
+class FeatureReductionService:
+    """Domain service for feature reduction"""
 
-    @staticmethod
-    def _get_model(target_type: str, random_state: int):
-        """
-        Return Model with using target type.
-        Parameters
-        ----------
-        target_type
-        random_state
-
-        Returns
-        -------
-        Returns Model object for LGBM
-        """
+    @classmethod
+    def get_reduction_classes_ordered(cls):
+        """Returns all control classes for executor
+        """
+        # NOTE: Please do not change dict order. Because order is important!
+        feature_reduction_dict = {
+            NullFeatureReductionSettings: NullFeatureReduction,
+            StabilityFeatureReductionSettings: StabilityFeatureReduction,
+            UnivariatePerformanceFeatureReductionSettings: UnivariatePerformanceFeatureReduction,
+            SimilarDistributionFeatureReductionSettings: SimilarDistributionFeatureReduction,
+            HighCorrelatedFeatureReductionSettings: HighCorrelatedFeatureReduction
+        }
+        return feature_reduction_dict
+
+    @classmethod
+    def execute(cls, settings: List[BaseFeatureReductionSettings], data: pd.DataFrame, drop_cols: bool) -> List[
+        FeatureReductionOutput]:
+        """
+        Executes feature reduction with given feature reduction type and settings.
+        :param settings:
+        :param data:
+        :param drop_cols:
+        :return:
+        """
+        feature_reduction_dict = cls.get_reduction_classes_ordered()
+        result_list: List[FeatureReductionOutput] = []
+        column_univariate_performances: Dict[str, float] = {}
+        for feature_reduction_settings, feature_reduction_settings_service in feature_reduction_dict.items():
+            for setting in settings:
+                if isinstance(setting, feature_reduction_settings):
+                    if isinstance(setting, SimilarDistributionFeatureReductionSettings):
+                        setting.univariate_performance_result = column_univariate_performances
+                    if isinstance(setting, HighCorrelatedFeatureReductionSettings):
+                        setting.univariate_performance_result = column_univariate_performances
+                    result = feature_reduction_settings_service(setting).execute()
+                    res_columns = result.reduced_column_list
+                    result_list.append(result)
+
+                    if isinstance(result, UnivariatePerformanceFeatureReductionOutput):
+                        column_univariate_performances.update(result.univariate_performance_result)
+                    elif isinstance(result, SimilarDistReductionOutput):
+                        if result.new_univariate_performance_results is not None:
+                            column_univariate_performances.update(result.new_univariate_performance_results)
+                    elif isinstance(result, HighCorrReductionOutput):
+                        if result.new_univariate_performance_results is not None:
+                            column_univariate_performances.update(result.new_univariate_performance_results)
 
-        if target_type in (TargetType.BINARY.name, TargetType.MULTICLASS.name):
-            model = LGBMClassifier(random_state=random_state)
-        else:
-            model = LGBMRegressor(random_state=random_state)
-        return model
+                    if drop_cols and res_columns is not None:
+                        data.drop(res_columns, axis=1, inplace=True)
 
-    @staticmethod
-    def _get_output(reduced_columns: List[str], score_result) -> UnivariatePerformanceFeatureReductionOutput:
-        """
-        Get output for univariate performance feature reduction.
-        Parameters
-        ----------
-        reduced_columns
-        score_result
-
-        Returns
-        -------
-        Returns UnivariatePerformanceFeatureReductionOutput
-        """
-        output = UnivariatePerformanceFeatureReductionOutput()
-        output.feature_reduction_type = FeatureReductionType.UNIVARIATE_PERFORMANCE
-        output.reduced_column_list = reduced_columns
-        output.univariate_performance_result = score_result
-        return output
+            if len(data.columns) == 0:
+                return result_list
 
-    def get_description(self) -> str:
-        return "Univariate Performance Feature Reduction"
+        return result_list
```

### Comparing `autonon-0.3.0.post1/organon/ml/feature_reduction/services/feature_reduction.py` & `autonon-0.4.0/organon/ml/feature_reduction/services/feature_reduction.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,77 +5,82 @@
 
 from organon.ml.feature_reduction.domain.objects.feature_reduction_output import FeatureReductionOutput
 
 from organon.ml.feature_reduction.domain.services.feature_reduction_service import FeatureReductionService
 from organon.ml.feature_reduction.settings.feature_reduction_user_input_service import FeatureReductionUserInputService
 from organon.ml.feature_reduction.settings.objects.user_feature_reduction_settings import UserFeatureReductionSettings
 
-
 class FeatureReduction:
     """Feature reduction user interface class"""
 
     def __init__(self):
         self._output: List[FeatureReductionOutput] = None
         self._input_service = FeatureReductionUserInputService()
         self.settings: UserFeatureReductionSettings = UserFeatureReductionSettings()
 
-    def execute(self, data: pd.DataFrame, included_reduction_types: List[str] = None,
+    def execute(self, data: pd.DataFrame, drop_cols: bool, included_reduction_types: List[str] = None,
                 target_type: str = None, target_column_name: str = None, performance_metric: str = None,
+                excluded_columns: List[str] = None
                 ) -> \
             List[FeatureReductionOutput]:
         """
         Execute feature reduction with given parameters
         :param included_reduction_types:
         :param data:
+        :param drop_cols:
         :param target_type:
         :param target_column_name:
         :param performance_metric:
         :return:
         """
-
+        # pylint: disable=too-many-arguments
         self.settings.data = data
         self.settings.included_reduction_types = included_reduction_types
         self.settings.target_type = target_type
         self.settings.target_column_name = target_column_name
         self.settings.performance_metric = performance_metric
+        self.settings.excluded_columns = excluded_columns
         feature_reduction_settings = self._input_service.generate_feature_reduction_settings(self.settings)
-        self._output = FeatureReductionService.execute(feature_reduction_settings)
+        self._output = FeatureReductionService.execute(feature_reduction_settings, self.settings.data, drop_cols)
+
         return self._output
 
-    def set_null_feature_reduction_settings(self, null_ratio_threshold: float = None):
+    def set_null_feature_reduction_settings(self, null_ratio_threshold: float = 0.99):
         """
         Set null_ratio_threshold parameter for null feature reduction entered by user
         :param null_ratio_threshold:
         :return:
         """
         self.settings.null_ratio_threshold = null_ratio_threshold
 
-    def set_high_correlated_feature_reduction_settings(self, correlation_threshold: float = None,
+    def set_high_correlated_feature_reduction_settings(self, correlation_threshold: float = 0.99,
                                                        random_state=None):
         """
         Set correlation_threshold parameter for high correlated feature reduction
-
         :param correlation_threshold:
+        :param random_state:
         :return:
         """
         self.settings.correlation_threshold = correlation_threshold
         self.settings.random_state = random_state
 
     def set_univariate_performance_feature_reduction_settings(self, univariate_performance_threshold: float = None,
                                                               random_state=None):
         """
         Set univariate_performance_threshold parameter for univariate performance feature reduction
         :param univariate_performance_threshold:
+        :param random_state:
         :return:
         """
         self.settings.univariate_performance_threshold = univariate_performance_threshold
         self.settings.random_state = random_state
 
-    def set_similar_distribution_feature_reduction_settings(self, nunique_count: int = None, random_state=None):
+    def set_similar_distribution_feature_reduction_settings(self, nunique_count: int = 20, random_state=None):
         """
         Set nunique_count parameter for similar distribution feature reduction
 
         :param nunique_count:
+        :param random_state:
         :return:
         """
         self.settings.nunique_count = nunique_count
         self.settings.random_state = random_state
```

### Comparing `autonon-0.3.0.post1/organon/ml/feature_reduction/settings/feature_reduction_user_input_service.py` & `autonon-0.4.0/organon/ml/feature_reduction/settings/feature_reduction_user_input_service.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     SimilarDistributionFeatureReductionSettings
 from organon.ml.feature_reduction.settings.objects.stability_feature_reduction_settings import \
     StabilityFeatureReductionSettings
 from organon.ml.feature_reduction.settings.objects.univariate_performance_feature_reduction_settings import \
     UnivariatePerformanceFeatureReductionSettings
 from organon.ml.feature_reduction.settings.objects.user_feature_reduction_settings import UserFeatureReductionSettings
 
-
 class FeatureReductionUserInputService:
     """Service for validating user input and generating settings for feature reduction"""
 
     @staticmethod
     def _set_default_metric(value: str, target_type: TargetType) -> str:
         """
         Set default metric
@@ -31,30 +30,30 @@
         :return:
         """
         if value is not None:
             return value
         if target_type.name == TargetType.BINARY.name:
             return "roc_auc"
         if target_type.name == TargetType.MULTICLASS.name:
-            return "accuracy"
+            return "roc_auc_ovr_weighted"
         if target_type.name == TargetType.SCALAR.name:
             return "r2"
         raise KnownException("Please control target type.")
 
     @staticmethod
     def _set_default_univariate_performance_threshold(value: float, target_type: TargetType) -> float:
         """Set default univariate performance threshold"""
         if value is not None:
             return value
         if target_type.name == TargetType.BINARY.name:
-            return 0.6
+            return 0.55
         if target_type.name == TargetType.MULTICLASS.name:
-            return 0.2
+            return 0.55
         if target_type.name == TargetType.SCALAR.name:
-            return 0.1
+            return 0.05
         raise KnownException("Please control target type.")
 
     @staticmethod
     def _get_included_reduction_types(input_settings: UserFeatureReductionSettings) -> List[str]:
         """
         Return included_reduction_types
         :param input_settings:
@@ -78,149 +77,169 @@
         BaseFeatureReductionSettings]:
 
         """
         Generate Feature Reduction Settings list
         :return:
         """
         settings = []
+        if input_settings.target_column_name is not None:
+            excluded_column_names = input_settings.excluded_columns + [
+                input_settings.target_column_name] if input_settings.excluded_columns is not None else [
+                input_settings.target_column_name]
+        else:
+            excluded_column_names = input_settings.excluded_columns
         included_reduction_types = self._get_included_reduction_types(input_settings)
 
         if FeatureReductionType.NULL.name in included_reduction_types:
             settings.append(self.get_null_feature_reduction_settings(
-                input_settings.data, input_settings.null_ratio_threshold))
+                input_settings.data, input_settings.null_ratio_threshold, excluded_column_names))
 
         if FeatureReductionType.STABILITY.name in included_reduction_types:
-            settings.append(self.get_stability_feature_reduction_settings(input_settings.data))
+            settings.append(
+                self.get_stability_feature_reduction_settings(input_settings.data, excluded_column_names))
 
         if FeatureReductionType.UNIVARIATE_PERFORMANCE.name in included_reduction_types:
             settings.append(self.get_univariate_performance_feature_reduction_settings(
                 input_settings.data, input_settings.target_type, input_settings.target_column_name,
                 input_settings.performance_metric, input_settings.univariate_performance_threshold,
-                input_settings.random_state))
+                input_settings.random_state, excluded_column_names))
 
         if FeatureReductionType.SIMILAR_DISTRIBUTION.name in included_reduction_types:
             settings.append(self.get_similar_distribution_feature_reduction_settings(
                 input_settings.data, input_settings.target_type, input_settings.target_column_name,
                 input_settings.performance_metric, input_settings.nunique_count,
-                input_settings.random_state))
+                input_settings.random_state, excluded_column_names))
 
         if FeatureReductionType.HIGH_CORRELATION.name in included_reduction_types:
             settings.append(self.get_high_correlated_feature_reduction_settings(
                 input_settings.data, input_settings.target_type, input_settings.target_column_name,
                 input_settings.performance_metric, input_settings.correlation_threshold,
-                input_settings.random_state))
+                input_settings.random_state, excluded_column_names))
 
         return settings
 
     @classmethod
-    def get_stability_feature_reduction_settings(cls, data: pd.DataFrame) -> StabilityFeatureReductionSettings:
+    def get_stability_feature_reduction_settings(cls, data: pd.DataFrame, excluded_col_names: List[
+        str] = None) -> StabilityFeatureReductionSettings:
         """
         Validates settings for stability feature reduction entered by user and generates settings object
         :param data:
+        :param excluded_col_names:
         :return:
         """
         if data is None:
             raise ValueError("Data should be given")
-        return StabilityFeatureReductionSettings(data)
+        return StabilityFeatureReductionSettings(data, excluded_columns=excluded_col_names)
 
     @classmethod
-    def get_null_feature_reduction_settings(cls, data: pd.DataFrame, null_ratio_threshold: float = None) -> \
-            NullFeatureReductionSettings:
+    def get_null_feature_reduction_settings(cls, data: pd.DataFrame, null_ratio_threshold: float = None,
+                                            excluded_col_names: List[str] = None) -> NullFeatureReductionSettings:
         """
         Validates settings for null feature reduction entered by user and generates settings object
         :param data:
         :param null_ratio_threshold:
+        :param excluded_col_names:
         :return:
         """
-
         if data is None:
             raise ValueError("Data should be given")
         null_ratio_threshold = get_default_if_none(null_ratio_threshold, 0.99)
-        return NullFeatureReductionSettings(data, null_ratio_threshold)
+        return NullFeatureReductionSettings(data, null_ratio_threshold, excluded_columns=excluded_col_names)
 
     @classmethod
     def get_high_correlated_feature_reduction_settings(cls, data: pd.DataFrame, target_type: str = None,
                                                        target_column_name: str = None, performance_metric: str = None,
                                                        correlation_threshold: float = None,
-                                                       random_state=None) -> \
+                                                       random_state=None, excluded_col_names: List[
+                str] = None) -> \
             HighCorrelatedFeatureReductionSettings:
         """
         Validates settings for high correlated feature reduction entered by user and generates settings object
         :param data:
         :param target_type:
         :param target_column_name:
         :param performance_metric:
         :param correlation_threshold:
+        :param random_state:
         :return:
         """
-
+        # pylint: disable=too-many-arguments
         if data is None:
             raise ValueError("Data should be given")
-        correlation_threshold = get_default_if_none(correlation_threshold, 0.90)
+        correlation_threshold = get_default_if_none(correlation_threshold, 0.99)
         target_type = get_enum(target_type, TargetType)
         if target_column_name is not None:
             if target_type is None:
                 raise ValueError("Type of target column should be given.")
             performance_metric = FeatureReductionUserInputService._set_default_metric(performance_metric, target_type)
             random_state = get_default_if_none(random_state, 42)
-        return HighCorrelatedFeatureReductionSettings(data, target_type, target_column_name, performance_metric,
-                                                      correlation_threshold, None, random_state)
+        return HighCorrelatedFeatureReductionSettings(data, target_type, target_column_name,
+                                                      performance_metric,
+                                                      correlation_threshold, None, random_state,
+                                                      excluded_columns=excluded_col_names)
 
     @classmethod
     def get_similar_distribution_feature_reduction_settings(cls, data: pd.DataFrame, target_type: str = None,
                                                             target_column_name: str = None,
                                                             performance_metric: str = None,
                                                             nunique_count: int = None,
-                                                            random_state=None) -> \
+                                                            random_state=None,
+                                                            excluded_col_names: List[str] = None) -> \
             SimilarDistributionFeatureReductionSettings:
         """
         Validates settings for similar distribution feature reduction
         entered by user and generates settings object
         :param data:
         :param target_type:
         :param target_column_name:
         :param performance_metric:
         :param nunique_count:
+        :param random_state:
         :return:
         """
-
+        # pylint: disable=too-many-arguments
         if data is None:
             raise ValueError("Data should be given")
         target_type = get_enum(target_type, TargetType)
         nunique_count = get_default_if_none(nunique_count, 20)
         if target_column_name is not None:
             if target_type is None:
                 raise ValueError("Type of target column should be given.")
             performance_metric = FeatureReductionUserInputService._set_default_metric(performance_metric, target_type)
             random_state = get_default_if_none(random_state, 42)
 
-        return SimilarDistributionFeatureReductionSettings(data, target_type, target_column_name, performance_metric,
-                                                           nunique_count, None, random_state)
+        return SimilarDistributionFeatureReductionSettings(data, target_type, target_column_name,
+                                                           performance_metric,
+                                                           nunique_count, None, random_state,
+                                                           excluded_columns=excluded_col_names)
 
     @classmethod
     def get_univariate_performance_feature_reduction_settings(cls, data: pd.DataFrame, target_type: str,
                                                               target_column_name: str, performance_metric: str = None,
                                                               univariate_performance_threshold: float = None,
-                                                              random_state=None) -> \
-            UnivariatePerformanceFeatureReductionSettings:
+                                                              random_state=None, excluded_col_names: List[
+                str] = None) -> UnivariatePerformanceFeatureReductionSettings:
         """
         Validates settings for univariate performance feature reduction entered by user and generates settings object
         :param data:
         :param target_type:
         :param target_column_name:
         :param performance_metric:
         :param univariate_performance_threshold:
+        :param random_state:
         :return:
         """
-
+        # pylint: disable=too-many-arguments
         if data is None:
             raise ValueError("Data should be given")
         if target_column_name is None or target_type is None:
             raise ValueError("Target column name and type of target column should be given.")
         target_type = get_enum(target_type, TargetType)
         performance_metric = FeatureReductionUserInputService._set_default_metric(performance_metric, target_type)
         random_state = get_default_if_none(random_state, 42)
 
         univariate_performance_threshold = FeatureReductionUserInputService \
             ._set_default_univariate_performance_threshold(univariate_performance_threshold, target_type)
-        return UnivariatePerformanceFeatureReductionSettings(data, target_type, target_column_name, performance_metric,
-                                                             univariate_performance_threshold, random_state)
+        return UnivariatePerformanceFeatureReductionSettings(data, target_type, target_column_name,
+                                                             performance_metric,
+                                                             univariate_performance_threshold, random_state,
+                                                             excluded_columns=excluded_col_names)
```

### Comparing `autonon-0.3.0.post1/organon/ml/feature_reduction/settings/objects/similar_distribution_feature_reduction_settings.py` & `autonon-0.4.0/organon/ml/feature_reduction/settings/objects/null_feature_reduction_settings.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,14 @@
-"""Includes SimilarDistributionFeatureReduction class."""
-from dataclasses import dataclass
-from typing import Dict
+"""Includes NullFeatureReductionSettings class."""
+from typing import List, Optional
+from pandas import DataFrame
+from organon.ml.feature_reduction.settings.objects.base_feature_reduction_settings import \
+    BaseFeatureReductionSettings
 
-from organon.ml.common.enums.target_type import TargetType
-from organon.ml.feature_reduction.settings.objects.base_feature_reduction_settings import BaseFeatureReductionSettings
 
+class NullFeatureReductionSettings(BaseFeatureReductionSettings):
+    """Settings for null feature reduction"""
 
-@dataclass
-class SimilarDistributionFeatureReductionSettings(BaseFeatureReductionSettings):
-    """Settings for similar distribution feature reduction"""
-
-    target_type: TargetType = None
-    target_column_name: str = None
-    performance_metric: str = None
-    nunique_count: int = None
-    univariate_performance_result: Dict[str, float] = None
-    random_state: int = None
+    def __init__(self, data: DataFrame, null_ratio_threshold: float = None,
+    excluded_columns: Optional[List[str]] = None):
+        super().__init__(data, excluded_columns)
+        self.null_ratio_threshold = null_ratio_threshold
```

### Comparing `autonon-0.3.0.post1/organon/ml/feature_reduction/settings/objects/user_feature_reduction_settings.py` & `autonon-0.4.0/organon/ml/feature_reduction/settings/objects/user_feature_reduction_settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,7 +11,8 @@
         self.target_column_name = None
         self.performance_metric = None
         self.univariate_performance_threshold = None
         self.correlation_threshold = None
         self.included_reduction_types = None
         self.nunique_count = None
         self.random_state = None
+        self.excluded_columns = None
```

### Comparing `autonon-0.3.0.post1/organon/ml/feature_selection/domain/objects/priority_queue.py` & `autonon-0.4.0/organon/ml/feature_selection/domain/objects/priority_queue.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/feature_selection/domain/objects/settings/base_supervised_feature_selection_settings.py` & `autonon-0.4.0/organon/ml/feature_selection/domain/objects/settings/base_supervised_feature_selection_settings.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/feature_selection/domain/objects/settings/cfs_selection_settings.py` & `autonon-0.4.0/organon/ml/feature_selection/domain/objects/settings/cfs_selection_settings.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/feature_selection/domain/objects/settings/feature_similarity_selection_settings.py` & `autonon-0.4.0/organon/ml/feature_selection/domain/objects/settings/feature_similarity_selection_settings.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/feature_selection/domain/objects/settings/lasso_selection_settings.py` & `autonon-0.4.0/organon/ml/feature_selection/domain/objects/settings/lasso_selection_settings.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/feature_selection/domain/objects/settings/rf_selection_settings.py` & `autonon-0.4.0/organon/ml/feature_selection/domain/objects/settings/rf_selection_settings.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/feature_selection/domain/objects/settings/sweep_selection_settings.py` & `autonon-0.4.0/organon/ml/feature_selection/domain/objects/settings/sweep_selection_settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from organon.ml.feature_selection.domain.objects.settings.base_unsupervised_feature_selection_settings import \
     BaseUnsupervisedFeatureSelectionSettings
 
 
 class SweepSelectionSettings(BaseUnsupervisedFeatureSelectionSettings):
     """Settings for sweep selection"""
 
-    def __init__(self, data: pd.DataFrame, bin_count: int = None, r_factor: float = None, max_col_count: int = None,
-                 n_threads: int = 1):
+    def __init__(self, data: pd.DataFrame, bin_count: int = None, r_factor: float = None, random_state: int = None,
+                 max_col_count: int = None, n_threads: int = 1):
         super().__init__(data)
         self.bin_count = bin_count
         self.r_factor = r_factor
+        self.random_state = random_state
         self.max_col_count = max_col_count
         self.n_threads = n_threads
```

### Comparing `autonon-0.3.0.post1/organon/ml/feature_selection/domain/objects/unsupervised_feature_extractor.py` & `autonon-0.4.0/organon/fl/modelling/unsupervised_feature_extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Includes UnsupervisedFeatureExtractor class."""
+import random
 import sys
-from random import SystemRandom
 from typing import Optional, List, Tuple, Dict
 
 import numpy as np
 from scipy.sparse import csc_matrix
 
 from organon.fl.core.executionutil.objects.stopwatch import StopWatch
 from organon.fl.logging.helpers.log_helper import LogHelper
@@ -17,19 +17,20 @@
 
 class UnsupervisedFeatureExtractor:
     """
     Class for Unsupervised Feature Extraction Algorithm.
     """
 
     def __init__(self, data_frame: Dict[str, np.ndarray], bin_count: int = 4, r_factor: float = 0.9,
-                 max_iter: int = 500,
+                 random_state: int = None, max_iter: int = 500,
                  is_logging: bool = False):
         self.__frame = data_frame
         self.__bin_count = bin_count
         self.__r_limit = bin_count * r_factor
+        self.__random_state = random_state
         self.__max_iter = max_iter
         if max_iter < 0:
             self.__max_iter = sys.maxsize
         self.__is_logging = is_logging
 
         self.__un_swept = None
         self.__operator = None
@@ -56,15 +57,16 @@
         input_frame, index_to_name = self.get_sparse_frame()
 
         if input_frame is None:
             return []
 
         self.log(f"Sparse Frame is Created in {watch.get_elapsed_seconds(True)}")
 
-        first_enter = SystemRandom().randrange(0, len(index_to_name))
+        random.seed(self.__random_state)
+        first_enter = random.randrange(0, len(index_to_name))  # nosec
         self.log(index_to_name[first_enter])
         self.__un_swept = set(range(len(index_to_name)))
 
         sweep_operator, generator = self.get_sweep_operator_generator(input_frame)
         self.__operator = sweep_operator
         self.__generator = generator
         self.__cov_info = generator.covariance_info
```

### Comparing `autonon-0.3.0.post1/organon/ml/feature_selection/domain/services/base_feature_selection_service.py` & `autonon-0.4.0/organon/ml/feature_selection/domain/services/base_feature_selection_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import pandas as pd
 
 from organon.fl.core.helpers.data_frame_helper import get_numerical_column_names
 from organon.fl.logging.helpers.log_helper import LogHelper
 from organon.ml.feature_selection.domain.objects.base_selection_output import BaseSelectionOutput
 from organon.ml.feature_selection.domain.objects.settings.base_feature_selection_settings import \
     BaseFeatureSelectionSettings
-from organon.ml.feature_selection.domain.objects.unsupervised_feature_extractor import UnsupervisedFeatureExtractor
+from organon.fl.modelling.unsupervised_feature_extractor import UnsupervisedFeatureExtractor
 from organon.ml.preprocessing.services.preprocessor import Preprocessor
 from organon.ml.preprocessing.settings.enums.imputer_type import ImputerType
 
 FeatureSelectionSettingsType = TypeVar("FeatureSelectionSettingsType", bound=BaseFeatureSelectionSettings)
 FeatureSelectionOutputType = TypeVar("FeatureSelectionOutputType", bound=BaseSelectionOutput)
 
 
@@ -61,19 +61,18 @@
         columns_with_nan_values = [col for col in numerical_columns if data[col].isnull().values.any()]
         execute_imputation = len(columns_with_nan_values) > 0
         execute_ohe = len(numerical_columns) != len(data.columns)
         ohe_columns_dict = None
         if execute_imputation or execute_ohe:
             data = data.copy()
             if execute_imputation:
-                imputation_service = Preprocessor().get_imputation_service(data,
-                                                                           numeric_data_method=ImputerType.SIMPLE.name,
+                imputation_service = Preprocessor().get_imputation_service(numeric_data_method=ImputerType.SIMPLE.name,
                                                                            n_strategy="median",
                                                                            included_columns=numerical_columns)
-                imputation_service.fit()
+                imputation_service.fit(data)
                 data = imputation_service.transform(data)
             if execute_ohe:
                 ohe_service = Preprocessor.get_one_hot_encoding_service()
                 ohe_service.fit(data)
                 data = ohe_service.transform(data)
                 ohe_columns_dict = ohe_service.columns_dict
         return data, ohe_columns_dict
```

### Comparing `autonon-0.3.0.post1/organon/ml/feature_selection/domain/services/base_supervised_feature_selection_service.py` & `autonon-0.4.0/organon/ml/feature_selection/domain/services/base_supervised_feature_selection_service.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/feature_selection/domain/services/base_unsupervised_feature_selection_service.py` & `autonon-0.4.0/organon/ml/feature_selection/domain/services/base_unsupervised_feature_selection_service.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/feature_selection/domain/services/cfs_selection_service.py` & `autonon-0.4.0/organon/ml/feature_selection/domain/services/cfs_selection_service.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/feature_selection/domain/services/feature_similarity_selection_service.py` & `autonon-0.4.0/organon/ml/feature_selection/domain/services/feature_similarity_selection_service.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/feature_selection/domain/services/lasso_selection_service.py` & `autonon-0.4.0/organon/ml/feature_selection/domain/services/lasso_selection_service.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/feature_selection/domain/services/rf_selection_service.py` & `autonon-0.4.0/organon/ml/feature_selection/domain/services/rf_selection_service.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/feature_selection/domain/services/sweep_selection_service.py` & `autonon-0.4.0/organon/ml/feature_selection/domain/services/sweep_selection_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,12 +25,14 @@
     @classmethod
     def _get_sweep_args(cls, settings: SweepSelectionSettings):
         sweep_args = {}
         if settings.bin_count is not None:
             sweep_args["bin_count"] = settings.bin_count
         if settings.r_factor is not None:
             sweep_args["r_factor"] = settings.r_factor
+        if settings.random_state is not None:
+            sweep_args["random_state"] = settings.random_state
         if settings.max_col_count is not None:
             sweep_args["max_col_count"] = settings.max_col_count
         if settings.n_threads is not None:
             sweep_args["n_threads"] = settings.n_threads
         return sweep_args
```

### Comparing `autonon-0.3.0.post1/organon/ml/feature_selection/services/abstractions/base_supervised_feature_selecter.py` & `autonon-0.4.0/organon/ml/feature_selection/services/abstractions/base_supervised_feature_selecter.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/feature_selection/services/cfs.py` & `autonon-0.4.0/organon/ml/feature_selection/services/cfs.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/feature_selection/services/feature_similarity_selection.py` & `autonon-0.4.0/organon/ml/feature_selection/services/feature_similarity_selection.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/feature_selection/services/lasso_selection.py` & `autonon-0.4.0/organon/ml/feature_selection/services/lasso_selection.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/feature_selection/services/rf_selection.py` & `autonon-0.4.0/organon/ml/feature_selection/services/rf_selection.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/feature_selection/services/sweep_selection.py` & `autonon-0.4.0/organon/ml/feature_selection/services/sweep_selection.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 from organon.ml.feature_selection.services.abstractions.base_unsupervised_feature_selecter import \
     BaseUnsupervisedFeatureSelecter
 
 
 class SweepSelection(BaseUnsupervisedFeatureSelecter):
     """Feature selecter which utilizes sweep algorithm for selection"""
 
-    def __init__(self, data: pd.DataFrame, *, bin_count: int = None, r_factor: float = None, max_col_count: int = None,
-                 n_threads: int = 1):
+    def __init__(self, data: pd.DataFrame, *, bin_count: int = None, r_factor: float = None, random_state: int = None,
+                 max_col_count: int = None, n_threads: int = 1):
         super().__init__(data)
-        self.settings = SweepSelectionSettings(data, bin_count=bin_count, r_factor=r_factor,
+        self.settings = SweepSelectionSettings(data, bin_count=bin_count, r_factor=r_factor, random_state=random_state,
                                                max_col_count=max_col_count, n_threads=n_threads)
         self.output: Optional[SweepSelectionOutput] = None
 
     def _run(self):
         service = SweepSelectionService()
         self.output = service.run_selection(self.settings)
         return self.output
```

### Comparing `autonon-0.3.0.post1/organon/ml/modelling/algorithms/classifiers/gam_classifier.py` & `autonon-0.4.0/organon/ml/modelling/algorithms/classifiers/gam_classifier.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/modelling/algorithms/classifiers/stacking_ensemble_classifier.py` & `autonon-0.4.0/organon/ml/modelling/algorithms/classifiers/stacking_ensemble_classifier.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/modelling/algorithms/classifiers/voting_ensemble_classifier.py` & `autonon-0.4.0/organon/ml/modelling/algorithms/classifiers/voting_ensemble_classifier.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/modelling/algorithms/core/abstractions/base_classifier.py` & `autonon-0.4.0/organon/ml/modelling/algorithms/core/abstractions/base_classifier.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/modelling/algorithms/core/abstractions/base_modeller.py` & `autonon-0.4.0/organon/ml/modelling/algorithms/core/abstractions/base_modeller.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/modelling/algorithms/core/abstractions/base_regressor.py` & `autonon-0.4.0/organon/ml/modelling/algorithms/core/abstractions/base_regressor.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/modelling/algorithms/core/abstractions/base_sklearn_classifier.py` & `autonon-0.4.0/organon/ml/modelling/algorithms/core/abstractions/base_sklearn_classifier.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/modelling/algorithms/core/abstractions/base_sklearn_regressor.py` & `autonon-0.4.0/organon/ml/modelling/algorithms/core/abstractions/base_sklearn_regressor.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/modelling/algorithms/core/abstractions/gam_mixin.py` & `autonon-0.4.0/organon/ml/modelling/algorithms/core/abstractions/gam_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,16 @@
 from organon.ml.preprocessing.services.preprocessor import Preprocessor
 
 
 class GamMixin:
     """Mixin class including common gam functions"""
 
     def _fit_gam(self, train_data: pd.DataFrame, target_data: pd.Series):
-        self._coarse_class = Preprocessor.get_coarse_class_service(train_data, target_data, 0.2,
-                                                                   target_column_type=self._get_target_type().name)
-        self._coarse_class.fit()
+        self._coarse_class = Preprocessor.get_coarse_class_service(0.2, target_column_type=self._get_target_type().name)
+        self._coarse_class.fit(train_data, target_data)
         train_data = self._get_preprocessed(train_data)
         target_data = target_data.to_numpy(copy=False)
         self._initial_selected_features, self._best_alpha = self._get_initial_keep_list_and_best_alpha(train_data,
                                                                                                        target_data)
         keep_list = self._reduce_features(train_data, target_data)
         if len(keep_list) == 0:
             keep_list = train_data.columns.to_list()
```

### Comparing `autonon-0.3.0.post1/organon/ml/modelling/algorithms/core/enums/modeller.py` & `autonon-0.4.0/organon/ml/modelling/algorithms/core/enums/modeller.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/modelling/algorithms/helpers/ensembling_helper.py` & `autonon-0.4.0/organon/ml/modelling/algorithms/helpers/ensembling_helper.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/modelling/algorithms/regressors/gam_regressor.py` & `autonon-0.4.0/organon/ml/modelling/algorithms/regressors/gam_regressor.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/modelling/algorithms/regressors/stacking_ensemble_regressor.py` & `autonon-0.4.0/organon/ml/modelling/algorithms/regressors/stacking_ensemble_regressor.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/modelling/algorithms/regressors/voting_ensemble_regressor.py` & `autonon-0.4.0/organon/ml/modelling/algorithms/regressors/voting_ensemble_regressor.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/modelling/algorithms/services/algorithm_service.py` & `autonon-0.4.0/organon/ml/modelling/algorithms/services/algorithm_service.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/modelling/algorithms/services/ml_application_operations.py` & `autonon-0.4.0/organon/ml/modelling/algorithms/services/ml_application_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 This module includes MLApplicationOperations class.
 """
 import threading
 
-from organon.fl.core.helpers import guid_helper
+import organon
+from organon.common.helpers import dev_mode_helper
 from organon.fl.core.iocutil import ioc_helper
 from organon.fl.core.iocutil.ioc_registration_item import IocRegistrationItem
 from organon.fl.generic.interaction.fl_initializer import FlInitializer
-from organon.fl.logging.helpers.log_helper import LogHelper
 from organon.ml.modelling.algorithms.classifiers.gam_classifier import GamClassifier
 from organon.ml.modelling.algorithms.classifiers.gbm_classifier import GBMClassifier
 from organon.ml.modelling.algorithms.classifiers.lightgbm_classifier import LightGBMClassifier
 from organon.ml.modelling.algorithms.classifiers.logistic_regression_classifier import LogisticRegressionClassifier
 from organon.ml.modelling.algorithms.classifiers.multi_layer_perceptron_classifier import MultiLayerPerceptronClassifier
 from organon.ml.modelling.algorithms.classifiers.rf_classifier import RFClassifier
 from organon.ml.modelling.algorithms.classifiers.xgboost_classifier import XGBoostClassifier
@@ -43,28 +43,23 @@
                 cls._on_init()
                 MLApplicationOperations.APPLICATION_INITIALIZED = True
 
     @classmethod
     def _on_init(cls):
         cls._initialize_fl()
         cls.register_types()
-        MLApplicationOperations.initialize_logging()
 
     @classmethod
     def _initialize_fl(cls):
         FlInitializer.application_initialize()
 
-    @staticmethod
-    def initialize_logging():
-        """Initializes logging."""
-        execution_id = guid_helper.new_guid(32)
-        default_format = "[%(asctime)s] [%(threadName)s] %(levelname)-8s %(module_name)s:%(line_number)s : " \
-                         "%(execution_id)s  - %(message)s"
-        LogHelper.add_global_extra("execution_id", execution_id)
-        LogHelper.set_default_format(default_format)
+    @classmethod
+    def init_dev_mode(cls, log_to_console: bool = True, log_file: str = "application.log"):
+        """Initializes development mode."""
+        dev_mode_helper.init_dev_mode(organon.ml.__name__, log_to_console=log_to_console, log_file=log_file)
 
     @classmethod
     def register_types(cls):
         """
         Registers ioc items
         """
         ioc_helper.register_type(IocRegistrationItem(Modeller.LOGISTIC_REGRESSION_CLASSIFIER.name,
```

### Comparing `autonon-0.3.0.post1/organon/ml/modelling/model_selection/domain/objects/selecter_output.py` & `autonon-0.4.0/organon/ml/modelling/model_selection/domain/objects/selecter_output.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/modelling/model_selection/domain/services/cross_validation_service.py` & `autonon-0.4.0/organon/ml/modelling/model_selection/domain/services/cross_validation_service.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/modelling/model_selection/domain/services/hpo_service.py` & `autonon-0.4.0/organon/ml/modelling/model_selection/domain/services/hpo_service.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/modelling/model_selection/domain/services/selection_service.py` & `autonon-0.4.0/organon/ml/modelling/model_selection/domain/services/selection_service.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/modelling/model_selection/services/cross_validation.py` & `autonon-0.4.0/organon/ml/modelling/model_selection/services/cross_validation.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/modelling/model_selection/services/hp_optimizer.py` & `autonon-0.4.0/organon/ml/modelling/model_selection/services/hp_optimizer.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/modelling/model_selection/services/selecter.py` & `autonon-0.4.0/organon/ml/modelling/model_selection/services/selecter.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/modelling/model_selection/services/user_settings/user_hp_optimization_settings.py` & `autonon-0.4.0/organon/ml/modelling/model_selection/services/user_settings/user_hp_optimization_settings.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/modelling/model_selection/services/user_settings/user_selection_settings.py` & `autonon-0.4.0/organon/ml/modelling/model_selection/services/user_settings/user_selection_settings.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/modelling/model_selection/settings/model_selection_user_input_service.py` & `autonon-0.4.0/organon/ml/modelling/model_selection/settings/model_selection_user_input_service.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/modelling/model_selection/settings/objects/hp_optimization_settings.py` & `autonon-0.4.0/organon/ml/modelling/model_selection/settings/objects/hp_optimization_settings.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/modelling/model_selection/settings/objects/selection_settings.py` & `autonon-0.4.0/organon/ml/modelling/model_selection/settings/objects/selection_settings.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/object_classification/domain/objects/object_clf_settings.py` & `autonon-0.4.0/organon/ml/object_classification/domain/objects/object_clf_settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 """Includes ObjectClfSettings class"""
 from typing import Tuple
 
 from organon.ml.common.enums.classification_type import ClassificationType
+from organon.ml.common.enums.color_type import ColorType
 from organon.ml.object_classification.domain.objects.fine_tuning_settings import FineTuningSettings
 from organon.ml.object_classification.domain.objects.pretrained_model_settings import PretrainedModelSettings
 from organon.ml.object_classification.domain.objects.transfer_learning_settings import TransferLearningSettings
+from organon.ml.object_classification.domain.objects.data_augmentation_settings import DataAugmentationSettings
 
 
 class ObjectClfSettings:
     """Settings for object classification"""
 
-    def __init__(self, train_data_dir: str, clf_mode: ClassificationType,
+    def __init__(self, train_data_dir: str,
                  pretrained_model_settings: PretrainedModelSettings = None,
                  transfer_learning_settings: TransferLearningSettings = None,
                  fine_tuning_settings: FineTuningSettings = None,
+                 data_augmentation_settings: DataAugmentationSettings = None,
                  validation_data_dir: str = None,
                  validation_data_ratio: float = 0.2, image_size: Tuple[int, int] = (150, 150),
-                 batch_size: int = 50, image_data_gen_args: dict = None, random_seed: int = None):
+                 batch_size: int = 50, prediction_threshold: float = 0, color_mode: ColorType = ColorType.RGB,
+                 random_seed: int = 42):
         # pylint: disable=too-many-arguments
         self.train_data_dir: str = train_data_dir
         self.validation_data_dir: str = validation_data_dir
-        self.clf_mode: ClassificationType = clf_mode
+        self.clf_mode: ClassificationType = None
+        self.color_mode: ColorType = color_mode
         self.validation_data_ratio: float = validation_data_ratio
         self.image_size: Tuple[int, int] = image_size
         self.batch_size: int = batch_size
         self.pretrained_model_settings = pretrained_model_settings if pretrained_model_settings is not None \
             else PretrainedModelSettings()
         self.transfer_learning_settings = transfer_learning_settings if transfer_learning_settings is not None \
             else TransferLearningSettings()
-        self.fine_tuning_settings = fine_tuning_settings if fine_tuning_settings is not None else FineTuningSettings()
-        self.image_data_gen_args = image_data_gen_args
+        self.data_augmentation_settings = data_augmentation_settings
+        self.fine_tuning_settings = fine_tuning_settings
+        self.prediction_threshold = prediction_threshold
         self.random_seed: int = random_seed
```

### Comparing `autonon-0.3.0.post1/organon/ml/preprocessing/domain/objects/imputation_fit_output.py` & `autonon-0.4.0/organon/ml/preprocessing/domain/objects/imputation_fit_output.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/preprocessing/domain/services/coarse_class_service.py` & `autonon-0.4.0/organon/ml/preprocessing/domain/services/coarse_class_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Includes CoarseClassService class"""
 from typing import Union, Tuple
 
 import numpy as np
 import pandas as pd
-from sklearn.tree import DecisionTreeRegressor, DecisionTreeClassifier
 
 from organon.fl.core.enums.column_native_type import ColumnNativeType
 from organon.fl.core.helpers.data_frame_helper import get_column_native_type
 from organon.fl.logging.helpers.log_helper import LogHelper
 from organon.ml.common.enums.target_type import TargetType
 from organon.ml.common.helpers.df_ops_helper import get_train_test_split_from_strata, get_sample_indices_from_series
 from organon.ml.preprocessing.domain.objects.coarse_class_fit_output import CoarseClassFitOutput
@@ -15,34 +14,53 @@
 from organon.ml.preprocessing.settings.objects.coarse_class_settings import CoarseClassSettings
 
 
 class CoarseClassService:
     """Service for CoarseClass conversion"""
 
     def __init__(self, settings: CoarseClassSettings):
+        if settings.target_type not in [TargetType.SCALAR, TargetType.BINARY]:
+            raise ValueError("Target type should be scalar or binary.")
         self.settings = settings
         self.fit_output: CoarseClassFitOutput = None
 
-    def fit(self) -> CoarseClassFitOutput:
+    def fit(self, data: pd.DataFrame, target_data: pd.Series, stability_check_data: pd.DataFrame = None,
+            stability_check_target_data: pd.Series = None) -> CoarseClassFitOutput:
         """fits coarse column and outputs coarse tables"""
-        target_native_type = get_column_native_type(pd.DataFrame({"target": self.settings.target_data}), "target")
-        if self.settings.target_type.name == TargetType.SCALAR.name and target_native_type != ColumnNativeType.Numeric:
+        self._validate_data(data, target_data, stability_check_target_data, stability_check_target_data)
+        target_native_type = get_column_native_type(pd.DataFrame({"target": target_data}), "target")
+        if self.settings.target_type == TargetType.SCALAR and target_native_type != ColumnNativeType.Numeric:
             raise ValueError("Target column should be numeric for categorical coarse classing.")
-        target_data, stability_check_target_data = self._check_target_data(
-            self.settings.target_data, self.settings.stability_check_target_data, target_native_type)
-        x_train, y_train, x_valid, y_valid = self._prepare_train_and_validation_data(
-            self.settings.fit_data, target_data, stability_check_target_data)
+        target_data, stability_check_target_data = self._check_target_data(target_data, stability_check_target_data,
+                                                                           target_native_type)
+        x_train, y_train, x_valid, y_valid = self._prepare_train_and_validation_data(data, target_data,
+                                                                                     stability_check_data,
+                                                                                     stability_check_target_data)
         fit_output = self._initialize_output(y_train)
         for col in x_train.columns:
             column_type = get_column_native_type(x_train, col)
             fit_output = self._execute_coarsing_for_col(fit_output, column_type, col, x_train[col], y_train,
                                                         x_valid[col], y_valid)
         self.fit_output = fit_output
         return fit_output
 
+    def _validate_data(self, data: pd.DataFrame, target_data: pd.Series, stability_check_data: pd.DataFrame = None,
+                       stability_check_target_data: pd.Series = None):
+        if data is None or data.empty:
+            raise ValueError("Data cannot be empty or None.")
+        if self.settings.target_type == TargetType.BINARY and target_data.nunique() > 2:
+            raise ValueError("Target type is binary but target contains more than two classes.")
+        if len(data) != len(target_data) or any(data.index != target_data.index):
+            raise ValueError("Data and target indexes are different.")
+        if self.settings.stability_check:
+            if stability_check_data is not None and stability_check_target_data is not None:
+                if len(stability_check_data) != len(stability_check_target_data) or \
+                        any(stability_check_data.index != stability_check_target_data.index):
+                    raise ValueError("Stability check data and target data indexes are different.")
+
     def _check_target_data(self, target_data: pd.Series, stability_check_target_data: pd.Series,
                            target_native_type: ColumnNativeType):
         change_valid_data = False
         if self.settings.target_type == TargetType.BINARY and target_native_type != ColumnNativeType.Numeric:
             if self.settings.stability_check and (stability_check_target_data is not None):
                 valid_target_type = get_column_native_type(pd.DataFrame(data=stability_check_target_data,
                                                                         columns=["target"]), "target")
@@ -122,27 +140,27 @@
                                              self.settings.max_leaf_nodes, x_tmp, y_tmp, col)
         del x_tmp
         # Prepare coarse class summary table
         dt_df = self._prepare_cc_summary(dt_df, y_tmp, col, y_train.count())
         return dt_df, x_val_tmp, y_val_tmp, null_char_table, null_cc_table, char_df
 
     def _prepare_train_and_validation_data(self, x_train: pd.DataFrame, y_train: pd.Series,
-                                           stability_target_data: pd.Series) \
+                                           stability_check_data: pd.DataFrame, stability_target_data: pd.Series) \
             -> Tuple[pd.DataFrame, pd.Series, pd.DataFrame, pd.Series]:
         """prepares train and validation data sets"""
         # Get validation data for stability check
         if self.settings.stability_check:
-            if self.settings.stability_check_data is None:
+            if stability_check_data is None:
                 x_train, y_train, x_valid, y_valid = get_train_test_split_from_strata(x_train,
                                                                                       y_train,
                                                                                       self.settings.test_ratio,
                                                                                       self.settings.random_state)
             else:
                 y_valid = stability_target_data
-                x_valid = self.settings.stability_check_data
+                x_valid = stability_check_data
         else:
             valid_indices = get_sample_indices_from_series(y_train, self.settings.test_ratio,
                                                            self.settings.random_state)
             x_valid, y_valid = x_train.loc[valid_indices], y_train.loc[valid_indices]
         return x_train, y_train, x_valid, y_valid
 
     @staticmethod
@@ -153,15 +171,15 @@
         return x_train.dropna(), y_train.loc[y_train.index.isin(x_train.dropna().index)], \
                x_valid.dropna(), y_valid.loc[
                    y_valid.index.isin(x_valid.dropna().index)], y_nulls, y_valid_nulls
 
     @staticmethod
     def _fill_cc_table_for_nulls(y_nulls: pd.Series, y_valid_nulls: pd.Series, col, target_mean: float,
                                  class_count: int):
-        y_null_mean = round(y_nulls.mean(), 2) if len(y_nulls) > 0 else float("nan")
+        y_null_mean = y_nulls.mean() if len(y_nulls) > 0 else float("nan")
         null_char_table = pd.DataFrame(
             {"char_value": ["NULL"],
              "num_value": [y_null_mean],
              "variable": [col]})
         null_char_table["num_value"].fillna(target_mean, inplace=True)
         null_cc_table = pd.DataFrame(
             {"class_min": [y_nulls.min()], "class_max": [y_nulls.max()], "class_count": [y_nulls.count()],
@@ -189,29 +207,31 @@
         char_df.columns = [column_name, column_name + '_num']
         data['indexcol'] = data.index
         data = pd.merge(data, char_df, how='left', on=column_name, copy=False)
         data = data.drop([column_name, "target"], axis=1).rename(
             columns={column_name + '_num': column_name})
         data.set_index('indexcol', inplace=True)
         char_df.columns = ['char_value', 'num_value']
-        char_df["num_value"] = round(char_df["num_value"], 2)
+        char_df["num_value"] = char_df["num_value"]
         char_df['variable'] = column_name
         return char_df, data[column_name]
 
     @staticmethod
     def _build_decision_tree_df(target_type: TargetType, min_class_size: int, max_leaf_nodes: int,
                                 x_fit_all: pd.Series, y_fit: pd.Series, column_name: str) -> pd.DataFrame:
         dt_df = pd.DataFrame(columns=[column_name, 'dt'])
         dt_df[column_name] = x_fit_all
         if target_type == TargetType.BINARY:
+            from sklearn.tree import DecisionTreeClassifier  # pylint: disable=import-outside-toplevel
             dt_classifier = DecisionTreeClassifier(min_samples_leaf=min_class_size,
                                                    max_leaf_nodes=max_leaf_nodes)
             dt_classifier.fit(x_fit_all.values.reshape(-1, 1), y_fit.values.reshape(-1, 1))
             dt_df["dt"] = dt_classifier.predict_proba(x_fit_all.values.reshape(-1, 1))[:, 1]
         elif target_type == TargetType.SCALAR:
+            from sklearn.tree import DecisionTreeRegressor  # pylint: disable=import-outside-toplevel
             dt_regressor = DecisionTreeRegressor(min_samples_leaf=min_class_size,
                                                  max_leaf_nodes=max_leaf_nodes)
             dt_regressor.fit(x_fit_all.values.reshape(-1, 1), y_fit.values.reshape(-1, 1))
             dt_df["dt"] = dt_regressor.predict(x_fit_all.values.reshape(-1, 1))
         return dt_df
 
     def _prepare_cc_summary(self, dt_df: pd.DataFrame, y_train: pd.Series,
@@ -445,16 +465,16 @@
 
     def _fill_nulls(self, x_df: pd.Series, c_series: pd.Series, c_df: pd.DataFrame, cc_table: pd.DataFrame,
                     with_class_value: bool) -> Tuple[
         pd.Series, pd.DataFrame]:
         if with_class_value:
             c_df.loc[c_series.isnull(), "C_col"] = "null"
         return pd.Series(data=np.where(x_df.isnull(),
-                                       round(cc_table[cc_table['class'] == "null"][
-                                                 'class_target_mean'] - self.fit_output.target_mean, 3),
+                                       cc_table[cc_table['class'] == "null"][
+                                           'class_target_mean'] - self.fit_output.target_mean,
                                        x_df)), c_df
 
     @staticmethod
     def _fill_outliers(x_df: pd.Series, c_series: pd.Series, c_df: pd.DataFrame, cc_table: pd.DataFrame,
                        with_class_value: bool) -> Tuple[
         pd.Series, pd.DataFrame]:
         minn = cc_table[cc_table["class"] != "null"]['class_min'].min()
@@ -476,33 +496,33 @@
         res_df = pd.DataFrame(columns=["column", "transformed"])
         res_df["column"] = x_df
         res_df["transformed"] = 0
         categories = []
         for class_no in cc_table[cc_table["class"] != "null"]["class_no"]:
             res_df.loc[res_df["column"].isin(
                 cc_table[cc_table['class_no'] == class_no]['class'].values[0].split(',')), "transformed"] = \
-                round(cc_table[cc_table['class_no'] == class_no]['class_target_mean'].values[0] - \
-                      self.fit_output.target_mean, 3)
+                cc_table[cc_table['class_no'] == class_no]['class_target_mean'].values[0] - \
+                self.fit_output.target_mean
             if with_class_value:
                 category = cc_table[cc_table['class_no'] == class_no]['class'].values[0]
                 category_values = category.split(',')
                 c_df.loc[c_df["C_col"].isin(category_values), "C_col"] = category
                 categories.extend(category_values)
         res_df.loc[res_df["column"].isnull(), "transformed"] = \
-            round(cc_table[cc_table['class'] == "null"]['class_target_mean'].values[0] - self.fit_output.target_mean, 3)
+            cc_table[cc_table['class'] == "null"]['class_target_mean'].values[0] - self.fit_output.target_mean
         if with_class_value:
             c_df.loc[c_series.notna() & ~c_series.isin(categories), "C_col"] = "Other (Unseen)"
             c_df.loc[c_series.isnull(), "C_col"] = "null"
         return res_df["transformed"], c_df
 
     def _fill_for_not_objects(self, x_df: pd.Series, c_series: pd.Series, c_df: pd.DataFrame, cc_table: pd.DataFrame,
                               with_class_value: bool) -> Tuple[pd.Series, pd.DataFrame]:
         for class_no in cc_table[cc_table["class"] != "null"]["class_no"]:
             minn = cc_table[cc_table["class_no"] == class_no]["class_min"].values[0]
             maxx = cc_table[cc_table["class_no"] == class_no]["class_max"].values[0]
             meann = cc_table[cc_table['class_no'] == class_no]['class_target_mean'].values[0]
-            x_df = np.where((x_df >= minn) & (x_df < maxx), round(meann - self.fit_output.target_mean, 3), x_df)
+            x_df = np.where((x_df >= minn) & (x_df < maxx), meann - self.fit_output.target_mean, x_df)
             if with_class_value:
                 category = cc_table[cc_table["class_no"] == class_no]["class"].values[0]
                 c_df.loc[((~c_series.isin([np.inf, -np.inf, np.nan])) & (c_series >= minn) & (
                         c_series < maxx)), "C_col"] = category
         return x_df, c_df
```

### Comparing `autonon-0.3.0.post1/organon/ml/preprocessing/domain/services/imputation_service.py` & `autonon-0.4.0/organon/ml/preprocessing/domain/services/imputation_service.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Includes ImputationService class."""
 from typing import List, Union, Dict, Type
 
+import numpy as np
 import pandas as pd
 # this import must stay: https://github.com/scikit-learn/scikit-learn/issues/16833
 # noinspection PyUnresolvedReferences
 from sklearn.experimental import enable_iterative_imputer  # pylint: disable=unused-import
 from sklearn.impute import IterativeImputer
 from sklearn.impute import SimpleImputer
 
@@ -19,43 +20,47 @@
 
 class ImputationService:
     """Service for null value imputation"""
 
     def __init__(self, settings: ImputationSettings):
         self.settings = settings
         self.fit_output: ImputationFitOutput = None
-        self.numerical_col_list: List = []
-        self.categorical_col_list: List = []
+        self.numerical_col_list: List[str] = None
+        self.categorical_col_list: List[str] = None
 
-    def fit(self) -> ImputationFitOutput:
+    def fit(self, data: pd.DataFrame) -> ImputationFitOutput:
         """Fits train data by categorical and numeric imputers based on whether a col is numeric or not"""
-        self._fill_column_lists()
+        if data is None or data.empty:
+            raise ValueError("Imputer cannot be fit. Data is not provided.")
+        if self.settings.categorical_data_method == ImputerType.ITERATIVE:
+            raise ValueError("IterativeImputer cannot be used for categorical columns")
+        self._fill_column_lists(data)
         fit_output = ImputationFitOutput()
         fit_output.numerical_imputer = {}
         fit_output.categorical_imputer = {}
         categorical_imputer = self._get_imputer(self.settings.categorical_data_method)
         categorical_imputer_params = self._get_params(self.settings.categorical_data_method,
                                                       self.settings.c_strategy, self.settings.c_missing_values,
                                                       self.settings.c_fill_value)
         for col in self.categorical_col_list:
             imputer = categorical_imputer(**categorical_imputer_params)
-            imputer.fit(self.settings.train_data[col].values.reshape(-1, 1))
+            imputer.fit(data[[col]])
             fit_output.categorical_imputer[col] = imputer
         numerical_imputer = self._get_imputer(self.settings.numeric_data_method)
         numerical_imputer_params = self._get_params(self.settings.numeric_data_method, self.settings.n_strategy,
                                                     self.settings.n_missing_values, self.settings.n_fill_value)
 
         if self.settings.numeric_data_method == ImputerType.SIMPLE:
             for col in self.numerical_col_list:
                 imputer = numerical_imputer(**numerical_imputer_params)
-                imputer.fit(self.settings.train_data[col].values.reshape(-1, 1))
+                imputer.fit(data[[col]])
                 fit_output.numerical_imputer[col] = imputer
         else:
             imputer = numerical_imputer(**numerical_imputer_params)
-            imputer.fit(self.settings.train_data[self.numerical_col_list])
+            imputer.fit(data[self.numerical_col_list])
             fit_output.numerical_imputer = imputer
         self.fit_output = fit_output
         return fit_output
 
     @staticmethod
     def _get_imputer(imputing_method: ImputerType) -> Union[Type[SimpleImputer], Type[IterativeImputer]]:
         if imputing_method is ImputerType.SIMPLE:
@@ -66,64 +71,105 @@
     def _get_params(imputing_method: ImputerType, strategy: str,
                     missing_values: Union[int, float, str, None],
                     fill_value: Union[float, str, int]) -> Dict:
         if imputing_method is ImputerType.SIMPLE:
             return get_params({"strategy": strategy, "missing_values": missing_values, "fill_value": fill_value})
         return get_params({"initial_strategy": strategy, "missing_values": missing_values})
 
-    def transform(self, data: pd.DataFrame, inplace: bool = False) -> pd.DataFrame:
+    def transform(self, data: pd.DataFrame, inplace: bool = False,
+                  ignore_extra_columns: bool = False) -> pd.DataFrame:
         """Fills missing values in data and return it."""
         if self.fit_output is None:
             raise ValueError("Imputer not fitted yet. Run fit method first.")
+
+        self._validate_transformation_data(data, ignore_extra_columns)
+
         if not inplace:
             trans_data = data.copy()
         else:
             trans_data = data
-        different_columns = [col for col in trans_data.columns if col not in self.settings.train_data.columns]
-        if different_columns:
-            raise ValueError(f"These columns are not found in the train data: {', '.join(different_columns)}.")
-        if self.settings.included_columns is None:
-            different_typed_columns = [col for col in trans_data if
-                                       (get_column_native_type(trans_data, col) != get_column_native_type(
-                                           self.settings.train_data, col))]
-        else:
-            different_typed_columns = [col for col in data if
-                                       (get_column_native_type(trans_data, col) != get_column_native_type(
-                                           self.settings.train_data, col)) and
-                                       (col in self.settings.included_columns)]
-        if different_typed_columns:
-            raise ValueError(
-                f"Type of these columns are different in the train data: {', '.join(different_typed_columns)}.")
         categorical_col_list = [col for col in trans_data.columns if col in self.categorical_col_list]
         numerical_col_list = [col for col in trans_data.columns if col in self.numerical_col_list]
+
         for col in categorical_col_list:
             self._try_set_col_after_transform(trans_data, col, self.fit_output.categorical_imputer[col])
         if isinstance(self.fit_output.numerical_imputer, IterativeImputer):
-            if numerical_col_list != self.numerical_col_list:
-                raise ValueError("Transformation numeric columns do not match train numeric columns.")
             trans_data[self.numerical_col_list] = self.fit_output.numerical_imputer.transform(
                 trans_data[self.numerical_col_list])
         else:
             for col in numerical_col_list:
                 self._try_set_col_after_transform(trans_data, col, self.fit_output.numerical_imputer[col])
         return trans_data
 
+    def _validate_transformation_data(self, trans_data: pd.DataFrame, ignore_extra_columns: bool):
+        self._check_extra_columns_in_transformation_data(trans_data, ignore_extra_columns)
+
+        if isinstance(self.fit_output.numerical_imputer, IterativeImputer):
+            missing_cols = [col for col in self.numerical_col_list if col not in trans_data.columns]
+            if missing_cols:
+                raise ValueError(f"Following numerical columns should be supplied to transform data: "
+                                 f"{self._get_list_str(missing_cols)}")
+
+        self._check_changed_type_columns(trans_data)
+
+    def _check_extra_columns_in_transformation_data(self, trans_data: pd.DataFrame, ignore_extra_columns: bool):
+        train_cols = self.numerical_col_list + self.categorical_col_list
+        if not ignore_extra_columns:
+            different_columns = [col for col in trans_data.columns if col not in train_cols]
+            if different_columns:
+                raise ValueError(f"Imputer was not fitted for following columns: "
+                                 f"{self._get_list_str(different_columns)}. "
+                                 "Set 'ignore_extra_columns=True' if you want to transform only columns fitted "
+                                 "and ignore others")
+
+    def _check_changed_type_columns(self, trans_data: pd.DataFrame):
+        numerical_changed_type_cols = []
+        for col in self.numerical_col_list:
+            if col in trans_data.columns:
+                if get_column_native_type(trans_data, col) != ColumnNativeType.Numeric:
+                    numerical_changed_type_cols.append(col)
+        if numerical_changed_type_cols:
+            raise ValueError(
+                f"Following columns are expected to be numerical: {self._get_list_str(numerical_changed_type_cols)}")
+        categorical_changed_type_cols = []
+        for col in self.categorical_col_list:
+            if col in trans_data.columns:
+                if get_column_native_type(trans_data, col) != ColumnNativeType.String:
+                    categorical_changed_type_cols.append(col)
+        if categorical_changed_type_cols:
+            raise ValueError(
+                f"Following columns are expected to be categorical: "
+                f"{self._get_list_str(categorical_changed_type_cols)}")
+
     @classmethod
     def _try_set_col_after_transform(cls, trans_data: pd.DataFrame, col: str, imputer):
+        initial_dtype = trans_data[col].dtype
         transformed_arr = imputer.transform(trans_data[[col]])
         if transformed_arr.shape[1] != 0:
             trans_data[col] = transformed_arr
+            if trans_data[col].dtype == np.dtype("O"):
+                # 'imputer.transform' can convert types like Int64DType to object. Here we try to convert it to
+                try:
+                    trans_data[col] = trans_data[col].astype(initial_dtype)
+                except:  # pylint: disable=bare-except
+                    trans_data[col] = trans_data[col].convert_dtypes()
         else:
             if trans_data[col].isna().all():
                 LogHelper.warning(f"Column {col} could not be transformed by imputer since all values are NaN.")
 
-    def _fill_column_lists(self):
+    def _fill_column_lists(self, data: pd.DataFrame):
+        self.numerical_col_list = []
+        self.categorical_col_list = []
         if self.settings.included_columns is None:
-            columns = self.settings.train_data.columns
+            columns = data.columns
         else:
             columns = self.settings.included_columns
         for col in columns:
-            col_type = get_column_native_type(self.settings.train_data, col)
+            col_type = get_column_native_type(data, col)
             if col_type == ColumnNativeType.String:
                 self.categorical_col_list.append(col)
             elif col_type == ColumnNativeType.Numeric:
                 self.numerical_col_list.append(col)
+
+    @staticmethod
+    def _get_list_str(_list: list):
+        return ",".join(_list)
```

### Comparing `autonon-0.3.0.post1/organon/ml/preprocessing/domain/services/scaling_service.py` & `autonon-0.4.0/organon/ml/preprocessing/domain/services/scaling_service.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/preprocessing/helpers/preprocessing_input_helper.py` & `autonon-0.4.0/organon/ml/preprocessing/helpers/preprocessing_input_helper.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/preprocessing/services/preprocessor.py` & `autonon-0.4.0/organon/ml/preprocessing/services/preprocessor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 """Includes Preprocessor class."""
 
 from typing import Union, List
 
-import pandas as pd
-
 from organon.fl.mathematics.constants import INT_MAX
 from organon.ml.common.enums.target_type import TargetType
 from organon.ml.common.helpers.parameter_helper import USE_CLASS_DEFAULT_STR
 from organon.ml.preprocessing.domain.services.coarse_class_service import CoarseClassService
 from organon.ml.preprocessing.domain.services.imputation_service import ImputationService
 from organon.ml.preprocessing.domain.services.one_hot_encoding_service import OneHotEncodingService
 from organon.ml.preprocessing.domain.services.scaling_service import ScalingService
@@ -16,34 +14,28 @@
 from organon.ml.preprocessing.settings.preprocessing_user_input_service import PreprocessingUserInputService
 
 
 class Preprocessor:
     """User interface class for preprocessing module"""
 
     @staticmethod
-    def get_coarse_class_service(data: pd.DataFrame, target_data: pd.Series, test_ratio: float,
-                                 target_column_type: str = TargetType.BINARY.name,
+    def get_coarse_class_service(test_ratio: float, target_column_type: str = TargetType.BINARY.name,
                                  min_class_size: int = 1, max_leaf_nodes: int = 20,
-                                 stability_check_data: pd.DataFrame = None,
-                                 stability_check_target_data: pd.Series = None,
                                  stability_check: bool = True,
                                  stability_threshold: float = 0.30, random_state=42,
                                  positive_class: str = None, negative_class: str = None) -> CoarseClassService:
         """returns coarse class service"""
         # pylint: disable=too-many-arguments
-        cc_input = CoarseInputDto(data, target_data, test_ratio, target_column_type, min_class_size,
-                                  max_leaf_nodes,
-                                  stability_check_data, stability_check_target_data, stability_check,
+        cc_input = CoarseInputDto(test_ratio, target_column_type, min_class_size, max_leaf_nodes, stability_check,
                                   stability_threshold, random_state, positive_class, negative_class)
         cc_settings = PreprocessingUserInputService.get_coarse_class_settings(cc_input)
         return CoarseClassService(cc_settings)
 
     @staticmethod
-    def get_imputation_service(data: pd.DataFrame,
-                               numeric_data_method: str,
+    def get_imputation_service(numeric_data_method: str,
                                categorical_data_method: str = ImputerType.SIMPLE.name,
                                n_missing_values: Union[int, float] = USE_CLASS_DEFAULT_STR,
                                c_missing_values: Union[int, float, str] = USE_CLASS_DEFAULT_STR,
                                n_fill_value: Union[float, int] = USE_CLASS_DEFAULT_STR,
                                c_fill_value: Union[str, float, int] = USE_CLASS_DEFAULT_STR,
                                n_strategy: str = USE_CLASS_DEFAULT_STR,
                                c_strategy: str = 'most_frequent',
@@ -67,16 +59,15 @@
             default: imputer default if None given.
         :param c_strategy: used to fill categorical imputer strategy field.
             default: "most-frequent"
         :param included_columns: columns to impute
             default: "all columns"
         """
         # pylint: disable=too-many-arguments
-        imputation_settings = PreprocessingUserInputService.get_imputation_settings(data,
-                                                                                    numeric_data_method,
+        imputation_settings = PreprocessingUserInputService.get_imputation_settings(numeric_data_method,
                                                                                     categorical_data_method,
                                                                                     n_strategy, c_strategy,
                                                                                     n_missing_values, c_missing_values,
                                                                                     n_fill_value, c_fill_value,
                                                                                     included_columns)
         return ImputationService(imputation_settings)
```

### Comparing `autonon-0.3.0.post1/organon/ml/preprocessing/settings/objects/imputation_settings.py` & `autonon-0.4.0/organon/ml/preprocessing/settings/objects/imputation_settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 """Includes ImputationSettings class."""
 from dataclasses import dataclass
 from typing import Union, List
 
-import pandas as pd
-
 from organon.ml.preprocessing.settings.enums.imputer_type import ImputerType
 
 
 @dataclass
 class ImputationSettings:
     """Settings for Imputation service"""
-    train_data: pd.DataFrame
     numeric_data_method: ImputerType
     categorical_data_method: ImputerType
     n_missing_values: Union[int, float, None]
     c_missing_values: Union[int, float, str, None]
     n_strategy: str
     c_strategy: str
     n_fill_value: Union[float, int]
```

### Comparing `autonon-0.3.0.post1/organon/ml/preprocessing/settings/preprocessing_user_input_service.py` & `autonon-0.4.0/organon/ml/preprocessing/settings/preprocessing_user_input_service.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 """Includes PreprocessingUserInputService class."""
 
 from typing import Union, List
 
-import pandas as pd
-
 from organon.fl.mathematics.constants import INT_MAX
 from organon.ml.common.enums.target_type import TargetType
 from organon.ml.common.helpers.parameter_helper import USE_CLASS_DEFAULT_STR
 from organon.ml.common.helpers.user_input_service_helper import get_enum
 from organon.ml.preprocessing.services.user_settings.coarse_input_dto import CoarseInputDto
 from organon.ml.preprocessing.settings.enums.imputer_type import ImputerType
 from organon.ml.preprocessing.settings.enums.scaler_type import ScalerType
@@ -20,58 +18,43 @@
 class PreprocessingUserInputService:
     """Service for validating user input and generating settings for preprocessor services"""
 
     @classmethod
     def get_coarse_class_settings(cls, cc_input: CoarseInputDto) -> CoarseClassSettings:
         """Validates settings entered by user and generates settings object for CoarseClass service"""
         target_type = get_enum(cc_input.target_column_type, TargetType)
-        cls._validate_cc_settings(cc_input.data, cc_input.target_data, cc_input.target_column_type)
-        cc_settings = CoarseClassSettings(cc_input.data, cc_input.target_data, cc_input.test_ratio,
+        cc_settings = CoarseClassSettings(cc_input.test_ratio,
                                           cc_input.min_class_size, target_type, cc_input.max_leaf_nodes,
-                                          cc_input.stability_check_data, cc_input.stability_check_target_data,
                                           cc_input.stability_check,
                                           cc_input.stability_threshold, cc_input.random_state,
                                           cc_input.positive_class, cc_input.negative_class)
         return cc_settings
 
-    @staticmethod
-    def _validate_cc_settings(data: pd.DataFrame, strata_data: pd.Series, target_column_type: str):
-        if data is None or data.empty:
-            raise ValueError("Data cannot be empty or None.")
-        if target_column_type not in [TargetType.SCALAR.name, TargetType.BINARY.name]:
-            raise ValueError("Target type should be scalar or binary.")
-        if strata_data.nunique() > 2 and target_column_type == TargetType.BINARY.name:
-            raise ValueError("Target type is binary but target contains more than two classes.")
-        if any(data.index != strata_data.index):
-            raise ValueError("Data and target indexes are different.")
-
     @classmethod
-    def get_imputation_settings(cls, data: pd.DataFrame, numeric_data_method: str,
+    def get_imputation_settings(cls, numeric_data_method: str,
                                 categorical_data_method: str = ImputerType.SIMPLE.name,
                                 n_strategy: str = USE_CLASS_DEFAULT_STR, c_strategy: str = 'most_frequent',
                                 n_missing_values: Union[int, float, None] = USE_CLASS_DEFAULT_STR,
                                 c_missing_values: Union[int, float, str, None] = USE_CLASS_DEFAULT_STR,
                                 n_fill_value: Union[float, int] = USE_CLASS_DEFAULT_STR,
                                 c_fill_value: Union[
                                     str, float, int] = USE_CLASS_DEFAULT_STR,
                                 included_columns: List[str] = None) -> ImputationSettings:
         """Validates settings entered by user and generates settings object for Imputation service"""
         # pylint: disable=too-many-arguments
         numeric_imputer_type = get_enum(numeric_data_method, ImputerType)
         categorical_imputer_type = get_enum(categorical_data_method, ImputerType)
-        cls._validate_imputation_settings(data, numeric_imputer_type, categorical_imputer_type, c_strategy)
-        return ImputationSettings(data, numeric_imputer_type, ImputerType.SIMPLE, n_missing_values,
+        cls._validate_imputation_settings(numeric_imputer_type, categorical_imputer_type, c_strategy)
+        return ImputationSettings(numeric_imputer_type, ImputerType.SIMPLE, n_missing_values,
                                   c_missing_values, n_strategy, c_strategy, n_fill_value, c_fill_value,
                                   included_columns)
 
     @staticmethod
-    def _validate_imputation_settings(data: pd.DataFrame, numeric_imputer_type: ImputerType,
+    def _validate_imputation_settings(numeric_imputer_type: ImputerType,
                                       categorical_imputer_type: ImputerType, c_strategy: str):
-        if data is None or data.empty:
-            raise ValueError("Imputation will not be executed. Data is not provided.")
         if numeric_imputer_type is None:
             raise ValueError("Numeric imputer type is None.")
         if categorical_imputer_type != ImputerType.SIMPLE:
             raise ValueError(
                 "The given categorical data imputer cannot be used. Please select SIMPLE as imputer.")
         if c_strategy not in ["most_frequent", "constant"]:
             raise ValueError(
```

### Comparing `autonon-0.3.0.post1/organon/ml/reporting/domain/services/base_reporter_service.py` & `autonon-0.4.0/organon/ml/reporting/domain/services/base_reporter_service.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/reporting/domain/services/binary_reporter_service.py` & `autonon-0.4.0/organon/ml/reporting/domain/services/binary_reporter_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,17 +58,17 @@
             general_performance, bin_performances, target_based_score_perf = cls.__get_details(settings, settings.data)
             performance_summary_df = pd.DataFrame([general_performance], columns=perf_sum_columns)
             detailed_performance_summary_df = pd.DataFrame(bin_performances, columns=detailed_perf_sum_columns)
             target_based_summary_df = pd.DataFrame([target_based_score_perf],
                                                    columns=target_based_summary_columns)
 
         report = BinaryReport()
-        report.performance_summary = performance_summary_df
+        report.performance_summary = performance_summary_df.T
         report.detailed_performance_summary = detailed_performance_summary_df
-        report.target_based_performance_summary = target_based_summary_df
+        report.target_based_performance_summary = target_based_summary_df.T
         return report
 
     @classmethod
     def __get_details(cls, settings, all_data):
         total_row_count = len(all_data)
         if settings.num_bins > total_row_count:
             raise ValueError("num_bins cannot be higher than number of rows in a set")
@@ -79,30 +79,31 @@
         total_pos_count = 0
         score_col = settings.score_column
 
         for bin_num in range(settings.num_bins):
             data = all_data.loc[bins == bin_num]
             total_count, positive_count, negative_count = cls.__get_row_positive_negative_count(data,
                                                                                                 settings.target_column)
-            total_pos_count += positive_count
-            total_neg_count += negative_count
 
             bin_dicts.append({
                 "BIN": bin_num,
                 "TOTAL COUNT": total_count,
                 "POSITIVE COUNT": positive_count,
                 "NEGATIVE COUNT": negative_count,
                 "TARGET RATIO": positive_count / total_count,
                 "SCORE AVG": data[score_col].mean(),
                 "SCORE SUM": data[score_col].sum(),
                 "SCORE MIN": data[score_col].min(),
                 "SCORE MAX": data[score_col].max(),
                 "TRUE NEGATIVE COUNT": total_neg_count,
                 "FALSE NEGATIVE COUNT": total_pos_count,
             })
+            total_pos_count += positive_count
+            total_neg_count += negative_count
+
         true_positive_count = 0
         false_positive_count = 0
 
         general_performance_dict = cls._get_general_performance_dict(all_data, settings, total_row_count,
                                                                      total_pos_count, total_neg_count)
         total_pos_ratio = general_performance_dict["POSITIVE RATIO"]
         pos_count_sum = 0
@@ -175,15 +176,15 @@
         general_performance_dict = {
             "ROW COUNT": total_row_count,
             "POSITIVE COUNT": total_pos_count,
             "NEGATIVE COUNT": total_neg_count,
             "POSITIVE RATIO": total_pos_count / total_row_count,
             "NEGATIVE RATIO": total_neg_count / total_row_count,
             "ODDS": total_pos_count / total_neg_count,
-            "AUC": roc_auc_score(all_data[settings.target_column], all_data[score_col] > 0.5),
+            "AUC": roc_auc_score(all_data[settings.target_column], all_data[score_col]),
             "SCORE AVG": aggregates["mean"],
             "SCORE STD": aggregates["std"],
             "SCORE MIN": aggregates["min"],
             "SCORE MAX": aggregates["max"],
             "SCORE P25": percentiles[0],
             "SCORE MEDIAN": percentiles[1],
             "SCORE P75": percentiles[2],
@@ -221,15 +222,15 @@
             columns = ["SPLIT"] + columns
         if id_str_col_exists:
             columns = ["ID_STR"] + columns
         return columns
 
     @classmethod
     def __get_columns_for_target_based_performance_summary_df(cls, id_str_col_exists: bool, split_col_exists: bool):
-        suffixes = ["COUNT", "STD", "MIN"]
+        suffixes = ["COUNT", "STD", "MEAN", "MIN"]
         suffixes.extend([f"P{5 * i}" for i in range(1, 20)])
         suffixes.append("MAX")
         columns = [f"{prefix} {suffix}" for prefix in ["POSITIVES", "NEGATIVES"] for suffix in suffixes]
         if split_col_exists:
             columns = ["SPLIT"] + columns
         if id_str_col_exists:
             columns = ["ID_STR"] + columns
```

### Comparing `autonon-0.3.0.post1/organon/ml/reporting/domain/services/regression_reporter_service.py` & `autonon-0.4.0/organon/ml/reporting/domain/services/regression_reporter_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Includes RegressionReporterService class."""
 from typing import List, Tuple
 
 import numpy as np
 import pandas as pd
 from sklearn.metrics import mean_absolute_error
-from sklearn.metrics import mean_squared_error
+from sklearn.metrics import mean_squared_error, mean_squared_log_error
 from sklearn.metrics import r2_score
 
 from organon.ml.common.helpers.df_ops_helper import get_bins
 from organon.ml.reporting.domain.objects.regression_report import RegressionReport
 from organon.ml.reporting.domain.services.base_reporter_service import BaseReporterService
 from organon.ml.reporting.settings.objects.reporter_settings import ReporterSettings
 
@@ -51,17 +51,16 @@
         report.performance_summary = performance_summary_table
         report.lift_table = lift_table
         return report
 
     @staticmethod
     def _get_lift_and_perf_columns(idstr_exists=False, split_exists=False) -> Tuple[List, List]:
         lift_columns = ["Bin", "Total Count", "Target Average", "Score Average", "Cumulative Lift"]
-        perf_summary_columns = ["MSE", "MAA", "MAPE", "R2", "ROW COUNT", "TARGET AVG", "SCORE AVG", "SCORE STD",
-                                "SCORE MIN",
-                                "SCORE P25", "SCORE MEDIAN", "SCORE P75", "SCORE MAX"]
+        perf_summary_columns = ["MSE", "RMSE", "MAA", "MAPE", "MSLOGE", "R2", "ROW COUNT", "TARGET AVG", "SCORE AVG",
+                                "SCORE STD", "SCORE MIN", "SCORE P25", "SCORE MEDIAN", "SCORE P75", "SCORE MAX"]
         if split_exists:
             lift_columns.insert(0, "Data")
             perf_summary_columns.insert(0, "Data")
         if idstr_exists:
             lift_columns.insert(0, "IdStr")
             perf_summary_columns.insert(0, "IdStr")
         return lift_columns, perf_summary_columns
@@ -88,22 +87,25 @@
             bin_target_avg = data_bins[target_column].mean()
             bin_length = len(data_bins)
             cumulative_sum += bin_target_avg * bin_length
             cumulative_count += bin_length
             bin_list.append([bin_num, bin_length, bin_target_avg,
                              data_bins[score_column].mean(),
                              cumulative_sum / (cumulative_count * target_avg)])
+        bin_list.reverse()
         return bin_list
 
     def _calc_performance_summary_for_split(self, split_data: pd.DataFrame, target_col: str, prediction_col: str):
         df_statistics = split_data[prediction_col].agg(["mean", "std", "min", "max", "median"])
         percentiles = np.percentile(split_data[prediction_col], [25, 50, 75])
         return pd.Series(data=[mean_squared_error(split_data[target_col], split_data[prediction_col]),
+                               mean_squared_error(split_data[target_col], split_data[prediction_col], squared=False),
                                mean_absolute_error(split_data[target_col], split_data[prediction_col]),
                                self._mean_absolute_percentage_error(split_data[target_col], split_data[prediction_col]),
+                               mean_squared_log_error(split_data[target_col], split_data[prediction_col]),
                                r2_score(split_data[target_col], split_data[prediction_col]),
                                len(split_data),
                                split_data[target_col].mean(),
                                df_statistics["mean"],
                                df_statistics["std"],
                                df_statistics["min"],
                                percentiles[0],
```

### Comparing `autonon-0.3.0.post1/organon/ml/reporting/services/reporter.py` & `autonon-0.4.0/organon/ml/reporting/services/reporter.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,42 @@
 """Includes Reporter class."""
-from typing import Union
+from typing import Union, List
 
+import numpy as np
 import pandas as pd
 
 from organon.ml.common.enums.target_type import TargetType
 from organon.ml.common.helpers.user_input_service_helper import get_enum
 from organon.ml.reporting.domain.objects.binary_report import BinaryReport
 from organon.ml.reporting.domain.objects.multiclass_report import MulticlassReport
 from organon.ml.reporting.domain.objects.regression_report import RegressionReport
 from organon.ml.reporting.domain.services.base_reporter_service import BaseReporterService
 from organon.ml.reporting.domain.services.binary_reporter_service import BinaryReporterService
 from organon.ml.reporting.domain.services.multiclass_reporter_service import MulticlassReporterService
 from organon.ml.reporting.domain.services.regression_reporter_service import RegressionReporterService
+from organon.ml.reporting.settings.objects.multiclass_reporter_settings import MultiClassReporterSettings
 from organon.ml.reporting.settings.objects.reporter_settings import ReporterSettings
 
 
 class Reporter:
     """Modelling performance reporter"""
 
     def __init__(self, data: pd.DataFrame, target_column: str, score_column: str, target_type: str,
-                 id_str_column: str = None, split_column: str = None, num_bins: int = 10):
+                 id_str_column: str = None, split_column: str = None, num_bins: int = 10,
+                 probability_values: np.array = None, ordered_class_names: List = None):
         # pylint: disable=too-many-arguments
-        self._settings = ReporterSettings(data, target_column, score_column, get_enum(target_type, TargetType),
-                                          id_str_column, split_column, num_bins)
+        target_type_enum = get_enum(target_type, TargetType)
+        if target_type_enum == TargetType.MULTICLASS:
+            self._settings = MultiClassReporterSettings(data, target_column, score_column, target_type_enum,
+                                                        id_str_column, split_column, num_bins, probability_values,
+                                                        ordered_class_names)
+        else:
+            self._settings = ReporterSettings(data, target_column, score_column, target_type_enum,
+                                              id_str_column, split_column, num_bins)
+
         self.report: Union[BinaryReport, MulticlassReport, RegressionReport] = None
 
     def execute(self):
         """Generates and returns report"""
         service = self._get_reporter_service()
         self.report = service.execute(self._settings)
         return self.report
```

### Comparing `autonon-0.3.0.post1/organon/ml/sampling/domain/services/sampling_preprocessing_service.py` & `autonon-0.4.0/organon/ml/sampling/domain/services/sampling_preprocessing_service.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/sampling/domain/services/sampling_service.py` & `autonon-0.4.0/organon/ml/sampling/domain/services/sampling_service.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/sampling/services/sampler.py` & `autonon-0.4.0/organon/ml/sampling/services/sampler.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/sampling/settings/objects/sampling_settings.py` & `autonon-0.4.0/organon/ml/sampling/settings/objects/sampling_settings.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/organon/ml/sampling/settings/sampling_user_input_service.py` & `autonon-0.4.0/organon/ml/sampling/settings/sampling_user_input_service.py`

 * *Files identical despite different names*

### Comparing `autonon-0.3.0.post1/setup.py` & `autonon-0.4.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 if __name__ == "__main__":
     with open("README.md", "r") as fh:
         long_description = fh.read()
 
     setup(
         name="autonon",
-        version="0.3.0.post1",
+        version="0.4.0",
         author="Organon Analytics",
         author_email="support@organonanalytics.com",
         description="Organon Automated ML Platform",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://gitlab.com/organon-os/autonon",
         packages=find_packages(exclude=["organon.tests*"]),
@@ -43,15 +43,21 @@
             "scikit-learn>=1.1",
             "lightgbm>=3.2.1",
             "python-dateutil>=2.8.2",
             "six>=1.16.0",
             "seaborn>=0.11.2",
             "xgboost>=1.6.1",
             "scikit-optimize>=0.9.0",
-            "statsmodels >= 0.13.2"
+            "statsmodels >= 0.13.2",
+            "tensorflow>=2.10",
+            "defusedxml >= 0.6.0",
+            "transformers>=4.26.0",
+            "datasets>=2.6.1",
+            "keras>=2.10.0",
+            "ultralytics>=8.0.59"
         ],
         classifiers=[
             "Programming Language :: Python :: 3",
             "License :: OSI Approved :: MIT License",
             "Operating System :: OS Independent",
         ],
         python_requires='>=3.8',
```

