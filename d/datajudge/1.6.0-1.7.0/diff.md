# Comparing `tmp/datajudge-1.6.0.tar.gz` & `tmp/datajudge-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datajudge-1.6.0.tar", last modified: Wed Apr 12 11:25:40 2023, max compression
+gzip compressed data, was "datajudge-1.7.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `datajudge-1.6.0.tar` & `datajudge-1.7.0.tar`

### file list

```diff
@@ -1,71 +1,74 @@
--rw-r--r--   0        0        0      378 2023-04-12 11:24:00.433271 datajudge-1.6.0/.flake8
--rw-r--r--   0        0        0      154 2023-04-12 11:24:00.433271 datajudge-1.6.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1388 2023-04-12 11:24:00.433271 datajudge-1.6.0/.github/workflows/build_and_publish.yaml
--rw-r--r--   0        0        0    17607 2023-04-12 11:24:00.433271 datajudge-1.6.0/.github/workflows/ci.yaml
--rw-r--r--   0        0        0     2962 2023-04-12 11:24:00.433271 datajudge-1.6.0/.github/workflows/codeql.yml
--rw-r--r--   0        0        0     1437 2023-04-12 11:24:00.433271 datajudge-1.6.0/.github/workflows/pre-commit-autoupdate.yml
--rw-r--r--   0        0        0     1311 2023-04-12 11:24:00.433271 datajudge-1.6.0/.gitignore
--rw-r--r--   0        0        0      958 2023-04-12 11:24:00.437271 datajudge-1.6.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      268 2023-04-12 11:24:00.437271 datajudge-1.6.0/.readthedocs.yml
--rw-r--r--   0        0        0     2866 2023-04-12 11:24:00.437271 datajudge-1.6.0/CHANGELOG.rst
--rw-r--r--   0        0        0     1515 2023-04-12 11:24:00.437271 datajudge-1.6.0/LICENSE
--rw-r--r--   0        0        0     1600 2023-04-12 11:24:00.437271 datajudge-1.6.0/README.md
--rw-r--r--   0        0        0       32 2023-04-12 11:24:00.437271 datajudge-1.6.0/_typos.toml
--rw-r--r--   0        0        0       84 2023-04-12 11:24:00.437271 datajudge-1.6.0/codecov.yml
--rw-r--r--   0        0        0     1241 2023-04-12 11:24:00.437271 datajudge-1.6.0/docker-compose.yaml
--rw-r--r--   0        0        0      638 2023-04-12 11:24:00.437271 datajudge-1.6.0/docs/Makefile
--rw-r--r--   0        0        0      764 2023-04-12 11:24:00.437271 datajudge-1.6.0/docs/make.bat
--rw-r--r--   0        0        0      905 2023-04-12 11:24:00.437271 datajudge-1.6.0/docs/source/conf.py
--rw-r--r--   0        0        0      983 2023-04-12 11:24:00.437271 datajudge-1.6.0/docs/source/development.rst
--rw-r--r--   0        0        0     5146 2023-04-12 11:24:00.437271 datajudge-1.6.0/docs/source/examples/example.rst
--rw-r--r--   0        0        0     6419 2023-04-12 11:24:00.437271 datajudge-1.6.0/docs/source/examples/example_dates.rst
--rw-r--r--   0        0        0     8642 2023-04-12 11:24:00.437271 datajudge-1.6.0/docs/source/examples/example_exploration.rst
--rw-r--r--   0        0        0    12556 2023-04-12 11:24:00.437271 datajudge-1.6.0/docs/source/examples/example_twitch.rst
--rw-r--r--   0        0        0      194 2023-04-12 11:24:00.437271 datajudge-1.6.0/docs/source/examples/examples.rst
--rw-r--r--   0        0        0     1381 2023-04-12 11:24:00.437271 datajudge-1.6.0/docs/source/examples/twitch_process.py
--rw-r--r--   0        0        0    17481 2023-04-12 11:24:00.437271 datajudge-1.6.0/docs/source/examples/twitch_report.html
--rw-r--r--   0        0        0     2663 2023-04-12 11:24:00.437271 datajudge-1.6.0/docs/source/examples/twitch_specification.py
--rw-r--r--   0        0        0      573 2023-04-12 11:24:00.437271 datajudge-1.6.0/docs/source/examples/twitch_upload.py
--rw-r--r--   0        0        0    70396 2023-04-12 11:24:00.437271 datajudge-1.6.0/docs/source/examples/twitch_version1.csv
--rw-r--r--   0        0        0    82951 2023-04-12 11:24:00.437271 datajudge-1.6.0/docs/source/examples/twitch_version2.csv
--rw-r--r--   0        0        0    78962 2023-04-12 11:24:00.437271 datajudge-1.6.0/docs/source/examples/twitchdata.csv
--rw-r--r--   0        0        0     8452 2023-04-12 11:24:00.437271 datajudge-1.6.0/docs/source/getting_started.rst
--rw-r--r--   0        0        0      543 2023-04-12 11:24:00.437271 datajudge-1.6.0/docs/source/index.rst
--rw-r--r--   0        0        0      155 2023-04-12 11:24:00.437271 datajudge-1.6.0/docs/source/installation.rst
--rw-r--r--   0        0        0     1527 2023-04-12 11:24:00.437271 datajudge-1.6.0/docs/source/motivation.rst
--rw-r--r--   0        0        0    51601 2023-04-12 11:24:00.437271 datajudge-1.6.0/docs/source/report_failing_query1.png
--rw-r--r--   0        0        0   163420 2023-04-12 11:24:00.441271 datajudge-1.6.0/docs/source/report_failing_query2.png
--rw-r--r--   0        0        0    11178 2023-04-12 11:24:00.441271 datajudge-1.6.0/docs/source/testing.rst
--rw-r--r--   0        0        0      445 2023-04-12 11:24:00.441271 datajudge-1.6.0/environment.yml
--rw-r--r--   0        0        0     1168 2023-04-12 11:24:00.441271 datajudge-1.6.0/pyproject.toml
--rw-r--r--   0        0        0      510 2023-04-12 11:24:00.441271 datajudge-1.6.0/src/datajudge/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 11:24:00.441271 datajudge-1.6.0/src/datajudge/constraints/__init__.py
--rw-r--r--   0        0        0     8560 2023-04-12 11:24:00.441271 datajudge-1.6.0/src/datajudge/constraints/base.py
--rw-r--r--   0        0        0     3437 2023-04-12 11:24:00.441271 datajudge-1.6.0/src/datajudge/constraints/column.py
--rw-r--r--   0        0        0    11708 2023-04-12 11:24:00.441271 datajudge-1.6.0/src/datajudge/constraints/date.py
--rw-r--r--   0        0        0     1788 2023-04-12 11:24:00.441271 datajudge-1.6.0/src/datajudge/constraints/groupby.py
--rw-r--r--   0        0        0     6427 2023-04-12 11:24:00.441271 datajudge-1.6.0/src/datajudge/constraints/miscs.py
--rw-r--r--   0        0        0     6075 2023-04-12 11:24:00.441271 datajudge-1.6.0/src/datajudge/constraints/nrows.py
--rw-r--r--   0        0        0     8260 2023-04-12 11:24:00.441271 datajudge-1.6.0/src/datajudge/constraints/numeric.py
--rw-r--r--   0        0        0     7220 2023-04-12 11:24:00.441271 datajudge-1.6.0/src/datajudge/constraints/row.py
--rw-r--r--   0        0        0     4532 2023-04-12 11:24:00.441271 datajudge-1.6.0/src/datajudge/constraints/stats.py
--rw-r--r--   0        0        0    11350 2023-04-12 11:24:00.441271 datajudge-1.6.0/src/datajudge/constraints/uniques.py
--rw-r--r--   0        0        0     7384 2023-04-12 11:24:00.441271 datajudge-1.6.0/src/datajudge/constraints/varchar.py
--rw-r--r--   0        0        0    42690 2023-04-12 11:24:00.441271 datajudge-1.6.0/src/datajudge/db_access.py
--rw-r--r--   0        0        0     1019 2023-04-12 11:24:00.441271 datajudge-1.6.0/src/datajudge/pytest_integration.py
--rw-r--r--   0        0        0    62220 2023-04-12 11:24:00.441271 datajudge-1.6.0/src/datajudge/requirements.py
--rwxr-xr-x   0        0        0      173 2023-04-12 11:24:00.441271 datajudge-1.6.0/start_db2.sh
--rwxr-xr-x   0        0        0      522 2023-04-12 11:24:00.441271 datajudge-1.6.0/start_mssql.sh
--rwxr-xr-x   0        0        0      140 2023-04-12 11:24:00.441271 datajudge-1.6.0/start_postgres.sh
--rw-r--r--   0        0        0        0 2023-04-12 11:24:00.441271 datajudge-1.6.0/tests/integration/__init__.py
--rw-r--r--   0        0        0    27552 2023-04-12 11:24:00.441271 datajudge-1.6.0/tests/integration/conftest.py
--rw-r--r--   0        0        0     2848 2023-04-12 11:24:00.441271 datajudge-1.6.0/tests/integration/test_column_capitalization.py
--rw-r--r--   0        0        0     6795 2023-04-12 11:24:00.441271 datajudge-1.6.0/tests/integration/test_data_source.py
--rw-r--r--   0        0        0    71469 2023-04-12 11:24:00.441271 datajudge-1.6.0/tests/integration/test_integration.py
--rw-r--r--   0        0        0     2520 2023-04-12 11:24:00.441271 datajudge-1.6.0/tests/integration/test_stats.py
--rw-r--r--   0        0        0     2216 2023-04-12 11:24:00.441271 datajudge-1.6.0/tests/unit/test_condition.py
--rw-r--r--   0        0        0      726 2023-04-12 11:24:00.441271 datajudge-1.6.0/tests/unit/test_db_access.py
--rw-r--r--   0        0        0      856 2023-04-12 11:24:00.441271 datajudge-1.6.0/tests/unit/test_percentiles.py
--rw-r--r--   0        0        0     2208 2023-04-12 11:24:00.441271 datajudge-1.6.0/tests/unit/test_pytest.py
--rw-r--r--   0        0        0     1763 2023-04-12 11:24:00.441271 datajudge-1.6.0/tests/unit/test_set_functions.py
--rw-r--r--   0        0        0     2360 1970-01-01 00:00:00.000000 datajudge-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0      378 2023-06-02 14:28:48.383106 datajudge-1.7.0/.flake8
+-rw-r--r--   0        0        0      238 2023-06-02 14:28:48.383106 datajudge-1.7.0/.github/.pull_request_template.md
+-rw-r--r--   0        0        0      823 2023-06-02 14:28:48.383106 datajudge-1.7.0/.github/actions/pytest/action.yml
+-rw-r--r--   0        0        0      154 2023-06-02 14:28:48.383106 datajudge-1.7.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1275 2023-06-02 14:28:48.383106 datajudge-1.7.0/.github/workflows/build_and_publish.yaml
+-rw-r--r--   0        0        0    11535 2023-06-02 14:28:48.383106 datajudge-1.7.0/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0     2962 2023-06-02 14:28:48.383106 datajudge-1.7.0/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0     1369 2023-06-02 14:28:48.383106 datajudge-1.7.0/.github/workflows/pre-commit-autoupdate.yml
+-rw-r--r--   0        0        0     1311 2023-06-02 14:28:48.383106 datajudge-1.7.0/.gitignore
+-rw-r--r--   0        0        0      958 2023-06-02 14:28:48.383106 datajudge-1.7.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      268 2023-06-02 14:28:48.383106 datajudge-1.7.0/.readthedocs.yml
+-rw-r--r--   0        0        0     3355 2023-06-02 14:28:48.383106 datajudge-1.7.0/CHANGELOG.rst
+-rw-r--r--   0        0        0     1515 2023-06-02 14:28:48.383106 datajudge-1.7.0/LICENSE
+-rw-r--r--   0        0        0     1600 2023-06-02 14:28:48.383106 datajudge-1.7.0/README.md
+-rw-r--r--   0        0        0       32 2023-06-02 14:28:48.383106 datajudge-1.7.0/_typos.toml
+-rw-r--r--   0        0        0       84 2023-06-02 14:28:48.383106 datajudge-1.7.0/codecov.yml
+-rw-r--r--   0        0        0     1241 2023-06-02 14:28:48.383106 datajudge-1.7.0/docker-compose.yaml
+-rw-r--r--   0        0        0      638 2023-06-02 14:28:48.383106 datajudge-1.7.0/docs/Makefile
+-rw-r--r--   0        0        0      764 2023-06-02 14:28:48.383106 datajudge-1.7.0/docs/make.bat
+-rw-r--r--   0        0        0      905 2023-06-02 14:28:48.383106 datajudge-1.7.0/docs/source/conf.py
+-rw-r--r--   0        0        0     1168 2023-06-02 14:28:48.383106 datajudge-1.7.0/docs/source/development.rst
+-rw-r--r--   0        0        0     5146 2023-06-02 14:28:48.383106 datajudge-1.7.0/docs/source/examples/example.rst
+-rw-r--r--   0        0        0     6419 2023-06-02 14:28:48.383106 datajudge-1.7.0/docs/source/examples/example_dates.rst
+-rw-r--r--   0        0        0     8642 2023-06-02 14:28:48.383106 datajudge-1.7.0/docs/source/examples/example_exploration.rst
+-rw-r--r--   0        0        0    12556 2023-06-02 14:28:48.383106 datajudge-1.7.0/docs/source/examples/example_twitch.rst
+-rw-r--r--   0        0        0      194 2023-06-02 14:28:48.383106 datajudge-1.7.0/docs/source/examples/examples.rst
+-rw-r--r--   0        0        0     1381 2023-06-02 14:28:48.383106 datajudge-1.7.0/docs/source/examples/twitch_process.py
+-rw-r--r--   0        0        0    17481 2023-06-02 14:28:48.383106 datajudge-1.7.0/docs/source/examples/twitch_report.html
+-rw-r--r--   0        0        0     2663 2023-06-02 14:28:48.383106 datajudge-1.7.0/docs/source/examples/twitch_specification.py
+-rw-r--r--   0        0        0      573 2023-06-02 14:28:48.383106 datajudge-1.7.0/docs/source/examples/twitch_upload.py
+-rw-r--r--   0        0        0    70396 2023-06-02 14:28:48.383106 datajudge-1.7.0/docs/source/examples/twitch_version1.csv
+-rw-r--r--   0        0        0    82951 2023-06-02 14:28:48.383106 datajudge-1.7.0/docs/source/examples/twitch_version2.csv
+-rw-r--r--   0        0        0    78962 2023-06-02 14:28:48.383106 datajudge-1.7.0/docs/source/examples/twitchdata.csv
+-rw-r--r--   0        0        0     8452 2023-06-02 14:28:48.383106 datajudge-1.7.0/docs/source/getting_started.rst
+-rw-r--r--   0        0        0      543 2023-06-02 14:28:48.383106 datajudge-1.7.0/docs/source/index.rst
+-rw-r--r--   0        0        0      155 2023-06-02 14:28:48.383106 datajudge-1.7.0/docs/source/installation.rst
+-rw-r--r--   0        0        0     1527 2023-06-02 14:28:48.383106 datajudge-1.7.0/docs/source/motivation.rst
+-rw-r--r--   0        0        0    51601 2023-06-02 14:28:48.383106 datajudge-1.7.0/docs/source/report_failing_query1.png
+-rw-r--r--   0        0        0   163420 2023-06-02 14:28:48.387106 datajudge-1.7.0/docs/source/report_failing_query2.png
+-rw-r--r--   0        0        0    11178 2023-06-02 14:28:48.387106 datajudge-1.7.0/docs/source/testing.rst
+-rw-r--r--   0        0        0      329 2023-06-02 14:28:48.387106 datajudge-1.7.0/environment.yml
+-rw-r--r--   0        0        0     1168 2023-06-02 14:28:48.387106 datajudge-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0      510 2023-06-02 14:28:48.387106 datajudge-1.7.0/src/datajudge/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-02 14:28:48.387106 datajudge-1.7.0/src/datajudge/constraints/__init__.py
+-rw-r--r--   0        0        0     8560 2023-06-02 14:28:48.387106 datajudge-1.7.0/src/datajudge/constraints/base.py
+-rw-r--r--   0        0        0     4636 2023-06-02 14:28:48.387106 datajudge-1.7.0/src/datajudge/constraints/column.py
+-rw-r--r--   0        0        0     8603 2023-06-02 14:28:48.387106 datajudge-1.7.0/src/datajudge/constraints/date.py
+-rw-r--r--   0        0        0     1788 2023-06-02 14:28:48.387106 datajudge-1.7.0/src/datajudge/constraints/groupby.py
+-rw-r--r--   0        0        0     4202 2023-06-02 14:28:48.387106 datajudge-1.7.0/src/datajudge/constraints/interval.py
+-rw-r--r--   0        0        0     6427 2023-06-02 14:28:48.387106 datajudge-1.7.0/src/datajudge/constraints/miscs.py
+-rw-r--r--   0        0        0     6075 2023-06-02 14:28:48.387106 datajudge-1.7.0/src/datajudge/constraints/nrows.py
+-rw-r--r--   0        0        0    10449 2023-06-02 14:28:48.387106 datajudge-1.7.0/src/datajudge/constraints/numeric.py
+-rw-r--r--   0        0        0     7220 2023-06-02 14:28:48.387106 datajudge-1.7.0/src/datajudge/constraints/row.py
+-rw-r--r--   0        0        0     4532 2023-06-02 14:28:48.387106 datajudge-1.7.0/src/datajudge/constraints/stats.py
+-rw-r--r--   0        0        0    15216 2023-06-02 14:28:48.387106 datajudge-1.7.0/src/datajudge/constraints/uniques.py
+-rw-r--r--   0        0        0     7384 2023-06-02 14:28:48.387106 datajudge-1.7.0/src/datajudge/constraints/varchar.py
+-rw-r--r--   0        0        0    43806 2023-06-02 14:28:48.387106 datajudge-1.7.0/src/datajudge/db_access.py
+-rw-r--r--   0        0        0     1019 2023-06-02 14:28:48.387106 datajudge-1.7.0/src/datajudge/pytest_integration.py
+-rw-r--r--   0        0        0    71257 2023-06-02 14:28:48.387106 datajudge-1.7.0/src/datajudge/requirements.py
+-rwxr-xr-x   0        0        0      173 2023-06-02 14:28:48.387106 datajudge-1.7.0/start_db2.sh
+-rwxr-xr-x   0        0        0      522 2023-06-02 14:28:48.387106 datajudge-1.7.0/start_mssql.sh
+-rwxr-xr-x   0        0        0      140 2023-06-02 14:28:48.387106 datajudge-1.7.0/start_postgres.sh
+-rw-r--r--   0        0        0        0 2023-06-02 14:28:48.387106 datajudge-1.7.0/tests/integration/__init__.py
+-rw-r--r--   0        0        0    32592 2023-06-02 14:28:48.387106 datajudge-1.7.0/tests/integration/conftest.py
+-rw-r--r--   0        0        0     2848 2023-06-02 14:28:48.387106 datajudge-1.7.0/tests/integration/test_column_capitalization.py
+-rw-r--r--   0        0        0     6795 2023-06-02 14:28:48.387106 datajudge-1.7.0/tests/integration/test_data_source.py
+-rw-r--r--   0        0        0    76755 2023-06-02 14:28:48.387106 datajudge-1.7.0/tests/integration/test_integration.py
+-rw-r--r--   0        0        0     2520 2023-06-02 14:28:48.387106 datajudge-1.7.0/tests/integration/test_stats.py
+-rw-r--r--   0        0        0     2216 2023-06-02 14:28:48.387106 datajudge-1.7.0/tests/unit/test_condition.py
+-rw-r--r--   0        0        0      726 2023-06-02 14:28:48.387106 datajudge-1.7.0/tests/unit/test_db_access.py
+-rw-r--r--   0        0        0      856 2023-06-02 14:28:48.387106 datajudge-1.7.0/tests/unit/test_percentiles.py
+-rw-r--r--   0        0        0     2208 2023-06-02 14:28:48.387106 datajudge-1.7.0/tests/unit/test_pytest.py
+-rw-r--r--   0        0        0     1763 2023-06-02 14:28:48.387106 datajudge-1.7.0/tests/unit/test_set_functions.py
+-rw-r--r--   0        0        0     2360 1970-01-01 00:00:00.000000 datajudge-1.7.0/PKG-INFO
```

### Comparing `datajudge-1.6.0/.github/workflows/build_and_publish.yaml` & `datajudge-1.7.0/.github/workflows/build_and_publish.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -17,21 +17,17 @@
     strategy:
       fail-fast: true
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
-      - uses: conda-incubator/setup-miniconda@v2
+      - uses: mamba-org/setup-micromamba@5d5dbebd87f7b9358c403c7a66651fa92b310105
         with:
-          miniforge-variant: Mambaforge
-          miniforge-version: 4.11.0-2
-          use-mamba: true
           environment-file: environment.yml
-          activate-environment: datajudge
 
       - name: Build
         shell: bash -l {0}
         # It seems as though flit publish expects a .pypirc file as compared to
         # only a token passed as an argument.
         # See https://flit.pypa.io/en/latest/cmdline.html#flit-publish
         run: |
@@ -48,11 +44,11 @@
     if: github.event_name == 'release' && github.event.action == 'published'
     steps:
       - uses: actions/download-artifact@v3
         with:
           name: artifact
           path: dist
 
-      - uses: pypa/gh-action-pypi-publish@v1.8.5
+      - uses: pypa/gh-action-pypi-publish@v1.8.6
         with:
           user: __token__
           password: ${{ secrets.PYPI_TOKEN }}
```

### Comparing `datajudge-1.6.0/.github/workflows/codeql.yml` & `datajudge-1.7.0/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `datajudge-1.6.0/.gitignore` & `datajudge-1.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `datajudge-1.6.0/.pre-commit-config.yaml` & `datajudge-1.7.0/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -12,20 +12,20 @@
       - id: flake8-conda
   - repo: https://github.com/Quantco/pre-commit-mirrors-isort
     rev: 5.12.0
     hooks:
       - id: isort-conda
         additional_dependencies: [-c, conda-forge, toml=0.10.2]
   - repo: https://github.com/Quantco/pre-commit-mirrors-mypy
-    rev: "1.1.1"
+    rev: "1.2.0"
     hooks:
       - id: mypy-conda
         additional_dependencies: [-c, conda-forge, types-setuptools]
   - repo: https://github.com/Quantco/pre-commit-mirrors-pyupgrade
-    rev: 3.3.1
+    rev: 3.3.2
     hooks:
       - id: pyupgrade-conda
         args:
           - --py38-plus
   - repo: https://github.com/Quantco/pre-commit-mirrors-typos
     rev: 1.13.20
     hooks:
```

### Comparing `datajudge-1.6.0/CHANGELOG.rst` & `datajudge-1.7.0/CHANGELOG.rst`

 * *Files 21% similar despite different names*

```diff
@@ -3,14 +3,22 @@
    * Update the major if you break the public API
    * Update the minor if you add new functionality
    * Update the patch if you fixed a bug
 
 Changelog
 =========
 
+1.7.0 - 2023.05.11
+------------------
+
+**New features**
+
+- Implement :meth:`datajudge.WithinRequirement.add_value_distribution_constraint`.
+- Extended :meth:`datajudge.WithinRequirement.add_column_type_constraint` to support column type specification using string format, backend-specific SQLAlchemy types, and SQLAlchemy's generic types.
+- Implement :meth:`datajudge.WithinRequirement.add_numeric_no_gap_constraint`, :meth:`datajudge.WithinRequirement.add_numeric_no_overlap_constraint`,
 
 1.6.0 - 2022.04.12
 ------------------
 
 **Other changes**
 
 - Ensure compatibility with ``sqlalchemy`` >= 2.0.
```

### Comparing `datajudge-1.6.0/LICENSE` & `datajudge-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datajudge-1.6.0/README.md` & `datajudge-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `datajudge-1.6.0/docker-compose.yaml` & `datajudge-1.7.0/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `datajudge-1.6.0/docs/Makefile` & `datajudge-1.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `datajudge-1.6.0/docs/make.bat` & `datajudge-1.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `datajudge-1.6.0/docs/source/conf.py` & `datajudge-1.7.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.6.0/docs/source/development.rst` & `datajudge-1.7.0/docs/source/development.rst`

 * *Files 26% similar despite different names*

```diff
@@ -15,22 +15,25 @@
 
 ::
 
    pytest tests/unit
 
 Integration tests are run against a specific backend at a time. As of now, we provide helper
 scripts to spin up either a Postgres or MSSQL backend.
+Our ``environment.yml`` does not include the necessary dependencies for these backends, so you will need to install them manually.
+
 
 To run integration tests against Postgres, first start a docker container with a Postgres database:
 
 ::
 
    ./start_postgres.sh
 
-Once this is running, you may execute integration tests as follows:
+In your current environment, install the ``psycopg2`` package.
+After this, you may execute integration tests as follows:
 
 ::
 
    pytest tests/integration --backend=postgres
 
 Analogously, for MSSQL, run
```

### Comparing `datajudge-1.6.0/docs/source/examples/example.rst` & `datajudge-1.7.0/docs/source/examples/example.rst`

 * *Files identical despite different names*

### Comparing `datajudge-1.6.0/docs/source/examples/example_dates.rst` & `datajudge-1.7.0/docs/source/examples/example_dates.rst`

 * *Files identical despite different names*

### Comparing `datajudge-1.6.0/docs/source/examples/example_exploration.rst` & `datajudge-1.7.0/docs/source/examples/example_exploration.rst`

 * *Files identical despite different names*

### Comparing `datajudge-1.6.0/docs/source/examples/example_twitch.rst` & `datajudge-1.7.0/docs/source/examples/example_twitch.rst`

 * *Files identical despite different names*

### Comparing `datajudge-1.6.0/docs/source/examples/twitch_process.py` & `datajudge-1.7.0/docs/source/examples/twitch_process.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.6.0/docs/source/examples/twitch_report.html` & `datajudge-1.7.0/docs/source/examples/twitch_report.html`

 * *Files identical despite different names*

### Comparing `datajudge-1.6.0/docs/source/examples/twitch_specification.py` & `datajudge-1.7.0/docs/source/examples/twitch_specification.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.6.0/docs/source/examples/twitch_upload.py` & `datajudge-1.7.0/docs/source/examples/twitch_upload.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.6.0/docs/source/examples/twitch_version1.csv` & `datajudge-1.7.0/docs/source/examples/twitch_version1.csv`

 * *Files identical despite different names*

### Comparing `datajudge-1.6.0/docs/source/examples/twitch_version2.csv` & `datajudge-1.7.0/docs/source/examples/twitch_version2.csv`

 * *Files identical despite different names*

### Comparing `datajudge-1.6.0/docs/source/examples/twitchdata.csv` & `datajudge-1.7.0/docs/source/examples/twitchdata.csv`

 * *Files identical despite different names*

### Comparing `datajudge-1.6.0/docs/source/getting_started.rst` & `datajudge-1.7.0/docs/source/getting_started.rst`

 * *Files identical despite different names*

### Comparing `datajudge-1.6.0/docs/source/index.rst` & `datajudge-1.7.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `datajudge-1.6.0/docs/source/motivation.rst` & `datajudge-1.7.0/docs/source/motivation.rst`

 * *Files identical despite different names*

### Comparing `datajudge-1.6.0/docs/source/report_failing_query1.png` & `datajudge-1.7.0/docs/source/report_failing_query1.png`

 * *Files identical despite different names*

### Comparing `datajudge-1.6.0/docs/source/report_failing_query2.png` & `datajudge-1.7.0/docs/source/report_failing_query2.png`

 * *Files identical despite different names*

### Comparing `datajudge-1.6.0/docs/source/testing.rst` & `datajudge-1.7.0/docs/source/testing.rst`

 * *Files identical despite different names*

### Comparing `datajudge-1.6.0/pyproject.toml` & `datajudge-1.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datajudge-1.6.0/src/datajudge/constraints/base.py` & `datajudge-1.7.0/src/datajudge/constraints/base.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.6.0/src/datajudge/constraints/date.py` & `datajudge-1.7.0/src/datajudge/constraints/numeric.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,307 +1,288 @@
-import abc
-import datetime as dt
-from typing import Any, List, Optional, Tuple, Union
+from typing import Any, Optional, Tuple
 
 import sqlalchemy as sa
 
 from .. import db_access
 from ..db_access import DataReference
 from .base import Constraint, OptionalSelections, TestResult
+from .interval import NoGapConstraint, NoOverlapConstraint
 
-INPUT_DATE_FORMAT = "'%Y-%m-%d'"
 
-Date = Union[str, dt.date, dt.datetime]
-
-
-def get_format_from_column_type(column_type: str) -> str:
-    if column_type.lower() == "date":
-        return "%Y-%m-%d"
-    if column_type.lower() in ["datetime", "datetime2", "smalldatetime"]:
-        return "%Y-%m-%d %H:%M:%S"
-    raise ValueError(f"Illegal date column type: {column_type}")
-
-
-def convert_to_date(db_result: Date, format: str) -> dt.date:
-    if isinstance(db_result, dt.datetime):
-        return db_result.date()
-    if isinstance(db_result, dt.date):
-        return db_result
-    if isinstance(db_result, str):
-        # Get rid of nanoseconds as they cannot be parsed by strptime.
-        return dt.datetime.strptime(db_result.split(".")[0], format).date()
-    raise TypeError(f"Value hast type {type(db_result)} cannot be converted to date.")
-
-
-class DateMin(Constraint):
+class NumericMin(Constraint):
     def __init__(
         self,
         ref: DataReference,
-        use_lower_bound_reference: bool,
-        column_type: str,
         name: str = None,
         *,
         ref2: DataReference = None,
-        min_value: str = None,
+        min_value: float = None,
     ):
-        self.format = get_format_from_column_type(column_type)
-        self.use_lower_bound_reference = use_lower_bound_reference
-        min_date: Optional[dt.date] = None
-        if min_value is not None:
-            min_date = dt.datetime.strptime(min_value, INPUT_DATE_FORMAT).date()
-        super().__init__(ref, ref2=ref2, ref_value=min_date, name=name)
+        super().__init__(ref, ref2=ref2, ref_value=min_value, name=name)
 
     def retrieve(
         self, engine: sa.engine.Engine, ref: DataReference
-    ) -> Tuple[dt.date, OptionalSelections]:
-        result, selections = db_access.get_min(engine, ref)
-        return convert_to_date(result, self.format), selections
+    ) -> Tuple[float, OptionalSelections]:
+        return db_access.get_min(engine, ref)
 
-    def compare(self, min_factual: dt.date, min_target: dt.date) -> Tuple[bool, str]:
+    def compare(
+        self, min_factual: float, min_target: float
+    ) -> Tuple[bool, Optional[str]]:
         if min_target is None:
-            return TestResult(True, "")
+            return True, None
         if min_factual is None:
-            return TestResult(min_target == 0, "Empty set.")
-        if self.use_lower_bound_reference:
-            assertion_text = (
-                f"{self.ref.get_string()} has min {min_factual} < "
-                f"{self.target_prefix} {min_target}. "
-                f"{self.condition_string}"
-            )
-            result = min_factual >= min_target
-        else:
-            assertion_text = (
-                f"{self.ref.get_string()} has min {min_factual} > "
-                f"{self.target_prefix} {min_target}. "
-                f"{self.condition_string}"
-            )
-            result = min_factual <= min_target
+            return min_target == 0, "Empty set."
+        assertion_text = (
+            f"{self.ref.get_string()} has min "
+            f"{min_factual} instead of {self.target_prefix}"
+            f"{min_target} . "
+            f"{self.condition_string}"
+        )
+        result = min_factual >= min_target
         return result, assertion_text
 
 
-class DateMax(Constraint):
+class NumericMax(Constraint):
     def __init__(
         self,
         ref: DataReference,
-        use_upper_bound_reference: bool,
-        column_type: str,
         name: str = None,
         *,
         ref2: DataReference = None,
-        max_value: str = None,
+        max_value: float = None,
     ):
-        self.format = get_format_from_column_type(column_type)
-        self.use_upper_bound_reference = use_upper_bound_reference
-        max_date: Optional[dt.date] = None
-        if max_value is not None:
-            max_date = dt.datetime.strptime(max_value, INPUT_DATE_FORMAT).date()
-        super().__init__(ref, ref2=ref2, ref_value=max_date, name=name)
+        super().__init__(
+            ref,
+            ref2=ref2,
+            ref_value=max_value,
+            name=name,
+        )
 
     def retrieve(
         self, engine: sa.engine.Engine, ref: DataReference
-    ) -> Tuple[dt.date, OptionalSelections]:
-        value, selections = db_access.get_max(engine, ref)
-        return convert_to_date(value, self.format), selections
+    ) -> Tuple[float, OptionalSelections]:
+        return db_access.get_max(engine, ref)
 
-    def compare(self, max_factual: dt.date, max_target: dt.date) -> Tuple[bool, str]:
+    def compare(
+        self, max_factual: float, max_target: float
+    ) -> Tuple[bool, Optional[str]]:
         if max_factual is None:
             return True, None
         if max_target is None:
             return max_factual == 0, "Empty reference set."
-        if self.use_upper_bound_reference:
-            assertion_text = (
-                f"{self.ref.get_string()} has max {max_factual} > "
-                f"{self.target_prefix} {max_target}. "
-                f"{self.condition_string}"
-            )
-            result = max_factual <= max_target
-        else:
-            assertion_text = (
-                f"{self.ref.get_string()} has max {max_factual} < "
-                f"{self.target_prefix} {max_target}. "
-                f"{self.condition_string}"
-            )
-            result = max_factual >= max_target
-
+        assertion_text = (
+            f"{self.ref.get_string()} has max "
+            f"{max_factual} instead of {self.target_prefix}"
+            f"{max_target}. "
+            f"{self.condition_string}"
+        )
+        result = max_factual <= max_target
         return result, assertion_text
 
 
-class DateBetween(Constraint):
+class NumericBetween(Constraint):
     def __init__(
         self,
         ref: DataReference,
         min_fraction: float,
-        lower_bound: str,
-        upper_bound: str,
+        lower_bound: float,
+        upper_bound: float,
         name: str = None,
     ):
         super().__init__(ref, ref_value=min_fraction, name=name)
         self.lower_bound = lower_bound
         self.upper_bound = upper_bound
 
     def retrieve(
         self, engine: sa.engine.Engine, ref: DataReference
     ) -> Tuple[float, OptionalSelections]:
         return db_access.get_fraction_between(
-            engine, ref, self.lower_bound, self.upper_bound
+            engine,
+            ref,
+            self.lower_bound,
+            self.upper_bound,
         )
 
     def compare(
         self, fraction_factual: float, fraction_target: float
-    ) -> Tuple[bool, str]:
+    ) -> Tuple[bool, Optional[str]]:
+        if fraction_factual is None:
+            return True, "Empty selection."
         assertion_text = (
-            f"{self.ref.get_string()} has {fraction_factual} < "
-            f"{fraction_target} of values between {self.lower_bound} and "
-            f"{self.upper_bound}. {self.condition_string} "
+            f"{self.ref.get_string()} "
+            f"has {fraction_factual} < {fraction_target} of rows "
+            f"between {self.lower_bound} and {self.upper_bound}. "
+            f"{self.condition_string}"
         )
         result = fraction_factual >= fraction_target
         return result, assertion_text
 
 
-class DateIntervals(Constraint, abc.ABC):
-    _DIMENSIONS = 0
-
+class NumericMean(Constraint):
     def __init__(
         self,
         ref: DataReference,
-        key_columns: Optional[List[str]],
-        start_columns: List[str],
-        end_columns: List[str],
-        end_included: bool,
-        max_relative_n_violations: float,
+        max_absolute_deviation: float,
         name: str = None,
+        *,
+        ref2: DataReference = None,
+        mean_value: float = None,
     ):
-        super().__init__(ref, ref_value=object(), name=name)
-        self.key_columns = key_columns
-        self.start_columns = start_columns
-        self.end_columns = end_columns
-        self.end_included = end_included
-        self.max_relative_n_violations = max_relative_n_violations
-        self._validate_dimensions()
+        super().__init__(
+            ref,
+            ref2=ref2,
+            ref_value=mean_value,
+            name=name,
+        )
+        self.max_absolute_deviation = max_absolute_deviation
 
-    @abc.abstractmethod
-    def select(self, engine: sa.engine.Engine, ref: DataReference):
-        pass
+    def retrieve(
+        self, engine: sa.engine.Engine, ref: DataReference
+    ) -> Tuple[float, OptionalSelections]:
+        result, selections = db_access.get_mean(engine, ref)
+        return result, selections
 
-    def _validate_dimensions(self):
-        if (length := len(self.start_columns)) != self._DIMENSIONS:
+    def test(self, engine: sa.engine.Engine) -> TestResult:
+        mean_factual = self.get_factual_value(engine)
+        mean_target = self.get_target_value(engine)
+        if mean_factual is None or mean_target is None:
+            return TestResult(
+                mean_factual is None and mean_target is None,
+                "Mean over empty set.",
+            )
+        deviation = abs(mean_factual - mean_target)
+        assertion_text = (
+            f"{self.ref.get_string()} "
+            f"has mean {mean_factual}, deviating more than "
+            f"{self.max_absolute_deviation} from "
+            f"{self.target_prefix} {mean_target}. "
+            f"{self.condition_string}"
+        )
+        result = deviation <= self.max_absolute_deviation
+        return TestResult(result, assertion_text)
+
+
+class NumericPercentile(Constraint):
+    def __init__(
+        self,
+        ref: DataReference,
+        percentage: float,
+        max_absolute_deviation: Optional[float] = None,
+        max_relative_deviation: Optional[float] = None,
+        name: Optional[str] = None,
+        *,
+        ref2: DataReference = None,
+        expected_percentile: float = None,
+    ):
+        super().__init__(
+            ref,
+            ref2=ref2,
+            ref_value=expected_percentile,
+            name=name,
+        )
+        if not (0 <= percentage <= 100):
             raise ValueError(
-                f"Expected {self._DIMENSIONS} start_column(s), got {length}."
+                f"Expected percentage to be a value between 0 and 100, got {percentage}."
             )
-        if (length := len(self.end_columns)) != self._DIMENSIONS:
+        self.percentage = percentage
+        if max_absolute_deviation is None and max_relative_deviation is None:
             raise ValueError(
-                f"Expected {self._DIMENSIONS} end_column(s), got {length}."
+                "At least one of 'max_absolute_deviation' and 'max_relative_deviation' "
+                "must be given."
             )
+        if max_absolute_deviation is not None and max_absolute_deviation < 0:
+            raise ValueError(
+                f"max_absolute_deviation must be at least 0 but is {max_absolute_deviation}."
+            )
+        if max_relative_deviation is not None and max_relative_deviation < 0:
+            raise ValueError(
+                f"max_relative_deviation must be at least 0 but is {max_relative_deviation}."
+            )
+        self.max_absolute_deviation = max_absolute_deviation
+        self.max_relative_deviation = max_relative_deviation
 
     def retrieve(
         self, engine: sa.engine.Engine, ref: DataReference
-    ) -> Tuple[Tuple[int, int], OptionalSelections]:
-        keys_ref = DataReference(
-            data_source=self.ref.data_source,
-            columns=self.key_columns,
-            condition=self.ref.condition,
-        )
-        n_distinct_key_values, n_keys_selections = db_access.get_unique_count(
-            engine, keys_ref
-        )
-
-        sample_selection, n_violations_selection = self.select(engine, ref)
-        with engine.connect() as connection:
-            self.sample = connection.execute(sample_selection).first()
-            n_violation_keys = connection.execute(n_violations_selection).scalar()
+    ) -> Tuple[float, OptionalSelections]:
+        result, selections = db_access.get_percentile(engine, ref, self.percentage)
+        return result, selections
 
-        selections = [*n_keys_selections, sample_selection, n_violations_selection]
-        return (n_violation_keys, n_distinct_key_values), selections
+    def compare(
+        self, percentile_factual: float, percentile_target: float
+    ) -> Tuple[bool, Optional[str]]:
+        abs_diff = abs(percentile_factual - percentile_target)
+        if (
+            self.max_absolute_deviation is not None
+            and abs_diff > self.max_absolute_deviation
+        ):
+            assertion_message = (
+                f"The {self.percentage}-th percentile of {self.ref.get_string()} was "
+                f"expected to be {self.target_prefix}{percentile_target} but was "
+                f"{percentile_factual}, resulting in an absolute difference of "
+                f"{abs_diff}. The maximally allowed absolute deviation would've been "
+                f"{self.max_absolute_deviation}."
+            )
+            return False, assertion_message
+        if self.max_relative_deviation is not None:
+            if percentile_target == 0:
+                raise ValueError("Cannot compute relative deviation wrt 0.")
+            if (
+                rel_diff := abs_diff / abs(percentile_target)
+            ) > self.max_relative_deviation:
+                assertion_message = (
+                    f"The {self.percentage}-th percentile of {self.ref.get_string()}  was "
+                    f"expected to be {self.target_prefix}{percentile_target} but "
+                    f"was {percentile_factual}, resulting in a relative difference of "
+                    f"{rel_diff}. The maximally allowed relative deviation would've been "
+                    f"{self.max_relative_deviation}."
+                )
+                return False, assertion_message
+        return True, None
 
 
-class DateNoOverlap(DateIntervals):
+class NumericNoGap(NoGapConstraint):
     _DIMENSIONS = 1
 
     def select(self, engine: sa.engine.Engine, ref: DataReference):
-        sample_selection, n_violations_selection = db_access.get_date_overlaps_nd(
-            engine,
-            ref,
-            self.key_columns,
-            start_columns=self.start_columns,
-            end_columns=self.end_columns,
-            end_included=self.end_included,
-        )
-        # TODO: Once get_unique_count also only returns a selection without
-        # executing it, one would want to list this selection here as well.
-        return sample_selection, n_violations_selection
-
-    def compare(self, factual: Tuple[int, int], target: Any) -> Tuple[bool, str]:
-        n_violation_keys, n_distinct_key_values = factual
-        if n_distinct_key_values == 0:
-            return TestResult.success()
-        violation_fraction = n_violation_keys / n_distinct_key_values
-        assertion_text = (
-            f"{self.ref.get_string()} has a ratio of {violation_fraction} > "
-            f"{self.max_relative_n_violations} keys in columns {self.key_columns} "
-            f"with overlapping date ranges in {self.start_columns[0]} and {self.end_columns[0]}."
-            f"E.g. for: {self.sample}."
-        )
-        result = violation_fraction <= self.max_relative_n_violations
-        return result, assertion_text
-
-
-class DateNoOverlap2d(DateIntervals):
-    _DIMENSIONS = 2
-
-    def select(self, engine: sa.engine.Engine, ref: DataReference):
-        sample_selection, n_violations_selection = db_access.get_date_overlaps_nd(
+        sample_selection, n_violations_selection = db_access.get_numeric_gaps(
             engine,
             ref,
             self.key_columns,
-            start_columns=self.start_columns,
-            end_columns=self.end_columns,
-            end_included=self.end_included,
+            self.start_columns[0],
+            self.end_columns[0],
+            self.legitimate_gap_size,
         )
         # TODO: Once get_unique_count also only returns a selection without
         # executing it, one would want to list this selection here as well.
         return sample_selection, n_violations_selection
 
     def compare(self, factual: Tuple[int, int], target: Any) -> Tuple[bool, str]:
         n_violation_keys, n_distinct_key_values = factual
         if n_distinct_key_values == 0:
             return TestResult.success()
         violation_fraction = n_violation_keys / n_distinct_key_values
         assertion_text = (
             f"{self.ref.get_string()} has a ratio of {violation_fraction} > "
             f"{self.max_relative_n_violations} keys in columns {self.key_columns} "
-            f"with overlapping date ranges in {self.start_columns[0]} and {self.end_columns[0]}."
-            f"and {self.start_columns[1]} and {self.end_columns[1]}."
+            f"with a gap in the range in {self.start_columns[0]} and {self.end_columns[0]}."
             f"E.g. for: {self.sample}."
         )
         result = violation_fraction <= self.max_relative_n_violations
         return result, assertion_text
 
 
-class DateNoGap(DateIntervals):
+class NumericNoOverlap(NoOverlapConstraint):
     _DIMENSIONS = 1
 
-    def select(self, engine: sa.engine.Engine, ref: DataReference):
-        sample_selection, n_violations_selection = db_access.get_date_gaps(
-            engine,
-            ref,
-            self.key_columns,
-            self.start_columns[0],
-            self.end_columns[0],
-            self.end_included,
-        )
-        # TODO: Once get_unique_count also only returns a selection without
-        # executing it, one would want to list this selection here as well.
-        return sample_selection, n_violations_selection
-
     def compare(self, factual: Tuple[int, int], target: Any) -> Tuple[bool, str]:
         n_violation_keys, n_distinct_key_values = factual
         if n_distinct_key_values == 0:
             return TestResult.success()
         violation_fraction = n_violation_keys / n_distinct_key_values
         assertion_text = (
             f"{self.ref.get_string()} has a ratio of {violation_fraction} > "
             f"{self.max_relative_n_violations} keys in columns {self.key_columns} "
-            f"with a gap in the date range in {self.start_columns[0]} and {self.end_columns[0]}."
+            f"with overlapping ranges in {self.start_columns[0]} and {self.end_columns[0]}."
             f"E.g. for: {self.sample}."
         )
         result = violation_fraction <= self.max_relative_n_violations
         return result, assertion_text
```

### Comparing `datajudge-1.6.0/src/datajudge/constraints/groupby.py` & `datajudge-1.7.0/src/datajudge/constraints/groupby.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.6.0/src/datajudge/constraints/miscs.py` & `datajudge-1.7.0/src/datajudge/constraints/miscs.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.6.0/src/datajudge/constraints/nrows.py` & `datajudge-1.7.0/src/datajudge/constraints/nrows.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.6.0/src/datajudge/constraints/numeric.py` & `datajudge-1.7.0/src/datajudge/constraints/varchar.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,238 +1,220 @@
+import itertools
+import re
 from typing import Optional, Tuple
 
 import sqlalchemy as sa
 
 from .. import db_access
 from ..db_access import DataReference
 from .base import Constraint, OptionalSelections, TestResult
 
 
-class NumericMin(Constraint):
+class VarCharRegexDb(Constraint):
     def __init__(
         self,
         ref: DataReference,
+        regex: str,
+        relative_tolerance: float = 0.0,
+        aggregated: bool = True,
+        n_counterexamples: int = 5,
         name: str = None,
-        *,
-        ref2: DataReference = None,
-        min_value: float = None,
-    ):
-        super().__init__(ref, ref2=ref2, ref_value=min_value, name=name)
-
-    def retrieve(
-        self, engine: sa.engine.Engine, ref: DataReference
-    ) -> Tuple[float, OptionalSelections]:
-        return db_access.get_min(engine, ref)
-
-    def compare(
-        self, min_factual: float, min_target: float
-    ) -> Tuple[bool, Optional[str]]:
-        if min_target is None:
-            return True, None
-        if min_factual is None:
-            return min_target == 0, "Empty set."
-        assertion_text = (
-            f"{self.ref.get_string()} has min "
-            f"{min_factual} instead of {self.target_prefix}"
-            f"{min_target} . "
-            f"{self.condition_string}"
-        )
-        result = min_factual >= min_target
-        return result, assertion_text
-
-
-class NumericMax(Constraint):
-    def __init__(
-        self,
-        ref: DataReference,
-        name: str = None,
-        *,
-        ref2: DataReference = None,
-        max_value: float = None,
     ):
-        super().__init__(
-            ref,
-            ref2=ref2,
-            ref_value=max_value,
-            name=name,
+        super().__init__(ref, ref_value=relative_tolerance, name=name)
+        self.regex = regex
+        self.aggregated = aggregated
+        self.n_counterexamples = n_counterexamples
+
+    def retrieve(self, engine: sa.engine.Engine, ref: DataReference):
+        (
+            n_violations,
+            counterexamples,
+        ), violations_selections = db_access.get_regex_violations(
+            engine=engine,
+            ref=ref,
+            aggregated=self.aggregated,
+            regex=self.regex,
+            n_counterexamples=self.n_counterexamples,
+        )
+        if self.aggregated:
+            n_rows, n_rows_selections = db_access.get_unique_count(
+                engine=engine, ref=ref
+            )
+        else:
+            n_rows, n_rows_selections = db_access.get_row_count(engine=engine, ref=ref)
+        return (
+            n_violations,
+            n_rows,
+            counterexamples,
+        ), violations_selections + n_rows_selections
+
+    def compare(self, violations_factual, violations_target):
+        (
+            factual_n_violations,
+            factual_n_rows,
+            factual_counterexamples,
+        ) = violations_factual
+        factual_relative_violations = factual_n_violations / factual_n_rows
+        result = factual_relative_violations <= violations_target
+        counterexample_string = (
+            (
+                "Some counterexamples consist of the following: "
+                f"{factual_counterexamples}. "
+            )
+            if factual_counterexamples and len(factual_counterexamples) > 0
+            else ""
         )
-
-    def retrieve(
-        self, engine: sa.engine.Engine, ref: DataReference
-    ) -> Tuple[float, OptionalSelections]:
-        return db_access.get_max(engine, ref)
-
-    def compare(
-        self, max_factual: float, max_target: float
-    ) -> Tuple[bool, Optional[str]]:
-        if max_factual is None:
-            return True, None
-        if max_target is None:
-            return max_factual == 0, "Empty reference set."
         assertion_text = (
-            f"{self.ref.get_string()} has max "
-            f"{max_factual} instead of {self.target_prefix}"
-            f"{max_target}. "
-            f"{self.condition_string}"
+            f"{self.ref.get_string()} "
+            f"breaks regex '{self.regex}' in {factual_relative_violations} > "
+            f"{violations_target} of the cases. "
+            f"In absolute terms, {factual_n_violations} of the {factual_n_rows} samples "
+            f"violated the regex. {counterexample_string}{self.condition_string}"
         )
-        result = max_factual <= max_target
         return result, assertion_text
 
 
-class NumericBetween(Constraint):
+class VarCharRegex(Constraint):
     def __init__(
         self,
         ref: DataReference,
-        min_fraction: float,
-        lower_bound: float,
-        upper_bound: float,
+        regex: str,
+        allow_none: bool = False,
+        relative_tolerance: float = 0.0,
+        aggregated: bool = True,
+        n_counterexamples: int = 5,
         name: str = None,
     ):
-        super().__init__(ref, ref_value=min_fraction, name=name)
-        self.lower_bound = lower_bound
-        self.upper_bound = upper_bound
+        super().__init__(ref, ref_value=regex, name=name)
+        self.allow_none = allow_none
+        self.relative_tolerance = relative_tolerance
+        self.aggregated = aggregated
+        self.n_counterexamples = n_counterexamples
 
-    def retrieve(
-        self, engine: sa.engine.Engine, ref: DataReference
-    ) -> Tuple[float, OptionalSelections]:
-        return db_access.get_fraction_between(
-            engine,
-            ref,
-            self.lower_bound,
-            self.upper_bound,
-        )
-
-    def compare(
-        self, fraction_factual: float, fraction_target: float
-    ) -> Tuple[bool, Optional[str]]:
-        if fraction_factual is None:
-            return True, "Empty selection."
-        assertion_text = (
-            f"{self.ref.get_string()} "
-            f"has {fraction_factual} < {fraction_target} of rows "
-            f"between {self.lower_bound} and {self.upper_bound}. "
-            f"{self.condition_string}"
-        )
-        result = fraction_factual >= fraction_target
-        return result, assertion_text
+    def test(self, engine: sa.engine.Engine) -> TestResult:
+        uniques_counter, selections = db_access.get_uniques(engine, self.ref)
+        self.factual_selections = selections
+        if not self.allow_none and uniques_counter.get(None):
+            return TestResult.failure(
+                "The column contains a None value when it's not allowed. "
+                "To ignore None values, please use `allow_none=True` option."
+            )
+        elif None in uniques_counter:
+            uniques_counter.pop(None)
+
+        uniques_factual = list(uniques_counter.keys())
+        if not self.ref_value:
+            return TestResult.failure("No regex pattern given")
+
+        pattern = re.compile(self.ref_value)
+        uniques_mismatching = {
+            x for x in uniques_factual if not pattern.match(x)  # type: ignore
+        }
+
+        if self.aggregated:
+            n_violations = len(uniques_mismatching)
+            n_total = len(uniques_factual)
+        else:
+            n_violations = sum(uniques_counter[key] for key in uniques_mismatching)
+            n_total = sum(count for _, count in uniques_counter.items())
+
+        n_relative_violations = n_violations / n_total
+
+        if self.n_counterexamples == -1:
+            counterexamples = list(uniques_mismatching)
+        else:
+            counterexamples = list(
+                itertools.islice(uniques_mismatching, self.n_counterexamples)
+            )
+
+        counterexample_string = (
+            ("Some counterexamples consist of the following: " f"{counterexamples}. ")
+            if counterexamples and len(counterexamples) > 0
+            else ""
+        )
+
+        if n_relative_violations > self.relative_tolerance:
+            assertion_text = (
+                f"{self.ref.get_string()} "
+                f"breaks regex '{self.ref_value}' in {n_relative_violations} > "
+                f"{self.relative_tolerance} of the cases. "
+                f"In absolute terms, {n_violations} of the {n_total} samples violated the regex. "
+                f"{counterexample_string}{self.condition_string}"
+            )
+            return TestResult.failure(assertion_text)
+        return TestResult.success()
 
 
-class NumericMean(Constraint):
+class VarCharMinLength(Constraint):
     def __init__(
         self,
-        ref: DataReference,
-        max_absolute_deviation: float,
-        name: str = None,
+        ref,
         *,
         ref2: DataReference = None,
-        mean_value: float = None,
+        min_length: int = None,
+        name: str = None,
     ):
         super().__init__(
             ref,
             ref2=ref2,
-            ref_value=mean_value,
+            ref_value=min_length,
             name=name,
         )
-        self.max_absolute_deviation = max_absolute_deviation
 
     def retrieve(
         self, engine: sa.engine.Engine, ref: DataReference
-    ) -> Tuple[float, OptionalSelections]:
-        result, selections = db_access.get_mean(engine, ref)
-        return result, selections
+    ) -> Tuple[int, OptionalSelections]:
+        return db_access.get_min_length(engine, ref)
 
-    def test(self, engine: sa.engine.Engine) -> TestResult:
-        mean_factual = self.get_factual_value(engine)
-        mean_target = self.get_target_value(engine)
-        if mean_factual is None or mean_target is None:
-            return TestResult(
-                mean_factual is None and mean_target is None,
-                "Mean over empty set.",
-            )
-        deviation = abs(mean_factual - mean_target)
+    def compare(
+        self, length_factual: int, length_target: int
+    ) -> Tuple[bool, Optional[str]]:
+        if length_target is None:
+            return True, None
+        if length_factual is None:
+            return length_target == 0, "Empty set."
         assertion_text = (
             f"{self.ref.get_string()} "
-            f"has mean {mean_factual}, deviating more than "
-            f"{self.max_absolute_deviation} from "
-            f"{self.target_prefix} {mean_target}. "
+            f"has min length {length_factual} instead of "
+            f"{self.target_prefix} {length_target}. "
             f"{self.condition_string}"
         )
-        result = deviation <= self.max_absolute_deviation
-        return TestResult(result, assertion_text)
+        result = length_factual >= length_target
+        return result, assertion_text
 
 
-class NumericPercentile(Constraint):
+class VarCharMaxLength(Constraint):
     def __init__(
         self,
         ref: DataReference,
-        percentage: float,
-        max_absolute_deviation: Optional[float] = None,
-        max_relative_deviation: Optional[float] = None,
-        name: Optional[str] = None,
         *,
         ref2: DataReference = None,
-        expected_percentile: float = None,
+        max_length: int = None,
+        name: str = None,
     ):
         super().__init__(
             ref,
             ref2=ref2,
-            ref_value=expected_percentile,
+            ref_value=max_length,
             name=name,
         )
-        if not (0 <= percentage <= 100):
-            raise ValueError(
-                f"Expected percentage to be a value between 0 and 100, got {percentage}."
-            )
-        self.percentage = percentage
-        if max_absolute_deviation is None and max_relative_deviation is None:
-            raise ValueError(
-                "At least one of 'max_absolute_deviation' and 'max_relative_deviation' "
-                "must be given."
-            )
-        if max_absolute_deviation is not None and max_absolute_deviation < 0:
-            raise ValueError(
-                f"max_absolute_deviation must be at least 0 but is {max_absolute_deviation}."
-            )
-        if max_relative_deviation is not None and max_relative_deviation < 0:
-            raise ValueError(
-                f"max_relative_deviation must be at least 0 but is {max_relative_deviation}."
-            )
-        self.max_absolute_deviation = max_absolute_deviation
-        self.max_relative_deviation = max_relative_deviation
 
     def retrieve(
         self, engine: sa.engine.Engine, ref: DataReference
-    ) -> Tuple[float, OptionalSelections]:
-        result, selections = db_access.get_percentile(engine, ref, self.percentage)
-        return result, selections
+    ) -> Tuple[int, OptionalSelections]:
+        return db_access.get_max_length(engine, ref)
 
     def compare(
-        self, percentile_factual: float, percentile_target: float
+        self, length_factual: int, length_target: int
     ) -> Tuple[bool, Optional[str]]:
-        abs_diff = abs(percentile_factual - percentile_target)
-        if (
-            self.max_absolute_deviation is not None
-            and abs_diff > self.max_absolute_deviation
-        ):
-            assertion_message = (
-                f"The {self.percentage}-th percentile of {self.ref.get_string()} was "
-                f"expected to be {self.target_prefix}{percentile_target} but was "
-                f"{percentile_factual}, resulting in an absolute difference of "
-                f"{abs_diff}. The maximally allowed absolute deviation would've been "
-                f"{self.max_absolute_deviation}."
-            )
-            return False, assertion_message
-        if self.max_relative_deviation is not None:
-            if percentile_target == 0:
-                raise ValueError("Cannot compute relative deviation wrt 0.")
-            if (
-                rel_diff := abs_diff / abs(percentile_target)
-            ) > self.max_relative_deviation:
-                assertion_message = (
-                    f"The {self.percentage}-th percentile of {self.ref.get_string()}  was "
-                    f"expected to be {self.target_prefix}{percentile_target} but "
-                    f"was {percentile_factual}, resulting in a relative difference of "
-                    f"{rel_diff}. The maximally allowed relative deviation would've been "
-                    f"{self.max_relative_deviation}."
-                )
-                return False, assertion_message
-        return True, None
+        if length_factual is None:
+            return True, None
+        if length_target is None:
+            return length_factual == 0, "Reference value is None."
+        assertion_text = (
+            f"{self.ref.get_string()} "
+            f"has max length {length_factual} instead of "
+            f"{self.target_prefix} {length_target}. "
+            f"{self.condition_string}"
+        )
+        result = length_factual <= length_target
+        return result, assertion_text
```

### Comparing `datajudge-1.6.0/src/datajudge/constraints/row.py` & `datajudge-1.7.0/src/datajudge/constraints/row.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.6.0/src/datajudge/constraints/stats.py` & `datajudge-1.7.0/src/datajudge/constraints/stats.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.6.0/src/datajudge/constraints/uniques.py` & `datajudge-1.7.0/src/datajudge/constraints/uniques.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import abc
+from collections import Counter
 from itertools import zip_longest
+from math import ceil, floor
 from typing import Callable, Collection, Dict, List, Optional, Set, Tuple, Union
 
 import sqlalchemy as sa
 
 from .. import db_access
 from ..db_access import DataReference
 from .base import Constraint, OptionalSelections, T, TestResult, ToleranceGetter
@@ -288,7 +290,95 @@
         )
         result = relative_gain <= self.max_relative_gain
         return result, assertion_text
 
     def test(self, engine: sa.engine.Engine) -> TestResult:
         self.max_relative_gain = self.max_relative_gain_getter(engine)
         return super().test(engine)
+
+
+class CategoricalBoundConstraint(Constraint):
+    """
+    `CategoricalBoundConstraint` is a constraint class that checks if the share of specific values
+    in a column falls within predefined bounds. It compares the actual distribution of values in a
+    `DataSource` column with a target distribution, supplied as a dictionary.
+
+    Example use cases include testing for consistency in columns with expected categorical values
+    or ensuring that the distribution of values in a column adheres to a certain criterion.
+
+    Parameters
+    ----------
+    ref : DataReference
+        A reference to the column in the data source.
+    distribution : Dict[T, Tuple[float, float]]
+        A dictionary with unique values as keys and tuples of minimum and maximum allowed shares as values.
+    default_bounds : Tuple[float, float], optional, default=(0, 0)
+        A tuple specifying the minimum and maximum bounds for values not explicitly outlined in the target
+        distribution dictionary.
+    name : Optional[str], default=None
+        An optional name for the constraint.
+    max_relative_violations : float, optional, default=0
+        A tolerance threshold (0 to 1) for the proportion of elements in the data that can violate the
+        bound constraints without triggering the constraint violation.
+    """
+
+    def __init__(
+        self,
+        ref: DataReference,
+        distribution: Dict[T, Tuple[float, float]],
+        default_bounds: Tuple[float, float] = (0, 0),
+        name: Optional[str] = None,
+        max_relative_violations: float = 0,
+        **kwargs,
+    ):
+        self.default_bounds = default_bounds
+        self.max_relative_violations = max_relative_violations
+        super().__init__(ref, ref_value=distribution, name=name, **kwargs)
+
+    def retrieve(
+        self, engine: sa.engine.Engine, ref: DataReference
+    ) -> Tuple[Counter, OptionalSelections]:
+        return db_access.get_uniques(engine, ref)
+
+    def compare(
+        self,
+        factual: Counter,
+        target: Dict[T, Tuple[float, float]],
+    ) -> Tuple[bool, Optional[str]]:
+        # TODO: use .total() of Counter as soon as we can assume Python 3.10
+        total = sum(factual.values())
+        all_variants = factual.keys() | target.keys()
+        min_counts = Counter(
+            {k: target.get(k, self.default_bounds)[0] * total for k in all_variants}
+        )
+        max_counts = Counter(
+            {k: target.get(k, self.default_bounds)[1] * total for k in all_variants}
+        )
+
+        violations = (factual - max_counts) + (min_counts - factual)
+
+        if (
+            # TODO: use .total() of Counter as soon as we can assume Python 3.10
+            relative_violations := (sum(violations.values()) / total)
+        ) > self.max_relative_violations:
+            assertion_text = (
+                f"{self.ref.get_string()} has {relative_violations * 100}% > "
+                f"{self.max_relative_violations * 100}% of element(s) violating the bound constraints:\n"
+            )
+
+            for variant in violations:
+                actual_share = factual[variant] / total
+                target_share = target.get(variant, self.default_bounds)
+                min_required = min_counts[variant]
+                max_required = max_counts[variant]
+
+                assertion_text += (
+                    f"'{variant}' with a share of {actual_share * 100}% "
+                    f"({factual[variant]} out of {total}) "
+                    f"while a share between {target_share[0] * 100}% ({ceil(min_required)}) "
+                    f"and {target_share[1] * 100}% ({floor(max_required)}) "
+                    f"is required\n"
+                )
+
+            assertion_text += f"{self.condition_string}"
+            return False, assertion_text
+        return True, None
```

### Comparing `datajudge-1.6.0/src/datajudge/db_access.py` & `datajudge-1.7.0/src/datajudge/db_access.py`

 * *Files 3% similar despite different names*

```diff
@@ -455,15 +455,15 @@
     date_span, selections = get_date_span(engine, ref, date_column)
     date_span2, selections2 = get_date_span(engine, ref2, date_column2)
     if date_span2 == 0:
         raise ValueError("Reference date span is not allowed to be zero.")
     return date_span / date_span2 - 1, [*selections, *selections2]
 
 
-def get_date_overlaps_nd(
+def get_interval_overlaps_nd(
     engine: sa.engine.Engine,
     ref: DataReference,
     key_columns: list[str] | None,
     start_columns: list[str],
     end_columns: list[str],
     end_included: bool,
 ):
@@ -481,15 +481,15 @@
     dimensionality = len(start_columns)
     table1 = ref.get_selection(engine).alias()
     table2 = ref.get_selection(engine).alias()
 
     key_conditions = (
         [table1.c[key_column] == table2.c[key_column] for key_column in key_columns]
         if key_columns
-        else [True]
+        else [sa.literal(True)]
     )
     table_key_columns = get_table_columns(table1, key_columns) if key_columns else []
 
     end_operator = operator.ge if end_included else operator.gt
     violation_condition = sa.and_(
         *[
             sa.and_(
@@ -566,21 +566,24 @@
                     main_table.c[date_column] < helper_table.c[end_column],
                 )
             )
         )
     )
 
 
-def get_date_gaps(
+def _get_interval_gaps(
     engine: sa.engine.Engine,
     ref: DataReference,
     key_columns: list[str] | None,
     start_column: str,
     end_column: str,
-    end_included: bool,
+    legitimate_gap_size: float,
+    make_gap_condition: Callable[
+        [sa.Engine, sa.Subquery, sa.Subquery, str, str, float], sa.ColumnElement[bool]
+    ],
 ):
     if is_snowflake(engine):
         if key_columns:
             key_columns = lowercase_column_names(key_columns)
         start_column = lowercase_column_names(start_column)
         end_column = lowercase_column_names(end_column)
 
@@ -631,16 +634,54 @@
 
     end_table = (
         sa.select(*raw_end_table.columns, end_rank_column)
         .where(end_not_in_other_interval_condition)
         .subquery()
     )
 
-    legitimate_gap_size = 1 if end_included else 0
+    gap_condition = make_gap_condition(
+        engine, start_table, end_table, start_column, end_column, legitimate_gap_size
+    )
+
+    join_condition = sa.and_(
+        *[
+            start_table.c[key_column] == end_table.c[key_column]
+            for key_column in key_columns
+        ],
+        start_table.c["start_rank"] == end_table.c["end_rank"] + 1,
+        gap_condition,
+    )
+
+    violation_selection = sa.select(
+        *get_table_columns(start_table, key_columns),
+        start_table.c[start_column],
+        end_table.c[end_column],
+    ).select_from(start_table.join(end_table, join_condition))
+
+    violation_subquery = violation_selection.subquery()
 
+    keys = get_table_columns(violation_subquery, key_columns)
+
+    grouped_violation_subquery = sa.select(*keys).group_by(*keys).subquery()
+
+    n_violations_selection = sa.select(sa.func.count()).select_from(
+        grouped_violation_subquery
+    )
+
+    return violation_selection, n_violations_selection
+
+
+def _date_gap_condition(
+    engine: sa.engine.Engine,
+    start_table: sa.Subquery,
+    end_table: sa.Subquery,
+    start_column: str,
+    end_column: str,
+    legitimate_gap_size: float,
+) -> sa.ColumnElement[bool]:
     if is_mssql(engine) or is_snowflake(engine):
         gap_condition = (
             sa.func.datediff(
                 sa.text("day"),
                 end_table.c[end_column],
                 start_table.c[start_column],
             )
@@ -682,42 +723,68 @@
                 start_table.c[start_column],
                 end_table.c[end_column],
             )
             > legitimate_gap_size
         )
     else:
         raise NotImplementedError(f"Date gaps not yet implemented for {engine.name}.")
+    return gap_condition
 
-    join_condition = sa.and_(
-        *[
-            start_table.c[key_column] == end_table.c[key_column]
-            for key_column in key_columns
-        ],
-        start_table.c["start_rank"] == end_table.c["end_rank"] + 1,
-        gap_condition,
-    )
 
-    violation_selection = sa.select(
-        *get_table_columns(start_table, key_columns),
-        start_table.c[start_column],
-        end_table.c[end_column],
-    ).select_from(start_table.join(end_table, join_condition))
+def get_date_gaps(
+    engine: sa.engine.Engine,
+    ref: DataReference,
+    key_columns: list[str] | None,
+    start_column: str,
+    end_column: str,
+    legitimate_gap_size: float,
+):
+    return _get_interval_gaps(
+        engine,
+        ref,
+        key_columns,
+        start_column,
+        end_column,
+        legitimate_gap_size,
+        _date_gap_condition,
+    )
 
-    violation_subquery = violation_selection.subquery()
 
-    keys = get_table_columns(violation_subquery, key_columns)
+def _numeric_gap_condition(
+    _engine: sa.engine.Engine,
+    start_table: sa.Subquery,
+    end_table: sa.Subquery,
+    start_column: str,
+    end_column: str,
+    legitimate_gap_size: float,
+) -> sa.ColumnElement[bool]:
+    gap_condition = (
+        start_table.c[start_column] - end_table.c[end_column]
+    ) > legitimate_gap_size
+    return gap_condition
 
-    grouped_violation_subquery = sa.select(*keys).group_by(*keys).subquery()
 
-    n_violations_selection = sa.select(sa.func.count()).select_from(
-        grouped_violation_subquery
+def get_numeric_gaps(
+    engine: sa.engine.Engine,
+    ref: DataReference,
+    key_columns: list[str] | None,
+    start_column: str,
+    end_column: str,
+    legitimate_gap_size: float = 0,
+):
+    return _get_interval_gaps(
+        engine,
+        ref,
+        key_columns,
+        start_column,
+        end_column,
+        legitimate_gap_size,
+        _numeric_gap_condition,
     )
 
-    return violation_selection, n_violations_selection
-
 
 def get_row_count(engine, ref, row_limit: int = None):
     """Return the number of rows for a `DataReference`.
 
     If `row_limit` is given, the number of rows is capped at the limit.
     """
     subquery = ref.get_selection(engine)
@@ -904,25 +971,15 @@
 def get_column_names(engine, ref):
     table = ref.data_source.get_clause(engine)
     return [column.name for column in table.columns], None
 
 
 def get_column_type(engine, ref):
     table = ref.get_selection(engine).alias()
-    if is_snowflake(engine):
-        column_type = [str(column.type) for column in table.columns][0]
-        # Integer columns loaded from snowflake database may be referred to as decimal with
-        # 0 scale. More here:
-        # https://docs.snowflake.com/en/sql-reference/data-types-numeric.html#decimal-numeric
-        if column_type == "DECIMAL(38, 0)":
-            column_type = "integer"
-        return column_type, None
-    column_type = [
-        str(column.type).split(" ", maxsplit=1)[0] for column in table.columns
-    ][0]
+    column_type = next(iter(table.columns)).type
     return column_type, None
 
 
 def get_primary_keys(engine, ref):
     table = ref.data_source.get_clause(engine)
     return [column.name for column in table.primary_key.columns], None
```

### Comparing `datajudge-1.6.0/src/datajudge/pytest_integration.py` & `datajudge-1.7.0/src/datajudge/pytest_integration.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.6.0/src/datajudge/requirements.py` & `datajudge-1.7.0/src/datajudge/requirements.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 from abc import ABC
 from collections.abc import MutableSequence
-from typing import Callable, Collection, List, Optional, Sequence, TypeVar
+from typing import (
+    Callable,
+    Collection,
+    Dict,
+    List,
+    Optional,
+    Sequence,
+    Tuple,
+    TypeVar,
+    Union,
+)
 
 import sqlalchemy as sa
 
 from .constraints import column as column_constraints
 from .constraints import date as date_constraints
 from .constraints import groupby as groupby_constraints
 from .constraints import miscs as miscs_constraints
@@ -162,16 +172,38 @@
                 max_absolute_n_duplicates=max_absolute_n_duplicates,
                 infer_pk_columns=infer_pk_columns,
                 name=name,
             )
         )
 
     def add_column_type_constraint(
-        self, column: str, column_type: str, name: str = None
+        self,
+        column: str,
+        column_type: Union[str, sa.types.TypeEngine],
+        name: str = None,
     ):
+        """
+        Check if a column type matches the expected column_type.
+
+        The column_type can be provided as a string (backend-specific type name), a backend-specific SQLAlchemy type, or a SQLAlchemy's generic type.
+
+        If SQLAlchemy's generic types are used, the check is performed using `isinstance`, which means that the actual type can also be a subclass of the target type.
+        For more information on SQLAlchemy's generic types, see https://docs.sqlalchemy.org/en/20/core/type_basics.html
+
+        Parameters
+        ----------
+        column : str
+            The name of the column to which the constraint will be applied.
+
+        column_type : Union[str, sa.types.TypeEngine]
+            The expected type of the column. This can be a string, a backend-specific SQLAlchemy type, or a generic SQLAlchemy type.
+
+        name : Optional[str]
+            An optional name for the constraint. If not provided, a name will be generated automatically.
+        """
         ref = DataReference(self.data_source, [column])
         self._constraints.append(
             column_constraints.ColumnType(ref, column_type=column_type, name=name)
         )
 
     def add_null_absence_constraint(
         self, column: str, condition: Condition = None, name: str = None
@@ -341,14 +373,82 @@
         name: str = None,
     ):
         ref = DataReference(self.data_source, columns, condition)
         self._constraints.append(
             uniques_constraints.NUniquesEquality(ref, n_uniques=n_uniques, name=name)
         )
 
+    def add_categorical_bound_constraint(
+        self,
+        columns: List[str],
+        distribution: Dict[T, Tuple[float, float]],
+        default_bounds: Tuple[float, float] = (0, 0),
+        max_relative_violations: float = 0,
+        condition: Condition = None,
+        name: str = None,
+    ):
+        """
+        Check if the distribution of unique values in columns falls within the
+        specified minimum and maximum bounds.
+
+        The `CategoricalBoundConstraint` is added to ensure the distribution of unique values
+        in the specified columns of a `DataSource` falls within the given minimum and maximum
+        bounds defined in the `distribution` parameter.
+
+        Parameters
+        ----------
+        columns : List[str]
+            A list of column names from the `DataSource` to apply the constraint on.
+        distribution : Dict[T, Tuple[float, float]]
+            A dictionary where keys represent unique values and the corresponding
+            tuple values represent the minimum and maximum allowed proportions of the respective
+            unique value in the columns.
+        default_bounds : Tuple[float, float], optional, default=(0, 0)
+            A tuple specifying the minimum and maximum allowed proportions for all
+            elements not mentioned in the distribution. By default, it's set to (0, 0), which means
+            all elements not present in `distribution` will cause a constraint failure.
+        max_relative_violations : float, optional, default=0
+            A tolerance threshold (0 to 1) for the proportion of elements in the data that can violate the
+            bound constraints without triggering the constraint violation.
+        condition : Condition, optional
+            An optional parameter to specify a `Condition` object to filter the data
+            before applying the constraint.
+        name : str, optional
+            An optional parameter to provide a custom name for the constraint.
+
+        Example
+        -------
+        This method can be used to test for consistency in columns with expected categorical
+        values or ensure that the distribution of values in a column adheres to a certain
+        criterion.
+
+        Usage:
+
+        ```
+        requirement = WithinRequirement(data_source)
+        requirement.add_categorical_bound_constraint(
+            columns=['column_name'],
+            distribution={'A': (0.2, 0.3), 'B': (0.4, 0.6), 'C': (0.1, 0.2)},
+            max_relative_violations=0.05,
+            name='custom_name'
+        )
+        ```
+        """
+
+        ref = DataReference(self.data_source, columns, condition)
+        self._constraints.append(
+            uniques_constraints.CategoricalBoundConstraint(
+                ref,
+                distribution=distribution,
+                default_bounds=default_bounds,
+                max_relative_violations=max_relative_violations,
+                name=name,
+            )
+        )
+
     def add_numeric_min_constraint(
         self, column: str, min_value: float, condition: Condition = None
     ):
         """All values in column are greater or equal min_value."""
         ref = DataReference(self.data_source, [column], condition)
         self._constraints.append(
             numeric_constraints.NumericMin(ref, min_value=min_value)
@@ -445,24 +545,23 @@
         )
 
     def add_date_min_constraint(
         self,
         column: str,
         min_value: str,
         use_lower_bound_reference: bool = True,
-        column_type: str = "date",
+        column_type: Union[str, sa.types.TypeEngine] = "date",
         condition: Condition = None,
         name: str = None,
     ):
         """Ensure all dates to be superior than min_value.
 
         Use string format: min_value="'20121230'".
 
-        For valid ``column_type`` values, see`` get_format_from_column_type`` in
-        constraints/base.py.
+        For more information on ``column_type`` values, see ``add_column_type_constraint``.
 
         If ``use_lower_bound_reference``, the min of the first table has to be
         greater or equal to ``min_value``.
         If not ``use_upper_bound_reference``, the min of the first table has to
         be smaller or equal to ``min_value``.
         """
         ref = DataReference(self.data_source, [column], condition)
@@ -477,24 +576,23 @@
         )
 
     def add_date_max_constraint(
         self,
         column: str,
         max_value: str,
         use_upper_bound_reference: bool = True,
-        column_type: str = "date",
+        column_type: Union[str, sa.types.TypeEngine] = "date",
         condition: Condition = None,
         name: str = None,
     ):
         """Ensure all dates to be superior than max_value.
 
         Use string format: max_value="'20121230'".
 
-        For valid ``column_type`` values, see ``get_format_from_column_type`` in
-        constraints/base.py..
+        For more information on ``column_type`` values, see ``add_column_type_constraint``.
 
         If ``use_upper_bound_reference``, the max of the first table has to be
         smaller or equal to ``max_value``.
         If not ``use_upper_bound_reference``, the max of the first table has to
         be greater or equal to ``max_value``.
         """
         ref = DataReference(self.data_source, [column], condition)
@@ -699,15 +797,123 @@
         self._constraints.append(
             date_constraints.DateNoGap(
                 ref,
                 key_columns=key_columns,
                 start_columns=[start_column],
                 end_columns=[end_column],
                 max_relative_n_violations=max_relative_n_violations,
+                legitimate_gap_size=1 if end_included else 0,
+                name=name,
+            )
+        )
+
+    def add_numeric_no_gap_constraint(
+        self,
+        start_column: str,
+        end_column: str,
+        key_columns: Optional[List[str]] = None,
+        legitimate_gap_size: float = 0,
+        max_relative_n_violations: float = 0,
+        condition: Condition = None,
+        name: str = None,
+    ):
+        """
+        Express that numeric interval rows have no gaps larger than some max value in-between them.
+        The table under inspection must consist of at least one but up to many key columns,
+        identifying an entity. Additionally, a ``start_column`` and an ``end_column``,
+        indicating interval start and end values, should be provided.
+
+        Neither of those columns should contain ``NULL`` values. Also, it should hold that
+        for a given row, the value of ``end_column`` is strictly greater than the value of
+        ``start_column``.
+
+        ``legitimate_gap_size`` is the maximum tollerated gap size between two intervals.
+
+        A 'key' is a fixed set of values in ``key_columns`` and represents an entity of
+        interest. A priori, a key is not a primary key, i.e., a key can have and often has
+        several rows. Thereby, a key will often come with several intervals.
+
+        If`` key_columns`` is ``None`` or ``[]``, all columns of the table will be
+        considered as composing the key.
+
+        In order to express a tolerance for some violations of this gap property, use the
+        ``max_relative_n_violations`` parameter. The latter expresses for what fraction
+        of all key_values, at least one gap may exist.
+
+        For illustrative examples of this constraint, please refer to its test cases.
+        """
+        relevant_columns = (
+            ([start_column, end_column] + key_columns) if key_columns else []
+        )
+        ref = DataReference(self.data_source, relevant_columns, condition)
+        self._constraints.append(
+            numeric_constraints.NumericNoGap(
+                ref,
+                key_columns=key_columns,
+                start_columns=[start_column],
+                end_columns=[end_column],
+                legitimate_gap_size=legitimate_gap_size,
+                max_relative_n_violations=max_relative_n_violations,
+                name=name,
+            )
+        )
+
+    def add_numeric_no_overlap_constraint(
+        self,
+        start_column: str,
+        end_column: str,
+        key_columns: Optional[List[str]] = None,
+        end_included: bool = True,
+        max_relative_n_violations: float = 0,
+        condition: Condition = None,
+        name: str = None,
+    ):
+        """Constraint expressing that several numeric interval rows may not overlap.
+
+        The ``DataSource`` under inspection must consist of at least one but up
+        to many ``key_columns``, identifying an entity, a ``start_column`` and an
+        ``end_column``.
+
+        For a given row in this ``DataSource``, ``start_column`` and ``end_column`` indicate a
+        numeric interval. Neither of those columns should contain NULL values. Also, it
+        should hold that for a given row, the value of ``end_column`` is strictly greater
+        than the value of ``start_column``.
+
+        Note that the value of ``start_column`` is expected to be included in each interval.
+        By default, the value of ``end_column`` is expected to be included as well -
+        this can however be changed by setting ``end_included`` to ``False``.
+
+        A 'key' is a fixed set of values in ``key_columns`` and represents an entity of
+        interest. A priori, a key is not a primary key, i.e., a key can have and often
+        has several rows. Thereby, a key will often come with several intervals.
+
+        Often, you might want the intervals for a given key not to overlap.
+
+        If ``key_columns`` is ``None`` or ``[]``, all columns of the table will be considered
+        as composing the key.
+
+        In order to express a tolerance for some violations of this non-overlapping
+        property, use the ``max_relative_n_violations`` parameter. The latter expresses for
+        what fraction of all key values, at least one overlap may exist.
+
+        For illustrative examples of this constraint, please refer to its test cases.
+        """
+
+        relevant_columns = [start_column, end_column] + (
+            key_columns if key_columns else []
+        )
+        ref = DataReference(self.data_source, relevant_columns, condition)
+        self._constraints.append(
+            numeric_constraints.NumericNoOverlap(
+                ref,
+                key_columns=key_columns,
+                start_columns=[start_column],
+                end_columns=[end_column],
                 end_included=end_included,
+                max_relative_n_violations=max_relative_n_violations,
                 name=name,
             )
         )
 
     def add_varchar_regex_constraint(
         self,
         column: str,
@@ -1355,24 +1561,24 @@
         )
 
     def add_date_min_constraint(
         self,
         column1: str,
         column2: str,
         use_lower_bound_reference: bool = True,
-        column_type: str = "date",
+        column_type: Union[str, sa.types.TypeEngine] = "date",
         condition1: Condition = None,
         condition2: Condition = None,
         name: str = None,
     ):
         """Ensure date min of first table is greater or equal date min of second table.
 
         The used columns of both tables need to be of the same type.
 
-        For valid column_type values, see get_format_from_column_type in constraints/base.py..
+        For more information on ``column_type`` values, see ``add_column_type_constraint``.
 
         If ``use_lower_bound_reference``, the min of the first table has to be
         greater or equal to the min of the second table.
         If not ``use_upper_bound_reference``, the min of the first table has to
         be smaller or equal to the min of the second table.
         """
         ref = DataReference(self.data_source, [column1], condition1)
@@ -1388,24 +1594,24 @@
         )
 
     def add_date_max_constraint(
         self,
         column1: str,
         column2: str,
         use_upper_bound_reference: bool = True,
-        column_type: str = "date",
+        column_type: Union[str, sa.types.TypeEngine] = "date",
         condition1: Condition = None,
         condition2: Condition = None,
         name: str = None,
     ):
         """Compare date max of first table to date max of second table.
 
         The used columns of both tables need to be of the same type.
 
-        For valid column_type values, see get_format_from_column_type in constraints/base.py.
+        For more information on ``column_type`` values, see ``add_column_type_constraint``.
 
         If ``use_upper_bound_reference``, the max of the first table has to be
         smaller or equal to the max of the second table.
         If not ``use_upper_bound_reference``, the max of the first table has to
         be greater or equal to the max of the second table.
         """
         ref = DataReference(self.data_source, [column1], condition1)
@@ -1457,14 +1663,15 @@
     def add_column_superset_constraint(self, name: str = None):
         """Columns of first table are superset of columns of second table."""
         self._constraints.append(
             column_constraints.ColumnSuperset(self.ref, ref2=self.ref2, name=name)
         )
 
     def add_column_type_constraint(self, column1: str, column2: str, name: str = None):
+        "Check that the columns have the same type."
         ref1 = DataReference(self.data_source, [column1])
         ref2 = DataReference(self.data_source2, [column2])
         self._constraints.append(
             column_constraints.ColumnType(ref1, ref2=ref2, name=name)
         )
 
     def add_row_equality_constraint(
```

### Comparing `datajudge-1.6.0/start_mssql.sh` & `datajudge-1.7.0/start_mssql.sh`

 * *Files identical despite different names*

### Comparing `datajudge-1.6.0/tests/integration/conftest.py` & `datajudge-1.7.0/tests/integration/conftest.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 import itertools
 import os
 import random
 import urllib.parse
 
 import pytest
 import sqlalchemy as sa
-from impala.dbapi import connect
 
 from datajudge.db_access import apply_patches, is_bigquery, is_db2, is_impala, is_mssql
 
 TEST_DB_NAME = "tempdb"
 SCHEMA = "dbo"  # 'dbo' is the standard schema in mssql
 
 
 def get_engine(backend) -> sa.engine.Engine:
     address = os.environ.get("DB_ADDR", "localhost")
 
     if backend == "impala":
+        from impala.dbapi import connect
 
         def conn_creator():
             return connect(
                 host=address,
                 port=21050,
                 database="default",
             )
@@ -380,14 +380,83 @@
         },
     ]
     _handle_table(engine, metadata, table_name, columns, data)
     return TEST_DB_NAME, SCHEMA, table_name
 
 
 @pytest.fixture(scope="module")
+def integer_table_overlap(engine, metadata):
+    table_name = "integer_table_overlap"
+    columns = [
+        sa.Column("id1", sa.Integer()),
+        sa.Column("range_start", sa.Integer()),
+        sa.Column("range_end", sa.Integer()),
+    ]
+    data = []
+    # Trivial case: single entry.
+    data += [
+        {
+            "id1": 1,
+            "range_start": 1,
+            "range_end": 10,
+        }
+    ]
+    # 'Normal case': Multiple entries without overlap.
+    data += [
+        {
+            "id1": 2,
+            "range_start": i * 2,
+            "range_end": i * 2 + 1,
+        }
+        for i in range(1, 5)
+    ]
+    # Multiple entries with non-singleton overlap.
+    data += [
+        {
+            "id1": 3,
+            "range_start": 1,
+            "range_end": 10,
+        },
+        {
+            "id1": 3,
+            "range_start": 7,
+            "range_end": 15,
+        },
+    ]
+    # Multiple entries with singleton overlap.
+    data += [
+        {
+            "id1": 4,
+            "range_start": 1,
+            "range_end": 10,
+        },
+        {
+            "id1": 4,
+            "range_start": 10,
+            "range_end": 15,
+        },
+    ]
+    # Multiple entries with subset relation.
+    data += [
+        {
+            "id1": 5,
+            "range_start": 1,
+            "range_end": 10,
+        },
+        {
+            "id1": 5,
+            "range_start": 4,
+            "range_end": 8,
+        },
+    ]
+    _handle_table(engine, metadata, table_name, columns, data)
+    return TEST_DB_NAME, SCHEMA, table_name
+
+
+@pytest.fixture(scope="module")
 def date_table_gap(engine, metadata):
     table_name = "date_table_gap"
     columns = [
         sa.Column("id1", sa.Integer()),
         sa.Column("date_start", sa.DateTime()),
         sa.Column("date_end", sa.DateTime()),
     ]
@@ -449,14 +518,139 @@
         },
     ]
     _handle_table(engine, metadata, table_name, columns, data)
     return TEST_DB_NAME, SCHEMA, table_name
 
 
 @pytest.fixture(scope="module")
+def integer_table_gap(engine, metadata):
+    table_name = "integer_table_gap"
+    columns = [
+        sa.Column("id1", sa.Integer()),
+        sa.Column("range_start", sa.Integer()),
+        sa.Column("range_end", sa.Integer()),
+    ]
+    data = []
+    # Single entry should not be considered a gap.
+    data += [
+        {
+            "id1": 1,
+            "range_start": 1,
+            "range_end": 3,
+        }
+    ]
+    # Multiple entries without gap.
+    data += [
+        {
+            "id1": 2,
+            "range_start": 3 + i * 2,
+            "range_end": 5 + i * 2,
+        }
+        for i in range(1, 5)
+    ]
+    # Multiple entries with overlap.
+    data += [
+        {
+            "id1": 3,
+            "range_start": 1,
+            "range_end": 10,
+        },
+        {
+            "id1": 3,
+            "range_start": 3,
+            "range_end": 7,
+        },
+    ]
+    # Multiple entries with gap.
+    data += [
+        {
+            "id1": 4,
+            "range_start": 1,
+            "range_end": 5,
+        },
+        {
+            "id1": 4,
+            "range_start": 7,
+            "range_end": 10,
+        },
+    ]
+    _handle_table(engine, metadata, table_name, columns, data)
+    return TEST_DB_NAME, SCHEMA, table_name
+
+
+@pytest.fixture(scope="module")
+def float_table_gap(engine, metadata):
+    table_name = "float_table_gap"
+    columns = [
+        sa.Column("id1", sa.Integer()),
+        sa.Column("range_start", sa.Float()),
+        sa.Column("range_end", sa.Float()),
+    ]
+    data = []
+    # Single entry should not be considered a gap.
+    data += [
+        {
+            "id1": 1,
+            "range_start": 1,
+            "range_end": 3,
+        }
+    ]
+    # Multiple entries without gap.
+    data += [
+        {
+            "id1": 2,
+            "range_start": 3 + i * 2,
+            "range_end": 5 + i * 2,
+        }
+        for i in range(1, 5)
+    ]
+    # Multiple entries with overlap.
+    data += [
+        {
+            "id1": 3,
+            "range_start": 1,
+            "range_end": 10,
+        },
+        {
+            "id1": 3,
+            "range_start": 3,
+            "range_end": 7,
+        },
+    ]
+    # Multiple entries with gap.
+    data += [
+        {
+            "id1": 4,
+            "range_start": 1,
+            "range_end": 5,
+        },
+        {
+            "id1": 4,
+            "range_start": 8,
+            "range_end": 10,
+        },
+    ]
+    # Multiple entries with tolerated gap.
+    data += [
+        {
+            "id1": 5,
+            "range_start": 1,
+            "range_end": 5,
+        },
+        {
+            "id1": 5,
+            "range_start": 5.5,
+            "range_end": 10,
+        },
+    ]
+    _handle_table(engine, metadata, table_name, columns, data)
+    return TEST_DB_NAME, SCHEMA, table_name
+
+
+@pytest.fixture(scope="module")
 def date_table_keys(engine, metadata):
     table_name = "date_table_keys"
     columns = [
         sa.Column("id1", sa.Integer()),
         sa.Column("id2", sa.Integer()),
         sa.Column("date_start1", sa.DateTime()),
         sa.Column("date_end1", sa.DateTime()),
@@ -477,14 +671,26 @@
             for i in range(1, 5)
         ]
     _handle_table(engine, metadata, table_name, columns, data)
     return TEST_DB_NAME, SCHEMA, table_name
 
 
 @pytest.fixture(scope="module")
+def distribution_table(engine, metadata):
+    table_name = "distribution_table"
+    columns = [
+        sa.Column("col_int", sa.Integer()),
+        sa.Column("col_varchar", _string_column(engine)),
+    ]
+    data = [{"col_int": i // 10, "col_varchar": f"hi{i // 15}"} for i in range(20)]
+    _handle_table(engine, metadata, table_name, columns, data)
+    return TEST_DB_NAME, SCHEMA, table_name
+
+
+@pytest.fixture(scope="module")
 def unique_table1(engine, metadata):
     table_name = "unique_table1"
     columns = [
         sa.Column("col_int", sa.Integer()),
         sa.Column("col_varchar", _string_column(engine)),
     ]
     data = [{"col_int": i // 2, "col_varchar": f"hi{i // 3}"} for i in range(60)]
```

### Comparing `datajudge-1.6.0/tests/integration/test_column_capitalization.py` & `datajudge-1.7.0/tests/integration/test_column_capitalization.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.6.0/tests/integration/test_data_source.py` & `datajudge-1.7.0/tests/integration/test_data_source.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.6.0/tests/integration/test_integration.py` & `datajudge-1.7.0/tests/integration/test_integration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import functools
 
 import pytest
+import sqlalchemy as sa
 
 import datajudge.requirements as requirements
 from datajudge.db_access import (
     Condition,
     is_bigquery,
     is_db2,
     is_impala,
@@ -741,14 +742,67 @@
     )
     assert operation(req[0].test(engine).outcome)
 
 
 @pytest.mark.parametrize(
     "data",
     [
+        (identity, ["col_int"], {0: (0.45, 0.55), 1: (0.45, 0.55)}, (0, 0)),
+        (negation, ["col_int"], {0: (0.35, 0.55), 1: (0.55, 0.6)}, (0, 0)),
+        (negation, ["col_int"], {0: (0.35, 0.55), 1: (0.35, 0.45)}, (0, 0)),
+        (
+            identity,
+            ["col_int", "col_varchar"],
+            {(0, "hi0"): (0.45, 0.55), (1, "hi0"): (0.25, 0.3), (1, "hi1"): (0.2, 0.3)},
+            (0, 0),
+        ),
+        (
+            negation,
+            ["col_int", "col_varchar"],
+            {
+                (0, "hi0"): (0.45, 0.55),
+                (1, "hi0"): (0.25, 0.3),
+            },
+            (0, 0),
+        ),
+        (identity, ["col_varchar"], {"hi0": (0.65, 0.85), "hi1": (0.1, 0.35)}, (0, 0)),
+        (negation, ["col_varchar"], {"hi0": (0.65, 0.85)}, (0, 0)),
+        (identity, ["col_varchar"], {"hi0": (0.65, 0.85)}, (0, 0.35)),
+        (negation, ["col_varchar"], {}, (0, 0.35)),
+    ],
+)
+def test_categorical_bound_within(engine, distribution_table, data):
+    (operation, columns, distribution, default_bounds) = data
+    req = requirements.WithinRequirement.from_table(*distribution_table)
+    req.add_categorical_bound_constraint(columns, distribution, default_bounds)
+    test_result = req[0].test(engine)
+    assert operation(test_result.outcome), test_result.failure_message
+
+
+@pytest.mark.parametrize(
+    "data",
+    [
+        (negation, ["col_int"], {0: (0.40, 0.45), 1: (0.55, 0.60)}, 0),
+        (negation, ["col_int"], {0: (0.40, 0.45), 1: (0.55, 0.60)}, 0.05),
+        (identity, ["col_int"], {0: (0.40, 0.45), 1: (0.55, 0.60)}, 0.125),
+    ],
+)
+def test_categorical_bound_within_relative_violations(engine, distribution_table, data):
+    (operation, columns, distribution, max_relative_violations) = data
+    req = requirements.WithinRequirement.from_table(*distribution_table)
+    req.add_categorical_bound_constraint(
+        columns, distribution, max_relative_violations=max_relative_violations
+    )
+    test_result = req[0].test(engine)
+    assert operation(test_result.outcome), test_result.failure_message
+
+
+@pytest.mark.parametrize(
+    "data",
+    [
         (identity, 1, None),
         (identity, 3, Condition(raw_string="col_int >= 3")),
         (negation, 2, None),
         (negation, 4, Condition(raw_string="col_int = 3")),
     ],
 )
 def test_numeric_min_within(engine, int_table1, data):
@@ -1114,14 +1168,44 @@
     test_result = req[0].test(engine)
     assert operation(test_result.outcome), test_result.failure_message
 
 
 @pytest.mark.parametrize(
     "data",
     [
+        (identity, 0, Condition(raw_string="id1 = 1")),
+        (identity, 0, Condition(raw_string="id1 = 2")),
+        (negation, 0, Condition(raw_string="id1 = 3")),
+        (identity, 1, Condition(raw_string="id1 = 3")),
+        (negation, 0, Condition(raw_string="id1 = 4")),
+        (identity, 1, Condition(raw_string="id1 = 4")),
+        (negation, 0, Condition(raw_string="id1 = 5")),
+        (identity, 1, Condition(raw_string="id1 = 5")),
+    ],
+)
+@pytest.mark.parametrize("key_columns", [["id1"], [], None])
+def test_integer_no_overlap_within_varying_key_columns(
+    engine, integer_table_overlap, data, key_columns
+):
+    operation, max_relative_n_violations, condition = data
+    req = requirements.WithinRequirement.from_table(*integer_table_overlap)
+    req.add_numeric_no_overlap_constraint(
+        key_columns=key_columns,
+        start_column="range_start",
+        end_column="range_end",
+        max_relative_n_violations=max_relative_n_violations,
+        condition=condition,
+    )
+    test_result = req[0].test(engine)
+    assert operation(test_result.outcome), test_result.failure_message
+
+
+@pytest.mark.parametrize(
+    "data",
+    [
         (negation, 0.59, None),
         (identity, 0.6, None),
         (identity, 0, Condition(raw_string="id1 IN (1, 2)")),
     ],
 )
 def test_date_no_overlap_within_fixed_key_column(engine, date_table_overlap, data):
     operation, max_relative_n_violations, condition = data
@@ -1325,14 +1409,65 @@
 @pytest.mark.parametrize(
     "data",
     [
         (identity, 0, Condition(raw_string="id1 = 1")),
         (identity, 0, Condition(raw_string="id1 = 2")),
         (identity, 0, Condition(raw_string="id1 = 3")),
         (negation, 0, Condition(raw_string="id1 = 4")),
+        (identity, 0, None),
+    ],
+)
+def test_integer_no_gap_within_fixed_key_columns(engine, integer_table_gap, data):
+    operation, max_relative_n_violations, condition = data
+    req = requirements.WithinRequirement.from_table(*integer_table_gap)
+    req.add_numeric_no_gap_constraint(
+        key_columns=["id1"],
+        start_column="range_start",
+        end_column="range_end",
+        max_relative_n_violations=max_relative_n_violations,
+        legitimate_gap_size=0,
+        condition=condition,
+    )
+    test_result = req[0].test(engine)
+    assert operation(test_result.outcome), test_result.failure_message
+
+
+@pytest.mark.parametrize(
+    "data",
+    [
+        (identity, 0, Condition(raw_string="id1 = 1")),
+        (identity, 0, Condition(raw_string="id1 = 2")),
+        (identity, 0, Condition(raw_string="id1 = 3")),
+        (negation, 0, Condition(raw_string="id1 = 4")),
+        (negation, 0, Condition(raw_string="id1 = 5")),
+        (identity, 0.6, Condition(raw_string="id1 = 5")),
+    ],
+)
+def test_float_no_gap_within_fixed_key_columns(engine, float_table_gap, data):
+    operation, legitimate_gap_size, condition = data
+    req = requirements.WithinRequirement.from_table(*float_table_gap)
+    req.add_numeric_no_gap_constraint(
+        key_columns=["id1"],
+        start_column="range_start",
+        end_column="range_end",
+        legitimate_gap_size=legitimate_gap_size,
+        max_relative_n_violations=0,
+        condition=condition,
+    )
+    test_result = req[0].test(engine)
+    assert operation(test_result.outcome), test_result.failure_message
+
+
+@pytest.mark.parametrize(
+    "data",
+    [
+        (identity, 0, Condition(raw_string="id1 = 1")),
+        (identity, 0, Condition(raw_string="id1 = 2")),
+        (identity, 0, Condition(raw_string="id1 = 3")),
+        (negation, 0, Condition(raw_string="id1 = 4")),
     ],
 )
 @pytest.mark.parametrize("key_columns", [["id1"], [], None])
 def test_date_no_gap_within_varying_key_column(
     engine, date_table_gap, data, key_columns
 ):
     operation, max_relative_n_violations, condition = data
@@ -1885,19 +2020,21 @@
 
 @pytest.mark.parametrize(
     "data",
     [
         (identity, "col_varchar", "VARCHAR"),
         (identity, "col_int", "INTEGER"),
         (negation, "col_varchar", "INTEGER"),
+        (identity, "col_varchar", sa.types.String()),
+        (negation, "col_varchar", sa.types.Numeric()),
     ],
 )
 def test_column_type_within(engine, mix_table1, data):
     (operation, col_name, type_name) = data
-    if is_impala(engine):
+    if is_impala(engine) and type(type_name) == str:
         type_name = {"VARCHAR": "string", "INTEGER": "int"}[type_name]
     req = requirements.WithinRequirement.from_table(*mix_table1)
     req.add_column_type_constraint(col_name, type_name)
     test_result = req[0].test(engine)
     assert operation(test_result.outcome), test_result.failure_message
```

### Comparing `datajudge-1.6.0/tests/integration/test_stats.py` & `datajudge-1.7.0/tests/integration/test_stats.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.6.0/tests/unit/test_condition.py` & `datajudge-1.7.0/tests/unit/test_condition.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.6.0/tests/unit/test_db_access.py` & `datajudge-1.7.0/tests/unit/test_db_access.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.6.0/tests/unit/test_percentiles.py` & `datajudge-1.7.0/tests/unit/test_percentiles.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.6.0/tests/unit/test_pytest.py` & `datajudge-1.7.0/tests/unit/test_pytest.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.6.0/tests/unit/test_set_functions.py` & `datajudge-1.7.0/tests/unit/test_set_functions.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.6.0/PKG-INFO` & `datajudge-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datajudge
-Version: 1.6.0
+Version: 1.7.0
 Summary: datajudge allows to assess  whether data from database complies with reference
 Keywords: test,databases,validation
 Author-email: "QuantCo, Inc." <noreply@quantco.com>
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

