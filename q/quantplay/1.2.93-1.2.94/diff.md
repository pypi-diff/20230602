# Comparing `tmp/quantplay-1.2.93.tar.gz` & `tmp/quantplay-1.2.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantplay-1.2.93.tar", last modified: Fri Jun  2 03:04:24 2023, max compression
+gzip compressed data, was "quantplay-1.2.94.tar", last modified: Fri Jun  2 03:09:04 2023, max compression
```

## Comparing `quantplay-1.2.93.tar` & `quantplay-1.2.94.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:04:24.309062 quantplay-1.2.93/
--rw-r--r--   0 ashok      (502) staff       (20)      663 2023-06-02 03:04:24.309123 quantplay-1.2.93/PKG-INFO
--rw-r--r--   0 ashok      (502) staff       (20)      494 2023-04-19 06:36:45.000000 quantplay-1.2.93/README.md
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:04:24.298179 quantplay-1.2.93/quantplay/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:04:24.298956 quantplay-1.2.93/quantplay/backtest/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/backtest/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    17605 2023-05-17 07:17:28.000000 quantplay-1.2.93/quantplay/backtest/backtest_trades.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:04:24.300400 quantplay-1.2.93/quantplay/broker/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/broker/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    10902 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/broker/angelone.py
--rw-r--r--   0 ashok      (502) staff       (20)     3738 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/broker/broker_client.py
--rw-r--r--   0 ashok      (502) staff       (20)       87 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/broker/client.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:04:24.300635 quantplay-1.2.93/quantplay/broker/finvasia_utils/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/broker/finvasia_utils/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     2576 2023-05-11 13:49:53.000000 quantplay-1.2.93/quantplay/broker/finvasia_utils/shoonya.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:04:24.300861 quantplay-1.2.93/quantplay/broker/generics/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/broker/generics/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    28802 2023-05-26 07:56:12.000000 quantplay-1.2.93/quantplay/broker/generics/broker.py
--rw-r--r--   0 ashok      (502) staff       (20)     3897 2023-05-17 07:17:28.000000 quantplay-1.2.93/quantplay/broker/iifl.py
--rw-r--r--   0 ashok      (502) staff       (20)      588 2023-06-01 01:35:25.000000 quantplay-1.2.93/quantplay/broker/iifl_xts.py
--rw-r--r--   0 ashok      (502) staff       (20)     2002 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/broker/kite_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)    31836 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/broker/motilal.py
--rw-r--r--   0 ashok      (502) staff       (20)    19618 2023-05-11 13:57:44.000000 quantplay-1.2.93/quantplay/broker/shoonya.py
--rw-r--r--   0 ashok      (502) staff       (20)      515 2023-04-19 06:37:00.000000 quantplay-1.2.93/quantplay/broker/symphony.py
--rw-r--r--   0 ashok      (502) staff       (20)    19148 2023-06-02 03:04:08.000000 quantplay-1.2.93/quantplay/broker/xts.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:04:24.301514 quantplay-1.2.93/quantplay/broker/xts_utils/
--rw-r--r--   0 ashok      (502) staff       (20)    33446 2023-04-24 08:10:10.000000 quantplay-1.2.93/quantplay/broker/xts_utils/Connect.py
--rw-r--r--   0 ashok      (502) staff       (20)     3046 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/broker/xts_utils/Exception.py
--rw-r--r--   0 ashok      (502) staff       (20)     6456 2023-06-02 03:04:08.000000 quantplay-1.2.93/quantplay/broker/xts_utils/InteractiveSocketClient.py
--rw-r--r--   0 ashok      (502) staff       (20)     9106 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/broker/xts_utils/MarketDataSocketClient.py
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/broker/xts_utils/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    17192 2023-05-23 09:41:25.000000 quantplay-1.2.93/quantplay/broker/zerodha.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:04:24.301612 quantplay-1.2.93/quantplay/brokerage/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/brokerage/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:04:24.301816 quantplay-1.2.93/quantplay/brokerage/angelone/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/brokerage/angelone/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    10989 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/brokerage/angelone/angel_broker.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:04:24.302329 quantplay-1.2.93/quantplay/brokerage/generics/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/brokerage/generics/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    28081 2023-04-26 18:39:03.000000 quantplay-1.2.93/quantplay/brokerage/generics/broker.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:04:24.302766 quantplay-1.2.93/quantplay/brokerage/zerodha/
--rw-r--r--   0 ashok      (502) staff       (20)    17690 2023-04-24 06:31:05.000000 quantplay-1.2.93/quantplay/brokerage/zerodha/ZBroker.py
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/brokerage/zerodha/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:04:24.302989 quantplay-1.2.93/quantplay/config/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/config/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     1461 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/config/qplay_config.py
--rw-r--r--   0 ashok      (502) staff       (20)     1127 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/create_sample_data.py
--rw-r--r--   0 ashok      (502) staff       (20)     1725 2023-04-19 06:37:00.000000 quantplay-1.2.93/quantplay/data_modify_script.py
--rw-r--r--   0 ashok      (502) staff       (20)     3481 2023-04-19 06:37:00.000000 quantplay-1.2.93/quantplay/date_fix.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:04:24.303238 quantplay-1.2.93/quantplay/exception/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/exception/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     2162 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/exception/exceptions.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:04:24.303488 quantplay-1.2.93/quantplay/executor/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/executor/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     6064 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/executor/strategy_executor.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:04:24.303831 quantplay-1.2.93/quantplay/indicators/
--rw-r--r--   0 ashok      (502) staff       (20)     1747 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/indicators/Indicator.py
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/indicators/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      455 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/indicators/atr.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:04:24.303960 quantplay-1.2.93/quantplay/model/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/model/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:04:24.304467 quantplay-1.2.93/quantplay/model/exchange/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/model/exchange/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     1472 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/model/exchange/instrument.py
--rw-r--r--   0 ashok      (502) staff       (20)     8794 2023-05-17 08:03:33.000000 quantplay-1.2.93/quantplay/model/exchange/order.py
--rw-r--r--   0 ashok      (502) staff       (20)     3238 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/model/exchange/tick.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:04:24.304678 quantplay-1.2.93/quantplay/model/strategy/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/model/strategy/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      206 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/model/strategy/strategy_response.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:04:24.304791 quantplay-1.2.93/quantplay/oms/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/oms/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:04:24.305122 quantplay-1.2.93/quantplay/order_execution/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/order_execution/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     2048 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/order_execution/execution_algorithm.py
--rw-r--r--   0 ashok      (502) staff       (20)     1281 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/order_execution/mean_price.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:04:24.305424 quantplay-1.2.93/quantplay/reporting/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/reporting/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    10780 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/reporting/strategy_report.py
--rw-r--r--   0 ashok      (502) staff       (20)     1521 2023-04-19 06:37:00.000000 quantplay-1.2.93/quantplay/reporting/visuals.py
--rw-r--r--   0 ashok      (502) staff       (20)      231 2023-04-24 06:31:05.000000 quantplay-1.2.93/quantplay/service.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:04:24.305770 quantplay-1.2.93/quantplay/services/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/services/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    18366 2023-05-26 07:55:13.000000 quantplay-1.2.93/quantplay/services/market.py
--rw-r--r--   0 ashok      (502) staff       (20)    11801 2023-05-31 03:18:14.000000 quantplay-1.2.93/quantplay/services/tradelens.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:04:24.305878 quantplay-1.2.93/quantplay/strategies/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:35:41.000000 quantplay-1.2.93/quantplay/strategies/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:04:24.305967 quantplay-1.2.93/quantplay/strategies/equities/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:48:09.000000 quantplay-1.2.93/quantplay/strategies/equities/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:04:24.306054 quantplay-1.2.93/quantplay/strategies/equities/intraday/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:48:26.000000 quantplay-1.2.93/quantplay/strategies/equities/intraday/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:04:24.306148 quantplay-1.2.93/quantplay/strategies/equities/overnight/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:49:47.000000 quantplay-1.2.93/quantplay/strategies/equities/overnight/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:04:24.306234 quantplay-1.2.93/quantplay/strategies/futures/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-24 08:54:42.000000 quantplay-1.2.93/quantplay/strategies/futures/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:04:24.306321 quantplay-1.2.93/quantplay/strategies/futures/overnight/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-24 08:54:48.000000 quantplay-1.2.93/quantplay/strategies/futures/overnight/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:04:24.306407 quantplay-1.2.93/quantplay/strategies/options/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:35:52.000000 quantplay-1.2.93/quantplay/strategies/options/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:04:24.306855 quantplay-1.2.93/quantplay/strategies/options/intraday/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:36:03.000000 quantplay-1.2.93/quantplay/strategies/options/intraday/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     1958 2022-09-14 18:05:01.000000 quantplay-1.2.93/quantplay/strategies/options/intraday/ladder.py
--rw-r--r--   0 ashok      (502) staff       (20)     2675 2022-06-25 11:41:44.000000 quantplay-1.2.93/quantplay/strategies/options/intraday/musk.py
--rw-r--r--   0 ashok      (502) staff       (20)      403 2022-09-17 07:36:48.000000 quantplay-1.2.93/quantplay/strategies/options/intraday/short_straddle.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:04:24.307071 quantplay-1.2.93/quantplay/strategy/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/strategy/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    12759 2023-05-17 07:17:28.000000 quantplay-1.2.93/quantplay/strategy/base.py
--rw-r--r--   0 ashok      (502) staff       (20)      214 2022-06-28 09:52:29.000000 quantplay-1.2.93/quantplay/strategy_run.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:04:24.308049 quantplay-1.2.93/quantplay/utils/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/utils/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      723 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/utils/config_util.py
--rw-r--r--   0 ashok      (502) staff       (20)    24181 2023-04-24 06:31:05.000000 quantplay-1.2.93/quantplay/utils/constant.py
--rw-r--r--   0 ashok      (502) staff       (20)     5433 2023-04-19 06:37:00.000000 quantplay-1.2.93/quantplay/utils/data_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)      711 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/utils/exchange.py
--rw-r--r--   0 ashok      (502) staff       (20)      517 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/utils/number_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)      458 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/utils/pickle_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)     1181 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/utils/selenium_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)     4094 2023-04-19 06:36:45.000000 quantplay-1.2.93/quantplay/utils/transaction_utils.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:04:24.298750 quantplay-1.2.93/quantplay.egg-info/
--rw-r--r--   0 ashok      (502) staff       (20)      663 2023-06-02 03:04:24.000000 quantplay-1.2.93/quantplay.egg-info/PKG-INFO
--rw-r--r--   0 ashok      (502) staff       (20)     3391 2023-06-02 03:04:24.000000 quantplay-1.2.93/quantplay.egg-info/SOURCES.txt
--rw-r--r--   0 ashok      (502) staff       (20)        1 2023-06-02 03:04:24.000000 quantplay-1.2.93/quantplay.egg-info/dependency_links.txt
--rw-r--r--   0 ashok      (502) staff       (20)      221 2023-06-02 03:04:24.000000 quantplay-1.2.93/quantplay.egg-info/requires.txt
--rw-r--r--   0 ashok      (502) staff       (20)       15 2023-06-02 03:04:24.000000 quantplay-1.2.93/quantplay.egg-info/top_level.txt
--rw-r--r--   0 ashok      (502) staff       (20)       49 2023-06-02 03:04:24.309322 quantplay-1.2.93/setup.cfg
--rw-r--r--   0 ashok      (502) staff       (20)      876 2023-06-02 03:04:22.000000 quantplay-1.2.93/setup.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:04:24.308250 quantplay-1.2.93/test/
--rw-------   0 ashok      (502) staff       (20)        0 2022-04-15 16:22:35.000000 quantplay-1.2.93/test/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:04:24.308445 quantplay-1.2.93/test/broker/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.93/test/broker/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      220 2023-04-19 06:36:45.000000 quantplay-1.2.93/test/broker/finvasia.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:04:24.308659 quantplay-1.2.93/test/executor/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.93/test/executor/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      304 2023-04-19 06:36:45.000000 quantplay-1.2.93/test/executor/strategy_executor.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:04:24.308959 quantplay-1.2.93/test/strategy/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.93/test/strategy/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      292 2023-04-19 06:36:45.000000 quantplay-1.2.93/test/strategy/base.py
--rw-r--r--   0 ashok      (502) staff       (20)     2194 2023-04-19 06:36:45.000000 quantplay-1.2.93/test/strategy/sample_strategy.py
--rw-r--r--   0 ashok      (502) staff       (20)     3302 2023-04-19 06:36:45.000000 quantplay-1.2.93/test/test_motilal.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.912576 quantplay-1.2.94/
+-rw-r--r--   0 ashok      (502) staff       (20)      663 2023-06-02 03:09:04.912633 quantplay-1.2.94/PKG-INFO
+-rw-r--r--   0 ashok      (502) staff       (20)      494 2023-04-19 06:36:45.000000 quantplay-1.2.94/README.md
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.901507 quantplay-1.2.94/quantplay/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.902347 quantplay-1.2.94/quantplay/backtest/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/backtest/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    17605 2023-05-17 07:17:28.000000 quantplay-1.2.94/quantplay/backtest/backtest_trades.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.904281 quantplay-1.2.94/quantplay/broker/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/broker/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    10902 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/broker/angelone.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3738 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/broker/broker_client.py
+-rw-r--r--   0 ashok      (502) staff       (20)       87 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/broker/client.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.904575 quantplay-1.2.94/quantplay/broker/finvasia_utils/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/broker/finvasia_utils/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2576 2023-05-11 13:49:53.000000 quantplay-1.2.94/quantplay/broker/finvasia_utils/shoonya.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.904823 quantplay-1.2.94/quantplay/broker/generics/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/broker/generics/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    28802 2023-05-26 07:56:12.000000 quantplay-1.2.94/quantplay/broker/generics/broker.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3897 2023-05-17 07:17:28.000000 quantplay-1.2.94/quantplay/broker/iifl.py
+-rw-r--r--   0 ashok      (502) staff       (20)      588 2023-06-01 01:35:25.000000 quantplay-1.2.94/quantplay/broker/iifl_xts.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2002 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/broker/kite_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)    31836 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/broker/motilal.py
+-rw-r--r--   0 ashok      (502) staff       (20)    19618 2023-05-11 13:57:44.000000 quantplay-1.2.94/quantplay/broker/shoonya.py
+-rw-r--r--   0 ashok      (502) staff       (20)      515 2023-04-19 06:37:00.000000 quantplay-1.2.94/quantplay/broker/symphony.py
+-rw-r--r--   0 ashok      (502) staff       (20)    19145 2023-06-02 03:08:35.000000 quantplay-1.2.94/quantplay/broker/xts.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.905582 quantplay-1.2.94/quantplay/broker/xts_utils/
+-rw-r--r--   0 ashok      (502) staff       (20)    33446 2023-04-24 08:10:10.000000 quantplay-1.2.94/quantplay/broker/xts_utils/Connect.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3046 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/broker/xts_utils/Exception.py
+-rw-r--r--   0 ashok      (502) staff       (20)     6456 2023-06-02 03:04:08.000000 quantplay-1.2.94/quantplay/broker/xts_utils/InteractiveSocketClient.py
+-rw-r--r--   0 ashok      (502) staff       (20)     9106 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/broker/xts_utils/MarketDataSocketClient.py
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/broker/xts_utils/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    17192 2023-05-23 09:41:25.000000 quantplay-1.2.94/quantplay/broker/zerodha.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.905700 quantplay-1.2.94/quantplay/brokerage/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/brokerage/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.905924 quantplay-1.2.94/quantplay/brokerage/angelone/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/brokerage/angelone/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    10989 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/brokerage/angelone/angel_broker.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.906136 quantplay-1.2.94/quantplay/brokerage/generics/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/brokerage/generics/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    28081 2023-04-26 18:39:03.000000 quantplay-1.2.94/quantplay/brokerage/generics/broker.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.906383 quantplay-1.2.94/quantplay/brokerage/zerodha/
+-rw-r--r--   0 ashok      (502) staff       (20)    17690 2023-04-24 06:31:05.000000 quantplay-1.2.94/quantplay/brokerage/zerodha/ZBroker.py
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/brokerage/zerodha/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.906568 quantplay-1.2.94/quantplay/config/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/config/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1461 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/config/qplay_config.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1127 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/create_sample_data.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1725 2023-04-19 06:37:00.000000 quantplay-1.2.94/quantplay/data_modify_script.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3481 2023-04-19 06:37:00.000000 quantplay-1.2.94/quantplay/date_fix.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.906766 quantplay-1.2.94/quantplay/exception/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/exception/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2162 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/exception/exceptions.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.906961 quantplay-1.2.94/quantplay/executor/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/executor/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     6064 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/executor/strategy_executor.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.907261 quantplay-1.2.94/quantplay/indicators/
+-rw-r--r--   0 ashok      (502) staff       (20)     1747 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/indicators/Indicator.py
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/indicators/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      455 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/indicators/atr.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.907367 quantplay-1.2.94/quantplay/model/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/model/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.907746 quantplay-1.2.94/quantplay/model/exchange/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/model/exchange/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1472 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/model/exchange/instrument.py
+-rw-r--r--   0 ashok      (502) staff       (20)     8794 2023-05-17 08:03:33.000000 quantplay-1.2.94/quantplay/model/exchange/order.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3238 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/model/exchange/tick.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.907963 quantplay-1.2.94/quantplay/model/strategy/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/model/strategy/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      206 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/model/strategy/strategy_response.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.908071 quantplay-1.2.94/quantplay/oms/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/oms/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.908368 quantplay-1.2.94/quantplay/order_execution/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/order_execution/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2048 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/order_execution/execution_algorithm.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1281 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/order_execution/mean_price.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.908663 quantplay-1.2.94/quantplay/reporting/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/reporting/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    10780 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/reporting/strategy_report.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1521 2023-04-19 06:37:00.000000 quantplay-1.2.94/quantplay/reporting/visuals.py
+-rw-r--r--   0 ashok      (502) staff       (20)      231 2023-04-24 06:31:05.000000 quantplay-1.2.94/quantplay/service.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.908991 quantplay-1.2.94/quantplay/services/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/services/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    18366 2023-05-26 07:55:13.000000 quantplay-1.2.94/quantplay/services/market.py
+-rw-r--r--   0 ashok      (502) staff       (20)    11801 2023-05-31 03:18:14.000000 quantplay-1.2.94/quantplay/services/tradelens.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.909103 quantplay-1.2.94/quantplay/strategies/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:35:41.000000 quantplay-1.2.94/quantplay/strategies/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.909198 quantplay-1.2.94/quantplay/strategies/equities/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:48:09.000000 quantplay-1.2.94/quantplay/strategies/equities/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.909299 quantplay-1.2.94/quantplay/strategies/equities/intraday/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:48:26.000000 quantplay-1.2.94/quantplay/strategies/equities/intraday/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.909388 quantplay-1.2.94/quantplay/strategies/equities/overnight/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:49:47.000000 quantplay-1.2.94/quantplay/strategies/equities/overnight/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.909495 quantplay-1.2.94/quantplay/strategies/futures/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-24 08:54:42.000000 quantplay-1.2.94/quantplay/strategies/futures/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.909591 quantplay-1.2.94/quantplay/strategies/futures/overnight/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-24 08:54:48.000000 quantplay-1.2.94/quantplay/strategies/futures/overnight/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.909679 quantplay-1.2.94/quantplay/strategies/options/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:35:52.000000 quantplay-1.2.94/quantplay/strategies/options/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.910121 quantplay-1.2.94/quantplay/strategies/options/intraday/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:36:03.000000 quantplay-1.2.94/quantplay/strategies/options/intraday/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1958 2022-09-14 18:05:01.000000 quantplay-1.2.94/quantplay/strategies/options/intraday/ladder.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2675 2022-06-25 11:41:44.000000 quantplay-1.2.94/quantplay/strategies/options/intraday/musk.py
+-rw-r--r--   0 ashok      (502) staff       (20)      403 2022-09-17 07:36:48.000000 quantplay-1.2.94/quantplay/strategies/options/intraday/short_straddle.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.910310 quantplay-1.2.94/quantplay/strategy/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/strategy/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    12759 2023-05-17 07:17:28.000000 quantplay-1.2.94/quantplay/strategy/base.py
+-rw-r--r--   0 ashok      (502) staff       (20)      214 2022-06-28 09:52:29.000000 quantplay-1.2.94/quantplay/strategy_run.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.911334 quantplay-1.2.94/quantplay/utils/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/utils/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      723 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/utils/config_util.py
+-rw-r--r--   0 ashok      (502) staff       (20)    24181 2023-04-24 06:31:05.000000 quantplay-1.2.94/quantplay/utils/constant.py
+-rw-r--r--   0 ashok      (502) staff       (20)     5433 2023-04-19 06:37:00.000000 quantplay-1.2.94/quantplay/utils/data_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)      711 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/utils/exchange.py
+-rw-r--r--   0 ashok      (502) staff       (20)      517 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/utils/number_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)      458 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/utils/pickle_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1181 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/utils/selenium_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)     4094 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/utils/transaction_utils.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.902116 quantplay-1.2.94/quantplay.egg-info/
+-rw-r--r--   0 ashok      (502) staff       (20)      663 2023-06-02 03:09:04.000000 quantplay-1.2.94/quantplay.egg-info/PKG-INFO
+-rw-r--r--   0 ashok      (502) staff       (20)     3391 2023-06-02 03:09:04.000000 quantplay-1.2.94/quantplay.egg-info/SOURCES.txt
+-rw-r--r--   0 ashok      (502) staff       (20)        1 2023-06-02 03:09:04.000000 quantplay-1.2.94/quantplay.egg-info/dependency_links.txt
+-rw-r--r--   0 ashok      (502) staff       (20)      221 2023-06-02 03:09:04.000000 quantplay-1.2.94/quantplay.egg-info/requires.txt
+-rw-r--r--   0 ashok      (502) staff       (20)       15 2023-06-02 03:09:04.000000 quantplay-1.2.94/quantplay.egg-info/top_level.txt
+-rw-r--r--   0 ashok      (502) staff       (20)       49 2023-06-02 03:09:04.912833 quantplay-1.2.94/setup.cfg
+-rw-r--r--   0 ashok      (502) staff       (20)      876 2023-06-02 03:09:02.000000 quantplay-1.2.94/setup.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.911550 quantplay-1.2.94/test/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-04-15 16:22:35.000000 quantplay-1.2.94/test/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.911775 quantplay-1.2.94/test/broker/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/test/broker/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      220 2023-04-19 06:36:45.000000 quantplay-1.2.94/test/broker/finvasia.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.912071 quantplay-1.2.94/test/executor/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/test/executor/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      304 2023-04-19 06:36:45.000000 quantplay-1.2.94/test/executor/strategy_executor.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.912450 quantplay-1.2.94/test/strategy/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/test/strategy/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      292 2023-04-19 06:36:45.000000 quantplay-1.2.94/test/strategy/base.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2194 2023-04-19 06:36:45.000000 quantplay-1.2.94/test/strategy/sample_strategy.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3302 2023-04-19 06:36:45.000000 quantplay-1.2.94/test/test_motilal.py
```

### Comparing `quantplay-1.2.93/PKG-INFO` & `quantplay-1.2.94/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantplay
-Version: 1.2.93
+Version: 1.2.94
 Summary: This python package will be stored in AWS CodeArtifact
 Home-page: 
 Author: 
 Author-email: 
 License: MIT
 
 # Quantplay Alpha playground
```

### Comparing `quantplay-1.2.93/quantplay/backtest/backtest_trades.py` & `quantplay-1.2.94/quantplay/backtest/backtest_trades.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/quantplay/broker/angelone.py` & `quantplay-1.2.94/quantplay/broker/angelone.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/quantplay/broker/broker_client.py` & `quantplay-1.2.94/quantplay/broker/broker_client.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/quantplay/broker/finvasia_utils/shoonya.py` & `quantplay-1.2.94/quantplay/broker/finvasia_utils/shoonya.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/quantplay/broker/generics/broker.py` & `quantplay-1.2.94/quantplay/broker/generics/broker.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/quantplay/broker/iifl.py` & `quantplay-1.2.94/quantplay/broker/iifl.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/quantplay/broker/iifl_xts.py` & `quantplay-1.2.94/quantplay/broker/iifl_xts.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/quantplay/broker/kite_utils.py` & `quantplay-1.2.94/quantplay/broker/kite_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/quantplay/broker/motilal.py` & `quantplay-1.2.94/quantplay/broker/motilal.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/quantplay/broker/shoonya.py` & `quantplay-1.2.94/quantplay/broker/shoonya.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/quantplay/broker/symphony.py` & `quantplay-1.2.94/quantplay/broker/symphony.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/quantplay/broker/xts.py` & `quantplay-1.2.94/quantplay/broker/xts.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,18 +102,19 @@
                     ).upper()
                     instrument["broker_symbol"] = f"{name} {expiry} FUT"
                 else:
                     instrument["broker_symbol"] = tradingsymbol
 
                 self.symbol_data["{}:{}".format(exchange, tradingsymbol)] = instrument
 
-            self.initialize_broker_symbol_map()
 
             PickleUtils.save_data(self.symbol_data, "xts_instruments")
             Constants.logger.info("[LOADING_INSTRUMENTS] loading data from server")
+        self.initialize_broker_symbol_map()
+
 
     def login(self):
         response_interact = self.wrapper.interactive_login()
         self.wrapper.marketdata_login()
 
         self.ClientID = response_interact["result"]["clientCodes"][0]
```

### Comparing `quantplay-1.2.93/quantplay/broker/xts_utils/Connect.py` & `quantplay-1.2.94/quantplay/broker/xts_utils/Connect.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/quantplay/broker/xts_utils/Exception.py` & `quantplay-1.2.94/quantplay/broker/xts_utils/Exception.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/quantplay/broker/xts_utils/InteractiveSocketClient.py` & `quantplay-1.2.94/quantplay/broker/xts_utils/InteractiveSocketClient.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/quantplay/broker/xts_utils/MarketDataSocketClient.py` & `quantplay-1.2.94/quantplay/broker/xts_utils/MarketDataSocketClient.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/quantplay/broker/zerodha.py` & `quantplay-1.2.94/quantplay/broker/zerodha.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/quantplay/brokerage/angelone/angel_broker.py` & `quantplay-1.2.94/quantplay/brokerage/angelone/angel_broker.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/quantplay/brokerage/generics/broker.py` & `quantplay-1.2.94/quantplay/brokerage/generics/broker.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/quantplay/brokerage/zerodha/ZBroker.py` & `quantplay-1.2.94/quantplay/brokerage/zerodha/ZBroker.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/quantplay/config/qplay_config.py` & `quantplay-1.2.94/quantplay/config/qplay_config.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/quantplay/create_sample_data.py` & `quantplay-1.2.94/quantplay/create_sample_data.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/quantplay/data_modify_script.py` & `quantplay-1.2.94/quantplay/data_modify_script.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/quantplay/date_fix.py` & `quantplay-1.2.94/quantplay/date_fix.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/quantplay/exception/exceptions.py` & `quantplay-1.2.94/quantplay/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/quantplay/executor/strategy_executor.py` & `quantplay-1.2.94/quantplay/executor/strategy_executor.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/quantplay/indicators/Indicator.py` & `quantplay-1.2.94/quantplay/indicators/Indicator.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/quantplay/model/exchange/instrument.py` & `quantplay-1.2.94/quantplay/model/exchange/instrument.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/quantplay/model/exchange/order.py` & `quantplay-1.2.94/quantplay/model/exchange/order.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/quantplay/model/exchange/tick.py` & `quantplay-1.2.94/quantplay/model/exchange/tick.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/quantplay/order_execution/execution_algorithm.py` & `quantplay-1.2.94/quantplay/order_execution/execution_algorithm.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/quantplay/order_execution/mean_price.py` & `quantplay-1.2.94/quantplay/order_execution/mean_price.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/quantplay/reporting/strategy_report.py` & `quantplay-1.2.94/quantplay/reporting/strategy_report.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/quantplay/reporting/visuals.py` & `quantplay-1.2.94/quantplay/reporting/visuals.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/quantplay/services/market.py` & `quantplay-1.2.94/quantplay/services/market.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/quantplay/services/tradelens.py` & `quantplay-1.2.94/quantplay/services/tradelens.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/quantplay/strategies/options/intraday/ladder.py` & `quantplay-1.2.94/quantplay/strategies/options/intraday/ladder.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/quantplay/strategies/options/intraday/musk.py` & `quantplay-1.2.94/quantplay/strategies/options/intraday/musk.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/quantplay/strategy/base.py` & `quantplay-1.2.94/quantplay/strategy/base.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/quantplay/utils/config_util.py` & `quantplay-1.2.94/quantplay/utils/config_util.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/quantplay/utils/constant.py` & `quantplay-1.2.94/quantplay/utils/constant.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/quantplay/utils/data_utils.py` & `quantplay-1.2.94/quantplay/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/quantplay/utils/exchange.py` & `quantplay-1.2.94/quantplay/utils/exchange.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/quantplay/utils/number_utils.py` & `quantplay-1.2.94/quantplay/utils/number_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/quantplay/utils/selenium_utils.py` & `quantplay-1.2.94/quantplay/utils/selenium_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/quantplay/utils/transaction_utils.py` & `quantplay-1.2.94/quantplay/utils/transaction_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/quantplay.egg-info/PKG-INFO` & `quantplay-1.2.94/quantplay.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantplay
-Version: 1.2.93
+Version: 1.2.94
 Summary: This python package will be stored in AWS CodeArtifact
 Home-page: 
 Author: 
 Author-email: 
 License: MIT
 
 # Quantplay Alpha playground
```

### Comparing `quantplay-1.2.93/quantplay.egg-info/SOURCES.txt` & `quantplay-1.2.94/quantplay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/setup.py` & `quantplay-1.2.94/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     for line in Path("requirements.txt").read_text().splitlines()
     if is_requirement(line)
 ]
 
 setup(
     name="quantplay",
     long_description=Path("README.md").read_text(),
-    version="1.2.93",
+    version="1.2.94",
     setup_requires=["pytest-runner"],
     install_requires=requirements,
     tests_require=[],
     packages=find_packages(),
     url="",
     license="MIT",
     author="",
```

### Comparing `quantplay-1.2.93/test/strategy/sample_strategy.py` & `quantplay-1.2.94/test/strategy/sample_strategy.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.93/test/test_motilal.py` & `quantplay-1.2.94/test/test_motilal.py`

 * *Files identical despite different names*

