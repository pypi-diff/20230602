# Comparing `tmp/easy_sql_easy_sql-1.0.0.tar.gz` & `tmp/easy_sql_easy_sql-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_sql_easy_sql-1.0.0.tar", max compression
+gzip compressed data, was "easy_sql_easy_sql-1.1.0.tar", max compression
```

## Comparing `easy_sql_easy_sql-1.0.0.tar` & `easy_sql_easy_sql-1.1.0.tar`

### file list

```diff
@@ -1,82 +1,81 @@
--rw-r--r--   0        0        0    11357 2023-05-08 01:51:58.192164 easy_sql_easy_sql-1.0.0/LICENSE
--rw-r--r--   0        0        0     9499 2023-05-08 01:51:58.192164 easy_sql_easy_sql-1.0.0/README.md
--rw-r--r--   0        0        0        0 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/__init__.py
--rw-r--r--   0        0        0     2886 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/base_test.py
--rw-r--r--   0        0        0        0 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/cli/__init__.py
--rw-r--r--   0        0        0     8595 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/cli/backend_processor.py
--rw-r--r--   0        0        0    14198 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/config/sql_config.py
--rw-r--r--   0        0        0     4296 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/config/sql_config_test.py
--rw-r--r--   0        0        0     2165 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/data_process.py
--rw-r--r--   0        0        0     1040 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/data_process_itest.py
--rw-r--r--   0        0        0     2779 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/data_process_test.py
--rw-r--r--   0        0        0     2531 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/local_spark.py
--rw-r--r--   0        0        0     1360 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/logger.py
--rw-r--r--   0        0        0     3048 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/report.py
--rw-r--r--   0        0        0      337 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/report_test.py
--rw-r--r--   0        0        0     3054 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/spark_optimizer.py
--rw-r--r--   0        0        0        0 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_linter/__init__.py
--rw-r--r--   0        0        0      106 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_linter/rules/__init__.py
--rw-r--r--   0        0        0     1430 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_linter/rules/bq_schema_rule.py
--rw-r--r--   0        0        0    10316 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_linter/sql_linter.py
--rw-r--r--   0        0        0     4323 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_linter/sql_linter_cli.py
--rw-r--r--   0        0        0     2605 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_linter/sql_linter_reportor.py
--rw-r--r--   0        0        0     6979 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_linter/sql_linter_test.py
--rw-r--r--   0        0        0      620 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/__init__.py
--rw-r--r--   0        0        0       62 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/__init__.py
--rw-r--r--   0        0        0     7036 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/base.py
--rw-r--r--   0        0        0      192 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/bigquery.py
--rw-r--r--   0        0        0      168 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/clickhouse.py
--rw-r--r--   0        0        0    15746 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/flink.py
--rw-r--r--   0        0        0    16114 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/flink_itest.py
--rw-r--r--   0        0        0     1498 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/flink_test.py
--rw-r--r--   0        0        0    11575 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/maxcompute.py
--rw-r--r--   0        0        0    11026 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/maxcompute_itest.py
--rw-r--r--   0        0        0      180 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/postgres.py
--rw-r--r--   0        0        0    36959 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/rdb.py
--rw-r--r--   0        0        0    22096 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/rdb_itest.py
--rw-r--r--   0        0        0     1941 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/rdb_test.py
--rw-r--r--   0        0        0    11086 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/spark.py
--rw-r--r--   0        0        0     1379 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/spark_test.py
--rw-r--r--   0        0        0     7500 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/sql_dialect/__init__.py
--rw-r--r--   0        0        0     9455 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/sql_dialect/bigquery.py
--rw-r--r--   0        0        0     9286 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/sql_dialect/clickhouse.py
--rw-r--r--   0        0        0      811 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/sql_dialect/clickhouse_test.py
--rw-r--r--   0        0        0    10484 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/sql_dialect/postgres.py
--rw-r--r--   0        0        0      900 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/common.py
--rw-r--r--   0        0        0     7408 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/context.py
--rw-r--r--   0        0        0     2177 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/context_test.py
--rw-r--r--   0        0        0    11013 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/funcs.py
--rw-r--r--   0        0        0    19985 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/funcs_common.py
--rw-r--r--   0        0        0     3832 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/funcs_flink.py
--rw-r--r--   0        0        0     3099 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/funcs_flink_itest.py
--rw-r--r--   0        0        0     9704 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/funcs_itest.py
--rw-r--r--   0        0        0    11492 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/funcs_rdb.py
--rw-r--r--   0        0        0     8150 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/funcs_spark.py
--rw-r--r--   0        0        0     5545 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/report.py
--rw-r--r--   0        0        0     6149 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/sql_processor.py
--rw-r--r--   0        0        0    27013 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/step.py
--rw-r--r--   0        0        0     2400 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/step_test.py
--rw-r--r--   0        0        0     7351 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor_debugger.py
--rw-r--r--   0        0        0     6944 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor_debugger_itest.py
--rw-r--r--   0        0        0     6769 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor_itest.py
--rw-r--r--   0        0        0    20906 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor_test.py
--rw-r--r--   0        0        0     5061 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/sql_test.py
--rw-r--r--   0        0        0      583 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/sql_test_itest.py
--rw-r--r--   0        0        0    45124 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/sql_tester.py
--rw-r--r--   0        0        0     5383 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/sql_tester_test.py
--rw-r--r--   0        0        0        0 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/udf/__init__.py
--rw-r--r--   0        0        0      495 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/udf/check.py
--rw-r--r--   0        0        0     3211 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/udf/udfs.py
--rw-r--r--   0        0        0     2847 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/udf/udfs_test.py
--rw-r--r--   0        0        0        0 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/utils/__init__.py
--rw-r--r--   0        0        0     1664 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/utils/db_connection_utils.py
--rw-r--r--   0        0        0     1945 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/utils/flink_test_cluster.py
--rw-r--r--   0        0        0      491 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/utils/flink_test_cluster_itest.py
--rw-r--r--   0        0        0     1911 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/utils/io_utils.py
--rw-r--r--   0        0        0     1241 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/utils/kv.py
--rw-r--r--   0        0        0      455 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/utils/object_utils.py
--rw-r--r--   0        0        0      550 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/utils/object_utils_test.py
--rw-r--r--   0        0        0     5258 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/utils/sql_expr.py
--rw-r--r--   0        0        0     5857 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/utils/sql_expr_test.py
--rw-r--r--   0        0        0     2063 2023-05-08 01:52:22.861510 easy_sql_easy_sql-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    11302 1970-01-01 00:00:00.000000 easy_sql_easy_sql-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-02 10:49:04.655905 easy_sql_easy_sql-1.1.0/LICENSE
+-rw-r--r--   0        0        0     9497 2023-06-02 10:49:04.655905 easy_sql_easy_sql-1.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/__init__.py
+-rw-r--r--   0        0        0     2870 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/base_test.py
+-rw-r--r--   0        0        0        0 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/cli/__init__.py
+-rw-r--r--   0        0        0     8537 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/cli/backend_processor.py
+-rw-r--r--   0        0        0    14595 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/config/sql_config.py
+-rw-r--r--   0        0        0     4219 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/config/sql_config_test.py
+-rw-r--r--   0        0        0     2165 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/data_process.py
+-rw-r--r--   0        0        0     1040 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/data_process_itest.py
+-rw-r--r--   0        0        0     2779 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/data_process_test.py
+-rw-r--r--   0        0        0     2531 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/local_spark.py
+-rw-r--r--   0        0        0     1360 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/logger.py
+-rw-r--r--   0        0        0     3048 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/report.py
+-rw-r--r--   0        0        0      337 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/report_test.py
+-rw-r--r--   0        0        0     3054 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/spark_optimizer.py
+-rw-r--r--   0        0        0        0 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_linter/__init__.py
+-rw-r--r--   0        0        0      106 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_linter/rules/__init__.py
+-rw-r--r--   0        0        0     1430 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_linter/rules/bq_schema_rule.py
+-rw-r--r--   0        0        0    10316 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_linter/sql_linter.py
+-rw-r--r--   0        0        0     4337 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_linter/sql_linter_cli.py
+-rw-r--r--   0        0        0     2605 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_linter/sql_linter_reportor.py
+-rw-r--r--   0        0        0     6979 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_linter/sql_linter_test.py
+-rw-r--r--   0        0        0      620 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/__init__.py
+-rw-r--r--   0        0        0       62 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/backend/__init__.py
+-rw-r--r--   0        0        0     7034 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/backend/base.py
+-rw-r--r--   0        0        0      192 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/backend/bigquery.py
+-rw-r--r--   0        0        0      168 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/backend/clickhouse.py
+-rw-r--r--   0        0        0    14890 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/backend/flink.py
+-rw-r--r--   0        0        0    21693 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/backend/flink_itest.py
+-rw-r--r--   0        0        0    11553 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/backend/maxcompute.py
+-rw-r--r--   0        0        0    11026 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/backend/maxcompute_itest.py
+-rw-r--r--   0        0        0      180 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/backend/postgres.py
+-rw-r--r--   0        0        0    36957 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/backend/rdb.py
+-rw-r--r--   0        0        0    22096 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/backend/rdb_itest.py
+-rw-r--r--   0        0        0     1941 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/backend/rdb_test.py
+-rw-r--r--   0        0        0    11086 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/backend/spark.py
+-rw-r--r--   0        0        0     1379 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/backend/spark_test.py
+-rw-r--r--   0        0        0     7548 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/backend/sql_dialect/__init__.py
+-rw-r--r--   0        0        0     9453 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/backend/sql_dialect/bigquery.py
+-rw-r--r--   0        0        0     9284 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/backend/sql_dialect/clickhouse.py
+-rw-r--r--   0        0        0      811 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/backend/sql_dialect/clickhouse_test.py
+-rw-r--r--   0        0        0    10484 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/backend/sql_dialect/postgres.py
+-rw-r--r--   0        0        0      898 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/common.py
+-rw-r--r--   0        0        0     7408 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/context.py
+-rw-r--r--   0        0        0     2177 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/context_test.py
+-rw-r--r--   0        0        0    11202 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/funcs.py
+-rw-r--r--   0        0        0    19985 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/funcs_common.py
+-rw-r--r--   0        0        0     4023 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/funcs_flink.py
+-rw-r--r--   0        0        0     2674 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/funcs_flink_itest.py
+-rw-r--r--   0        0        0     9962 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/funcs_itest.py
+-rw-r--r--   0        0        0    11492 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/funcs_rdb.py
+-rw-r--r--   0        0        0     8092 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/funcs_spark.py
+-rw-r--r--   0        0        0     5523 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/report.py
+-rw-r--r--   0        0        0     6149 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/sql_processor.py
+-rw-r--r--   0        0        0    27013 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/step.py
+-rw-r--r--   0        0        0     2340 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/step_test.py
+-rw-r--r--   0        0        0     7351 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_processor_debugger.py
+-rw-r--r--   0        0        0     6944 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_processor_debugger_itest.py
+-rw-r--r--   0        0        0     6769 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_processor_itest.py
+-rw-r--r--   0        0        0    20906 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_processor_test.py
+-rw-r--r--   0        0        0     5061 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_test.py
+-rw-r--r--   0        0        0      583 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_test_itest.py
+-rw-r--r--   0        0        0    45024 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_tester.py
+-rw-r--r--   0        0        0     5383 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/sql_tester_test.py
+-rw-r--r--   0        0        0        0 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/udf/__init__.py
+-rw-r--r--   0        0        0      495 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/udf/check.py
+-rw-r--r--   0        0        0     3189 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/udf/udfs.py
+-rw-r--r--   0        0        0     2847 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/udf/udfs_test.py
+-rw-r--r--   0        0        0        0 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/utils/__init__.py
+-rw-r--r--   0        0        0     1279 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/utils/db_connection_utils.py
+-rw-r--r--   0        0        0     1945 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/utils/flink_test_cluster.py
+-rw-r--r--   0        0        0      491 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/utils/flink_test_cluster_itest.py
+-rw-r--r--   0        0        0     1932 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/utils/io_utils.py
+-rw-r--r--   0        0        0     1241 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/utils/kv.py
+-rw-r--r--   0        0        0      455 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/utils/object_utils.py
+-rw-r--r--   0        0        0      550 2023-06-02 10:49:04.671906 easy_sql_easy_sql-1.1.0/easy_sql/utils/object_utils_test.py
+-rw-r--r--   0        0        0     5258 2023-06-02 10:49:04.675906 easy_sql_easy_sql-1.1.0/easy_sql/utils/sql_expr.py
+-rw-r--r--   0        0        0     5857 2023-06-02 10:49:04.675906 easy_sql_easy_sql-1.1.0/easy_sql/utils/sql_expr_test.py
+-rw-r--r--   0        0        0     2599 2023-06-02 10:49:21.588178 easy_sql_easy_sql-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    11762 1970-01-01 00:00:00.000000 easy_sql_easy_sql-1.1.0/PKG-INFO
```

### Comparing `easy_sql_easy_sql-1.0.0/LICENSE` & `easy_sql_easy_sql-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_sql_easy_sql-1.0.0/README.md` & `easy_sql_easy_sql-1.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,15 @@
 mkdir -pv test/flink/jars
 wget -P test/flink/jars https://repo1.maven.org/maven2/org/apache/flink/flink-connector-jdbc/1.15.1/flink-connector-jdbc-1.15.1.jar
 wget -P test/flink/jars https://repo1.maven.org/maven2/org/postgresql/postgresql/42.2.14/postgresql-42.2.14.jar
 ```
 
 Create a file named `sample_etl.flink.postgres.sql` with content as the test file [here](https://github.com/easysql/easy_sql/blob/main/test/sample_etl.flink.postgres.sql).
 
-Create a connector configuration file named `sample_etl.flink_tables_file.json` with content as the test configuration file [here](https://github.com/easysql/easy_sql/blob/main/test/sample_etl.flink_tables_file.json).
+Create a connector configuration file named `sample_etl.flink_tables_file.yml` with content as the test configuration file [here](https://github.com/easysql/easy_sql/blob/main/test/sample_etl.flink_tables_file.yml).
 
 Run it with command:
 
 ```bash
 bash -c "$(python3 -m easy_sql.data_process -f sample_etl.flink.postgres.sql -p)"
 ```
```

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/base_test.py` & `easy_sql_easy_sql-1.1.0/easy_sql/base_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,29 +24,25 @@
 TEST_PG_URL = os.environ.get("PG_URL", "postgresql://postgres:123456@testpg:15432/postgres")
 TEST_PG_JDBC_URL = os.environ.get("PG_JDBC_URL", "jdbc:postgresql://testpg:15432/postgres")
 TEST_PG_JDBC_USER = os.environ.get("PG_JDBC_USER", "postgres")
 TEST_PG_JDBC_PASSWD = os.environ.get("PG_JDBC_PASSWD", "123456")
 TEST_CH_URL = os.environ.get("CLICKHOUSE_URL", "clickhouse+native://default@testch:30123")
 TEST_BQ_URL = os.environ.get("BQ_URL", "bigquery://")
 
-__partition_col_converter__ = (
-    lambda col: f"PARSE_DATE('%Y-%m', {col}) as {col}"
-    if col in ["data_month", ":data_month"]
-    else f"CAST({col} as DATE)"
+__partition_col_converter__ = lambda col: (
+    f"PARSE_DATE('%Y-%m', {col}) as {col}" if col in ["data_month", ":data_month"] else f"CAST({col} as DATE)"
 )
-__partition_value_converter__ = (
-    lambda col, value: datetime.strptime(value, "%Y-%m").date()
-    if col == "data_month"
-    else datetime.strptime(value, "%Y-%m-%d").date()
+__partition_value_converter__ = lambda col, value: (
+    datetime.strptime(value, "%Y-%m").date() if col == "data_month" else datetime.strptime(value, "%Y-%m-%d").date()
 )
-__column_sql_type_converter__ = (
-    lambda backend_type, col_name, col_type: "DATE" if col_name in ["di", "dt", "data_date", "data_month"] else None
+__column_sql_type_converter__ = lambda backend_type, col_name, col_type: (
+    "DATE" if col_name in ["di", "dt", "data_date", "data_month"] else None
 )
-__partition_expr__ = (
-    lambda backend_type, partition_col: f"DATE_TRUNC({partition_col}, MONTH)"
+__partition_expr__ = lambda backend_type, partition_col: (
+    f"DATE_TRUNC({partition_col}, MONTH)"
     if backend_type == "bigqiery" and partition_col == "data_month"
     else partition_col
 )
 bigquery_sql_expr = SqlExpr(
     column_sql_type_converter=__column_sql_type_converter__,
     partition_col_converter=__partition_col_converter__,
     partition_value_converter=__partition_value_converter__,
```

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/cli/backend_processor.py` & `easy_sql_easy_sql-1.1.0/easy_sql/cli/backend_processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     FlinkBackendConfig,
     SparkBackendConfig,
     parse_vars,
 )
 from easy_sql.logger import logger
 from easy_sql.sql_processor import SqlProcessor
 from easy_sql.sql_processor.backend import Backend
+from easy_sql.utils import db_connection_utils
 
 
 class BackendProcessor:
     def __init__(self, config: EasySqlConfig) -> None:
         self.config = config
 
     @staticmethod
@@ -124,41 +125,39 @@
         )
 
     def _create_backend(self, backend_config: Optional[List[str]]) -> Backend:
         from easy_sql.sql_processor.backend import FlinkBackend, FlinkTablesConfig
 
         config = FlinkBackendConfig(self.config, backend_config)
         backend = FlinkBackend(
-            self.config.is_batch, flink_tables_config=FlinkTablesConfig.from_config_file(config.flink_tables_file_path)
+            self.config.is_batch, flink_tables_config=FlinkTablesConfig.from_yml(config.flink_tables_file_path)
         )
 
         logger.info(f"Using flink configurations: {config.flink_configurations}")
         backend.set_configurations(config.flink_configurations)
 
-        backend.register_tables(self.config.tables)
-        if self.config.tables:
-            conn = None
-            for table in self.config.tables:
-                from easy_sql.utils import db_connection_utils
-
-                conn = db_connection_utils.get_table_raw_conn_for_flink_backend(backend, table)
-                if conn:
-                    break
+        backend.register_tables()
+
+        connector_name = self.config.get("prepare_sql_connector")
+        if connector_name:
+            conn = db_connection_utils.get_connector_raw_conn_for_flink_backend(backend, connector_name)
             if conn:
                 from easy_sql.sql_processor.backend.rdb import _exec_sql
 
                 self._exec_sql = lambda sql: _exec_sql(conn, sql)
 
         return backend
 
     def _exec_prepare_sql(self, backend: Backend, prepare_sql: str):
         if self._exec_sql:
             self._exec_sql(prepare_sql)
         else:
-            logger.warn("Cannot execute prepare-sql: the connector is not configured or not supported. Will skip this.")
+            logger.warning(
+                "Cannot execute prepare-sql: the connector is not configured or not supported. Will skip this."
+            )
 
 
 class PostgresBackendProcessor(BackendProcessor):
     def __init__(self, config: EasySqlConfig) -> None:
         super().__init__(config)
 
     def _create_backend(self, backend_config: Optional[List[str]]) -> Backend:
```

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/config/sql_config.py` & `easy_sql_easy_sql-1.1.0/easy_sql/config/sql_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,14 +154,23 @@
         return prepare_sql_list
 
     @property
     def abs_sql_file_path(self) -> str:
         assert self.sql_file is not None
         return resolve_file(self.sql_file, abs_path=True)
 
+    def get(self, key: str, splitter: Optional[str] = "=", strip: Optional[str] = None) -> str | None:
+        config = next(
+            filter(lambda c: get_key_by_splitter_and_strip(c, splitter, strip) == key, self.customized_easy_sql_conf),
+            None,
+        )
+        if config is None:
+            return None
+        return get_value_by_splitter_and_strip(config, splitter, strip)
+
     def _resolve_file(self, file_path: str, *, prefix: str = "") -> str:
         return resolve_file(file_path, abs_path=True, prefix=prefix, relative_to=self.abs_sql_file_path)
 
     def _build_conf_command_args(
         self,
         default_conf: List[str],
         user_default_conf: List[str],
@@ -309,16 +318,16 @@
         # config 的优先级：1. sql 代码里的 config 优先级高于这里的 default 配置
         # 对于数组类的 config，sql 代码里的 config 会添加进来，而不是覆盖默认配置
         config = self.config
         default_conf = [
             "--parallelism=1",
             (
                 f"--pyFiles={'file://' + self.config.abs_sql_file_path}"
-                f'{"," + self._resolve_file(config.udf_file_path) if config.udf_file_path else ""}'
-                f'{"," + self._resolve_file(config.func_file_path) if config.func_file_path else ""}'
+                f"{',' + self._resolve_file(config.udf_file_path) if config.udf_file_path else ''}"
+                f"{',' + self._resolve_file(config.func_file_path) if config.func_file_path else ''}"
             ),
         ]
 
         # refer: https://nightlies.apache.org/flink/flink-docs-master/docs/deployment/cli/
         file_keys = [
             "-pyarch",
             "--pyArchives",
```

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/config/sql_config_test.py` & `easy_sql_easy_sql-1.1.0/easy_sql/config/sql_config_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,14 @@
         self.assertEqual(find_conf("--pyFiles ")[0].count(","), 2)
 
     def test_parse_flink_config_with_relative_files(self):
         _config = EasySqlConfig.from_sql(
             sql="""
 -- config: easy_sql.udf_file_path=sample_data_process.py
 -- config: easy_sql.func_file_path=sample_data_process.py
--- config: easy_sql.flink_tables_file_path=sample_etl.flink_tables_file.json
 -- config: flink.cmd=--pyFiles sample_etl.postgres.sql
 -- config: flink.cmd=-pyarch sample_etl.spark.sql,test/sample_etl.postgres.sql,
         """,
             sql_file="test/sample_etl.spark.sql",
         )
 
         config = FlinkBackendConfig(_config)
```

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/data_process.py` & `easy_sql_easy_sql-1.1.0/easy_sql/data_process.py`

 * *Files identical despite different names*

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/data_process_itest.py` & `easy_sql_easy_sql-1.1.0/easy_sql/data_process_itest.py`

 * *Files identical despite different names*

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/data_process_test.py` & `easy_sql_easy_sql-1.1.0/easy_sql/data_process_test.py`

 * *Files identical despite different names*

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/local_spark.py` & `easy_sql_easy_sql-1.1.0/easy_sql/local_spark.py`

 * *Files identical despite different names*

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/logger.py` & `easy_sql_easy_sql-1.1.0/easy_sql/logger.py`

 * *Files identical despite different names*

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/report.py` & `easy_sql_easy_sql-1.1.0/easy_sql/report.py`

 * *Files identical despite different names*

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/spark_optimizer.py` & `easy_sql_easy_sql-1.1.0/easy_sql/spark_optimizer.py`

 * *Files identical despite different names*

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/sql_linter/rules/bq_schema_rule.py` & `easy_sql_easy_sql-1.1.0/easy_sql/sql_linter/rules/bq_schema_rule.py`

 * *Files identical despite different names*

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/sql_linter/sql_linter.py` & `easy_sql_easy_sql-1.1.0/easy_sql/sql_linter/sql_linter.py`

 * *Files identical despite different names*

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/sql_linter/sql_linter_cli.py` & `easy_sql_easy_sql-1.1.0/easy_sql/sql_linter/sql_linter_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     exclude: str,
     include: str,
     backend: str,
     easy_sql: bool,
     config_path: Optional[str] = None,
 ):
     if not check_sql_file_path.endswith(".sql"):
-        warnings.warn("file name:" + check_sql_file_path + " must end with .sql")
+        warnings.warn("file name:" + check_sql_file_path + " must end with .sql", stacklevel=2)
 
     with open(check_sql_file_path, "r") as file:
         sql = file.read()
     sql_linter = SqlLinter(sql, exclude_rules=split_rules_to_list(exclude), include_rules=split_rules_to_list(include))
     backend = backend if backend else parse_backend(sql)
     print("using backend:", backend)
     result = sql_linter.lint(backend, easysql=easy_sql, config_path=config_path)
```

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/sql_linter/sql_linter_reportor.py` & `easy_sql_easy_sql-1.1.0/easy_sql/sql_linter/sql_linter_reportor.py`

 * *Files identical despite different names*

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/sql_linter/sql_linter_test.py` & `easy_sql_easy_sql-1.1.0/easy_sql/sql_linter/sql_linter_test.py`

 * *Files identical despite different names*

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/__init__.py` & `easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/__init__.py`

 * *Files identical despite different names*

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/base.py` & `easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/backend/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,15 +174,15 @@
             catalog_name, dbname, pure_table_name = None, None, self.table_name
         return catalog_name, dbname, pure_table_name
 
     def has_partitions(self):
         return len(self.partitions) > 0
 
     def has_dynamic_partition(self):
-        return any([pt.value is None for pt in self.partitions])
+        return any(pt.value is None for pt in self.partitions)
 
     def get_full_table_name(self, temp_db: Optional[str] = None):
         return (
             f"{self.catalog_name}.{self.dbname or temp_db}.{self.pure_table_name}"
             if self.catalog_name
             else f"{self.dbname or temp_db}.{self.pure_table_name}"
         )
```

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/flink.py` & `easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/backend/flink.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
-import json
-import os
-import re
-from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple
+from dataclasses import dataclass
+from pathlib import Path
+from typing import TYPE_CHECKING, Any, Callable, Dict, Iterable, List, Optional, Tuple
 
 from ...logger import logger
 from .base import Backend, Row, SaveMode, Table, TableMeta
 
 if TYPE_CHECKING:
     from pyflink.common import Row as PyFlinkRow
     from pyflink.table import Table as PyFlinkTable
@@ -82,15 +81,15 @@
 
 class FlinkBackend(Backend):
     # todo: 考虑是否需要在外面实例化flink: TableEnvironment
     def __init__(self, is_batch: Optional[bool] = True, flink_tables_config: Optional[FlinkTablesConfig] = None):
         from pyflink.datastream import StreamExecutionEnvironment
         from pyflink.table import EnvironmentSettings, StreamTableEnvironment
 
-        self.flink_tables_config = flink_tables_config or FlinkTablesConfig({})
+        self.flink_tables_config = flink_tables_config or FlinkTablesConfig({}, {})
 
         self.flink_stream_env = None if is_batch else StreamExecutionEnvironment.get_execution_environment()
         env_settings = EnvironmentSettings.in_batch_mode() if is_batch else EnvironmentSettings.in_streaming_mode()
         self.flink: StreamTableEnvironment = StreamTableEnvironment.create(
             stream_execution_environment=self.flink_stream_env,  # type: ignore
             environment_settings=env_settings,
         )
@@ -123,17 +122,18 @@
                 logger.info("committed insert statements.")
                 self.streaming_insert_stmts = self.flink.create_statement_set()
                 self.has_streaming_insert_stmts = False
             else:
                 logger.info("no insert statements to commit.")
 
     def clean(self):
+        self.execute_streaming_inserts()
+
         for temp_view in self.flink.list_temporary_views():
             self.flink.drop_temporary_view(temp_view)
-        self.execute_streaming_inserts()
 
     def exec_native_sql(self, sql: str) -> TableResult:
         logger.info(f"will exec sql: {sql}")
         return self.flink.execute_sql(sql)
 
     def exec_native_sql_query(self, sql: str) -> PyFlinkTable:
         logger.info(f"will exec sql: {sql}")
@@ -167,199 +167,199 @@
     def save_table(
         self,
         source_table_meta: TableMeta,
         target_table_meta: TableMeta,
         save_mode: SaveMode,
         create_target_table: bool = False,
     ):
-        from pyflink.table.expressions import col, lit
-
+        source_table_name = source_table_meta.table_name
+        sink_table_name = target_table_meta.table_name
         if not self.table_exists(target_table_meta):
             raise Exception(
-                f"target table {target_table_meta.table_name} does not exist, "
-                f"cannot save table {target_table_meta.table_name} to {target_table_meta.table_name}"
+                f"target table {sink_table_name} does not exist, "
+                f"cannot save table {source_table_name} to {sink_table_name}"
             )
 
-        temp_res = self.exec_native_sql_query(f"select * from {source_table_meta.table_name}")
-        # 纯动态分区时，如果当日没有新增数据，则不会创建 partition。而我们希望对于静态分区，总是应该创建分区，即使当日没有数据
-        static_partitions = list(filter(lambda p: p.value, target_table_meta.partitions))
-        table_description = list(self.exec_native_sql(f"desc {target_table_meta.table_name}").collect())
-        columns: List[str] = [f[0] for f in table_description]  # type: ignore
-        for p in static_partitions:
-            temp_res = temp_res.add_columns(lit(p.value).alias(p.field))
-        temp_res = temp_res.select(*[col(column) for column in columns])
+        source_table = self._align_fields(source_table_meta, target_table_meta)
 
-        logger.info(f"save table {source_table_meta.table_name} to {target_table_meta.table_name}")
+        override_insert = save_mode == SaveMode.overwrite
         if self.streaming_insert_stmts is not None:
-            logger.info("add insert to streaming_insert_stmts.")
-            self.streaming_insert_stmts.add_insert(
-                target_table_meta.table_name, temp_res, save_mode == SaveMode.overwrite
-            )
+            logger.info(f"prepare insert into streaming_insert_stmts: from {source_table_name} to {sink_table_name}.")
+            self.streaming_insert_stmts.add_insert(sink_table_name, source_table, overwrite=override_insert)
             self.has_streaming_insert_stmts = True
         else:
-            temp_res.execute_insert(target_table_meta.table_name, save_mode == SaveMode.overwrite)
+            logger.info(f"save table {source_table_name} to {sink_table_name}")
+            source_table.execute_insert(sink_table_name, overwrite=override_insert)
+
+    def _align_fields(self, source_table_meta: TableMeta, target_table_meta: TableMeta):
+        from pyflink.table.expressions import col, lit
+
+        source_table = self.flink.from_path(source_table_meta.table_name)
+
+        # 纯动态分区时，如果当日没有新增数据，则不会创建 partition。而我们希望对于静态分区，总是应该创建分区，即使当日没有数据
+        static_partitions = list(filter(lambda p: p.value, target_table_meta.partitions))
+        for p in static_partitions:
+            source_table = source_table.add_columns(lit(p.value).alias(p.field))
+
+        target_table_schema = list(self.exec_native_sql(f"desc {target_table_meta.table_name}").collect())
+        # <Row('computed_field', 'BIGINT', True, None, 'AS `user` * `amount`', None)>
+        target_needed_columns: List[str] = [f[0] for f in target_table_schema if f[4] is None]  # type: ignore
+
+        source_table = source_table.select(*[col(column) for column in target_needed_columns])
+        return source_table
 
     def refresh_table_partitions(self, table: TableMeta):
         # flink无法从`desc table`中解析出partition字段，但是可以在flink_source_file中配置table的partition字段
         pass
 
-    def _register_catalog(self):
-        for catalog in self.flink_tables_config.catalogs:
-            catalog = catalog.copy()
-            catalog_name = catalog["name"]
-            del catalog["name"]
-            catalog_expr = " , ".join([f"'{option}' = '{catalog[option]}'" for option in catalog])
-            try:  # noqa: SIM105
-                self.exec_native_sql(
-                    f"""
-                        CREATE CATALOG {catalog_name}
-                        WITH (
-                            {catalog_expr}
-                        );
-                    """
-                )
-            except Exception:
-                logger.warn(f"create catalog {catalog_name} failed.", exc_info=True)
-
-    def _register_tables(self, tables: List[str]):
-        if len(tables) == 0:
-            return
-        for table in tables:
-            db_name, table_config, connector = self.get_table_config_and_connector(table)
-            if db_name and table_config and connector:
-                self.exec_native_sql(f"create database if not exists {db_name}")
-                self._create_table(table, table_config, connector)
-            else:
-                logger.warn(f"register table {table} failed, no configuration found")
-
-    def get_table_config_and_connector(self, table: str) -> Tuple[Optional[str], Optional[Dict], Optional[Dict]]:
-        db_name = table.strip().split(".")[0]
-        database = self.flink_tables_config.database(db_name)
-        if not database:
-            logger.warn(f"database {db_name} does not exist in flink tables config file")
-            return None, None, None
-
-        table_name = table.strip().split(".")[1]
-        table_config = self.flink_tables_config.table(database, table_name)
-        if not table_config:
-            logger.warn(f"table {table} does not exist in flink tables config file")
-            return None, None, None
-
-        connector_name = table_config["connector"]["name"]
-        connector = self.flink_tables_config.connector(database, connector_name)
-        if not connector:
-            logger.warn(f"connector {connector_name} does not exist in flink tables config file")
-            return None, None, None
-        return db_name, table_config, connector
-
-    def get_db_connector(self, db_name: str, connector_name: str) -> Optional[Dict]:
-        database = self.flink_tables_config.database(db_name)
-        if not database:
-            logger.warn(f"database {db_name} does not exist in flink tables config file")
-            return None
-        connector_config = self.flink_tables_config.connector(database, connector_name)
-        if not connector_config:
-            logger.warn(f"connector {connector_name} does not exist in flink tables config file")
-            return None
-        return connector_config
-
-    def _create_table(self, table: str, table_config: Dict, connector: Dict):
-        schema = table_config["schema"]
-        schema_expr = " , ".join(schema)
-        partition_by_expr = (
-            f"""
-                PARTITIONED BY ({','.join(table_config['partition_by'])})"""
-            if "partition_by" in table_config
-            else ""
-        )
-        options = self.flink_tables_config.table_options(connector, table_config)
-        options_expr = " , ".join([f"'{option}' = '{options[option]}'" for option in options])
-        create_sql = f"""
-            create table {table.strip()} (
-                {schema_expr}
-            )
-            {partition_by_expr}
-            WITH (
-                {options_expr}
-            );
-        """
-        self.exec_native_sql(create_sql)
-
-    def register_tables(self, tables: List[str], include_catalog: bool = True):
-        if self.flink_tables_config:
-            if include_catalog:
-                self._register_catalog()
-            self._register_tables(tables)
+    def register_tables(self):
+        for name, ddl in self.flink_tables_config.generate_catalog_ddl():
+            exists = self.flink.get_catalog(name)
+            if not exists:
+                self.exec_native_sql(ddl)
+        for ddl in self.flink_tables_config.generate_db_ddl():
+            self.exec_native_sql(ddl)
+        for ddl in self.flink_tables_config.generate_table_ddl():
+            self.exec_native_sql(ddl)
 
     def add_jars(self, jars_path: List[str]):
         self.flink.get_config().set("pipeline.jars", f'{";".join([f"file://{path}" for path in jars_path])}')
 
     def set_configurations(self, configs: dict):
         for c in configs:
             self.flink.get_config().set(c, configs[c])
 
 
+@dataclass
 class FlinkTablesConfig:
-    def __init__(self, config: Dict[str, Any]) -> None:
-        self.config = config
+    connectors: Dict[str, Connector]
+    catalogs: Dict[str, Catalog]
+
+    @dataclass
+    class Connector:
+        options: str
+
+        @staticmethod
+        def from_dict(data: dict) -> FlinkTablesConfig.Connector:
+            return FlinkTablesConfig.Connector(data.get("options", ""))
+
+    @dataclass
+    class Catalog:
+        databases: Dict[str, FlinkTablesConfig.Database]
+        temporary_tables: Dict[str, FlinkTablesConfig.Table]
+        options: str
+
+        @staticmethod
+        def from_dict(data: dict) -> FlinkTablesConfig.Catalog:
+            options = data.get("options", "")
+            databases = {
+                key: FlinkTablesConfig.Database.from_dict(item) for key, item in data.get("databases", {}).items()
+            }
+            temporary_tables = {
+                key: FlinkTablesConfig.Table.from_dict(item) for key, item in data.get("temporary_tables", {}).items()
+            }
+
+            return FlinkTablesConfig.Catalog(options=options, databases=databases, temporary_tables=temporary_tables)
+
+    @dataclass
+    class Database:
+        tables: Dict[str, FlinkTablesConfig.Table]
+
+        @staticmethod
+        def from_dict(data: dict) -> FlinkTablesConfig.Database:
+            tables = {key: FlinkTablesConfig.Table.from_dict(item) for key, item in data.get("tables", {}).items()}
+
+            return FlinkTablesConfig.Database(tables=tables)
+
+    @dataclass
+    class Table:
+        schema: str
+        options: str | None = None
+        partition_by: str | None = None
+        connector: str | None = None
+
+        @staticmethod
+        def from_dict(data: dict) -> FlinkTablesConfig.Table:
+            return FlinkTablesConfig.Table(**data)
 
     @staticmethod
-    def from_config_file(config_file_path: Optional[str] = None) -> FlinkTablesConfig:
-        if not config_file_path or not os.path.exists(config_file_path) or not os.path.isfile(config_file_path):
-            logger.warn(
-                "config file '{config_file_path}' does not exist or is not a file, will create an empty"
-                " FlinkTablesConfig"
-            )
-            return FlinkTablesConfig({})
-        with open(config_file_path, "r") as f:
-            config = json.loads(f.read())
-            return FlinkTablesConfig(config)
-
-    @property
-    def catalogs(self) -> List[Dict]:
-        if "catalogs" in self.config:
-            return self.config["catalogs"]
-        else:
-            return []
+    def from_yml(file_path: str | None) -> FlinkTablesConfig:
+        import yaml
 
-    @property
-    def databases(self) -> List[Dict]:
-        if "databases" in self.config:
-            return self.config["databases"]
-        else:
-            return []
+        if file_path is None:
+            return FlinkTablesConfig({}, {})
 
-    def database(self, name: str) -> Optional[Dict]:
-        return next(filter(lambda t: t["name"] == name, self.databases), None)
+        with Path(file_path).open() as f:
+            res: dict = yaml.safe_load(f)
+            return FlinkTablesConfig.from_dict(res)
+
+    @staticmethod
+    def from_dict(data: dict) -> FlinkTablesConfig:
+        connectors = {
+            key: FlinkTablesConfig.Connector.from_dict(item) for key, item in data.get("connectors", {}).items()
+        }
+        catalogs = {key: FlinkTablesConfig.Catalog.from_dict(item) for key, item in data.get("catalogs", {}).items()}
+
+        return FlinkTablesConfig(connectors=connectors, catalogs=catalogs)
+
+    def generate_catalog_ddl(self) -> Iterable[tuple[str, str]]:
+        for name, catalog in self.catalogs.items():
+            ddl = f"CREATE CATALOG {name} with ({catalog.options})"
+            yield name, ddl
+
+    def generate_db_ddl(self) -> Iterable[str]:
+        for cata_name, cata in self.catalogs.items():
+            for db_name, _ in cata.databases.items():
+                ddl = f"CREATE database if not exists {cata_name}.{db_name}"
+                yield ddl
+
+    def generate_table_ddl(self) -> Iterable[str]:
+        for cata_name, cata in self.catalogs.items():
+            for db_name, db in cata.databases.items():
+                for tb_name, tb in db.tables.items():
+                    full_tb_name = f"{cata_name}.{db_name}.{tb_name}"
+                    ddl = self._generate_table_ddl(tb, full_tb_name)
+                    yield ddl
+            for tp_tb_name, tp_tb in cata.temporary_tables.items():
+                ddl = self._generate_table_ddl(tp_tb, tp_tb_name, is_temporary=True)
+                yield ddl
+
+    def _generate_table_ddl(self, tb: FlinkTablesConfig.Table, tb_name: str, is_temporary=False) -> str:
+        merged_options = self._merge_table_options(tb)
+        options_expr = f"with ({merged_options})" if merged_options else ""
+
+        partition_by_expr = f"partitioned by ({tb.partition_by})" if tb.partition_by else ""
+        ddl = (
+            f'create {"temporary" if is_temporary else ""} table if not exists {tb_name} ({tb.schema})'
+            f" {partition_by_expr} {options_expr}"
+        )
+        return ddl
 
-    def table(self, database_config: Dict, table_name: str) -> Optional[Dict]:
-        return next(filter(lambda t: t["name"] == table_name, database_config["tables"]), None)
+    def _merge_table_options(self, tb: FlinkTablesConfig.Table) -> str | None:
+        base_options = {}
+        tb_options = self.parse_options(tb.options or "")
+        connector_name = tb.connector
+        if connector_name:
+            base_options = self.get_connector_options(connector_name)
+
+        base_options.update(tb_options)
+        merged_options = " , ".join([f"{k} = {v}" for k, v in base_options.items()])
+        return merged_options
 
-    def connector(self, database_config: Dict, connector_name: str) -> Optional[Dict]:
-        connectors = database_config.get("connectors", [])
-        return next(filter(lambda conn: conn["name"] == connector_name, connectors), None)
-
-    def table_options(self, connector: Dict, table: Dict) -> Dict[str, str]:
-        options = connector.get("options", {}).copy()
-        tableOptions = table.get("connector", {}).get("options", {})
-        options.update(tableOptions)
-        if "path" in options and "path" not in tableOptions:
-            assert "." not in table["name"], "Table name in configuration must not contains db, found " + table["name"]
-            options["path"] = options["path"].rstrip("/") + f"/{table['name']}"
+    def get_connector_options(self, name: str) -> Dict[str, str]:
+        connector = self.connectors.get(name)
+        if not connector:
+            raise Exception(f"couldn't find connector {name} in {list(self.connectors.keys())}")
+        options = self.parse_options(connector.options)
         return options
 
-    def table_fields(self, full_table_name: str, exclude_fields: Optional[List[str]] = None) -> List[str]:
-        exclude_fields = exclude_fields or []
-        assert full_table_name.count(".") == 1, 'full_table_name must in format "db.table", found: ' + full_table_name
-        db, table = tuple(full_table_name.split("."))
-        db_config = self.database(db)
-        if not db_config:
-            raise Exception("db configuration not found for " + db)
-        table_config = self.table(db_config, table)
-        if not table_config:
-            raise Exception("table configuration not found for " + full_table_name)
-        if "schema" not in table_config:
-            raise Exception("schema not found in table configuration for " + full_table_name)
-        field_expr_list: List[str] = table_config["schema"]
-        extract_field_name = lambda field_expr: re.split(r"\s", field_expr)[0].strip("'\"`")
-        fields = [extract_field_name(field_expr) for field_expr in field_expr_list]
-        return [f for f in fields if f not in exclude_fields]
+    @staticmethod
+    def parse_options(option_str: str) -> Dict[str, str]:
+        option_str = option_str or ""
+        options = {}
+        for line in option_str.splitlines():
+            for each_option in line.split(","):
+                if each_option.strip() == "":
+                    continue
+                key, value = each_option.split("=")
+                options[key.strip()] = value.strip()
+        return options
```

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/maxcompute.py` & `easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/backend/maxcompute.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,22 +174,20 @@
 
         else:
             target_cols = target_table.schema.names
             partition_expr = self.__partition_expr__(target_table_meta, PartitionMode.ALL_STATIC)
 
         temp_res = self.backend.exec_sql(f"select {', '.join(target_cols)} from {temp_res.table_name}")
 
-        self.backend.exec_native_sql(
-            f"""
+        self.backend.exec_native_sql(f"""
             insert {'into' if save_mode == SaveMode.append else save_mode.name}
             table {target_table_meta.table_name}
             {partition_expr}
             select * from {temp_res.table_name}
-        """
-        )
+        """)
 
 
 class MaxComputeBackend(Backend):
     def __init__(self, sql_expr: Optional[SqlExpr], **kwargs):
         from odps import ODPS
 
         self.conn = ODPS(**kwargs)
```

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/maxcompute_itest.py` & `easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/backend/maxcompute_itest.py`

 * *Files identical despite different names*

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/rdb.py` & `easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/backend/rdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,15 @@
 
     def _field_names(self, table_name: str) -> List[str]:
         result: ResultProxy = self._exec_sql(f"select * from {table_name} limit 0")
         result.close()
         return list(result.keys())
 
     def first(self) -> RdbRow:
-        all_action_are_limit = all([action[0] == "limit" for action in self._actions])
+        all_action_are_limit = all(action[0] == "limit" for action in self._actions)
         if all_action_are_limit:
             min_limit = min([action[1] for action in self._actions]) if len(self._actions) > 0 else 1
 
             result: ResultProxy = self._exec_sql(self.sql)
             if min_limit <= 0:
                 return RdbRow(list(result.keys()), ())
             with TimeLog(
```

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/rdb_itest.py` & `easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/backend/rdb_itest.py`

 * *Files identical despite different names*

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/rdb_test.py` & `easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/backend/rdb_test.py`

 * *Files identical despite different names*

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/spark.py` & `easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/backend/spark.py`

 * *Files identical despite different names*

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/spark_test.py` & `easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/backend/spark_test.py`

 * *Files identical despite different names*

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/sql_dialect/__init__.py` & `easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/backend/sql_dialect/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,17 +165,19 @@
         else:
             if len(partition_cols) > 1:
                 raise SqlProcessorAssertionError(
                     f"Only single-column partitioning is supported! found: {partition_cols}"
                 )
             # the format of pt_col may be :{pt_col}, which is transferred by method create_table_with_data
             return [
-                col
-                if col not in [partition_cols[0], f":{partition_cols[0]}"]
-                else self.sql_expr.convert_partition_col(col)
+                (
+                    col
+                    if col not in [partition_cols[0], f":{partition_cols[0]}"]
+                    else self.sql_expr.convert_partition_col(col)
+                )
                 for col in all_cols
             ]
 
     def insert_data_sql(
         self, table_name: str, col_names_expr: str, select_sql: str, partitions: List[Partition]
     ) -> Union[str, List[str]]:
         raise NotImplementedError()
```

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/sql_dialect/bigquery.py` & `easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/backend/sql_dialect/bigquery.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
 
     def create_partition_automatically(self):
         return True
 
     def insert_data_sql(self, table_name: str, col_names_expr: str, select_sql: str, partitions: List[Partition]):
         if not self.contains_db(table_name):
             raise SqlProcessorAssertionError("BigQuery table must be qualified with a dataset.")
-        if any([pt.value is None for pt in partitions]):
+        if any(pt.value is None for pt in partitions):
             raise SqlProcessorAssertionError(
                 f"cannot insert data when partition value is None, partitions: {partitions}, "
                 "there maybe some bug, please check"
             )
 
         insert_date_sql = f"insert into {table_name}({col_names_expr}) {select_sql};"
         delete_pt_metadata_if_exist = self.delete_pt_metadata_sql(table_name, partitions)
```

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/sql_dialect/clickhouse.py` & `easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/backend/sql_dialect/clickhouse.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,15 +192,15 @@
             f"where db_name = '{db}' and table_name = '{pure_table_name}' "
             f"and partition_value = '{partitions[0].value}'"
         )
         insert_pt_metadata = self.insert_pt_metadata_sql(table_name, partitions)
         return drop_pt_metadata_if_exist, insert_pt_metadata
 
     def _check_no_none_in_partition_values(self, partitions: List[Partition]):
-        if any([pt.value is None for pt in partitions]):
+        if any(pt.value is None for pt in partitions):
             raise SqlProcessorAssertionError(
                 f"cannot insert data when partition value is None, partitions: {partitions}, there maybe some bug,"
                 " please check"
             )
 
     def _check_partition_field_single(self, partitions: List[Partition]):
         if len(partitions) > 1:
```

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/sql_dialect/clickhouse_test.py` & `easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/backend/sql_dialect/clickhouse_test.py`

 * *Files identical despite different names*

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/sql_dialect/postgres.py` & `easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/backend/sql_dialect/postgres.py`

 * *Files identical despite different names*

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/common.py` & `easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/common.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 def _exec_sql(spark: SparkSession, sql: str) -> DataFrame:
     logger.info(f"will exec sql: {sql}")
     return spark.sql(sql)
 
 
 def is_int_type(type_name):
-    return any([type_name.startswith(t) for t in ["integer", "long", "decimal", "short"]])
+    return any(type_name.startswith(t) for t in ["integer", "long", "decimal", "short"])
 
 
 class Column:
     def __init__(self, name: str, value: Any):
         self.name, self.value = name, value
```

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/context.py` & `easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/context.py`

 * *Files identical despite different names*

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/context_test.py` & `easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/context_test.py`

 * *Files identical despite different names*

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/funcs.py` & `easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/funcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from typing import Callable, Dict, List, Optional, Tuple
 
+from easy_sql.sql_processor.funcs_flink import SetConfigFuncs
+
 from .backend import Backend, FlinkBackend, SparkBackend
 from .backend.rdb import RdbBackend
 from .common import SqlProcessorException, VarsReplacer
 
 __all__ = ["FuncRunner"]
 
 
@@ -88,15 +90,17 @@
             "partition_not_exists": partition_funcs.partition_not_exists,
             "is_first_partition": partition_funcs.is_first_partition,
             "is_not_first_partition": partition_funcs.is_not_first_partition,
             "previous_partition_exists": partition_funcs.previous_partition_exists,
             "get_partition_or_first_partition": partition_funcs.get_partition_or_first_partition,
             "ensure_dwd_partition_exists": partition_funcs.ensure_dwd_partition_exists,
             "ensure_table_partition_exists": partition_funcs.ensure_table_partition_exists,
-            "ensure_table_partition_or_first_partition_exists": partition_funcs.ensure_table_partition_or_first_partition_exists,
+            "ensure_table_partition_or_first_partition_exists": (
+                partition_funcs.ensure_table_partition_or_first_partition_exists
+            ),
             "get_partition_col": partition_funcs.get_partition_col,
             "get_first_partition": partition_funcs.get_first_partition,
             "get_last_partition": partition_funcs.get_last_partition,
             "ensure_partition_exists": partition_funcs.ensure_partition_exists,
             "ensure_partition_or_first_partition_exists": partition_funcs.ensure_partition_or_first_partition_exists,
             "get_partition_values_as_joined_str": partition_funcs.get_partition_values_as_joined_str,
             "all_cols_without_one_expr": col_funcs.all_cols_without_one_expr,
@@ -136,14 +140,15 @@
             "check_not_null_column_in_table": table_funcs.check_not_null_column_in_table,
             "data_profiling_report": ana_funcs.data_profiling_report,
             "set_parallelism": parallelism_funcs.set_parallelism,
             "execute_streaming_inserts": streaming_funcs.execute_streaming_inserts,
             "sleep": test_funcs.sleep,
             "test_run_etl": test_funcs.test_run_etl,
             "exec_sql_in_source": test_funcs.exec_sql_in_source,
+            "set_config": SetConfigFuncs(backend).set_config,
         }
 
     @staticmethod
     def _get_spark_funcs(backend) -> Dict[str, Callable]:
         from easy_sql.sql_processor.funcs_spark import (
             AnalyticsFuncs,
             CacheFuncs,
@@ -177,15 +182,17 @@
             "partition_not_exists": partition_funcs.partition_not_exists,
             "is_first_partition": partition_funcs.is_first_partition,
             "is_not_first_partition": partition_funcs.is_not_first_partition,
             "previous_partition_exists": partition_funcs.previous_partition_exists,
             "get_partition_or_first_partition": partition_funcs.get_partition_or_first_partition,
             "ensure_dwd_partition_exists": partition_funcs.ensure_dwd_partition_exists,
             "ensure_table_partition_exists": partition_funcs.ensure_table_partition_exists,
-            "ensure_table_partition_or_first_partition_exists": partition_funcs.ensure_table_partition_or_first_partition_exists,
+            "ensure_table_partition_or_first_partition_exists": (
+                partition_funcs.ensure_table_partition_or_first_partition_exists
+            ),
             "get_partition_col": partition_funcs.get_partition_col,
             "get_first_partition": partition_funcs.get_first_partition,
             "get_last_partition": partition_funcs.get_last_partition,
             "ensure_partition_exists": partition_funcs.ensure_partition_exists,
             "ensure_partition_or_first_partition_exists": partition_funcs.ensure_partition_or_first_partition_exists,
             "get_partition_values_as_joined_str": partition_funcs.get_partition_values_as_joined_str,
             "all_cols_without_one_expr": col_funcs.all_cols_without_one_expr,
```

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/funcs_common.py` & `easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/funcs_common.py`

 * *Files identical despite different names*

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/funcs_flink.py` & `easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/funcs_flink.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,23 @@
     "AlertFunc",
     "TableFuncs",
     "AnalyticsFuncs",
     "TestFuncs",
 ]
 
 
+class SetConfigFuncs:
+    def __init__(self, bkd: FlinkBackend) -> None:
+        self.bkd = bkd
+        pass
+
+    def set_config(self, key: str, value: str):
+        return self.bkd.flink.get_config().set(key, value)
+
+
 class ParallelismFuncs:
     def __init__(self, flink: FlinkBackend):
         self.flink = flink
 
     def set_parallelism(self, partitions: str):
         try:
             int(partitions)
@@ -52,15 +61,15 @@
 
     def exec_sql_in_source(self, step: Step, db: str, connector: str):
         from easy_sql.utils.db_connection_utils import (
             get_connector_raw_conn_for_flink_backend,
         )
 
         if step.select_sql:
-            conn = get_connector_raw_conn_for_flink_backend(self.flink, db, connector)
+            conn = get_connector_raw_conn_for_flink_backend(self.flink, connector)
             if not conn:
                 raise Exception(
                     f"Cannot build a suitable coonnection for db {db} and connector {connector}. Please ensure it is"
                     " configured properly."
                 )
             sql_list = [
                 sql.strip() for sql in step.select_sql.split("\n") if sql.strip() and not sql.strip().startswith("--")
@@ -92,17 +101,15 @@
             print("relative to: ", relative_to)
         else:
             relative_to = ""
 
         etl_file = resolve_file(etl_file, abs_path=True, relative_to=relative_to)
         with open(etl_file, "r") as f:
             etl_content = f.readlines()
-        is_streaming = any(
-            [re.match(r"^-- config:\s*easy_sql\.etl_type\s*=\s*streaming", line) for line in etl_content]
-        )
+        is_streaming = any(re.match(r"^-- config:\s*easy_sql\.etl_type\s*=\s*streaming", line) for line in etl_content)
 
         if is_streaming:
             fm = FlinkTestClusterManager()
 
             originally_started = True
             if fm.is_not_started():
                 originally_started = False
```

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/funcs_flink_itest.py` & `easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/funcs_flink_itest.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,79 +14,65 @@
 
 
 class FlinkFuncsTest(unittest.TestCase):
     def create_flink_backend(self):
         return FlinkBackend(
             True,
             FlinkTablesConfig(
-                {
-                    "databases": [
-                        {
-                            "name": "db",
-                            "connectors": [
-                                {
-                                    "name": "jdbc",
-                                    "options": {
-                                        "connector": "jdbc",
-                                        "url": TEST_PG_JDBC_URL,
-                                        "username": TEST_PG_JDBC_USER,
-                                        "password": TEST_PG_JDBC_PASSWD,
-                                    },
-                                }
-                            ],
-                        }
-                    ]
-                }
+                connectors={
+                    "jdbc": FlinkTablesConfig.Connector(f"""
+                                    'url' = '{TEST_PG_JDBC_URL}',
+                                    'username' = '{TEST_PG_JDBC_USER}',
+                                    'password' = '{TEST_PG_JDBC_PASSWD}'
+                    """),
+                },
+                catalogs={},
             ),
         )
 
     def test_exec_sql_in_source(self):
         fb = self.create_flink_backend()
         tf = TestFuncs(fb)
         tf.exec_sql_in_source(step_with_sql("select 1;\nselect now();"), "db", "jdbc")
 
     def test_run_etl_streaming(self):
         fb = self.create_flink_backend()
         tf = TestFuncs(fb)
         with open("/tmp/flink_func_test__test_run_etl.sql", "w") as f:
-            f.write(
-                """
+            f.write("""
 -- backend: flink
 -- config: easy_sql.etl_type=streaming
 -- config: flink.cmd=-pyexec python3
 -- config: flink.cmd=-t remote
 -- config: flink.cmd=-pyclientexec python3
 -- target=variables
 select
     'append'           as __save_mode__
-            """
-            )
+            """)
         fm = FlinkTestClusterManager()
         if fm.is_not_started():
             fm.start_cluster()
         tf.test_run_etl(None, "/tmp/flink_func_test__test_run_etl.sql")
         self.assertTrue(fm.is_started())
         fm.stop_cluster()
 
         tf.test_run_etl(None, "/tmp/flink_func_test__test_run_etl.sql")
         self.assertTrue(fm.is_not_started())
 
     def test_run_etl_batch(self):
         fb = self.create_flink_backend()
         tf = TestFuncs(fb)
         with open("/tmp/flink_func_test__test_run_etl.sql", "w") as f:
-            f.write(
-                """
+            f.write("""
 -- backend: flink
 -- config: easy_sql.etl_type=batch
 -- config: flink.cmd=-pyexec python3
 -- config: flink.cmd=-t local
 -- config: flink.cmd=-pyclientexec python3
 -- target=variables
 select
     'append'           as __save_mode__
-            """
-            )
+            """)
         tf.test_run_etl(
             EasySqlConfig.from_sql(sql_file="/tmp/flink_func_test__test_run_etl.sql"),
             "/tmp/flink_func_test__test_run_etl.sql",
         )
```

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/funcs_itest.py` & `easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/funcs_itest.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import Optional, Tuple
 
 from easy_sql.base_test import TEST_CH_URL, TEST_PG_URL
 from easy_sql.local_spark import LocalSpark
 from easy_sql.sql_processor import FuncRunner, Step
 from easy_sql.sql_processor.backend import Partition, SparkTable
 from easy_sql.sql_processor.backend.base import Backend, Col
+from easy_sql.sql_processor.backend.flink import FlinkBackend
 from easy_sql.sql_processor.backend.rdb import RdbBackend
 from easy_sql.sql_processor.context import (
     ProcessorContext,
     TemplatesContext,
     VarsContext,
 )
 from easy_sql.sql_processor.funcs_common import (
@@ -203,7 +204,13 @@
         if os.path.exists(test_file_moved):
             os.remove(test_file_moved)
         with open(test_file, "w") as tmp_file:
             tmp_file.write("")
         f.move_file(test_file, test_file_moved)
         self.assertFalse(os.path.exists(test_file))
         self.assertTrue(os.path.exists(test_file_moved))
+
+
+def test_flink_func_set_config():
+    cf = FuncRunner.create(FlinkBackend()).run_func("set_config(a.b.c, 10 s)", VarsContext())
+    actural = cf.get("a.b.c", "666")
+    assert actural == "10 s"
```

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/funcs_rdb.py` & `easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/funcs_rdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,26 +180,26 @@
             columns_def = ", ".join([f"{col} {data_type_map[col_type]}" for col, col_type in output_dtypes])
             return f"""CREATE TABLE IF NOT EXISTS {output_table_name} ({columns_def}) engine = MergeTree
             PRIMARY KEY {id_col}
             ORDER BY {id_col}"""
         else:
             msg = (
                 "Backend of type"
-                f' {type(self.backend)}-{self.backend.backend_type if isinstance(self.backend, RdbBackend) else ""} is'
+                f" {type(self.backend)}-{self.backend.backend_type if isinstance(self.backend, RdbBackend) else ''} is"
                 " not supported yet"
             )
             raise Exception(msg)
 
 
 class PartitionFuncs(PartitionFuncsBase):
     def __check_backend(self):
         if not isinstance(self.backend, RdbBackend):
             msg = (
                 "Backend of type"
-                f' {type(self.backend)}-{self.backend.backend_type if isinstance(self.backend, RdbBackend) else ""} is'
+                f" {type(self.backend)}-{self.backend.backend_type if isinstance(self.backend, RdbBackend) else ''} is"
                 " not supported yet"
             )
             raise Exception(msg)
 
     def _get_bigquery_partition_values(self, table_name):
         db, table = self.__parse_table_name(table_name)
         sql = (
@@ -250,15 +250,15 @@
         elif backend.is_ch:
             return self._get_clickhouse_partition_values(table_name)
         elif backend.is_bq:
             return self._get_bigquery_partition_values(table_name)
         else:
             msg = (
                 "Backend of type"
-                f' {type(backend)}-{backend.backend_type if isinstance(backend, RdbBackend) else ""} is'
+                f" {type(backend)}-{backend.backend_type if isinstance(backend, RdbBackend) else ''} is"
                 " not supported yet"
             )
             raise Exception(msg)
 
     def get_partition_cols(self, table_name: str) -> List[str]:
         self.__check_backend()
         backend: RdbBackend = self.backend  # type: ignore
```

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/funcs_spark.py` & `easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/funcs_spark.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,21 +111,17 @@
         data: List[Row] = _data.collect()  # type: ignore
         data: List[Dict] = [row.asDict() for row in data]  # type: ignore
         os.makedirs(os.path.dirname(output_file), exist_ok=True)
         with open(output_file, "w") as f:
             f.write(json.dumps(data, ensure_ascii=False, indent=4, sort_keys=False))
 
     def update_json_local(self, context: ProcessorContext, vars: str, list_vars: str, json_attr: str, output_file: str):
-        vars_value = {
-            var.strip(): context.vars_context.vars.get(var.strip(), None) for var in vars.split(",") if var.strip()
-        }
+        vars_value = {var.strip(): context.vars_context.vars.get(var.strip()) for var in vars.split(",") if var.strip()}
         list_vars_value = {
-            var.strip(): context.vars_context.list_vars.get(var.strip(), None)
-            for var in list_vars.split(",")
-            if var.strip()
+            var.strip(): context.vars_context.list_vars.get(var.strip()) for var in list_vars.split(",") if var.strip()
         }
 
         data = {}
         if os.path.exists(output_file):
             with open(output_file, "r") as f:
                 data = json.loads(f.read())
```

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/report.py` & `easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/report.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,17 +40,15 @@
         verbose_parts = "\n" + f"sql: {self.step.select_sql}" if verbose else ""
         return f"""
 ===================== REPORT FOR {self.step.id} ==================
 config: {self.step.target_config} {verbose_parts}
 status: {self.status}
 start time: {start_time_str}, end time: {end_time_str}, execution time: {self.execution_time}s - {self.execution_time / total_execution_time * 100:.2f}%
 messages:
-""" + "\n".join(
-            self.messages
-        )
+""" + "\n".join(self.messages)
 
 
 class SqlProcessorReporter(ReportCollector):
     def __init__(
         self,
         report_task_id: str,
         report_hdfs_path: Optional[str] = None,
```

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/sql_processor.py` & `easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/sql_processor.py`

 * *Files identical despite different names*

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/step.py` & `easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/step.py`

 * *Files identical despite different names*

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/step_test.py` & `easy_sql_easy_sql-1.1.0/easy_sql/sql_processor/step_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,41 +31,37 @@
     def test_should_clean_sql(self):
         self.assertEquals(
             """
         with a as (select 1 as a) -- comment
         --comment
 select * from a
         """.strip(),
-            SqlCleaner().clean_sql(
-                """
+            SqlCleaner().clean_sql("""
         -- comment
         with a as (select 1 as a) -- comment
         --comment
         select * from a -- comment
         ;
         --comment
-        """
-            ),
+        """),
         )
 
     def test_should_clean_sql_with_semicolon_before_comment(self):
         self.assertEquals(
             """
         with a as (select 1 as a) -- comment
         --comment
 select * from a
         """.strip(),
-            SqlCleaner().clean_sql(
-                """
+            SqlCleaner().clean_sql("""
         -- comment
         with a as (select 1 as a) -- comment
         --comment
         select * from a; -- comment
         ;
         --comment
-        """
-            ),
+        """),
         )
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor_debugger.py` & `easy_sql_easy_sql-1.1.0/easy_sql/sql_processor_debugger.py`

 * *Files identical despite different names*

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor_debugger_itest.py` & `easy_sql_easy_sql-1.1.0/easy_sql/sql_processor_debugger_itest.py`

 * *Files identical despite different names*

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor_itest.py` & `easy_sql_easy_sql-1.1.0/easy_sql/sql_processor_itest.py`

 * *Files identical despite different names*

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor_test.py` & `easy_sql_easy_sql-1.1.0/easy_sql/sql_processor_test.py`

 * *Files identical despite different names*

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/sql_test.py` & `easy_sql_easy_sql-1.1.0/easy_sql/sql_test.py`

 * *Files identical despite different names*

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/sql_test_itest.py` & `easy_sql_easy_sql-1.1.0/easy_sql/sql_test_itest.py`

 * *Files identical despite different names*

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/sql_tester.py` & `easy_sql_easy_sql-1.1.0/easy_sql/sql_tester.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,16 +236,16 @@
                 backend_is_bigquery = self.backend == "bigquery"
                 if backend_is_bigquery or col_name == "data_date":
                     # for bigquery, partition column must be a date
                     return col_type, process_pt_val(date_converter, col_value)
                 else:
                     try:
                         # try convert partition column to int to remove possible float values
-                        return col_type, str(round(float(col_value))) if col_type == "string" else round(
-                            float(col_value)
+                        return col_type, (
+                            str(round(float(col_value))) if col_type == "string" else round(float(col_value))
                         )
                     except ValueError as e:
                         if col_type == "string":
                             return col_type, str(col_value)
                         else:
                             raise e
 
@@ -320,15 +320,15 @@
                 "outputs": [table_data.as_dict() for table_data in self.outputs],
             }
         )
         return data
 
     @staticmethod
     def from_dict(data: Dict) -> TestCase:
-        case = TestCase(data["sql_file_path"], data.get("sql_file_content", None))
+        case = TestCase(data["sql_file_path"], data.get("sql_file_content"))
         case.name = data["name"]
         case.vars = data["vars"]
         case.includes = data["includes"] if "includes" in data else {}
         case.inputs = [TableData.from_dict(table_data_dict) for table_data_dict in data["inputs"]]
         case.outputs = [TableData.from_dict(table_data_dict) for table_data_dict in data["outputs"]]
         case.udf_file_paths = data["udf_file_paths"] if "udf_file_paths" in data else []
         case.func_file_paths = data["func_file_paths"] if "func_file_paths" in data else []
@@ -476,15 +476,15 @@
                     column_types.append(table_column_types.get_col_type(table_name, columns[-1]))
                 else:
                     raise Exception(f"Unable to resolve types for table: {table_name}")
 
         values, value_descriptions = [], []
         for row_idx, cells in enumerate(rows[1:]):
             value_cells = cells[2:]
-            has_values = any([value_cells[i].value not in [None, ""] for i in range(len(columns))])
+            has_values = any(value_cells[i].value not in [None, ""] for i in range(len(columns)))
             if cells[1].value and str(cells[1].value).strip():
                 value_descriptions.append(str(cells[1].value).strip())
                 values.append(
                     self._parse_table_row_values(
                         wb, table_name, columns, row_idx, row_start_idx, value_cells, column_types, table_column_types
                     )
                 )
@@ -492,15 +492,15 @@
                 # If no description mentioned for this row, just ignore it.
                 # This ensures we must add description for a row, to clarify how the data comes.
                 if has_values:
                     raise AssertionError(
                         f"no description for table({table_name}) data at row {row_start_idx + 1 + row_idx + 1}"
                     )
             elif label == "OUTPUT":
-                has_values = any([value_cells[i].value not in [None, ""] for i in range(len(columns))])
+                has_values = any(value_cells[i].value not in [None, ""] for i in range(len(columns)))
                 if has_values:
                     values.append(
                         self._parse_table_row_values(
                             wb,
                             table_name,
                             columns,
                             row_idx,
@@ -676,15 +676,15 @@
 
     @property
     def failed_cases(self):
         return list(filter(lambda cr: cr["result"] == TestResult.FAILED, self.case_results))
 
     @property
     def is_fail(self) -> bool:
-        return any([r["result"] == TestResult.FAILED for r in self.case_results])
+        return any(r["result"] == TestResult.FAILED for r in self.case_results)
 
     @property
     def is_success(self) -> bool:
         return not self.is_fail
 
     @property
     def passed_cases(self):
@@ -959,18 +959,15 @@
         cases = self.parse_test_cases(test_data_file, self.table_column_types)
         py_file = os.path.join(
             os.path.dirname(test_data_file),
             os.path.basename(test_data_file).replace(".", "__").replace("__xlsx", "_test.py"),
         )
         import jinja2
 
-        env = jinja2.Environment(
-            loader=jinja2.DictLoader(
-                {
-                    "py_file_tpl": f"""import os
+        env = jinja2.Environment(loader=jinja2.DictLoader({"py_file_tpl": f"""import os
 import unittest
 import sys
 import importlib
 
 try:
     sys.path.insert(0, 'common')
     SqlTester = importlib.import_module('sql_test').SqlTester  # type: ignore
@@ -993,18 +990,15 @@
     def test_{{{{loop.index}}}}(self):
         # {{{{ case.name }}}}
         self.assertTrue(self.sql_tester.run_test(self.test_data_file, {{{{loop.index0}}}}).is_success)
 
 {{% endfor %}}
 if __name__ == '__main__':
     unittest.main()
-"""
-                }
-            )
-        )
+"""}))
         with open(py_file, "wb") as f:
             env.get_template("py_file_tpl").stream(cases=cases).dump(f, encoding="utf8")
             logger.info(f"created file: {py_file}")
 
 
 class SqlReader:
     def read_sql(self, test_data_file: str) -> str:
```

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/sql_tester_test.py` & `easy_sql_easy_sql-1.1.0/easy_sql/sql_tester_test.py`

 * *Files identical despite different names*

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/udf/udfs.py` & `easy_sql_easy_sql-1.1.0/easy_sql/udf/udfs.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,17 +94,15 @@
         return """
 CREATE EXTENSION IF NOT EXISTS pgcrypto with schema public;
 create or replace function sha1(value text) returns text
     as $$ select encode(public.digest($1::bytea, cast('sha1' as text)), 'hex') $$
     LANGUAGE SQL
     IMMUTABLE
     RETURNS NULL ON NULL INPUT
-""".split(
-            ";"
-        )
+""".split(";")
 
 
 class ChUdfs:
     """
     https://clickhouse.com/docs/en/sql-reference/statements/create/function
     CREATE FUNCTION name AS (parameter0, ...) -> expression
     """
```

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/udf/udfs_test.py` & `easy_sql_easy_sql-1.1.0/easy_sql/udf/udfs_test.py`

 * *Files identical despite different names*

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/utils/db_connection_utils.py` & `easy_sql_easy_sql-1.1.0/easy_sql/utils/db_connection_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,34 +6,26 @@
 
 if TYPE_CHECKING:
     from sqlalchemy.engine.base import Connection, Engine
 
     from easy_sql.sql_processor.backend.flink import FlinkBackend
 
 
-def _create_sqlalchemy_conn(flink_connector_config: Dict) -> Optional[Connection]:
-    if flink_connector_config and flink_connector_config["options"]["connector"] == "jdbc":
-        base_url = flink_connector_config["options"]["url"]
-        username = flink_connector_config["options"]["username"]
-        password = flink_connector_config["options"]["password"]
-        split_expr = "://"
-        split_expr_index = base_url.index(split_expr)
-        db_type = base_url[len("jdbc:") : split_expr_index]
-        sqlalchemy_db_url = f"{db_type}{split_expr}{username}:{password}@{KV.from_config(base_url, split_expr).v}"
-        if sqlalchemy_db_url:
-            from sqlalchemy import create_engine
-
-            engine: Engine = create_engine(sqlalchemy_db_url, isolation_level="AUTOCOMMIT", pool_size=1)
-            conn: Connection = engine.connect()
-            return conn
-
-
-def get_table_raw_conn_for_flink_backend(backend: FlinkBackend, table: str) -> Optional[Connection]:
-    _, _, connector = backend.get_table_config_and_connector(table)
-    return _create_sqlalchemy_conn(connector) if connector and table else None
-
-
-def get_connector_raw_conn_for_flink_backend(
-    backend: FlinkBackend, db_name: str, connector_name: str
-) -> Optional[Connection]:
-    connector = backend.get_db_connector(db_name, connector_name)
-    return _create_sqlalchemy_conn(connector) if connector else None
+def _create_sqlalchemy_conn(flink_connector_config: Dict[str, str]) -> Optional[Connection]:
+    base_url = flink_connector_config["'url'"].strip("'")
+    username = flink_connector_config["'username'"].strip("'")
+    password = flink_connector_config["'password'"].strip("'")
+    split_expr = "://"
+    split_expr_index = base_url.index(split_expr)
+    db_type = base_url[len("jdbc:") : split_expr_index]
+    sqlalchemy_db_url = f"{db_type}{split_expr}{username}:{password}@{KV.from_config(base_url, split_expr).v}"
+    if sqlalchemy_db_url:
+        from sqlalchemy import create_engine
+
+        engine: Engine = create_engine(sqlalchemy_db_url, isolation_level="AUTOCOMMIT", pool_size=1)
+        conn: Connection = engine.connect()
+        return conn
+
+
+def get_connector_raw_conn_for_flink_backend(backend: FlinkBackend, connector_name: str) -> Optional[Connection]:
+    connector_options = backend.flink_tables_config.get_connector_options(connector_name)
+    return _create_sqlalchemy_conn(connector_options)
```

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/utils/flink_test_cluster.py` & `easy_sql_easy_sql-1.1.0/easy_sql/utils/flink_test_cluster.py`

 * *Files identical despite different names*

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/utils/io_utils.py` & `easy_sql_easy_sql-1.1.0/easy_sql/utils/io_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         elif path.exists(path.basename(file_path)):
             file_path = path.basename(file_path)
         elif relative_to and path.isfile(relative_to) and path.exists(path.join(path.dirname(relative_to), file_path)):
             file_path = path.join(path.dirname(relative_to), file_path)
         elif relative_to and path.isdir(relative_to) and path.exists(path.join(relative_to, file_path)):
             path.join(relative_to, file_path)
         else:
-            raise Exception(f"file not found: {file_path}")
+            raise Exception(f"file not found: {file_path}, curdir: {base_path}")
     if abs_path:
         file_path = path.abspath(file_path)
     if " " in file_path:
         parts = file_path.split("/")
         file_path_no_space = "/".join([re.sub(r" .*$", "", part) for part in parts])
         logger.warn(
             "Remove space inside file path, since spark will raise issue with space in path. "
```

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/utils/kv.py` & `easy_sql_easy_sql-1.1.0/easy_sql/utils/kv.py`

 * *Files identical despite different names*

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/utils/object_utils_test.py` & `easy_sql_easy_sql-1.1.0/easy_sql/utils/object_utils_test.py`

 * *Files identical despite different names*

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/utils/sql_expr.py` & `easy_sql_easy_sql-1.1.0/easy_sql/utils/sql_expr.py`

 * *Files identical despite different names*

### Comparing `easy_sql_easy_sql-1.0.0/easy_sql/utils/sql_expr_test.py` & `easy_sql_easy_sql-1.1.0/easy_sql/utils/sql_expr_test.py`

 * *Files identical despite different names*

### Comparing `easy_sql_easy_sql-1.0.0/pyproject.toml` & `easy_sql_easy_sql-1.1.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "easy_sql-easy_sql"
-version = "1.0.0"
+version = "1.1.0"
 description = "A library developed to ease the data ETL development process."
 authors = ["Easy SQL from Thoughtworks <easy_sql@thoughtworks.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/easysql/easy_sql"
 homepage = "https://easy-sql.readthedocs.io"
 
@@ -29,44 +29,57 @@
 sqlfluff = {version = "~1.4.5", optional = true}
 SQLAlchemy = {version = "^1.4.40", optional = true}
 clickhouse-driver = {version = "^0.2.4", optional = true}
 clickhouse-sqlalchemy = {version = "^0.2.1", optional = true}
 psycopg2 = {version = "^2.9.3", optional = true}
 pyodps = {version = "^0.11.2.1", optional = true}
 pyspark = [{version = ">=2.3.0, != 3.1.1, != 3.1.2, != 3.1.3, !=3.2.0, != 3.2.1", optional = true}]
+numpy = {version="~1.21.4", python=">=3.7,<3.11", optional=true}
+pandas = {version="~1.3", python=">=3.7.1", optional=true}
+apache-flink = {version = "^1.17.0", optional = true}
+ydata-profiling = {version = "^4.2.0", optional = true, python = ">=3.8,<3.12"}
+pyyaml = {version = "^6.0", optional = true}
+pymongo = "^3.8.0"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.test.dependencies]
 pytest = "^7.1.2"
-pymongo = "^3.8.0"
 coverage = "^6.4.3"
-pre-commit = "^2.20.0"
-flake8 = "^5.0.4"
-flake8-bugbear = "^22.7.1"
-flake8-comprehensions = "^3.10.0"
-flake8-simplify = "^0.19.3"
-flake8-type-checking = { version = "^2.1.2", python = "^3.8" }
 openpyxl = "^3.0.10"
 
+[tool.poetry.group.dev.dependencies]
+pre-commit = "^2.20.0"
+flake8 = {version = "^6.0.0", python = ">=3.8.1"}
+flake8-bugbear = {version = "^23.5.9", python = ">=3.8.1"}
+flake8-comprehensions = "^3.12.0"
+flake8-simplify = "^0.20.0"
+flake8-type-checking = {version = "^2.4.0", python = ">=3.8"}
+
 [tool.poetry.extras]
 cli = ["click"]
 linter = ["sqlfluff","colorlog","regex"]
 spark = ["pyspark"]
 pg = ["SQLAlchemy", "psycopg2"]
 clickhouse = ["SQLAlchemy","clickhouse-driver","clickhouse-sqlalchemy"]
 maxcompute = ["pyodps"]
+flink = ["apache-flink", "pyyaml"]
+ydata-profiling=["ydata-profiling"]
 
 [tool.isort]
 profile = "black"
 src_paths = ["easy_sql"]
 
 [tool.black]
 line-length = 120
 preview = true
 
 [tool.pytest.ini_options]
 testpaths = [
     "easy_sql",
 ]
+python_files = [
+    "*_itest.py",
+    "*_test.py",
+]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `easy_sql_easy_sql-1.0.0/PKG-INFO` & `easy_sql_easy_sql-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-sql-easy-sql
-Version: 1.0.0
+Version: 1.1.0
 Summary: A library developed to ease the data ETL development process.
 Home-page: https://easy-sql.readthedocs.io
 License: Apache-2.0
 Author: Easy SQL from Thoughtworks
 Author-email: easy_sql@thoughtworks.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,31 +12,38 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
 Provides-Extra: cli
 Provides-Extra: clickhouse
+Provides-Extra: flink
 Provides-Extra: linter
 Provides-Extra: maxcompute
 Provides-Extra: pg
 Provides-Extra: spark
+Provides-Extra: ydata-profiling
 Requires-Dist: SQLAlchemy (>=1.4.40,<2.0.0) ; extra == "pg" or extra == "clickhouse"
+Requires-Dist: apache-flink (>=1.17.0,<2.0.0) ; extra == "flink"
 Requires-Dist: click (>=8.1.3,<9.0.0) ; extra == "cli"
 Requires-Dist: clickhouse-driver (>=0.2.4,<0.3.0) ; extra == "clickhouse"
 Requires-Dist: clickhouse-sqlalchemy (>=0.2.1,<0.3.0) ; extra == "clickhouse"
 Requires-Dist: colorlog (>=6.6.0,<7.0.0) ; extra == "linter"
+Requires-Dist: numpy (>=1.21.4,<1.22.0) ; python_version >= "3.7" and python_version < "3.11"
+Requires-Dist: pandas (>=1.3,<1.4) ; python_full_version >= "3.7.1"
 Requires-Dist: psycopg2 (>=2.9.3,<3.0.0) ; extra == "pg"
+Requires-Dist: pymongo (>=3.8.0,<4.0.0)
 Requires-Dist: pyodps (>=0.11.2.1,<0.12.0.0) ; extra == "maxcompute"
 Requires-Dist: pyspark (>=2.3.0,!=3.1.1,!=3.1.2,!=3.1.3,!=3.2.0,!=3.2.1) ; extra == "spark"
+Requires-Dist: pyyaml (>=6.0,<7.0) ; extra == "flink"
 Requires-Dist: regex (>=2022.7.25,<2023.0.0) ; extra == "linter"
 Requires-Dist: sqlfluff (>=1.4.5,<1.5.0) ; extra == "linter"
+Requires-Dist: ydata-profiling (>=4.2.0,<5.0.0) ; (python_version >= "3.8" and python_version < "3.12") and (extra == "ydata-profiling")
 Project-URL: Bug Tracker, https://github.com/easysql/easy_sql/issues
 Project-URL: Repository, https://github.com/easysql/easy_sql
 Description-Content-Type: text/markdown
 
 # Easy SQL
 
 Easy SQL is built to ease the data ETL development process.
@@ -194,15 +201,15 @@
 mkdir -pv test/flink/jars
 wget -P test/flink/jars https://repo1.maven.org/maven2/org/apache/flink/flink-connector-jdbc/1.15.1/flink-connector-jdbc-1.15.1.jar
 wget -P test/flink/jars https://repo1.maven.org/maven2/org/postgresql/postgresql/42.2.14/postgresql-42.2.14.jar
 ```
 
 Create a file named `sample_etl.flink.postgres.sql` with content as the test file [here](https://github.com/easysql/easy_sql/blob/main/test/sample_etl.flink.postgres.sql).
 
-Create a connector configuration file named `sample_etl.flink_tables_file.json` with content as the test configuration file [here](https://github.com/easysql/easy_sql/blob/main/test/sample_etl.flink_tables_file.json).
+Create a connector configuration file named `sample_etl.flink_tables_file.yml` with content as the test configuration file [here](https://github.com/easysql/easy_sql/blob/main/test/sample_etl.flink_tables_file.yml).
 
 Run it with command:
 
 ```bash
 bash -c "$(python3 -m easy_sql.data_process -f sample_etl.flink.postgres.sql -p)"
 ```
```

