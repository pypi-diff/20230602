# Comparing `tmp/rqalpha-4.9.2.tar.gz` & `tmp/rqalpha-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/rqalpha/rqalpha/dist/tmpvihuja4t/rqalpha-4.9.2.tar", last modified: Thu Jul 21 04:01:35 2022, max compression
+gzip compressed data, was "/home/runner/work/rqalpha/rqalpha/dist/.tmp-74wqqrpp/rqalpha-5.0.0.tar", last modified: Fri Jun  2 01:50:19 2023, max compression
```

## Comparing `rqalpha-4.9.2.tar` & `rqalpha-5.0.0.tar`

### file list

```diff
@@ -1,235 +1,243 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/
--rw-r--r--   0 runner    (1001) docker     (121)    56630 2022-07-21 04:01:26.000000 rqalpha-4.9.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1444 2022-07-21 04:01:26.000000 rqalpha-4.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      300 2022-07-21 04:01:26.000000 rqalpha-4.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      609 2022-07-21 04:01:35.000000 rqalpha-4.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11339 2022-07-21 04:01:26.000000 rqalpha-4.9.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/
--rw-r--r--   0 runner    (1001) docker     (121)     7790 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1715 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     3290 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/api.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/apis/
--rw-r--r--   0 runner    (1001) docker     (121)     1605 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19532 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/apis/api_abstract.py
--rw-r--r--   0 runner    (1001) docker     (121)    32995 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/apis/api_base.py
--rw-r--r--   0 runner    (1001) docker     (121)    50314 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/apis/api_rqdatac.py
--rw-r--r--   0 runner    (1001) docker     (121)     3775 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/apis/names.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/cmds/
--rw-r--r--   0 runner    (1001) docker     (121)     1634 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7599 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/cmds/bundle.py
--rw-r--r--   0 runner    (1001) docker     (121)     1586 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/cmds/entry.py
--rw-r--r--   0 runner    (1001) docker     (121)     2862 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/cmds/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)     4209 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/cmds/mod.py
--rw-r--r--   0 runner    (1001) docker     (121)     5043 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/cmds/run.py
--rw-r--r--   0 runner    (1001) docker     (121)     2111 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/config.yml
--rw-r--r--   0 runner    (1001) docker     (121)     6471 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/const.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/core/
--rw-r--r--   0 runner    (1001) docker     (121)     1489 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6597 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/core/events.py
--rw-r--r--   0 runner    (1001) docker     (121)     4359 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/core/execution_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     5531 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/core/executor.py
--rw-r--r--   0 runner    (1001) docker     (121)     2264 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/core/global_var.py
--rw-r--r--   0 runner    (1001) docker     (121)     5748 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/core/strategy.py
--rw-r--r--   0 runner    (1001) docker     (121)     6883 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/core/strategy_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     2506 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/core/strategy_loader.py
--rw-r--r--   0 runner    (1001) docker     (121)     2863 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/core/strategy_universe.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/data/
--rw-r--r--   0 runner    (1001) docker     (121)     1549 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2492 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/data/bar_dict_price_board.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/data/base_data_source/
--rw-r--r--   0 runner    (1001) docker     (121)     1562 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/data/base_data_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3209 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/data/base_data_source/adjust.py
--rw-r--r--   0 runner    (1001) docker     (121)    16225 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/data/base_data_source/data_source.py
--rw-r--r--   0 runner    (1001) docker     (121)     3259 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/data/base_data_source/storage_interface.py
--rw-r--r--   0 runner    (1001) docker     (121)    10044 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/data/base_data_source/storages.py
--rw-r--r--   0 runner    (1001) docker     (121)    18663 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/data/bundle.py
--rw-r--r--   0 runner    (1001) docker     (121)    13947 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/data/data_proxy.py
--rw-r--r--   0 runner    (1001) docker     (121)     5837 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/data/trading_dates_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)     8025 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/examples/
--rw-r--r--   0 runner    (1001) docker     (121)    22343 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/examples/IF1706_20161108.csv
--rw-r--r--   0 runner    (1001) docker     (121)     2000 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/examples/IF_macd.py
--rw-r--r--   0 runner    (1001) docker     (121)     1005 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/examples/buy_and_hold.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/examples/data_source/
--rw-r--r--   0 runner    (1001) docker     (121)     1739 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/examples/data_source/get_csv_module.py
--rw-r--r--   0 runner    (1001) docker     (121)     2180 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/examples/data_source/import_get_csv_module.py
--rw-r--r--   0 runner    (1001) docker     (121)     2267 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/examples/data_source/read_csv_as_df.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/examples/extend_api/
--rw-r--r--   0 runner    (1001) docker     (121)     2706 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/examples/extend_api/rqalpha_mod_extend_api_demo.py
--rw-r--r--   0 runner    (1001) docker     (121)     2206 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/examples/extend_api/test_extend_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     2151 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/examples/golden_cross.py
--rw-r--r--   0 runner    (1001) docker     (121)     2110 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/examples/macd.py
--rw-r--r--   0 runner    (1001) docker     (121)     5532 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/examples/pair_trading.py
--rw-r--r--   0 runner    (1001) docker     (121)     2014 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/examples/rsi.py
--rw-r--r--   0 runner    (1001) docker     (121)      822 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/examples/run_code_demo.py
--rw-r--r--   0 runner    (1001) docker     (121)      436 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/examples/run_file_demo.py
--rw-r--r--   0 runner    (1001) docker     (121)     1031 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/examples/run_func_demo.py
--rw-r--r--   0 runner    (1001) docker     (121)     1623 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/examples/subscribe_event.py
--rw-r--r--   0 runner    (1001) docker     (121)     1280 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/examples/test_pt.py
--rw-r--r--   0 runner    (1001) docker     (121)     4619 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/examples/turtle.py
--rw-r--r--   0 runner    (1001) docker     (121)    20838 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/interface.py
--rw-r--r--   0 runner    (1001) docker     (121)    12204 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/mod/
--rw-r--r--   0 runner    (1001) docker     (121)     4489 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_accounts/
--rw-r--r--   0 runner    (1001) docker     (121)     3200 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_accounts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_accounts/api/
--rw-r--r--   0 runner    (1001) docker     (121)     1489 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_accounts/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10930 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py
--rw-r--r--   0 runner    (1001) docker     (121)    32509 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py
--rw-r--r--   0 runner    (1001) docker     (121)     2973 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_accounts/mod.py
--rw-r--r--   0 runner    (1001) docker     (121)    19262 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_accounts/position_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     3396 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_accounts/position_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/
--rw-r--r--   0 runner    (1001) docker     (121)     5712 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20668 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/mod.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/plot/
--rw-r--r--   0 runner    (1001) docker     (121)     1773 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5479 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py
--rw-r--r--   0 runner    (1001) docker     (121)     9256 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/plot/plot.py
--rw-r--r--   0 runner    (1001) docker     (121)     3740 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/plot/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3000 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/plot_store.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/report/
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3190 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/report/excel_template.py
--rw-r--r--   0 runner    (1001) docker     (121)     5526 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/report/report.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/report/templates/
--rw-r--r--   0 runner    (1001) docker     (121)    13833 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/report/templates/summary.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_progress/
--rw-r--r--   0 runner    (1001) docker     (121)     2018 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_progress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2446 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_progress/mod.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_risk/
--rw-r--r--   0 runner    (1001) docker     (121)     2359 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_risk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2208 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_risk/mod.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_risk/validators/
--rw-r--r--   0 runner    (1001) docker     (121)     1825 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_risk/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2801 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_risk/validators/cash_validator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2902 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_risk/validators/is_trading_validator.py
--rw-r--r--   0 runner    (1001) docker     (121)     3211 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_risk/validators/price_validator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2862 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_risk/validators/self_trade_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_scheduler/
--rw-r--r--   0 runner    (1001) docker     (121)     1578 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2448 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_scheduler/mod.py
--rw-r--r--   0 runner    (1001) docker     (121)    13505 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_scheduler/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_simulation/
--rw-r--r--   0 runner    (1001) docker     (121)     5339 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16525 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py
--rw-r--r--   0 runner    (1001) docker     (121)     5480 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_simulation/mod.py
--rw-r--r--   0 runner    (1001) docker     (121)     6053 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_simulation/signal_broker.py
--rw-r--r--   0 runner    (1001) docker     (121)     9498 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_broker.py
--rw-r--r--   0 runner    (1001) docker     (121)     9732 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_event_source.py
--rw-r--r--   0 runner    (1001) docker     (121)     5156 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_simulation/slippage.py
--rw-r--r--   0 runner    (1001) docker     (121)     2041 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_simulation/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_transaction_cost/
--rw-r--r--   0 runner    (1001) docker     (121)     3067 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_transaction_cost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7348 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_transaction_cost/deciders.py
--rw-r--r--   0 runner    (1001) docker     (121)     2785 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_transaction_cost/mod.py
--rw-r--r--   0 runner    (1001) docker     (121)     2560 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/model/
--rw-r--r--   0 runner    (1001) docker     (121)     1657 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12793 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/model/bar.py
--rw-r--r--   0 runner    (1001) docker     (121)    23525 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/model/instrument.py
--rw-r--r--   0 runner    (1001) docker     (121)    12026 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/model/order.py
--rw-r--r--   0 runner    (1001) docker     (121)     6448 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/model/tick.py
--rw-r--r--   0 runner    (1001) docker     (121)     5168 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/model/trade.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/portfolio/
--rw-r--r--   0 runner    (1001) docker     (121)    11108 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/portfolio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17895 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/portfolio/account.py
--rw-r--r--   0 runner    (1001) docker     (121)    14993 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/portfolio/position.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/resource/
--rw-r--r--   0 runner    (1001) docker     (121)    32799 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/resource/ricequant-logo.png
--rw-r--r--   0 runner    (1001) docker     (121)     1490 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/user_module.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     7589 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17569 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/arg_checker.py
--rw-r--r--   0 runner    (1001) docker     (121)     2357 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/class_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     1810 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/click_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     3670 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (121)    10415 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     3729 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/datetime_func.py
--rw-r--r--   0 runner    (1001) docker     (121)     1829 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/dict_func.py
--rw-r--r--   0 runner    (1001) docker     (121)     4853 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/exception.py
--rw-r--r--   0 runner    (1001) docker     (121)     4445 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/functools.py
--rw-r--r--   0 runner    (1001) docker     (121)     3080 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/i18n.py
--rw-r--r--   0 runner    (1001) docker     (121)     2257 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/log_capture.py
--rw-r--r--   0 runner    (1001) docker     (121)     3141 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     1900 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/package_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     3863 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/persisit_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     4038 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/repr.py
--rw-r--r--   0 runner    (1001) docker     (121)     2205 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/risk_free_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     2651 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/rq_json.py
--rw-r--r--   0 runner    (1001) docker     (121)     2695 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/strategy_loader_help.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/utils/testing/
--rw-r--r--   0 runner    (1001) docker     (121)      988 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5056 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/testing/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (121)      564 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/testing/mocking.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/utils/translations/
--rw-r--r--   0 runner    (1001) docker     (121)     1490 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/translations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/utils/translations/zh_Hans_CN/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1490 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17796 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (121)    48759 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (121)     1490 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/translations/zh_Hans_CN/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1803 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      609 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6993 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      260 2022-07-21 04:01:35.000000 rqalpha-4.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3430 2022-07-21 04:01:26.000000 rqalpha-4.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1489 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/tests/api_tests/
--rw-r--r--   0 runner    (1001) docker     (121)     3205 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/api_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/tests/api_tests/mod/
--rw-r--r--   0 runner    (1001) docker     (121)     1489 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/api_tests/mod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/tests/api_tests/mod/sys_accounts/
--rw-r--r--   0 runner    (1001) docker     (121)     1522 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/api_tests/mod/sys_accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5407 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/api_tests/mod/sys_accounts/test_account_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     2318 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/api_tests/mod/sys_accounts/test_position_models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/tests/api_tests/mod/sys_scheduler/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/api_tests/mod/sys_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2282 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/api_tests/mod/sys_scheduler/test_physical_time.py
--rw-r--r--   0 runner    (1001) docker     (121)     2215 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/api_tests/mod/sys_scheduler/test_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/tests/api_tests/mod/sys_simulation/
--rw-r--r--   0 runner    (1001) docker     (121)     1489 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/api_tests/mod/sys_simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3342 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/api_tests/mod/sys_simulation/test_management_fee.py
--rw-r--r--   0 runner    (1001) docker     (121)     2456 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/api_tests/mod/sys_simulation/test_signal_broker.py
--rw-r--r--   0 runner    (1001) docker     (121)     3624 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/api_tests/mod/sys_simulation/test_simulation_broker.py
--rw-r--r--   0 runner    (1001) docker     (121)     2719 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/api_tests/mod/sys_simulation/test_simulation_event_source.py
--rw-r--r--   0 runner    (1001) docker     (121)    16648 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/api_tests/test_api_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4390 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/api_tests/test_api_future.py
--rw-r--r--   0 runner    (1001) docker     (121)     9118 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/api_tests/test_api_stock.py
--rw-r--r--   0 runner    (1001) docker     (121)     4086 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/api_tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/api_tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/test_f_buy_and_hold.py
--rw-r--r--   0 runner    (1001) docker     (121)     2468 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/test_f_macd.py
--rw-r--r--   0 runner    (1001) docker     (121)     2534 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/test_f_macd_signal.py
--rw-r--r--   0 runner    (1001) docker     (121)     5741 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/test_f_mean_reverting.py
--rw-r--r--   0 runner    (1001) docker     (121)      661 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/test_s_buy_and_hold.py
--rw-r--r--   0 runner    (1001) docker     (121)     2307 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/test_s_dual_thrust.py
--rw-r--r--   0 runner    (1001) docker     (121)      760 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/test_s_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (121)     1170 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/test_s_tick_size.py
--rw-r--r--   0 runner    (1001) docker     (121)     5043 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/test_s_turtle.py
--rw-r--r--   0 runner    (1001) docker     (121)     5109 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/test_s_turtle_signal.py
--rw-r--r--   0 runner    (1001) docker     (121)     1842 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/test_sf_buy_and_hold.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/tests/unittest/
--rw-r--r--   0 runner    (1001) docker     (121)     1892 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/unittest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/tests/unittest/test_data/
--rw-r--r--   0 runner    (1001) docker     (121)      210 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/unittest/test_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2876 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/unittest/test_data/test_instrument_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)     2078 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/unittest/test_data/test_trading_dates_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/tests/unittest/test_mod/
--rw-r--r--   0 runner    (1001) docker     (121)     1700 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/unittest/test_mod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/tests/unittest/test_mod/test_sys_simulation/
--rw-r--r--   0 runner    (1001) docker     (121)     1700 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/unittest/test_mod/test_sys_simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4219 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/unittest/test_mod/test_sys_simulation/test_simulation_event_source.py
--rw-r--r--   0 runner    (1001) docker     (121)     1262 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    79815 2022-07-21 04:01:26.000000 rqalpha-4.9.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    61035 2023-06-02 01:50:10.000000 rqalpha-5.0.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-02 01:50:10.000000 rqalpha-5.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-02 01:50:10.000000 rqalpha-5.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-02 01:50:19.000000 rqalpha-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-06-02 01:50:10.000000 rqalpha-5.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/
+-rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24556 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/apis/api_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35283 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/apis/api_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52911 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/apis/api_rqdatac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/apis/names.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/cmds/
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/cmds/bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/cmds/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/cmds/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/cmds/mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/cmds/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/core/execution_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/core/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/core/global_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/core/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/core/strategy_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/core/strategy_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/core/strategy_universe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/data/bar_dict_price_board.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/data/base_data_source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/data/base_data_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/data/base_data_source/adjust.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16668 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/data/base_data_source/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/data/base_data_source/storage_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10064 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/data/base_data_source/storages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17445 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/data/bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14715 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/data/data_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/data/trading_dates_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    22343 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/examples/IF1706_20161108.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/examples/IF_macd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/examples/buy_and_hold.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/examples/data_source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/examples/data_source/get_csv_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/examples/data_source/import_get_csv_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/examples/data_source/read_csv_as_df.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/examples/extend_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/examples/extend_api/rqalpha_mod_extend_api_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/examples/extend_api/test_extend_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/examples/golden_cross.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/examples/macd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/examples/pair_trading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/examples/rsi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/examples/run_code_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/examples/run_file_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/examples/run_func_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/examples/subscribe_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/examples/test_pt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/examples/turtle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21124 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12580 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/mod/
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_accounts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_accounts/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_accounts/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11188 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34524 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_accounts/component_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_accounts/mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20020 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_accounts/position_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_accounts/position_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_accounts/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/
+-rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24306 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/mod.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10160 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/report/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/report/excel_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/report/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/report/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    15036 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/report/templates/summary.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_progress/
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_progress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_progress/mod.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_risk/
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_risk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_risk/mod.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/cash_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/is_trading_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/price_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/self_trade_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_scheduler/mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13593 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_scheduler/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29229 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_simulation/mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_simulation/signal_broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9750 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10300 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_event_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_simulation/slippage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_simulation/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_simulation/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_transaction_cost/
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_transaction_cost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_transaction_cost/deciders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_transaction_cost/mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12793 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/model/bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24670 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/model/instrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13053 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/model/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/model/tick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/model/trade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/portfolio/
+-rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/portfolio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20437 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/portfolio/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14772 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/portfolio/position.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)    32799 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/resource/ricequant-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/user_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18080 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/arg_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/class_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/click_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10415 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/datetime_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/dict_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/log_capture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/package_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/persisit_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/risk_free_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/rq_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/strategy_loader_help.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/utils/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/testing/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/testing/mocking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/utils/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/translations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/utils/translations/zh_Hans_CN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19267 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    51160 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/translations/zh_Hans_CN/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-02 01:50:19.000000 rqalpha-5.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-06-02 01:50:10.000000 rqalpha-5.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/tests/api_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/api_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/tests/api_tests/mod/
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/api_tests/mod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/tests/api_tests/mod/sys_accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/api_tests/mod/sys_accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/api_tests/mod/sys_accounts/test_account_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/api_tests/mod/sys_accounts/test_futures_settlement_price_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/api_tests/mod/sys_accounts/test_margin_stocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/api_tests/mod/sys_accounts/test_position_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/tests/api_tests/mod/sys_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/api_tests/mod/sys_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/api_tests/mod/sys_scheduler/test_physical_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/api_tests/mod/sys_scheduler/test_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/tests/api_tests/mod/sys_simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/api_tests/mod/sys_simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/api_tests/mod/sys_simulation/test_management_fee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/api_tests/mod/sys_simulation/test_signal_broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/api_tests/mod/sys_simulation/test_simulation_broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/api_tests/mod/sys_simulation/test_simulation_event_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/tests/api_tests/mod/sys_transaction_cost/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/api_tests/mod/sys_transaction_cost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/api_tests/mod/sys_transaction_cost/test_commission_multiplier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/api_tests/test_api_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/api_tests/test_api_future.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/api_tests/test_api_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/api_tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/api_tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/test_f_buy_and_hold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/test_f_macd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/test_f_macd_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/test_f_mean_reverting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/test_s_buy_and_hold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/test_s_dual_thrust.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/test_s_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/test_s_tick_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/test_s_turtle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/test_s_turtle_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/test_sf_buy_and_hold.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/tests/unittest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/unittest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/tests/unittest/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/unittest/test_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/unittest/test_data/test_instrument_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/unittest/test_data/test_trading_dates_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/tests/unittest/test_mod/
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/unittest/test_mod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/tests/unittest/test_mod/test_sys_simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/unittest/test_mod/test_sys_simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/unittest/test_mod/test_sys_simulation/test_simulation_event_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79879 2023-06-02 01:50:10.000000 rqalpha-5.0.0/versioneer.py
```

### Comparing `rqalpha-4.9.2/CHANGELOG.rst` & `rqalpha-5.0.0/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,145 @@
 ==================
 CHANGELOG
 ==================
 
+5.0.0
+==================
+- 适配pandas2.0
+- 交易指数标的时，不检查上市日期，根据行情数据有无决定
+- 撮合时屏蔽已完成的订单
+- 修复get_prev_settlement取不到第一天的，采用prev_settlement字段
+- 新增算法单：VWAPOrder 和 TWAPOrder
+
+4.16.2
+==================
+- 修复bundle更新异常
+- 限制pandas版本为 < 2.0.0
+- sys_analyser检查基准合法性
+- sys_accounts支持分别设置股票、期货佣金倍率
+
+4.16.1
+==================
+- 修正文档
+
+4.16.0
+==================
+- 新增check-bundle检查日线bundle命令
+- report年度指标sheet新增指标
+- 修复tick回测和获取无风险收益率的异常
+- 改善order_target_portfolio并完善api文档
+
+4.15.0
+==================
+- 修复python3.10在Ubuntu和Centos下更新数据异常
+- 期货回测支持使用结算价进行结算
+- 修正报告中跟踪误差，使用年化跟踪误差
+- 修改超额收益相关指标的计算，具体公式可参考rqrisk
+
+4.14.1
+==================
+- ricequant报告图模版调整超额收益曲线，公式改为每日的超额收益率的累计
+- 改善summary报告中数据的展示格式并新增部分指标
+
+4.14.0
+==================
+- 分析报告新增UlcerIndex(累计回撤深度)和UlcerPerformanceIndex(累计回撤夏普率)相关指标
+- 修复多次输出plot图时水印异常
+
+4.13.1
+==================
+- 适配次主力合约(88A2)和次次主力合约(88A3)
+
+4.13.0
+==================
+- analyser plot 新增报告图模版功能
+- account 弃用 equity 改为 position_equity
+- INSTRUMENT_TYPE 新增 Fund 类型
+
+4.12.1
+==================
+- 修正日志
+
+4.12.0
+==================
+- 调整分析指标中部分指标的显示格式为百分比
+- 将分析指标中的超额收益波动率从日度改为年化
+- 入金支持延迟到账
+
+4.11.3
+==================
+- 分析指标新增胜率和盈亏比，调整了作图中指标的布局
+- 修复当本地语言为中文但无中文字体时基准名称显示的异常
+- 修复输出report时账户未记录清仓手续费的异常
+- 修复前一个交易日发生除息,当前交易日在before_trading时 position.last_price 未进行复权的异常
+
+4.11.2
+==================
+- 修复 physical_time api接口的导出，策略编写不在需要显式导出
+- 修复 更新base数据时window系统下出现内存错误的异常
+
+4.11.1
+==================
+- 新增取消rqdatac init 开关, config base rqdatac_uri 可设置为 'disabled' 或 'DISABLED'
+- 修正关于888前复权合约的数据问题
+- 调整默认撮合方式, matching_type 为 None 则表示根据回测频率自动选择。日/分钟回测下为 current_bar , tick 回测下为 last
+- 修复性能分析
+
+4.11.0
+==================
+- 针对股票和ETF新增融资功能，新增 finance 和 repay API
+- Account 新增 cash_liabilities(现金负债) 属性
+- sys_account 新增 financing_rate(融资利率/年) 和 financing_stocks_restriction_enabled(是否开启融资可买股票池限制) 配置项
+- 优化回测报告，在图例中显示基准的名称
+
+4.10.1
+==================
+- 优化回测报告及返回值输出情况，增加最长回撤持续期相关指标
+
+4.10.0
+==================
+- 将DefaultMatcher划分DefaultBarMatcher和DefaultTickMatcher
+- Tick回测支持成交量限制，成交量限制为两个tick的成交量之差乘以volume_percent
+- Tick回测handle_bar支持盘前的tick
+- Tick回测不再支持open_auction接口，集合竞价时段内成交一律使用last
+- 修复get_open_auction_bar获取非交易日时的异常
+
+4.9.2
+==================
+- 修改get_pit_financials_ex接口中count参数的含义为当前标的已发布财报的数量
+
+4.9.1
+==================
+- 修复get_pit_financials_ex接口的bug
+
+4.9.0
+==================
+- 定时器新增期货应用场景
+- 改善tick回测性能
+
+4.8.1
+==================
+- 改善回测输出的summary和净值图，新增超额累计收益指标
+
+4.8.0
+==================
+- Position类移除了 _today_quantity 属性，新增 _quantity 属性
+- 部分接口新增了缓存
+- Environment类新增submit_order接口
+- Interface中AbstractPosition移除了margin接口
+- order_target_portfolio接口支持 limit order
+- rqalpha_mod_sys_analyser组件报表新增excel格式
+- 提升框架的整体性能
+
+4.7.1
+==================
+- 补全类型提示
+- 优化翻译和错误提示
+- 全面支持Python3.10
+
 4.7.0
 ==================
 - 重构绘制策略收益图的逻辑。增加绘制买卖点的选项，周度收益曲线和指标改为通过配置项激活
 - 调整 Signal 模式的逻辑。现在在 Signal 模式下开启 price_limit 选项时，超出涨跌停价格范围的订单将会被拒绝
 - 重构国际化逻辑。现在 RQAlpha 将自动检测操作系统的语言设置从而在中英文间进行切换（而不是强制使用中文）
 - 优化部分日志和错误信息的中文翻译
 - 调整了部分在 Python3.10 下会报错的代码
```

### Comparing `rqalpha-4.9.2/LICENSE` & `rqalpha-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/PKG-INFO` & `rqalpha-5.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: rqalpha
-Version: 4.9.2
+Version: 5.0.0
 Summary: Ricequant Algorithm Trading System
 Home-page: https://github.com/ricequant/rqalpha
 Author: ricequant
 Author-email: public@ricequant.com
 License: Apache License v2
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
+Provides-Extra: profiler
 License-File: LICENSE
```

### Comparing `rqalpha-4.9.2/README.rst` & `rqalpha-5.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/__init__.py` & `rqalpha-5.0.0/rqalpha/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/__main__.py` & `rqalpha-5.0.0/rqalpha/__main__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/api.py` & `rqalpha-5.0.0/rqalpha/api.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/apis/__init__.py` & `rqalpha-5.0.0/rqalpha/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/apis/api_abstract.py` & `rqalpha-5.0.0/rqalpha/apis/api_abstract.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,191 +11,224 @@
 #     * 商业用途（商业用途指个人出于任何商业目的使用本软件，或者法人或其他组织出于任何目的使用本软件）：
 #         未经米筐科技授权，任何个人不得出于任何商业目的使用本软件（包括但不限于向第三方提供、销售、出租、出借、转让本软件、
 #         本软件的衍生产品、引用或借鉴了本软件功能或源代码的产品或服务），任何法人或其他组织不得出于任何目的使用本软件，
 #         否则米筐科技有权追究相应的知识产权侵权责任。
 #         在此前提下，对本软件的使用同样需要遵守 Apache 2.0 许可，Apache 2.0 许可与本许可冲突之处，以本许可为准。
 #         详细的授权流程，请联系 public@ricequant.com 获取。
 
-from typing import Union, Optional, List
+from typing import Union, Optional, List, Tuple
 
 from rqalpha.api import export_as_api
 from rqalpha.core.execution_context import ExecutionContext
 from rqalpha.const import EXECUTION_PHASE
 from rqalpha.model.instrument import Instrument
-from rqalpha.model.order import MarketOrder, LimitOrder, OrderStyle, Order
+from rqalpha.model.order import MarketOrder, LimitOrder, OrderStyle, Order, ALL_ORDER_STYPES
 from rqalpha.utils.arg_checker import apply_rules, verify_that
 from rqalpha.utils.functools import instype_singledispatch
 
 
+common_rules = (
+    verify_that('price', pre_check=True).deprecated("please use price_or_style instead.").is_greater_than(0),
+    verify_that('style', pre_check=True).deprecated("please use price_or_style instead.").is_instance_of(
+        (*ALL_ORDER_STYPES, type(None))
+    ),
+    verify_that("price_or_style", pre_check=True).is_instance_of((float, type(None), tuple, *ALL_ORDER_STYPES)),
+)
+
+
+PRICE_OR_STYLE_TYPE = Union[float, OrderStyle, None]
+TUPLE_PRICE_OR_STYLE_TYPE = Union[
+    float, OrderStyle, None, Tuple, Tuple[PRICE_OR_STYLE_TYPE], Tuple[PRICE_OR_STYLE_TYPE, PRICE_OR_STYLE_TYPE]
+]
+
+
 @export_as_api
 @ExecutionContext.enforce_phase(
     EXECUTION_PHASE.OPEN_AUCTION,
     EXECUTION_PHASE.ON_BAR,
     EXECUTION_PHASE.ON_TICK,
     EXECUTION_PHASE.SCHEDULED,
     EXECUTION_PHASE.GLOBAL
 )
 @apply_rules(
     verify_that('amount').is_number(),
-    verify_that('style').is_instance_of((MarketOrder, LimitOrder, type(None)))
+    *common_rules
 )
 @instype_singledispatch
-def order_shares(id_or_ins, amount, price=None, style=None):
-    # type: (Union[str, Instrument], int, Optional[float], Optional[OrderStyle]) -> Optional[Order]
+def order_shares(id_or_ins, amount, price=None, style=None, price_or_style=None):
+    # type: (Union[str, Instrument], int, Optional[float], Optional[OrderStyle], PRICE_OR_STYLE_TYPE) -> Optional[Order]
     """
     指定股数的买/卖单，最常见的落单方式之一。如有需要落单类型当做一个参量传入，如果忽略掉落单类型，那么默认是市价单（market order）。
 
     :param id_or_ins: 下单标的物
     :param amount: 下单量, 正数代表买入，负数代表卖出。将会根据一手xx股来向下调整到一手的倍数，比如中国A股就是调整成100股的倍数。
     :param price: 下单价格，默认为None，表示 :class:`~MarketOrder`, 此参数主要用于简化 `style` 参数。
     :param style: 下单类型, 默认是市价单。目前支持的订单类型有 :class:`~LimitOrder` 和 :class:`~MarketOrder`
+    :param price_or_style: 默认为None，表示市价单，可设置价格，表示限价单，也可以直接设置订单类型，有如下选项：MarketOrder、LimitOrder、
+                            TWAPOrder、VWAPOrder
 
     :example:
 
     .. code-block:: python
 
         #购买Buy 2000 股的平安银行股票，并以市价单发送：
         order_shares('000001.XSHE', 2000)
         #卖出2000股的平安银行股票，并以市价单发送：
         order_shares('000001.XSHE', -2000)
+        #购买1000股的平安银行股票，并以限价单发送，价格为￥11：
+        order_shares('000001.XSHG', 1000, price_or_style=11)
         #购买1000股的平安银行股票，并以限价单发送，价格为￥10：
-        order_shares('000001.XSHG', 1000, style=LimitOrder(10))
+        order_shares('000001.XSHG', 1000, price_or_style=LimitOrder(10))
+        #购买1000股的平安银行股票，并以 9:31 到 9:45 的VWAP价格发送：
+        order_shares('000001.XSHG', 1000, price_or_style=VWAPOrder(931, 945))
     """
     raise NotImplementedError
 
 
 @export_as_api
 @ExecutionContext.enforce_phase(
     EXECUTION_PHASE.OPEN_AUCTION,
     EXECUTION_PHASE.ON_BAR,
     EXECUTION_PHASE.ON_TICK,
     EXECUTION_PHASE.SCHEDULED,
     EXECUTION_PHASE.GLOBAL
 )
 @apply_rules(
     verify_that('cash_amount').is_number(),
-    verify_that('style').is_instance_of((MarketOrder, LimitOrder, type(None)))
+    *common_rules
 )
 @instype_singledispatch
-def order_value(id_or_ins, cash_amount, price=None, style=None):
-    # type: (Union[str, Instrument], float, Optional[float], Optional[OrderStyle]) -> Optional[Order]
+def order_value(id_or_ins, cash_amount, price=None, style=None, price_or_style=None):
+    # type: (Union[str, Instrument], float, Optional[float], Optional[OrderStyle], PRICE_OR_STYLE_TYPE) -> Optional[Order]
     """
-    使用想要花费的金钱买入/卖出股票，而不是买入/卖出想要的股数，正数代表买入，负数代表卖出。股票的股数总是会被调整成对应的100的倍数（在A中国A股市场1手是100股）。如果资金不足，该API将不会创建发送订单。
+    使用想要花费的金钱买入/卖出股票，而不是买入/卖出想要的股数，正数代表买入，负数代表卖出。股票的股数总是会被调整成对应的100的倍数（在A中国A股市场1手是100股）。
+    如果资金不足，该API将会使用最大可用资金发单。
 
     需要注意：
     当您提交一个买单时，cash_amount 代表的含义是您希望买入股票消耗的金额（包含税费），最终买入的股数不仅和发单的价格有关，还和税费相关的参数设置有关。
     当您提交一个卖单时，cash_amount 代表的意义是您希望卖出股票的总价值。如果金额超出了您所持有股票的价值，那么您将卖出所有股票。
 
     :param id_or_ins: 下单标的物
     :param cash_amount: 需要花费现金购买/卖出证券的数目。正数代表买入，负数代表卖出。
     :param price: 下单价格，默认为None，表示 :class:`~MarketOrder`, 此参数主要用于简化 `style` 参数。
     :param style: 下单类型, 默认是市价单。目前支持的订单类型有 :class:`~LimitOrder` 和 :class:`~MarketOrder`
+    :param price_or_style: 默认为None，表示市价单，可设置价格，表示限价单，也可以直接设置订单类型，有如下选项：MarketOrder、LimitOrder、
+                            TWAPOrder、VWAPOrder
 
     :example:
 
     .. code-block:: python
 
         #花费最多￥10000买入平安银行股票，并以市价单发送。具体下单的数量与您策略税费相关的配置有关。
         order_value('000001.XSHE', 10000)
-        #卖出价值￥10000的现在持有的平安银行：
-        order_value('000001.XSHE', -10000)
+        #卖出价值￥10000的现在持有的平安银行, 以10￥价格发出限价单：
+        order_value('000001.XSHE', -10000, price_or_style=10)
     """
     raise NotImplementedError
 
 
 @export_as_api
 @ExecutionContext.enforce_phase(
     EXECUTION_PHASE.OPEN_AUCTION,
     EXECUTION_PHASE.ON_BAR,
     EXECUTION_PHASE.ON_TICK,
     EXECUTION_PHASE.SCHEDULED,
     EXECUTION_PHASE.GLOBAL
 )
 @apply_rules(
     verify_that('percent', pre_check=True).is_number().is_greater_or_equal_than(-1).is_less_or_equal_than(1),
-    verify_that('style').is_instance_of((MarketOrder, LimitOrder, type(None)))
+    *common_rules
 )
 @instype_singledispatch
-def order_percent(id_or_ins, percent, price=None, style=None):
-    # type: (Union[str, Instrument], float, Optional[float], Optional[OrderStyle]) -> Optional[Order]
+def order_percent(id_or_ins, percent, price=None, style=None, price_or_style=None):
+    # type: (Union[str, Instrument], float, Optional[float], Optional[OrderStyle], PRICE_OR_STYLE_TYPE) -> Optional[Order]
     """
-    发送一个花费价值等于目前投资组合（市场价值和目前现金的总和）一定百分比现金的买/卖单，正数代表买，负数代表卖。股票的股数总是会被调整成对应的一手的股票数的倍数（1手是100股）。百分比是一个小数，并且小于或等于1（<=100%），0.5表示的是50%.需要注意，如果资金不足，该API将不会创建发送订单。
+    发送一个花费价值等于目前投资组合（市场价值和目前现金的总和）一定百分比现金的买/卖单，正数代表买，负数代表卖。股票的股数总是会被调整成对应的一手的股票数的倍数（1手是100股）。百分比是一个小数，并且小于或等于1（<=100%），0.5表示的是50%.需要注意，如果资金不足，该API将会使用最大可用资金发单。
 
     需要注意：
 
     发送买单时，percent 代表的是期望买入股票消耗的金额（包含税费）占投资组合总权益的比例。
     发送卖单时，percent 代表的是期望卖出的股票总价值占投资组合总权益的比例。
 
     :param id_or_ins: 下单标的物
     :param percent: 占有现有的投资组合价值的百分比。正数表示买入，负数表示卖出。
     :param price: 下单价格，默认为None，表示 :class:`~MarketOrder`, 此参数主要用于简化 `style` 参数。
     :param style: 下单类型, 默认是市价单。目前支持的订单类型有 :class:`~LimitOrder` 和 :class:`~MarketOrder`
+    :param price_or_style: 默认为None，表示市价单，可设置价格，表示限价单，也可以直接设置订单类型，有如下选项：MarketOrder、LimitOrder、
+                            TWAPOrder、VWAPOrder
 
     :example:
 
     .. code-block:: python
 
         #花费等于现有投资组合50%价值的现金买入平安银行股票：
         order_percent('000001.XSHG', 0.5)
+        #花费等于现有投资组合50%价值的现金买入平安银行股票, 以10￥限价单：
+        order_percent('000001.XSHG', 0.5, price_or_style=10)
     """
     raise NotImplementedError
 
 
 @export_as_api
 @ExecutionContext.enforce_phase(
     EXECUTION_PHASE.OPEN_AUCTION,
     EXECUTION_PHASE.ON_BAR,
     EXECUTION_PHASE.ON_TICK,
     EXECUTION_PHASE.SCHEDULED,
     EXECUTION_PHASE.GLOBAL
 )
 @apply_rules(
     verify_that('cash_amount').is_number(),
-    verify_that('style').is_instance_of((MarketOrder, LimitOrder, type(None)))
+    *common_rules
 )
 @instype_singledispatch
-def order_target_value(id_or_ins, cash_amount, price=None, style=None):
-    # type: (Union[str, Instrument], float, Optional[float], Optional[OrderStyle]) -> Optional[Order]
+def order_target_value(id_or_ins, cash_amount, price=None, style=None, price_or_style=None):
+    # type: (Union[str, Instrument], float, Optional[float], Optional[OrderStyle], TUPLE_PRICE_OR_STYLE_TYPE) -> Optional[Order]
     """
     买入/卖出并且自动调整该证券的仓位到一个目标价值。
     加仓时，cash_amount 代表现有持仓的价值加上即将花费（包含税费）的现金的总价值。
     减仓时，cash_amount 代表调整仓位的目标价至。
 
-    需要注意，如果资金不足，该API将不会创建发送订单。
+    需要注意，如果资金不足，该API将会使用最大可用资金发单。
 
     :param id_or_ins: 下单标的物
     :param cash_amount: 最终的该证券的仓位目标价值。
     :param price: 下单价格，默认为None，表示 :class:`~MarketOrder`, 此参数主要用于简化 `style` 参数。
     :param style: 下单类型, 默认是市价单。目前支持的订单类型有 :class:`~LimitOrder` 和 :class:`~MarketOrder`
+    :param price_or_style: 默认为None，表示市价单，可设置价格，表示限价单，也可以直接设置订单类型，有如下选项：MarketOrder、LimitOrder、
+                            TWAPOrder、VWAPOrder
 
     :example:
 
     .. code-block:: python
 
         #如果现在的投资组合中持有价值￥3000的平安银行股票的仓位，以下代码范例会发送花费 ￥7000 现金的平安银行买单到市场。（向下调整到最接近每手股数即100的倍数的股数）：
         order_target_value('000001.XSHE', 10000)
+        #如果现在的投资组合中持有价值￥3000的平安银行股票的仓位，以下代码范例会发送10￥限价单共花费 ￥7000 现金的平安银行买单到市场
+        #或者如果现在的投资组合中持有价值￥13000的平安银行股票的仓位，以下代码范例会发送11￥限价单共花费 ￥3000 现金的平安银行卖单到市场
+        order_target_value('000001.XSHE', 10000, price_or_style=(10, 11)
     """
     raise NotImplementedError
 
 
 @export_as_api
 @ExecutionContext.enforce_phase(
     EXECUTION_PHASE.OPEN_AUCTION,
     EXECUTION_PHASE.ON_BAR,
     EXECUTION_PHASE.ON_TICK,
     EXECUTION_PHASE.SCHEDULED,
     EXECUTION_PHASE.GLOBAL
 )
 @apply_rules(
     verify_that('percent', pre_check=True).is_number().is_greater_or_equal_than(0).is_less_or_equal_than(1),
-    verify_that('style').is_instance_of((MarketOrder, LimitOrder, type(None)))
+    *common_rules
 )
 @instype_singledispatch
-def order_target_percent(id_or_ins, percent, price=None, style=None):
-    # type: (Union[str, Instrument], float, Optional[float], Optional[OrderStyle]) -> Optional[Order]
+def order_target_percent(id_or_ins, percent, price=None, style=None, price_or_style=None):
+    # type: (Union[str, Instrument], float, Optional[float], Optional[OrderStyle], TUPLE_PRICE_OR_STYLE_TYPE) -> Optional[Order]
     """
     买入/卖出证券以自动调整该证券的仓位到占有一个目标价值。
 
     加仓时，percent 代表证券已有持仓的价值加上即将花费的现金（包含税费）的总值占当前投资组合总价值的比例。
     减仓时，percent 代表证券将被调整到的目标价至占当前投资组合总价值的比例。
 
     其实我们需要计算一个position_to_adjust (即应该调整的仓位)
@@ -208,81 +241,90 @@
 
     另外，如果您希望大量调整股票仓位，推荐使用 order_target_portfolio 而非在循环中调取 order_target_percent，前者将拥有更好的性能。
 
     :param id_or_ins: 下单标的物
     :param percent: 仓位最终所占投资组合总价值的目标百分比。
     :param price: 下单价格，默认为None，表示 :class:`~MarketOrder`, 此参数主要用于简化 `style` 参数。
     :param style: 下单类型, 默认是市价单。目前支持的订单类型有 :class:`~LimitOrder` 和 :class:`~MarketOrder`
+    :param price_or_style: 默认为None，表示市价单，可设置价格，表示限价单，也可以直接设置订单类型，有如下选项：MarketOrder、LimitOrder、
+                            TWAPOrder、VWAPOrder
 
     :example:
 
     .. code-block:: python
 
         #如果投资组合中已经有了平安银行股票的仓位，并且占据目前投资组合的10%的价值，那么以下代码会消耗相当于当前投资组合价值5%的现金买入平安银行股票：
         order_target_percent('000001.XSHE', 0.15)
+        #如果投资组合中已经有了平安银行股票的仓位，并且占据目前投资组合的10%的价值，那么以下代码会消耗相当于当前投资组合价值5%的现金以10￥限价单买入平安银行股票：
+        #或者如果投资组合中已经有了平安银行股票的仓位，并且占据目前投资组合的20%的价值，那么以下代码会消耗相当于当前投资组合价值5%的现金以11￥限价单卖出平安银行股票：
+        order_target_percent('000001.XSHE', 0.15, price_or_style=(10, 11))
     """
     raise NotImplementedError
 
 
 @export_as_api
 @ExecutionContext.enforce_phase(
     EXECUTION_PHASE.OPEN_AUCTION,
     EXECUTION_PHASE.ON_BAR,
     EXECUTION_PHASE.ON_TICK,
     EXECUTION_PHASE.SCHEDULED,
     EXECUTION_PHASE.GLOBAL
 )
 @apply_rules(
     verify_that('amount', pre_check=True).is_number().is_greater_or_equal_than(0),
-    verify_that('style').is_instance_of((MarketOrder, LimitOrder, type(None)))
+    *common_rules
 )
 @instype_singledispatch
-def buy_open(id_or_ins, amount, price=None, style=None):
-    # type: (Union[str, Instrument], int, Optional[float], Optional[OrderStyle]) -> Union[Order, List[Order], None]
+def buy_open(id_or_ins, amount, price=None, style=None, price_or_style=None):
+    # type: (Union[str, Instrument], int, Optional[float], Optional[OrderStyle], PRICE_OR_STYLE_TYPE) -> Union[Order, List[Order], None]
     """
     买入开仓。
 
     :param id_or_ins: 下单标的物
     :param amount: 下单手数
     :param price: 下单价格，默认为None，表示 :class:`~MarketOrder`, 此参数主要用于简化 `style` 参数。
     :param style: 下单类型, 默认是市价单。目前支持的订单类型有 :class:`~LimitOrder` 和 :class:`~MarketOrder`
+    :param price_or_style: 默认为None，表示市价单，可设置价格，表示限价单，也可以直接设置订单类型，有如下选项：MarketOrder、LimitOrder、
+                            TWAPOrder、VWAPOrder
 
     :example:
 
     .. code-block:: python
 
         #以价格为3500的限价单开仓买入2张上期所AG1607合约：
-        buy_open('AG1607', amount=2, price=3500))
+        buy_open('AG1607', amount=2, price_or_style=3500))
     """
     raise NotImplementedError
 
 
 @export_as_api
 @ExecutionContext.enforce_phase(
     EXECUTION_PHASE.OPEN_AUCTION,
     EXECUTION_PHASE.ON_BAR,
     EXECUTION_PHASE.ON_TICK,
     EXECUTION_PHASE.SCHEDULED,
     EXECUTION_PHASE.GLOBAL
 )
 @apply_rules(
     verify_that('amount', pre_check=True).is_number().is_greater_or_equal_than(0),
-    verify_that('style').is_instance_of((MarketOrder, LimitOrder, type(None)))
+    *common_rules
 )
 @instype_singledispatch
-def buy_close(id_or_ins, amount, price=None, style=None, close_today=False):
-    # type: (Union[str, Instrument], int, Optional[float], Optional[OrderStyle], Optional[bool]) -> Union[Order, List[Order], None]
+def buy_close(id_or_ins, amount, price=None, style=None, price_or_style=None, close_today=False):
+    # type: (Union[str, Instrument], int, Optional[float], Optional[OrderStyle], PRICE_OR_STYLE_TYPE, Optional[bool]) -> Union[Order, List[Order], None]
     """
     平卖仓
 
     :param id_or_ins: 下单标的物
     :param amount: 下单手数
     :param price: 下单价格，默认为None，表示 :class:`~MarketOrder`, 此参数主要用于简化 `style` 参数。
     :param style: 下单类型, 默认是市价单。目前支持的订单类型有 :class:`~LimitOrder` 和 :class:`~MarketOrder`
     :param close_today: 是否指定发平今仓单，默认为False，发送平仓单
+    :param price_or_style: 默认为None，表示市价单，可设置价格，表示限价单，也可以直接设置订单类型，有如下选项：MarketOrder、LimitOrder、
+                            TWAPOrder、VWAPOrder
 
     :example:
 
     .. code-block:: python
 
         #市价单将现有IF1603空仓买入平仓2张：
         buy_close('IF1603', 2)
@@ -296,62 +338,83 @@
     EXECUTION_PHASE.ON_BAR,
     EXECUTION_PHASE.ON_TICK,
     EXECUTION_PHASE.SCHEDULED,
     EXECUTION_PHASE.GLOBAL
 )
 @apply_rules(
     verify_that('amount', pre_check=True).is_number().is_greater_or_equal_than(0),
-    verify_that('style').is_instance_of((MarketOrder, LimitOrder, type(None)))
+    *common_rules
 )
 @instype_singledispatch
-def sell_open(id_or_ins, amount, price=None, style=None):
-    # type: (Union[str, Instrument], int, Optional[float], Optional[OrderStyle]) -> Union[Order, List[Order], None]
+def sell_open(id_or_ins, amount, price=None, style=None, price_or_style=None):
+    # type: (Union[str, Instrument], int, Optional[float], Optional[OrderStyle], PRICE_OR_STYLE_TYPE) -> Union[Order, List[Order], None]
     """
     卖出开仓
 
     :param id_or_ins: 下单标的物
     :param amount: 下单手数
     :param price: 下单价格，默认为None，表示 :class:`~MarketOrder`, 此参数主要用于简化 `style` 参数。
     :param style: 下单类型, 默认是市价单。目前支持的订单类型有 :class:`~LimitOrder` 和 :class:`~MarketOrder`
+    :param price_or_style: 默认为None，表示市价单，可设置价格，表示限价单，也可以直接设置订单类型，有如下选项：MarketOrder、LimitOrder、
+                            TWAPOrder、VWAPOrder
+
+    :example:
+
+    .. code-block:: python
+
+        # 以3100发出限价单将现有IF1603卖出开仓2张：
+        sell_open('IF1603', 2, price_or_style=3100)
+
     """
     raise NotImplementedError
 
 
 @export_as_api
 @ExecutionContext.enforce_phase(
     EXECUTION_PHASE.OPEN_AUCTION,
     EXECUTION_PHASE.ON_BAR,
     EXECUTION_PHASE.ON_TICK,
     EXECUTION_PHASE.SCHEDULED,
     EXECUTION_PHASE.GLOBAL
 )
 @apply_rules(
     verify_that('amount', pre_check=True).is_number().is_greater_or_equal_than(0),
-    verify_that('style').is_instance_of((MarketOrder, LimitOrder, type(None)))
+    *common_rules
 )
 @instype_singledispatch
-def sell_close(id_or_ins, amount, price=None, style=None, close_today=False):
-    # type: (Union[str, Instrument], float, Optional[float], Optional[OrderStyle], Optional[bool]) -> Union[Order, List[Order], None]
+def sell_close(id_or_ins, amount, price=None, style=None, price_or_style=None, close_today=False):
+    # type: (Union[str, Instrument], float, Optional[float], Optional[OrderStyle], PRICE_OR_STYLE_TYPE, Optional[bool]) -> Union[Order, List[Order], None]
     """
     平买仓
 
     :param id_or_ins: 下单标的物
     :param amount: 下单手数
     :param price: 下单价格，默认为None，表示 :class:`~MarketOrder`, 此参数主要用于简化 `style` 参数。
     :param style: 下单类型, 默认是市价单。目前支持的订单类型有 :class:`~LimitOrder` 和 :class:`~MarketOrder`
     :param close_today: 是否指定发平今仓单，默认为False，发送平仓单
+    :param price_or_style: 默认为None，表示市价单，可设置价格，表示限价单，也可以直接设置订单类型，有如下选项：MarketOrder、LimitOrder、
+                            TWAPOrder、VWAPOrder
+
+    :example:
+
+    .. code-block:: python
+
+        # 以市价单单将现有IF1603买入平仓2张：
+        sell_close('IF1603', 2, price_or_style=MarketOrder())
+
+
     """
     raise NotImplementedError
 
 
 @export_as_api
-@apply_rules(verify_that("quantity").is_number())
+@apply_rules(verify_that("quantity").is_number(), *common_rules)
 @instype_singledispatch
-def order(order_book_id, quantity, price=None, style=None):
-    # type: (Union[str, Instrument], int, Optional[float], Optional[OrderStyle]) -> List[Order]
+def order(order_book_id, quantity, price=None, style=None, price_or_style=None):
+    # type: (Union[str, Instrument], int, Optional[float], Optional[OrderStyle], PRICE_OR_STYLE_TYPE) -> List[Order]
     """
       全品种通用智能调仓函数
 
       如果不指定 price, 则相当于下 MarketOrder
 
       如果 order_book_id 是股票，等同于调用 order_shares
 
@@ -361,14 +424,16 @@
           *   如果 quantity 为正数，则先平 Sell 方向仓位，再开 Buy 方向仓位
           *   如果 quantity 为负数，则先平 Buy 反向仓位，再开 Sell 方向仓位
 
       :param order_book_id: 下单标的物
       :param quantity: 调仓量
       :param price: 下单价格
       :param style: 下单类型, 默认是市价单。目前支持的订单类型有 :class:`~LimitOrder` 和 :class:`~MarketOrder`
+      :param price_or_style: 默认为None，表示市价单，可设置价格，表示限价单，也可以直接设置订单类型，有如下选项：MarketOrder、LimitOrder、
+                            TWAPOrder、VWAPOrder
 
       :example:
 
       ..  code-block:: python3
           :linenos:
 
           # 当前仓位为0
@@ -379,18 +444,18 @@
           order('RB1710', -3)
 
     """
     raise NotImplementedError
 
 
 @export_as_api
-@apply_rules(verify_that("quantity").is_number())
+@apply_rules(verify_that("quantity").is_number(), *common_rules)
 @instype_singledispatch
-def order_to(order_book_id, quantity, price=None, style=None):
-    # type: (Union[str, Instrument], int, Optional[float], Optional[OrderStyle]) -> List[Order]
+def order_to(order_book_id, quantity, price=None, style=None, price_or_style=None):
+    # type: (Union[str, Instrument], int, Optional[float], Optional[OrderStyle], PRICE_OR_STYLE_TYPE) -> List[Order]
     """
     全品种通用智能调仓函数
 
     如果不指定 price, 则相当于 MarketOrder
 
     如果 order_book_id 是股票，则表示仓位调整到多少股
 
@@ -400,14 +465,17 @@
         *   quantity 如果为正数，则先平 SELL 方向仓位，再 BUY 方向开仓 quantity 手
         *   quantity 如果为负数，则先平 BUY 方向仓位，再 SELL 方向开仓 -quantity 手
 
     :param order_book_id: 下单标的物
     :param int quantity: 调仓量
     :param float price: 下单价格
     :param style: 下单类型, 默认是市价单。目前支持的订单类型有 :class:`~LimitOrder` 和 :class:`~MarketOrder`
+    :param price_or_style: 默认为None，表示市价单，可设置价格，表示限价单，也可以直接设置订单类型，有如下选项：MarketOrder、LimitOrder、
+                            TWAPOrder、VWAPOrder
+
     :example:
 
     ..  code-block:: python3
         :linenos:
 
         # 当前仓位为0
         # RB1710 调仓至 BUY 2手
```

### Comparing `rqalpha-4.9.2/rqalpha/apis/api_base.py` & `rqalpha-5.0.0/rqalpha/apis/api_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,23 +35,25 @@
 from rqalpha.utils.logger import user_log as logger, user_system_log, user_print
 from rqalpha.model.instrument import Instrument
 from rqalpha.model.tick import TickObject
 from rqalpha.const import (
     EXECUTION_PHASE, ORDER_STATUS, SIDE, POSITION_EFFECT, ORDER_TYPE, MATCHING_TYPE, RUN_TYPE, POSITION_DIRECTION,
     DEFAULT_ACCOUNT_TYPE
 )
-from rqalpha.model.order import Order, MarketOrder, LimitOrder, OrderStyle
+from rqalpha.model.order import Order, MarketOrder, LimitOrder, OrderStyle, VWAPOrder, TWAPOrder
 from rqalpha.core.events import EVENT, Event
 from rqalpha.core.strategy_context import StrategyContext
 from rqalpha.portfolio.position import Position
 
 export_as_api(logger, name='logger')
 export_as_api(user_print, name='print')
 export_as_api(LimitOrder, name='LimitOrder')
 export_as_api(MarketOrder, name='MarketOrder')
+export_as_api(VWAPOrder, name='VWAPOrder')
+export_as_api(TWAPOrder, name='TWAPOrder')
 export_as_api(ORDER_STATUS, name='ORDER_STATUS')
 export_as_api(SIDE, name='SIDE')
 export_as_api(POSITION_EFFECT, name='POSITION_EFFECT')
 export_as_api(POSITION_DIRECTION, name='POSITION_DIRECTION')
 export_as_api(ORDER_TYPE, name='ORDER_TYPE')
 export_as_api(RUN_TYPE, name='RUN_TYPE')
 export_as_api(MATCHING_TYPE, name='MATCHING_TYPE')
@@ -67,34 +69,48 @@
         raise RQInvalidArgument(_(u"unsupported order_book_id type"))
 
 
 def assure_order_book_id(id_or_ins):
     return assure_instrument(id_or_ins).order_book_id
 
 
-def cal_style(price, style):
-    if price is None and style is None:
+def cal_style(price, style, price_or_style=None):
+    if price_or_style is None:
+        if price:
+            price_or_style = price
+        if style:
+            price_or_style = style
+
+    if price_or_style is None:
         return MarketOrder()
 
-    if style is not None:
-        if not isinstance(style, OrderStyle):
-            raise RuntimeError
-        return style
-
-    if isinstance(price, OrderStyle):
-        # 为了 order_xxx('RB1710', 10, MarketOrder()) 这种写法
-        if isinstance(price, LimitOrder):
-            if np.isnan(price.get_limit_price()):
-                raise RQInvalidArgument(_(u"Limit order price should not be nan."))
-        return price
+    if not isinstance(price_or_style, (int, float, OrderStyle)):
+        raise RQInvalidArgument(f"price or style or price_or_style type no support. {price_or_style}")
+
+    if isinstance(price_or_style, OrderStyle):
+        return price_or_style
+
+    return LimitOrder(price_or_style)
 
-    if np.isnan(price):
-        raise RQInvalidArgument(_(u"Limit order price should not be nan."))
 
-    return LimitOrder(price)
+def calc_open_close_style(price, style, price_or_style):
+    if isinstance(price_or_style, tuple):
+        _length = len(price_or_style)
+        if _length == 0:
+            o, c = None, None
+        elif _length == 1:
+            o, c = price_or_style[0], price_or_style[0]
+        else:
+            o, c = price_or_style[0], price_or_style[1]
+        open_style = cal_style(price, style, o)
+        close_style = cal_style(price, style, c)
+    else:
+        open_style = cal_style(price, style, price_or_style)
+        close_style = open_style
+    return open_style, close_style
 
 
 @export_as_api
 @ExecutionContext.enforce_phase(
     EXECUTION_PHASE.BEFORE_TRADING,
     EXECUTION_PHASE.OPEN_AUCTION,
     EXECUTION_PHASE.ON_BAR,
@@ -242,17 +258,21 @@
     EXECUTION_PHASE.SCHEDULED,
 )
 @apply_rules(verify_that("id_or_symbols").are_valid_instruments())
 def subscribe(id_or_symbols):
     # type: (Union[str, Instrument, Iterable[str], Iterable[Instrument]]) -> None
 
     """
-    订阅合约行情。该操作会导致合约池内合约的增加，从而影响handle_bar中处理bar数据的数量。
+    订阅合约行情。
+
+    在日级别回测中不需要订阅合约。
+
+    在分钟回测中，若策略只设置了股票账户则不需要订阅合约；若设置了期货账户，则需要订阅策略关注的期货合约，框架会根据订阅的期货合约品种触发对应交易时间的 handle_bar。为了方便起见，也可以以直接订阅主力连续合约。
 
-    需要注意，用户在初次编写策略时候需要首先订阅合约行情，否则handle_bar不会被触发。
+    在 tick 回测中，策略需要订阅每一个关注的股票/期货合约，框架会根据订阅池触发对应标的的 handle_tick。
 
     :param id_or_symbols: 标的物
 
     """
     current_universe = Environment.get_instance().get_universe()
     if isinstance(id_or_symbols, six.string_types):
         order_book_id = instruments(id_or_symbols).order_book_id
@@ -505,15 +525,15 @@
 @apply_rules(
     verify_that("order_book_id", pre_check=True).is_listed_instrument(),
     verify_that('count').is_instance_of(int).is_greater_than(0)
 )
 def history_ticks(order_book_id, count):
     # type: (str, int) -> List[TickObject]
     """
-    获取指定合约历史 tick 对象，仅支持在 tick 级别的策略（回测、模拟交易、实盘）中调用
+    获取指定合约历史（不晚于当前时间的）tick 对象，仅支持在 tick 级别的策略（回测、模拟交易、实盘）中调用。
 
     :param order_book_id: 合约代码
     :param count: 获取的 tick 数量
 
     """
     env = Environment.get_instance()
     sys_frequency = env.config.base.frequency
@@ -857,25 +877,25 @@
 @ExecutionContext.enforce_phase(
     EXECUTION_PHASE.OPEN_AUCTION,
     EXECUTION_PHASE.ON_BAR,
     EXECUTION_PHASE.ON_TICK,
     EXECUTION_PHASE.SCHEDULED,
     EXECUTION_PHASE.GLOBAL
 )
-def deposit(account_type, amount):
-    # type: (str, float) -> None
+def deposit(account_type: str, amount: float, receiving_days: int = 0):
     """
     入金（增加账户资金）
 
     :param account_type: 账户类型
-    :param amount: 增加金额
+    :param amount: 入金金额
+    :param receiving_days: 入金到账天数，0 表示立刻到账，1 表示资金在下一个交易日盘前到账
     :return: None
     """
     env = Environment.get_instance()
-    return env.portfolio.deposit_withdraw(account_type, amount)
+    return env.portfolio.deposit_withdraw(account_type, amount, receiving_days)
 
 
 @export_as_api
 @ExecutionContext.enforce_phase(
     EXECUTION_PHASE.OPEN_AUCTION,
     EXECUTION_PHASE.ON_BAR,
     EXECUTION_PHASE.ON_TICK,
@@ -893,7 +913,56 @@
 
     :param account_type: 账户类型
     :param amount: 减少金额
     :return: None
     """
     env = Environment.get_instance()
     return env.portfolio.deposit_withdraw(account_type, amount * -1)
+
+
+@export_as_api
+@ExecutionContext.enforce_phase(
+    EXECUTION_PHASE.OPEN_AUCTION,
+    EXECUTION_PHASE.ON_BAR,
+    EXECUTION_PHASE.ON_TICK,
+    EXECUTION_PHASE.SCHEDULED,
+    EXECUTION_PHASE.GLOBAL
+)
+@apply_rules(
+    verify_that("account_type").is_in(DEFAULT_ACCOUNT_TYPE),
+    verify_that("amount", pre_check=True).is_instance_of((int, float)).is_greater_than(0),
+)
+def finance(amount, account_type=DEFAULT_ACCOUNT_TYPE.STOCK):
+    """
+    融资
+
+    :param amount: 融资金额
+    :param account_type: 融资账户
+    :return: None
+    """
+    env = Environment.get_instance()
+    return env.portfolio.finance_repay(amount, account_type)
+
+
+@export_as_api
+@ExecutionContext.enforce_phase(
+    EXECUTION_PHASE.OPEN_AUCTION,
+    EXECUTION_PHASE.ON_BAR,
+    EXECUTION_PHASE.ON_TICK,
+    EXECUTION_PHASE.SCHEDULED,
+)
+@apply_rules(
+    verify_that("account_type").is_in(DEFAULT_ACCOUNT_TYPE),
+    verify_that("amount", pre_check=True).is_instance_of((int, float)).is_greater_than(0),
+)
+def repay(amount, account_type=DEFAULT_ACCOUNT_TYPE.STOCK):
+    """
+    还款
+
+    :param amount: 还款金额
+    :param account_type: 还款账户
+    :return: None
+    """
+    env = Environment.get_instance()
+    return env.portfolio.finance_repay(amount * -1, account_type)
+
+
```

### Comparing `rqalpha-4.9.2/rqalpha/apis/api_rqdatac.py` & `rqalpha-5.0.0/rqalpha/apis/api_rqdatac.py`

 * *Files 3% similar despite different names*

```diff
@@ -231,14 +231,78 @@
     env = Environment.get_instance()
     dt = env.trading_dt.date()
 
     return rqdatac.concept(*concept_names, date=dt)
 
 
 @export_as_api
+def get_margin_stocks(exchange=None, margin_type="all"):
+    # type: (str, str) -> List[str]
+    """
+    获取某个日期深证、上证融资融券股票列表。
+
+    :param exchange: 交易所，默认为 None，返回所有字段。可选字段包括：'XSHE', 'sz' 代表深交所；'XSHG', 'sh' 代表上交所
+    :param margin_type: 'stock' 代表融券卖出，'cash'，代表融资买入，'all'，代表包含融资和融券，默认为'all'
+    :return: 属于该概念的股票 order_book_id
+
+    :example:
+
+    获取沪深市场的融券卖出列表:
+
+    .. code-block:: python3
+        :linenos:
+
+        get_margin_stocks(exchange=None,margin_type='stock')
+        # [Out]
+        # ['000001.XSHE',
+        # '000002.XSHE',
+        # '000006.XSHE',
+        # ...]
+
+    获取沪深市场融资买入列表:
+
+    .. code-block::
+        :linenos:
+
+        get_margin_stocks(exchange='XSHE',margin_type='stock')
+        # [Out]
+        # ['000001.XSHE',
+        # '000002.XSHE',
+        # '000006.XSHE',
+        # ...]
+
+    获取上证融资买入列表:
+
+    .. code-block::
+        :linenos:
+
+        get_margin_stocks(exchange='XSHG',margin_type='cash')
+        # [Out]
+        # ['510050.XSHG',
+        # '510160.XSHG',
+        # '510180.XSHG',
+        # ...]
+
+    """
+    trade_dt = Environment.get_instance().trading_dt.date()
+
+    symbols = []
+
+    if margin_type == "all":
+        symbols.extend(rqdatac.get_margin_stocks(trade_dt, exchange, margin_type="stock", market="cn"))
+        symbols.extend(rqdatac.get_margin_stocks(trade_dt, exchange, margin_type="cash", market="cn"))
+    elif margin_type in ["cash", "stock"]:
+        symbols.extend(rqdatac.get_margin_stocks(trade_dt, exchange, margin_type=margin_type, market="cn"))
+    else:
+        raise ValueError("MarginComponentValidator margin_type value error, got {}".format(margin_type))
+
+    return list(set(symbols))
+
+
+@export_as_api
 @ExecutionContext.enforce_phase(
     EXECUTION_PHASE.ON_INIT,
     EXECUTION_PHASE.BEFORE_TRADING,
     EXECUTION_PHASE.OPEN_AUCTION,
     EXECUTION_PHASE.AFTER_TRADING,
     EXECUTION_PHASE.SCHEDULED
 )
@@ -1090,14 +1154,25 @@
         result = result.set_index(['order_book_id', 'end_date']).sort_index()
     return result
 
 
 @export_as_api
 @apply_rules(verify_that('statements').is_in(['all', 'latest'], ignore_none=True))
 def get_pit_financials_ex(order_book_ids, fields, count, statements='latest'):
+    # type: (Union[str, List[str]], Union[str, List[str]], int, str) -> Optional[pd.DataFrame]
+    """
+    以给定一个报告期回溯的方式获取季度基础财务数据（三大表），即利润表（income_statement），资产负债表（balance_sheet），现金流量表（cash_flow_statement)。
+
+    :param order_book_ids: 合约代码，可传入order_book_id, order_book_id list，这里输入的是A股编码
+    :param fields: 需要返回的财务字段
+    :param count: 几条数据
+    :param statements: 设置 statements 为 all 时返回所有记录，statements 等于 latest 时返回最新的一条记录，默认为 latest.
+
+    :return:
+    """
     if isinstance(order_book_ids, str):
         order_book_ids = [order_book_ids]
     env = Environment.get_instance()
 
     if count < 0:
         user_log.warn("function get_pit_financials_ex : count must >= 0")
         return None
```

### Comparing `rqalpha-4.9.2/rqalpha/apis/names.py` & `rqalpha-5.0.0/rqalpha/apis/names.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/cmds/__init__.py` & `rqalpha-5.0.0/rqalpha/cmds/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/cmds/bundle.py` & `rqalpha-5.0.0/rqalpha/cmds/bundle.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import time
 import datetime
 import dateutil
 
 import click
 import requests
 import six
+import h5py
 
 from rqalpha.utils.i18n import gettext as _
 
 from rqalpha.cmds.entry import cli
 from rqalpha.utils import init_rqdatac_env
 
 
@@ -119,14 +120,20 @@
     tar = tarfile.open(tmp, 'r:bz2')
     tar.extractall(data_bundle_path)
     tar.close()
     os.remove(tmp)
     six.print_(_(u"Data bundle download successfully in {bundle_path}").format(bundle_path=data_bundle_path))
 
 
+@cli.command(help=_("Check bundle"))
+@click.option('-d', '--data-bundle-path', default=os.path.expanduser('~/.rqalpha'), type=click.Path(file_okay=False))
+def check_bundle(data_bundle_path):
+    check_bundle_data(os.path.join(data_bundle_path, "bundle"))
+
+
 CDN_URL = 'http://bundle.assets.ricequant.com/bundles_v4/rqbundle_%04d%02d.tar.bz2'
 
 
 def get_exactly_url():
     day = datetime.date.today()
     proxy_uri = os.environ.get('RQALPHA_PROXY')
     while True:  # get exact url
@@ -157,7 +164,38 @@
                     return True  # Download complete . exit
             except requests.exceptions.RequestException:
                 if i < retry_times - 1:
                     six.print_(_("\nDownload failed, retry in {} seconds.".format(retry_interval)))
                     time.sleep(retry_interval)
                 else:
                     raise
+
+
+def check_bundle_data(data_bundle_path):
+    instruments = ["stocks", "indexes", "futures", "funds"]
+    corrupt_files, not_exists_instruments = [], []
+    for instrument in instruments:
+        file = os.path.join(data_bundle_path, "{}.h5".format(instrument))
+        if not os.path.exists(file):
+            not_exists_instruments.append(instrument)
+            continue
+        try:
+            with h5py.File(file, mode="r") as f:
+                for order_book_id in f.keys():
+                    __ = f[order_book_id][:1]
+        except Exception:
+            corrupt_files.append(file)
+    if len(corrupt_files):
+        click.echo("{}:\n{}".format(_("corrupted files"), corrupt_files))
+        is_ok = input("{}(yes/no):".format(_("remove files"))).lower()
+        if is_ok in ["yes", "y"]:
+            [os.remove(file) for file in corrupt_files]
+            click.echo(_("remove success"))
+        elif is_ok in ["no", "n"]:
+            click.echo(_("corrupted files not remove"))
+        else:
+            click.echo(_("input error"))
+    elif len(not_exists_instruments):
+        click.echo(_("bundle's day bar is incomplete, please update bundle"))
+    else:
+        click.echo(_("good bundle's day bar"))
+
```

### Comparing `rqalpha-4.9.2/rqalpha/cmds/entry.py` & `rqalpha-5.0.0/rqalpha/cmds/entry.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/cmds/misc.py` & `rqalpha-5.0.0/rqalpha/cmds/misc.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/cmds/mod.py` & `rqalpha-5.0.0/rqalpha/cmds/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/cmds/run.py` & `rqalpha-5.0.0/rqalpha/cmds/run.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/config.yml` & `rqalpha-5.0.0/rqalpha/config.yml`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/const.py` & `rqalpha-5.0.0/rqalpha/const.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,14 +90,20 @@
     NEXT_TICK_BEST_COUNTERPARTY = "NEXT_TICK_BEST_COUNTERPARTY"
 
 
 # noinspection PyPep8Naming
 class ORDER_TYPE(CustomEnum):
     MARKET = "MARKET"
     LIMIT = "LIMIT"
+    ALGO = "ALGO"
+
+
+class ALGO(CustomEnum):
+    TWAP = "TWAP"
+    VWAP = "VWAP"
 
 
 # noinspection PyPep8Naming
 class ORDER_STATUS(CustomEnum):
     PENDING_NEW = "PENDING_NEW"        # 待报
     ACTIVE = "ACTIVE"                  # 已报/部成
     FILLED = "FILLED"                  # 已成
@@ -142,14 +148,15 @@
     CS = "CS"
     FUTURE = "Future"
     OPTION = "Option"
     ETF = "ETF"
     LOF = "LOF"
     INDX = "INDX"
     PUBLIC_FUND = 'PublicFund'
+    FUND = "Fund"
     BOND = "Bond"
     CONVERTIBLE = "Convertible"
     SPOT = "Spot"
     REPO = "Repo"
 
 
 # noinspection PyPep8Naming
```

### Comparing `rqalpha-4.9.2/rqalpha/core/__init__.py` & `rqalpha-5.0.0/rqalpha/core/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/core/events.py` & `rqalpha-5.0.0/rqalpha/core/events.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/core/execution_context.py` & `rqalpha-5.0.0/rqalpha/core/execution_context.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/core/executor.py` & `rqalpha-5.0.0/rqalpha/core/executor.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/core/global_var.py` & `rqalpha-5.0.0/rqalpha/core/global_var.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/core/strategy.py` & `rqalpha-5.0.0/rqalpha/core/strategy.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/core/strategy_context.py` & `rqalpha-5.0.0/rqalpha/core/strategy_context.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,14 +41,20 @@
         self._margin_multiplier = config.base.margin_multiplier
         self._run_type = config.base.run_type
 
         try:
             self._matching_type = config.mod.sys_simulation.matching_type
             self._slippage = config.mod.sys_simulation.slippage
             self._commission_multiplier = config.mod.sys_transaction_cost.commission_multiplier
+            if config.mod.sys_transaction_cost.commission_multiplier:
+                self._stock_commission_multiplier = self._commission_multiplier
+                self._futures_commission_multiplier = self._commission_multiplier
+            else:
+                self._stock_commission_multiplier = config.mod.sys_transaction_cost.stock_commission_multiplier
+                self._futures_commission_multiplier = config.mod.sys_transaction_cost.futures_commission_multiplier
         except:
             pass
 
     @property
     def start_date(self):
         # type: () -> date
         """
@@ -109,14 +115,28 @@
         # type: () -> float
         """
         手续费倍率
         """
         return self._commission_multiplier
 
     @property
+    def stock_commission_multiplier(self):
+        """
+        股票手续费倍率
+        """
+        return self._stock_commission_multiplier
+
+    @property
+    def futures_commission_multiplier(self):
+        """
+        期货手续费倍率
+        """
+        return self._futures_commission_multiplier
+
+    @property
     def margin_multiplier(self):
         # type: () -> float
         """
         保证金倍率
         """
         return self._margin_multiplier
```

### Comparing `rqalpha-4.9.2/rqalpha/core/strategy_loader.py` & `rqalpha-5.0.0/rqalpha/core/strategy_loader.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/core/strategy_universe.py` & `rqalpha-5.0.0/rqalpha/core/strategy_universe.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/data/__init__.py` & `rqalpha-5.0.0/rqalpha/data/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/data/bar_dict_price_board.py` & `rqalpha-5.0.0/rqalpha/data/bar_dict_price_board.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/data/base_data_source/__init__.py` & `rqalpha-5.0.0/rqalpha/data/base_data_source/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/data/base_data_source/adjust.py` & `rqalpha-5.0.0/rqalpha/data/base_data_source/adjust.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/data/base_data_source/data_source.py` & `rqalpha-5.0.0/rqalpha/data/base_data_source/data_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,18 +87,20 @@
             INSTRUMENT_TYPE.LOF: funds_day_bar_store
         }  # type: Dict[INSTRUMENT_TYPE, AbstractDayBarStore]
 
         self._future_info_store = FutureInfoStore(_p("future_info.json"), custom_future_info)
 
         self._instruments_stores = {}  # type: Dict[INSTRUMENT_TYPE, AbstractInstrumentStore]
         self._ins_id_or_sym_type_map = {}  # type: Dict[str, INSTRUMENT_TYPE]
+        instruments = []
         with open(_p('instruments.pk'), 'rb') as f:
-            instruments = [Instrument(
-                i, lambda i: self._future_info_store.get_future_info(i)["tick_size"]
-            ) for i in pickle.load(f)]
+            for i in pickle.load(f):
+                if i["type"] == "Future" and Instrument.is_future_continuous_contract(i["order_book_id"]):
+                    i["listed_date"] = datetime(1990, 1, 1)
+                instruments.append(Instrument(i, lambda i: self._future_info_store.get_future_info(i)["tick_size"]))
         for ins_type in self.DEFAULT_INS_TYPES:
             self.register_instruments_store(InstrumentStore(instruments, ins_type))
 
         dividend_store = DividendStore(_p('dividends.h5'))
         self._dividends = {
             INSTRUMENT_TYPE.CS: dividend_store,
             INSTRUMENT_TYPE.ETF: dividend_store,
@@ -217,15 +219,18 @@
         return bars[pos]
 
     OPEN_AUCTION_BAR_FIELDS = ["datetime", "open", "limit_up", "limit_down", "volume", "total_turnover"]
 
     def get_open_auction_bar(self, instrument, dt):
         # type: (Instrument, Union[datetime, date]) -> Dict
         day_bar = self.get_bar(instrument, dt, "1d")
-        bar = {k: day_bar[k] if k in day_bar.dtype.names else np.nan for k in self.OPEN_AUCTION_BAR_FIELDS}
+        if day_bar is None:
+            bar = dict.fromkeys(self.OPEN_AUCTION_BAR_FIELDS, np.nan)
+        else:
+            bar = {k: day_bar[k] if k in day_bar.dtype.names else np.nan for k in self.OPEN_AUCTION_BAR_FIELDS}
         bar["last"] = bar["open"]
         return bar
 
     def get_settle_price(self, instrument, date):
         bar = self.get_bar(instrument, date, '1d')
         if bar is None:
             return np.nan
@@ -358,7 +363,10 @@
         return self._future_info_store.get_future_info(instrument)
 
     def get_merge_ticks(self, order_book_id_list, trading_date, last_dt=None):
         raise NotImplementedError
 
     def history_ticks(self, instrument, count, dt):
         raise NotImplementedError
+
+    def get_algo_bar(self, id_or_ins, start_min, end_min, dt):
+        raise NotImplementedError("open source rqalpha not support algo order")
```

### Comparing `rqalpha-4.9.2/rqalpha/data/base_data_source/storage_interface.py` & `rqalpha-5.0.0/rqalpha/data/base_data_source/storage_interface.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/data/base_data_source/storages.py` & `rqalpha-5.0.0/rqalpha/data/base_data_source/storages.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,18 +24,19 @@
 from itertools import chain
 from contextlib import contextmanager
 from typing import Dict, Iterable, Optional
 
 import h5py
 import numpy as np
 import pandas
+from methodtools import lru_cache
+
 from rqalpha.const import COMMISSION_TYPE, INSTRUMENT_TYPE
 from rqalpha.model.instrument import Instrument
 from rqalpha.utils.datetime_func import convert_date_to_date_int
-from rqalpha.utils.functools import lru_cache
 from rqalpha.utils.i18n import gettext as _
 
 from .storage_interface import (AbstractCalendarStore, AbstractDateSet,
                                 AbstractDayBarStore, AbstractDividendStore,
                                 AbstractInstrumentStore,
                                 AbstractSimpleFactorStore)
 
@@ -171,19 +172,19 @@
         finally:
             h5.close()
 
 
 class DayBarStore(AbstractDayBarStore):
     DEFAULT_DTYPE = np.dtype([
         ('datetime', np.uint64),
-        ('open', np.float),
-        ('close', np.float),
-        ('high', np.float),
-        ('low', np.float),
-        ('volume', np.float),
+        ('open', np.float64),
+        ('close', np.float64),
+        ('high', np.float64),
+        ('low', np.float64),
+        ('volume', np.float64),
     ])
 
     def __init__(self, path):
         if not os.path.exists(path):
             raise FileExistsError("File {} not exist，please update bundle.".format(path))
         self._path = path
 
@@ -248,14 +249,15 @@
         return df
 
 
 class SimpleFactorStore(AbstractSimpleFactorStore):
     def __init__(self, path):
         self._path = path
 
+    @lru_cache(1024)
     def get_factors(self, order_book_id):
         with h5_file(self._path) as h5:
             try:
                 return h5[order_book_id][:]
             except KeyError:
                 return None
```

### Comparing `rqalpha-4.9.2/rqalpha/data/bundle.py` & `rqalpha-5.0.0/rqalpha/data/bundle.py`

 * *Files 9% similar despite different names*

```diff
@@ -71,14 +71,16 @@
         for order_book_id, days in suspended_days.items():
             h5[order_book_id] = days
 
 
 def gen_dividends(d):
     stocks = rqdatac.all_instruments().order_book_id.tolist()
     dividend = rqdatac.get_dividend(stocks)
+    need_cols = ["dividend_cash_before_tax", "book_closure_date", "ex_dividend_date", "payable_date", "round_lot"]
+    dividend = dividend[need_cols]
     dividend.reset_index(inplace=True)
     dividend.rename(columns={'declaration_announcement_date': 'announcement_date'}, inplace=True)
     for f in ('book_closure_date', 'ex_dividend_date', 'payable_date', 'announcement_date'):
         dividend[f] = [convert_date_to_date_int(d) for d in dividend[f]]
     dividend.set_index(['order_book_id', 'book_closure_date'], inplace=True)
     with h5py.File(os.path.join(d, 'dividends.h5'), 'w') as h5:
         for order_book_id in dividend.index.levels[0]:
@@ -127,120 +129,92 @@
     df.predecessor_delisted_date = df.predecessor_delisted_date.astype(str)
 
     json_file = os.path.join(d, 'share_transformation.json')
     with open(json_file, 'w') as f:
         f.write(df.to_json(orient='index'))
 
 
-def init_future_info(d):
-    all_futures_info = []
-    underlying_symbol_list = []
-    fields = ['close_commission_ratio', 'close_commission_today_ratio', 'commission_type', 'open_commission_ratio']
-
-    futures_order_book_id = rqdatac.all_instruments(type='Future')['order_book_id'].unique()
-    for future in futures_order_book_id:
-        future_dict = {}
-        underlying_symbol = re.match(r'^[a-zA-Z]*', future).group()
-        commission = rqdatac.futures.get_commission_margin(future)
-        if not commission.empty:
-            future_dict['order_book_id'] = future
-            commission = commission.iloc[0]
-            for p in fields:
-                future_dict[p] = commission[p]
-            future_dict['tick_size'] = rqdatac.instruments(future).tick_size()
-        elif underlying_symbol not in underlying_symbol_list:
-            if underlying_symbol in {'S', 'TC', 'ER', 'WS', 'WT', 'RO', 'ME'}:
-                continue
-            underlying_symbol_list.append(underlying_symbol)
-            future_dict['underlying_symbol'] = underlying_symbol
-            try:
-                dominant = rqdatac.futures.get_dominant(underlying_symbol).iloc[-1]
-            except AttributeError:
-                # FIXME: why get_dominant return None???
-                continue
-            commission = rqdatac.futures.get_commission_margin(dominant).iloc[0]
-            for p in fields:
-                future_dict[p] = commission[p]
-            future_dict['tick_size'] = rqdatac.instruments(dominant).tick_size()
-        else:
-            continue
-        all_futures_info.append(future_dict)
-
-    hard_info = [{'underlying_symbol': 'TC',
-                  'close_commission_ratio': 4.0,
-                  'close_commission_today_ratio': 0.0,
-                  'commission_type': "by_volume",
-                  'open_commission_ratio': 4.0,
-                  'tick_size': 0.2},
-                 {'underlying_symbol': 'ER',
-                  'close_commission_ratio': 2.5,
-                  'close_commission_today_ratio': 2.5,
-                  'commission_type': "by_volume",
-                  'open_commission_ratio': 2.5,
-                  'tick_size': 1.0},
-                 {'underlying_symbol': 'WS',
-                  'close_commission_ratio': 2.5,
-                  'close_commission_today_ratio': 0.0,
-                  'commission_type': "by_volume",
-                  'open_commission_ratio': 2.5,
-                  'tick_size': 1.0},
-                 {'underlying_symbol': 'RO',
-                  'close_commission_ratio': 2.5,
-                  'close_commission_today_ratio': 0.0,
-                  'commission_type': "by_volume",
-                  'open_commission_ratio': 2.5,
-                  'tick_size': 2.0},
-                 {'underlying_symbol': 'ME',
-                  'close_commission_ratio': 1.4,
-                  'close_commission_today_ratio': 0.0,
-                  'commission_type': "by_volume",
-                  'open_commission_ratio': 1.4,
-                  'tick_size': 1.0}]
-
-    all_futures_info += hard_info
-
-    with open(os.path.join(d, 'future_info.json'), 'w') as f:
-        json.dump(all_futures_info, f, separators=(',', ':'), indent=2)
-
-
 def gen_future_info(d):
     future_info_file = os.path.join(d, 'future_info.json')
-    if not os.path.exists(future_info_file):
-        init_future_info(d)
-        return
 
-    with open(future_info_file, 'r') as f:
-        all_futures_info = json.load(f)
+    hard_code = [
+        {'underlying_symbol': 'TC',
+          'close_commission_ratio': 4.0,
+          'close_commission_today_ratio': 0.0,
+          'commission_type': "by_volume",
+          'open_commission_ratio': 4.0,
+          'tick_size': 0.2},
+         {'underlying_symbol': 'ER',
+          'close_commission_ratio': 2.5,
+          'close_commission_today_ratio': 2.5,
+          'commission_type': "by_volume",
+          'open_commission_ratio': 2.5,
+          'tick_size': 1.0},
+         {'underlying_symbol': 'WS',
+          'close_commission_ratio': 2.5,
+          'close_commission_today_ratio': 0.0,
+          'commission_type': "by_volume",
+          'open_commission_ratio': 2.5,
+          'tick_size': 1.0},
+         {'underlying_symbol': 'RO',
+          'close_commission_ratio': 2.5,
+          'close_commission_today_ratio': 0.0,
+          'commission_type': "by_volume",
+          'open_commission_ratio': 2.5,
+          'tick_size': 2.0},
+         {'underlying_symbol': 'ME',
+          'close_commission_ratio': 1.4,
+          'close_commission_today_ratio': 0.0,
+          'commission_type': "by_volume",
+          'open_commission_ratio': 1.4,
+          'tick_size': 1.0},
+        {'underlying_symbol': 'WT',
+         'close_commission_ratio': 5.0,
+         'close_commission_today_ratio': 5.0,
+         'commission_type': "by_volume",
+         'open_commission_ratio': 5.0,
+         'tick_size': 1.0},
+    ]
+
+    if not os.path.exists(future_info_file):
+        all_futures_info = hard_code
+    else:
+        with open(future_info_file, 'r') as f:
+            all_futures_info = json.load(f)
 
     future_list = []
     symbol_list = []
     param = ['close_commission_ratio', 'close_commission_today_ratio', 'commission_type', 'open_commission_ratio']
 
     for i in all_futures_info:
         if i.get('order_book_id'):
             future_list.append(i.get('order_book_id'))
         else:
             symbol_list.append(i.get('underlying_symbol'))
 
+    # 当修改了hard_code以后，避免用户需要手动删除future_info.json文件
+    for info in hard_code:
+        if info["underlying_symbol"] not in symbol_list:
+            all_futures_info.append(info)
+            symbol_list.append(info["underlying_symbol"])
+
     futures_order_book_id = rqdatac.all_instruments(type='Future')['order_book_id'].unique()
     for future in futures_order_book_id:
         underlying_symbol = re.match(r'^[a-zA-Z]*', future).group()
         if future in future_list:
             continue
         future_dict = {}
         commission = rqdatac.futures.get_commission_margin(future)
         if not commission.empty:
-            future_list.append(future)
             future_dict['order_book_id'] = future
             commission = commission.iloc[0]
             for p in param:
                 future_dict[p] = commission[p]
             future_dict['tick_size'] = rqdatac.instruments(future).tick_size()
-        elif underlying_symbol in symbol_list \
-                or underlying_symbol in {'S', 'TC', 'ER', 'WS', 'WT', 'RO', 'ME'}:
+        elif underlying_symbol in symbol_list:
             continue
         else:
             symbol_list.append(underlying_symbol)
             future_dict['underlying_symbol'] = underlying_symbol
             try:
                 dominant = rqdatac.futures.get_dominant(underlying_symbol).iloc[-1]
             except AttributeError:
@@ -338,16 +312,19 @@
         else:
             try:
                 h5 = h5py.File(path, 'a')
             except OSError:
                 raise OSError("File {} update failed, if it is using, please update later, "
                               "or you can delete then update again".format(path))
             try:
+                is_futures = "futures" == os.path.basename(path).split(".")[0]
                 for order_book_id in self._order_book_ids:
-                    if order_book_id in h5:
+                    # 特殊处理前复权合约，需要全量更新
+                    is_pre = is_futures and "888" in order_book_id
+                    if order_book_id in h5 and not is_pre:
                         try:
                             last_date = int(h5[order_book_id]['datetime'][-1] // 1000000)
                         except OSError:
                             raise OSError("File {} update failed, if it is using, please update later, "
                                           "or you can delete then update again".format(path))
                         except ValueError:
                             h5.pop(order_book_id)
```

### Comparing `rqalpha-4.9.2/rqalpha/data/data_proxy.py` & `rqalpha-5.0.0/rqalpha/data/data_proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,28 +11,28 @@
 #     * 商业用途（商业用途指个人出于任何商业目的使用本软件，或者法人或其他组织出于任何目的使用本软件）：
 #         未经米筐科技授权，任何个人不得出于任何商业目的使用本软件（包括但不限于向第三方提供、销售、出租、出借、转让本软件、
 #         本软件的衍生产品、引用或借鉴了本软件功能或源代码的产品或服务），任何法人或其他组织不得出于任何目的使用本软件，
 #         否则米筐科技有权追究相应的知识产权侵权责任。
 #         在此前提下，对本软件的使用同样需要遵守 Apache 2.0 许可，Apache 2.0 许可与本许可冲突之处，以本许可为准。
 #         详细的授权流程，请联系 public@ricequant.com 获取。
 
-import re
 from datetime import datetime, date
-from typing import Union, List, Sequence, Optional
+from typing import Union, List, Sequence, Optional, Tuple
 
 import six
 import numpy as np
 import pandas as pd
 
 from rqalpha.const import INSTRUMENT_TYPE, TRADING_CALENDAR_TYPE
 from rqalpha.utils import risk_free_helper, TimeRange, merge_trading_period
 from rqalpha.data.trading_dates_mixin import TradingDatesMixin
 from rqalpha.model.bar import BarObject, NANDict, PartialBarObject
 from rqalpha.model.tick import TickObject
 from rqalpha.model.instrument import Instrument
+from rqalpha.model.order import TWAPOrder, VWAPOrder, ALGO_ORDER_STYLES
 from rqalpha.utils.functools import lru_cache
 from rqalpha.utils.datetime_func import convert_int_to_datetime, convert_date_to_int
 from rqalpha.utils.typing import DateLike, StrOrIter
 from rqalpha.interface import AbstractDataSource, AbstractPriceBoard
 
 
 class DataProxy(TradingDatesMixin):
@@ -57,21 +57,27 @@
 
     def get_yield_curve(self, start_date, end_date, tenor=None):
         if isinstance(tenor, six.string_types):
             tenor = [tenor]
         return self._data_source.get_yield_curve(start_date, end_date, tenor)
 
     def get_risk_free_rate(self, start_date, end_date):
-        tenor = risk_free_helper.get_tenor_for(start_date, end_date)
+        tenors = risk_free_helper.get_tenors_for(start_date, end_date)
         # 为何取 start_date 当日的？表示 start_date 时借入资金、end_date 归还的成本
-        yc = self._data_source.get_yield_curve(start_date, start_date, [tenor])
+        _s = start_date if self.is_trading_date(start_date) else self.get_next_trading_date(start_date, n=1)
+        yc = self._data_source.get_yield_curve(_s, _s)
         if yc is None or yc.empty:
-            return 0
-        rate = yc.values[0, 0]
-        return 0 if np.isnan(rate) else rate
+            return np.nan
+        yc = yc.iloc[0]
+        for tenor in tenors[::-1]:
+            rate = yc.get(tenor)
+            if rate and not np.isnan(rate):
+                return rate
+        else:
+            return np.nan
 
     def get_dividend(self, order_book_id):
         instrument = self.instruments(order_book_id)
         return self._data_source.get_dividend(instrument)
 
     def get_split(self, order_book_id):
         instrument = self.instruments(order_book_id)
@@ -121,17 +127,17 @@
         return bar[0]
 
     def get_prev_close(self, order_book_id, dt):
         return self._get_prev_close(order_book_id, dt.replace(hour=0, minute=0, second=0))
 
     @lru_cache(10240)
     def _get_prev_settlement(self, instrument, dt):
-        prev_trading_date = self.get_previous_trading_date(dt)
-        bar = self._data_source.history_bars(instrument, 1, '1d', 'settlement', prev_trading_date,
-                                             skip_suspended=False, adjust_orig=dt)
+        bar = self._data_source.history_bars(
+            instrument, 1, '1d', fields='prev_settlement', dt=dt, skip_suspended=False, adjust_orig=dt
+        )
         if bar is None or len(bar) == 0:
             return np.nan
         return bar[0]
 
     @lru_cache(10240)
     def _get_settlement(self, instrument, dt):
         bar = self._data_source.history_bars(instrument, 1, '1d', 'settlement', dt, skip_suspended=False)
@@ -278,25 +284,36 @@
     def instruments(self, sym_or_ids):
         # type: (StrOrIter) -> Union[None, Instrument, List[Instrument]]
         if isinstance(sym_or_ids, str):
             return next(iter(self._data_source.get_instruments(id_or_syms=[sym_or_ids])), None)
         else:
             return list(self._data_source.get_instruments(id_or_syms=sym_or_ids))
 
-    FUTURE_CONTINUOUS_CONTRACT = re.compile("^[A-Z]{1,2}(88|888|99|889)$")
-
     def get_future_contracts(self, underlying, date):
         # type: (str, DateLike) -> List[str]
         return sorted(i.order_book_id for i in self.all_instruments(
             [INSTRUMENT_TYPE.FUTURE], date
-        ) if i.underlying_symbol == underlying and not re.match(self.FUTURE_CONTINUOUS_CONTRACT, i.order_book_id))
+        ) if i.underlying_symbol == underlying and not Instrument.is_future_continuous_contract(i.order_book_id))
 
     def get_trading_period(self, sym_or_ids, default_trading_period=None):
         # type: (StrOrIter, Optional[Sequence[TimeRange]]) -> List[TimeRange]
         trading_period = default_trading_period or []
         for instrument in self.instruments(sym_or_ids):
             trading_period.extend(instrument.trading_hours or [])
         return merge_trading_period(trading_period)
 
     def is_night_trading(self, sym_or_ids):
         # type: (StrOrIter) -> bool
         return any((instrument.trade_at_night for instrument in self.instruments(sym_or_ids)))
+
+    def get_algo_bar(self, id_or_ins, order_style, dt):
+        # type: (Union[str, Instrument], Union[*ALGO_ORDER_STYLES], datetime) -> Tuple[float, int]
+        if not isinstance(order_style, ALGO_ORDER_STYLES):
+            raise RuntimeError("get_algo_bar only support VWAPOrder and TWAPOrder")
+        if not isinstance(id_or_ins, Instrument):
+            id_or_ins = self.instrument(id_or_ins)
+        if id_or_ins is None:
+            return np.nan, 0
+        bar = self._data_source.get_algo_bar(id_or_ins, order_style.start_min, order_style.end_min, dt)
+        return (bar[order_style.TYPE], bar["volume"]) if bar else (np.nan, 0)
+
+
```

### Comparing `rqalpha-4.9.2/rqalpha/data/trading_dates_mixin.py` & `rqalpha-5.0.0/rqalpha/data/trading_dates_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
             return trading_dates[-1]
         else:
             return trading_dates[pos + n - 1]
 
     def is_trading_date(self, date, trading_calendar_type=None):
         trading_dates = self.get_trading_calendar(trading_calendar_type)
         pos = trading_dates.searchsorted(_to_timestamp(date))
-        return pos < len(trading_dates) and trading_dates[pos] == date
+        return pos < len(trading_dates) and trading_dates[pos].date() == date
 
     def get_trading_dt(self, calendar_dt):
         trading_date = self.get_future_trading_date(calendar_dt)
         return datetime.datetime.combine(trading_date, calendar_dt.time())
 
     def get_future_trading_date(self, dt):
         # type: (datetime.datetime) -> pd.Timestamp
```

### Comparing `rqalpha-4.9.2/rqalpha/environment.py` & `rqalpha-5.0.0/rqalpha/environment.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,8 +181,9 @@
     def can_submit_order(self, order):
         # forward compatible
         instrument_type = self.data_proxy.instrument(order.order_book_id).type
         account = self.portfolio.get_account(order.order_book_id)
         for v in self._get_frontend_validators(instrument_type):
             if not v.can_submit_order(order, account):
                 return False
-        return True
+        return True
+
```

### Comparing `rqalpha-4.9.2/rqalpha/examples/IF1706_20161108.csv` & `rqalpha-5.0.0/rqalpha/examples/IF1706_20161108.csv`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/examples/IF_macd.py` & `rqalpha-5.0.0/rqalpha/examples/IF_macd.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/examples/buy_and_hold.py` & `rqalpha-5.0.0/rqalpha/examples/buy_and_hold.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/examples/data_source/get_csv_module.py` & `rqalpha-5.0.0/rqalpha/examples/data_source/get_csv_module.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/examples/data_source/import_get_csv_module.py` & `rqalpha-5.0.0/rqalpha/examples/data_source/import_get_csv_module.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/examples/data_source/read_csv_as_df.py` & `rqalpha-5.0.0/rqalpha/examples/data_source/read_csv_as_df.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/examples/extend_api/rqalpha_mod_extend_api_demo.py` & `rqalpha-5.0.0/rqalpha/examples/extend_api/rqalpha_mod_extend_api_demo.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/examples/extend_api/test_extend_api.py` & `rqalpha-5.0.0/rqalpha/examples/extend_api/test_extend_api.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/examples/golden_cross.py` & `rqalpha-5.0.0/rqalpha/examples/golden_cross.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/examples/macd.py` & `rqalpha-5.0.0/rqalpha/examples/macd.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/examples/pair_trading.py` & `rqalpha-5.0.0/rqalpha/examples/pair_trading.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/examples/rsi.py` & `rqalpha-5.0.0/rqalpha/examples/rsi.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/examples/run_code_demo.py` & `rqalpha-5.0.0/rqalpha/examples/run_code_demo.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/examples/run_func_demo.py` & `rqalpha-5.0.0/rqalpha/examples/run_func_demo.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/examples/subscribe_event.py` & `rqalpha-5.0.0/rqalpha/examples/subscribe_event.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/examples/test_pt.py` & `rqalpha-5.0.0/rqalpha/examples/test_pt.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/examples/turtle.py` & `rqalpha-5.0.0/rqalpha/examples/turtle.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/interface.py` & `rqalpha-5.0.0/rqalpha/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -441,14 +441,19 @@
         # type: (str, Sequence[DateLike]) -> Sequence[bool]
         raise NotImplementedError
 
     def is_st_stock(self, order_book_id, dates):
         # type: (str, Sequence[DateLike]) -> Sequence[bool]
         raise NotImplementedError
 
+    def get_algo_bar(self, id_or_ins, start_min, end_min, dt):
+        # type: (Union[str, Instrument], int, int, datetime) -> Optional[numpy.void]
+        # 格式: (date, VWAP, TWAP, volume) -> 案例 (20200102, 16.79877183, 16.83271429, 144356044)
+        raise NotImplementedError
+
 
 class AbstractBroker(with_metaclass(abc.ABCMeta)):
     """
     券商接口。
 
     RQAlpha 将产生的订单提交给此对象，此对象负责对订单进行撮合（不论是自行撮合还是委托给外部的真实交易所），
     并通过 ``EVENT.ORDER_*`` 及 ``EVENT.TRADE`` 事件将撮合结果反馈进入 RQAlpha。
```

### Comparing `rqalpha-4.9.2/rqalpha/main.py` & `rqalpha-5.0.0/rqalpha/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 #         本软件的衍生产品、引用或借鉴了本软件功能或源代码的产品或服务），任何法人或其他组织不得出于任何目的使用本软件，
 #         否则米筐科技有权追究相应的知识产权侵权责任。
 #         在此前提下，对本软件的使用同样需要遵守 Apache 2.0 许可，Apache 2.0 许可与本许可冲突之处，以本许可为准。
 #         详细的授权流程，请联系 public@ricequant.com 获取。
 
 import datetime
 import sys
-import traceback
 from pprint import pformat
 from itertools import chain
 
 import jsonpickle.ext.numpy as jsonpickle_numpy
 import logbook
 import six
 from rqalpha import const
@@ -107,27 +106,28 @@
 
 def get_strategy_apis():
     from rqalpha import api
     return {n: getattr(api, n) for n in api.__all__}
 
 
 def init_rqdatac(rqdatac_uri):
+    if rqdatac_uri in ["disabled", "DISABLED"]:
+        return
+
     try:
         import rqdatac
     except ImportError:
         return
 
-    import warnings
-
-    try:
+    if isinstance(rqdatac.client.get_client(), rqdatac.client.DummyClient):
         init_rqdatac_env(rqdatac_uri)
-        with warnings.catch_warnings(record=True):
+        try:
             rqdatac.init()
-    except Exception as e:
-        system_log.warn(_('rqdatac init failed, some apis will not function properly: {}').format(str(e)))
+        except Exception as e:
+            system_log.warn(_('rqdatac init failed, some apis will not function properly: {}').format(str(e)))
 
 
 def run(config, source_code=None, user_funcs=None):
     env = Environment(config)
     persist_helper = None
     init_succeed = False
     mod_handler = ModHandler()
@@ -161,15 +161,16 @@
         env.trading_dt = start_dt
 
         assert env.broker is not None
         assert env.event_source is not None
         if env.portfolio is None:
             from rqalpha.portfolio import Portfolio
             env.set_portfolio(Portfolio(
-                config.base.accounts, config.base.init_positions, config.base.start_date, env.data_proxy, env.event_bus
+                config.base.accounts, config.base.init_positions, config.mod.sys_accounts.financing_rate,
+                config.base.start_date, env.data_proxy, env.event_bus
             ))
 
         env.event_bus.publish_event(Event(EVENT.POST_SYSTEM_INIT))
 
         scope = create_base_scope()
         scope.update({"g": env.global_vars})
         scope.update(get_strategy_apis())
@@ -260,15 +261,19 @@
     except ImportError:
         raise RuntimeError('--enable-profiler needs line_profiler')
 
     import inspect
     env.profile_deco = profile_deco = line_profiler.LineProfiler()
     for name in scope:
         obj = scope[name]
-        if getattr(obj, "__module__", None) != "rqalpha.user_module":
+        # 针对 run_func
+        func_cond = "__globals__" in dir(obj) and obj.__globals__.get("__name__", None) == "rqalpha.user_module"
+        # 针对 run_code 和 run_file
+        file_or_code_cond = "__module__" in dir(obj) and obj.__module__ == "rqalpha.user_module"
+        if not any([func_cond, file_or_code_cond]):
             continue
         if inspect.isfunction(obj):
             scope[name] = profile_deco(obj)
         if inspect.isclass(obj):
             for key, val in obj.__dict__.items():
                 if inspect.isfunction(val):
                     setattr(obj, key, profile_deco(val))
```

### Comparing `rqalpha-4.9.2/rqalpha/mod/__init__.py` & `rqalpha-5.0.0/rqalpha/mod/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_accounts/__init__.py` & `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_accounts/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,14 +25,20 @@
     "cash_return_by_stock_delisted": True,
     # 股票下单因资金不足被拒时改为使用全部剩余资金下单
     "auto_switch_order_value": False,
     # 开启对股票仓位是否能满足平仓需求的检查
     "validate_stock_position": True,
     # 开启对期货仓位是否能满足平仓需求的检查
     "validate_future_position": True,
+    # 融资利率/年
+    "financing_rate": 0.00,
+    # 是否开启融资可买入股票的限制
+    "financing_stocks_restriction_enabled": False,
+    # 逐日盯市结算价: settlement/close
+    "futures_settlement_price_type": "close",
 }
 
 
 def load_mod():
     from .mod import AccountMod
     return AccountMod()
 
@@ -71,7 +77,15 @@
 cli.commands['run'].params.append(
     click.Option(
         ("--no-short-stock/--short-stock", cli_prefix + "validate_stock_position"),
         is_flag=True, default=True,
         help="[sys_accounts] enable stock shorting"
     )
 )
+
+cli.commands['run'].params.append(
+    click.Option(
+        ('--futures-settlement-price-type', cli_prefix + 'futures_settlement_price_type'),
+        default=None,
+        help="[sys_accounts] future settlement price"
+    )
+)
```

### Comparing `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_accounts/api/__init__.py` & `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_accounts/api/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py` & `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,49 +14,49 @@
 #         否则米筐科技有权追究相应的知识产权侵权责任。
 #         在此前提下，对本软件的使用同样需要遵守 Apache 2.0 许可，Apache 2.0 许可与本许可冲突之处，以本许可为准。
 #         详细的授权流程，请联系 public@ricequant.com 获取。
 
 from __future__ import division
 from typing import Union, Optional, List
 
+import numpy as np
+
 from rqalpha.api import export_as_api
 from rqalpha.apis.api_base import assure_instrument
 from rqalpha.apis.api_abstract import order, order_to, buy_open, buy_close, sell_open, sell_close
 from rqalpha.apis.api_base import cal_style
 from rqalpha.apis.api_rqdatac import futures
 from rqalpha.environment import Environment
-from rqalpha.model.order import Order, LimitOrder, OrderStyle
+from rqalpha.model.order import Order, LimitOrder, OrderStyle, ALGO_ORDER_STYLES
 from rqalpha.const import SIDE, POSITION_EFFECT, ORDER_TYPE, RUN_TYPE, INSTRUMENT_TYPE, POSITION_DIRECTION
 from rqalpha.model.instrument import Instrument
 from rqalpha.portfolio.position import Position
 from rqalpha.utils import is_valid_price
 from rqalpha.utils.exception import RQInvalidArgument
 from rqalpha.utils.logger import user_system_log
 from rqalpha.utils.i18n import gettext as _
 from rqalpha.utils.arg_checker import apply_rules, verify_that
 
 
-__all__ = [
-]
+__all__ = []
 
 
 def _submit_order(id_or_ins, amount, side, position_effect, style):
     instrument = assure_instrument(id_or_ins)
     order_book_id = instrument.order_book_id
     env = Environment.get_instance()
 
     amount = int(amount)
     if amount == 0:
         user_system_log.warn(_(
             u"Order Creation Failed: 0 order quantity, order_book_id={order_book_id}"
         ).format(order_book_id=order_book_id))
         return None
-    if isinstance(style, LimitOrder) and style.get_limit_price() <= 0:
-        raise RQInvalidArgument(_(u"Limit order price should be positive"))
-
+    if isinstance(style, LimitOrder) and np.isnan(style.get_limit_price()):
+        raise RQInvalidArgument(_(u"Limit order price should not be nan."))
 
     if env.config.base.run_type != RUN_TYPE.BACKTEST and instrument.type == INSTRUMENT_TYPE.FUTURE:
         if "88" in order_book_id:
             raise RQInvalidArgument(_(u"Main Future contracts[88] are not supported in paper trading."))
         if "99" in order_book_id:
             raise RQInvalidArgument(_(u"Index Future contracts[99] are not supported in paper trading."))
 
@@ -117,16 +117,14 @@
                 ), new_orders_repr=", ".join(["Order({}, {}, {}, {})".format(
                     o.order_book_id, o.quantity, o.side, o.position_effect
                 ) for o in orders])
             )
         )
 
     for o in orders:
-        if o.type == ORDER_TYPE.MARKET:
-            o.set_frozen_price(price)
         if env.can_submit_order(o):
             env.broker.submit_order(o)
         else:
             orders.remove(o)
 
     # 向前兼容，如果创建的order_list 只包含一个订单的话，直接返回对应的订单，否则返回列表
     if len(orders) == 1:
@@ -172,45 +170,45 @@
         return orders
     # 开仓
     orders.append(_submit_order(order_book_id, quantity, side, POSITION_EFFECT.OPEN, style))
     return orders
 
 
 @order.register(INSTRUMENT_TYPE.FUTURE)
-def future_order(order_book_id, quantity, price=None, style=None):
-    # type: (Union[str, Instrument], int, Optional[float], Optional[OrderStyle]) -> List[Order]
-    return _order(order_book_id, quantity, cal_style(price, style), False)
+def future_order(order_book_id, quantity, price=None, style=None, price_or_style=None):
+    # type: (Union[str, Instrument], int, Optional[float], Optional[OrderStyle], Optional[Union[float, OrderStyle]]) -> List[Order]
+    return _order(order_book_id, quantity, cal_style(price, style, price_or_style), False)
 
 
 @order_to.register(INSTRUMENT_TYPE.FUTURE)
-def future_order_to(order_book_id, quantity, price=None, style=None):
-    # type: (Union[str, Instrument], int, Optional[float], Optional[OrderStyle]) -> List[Order]
-    return _order(order_book_id, quantity, cal_style(price, style), True)
+def future_order_to(order_book_id, quantity, price=None, style=None, price_or_style=None):
+    # type: (Union[str, Instrument], int, Optional[float], Optional[OrderStyle], Optional[Union[float, OrderStyle]]) -> List[Order]
+    return _order(order_book_id, quantity, cal_style(price, style, price_or_style), True)
 
 
 @buy_open.register(INSTRUMENT_TYPE.FUTURE)
-def future_buy_open(id_or_ins, amount, price=None, style=None):
-    return _submit_order(id_or_ins, amount, SIDE.BUY, POSITION_EFFECT.OPEN, cal_style(price, style))
+def future_buy_open(id_or_ins, amount, price=None, style=None, price_or_style=None):
+    return _submit_order(id_or_ins, amount, SIDE.BUY, POSITION_EFFECT.OPEN, cal_style(price, style, price_or_style))
 
 
 @buy_close.register(INSTRUMENT_TYPE.FUTURE)
-def future_buy_close(id_or_ins, amount, price=None, style=None, close_today=False):
+def future_buy_close(id_or_ins, amount, price=None, style=None, close_today=False, price_or_style=None):
     position_effect = POSITION_EFFECT.CLOSE_TODAY if close_today else POSITION_EFFECT.CLOSE
-    return _submit_order(id_or_ins, amount, SIDE.BUY, position_effect, cal_style(price, style))
+    return _submit_order(id_or_ins, amount, SIDE.BUY, position_effect, cal_style(price, style, price_or_style))
 
 
 @sell_open.register(INSTRUMENT_TYPE.FUTURE)
-def future_sell_open(id_or_ins, amount, price=None, style=None):
-    return _submit_order(id_or_ins, amount, SIDE.SELL, POSITION_EFFECT.OPEN, cal_style(price, style))
+def future_sell_open(id_or_ins, amount, price=None, style=None, price_or_style=None):
+    return _submit_order(id_or_ins, amount, SIDE.SELL, POSITION_EFFECT.OPEN, cal_style(price, style, price_or_style))
 
 
 @sell_close.register(INSTRUMENT_TYPE.FUTURE)
-def future_sell_close(id_or_ins, amount, price=None, style=None, close_today=False):
+def future_sell_close(id_or_ins, amount, price=None, style=None, close_today=False, price_or_style=None):
     position_effect = POSITION_EFFECT.CLOSE_TODAY if close_today else POSITION_EFFECT.CLOSE
-    return _submit_order(id_or_ins, amount, SIDE.SELL, position_effect, cal_style(price, style))
+    return _submit_order(id_or_ins, amount, SIDE.SELL, position_effect, cal_style(price, style, price_or_style))
 
 
 @export_as_api
 @apply_rules(verify_that('underlying_symbol').is_instance_of(str))
 def get_future_contracts(underlying_symbol):
     # type: (str) -> List[str]
     """
```

### Comparing `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py` & `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,29 +22,30 @@
 
 import numpy as np
 import pandas as pd
 from rqalpha.api import export_as_api
 from rqalpha.apis.api_abstract import (order, order_percent, order_shares,
                                        order_target_percent,
                                        order_target_value, order_to,
-                                       order_value)
+                                       order_value,
+                                       common_rules, TUPLE_PRICE_OR_STYLE_TYPE, PRICE_OR_STYLE_TYPE)
 from rqalpha.apis.api_base import (assure_instrument, assure_order_book_id,
-                                   cal_style)
+                                   cal_style, calc_open_close_style)
 from rqalpha.const import (DEFAULT_ACCOUNT_TYPE, EXECUTION_PHASE,
                            INSTRUMENT_TYPE, ORDER_TYPE, POSITION_DIRECTION,
                            POSITION_EFFECT, SIDE)
 from rqalpha.core.execution_context import ExecutionContext
 from rqalpha.environment import Environment
 from rqalpha.mod.rqalpha_mod_sys_risk.validators.cash_validator import \
     is_cash_enough
 from rqalpha.model.instrument import IndustryCode as industry_code
 from rqalpha.model.instrument import IndustryCodeItem, Instrument
 from rqalpha.model.instrument import SectorCode as sector_code
 from rqalpha.model.instrument import SectorCodeItem
-from rqalpha.model.order import LimitOrder, MarketOrder, Order, OrderStyle
+from rqalpha.model.order import LimitOrder, MarketOrder, Order, OrderStyle, ALGO_ORDER_STYLES
 from rqalpha.utils import INST_TYPE_IN_STOCK_ACCOUNT, is_valid_price
 from rqalpha.utils.arg_checker import apply_rules, verify_that
 from rqalpha.utils.datetime_func import to_date
 from rqalpha.utils.exception import RQInvalidArgument
 from rqalpha.utils.i18n import gettext as _
 from rqalpha.utils.logger import user_system_log
 
@@ -71,22 +72,36 @@
 
 def _round_order_quantity(ins, quantity) -> int:
     if ins.type == "CS" and ins.board_type == "KSH":
         # KSH can buy(sell) 201, 202 shares
         return 0 if abs(quantity) < KSH_MIN_AMOUNT else int(quantity)
     else:
         round_lot = ins.round_lot
-        return int(Decimal(quantity) / Decimal(round_lot)) * round_lot
+        try:
+            return int(Decimal(quantity) / Decimal(round_lot)) * round_lot
+        except ValueError:
+            raise
+
+
+def _get_order_style_price(order_book_id, style):
+    if isinstance(style, LimitOrder):
+        return style.get_limit_price()
+    env = Environment.get_instance()
+    if isinstance(style, MarketOrder):
+        return env.data_proxy.get_last_price(order_book_id)
+    if isinstance(style, ALGO_ORDER_STYLES):
+        price, _ = env.data_proxy.get_algo_bar(order_book_id, style, env.calendar_dt)
+        return price
+    raise RuntimeError(f"no support {style} order style")
 
 
 def _submit_order(ins, amount, side, position_effect, style, current_quantity, auto_switch_order_value):
     env = Environment.get_instance()
-    if isinstance(style, LimitOrder):
-        if not is_valid_price(style.get_limit_price()):
-            raise RQInvalidArgument(_(u"Limit order price should be positive"))
+    if isinstance(style, LimitOrder) and np.isnan(style.get_limit_price()):
+        raise RQInvalidArgument(_(u"Limit order price should not be nan."))
     price = env.data_proxy.get_last_price(ins.order_book_id)
     if not is_valid_price(price):
         user_system_log.warn(
             _(u"Order Creation Failed: [{order_book_id}] No market data").format(order_book_id=ins.order_book_id))
         return
 
     if (side == SIDE.BUY) or (side == SIDE.SELL and current_quantity != abs(amount)):
@@ -94,16 +109,14 @@
 
     if amount == 0:
         user_system_log.warn(_(
             u"Order Creation Failed: 0 order quantity, order_book_id={order_book_id}"
         ).format(order_book_id=ins.order_book_id))
         return
     order = Order.__from_create__(ins.order_book_id, abs(amount), side, style, position_effect)
-    if order.type == ORDER_TYPE.MARKET:
-        order.set_frozen_price(price)
     if side == SIDE.BUY and auto_switch_order_value:
         account, position, ins = _get_account_position_ins(ins)
         if not is_cash_enough(env, order, account.cash):
             user_system_log.warn(_(
                 "insufficient cash, use all remaining cash({}) to create order"
             ).format(account.cash))
             return _order_value(account, position, ins, account.cash, style)
@@ -149,221 +162,252 @@
     if amount < 0:
         amount = max(amount, -position.closable)
 
     return _order_shares(ins, amount, style, position.quantity, auto_switch_order_value=False)
 
 
 @order_shares.register(INST_TYPE_IN_STOCK_ACCOUNT)
-def stock_order_shares(id_or_ins, amount, price=None, style=None):
+def stock_order_shares(id_or_ins, amount, price=None, style=None, price_or_style=None):
     auto_switch_order_value = Environment.get_instance().config.mod.sys_accounts.auto_switch_order_value
     account, position, ins = _get_account_position_ins(id_or_ins)
-    return _order_shares(assure_instrument(id_or_ins), amount, cal_style(price, style), position.quantity,
-                         auto_switch_order_value)
+    return _order_shares(
+        assure_instrument(id_or_ins), amount, cal_style(price, style, price_or_style), position.quantity,
+        auto_switch_order_value
+    )
 
 
 @order_value.register(INST_TYPE_IN_STOCK_ACCOUNT)
-def stock_order_value(id_or_ins, cash_amount, price=None, style=None):
+def stock_order_value(id_or_ins, cash_amount, price=None, style=None, price_or_style=None):
     account, position, ins = _get_account_position_ins(id_or_ins)
-    return _order_value(account, position, ins, cash_amount, cal_style(price, style))
+    return _order_value(account, position, ins, cash_amount, cal_style(price, style, price_or_style))
 
 
 @order_percent.register(INST_TYPE_IN_STOCK_ACCOUNT)
-def stock_order_percent(id_or_ins, percent, price=None, style=None):
+def stock_order_percent(id_or_ins, percent, price=None, style=None, price_or_style=None):
     account, position, ins = _get_account_position_ins(id_or_ins)
-    return _order_value(account, position, ins, account.total_value * percent, cal_style(price, style))
+    return _order_value(account, position, ins, account.total_value * percent, cal_style(price, style, price_or_style))
 
 
 @order_target_value.register(INST_TYPE_IN_STOCK_ACCOUNT)
-def stock_order_target_value(id_or_ins, cash_amount, price=None, style=None):
+def stock_order_target_value(id_or_ins, cash_amount, price=None, style=None, price_or_style=None):
     account, position, ins = _get_account_position_ins(id_or_ins)
+    open_style, close_style = calc_open_close_style(price, style, price_or_style)
     if cash_amount == 0:
-        return _submit_order(ins, position.closable, SIDE.SELL, POSITION_EFFECT.CLOSE, cal_style(price, style),
-                             position.quantity, False)
-    return _order_value(account, position, ins, cash_amount - position.market_value, cal_style(price, style))
+        return _submit_order(
+            ins, position.closable, SIDE.SELL, POSITION_EFFECT.CLOSE, close_style, position.quantity, False
+        )
+    _delta = cash_amount - position.market_value
+    _style = open_style if _delta > 0 else close_style
+    return _order_value(account, position, ins, _delta, _style)
 
 
 @order_target_percent.register(INST_TYPE_IN_STOCK_ACCOUNT)
-def stock_order_target_percent(id_or_ins, percent, price=None, style=None):
+def stock_order_target_percent(id_or_ins, percent, price=None, style=None, price_or_style=None):
     account, position, ins = _get_account_position_ins(id_or_ins)
+    open_style, close_style = calc_open_close_style(price, style, price_or_style)
     if percent == 0:
-        return _submit_order(ins, position.closable, SIDE.SELL, POSITION_EFFECT.CLOSE, cal_style(price, style),
-                             position.quantity, False)
-    else:
-        return _order_value(
-            account, position, ins, account.total_value * percent - position.market_value, cal_style(price, style)
+        return _submit_order(
+            ins, position.closable, SIDE.SELL, POSITION_EFFECT.CLOSE, close_style, position.quantity, False
         )
+    _delta = account.total_value * percent - position.market_value
+    _style = open_style if _delta > 0 else close_style
+    return _order_value(account, position, ins, _delta, _style)
 
 
 @order.register(INST_TYPE_IN_STOCK_ACCOUNT)
-def stock_order(order_book_id, quantity, price=None, style=None):
-    result_order = stock_order_shares(order_book_id, quantity, price, style)
+def stock_order(order_book_id, quantity, price=None, style=None, price_or_style=None):
+    result_order = stock_order_shares(order_book_id, quantity, price, style, price_or_style)
     if result_order:
         return [result_order]
     return []
 
 
 @order_to.register(INST_TYPE_IN_STOCK_ACCOUNT)
-def stock_order_to(order_book_id, quantity, price=None, style=None):
+def stock_order_to(order_book_id, quantity, price=None, style=None, price_or_style=None):
     position = Environment.get_instance().portfolio.get_position(order_book_id, POSITION_DIRECTION.LONG)
+    open_style, close_style = calc_open_close_style(price, style, price_or_style)
     quantity = quantity - position.quantity
-    result_order = stock_order_shares(order_book_id, quantity, price, style)
+    _style = open_style if quantity > 0 else close_style
+    result_order = stock_order_shares(order_book_id, quantity, price, _style, price_or_style)
     if result_order:
         return [result_order]
     return []
 
 
 @export_as_api
 @ExecutionContext.enforce_phase(
     EXECUTION_PHASE.OPEN_AUCTION,
     EXECUTION_PHASE.ON_BAR,
     EXECUTION_PHASE.ON_TICK,
     EXECUTION_PHASE.SCHEDULED,
     EXECUTION_PHASE.GLOBAL
 )
-@apply_rules(verify_that('id_or_ins').is_valid_stock(),
-             verify_that('amount').is_number(),
-             verify_that('style').is_instance_of((MarketOrder, LimitOrder, type(None))))
-def order_lots(id_or_ins, amount, price=None, style=None):
-    # type: (Union[str, Instrument], int, Optional[float], Optional[OrderStyle]) -> Optional[Order]
+@apply_rules(verify_that('id_or_ins').is_valid_stock(), verify_that('amount').is_number(), *common_rules)
+def order_lots(id_or_ins, amount, price=None, style=None, price_or_style=None):
+    # type: (Union[str, Instrument], int, Optional[float], Optional[OrderStyle], PRICE_OR_STYLE_TYPE) -> Optional[Order]
     """
     指定手数发送买/卖单。如有需要落单类型当做一个参量传入，如果忽略掉落单类型，那么默认是市价单（market order）。
 
     :param id_or_ins: 下单标的物
     :param int amount: 下单量, 正数代表买入，负数代表卖出。将会根据一手xx股来向下调整到一手的倍数，比如中国A股就是调整成100股的倍数。
     :param float price: 下单价格，默认为None，表示 :class:`~MarketOrder`, 此参数主要用于简化 `style` 参数。
     :param style: 下单类型, 默认是市价单。目前支持的订单类型有 :class:`~LimitOrder` 和 :class:`~MarketOrder`
+    :param price_or_style: 默认为None，表示市价单，可设置价格，表示限价单，也可以直接设置订单类型，有如下选项：MarketOrder、LimitOrder、
+                            TWAPOrder、VWAPOrder
 
     :example:
 
     .. code-block:: python
 
         #买入20手的平安银行股票，并且发送市价单：
         order_lots('000001.XSHE', 20)
         #买入10手平安银行股票，并且发送限价单，价格为￥10：
         order_lots('000001.XSHE', 10, style=LimitOrder(10))
 
     """
     auto_switch_order_value = Environment.get_instance().config.mod.sys_accounts.auto_switch_order_value
     account, position, ins = _get_account_position_ins(id_or_ins)
-    return _order_shares(ins, amount * int(ins.round_lot), cal_style(price, style), position.quantity,
-                         auto_switch_order_value)
+    return _order_shares(
+        ins, amount * int(ins.round_lot), cal_style(price, style, price_or_style), position.quantity,
+        auto_switch_order_value
+    )
 
 
 ORDER_TARGET_PORTFOLIO_SUPPORTED_INS_TYPES = {
-    INSTRUMENT_TYPE.CS, INSTRUMENT_TYPE.ETF, INSTRUMENT_TYPE.LOF, INSTRUMENT_TYPE.INDX}
+    INSTRUMENT_TYPE.CS, INSTRUMENT_TYPE.ETF, INSTRUMENT_TYPE.LOF, INSTRUMENT_TYPE.INDX
+}
 
 
 @export_as_api
 @ExecutionContext.enforce_phase(
     EXECUTION_PHASE.OPEN_AUCTION,
     EXECUTION_PHASE.ON_BAR,
     EXECUTION_PHASE.ON_TICK,
     EXECUTION_PHASE.SCHEDULED,
     EXECUTION_PHASE.GLOBAL
 )
-def order_target_portfolio(target_portfolio: Dict[Union[str, Instrument], Union[float, Tuple[float, float]]]) -> List[Order]:
+def order_target_portfolio(
+        target_portfolio: Dict[str, float], price_or_styles: Dict[str, TUPLE_PRICE_OR_STYLE_TYPE] = dict({}),
+) -> List[Order]:
     """
     批量调整股票仓位至目标权重。注意：股票账户中未出现在 target_portfolio 中的资产将被平仓！
 
-    该 API 的参数 target_portfolio 为字典，key 为 order_book_id 或 instrument，value 有两种数据类型可选：
+    该 API 的参数 target_portfolio 为字典，key 为 order_book_id 或 instrument，value 为权重。
+    此时将根据参数 price_or_styles 中设置的价格来计算目标持仓数量并调仓。
 
-      * value 为权重。此时将根据股票最新价计算目标持仓数量并发出市价单调仓。
-
-      * value 为权重和价格组成的 tuple。此时将根据该价格计算目标权重并发出限价单（Signal 模式下将使用该价格撮合）。
-
-    :param target_portfolio: 目标权重字典，key 为 order_book_id，value 为权重或权重和价格组成的 tuple。
+    :param target_portfolio: 目标权重字典，key 为 order_book_id，value 为权重。
+    :param price_or_styles: 目标下单价格字典，key 为 order_book_id, value 为价格或订单类型或订单类型和价格组成的 tuple
 
     :example:
 
     .. code-block:: python
 
-        # 调整仓位，以使平安银行和万科 A 的持仓占比分别达到 10% 和 15%
+        # 调整仓位，以使平安银行和万科 A 的持仓占比分别达到 10% 和 15%, 同时发送市价单
         order_target_portfolio({
             '000001.XSHE': 0.1,
             '000002.XSHE': 0.15
         })
 
         # 调整仓位，分别以 14 和 26 元发出限价单，目标是使平安银行和万科 A 的持仓占比分别达到 10% 和 15%
         order_target_portfolio({
-            '000001.XSHE': (0.1, 14),
-            '000002.XSHE': (0.15, 26)
+            '000001.XSHE': 0.1,
+            '000002.XSHE': 0.15
+        }, {
+            '000001.XSHE': 14,
+            '000002.XSHE': 26,
         })
+
+        # 调整仓位，使平安银行和万科 A 的持仓占比分别达到 10% 和 15%。
+        # 其中平安银行的平仓价为 14 元，开仓价为 15 元；万科 A 的平仓价为 26 元，开仓价为 27 元。
+        order_target_portfolio({
+            '000001.XSHE': 0.1,
+            '000002.XSHE': 0.15
+        }, {
+            '000001.XSHE': (15, 14),
+            '000002.XSHE': (27, 26)
+        })
+
     """
     env = Environment.get_instance()
-    target = {}
-    for id_or_ins, target_quantity_price in target_portfolio.items():
+    target: Dict[str, Tuple[float, float, float, float]] = {}
+    for id_or_ins, percent in target_portfolio.items():
         ins = assure_instrument(id_or_ins)
         if not ins:
             raise RQInvalidArgument(_(
                 "function order_target_portfolio: invalid keys of target_portfolio, "
                 "expected order_book_ids or Instrument objects, got {} (type: {})"
             ).format(id_or_ins, type(id_or_ins)))
         if ins.type not in ORDER_TARGET_PORTFOLIO_SUPPORTED_INS_TYPES:
             raise RQInvalidArgument(_(
                 "function order_target_portfolio: invalid instrument type, excepted CS/ETF/LOF/INDX, got {}"
             ).format(ins.order_book_id))
         order_book_id = ins.order_book_id
-        price = env.data_proxy.get_last_price(order_book_id)
-        if not is_valid_price(price):
+        last_price = env.data_proxy.get_last_price(order_book_id)
+        if not is_valid_price(last_price):
             user_system_log.warn(
                 _(u"Order Creation Failed: [{order_book_id}] No market data").format(order_book_id=order_book_id)
             )
             continue
-        try:
-            target_percent, target_price = target_quantity_price
-        except TypeError:
-            target_percent = target_quantity_price
-            target_price = None
-        else:
-            if not is_valid_price(target_price):
-                raise RQInvalidArgument(_(
-                    "function order_target_portfolio: invalid order price {target_price} of {id_or_ins}"
-                ).format(id_or_ins=id_or_ins, target_price=target_price))
-        if target_percent == 0:
-            continue
-        elif target_percent < 0:
+
+        price_or_style = price_or_styles.get(ins.order_book_id)
+        open_style, close_style = calc_open_close_style(price=None, style=None, price_or_style=price_or_style)
+
+        if percent < 0:
             raise RQInvalidArgument(_(
                 "function order_target_portfolio: invalid values of target_portfolio, "
                 "excepted float between 0 and 1, got {} (key: {})"
-            ).format(target_percent, id_or_ins))
+            ).format(percent, id_or_ins))
+
+        target[order_book_id] = percent, open_style, close_style, last_price
 
-        target[order_book_id] = target_percent, target_price, price
     total_percent = sum(p for p, *__ in target.values())
     if total_percent > 1 and not np.isclose(total_percent, 1):
         raise RQInvalidArgument(_("total percent should be lower than 1, current: {}").format(total_percent))
 
     account = env.portfolio.accounts[DEFAULT_ACCOUNT_TYPE.STOCK]
+
+    # 先把不在目标权重中的仓位平掉
     current_quantities = {
         p.order_book_id: p.quantity for p in account.get_positions() if p.direction == POSITION_DIRECTION.LONG
     }
     for order_book_id, quantity in current_quantities.items():
-        # 先把不在目标权重中的仓位平掉
         if order_book_id not in target:
             env.submit_order(Order.__from_create__(
                 order_book_id, quantity, SIDE.SELL, MarketOrder(), POSITION_EFFECT.CLOSE
             ))
 
     account_value = account.total_value
     close_orders, open_orders = [], []
-    for order_book_id, (target_percent, target_price, price) in target.items():
-        delta_quantity = (account_value * target_percent / (target_price or price)) - current_quantities.get(order_book_id, 0)
+    for order_book_id, (target_percent, open_style, close_style, last_price) in target.items():
+        open_price = _get_order_style_price(order_book_id, open_style)
+        close_price = _get_order_style_price(order_book_id, close_style)
+        if not (is_valid_price(close_price) and is_valid_price(open_price)):
+            user_system_log.warn(_(
+                "Adjust position of {id_or_ins} Failed: "
+                "Invalid close/open price {close_price}/{open_price}").format(
+                    id_or_ins=order_book_id, close_price=close_price, open_price=open_price
+                )
+            )
+            continue
+
+        delta_quantity = (account_value * target_percent / close_price) - current_quantities.get(order_book_id, 0)
         delta_quantity = _round_order_quantity(env.data_proxy.instrument(order_book_id), delta_quantity)
         if delta_quantity == 0:
             continue
         elif delta_quantity > 0:
             quantity, side, position_effect = delta_quantity, SIDE.BUY, POSITION_EFFECT.OPEN
             order_list = open_orders
+            target_style = open_style
         else:
             quantity, side, position_effect = abs(delta_quantity), SIDE.SELL, POSITION_EFFECT.CLOSE
             order_list = close_orders
-        if target_price:
-            order = Order.__from_create__(order_book_id, quantity, side, LimitOrder(target_price), position_effect)
-        else:
-            order = Order.__from_create__(order_book_id, quantity, side, MarketOrder(), position_effect)
-            order.set_frozen_price(price)
+            target_style = close_style
+        order = Order.__from_create__(order_book_id, quantity, side, target_style, position_effect)
+        if isinstance(target_style, MarketOrder):
+            order.set_frozen_price(last_price)
         order_list.append(order)
 
     return list(env.submit_order(o) for o in chain(close_orders, open_orders))
 
 
 @export_as_api
 @ExecutionContext.enforce_phase(EXECUTION_PHASE.ON_INIT,
```

### Comparing `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_accounts/mod.py` & `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_scheduler/mod.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,43 @@
 # -*- coding: utf-8 -*-
-# 版权所有 2019 深圳米筐科技有限公司（下称“米筐科技”）
+# 版权所有 2020 深圳米筐科技有限公司（下称“米筐科技”）
 #
 # 除非遵守当前许可，否则不得使用本软件。
 #
 #     * 非商业用途（非商业用途指个人出于非商业目的使用本软件，或者高校、研究所等非营利机构出于教育、科研等目的使用本软件）：
-#         遵守 Apache License 2.0（下称“Apache 2.0 许可”），
-#         您可以在以下位置获得 Apache 2.0 许可的副本：http://www.apache.org/licenses/LICENSE-2.0。
+#         遵守 Apache License 2.0（下称“Apache 2.0 许可”），您可以在以下位置获得 Apache 2.0 许可的副本：
+#         http://www.apache.org/licenses/LICENSE-2.0。
 #         除非法律有要求或以书面形式达成协议，否则本软件分发时需保持当前许可“原样”不变，且不得附加任何条件。
 #
 #     * 商业用途（商业用途指个人出于任何商业目的使用本软件，或者法人或其他组织出于任何目的使用本软件）：
-#         未经米筐科技授权，任何个人不得出于任何商业目的使用本软件（包括但不限于向第三方提供、销售、出租、出借、转让本软件、
-#         本软件的衍生产品、引用或借鉴了本软件功能或源代码的产品或服务），任何法人或其他组织不得出于任何目的使用本软件，
-#         否则米筐科技有权追究相应的知识产权侵权责任。
+#         未经米筐科技授权，任何个人不得出于任何商业目的使用本软件（包括但不限于向第三方提供、销售、出租、出借、转让本软件、本软件的衍生产品、引用或借鉴了本软件功能或源代码的产品或服务），任何法人或其他组织不得出于任何目的使用本软件，否则米筐科技有权追究相应的知识产权侵权责任。
 #         在此前提下，对本软件的使用同样需要遵守 Apache 2.0 许可，Apache 2.0 许可与本许可冲突之处，以本许可为准。
 #         详细的授权流程，请联系 public@ricequant.com 获取。
-
-from typing import Any
-
-from rqalpha.utils import INST_TYPE_IN_STOCK_ACCOUNT
 from rqalpha.interface import AbstractMod
-from rqalpha.const import DEFAULT_ACCOUNT_TYPE, INSTRUMENT_TYPE
-from rqalpha.environment import Environment
-
-from .position_model import StockPosition
-from .position_validator import PositionValidator
+from rqalpha.const import DEFAULT_ACCOUNT_TYPE
+from rqalpha.api import export_as_api
 
 
-class AccountMod(AbstractMod):
+class SchedulerMod(AbstractMod):
+    def __init__(self):
+        self._scheduler = None
 
     def start_up(self, env, mod_config):
-        # type: (Environment, Any) -> None
-
-        StockPosition.dividend_reinvestment = mod_config.dividend_reinvestment
-        StockPosition.cash_return_by_stock_delisted = mod_config.cash_return_by_stock_delisted
-        StockPosition.t_plus_enabled = mod_config.stock_t1
-
-        pos_validator = PositionValidator()
-        if mod_config.validate_future_position:
-            env.add_frontend_validator(pos_validator, INSTRUMENT_TYPE.FUTURE)
-        if mod_config.validate_stock_position:
-            for ins_type in INST_TYPE_IN_STOCK_ACCOUNT:
-                env.add_frontend_validator(pos_validator, ins_type)
-
-        if DEFAULT_ACCOUNT_TYPE.FUTURE in env.config.base.accounts:
-            # 注入期货API
-            # noinspection PyUnresolvedReferences
-            from .api import api_future
-        if DEFAULT_ACCOUNT_TYPE.STOCK in env.config.base.accounts:
-            # 注入股票API
-            # noinspection PyUnresolvedReferences
-            from .api import api_stock
+        if not any(t in env.config.base.accounts for t in (DEFAULT_ACCOUNT_TYPE.STOCK, DEFAULT_ACCOUNT_TYPE.FUTURE)):
+            return 
+        from .scheduler import Scheduler, market_close, market_open, physical_time
+        self._scheduler = Scheduler(env.config.base.frequency)
+        export_as_api(self._scheduler, name='scheduler')
+        export_as_api(market_open)
+        export_as_api(market_close)
+        export_as_api(physical_time)
 
     def tear_down(self, code, exception=None):
         pass
+
+    def get_state(self):
+        if self._scheduler is not None:
+            return self._scheduler.get_state()
+
+    def set_state(self, state):
+        if self._scheduler is not None:
+            self._scheduler.set_state(state)
```

### Comparing `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_accounts/position_model.py` & `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_accounts/position_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,23 +15,22 @@
 #         在此前提下，对本软件的使用同样需要遵守 Apache 2.0 许可，Apache 2.0 许可与本许可冲突之处，以本许可为准。
 #         详细的授权流程，请联系 public@ricequant.com 获取。
 
 from datetime import date
 
 from decimal import Decimal
 
-from rqalpha.utils.functools import lru_cache
 from rqalpha.model.trade import Trade
 from rqalpha.const import POSITION_DIRECTION, SIDE, POSITION_EFFECT, DEFAULT_ACCOUNT_TYPE, INSTRUMENT_TYPE
 from rqalpha.environment import Environment
 from rqalpha.portfolio.position import Position, PositionProxy
 from rqalpha.data.data_proxy import DataProxy
-from rqalpha.utils import INST_TYPE_IN_STOCK_ACCOUNT
+from rqalpha.utils import INST_TYPE_IN_STOCK_ACCOUNT, is_valid_price
 from rqalpha.utils.logger import user_system_log
-from rqalpha.utils.class_helper import deprecated_property
+from rqalpha.utils.class_helper import deprecated_property, cached_property
 from rqalpha.utils.i18n import gettext as _
 
 
 def _int_to_date(d):
     r, d = divmod(d, 100)
     y, m = divmod(r, 100)
     return date(year=y, month=m, day=d)
@@ -97,15 +96,15 @@
     def before_trading(self, trading_date):
         # type: (date) -> float
         delta_cash = super(StockPosition, self).before_trading(trading_date)
         if self._quantity == 0 and not self._dividend_receivable:
             return delta_cash
         if self.direction != POSITION_DIRECTION.LONG:
             raise RuntimeError("direction of stock position {} is not supposed to be short".format(self._order_book_id))
-        data_proxy = Environment.get_instance().data_proxy
+        data_proxy = self._env.data_proxy
         self._handle_dividend_book_closure(trading_date, data_proxy)
         delta_cash += self._handle_dividend_payable(trading_date)
         self._handle_split(trading_date, data_proxy)
         return delta_cash
 
     def apply_trade(self, trade):
         # type: (Trade) -> float
@@ -148,29 +147,30 @@
                     # 把购买 successor 消耗的 cash 补充回来
                     delta_cash = self.market_value
             if self.cash_return_by_stock_delisted:
                 delta_cash = self.market_value
             self._quantity = self._old_quantity = 0
         return delta_cash
 
-    @property
-    @lru_cache()
+    @cached_property
     def _market_tplus(self):
         return self._instrument.market_tplus
 
     def _handle_dividend_book_closure(self, trading_date, data_proxy):
         # type: (date, DataProxy) -> None
         last_date = data_proxy.get_previous_trading_date(trading_date)
         dividend = data_proxy.get_dividend_by_book_date(self._order_book_id, last_date)
         if dividend is None:
             return
         dividend_per_share = sum(dividend['dividend_cash_before_tax'] / dividend['round_lot'])
         if dividend_per_share != dividend_per_share:
             raise RuntimeError("Dividend per share of {} is not supposed to be nan.".format(self._order_book_id))
         self._avg_price -= dividend_per_share
+        # 前一天结算发生了除息, 此时 last_price 还是前一个交易日的收盘价，需要改为 除息后收盘价, 否则影响在before_trading中查看盈亏
+        self._last_price -= dividend_per_share
 
         try:
             payable_date = _int_to_date(dividend["payable_date"][0])
         except ValueError:
             payable_date = _int_to_date(dividend["ex_dividend_date"][0])
 
         self._dividend_receivable = (payable_date, self._quantity * dividend_per_share)
@@ -199,15 +199,14 @@
 
     def _handle_split(self, trading_date, data_proxy):
         ratio = data_proxy.get_split_by_ex_date(self._order_book_id, trading_date)
         if ratio is None:
             return
         self._avg_price /= ratio
         self._last_price /= ratio
-        self._prev_close /= ratio
         ratio = Decimal(ratio)
         # int(6000 * 1.15) -> 6899
         self._old_quantity = self._quantity = int(Decimal(self._quantity) * ratio)
         self._logical_old_quantity = int(Decimal(self._logical_old_quantity) * ratio)
 
 
 class FuturePosition(Position):
@@ -216,23 +215,21 @@
         "position_pnl", "last_price"
     )
     __instrument_types__ = [INSTRUMENT_TYPE.FUTURE]
 
     old_quantity = property(lambda self: self._old_quantity)
     today_quantity = property(lambda self: self._quantity - self._old_quantity)
 
-    @property
-    @lru_cache()
+    @cached_property
     def contract_multiplier(self):
         return self._instrument.contract_multiplier
 
-    @property
-    @lru_cache()
+    @cached_property
     def margin_rate(self):
-        return self._instrument.margin_rate * Environment.get_instance().config.base.margin_multiplier
+        return self._instrument.margin_rate * self._env.config.base.margin_multiplier
 
     @property
     def equity(self):
         # type: () -> float
         """"""
         return self._quantity * (self.last_price - self._avg_price) * self.contract_multiplier * self._direction_factor
 
@@ -279,28 +276,41 @@
         if trade.position_effect == POSITION_EFFECT.OPEN:
             return -1 * trade.transaction_cost
         else:
             return -1 * trade.transaction_cost + (
                     trade.last_price - self._avg_price
             ) * trade.last_quantity * self.contract_multiplier * self._direction_factor
 
+    @property
+    def prev_close(self):
+        if not is_valid_price(self._prev_close):
+            if self._env.config.mod.sys_accounts.futures_settlement_price_type == "settlement":
+                self._prev_close = self._env.data_proxy.get_prev_settlement(self._order_book_id, self._env.trading_dt)
+            else:
+                self._prev_close = super().prev_close
+        return self._prev_close
+
     def settlement(self, trading_date):
         # type: (date) -> float
         super(FuturePosition, self).settlement(trading_date)
         if self._quantity == 0:
             return 0
-        data_proxy = Environment.get_instance().data_proxy
+        data_proxy = self._env.data_proxy
         instrument = data_proxy.instrument(self._order_book_id)
         next_date = data_proxy.get_next_trading_date(trading_date)
-        delta_cash = self.equity
         if instrument.de_listed_at(next_date):
             user_system_log.warn(_(u"{order_book_id} is expired, close all positions by system").format(
                 order_book_id=self._order_book_id
             ))
             self._quantity = self._old_quantity = 0
+
+        if self._env.config.mod.sys_accounts.futures_settlement_price_type == "settlement":
+            # 逐日盯市按照结算价结算
+            self._last_price = self._env.data_proxy.get_settle_price(self._order_book_id, self._env.trading_dt)
+        delta_cash = self.equity
         self._avg_price = self.last_price
         return delta_cash
 
 
 class StockPositionProxy(PositionProxy):
     __repr_properties__ = (
         "order_book_id", "quantity", "avg_price", "market_value"
```

### Comparing `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_accounts/position_validator.py` & `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_accounts/position_validator.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/__init__.py` & `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,16 +65,16 @@
 ))
 inject_run_param(click.Option(
     ('-o', '--output-file', 'mod__sys_analyser__output_file'),
     type=click.Path(writable=True),
     help=_("[sys_analyser] output result pickle file")
 ))
 inject_run_param(click.Option(
-    ('-p', '--plot/--no-plot', 'mod__sys_analyser__plot'),
-    default=None,
+    ('-p', '--plot', 'mod__sys_analyser__plot'),
+    default=None, is_flag=False, flag_value="default",
     help=_("[sys_analyser] plot result")
 ))
 inject_run_param(click.Option(
     ('--plot-save', 'mod__sys_analyser__plot_save_file'),
     default=None,
     help=_("[sys_analyser] save plot to file")
 ))
```

### Comparing `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/mod.py` & `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/mod.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,25 +22,26 @@
 import datetime
 from operator import attrgetter
 from collections import defaultdict
 from typing import Dict, Optional, List, Tuple, Union, Iterable
 
 import numpy as np
 import pandas as pd
-from rqrisk import Risk, WEEKLY
+from rqrisk import Risk, WEEKLY, MONTHLY
 
 from rqalpha.const import EXIT_CODE, DEFAULT_ACCOUNT_TYPE, INSTRUMENT_TYPE, POSITION_DIRECTION
 from rqalpha.core.events import EVENT
 from rqalpha.interface import AbstractMod, AbstractPosition
 from rqalpha.utils.i18n import gettext as _
 from rqalpha.utils import INST_TYPE_IN_STOCK_ACCOUNT
 from rqalpha.utils.logger import user_system_log
 from rqalpha.const import DAYS_CNT
 from rqalpha.api import export_as_api
-
+from .plot.consts import DefaultPlot, PLOT_TEMPLATE
+from .plot.utils import max_ddd as _max_ddd
 from .plot_store import PlotStore
 
 
 def _get_yearly_risk_free_rates(
         data_proxy, start_date: datetime.date, end_date: datetime.date
 ) -> Iterable[Tuple[int, float]]:
     while start_date <= end_date:
@@ -57,14 +58,15 @@
 
         self._orders = []
         self._trades = []
         self._total_portfolios = []
         self._total_benchmark_portfolios = []
         self._sub_accounts = defaultdict(list)
         self._positions = defaultdict(list)
+        self._daily_pnl = []
 
         self._benchmark_daily_returns = []
         self._portfolio_daily_returns = []
 
         self._benchmark: Optional[List[Tuple[str, float]]] = None
 
         self._plot_store = None
@@ -75,33 +77,35 @@
             'portfolio_daily_returns': [float(v) for v in self._portfolio_daily_returns],
             'total_portfolios': self._total_portfolios,
             'total_benchmark_portfolios': self._total_benchmark_portfolios,
             'sub_accounts': self._sub_accounts,
             'positions': self._positions,
             'orders': self._orders,
             'trades': self._trades,
+            'daily_pnl': self._daily_pnl,
         }).encode('utf-8')
 
     def set_state(self, state):
         value = jsonpickle.loads(state.decode('utf-8'))
         self._benchmark_daily_returns = value['benchmark_daily_returns']
         self._portfolio_daily_returns = value["portfolio_daily_returns"]
         self._total_portfolios = value['total_portfolios']
         self._total_benchmark_portfolios = value["total_benchmark_portfolios"]
         self._sub_accounts = value['sub_accounts']
         self._positions = value["positions"]
         self._orders = value['orders']
         self._trades = value["trades"]
+        self._daily_pnl = value.get("daily_pnl", [])
 
     def start_up(self, env, mod_config):
         self._env = env
         self._mod_config = mod_config
         self._enabled = (
             mod_config.record or mod_config.plot or mod_config.output_file or
-            mod_config.plot_save_file or mod_config.report_save_path or mod_config.bechmark
+            mod_config.plot_save_file or mod_config.report_save_path or mod_config.benchmark
         )
         if self._enabled:
             env.event_bus.add_listener(EVENT.POST_SYSTEM_INIT, self._subscribe_events)
 
             if not mod_config.benchmark:
                 if getattr(env.config.base, "benchmark", None):
                     user_system_log.warning(
@@ -124,15 +128,22 @@
             if bar.close != bar.close:
                 daily_return_list.append((0.0, benchmark[1]))
             else:
                 daily_return_list.append((bar.close / bar.prev_close - 1.0, benchmark[1]))
             weights += benchmark[1]
         return sum([daily[0] * daily[1] / weights for daily in daily_return_list])
 
-    def _subscribe_events(self, _):
+    def _subscribe_events(self, event):
+        if self._benchmark:
+            for order_book_id, weight in self._benchmark:
+                if self._env.data_proxy.instrument(order_book_id) is None:
+                    raise RuntimeError(
+                        _("benchmark not exists, please entry correct order_book_id").format(order_book_id)
+                    )
+
         self._env.event_bus.add_listener(EVENT.TRADE, self._collect_trade)
         self._env.event_bus.add_listener(EVENT.ORDER_CREATION_PASS, self._collect_order)
         self._env.event_bus.add_listener(EVENT.POST_SETTLEMENT, self._collect_daily)
 
     def _collect_trade(self, event):
         self._trades.append(self._to_trade_record(event.trade))
 
@@ -146,14 +157,15 @@
         self._portfolio_daily_returns.append(portfolio.daily_returns)
         self._total_portfolios.append(self._to_portfolio_record(date, portfolio))
         self._benchmark_daily_returns.append(self.get_benchmark_daily_returns())
         self._total_benchmark_portfolios.append({
             "date": date,
             "unit_net_value": (np.array(self._benchmark_daily_returns) + 1).prod()
         })
+        self._daily_pnl.append(portfolio.daily_pnl)
 
         for account_type, account in self._env.portfolio.accounts.items():
             self._sub_accounts[account_type].append(self._to_account_record(date, account))
             pos_dict = {}
             for pos in account.get_positions():
                 pos_dict.setdefault(pos.order_book_id, {})[pos.direction] = pos
 
@@ -301,14 +313,15 @@
         if self._benchmark:
             if len(self._benchmark) == 1:
                 benchmark_obid, _ = self._benchmark[0]
                 summary["benchmark"] = benchmark_obid
                 summary["benchmark_symbol"] = self._env.data_proxy.instrument(benchmark_obid).symbol
             else:
                 summary["benchmark"] = ",".join(f"{o}:{w}" for o, w in self._benchmark)
+                summary["benchmark_symbol"] = ",".join(f"{self._env.data_proxy.instrument(o).symbol}:{w}" for o, w in self._benchmark)
 
         risk_free_rate = data_proxy.get_risk_free_rate(self._env.config.base.start_date, self._env.config.base.end_date)
         risk = Risk(
             np.array(self._portfolio_daily_returns), np.array(self._benchmark_daily_returns), risk_free_rate
         )
         summary.update({
             'alpha': risk.alpha,
@@ -316,21 +329,32 @@
             'sharpe': risk.sharpe,
             'excess_sharpe': risk.excess_sharpe,
             'information_ratio': risk.information_ratio,
             'downside_risk': risk.annual_downside_risk,
             'tracking_error': risk.annual_tracking_error,
             'sortino': risk.sortino,
             'volatility': risk.annual_volatility,
-            'excess_volatility': risk.excess_volatility,
-            'excess_annual_volatility': risk.excess_annual_volatility,
+            'excess_volatility': risk.excess_annual_volatility,
             'max_drawdown': risk.max_drawdown,
-            'excess_max_drawdown': risk.excess_max_drawdown,
-            'excess_returns': risk.excess_return_rate,
-            'excess_annual_returns': risk.excess_annual_return,
+            'excess_max_drawdown': risk.geometric_excess_drawdown,
+            'excess_returns': risk.geometric_excess_return,
+            'excess_annual_returns': risk.geometric_excess_annual_return,
             'var': risk.var,
+            "win_rate": risk.win_rate,
+            "excess_win_rate": risk.excess_win_rate,
+            "excess_cum_returns": risk.arithmetic_excess_return,
+        })
+
+        # 盈亏比
+        daily_pnl = np.array(self._daily_pnl)
+        profit, loss = daily_pnl[daily_pnl > 0], daily_pnl[daily_pnl < 0]
+        profit, loss = profit.mean() if len(profit) else 0, loss.mean() if len(loss) else 0
+
+        summary.update({
+            "profit_loss_rate": np.abs(profit / loss) if loss else np.nan
         })
 
         summary.update({
             'total_value': self._env.portfolio.total_value,
             'cash': self._env.portfolio.cash,
             'total_returns': self._env.portfolio.total_returns,
             'annualized_returns': self._env.portfolio.annualized_returns,
@@ -341,26 +365,36 @@
         if self._benchmark:
             benchmark_total_returns = (np.array(self._benchmark_daily_returns) + 1.0).prod() - 1.0
             summary['benchmark_total_returns'] = benchmark_total_returns
             date_count = len(self._benchmark_daily_returns)
             benchmark_annualized_returns = (benchmark_total_returns + 1) ** (DAYS_CNT.TRADING_DAYS_A_YEAR / date_count) - 1
             summary['benchmark_annualized_returns'] = benchmark_annualized_returns
 
-            # 新增一个超额累计收益
-            summary['excess_cum_returns'] = summary["total_returns"] - summary["benchmark_total_returns"]
-
         trades = pd.DataFrame(self._trades)
         if 'datetime' in trades.columns:
             trades = trades.set_index(pd.DatetimeIndex(trades['datetime']))
 
         df = pd.DataFrame(self._total_portfolios)
         df['date'] = pd.to_datetime(df['date'])
         total_portfolios = df.set_index('date').sort_index()
-        weekly_nav = df.resample("W", on="date").last().set_index("date").unit_net_value.dropna()
+        df.index = df['date']
+        weekly_nav = df.resample("W").last().set_index("date").unit_net_value.dropna()
+        monthly_nav = df.resample("M").last().set_index("date").unit_net_value.dropna()
         weekly_returns = (weekly_nav / weekly_nav.shift(1).fillna(1)).fillna(0) - 1
+        monthly_returns = (monthly_nav / monthly_nav.shift(1).fillna(1)).fillna(0) - 1
+
+        # 最长回撤持续期
+        max_ddd = _max_ddd(total_portfolios.unit_net_value.values, total_portfolios.index)
+        summary["max_drawdown_duration"] = max_ddd
+        summary.update({
+            "max_drawdown_duration_start_date": str(max_ddd.start_date),
+            "max_drawdown_duration_end_date": str(max_ddd.end_date),
+            "max_drawdown_duration_days": (max_ddd.end_date - max_ddd.start_date).days,
+        })
+
         result_dict = {
             'summary': summary,
             'trades': trades,
             'portfolio': total_portfolios,
         }
 
         if not trades.empty and all(
@@ -376,30 +410,61 @@
         else:
             summary["turnover"] = np.nan
 
         if self._benchmark:
             df = pd.DataFrame(self._total_benchmark_portfolios)
             df['date'] = pd.to_datetime(df['date'])
             benchmark_portfolios = df.set_index('date').sort_index()
-            weekly_b_nav = df.resample("W", on="date").last().set_index("date").unit_net_value.dropna()
+            df.index = df['date']
+            weekly_b_nav = df.resample("W").last().set_index("date").unit_net_value.dropna()
+            monthly_b_nav = df.resample("M").last().set_index("date").unit_net_value.dropna()
             weekly_b_returns = (weekly_b_nav / weekly_b_nav.shift(1).fillna(1)).fillna(0) - 1
+            monthly_b_returns = (monthly_b_nav / monthly_b_nav.shift(1).fillna(1)).fillna(0) - 1
             result_dict['benchmark_portfolio'] = benchmark_portfolios
+            # 超额收益最长回撤持续期
+            ex_returns = total_portfolios.unit_net_value / benchmark_portfolios.unit_net_value - 1
+            max_ddd = _max_ddd(ex_returns + 1, total_portfolios.index)
+            result_dict["summary"]["excess_max_drawdown_duration"] = max_ddd
+            result_dict["summary"]["excess_max_drawdown_duration_start_date"] = str(max_ddd.start_date)
+            result_dict["summary"]["excess_max_drawdown_duration_end_date"] = str(max_ddd.end_date)
+            result_dict["summary"]["excess_max_drawdown_duration_days"] = (max_ddd.end_date - max_ddd.start_date).days
         else:
             weekly_b_returns = pandas.Series(index=weekly_returns.index)
+            monthly_b_returns = pandas.Series(index=monthly_returns.index)
+
+        # 周度风险指标
         weekly_risk = Risk(weekly_returns, weekly_b_returns, risk_free_rate, WEEKLY)
         summary.update({
             "weekly_alpha": weekly_risk.alpha,
             "weekly_beta": weekly_risk.beta,
             "weekly_sharpe": weekly_risk.sharpe,
             "weekly_sortino": weekly_risk.sortino,
-            'weekly_information_ratio': weekly_risk.information_ratio,
-            "weekly_tracking_error": weekly_risk.tracking_error,
+            "weekly_information_ratio": weekly_risk.information_ratio,
+            "weekly_tracking_error": weekly_risk.annual_tracking_error,
             "weekly_max_drawdown": weekly_risk.max_drawdown,
+            "weekly_win_rate": weekly_risk.win_rate,
+            "weekly_volatility": weekly_risk.annual_volatility,
+            "weekly_ulcer_index": weekly_risk.ulcer_index,
+            "weekly_ulcer_performance_index": weekly_risk.ulcer_performance_index,
+        })
+
+        # 月度风险指标
+        monthly_risk = Risk(monthly_returns, monthly_b_returns, risk_free_rate, MONTHLY)
+        summary.update({
+            "monthly_sharpe": monthly_risk.sharpe,
+            "monthly_volatility": monthly_risk.annual_volatility,
+            "monthly_excess_win_rate": monthly_risk.excess_win_rate,
         })
 
+        if self._benchmark:
+            summary.update({
+                "weekly_excess_ulcer_index": weekly_risk.excess_ulcer_index,
+                "weekly_excess_ulcer_performance_index": weekly_risk.excess_ulcer_performance_index,
+            })
+
         plots = self._plot_store.get_plots()
         if plots:
             plots_items = defaultdict(dict)
             for series_name, value_dict in plots.items():
                 for date, value in value_dict.items():
                     plots_items[date][series_name] = value
                     plots_items[date]["date"] = date
@@ -430,16 +495,19 @@
             with open(self._mod_config.output_file, 'wb') as f:
                 pickle.dump(result_dict, f)
 
         if self._mod_config.report_save_path:
             from .report import generate_report
             generate_report(result_dict, self._mod_config.report_save_path)
 
-        if self._mod_config.plot or self._mod_config.plot_save_file:
+        _plot = True if self._mod_config.plot else False
+
+        if _plot or self._mod_config.plot_save_file:
             from .plot import plot_result
             plot_config = self._mod_config.plot_config
+            _plot_template_cls = PLOT_TEMPLATE.get(self._mod_config.plot, DefaultPlot)
             plot_result(
                 result_dict, self._mod_config.plot, self._mod_config.plot_save_file,
-                plot_config.weekly_indicators, plot_config.open_close_points
+                plot_config.weekly_indicators, plot_config.open_close_points, _plot_template_cls
             )
 
         return result_dict
```

### Comparing `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/plot/__init__.py` & `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/plot/plot.py` & `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot/plot.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,20 +22,20 @@
 import pandas as pd
 from matplotlib.axes import Axes
 from matplotlib.figure import Figure
 from matplotlib import gridspec, ticker, image as mpimg, pyplot
 
 import rqalpha
 from rqalpha.const import POSITION_EFFECT
-from .utils import IndicatorInfo, LineInfo, max_ddd as _max_ddd, max_dd as _max_dd, SpotInfo
+from .utils import IndicatorInfo, LineInfo, max_dd as _max_dd, SpotInfo, max_ddd as _max_ddd
 from .utils import weekly_returns, trading_dates_index
-from .consts import INDICATOR_WIDTH, INDICATOR_VALUE_HEIGHT, INDICATOR_LABEL_HEIGHT
+from .consts import PlotTemplate, DefaultPlot
 from .consts import IMG_WIDTH, INDICATOR_AREA_HEIGHT, PLOT_AREA_HEIGHT, USER_PLOT_AREA_HEIGHT
-from .consts import LABEL_FONT_SIZE, BLACK
-from .consts import INDICATORS, WEEKLY_INDICATORS, EXCESS_INDICATORS, MAX_DD, MAX_DDD, OPEN_POINT, CLOSE_POINT
+from .consts import LABEL_FONT_SIZE, BLACK, SUPPORT_CHINESE
+from .consts import MAX_DD, MAX_DDD, OPEN_POINT, CLOSE_POINT
 from .consts import LINE_BENCHMARK, LINE_STRATEGY, LINE_WEEKLY_BENCHMARK, LINE_WEEKLY, LINE_EXCESS
 
 
 class SubPlot:
     height: int
     right_pad: Optional[int] = None
 
@@ -43,25 +43,31 @@
         raise NotImplementedError
 
 
 class IndicatorArea(SubPlot):
     height: int = INDICATOR_AREA_HEIGHT
     right_pad = -1
 
-    def __init__(self, indicators: List[List[IndicatorInfo]], indicator_values: Mapping[str, float]):
+    def __init__(
+            self, indicators: List[List[IndicatorInfo]], indicator_values: Mapping[str, float],
+            plot_template: PlotTemplate
+    ):
         self._indicators = indicators
         self._values = indicator_values
+        self._template = plot_template
 
     def plot(self, ax: Axes):
         ax.axis("off")
         for lineno, indicators in enumerate(self._indicators[::-1]):  # lineno: 自下而上的行号
+            _extra_width = 0  # 用于保存加长的部分, 原因是部分label太长出现覆盖
             for index_in_line, i in enumerate(indicators):
-                x = index_in_line * INDICATOR_WIDTH
-                y_value = lineno * (INDICATOR_VALUE_HEIGHT + INDICATOR_LABEL_HEIGHT)
-                y_label = y_value + INDICATOR_LABEL_HEIGHT
+                _extra_width += (i.label_width_multiplier - 1) * self._template.INDICATOR_WIDTH
+                x = index_in_line * self._template.INDICATOR_WIDTH + _extra_width
+                y_value = lineno * (self._template.INDICATOR_VALUE_HEIGHT + self._template.INDICATOR_LABEL_HEIGHT)
+                y_label = y_value + self._template.INDICATOR_LABEL_HEIGHT
                 try:
                     value = i.formatter.format(self._values[i.key])
                 except KeyError:
                     value = "nan"
                 ax.text(x, y_label, i.label, color=i.color, fontsize=LABEL_FONT_SIZE),
                 ax.text(x, y_value, value, color=BLACK, fontsize=i.value_font_size)
 
@@ -89,16 +95,16 @@
             self._returns.index[positions], self._returns[positions],
             info.marker, color=info.color, markersize=info.markersize, alpha=info.alpha, label=info.label
         )
 
     def plot(self, ax: Axes):
         ax.get_xaxis().set_minor_locator(ticker.AutoMinorLocator())
         ax.get_yaxis().set_minor_locator(ticker.AutoMinorLocator())
-        ax.grid(b=True, which='minor', linewidth=.2)
-        ax.grid(b=True, which='major', linewidth=1)
+        ax.grid(visible=True, which='minor', linewidth=.2)
+        ax.grid(visible=True, which='major', linewidth=1)
         ax.patch.set_alpha(0.6)
 
         # plot lines
         for returns, info in self._lines:
             self._plot_line(ax, returns, info)
         # plot MaxDD/MaxDDD
         for positions, info in self._spots_on_returns:
@@ -142,66 +148,79 @@
             alpha=0.4,
         )
         
 
 def _plot(title: str, sub_plots: List[SubPlot]):
     img_height = sum(s.height for s in sub_plots)
     water_mark = WaterMark(IMG_WIDTH, img_height)
-    fig = pyplot.figure(title, figsize=(IMG_WIDTH, img_height), dpi=water_mark.dpi)
+    fig = pyplot.figure(title, figsize=(IMG_WIDTH, img_height), dpi=water_mark.dpi, clear=True)
     water_mark.plot(fig)
 
     gs = gridspec.GridSpec(img_height, 8, figure=fig)
     last_height = 0
     for p in sub_plots:
         p.plot(pyplot.subplot(gs[last_height:last_height + p.height, :p.right_pad]))
         last_height += p.height
 
     pyplot.tight_layout()
     return fig
 
 
-def plot_result(result_dict, show=True, save=None, weekly_indicators: bool = False, open_close_points: bool = False):
+def plot_result(
+        result_dict, show=True, save=None, weekly_indicators: bool = False, open_close_points: bool = False,
+        plot_template_cls=DefaultPlot
+):
     summary = result_dict["summary"]
     portfolio = result_dict["portfolio"]
 
     return_lines: List[Tuple[pd.Series, LineInfo]] = [(portfolio.unit_net_value - 1, LINE_STRATEGY)]
     if "benchmark_portfolio" in result_dict:
         benchmark_portfolio = result_dict["benchmark_portfolio"]
-        ex_returns = portfolio.unit_net_value - benchmark_portfolio.unit_net_value
+        plot_template = plot_template_cls(portfolio.unit_net_value, benchmark_portfolio.unit_net_value)
+        ex_returns = plot_template.geometric_excess_returns
         ex_max_dd_ddd = "MaxDD {}\nMaxDDD {}".format(
             _max_dd(ex_returns + 1, portfolio.index).repr, _max_ddd(ex_returns + 1, portfolio.index).repr
         )
-        indicators = INDICATORS + [EXCESS_INDICATORS]
+        indicators = plot_template.INDICATORS + plot_template.EXCESS_INDICATORS
+
+        # 在图例中输出基准信息
+        _b_str = summary["benchmark_symbol"] if SUPPORT_CHINESE else summary["benchmark"]
+        _INFO = LineInfo(
+            LINE_BENCHMARK.label + "({})".format(_b_str), LINE_BENCHMARK.color,
+            LINE_BENCHMARK.alpha, LINE_BENCHMARK.linewidth
+        )
+
         return_lines.extend([
-            (benchmark_portfolio.unit_net_value - 1, LINE_BENCHMARK),
+            (benchmark_portfolio.unit_net_value - 1, _INFO),
             (ex_returns, LINE_EXCESS),
         ])
         if weekly_indicators:
             return_lines.append((weekly_returns(benchmark_portfolio), LINE_WEEKLY_BENCHMARK))
     else:
         ex_max_dd_ddd = "nan"
-        indicators = INDICATORS
+        plot_template = plot_template_cls(portfolio.unit_net_value, None)
+        indicators = plot_template.INDICATORS
     if weekly_indicators:
         return_lines.append((weekly_returns(portfolio), LINE_WEEKLY))
-        indicators.append(WEEKLY_INDICATORS)
+        indicators.extend(plot_template.WEEKLY_INDICATORS)
     max_dd = _max_dd(portfolio.unit_net_value.values, portfolio.index)
-    max_ddd = _max_ddd(portfolio.unit_net_value.values, portfolio.index)
+    max_ddd = summary["max_drawdown_duration"]
     spots_on_returns: List[Tuple[Sequence[int], SpotInfo]] = [
         ([max_dd.start, max_dd.end], MAX_DD),
         ([max_ddd.start, max_ddd.end], MAX_DDD)
     ]
-    if open_close_points:
+    if open_close_points and not result_dict["trades"].empty:
         trades: pd.DataFrame = result_dict["trades"]
         spots_on_returns.append((trading_dates_index(trades, POSITION_EFFECT.CLOSE, portfolio.index), CLOSE_POINT))
         spots_on_returns.append((trading_dates_index(trades, POSITION_EFFECT.OPEN, portfolio.index), OPEN_POINT))
 
     sub_plots = [IndicatorArea(indicators, ChainMap(summary, {
         "max_dd_ddd": "MaxDD {}\nMaxDDD {}".format(max_dd.repr, max_ddd.repr),
         "excess_max_dd_ddd": ex_max_dd_ddd,
-    })), ReturnPlot(
+    }), plot_template), ReturnPlot(
         portfolio.unit_net_value - 1, return_lines, spots_on_returns
     )]
     if "plots" in result_dict:
         sub_plots.append(UserPlot(result_dict["plots"]))
     
     _plot(summary["strategy_file"], sub_plots)
```

### Comparing `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/plot/utils.py` & `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 
 from collections import namedtuple
 
 import numpy as np
 from numpy import array
 from pandas import DatetimeIndex, DataFrame, Series, to_datetime
 
-IndicatorInfo = namedtuple("IndicatorInfo", ("key", "label", "color", "formatter", "value_font_size"))
+IndicatorInfo = namedtuple(
+    "IndicatorInfo", ("key", "label", "color", "formatter", "value_font_size", "label_width_multiplier")
+)
 LineInfo = namedtuple("LineInfo", ("label", "color", "alpha", "linewidth"))
 SpotInfo = namedtuple("SpotInfo", ("label", "marker", "color", "markersize", "alpha"))
 
 
 class IndexRange(namedtuple("IndexRange", ("start", "end", "start_date", "end_date"))):
     @classmethod
     def new(cls, start, end, index):
@@ -70,15 +72,14 @@
         if i - start > ddd:
             return IndexRange.new(start, i, index)
 
     return IndexRange.new(ddd_start, ddd_end, index)
 
 
 def weekly_returns(portfolio: DataFrame) -> Series:
-    return portfolio.unit_net_value.reset_index().resample(
-        "W", on="date").last().set_index("date").unit_net_value.dropna() - 1
+    return portfolio.unit_net_value.resample("W").last().dropna() - 1
 
 
 def trading_dates_index(trades: DataFrame, position_effect, index: DatetimeIndex):
     return index.searchsorted(
         to_datetime(trades[trades.position_effect == position_effect].trading_datetime), side="right"
     ) - 1
```

### Comparing `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/plot_store.py` & `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot_store.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/report/excel_template.py` & `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/report/excel_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
 class SummaryTemplate(ExcelTemplate):
     TEMPLATE_NAME = "summary"
     SCHEMA_CLASSES = {
         "概览": SingleCellSchema,
         "年度指标": VerticalSeriesSchema,
         "月度收益": VerticalSeriesSchema,
-        "月度主动收益": VerticalSeriesSchema
+        "月度超额收益（几何）": VerticalSeriesSchema
     }
 
 
 SUMMARY_TEMPLATE = SummaryTemplate()
 
 
 def generate_xlsx_reports(data, output_path):
```

### Comparing `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_progress/__init__.py` & `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_progress/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_progress/mod.py` & `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_progress/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_risk/__init__.py` & `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_risk/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_risk/mod.py` & `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_risk/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_risk/validators/__init__.py` & `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_risk/validators/cash_validator.py` & `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/cash_validator.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_risk/validators/is_trading_validator.py` & `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/price_validator.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,52 +1,61 @@
 # -*- coding: utf-8 -*-
 # 版权所有 2019 深圳米筐科技有限公司（下称“米筐科技”）
 #
 # 除非遵守当前许可，否则不得使用本软件。
 #
 #     * 非商业用途（非商业用途指个人出于非商业目的使用本软件，或者高校、研究所等非营利机构出于教育、科研等目的使用本软件）：
-#         遵守 Apache License 2.0（下称“Apache 2.0 许可”），
-#         您可以在以下位置获得 Apache 2.0 许可的副本：http://www.apache.org/licenses/LICENSE-2.0。
+#         遵守 Apache License 2.0（下称“Apache 2.0 许可”），您可以在以下位置获得 Apache 2.0 许可的副本：http://www.apache.org/licenses/LICENSE-2.0。
 #         除非法律有要求或以书面形式达成协议，否则本软件分发时需保持当前许可“原样”不变，且不得附加任何条件。
 #
 #     * 商业用途（商业用途指个人出于任何商业目的使用本软件，或者法人或其他组织出于任何目的使用本软件）：
-#         未经米筐科技授权，任何个人不得出于任何商业目的使用本软件（包括但不限于向第三方提供、销售、出租、出借、转让本软件、
-#         本软件的衍生产品、引用或借鉴了本软件功能或源代码的产品或服务），任何法人或其他组织不得出于任何目的使用本软件，
-#         否则米筐科技有权追究相应的知识产权侵权责任。
+#         未经米筐科技授权，任何个人不得出于任何商业目的使用本软件（包括但不限于向第三方提供、销售、出租、出借、转让本软件、本软件的衍生产品、引用或借鉴了本软件功能或源代码的产品或服务），任何法人或其他组织不得出于任何目的使用本软件，否则米筐科技有权追究相应的知识产权侵权责任。
 #         在此前提下，对本软件的使用同样需要遵守 Apache 2.0 许可，Apache 2.0 许可与本许可冲突之处，以本许可为准。
 #         详细的授权流程，请联系 public@ricequant.com 获取。
 
-from rqalpha.interface import AbstractFrontendValidator
 
+from rqalpha.interface import AbstractFrontendValidator
+from rqalpha.const import ORDER_TYPE, POSITION_EFFECT
 from rqalpha.utils.logger import user_system_log
+
 from rqalpha.utils.i18n import gettext as _
 
 
-class IsTradingValidator(AbstractFrontendValidator):
+class PriceValidator(AbstractFrontendValidator):
     def __init__(self, env):
         self._env = env
 
     def can_submit_order(self, order, account=None):
-        instrument = self._env.data_proxy.instrument(order.order_book_id)
-        if instrument.listed_date > self._env.trading_dt:
-            user_system_log.warn(_(u"Order Creation Failed: {order_book_id} is not listed!").format(
-                order_book_id=order.order_book_id,
-            ))
-            return False
+        if (order.type != ORDER_TYPE.LIMIT) or (order.position_effect == POSITION_EFFECT.EXERCISE):
+            return True
 
-        if instrument.de_listed_date.date() < self._env.trading_dt.date():
-            user_system_log.warn(_(u"Order Creation Failed: {order_book_id} has been delisted!").format(
+        # FIXME: it may be better to round price in data source
+        limit_up = round(self._env.price_board.get_limit_up(order.order_book_id), 4)
+        if order.price > limit_up:
+            reason = _(
+                "Order Creation Failed: limit order price {limit_price} is higher "
+                "than limit up {limit_up}, order_book_id={order_book_id}"
+            ).format(
                 order_book_id=order.order_book_id,
-            ))
+                limit_price=order.price,
+                limit_up=limit_up
+            )
+            user_system_log.warn(reason)
             return False
 
-        if instrument.type == 'CS' and self._env.data_proxy.is_suspended(order.order_book_id, self._env.trading_dt):
-            user_system_log.warn(_(u"Order Creation Failed: security {order_book_id} is suspended on {date}").format(
+        limit_down = round(self._env.price_board.get_limit_down(order.order_book_id), 4)
+        if order.price < limit_down:
+            reason = _(
+                "Order Creation Failed: limit order price {limit_price} is lower "
+                "than limit down {limit_down}, order_book_id={order_book_id}"
+            ).format(
                 order_book_id=order.order_book_id,
-                date=self._env.trading_dt.date()
-            ))
+                limit_price=order.price,
+                limit_down=limit_down
+            )
+            user_system_log.warn(reason)
             return False
 
         return True
 
     def can_cancel_order(self, order, account=None):
         return True
```

### Comparing `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_risk/validators/self_trade_validator.py` & `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/self_trade_validator.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_scheduler/__init__.py` & `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_scheduler/mod.py` & `rqalpha-5.0.0/tests/unittest/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,31 @@
 # -*- coding: utf-8 -*-
-# 版权所有 2020 深圳米筐科技有限公司（下称“米筐科技”）
+# 版权所有 2019 深圳米筐科技有限公司（下称“米筐科技”）
 #
 # 除非遵守当前许可，否则不得使用本软件。
 #
 #     * 非商业用途（非商业用途指个人出于非商业目的使用本软件，或者高校、研究所等非营利机构出于教育、科研等目的使用本软件）：
-#         遵守 Apache License 2.0（下称“Apache 2.0 许可”），您可以在以下位置获得 Apache 2.0 许可的副本：
-#         http://www.apache.org/licenses/LICENSE-2.0。
+#         遵守 Apache License 2.0（下称“Apache 2.0 许可”），您可以在以下位置获得 Apache 2.0 许可的副本：http://www.apache.org/licenses/LICENSE-2.0。
 #         除非法律有要求或以书面形式达成协议，否则本软件分发时需保持当前许可“原样”不变，且不得附加任何条件。
 #
 #     * 商业用途（商业用途指个人出于任何商业目的使用本软件，或者法人或其他组织出于任何目的使用本软件）：
 #         未经米筐科技授权，任何个人不得出于任何商业目的使用本软件（包括但不限于向第三方提供、销售、出租、出借、转让本软件、本软件的衍生产品、引用或借鉴了本软件功能或源代码的产品或服务），任何法人或其他组织不得出于任何目的使用本软件，否则米筐科技有权追究相应的知识产权侵权责任。
 #         在此前提下，对本软件的使用同样需要遵守 Apache 2.0 许可，Apache 2.0 许可与本许可冲突之处，以本许可为准。
 #         详细的授权流程，请联系 public@ricequant.com 获取。
-from rqalpha.interface import AbstractMod
-from rqalpha.const import DEFAULT_ACCOUNT_TYPE
-from rqalpha.api import export_as_api
-
-
-class SchedulerMod(AbstractMod):
-    def __init__(self):
-        self._scheduler = None
-
-    def start_up(self, env, mod_config):
-        if not any(t in env.config.base.accounts for t in (DEFAULT_ACCOUNT_TYPE.STOCK, DEFAULT_ACCOUNT_TYPE.FUTURE)):
-            return 
-        from .scheduler import Scheduler, market_close, market_open
-        self._scheduler = Scheduler(env.config.base.frequency)
-        export_as_api(self._scheduler, name='scheduler')
-        export_as_api(market_open)
-        export_as_api(market_close)
-
-    def tear_down(self, code, exception=None):
-        pass
-
-    def get_state(self):
-        if self._scheduler is not None:
-            return self._scheduler.get_state()
-
-    def set_state(self, state):
-        if self._scheduler is not None:
-            self._scheduler.set_state(state)
+
+import os
+
+from unittest import TestLoader, TestSuite, TextTestRunner
+
+
+def load_tests():
+    test_suite = TestSuite()
+    this_dir = os.path.dirname(__file__)
+    loader = TestLoader()
+    package_tests = loader.discover(start_dir=this_dir)
+    test_suite.addTests(package_tests)
+    return test_suite
+
+
+if __name__ == "__main__":
+    runner = TextTestRunner(verbosity=2)
+    runner.run(load_tests())
```

### Comparing `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_scheduler/scheduler.py` & `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_scheduler/scheduler.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,25 +27,25 @@
 from rqalpha.core.events import EVENT
 from inspect import signature
 from rqalpha.utils.exception import patch_user_exc, ModifyExceptionFromType
 from rqalpha.utils.logger import system_log
 
 
 def market_close(hour=0, minute=0):
-    if Environment.get_instance().config.base.accounts.get("STOCK") is None:
-        system_log.warning("market_close using in stock market")
+    if Environment.get_instance().config.base.accounts.get(DEFAULT_ACCOUNT_TYPE.FUTURE):
+        system_log.warning("using 'market_close' in futures/option strategy is not recommended")
     minutes_since_midnight = 15 * 60 - hour * 60 - minute
     if minutes_since_midnight < 13 * 60:
         minutes_since_midnight -= 90
     return minutes_since_midnight
 
 
 def market_open(hour=0, minute=0):
-    if Environment.get_instance().config.base.accounts.get("STOCK") is None:
-        system_log.warning("market_open using in stock market")
+    if Environment.get_instance().config.base.accounts.get(DEFAULT_ACCOUNT_TYPE.FUTURE):
+        system_log.warning("using 'market_open' in futures/option strategy is not recommended")
     minutes_since_midnight = 9 * 60 + 31 + hour * 60 + minute
     if minutes_since_midnight > 11 * 60 + 30:
         minutes_since_midnight += 90
     return minutes_since_midnight
 
 
 def physical_time(hour=0, minute=0):
```

### Comparing `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_simulation/__init__.py` & `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_simulation/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,23 +19,25 @@
 __config__ = {
     # 开启信号模式：该模式下，所有通过风控的订单将不进行撮合，直接产生交易
     "signal": False,
     # 撮合方式，其中：
     #   日回测的可选值为 "current_bar"|"vwap"（以当前 bar 收盘价｜成交量加权平均价撮合）
     #   分钟回测的可选值有 "current_bar"|"next_bar"|"vwap"（以当前 bar 收盘价｜下一个 bar 的开盘价｜成交量加权平均价撮合)
     #   tick 回测的可选值有 "last"|"best_own"|"best_counterparty"（以最新价｜己方最优价｜对手方最优价撮合）和 "counterparty_offer"（逐档撮合）
-    "matching_type": "current_bar",
+    #   matching_type 为 None 则表示根据回测频率自动选择。日/分钟回测下为 current_bar , tick 回测下为 last
+    "matching_type": None,
     # 开启对于处于涨跌停状态的证券的撮合限制
     "price_limit": True,
     # 开启对于对手盘无流动性的证券的撮合限制（仅在 tick 回测下生效）
     "liquidity_limit": False,
-    # 开启成交量限制（仅在日和分钟回测下生效）
+    # 开启成交量限制
     #   开启该限制意味着每个 bar 的累计成交量将不会超过该时间段内市场上总成交量的一定比值（volume_percent）
+    #   开启该限制意味着每个 tick 的累计成交量将不会超过当前tick与上一个tick的市场总成交量之差的一定比值
     "volume_limit": True,
-    # 每个 bar 可成交数量占市场总成交量的比值，在 volume_limit 开启时生效
+    # 每个 bar/tick 可成交数量占市场总成交量的比值，在 volume_limit 开启时生效
     "volume_percent": 0.25,
     # 滑点模型，可选值有 "PriceRatioSlippage"（按价格比例设置滑点）和 "TickSizeSlippage"（按跳设置滑点）
     #    亦可自己实现滑点模型，选择自己实现的滑点模型时，此处需传入包含包和模块的完整类路径
     #    滑点模型类需继承自 rqalpha.mod.rqalpha_mod_sys_simulation.slippage.BaseSlippage
     "slippage_model": "PriceRatioSlippage",
     # 设置滑点值，对于 PriceRatioSlippage 表示价格的比例，对于 TickSizeSlippage 表示跳的数量
     "slippage": 0,
```

### Comparing `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py` & `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,62 +10,54 @@
 #
 #     * 商业用途（商业用途指个人出于任何商业目的使用本软件，或者法人或其他组织出于任何目的使用本软件）：
 #         未经米筐科技授权，任何个人不得出于任何商业目的使用本软件（包括但不限于向第三方提供、销售、出租、出借、转让本软件、
 #         本软件的衍生产品、引用或借鉴了本软件功能或源代码的产品或服务），任何法人或其他组织不得出于任何目的使用本软件，
 #         否则米筐科技有权追究相应的知识产权侵权责任。
 #         在此前提下，对本软件的使用同样需要遵守 Apache 2.0 许可，Apache 2.0 许可与本许可冲突之处，以本许可为准。
 #         详细的授权流程，请联系 public@ricequant.com 获取。
-
+import datetime
 from collections import defaultdict
-
 from rqalpha.const import MATCHING_TYPE, ORDER_TYPE, POSITION_EFFECT, SIDE
 from rqalpha.environment import Environment
 from rqalpha.core.events import EVENT, Event
-from rqalpha.model.order import Order
+from rqalpha.model.order import Order, ALGO_ORDER_STYLES
 from rqalpha.model.trade import Trade
+from rqalpha.model.tick import TickObject
 from rqalpha.portfolio.account import Account
 from rqalpha.utils import is_valid_price
+from typing import Dict
 from rqalpha.utils.i18n import gettext as _
 from .slippage import SlippageDecider
 
 
 class AbstractMatcher:
     def match(self, account, order, open_auction):
         # type: (Account, Order, bool) -> None
         raise NotImplementedError
 
-    def update(self):
+    def update(self, event):
         raise NotImplementedError
 
 
-class DefaultMatcher(AbstractMatcher):
+class DefaultBarMatcher(AbstractMatcher):
     def __init__(self, env, mod_config):
         self._slippage_decider = SlippageDecider(mod_config.slippage_model, mod_config.slippage)
         self._turnover = defaultdict(int)
         self._volume_percent = mod_config.volume_percent
         self._price_limit = mod_config.price_limit
-        self._liquidity_limit = mod_config.liquidity_limit and env.config.base.frequency == "tick"
-        self._inactive_limit = env.config.base.frequency != 'tick' and mod_config.inactive_limit
+        self._inactive_limit = mod_config.inactive_limit
         self._volume_limit = mod_config.volume_limit
         self._env = env  # type: Environment
         self._deal_price_decider = self._create_deal_price_decider(mod_config.matching_type)
 
     def _create_deal_price_decider(self, matching_type):
         decider_dict = {
             MATCHING_TYPE.CURRENT_BAR_CLOSE: self._current_bar_close_decider,
             MATCHING_TYPE.VWAP: self._vwap_decider,
             MATCHING_TYPE.NEXT_BAR_OPEN: self._next_bar_open_decider,
-            MATCHING_TYPE.NEXT_TICK_LAST: lambda order_book_id, side: self._env.price_board.get_last_price(
-                order_book_id),
-            MATCHING_TYPE.NEXT_TICK_BEST_OWN: lambda order_book_id, side: self._best_own_price_decider(order_book_id,
-                                                                                                       side),
-            MATCHING_TYPE.COUNTERPARTY_OFFER: None,
-            MATCHING_TYPE.NEXT_TICK_BEST_COUNTERPARTY: lambda order_book_id, side: (
-                self._env.price_board.get_a1(order_book_id) if side == SIDE.BUY else self._env.price_board.get_b1(
-                    order_book_id))
         }
         return decider_dict[matching_type]
 
     def _current_bar_close_decider(self, order_book_id, _):
         try:
             return self._env.get_bar(order_book_id).close
         except (KeyError, TypeError):
@@ -81,48 +73,60 @@
         try:
             contract_multiplier = self._env.get_instrument(order_book_id).contract_multiplier
             bar = self._env.get_bar(order_book_id)
             return bar.total_turnover / bar.volume / contract_multiplier
         except (KeyError, TypeError, ZeroDivisionError):
             return 0
 
-    def _best_own_price_decider(self, order_book_id, side):
-        price = self._env.price_board.get_b1(order_book_id) if side == SIDE.BUY else self._env.price_board.get_a1(
-            order_book_id)
-        if price == 0:
-            price = self._env.price_board.get_last_price(order_book_id)
-        return price
-
     def _open_auction_deal_price_decider(self, order_book_id, _):
         return self._env.data_proxy.get_open_auction_bar(order_book_id, self._env.calendar_dt).open
 
     SUPPORT_POSITION_EFFECTS = (POSITION_EFFECT.OPEN, POSITION_EFFECT.CLOSE, POSITION_EFFECT.CLOSE_TODAY)
     SUPPORT_SIDES = (SIDE.BUY, SIDE.SELL)
 
+    def _get_bar_volume(self, order, open_auction=False):
+        if open_auction:
+            volume = self._env.data_proxy.get_open_auction_bar(order.order_book_id, self._env.calendar_dt).volume
+        else:
+            if isinstance(order.style, ALGO_ORDER_STYLES):
+                _, volume = self._env.data_proxy.get_algo_bar(order.order_book_id, order.style, self._env.calendar_dt)
+            else:
+                volume = self._env.get_bar(order.order_book_id).volume
+        return volume
+
+    def _get_deal_price(self, order, open_auction=False):
+        if open_auction:
+            deal_price = self._open_auction_deal_price_decider(order.order_book_id, order.side)
+        else:
+            if isinstance(order.style, ALGO_ORDER_STYLES):
+                deal_price, v = self._env.data_proxy.get_algo_bar(order.order_book_id, order.style, self._env.calendar_dt)
+            else:
+                deal_price = self._deal_price_decider(order.order_book_id, order.side)
+        return deal_price
+
     def match(self, account, order, open_auction):
         # type: (Account, Order, bool) -> None
         if not (order.position_effect in self.SUPPORT_POSITION_EFFECTS and order.side in self.SUPPORT_SIDES):
             raise NotImplementedError
         order_book_id = order.order_book_id
         instrument = self._env.get_instrument(order_book_id)
 
-        if open_auction:
-            deal_price = self._open_auction_deal_price_decider(order_book_id, order.side)
-        else:
-            deal_price = self._deal_price_decider(order_book_id, order.side)
+        deal_price = self._get_deal_price(order, open_auction)
 
         if not is_valid_price(deal_price):
             listed_date = instrument.listed_date.date()
             if listed_date == self._env.trading_dt.date():
                 reason = _(
                     u"Order Cancelled: current security [{order_book_id}] can not be traded"
                     u" in listed date [{listed_date}]").format(
                     order_book_id=order.order_book_id,
                     listed_date=listed_date,
                 )
+            elif isinstance(order.style, ALGO_ORDER_STYLES):
+                reason = _(u"Order Cancelled: {order_book_id} bar no volume").format(order_book_id=order.order_book_id)
             else:
                 reason = _(u"Order Cancelled: current bar [{order_book_id}] miss market data.").format(
                     order_book_id=order.order_book_id)
             order.mark_rejected(reason)
             return
 
         price_board = self._env.price_board
@@ -133,59 +137,38 @@
                 return
             # 是否限制涨跌停不成交
             if self._price_limit:
                 if order.side == SIDE.BUY and deal_price >= price_board.get_limit_up(order_book_id):
                     return
                 if order.side == SIDE.SELL and deal_price <= price_board.get_limit_down(order_book_id):
                     return
-            if self._liquidity_limit:
-                if order.side == SIDE.BUY and price_board.get_a1(order_book_id) == 0:
-                    return
-                if order.side == SIDE.SELL and price_board.get_b1(order_book_id) == 0:
-                    return
         else:
             if self._price_limit:
                 if order.side == SIDE.BUY and deal_price >= price_board.get_limit_up(order_book_id):
                     reason = _(
                         "Order Cancelled: current bar [{order_book_id}] reach the limit_up price."
                     ).format(order_book_id=order.order_book_id)
                     order.mark_rejected(reason)
                     return
                 if order.side == SIDE.SELL and deal_price <= price_board.get_limit_down(order_book_id):
                     reason = _(
                         "Order Cancelled: current bar [{order_book_id}] reach the limit_down price."
                     ).format(order_book_id=order.order_book_id)
                     order.mark_rejected(reason)
                     return
-            if self._liquidity_limit:
-                if order.side == SIDE.BUY and price_board.get_a1(order_book_id) == 0:
-                    reason = _(
-                        "Order Cancelled: [{order_book_id}] has no liquidity."
-                    ).format(order_book_id=order.order_book_id)
-                    order.mark_rejected(reason)
-                    return
-                if order.side == SIDE.SELL and price_board.get_b1(order_book_id) == 0:
-                    reason = _(
-                        "Order Cancelled: [{order_book_id}] has no liquidity."
-                    ).format(order_book_id=order.order_book_id)
-                    order.mark_rejected(reason)
-                    return
 
         if self._inactive_limit:
-            bar_volume = self._env.get_bar(order_book_id).volume
+            bar_volume = self._get_bar_volume(order, open_auction=open_auction)
             if bar_volume == 0:
                 reason = _(u"Order Cancelled: {order_book_id} bar no volume").format(order_book_id=order.order_book_id)
                 order.mark_cancelled(reason)
                 return
 
         if self._volume_limit:
-            if open_auction:
-                volume = self._env.data_proxy.get_open_auction_bar(order_book_id, self._env.calendar_dt).volume
-            else:
-                volume = self._env.get_bar(order_book_id).volume
+            volume = self._get_bar_volume(order, open_auction=open_auction)
             if volume == volume:
                 volume_limit = round(volume * self._volume_percent) - self._turnover[order.order_book_id]
 
                 round_lot = instrument.round_lot
                 volume_limit = (volume_limit // round_lot) * round_lot
                 if volume_limit <= 0:
                     if order.type == ORDER_TYPE.MARKET:
@@ -200,14 +183,15 @@
                 fill = min(order.unfilled_quantity, volume_limit)
             else:
                 fill = order.unfilled_quantity
         else:
             fill = order.unfilled_quantity
 
         ct_amount = account.calc_close_today_amount(order_book_id, fill, order.position_direction)
+
         if open_auction:
             price = deal_price
         else:
             price = self._slippage_decider.get_trade_price(order, deal_price)
 
         trade = Trade.__from_create__(
             order_id=order.order_id,
@@ -234,40 +218,288 @@
                 order_book_id=order.order_book_id,
                 order_volume=order.quantity,
                 filled_volume=order.filled_quantity,
                 volume_percent_limit=self._volume_percent * 100.0
             )
             order.mark_cancelled(reason)
 
-    def update(self):
+    def update(self, event):
         self._turnover.clear()
 
 
-class CounterPartyOfferMatcher(DefaultMatcher):
+class DefaultTickMatcher(AbstractMatcher):
+    """ tick回测使用 """
+
+    SUPPORT_POSITION_EFFECTS = (POSITION_EFFECT.OPEN, POSITION_EFFECT.CLOSE, POSITION_EFFECT.CLOSE_TODAY)
+    SUPPORT_SIDES = (SIDE.BUY, SIDE.SELL)
+
+    def __init__(self, env, mod_config):
+        self._slippage_decider = SlippageDecider(mod_config.slippage_model, mod_config.slippage)
+        self._turnover = defaultdict(int)
+        self._volume_percent = mod_config.volume_percent
+        self._price_limit = mod_config.price_limit
+        self._liquidity_limit = mod_config.liquidity_limit
+        self._volume_limit = mod_config.volume_limit
+        self._env = env  # type: Environment
+        self._deal_price_decider = self._create_deal_price_decider(mod_config.matching_type)
+
+        # 每个交易日期内的上一个时刻的tick(第一个除外)
+        self._last_tick: Dict[str, TickObject] = dict()
+        # 当前的tick
+        self._cur_tick: Dict[str, TickObject] = dict()
+
+        # 订阅一些事件
+        self._env.event_bus.add_listener(EVENT.BEFORE_TRADING, self._on_before_trading)
+
+    def _create_deal_price_decider(self, matching_type):
+        decider_dict = {
+            MATCHING_TYPE.NEXT_TICK_LAST: lambda order_book_id, side: self._env.price_board.get_last_price(
+                order_book_id),
+            MATCHING_TYPE.NEXT_TICK_BEST_OWN: lambda order_book_id, side: self._best_own_price_decider(order_book_id,
+                                                                                                       side),
+            MATCHING_TYPE.COUNTERPARTY_OFFER: None,
+            MATCHING_TYPE.NEXT_TICK_BEST_COUNTERPARTY: lambda order_book_id, side: (
+                self._env.price_board.get_a1(order_book_id) if side == SIDE.BUY else self._env.price_board.get_b1(
+                    order_book_id))
+        }
+        return decider_dict[matching_type]
+
+    def _best_own_price_decider(self, order_book_id, side):
+        """ 己方最优价 """
+        price = self._env.price_board.get_b1(order_book_id) if side == SIDE.BUY else self._env.price_board.get_a1(
+            order_book_id)
+        if price == 0:
+            price = self._env.price_board.get_last_price(order_book_id)
+        return price
+
+    def _on_before_trading(self, event):
+        # 在每个交易日的盘前删除前一个交易日的数据
+        self._last_tick.clear()
+        self._cur_tick.clear()
+
+    def _get_today_history_ticks(self, order_book_id, count):
+        """ 获取当前交易日的历史tick数据 """
+        cal_dt = self._env.calendar_dt
+        tick_list = self._env.data_proxy.history_ticks(order_book_id, count, cal_dt)
+        start = cal_dt if cal_dt.hour >= 19 else cal_dt - datetime.timedelta(days=1)
+        start = start.replace(hour=17, minute=0, second=0, microsecond=0)
+        ticks = [tick for tick in tick_list if start <= tick.datetime <= cal_dt]
+        return ticks
+
+    def _get_last_tick(self, order_book_id):
+        """ 获取上一个tick """
+        _last_tick = self._last_tick.get(order_book_id)
+        trading_dt = self._env.trading_dt
+        # 上一根tick缺失
+        if not _last_tick:
+            tick_list = self._get_today_history_ticks(order_book_id, 2)
+            _last_tick = tick_list[0] if len(tick_list) == 2 else None
+        else:
+            # 两个tick之间的时间差(秒)
+            diff_time = trading_dt.timestamp() - _last_tick.datetime.timestamp()
+            # 在非回测状态下，时差间隔太大时，需要重新获取tick
+            if diff_time > 5:
+                tick_list = self._get_today_history_ticks(order_book_id, 2)
+                _last_tick = tick_list[0] if len(tick_list) == 2 else None
+        return _last_tick
+
+    def match(self, account, order, open_auction):  # type: (Account, Order, bool) -> None
+
+        # order 是否合法
+        if not (order.position_effect in self.SUPPORT_POSITION_EFFECTS and order.side in self.SUPPORT_SIDES):
+            raise NotImplementedError
+
+        # 标的信息
+        order_book_id = order.order_book_id
+        instrument = self._env.get_instrument(order_book_id)
+
+        # 获取tick数据
+        _cur_tick = self._cur_tick.get(order_book_id)
+
+        # 判断订单在交易时间下处于那个阶段
+        if instrument.during_call_auction(self._env.calendar_dt):
+            # 集合竞价时段内撮合无视 matching_type 的设置，直接使用 last 进行撮合
+            deal_price = _cur_tick.last
+            # 集合竞价默认开启成交量限制，用来保证在集合竞价中只有一笔成交
+            _volume_limit_flag = True
+        else:
+            deal_price = self._deal_price_decider(order_book_id, order.side)
+            _volume_limit_flag = self._volume_limit
+
+        # 确认价格是否有效
+        if not is_valid_price(deal_price):
+            listed_date = instrument.listed_date.date()
+            if listed_date == self._env.trading_dt.date():
+                reason = _(
+                    u"Order Cancelled: current security [{order_book_id}] can not be traded"
+                    u" in listed date [{listed_date}]").format(
+                    order_book_id=order.order_book_id,
+                    listed_date=listed_date,
+                )
+            else:
+                # TODO：这里报错信息比较模糊，可以根据撮合类型给出更明确的提示，比如是否是熔断了，是否是涨跌停了
+                reason = _(u"Order Cancelled: current tick [{order_book_id}] miss market data.").format(
+                    order_book_id=order.order_book_id)
+            order.mark_rejected(reason)
+            return
+
+        price_board = self._env.price_board
+        if order.type == ORDER_TYPE.LIMIT:
+            if order.side == SIDE.BUY and order.price < deal_price:
+                return
+            if order.side == SIDE.SELL and order.price > deal_price:
+                return
+            # 是否限制涨跌停不成交
+            if self._price_limit:
+                if order.side == SIDE.BUY and deal_price >= price_board.get_limit_up(order_book_id):
+                    return
+                if order.side == SIDE.SELL and deal_price <= price_board.get_limit_down(order_book_id):
+                    return
+            if self._liquidity_limit:
+                if order.side == SIDE.BUY and price_board.get_a1(order_book_id) == 0:
+                    return
+                if order.side == SIDE.SELL and price_board.get_b1(order_book_id) == 0:
+                    return
+        else:
+            if self._price_limit:
+                if order.side == SIDE.BUY and deal_price >= price_board.get_limit_up(order_book_id):
+                    reason = _(
+                        "Order Cancelled: current tick [{order_book_id}] reach the limit_up price."
+                    ).format(order_book_id=order.order_book_id)
+                    order.mark_rejected(reason)
+                    return
+                if order.side == SIDE.SELL and deal_price <= price_board.get_limit_down(order_book_id):
+                    reason = _(
+                        "Order Cancelled: current tick [{order_book_id}] reach the limit_down price."
+                    ).format(order_book_id=order.order_book_id)
+                    order.mark_rejected(reason)
+                    return
+            if self._liquidity_limit:
+                if order.side == SIDE.BUY and price_board.get_a1(order_book_id) == 0:
+                    reason = _(
+                        "Order Cancelled: [{order_book_id}] has no liquidity."
+                    ).format(order_book_id=order.order_book_id)
+                    order.mark_rejected(reason)
+                    return
+                if order.side == SIDE.SELL and price_board.get_b1(order_book_id) == 0:
+                    reason = _(
+                        "Order Cancelled: [{order_book_id}] has no liquidity."
+                    ).format(order_book_id=order.order_book_id)
+                    order.mark_rejected(reason)
+                    return
+
+        # 是否开启成交量限制
+        if _volume_limit_flag:
+            # 获取上一个tick
+            _last_tick = self._get_last_tick(order_book_id)
+
+            if _last_tick:
+                # 当前的时刻的成交量 = 当前tick - 上一个时刻的tick
+                volume = _cur_tick.volume - _last_tick.volume
+            else:
+                # 当天第一个tick
+                volume = _cur_tick.volume
+
+            if self._volume_limit:
+                volume_limit = round(volume * self._volume_percent) - self._turnover[order.order_book_id]
+            else:
+                # 主要是处理未开启时集合竞价的成交情况，只要有成交量就表示能撮合
+                volume_limit = volume
+
+            # 对成交量根据 1手 : n股 的比例进行限制
+            volume_limit = (volume_limit // instrument.round_lot) * instrument.round_lot
+
+            if volume_limit <= 0:
+                # 集合竞价无法撤单
+                if order.type == ORDER_TYPE.MARKET:
+                    reason = _(u"Order Cancelled: market order {order_book_id} volume {order_volume}"
+                               u" due to volume limit").format(
+                        order_book_id=order.order_book_id,
+                        order_volume=order.quantity
+                    )
+                    order.mark_cancelled(reason)
+                return
+
+            # 实际成交数量
+            if self._volume_limit:
+                fill = min(order.unfilled_quantity, volume_limit)
+            else:
+                fill = order.unfilled_quantity
+        else:
+            # 下单数量就是成交数量
+            fill = order.unfilled_quantity
+
+        # 平今的数量
+        ct_amount = account.calc_close_today_amount(order_book_id, fill, order.position_direction)
+
+        # 对价格进行滑点处理
+        if instrument.during_call_auction(self._env.calendar_dt):
+            price = deal_price
+        else:
+            price = self._slippage_decider.get_trade_price(order, deal_price)
+
+        # 成交记录
+        trade = Trade.__from_create__(
+            order_id=order.order_id,
+            price=price,
+            amount=fill,
+            side=order.side,
+            position_effect=order.position_effect,
+            order_book_id=order.order_book_id,
+            frozen_price=order.frozen_price,
+            close_today_amount=ct_amount
+        )
+        trade._commission = self._env.get_trade_commission(trade)
+        trade._tax = self._env.get_trade_tax(trade)
+        order.fill(trade)
+        self._turnover[order.order_book_id] += fill
+
+        self._env.event_bus.publish_event(Event(EVENT.TRADE, account=account, trade=trade, order=order))
+
+        if order.type == ORDER_TYPE.MARKET and order.unfilled_quantity != 0:
+            reason = _(
+                u"Order Cancelled: market order {order_book_id} volume {order_volume} is"
+                u" larger than {volume_percent_limit} percent of current tick volume, fill {filled_volume} actually"
+            ).format(
+                order_book_id=order.order_book_id,
+                order_volume=order.quantity,
+                filled_volume=order.filled_quantity,
+                volume_percent_limit=self._volume_percent * 100.0
+            )
+            order.mark_cancelled(reason)
+
+    def update(self, event):
+        self._last_tick[event.tick.order_book_id] = self._cur_tick.get(event.tick.order_book_id)
+        self._cur_tick[event.tick.order_book_id] = event.tick
+        self._turnover.clear()
+
+
+class CounterPartyOfferMatcher(DefaultTickMatcher):
     def __init__(self, env, mod_config):
         super(CounterPartyOfferMatcher, self).__init__(env, mod_config)
         self._env = env
         self._a_volume = {}
         self._b_volume = {}
         self._a_price = {}
         self._b_price = {}
-        self._env.event_bus.add_listener(EVENT.TICK, self._pre_tick)
+        self._env.event_bus.prepend_listener(EVENT.TICK, self._pre_tick)
 
     def match(self, account, order, open_auction):
         # type: (Account, Order, bool) -> None
         #
         """限价撮合：
         订单买价>卖x价
         买量>卖x量，按照卖x价成交，订单减去卖x量，继续撮合卖x+1，直至该tick中所有报价被买完。买完后若有剩余买量，则在下一个tick继续撮合。
         买量<卖x量，按照卖x价成交。
         反之亦然
         市价单：
         按照该tick，a1，b1进行成交，剩余订单直接撤单
         """
         order_book_id = order.order_book_id
+        instrument = self._env.get_instrument(order_book_id)
 
         self._pop_volume_and_price(order)
         if order.side == SIDE.BUY:
             if len(self._a_volume[order_book_id]) == 0:
                 return
             volume_limit = self._a_volume[order_book_id][0]
             matching_price = self._a_price[order_book_id][0]
@@ -283,46 +515,98 @@
             if volume_limit != volume_limit:
                 return
             amount = volume_limit
             if amount == 0.0 and order.unfilled_quantity != 0:
                 # if order.unfilled_quantity != 0:
                 return self.match(account, order, open_auction)
 
+        if instrument.during_call_auction(self._env.trading_dt):
+            # 集合竞价期间一律使用last
+            matching_price = self._cur_tick[order_book_id].last
+            _volume_limit_flag = True
+        else:
+            _volume_limit_flag = self._volume_limit
+
         if matching_price != matching_price:
             return
 
         if not (order.position_effect in self.SUPPORT_POSITION_EFFECTS and order.side in self.SUPPORT_SIDES):
             raise NotImplementedError
         if order.type == ORDER_TYPE.LIMIT:
             if order.side == SIDE.BUY and order.price < matching_price:
                 return
             if order.side == SIDE.SELL and order.price > matching_price:
                 return
-        fill = order.unfilled_quantity
+
+        # 成交量限制
+        if _volume_limit_flag:
+            # 获取tick
+            _last_tick = self._get_last_tick(order_book_id)
+            _cur_tick = self._cur_tick[order_book_id]
+
+            if _last_tick:
+                # 当前的时刻的成交量 = 当前tick - 上一个时刻的tick
+                volume = _cur_tick.volume - _last_tick.volume
+            else:
+                # 当天第一个tick
+                volume = _cur_tick.volume
+
+            if self._volume_limit:
+                volume_limit = round(volume * self._volume_percent) - self._turnover[order.order_book_id]
+            else:
+                volume_limit = volume
+
+            # 对成交量根据 1手 : n股 的比例进行限制
+            volume_limit = (volume_limit // instrument.round_lot) * instrument.round_lot
+
+            if volume_limit <= 0:
+                # 集合竞价无法撤单
+                if order.type == ORDER_TYPE.MARKET:
+                    reason = _(u"Order Cancelled: market order {order_book_id} volume {order_volume}"
+                               u" due to volume limit").format(
+                        order_book_id=order.order_book_id,
+                        order_volume=order.quantity
+                    )
+                    order.mark_cancelled(reason)
+                return
+
+            if self._volume_limit:
+                if instrument.during_call_auction(self._env.trading_dt):
+                    fill = min(order.unfilled_quantity, volume_limit)
+                else:
+                    fill = min(order.unfilled_quantity, amount, volume_limit)
+            else:
+                fill = min(order.unfilled_quantity, amount)
+        else:
+            fill = min(order.unfilled_quantity, amount)
+
         ct_amount = account.calc_close_today_amount(order_book_id, fill, order.position_direction)
 
         trade = Trade.__from_create__(
             order_id=order.order_id,
             price=matching_price,
-            amount=min(amount, fill),
+            amount=fill,
             side=order.side,
             position_effect=order.position_effect,
             order_book_id=order.order_book_id,
             frozen_price=order.frozen_price,
             close_today_amount=ct_amount
         )
         trade._commission = self._env.get_trade_commission(trade)
         trade._tax = self._env.get_trade_tax(trade)
         order.fill(trade)
+        self._turnover[order.order_book_id] += fill
         self._env.event_bus.publish_event(Event(EVENT.TRADE, account=account, trade=trade, order=order))
 
-        if order.side == SIDE.BUY:
-            self._a_volume[order.order_book_id][0] -= min(amount, fill)
-        else:
-            self._b_volume[order.order_book_id][0] -= min(amount, fill)
+        if not instrument.during_call_auction(self._env.trading_dt):
+            # 常规交易时间逐档
+            if order.side == SIDE.BUY:
+                self._a_volume[order.order_book_id][0] -= fill
+            else:
+                self._b_volume[order.order_book_id][0] -= fill
 
         if order.type == ORDER_TYPE.MARKET and order.unfilled_quantity != 0:
             reason = _("Order Cancelled: market order {order_book_id} fill {filled_volume} actually").format(
                 order_book_id=order.order_book_id,
                 filled_volume=order.filled_quantity,
             )
             order.mark_cancelled(reason)
@@ -346,10 +630,7 @@
     def _pre_tick(self, event):
         order_book_id = event.tick.order_book_id
         self._a_volume[order_book_id] = event.tick.ask_vols
         self._b_volume[order_book_id] = event.tick.bid_vols
 
         self._a_price[order_book_id] = event.tick.asks
         self._b_price[order_book_id] = event.tick.bids
-
-    def update(self):
-        pass
```

### Comparing `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_simulation/mod.py` & `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_simulation/mod.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,21 +32,20 @@
         self._env = None
 
     def start_up(self, env, mod_config):
         self._env = env
         if env.config.base.run_type == RUN_TYPE.LIVE_TRADING:
             return
 
-        mod_config.matching_type = self.parse_matching_type(mod_config.matching_type)
+        mod_config.matching_type = self.parse_matching_type(mod_config.matching_type, env.config.base.frequency)
 
         if env.config.base.margin_multiplier <= 0:
             raise patch_user_exc(ValueError(_(u"invalid margin multiplier value: value range is (0, +∞]")))
 
         if env.config.base.frequency == "tick":
-            mod_config.volume_limit = False
             if mod_config.matching_type not in [
                 MATCHING_TYPE.NEXT_TICK_LAST,
                 MATCHING_TYPE.NEXT_TICK_BEST_OWN,
                 MATCHING_TYPE.NEXT_TICK_BEST_COUNTERPARTY,
                 MATCHING_TYPE.COUNTERPARTY_OFFER,
             ]:
                 raise RuntimeError(_("Not supported matching type {}").format(mod_config.matching_type))
@@ -70,19 +69,31 @@
 
         if mod_config.management_fee:
             env.event_bus.add_listener(EVENT.POST_SYSTEM_INIT, self.register_management_fee_calculator)
 
         event_source = SimulationEventSource(env)
         env.set_event_source(event_source)
 
+        from .validator import OrderStyleValidator
+        env.add_frontend_validator(OrderStyleValidator(env.config.base.frequency))
+
     def tear_down(self, code, exception=None):
         pass
 
     @staticmethod
-    def parse_matching_type(me_str):
+    def parse_matching_type(me_str, frequency):
+        if me_str is None:
+            # None 表示根据 frequency 自动选择
+            if frequency in ["1d", "1m"]:
+                me_str = "current_bar"
+            elif frequency == "tick":
+                me_str = "last"
+            else:
+                raise ValueError("frequency only support ['1d', '1m', 'tick']")
+
         assert isinstance(me_str, six.string_types)
         me_str = me_str.lower()
         if me_str == "current_bar":
             return MATCHING_TYPE.CURRENT_BAR_CLOSE
         if me_str == "vwap":
             return MATCHING_TYPE.VWAP
         elif me_str == "next_bar":
```

### Comparing `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_simulation/signal_broker.py` & `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_simulation/signal_broker.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,20 +14,23 @@
 #         否则米筐科技有权追究相应的知识产权侵权责任。
 #         在此前提下，对本软件的使用同样需要遵守 Apache 2.0 许可，Apache 2.0 许可与本许可冲突之处，以本许可为准。
 #         详细的授权流程，请联系 public@ricequant.com 获取。
 
 
 from copy import copy
 
+import numpy as np
+
 from rqalpha.interface import AbstractBroker
 from rqalpha.utils.logger import user_system_log
 from rqalpha.utils.i18n import gettext as _
 from rqalpha.utils import is_valid_price
 from rqalpha.core.events import EVENT, Event
 from rqalpha.model.trade import Trade
+from rqalpha.model.order import ALGO_ORDER_STYLES
 from rqalpha.const import SIDE, ORDER_TYPE, POSITION_EFFECT
 
 from .slippage import SlippageDecider
 
 
 class SignalBroker(AbstractBroker):
     def __init__(self, env, mod_config):
@@ -73,14 +76,20 @@
                     order_book_id=order_book_id)
             order.mark_rejected(reason)
             self._env.event_bus.publish_event(Event(EVENT.ORDER_UNSOLICITED_UPDATE, account=account, order=copy(order)))
             return
 
         if order.type == ORDER_TYPE.LIMIT:
             deal_price = order.frozen_price
+        elif isinstance(order.style, ALGO_ORDER_STYLES):
+            deal_price, v = self._env.data_proxy.get_algo_bar(order.order_book_id, order.style, self._env.calendar_dt)
+            if np.isnan(deal_price):
+                reason = _(u"Order Cancelled: {order_book_id} bar no volume").format(order_book_id=order.order_book_id)
+                order.mark_rejected(reason)
+                return
         else:
             deal_price = last_price
 
         if self._price_limit:
             if order.position_effect != POSITION_EFFECT.EXERCISE:
                 if order.side == SIDE.BUY and deal_price >= price_board.get_limit_up(order_book_id):
                     order.mark_rejected(_(
```

### Comparing `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_broker.py` & `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_broker.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from rqalpha.interface import AbstractBroker, Persistable
 from rqalpha.utils.i18n import gettext as _
 from rqalpha.core.events import EVENT, Event
 from rqalpha.const import MATCHING_TYPE, ORDER_STATUS, POSITION_EFFECT, EXECUTION_PHASE, INSTRUMENT_TYPE
 from rqalpha.model.order import Order
 from rqalpha.environment import Environment
 
-from .matcher import DefaultMatcher, AbstractMatcher, CounterPartyOfferMatcher
+from .matcher import DefaultBarMatcher, AbstractMatcher, CounterPartyOfferMatcher, DefaultTickMatcher
 
 
 class SimulationBroker(AbstractBroker, Persistable):
     def __init__(self, env, mod_config):
         self._env = env  # type: Environment
         self._mod_config = mod_config
 
@@ -47,14 +47,15 @@
         self._open_exercise_orders = []  # type: List[Tuple[Account, Order]]
 
         self._frontend_validator = {}
 
         if self._mod_config.matching_type == MATCHING_TYPE.COUNTERPARTY_OFFER:
             for instrument_type in INSTRUMENT_TYPE:
                 self.register_matcher(instrument_type, CounterPartyOfferMatcher(self._env, self._mod_config))
+
         # 该事件会触发策略的before_trading函数
         self._env.event_bus.add_listener(EVENT.BEFORE_TRADING, self.before_trading)
         # 该事件会触发策略的handle_bar函数
         self._env.event_bus.add_listener(EVENT.BAR, self.on_bar)
         # 该事件会触发策略的handel_tick函数
         self._env.event_bus.add_listener(EVENT.TICK, self.on_tick)
         # 该事件会触发策略的after_trading函数
@@ -64,15 +65,18 @@
     @lru_cache(1024)
     def _get_matcher(self, order_book_id):
         # type: (str) -> AbstractMatcher
         instrument_type = self._env.data_proxy.instrument(order_book_id).type
         try:
             return self._matchers[instrument_type]
         except KeyError:
-            return self._matchers.setdefault(instrument_type, DefaultMatcher(self._env, self._mod_config))
+            if self._env.config.base.frequency == "tick":
+                return self._matchers.setdefault(instrument_type, DefaultTickMatcher(self._env, self._mod_config))
+            else:
+                return self._matchers.setdefault(instrument_type, DefaultBarMatcher(self._env, self._mod_config))
 
     def register_matcher(self, instrument_type, matcher):
         # type: (INSTRUMENT_TYPE, AbstractMatcher) -> None
         self._matchers[instrument_type] = matcher
 
     def get_open_orders(self, order_book_id=None):
         if order_book_id is None:
@@ -147,26 +151,26 @@
     def pre_settlement(self, __):
         for account, order in self._open_exercise_orders:
             self._get_matcher(order.order_book_id).match(account, order, False)
             if order.status == ORDER_STATUS.REJECTED or order.status == ORDER_STATUS.CANCELLED:
                 self._env.event_bus.publish_event(Event(EVENT.ORDER_UNSOLICITED_UPDATE, account=account, order=order))
         self._open_exercise_orders.clear()
 
-    def on_bar(self, _):
+    def on_bar(self, event):
         for matcher in self._matchers.values():
-            matcher.update()
+            matcher.update(event)
         self._match()
 
     def on_tick(self, event):
         tick = event.tick
-        self._get_matcher(tick.order_book_id).update()
+        self._get_matcher(tick.order_book_id).update(event)
         self._match(tick.order_book_id)
 
     def _match(self, order_book_id=None):
-        order_filter = None if order_book_id is None else lambda a_and_o: a_and_o[1].order_book_id == order_book_id
+        order_filter = lambda a_and_o: not (a_and_o[1].is_final() or (order_book_id and a_and_o[1].order_book_id != order_book_id))
         for account, order in filter(order_filter, self._open_orders):
             self._get_matcher(order.order_book_id).match(account, order, open_auction=False)
         for account, order in filter(order_filter, self._open_auction_orders):
             self._get_matcher(order.order_book_id).match(account, order, open_auction=True)
         final_orders = [(a, o) for a, o in chain(self._open_orders, self._open_auction_orders) if o.is_final()]
         self._open_orders = [(a, o) for a, o in chain(self._open_orders, self._open_auction_orders) if not o.is_final()]
         self._open_auction_orders.clear()
```

### Comparing `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_event_source.py` & `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_event_source.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from datetime import timedelta, datetime, time
 
 from rqalpha.environment import Environment
 from rqalpha.interface import AbstractEventSource
 from rqalpha.core.events import Event, EVENT
 from rqalpha.utils.exception import patch_user_exc
 from rqalpha.utils.datetime_func import convert_int_to_datetime
-from rqalpha.const import DEFAULT_ACCOUNT_TYPE
+from rqalpha.const import DEFAULT_ACCOUNT_TYPE, INSTRUMENT_TYPE
 from rqalpha.utils.i18n import gettext as _
 
 
 class SimulationEventSource(AbstractEventSource):
     def __init__(self, env):
         # type: (Environment) -> None
         self._env = env
@@ -165,24 +165,30 @@
                             trading_dt = calendar_dt.replace(year=date.year, month=date.month, day=date.day)
                         else:
                             trading_dt = calendar_dt
 
                         if last_tick is None:
                             last_tick = tick
 
-                            yield Event(
-                                EVENT.BEFORE_TRADING,
-                                calendar_dt=calendar_dt - timedelta(minutes=30),
-                                trading_dt=trading_dt - timedelta(minutes=30)
-                            )
-                            yield Event(
-                                EVENT.OPEN_AUCTION,
-                                calendar_dt=calendar_dt - timedelta(minutes=3),
-                                trading_dt=trading_dt - timedelta(minutes=3),
-                            )
+                            """
+                            这里区分时间主要是为了对其之前，之前对获取tick数据的时间有限制，期货的盘前时间是20:30，股票是09:00。
+                            在解除获取tick数据的限制后，股票的tick的开始时间是09:15，而期货则是20:59
+                            """
+                            if self._env.get_instrument(tick.order_book_id).type == INSTRUMENT_TYPE.FUTURE:
+                                yield Event(
+                                    EVENT.BEFORE_TRADING,
+                                    calendar_dt=calendar_dt - timedelta(minutes=30),
+                                    trading_dt=trading_dt - timedelta(minutes=30),
+                                )
+                            else:
+                                yield Event(
+                                    EVENT.BEFORE_TRADING,
+                                    calendar_dt=calendar_dt - timedelta(minutes=15),
+                                    trading_dt=trading_dt - timedelta(minutes=15),
+                                )
 
                         if self._universe_changed:
                             self._universe_changed = False
                             break
 
                         last_dt = calendar_dt
                         yield Event(EVENT.TICK, calendar_dt=calendar_dt, trading_dt=trading_dt, tick=tick)
```

### Comparing `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_simulation/slippage.py` & `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_simulation/slippage.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_simulation/testing.py` & `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_simulation/testing.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_transaction_cost/__init__.py` & `rqalpha-5.0.0/tests/api_tests/mod/sys_transaction_cost/test_commission_multiplier.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,60 +8,48 @@
 #         除非法律有要求或以书面形式达成协议，否则本软件分发时需保持当前许可“原样”不变，且不得附加任何条件。
 #
 #     * 商业用途（商业用途指个人出于任何商业目的使用本软件，或者法人或其他组织出于任何目的使用本软件）：
 #         未经米筐科技授权，任何个人不得出于任何商业目的使用本软件（包括但不限于向第三方提供、销售、出租、出借、转让本软件、本软件的衍生产品、引用或借鉴了本软件功能或源代码的产品或服务），任何法人或其他组织不得出于任何目的使用本软件，否则米筐科技有权追究相应的知识产权侵权责任。
 #         在此前提下，对本软件的使用同样需要遵守 Apache 2.0 许可，Apache 2.0 许可与本许可冲突之处，以本许可为准。
 #         详细的授权流程，请联系 public@ricequant.com 获取。
 
-import click
-from rqalpha import cli
+from rqalpha.apis import *
+from rqalpha.environment import Environment
 
 __config__ = {
-    # 股票最小手续费，单位元
-    "cn_stock_min_commission": 5,
-    # 佣金倍率，即在默认的手续费率基础上按该倍数进行调整，股票的默认佣金为万八，期货默认佣金因合约而异
-    "commission_multiplier": 1,
-    # 印花倍率，即在默认的印花税基础上按该倍数进行调整，股票默认印花税为千分之一，单边收取
-    "tax_multiplier": 1,
+    "base": {
+        "start_date": "2022-01-01",
+        "end_date": "2022-01-30",
+        "frequency": "1d",
+        "accounts": {
+            "stock": 1000000,
+            "future": 1000000,
+        }
+    },
+    "mod": {
+        "sys_transaction_cost": {
+            "stock_commission_multiplier": 2,
+            "futures_commission_multiplier": 3,
+        }
+    }
 }
 
-cli_prefix = "mod__sys_transaction_cost__"
 
+def test_commission_multiplier():
+
+    def init(context):
+        context.s1 = "000001.XSHE"
+        context.s2 = "IC2203"
+        context.fixed = True
+
+    def handle_bar(context, bar_dict):
+        if context.fixed:
+            stock_order = order_percent(context.s1, 1)
+            future_order = buy_open(context.s2, 1)
+            env = Environment.get_instance()
+            future_commission_info = env.data_proxy.get_commission_info(context.s2)
+            context.fixed = False
+            assert stock_order.transaction_cost == 16.66 * 59900 * 8 / 10000 * 2
+            assert future_order.transaction_cost == 7308 * 200 * future_commission_info["open_commission_ratio"] * 3
+
+    return locals()
 
-cli.commands['run'].params.append(
-    click.Option(
-        ('-cm', '--commission-multiplier', cli_prefix + "commission_multiplier"),
-        type=click.FLOAT,
-        help="[sys_simulation] set commission multiplier"
-    )
-)
-
-
-cli.commands['run'].params.append(
-    click.Option(
-        ('-cnsmc', '--cn-stock-min-commission', cli_prefix + 'cn_stock_min_commission'),
-        type=click.FLOAT,
-        help="[sys_simulation] set minimum commission in chinese stock trades."
-    )
-)
-
-# [deprecated]
-cli.commands['run'].params.append(
-    click.Option(
-        ('-smc', '--stock-min-commission', cli_prefix + 'cn_stock_min_commission'),
-        type=click.FLOAT,
-        help="[sys_simulation][deprecated] set minimum commission in chinese stock trades."
-    )
-)
-
-cli.commands['run'].params.append(
-    click.Option(
-        ('-tm', '--tax-multiplier', cli_prefix + "tax_multiplier"),
-        type=click.FLOAT,
-        help="[sys_simulation] set tax multiplier"
-    )
-)
-
-
-def load_mod():
-    from .mod import TransactionCostMod
-    return TransactionCostMod()
```

### Comparing `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_transaction_cost/deciders.py` & `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_transaction_cost/deciders.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_transaction_cost/mod.py` & `rqalpha-5.0.0/rqalpha/mod/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,36 +11,46 @@
 #     * 商业用途（商业用途指个人出于任何商业目的使用本软件，或者法人或其他组织出于任何目的使用本软件）：
 #         未经米筐科技授权，任何个人不得出于任何商业目的使用本软件（包括但不限于向第三方提供、销售、出租、出借、转让本软件、
 #         本软件的衍生产品、引用或借鉴了本软件功能或源代码的产品或服务），任何法人或其他组织不得出于任何目的使用本软件，
 #         否则米筐科技有权追究相应的知识产权侵权责任。
 #         在此前提下，对本软件的使用同样需要遵守 Apache 2.0 许可，Apache 2.0 许可与本许可冲突之处，以本许可为准。
 #         详细的授权流程，请联系 public@ricequant.com 获取。
 
-from rqalpha.interface import AbstractMod
-from rqalpha.const import INSTRUMENT_TYPE
-from rqalpha.utils.exception import patch_user_exc
-from rqalpha.utils import INST_TYPE_IN_STOCK_ACCOUNT
-from rqalpha.utils.i18n import gettext as _
-
-from .deciders import CNStockTransactionCostDecider, CNFutureTransactionCostDecider
-
-
-class TransactionCostMod(AbstractMod):
-    def start_up(self, env, mod_config):
-        if mod_config.commission_multiplier < 0 or mod_config.tax_multiplier < 0:
-            raise patch_user_exc(ValueError(_(u"invalid commission multiplier or tax multiplier"
-                                              u" value: value range is [0, +∞)")))
-
-        for instrument_type in INST_TYPE_IN_STOCK_ACCOUNT:
-            if instrument_type == INSTRUMENT_TYPE.PUBLIC_FUND:
-                continue
-            env.set_transaction_cost_decider(instrument_type, CNStockTransactionCostDecider(
-                mod_config.commission_multiplier, mod_config.cn_stock_min_commission,
-                mod_config.tax_multiplier
-            ))
-
-        env.set_transaction_cost_decider(INSTRUMENT_TYPE.FUTURE, CNFutureTransactionCostDecider(
-            mod_config.commission_multiplier
-        ))
-
-    def tear_down(self, code, exception=None):
+def mod_config_value_parse(value):
+    if value in ["True", "true"]:
+        return True
+    if value in ["False", "false"]:
+        return False
+
+    if value.isdigit():
+        return int(value)
+
+    try:
+        return float(value)
+    except ValueError:
         pass
+
+    return value
+
+
+def inject_mod_commands():
+    from rqalpha.utils.config import get_mod_conf
+    from rqalpha.mod import SYSTEM_MOD_LIST
+    from rqalpha.utils.package_helper import import_mod
+    mod_config = get_mod_conf()
+
+    for mod_name, config in mod_config['mod'].items():
+        if 'lib' in config:
+            lib_name = config["lib"]
+        else:
+            lib_name = "rqalpha_mod_{}".format(mod_name)
+        if not config['enabled']:
+            continue
+        try:
+            if mod_name in SYSTEM_MOD_LIST:
+                # inject system mod
+                import_mod("rqalpha.mod." + lib_name)
+            else:
+                # inject third part mod
+                import_mod(lib_name)
+        except Exception as e:
+            pass
```

### Comparing `rqalpha-4.9.2/rqalpha/mod/utils.py` & `rqalpha-5.0.0/rqalpha/utils/strategy_loader_help.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,52 @@
 # -*- coding: utf-8 -*-
 # 版权所有 2019 深圳米筐科技有限公司（下称“米筐科技”）
 #
 # 除非遵守当前许可，否则不得使用本软件。
 #
 #     * 非商业用途（非商业用途指个人出于非商业目的使用本软件，或者高校、研究所等非营利机构出于教育、科研等目的使用本软件）：
-#         遵守 Apache License 2.0（下称“Apache 2.0 许可”），
-#         您可以在以下位置获得 Apache 2.0 许可的副本：http://www.apache.org/licenses/LICENSE-2.0。
+#         遵守 Apache License 2.0（下称“Apache 2.0 许可”），您可以在以下位置获得 Apache 2.0 许可的副本：http://www.apache.org/licenses/LICENSE-2.0。
 #         除非法律有要求或以书面形式达成协议，否则本软件分发时需保持当前许可“原样”不变，且不得附加任何条件。
 #
 #     * 商业用途（商业用途指个人出于任何商业目的使用本软件，或者法人或其他组织出于任何目的使用本软件）：
-#         未经米筐科技授权，任何个人不得出于任何商业目的使用本软件（包括但不限于向第三方提供、销售、出租、出借、转让本软件、
-#         本软件的衍生产品、引用或借鉴了本软件功能或源代码的产品或服务），任何法人或其他组织不得出于任何目的使用本软件，
-#         否则米筐科技有权追究相应的知识产权侵权责任。
+#         未经米筐科技授权，任何个人不得出于任何商业目的使用本软件（包括但不限于向第三方提供、销售、出租、出借、转让本软件、本软件的衍生产品、引用或借鉴了本软件功能或源代码的产品或服务），任何法人或其他组织不得出于任何目的使用本软件，否则米筐科技有权追究相应的知识产权侵权责任。
 #         在此前提下，对本软件的使用同样需要遵守 Apache 2.0 许可，Apache 2.0 许可与本许可冲突之处，以本许可为准。
 #         详细的授权流程，请联系 public@ricequant.com 获取。
 
-def mod_config_value_parse(value):
-    if value in ["True", "true"]:
-        return True
-    if value in ["False", "false"]:
-        return False
+import sys
+import traceback
+import six
 
-    if value.isdigit():
-        return int(value)
+from rqalpha.utils.exception import patch_user_exc, CustomError, CustomException
 
+
+def compile_strategy(source_code, strategy, scope):
     try:
-        return float(value)
-    except ValueError:
-        pass
-
-    return value
-
-
-def inject_mod_commands():
-    from rqalpha.utils.config import get_mod_conf
-    from rqalpha.mod import SYSTEM_MOD_LIST
-    from rqalpha.utils.package_helper import import_mod
-    mod_config = get_mod_conf()
-
-    for mod_name, config in mod_config['mod'].items():
-        if 'lib' in config:
-            lib_name = config["lib"]
-        else:
-            lib_name = "rqalpha_mod_{}".format(mod_name)
-        if not config['enabled']:
-            continue
+        code = compile(source_code, strategy, 'exec')
+        six.exec_(code, scope)
+        return scope
+    except Exception as e:
+        exc_type, exc_val, exc_tb = sys.exc_info()
+        exc_val = patch_user_exc(exc_val, force=True)
         try:
-            if mod_name in SYSTEM_MOD_LIST:
-                # inject system mod
-                import_mod("rqalpha.mod." + lib_name)
-            else:
-                # inject third part mod
-                import_mod(lib_name)
-        except Exception as e:
-            pass
+            msg = str(exc_val)
+        except Exception as e1:
+            msg = ""
+            six.print_(e1)
+
+        error = CustomError()
+        error.set_msg(msg)
+        error.set_exc(exc_type, exc_val, exc_tb)
+        stackinfos = list(traceback.extract_tb(exc_tb))
+
+        if isinstance(e, (SyntaxError, IndentationError)):
+            error.add_stack_info(exc_val.filename, exc_val.lineno, "", exc_val.text)
+        else:
+            for item in stackinfos:
+                filename, lineno, func_name, code = item
+                if strategy == filename:
+                    error.add_stack_info(*item)
+            # avoid empty stack
+            if error.stacks_length == 0:
+                error.add_stack_info(*item)
+
+        raise CustomException(error)
```

### Comparing `rqalpha-4.9.2/rqalpha/model/__init__.py` & `rqalpha-5.0.0/rqalpha/model/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/model/bar.py` & `rqalpha-5.0.0/rqalpha/model/bar.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/model/instrument.py` & `rqalpha-5.0.0/rqalpha/model/instrument.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,48 +11,52 @@
 #     * 商业用途（商业用途指个人出于任何商业目的使用本软件，或者法人或其他组织出于任何目的使用本软件）：
 #         未经米筐科技授权，任何个人不得出于任何商业目的使用本软件（包括但不限于向第三方提供、销售、出租、出借、转让本软件、
 #         本软件的衍生产品、引用或借鉴了本软件功能或源代码的产品或服务），任何法人或其他组织不得出于任何目的使用本软件，
 #         否则米筐科技有权追究相应的知识产权侵权责任。
 #         在此前提下，对本软件的使用同样需要遵守 Apache 2.0 许可，Apache 2.0 许可与本许可冲突之处，以本许可为准。
 #         详细的授权流程，请联系 public@ricequant.com 获取。
 
+import re
 import copy
 import datetime
 from typing import Dict, Callable, Optional
 
 import numpy as np
+from dateutil.parser import parse
 
 from rqalpha.environment import Environment
 from rqalpha.const import INSTRUMENT_TYPE, POSITION_DIRECTION, DEFAULT_ACCOUNT_TYPE, EXCHANGE
 from rqalpha.utils import TimeRange, INST_TYPE_IN_STOCK_ACCOUNT
 from rqalpha.utils.repr import property_repr, PropertyReprMeta
 
 
 class Instrument(metaclass=PropertyReprMeta):
-    DEFAULT_LISTED_DATE = datetime.datetime(1990, 1, 1)
     DEFAULT_DE_LISTED_DATE = datetime.datetime(2999, 12, 31)
 
     @staticmethod
-    def _fix_date(ds, dflt):
+    def _fix_date(ds, dflt=None) -> datetime:
         if isinstance(ds, datetime.datetime):
             return ds
-        if ds == '0000-00-00':
+        if ds == '0000-00-00' or ds is None:
             return dflt
-        year, month, day = ds.split('-')
-        return datetime.datetime(int(year), int(month), int(day))
+        try:
+            year, month, day = ds.split('-')
+            return datetime.datetime(int(year), int(month), int(day))
+        except:
+            return parse(ds)
 
     __repr__ = property_repr
 
     def __init__(self, dic, future_tick_size_getter=None):
         # type: (Dict, Optional[Callable[[Instrument], float]]) -> None
         self.__dict__ = copy.copy(dic)
         self._future_tick_size_getter = future_tick_size_getter
 
         if "listed_date" in dic:
-            self.__dict__["listed_date"] = self._fix_date(dic["listed_date"], self.DEFAULT_LISTED_DATE)
+            self.__dict__["listed_date"] = self._fix_date(dic["listed_date"])
         if "de_listed_date" in dic:
             self.__dict__["de_listed_date"] = self._fix_date(dic["de_listed_date"], self.DEFAULT_DE_LISTED_DATE)
         if "maturity_date" in self.__dict__:
             self.__dict__["maturity_date"] = self._fix_date(dic["maturity_date"], self.DEFAULT_DE_LISTED_DATE)
 
         if 'contract_multiplier' in dic:
             if np.isnan(self.contract_multiplier):
@@ -82,16 +86,15 @@
         [int] 股票：一手对应多少股，中国A股一手是100股。期货：一律为1。
         """
         if self.__dict__.get("type") == INSTRUMENT_TYPE.CS and self.__dict__["board_type"] == "KSH":
             return 1
         return int(self.__dict__["round_lot"])
 
     @property
-    def listed_date(self):
-        # type: () -> datetime.datetime
+    def listed_date(self) -> Optional[datetime.datetime]:
         """
         [datetime] 股票：该证券上市日期。期货：期货的上市日期，主力连续合约与指数连续合约都为 datetime(1990, 1, 1)。
         """
         return self.__dict__["listed_date"]
 
     @property
     def de_listed_date(self):
@@ -325,19 +328,19 @@
         :param dt: datetime.datetime
         :return: bool
         """
         return self.listed_at(dt) and not self.de_listed_at(dt)
 
     def listed_at(self, dt):
         """
-        该合约在指定日期是否已上日
+        该合约在指定日期是否已上市
         :param dt: datetime.datetime
         :return: bool
         """
-        return self.listed_date <= dt
+        return self.listed_date and self.listed_date <= dt
 
     def de_listed_at(self, dt):
         """
         该合约在指定日期是否已退市
         :param dt: datetime.datetime
         :return: bool
         """
@@ -382,27 +385,48 @@
                 "Instrument(order_book_id={}) has no attribute 'trading_code' ".format(self.order_book_id)
             )
 
     @property
     def trade_at_night(self):
         return any(r.start <= datetime.time(4, 0) or r.end >= datetime.time(19, 0) for r in (self.trading_hours or []))
 
+    def during_call_auction(self, dt):
+        """ 是否处于集合竞价交易时段 """
+        # 当前的分钟数
+        _minute = dt.hour * 60 + dt.minute
+
+        if self.type in [INSTRUMENT_TYPE.CS, INSTRUMENT_TYPE.ETF]:
+            # 9:30 前或 14:57 之后为集合竞价
+            return _minute < 9 * 60 + 30 or _minute >= 14 * 60 + 57
+        elif self.type == INSTRUMENT_TYPE.FUTURE:
+            # 期货开盘时间
+            start_time = self.trading_hours[0].start
+
+            # -1 是因为获取到的时间都是开盘后1分钟，如 09:31
+            start_minute = start_time.hour * 60 + start_time.minute - 1
+
+            # 开盘集合竞价时间段为开盘前5分钟，期货无收盘集合竞价
+            return start_minute - 5 <= _minute < start_minute
+        else:
+            # 其他品种由子类实现
+            return False
+
     def days_from_listed(self):
-        if self.listed_date == self.DEFAULT_LISTED_DATE:
+        if not self.listed_date:
             return -1
 
         date = Environment.get_instance().trading_dt.date()
         if self.de_listed_date.date() < date:
             return -1
 
         ipo_days = (date - self.listed_date.date()).days
         return ipo_days if ipo_days >= 0 else -1
 
     def days_to_expire(self):
-        if self.type != 'Future' or self.order_book_id[-2:] == '88' or self.order_book_id[-2:] == '99':
+        if self.type != 'Future' or self.is_future_continuous_contract(self.order_book_id):
             return -1
 
         date = Environment.get_instance().trading_dt.date()
         days = (self.maturity_date.date() - date).days
         return -1 if days < 0 else days
 
     def tick_size(self):
@@ -422,14 +446,20 @@
             return price * quantity
         elif self.type == INSTRUMENT_TYPE.FUTURE:
             margin_multiplier = Environment.get_instance().config.base.margin_multiplier
             return price * quantity * self.contract_multiplier * self.margin_rate * margin_multiplier
         else:
             raise NotImplementedError
 
+    FUTURE_CONTINUOUS_CONTRACT = re.compile(r"^[A-Z]+(88|888|99|889)([A-Z]\d+)?$")
+
+    @classmethod
+    def is_future_continuous_contract(cls, order_book_id):
+        return re.match(cls.FUTURE_CONTINUOUS_CONTRACT, order_book_id)
+
 
 class SectorCodeItem(object):
     def __init__(self, cn, en, name):
         self.__cn = cn
         self.__en = en
         self.__name = name
```

### Comparing `rqalpha-4.9.2/rqalpha/model/order.py` & `rqalpha-5.0.0/rqalpha/model/order.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #         详细的授权流程，请联系 public@ricequant.com 获取。
 
 import time
 from decimal import Decimal
 
 import numpy as np
 
-from rqalpha.const import ORDER_STATUS, ORDER_TYPE, SIDE, POSITION_EFFECT, POSITION_DIRECTION
+from rqalpha.const import ORDER_STATUS, ORDER_TYPE, SIDE, POSITION_EFFECT, POSITION_DIRECTION, ALGO
 from rqalpha.utils import id_gen, decimal_rounding_floor, get_position_direction
 from rqalpha.utils.repr import property_repr, properties
 from rqalpha.utils.logger import user_system_log
 from rqalpha.environment import Environment
 
 
 class Order(object):
@@ -46,14 +46,15 @@
         self._filled_quantity = None
         self._status = None
         self._frozen_price = None
         self._init_frozen_cash = None
         self._type = None
         self._avg_price = None
         self._transaction_cost = None
+        self._style = None
         self._kwargs = {}
 
     @staticmethod
     def _str_to_enum(enum_class, s):
         return enum_class.__members__[s]
 
     def get_state(self):
@@ -105,22 +106,27 @@
         order._quantity = quantity
         order._order_book_id = order_book_id
         order._side = side
         order._position_effect = position_effect
         order._message = ""
         order._filled_quantity = 0
         order._status = ORDER_STATUS.PENDING_NEW
+        order._style = style
         if isinstance(style, LimitOrder):
             if env.config.base.round_price:
                 tick_size = env.data_proxy.get_tick_size(order_book_id)
                 style.round_price(tick_size)
             order._frozen_price = style.get_limit_price()
             order._type = ORDER_TYPE.LIMIT
+        elif isinstance(style, ALGO_ORDER_STYLES):
+            algo_price, _ = env.data_proxy.get_algo_bar(order_book_id, style, env.calendar_dt)
+            order._frozen_price = env.get_last_price(order_book_id) if np.isnan(algo_price) else algo_price
+            order._type = ORDER_TYPE.ALGO
         else:
-            order._frozen_price = 0.
+            order._frozen_price = env.get_last_price(order_book_id)
             order._type = ORDER_TYPE.MARKET
         order._avg_price = 0
         order._transaction_cost = 0
         order._kwargs = kwargs
         return order
 
     @property
@@ -234,14 +240,21 @@
     def type(self):
         """
         [ORDER_TYPE] 订单类型
         """
         return self._type
 
     @property
+    def style(self):
+        """
+        [ORDER_STYLE] 订单类型
+        """
+        return self._style
+
+    @property
     def avg_price(self):
         """
         [float] 成交均价
         """
         return self._avg_price
 
     @property
@@ -334,14 +347,35 @@
 
 
 class OrderStyle(object):
     def get_limit_price(self):
         raise NotImplementedError
 
 
+class AlgoOrder(OrderStyle):
+    __repr__ = ORDER_TYPE.ALGO.__repr__
+
+    def __init__(self, start_min, end_min):
+        self.start_min = start_min
+        self.end_min = end_min
+
+    def get_limit_price(self):
+        return None
+
+
+class TWAPOrder(AlgoOrder):
+    TYPE = ALGO.TWAP
+    __repr__ = ALGO.TWAP.__repr__
+
+
+class VWAPOrder(AlgoOrder):
+    TYPE = ALGO.VWAP
+    __repr__ = ALGO.VWAP.__repr__
+
+
 class MarketOrder(OrderStyle):
     __repr__ = ORDER_TYPE.MARKET.__repr__
 
     def get_limit_price(self):
         return None
 
 
@@ -358,7 +392,11 @@
         if tick_size:
             with decimal_rounding_floor():
                 limit_price_decimal = Decimal("{:.4f}".format(self.limit_price))
                 tick_size_decimal = Decimal("{:.4f}".format(tick_size))
                 self.limit_price = float((limit_price_decimal / tick_size_decimal).to_integral() * tick_size_decimal)
         else:
             user_system_log.warn('Invalid tick size: {}'.format(tick_size))
+
+
+ALGO_ORDER_STYLES = (VWAPOrder, TWAPOrder)
+ALL_ORDER_STYPES = (LimitOrder, MarketOrder, TWAPOrder, VWAPOrder)
```

### Comparing `rqalpha-4.9.2/rqalpha/model/tick.py` & `rqalpha-5.0.0/rqalpha/model/tick.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/model/trade.py` & `rqalpha-5.0.0/rqalpha/model/trade.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/portfolio/__init__.py` & `rqalpha-5.0.0/rqalpha/portfolio/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,31 +13,32 @@
 #         本软件的衍生产品、引用或借鉴了本软件功能或源代码的产品或服务），任何法人或其他组织不得出于任何目的使用本软件，
 #         否则米筐科技有权追究相应的知识产权侵权责任。
 #         在此前提下，对本软件的使用同样需要遵守 Apache 2.0 许可，Apache 2.0 许可与本许可冲突之处，以本许可为准。
 #         详细的授权流程，请联系 public@ricequant.com 获取。
 
 from itertools import chain
 from datetime import date
+from collections.abc import Mapping
 from typing import Callable, Dict, List, Tuple, Union
 
 import jsonpickle
 import numpy as np
 import six
 
-from rqalpha.const import DAYS_CNT, DEFAULT_ACCOUNT_TYPE, POSITION_DIRECTION
+from rqalpha.const import DAYS_CNT, DEFAULT_ACCOUNT_TYPE, POSITION_DIRECTION, RUN_TYPE
 from rqalpha.environment import Environment
 from rqalpha.core.events import EVENT, EventBus
 from rqalpha.interface import AbstractPosition
 from rqalpha.model.order import Order, OrderStyle
 from rqalpha.portfolio.account import Account
 from rqalpha.data import DataProxy
-from rqalpha.utils import merge_dicts, is_valid_price
+from rqalpha.utils import is_valid_price
 from rqalpha.utils.functools import lru_cache
 from rqalpha.utils.i18n import gettext as _
-from rqalpha.utils.logger import user_log
+from rqalpha.utils.logger import user_system_log
 from rqalpha.utils.repr import PropertyReprMeta
 
 OrderApiType = Callable[[str, Union[int, float], OrderStyle, bool], List[Order]]
 
 
 class Portfolio(object, metaclass=PropertyReprMeta):
     """
@@ -47,21 +48,24 @@
         "total_value", "unit_net_value", "daily_pnl", "daily_returns", "total_returns", "annualized_returns"
     )
 
     def __init__(
             self,
             starting_cash: Dict[str, float],
             init_positions: List[Tuple[str, int]],
+            financing_rate: float,
             start_date: date,
             data_proxy: DataProxy,
             event_bus: EventBus
     ):
         account_args = {}
         for account_type, cash in starting_cash.items():
-            account_args[account_type] = {"account_type": account_type, "total_cash": cash, "init_positions": {}}
+            account_args[account_type] = {
+                "account_type": account_type, "total_cash": cash, "init_positions": {}, "financing_rate": financing_rate
+            }
         last_trading_date = data_proxy.get_previous_trading_date(start_date)
         for order_book_id, quantity in init_positions:
             account_type = self.get_account_type(order_book_id)
             if account_type in account_args:
                 price = data_proxy.get_bar(order_book_id, last_trading_date).close
                 if not is_valid_price(price):
                     raise ValueError(_("invalid init position {order_book_id}: no valid price at {date}").format(
@@ -252,65 +256,68 @@
     @property
     def frozen_cash(self):
         """
         [float] 冻结资金
         """
         return sum(account.frozen_cash for account in six.itervalues(self._accounts))
 
+    @property
+    def cash_liabilities(self):
+        """
+        [float] 现金负债
+        """
+        return sum(account.cash_liabilities for account in six.itervalues(self._accounts))
+
     def _pre_before_trading(self, _):
         self._static_unit_net_value = self.unit_net_value
 
-    def deposit_withdraw(self, account_type, amount):
+    def deposit_withdraw(self, account_type, amount, receiving_days=0):
         """出入金"""
         # 入金 现金增加，份额增加，总权益增加，单位净值不变
         # 出金 现金减少，份额减少，总权益减少，单位净值不变
         if account_type not in self._accounts:
             raise ValueError(_("invalid account type {}, choose in {}".format(account_type, list(self._accounts.keys()))))
         unit_net_value = self.unit_net_value
-        self._accounts[account_type].deposit_withdraw(amount)
+        self._accounts[account_type].deposit_withdraw(amount, receiving_days)
         _units = self.total_value / unit_net_value
-        user_log.info(_("Cash add {}. units {} become to {}".format(amount, self._units ,_units)))
+        user_system_log.debug(_("Cash add {}. units {} become to {}".format(amount, self._units, _units)))
         self._units = _units
 
+    def finance_repay(self, amount, account_type):
+        """ 融资还款 """
+        if Environment.get_instance().config.base.run_type == RUN_TYPE.LIVE_TRADING:
+            raise ValueError("finance and report api not support LIVE_TRADING")
+
+        if account_type not in self._accounts:
+            raise ValueError(_("invalid account type {}, choose in {}".format(account_type, list(self._accounts.keys()))))
+        self._accounts[account_type].finance_repay(amount)
 
-class MixedPositions(dict):
 
+class MixedPositions(Mapping):
     def __init__(self, accounts):
         super(MixedPositions, self).__init__()
         self._accounts = accounts
 
-    def __missing__(self, key):
-        account_type = Portfolio.get_account_type(key)
-        for a_type in self._accounts:
-            if a_type == account_type:
-                return self._accounts[a_type].positions[key]
-        return None
-
     def __contains__(self, item):
-        return item in self.keys()
+        account_type = Portfolio.get_account_type(item)
+        return item in self._accounts[account_type].positions
+
+    def __getitem__(self, item):
+        account_type = Portfolio.get_account_type(item)
+        return self._accounts[account_type].positions[item]
 
     def __repr__(self):
         keys = []
         for account in six.itervalues(self._accounts):
-            keys += [order_book_id for order_book_id, position in account.positions.items() if position.quantity > 0]
+            keys += [
+                order_book_id for order_book_id, position in account.positions.items()
+                if getattr(position, "quantity", 0) > 0 or
+                getattr(position, "buy_quantity", 0) + getattr(position, "sell_quantity", 0) > 0
+            ]
         return str(sorted(keys))
 
     def __len__(self):
         return sum(len(account.positions) for account in six.itervalues(self._accounts))
 
     def __iter__(self):
-        keys = []
-        for account in six.itervalues(self._accounts):
-            keys += account.positions.keys()
-        for key in sorted(keys):
-            yield key
-
-    def items(self):
-        items = merge_dicts(*[account.positions.items() for account in six.itervalues(self._accounts)])
-        for k in sorted(items.keys()):
-            yield k, items[k]
-
-    def keys(self):
-        keys = []
-        for account in six.itervalues(self._accounts):
-            keys += list(account.positions.keys())
-        return sorted(keys)
+        for account in self._accounts.values():
+            yield from account.positions.keys()
```

### Comparing `rqalpha-4.9.2/rqalpha/portfolio/account.py` & `rqalpha-5.0.0/rqalpha/portfolio/account.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,18 +12,19 @@
 #         未经米筐科技授权，任何个人不得出于任何商业目的使用本软件（包括但不限于向第三方提供、销售、出租、出借、转让本软件、
 #         本软件的衍生产品、引用或借鉴了本软件功能或源代码的产品或服务），任何法人或其他组织不得出于任何目的使用本软件，
 #         否则米筐科技有权追究相应的知识产权侵权责任。
 #         在此前提下，对本软件的使用同样需要遵守 Apache 2.0 许可，Apache 2.0 许可与本许可冲突之处，以本许可为准。
 #         详细的授权流程，请联系 public@ricequant.com 获取。
 
 from itertools import chain
+from datetime import date
 from typing import Callable, Dict, Iterable, List, Optional, Union, Tuple
 
 import six
-from rqalpha.const import POSITION_DIRECTION, POSITION_EFFECT
+from rqalpha.const import POSITION_DIRECTION, POSITION_EFFECT, DEFAULT_ACCOUNT_TYPE, DAYS_CNT
 from rqalpha.environment import Environment
 from rqalpha.core.events import EVENT
 from rqalpha.model.order import Order, OrderStyle
 from rqalpha.model.trade import Trade
 from rqalpha.utils.class_helper import deprecated_property
 from rqalpha.utils.functools import lru_cache
 from rqalpha.utils.i18n import gettext as _
@@ -50,28 +51,38 @@
 
     __abandon_properties__ = [
         "holding_pnl",
         "realized_pnl",
         "dividend_receivable",
     ]
 
-    def __init__(self, account_type: str, total_cash: float, init_positions: Dict[str, Tuple[int, Optional[float]]]):
+    def __init__(
+            self, account_type: str, total_cash: float, init_positions: Dict[str, Tuple[int, Optional[float]]],
+            financing_rate: float
+    ):
         self._type = account_type
         self._total_cash = total_cash  # 包含保证金的总资金
+        self._env = Environment.get_instance()
 
         self._positions: Dict[str, Dict[POSITION_DIRECTION, Position]] = {}
         self._backward_trade_set = set()
         self._frozen_cash = 0
+        self._pending_deposit_withdraw: List[Tuple[date, float]] = []
+
+        self._cash_liabilities = 0      # 现金负债
 
         self.register_event()
 
         self._management_fee_calculator_func = lambda account, rate: account.total_value * rate
         self._management_fee_rate = 0.0
         self._management_fees = 0.0
 
+        # 融资利率/年
+        self._financing_rate = financing_rate
+
         for order_book_id, (init_quantity, init_price) in init_positions.items():
             position_direction = POSITION_DIRECTION.LONG if init_quantity > 0 else POSITION_DIRECTION.SHORT
             self._get_or_create_pos(order_book_id, position_direction, init_quantity, init_price)
 
     def __repr__(self):
         positions_repr = {}
         for order_book_id, positions in self._positions.items():
@@ -79,15 +90,15 @@
                 if position.quantity != 0:
                     positions_repr.setdefault(order_book_id, {})[direction.value] = position.quantity
         return "Account(cash={}, total_value={}, positions={})".format(
             self.cash, self.total_value, positions_repr
         )
 
     def register_event(self):
-        event_bus = Environment.get_instance().event_bus
+        event_bus = self._env.event_bus
         event_bus.add_listener(
             EVENT.TRADE, lambda e: self.apply_trade(e.trade, e.order) if e.account == self else None
         )
         event_bus.add_listener(EVENT.ORDER_PENDING_NEW, self._on_order_pending_new)
         event_bus.add_listener(EVENT.ORDER_CREATION_REJECT, self._on_order_unsolicited_update)
         event_bus.add_listener(EVENT.ORDER_UNSOLICITED_UPDATE, self._on_order_unsolicited_update)
         event_bus.add_listener(EVENT.ORDER_CANCELLATION_PASS, self._on_order_unsolicited_update)
@@ -209,14 +220,30 @@
         # type: () -> float
         """
         总费用
         """
         return sum(p.transaction_cost for p in self._iter_pos())
 
     @property
+    def cash_liabilities(self):
+        # type: () -> float
+        """
+        现金负债
+        """
+        return self._cash_liabilities
+
+    @property
+    def cash_liabilities_interest(self):
+        # type: () -> float
+        """
+        现金负债当日的利息
+        """
+        return self._cash_liabilities * self._financing_rate / DAYS_CNT.DAYS_A_YEAR
+
+    @property
     def margin(self) -> float:
         """
         总保证金
         """
         return sum(getattr(p, "margin", 0) for p in self._iter_pos())
 
     @property
@@ -237,31 +264,33 @@
 
     @property
     def daily_pnl(self):
         # type: () -> float
         """
         当日盈亏
         """
-        return self.trading_pnl + self.position_pnl - self.transaction_cost
+        return self.trading_pnl + self.position_pnl - self.transaction_cost - self.cash_liabilities_interest
 
     @property
-    def equity(self):
+    def position_equity(self):
         # type: () -> float
         """
         持仓总权益
         """
         return sum(p.equity for p in self._iter_pos())
 
     @property
-    def total_value(self):
-        # type: () -> float
+    def total_value(self) -> float:
         """
         账户总权益
         """
-        return self._total_cash + self.equity
+        total_value = self._total_cash + self.position_equity - self.cash_liabilities - self.cash_liabilities_interest
+        if self._pending_deposit_withdraw:
+            total_value += sum(amount for _, amount in self._pending_deposit_withdraw)
+        return total_value
 
     @property
     def total_cash(self):
         # type: () -> float
         """
         账户总资金
         """
@@ -280,38 +309,46 @@
         # type: () -> float
         """
         交易盈亏
         """
         return sum(p.trading_pnl for p in self._iter_pos())
 
     def _on_before_trading(self, _):
-        trading_date = Environment.get_instance().trading_dt.date()
+        for order_book_id, positions in list(self._positions.items()):
+            if all(p.quantity == 0 and p.equity == 0 for p in six.itervalues(positions)):
+                del self._positions[order_book_id]
+
+        trading_date = self._env.trading_dt.date()
+        while self._pending_deposit_withdraw and self._pending_deposit_withdraw[0][0].date() <= trading_date:
+            _, amount = self._pending_deposit_withdraw.pop(0)
+            self._total_cash += amount
+
         for position in self._iter_pos():
             self._total_cash += position.before_trading(trading_date)
 
+        # 负债自增利息
+        if self._cash_liabilities > 0:
+            self._cash_liabilities += self.cash_liabilities_interest
+
     def _on_settlement(self, event):
-        trading_date = Environment.get_instance().trading_dt.date()
+        trading_date = self._env.trading_dt.date()
 
         for order_book_id, positions in list(self._positions.items()):
             for position in six.itervalues(positions):
                 delta_cash = position.settlement(trading_date)
                 self._total_cash += delta_cash
 
-        for order_book_id, positions in list(self._positions.items()):
-            if all(p.quantity == 0 and p.equity == 0 for p in six.itervalues(positions)):
-                del self._positions[order_book_id]
-
         self._backward_trade_set.clear()
 
         fee = self._management_fee()
         self._management_fees += fee
         self._total_cash -= fee
 
         # 如果 total_value <= 0 则认为已爆仓，清空仓位，资金归0
-        forced_liquidation = Environment.get_instance().config.base.forced_liquidation
+        forced_liquidation = self._env.config.base.forced_liquidation
         if self.total_value <= 0 and forced_liquidation:
             if self._positions:
                 user_system_log.warn(_("Trigger Forced Liquidation, current total_value is 0"))
             self._positions.clear()
             self._total_cash = 0
 
     def _on_order_pending_new(self, event):
@@ -363,25 +400,24 @@
             self,
             order_book_id: str,
             direction: Union[POSITION_DIRECTION, str],
             init_quantity: float = 0,
             init_price : Optional[float] = None
     ) -> Position:
         if order_book_id not in self._positions:
-            env = Environment.get_instance()
             if direction == POSITION_DIRECTION.LONG:
                 long_quantity, short_quantity = init_quantity, 0
             else:
                 long_quantity, short_quantity = 0, init_quantity
             positions = self._positions.setdefault(order_book_id, {
                 POSITION_DIRECTION.LONG: Position(order_book_id, POSITION_DIRECTION.LONG, long_quantity, init_price),
                 POSITION_DIRECTION.SHORT: Position(order_book_id, POSITION_DIRECTION.SHORT, short_quantity, init_price)
             })
             if not init_price:
-                last_price = env.get_last_price(order_book_id)
+                last_price = self._env.get_last_price(order_book_id)
                 for p in positions.values():
                     p.update_last_price(last_price)
             if hasattr(positions[direction], "margin") and hasattr(self.__class__, "_margin"):
                 # black magic: improve performance for pure stock strategy
                 setattr(self.__class__, "margin", self.__class__._margin)
                 del self.__class__._margin
         else:
@@ -394,29 +430,27 @@
             positions = self._positions[tick.order_book_id]
         except KeyError:
             return
         for position in positions.values():
             position.update_last_price(tick.last)
 
     def _on_bar(self, _):
-        env = Environment.get_instance()
         for order_book_id, positions in self._positions.items():
-            price = env.get_last_price(order_book_id)
+            price = self._env.get_last_price(order_book_id)
             if price == price:
                 for position in six.itervalues(positions):
                     position.update_last_price(price)
 
     def _frozen_cash_of_order(self, order):
-        env = Environment.get_instance()
         if order.position_effect == POSITION_EFFECT.OPEN:
-            instrument = env.data_proxy.instrument(order.order_book_id)
+            instrument = self._env.data_proxy.instrument(order.order_book_id)
             order_cost = instrument.calc_cash_occupation(order.frozen_price, order.quantity, order.position_direction)
         else:
             order_cost = 0
-        return order_cost + env.get_order_transaction_cost(order)
+        return order_cost + self._env.get_order_transaction_cost(order)
 
     def _management_fee(self):
         # type: () -> float
         """计算账户管理费用"""
         if self._management_fee_rate == 0:
             return 0
         fee = self._management_fee_calculator_func(self, self._management_fee_rate)
@@ -446,16 +480,44 @@
 
     @property
     def management_fees(self):
         # type: () -> float
         """该账户的管理费用总计"""
         return self._management_fees
 
-    def deposit_withdraw(self, amount):
-        # type: (float) -> None
+    def deposit_withdraw(self, amount: float, receiving_days: int = 0):
         """出入金"""
         if (amount < 0) and (self.cash < amount * -1):
             raise ValueError(_('insufficient cash, current {}, target withdrawal {}').format(self._total_cash, amount))
-        self._total_cash += amount
+        if receiving_days >= 1:
+            receiving_date = self._env.data_proxy.get_next_trading_date(self._env.trading_dt.date(), n=receiving_days)
+            self._pending_deposit_withdraw.append((receiving_date, amount))
+            self._pending_deposit_withdraw.sort(key=lambda i: i[0])
+        else:
+            self._total_cash += amount
+
+    def finance_repay(self, amount):
+        """ 融资还款 """
+        if self.type == DEFAULT_ACCOUNT_TYPE.STOCK:
+            if amount > 0:
+                # 融资
+                self._cash_liabilities += amount
+                self._total_cash += amount
+            elif amount < 0:
+                # 还款
+                amount *= -1
+                if amount > self.cash:
+                    user_system_log.warn(_('insufficient cash, current {}, target withdrawal {}').format(self.cash, amount))
+                # 预防还多了
+                excess = min(0, self._cash_liabilities - amount)
+                if excess < 0:
+                    user_system_log.warn("repay amount is greater than cash liabilities")
+                self._cash_liabilities = max(0, self._cash_liabilities - amount)
+                self._total_cash -= amount + excess
+            else:
+                pass
+        else:
+            user_system_log.warn(f"{self.type} not support finance_repay")
 
     holding_pnl = deprecated_property("holding_pnl", "position_pnl")
     realized_pnl = deprecated_property("realized_pnl", "trading_pnl")
+    equity = deprecated_property("equity", "position_equity")
```

### Comparing `rqalpha-4.9.2/rqalpha/portfolio/position.py` & `rqalpha-5.0.0/rqalpha/portfolio/position.py`

 * *Files 4% similar despite different names*

```diff
@@ -115,20 +115,23 @@
         # type: () -> float
         return self._avg_price
 
     @property
     def trading_pnl(self):
         # type: () -> float
         trade_quantity = self._quantity - self._logical_old_quantity
-        return (trade_quantity * self.last_price - self._trade_cost) * self._direction_factor
+        return (trade_quantity * self.last_price - self._trade_cost) * self._direction_factor if trade_quantity else 0
 
     @property
     def position_pnl(self):
         # type: () -> float
-        return self._logical_old_quantity * (self.last_price - self.prev_close) * self._direction_factor
+        if self._logical_old_quantity:
+            return self._logical_old_quantity * (self.last_price - self.prev_close) * self._direction_factor
+        else:
+            return 0
 
     @property
     def pnl(self):
         # type: () -> float
         """
         返回该持仓的累积盈亏
         """
@@ -143,27 +146,21 @@
     def equity(self):
         # type: () -> float
         return self.last_price * self._quantity if self._quantity else 0
 
     @property
     def prev_close(self):
         if not is_valid_price(self._prev_close):
-            env = Environment.get_instance()
-            self._prev_close = env.data_proxy.get_prev_close(self._order_book_id, env.trading_dt)
+            self._prev_close = self._env.data_proxy.get_prev_close(self._order_book_id, self._env.trading_dt)
         return self._prev_close
 
     @property
     def last_price(self):
-        if not self._last_price:
-            env = Environment.get_instance()
-            self._last_price = env.data_proxy.get_last_price(self._order_book_id)
-            if not is_valid_price(self._last_price):
-                raise RuntimeError(_("invalid price of {order_book_id}: {price}").format(
-                    order_book_id=self._order_book_id, price=self._last_price
-                ))
+        if not is_valid_price(self._last_price):
+            self._last_price = self._env.data_proxy.get_last_price(self._order_book_id)
         return self._last_price
 
     @property
     def closable(self):
         # type: () -> int
         """
         可平仓位
@@ -205,16 +202,19 @@
         self._trade_cost = state.get("trade_cost", 0)
         self._transaction_cost = state.get("transaction_cost", 0)
         self._prev_close = state.get("prev_close")
 
     def before_trading(self, trading_date):
         # type: (date) -> float
         # 返回该阶段导致总资金的变化量
-        self._prev_close = self.last_price
+        self._old_quantity = self._quantity
+        self._logical_old_quantity = self._old_quantity
+        self._trade_cost = self._non_closable = 0
         self._transaction_cost = 0
+        self._prev_close = None
         return 0
 
     def apply_trade(self, trade):
         # type: (Trade) -> float
         # 返回总资金的变化量
         self._transaction_cost += trade.transaction_cost
         if trade.position_effect == POSITION_EFFECT.OPEN:
@@ -236,29 +236,26 @@
             raise NotImplementedError("{} does not support position effect {}".format(
                 self.__class__.__name__, trade.position_effect
             ))
 
     def settlement(self, trading_date):
         # type: (date) -> float
         # 返回该阶段导致总资金的变化量以及反映该阶段引起其他持仓变化的虚拟交易，虚拟交易用于换代码，转股等操作
-        self._old_quantity = self._quantity
-        self._logical_old_quantity = self._old_quantity
-        self._trade_cost = self._non_closable = 0
         return 0
 
     def update_last_price(self, price):
         self._last_price = price
 
     def calc_close_today_amount(self, trade_amount):
         return 0
 
     @property
     def _open_orders(self):
         # type: () -> Iterable[Order]
-        for order in Environment.get_instance().broker.get_open_orders(self.order_book_id):
+        for order in self._env.broker.get_open_orders(self.order_book_id):
             if order.position_direction == self._direction:
                 yield order
 
 
 class PositionProxy(metaclass=PositionProxyMeta):
     __repr_properties__ = (
         "order_book_id", "positions"
```

### Comparing `rqalpha-4.9.2/rqalpha/resource/ricequant-logo.png` & `rqalpha-5.0.0/rqalpha/resource/ricequant-logo.png`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/user_module.py` & `rqalpha-5.0.0/rqalpha/user_module.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/utils/__init__.py` & `rqalpha-5.0.0/rqalpha/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
             other = other.__dict__
         target_dict = target.__dict__ if isinstance(target, RqAttrDict) else target
 
         for k, v in other.items():
             if isinstance(v, RqAttrDict):
                 v = v.__dict__
             if isinstance(v, Mapping):
-                r = RqAttrDict._update_dict_recursive(target_dict.get(k, {}), v)
+                r = RqAttrDict._update_dict_recursive(target_dict[k] if target_dict.get(k) else {}, v)
                 target_dict[k] = r
             else:
                 target_dict[k] = other[k]
         return target
 
     def convert_to_dict(self):
         result_dict = {}
@@ -123,21 +123,14 @@
     if filename == strategy_filename:
         error.error_type = EXC_TYPE.USER_EXC
 
     user_exc = CustomException(error)
     return user_exc
 
 
-def merge_dicts(*dict_args):
-    result = {}
-    for d in dict_args:
-        result.update(d)
-    return result
-
-
 def account_type_str2enum(type_str):
     return DEFAULT_ACCOUNT_TYPE[type_str]
 
 
 INST_TYPE_IN_STOCK_ACCOUNT = [
     INSTRUMENT_TYPE.CS,
     INSTRUMENT_TYPE.ETF,
@@ -239,7 +232,12 @@
 # -------------- deprecated --------------
 
 def get_trading_period(universe, accounts):
     # for compatible
     from rqalpha.environment import Environment
     trading_period = STOCK_TRADING_PERIOD if DEFAULT_ACCOUNT_TYPE.STOCK in accounts else []
     return Environment.get_instance().data_proxy.get_trading_period(universe, trading_period)
+
+
+def safe_div(dividend, divisor):
+    return dividend / divisor if divisor else np.nan
+
```

### Comparing `rqalpha-4.9.2/rqalpha/utils/arg_checker.py` & `rqalpha-5.0.0/rqalpha/utils/arg_checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from rqalpha.utils.exception import RQInvalidArgument, RQTypeError, RQApiNotSupportedError
 from rqalpha.model.instrument import Instrument
 from rqalpha.environment import Environment
 from rqalpha.const import INSTRUMENT_TYPE, EXC_TYPE
 from rqalpha.utils import unwrapper, INST_TYPE_IN_STOCK_ACCOUNT
 from rqalpha.utils.i18n import gettext as _
 from rqalpha.utils.exception import patch_system_exc, EXC_EXT_NAME
+from rqalpha.utils.logger import user_system_log
 
 
 main_contract_warning_flag = True
 index_contract_warning_flag = True
 
 
 class ArgumentChecker(object):
@@ -137,14 +138,22 @@
                     func_name, self._arg_name, value, type(value))
             )
 
     def is_number(self):
         self._rules.append(self._is_number)
         return self
 
+    def deprecated(self, hint="deprecated"):
+        def inner(func_name, value):
+            if value is not None:
+                content = "{} param {} is deprecated. {}".format(func_name, self._arg_name, hint)
+                user_system_log.warning(content)
+        self._rules.append(inner)
+        return self
+
     def is_in(self, valid_values, ignore_none=True):
         def check_is_in(func_name, value):
             if ignore_none and value is None:
                 return
 
             if value not in valid_values:
                 raise RQInvalidArgument(
@@ -232,46 +241,46 @@
                 ))
 
         self._rules.append(check_is_valid_date)
         return self
 
     def is_greater_or_equal_than(self, low):
         def check_greater_or_equal_than(func_name, value):
-            if value < low:
+            if isinstance(value, (int, float)) and value < low:
                 raise RQInvalidArgument(
                     _(u"function {}: invalid {} argument, expect a value >= {}, got {} (type: {})").format(
                         func_name, self._arg_name, low, value, type(value)
                     ))
         self._rules.append(check_greater_or_equal_than)
         return self
 
     def is_greater_than(self, low):
         def check_greater_than(func_name, value):
-            if value <= low:
+            if isinstance(value, (int, float)) and value <= low:
                 raise RQInvalidArgument(
                     _(u"function {}: invalid {} argument, expect a value > {}, got {} (type: {})").format(
                         func_name, self._arg_name, low, value, type(value)
                     ))
         self._rules.append(check_greater_than)
         return self
 
     def is_less_or_equal_than(self, high):
         def check_less_or_equal_than(func_name, value):
-            if value > high:
+            if isinstance(value, (int, float)) and value > high:
                 raise RQInvalidArgument(
                     _(u"function {}: invalid {} argument, expect a value <= {}, got {} (type: {})").format(
                         func_name, self._arg_name, high, value, type(value)
                     ))
 
         self._rules.append(check_less_or_equal_than)
         return self
 
     def is_less_than(self, high):
         def check_less_than(func_name, value):
-            if value >= high:
+            if isinstance(value, (int, float)) and value >= high:
                 raise RQInvalidArgument(
                     _(u"function {}: invalid {} argument, expect a value < {}, got {} (type: {})").format(
                         func_name, self._arg_name, high, value, type(value)
                     ))
 
         self._rules.append(check_less_than)
         return self
```

### Comparing `rqalpha-4.9.2/rqalpha/utils/class_helper.py` & `rqalpha-5.0.0/rqalpha/utils/class_helper.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/utils/click_helper.py` & `rqalpha-5.0.0/rqalpha/utils/click_helper.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/utils/concurrent.py` & `rqalpha-5.0.0/rqalpha/utils/concurrent.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,22 +46,24 @@
         self._progress_queue = multiprocessing.Queue()
         self._futures = []
         self._total_steps = 0
 
     def _adjust_process_count(self):
         # noinspection PyUnresolvedReferences
         for _ in range(len(self._processes), self._max_workers):
-            # noinspection PyUnresolvedReferences
-            p = multiprocessing.Process(
-                target=_process_worker,
-                args=(self._call_queue, self._result_queue, self._progress_queue, self._initializer, self._initargs)
-            )
-            p.start()
-            # noinspection PyUnresolvedReferences
-            self._processes[p.pid] = p
+            self._spawn_process()
+
+    def _spawn_process(self):
+        p = multiprocessing.Process(
+            target=_process_worker,
+            args=(self._call_queue, self._result_queue, self._progress_queue, self._initializer, self._initargs)
+        )
+        p.start()
+        # noinspection PyUnresolvedReferences
+        self._processes[p.pid] = p
 
     def submit(self, fn, *args, **kwargs):
         if isinstance(fn, ProgressedTask):
             # noinspection PyUnresolvedReferences
             self._total_steps += fn.total_steps
         else:
             self._total_steps += 1
```

### Comparing `rqalpha-4.9.2/rqalpha/utils/config.py` & `rqalpha-5.0.0/rqalpha/utils/config.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/utils/datetime_func.py` & `rqalpha-5.0.0/rqalpha/utils/datetime_func.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 
 def convert_date_to_date_int(dt):
     t = dt.year * 10000 + dt.month * 100 + dt.day
     return t
 
 
 def convert_date_to_int(dt):
-    t = dt.year * 10000 + dt.month * 100 + dt.day
-    t *= 1000000
+    # 原先的写法在pandas2.0下会被转化为int32类型导致精度丢失
+    t = dt.year * 10000000000 + dt.month * 100000000 + dt.day * 1000000
     return t
 
 
 def convert_dt_to_int(dt):
     t = convert_date_to_int(dt)
     t += dt.hour * 10000 + dt.minute * 100 + dt.second
     return t
```

### Comparing `rqalpha-4.9.2/rqalpha/utils/dict_func.py` & `rqalpha-5.0.0/rqalpha/utils/dict_func.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/utils/exception.py` & `rqalpha-5.0.0/rqalpha/utils/exception.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/utils/functools.py` & `rqalpha-5.0.0/rqalpha/utils/functools.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/utils/i18n.py` & `rqalpha-5.0.0/rqalpha/utils/i18n.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,22 +25,27 @@
 from rqalpha.utils.logger import system_log
 
 
 class Localization(object):
 
     def __init__(self, lc=None):
         if lc is None:
-            # https://stackoverflow.com/questions/3425294/how-to-detect-the-os-default-language-in-python
-            if os.name == "nt":
-                lc = locale.windows_locale[ctypes.windll.kernel32.GetUserDefaultUILanguage()]
-            else:
-                # 修改虚拟环境的本地语言读取
-                lc = os.getenv("LANG") or os.getenv("LC_CTYPE")
+            lc = self.get_sys_lc()
         self.trans = self.get_trans(lc)
 
+    @staticmethod
+    def get_sys_lc():
+        # https://stackoverflow.com/questions/3425294/how-to-detect-the-os-default-language-in-python
+        if os.name == "nt":
+            lc = locale.windows_locale[ctypes.windll.kernel32.GetUserDefaultUILanguage()]
+        else:
+            # 修改虚拟环境的本地语言读取
+            lc = os.getenv("LANG") or os.getenv("LC_CTYPE")
+        return lc
+
     @classmethod
     def get_trans(cls, lc: Optional[str], trans_dir=None):
         if lc is not None and "cn" in lc.lower():
             locales = ["zh_Hans_CN"]
             try:
                 if trans_dir is None:
                     trans_dir = os.path.join(os.path.dirname(os.path.abspath(__file__)), "translations")
```

### Comparing `rqalpha-4.9.2/rqalpha/utils/log_capture.py` & `rqalpha-5.0.0/rqalpha/utils/log_capture.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/utils/logger.py` & `rqalpha-5.0.0/rqalpha/utils/logger.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/utils/package_helper.py` & `rqalpha-5.0.0/rqalpha/utils/package_helper.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/utils/persisit_helper.py` & `rqalpha-5.0.0/rqalpha/utils/persisit_helper.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/utils/repr.py` & `rqalpha-5.0.0/rqalpha/utils/repr.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/utils/risk_free_helper.py` & `rqalpha-5.0.0/rqalpha/utils/risk_free_helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,7 +45,11 @@
     for t in YIELD_CURVE_DURATION:
         if duration >= t:
             tenor = t
         else:
             break
 
     return YIELD_CURVE_TENORS[tenor]
+
+
+def get_tenors_for(start_date, end_date):
+    return [YIELD_CURVE_TENORS[t] for t in YIELD_CURVE_DURATION if (end_date - start_date).days >= t]
```

### Comparing `rqalpha-4.9.2/rqalpha/utils/rq_json.py` & `rqalpha-5.0.0/rqalpha/utils/rq_json.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/utils/strategy_loader_help.py` & `rqalpha-5.0.0/tests/api_tests/mod/sys_scheduler/test_physical_time.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 # -*- coding: utf-8 -*-
 # 版权所有 2019 深圳米筐科技有限公司（下称“米筐科技”）
 #
 # 除非遵守当前许可，否则不得使用本软件。
 #
 #     * 非商业用途（非商业用途指个人出于非商业目的使用本软件，或者高校、研究所等非营利机构出于教育、科研等目的使用本软件）：
-#         遵守 Apache License 2.0（下称“Apache 2.0 许可”），您可以在以下位置获得 Apache 2.0 许可的副本：http://www.apache.org/licenses/LICENSE-2.0。
+#         遵守 Apache License 2.0（下称“Apache 2.0 许可”），
+#         您可以在以下位置获得 Apache 2.0 许可的副本：http://www.apache.org/licenses/LICENSE-2.0。
 #         除非法律有要求或以书面形式达成协议，否则本软件分发时需保持当前许可“原样”不变，且不得附加任何条件。
 #
 #     * 商业用途（商业用途指个人出于任何商业目的使用本软件，或者法人或其他组织出于任何目的使用本软件）：
-#         未经米筐科技授权，任何个人不得出于任何商业目的使用本软件（包括但不限于向第三方提供、销售、出租、出借、转让本软件、本软件的衍生产品、引用或借鉴了本软件功能或源代码的产品或服务），任何法人或其他组织不得出于任何目的使用本软件，否则米筐科技有权追究相应的知识产权侵权责任。
+#         未经米筐科技授权，任何个人不得出于任何商业目的使用本软件（包括但不限于向第三方提供、销售、出租、出借、转让本软件、
+#         本软件的衍生产品、引用或借鉴了本软件功能或源代码的产品或服务），任何法人或其他组织不得出于任何目的使用本软件，
+#         否则米筐科技有权追究相应的知识产权侵权责任。
 #         在此前提下，对本软件的使用同样需要遵守 Apache 2.0 许可，Apache 2.0 许可与本许可冲突之处，以本许可为准。
 #         详细的授权流程，请联系 public@ricequant.com 获取。
 
-import sys
-import traceback
-import six
-
-from rqalpha.utils.exception import patch_user_exc, CustomError, CustomException
-
-
-def compile_strategy(source_code, strategy, scope):
-    try:
-        code = compile(source_code, strategy, 'exec')
-        six.exec_(code, scope)
-        return scope
-    except Exception as e:
-        exc_type, exc_val, exc_tb = sys.exc_info()
-        exc_val = patch_user_exc(exc_val, force=True)
-        try:
-            msg = str(exc_val)
-        except Exception as e1:
-            msg = ""
-            six.print_(e1)
-
-        error = CustomError()
-        error.set_msg(msg)
-        error.set_exc(exc_type, exc_val, exc_tb)
-        stackinfos = list(traceback.extract_tb(exc_tb))
-
-        if isinstance(e, (SyntaxError, IndentationError)):
-            error.add_stack_info(exc_val.filename, exc_val.lineno, "", exc_val.text)
-        else:
-            for item in stackinfos:
-                filename, lineno, func_name, code = item
-                if strategy == filename:
-                    error.add_stack_info(*item)
-            # avoid empty stack
-            if error.stacks_length == 0:
-                error.add_stack_info(*item)
 
-        raise CustomException(error)
+__config__ = {
+    "base": {
+        "start_date": "2015-01-01",
+        "end_date": "2015-12-31",
+        "frequency": "1d",
+        "accounts": {
+            "future": 1000000,
+        }
+    },
+    "extra": {
+        "log_level": "error",
+    },
+}
+
+
+def test_physical_time():
+    """
+    测试 physical_time 的使用
+    """
+    from rqalpha.mod.rqalpha_mod_sys_scheduler.scheduler import physical_time
+
+    def _day(context, bar_dict):
+        context.counter += 1
+
+    def init(context):
+        context.counter = 0
+        scheduler.run_daily(_day, time_rule=physical_time(hour=9, minute=31))
+        context.days = 0
+
+    def handle_bar(context, bar_dict):
+        context.days += 1
+        assert context.counter == context.days
+
+    return locals()
```

### Comparing `rqalpha-4.9.2/rqalpha/utils/testing/__init__.py` & `rqalpha-5.0.0/rqalpha/utils/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/utils/testing/fixtures.py` & `rqalpha-5.0.0/rqalpha/utils/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/utils/testing/mocking.py` & `rqalpha-5.0.0/rqalpha/utils/testing/mocking.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/utils/translations/__init__.py` & `rqalpha-5.0.0/rqalpha/utils/translations/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/__init__.py` & `rqalpha-5.0.0/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.mo` & `rqalpha-5.0.0/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.mo`

 * *Files 14% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,19 +2,19 @@
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "PO-Revision-Date: 2016-10-24 21:20+0800\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: zh_Hans_CN\n"
 "Language-Team: zh_Hans_CN <LL@li.org>\n"
-"Plural-Forms: nplurals=1; plural=0\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.9.1\n"
+"Generated-By: Babel 2.10.1\n"
 
 msgid ""
 "\n"
 "    [WARNING]\n"
 "    Target bundle path {data_bundle_path} is not empty.\n"
 "    The content of this folder will be REMOVED before updating.\n"
 "    Are you sure to continue?"
@@ -60,14 +60,17 @@
 
 msgid "Beta"
 msgstr "贝塔"
 
 msgid "Cash add {}. units {} become to {}"
 msgstr "入金{}元，份额由{}变动为{}"
 
+msgid "Check bundle"
+msgstr "检测 Bundle 数据"
+
 msgid "Close"
 msgstr "平仓"
 
 msgid ""
 "Create order failed, there are active orders leading to the risk of self-"
 "trade: [{}...]"
 msgstr "订单创建失败，当前存在可能导致自成交的挂单：[{}...]"
@@ -91,37 +94,37 @@
 "Environment 并没有被创建，请再 RQAlpha 初始化之后使用 `Environment."
 "get_instance() 函数`"
 
 msgid "Excess"
 msgstr "超额收益"
 
 msgid "ExcessAnnual"
-msgstr "年化超额收益率"
-
-msgid "ExcessAnnualVolatility"
-msgstr "超额收益年化波动率"
+msgstr "年化超额收益率（几何）"
 
 msgid "ExcessCumReturns"
-msgstr "超额累计收益"
+msgstr "超额收益率（算术）"
 
 msgid "ExcessMaxDD"
-msgstr "超额收益最大回撤"
+msgstr "超额收益最大回撤（几何）"
 
 msgid "ExcessMaxDD/ExcessMaxDDD"
 msgstr "超额收益最大回撤/最长回撤持续期"
 
 msgid "ExcessReturns"
-msgstr "超额收益率"
+msgstr "超额收益率（几何）"
 
 msgid "ExcessSharpe"
 msgstr "超额夏普率"
 
 msgid "ExcessVolatility"
 msgstr "超额收益波动率"
 
+msgid "ExcessWinRate"
+msgstr "超额胜率"
+
 msgid "Frequency {} is not support."
 msgstr "不支持回测频率: {}"
 
 msgid "Generate default config file"
 msgstr "生成默认的配置文件"
 
 msgid "Generate example strategies to target folder"
@@ -167,14 +170,20 @@
 msgid ""
 "Missing persist provider. You need to set persist_provider before use persist"
 msgstr "Persist provider 未加载，加载 Persist provider 方可使用 persist 功能。"
 
 msgid "Mod management command"
 msgstr "Mod 管理命令"
 
+msgid "MonthlySharpe"
+msgstr "月度夏普率"
+
+msgid "MonthlyVolatility"
+msgstr "月度波动率"
+
 msgid "Not supported matching type {}"
 msgstr "不支持撮合类型: {}"
 
 msgid "Open"
 msgstr "开仓"
 
 msgid "Order Cancelled: [{order_book_id}] has no liquidity."
@@ -192,14 +201,25 @@
 msgstr "订单被拒单: [{order_book_id}] 已涨停。"
 
 msgid ""
 "Order Cancelled: current security [{order_book_id}] can not be traded in "
 "listed date [{listed_date}]"
 msgstr "订单被撤销: [{order_book_id}] 上市首日无法交易"
 
+msgid "Order Cancelled: current tick [{order_book_id}] miss market data."
+msgstr "订单被拒单: [{order_book_id}] 当前缺失市场数据。"
+
+msgid ""
+"Order Cancelled: current tick [{order_book_id}] reach the limit_down price."
+msgstr "订单被拒单: [{order_book_id}] 已跌停。"
+
+msgid ""
+"Order Cancelled: current tick [{order_book_id}] reach the limit_up price."
+msgstr "订单被拒单: [{order_book_id}] 已涨停。"
+
 msgid ""
 "Order Cancelled: market order {order_book_id} fill {filled_volume} actually"
 msgstr "订单取消：标的 {order_book_id} 实际成交 {filled_volume}"
 
 msgid ""
 "Order Cancelled: market order {order_book_id} volume {order_volume} due to "
 "volume limit"
@@ -253,31 +273,28 @@
 msgstr ""
 "订单创建失败：{order_book_id} 的今仓不足，目标平今仓量为 {quantity}，可平今仓"
 "量为 {closable}"
 
 msgid "Order Creation Failed: security {order_book_id} is suspended on {date}"
 msgstr "订单创建失败: {order_book_id} 在 {date} 时停牌"
 
-msgid "Order Creation Failed: {order_book_id} has been delisted!"
-msgstr "订单创建失败: {order_book_id} 已退市"
-
-msgid "Order Creation Failed: {order_book_id} is not listed!"
-msgstr "订单创建失败: {order_book_id} 未上市"
-
 msgid "Order Rejected: {order_book_id} can not match. Market close."
 msgstr "订单被拒单: {order_book_id} 当天交易结束，订单无法成交。"
 
 msgid ""
 "Order was separated, original order: {original_order_repr}, new orders: "
 "[{new_orders_repr}]"
 msgstr "订单被拆分，原订单：{original_order_repr}，新订单：[{new_orders_repr}]"
 
 msgid "Output Version Info"
 msgstr "输出版本号信息"
 
+msgid "ProfitLossRate"
+msgstr "盈亏比"
+
 msgid "Run a strategy"
 msgstr "运行策略"
 
 msgid "Sharpe"
 msgstr "夏普率"
 
 msgid "Sortino"
@@ -313,49 +330,79 @@
 
 msgid "WeeklyAlpha"
 msgstr "周度阿尔法"
 
 msgid "WeeklyBeta"
 msgstr "周度贝塔"
 
+msgid "WeeklyExcessUlcerIndex"
+msgstr "周度超额累计回撤深度"
+
+msgid "WeeklyExcessUlcerPerformanceIndex"
+msgstr "周度超额累计回撤夏普率"
+
 msgid "WeeklyInfoRatio"
 msgstr "周度信息比率"
 
 msgid "WeeklyMaxDrawdown"
 msgstr "周度最大回撤"
 
 msgid "WeeklySharpe"
 msgstr "周度夏普率"
 
-msgid "WeeklySortino"
-msgstr "周度索提诺比率"
-
 msgid "WeeklyTrackingError"
 msgstr "周度跟踪误差"
 
+msgid "WeeklyUlcerIndex"
+msgstr "周度累计回撤深度"
+
+msgid "WeeklyUlcerPerformanceIndex"
+msgstr "周度累计回撤夏普率"
+
+msgid "WeeklyVolatility"
+msgstr "周度波动率"
+
+msgid "WeeklyWinRate"
+msgstr "周度胜率"
+
+msgid "WinRate"
+msgstr "胜率"
+
 msgid "You cannot call %s when executing %s"
 msgstr "%s 不能在 %s 中调用。"
 
 msgid "[sys_analyser] Generate report from strategy output file"
 msgstr "【sys_analyser】使用策略输出的文件生成报告"
 
 msgid "[sys_analyser] Plot from strategy output file"
 msgstr "【sys_analyser】使用策略输出的文件绘制收益图"
 
+msgid "benchmark not exists, please entry correct order_book_id"
+msgstr "当前使用的基准合约信息不存在，请输入正确的合约"
+
 msgid "bundle not exist, use \"rqalpha create-bundle\" command instead"
 msgstr "bundle 不存在，执行 \"rqalpha create-bundle\" 以创建 bundle"
 
+msgid "bundle's day bar is incomplete, please update bundle"
+msgstr "Bundle日线数据不完整，请及时更新bundle"
+
 msgid "cancel_order function is not supported in signal mode"
 msgstr "在 Signal 模式下，不支持 cancel_order 函数"
 
 msgid ""
 "config 'base.benchmark' is deprecated, use 'mod.sys_analyser.benchmark' "
 "instead"
 msgstr "配置'base.benchmark'已被弃用，使用'mod.sys_analyser.benchmark'代替"
 
+msgid "corrupted files"
+msgstr "已损坏的文件"
+
+msgid "corrupted files not remove"
+msgstr "已损坏的文件尚未删除"
+
 msgid "create bundle using RQDatac"
 msgstr "使用 RQDatac 创建 Bundle"
 
 msgid "deprecated parameter[bar_dict] in before_trading function."
 msgstr "[Deprecated]在before_trading函数中，第二个参数bar_dict已经不再使用了。"
 
 msgid "downloading ..."
@@ -382,14 +429,17 @@
 msgid ""
 "function {}: invalid {} argument, quarter should be in form of '2012q3', got "
 "{} (type: {})"
 msgstr ""
 "函数 {}：参数 {} 不合法，季度应为形如 '2012q3' 的字符串，传入的是 {}（类型："
 "{}）"
 
+msgid "good bundle's day bar"
+msgstr "Bundle日线数据良好"
+
 msgid "id_or_symbols {} does not exist"
 msgstr "您选择的证券[{}]不存在。"
 
 msgid "in get_dividend, start_date {} is later than the previous test day {}"
 msgstr ""
 "在 get_dividend 函数中，start_date {} 晚于当前回测时间的上一个交易日 {}。"
 
@@ -413,14 +463,17 @@
 
 msgid "in index_weights, date {} is no earlier than previous test date {}"
 msgstr "在API index_weights 中, 参数date={} 不应晚于上一交易日 {}"
 
 msgid "in parse_user_config, exception: {e}"
 msgstr "在执行 parse_user_config 时，产生异常: {e}"
 
+msgid "input error"
+msgstr "输入异常"
+
 msgid "insufficient cash, current {}, target withdrawal {}"
 msgstr "现金不足，当前现金 {}，目标出金 {}"
 
 msgid "insufficient cash, use all remaining cash({}) to create order"
 msgstr "现金不足，使用当前剩余资金({})创建订单"
 
 msgid "invalid account type {}, choose in {}"
@@ -461,14 +514,20 @@
 msgid "not run {}({}, {}) because strategy is hold"
 msgstr "策略暂停中，取消执行 {}({}, {})"
 
 msgid ""
 "open data bundle failed, you can remove {} and try to regenerate bundle: {}"
 msgstr "读取 bundle 文件失败，请删除 {} 后尝试重新生成 bundle：{}"
 
+msgid "remove files"
+msgstr "是否删除文件"
+
+msgid "remove success"
+msgstr "文件删除完毕"
+
 msgid "rqdatac init failed with error: {}"
 msgstr "rqdatac 初始化失败：{}"
 
 msgid "rqdatac init failed, some apis will not function properly: {}"
 msgstr ""
 "rqdatac 初始化失败，部分扩展 API 可能无法使用，错误信息：{}。您可以访问 "
 "https://www.ricequant.com/welcome/rqdata 获取 rqdatac"
```

### Comparing `rqalpha-4.9.2/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.po` & `rqalpha-5.0.0/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2016.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2022-03-10 10:15+0800\n"
+"POT-Creation-Date: 2022-06-24 10:33+0800\n"
 "PO-Revision-Date: 2016-10-24 21:20+0800\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: zh_Hans_CN\n"
 "Language-Team: zh_Hans_CN <LL@li.org>\n"
-"Plural-Forms: nplurals=1; plural=0\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.9.1\n"
+"Generated-By: Babel 2.10.1\n"
 
 #: rqalpha/environment.py:70
 msgid ""
 "Environment has not been created. Please Use `Environment.get_instance()`"
 " after RQAlpha init"
 msgstr "Environment 并没有被创建，请再 RQAlpha 初始化之后使用 `Environment.get_instance() 函数`"
 
@@ -164,14 +164,41 @@
 msgid "bundle not exist, use \"rqalpha create-bundle\" command instead"
 msgstr "bundle 不存在，执行 \"rqalpha create-bundle\" 以创建 bundle"
 
 #: rqalpha/cmds/bundle.py:94
 msgid "Download bundle (monthly updated)"
 msgstr "下载（月度更新的）Bundle"
 
+msgid "Check bundle"
+msgstr "检测 Bundle 数据"
+
+msgid "corrupted files"
+msgstr "已损坏的文件"
+
+msgid "remove files"
+msgstr "是否删除文件"
+
+msgid "remove success"
+msgstr "文件删除完毕"
+
+msgid "corrupted files not remove"
+msgstr "已损坏的文件尚未删除"
+
+msgid "input error"
+msgstr "输入异常"
+
+msgid "bundle's day bar is incomplete, please update bundle"
+msgstr "Bundle日线数据不完整，请及时更新bundle"
+
+msgid "good bundle's day bar"
+msgstr "Bundle日线数据良好"
+
+msgid "benchmark not exists, please entry correct order_book_id"
+msgstr "当前使用的基准合约信息不存在，请输入正确的合约"
+
 #: rqalpha/cmds/bundle.py:105
 msgid ""
 "\n"
 "    [WARNING]\n"
 "    Target bundle path {data_bundle_path} is not empty.\n"
 "    The content of this folder will be REMOVED before updating.\n"
 "    Are you sure to continue?"
@@ -328,15 +355,17 @@
 msgstr "现金不足，使用当前剩余资金({})创建订单"
 
 #: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:296
 #, fuzzy
 msgid ""
 "function order_target_portfolio: invalid keys of target_portfolio, "
 "expected order_book_ids or Instrument objects, got {} (type: {})"
-msgstr "函数 order_target_portfolio：不合法的参数。target_portfolio 的键应为合约代码或 Instrument 对象，实际传入了 {}（类型：{}）。"
+msgstr ""
+"函数 order_target_portfolio：不合法的参数。target_portfolio 的键应为合约代码或 Instrument "
+"对象，实际传入了 {}（类型：{}）。"
 
 #: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:301
 msgid ""
 "function order_target_portfolio: invalid instrument type, excepted "
 "CS/ETF/LOF/INDX, got {}"
 msgstr "函数 order_target_portfolio：不合法的资产类型。应传入股票、ETF、LOF 或指数，实际传入了 {}。"
 
@@ -406,192 +435,217 @@
 msgid "show weekly indicators and return curve on plot"
 msgstr ""
 
 #: rqalpha/mod/rqalpha_mod_sys_analyser/__init__.py:113
 msgid "[sys_analyser] Generate report from strategy output file"
 msgstr "【sys_analyser】使用策略输出的文件生成报告"
 
-#: rqalpha/mod/rqalpha_mod_sys_analyser/mod.py:100
+#: rqalpha/mod/rqalpha_mod_sys_analyser/mod.py:108
 msgid ""
 "config 'base.benchmark' is deprecated, use 'mod.sys_analyser.benchmark' "
 "instead"
 msgstr "配置'base.benchmark'已被弃用，使用'mod.sys_analyser.benchmark'代替"
 
-#: rqalpha/mod/rqalpha_mod_sys_analyser/mod.py:182
+#: rqalpha/mod/rqalpha_mod_sys_analyser/mod.py:190
 msgid "invalid init benchmark {}, should be in format 'order_book_id:weight'"
 msgstr ""
 
-#: rqalpha/mod/rqalpha_mod_sys_analyser/mod.py:187
+#: rqalpha/mod/rqalpha_mod_sys_analyser/mod.py:195
 msgid "invalid weight for instrument {order_book_id}: {weight}"
 msgstr ""
 
-#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:59
+#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:61
 msgid "Strategy"
 msgstr "策略收益"
 
-#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:60
+#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:62
 msgid "Benchmark"
 msgstr "基准收益"
 
-#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:61
+#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:63
 msgid "Excess"
 msgstr "超额收益"
 
-#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:62
+#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:64
 msgid "Weekly"
 msgstr "策略周度收益"
 
-#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:63
+#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:65
 msgid "BenchmarkWeekly"
 msgstr "基准周度收益"
 
-#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:65
-#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:82
+#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:67
+#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:91
 msgid "MaxDrawDown"
 msgstr "最大回撤"
 
-#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:66
+#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:68
 msgid "MaxDDD"
 msgstr "最长回撤持续期"
 
-#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:67
+#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:69
 msgid "Open"
 msgstr "开仓"
 
-#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:68
+#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:70
 msgid "Close"
 msgstr "平仓"
 
-#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:71
+#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:73
 msgid "TotalReturns"
 msgstr "策略收益率"
 
-#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:72
+#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:74
 msgid "AnnualReturns"
 msgstr "策略年化收益率"
 
-#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:73
+#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:75
 msgid "Alpha"
 msgstr "阿尔法"
 
-#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:74
+#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:76
 msgid "Beta"
 msgstr "贝塔"
 
-#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:75
+#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:77
 msgid "Sharpe"
 msgstr "夏普率"
 
-#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:76
+#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:78
 msgid "Sortino"
 msgstr "索提诺比率"
 
-#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:77
-msgid "InformationRatio"
-msgstr "信息比率"
+msgid "WeeklyUlcerIndex"
+msgstr "周度累计回撤深度"
 
-#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:79
+#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:80
 msgid "BenchmarkReturns"
 msgstr "基准收益率"
 
-#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:80
+#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:81
 msgid "BenchmarkAnnual"
 msgstr "基准年化收益率"
 
-#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:81
+#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:82
 msgid "Volatility"
 msgstr "波动率"
 
 #: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:83
 msgid "TrackingError"
 msgstr "跟踪误差"
 
 #: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:84
 msgid "DownsideRisk"
 msgstr "下行风险"
 
 #: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:85
+msgid "InformationRatio"
+msgstr "信息比率"
+
+msgid "WeeklyUlcerPerformanceIndex"
+msgstr "周度累计回撤夏普率"
+
+#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:87
+msgid "ExcessCumReturns"
+msgstr "超额收益率（算术）"
+
+#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:88
+msgid "WinRate"
+msgstr "胜率"
+
+#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:89
+msgid "WeeklyWinRate"
+msgstr "周度胜率"
+
+#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:90
+msgid "ProfitLossRate"
+msgstr "盈亏比"
+
+#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:92
 msgid "MaxDD/MaxDDD"
 msgstr "最大回撤/最长回撤持续期"
 
-#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:89
+msgid "WeeklyExcessUlcerIndex"
+msgstr "周度超额累计回撤深度"
+
+#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:96
 msgid "WeeklyAlpha"
 msgstr "周度阿尔法"
 
-#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:90
+#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:97
 msgid "WeeklyBeta"
 msgstr "周度贝塔"
 
-#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:91
+#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:98
 msgid "WeeklySharpe"
 msgstr "周度夏普率"
 
-#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:92
-msgid "WeeklySortino"
-msgstr "周度索提诺比率"
-
-#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:93
+#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:99
 msgid "WeeklyInfoRatio"
 msgstr "周度信息比率"
 
-#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:94
+#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:100
 msgid "WeeklyTrackingError"
 msgstr "周度跟踪误差"
 
-#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:95
+#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:101
 msgid "WeeklyMaxDrawdown"
 msgstr "周度最大回撤"
 
-#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:99
+msgid "WeeklyVolatility"
+msgstr "周度波动率"
+
+msgid "MonthlySharpe"
+msgstr "月度夏普率"
+
+msgid "MonthlyVolatility"
+msgstr "月度波动率"
+
+#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:105
 msgid "ExcessReturns"
-msgstr "超额收益率"
+msgstr "超额收益率（几何）"
 
-#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:100
+#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:106
 msgid "ExcessAnnual"
-msgstr "年化超额收益率"
+msgstr "年化超额收益率（几何）"
 
-#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:101
+#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:107
 msgid "ExcessSharpe"
 msgstr "超额夏普率"
 
-#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:102
+#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:108
 msgid "ExcessVolatility"
 msgstr "超额收益波动率"
 
-#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:103
-msgid "ExcessAnnualVolatility"
-msgstr "超额收益年化波动率"
-
-#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:99
-msgid "ExcessCumReturns"
-msgstr "超额累计收益"
-
-#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:104
+#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:109
 msgid "ExcessMaxDD"
-msgstr "超额收益最大回撤"
+msgstr "超额收益最大回撤（几何）"
 
-#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:105
+msgid "ExcessWinRate"
+msgstr "超额胜率"
+
+#: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:110
 msgid "ExcessMaxDD/ExcessMaxDDD"
 msgstr "超额收益最大回撤/最长回撤持续期"
 
+msgid "WeeklyExcessUlcerPerformanceIndex"
+msgstr "周度超额累计回撤夏普率"
+
 #: rqalpha/mod/rqalpha_mod_sys_risk/validators/cash_validator.py:33
 msgid ""
 "Order Creation Failed: not enough money to buy {order_book_id}, needs "
 "{cost_money:.2f}, cash {cash:.2f}"
 msgstr "订单创建失败: 可用资金不足。当前资金: {cash:.2f}，{order_book_id} 下单所需资金: {cost_money:.2f}"
 
 #: rqalpha/mod/rqalpha_mod_sys_risk/validators/is_trading_validator.py:31
-msgid "Order Creation Failed: {order_book_id} is not listed!"
-msgstr "订单创建失败: {order_book_id} 未上市"
+#, fuzzy
+msgid "Order Creation Failed: {order_book_id} is not listing!"
+msgstr "订单创建失败: {order_book_id} 未上市或已退市"
 
 #: rqalpha/mod/rqalpha_mod_sys_risk/validators/is_trading_validator.py:37
-msgid "Order Creation Failed: {order_book_id} has been delisted!"
-msgstr "订单创建失败: {order_book_id} 已退市"
-
-#: rqalpha/mod/rqalpha_mod_sys_risk/validators/is_trading_validator.py:43
 msgid "Order Creation Failed: security {order_book_id} is suspended on {date}"
 msgstr "订单创建失败: {order_book_id} 在 {date} 时停牌"
 
 #: rqalpha/mod/rqalpha_mod_sys_risk/validators/price_validator.py:34
 msgid ""
 "Order Creation Failed: limit order price {limit_price} is higher than "
 "limit up {limit_up}, order_book_id={order_book_id}"
@@ -605,110 +659,136 @@
 
 #: rqalpha/mod/rqalpha_mod_sys_risk/validators/self_trade_validator.py:32
 msgid ""
 "Create order failed, there are active orders leading to the risk of self-"
 "trade: [{}...]"
 msgstr "订单创建失败，当前存在可能导致自成交的挂单：[{}...]"
 
-#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:116
+#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:101
+#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:319
 #: rqalpha/mod/rqalpha_mod_sys_simulation/signal_broker.py:66
 msgid ""
 "Order Cancelled: current security [{order_book_id}] can not be traded in "
 "listed date [{listed_date}]"
 msgstr "订单被撤销: [{order_book_id}] 上市首日无法交易"
 
-#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:123
+#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:108
 #: rqalpha/mod/rqalpha_mod_sys_simulation/signal_broker.py:72
 msgid "Order Cancelled: current bar [{order_book_id}] miss market data."
 msgstr "订单被拒单: [{order_book_id}] 当前缺失市场数据。"
 
-#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:148
+#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:128
 #: rqalpha/mod/rqalpha_mod_sys_simulation/signal_broker.py:86
 msgid "Order Cancelled: current bar [{order_book_id}] reach the limit_up price."
 msgstr "订单被拒单: [{order_book_id}] 已涨停。"
 
-#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:154
+#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:134
 #: rqalpha/mod/rqalpha_mod_sys_simulation/signal_broker.py:95
 msgid "Order Cancelled: current bar [{order_book_id}] reach the limit_down price."
 msgstr "订单被拒单: [{order_book_id}] 已跌停。"
 
-#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:161
-#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:167
-msgid "Order Cancelled: [{order_book_id}] has no liquidity."
-msgstr "合约 [{order_book_id}] 流动性不足，拒单。"
-
-#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:176
+#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:143
 msgid "Order Cancelled: {order_book_id} bar no volume"
 msgstr "订单被撤销：{order_book_id} 当前无成交量"
 
-#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:192
+#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:159
+#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:396
 msgid ""
 "Order Cancelled: market order {order_book_id} volume {order_volume} due "
 "to volume limit"
 msgstr "订单被撤销: 订单 [{order_book_id}] 的下单量 {order_volume} 超过了成交量限制。"
 
-#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:227
+#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:197
 msgid ""
 "Order Cancelled: market order {order_book_id} volume {order_volume} is "
 "larger than {volume_percent_limit} percent of current bar volume, fill "
 "{filled_volume} actually"
 msgstr ""
 "{order_book_id} 下单量 {order_volume} 超过当前 Bar 成交量的 "
 "{volume_percent_limit}%，实际成交 {filled_volume}"
 
-#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:321
+#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:326
+msgid "Order Cancelled: current tick [{order_book_id}] miss market data."
+msgstr "订单被拒单: [{order_book_id}] 当前缺失市场数据。"
+
+#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:351
+msgid "Order Cancelled: current tick [{order_book_id}] reach the limit_up price."
+msgstr "订单被拒单: [{order_book_id}] 已涨停。"
+
+#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:357
+msgid ""
+"Order Cancelled: current tick [{order_book_id}] reach the limit_down "
+"price."
+msgstr "订单被拒单: [{order_book_id}] 已跌停。"
+
+#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:364
+#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:370
+msgid "Order Cancelled: [{order_book_id}] has no liquidity."
+msgstr "合约 [{order_book_id}] 流动性不足，拒单。"
+
+#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:438
+#, fuzzy
+msgid ""
+"Order Cancelled: market order {order_book_id} volume {order_volume} is "
+"larger than {volume_percent_limit} percent of current tick volume, fill "
+"{filled_volume} actually"
+msgstr ""
+"{order_book_id} 下单量 {order_volume} 超过当前 Tick 成交量的 "
+"{volume_percent_limit}%，实际成交 {filled_volume}"
+
+#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:571
 msgid ""
 "Order Cancelled: market order {order_book_id} fill {filled_volume} "
 "actually"
 msgstr "订单取消：标的 {order_book_id} 实际成交 {filled_volume}"
 
 #: rqalpha/mod/rqalpha_mod_sys_simulation/mod.py:42
 msgid "invalid margin multiplier value: value range is (0, +∞]"
 msgstr "无效的 保证金乘数 设置: 其值范围为 (0, +∞]"
 
-#: rqalpha/mod/rqalpha_mod_sys_simulation/mod.py:52
-#: rqalpha/mod/rqalpha_mod_sys_simulation/mod.py:59
+#: rqalpha/mod/rqalpha_mod_sys_simulation/mod.py:51
+#: rqalpha/mod/rqalpha_mod_sys_simulation/mod.py:58
 msgid "Not supported matching type {}"
 msgstr "不支持撮合类型: {}"
 
-#: rqalpha/mod/rqalpha_mod_sys_simulation/mod.py:63
+#: rqalpha/mod/rqalpha_mod_sys_simulation/mod.py:62
 msgid ""
 "matching_type = 'next_bar' is abandoned when frequency == '1d',Current "
 "matching_type is 'current_bar'."
 msgstr "日回测 'next_bar' 撮合方式已废弃，当前按 'current_bar' 撮合方式成交"
 
-#: rqalpha/mod/rqalpha_mod_sys_simulation/mod.py:108
+#: rqalpha/mod/rqalpha_mod_sys_simulation/mod.py:107
 msgid "NO account_type = ({}) in {}"
 msgstr ""
 
 #: rqalpha/mod/rqalpha_mod_sys_simulation/signal_broker.py:53
 msgid "cancel_order function is not supported in signal mode"
 msgstr "在 Signal 模式下，不支持 cancel_order 函数"
 
-#: rqalpha/mod/rqalpha_mod_sys_simulation/simulation_broker.py:104
+#: rqalpha/mod/rqalpha_mod_sys_simulation/simulation_broker.py:108
 msgid "unsupported position_effect {}"
 msgstr "不支持的 position_effect {}"
 
-#: rqalpha/mod/rqalpha_mod_sys_simulation/simulation_broker.py:125
+#: rqalpha/mod/rqalpha_mod_sys_simulation/simulation_broker.py:129
 msgid "{order_id} order has been cancelled by user."
 msgstr "订单 {order_id} 被手动取消。"
 
-#: rqalpha/mod/rqalpha_mod_sys_simulation/simulation_broker.py:141
+#: rqalpha/mod/rqalpha_mod_sys_simulation/simulation_broker.py:145
 msgid "Order Rejected: {order_book_id} can not match. Market close."
 msgstr "订单被拒单: {order_book_id} 当天交易结束，订单无法成交。"
 
-#: rqalpha/mod/rqalpha_mod_sys_simulation/simulation_broker.py:180
+#: rqalpha/mod/rqalpha_mod_sys_simulation/simulation_broker.py:184
 msgid "{order_book_id} should be subscribed when frequency is tick."
 msgstr "tick回测下单失败，请使用 subscribe 订阅合约 {order_book_id}。"
 
 #: rqalpha/mod/rqalpha_mod_sys_simulation/simulation_event_source.py:46
 msgid "Current universe is empty. Please use subscribe function before trade"
 msgstr "当前合约池为空。请使用 subscribe 订阅合约。"
 
-#: rqalpha/mod/rqalpha_mod_sys_simulation/simulation_event_source.py:196
+#: rqalpha/mod/rqalpha_mod_sys_simulation/simulation_event_source.py:202
 msgid "Frequency {} is not support."
 msgstr "不支持回测频率: {}"
 
 #: rqalpha/mod/rqalpha_mod_sys_simulation/slippage.py:46
 msgid "Missing SlippageModel {}"
 msgstr "无法加载滑点模型 {}。"
 
@@ -753,15 +833,15 @@
 msgid "Cash add {}. units {} become to {}"
 msgstr "入金{}元，份额由{}变动为{}"
 
 #: rqalpha/portfolio/account.py:313
 msgid "Trigger Forced Liquidation, current total_value is 0"
 msgstr "触发强制清算，当前总权益为 0"
 
-#: rqalpha/portfolio/account.py:448
+#: rqalpha/portfolio/account.py:457
 msgid "insufficient cash, current {}, target withdrawal {}"
 msgstr "现金不足，当前现金 {}，目标出金 {}"
 
 #: rqalpha/portfolio/position.py:160
 msgid "invalid price of {order_book_id}: {price}"
 msgstr "{order_book_id} 的价格不合法：{price}"
 
@@ -1380,7 +1460,13 @@
 
 #~ msgid "last price of position {} is not supposed to be nan"
 #~ msgstr "仓位 {} 最新价不应该为 nan"
 
 #~ msgid "target percent of {} should between 0 and 1, current: {}"
 #~ msgstr "{} 的目标持仓需要在 0 到 1 之间，当前值：{}"
 
+#~ msgid "ExcessAnnualVolatility"
+#~ msgstr "超额收益年化波动率"
+
+#~ msgid "Order Creation Failed: {order_book_id} has been delisted!"
+#~ msgstr "订单创建失败: {order_book_id} 已退市"
+
```

### Comparing `rqalpha-4.9.2/rqalpha/utils/translations/zh_Hans_CN/__init__.py` & `rqalpha-5.0.0/rqalpha/utils/translations/zh_Hans_CN/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha/utils/typing.py` & `rqalpha-5.0.0/rqalpha/utils/typing.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/rqalpha.egg-info/PKG-INFO` & `rqalpha-5.0.0/rqalpha.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: rqalpha
-Version: 4.9.2
+Version: 5.0.0
 Summary: Ricequant Algorithm Trading System
 Home-page: https://github.com/ricequant/rqalpha
 Author: ricequant
 Author-email: public@ricequant.com
 License: Apache License v2
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
+Provides-Extra: profiler
 License-File: LICENSE
```

### Comparing `rqalpha-4.9.2/rqalpha.egg-info/SOURCES.txt` & `rqalpha-5.0.0/rqalpha.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -70,17 +70,19 @@
 rqalpha/examples/data_source/import_get_csv_module.py
 rqalpha/examples/data_source/read_csv_as_df.py
 rqalpha/examples/extend_api/rqalpha_mod_extend_api_demo.py
 rqalpha/examples/extend_api/test_extend_api.py
 rqalpha/mod/__init__.py
 rqalpha/mod/utils.py
 rqalpha/mod/rqalpha_mod_sys_accounts/__init__.py
+rqalpha/mod/rqalpha_mod_sys_accounts/component_validator.py
 rqalpha/mod/rqalpha_mod_sys_accounts/mod.py
 rqalpha/mod/rqalpha_mod_sys_accounts/position_model.py
 rqalpha/mod/rqalpha_mod_sys_accounts/position_validator.py
+rqalpha/mod/rqalpha_mod_sys_accounts/validator.py
 rqalpha/mod/rqalpha_mod_sys_accounts/api/__init__.py
 rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py
 rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py
 rqalpha/mod/rqalpha_mod_sys_analyser/__init__.py
 rqalpha/mod/rqalpha_mod_sys_analyser/mod.py
 rqalpha/mod/rqalpha_mod_sys_analyser/plot_store.py
 rqalpha/mod/rqalpha_mod_sys_analyser/plot/__init__.py
@@ -107,14 +109,15 @@
 rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py
 rqalpha/mod/rqalpha_mod_sys_simulation/mod.py
 rqalpha/mod/rqalpha_mod_sys_simulation/signal_broker.py
 rqalpha/mod/rqalpha_mod_sys_simulation/simulation_broker.py
 rqalpha/mod/rqalpha_mod_sys_simulation/simulation_event_source.py
 rqalpha/mod/rqalpha_mod_sys_simulation/slippage.py
 rqalpha/mod/rqalpha_mod_sys_simulation/testing.py
+rqalpha/mod/rqalpha_mod_sys_simulation/validator.py
 rqalpha/mod/rqalpha_mod_sys_transaction_cost/__init__.py
 rqalpha/mod/rqalpha_mod_sys_transaction_cost/deciders.py
 rqalpha/mod/rqalpha_mod_sys_transaction_cost/mod.py
 rqalpha/model/__init__.py
 rqalpha/model/bar.py
 rqalpha/model/instrument.py
 rqalpha/model/order.py
@@ -170,23 +173,27 @@
 tests/api_tests/test_api_future.py
 tests/api_tests/test_api_stock.py
 tests/api_tests/test_config.py
 tests/api_tests/utils.py
 tests/api_tests/mod/__init__.py
 tests/api_tests/mod/sys_accounts/__init__.py
 tests/api_tests/mod/sys_accounts/test_account_model.py
+tests/api_tests/mod/sys_accounts/test_futures_settlement_price_type.py
+tests/api_tests/mod/sys_accounts/test_margin_stocks.py
 tests/api_tests/mod/sys_accounts/test_position_models.py
 tests/api_tests/mod/sys_scheduler/__init__.py
 tests/api_tests/mod/sys_scheduler/test_physical_time.py
 tests/api_tests/mod/sys_scheduler/test_scheduler.py
 tests/api_tests/mod/sys_simulation/__init__.py
 tests/api_tests/mod/sys_simulation/test_management_fee.py
 tests/api_tests/mod/sys_simulation/test_signal_broker.py
 tests/api_tests/mod/sys_simulation/test_simulation_broker.py
 tests/api_tests/mod/sys_simulation/test_simulation_event_source.py
+tests/api_tests/mod/sys_transaction_cost/__init__.py
+tests/api_tests/mod/sys_transaction_cost/test_commission_multiplier.py
 tests/unittest/__init__.py
 tests/unittest/test_data/__init__.py
 tests/unittest/test_data/test_instrument_mixin.py
 tests/unittest/test_data/test_trading_dates_mixin.py
 tests/unittest/test_mod/__init__.py
 tests/unittest/test_mod/test_sys_simulation/__init__.py
 tests/unittest/test_mod/test_sys_simulation/test_simulation_event_source.py
```

### Comparing `rqalpha-4.9.2/setup.py` & `rqalpha-5.0.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,18 +23,19 @@
     'six',
     'logbook',
     'click >=7.0.0',
     'jsonpickle',
     'simplejson',
     'PyYAML',
     'tabulate',
-    'rqrisk >=1.0.0',
+    'rqrisk >=1.0.6',
     'h5py',
-    'matplotlib >=2.2.0',
-    "openpyxl"
+    'matplotlib >=3.1.0',
+    "openpyxl",
+    "methodtools"
 ]
 
 if sys.version_info < (3, 5):
     requirements.append('typing')
 
 if sys.version_info.major == 2 and sys.version_info.minor == 7:
     requirements.extend([
@@ -49,25 +50,25 @@
     version=versioneer.get_version(),
     cmdclass=versioneer.get_cmdclass(),
     description='Ricequant Algorithm Trading System',
     packages=find_packages(exclude=[]),
     author='ricequant',
     author_email='public@ricequant.com',
     license='Apache License v2',
-    include_package_date=True,
+    include_package_data=True,
     package_data={
         'rqalpha': ['*.yml',
                     'examples/*.*', 'examples/data_source/*.*', 'examples/extend_api/*.*',
                     'resource/*.*', 'utils/translations/zh_Hans_CN/LC_MESSAGES/*',
                     "mod/rqalpha_mod_sys_analyser/report/templates/*.xlsx",
                     ],
     },
     url='https://github.com/ricequant/rqalpha',
     install_requires=requirements,
-    extra_requires={
+    extras_require={
         'profiler': ["line_profiler"],
     },
     zip_safe=False,
     entry_points={
         "console_scripts": [
             "rqalpha = rqalpha.__main__:entry_point"
         ]
```

### Comparing `rqalpha-4.9.2/tests/__init__.py` & `rqalpha-5.0.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/tests/api_tests/__init__.py` & `rqalpha-5.0.0/tests/api_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/tests/api_tests/mod/__init__.py` & `rqalpha-5.0.0/tests/api_tests/mod/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/tests/api_tests/mod/sys_accounts/__init__.py` & `rqalpha-5.0.0/tests/api_tests/mod/sys_accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/tests/api_tests/mod/sys_accounts/test_account_model.py` & `rqalpha-5.0.0/tests/api_tests/mod/sys_accounts/test_account_model.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/tests/api_tests/mod/sys_accounts/test_position_models.py` & `rqalpha-5.0.0/tests/api_tests/mod/sys_accounts/test_position_models.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/tests/api_tests/mod/sys_scheduler/test_physical_time.py` & `rqalpha-5.0.0/tests/unittest/test_data/test_trading_dates_mixin.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,52 +1,27 @@
 # -*- coding: utf-8 -*-
 # 版权所有 2019 深圳米筐科技有限公司（下称“米筐科技”）
 #
 # 除非遵守当前许可，否则不得使用本软件。
 #
 #     * 非商业用途（非商业用途指个人出于非商业目的使用本软件，或者高校、研究所等非营利机构出于教育、科研等目的使用本软件）：
-#         遵守 Apache License 2.0（下称“Apache 2.0 许可”），
-#         您可以在以下位置获得 Apache 2.0 许可的副本：http://www.apache.org/licenses/LICENSE-2.0。
+#         遵守 Apache License 2.0（下称“Apache 2.0 许可”），您可以在以下位置获得 Apache 2.0 许可的副本：http://www.apache.org/licenses/LICENSE-2.0。
 #         除非法律有要求或以书面形式达成协议，否则本软件分发时需保持当前许可“原样”不变，且不得附加任何条件。
 #
 #     * 商业用途（商业用途指个人出于任何商业目的使用本软件，或者法人或其他组织出于任何目的使用本软件）：
-#         未经米筐科技授权，任何个人不得出于任何商业目的使用本软件（包括但不限于向第三方提供、销售、出租、出借、转让本软件、
-#         本软件的衍生产品、引用或借鉴了本软件功能或源代码的产品或服务），任何法人或其他组织不得出于任何目的使用本软件，
-#         否则米筐科技有权追究相应的知识产权侵权责任。
+#         未经米筐科技授权，任何个人不得出于任何商业目的使用本软件（包括但不限于向第三方提供、销售、出租、出借、转让本软件、本软件的衍生产品、引用或借鉴了本软件功能或源代码的产品或服务），任何法人或其他组织不得出于任何目的使用本软件，否则米筐科技有权追究相应的知识产权侵权责任。
 #         在此前提下，对本软件的使用同样需要遵守 Apache 2.0 许可，Apache 2.0 许可与本许可冲突之处，以本许可为准。
 #         详细的授权流程，请联系 public@ricequant.com 获取。
 
+from rqalpha.utils.testing import DataProxyFixture, RQAlphaTestCase
 
-__config__ = {
-    "base": {
-        "start_date": "2015-01-01",
-        "end_date": "2015-12-31",
-        "frequency": "1d",
-        "accounts": {
-            "future": 1000000,
-        }
-    },
-    "extra": {
-        "log_level": "error",
-    },
-}
 
+class TradingDateMixinTestCase(DataProxyFixture, RQAlphaTestCase):
+    def init_fixture(self):
+        super(TradingDateMixinTestCase, self).init_fixture()
 
-def test_physical_time():
-    """
-    测试 physical_time 的使用
-    """
-    from rqalpha.mod.rqalpha_mod_sys_scheduler.scheduler import physical_time
+    def test_count_trading_dates(self):
+        from datetime import date
 
-    def _day(context, bar_dict):
-        context.counter += 1
-
-    def init(context):
-        context.counter = 0
-        scheduler.run_daily(_day, time_rule=physical_time(hour=9, minute=31))
-        context.days = 0
-
-    def handle_bar(context, bar_dict):
-        context.days += 1
-        assert context.counter == context.days
-
-    return locals()
+        assert self.data_proxy.count_trading_dates(date(2018, 11, 1), date(2018, 11, 12)) == 8
+        assert self.data_proxy.count_trading_dates(date(2018, 11, 3), date(2018, 11, 12)) == 6
+        assert self.data_proxy.count_trading_dates(date(2018, 11, 3), date(2018, 11, 18)) == 10
```

### Comparing `rqalpha-4.9.2/tests/api_tests/mod/sys_scheduler/test_scheduler.py` & `rqalpha-5.0.0/tests/api_tests/mod/sys_scheduler/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/tests/api_tests/mod/sys_simulation/__init__.py` & `rqalpha-5.0.0/tests/api_tests/mod/sys_simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/tests/api_tests/mod/sys_simulation/test_management_fee.py` & `rqalpha-5.0.0/tests/api_tests/mod/sys_simulation/test_management_fee.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/tests/api_tests/mod/sys_simulation/test_signal_broker.py` & `rqalpha-5.0.0/tests/api_tests/mod/sys_simulation/test_signal_broker.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/tests/api_tests/mod/sys_simulation/test_simulation_broker.py` & `rqalpha-5.0.0/tests/api_tests/mod/sys_simulation/test_simulation_broker.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/tests/api_tests/mod/sys_simulation/test_simulation_event_source.py` & `rqalpha-5.0.0/tests/api_tests/mod/sys_simulation/test_simulation_event_source.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/tests/api_tests/test_api_base.py` & `rqalpha-5.0.0/tests/api_tests/test_api_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -478,8 +478,14 @@
             try:
                 flag = withdraw("FUTURE", 100000000)
             except ValueError as err:
                 assert True, "捕获输入异常"
             else:
                 assert False, "未报出当前账户可取出金额不足异常"
 
+            deposit("STOCK", 10000, 3)
+            context.cash = context.portfolio.accounts["STOCK"].cash
+
+        elif context.counter == 9:
+            assert int(context.portfolio.accounts["STOCK"].cash) == int(context.cash) + 10000
+
     return locals()
```

### Comparing `rqalpha-4.9.2/tests/api_tests/test_api_future.py` & `rqalpha-5.0.0/tests/api_tests/test_api_future.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/tests/api_tests/test_api_stock.py` & `rqalpha-5.0.0/tests/api_tests/test_api_stock.py`

 * *Files 10% similar despite different names*

```diff
@@ -151,31 +151,37 @@
             }
         },
     }
 
     def init(context):
         context.counter = 0
 
-    def handle_bar(context, handle_bar):
+    def handle_bar(context, bar_dict):
         context.counter += 1
         if context.counter == 1:
             order_target_portfolio({
                 "000001.XSHE": 0.1,
                 "000004.XSHE": 0.2,
             })
             assert get_position("000001.XSHE").quantity == 6900   # (1000000 * 0.1) / 14.37 = 6958.94
             assert get_position("000004.XSHE").quantity == 10500  # (1000000 * 0.2) / 18.92 = 10570.82
         elif context.counter == 2:
             order_target_portfolio({
                 "000004.XSHE": 0.1,
-                "000005.XSHE": 0.2
+                "000005.XSHE": 0.2,
+                "600519.XSHG": 0.6,
+            }, {
+                "000004.XSHE": (18.5, 18),
+                "000005.XSHE": (2.92, ),
+                "600519.XSHG": (970, 980),
             })
-            assert get_position("000001.XSHE").quantity == 0
-            assert get_position("000004.XSHE").quantity == 5400   # (993695.7496 * 0.1) / 18.50 = 5371.33
+            assert get_position("000001.XSHE").quantity == 0  # 清仓
+            assert get_position("000004.XSHE").quantity == 5600  # (993695.7496 * 0.1) / 18 = 5520.53
             assert get_position("000005.XSHE").quantity == 68000  # (993695.7496 * 0.2) / 2.92 = 68061.35
+            assert get_position("600519.XSHG").quantity == 0  # 970 低于 收盘价 无法买进
 
     return locals()
 
 
 def test_order_target_portfolio_in_signal_mode():
     __config__ = {
         "base": {
@@ -195,16 +201,19 @@
     def init(context):
         context.counter = 0
 
     def handle_bar(context, handle_bar):
         context.counter += 1
         if context.counter == 1:
             order_target_portfolio({
-                "000001.XSHE": (0.1, 14),
-                "000004.XSHE": (0.2, 10),
+                "000001.XSHE": 0.1,
+                "000004.XSHE": 0.2,
+            }, {
+                "000001.XSHE": 14,
+                "000004.XSHE": 10,
             })
             assert get_position("000001.XSHE").quantity == 7100   # (1000000 * 0.1) / 14.37 = 7142.86
             assert get_position("000004.XSHE").quantity == 0  # 价格低过跌停价，被拒单
 
     return locals()
 
 
@@ -263,7 +272,53 @@
             # 5 块最小手续费
             order_value(context.s1, context.amount_s1 * order_price_s1 + 5, order_price_s1)
             order_value(context.s2, context.amount_s2 * order_price_s2 + 5, order_price_s2)
             assert context.portfolio.positions[context.s1].quantity == 201
             assert context.portfolio.positions[context.s2].quantity == 0
 
     return locals()
+
+
+def test_finance_repay():
+    """ 测试融资还款接口 """
+
+    financing_rate = 0.1
+    money = 10000
+
+    __config__ = {
+        "base": {
+            "start_date": "2016-01-01",
+            "end_date": "2016-01-31"
+        },
+        "mod": {
+            "sys_accounts": {
+                "financing_rate": financing_rate,
+            }
+        }
+    }
+
+    def cal_interest(capital, days):
+        for i in range(days):
+            capital += capital * financing_rate / 365
+        return capital
+
+    def init(context):
+        context.fixed = True
+        context.total = 0
+
+    def handle_bar(context, bar_dict):
+        if context.fixed:
+            finance(money)
+            context.fixed = False
+
+        if context.total == 5:
+            assert context.stock_account.cash_liabilities == cal_interest(money, 5)
+        elif context.total == 10:
+            assert context.stock_account.cash_liabilities == cal_interest(money, 10)
+            repay(10100)
+        elif context.total == 11:
+            assert context.stock_account.total_value == 99999972.5689376
+            assert context.stock_account.cash_liabilities == 0
+
+        context.total += 1
+
+    return locals()
```

### Comparing `rqalpha-4.9.2/tests/api_tests/test_config.py` & `rqalpha-5.0.0/tests/api_tests/test_config.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/tests/test_f_buy_and_hold.py` & `rqalpha-5.0.0/tests/test_f_buy_and_hold.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/tests/test_f_macd.py` & `rqalpha-5.0.0/tests/test_f_macd.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/tests/test_f_macd_signal.py` & `rqalpha-5.0.0/tests/test_f_macd_signal.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/tests/test_f_mean_reverting.py` & `rqalpha-5.0.0/tests/test_f_mean_reverting.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/tests/test_s_buy_and_hold.py` & `rqalpha-5.0.0/tests/test_s_buy_and_hold.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/tests/test_s_dual_thrust.py` & `rqalpha-5.0.0/tests/test_s_dual_thrust.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/tests/test_s_scheduler.py` & `rqalpha-5.0.0/tests/test_s_scheduler.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/tests/test_s_tick_size.py` & `rqalpha-5.0.0/tests/test_s_tick_size.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/tests/test_s_turtle.py` & `rqalpha-5.0.0/tests/test_s_turtle.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/tests/test_s_turtle_signal.py` & `rqalpha-5.0.0/tests/test_s_turtle_signal.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/tests/test_sf_buy_and_hold.py` & `rqalpha-5.0.0/tests/test_sf_buy_and_hold.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/tests/unittest/__init__.py` & `rqalpha-5.0.0/tests/unittest/test_mod/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,22 +10,12 @@
 #     * 商业用途（商业用途指个人出于任何商业目的使用本软件，或者法人或其他组织出于任何目的使用本软件）：
 #         未经米筐科技授权，任何个人不得出于任何商业目的使用本软件（包括但不限于向第三方提供、销售、出租、出借、转让本软件、本软件的衍生产品、引用或借鉴了本软件功能或源代码的产品或服务），任何法人或其他组织不得出于任何目的使用本软件，否则米筐科技有权追究相应的知识产权侵权责任。
 #         在此前提下，对本软件的使用同样需要遵守 Apache 2.0 许可，Apache 2.0 许可与本许可冲突之处，以本许可为准。
 #         详细的授权流程，请联系 public@ricequant.com 获取。
 
 import os
 
-from unittest import TestLoader, TestSuite, TextTestRunner
 
-
-def load_tests():
-    test_suite = TestSuite()
+def load_tests(loader, standard_tests, pattern):
     this_dir = os.path.dirname(__file__)
-    loader = TestLoader()
-    package_tests = loader.discover(start_dir=this_dir)
-    test_suite.addTests(package_tests)
-    return test_suite
-
-
-if __name__ == "__main__":
-    runner = TextTestRunner(verbosity=2)
-    runner.run(load_tests())
+    standard_tests.addTests(loader.discover(start_dir=this_dir, pattern=pattern))
+    return standard_tests
```

### Comparing `rqalpha-4.9.2/tests/unittest/test_data/test_instrument_mixin.py` & `rqalpha-5.0.0/tests/unittest/test_data/test_instrument_mixin.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/tests/unittest/test_mod/__init__.py` & `rqalpha-5.0.0/tests/unittest/test_mod/test_sys_simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/tests/unittest/test_mod/test_sys_simulation/__init__.py` & `rqalpha-5.0.0/tests/api_tests/mod/sys_accounts/test_futures_settlement_price_type.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,14 +8,48 @@
 #         除非法律有要求或以书面形式达成协议，否则本软件分发时需保持当前许可“原样”不变，且不得附加任何条件。
 #
 #     * 商业用途（商业用途指个人出于任何商业目的使用本软件，或者法人或其他组织出于任何目的使用本软件）：
 #         未经米筐科技授权，任何个人不得出于任何商业目的使用本软件（包括但不限于向第三方提供、销售、出租、出借、转让本软件、本软件的衍生产品、引用或借鉴了本软件功能或源代码的产品或服务），任何法人或其他组织不得出于任何目的使用本软件，否则米筐科技有权追究相应的知识产权侵权责任。
 #         在此前提下，对本软件的使用同样需要遵守 Apache 2.0 许可，Apache 2.0 许可与本许可冲突之处，以本许可为准。
 #         详细的授权流程，请联系 public@ricequant.com 获取。
 
-import os
+from rqalpha.apis import *
 
+__config__ = {
+    "base": {
+        "start_date": "2016-01-01",
+        "end_date": "2016-01-31",
+        "frequency": "1d",
+        "accounts": {
+            "future": 1000000,
+        }
+    },
+    "mod": {
+        "sys_accounts": {
+            "futures_settlement_price_type": "settlement"
+        }
+    }
+}
+
+
+def test_futures_settlement_price_type():
+
+    def init(context):
+        context.fixed = True
+        context.symbol = "IC1603"
+        context.total = 0
+
+    def handle_bar(context, bar_dict):
+        if context.fixed:
+            buy_open(context.symbol, 1)
+            context.fixed = False
+        context.total += 1
+
+    def after_trading(context):
+        pos = get_position(context.symbol)
+        # close - prev_settlement
+        if context.total == 2:
+            assert pos.position_pnl == (6364.6 - 6657.0) * 200
+        elif context.total == 3:
+            assert pos.position_pnl == (6468 - 6351.2) * 200
+    return locals()
 
-def load_tests(loader, standard_tests, pattern):
-    this_dir = os.path.dirname(__file__)
-    standard_tests.addTests(loader.discover(start_dir=this_dir, pattern=pattern))
-    return standard_tests
```

### Comparing `rqalpha-4.9.2/tests/unittest/test_mod/test_sys_simulation/test_simulation_event_source.py` & `rqalpha-5.0.0/tests/unittest/test_mod/test_sys_simulation/test_simulation_event_source.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,19 +57,14 @@
 
             self.env.update_universe({"AU1812", "TF1812"})
             self.assertEvent(
                 next(events), EVENT.BEFORE_TRADING,
                 datetime(2018, 9, 13, 20, 29, 0, 500000), datetime(2018, 9, 14, 20, 29, 0, 500000)
             )
 
-            self.assertEvent(
-                next(events), EVENT.OPEN_AUCTION,
-                datetime(2018, 9, 13, 20, 56, 0, 500000), datetime(2018, 9, 14, 20, 56, 0, 500000)
-            )
-
             self.env.update_universe({"TF1812"})
             self.assertEvent(
                 next(events), EVENT.TICK,
                 datetime(2018, 9, 14, 9, 14, 0, 400000), datetime(2018, 9, 14, 9, 14, 0, 400000),
                 tick={"order_book_id": "TF1812"}
             )
```

### Comparing `rqalpha-4.9.2/tests/utils.py` & `rqalpha-5.0.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.2/versioneer.py` & `rqalpha-5.0.0/versioneer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1423,16 +1423,17 @@
             rendered += ".dirty"
 
     tracking_branch = git_tracking_branch()
     # # 如果是dev和master分支或者hotfix分支来的，或者是一个tag，那就用pep440的版本号，否则带上git commit id
     if tracking_branch in ["origin/develop", "origin/master"] or tracking_branch.startswith("origin/hotfix/") or pieces[
         "distance"] == 0:
         return rendered
-
-    return rendered
+    else:
+        rendered += "+g{}".format(pieces["short"])
+        return rendered
 
 
 def render_pep440_old(pieces):
     """TAG[.postDISTANCE[.dev0]] .
 
     The ".dev0" means dirty.
```

