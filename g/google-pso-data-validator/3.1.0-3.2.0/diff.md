# Comparing `tmp/google-pso-data-validator-3.1.0.tar.gz` & `tmp/google-pso-data-validator-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-pso-data-validator-3.1.0.tar", last modified: Mon Apr 24 05:22:28 2023, max compression
+gzip compressed data, was "google-pso-data-validator-3.2.0.tar", last modified: Fri Jun  2 16:20:16 2023, max compression
```

## Comparing `google-pso-data-validator-3.1.0.tar` & `google-pso-data-validator-3.2.0.tar`

### file list

```diff
@@ -1,109 +1,113 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 05:22:28.948369 google-pso-data-validator-3.1.0/
--rw-r--r--   0 root         (0) root         (0)    11358 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    35942 2023-04-24 05:22:28.948369 google-pso-data-validator-3.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    35230 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 05:22:28.912366 google-pso-data-validator-3.1.0/data_validation/
--rw-r--r--   0 root         (0) root         (0)      715 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20439 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/__main__.py
--rw-r--r--   0 root         (0) root         (0)     1986 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/app.py
--rw-r--r--   0 root         (0) root         (0)    44528 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/cli_tools.py
--rw-r--r--   0 root         (0) root         (0)      881 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/client_info.py
--rw-r--r--   0 root         (0) root         (0)    10258 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/clients.py
--rw-r--r--   0 root         (0) root         (0)    13911 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/combiner.py
--rw-r--r--   0 root         (0) root         (0)    34285 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/config_manager.py
--rw-r--r--   0 root         (0) root         (0)     5052 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/consts.py
--rw-r--r--   0 root         (0) root         (0)    16222 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/data_validation.py
--rw-r--r--   0 root         (0) root         (0)      632 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1269 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/jellyfish_distance.py
--rw-r--r--   0 root         (0) root         (0)     2497 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/metadata.py
--rw-r--r--   0 root         (0) root         (0)    10638 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/partition_builder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 05:22:28.916366 google-pso-data-validator-3.1.0/data_validation/query_builder/
--rw-r--r--   0 root         (0) root         (0)      575 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/query_builder/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2880 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/query_builder/partition_row_builder.py
--rw-r--r--   0 root         (0) root         (0)    18741 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/query_builder/query_builder.py
--rw-r--r--   0 root         (0) root         (0)     7520 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/query_builder/random_row_builder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 05:22:28.916366 google-pso-data-validator-3.1.0/data_validation/result_handlers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/result_handlers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3970 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/result_handlers/bigquery.py
--rw-r--r--   0 root         (0) root         (0)     2548 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/result_handlers/text.py
--rw-r--r--   0 root         (0) root         (0)    11146 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/schema_validation.py
--rw-r--r--   0 root         (0) root         (0)     1773 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/secret_manager.py
--rw-r--r--   0 root         (0) root         (0)     9477 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/state_manager.py
--rw-r--r--   0 root         (0) root         (0)    16109 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/validation_builder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 05:22:28.920367 google-pso-data-validator-3.1.0/google_pso_data_validator.egg-info/
--rw-r--r--   0 root         (0) root         (0)    35942 2023-04-24 05:22:28.000000 google-pso-data-validator-3.1.0/google_pso_data_validator.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3483 2023-04-24 05:22:28.000000 google-pso-data-validator-3.1.0/google_pso_data_validator.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 05:22:28.000000 google-pso-data-validator-3.1.0/google_pso_data_validator.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-04-24 05:22:28.000000 google-pso-data-validator-3.1.0/google_pso_data_validator.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      587 2023-04-24 05:22:28.000000 google-pso-data-validator-3.1.0/google_pso_data_validator.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2023-04-24 05:22:28.000000 google-pso-data-validator-3.1.0/google_pso_data_validator.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       67 2023-04-24 05:22:28.948369 google-pso-data-validator-3.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2877 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 05:22:28.892365 google-pso-data-validator-3.1.0/third_party/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 05:22:28.900365 google-pso-data-validator-3.1.0/third_party/ibis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 05:22:28.924367 google-pso-data-validator-3.1.0/third_party/ibis/ibis_DB2/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_DB2/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3434 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_DB2/alchemy.py
--rw-r--r--   0 root         (0) root         (0)     1198 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_DB2/api.py
--rw-r--r--   0 root         (0) root         (0)     7727 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_DB2/client.py
--rw-r--r--   0 root         (0) root         (0)    18668 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_DB2/compiler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 05:22:28.924367 google-pso-data-validator-3.1.0/third_party/ibis/ibis_DB2/expr/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_DB2/expr/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4949 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_DB2/expr/datatypes.py
--rw-r--r--   0 root         (0) root         (0)     2373 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_DB2/expr/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 05:22:28.928367 google-pso-data-validator-3.1.0/third_party/ibis/ibis_addon/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_addon/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1524 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_addon/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 05:22:28.928367 google-pso-data-validator-3.1.0/third_party/ibis/ibis_addon/base_sqlalchemy/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_addon/base_sqlalchemy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7579 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_addon/base_sqlalchemy/alchemy.py
--rw-r--r--   0 root         (0) root         (0)     3551 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_addon/datatypes.py
--rw-r--r--   0 root         (0) root         (0)    12820 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_addon/operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 05:22:28.932368 google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/
--rw-r--r--   0 root         (0) root         (0)        2 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2069 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/api.py
--rw-r--r--   0 root         (0) root         (0)    14574 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/client.py
--rw-r--r--   0 root         (0) root         (0)     1898 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/compiler.py
--rw-r--r--   0 root         (0) root         (0)     2750 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/datatypes.py
--rw-r--r--   0 root         (0) root         (0)     3789 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 05:22:28.932368 google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/tests/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4944 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)    14058 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/tests/test_client.py
--rw-r--r--   0 root         (0) root         (0)    14908 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/tests/test_compiler.py
--rw-r--r--   0 root         (0) root         (0)     1916 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/tests/test_datatypes.py
--rw-r--r--   0 root         (0) root         (0)     1494 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/to_pandas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 05:22:28.936368 google-pso-data-validator-3.1.0/third_party/ibis/ibis_impala/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_impala/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7010 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_impala/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 05:22:28.936368 google-pso-data-validator-3.1.0/third_party/ibis/ibis_mssql/
--rw-r--r--   0 root         (0) root         (0)       69 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_mssql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4042 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_mssql/api.py
--rw-r--r--   0 root         (0) root         (0)     8514 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_mssql/client.py
--rw-r--r--   0 root         (0) root         (0)    14803 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_mssql/compiler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 05:22:28.940368 google-pso-data-validator-3.1.0/third_party/ibis/ibis_mssql/expr/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_mssql/expr/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4032 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_mssql/expr/api.py
--rw-r--r--   0 root         (0) root         (0)     1867 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_mssql/expr/operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 05:22:28.940368 google-pso-data-validator-3.1.0/third_party/ibis/ibis_oracle/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_oracle/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2135 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_oracle/alchemy.py
--rw-r--r--   0 root         (0) root         (0)     1215 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_oracle/api.py
--rw-r--r--   0 root         (0) root         (0)     9908 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_oracle/client.py
--rw-r--r--   0 root         (0) root         (0)    17172 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_oracle/compiler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 05:22:28.944369 google-pso-data-validator-3.1.0/third_party/ibis/ibis_oracle/expr/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_oracle/expr/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6010 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_oracle/expr/datatypes.py
--rw-r--r--   0 root         (0) root         (0)     2449 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_oracle/expr/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 05:22:28.944369 google-pso-data-validator-3.1.0/third_party/ibis/ibis_oracle/udf/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_oracle/udf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6995 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_oracle/udf/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 05:22:28.944369 google-pso-data-validator-3.1.0/third_party/ibis/ibis_postgres/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_postgres/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4788 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_postgres/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 05:22:28.948369 google-pso-data-validator-3.1.0/third_party/ibis/ibis_teradata/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_teradata/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1494 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_teradata/api.py
--rw-r--r--   0 root         (0) root         (0)     9302 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_teradata/client.py
--rw-r--r--   0 root         (0) root         (0)    26138 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_teradata/compiler.py
--rw-r--r--   0 root         (0) root         (0)     4738 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_teradata/datatypes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:20:16.191492 google-pso-data-validator-3.2.0/
+-rw-r--r--   0 root         (0) root         (0)    11358 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    37001 2023-06-02 16:20:16.191492 google-pso-data-validator-3.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    36289 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:20:16.143489 google-pso-data-validator-3.2.0/data_validation/
+-rw-r--r--   0 root         (0) root         (0)      715 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20968 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     1986 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/app.py
+-rw-r--r--   0 root         (0) root         (0)    45053 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/cli_tools.py
+-rw-r--r--   0 root         (0) root         (0)      881 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/client_info.py
+-rw-r--r--   0 root         (0) root         (0)    10409 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/clients.py
+-rw-r--r--   0 root         (0) root         (0)    13911 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/combiner.py
+-rw-r--r--   0 root         (0) root         (0)    34436 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/config_manager.py
+-rw-r--r--   0 root         (0) root         (0)     5052 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/consts.py
+-rw-r--r--   0 root         (0) root         (0)    16222 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/data_validation.py
+-rw-r--r--   0 root         (0) root         (0)      632 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1269 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/jellyfish_distance.py
+-rw-r--r--   0 root         (0) root         (0)     2497 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/metadata.py
+-rw-r--r--   0 root         (0) root         (0)    10638 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/partition_builder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:20:16.147489 google-pso-data-validator-3.2.0/data_validation/query_builder/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/query_builder/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2880 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/query_builder/partition_row_builder.py
+-rw-r--r--   0 root         (0) root         (0)    18741 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/query_builder/query_builder.py
+-rw-r--r--   0 root         (0) root         (0)     7520 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/query_builder/random_row_builder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:20:16.147489 google-pso-data-validator-3.2.0/data_validation/result_handlers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/result_handlers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3970 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/result_handlers/bigquery.py
+-rw-r--r--   0 root         (0) root         (0)     2548 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/result_handlers/text.py
+-rw-r--r--   0 root         (0) root         (0)    11146 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/schema_validation.py
+-rw-r--r--   0 root         (0) root         (0)     1773 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/secret_manager.py
+-rw-r--r--   0 root         (0) root         (0)     9481 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/state_manager.py
+-rw-r--r--   0 root         (0) root         (0)    16109 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/validation_builder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:20:16.151489 google-pso-data-validator-3.2.0/google_pso_data_validator.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    37001 2023-06-02 16:20:16.000000 google-pso-data-validator-3.2.0/google_pso_data_validator.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3610 2023-06-02 16:20:16.000000 google-pso-data-validator-3.2.0/google_pso_data_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 16:20:16.000000 google-pso-data-validator-3.2.0/google_pso_data_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-06-02 16:20:16.000000 google-pso-data-validator-3.2.0/google_pso_data_validator.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      587 2023-06-02 16:20:16.000000 google-pso-data-validator-3.2.0/google_pso_data_validator.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2023-06-02 16:20:16.000000 google-pso-data-validator-3.2.0/google_pso_data_validator.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2023-06-02 16:20:16.191492 google-pso-data-validator-3.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2877 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:20:16.123487 google-pso-data-validator-3.2.0/third_party/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:20:16.127488 google-pso-data-validator-3.2.0/third_party/ibis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:20:16.155490 google-pso-data-validator-3.2.0/third_party/ibis/ibis_DB2/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_DB2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3434 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_DB2/alchemy.py
+-rw-r--r--   0 root         (0) root         (0)     1198 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_DB2/api.py
+-rw-r--r--   0 root         (0) root         (0)     7727 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_DB2/client.py
+-rw-r--r--   0 root         (0) root         (0)    18668 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_DB2/compiler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:20:16.155490 google-pso-data-validator-3.2.0/third_party/ibis/ibis_DB2/expr/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_DB2/expr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4949 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_DB2/expr/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)     2373 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_DB2/expr/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:20:16.159490 google-pso-data-validator-3.2.0/third_party/ibis/ibis_addon/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_addon/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1524 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_addon/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:20:16.159490 google-pso-data-validator-3.2.0/third_party/ibis/ibis_addon/base_sqlalchemy/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_addon/base_sqlalchemy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7579 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_addon/base_sqlalchemy/alchemy.py
+-rw-r--r--   0 root         (0) root         (0)     3551 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_addon/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)    13566 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_addon/operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:20:16.167491 google-pso-data-validator-3.2.0/third_party/ibis/ibis_cloud_spanner/
+-rw-r--r--   0 root         (0) root         (0)        2 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_cloud_spanner/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2069 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_cloud_spanner/api.py
+-rw-r--r--   0 root         (0) root         (0)    14574 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_cloud_spanner/client.py
+-rw-r--r--   0 root         (0) root         (0)     1898 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_cloud_spanner/compiler.py
+-rw-r--r--   0 root         (0) root         (0)     2750 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_cloud_spanner/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)     3789 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_cloud_spanner/table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:20:16.171491 google-pso-data-validator-3.2.0/third_party/ibis/ibis_cloud_spanner/tests/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_cloud_spanner/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4944 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_cloud_spanner/tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)    14058 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_cloud_spanner/tests/test_client.py
+-rw-r--r--   0 root         (0) root         (0)    14908 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_cloud_spanner/tests/test_compiler.py
+-rw-r--r--   0 root         (0) root         (0)     1916 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_cloud_spanner/tests/test_datatypes.py
+-rw-r--r--   0 root         (0) root         (0)     1494 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_cloud_spanner/to_pandas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:20:16.171491 google-pso-data-validator-3.2.0/third_party/ibis/ibis_impala/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_impala/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7090 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_impala/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:20:16.175491 google-pso-data-validator-3.2.0/third_party/ibis/ibis_mssql/
+-rw-r--r--   0 root         (0) root         (0)       69 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_mssql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4042 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_mssql/api.py
+-rw-r--r--   0 root         (0) root         (0)     9537 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_mssql/client.py
+-rw-r--r--   0 root         (0) root         (0)    15249 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_mssql/compiler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:20:16.175491 google-pso-data-validator-3.2.0/third_party/ibis/ibis_mssql/expr/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_mssql/expr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4032 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_mssql/expr/api.py
+-rw-r--r--   0 root         (0) root         (0)     1867 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_mssql/expr/operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:20:16.179491 google-pso-data-validator-3.2.0/third_party/ibis/ibis_oracle/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_oracle/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2135 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_oracle/alchemy.py
+-rw-r--r--   0 root         (0) root         (0)     1215 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_oracle/api.py
+-rw-r--r--   0 root         (0) root         (0)     9908 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_oracle/client.py
+-rw-r--r--   0 root         (0) root         (0)    17172 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_oracle/compiler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:20:16.179491 google-pso-data-validator-3.2.0/third_party/ibis/ibis_oracle/expr/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_oracle/expr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6010 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_oracle/expr/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)     2449 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_oracle/expr/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:20:16.183492 google-pso-data-validator-3.2.0/third_party/ibis/ibis_oracle/udf/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_oracle/udf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6995 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_oracle/udf/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:20:16.183492 google-pso-data-validator-3.2.0/third_party/ibis/ibis_postgres/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_postgres/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4788 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_postgres/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:20:16.187492 google-pso-data-validator-3.2.0/third_party/ibis/ibis_redshift/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_redshift/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10245 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_redshift/client.py
+-rw-r--r--   0 root         (0) root         (0)      660 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_redshift/compiler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:20:16.187492 google-pso-data-validator-3.2.0/third_party/ibis/ibis_teradata/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_teradata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1494 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_teradata/api.py
+-rw-r--r--   0 root         (0) root         (0)     9302 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_teradata/client.py
+-rw-r--r--   0 root         (0) root         (0)    26138 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_teradata/compiler.py
+-rw-r--r--   0 root         (0) root         (0)     4830 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_teradata/datatypes.py
```

### Comparing `google-pso-data-validator-3.1.0/LICENSE` & `google-pso-data-validator-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/PKG-INFO` & `google-pso-data-validator-3.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-pso-data-validator
-Version: 3.1.0
+Version: 3.2.0
 Summary: A package to enable easy data validation
 Home-page: https://github.com/pypa/sampleproject
 Author: Dylan Hercher
 Author-email: dhercher@google.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -152,15 +152,15 @@
 The default aggregation type is a 'COUNT *'. If no aggregation flag (i.e count,
 sum , min, etc.) is provided, the default aggregation will run.
 
 The [Examples](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/examples.md) page provides many examples of how a tool can be used to run powerful validations without writing any queries.
 
 #### Row Validations
 
-(Note: Row hash validation is currently supported for BigQuery, Teradata, Impala/Hive, Oracle, SQL Server, Postgres, Mysql, Db2 and Alloy DB. Struct and array data types are not currently supported.
+(Note: Row hash validation is currently supported for BigQuery, Teradata, Impala/Hive, Oracle, SQL Server, Redshift, Postgres, Mysql, Db2 and Alloy DB. Struct and array data types are not currently supported.
 In addition, please note that SHA256 is not a supported function on Teradata systems. 
 If you wish to perform this comparison on Teradata you will need to 
 [deploy a UDF to perform the conversion](https://github.com/akuroda/teradata-udf-sha2/blob/master/src/sha256.c).)
 
 Below is the command syntax for row validations. In order to run row level
 validations you need to pass a `--primary-key` flag which defines what field(s)
 the validation will be compared on, as well as either the `--comparison-fields` flag
@@ -197,15 +197,15 @@
   --concat COLUMNS      Comma separated list of columns to concatenate or * for all columns (use if a common hash function is not available between databases)
   [--bq-result-handler or -bqrh PROJECT_ID.DATASET.TABLE]
                         BigQuery destination for validation results. Defaults to stdout.
                         See: *Validation Reports* section
   [--service-account or -sa PATH_TO_SA_KEY]
                         Service account to use for BigQuery result handler output.
   [--filters SOURCE_FILTER:TARGET_FILTER]
-                        Colon spearated string values of source and target filters.
+                        Colon separated string values of source and target filters.
                         If target filter is not provided, the source filter will run on source and target tables.
                         See: *Filters* section
   [--config-file or -c CONFIG_FILE]
                         YAML Config File Path to be used for storing validations.
   [--labels or -l KEY1=VALUE1,KEY2=VALUE2]
                         Comma-separated key value pair labels for the run.
   [--format or -fmt]    Format for stdout output. Supported formats are (text, csv, json, table).
@@ -253,15 +253,15 @@
                         Local: Provide a relative path of the target directory. Eg: `partitions_dir`
   --partition-num [1-1000], -pn [1-1000]
                         Number of partitions/config files to generate
                         In case this value exceeds the row count of the source/target table, it will be decreased to max(source_row_count, target_row_count)
   [--partition-key PARTITION_KEY, -partkey PARTITION_KEY]
                         Column on which the partitions would be generated. Column type must be integer. Defaults to Primary key
   [--filters SOURCE_FILTER:TARGET_FILTER]
-                        Colon spearated string values of source and target filters.
+                        Colon separated string values of source and target filters.
                         If target filter is not provided, the source filter will run on source and target tables.
                         See: *Filters* section
 ```
 #### Schema Validations
 
 Below is the syntax for schema validations. These can be used to compare case insensitive column names and
 types between source and target.
@@ -341,15 +341,15 @@
 
 The [Examples](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/examples.md)
 page provides few examples of how this tool can be used to run custom query validations.
 
 
 #### Custom Query Row Validations 
 
-(Note: Custom query row validation is currently only supported for BigQuery, Teradata, SQL Server, PostgreSQL, Oracle, AlloyDB, and Impala/Hive. Struct and array data types are not currently supported.)
+(Note: Custom query row validation is currently only supported for BigQuery, Teradata, SQL Server, PostgreSQL, Oracle, Redshift, DB2, AlloyDB, and Impala/Hive. Struct and array data types are not currently supported.)
 
 Below is the command syntax for row validations. In order to run row level
 validations you need to pass `--hash` flag which will specify the fields
 of the custom query result that will be concatenated and hashed. The primary key should be included
 in the SELECT statement of both source_query.sql and target_query.sql
 
 Below is the command syntax for custom query row validations.
@@ -392,14 +392,39 @@
   [--filter-status or -fs STATUSES_LIST]
                         Comma separated list of statuses to filter the validation results. Supported statuses are (success, fail). If no list is provided, all statuses are returned.
 ```
 
 The [Examples](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/examples.md)
 page provides few examples of how this tool can be used to run custom query row validations.
 
+#### Dry Run Validation
+
+The `validate` command takes a `--dry-run` command line flag that prints source
+and target SQL to stdout as JSON in lieu of performing a validation:
+
+```
+data-validation (--verbose or -v) (--log-level or -ll) validate
+  [--dry-run or -dr]    Prints source and target SQL to stdout in lieu of performing a validation.
+```
+
+For example, this flag can be used as follows:
+
+```shell
+> data-validation validate --dry-run row \
+  -sc my_bq_conn \
+  -tc my_bq_conn \
+  -tbls bigquery-public-data.new_york_citibike.citibike_stations \
+  --primary-keys station_id \
+  --hash '*'
+{
+    "source_query": "SELECT `hash__all`, `station_id`\nFROM ...",
+    "target_query": "SELECT `hash__all`, `station_id`\nFROM ..."
+}
+```
+
 ### YAML Configuration Files
 
 You can customize the configuration for any given validation by providing use
 case specific CLI arguments or editing the YAML configuration file.
 
 For example, the following command creates a YAML file for the validation of the
 `new_york_citibike` table: `data-validation validate column -sc my_bq_conn -tc
@@ -464,23 +489,23 @@
           The raw query to run against the supplied connection
 ```
 
 ### Building Matched Table Lists
 
 Creating the list of matched tables can be a hassle. We have added a feature
 which may help you to match all of the tables together between source and
-target. The find-tables tool:
+target. The `find-tables` command:
 
--   Pulls all tables in the source (applying a supplied allowed-schemas filter)
+-   Pulls all tables in the source (applying a supplied `allowed-schemas` filter)
 -   Pulls all tables from the target
--   Uses Levenshtein distance to match tables
+-   Uses Jaro Similarity algorithm to match tables
 -   Finally, it prints a JSON list of tables which can be a reference for the
     validation run config.
 
-Note that our score cutoff default is 1. If no matches occur, reduce this value as deemed necessary.
+Note that our default value for the `score-cutoff` parameter is 1 and it seeks for identical matches. If no matches occur, reduce this value as deemed necessary. By using smaller numbers such as 0.7, 0.65 etc you can get more matches. For reference, we make use of [this jaro_similarity method](https://jamesturk.github.io/jellyfish/functions/#jaro-similarity) for the string comparison.
 
 ```
 data-validation find-tables --source-conn source --target-conn target \
     --allowed-schemas pso_data_validator \
     --score-cutoff 1
 ```
```

### Comparing `google-pso-data-validator-3.1.0/README.md` & `google-pso-data-validator-3.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -132,15 +132,15 @@
 The default aggregation type is a 'COUNT *'. If no aggregation flag (i.e count,
 sum , min, etc.) is provided, the default aggregation will run.
 
 The [Examples](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/examples.md) page provides many examples of how a tool can be used to run powerful validations without writing any queries.
 
 #### Row Validations
 
-(Note: Row hash validation is currently supported for BigQuery, Teradata, Impala/Hive, Oracle, SQL Server, Postgres, Mysql, Db2 and Alloy DB. Struct and array data types are not currently supported.
+(Note: Row hash validation is currently supported for BigQuery, Teradata, Impala/Hive, Oracle, SQL Server, Redshift, Postgres, Mysql, Db2 and Alloy DB. Struct and array data types are not currently supported.
 In addition, please note that SHA256 is not a supported function on Teradata systems. 
 If you wish to perform this comparison on Teradata you will need to 
 [deploy a UDF to perform the conversion](https://github.com/akuroda/teradata-udf-sha2/blob/master/src/sha256.c).)
 
 Below is the command syntax for row validations. In order to run row level
 validations you need to pass a `--primary-key` flag which defines what field(s)
 the validation will be compared on, as well as either the `--comparison-fields` flag
@@ -177,15 +177,15 @@
   --concat COLUMNS      Comma separated list of columns to concatenate or * for all columns (use if a common hash function is not available between databases)
   [--bq-result-handler or -bqrh PROJECT_ID.DATASET.TABLE]
                         BigQuery destination for validation results. Defaults to stdout.
                         See: *Validation Reports* section
   [--service-account or -sa PATH_TO_SA_KEY]
                         Service account to use for BigQuery result handler output.
   [--filters SOURCE_FILTER:TARGET_FILTER]
-                        Colon spearated string values of source and target filters.
+                        Colon separated string values of source and target filters.
                         If target filter is not provided, the source filter will run on source and target tables.
                         See: *Filters* section
   [--config-file or -c CONFIG_FILE]
                         YAML Config File Path to be used for storing validations.
   [--labels or -l KEY1=VALUE1,KEY2=VALUE2]
                         Comma-separated key value pair labels for the run.
   [--format or -fmt]    Format for stdout output. Supported formats are (text, csv, json, table).
@@ -233,15 +233,15 @@
                         Local: Provide a relative path of the target directory. Eg: `partitions_dir`
   --partition-num [1-1000], -pn [1-1000]
                         Number of partitions/config files to generate
                         In case this value exceeds the row count of the source/target table, it will be decreased to max(source_row_count, target_row_count)
   [--partition-key PARTITION_KEY, -partkey PARTITION_KEY]
                         Column on which the partitions would be generated. Column type must be integer. Defaults to Primary key
   [--filters SOURCE_FILTER:TARGET_FILTER]
-                        Colon spearated string values of source and target filters.
+                        Colon separated string values of source and target filters.
                         If target filter is not provided, the source filter will run on source and target tables.
                         See: *Filters* section
 ```
 #### Schema Validations
 
 Below is the syntax for schema validations. These can be used to compare case insensitive column names and
 types between source and target.
@@ -321,15 +321,15 @@
 
 The [Examples](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/examples.md)
 page provides few examples of how this tool can be used to run custom query validations.
 
 
 #### Custom Query Row Validations 
 
-(Note: Custom query row validation is currently only supported for BigQuery, Teradata, SQL Server, PostgreSQL, Oracle, AlloyDB, and Impala/Hive. Struct and array data types are not currently supported.)
+(Note: Custom query row validation is currently only supported for BigQuery, Teradata, SQL Server, PostgreSQL, Oracle, Redshift, DB2, AlloyDB, and Impala/Hive. Struct and array data types are not currently supported.)
 
 Below is the command syntax for row validations. In order to run row level
 validations you need to pass `--hash` flag which will specify the fields
 of the custom query result that will be concatenated and hashed. The primary key should be included
 in the SELECT statement of both source_query.sql and target_query.sql
 
 Below is the command syntax for custom query row validations.
@@ -372,14 +372,39 @@
   [--filter-status or -fs STATUSES_LIST]
                         Comma separated list of statuses to filter the validation results. Supported statuses are (success, fail). If no list is provided, all statuses are returned.
 ```
 
 The [Examples](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/examples.md)
 page provides few examples of how this tool can be used to run custom query row validations.
 
+#### Dry Run Validation
+
+The `validate` command takes a `--dry-run` command line flag that prints source
+and target SQL to stdout as JSON in lieu of performing a validation:
+
+```
+data-validation (--verbose or -v) (--log-level or -ll) validate
+  [--dry-run or -dr]    Prints source and target SQL to stdout in lieu of performing a validation.
+```
+
+For example, this flag can be used as follows:
+
+```shell
+> data-validation validate --dry-run row \
+  -sc my_bq_conn \
+  -tc my_bq_conn \
+  -tbls bigquery-public-data.new_york_citibike.citibike_stations \
+  --primary-keys station_id \
+  --hash '*'
+{
+    "source_query": "SELECT `hash__all`, `station_id`\nFROM ...",
+    "target_query": "SELECT `hash__all`, `station_id`\nFROM ..."
+}
+```
+
 ### YAML Configuration Files
 
 You can customize the configuration for any given validation by providing use
 case specific CLI arguments or editing the YAML configuration file.
 
 For example, the following command creates a YAML file for the validation of the
 `new_york_citibike` table: `data-validation validate column -sc my_bq_conn -tc
@@ -444,23 +469,23 @@
           The raw query to run against the supplied connection
 ```
 
 ### Building Matched Table Lists
 
 Creating the list of matched tables can be a hassle. We have added a feature
 which may help you to match all of the tables together between source and
-target. The find-tables tool:
+target. The `find-tables` command:
 
--   Pulls all tables in the source (applying a supplied allowed-schemas filter)
+-   Pulls all tables in the source (applying a supplied `allowed-schemas` filter)
 -   Pulls all tables from the target
--   Uses Levenshtein distance to match tables
+-   Uses Jaro Similarity algorithm to match tables
 -   Finally, it prints a JSON list of tables which can be a reference for the
     validation run config.
 
-Note that our score cutoff default is 1. If no matches occur, reduce this value as deemed necessary.
+Note that our default value for the `score-cutoff` parameter is 1 and it seeks for identical matches. If no matches occur, reduce this value as deemed necessary. By using smaller numbers such as 0.7, 0.65 etc you can get more matches. For reference, we make use of [this jaro_similarity method](https://jamesturk.github.io/jellyfish/functions/#jaro-similarity) for the string comparison.
 
 ```
 data-validation find-tables --source-conn source --target-conn target \
     --allowed-schemas pso_data_validator \
     --score-cutoff 1
 ```
```

### Comparing `google-pso-data-validator-3.1.0/data_validation/__init__.py` & `google-pso-data-validator-3.2.0/data_validation/__init__.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/data_validation/__main__.py` & `google-pso-data-validator-3.2.0/data_validation/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -415,28 +415,40 @@
     for config_manager in config_managers:
         yaml_config[consts.YAML_VALIDATIONS].append(
             config_manager.get_yaml_validation_block()
         )
     return yaml_config
 
 
-def run_validation(config_manager, verbose=False):
+def run_validation(config_manager, dry_run=False, verbose=False):
     """Run a single validation.
 
     Args:
         config_manager (ConfigManager): Validation config manager instance.
+        dry_run (bool): Print source and target SQL to stdout in lieu of validation.
         verbose (bool): Validation setting to log queries run.
     """
     validator = DataValidation(
         config_manager.config,
         validation_builder=None,
         result_handler=None,
         verbose=verbose,
     )
-    validator.execute()
+    if dry_run:
+        print(
+            json.dumps(
+                {
+                    "source_query": validator.validation_builder.get_source_query().compile(),
+                    "target_query": validator.validation_builder.get_target_query().compile(),
+                },
+                indent=4,
+            )
+        )
+    else:
+        validator.execute()
 
 
 def run_validations(args, config_managers):
     """Run and manage a series of validations.
 
     Args:
         config_managers (list[ConfigManager]): List of config manager instances.
@@ -445,23 +457,25 @@
     for config_manager in config_managers:
         if config_manager.config and consts.CONFIG_FILE in config_manager.config:
             logging.info(
                 "Currently running the validation for yml file: %s",
                 config_manager.config[consts.CONFIG_FILE],
             )
             try:
-                run_validation(config_manager, verbose=args.verbose)
+                run_validation(
+                    config_manager, dry_run=args.dry_run, verbose=args.verbose
+                )
             except Exception as e:
                 logging.error(
-                    "Error %s occured while running config file %s. Skipping it for now.",
+                    "Error %s occurred while running config file %s. Skipping it for now.",
                     str(e),
                     config_manager.config[consts.CONFIG_FILE],
                 )
         else:
-            run_validation(config_manager, verbose=args.verbose)
+            run_validation(config_manager, dry_run=args.dry_run, verbose=args.verbose)
 
 
 def store_yaml_config_file(args, config_managers):
     """Build a YAML config file from the supplied configs.
 
     Args:
         config_managers (list[ConfigManager]): List of config manager instances.
```

### Comparing `google-pso-data-validator-3.1.0/data_validation/app.py` & `google-pso-data-validator-3.2.0/data_validation/app.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/data_validation/cli_tools.py` & `google-pso-data-validator-3.2.0/data_validation/cli_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,18 +45,18 @@
 
 import argparse
 import csv
 import json
 import logging
 import sys
 import uuid
-from typing import List, Dict
 from argparse import Namespace
+from typing import Dict, List
 
-from data_validation import consts, state_manager, clients
+from data_validation import clients, consts, state_manager
 
 CONNECTION_SOURCE_FIELDS = {
     "BigQuery": [
         ["project_id", "GCP Project to use for BigQuery"],
         ["google_service_account_key_path", "(Optional) GCP SA Key Path"],
     ],
     "Teradata": [
@@ -140,14 +140,16 @@
         ["user", "LDAP user to authenticate"],
         ["password", "LDAP password to authenticate"],
         [
             "pool_size",
             "Size of the connection pool. Typically this is not necessary to configure. (default is 8)",
         ],
         ["hdfs_client", "An existing HDFS client"],
+        ["use_http_transport", "Boolean if HTTP proxy is provided (default is False)"],
+        ["http_path", "URL path of HTTP proxy"],
     ],
     "DB2": [
         ["host", "Desired DB2 host"],
         ["port", "Desired DB2 port (50000 if not provided)"],
         ["user", "Username to connect to"],
         ["password", "Password for authentication of user"],
         ["database", "Database in DB2 to connect to"],
@@ -322,14 +324,20 @@
         dest="validation_config_cmd"
     )
     _ = configs_subparsers.add_parser("list", help="List your validation configs")
     run_parser = configs_subparsers.add_parser(
         "run", help="Run your validation configs"
     )
     run_parser.add_argument(
+        "--dry-run",
+        "-dr",
+        action="store_true",
+        help="Prints source and target SQL to stdout in lieu of performing a validation.",
+    )
+    run_parser.add_argument(
         "--config-file",
         "-c",
         help="YAML Config File Path to be used for building or running validations.",
     )
     run_parser.add_argument(
         "--config-dir",
         "-cdir",
@@ -395,14 +403,21 @@
 
 def _configure_validate_parser(subparsers):
     """Configure arguments to run validations."""
     validate_parser = subparsers.add_parser(
         "validate", help="Run a validation and optionally store to config"
     )
 
+    validate_parser.add_argument(
+        "--dry-run",
+        "-dr",
+        action="store_true",
+        help="Prints source and target SQL to stdout in lieu of performing a validation.",
+    )
+
     validate_subparsers = validate_parser.add_subparsers(dest="validate_cmd")
 
     column_parser = validate_subparsers.add_parser(
         "column", help="Run a column validation"
     )
     _configure_column_parser(column_parser)
```

### Comparing `google-pso-data-validator-3.1.0/data_validation/client_info.py` & `google-pso-data-validator-3.2.0/data_validation/client_info.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/data_validation/clients.py` & `google-pso-data-validator-3.2.0/data_validation/clients.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from ibis.backends.mysql.client import MySQLClient
 from ibis.backends.pandas.client import PandasClient
 from ibis.backends.postgres.client import PostgreSQLClient
 from third_party.ibis.ibis_cloud_spanner.api import connect as spanner_connect
 from third_party.ibis.ibis_impala.api import impala_connect
 from data_validation import client_info, consts, exceptions
 from data_validation.secret_manager import SecretManagerBuilder
+from third_party.ibis.ibis_redshift.client import RedShiftClient
 
 ibis.options.sql.default_limit = None
 
 # Our customized Ibis Datatype logic add support for new types
 third_party.ibis.ibis_addon.datatypes
 
 # TODO(googleapis/google-auth-library-python#520): Remove after issue is resolved
@@ -143,14 +144,15 @@
     database_name (str): Database name (generally default is used)
     """
     if type(client) in [
         OracleClient,
         PostgreSQLClient,
         DB2Client,
         MSSQLClient,
+        RedShiftClient,
     ]:
         return client.table(table_name, database=database_name, schema=schema_name)
     elif type(client) in [PandasClient]:
         return client.table(table_name, schema=schema_name)
     else:
         return client.table(table_name, database=schema_name)
 
@@ -164,27 +166,28 @@
     """Return Ibis Table Schema for Supplied Client.
 
     client (IbisClient): Client to use for table
     schema_name (str): Schema name of table object
     table_name (str): Table name of table object
     database_name (str): Database name (generally default is used)
     """
-    if type(client) in [MySQLClient, PostgreSQLClient]:
+    if type(client) in [MySQLClient, PostgreSQLClient, RedShiftClient]:
         return client.schema(schema_name).table(table_name).schema()
     else:
         return client.get_schema(table_name, schema_name)
 
 
 def list_schemas(client):
     """Return a list of schemas in the DB."""
     if type(client) in [
         OracleClient,
         PostgreSQLClient,
         DB2Client,
         MSSQLClient,
+        RedShiftClient,
     ]:
         return client.list_schemas()
     elif hasattr(client, "list_databases"):
         return client.list_databases()
     else:
         return [None]
 
@@ -192,14 +195,15 @@
 def list_tables(client, schema_name):
     """Return a list of tables in the DB schema."""
     if type(client) in [
         OracleClient,
         PostgreSQLClient,
         DB2Client,
         MSSQLClient,
+        RedShiftClient,
     ]:
         return client.list_tables(schema=schema_name)
     elif schema_name:
         return client.list_tables(database=schema_name)
     else:
         return client.list_tables()
 
@@ -295,14 +299,14 @@
 CLIENT_LOOKUP = {
     "BigQuery": get_bigquery_client,
     "Impala": impala_connect,
     "MySQL": MySQLClient,
     "Oracle": OracleClient,
     "FileSystem": get_pandas_client,
     "Postgres": PostgreSQLClient,
-    "Redshift": PostgreSQLClient,
+    "Redshift": RedShiftClient,
     "Teradata": TeradataClient,
     "MSSQL": MSSQLClient,
     "Snowflake": snowflake_connect,
     "Spanner": spanner_connect,
     "DB2": DB2Client,
 }
```

### Comparing `google-pso-data-validator-3.1.0/data_validation/combiner.py` & `google-pso-data-validator-3.2.0/data_validation/combiner.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/data_validation/config_manager.py` & `google-pso-data-validator-3.2.0/data_validation/config_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -600,14 +600,18 @@
 
             calc_func = "epoch_seconds"
 
         elif column_type == "int32":
             calc_func = "cast"
             cast_type = "int64"
 
+        elif column_type == "decimal":
+            calc_func = "cast"
+            cast_type = "float64"
+
         else:
             raise ValueError(f"Unsupported column type: {column_type}")
 
         calculated_config = self.build_and_append_pre_agg_calc_config(
             source_column, target_column, calc_func, column_position, cast_type, depth
         )
 
@@ -668,14 +672,15 @@
                     and agg_type
                     in (
                         "sum",
                         "avg",
                         "bit_xor",
                     )  # For timestamps: do not convert to epoch seconds for min/max
                 )
+                or (column_type == "decimal")
             ):
                 aggregate_config = self.append_pre_agg_calc_field(
                     casefold_source_columns[column],
                     casefold_target_columns[column],
                     agg_type,
                     column_type,
                     column_position,
```

### Comparing `google-pso-data-validator-3.1.0/data_validation/consts.py` & `google-pso-data-validator-3.2.0/data_validation/consts.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/data_validation/data_validation.py` & `google-pso-data-validator-3.2.0/data_validation/data_validation.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/data_validation/exceptions.py` & `google-pso-data-validator-3.2.0/data_validation/exceptions.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/data_validation/jellyfish_distance.py` & `google-pso-data-validator-3.2.0/data_validation/jellyfish_distance.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/data_validation/metadata.py` & `google-pso-data-validator-3.2.0/data_validation/metadata.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/data_validation/partition_builder.py` & `google-pso-data-validator-3.2.0/data_validation/partition_builder.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/data_validation/query_builder/__init__.py` & `google-pso-data-validator-3.2.0/data_validation/query_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/data_validation/query_builder/partition_row_builder.py` & `google-pso-data-validator-3.2.0/data_validation/query_builder/partition_row_builder.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/data_validation/query_builder/query_builder.py` & `google-pso-data-validator-3.2.0/data_validation/query_builder/query_builder.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/data_validation/query_builder/random_row_builder.py` & `google-pso-data-validator-3.2.0/data_validation/query_builder/random_row_builder.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/data_validation/result_handlers/bigquery.py` & `google-pso-data-validator-3.2.0/data_validation/result_handlers/bigquery.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/data_validation/result_handlers/text.py` & `google-pso-data-validator-3.2.0/data_validation/result_handlers/text.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/data_validation/schema_validation.py` & `google-pso-data-validator-3.2.0/data_validation/schema_validation.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/data_validation/secret_manager.py` & `google-pso-data-validator-3.2.0/data_validation/secret_manager.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/data_validation/state_manager.py` & `google-pso-data-validator-3.2.0/data_validation/state_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
         return json.loads(conn_str)
 
     def list_connections(self) -> List[str]:
         """Returns a list of the connection names that exist."""
         file_names = self._list_directory(self._get_connections_directory())
         return [
-            file_name.split(".")[0]
+            file_name.rsplit(".", 2)[0]
             for file_name in file_names
             if file_name.endswith(".connection.json")
         ]
 
     def _get_connections_directory(self) -> str:
         """Returns the connections directory path."""
         if self.file_system == FileSystem.LOCAL:
```

### Comparing `google-pso-data-validator-3.1.0/data_validation/validation_builder.py` & `google-pso-data-validator-3.2.0/data_validation/validation_builder.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/google_pso_data_validator.egg-info/PKG-INFO` & `google-pso-data-validator-3.2.0/google_pso_data_validator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-pso-data-validator
-Version: 3.1.0
+Version: 3.2.0
 Summary: A package to enable easy data validation
 Home-page: https://github.com/pypa/sampleproject
 Author: Dylan Hercher
 Author-email: dhercher@google.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -152,15 +152,15 @@
 The default aggregation type is a 'COUNT *'. If no aggregation flag (i.e count,
 sum , min, etc.) is provided, the default aggregation will run.
 
 The [Examples](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/examples.md) page provides many examples of how a tool can be used to run powerful validations without writing any queries.
 
 #### Row Validations
 
-(Note: Row hash validation is currently supported for BigQuery, Teradata, Impala/Hive, Oracle, SQL Server, Postgres, Mysql, Db2 and Alloy DB. Struct and array data types are not currently supported.
+(Note: Row hash validation is currently supported for BigQuery, Teradata, Impala/Hive, Oracle, SQL Server, Redshift, Postgres, Mysql, Db2 and Alloy DB. Struct and array data types are not currently supported.
 In addition, please note that SHA256 is not a supported function on Teradata systems. 
 If you wish to perform this comparison on Teradata you will need to 
 [deploy a UDF to perform the conversion](https://github.com/akuroda/teradata-udf-sha2/blob/master/src/sha256.c).)
 
 Below is the command syntax for row validations. In order to run row level
 validations you need to pass a `--primary-key` flag which defines what field(s)
 the validation will be compared on, as well as either the `--comparison-fields` flag
@@ -197,15 +197,15 @@
   --concat COLUMNS      Comma separated list of columns to concatenate or * for all columns (use if a common hash function is not available between databases)
   [--bq-result-handler or -bqrh PROJECT_ID.DATASET.TABLE]
                         BigQuery destination for validation results. Defaults to stdout.
                         See: *Validation Reports* section
   [--service-account or -sa PATH_TO_SA_KEY]
                         Service account to use for BigQuery result handler output.
   [--filters SOURCE_FILTER:TARGET_FILTER]
-                        Colon spearated string values of source and target filters.
+                        Colon separated string values of source and target filters.
                         If target filter is not provided, the source filter will run on source and target tables.
                         See: *Filters* section
   [--config-file or -c CONFIG_FILE]
                         YAML Config File Path to be used for storing validations.
   [--labels or -l KEY1=VALUE1,KEY2=VALUE2]
                         Comma-separated key value pair labels for the run.
   [--format or -fmt]    Format for stdout output. Supported formats are (text, csv, json, table).
@@ -253,15 +253,15 @@
                         Local: Provide a relative path of the target directory. Eg: `partitions_dir`
   --partition-num [1-1000], -pn [1-1000]
                         Number of partitions/config files to generate
                         In case this value exceeds the row count of the source/target table, it will be decreased to max(source_row_count, target_row_count)
   [--partition-key PARTITION_KEY, -partkey PARTITION_KEY]
                         Column on which the partitions would be generated. Column type must be integer. Defaults to Primary key
   [--filters SOURCE_FILTER:TARGET_FILTER]
-                        Colon spearated string values of source and target filters.
+                        Colon separated string values of source and target filters.
                         If target filter is not provided, the source filter will run on source and target tables.
                         See: *Filters* section
 ```
 #### Schema Validations
 
 Below is the syntax for schema validations. These can be used to compare case insensitive column names and
 types between source and target.
@@ -341,15 +341,15 @@
 
 The [Examples](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/examples.md)
 page provides few examples of how this tool can be used to run custom query validations.
 
 
 #### Custom Query Row Validations 
 
-(Note: Custom query row validation is currently only supported for BigQuery, Teradata, SQL Server, PostgreSQL, Oracle, AlloyDB, and Impala/Hive. Struct and array data types are not currently supported.)
+(Note: Custom query row validation is currently only supported for BigQuery, Teradata, SQL Server, PostgreSQL, Oracle, Redshift, DB2, AlloyDB, and Impala/Hive. Struct and array data types are not currently supported.)
 
 Below is the command syntax for row validations. In order to run row level
 validations you need to pass `--hash` flag which will specify the fields
 of the custom query result that will be concatenated and hashed. The primary key should be included
 in the SELECT statement of both source_query.sql and target_query.sql
 
 Below is the command syntax for custom query row validations.
@@ -392,14 +392,39 @@
   [--filter-status or -fs STATUSES_LIST]
                         Comma separated list of statuses to filter the validation results. Supported statuses are (success, fail). If no list is provided, all statuses are returned.
 ```
 
 The [Examples](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/examples.md)
 page provides few examples of how this tool can be used to run custom query row validations.
 
+#### Dry Run Validation
+
+The `validate` command takes a `--dry-run` command line flag that prints source
+and target SQL to stdout as JSON in lieu of performing a validation:
+
+```
+data-validation (--verbose or -v) (--log-level or -ll) validate
+  [--dry-run or -dr]    Prints source and target SQL to stdout in lieu of performing a validation.
+```
+
+For example, this flag can be used as follows:
+
+```shell
+> data-validation validate --dry-run row \
+  -sc my_bq_conn \
+  -tc my_bq_conn \
+  -tbls bigquery-public-data.new_york_citibike.citibike_stations \
+  --primary-keys station_id \
+  --hash '*'
+{
+    "source_query": "SELECT `hash__all`, `station_id`\nFROM ...",
+    "target_query": "SELECT `hash__all`, `station_id`\nFROM ..."
+}
+```
+
 ### YAML Configuration Files
 
 You can customize the configuration for any given validation by providing use
 case specific CLI arguments or editing the YAML configuration file.
 
 For example, the following command creates a YAML file for the validation of the
 `new_york_citibike` table: `data-validation validate column -sc my_bq_conn -tc
@@ -464,23 +489,23 @@
           The raw query to run against the supplied connection
 ```
 
 ### Building Matched Table Lists
 
 Creating the list of matched tables can be a hassle. We have added a feature
 which may help you to match all of the tables together between source and
-target. The find-tables tool:
+target. The `find-tables` command:
 
--   Pulls all tables in the source (applying a supplied allowed-schemas filter)
+-   Pulls all tables in the source (applying a supplied `allowed-schemas` filter)
 -   Pulls all tables from the target
--   Uses Levenshtein distance to match tables
+-   Uses Jaro Similarity algorithm to match tables
 -   Finally, it prints a JSON list of tables which can be a reference for the
     validation run config.
 
-Note that our score cutoff default is 1. If no matches occur, reduce this value as deemed necessary.
+Note that our default value for the `score-cutoff` parameter is 1 and it seeks for identical matches. If no matches occur, reduce this value as deemed necessary. By using smaller numbers such as 0.7, 0.65 etc you can get more matches. For reference, we make use of [this jaro_similarity method](https://jamesturk.github.io/jellyfish/functions/#jaro-similarity) for the string comparison.
 
 ```
 data-validation find-tables --source-conn source --target-conn target \
     --allowed-schemas pso_data_validator \
     --score-cutoff 1
 ```
```

### Comparing `google-pso-data-validator-3.1.0/google_pso_data_validator.egg-info/SOURCES.txt` & `google-pso-data-validator-3.2.0/google_pso_data_validator.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -76,12 +76,15 @@
 third_party/ibis/ibis_oracle/expr/__init__.py
 third_party/ibis/ibis_oracle/expr/datatypes.py
 third_party/ibis/ibis_oracle/expr/types.py
 third_party/ibis/ibis_oracle/udf/__init__.py
 third_party/ibis/ibis_oracle/udf/api.py
 third_party/ibis/ibis_postgres/__init__.py
 third_party/ibis/ibis_postgres/client.py
+third_party/ibis/ibis_redshift/__init__.py
+third_party/ibis/ibis_redshift/client.py
+third_party/ibis/ibis_redshift/compiler.py
 third_party/ibis/ibis_teradata/__init__.py
 third_party/ibis/ibis_teradata/api.py
 third_party/ibis/ibis_teradata/client.py
 third_party/ibis/ibis_teradata/compiler.py
 third_party/ibis/ibis_teradata/datatypes.py
```

### Comparing `google-pso-data-validator-3.1.0/google_pso_data_validator.egg-info/requires.txt` & `google-pso-data-validator-3.2.0/google_pso_data_validator.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/setup.py` & `google-pso-data-validator-3.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 import os
 
 import setuptools
 
 name = "google-pso-data-validator"
 description = "A package to enable easy data validation"
-version = "3.1.0"
+version = "3.2.0"
 release_status = "Development Status :: 3 - Alpha"
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 dependencies = [
     # Dependency corrections from our requirements
```

### Comparing `google-pso-data-validator-3.1.0/third_party/ibis/ibis_DB2/alchemy.py` & `google-pso-data-validator-3.2.0/third_party/ibis/ibis_DB2/alchemy.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/third_party/ibis/ibis_DB2/api.py` & `google-pso-data-validator-3.2.0/third_party/ibis/ibis_DB2/api.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/third_party/ibis/ibis_DB2/client.py` & `google-pso-data-validator-3.2.0/third_party/ibis/ibis_DB2/client.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/third_party/ibis/ibis_DB2/compiler.py` & `google-pso-data-validator-3.2.0/third_party/ibis/ibis_DB2/compiler.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/third_party/ibis/ibis_DB2/expr/datatypes.py` & `google-pso-data-validator-3.2.0/third_party/ibis/ibis_DB2/expr/datatypes.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/third_party/ibis/ibis_DB2/expr/types.py` & `google-pso-data-validator-3.2.0/third_party/ibis/ibis_DB2/expr/types.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/third_party/ibis/ibis_addon/api.py` & `google-pso-data-validator-3.2.0/third_party/ibis/ibis_addon/api.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/third_party/ibis/ibis_addon/base_sqlalchemy/alchemy.py` & `google-pso-data-validator-3.2.0/third_party/ibis/ibis_addon/base_sqlalchemy/alchemy.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/third_party/ibis/ibis_addon/datatypes.py` & `google-pso-data-validator-3.2.0/third_party/ibis/ibis_addon/datatypes.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/third_party/ibis/ibis_addon/operations.py` & `google-pso-data-validator-3.2.0/third_party/ibis/ibis_addon/operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 from ibis.backends.base_sqlalchemy.compiler import ExprTranslator
 from ibis.backends.base_sql.compiler import BaseExprTranslator
 from third_party.ibis.ibis_oracle.compiler import OracleExprTranslator
 from third_party.ibis.ibis_teradata.compiler import TeradataExprTranslator
 from third_party.ibis.ibis_mssql.compiler import MSSQLExprTranslator
 from ibis.backends.postgres.compiler import PostgreSQLExprTranslator
 from ibis.backends.mysql.compiler import MySQLExprTranslator
+from third_party.ibis.ibis_redshift.compiler import RedShiftExprTranslator
 
 # avoid errors if Db2 is not installed and not needed
 try:
     from third_party.ibis.ibis_DB2.compiler import DB2ExprTranslator
 except Exception:
     DB2ExprTranslator = None
 
@@ -152,14 +153,23 @@
             arg_formatted,
             arg_type.timezone if arg_type.timezone is not None else "UTC",
         )
     return "FORMAT_{}({}, {})".format(
         strftime_format_func_name, fmt_string, arg_formatted
     )
 
+def strftime_mysql(translator, expr):
+    arg, format_string = expr.op().args 
+    arg_formatted = translator.translate(arg)
+    arg_type = arg.type()
+    fmt_string = translator.translate(format_string)
+    if isinstance(arg_type, dt.Timestamp):
+        fmt_string = "%Y-%m-%d %H:%i:%S"
+    return sa.func.date_format(arg_formatted, fmt_string)
+
 
 def format_hashbytes_teradata(translator, expr):
     arg, how = expr.op().args
     compiled_arg = translator.translate(arg)
     if how == "sha256":
         return f"rtrim(hash_sha256({compiled_arg}))"
     elif how == "sha512":
@@ -232,14 +242,19 @@
 def sa_format_hashbytes_db2(translator, expr):
     arg, how = expr.op().args
     compiled_arg = translator.translate(arg)
     hashfunc = sa.func.hash(compiled_arg,sa.sql.literal_column("2"))
     hex = sa.func.hex(hashfunc)
     return sa.func.lower(hex)
 
+def sa_format_hashbytes_redshift(translator, expr):
+    arg, how  = expr.op().args
+    compiled_arg = translator.translate(arg)
+    return sa.sql.literal_column(f"sha2({compiled_arg}, 256)")
+
 def sa_format_hashbytes_postgres(translator, expr):
     arg, how = expr.op().args
     compiled_arg = translator.translate(arg)
     convert = sa.func.convert_to(compiled_arg, sa.sql.literal_column("'UTF8'"))
     hash_func = sa.func.sha256(convert)
     return sa.func.encode(hash_func, sa.sql.literal_column("'hex'"))
 
@@ -298,14 +313,15 @@
 NumericValue.to_char = compile_to_char
 TemporalValue.to_char = compile_to_char
 BigQueryExprTranslator._registry[BitXor] = bq_reduction("BIT_XOR")
 BigQueryExprTranslator._registry[Hash] = format_hash_bigquery
 BigQueryExprTranslator._registry[HashBytes] = format_hashbytes_bigquery
 BigQueryExprTranslator._registry[RawSQL] = format_raw_sql
 BigQueryExprTranslator._registry[Strftime] = strftime_bigquery
+MySQLExprTranslator._registry[Strftime] = strftime_mysql
 AlchemyExprTranslator._registry[RawSQL] = format_raw_sql
 AlchemyExprTranslator._registry[HashBytes] = format_hashbytes_alchemy
 MSSQLExprTranslator._registry[HashBytes] = sa_format_hashbytes_mssql
 MSSQLExprTranslator._registry[RawSQL] = sa_format_raw_sql
 BaseExprTranslator._registry[RawSQL] = format_raw_sql
 BaseExprTranslator._registry[HashBytes] = format_hashbytes_base
 ImpalaExprTranslator._registry[RawSQL] = format_raw_sql
@@ -319,10 +335,11 @@
 PostgreSQLExprTranslator._registry[RawSQL] = sa_format_raw_sql
 PostgreSQLExprTranslator._registry[ToChar] = sa_format_to_char
 PostgreSQLExprTranslator._registry[Cast] = sa_cast_postgres
 MySQLExprTranslator._registry[RawSQL] = sa_format_raw_sql
 MySQLExprTranslator._registry[HashBytes] = sa_format_hashbytes_mysql
 MySQLExprTranslator._registry[ops.IfNull] = fixed_arity(sa.func.ifnull, 2)
 MySQLExprTranslator._registry[ops.StringJoin] = sa_format_to_stringjoin
+RedShiftExprTranslator._registry[HashBytes] = sa_format_hashbytes_redshift
 
 if DB2ExprTranslator: #check if Db2 driver is loaded
     DB2ExprTranslator._registry[HashBytes] = sa_format_hashbytes_db2
```

### Comparing `google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/api.py` & `google-pso-data-validator-3.2.0/third_party/ibis/ibis_cloud_spanner/api.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/client.py` & `google-pso-data-validator-3.2.0/third_party/ibis/ibis_cloud_spanner/client.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/compiler.py` & `google-pso-data-validator-3.2.0/third_party/ibis/ibis_cloud_spanner/compiler.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/datatypes.py` & `google-pso-data-validator-3.2.0/third_party/ibis/ibis_cloud_spanner/datatypes.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/table.py` & `google-pso-data-validator-3.2.0/third_party/ibis/ibis_cloud_spanner/table.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/tests/conftest.py` & `google-pso-data-validator-3.2.0/third_party/ibis/ibis_cloud_spanner/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/tests/test_client.py` & `google-pso-data-validator-3.2.0/third_party/ibis/ibis_cloud_spanner/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/tests/test_compiler.py` & `google-pso-data-validator-3.2.0/third_party/ibis/ibis_cloud_spanner/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/tests/test_datatypes.py` & `google-pso-data-validator-3.2.0/third_party/ibis/ibis_cloud_spanner/tests/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/to_pandas.py` & `google-pso-data-validator-3.2.0/third_party/ibis/ibis_cloud_spanner/to_pandas.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/third_party/ibis/ibis_impala/api.py` & `google-pso-data-validator-3.2.0/third_party/ibis/ibis_impala/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,21 +11,30 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from ibis.backends.base_sql import fixed_arity
 from ibis.backends.impala import connect, udf
 from ibis.backends.impala.compiler import rewrites
-from ibis.backends.impala.client import ImpalaClient, ImpalaQuery, _HS2_TTypeId_to_dtype
 import ibis.expr.datatypes as dt
 import ibis.expr.operations as ops
 import ibis.expr.schema as sch
 import numpy as np
 import pandas as pd
 
+from ibis.config import options
+from ibis.backends.impala.client import (  
+    ImpalaClient,
+    ImpalaConnection,
+    ImpalaDatabase,
+    ImpalaTable,
+    ImpalaQuery,
+    _HS2_TTypeId_to_dtype
+)
+
 _impala_to_ibis_type = udf._impala_to_ibis_type
 
 _impala_to_ibis_type["date"] = "date"
 _HS2_TTypeId_to_dtype["DATE"] = "datetime64[ns]"
 
 def impala_connect(
     host=None,
@@ -35,40 +44,42 @@
     kerberos_service_name="impala",
     use_ssl=False,
     timeout=45,
     ca_cert=None,
     user=None,
     password=None,
     pool_size=8,
-    hdfs_client=None
+    hdfs_client=None,
+    use_http_transport=False,
+    http_path="",
 ):
-    auth_mechanism = (auth_mechanism, "PLAIN")[auth_mechanism is None]
-    database = (database, "default")[database is None]
-    port = (port, 10000)[port is None]
-    kerberos_service_name = (kerberos_service_name, "impala")[
-        kerberos_service_name is None
-    ]
-    use_ssl = (use_ssl, False)[use_ssl is None]
-    timeout = (timeout, 45)[timeout is None]
-    pool_size = (pool_size, 8)[pool_size is None]
-    
-    return connect(
-        host=host,
-        port=int(port),
-        database=database,
-        auth_mechanism=auth_mechanism,
-        kerberos_service_name=kerberos_service_name,
-        use_ssl=use_ssl,
-        timeout=timeout,
-        ca_cert=ca_cert,
-        user=user,
-        password=password,
-        pool_size=pool_size,
-        hdfs_client=hdfs_client
-    )
+    params = {
+        'host': host,
+        'port': port,
+        'database': database,
+        'timeout': timeout,
+        'use_ssl': use_ssl,
+        'ca_cert': ca_cert,
+        'user': user,
+        'password': password,
+        'auth_mechanism': auth_mechanism,
+        'kerberos_service_name': kerberos_service_name,
+        'use_http_transport': use_http_transport,
+        'http_path': http_path,
+    }
+    con = ImpalaConnection(pool_size=pool_size, **params)
+    try:
+        client = ImpalaClient(con, hdfs_client=hdfs_client)
+    except Exception:
+        con.close()
+        raise
+    else:
+        if options.default_backend is None:
+            options.default_backend = client
+    return client
 
 
 def parse_type(t):
     """Returns the Ibis datatype from source type."""
     t = t.lower()
     if t in _impala_to_ibis_type:
         return _impala_to_ibis_type[t]
```

### Comparing `google-pso-data-validator-3.1.0/third_party/ibis/ibis_mssql/api.py` & `google-pso-data-validator-3.2.0/third_party/ibis/ibis_mssql/api.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/third_party/ibis/ibis_mssql/client.py` & `google-pso-data-validator-3.2.0/third_party/ibis/ibis_mssql/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -46,14 +46,49 @@
 
 
 @dt.dtype.register(MSDialect_pyodbc, sa.dialects.mssql.FLOAT)
 def sa_float64(_, satype, nullable=True):
     return dt.Float64(nullable=nullable)
 
 
+@dt.dtype.register(MSDialect_pyodbc, sa.dialects.mssql.MONEY)
+def sa_money(_, satype, nullable=True):
+    return dt.Int64(nullable=nullable)
+
+
+@dt.dtype.register(MSDialect_pyodbc, sa.dialects.mssql.BINARY)
+def sa_binary(_, satype, nullable=True):
+    return dt.Binary(nullable=nullable)
+
+
+@dt.dtype.register(MSDialect_pyodbc, sa.dialects.mssql.VARBINARY)
+def sa_varbinary(_, satype, nullable=True):
+    return dt.Binary(nullable=nullable)
+
+
+@dt.dtype.register(MSDialect_pyodbc, sa.dialects.mssql.IMAGE)
+def sa_image(_, satype, nullable=True):
+    return dt.Binary(nullable=nullable)
+
+
+@dt.dtype.register(MSDialect_pyodbc, sa.dialects.mssql.NCHAR)
+def sa_nchar(_, satype, nullable=True):
+    return dt.String(nullable=nullable)
+
+
+@dt.dtype.register(MSDialect_pyodbc, sa.dialects.mssql.NTEXT)
+def sa_ntext(_, satype, nullable=True):
+    return dt.String(nullable=nullable)
+
+
+@dt.dtype.register(MSDialect_pyodbc, sa.dialects.mssql.NVARCHAR)
+def sa_nvarchar(_, satype, nullable=True):
+    return dt.String(nullable=nullable)
+
+
 class MSSQLTable(alch.AlchemyTable):
     pass
 
 
 class MSSQLSchema(alch.AlchemyDatabaseSchema):
     pass
```

### Comparing `google-pso-data-validator-3.1.0/third_party/ibis/ibis_mssql/compiler.py` & `google-pso-data-validator-3.2.0/third_party/ibis/ibis_mssql/compiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -367,18 +367,20 @@
     )
 
 
 def _day_of_week_name(t, expr):
     (sa_arg,) = map(t.translate, expr.op().args)
     return sa.func.trim(sa.func.format(sa_arg, 'dddd'))
 
+
 def _string_join(t, expr):
     sep, elements = expr.op().args
     return sa.func.concat(*map(t.translate, elements))
 
+
 _operation_registry = alch._operation_registry.copy()
 
 _operation_registry.update(
     {
         # aggregate methods
         ops.Count: _reduction_count(sa.func.count),
         ops.Max: _reduction('max'),
@@ -414,19 +416,27 @@
         ops.Sqrt: unary(sa.func.sqrt),
         ops.Tan: unary(sa.func.tan),
         # timestamp methods
         ops.TimestampNow: fixed_arity(sa.func.GETDATE, 0),
         ops.ExtractYear: _extract('year'),
         ops.ExtractMonth: _extract('month'),
         ops.ExtractDay: _extract('day'),
+        ops.ExtractDayOfYear: _extract('dayofyear'),
         ops.ExtractHour: _extract('hour'),
         ops.ExtractMinute: _extract('minute'),
         ops.ExtractSecond: _extract('second'),
         ops.ExtractMillisecond: _extract('millisecond'),
+        ops.ExtractWeekOfYear: _extract('iso_week'),
         ops.Strftime: _strftime,
+        ops.ExtractEpochSeconds: fixed_arity(
+            lambda x: sa.cast(
+                sa.func.datediff(sa.text('s'), '1970-01-01 00:00:00', x), sa.BIGINT
+            ),
+            1,
+        ),
         # newly added
         ops.Lag: _lag,
         ops.Lead: _lead,
         ops.NTile: _ntile,
         ops.FirstValue: unary(sa.func.first_value),
         ops.LastValue: unary(sa.func.last_value),
         ops.RowNumber: fixed_arity(lambda: sa.func.row_number(), 0),
@@ -485,14 +495,15 @@
 _operation_registry.update(_unsupported_ops)
 
 
 class MSSQLExprTranslator(alch.AlchemyExprTranslator):
     _registry = _operation_registry
     _rewrites = alch.AlchemyExprTranslator._rewrites.copy()
     _type_map = alch.AlchemyExprTranslator._type_map.copy()
+    # only used to map SQLAlchemy types back to SQL Server types, it does not add support to new data types, for that go to client.py
     _type_map.update(
         {
             dt.Boolean: mssql.BIT,
             dt.Int8: mssql.TINYINT,
             dt.Int32: mssql.INTEGER,
             dt.Int64: mssql.BIGINT,
             dt.Float: mssql.REAL,
@@ -504,11 +515,11 @@
 
 rewrites = MSSQLExprTranslator.rewrites
 compiles = MSSQLExprTranslator.compiles
 
 
 class MSSQLDialect(alch.AlchemyDialect):
 
-    translator = MSSQLExprTranslator
+      translator = MSSQLExprTranslator
 
 
 dialect = MSSQLDialect
```

### Comparing `google-pso-data-validator-3.1.0/third_party/ibis/ibis_mssql/expr/api.py` & `google-pso-data-validator-3.2.0/third_party/ibis/ibis_mssql/expr/api.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/third_party/ibis/ibis_mssql/expr/operations.py` & `google-pso-data-validator-3.2.0/third_party/ibis/ibis_mssql/expr/operations.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/third_party/ibis/ibis_oracle/alchemy.py` & `google-pso-data-validator-3.2.0/third_party/ibis/ibis_oracle/alchemy.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/third_party/ibis/ibis_oracle/api.py` & `google-pso-data-validator-3.2.0/third_party/ibis/ibis_oracle/api.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/third_party/ibis/ibis_oracle/client.py` & `google-pso-data-validator-3.2.0/third_party/ibis/ibis_oracle/client.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/third_party/ibis/ibis_oracle/compiler.py` & `google-pso-data-validator-3.2.0/third_party/ibis/ibis_oracle/compiler.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/third_party/ibis/ibis_oracle/expr/datatypes.py` & `google-pso-data-validator-3.2.0/third_party/ibis/ibis_oracle/expr/datatypes.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/third_party/ibis/ibis_oracle/expr/types.py` & `google-pso-data-validator-3.2.0/third_party/ibis/ibis_oracle/expr/types.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/third_party/ibis/ibis_oracle/udf/api.py` & `google-pso-data-validator-3.2.0/third_party/ibis/ibis_oracle/udf/api.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/third_party/ibis/ibis_postgres/client.py` & `google-pso-data-validator-3.2.0/third_party/ibis/ibis_postgres/client.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/third_party/ibis/ibis_teradata/api.py` & `google-pso-data-validator-3.2.0/third_party/ibis/ibis_teradata/api.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/third_party/ibis/ibis_teradata/client.py` & `google-pso-data-validator-3.2.0/third_party/ibis/ibis_teradata/client.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/third_party/ibis/ibis_teradata/compiler.py` & `google-pso-data-validator-3.2.0/third_party/ibis/ibis_teradata/compiler.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.1.0/third_party/ibis/ibis_teradata/datatypes.py` & `google-pso-data-validator-3.2.0/third_party/ibis/ibis_teradata/datatypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,49 +51,55 @@
 
     @classmethod
     def to_ibis_from_N(cls, col_data, return_ibis_type=True):
         return cls.to_ibis_from_D(col_data, return_ibis_type=return_ibis_type)
 
     @classmethod
     def to_ibis_from_D(cls, col_data, return_ibis_type=True):
-        precision = int(col_data.get("DecimalTotalDigits", col_data.get("Decimal Total Digits", 20)))
-        scale = int(col_data.get("DecimalFractionalDigits", col_data.get("Decimal Fractional Digits", 4)))
+        precision = int(
+            col_data.get("DecimalTotalDigits", col_data.get("Decimal Total Digits", 20))
+        )
+        scale = int(
+            col_data.get(
+                "DecimalFractionalDigits", col_data.get("Decimal Fractional Digits", 4)
+            )
+        )
         if return_ibis_type:
-            return dt.float64
+            return dt.Decimal(precision, scale)
         value_type = "DECIMAL(%d, %d)" % (precision, scale)
         return value_type
 
     @classmethod
     def to_ibis_from_F(cls, col_data, return_ibis_type=True):
         if return_ibis_type:
             return dt.float64
         return "FLOAT"
 
     @classmethod
     def to_ibis_from_I(cls, col_data, return_ibis_type=True):
         if return_ibis_type:
-            return dt.int64
+            return dt.int32
         return "INT"
 
     @classmethod
     def to_ibis_from_I1(cls, col_data, return_ibis_type=True):
         if return_ibis_type:
             return dt.int8
         return "INT"
 
     @classmethod
     def to_ibis_from_I2(cls, col_data, return_ibis_type=True):
         if return_ibis_type:
-            return dt.int8
+            return dt.int16
         return "INT"
 
     @classmethod
     def to_ibis_from_I8(cls, col_data, return_ibis_type=True):
         if return_ibis_type:
-            return dt.int16
+            return dt.int64
         return "INT"
 
     @classmethod
     def to_ibis_from_DA(cls, col_data, return_ibis_type=True):
         if return_ibis_type:
             return dt.date
 
@@ -112,14 +118,15 @@
             return dt.timestamp
 
         return "TIMESTAMP"
 
 
 ibis_type_to_teradata_type = Dispatcher("ibis_type_to_teradata_type")
 
+
 @ibis_type_to_teradata_type.register(dt.DataType)
 def trans_default(t):
     return ibis_type_to_teradata_type(t, TypeTranslationContext())
 
 
 @ibis_type_to_teradata_type.register(str, TypeTranslationContext)
 def trans_string_context(datatype, context):
@@ -129,15 +136,15 @@
 @ibis_type_to_teradata_type.register(dt.String, TypeTranslationContext)
 def trans_string(t, context):
     return "VARCHAR(255)"
 
 
 @ibis_type_to_teradata_type.register(dt.Floating, TypeTranslationContext)
 def trans_float64(t, context):
-    return "FLOAT64"
+    return "FLOAT"
 
 
 @ibis_type_to_teradata_type.register(dt.Integer, TypeTranslationContext)
 def trans_integer(t, context):
     return "INT64"
```

