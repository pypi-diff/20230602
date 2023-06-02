# Comparing `tmp/Finance-Jindowin-1.2.5.1.tar.gz` & `tmp/Finance-Jindowin-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Finance-Jindowin-1.2.5.1.tar", last modified: Fri Apr 14 15:45:44 2023, max compression
+gzip compressed data, was "dist/Finance-Jindowin-1.2.6.tar", last modified: Fri Jun  2 07:27:58 2023, max compression
```

## Comparing `Finance-Jindowin-1.2.5.1.tar` & `Finance-Jindowin-1.2.6.tar`

### file list

```diff
@@ -1,213 +1,224 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/Finance_Jindowin.egg-info/
--rw-r--r--   0 root         (0) root         (0)      170 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/Finance_Jindowin.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5486 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/Finance_Jindowin.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       74 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/Finance_Jindowin.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      243 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/Finance_Jindowin.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/Finance_Jindowin.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      114 2023-03-23 02:22:41.000000 Finance-Jindowin-1.2.5.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      170 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      416 2023-03-23 02:24:04.000000 Finance-Jindowin-1.2.5.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/
--rw-r--r--   0 root         (0) root         (0)     2921 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.5.1/jdw/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/
--rw-r--r--   0 root         (0) root         (0)      120 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/db/
--rw-r--r--   0 root         (0) root         (0)      101 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)    69155 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/db/db_factory.py
--rw-r--r--   0 root         (0) root         (0)     7326 2023-03-30 00:48:57.000000 Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/db/fetch_engine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/db/kd/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/db/kd/__init__.py
--rw-r--r--   0 root         (0) root         (0)    68482 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/db/kd/kd_engine.py
--rw-r--r--   0 root         (0) root         (0)      583 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/db/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/mg/
--rw-r--r--   0 root         (0) root         (0)      111 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/mg/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1265 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/mg/fetch_engine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/mg/kn/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/mg/kn/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10552 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/mg/kn/kn_engine.py
--rw-r--r--   0 root         (0) root         (0)     6160 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/mg/mg_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/rf/
--rw-r--r--   0 root         (0) root         (0)     1209 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/rf/EVENT.py
--rw-r--r--   0 root         (0) root         (0)      596 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/rf/STOCK.py
--rw-r--r--   0 root         (0) root         (0)     1999 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/rf/THEME.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/rf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/data/ExternalAPI/
--rw-r--r--   0 root         (0) root         (0)      191 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/data/ExternalAPI/__init__.py
--rw-r--r--   0 root         (0) root         (0)      233 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/data/ExternalAPI/datayes.py
--rw-r--r--   0 root         (0) root         (0)      208 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/data/ExternalAPI/ricequant.py
--rw-r--r--   0 root         (0) root         (0)      258 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.5.1/jdw/data/ExternalAPI/tushare.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/
--rw-r--r--   0 root         (0) root         (0)      922 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1765 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/dummy.py
--rw-r--r--   0 root         (0) root         (0)      441 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/engine.py
--rw-r--r--   0 root         (0) root         (0)     8728 2023-04-02 00:54:37.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/factors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/futures/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/futures/__init__.py
--rw-r--r--   0 root         (0) root         (0)      829 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/futures/basic.py
--rw-r--r--   0 root         (0) root         (0)     3432 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/futures/classify.py
--rw-r--r--   0 root         (0) root         (0)      233 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/futures/factors.py
--rw-r--r--   0 root         (0) root         (0)     1775 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/futures/index_market.py
--rw-r--r--   0 root         (0) root         (0)     1090 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/futures/yields.py
--rw-r--r--   0 root         (0) root         (0)      733 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/index_component.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/index_market.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/stock/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/stock/__init__.py
--rw-r--r--   0 root         (0) root         (0)      233 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/stock/factors.py
--rw-r--r--   0 root         (0) root         (0)     6640 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/stock/industry.py
--rw-r--r--   0 root         (0) root         (0)     2015 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/stock/market_stock.py
--rw-r--r--   0 root         (0) root         (0)    14724 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/stock/risk_model.py
--rw-r--r--   0 root         (0) root         (0)     1056 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/stock/yields.py
--rw-r--r--   0 root         (0) root         (0)     2765 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/universe.py
--rw-r--r--   0 root         (0) root         (0)     1213 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/utilities.py
--rw-r--r--   0 root         (0) root         (0)     4888 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/yields.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/data/__init__.py
--rw-r--r--   0 root         (0) root         (0)      134 2023-03-23 02:22:58.000000 Finance-Jindowin-1.2.5.1/jdw/jdcw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/kdutils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:22:58.000000 Finance-Jindowin-1.2.5.1/jdw/kdutils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1227 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.5.1/jdw/kdutils/create_id.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/kdutils/data/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:22:58.000000 Finance-Jindowin-1.2.5.1/jdw/kdutils/data/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2403 2023-03-23 02:22:58.000000 Finance-Jindowin-1.2.5.1/jdw/kdutils/data/mongodb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/kdutils/division/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/kdutils/division/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2048 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/kdutils/division/decorator.py
--rw-r--r--   0 root         (0) root         (0)     4786 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/kdutils/division/export.py
--rw-r--r--   0 root         (0) root         (0)     7249 2023-03-23 02:22:58.000000 Finance-Jindowin-1.2.5.1/jdw/kdutils/file_utils.py
--rw-r--r--   0 root         (0) root         (0)     5188 2023-03-23 02:22:58.000000 Finance-Jindowin-1.2.5.1/jdw/kdutils/logger.py
--rw-r--r--   0 root         (0) root         (0)      429 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/kdutils/singleton.py
--rw-r--r--   0 root         (0) root         (0)      357 2023-03-23 02:22:58.000000 Finance-Jindowin-1.2.5.1/jdw/kdutils/utils.py
--rw-r--r--   0 root         (0) root         (0)      396 2023-03-23 02:22:58.000000 Finance-Jindowin-1.2.5.1/jdw/kdutils/warning.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/
--rw-r--r--   0 root         (0) root         (0)      344 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/anode/
--rw-r--r--   0 root         (0) root         (0)      175 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/anode/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10145 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/anode/axtell.py
--rw-r--r--   0 root         (0) root         (0)    13341 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/anode/conor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/deckard/
--rw-r--r--   0 root         (0) root         (0)       41 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/deckard/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2038 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/deckard/goslin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/
--rw-r--r--   0 root         (0) root         (0)     1754 2023-03-27 07:08:57.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/evolution/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:05.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/evolution/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20603 2023-04-06 15:20:32.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/evolution/base.py
--rw-r--r--   0 root         (0) root         (0)     2561 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/evolution/futures.py
--rw-r--r--   0 root         (0) root         (0)     3932 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/evolution/paramizer.py
--rw-r--r--   0 root         (0) root         (0)     2432 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/evolution/stock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/geneticist/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:05.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/geneticist/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12110 2023-04-11 03:16:45.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/geneticist/base.py
--rw-r--r--   0 root         (0) root         (0)     2378 2023-03-23 02:23:05.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/geneticist/futures.py
--rw-r--r--   0 root         (0) root         (0)     2255 2023-03-23 02:23:05.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/geneticist/stock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/mutation/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/mutation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11224 2023-03-23 02:23:05.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/mutation/base.py
--rw-r--r--   0 root         (0) root         (0)     1921 2023-03-23 02:23:05.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/mutation/futures.py
--rw-r--r--   0 root         (0) root         (0)     1806 2023-03-23 02:23:05.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/mutation/stock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:07.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/carnot/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/carnot/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15382 2023-04-09 01:55:30.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/carnot/base.py
--rw-r--r--   0 root         (0) root         (0)     1902 2023-04-07 08:05:19.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/carnot/futures.py
--rw-r--r--   0 root         (0) root         (0)     1854 2023-04-07 08:05:50.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/carnot/stock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/dendall/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/dendall/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11683 2023-03-27 02:53:43.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/dendall/base.py
--rw-r--r--   0 root         (0) root         (0)     4157 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/dendall/futures.py
--rw-r--r--   0 root         (0) root         (0)     5684 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/dendall/params.py
--rw-r--r--   0 root         (0) root         (0)     3415 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/dendall/stock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/futures/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/futures/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1862 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/futures/alpha.py
--rw-r--r--   0 root         (0) root         (0)    12715 2023-03-26 11:36:16.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/futures/daily.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/mixture/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/mixture/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17309 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/mixture/base copy.py
--rw-r--r--   0 root         (0) root         (0)    11936 2023-04-10 03:16:30.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/mixture/base.py
--rw-r--r--   0 root         (0) root         (0)     1936 2023-04-10 03:16:39.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/mixture/futures.py
--rw-r--r--   0 root         (0) root         (0)    17300 2023-04-10 03:33:10.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/mixture/models.py
--rw-r--r--   0 root         (0) root         (0)     1888 2023-04-10 03:16:49.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/mixture/stock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/stock/
--rw-r--r--   0 root         (0) root         (0)       53 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/stock/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1915 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/stock/alpha.py
--rw-r--r--   0 root         (0) root         (0)    12004 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/stock/daily.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/pascal/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/pascal/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/pascal/metrics/
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/pascal/metrics/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9330 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/pascal/metrics/base.py
--rw-r--r--   0 root         (0) root         (0)     1563 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/pascal/metrics/futures.py
--rw-r--r--   0 root         (0) root         (0)     1689 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/pascal/metrics/stock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/pascal/score/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/pascal/score/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9894 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/pascal/score/base.py
--rw-r--r--   0 root         (0) root         (0)     1969 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/pascal/score/futures.py
--rw-r--r--   0 root         (0) root         (0)     1914 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/pascal/score/stock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/experimental/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/experimental/DataAPI/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/experimental/DataAPI/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/experimental/DataAPI/mg/
--rw-r--r--   0 root         (0) root         (0)      120 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/experimental/DataAPI/mg/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/experimental/DataAPI/mg/atl/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/experimental/DataAPI/mg/atl/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4170 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/experimental/DataAPI/mg/atl/engine.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/experimental/DataAPI/mg/mg_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/experimental/DataAPI/mg/ntn/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/experimental/DataAPI/mg/ntn/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3287 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/experimental/DataAPI/mg/ntn/engine.py
--rw-r--r--   0 root         (0) root         (0)     2952 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/experimental/DataAPI/mg/operator_engine.py
--rw-r--r--   0 root         (0) root         (0)      243 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/experimental/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/irey/
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/irey/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8222 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/irey/kestle.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/lombard/
--rw-r--r--   0 root         (0) root         (0)      116 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/lombard/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2240 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/lombard/base.py
--rw-r--r--   0 root         (0) root         (0)     5979 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/lombard/futures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/lombard/indicator/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/lombard/indicator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2401 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/lombard/indicator/atr.py
--rw-r--r--   0 root         (0) root         (0)     3270 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/lombard/indicator/base.py
--rw-r--r--   0 root         (0) root         (0)     3435 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/lombard/indicator/date.py
--rw-r--r--   0 root         (0) root         (0)     3312 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/lombard/indicator/symbol_pd.py
--rw-r--r--   0 root         (0) root         (0)     4466 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/lombard/stock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/neutron/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/neutron/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5540 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/neutron/analysis.py
--rw-r--r--   0 root         (0) root         (0)     6955 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/neutron/factory.py
--rw-r--r--   0 root         (0) root         (0)     1635 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/neutron/strategy.py
--rw-r--r--   0 root         (0) root         (0)     1806 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/neutron/trader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/oss/
--rw-r--r--   0 root         (0) root         (0)       37 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/oss/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2834 2023-03-23 02:23:09.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/oss/aliyun.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/plot/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/plot/STOCK/
--rw-r--r--   0 root         (0) root         (0)      212 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/plot/STOCK/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2764 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/plot/STOCK/detail.py
--rw-r--r--   0 root         (0) root         (0)     3793 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/plot/STOCK/flow_money.py
--rw-r--r--   0 root         (0) root         (0)     5916 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/plot/STOCK/hkshshz.py
--rw-r--r--   0 root         (0) root         (0)     3732 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/plot/STOCK/sentiment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/plot/THEME/
--rw-r--r--   0 root         (0) root         (0)      369 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/plot/THEME/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6599 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/plot/THEME/brief.py
--rw-r--r--   0 root         (0) root         (0)     7396 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/plot/THEME/detail.py
--rw-r--r--   0 root         (0) root         (0)     3836 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/plot/THEME/flow_money.py
--rw-r--r--   0 root         (0) root         (0)     6347 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/plot/THEME/hkshshz.py
--rw-r--r--   0 root         (0) root         (0)     7672 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/plot/THEME/indicators.py
--rw-r--r--   0 root         (0) root         (0)     3123 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/plot/THEME/returns.py
--rw-r--r--   0 root         (0) root         (0)     3732 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/plot/THEME/sentiment.py
--rw-r--r--   0 root         (0) root         (0)      612 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/plot/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4200 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/plot/returns.py
--rw-r--r--   0 root         (0) root         (0)     1744 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/plot/stock.py
--rw-r--r--   0 root         (0) root         (0)     6727 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.5.1/jdw/to_pandas.py
--rw-r--r--   0 root         (0) root         (0)     2114 2023-03-23 02:22:58.000000 Finance-Jindowin-1.2.5.1/jdw/utils.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-14 15:44:53.000000 Finance-Jindowin-1.2.5.1/jdw/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/requirements/
--rw-r--r--   0 root         (0) root         (0)      242 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.5.1/requirements/py3.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2065 2023-03-23 02:22:41.000000 Finance-Jindowin-1.2.5.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/Finance_Jindowin.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      222 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/Finance_Jindowin.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5769 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/Finance_Jindowin.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       74 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/Finance_Jindowin.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      243 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/Finance_Jindowin.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/Finance_Jindowin.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      114 2023-03-23 02:22:41.000000 Finance-Jindowin-1.2.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      222 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      416 2023-03-23 02:24:04.000000 Finance-Jindowin-1.2.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/
+-rw-r--r--   0 root         (0) root         (0)     3138 2023-06-02 07:16:57.000000 Finance-Jindowin-1.2.6/jdw/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/data/DataAPI/
+-rw-r--r--   0 root         (0) root         (0)      120 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.6/jdw/data/DataAPI/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/data/DataAPI/db/
+-rw-r--r--   0 root         (0) root         (0)      101 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.6/jdw/data/DataAPI/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    70043 2023-06-01 01:39:01.000000 Finance-Jindowin-1.2.6/jdw/data/DataAPI/db/db_factory.py
+-rw-r--r--   0 root         (0) root         (0)     7326 2023-03-30 00:48:57.000000 Finance-Jindowin-1.2.6/jdw/data/DataAPI/db/fetch_engine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/data/DataAPI/db/kd/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.6/jdw/data/DataAPI/db/kd/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71586 2023-06-01 13:15:26.000000 Finance-Jindowin-1.2.6/jdw/data/DataAPI/db/kd/kd_engine.py
+-rw-r--r--   0 root         (0) root         (0)      583 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.6/jdw/data/DataAPI/db/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/data/DataAPI/ddb/
+-rw-r--r--   0 root         (0) root         (0)      104 2023-06-01 01:52:53.000000 Finance-Jindowin-1.2.6/jdw/data/DataAPI/ddb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/data/DataAPI/ddb/ch/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 14:09:04.000000 Finance-Jindowin-1.2.6/jdw/data/DataAPI/ddb/ch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      366 2023-06-01 11:17:20.000000 Finance-Jindowin-1.2.6/jdw/data/DataAPI/ddb/ch/ch_engine.py
+-rw-r--r--   0 root         (0) root         (0)     1559 2023-06-01 23:53:43.000000 Finance-Jindowin-1.2.6/jdw/data/DataAPI/ddb/ddb_factory.py
+-rw-r--r--   0 root         (0) root         (0)     7594 2023-06-01 12:24:33.000000 Finance-Jindowin-1.2.6/jdw/data/DataAPI/ddb/fetch_engine.py
+-rw-r--r--   0 root         (0) root         (0)      589 2023-06-02 03:11:22.000000 Finance-Jindowin-1.2.6/jdw/data/DataAPI/ddb/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/data/DataAPI/mg/
+-rw-r--r--   0 root         (0) root         (0)      111 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.6/jdw/data/DataAPI/mg/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1265 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.6/jdw/data/DataAPI/mg/fetch_engine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/data/DataAPI/mg/kn/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.6/jdw/data/DataAPI/mg/kn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10552 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.6/jdw/data/DataAPI/mg/kn/kn_engine.py
+-rw-r--r--   0 root         (0) root         (0)     6160 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.6/jdw/data/DataAPI/mg/mg_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/data/DataAPI/rf/
+-rw-r--r--   0 root         (0) root         (0)     1209 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.6/jdw/data/DataAPI/rf/EVENT.py
+-rw-r--r--   0 root         (0) root         (0)      596 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.6/jdw/data/DataAPI/rf/STOCK.py
+-rw-r--r--   0 root         (0) root         (0)     1999 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.6/jdw/data/DataAPI/rf/THEME.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.6/jdw/data/DataAPI/rf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/data/ExternalAPI/
+-rw-r--r--   0 root         (0) root         (0)      191 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.6/jdw/data/ExternalAPI/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      233 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.6/jdw/data/ExternalAPI/datayes.py
+-rw-r--r--   0 root         (0) root         (0)      208 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.6/jdw/data/ExternalAPI/ricequant.py
+-rw-r--r--   0 root         (0) root         (0)      258 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.6/jdw/data/ExternalAPI/tushare.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/data/RetrievalAPI/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-06-02 06:43:44.000000 Finance-Jindowin-1.2.6/jdw/data/RetrievalAPI/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2235 2023-06-02 07:03:59.000000 Finance-Jindowin-1.2.6/jdw/data/RetrievalAPI/customized.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/data/SurfaceAPI/
+-rw-r--r--   0 root         (0) root         (0)      922 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.6/jdw/data/SurfaceAPI/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1765 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.6/jdw/data/SurfaceAPI/dummy.py
+-rw-r--r--   0 root         (0) root         (0)      441 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.6/jdw/data/SurfaceAPI/engine.py
+-rw-r--r--   0 root         (0) root         (0)     8728 2023-04-02 00:54:37.000000 Finance-Jindowin-1.2.6/jdw/data/SurfaceAPI/factors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/data/SurfaceAPI/futures/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.6/jdw/data/SurfaceAPI/futures/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      829 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.6/jdw/data/SurfaceAPI/futures/basic.py
+-rw-r--r--   0 root         (0) root         (0)     3432 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.6/jdw/data/SurfaceAPI/futures/classify.py
+-rw-r--r--   0 root         (0) root         (0)      233 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.6/jdw/data/SurfaceAPI/futures/factors.py
+-rw-r--r--   0 root         (0) root         (0)     1775 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.6/jdw/data/SurfaceAPI/futures/index_market.py
+-rw-r--r--   0 root         (0) root         (0)     1090 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.6/jdw/data/SurfaceAPI/futures/yields.py
+-rw-r--r--   0 root         (0) root         (0)      733 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.6/jdw/data/SurfaceAPI/index_component.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.6/jdw/data/SurfaceAPI/index_market.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/data/SurfaceAPI/stock/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.6/jdw/data/SurfaceAPI/stock/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      233 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.6/jdw/data/SurfaceAPI/stock/factors.py
+-rw-r--r--   0 root         (0) root         (0)     6640 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.6/jdw/data/SurfaceAPI/stock/industry.py
+-rw-r--r--   0 root         (0) root         (0)     2015 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.6/jdw/data/SurfaceAPI/stock/market_stock.py
+-rw-r--r--   0 root         (0) root         (0)    14724 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.6/jdw/data/SurfaceAPI/stock/risk_model.py
+-rw-r--r--   0 root         (0) root         (0)     1056 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.6/jdw/data/SurfaceAPI/stock/yields.py
+-rw-r--r--   0 root         (0) root         (0)     2765 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.6/jdw/data/SurfaceAPI/universe.py
+-rw-r--r--   0 root         (0) root         (0)     1213 2023-04-30 12:09:18.000000 Finance-Jindowin-1.2.6/jdw/data/SurfaceAPI/utilities.py
+-rw-r--r--   0 root         (0) root         (0)     4888 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.6/jdw/data/SurfaceAPI/yields.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.6/jdw/data/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      134 2023-03-23 02:22:58.000000 Finance-Jindowin-1.2.6/jdw/jdcw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/kdutils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:22:58.000000 Finance-Jindowin-1.2.6/jdw/kdutils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1227 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.6/jdw/kdutils/create_id.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/kdutils/data/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:22:58.000000 Finance-Jindowin-1.2.6/jdw/kdutils/data/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2403 2023-03-23 02:22:58.000000 Finance-Jindowin-1.2.6/jdw/kdutils/data/mongodb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/kdutils/division/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.6/jdw/kdutils/division/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2048 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.6/jdw/kdutils/division/decorator.py
+-rw-r--r--   0 root         (0) root         (0)     4786 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.6/jdw/kdutils/division/export.py
+-rw-r--r--   0 root         (0) root         (0)     7249 2023-03-23 02:22:58.000000 Finance-Jindowin-1.2.6/jdw/kdutils/file_utils.py
+-rw-r--r--   0 root         (0) root         (0)     5188 2023-03-23 02:22:58.000000 Finance-Jindowin-1.2.6/jdw/kdutils/logger.py
+-rw-r--r--   0 root         (0) root         (0)      429 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.6/jdw/kdutils/singleton.py
+-rw-r--r--   0 root         (0) root         (0)      357 2023-03-23 02:22:58.000000 Finance-Jindowin-1.2.6/jdw/kdutils/utils.py
+-rw-r--r--   0 root         (0) root         (0)      396 2023-03-23 02:22:58.000000 Finance-Jindowin-1.2.6/jdw/kdutils/warning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/mfc/
+-rw-r--r--   0 root         (0) root         (0)      344 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.6/jdw/mfc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/mfc/anode/
+-rw-r--r--   0 root         (0) root         (0)      175 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.6/jdw/mfc/anode/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10145 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.6/jdw/mfc/anode/axtell.py
+-rw-r--r--   0 root         (0) root         (0)    13341 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.6/jdw/mfc/anode/conor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/mfc/deckard/
+-rw-r--r--   0 root         (0) root         (0)       41 2023-05-13 11:14:20.000000 Finance-Jindowin-1.2.6/jdw/mfc/deckard/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2038 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.6/jdw/mfc/deckard/goslin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/
+-rw-r--r--   0 root         (0) root         (0)     1754 2023-04-19 09:57:11.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/catalyst/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/catalyst/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/catalyst/evolution/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:05.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/catalyst/evolution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21105 2023-05-04 15:13:28.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/catalyst/evolution/base.py
+-rw-r--r--   0 root         (0) root         (0)     2666 2023-05-05 05:28:29.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/catalyst/evolution/futures.py
+-rw-r--r--   0 root         (0) root         (0)     3932 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/catalyst/evolution/paramizer.py
+-rw-r--r--   0 root         (0) root         (0)     2535 2023-05-05 05:29:04.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/catalyst/evolution/stock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/catalyst/geneticist/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:05.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/catalyst/geneticist/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12110 2023-04-19 09:57:11.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/catalyst/geneticist/base.py
+-rw-r--r--   0 root         (0) root         (0)     2378 2023-03-23 02:23:05.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/catalyst/geneticist/futures.py
+-rw-r--r--   0 root         (0) root         (0)     2255 2023-03-23 02:23:05.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/catalyst/geneticist/stock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/catalyst/mutation/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/catalyst/mutation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11224 2023-03-23 02:23:05.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/catalyst/mutation/base.py
+-rw-r--r--   0 root         (0) root         (0)     1921 2023-03-23 02:23:05.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/catalyst/mutation/futures.py
+-rw-r--r--   0 root         (0) root         (0)     1806 2023-03-23 02:23:05.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/catalyst/mutation/stock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/gravity/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:07.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/gravity/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/gravity/carnot/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/gravity/carnot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15382 2023-04-19 09:57:11.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/gravity/carnot/base.py
+-rw-r--r--   0 root         (0) root         (0)     1902 2023-04-19 09:57:11.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/gravity/carnot/futures.py
+-rw-r--r--   0 root         (0) root         (0)     1854 2023-04-19 09:57:11.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/gravity/carnot/stock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/gravity/dendall/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/gravity/dendall/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11683 2023-03-27 02:53:43.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/gravity/dendall/base.py
+-rw-r--r--   0 root         (0) root         (0)     4157 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/gravity/dendall/futures.py
+-rw-r--r--   0 root         (0) root         (0)     5684 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/gravity/dendall/params.py
+-rw-r--r--   0 root         (0) root         (0)     3415 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/gravity/dendall/stock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/gravity/futures/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/gravity/futures/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1862 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/gravity/futures/alpha.py
+-rw-r--r--   0 root         (0) root         (0)    12715 2023-03-26 11:36:16.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/gravity/futures/daily.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/gravity/mixture/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/gravity/mixture/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17309 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/gravity/mixture/base copy.py
+-rw-r--r--   0 root         (0) root         (0)    11936 2023-04-19 09:57:11.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/gravity/mixture/base.py
+-rw-r--r--   0 root         (0) root         (0)     1936 2023-04-19 09:57:11.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/gravity/mixture/futures.py
+-rw-r--r--   0 root         (0) root         (0)    17300 2023-04-19 09:57:11.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/gravity/mixture/models.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2023-04-19 09:57:11.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/gravity/mixture/stock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/gravity/stock/
+-rw-r--r--   0 root         (0) root         (0)       53 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/gravity/stock/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1915 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/gravity/stock/alpha.py
+-rw-r--r--   0 root         (0) root         (0)    12004 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/gravity/stock/daily.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/pascal/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/pascal/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/pascal/metrics/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/pascal/metrics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9330 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/pascal/metrics/base.py
+-rw-r--r--   0 root         (0) root         (0)     1563 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/pascal/metrics/futures.py
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/pascal/metrics/stock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/pascal/score/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/pascal/score/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9894 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/pascal/score/base.py
+-rw-r--r--   0 root         (0) root         (0)     1969 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/pascal/score/futures.py
+-rw-r--r--   0 root         (0) root         (0)     1914 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.6/jdw/mfc/entropy/pascal/score/stock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/mfc/experimental/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/mfc/experimental/DataAPI/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.6/jdw/mfc/experimental/DataAPI/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/mfc/experimental/DataAPI/mg/
+-rw-r--r--   0 root         (0) root         (0)      120 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.6/jdw/mfc/experimental/DataAPI/mg/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/mfc/experimental/DataAPI/mg/atl/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.6/jdw/mfc/experimental/DataAPI/mg/atl/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4170 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.6/jdw/mfc/experimental/DataAPI/mg/atl/engine.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.6/jdw/mfc/experimental/DataAPI/mg/mg_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/mfc/experimental/DataAPI/mg/ntn/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.6/jdw/mfc/experimental/DataAPI/mg/ntn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3287 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.6/jdw/mfc/experimental/DataAPI/mg/ntn/engine.py
+-rw-r--r--   0 root         (0) root         (0)     2952 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.6/jdw/mfc/experimental/DataAPI/mg/operator_engine.py
+-rw-r--r--   0 root         (0) root         (0)      243 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.6/jdw/mfc/experimental/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/mfc/irey/
+-rw-r--r--   0 root         (0) root         (0)       38 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.6/jdw/mfc/irey/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8222 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.6/jdw/mfc/irey/kestle.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/mfc/lombard/
+-rw-r--r--   0 root         (0) root         (0)      116 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.6/jdw/mfc/lombard/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2240 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.6/jdw/mfc/lombard/base.py
+-rw-r--r--   0 root         (0) root         (0)     5979 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.6/jdw/mfc/lombard/futures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/mfc/lombard/indicator/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.6/jdw/mfc/lombard/indicator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2401 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.6/jdw/mfc/lombard/indicator/atr.py
+-rw-r--r--   0 root         (0) root         (0)     3270 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.6/jdw/mfc/lombard/indicator/base.py
+-rw-r--r--   0 root         (0) root         (0)     3435 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.6/jdw/mfc/lombard/indicator/date.py
+-rw-r--r--   0 root         (0) root         (0)     3312 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.6/jdw/mfc/lombard/indicator/symbol_pd.py
+-rw-r--r--   0 root         (0) root         (0)     4466 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.6/jdw/mfc/lombard/stock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/mfc/neutron/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.6/jdw/mfc/neutron/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5540 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.6/jdw/mfc/neutron/analysis.py
+-rw-r--r--   0 root         (0) root         (0)     6955 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.6/jdw/mfc/neutron/factory.py
+-rw-r--r--   0 root         (0) root         (0)     1635 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.6/jdw/mfc/neutron/strategy.py
+-rw-r--r--   0 root         (0) root         (0)     1806 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.6/jdw/mfc/neutron/trader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/mfc/oss/
+-rw-r--r--   0 root         (0) root         (0)       37 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.6/jdw/mfc/oss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2834 2023-03-23 02:23:09.000000 Finance-Jindowin-1.2.6/jdw/mfc/oss/aliyun.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/plot/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/plot/STOCK/
+-rw-r--r--   0 root         (0) root         (0)      212 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.6/jdw/plot/STOCK/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2764 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.6/jdw/plot/STOCK/detail.py
+-rw-r--r--   0 root         (0) root         (0)     3793 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.6/jdw/plot/STOCK/flow_money.py
+-rw-r--r--   0 root         (0) root         (0)     5916 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.6/jdw/plot/STOCK/hkshshz.py
+-rw-r--r--   0 root         (0) root         (0)     3732 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.6/jdw/plot/STOCK/sentiment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/jdw/plot/THEME/
+-rw-r--r--   0 root         (0) root         (0)      369 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.6/jdw/plot/THEME/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6599 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.6/jdw/plot/THEME/brief.py
+-rw-r--r--   0 root         (0) root         (0)     7396 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.6/jdw/plot/THEME/detail.py
+-rw-r--r--   0 root         (0) root         (0)     3836 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.6/jdw/plot/THEME/flow_money.py
+-rw-r--r--   0 root         (0) root         (0)     6347 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.6/jdw/plot/THEME/hkshshz.py
+-rw-r--r--   0 root         (0) root         (0)     7672 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.6/jdw/plot/THEME/indicators.py
+-rw-r--r--   0 root         (0) root         (0)     3123 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.6/jdw/plot/THEME/returns.py
+-rw-r--r--   0 root         (0) root         (0)     3732 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.6/jdw/plot/THEME/sentiment.py
+-rw-r--r--   0 root         (0) root         (0)      612 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.6/jdw/plot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4200 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.6/jdw/plot/returns.py
+-rw-r--r--   0 root         (0) root         (0)     1744 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.6/jdw/plot/stock.py
+-rw-r--r--   0 root         (0) root         (0)     6727 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.6/jdw/to_pandas.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2023-03-23 02:22:58.000000 Finance-Jindowin-1.2.6/jdw/utils.py
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-02 07:26:45.000000 Finance-Jindowin-1.2.6/jdw/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/requirements/
+-rw-r--r--   0 root         (0) root         (0)      242 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.6/requirements/py3.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-02 07:27:58.000000 Finance-Jindowin-1.2.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2065 2023-04-15 00:11:07.000000 Finance-Jindowin-1.2.6/setup.py
```

### Comparing `Finance-Jindowin-1.2.5.1/Finance_Jindowin.egg-info/SOURCES.txt` & `Finance-Jindowin-1.2.6/Finance_Jindowin.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -16,27 +16,35 @@
 jdw/data/DataAPI/__init__.py
 jdw/data/DataAPI/db/__init__.py
 jdw/data/DataAPI/db/db_factory.py
 jdw/data/DataAPI/db/fetch_engine.py
 jdw/data/DataAPI/db/utilities.py
 jdw/data/DataAPI/db/kd/__init__.py
 jdw/data/DataAPI/db/kd/kd_engine.py
+jdw/data/DataAPI/ddb/__init__.py
+jdw/data/DataAPI/ddb/ddb_factory.py
+jdw/data/DataAPI/ddb/fetch_engine.py
+jdw/data/DataAPI/ddb/utilities.py
+jdw/data/DataAPI/ddb/ch/__init__.py
+jdw/data/DataAPI/ddb/ch/ch_engine.py
 jdw/data/DataAPI/mg/__init__.py
 jdw/data/DataAPI/mg/fetch_engine.py
 jdw/data/DataAPI/mg/mg_factory.py
 jdw/data/DataAPI/mg/kn/__init__.py
 jdw/data/DataAPI/mg/kn/kn_engine.py
 jdw/data/DataAPI/rf/EVENT.py
 jdw/data/DataAPI/rf/STOCK.py
 jdw/data/DataAPI/rf/THEME.py
 jdw/data/DataAPI/rf/__init__.py
 jdw/data/ExternalAPI/__init__.py
 jdw/data/ExternalAPI/datayes.py
 jdw/data/ExternalAPI/ricequant.py
 jdw/data/ExternalAPI/tushare.py
+jdw/data/RetrievalAPI/__init__.py
+jdw/data/RetrievalAPI/customized.py
 jdw/data/SurfaceAPI/__init__.py
 jdw/data/SurfaceAPI/dummy.py
 jdw/data/SurfaceAPI/engine.py
 jdw/data/SurfaceAPI/factors.py
 jdw/data/SurfaceAPI/index_component.py
 jdw/data/SurfaceAPI/index_market.py
 jdw/data/SurfaceAPI/universe.py
```

### Comparing `Finance-Jindowin-1.2.5.1/jdw/__init__.py` & `Finance-Jindowin-1.2.6/jdw/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,15 +41,21 @@
     warnings.warn("pip install --upgrade pymongo")
 
 try:
     import jdw.data.DataAPI.db as DBAPI
 except ImportError:
     warnings.warn("pip install --upgrade SQLCharmy")
 
+try:
+    import jdw.data.DataAPI.ddb as DDBAPI
+except ImportError:
+    warnings.warn("pip install --upgrade dolphinDB")
+
 import jdw.data.SurfaceAPI as SurfaceAPI
+import jdw.data.RetrievalAPI as RetrievalAPI
 
 try:
     import jdw.mfc.experimental.DataAPI.mg as ExperimentalAPI
     import jdw.mfc.irey as IreyAPI
     import jdw.mfc.deckard as DeckardAPI
     import jdw.mfc.lombard as LombardAPI
     #import jdw.data.ExternalAPI as ExternalAPI
@@ -59,14 +65,15 @@
 except ImportError as e:
     warnings.warn("pip install --upgrade  Jindowin:{0}".format(e))
 #try:
 #    import jdw.mfc.anode as AnodeAPI
 #except ImportError:
 #    warnings.warn("the environment cannot be traded")
 
+import jdw.data.DataAPI.ddb.utilities as ddb_tools
 from .version import __version__
 
 try:
     unicode
 except:
     unicode = str
```

### Comparing `Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/db/db_factory.py` & `Finance-Jindowin-1.2.6/jdw/data/DataAPI/db/db_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -360,14 +360,33 @@
                                                   begin_date=begin_date,
                                                   end_date=end_date,
                                                   columns=columns,
                                                   freq=freq,
                                                   dates=dates)
 
 
+class FuturesFactorsFactoryV1(EngineFactory):
+
+    def result(self,
+               codes=None,
+               key=None,
+               begin_date=None,
+               end_date=None,
+               columns=None,
+               freq=None,
+               dates=None):
+        return self._fetch_engine.futures_factors_v1(codes=codes,
+                                                     key=key,
+                                                     begin_date=begin_date,
+                                                     end_date=end_date,
+                                                     columns=columns,
+                                                     freq=freq,
+                                                     dates=dates)
+
+
 class FutWareFactory(EngineFactory):
 
     __name__ = 'fut_ware'
 
     def result(self,
                codes,
                key=None,
@@ -1260,14 +1279,20 @@
 
 class FactorsCategory(EngineFactory):
 
     def result(self, factors):
         return self._fetch_engine.factors_category(factors=factors)
 
 
+class FactorsCategoryV1(EngineFactory):
+
+    def result(self, factors):
+        return self._fetch_engine.factors_category_v1(factors=factors)
+
+
 ##### 风险模型数据
 
 
 class RiskCovDayFactory(EngineFactory):
     __name__ = 'risk_cov_day'
 
     def result(self,
```

### Comparing `Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/db/fetch_engine.py` & `Finance-Jindowin-1.2.6/jdw/data/DataAPI/db/fetch_engine.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/db/kd/kd_engine.py` & `Finance-Jindowin-1.2.6/jdw/data/DataAPI/db/kd/kd_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,26 @@
             if 'stk_factor' in k or 'stk_derived' in k
         ]
         self._futures_factor_tables = [
             self._base.classes[k] for k in self._base.classes.keys()
             if 'fut_factor' in k or 'fut_derived' in k
         ]
 
+        self._futures_factor_tables_v1 = [
+            self._base.classes['market_fut'], self._base.classes['research'],
+            self._base.classes['factor_basis'],
+            self._base.classes['factor_fundamentals'],
+            self._base.classes['factor_momentum'],
+            self._base.classes['factor_position'],
+            self._base.classes['factor_term_structure'],
+            self._base.classes['factor_sentiment'],
+            self._base.classes['factor_reversal'],
+            self._base.classes['factor_tf_fundamentals']
+        ]
+
     def default_dates(self, table, dates, codes=None, key=None):
 
         return and_(table.trade_date.in_(dates), table.flag
                     == 1) if key is None else and_(
                         table.trade_date.in_(dates), table.flag == 1,
                         table.__dict__[key].in_(codes))
 
@@ -318,14 +330,61 @@
                        list(factor_cols.keys())).select_from(big_table).where(
                            clause_list)
         return pd.read_sql(query, self._engine.sql_engine()).drop_duplicates(
             subset=['trade_date', 'code']).replace(
                 [-np.inf, np.inf],
                 np.nan).sort_values(by=['trade_date', 'code'])
 
+    def futures_factors_v1(self,
+                           codes=None,
+                           key=None,
+                           begin_date=None,
+                           end_date=None,
+                           columns=None,
+                           freq=None,
+                           dates=None):
+        factor_cols = _map_factors(columns, self._futures_factor_tables_v1)
+        Market = self._base.classes['market_fut']
+        joined_tables = set()
+        big_table = Market
+        joined_tables.add(Market.__table__.name)
+        for t in set(factor_cols.values()):
+            if t.__table__.name not in joined_tables:
+                big_table = outerjoin(
+                    big_table, t,
+                    and_(Market.trade_date == t.trade_date,
+                         Market.contractObject == t.code, Market.mainCon == 1,
+                         t.flag == 1))
+                joined_tables.add(t.__table__.name)
+        if dates is not None and codes is not None:
+            query = select([
+                Market.trade_date,
+                Market.contractObject,
+                Market.closePrice,
+                Market.code,
+                Market.accumAdjFactor,
+                Market.turnoverVol,
+                Market.CHG,
+            ] + list(factor_cols.keys())).select_from(big_table).where(
+                and_(Market.trade_date.in_(dates), Market.flag == 1,
+                     Market.mainCon == 1, Market.contractObject.in_(codes)))
+        elif dates is None and codes is not None:
+            query = select([
+                Market.trade_date, Market.contractObject, Market.closePrice,
+                Market.code, Market.turnoverVol, Market.CHG
+            ] + list(factor_cols.keys())).select_from(big_table).where(
+                and_(Market.trade_date.between(begin_date, end_date),
+                     Market.flag == 1, Market.mainCon == 1,
+                     Market.contractObject.in_(codes)))
+
+        return pd.read_sql(query, self._engine.sql_engine()).drop_duplicates(
+            subset=['trade_date', 'code']).replace(
+                [-np.inf, np.inf],
+                np.nan).sort_values(by=['trade_date', 'code'])
+
     def fut_ware(self,
                  codes,
                  key=None,
                  begin_date=None,
                  end_date=None,
                  columns=None,
                  freq=None,
@@ -1602,14 +1661,24 @@
         for f in factors:
             for t in factors_tables:
                 if f in t.__table__.columns:
                     cat.append({'name': f, 'category': t.__name__})
         detail = pd.DataFrame(cat)
         return detail
 
+    def factors_category_v1(self, factors, type=1):
+        cat = []
+        factors_tables = self._futures_factor_tables_v1
+        for f in factors:
+            for t in factors_tables:
+                if f in t.__table__.columns:
+                    cat.append({'name': f, 'category': t.__name__})
+        detail = pd.DataFrame(cat)
+        return detail
+
     def stock_factors(self,
                       codes=None,
                       key=None,
                       begin_date=None,
                       end_date=None,
                       columns=None,
                       freq=None,
```

### Comparing `Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/db/utilities.py` & `Finance-Jindowin-1.2.6/jdw/data/DataAPI/db/utilities.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/mg/fetch_engine.py` & `Finance-Jindowin-1.2.6/jdw/data/DataAPI/mg/fetch_engine.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/mg/kn/kn_engine.py` & `Finance-Jindowin-1.2.6/jdw/data/DataAPI/mg/kn/kn_engine.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/mg/mg_factory.py` & `Finance-Jindowin-1.2.6/jdw/data/DataAPI/mg/mg_factory.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/rf/EVENT.py` & `Finance-Jindowin-1.2.6/jdw/data/DataAPI/rf/EVENT.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/rf/STOCK.py` & `Finance-Jindowin-1.2.6/jdw/data/DataAPI/rf/STOCK.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/rf/THEME.py` & `Finance-Jindowin-1.2.6/jdw/data/DataAPI/rf/THEME.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/__init__.py` & `Finance-Jindowin-1.2.6/jdw/data/SurfaceAPI/__init__.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/dummy.py` & `Finance-Jindowin-1.2.6/jdw/data/SurfaceAPI/dummy.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/factors.py` & `Finance-Jindowin-1.2.6/jdw/data/SurfaceAPI/factors.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/futures/basic.py` & `Finance-Jindowin-1.2.6/jdw/data/SurfaceAPI/futures/basic.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/futures/classify.py` & `Finance-Jindowin-1.2.6/jdw/data/SurfaceAPI/futures/classify.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/futures/index_market.py` & `Finance-Jindowin-1.2.6/jdw/data/SurfaceAPI/futures/index_market.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/futures/yields.py` & `Finance-Jindowin-1.2.6/jdw/data/SurfaceAPI/futures/yields.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/index_component.py` & `Finance-Jindowin-1.2.6/jdw/data/SurfaceAPI/index_component.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/index_market.py` & `Finance-Jindowin-1.2.6/jdw/data/SurfaceAPI/index_market.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/stock/industry.py` & `Finance-Jindowin-1.2.6/jdw/data/SurfaceAPI/stock/industry.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/stock/market_stock.py` & `Finance-Jindowin-1.2.6/jdw/data/SurfaceAPI/stock/market_stock.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/stock/risk_model.py` & `Finance-Jindowin-1.2.6/jdw/data/SurfaceAPI/stock/risk_model.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/stock/yields.py` & `Finance-Jindowin-1.2.6/jdw/data/SurfaceAPI/stock/yields.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/universe.py` & `Finance-Jindowin-1.2.6/jdw/data/SurfaceAPI/universe.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/utilities.py` & `Finance-Jindowin-1.2.6/jdw/data/SurfaceAPI/utilities.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/yields.py` & `Finance-Jindowin-1.2.6/jdw/data/SurfaceAPI/yields.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/kdutils/create_id.py` & `Finance-Jindowin-1.2.6/jdw/kdutils/create_id.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/kdutils/data/mongodb.py` & `Finance-Jindowin-1.2.6/jdw/kdutils/data/mongodb.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/kdutils/division/decorator.py` & `Finance-Jindowin-1.2.6/jdw/kdutils/division/decorator.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/kdutils/division/export.py` & `Finance-Jindowin-1.2.6/jdw/kdutils/division/export.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/kdutils/file_utils.py` & `Finance-Jindowin-1.2.6/jdw/kdutils/file_utils.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/kdutils/logger.py` & `Finance-Jindowin-1.2.6/jdw/kdutils/logger.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/anode/axtell.py` & `Finance-Jindowin-1.2.6/jdw/mfc/anode/axtell.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/anode/conor.py` & `Finance-Jindowin-1.2.6/jdw/mfc/anode/conor.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/deckard/goslin.py` & `Finance-Jindowin-1.2.6/jdw/mfc/deckard/goslin.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/__init__.py` & `Finance-Jindowin-1.2.6/jdw/mfc/entropy/__init__.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/evolution/base.py` & `Finance-Jindowin-1.2.6/jdw/mfc/entropy/catalyst/evolution/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,15 @@
                  dummy_name=None,
                  offset=0,
                  horizon=0,
                  factors_normal=True,
                  callback_save=None,
                  is_loop=False,
                  model_sets=None,
+                 params_sets=None,
                  yield_name='returns'):
         self._yields_class = yields_class
         self._factors_class = factors_class
         self._universe_class = universe_class
         self._industry_class = industry_class
         #self._factor_columns = factor_columns
         self._factors_normal = factors_normal
@@ -73,14 +74,15 @@
         self._dummy_class = dummy_class
         self._dummy_name = dummy_name
         self._results = None
         self._total_data = None
         self._best_programs = None
         self._gentic_class = Engine if is_loop else Gentic
         self._model_sets = default_models if model_sets is None else model_sets
+        self._params_sets = params_sets
         self._transformer = Transformer(factor_columns)
 
     def industry_fillna(self, industry_data, factors_data):
         return factors_data
 
     def fetch_returns(self, begin_date, end_date, universe=None):
         yields = self._yields_class()
@@ -295,25 +297,38 @@
 
     def best_programs(self):
         return self._best_programs.reset_index(
             drop=True).sort_values(by=['fitness']) if isinstance(
                 self._best_programs, pd.DataFrame) is not None else None
 
     def calculate_result(self, dimension_data, configure, custom_params=None):
+
+        def change_params(model, custom_sets):
+            if model in custom_sets:
+                return custom_sets[model]
+            else:
+                return Paramizer().__getattribute__(model)()
+
         self.create_configure(configure)
         kwargs = custom_params if isinstance(custom_params, dict) else {}
         kwargs['mode'] = configure['mode']
         kwargs['horizon'] = self._horizon
         kwargs['offset'] = self._offset
         kwargs['universe'] = self._universe
 
         configure['custom_params'] = kwargs
-        params_sets = dict(
-            zip(self._model_sets,
-                [Paramizer().__getattribute__(m)() for m in self._model_sets]))
+        params_sets = [
+            change_params(model, self._params_sets)
+            for model in self._model_sets
+        ]
+        params_sets = dict(zip(self._model_sets, params_sets))
+
+        #params_sets = dict(
+        #    zip(self._model_sets,
+        #        [Paramizer().__getattribute__(m)() for m in self._model_sets]))
 
         columns = [
             col for col in dimension_data.columns.tolist()
             if col not in ['trade_date', 'code', 'nxt1_ret', 'nxt1_ret_w']
         ]
 
         ### 数据切分
@@ -435,14 +450,15 @@
 
         #returns_data = yields_data.copy()
         ## 提取非累积收益 偏移
         returns_data = self.fetch_returns(
             begin_date=begin_date,
             end_date=end_date,
             universe=self._universe_class(u_name=self._universe))
+
         if self._factors_normal:
             total_data = factors_data.merge(yields_data,
                                             on=['trade_date', 'code'])
             total_data = self.factors_normal(
                 total_data, self._transformer.names + ['nxt1_ret'])
             factors_data = total_data[['trade_date', 'code'] +
                                       self._transformer.names]
@@ -459,14 +475,15 @@
                             ]) if dummy_data is not None else dimension_data
 
         return dimension_data.merge(returns_data,
                                     on=['trade_date', 'code'],
                                     suffixes=('', '_w'))
 
     def run(self, begin_date, end_date, configure, custom_params=None):
+        pdb.set_trace()
         kd_logger.info("start service")
         dimension_data = self.prepare_data(begin_date=begin_date,
                                            end_date=end_date)
 
         self.calculate_result(dimension_data=dimension_data,
                               configure=configure,
                               custom_params=custom_params)
```

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/evolution/futures.py` & `Finance-Jindowin-1.2.6/jdw/mfc/entropy/catalyst/evolution/futures.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,15 @@
                  industry_level,
                  is_weighted=False,
                  dummy_name=None,
                  is_loop=False,
                  offset=0,
                  horizon=0,
                  model_sets=None,
+                 params_sets={},
                  factors_normal=True,
                  callback_save=None,
                  yield_name='returns'):
         super(FuturesEvolution, self).__init__(yields_class=FutYields,
                                                factors_class=FutFactors,
                                                universe_class=FutUniverse,
                                                industry_class=FutClassify,
@@ -36,14 +37,15 @@
                                                universe=universe,
                                                dummy_name=dummy_name,
                                                is_loop=is_loop,
                                                factor_columns=factor_columns,
                                                industry_name=industry_name,
                                                industry_level=industry_level,
                                                model_sets=model_sets,
+                                               params_sets=params_sets,
                                                factors_normal=factors_normal,
                                                callback_save=callback_save,
                                                yield_name=yield_name)
 
     def industry_fillna(self, industry_data, factors_data):
         factors_data = factors_data.merge(industry_data.drop(['trade_date'],
                                                              axis=1),
```

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/evolution/paramizer.py` & `Finance-Jindowin-1.2.6/jdw/mfc/entropy/catalyst/evolution/paramizer.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/evolution/stock.py` & `Finance-Jindowin-1.2.6/jdw/mfc/entropy/catalyst/mutation/stock.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,39 @@
 # -*- coding: utf-8 -*-
 from jdw.data.SurfaceAPI.stock.yields import StkYields
 from jdw.data.SurfaceAPI.stock.factors import StkFactors
 from jdw.data.SurfaceAPI.universe import StkUniverse
 from jdw.data.SurfaceAPI.stock.industry import Industry
-from jdw.data.SurfaceAPI.dummy import Dummy
-from jdw.mfc.entropy.catalyst.evolution.base import Base
+from jdw.mfc.entropy.catalyst.mutation.base import Base
 
 
-class StockEvolution(Base):
+class StockMutation(Base):
 
     def __init__(self,
-                 thresh,
-                 universe,
+                 offset,
+                 horizon,
                  factor_columns,
+                 universe,
                  industry_name,
                  industry_level,
-                 is_weighted=True,
-                 dummy_name=None,
-                 is_loop=False,
-                 offset=0,
-                 horizon=0,
-                 model_sets=None,
                  factors_normal=True,
-                 callback_save=None,
+                 operators=None,
                  yield_name='returns'):
-        super(StockEvolution, self).__init__(yields_class=StkYields,
-                                             factors_class=StkFactors,
-                                             universe_class=StkUniverse,
-                                             industry_class=Industry,
-                                             dummy_class=Dummy,
-                                             is_weighted=is_weighted,
-                                             thresh=thresh,
-                                             offset=offset,
-                                             horizon=horizon,
-                                             universe=universe,
-                                             dummy_name=dummy_name,
-                                             is_loop=is_loop,
-                                             factor_columns=factor_columns,
-                                             industry_name=industry_name,
-                                             industry_level=industry_level,
-                                             model_sets=model_sets,
-                                             factors_normal=factors_normal,
-                                             callback_save=callback_save,
-                                             yield_name=yield_name)
+        super(StockMutation, self).__init__(offset=offset,
+                                            horizon=horizon,
+                                            factor_columns=factor_columns,
+                                            universe=universe,
+                                            yields_class=StkYields,
+                                            universe_class=StkUniverse,
+                                            industry_class=Industry,
+                                            factors_class=StkFactors,
+                                            industry_name=industry_name,
+                                            industry_level=industry_level,
+                                            factors_normal=factors_normal,
+                                            operators=operators,
+                                            yield_name=yield_name)
 
     def industry_fillna(self, industry_data, factors_data):
         factors_data = factors_data.merge(industry_data,
                                           on=['trade_date', 'code'])
         factors_data = self.industry_median(factors_data)
-        return factors_data
+        return factors_data
```

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/geneticist/base.py` & `Finance-Jindowin-1.2.6/jdw/mfc/entropy/catalyst/geneticist/base.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/geneticist/futures.py` & `Finance-Jindowin-1.2.6/jdw/mfc/entropy/catalyst/geneticist/futures.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/geneticist/stock.py` & `Finance-Jindowin-1.2.6/jdw/mfc/entropy/catalyst/geneticist/stock.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/mutation/base.py` & `Finance-Jindowin-1.2.6/jdw/mfc/entropy/catalyst/mutation/base.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/mutation/futures.py` & `Finance-Jindowin-1.2.6/jdw/mfc/entropy/catalyst/mutation/futures.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/mutation/stock.py` & `Finance-Jindowin-1.2.6/jdw/mfc/entropy/pascal/metrics/futures.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 # -*- coding: utf-8 -*-
-from jdw.data.SurfaceAPI.stock.yields import StkYields
-from jdw.data.SurfaceAPI.stock.factors import StkFactors
-from jdw.data.SurfaceAPI.universe import StkUniverse
-from jdw.data.SurfaceAPI.stock.industry import Industry
-from jdw.mfc.entropy.catalyst.mutation.base import Base
+from jdw.data.SurfaceAPI.futures.yields import FutYields
+from jdw.data.SurfaceAPI.futures.factors import FutFactors
+from jdw.data.SurfaceAPI.universe import FutUniverse
+from jdw.data.SurfaceAPI.futures.classify import FutClassify
+from jdw.mfc.entropy.pascal.metrics.base import Base
 
 
-class StockMutation(Base):
+class FuturesMetrics(Base):
 
     def __init__(self,
-                 offset,
-                 horizon,
-                 factor_columns,
                  universe,
+                 factor_columns,
                  industry_name,
                  industry_level,
-                 factors_normal=True,
-                 operators=None,
+                 offset=0,
+                 horizon=0,
+                 factors_data=None,
                  yield_name='returns'):
-        super(StockMutation, self).__init__(offset=offset,
-                                            horizon=horizon,
-                                            factor_columns=factor_columns,
-                                            universe=universe,
-                                            yields_class=StkYields,
-                                            universe_class=StkUniverse,
-                                            industry_class=Industry,
-                                            factors_class=StkFactors,
-                                            industry_name=industry_name,
-                                            industry_level=industry_level,
-                                            factors_normal=factors_normal,
-                                            operators=operators,
-                                            yield_name=yield_name)
+        super().__init__(yields_class=FutYields,
+                         factors_class=FutFactors,
+                         universe_class=FutUniverse,
+                         industry_class=FutClassify,
+                         universe=universe,
+                         offset=offset,
+                         horizon=horizon,
+                         industry_name=industry_name,
+                         industry_level=industry_level,
+                         factor_columns=factor_columns,
+                         factors_data=factors_data,
+                         yield_name=yield_name)
 
     def industry_fillna(self, industry_data, factors_data):
-        factors_data = factors_data.merge(industry_data,
-                                          on=['trade_date', 'code'])
+        factors_data = factors_data.merge(industry_data.drop(['trade_date'],
+                                                             axis=1),
+                                          on=['code'])
         factors_data = self.industry_median(factors_data)
-        return factors_data
+        return factors_data
```

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/carnot/base.py` & `Finance-Jindowin-1.2.6/jdw/mfc/entropy/gravity/carnot/base.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/carnot/futures.py` & `Finance-Jindowin-1.2.6/jdw/mfc/entropy/gravity/carnot/futures.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/carnot/stock.py` & `Finance-Jindowin-1.2.6/jdw/mfc/entropy/gravity/carnot/stock.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/dendall/base.py` & `Finance-Jindowin-1.2.6/jdw/mfc/entropy/gravity/dendall/base.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/dendall/futures.py` & `Finance-Jindowin-1.2.6/jdw/mfc/entropy/gravity/dendall/futures.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/dendall/params.py` & `Finance-Jindowin-1.2.6/jdw/mfc/entropy/gravity/dendall/params.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/dendall/stock.py` & `Finance-Jindowin-1.2.6/jdw/mfc/entropy/gravity/dendall/stock.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/futures/alpha.py` & `Finance-Jindowin-1.2.6/jdw/mfc/entropy/gravity/futures/alpha.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/futures/daily.py` & `Finance-Jindowin-1.2.6/jdw/mfc/entropy/gravity/futures/daily.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/mixture/base copy.py` & `Finance-Jindowin-1.2.6/jdw/mfc/entropy/gravity/mixture/base copy.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/mixture/base.py` & `Finance-Jindowin-1.2.6/jdw/mfc/entropy/gravity/mixture/base.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/mixture/futures.py` & `Finance-Jindowin-1.2.6/jdw/mfc/entropy/gravity/mixture/futures.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/mixture/models.py` & `Finance-Jindowin-1.2.6/jdw/mfc/entropy/gravity/mixture/models.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/mixture/stock.py` & `Finance-Jindowin-1.2.6/jdw/mfc/entropy/gravity/mixture/stock.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/stock/alpha.py` & `Finance-Jindowin-1.2.6/jdw/mfc/entropy/gravity/stock/alpha.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/stock/daily.py` & `Finance-Jindowin-1.2.6/jdw/mfc/entropy/gravity/stock/daily.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/pascal/metrics/base.py` & `Finance-Jindowin-1.2.6/jdw/mfc/entropy/pascal/metrics/base.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/pascal/metrics/futures.py` & `Finance-Jindowin-1.2.6/jdw/mfc/entropy/pascal/score/stock.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 # -*- coding: utf-8 -*-
-from jdw.data.SurfaceAPI.futures.yields import FutYields
-from jdw.data.SurfaceAPI.futures.factors import FutFactors
-from jdw.data.SurfaceAPI.universe import FutUniverse
-from jdw.data.SurfaceAPI.futures.classify import FutClassify
-from jdw.mfc.entropy.pascal.metrics.base import Base
+from jdw.mfc.entropy.pascal.score.base import Base
+from jdw.data.SurfaceAPI.stock.yields import StkYields
+from jdw.data.SurfaceAPI.stock.factors import StkFactors
+from jdw.data.SurfaceAPI.universe import StkUniverse
+from jdw.data.SurfaceAPI.stock.market_stock import MarketStock
+from jdw.data.SurfaceAPI.stock.industry import Industry
 
 
-class FuturesMetrics(Base):
+class StockScore(Base):
 
     def __init__(self,
                  universe,
                  factor_columns,
                  industry_name,
                  industry_level,
                  offset=0,
                  horizon=0,
+                 score_class=None,
                  factors_data=None,
+                 weights=None,
                  yield_name='returns'):
-        super().__init__(yields_class=FutYields,
-                         factors_class=FutFactors,
-                         universe_class=FutUniverse,
-                         industry_class=FutClassify,
-                         universe=universe,
-                         offset=offset,
-                         horizon=horizon,
-                         industry_name=industry_name,
-                         industry_level=industry_level,
-                         factor_columns=factor_columns,
-                         factors_data=factors_data,
-                         yield_name=yield_name)
+        super(StockScore, self).__init__(yields_class=StkYields,
+                                         factors_class=StkFactors,
+                                         industry_class=Industry,
+                                         universe_class=StkUniverse,
+                                         universe=universe,
+                                         offset=offset,
+                                         horizon=horizon,
+                                         factor_columns=factor_columns,
+                                         industry_name=industry_name,
+                                         industry_level=industry_level,
+                                         score_class=score_class,
+                                         factors_data=factors_data,
+                                         weights=weights,
+                                         yield_name=yield_name)
 
     def industry_fillna(self, industry_data, factors_data):
-        factors_data = factors_data.merge(industry_data.drop(['trade_date'],
-                                                             axis=1),
-                                          on=['code'])
+        factors_data = factors_data.merge(industry_data,
+                                          on=['trade_date', 'code'])
         factors_data = self.industry_median(factors_data)
         return factors_data
```

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/pascal/metrics/stock.py` & `Finance-Jindowin-1.2.6/jdw/mfc/entropy/pascal/metrics/stock.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/pascal/score/base.py` & `Finance-Jindowin-1.2.6/jdw/mfc/entropy/pascal/score/base.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/pascal/score/futures.py` & `Finance-Jindowin-1.2.6/jdw/mfc/entropy/pascal/score/futures.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/pascal/score/stock.py` & `Finance-Jindowin-1.2.6/jdw/mfc/entropy/catalyst/evolution/stock.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,53 @@
 # -*- coding: utf-8 -*-
-from jdw.mfc.entropy.pascal.score.base import Base
 from jdw.data.SurfaceAPI.stock.yields import StkYields
 from jdw.data.SurfaceAPI.stock.factors import StkFactors
 from jdw.data.SurfaceAPI.universe import StkUniverse
-from jdw.data.SurfaceAPI.stock.market_stock import MarketStock
 from jdw.data.SurfaceAPI.stock.industry import Industry
+from jdw.data.SurfaceAPI.dummy import Dummy
+from jdw.mfc.entropy.catalyst.evolution.base import Base
 
 
-class StockScore(Base):
+class StockEvolution(Base):
 
     def __init__(self,
+                 thresh,
                  universe,
                  factor_columns,
                  industry_name,
                  industry_level,
+                 is_weighted=True,
+                 dummy_name=None,
+                 is_loop=False,
                  offset=0,
                  horizon=0,
-                 score_class=None,
-                 factors_data=None,
-                 weights=None,
+                 model_sets=None,
+                 params_sets={},
+                 factors_normal=True,
+                 callback_save=None,
                  yield_name='returns'):
-        super(StockScore, self).__init__(yields_class=StkYields,
-                                         factors_class=StkFactors,
-                                         industry_class=Industry,
-                                         universe_class=StkUniverse,
-                                         universe=universe,
-                                         offset=offset,
-                                         horizon=horizon,
-                                         factor_columns=factor_columns,
-                                         industry_name=industry_name,
-                                         industry_level=industry_level,
-                                         score_class=score_class,
-                                         factors_data=factors_data,
-                                         weights=weights,
-                                         yield_name=yield_name)
+        super(StockEvolution, self).__init__(yields_class=StkYields,
+                                             factors_class=StkFactors,
+                                             universe_class=StkUniverse,
+                                             industry_class=Industry,
+                                             dummy_class=Dummy,
+                                             is_weighted=is_weighted,
+                                             thresh=thresh,
+                                             offset=offset,
+                                             horizon=horizon,
+                                             universe=universe,
+                                             dummy_name=dummy_name,
+                                             is_loop=is_loop,
+                                             factor_columns=factor_columns,
+                                             industry_name=industry_name,
+                                             industry_level=industry_level,
+                                             model_sets=model_sets,
+                                             params_sets=params_sets,
+                                             factors_normal=factors_normal,
+                                             callback_save=callback_save,
+                                             yield_name=yield_name)
 
     def industry_fillna(self, industry_data, factors_data):
         factors_data = factors_data.merge(industry_data,
                                           on=['trade_date', 'code'])
         factors_data = self.industry_median(factors_data)
         return factors_data
```

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/experimental/DataAPI/mg/atl/engine.py` & `Finance-Jindowin-1.2.6/jdw/mfc/experimental/DataAPI/mg/atl/engine.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/experimental/DataAPI/mg/mg_factory.py` & `Finance-Jindowin-1.2.6/jdw/mfc/experimental/DataAPI/mg/mg_factory.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/experimental/DataAPI/mg/ntn/engine.py` & `Finance-Jindowin-1.2.6/jdw/mfc/experimental/DataAPI/mg/ntn/engine.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/experimental/DataAPI/mg/operator_engine.py` & `Finance-Jindowin-1.2.6/jdw/mfc/experimental/DataAPI/mg/operator_engine.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/irey/kestle.py` & `Finance-Jindowin-1.2.6/jdw/mfc/irey/kestle.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/lombard/base.py` & `Finance-Jindowin-1.2.6/jdw/mfc/lombard/base.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/lombard/futures.py` & `Finance-Jindowin-1.2.6/jdw/mfc/lombard/futures.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/lombard/indicator/atr.py` & `Finance-Jindowin-1.2.6/jdw/mfc/lombard/indicator/atr.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/lombard/indicator/base.py` & `Finance-Jindowin-1.2.6/jdw/mfc/lombard/indicator/base.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/lombard/indicator/date.py` & `Finance-Jindowin-1.2.6/jdw/mfc/lombard/indicator/date.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/lombard/indicator/symbol_pd.py` & `Finance-Jindowin-1.2.6/jdw/mfc/lombard/indicator/symbol_pd.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/lombard/stock.py` & `Finance-Jindowin-1.2.6/jdw/mfc/lombard/stock.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/neutron/analysis.py` & `Finance-Jindowin-1.2.6/jdw/mfc/neutron/analysis.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/neutron/factory.py` & `Finance-Jindowin-1.2.6/jdw/mfc/neutron/factory.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/neutron/strategy.py` & `Finance-Jindowin-1.2.6/jdw/mfc/neutron/strategy.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/neutron/trader.py` & `Finance-Jindowin-1.2.6/jdw/mfc/neutron/trader.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/mfc/oss/aliyun.py` & `Finance-Jindowin-1.2.6/jdw/mfc/oss/aliyun.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/plot/STOCK/detail.py` & `Finance-Jindowin-1.2.6/jdw/plot/STOCK/detail.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/plot/STOCK/flow_money.py` & `Finance-Jindowin-1.2.6/jdw/plot/STOCK/flow_money.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/plot/STOCK/hkshshz.py` & `Finance-Jindowin-1.2.6/jdw/plot/STOCK/hkshshz.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/plot/STOCK/sentiment.py` & `Finance-Jindowin-1.2.6/jdw/plot/STOCK/sentiment.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/plot/THEME/brief.py` & `Finance-Jindowin-1.2.6/jdw/plot/THEME/brief.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/plot/THEME/detail.py` & `Finance-Jindowin-1.2.6/jdw/plot/THEME/detail.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/plot/THEME/flow_money.py` & `Finance-Jindowin-1.2.6/jdw/plot/THEME/flow_money.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/plot/THEME/hkshshz.py` & `Finance-Jindowin-1.2.6/jdw/plot/THEME/hkshshz.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/plot/THEME/indicators.py` & `Finance-Jindowin-1.2.6/jdw/plot/THEME/indicators.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/plot/THEME/returns.py` & `Finance-Jindowin-1.2.6/jdw/plot/THEME/returns.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/plot/THEME/sentiment.py` & `Finance-Jindowin-1.2.6/jdw/plot/THEME/sentiment.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/plot/__init__.py` & `Finance-Jindowin-1.2.6/jdw/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/plot/returns.py` & `Finance-Jindowin-1.2.6/jdw/plot/returns.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/plot/stock.py` & `Finance-Jindowin-1.2.6/jdw/plot/stock.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/to_pandas.py` & `Finance-Jindowin-1.2.6/jdw/to_pandas.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/jdw/utils.py` & `Finance-Jindowin-1.2.6/jdw/utils.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5.1/setup.py` & `Finance-Jindowin-1.2.6/setup.py`

 * *Files identical despite different names*

