# Comparing `tmp/psdm-analysis-0.1.5.tar.gz` & `tmp/psdm-analysis-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psdm-analysis-0.1.5.tar", max compression
+gzip compressed data, was "psdm-analysis-0.1.6.tar", max compression
```

## Comparing `psdm-analysis-0.1.5.tar` & `psdm-analysis-0.1.6.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0     1581 2023-01-31 09:55:39.404671 psdm-analysis-0.1.5/LICENSE
--rw-r--r--   0        0        0      373 2023-04-19 12:49:15.037328 psdm-analysis-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.038177 psdm-analysis-0.1.5/psdm_analysis/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.038287 psdm-analysis-0.1.5/psdm_analysis/analysis/__init__.py
--rw-r--r--   0        0        0      601 2023-04-19 12:49:15.038571 psdm-analysis-0.1.5/psdm_analysis/analysis/calc.py
--rw-r--r--   0        0        0     1200 2023-04-19 12:49:15.038918 psdm-analysis-0.1.5/psdm_analysis/analysis/grid.py
--rw-r--r--   0        0        0        0 2023-05-02 07:38:45.729757 psdm-analysis-0.1.5/psdm_analysis/conversion/__init__.py
--rw-r--r--   0        0        0     3960 2023-05-02 07:38:45.730387 psdm-analysis-0.1.5/psdm_analysis/conversion/pandapower.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.038964 psdm-analysis-0.1.5/psdm_analysis/io/__init__.py
--rw-r--r--   0        0        0     2842 2023-04-19 12:49:15.039092 psdm-analysis-0.1.5/psdm_analysis/io/utils.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.039122 psdm-analysis-0.1.5/psdm_analysis/models/__init__.py
--rw-r--r--   0        0        0     9503 2023-05-23 11:13:37.867698 psdm-analysis-0.1.5/psdm_analysis/models/entity.py
--rw-r--r--   0        0        0     6788 2023-05-30 12:42:51.429533 psdm-analysis-0.1.5/psdm_analysis/models/grid_with_results.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.039422 psdm-analysis-0.1.5/psdm_analysis/models/input/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.039466 psdm-analysis-0.1.5/psdm_analysis/models/input/connector/__init__.py
--rw-r--r--   0        0        0     1329 2023-05-30 12:42:56.398213 psdm-analysis-0.1.5/psdm_analysis/models/input/connector/connector.py
--rw-r--r--   0        0        0     1888 2023-05-23 11:13:37.869005 psdm-analysis-0.1.5/psdm_analysis/models/input/connector/lines.py
--rw-r--r--   0        0        0      779 2023-05-30 12:42:56.398558 psdm-analysis-0.1.5/psdm_analysis/models/input/connector/switches.py
--rw-r--r--   0        0        0     2240 2023-05-29 07:50:38.432624 psdm-analysis-0.1.5/psdm_analysis/models/input/connector/transformer.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.040065 psdm-analysis-0.1.5/psdm_analysis/models/input/container/__init__.py
--rw-r--r--   0        0        0     6786 2023-05-30 12:42:51.429869 psdm-analysis-0.1.5/psdm_analysis/models/input/container/grid_container.py
--rw-r--r--   0        0        0     3456 2023-05-04 10:09:12.848994 psdm-analysis-0.1.5/psdm_analysis/models/input/container/mixins.py
--rw-r--r--   0        0        0     6312 2023-05-23 11:13:37.870997 psdm-analysis-0.1.5/psdm_analysis/models/input/container/participants_container.py
--rw-r--r--   0        0        0     3134 2023-05-23 11:13:37.871280 psdm-analysis-0.1.5/psdm_analysis/models/input/enums.py
--rw-r--r--   0        0        0     1365 2023-05-23 11:13:37.871527 psdm-analysis-0.1.5/psdm_analysis/models/input/node.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.041104 psdm-analysis-0.1.5/psdm_analysis/models/input/participant/__init__.py
--rw-r--r--   0        0        0     1368 2023-04-19 12:49:15.041213 psdm-analysis-0.1.5/psdm_analysis/models/input/participant/bm.py
--rw-r--r--   0        0        0     3138 2023-04-19 12:49:15.041309 psdm-analysis-0.1.5/psdm_analysis/models/input/participant/charging.py
--rw-r--r--   0        0        0      654 2023-04-19 12:49:15.041628 psdm-analysis-0.1.5/psdm_analysis/models/input/participant/em.py
--rw-r--r--   0        0        0      936 2023-04-19 12:49:15.041802 psdm-analysis-0.1.5/psdm_analysis/models/input/participant/evcs.py
--rw-r--r--   0        0        0      965 2023-04-19 12:49:15.041899 psdm-analysis-0.1.5/psdm_analysis/models/input/participant/evs.py
--rw-r--r--   0        0        0      527 2023-04-19 12:49:15.042031 psdm-analysis-0.1.5/psdm_analysis/models/input/participant/fixed_feed_in.py
--rw-r--r--   0        0        0      813 2023-05-23 11:13:37.872710 psdm-analysis-0.1.5/psdm_analysis/models/input/participant/hp.py
--rw-r--r--   0        0        0      953 2023-04-19 12:49:15.042385 psdm-analysis-0.1.5/psdm_analysis/models/input/participant/load.py
--rw-r--r--   0        0        0     1266 2023-05-23 11:13:37.873708 psdm-analysis-0.1.5/psdm_analysis/models/input/participant/participant.py
--rw-r--r--   0        0        0     1320 2023-04-19 12:49:15.042694 psdm-analysis-0.1.5/psdm_analysis/models/input/participant/pv.py
--rw-r--r--   0        0        0     1527 2023-04-19 12:49:15.042799 psdm-analysis-0.1.5/psdm_analysis/models/input/participant/storage.py
--rw-r--r--   0        0        0     1113 2023-04-19 12:49:15.042895 psdm-analysis-0.1.5/psdm_analysis/models/input/participant/wec.py
--rw-r--r--   0        0        0     4354 2023-05-23 11:13:37.874172 psdm-analysis-0.1.5/psdm_analysis/models/primary_data.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.043156 psdm-analysis-0.1.5/psdm_analysis/models/result/__init__.py
--rw-r--r--   0        0        0     2243 2023-04-19 12:49:15.043509 psdm-analysis-0.1.5/psdm_analysis/models/result/flex_option.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.043543 psdm-analysis-0.1.5/psdm_analysis/models/result/grid/__init__.py
--rw-r--r--   0        0        0     2842 2023-05-23 11:13:37.874372 psdm-analysis-0.1.5/psdm_analysis/models/result/grid/connector.py
--rw-r--r--   0        0        0     2284 2023-05-30 12:42:51.430207 psdm-analysis-0.1.5/psdm_analysis/models/result/grid/enhanced_node.py
--rw-r--r--   0        0        0     2626 2023-05-30 12:42:51.430763 psdm-analysis-0.1.5/psdm_analysis/models/result/grid/node.py
--rw-r--r--   0        0        0     1701 2023-05-23 11:13:37.875468 psdm-analysis-0.1.5/psdm_analysis/models/result/grid/transformer.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.043823 psdm-analysis-0.1.5/psdm_analysis/models/result/participant/__init__.py
--rw-r--r--   0        0        0     6696 2023-05-30 12:42:51.431347 psdm-analysis-0.1.5/psdm_analysis/models/result/participant/dict.py
--rw-r--r--   0        0        0     3170 2023-04-19 12:49:15.044163 psdm-analysis-0.1.5/psdm_analysis/models/result/participant/flex_options.py
--rw-r--r--   0        0        0     3619 2023-05-30 12:42:51.431649 psdm-analysis-0.1.5/psdm_analysis/models/result/participant/participant.py
--rw-r--r--   0        0        0    10556 2023-05-26 09:57:21.675417 psdm-analysis-0.1.5/psdm_analysis/models/result/participant/participants_res_container.py
--rw-r--r--   0        0        0     5842 2023-05-23 11:13:37.877331 psdm-analysis-0.1.5/psdm_analysis/models/result/power.py
--rw-r--r--   0        0        0     4499 2023-05-23 11:13:37.878078 psdm-analysis-0.1.5/psdm_analysis/models/result/res_container.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.044717 psdm-analysis-0.1.5/psdm_analysis/plots/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 11:13:37.878152 psdm-analysis-0.1.5/psdm_analysis/plots/common/__init__.py
--rw-r--r--   0        0        0     2431 2023-05-23 11:13:37.878287 psdm-analysis-0.1.5/psdm_analysis/plots/common/bar_plot.py
--rw-r--r--   0        0        0     1103 2023-05-23 11:13:37.878583 psdm-analysis-0.1.5/psdm_analysis/plots/common/line_plot.py
--rw-r--r--   0        0        0     5500 2023-05-30 12:42:51.432073 psdm-analysis-0.1.5/psdm_analysis/plots/common/utils.py
--rw-r--r--   0        0        0     4128 2023-05-23 11:13:37.879462 psdm-analysis-0.1.5/psdm_analysis/plots/grid.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.044851 psdm-analysis-0.1.5/psdm_analysis/plots/results/__init__.py
--rw-r--r--   0        0        0     6143 2023-05-23 11:13:37.879649 psdm-analysis-0.1.5/psdm_analysis/plots/results/connector_plot.py
--rw-r--r--   0        0        0     3467 2023-05-23 11:13:37.880115 psdm-analysis-0.1.5/psdm_analysis/plots/results/flex_plot.py
--rw-r--r--   0        0        0     1083 2023-04-19 12:49:15.045811 psdm-analysis-0.1.5/psdm_analysis/plots/results/nodes.py
--rw-r--r--   0        0        0    11960 2023-05-23 11:13:37.880667 psdm-analysis-0.1.5/psdm_analysis/plots/results/power_plot.py
--rw-r--r--   0        0        0     7726 2023-05-30 12:42:51.432565 psdm-analysis-0.1.5/psdm_analysis/plots/results/voltage_plot.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.046127 psdm-analysis-0.1.5/psdm_analysis/processing/__init__.py
--rw-r--r--   0        0        0     1217 2023-05-04 10:44:30.440027 psdm-analysis-0.1.5/psdm_analysis/processing/dataframe.py
--rw-r--r--   0        0        0     2174 2023-04-19 12:49:15.046324 psdm-analysis-0.1.5/psdm_analysis/processing/series.py
--rw-r--r--   0        0        0      789 2023-05-30 13:16:04.964764 psdm-analysis-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1799 1970-01-01 00:00:00.000000 psdm-analysis-0.1.5/setup.py
--rw-r--r--   0        0        0     1156 1970-01-01 00:00:00.000000 psdm-analysis-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1581 2023-01-31 09:55:39.404671 psdm-analysis-0.1.6/LICENSE
+-rw-r--r--   0        0        0      373 2023-04-19 12:49:15.037328 psdm-analysis-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.038177 psdm-analysis-0.1.6/psdm_analysis/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.038287 psdm-analysis-0.1.6/psdm_analysis/analysis/__init__.py
+-rw-r--r--   0        0        0      601 2023-04-19 12:49:15.038571 psdm-analysis-0.1.6/psdm_analysis/analysis/calc.py
+-rw-r--r--   0        0        0     1200 2023-06-01 14:41:34.770255 psdm-analysis-0.1.6/psdm_analysis/analysis/grid.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:41:34.770303 psdm-analysis-0.1.6/psdm_analysis/conversion/__init__.py
+-rw-r--r--   0        0        0     3960 2023-06-01 14:41:34.770476 psdm-analysis-0.1.6/psdm_analysis/conversion/pandapower.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.038964 psdm-analysis-0.1.6/psdm_analysis/io/__init__.py
+-rw-r--r--   0        0        0     2842 2023-06-01 14:41:34.770725 psdm-analysis-0.1.6/psdm_analysis/io/utils.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.039122 psdm-analysis-0.1.6/psdm_analysis/models/__init__.py
+-rw-r--r--   0        0        0    11089 2023-06-01 14:41:34.770997 psdm-analysis-0.1.6/psdm_analysis/models/entity.py
+-rw-r--r--   0        0        0     6788 2023-06-01 14:41:34.771211 psdm-analysis-0.1.6/psdm_analysis/models/grid_with_results.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.039422 psdm-analysis-0.1.6/psdm_analysis/models/input/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.039466 psdm-analysis-0.1.6/psdm_analysis/models/input/connector/__init__.py
+-rw-r--r--   0        0        0     1329 2023-06-01 14:41:34.771364 psdm-analysis-0.1.6/psdm_analysis/models/input/connector/connector.py
+-rw-r--r--   0        0        0     3054 2023-06-01 14:41:34.771548 psdm-analysis-0.1.6/psdm_analysis/models/input/connector/lines.py
+-rw-r--r--   0        0        0      728 2023-06-01 14:41:34.771672 psdm-analysis-0.1.6/psdm_analysis/models/input/connector/switches.py
+-rw-r--r--   0        0        0     2189 2023-06-01 14:41:34.771884 psdm-analysis-0.1.6/psdm_analysis/models/input/connector/transformer.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.040065 psdm-analysis-0.1.6/psdm_analysis/models/input/container/__init__.py
+-rw-r--r--   0        0        0     6786 2023-06-01 14:41:34.772117 psdm-analysis-0.1.6/psdm_analysis/models/input/container/grid_container.py
+-rw-r--r--   0        0        0     3456 2023-06-01 14:41:34.772254 psdm-analysis-0.1.6/psdm_analysis/models/input/container/mixins.py
+-rw-r--r--   0        0        0     6312 2023-06-01 14:41:34.772447 psdm-analysis-0.1.6/psdm_analysis/models/input/container/participants_container.py
+-rw-r--r--   0        0        0     3134 2023-06-01 14:41:34.772640 psdm-analysis-0.1.6/psdm_analysis/models/input/enums.py
+-rw-r--r--   0        0        0     1365 2023-06-01 14:41:34.772819 psdm-analysis-0.1.6/psdm_analysis/models/input/node.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.041104 psdm-analysis-0.1.6/psdm_analysis/models/input/participant/__init__.py
+-rw-r--r--   0        0        0     1368 2023-06-01 14:41:34.773031 psdm-analysis-0.1.6/psdm_analysis/models/input/participant/bm.py
+-rw-r--r--   0        0        0     3138 2023-06-01 14:41:34.773220 psdm-analysis-0.1.6/psdm_analysis/models/input/participant/charging.py
+-rw-r--r--   0        0        0      654 2023-06-01 14:41:34.773387 psdm-analysis-0.1.6/psdm_analysis/models/input/participant/em.py
+-rw-r--r--   0        0        0      936 2023-06-01 14:41:34.773553 psdm-analysis-0.1.6/psdm_analysis/models/input/participant/evcs.py
+-rw-r--r--   0        0        0      965 2023-06-01 14:41:34.773740 psdm-analysis-0.1.6/psdm_analysis/models/input/participant/evs.py
+-rw-r--r--   0        0        0      527 2023-06-01 14:41:34.773941 psdm-analysis-0.1.6/psdm_analysis/models/input/participant/fixed_feed_in.py
+-rw-r--r--   0        0        0      813 2023-06-01 14:41:34.774110 psdm-analysis-0.1.6/psdm_analysis/models/input/participant/hp.py
+-rw-r--r--   0        0        0      953 2023-06-01 14:41:34.774290 psdm-analysis-0.1.6/psdm_analysis/models/input/participant/load.py
+-rw-r--r--   0        0        0     1266 2023-06-01 14:41:34.774470 psdm-analysis-0.1.6/psdm_analysis/models/input/participant/participant.py
+-rw-r--r--   0        0        0     1320 2023-06-01 14:41:34.774653 psdm-analysis-0.1.6/psdm_analysis/models/input/participant/pv.py
+-rw-r--r--   0        0        0     1527 2023-06-01 14:41:34.774822 psdm-analysis-0.1.6/psdm_analysis/models/input/participant/storage.py
+-rw-r--r--   0        0        0     1113 2023-06-01 14:41:34.774986 psdm-analysis-0.1.6/psdm_analysis/models/input/participant/wec.py
+-rw-r--r--   0        0        0     4354 2023-06-01 14:41:34.775171 psdm-analysis-0.1.6/psdm_analysis/models/primary_data.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.043156 psdm-analysis-0.1.6/psdm_analysis/models/result/__init__.py
+-rw-r--r--   0        0        0     2243 2023-04-19 12:49:15.043509 psdm-analysis-0.1.6/psdm_analysis/models/result/flex_option.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.043543 psdm-analysis-0.1.6/psdm_analysis/models/result/grid/__init__.py
+-rw-r--r--   0        0        0     2842 2023-06-01 14:41:34.775326 psdm-analysis-0.1.6/psdm_analysis/models/result/grid/connector.py
+-rw-r--r--   0        0        0     2284 2023-06-01 14:41:34.775503 psdm-analysis-0.1.6/psdm_analysis/models/result/grid/enhanced_node.py
+-rw-r--r--   0        0        0     2626 2023-06-01 14:41:34.775678 psdm-analysis-0.1.6/psdm_analysis/models/result/grid/node.py
+-rw-r--r--   0        0        0     1701 2023-06-01 14:41:34.775806 psdm-analysis-0.1.6/psdm_analysis/models/result/grid/transformer.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.043823 psdm-analysis-0.1.6/psdm_analysis/models/result/participant/__init__.py
+-rw-r--r--   0        0        0     6696 2023-06-02 06:58:54.263274 psdm-analysis-0.1.6/psdm_analysis/models/result/participant/dict.py
+-rw-r--r--   0        0        0     3170 2023-04-19 12:49:15.044163 psdm-analysis-0.1.6/psdm_analysis/models/result/participant/flex_options.py
+-rw-r--r--   0        0        0     3619 2023-06-01 14:41:34.776241 psdm-analysis-0.1.6/psdm_analysis/models/result/participant/participant.py
+-rw-r--r--   0        0        0    10556 2023-06-01 14:41:34.776478 psdm-analysis-0.1.6/psdm_analysis/models/result/participant/participants_res_container.py
+-rw-r--r--   0        0        0     5842 2023-06-01 14:41:34.776674 psdm-analysis-0.1.6/psdm_analysis/models/result/power.py
+-rw-r--r--   0        0        0     4499 2023-06-01 14:41:34.776876 psdm-analysis-0.1.6/psdm_analysis/models/result/res_container.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.044717 psdm-analysis-0.1.6/psdm_analysis/plots/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:41:34.776929 psdm-analysis-0.1.6/psdm_analysis/plots/common/__init__.py
+-rw-r--r--   0        0        0     2431 2023-06-01 14:41:34.777070 psdm-analysis-0.1.6/psdm_analysis/plots/common/bar_plot.py
+-rw-r--r--   0        0        0     1103 2023-06-01 14:41:34.777209 psdm-analysis-0.1.6/psdm_analysis/plots/common/line_plot.py
+-rw-r--r--   0        0        0     5500 2023-06-01 14:41:34.777594 psdm-analysis-0.1.6/psdm_analysis/plots/common/utils.py
+-rw-r--r--   0        0        0     4128 2023-06-01 14:41:34.777725 psdm-analysis-0.1.6/psdm_analysis/plots/grid.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.044851 psdm-analysis-0.1.6/psdm_analysis/plots/results/__init__.py
+-rw-r--r--   0        0        0     6143 2023-06-01 14:41:34.777859 psdm-analysis-0.1.6/psdm_analysis/plots/results/connector_plot.py
+-rw-r--r--   0        0        0     3467 2023-06-01 14:41:34.778051 psdm-analysis-0.1.6/psdm_analysis/plots/results/flex_plot.py
+-rw-r--r--   0        0        0     1083 2023-04-19 12:49:15.045811 psdm-analysis-0.1.6/psdm_analysis/plots/results/nodes.py
+-rw-r--r--   0        0        0    11960 2023-06-01 14:41:34.778248 psdm-analysis-0.1.6/psdm_analysis/plots/results/power_plot.py
+-rw-r--r--   0        0        0     7726 2023-06-01 14:41:34.778390 psdm-analysis-0.1.6/psdm_analysis/plots/results/voltage_plot.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.046127 psdm-analysis-0.1.6/psdm_analysis/processing/__init__.py
+-rw-r--r--   0        0        0     1217 2023-06-01 14:41:34.778551 psdm-analysis-0.1.6/psdm_analysis/processing/dataframe.py
+-rw-r--r--   0        0        0     2174 2023-06-01 14:41:34.778712 psdm-analysis-0.1.6/psdm_analysis/processing/series.py
+-rw-r--r--   0        0        0      789 2023-06-02 06:59:24.517952 psdm-analysis-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1799 1970-01-01 00:00:00.000000 psdm-analysis-0.1.6/setup.py
+-rw-r--r--   0        0        0     1156 1970-01-01 00:00:00.000000 psdm-analysis-0.1.6/PKG-INFO
```

### Comparing `psdm-analysis-0.1.5/LICENSE` & `psdm-analysis-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/psdm_analysis/analysis/calc.py` & `psdm-analysis-0.1.6/psdm_analysis/analysis/calc.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/psdm_analysis/analysis/grid.py` & `psdm-analysis-0.1.6/psdm_analysis/analysis/grid.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/psdm_analysis/conversion/pandapower.py` & `psdm-analysis-0.1.6/psdm_analysis/conversion/pandapower.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/psdm_analysis/io/utils.py` & `psdm-analysis-0.1.6/psdm_analysis/io/utils.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/psdm_analysis/models/entity.py` & `psdm-analysis-0.1.6/psdm_analysis/models/entity.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,30 +30,113 @@
 @dataclass(frozen=True)
 class Entities(ABC):
     data: DataFrame
 
     def __len__(self):
         return len(self.data)
 
+    def __repr__(self):
+        return self.data
+
     def __contains__(self, uuid: str):
         return uuid in self.data.index
 
-    @classmethod
-    def from_csv(cls, path: str, delimiter: str):
-        return cls._from_csv(path, delimiter, cls.get_enum())
+    def __add__(self: EntityType, other: EntityType) -> EntityType:
+        """
+        Concatenates two Entities instances.
+
+        Args:
+            other: The other Entities instance to concatenate with.
+
+        Returns:
+            The concatenated Entities instance.
+        """
+        columns_diff = set(self.data.columns).symmetric_difference(other.data.columns)
+        if columns_diff:
+            raise ValueError(
+                f"Columns of the dataframes are not the same: {columns_diff}"
+            )
+        else:
+            return type(self)(pd.concat([self.data, other.data]))
+
+    def __sub__(self: EntityType, other: Union[EntityType, List[str]]) -> EntityType:
+        """
+        Subtacts the entities with the given uuids from the Entities instance.
+
+        Args:
+            other: The other Entities instance or a list of uuids to subtract.
+
+        Returns:
+            A new Entities instance with the uuids removed.
+        """
+        if isinstance(other, Entities):
+            indices_to_remove = other.data.index
+        elif isinstance(other, list) and all(isinstance(index, str) for index in other):
+            indices_to_remove = other
+        else:
+            raise TypeError("other must be an Entities instance or a list of strings")
+
+        if not set(indices_to_remove).issubset(self.data.index):
+            raise ValueError(
+                f"All indices to remove must exist in the current Entities instance: {set(indices_to_remove) - set(self.data.index)}"
+            )
+
+        return type(self)(self.data.drop(indices_to_remove))
+
+    @property
+    def uuids(self):
+        return self.data.index
+
+    @property
+    def ids(self):
+        return self.data["id"]
+
+    @property
+    def operates_from(self):
+        return self.data["operates_from"]
+
+    @property
+    def operates_until(self):
+        return self.data["operates_until"]
+
+    @property
+    def operator(self):
+        return self.data["operator"]
 
-    @staticmethod
     @abstractmethod
-    def get_enum() -> EntitiesEnum:
+    def nodes(self):
         pass
 
+    def get(self, uuid: str) -> Series:
+        return self.data.loc[uuid]
+
+    def subset(self, uuids: Union[list[str], str]):
+        if isinstance(uuids, str):
+            uuids = [uuids]
+        return type(self)(self.data.loc[uuids])
+
+    def subset_split(self, uuids: list[str]):
+        rmd = set(self.uuids) - set(uuids)
+        return self.subset(uuids), self.subset(list(rmd))
+
+    def filter_for_node(self, uuid: str):
+        data = self.data[self.nodes() == str(uuid)]
+        return type(self)(data)
+
+    def find_nodes(self, nodes: Nodes) -> Nodes:
+        return nodes.subset(self.nodes())
+
     def to_csv(self, path: str, delimiter: str = ","):
         df_to_csv(self.data, path, self.get_enum().get_csv_input_file_name(), delimiter)
 
     @classmethod
+    def from_csv(cls, path: str, delimiter: str):
+        return cls._from_csv(path, delimiter, cls.get_enum())
+
+    @classmethod
     def _from_csv(cls, path: str, delimiter: str, entity: EntitiesEnum):
         file_path = utils.get_file_path(path, entity.get_csv_input_file_name())
         if os.path.exists(file_path):
             return cls(Entities._data_from_csv(entity, path, delimiter))
         else:
             logging.debug(
                 "There is no file named: "
@@ -101,74 +184,33 @@
         try:
             return data.set_index("uuid")
         except KeyError as e:
             raise KeyError(
                 "Column 'uuid' not found. This might be due to wrong csv delimiter!", e
             )
 
-    @property
-    def uuids(self):
-        return self.data.index
-
-    @property
-    def ids(self):
-        return self.data["id"]
-
-    @property
-    def operates_from(self):
-        return self.data["operates_from"]
-
-    @property
-    def operates_until(self):
-        return self.data["operates_until"]
-
-    @property
-    def operator(self):
-        return self.data["operator"]
-
-    def __repr__(self):
-        return self.data
+    @classmethod
+    def create_empty(cls):
+        data = pd.DataFrame(columns=cls.attributes())
+        return cls(data)
 
-    def get(self, uuid: str) -> Series:
-        return self.data.loc[uuid]
+    @staticmethod
+    @abstractmethod
+    def get_enum() -> EntitiesEnum:
+        pass
 
     @staticmethod
     def attributes() -> List[str]:
         """
         Method that should hold all attributes field (transformed to snake_case and case-sensitive)
         of the corresponding PSDM entity
         :return:
         """
         return ["uuid", "id", "operates_from", "operates_until", "operator"]
 
-    @classmethod
-    def create_empty(cls):
-        data = pd.DataFrame(columns=cls.attributes())
-        return cls(data)
-
-    def subset(self, uuids: Union[list[str], str]):
-        if isinstance(uuids, str):
-            uuids = [uuids]
-        return type(self)(self.data.loc[uuids])
-
-    def subset_split(self, uuids: list[str]):
-        rmd = set(self.uuids) - set(uuids)
-        return self.subset(uuids), self.subset(list(rmd))
-
-    @abstractmethod
-    def nodes(self):
-        pass
-
-    def filter_for_node(self, uuid: str):
-        data = self.data[self.nodes() == str(uuid)]
-        return type(self)(data)
-
-    def find_nodes(self, nodes: Nodes) -> Nodes:
-        return nodes.subset(self.nodes())
-
 
 ResultType = TypeVar("ResultType", bound="ResultEntities")
 
 
 @dataclass(frozen=True)
 class ResultEntities(ABC):
     # todo: type is a reserved keyword -> rename
```

### Comparing `psdm-analysis-0.1.5/psdm_analysis/models/grid_with_results.py` & `psdm-analysis-0.1.6/psdm_analysis/models/grid_with_results.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/psdm_analysis/models/input/connector/connector.py` & `psdm-analysis-0.1.6/psdm_analysis/models/input/connector/connector.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/psdm_analysis/models/input/connector/lines.py` & `psdm-analysis-0.1.6/psdm_analysis/models/input/participant/storage.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,75 +1,63 @@
-from dataclasses import dataclass
-from typing import List
+from pandas import Series
 
-from pandas import DataFrame, Series
+from psdm_analysis.models.input.container.mixins import SpTypeMixin
+from psdm_analysis.models.input.enums import SystemParticipantsEnum
+from psdm_analysis.models.input.participant.participant import (
+    SystemParticipantsWithCapacity,
+)
 
-from psdm_analysis.models.input.connector.connector import Connector
-from psdm_analysis.models.input.container.mixins import HasTypeMixin
-from psdm_analysis.models.input.enums import RawGridElementsEnum
-
-
-@dataclass(frozen=True)
-class Lines(Connector, HasTypeMixin):
-    data: DataFrame
 
+class Storages(SystemParticipantsWithCapacity, SpTypeMixin):
     @staticmethod
-    def get_enum() -> RawGridElementsEnum:
-        return RawGridElementsEnum.LINE
+    def get_enum() -> SystemParticipantsEnum:
+        return SystemParticipantsEnum.STORAGE
 
     @property
-    def length(self) -> Series:
-        return self.data["length"]
+    def behaviour(self) -> Series:
+        return self.data["behaviour"]
 
-    @property
-    def geo_position(self) -> Series:
-        return self.data["geo_position"]
+    @staticmethod
+    def capacity_attribute() -> str:
+        return "e_storage"
 
     @property
-    def olm_characteristic(self) -> Series:
-        return self.data["olm_characteristic"]
+    def p_max(self) -> Series:
+        return self.data["p_max"]
 
     @property
-    def v_rated(self) -> Series:
-        return self.data["v_rated"]
+    def active_power_gradient(self) -> Series:
+        return self.data["active_power_gradient"]
 
     @property
-    def r(self) -> Series:
-        return self.data["r"]
+    def eta(self) -> Series:
+        return self.data["eta"]
 
     @property
-    def x(self) -> Series:
-        return self.data["x"]
+    def dod(self) -> Series:
+        return self.data["dod"]
 
     @property
-    def b(self) -> Series:
-        return self.data["b"]
+    def life_time(self) -> Series:
+        return self.data["life_time"]
 
     @property
-    def i_max(self) -> Series:
-        return self.data["i_max"]
+    def life_cycle(self) -> Series:
+        return self.data["life_cycle"]
 
     @staticmethod
-    def entity_attributes() -> List[str]:
+    def entity_attributes() -> [str]:
         return [
-            "node_a",
-            "node_b",
-            "length",
-            "geo_position",
-            "olm_characteristic",
-            "parallel_devices",
+            "behaviour",
         ]
 
     @staticmethod
-    def type_attributes() -> List[str]:
-        return HasTypeMixin.attributes() + ["r", "x", "b", "i_max", "v_rated"]
-
-    def aggregated_line_length(self) -> float:
-        return self.data["length"].sum()
-
-    def relative_line_length(self) -> float:
-        return self.data["length"] / len(self.data)
-
-    def find_lines_by_nodes(self, node_uuids):
-        return Lines(
-            self.data[(self.node_a.isin(node_uuids)) | (self.node_b.isin(node_uuids))]
-        )
+    def type_attributes() -> [str]:
+        return SpTypeMixin.type_attributes() + [
+            "p_max",
+            "active_power_gradient",
+            "e_storage",
+            "eta",
+            "dod",
+            "life_time",
+            "life_cycle",
+        ]
```

### Comparing `psdm-analysis-0.1.5/psdm_analysis/models/input/connector/switches.py` & `psdm-analysis-0.1.6/psdm_analysis/models/input/connector/switches.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 from dataclasses import dataclass
 
-from pandas import DataFrame
-
 from psdm_analysis.models.input.connector.connector import Connector
 from psdm_analysis.models.input.enums import EntitiesEnum, RawGridElementsEnum
 
 
 @dataclass(frozen=True)
 class Switches(Connector):
-    data: DataFrame
-
     @staticmethod
     def attributes() -> list[str]:
         return Connector.attributes() + ["closed"]
 
     @staticmethod
     def get_enum() -> EntitiesEnum:
         return RawGridElementsEnum.SWITCH
```

### Comparing `psdm-analysis-0.1.5/psdm_analysis/models/input/connector/transformer.py` & `psdm-analysis-0.1.6/psdm_analysis/models/input/connector/transformer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 from dataclasses import dataclass
 
-from pandas import DataFrame
-
 from psdm_analysis.models.input.connector.connector import Connector
 from psdm_analysis.models.input.container.mixins import HasTypeMixin
 from psdm_analysis.models.input.enums import RawGridElementsEnum
 
 
 @dataclass(frozen=True)
 class Transformers2W(Connector, HasTypeMixin):
-    data: DataFrame
-
     @property
     def type_id(self):
         return self.data["type_id"]
 
     @property
     def tap_pos(self):
         return self.data["tap_pos"]
```

### Comparing `psdm-analysis-0.1.5/psdm_analysis/models/input/container/grid_container.py` & `psdm-analysis-0.1.6/psdm_analysis/models/input/container/grid_container.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/psdm_analysis/models/input/container/mixins.py` & `psdm-analysis-0.1.6/psdm_analysis/models/input/container/mixins.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/psdm_analysis/models/input/container/participants_container.py` & `psdm-analysis-0.1.6/psdm_analysis/models/input/container/participants_container.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/psdm_analysis/models/input/enums.py` & `psdm-analysis-0.1.6/psdm_analysis/models/input/enums.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/psdm_analysis/models/input/node.py` & `psdm-analysis-0.1.6/psdm_analysis/models/input/node.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/psdm_analysis/models/input/participant/bm.py` & `psdm-analysis-0.1.6/psdm_analysis/models/input/participant/bm.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/psdm_analysis/models/input/participant/charging.py` & `psdm-analysis-0.1.6/psdm_analysis/models/input/participant/charging.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/psdm_analysis/models/input/participant/em.py` & `psdm-analysis-0.1.6/psdm_analysis/models/input/participant/em.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/psdm_analysis/models/input/participant/evcs.py` & `psdm-analysis-0.1.6/psdm_analysis/models/input/participant/evcs.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/psdm_analysis/models/input/participant/evs.py` & `psdm-analysis-0.1.6/psdm_analysis/models/input/participant/evs.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/psdm_analysis/models/input/participant/fixed_feed_in.py` & `psdm-analysis-0.1.6/psdm_analysis/models/input/participant/fixed_feed_in.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/psdm_analysis/models/input/participant/hp.py` & `psdm-analysis-0.1.6/psdm_analysis/models/input/participant/hp.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/psdm_analysis/models/input/participant/load.py` & `psdm-analysis-0.1.6/psdm_analysis/models/input/participant/load.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/psdm_analysis/models/input/participant/participant.py` & `psdm-analysis-0.1.6/psdm_analysis/models/input/participant/participant.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/psdm_analysis/models/input/participant/pv.py` & `psdm-analysis-0.1.6/psdm_analysis/models/input/participant/pv.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/psdm_analysis/models/input/participant/wec.py` & `psdm-analysis-0.1.6/psdm_analysis/models/input/participant/wec.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/psdm_analysis/models/primary_data.py` & `psdm-analysis-0.1.6/psdm_analysis/models/primary_data.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/psdm_analysis/models/result/flex_option.py` & `psdm-analysis-0.1.6/psdm_analysis/models/result/flex_option.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/psdm_analysis/models/result/grid/connector.py` & `psdm-analysis-0.1.6/psdm_analysis/models/result/grid/connector.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/psdm_analysis/models/result/grid/enhanced_node.py` & `psdm-analysis-0.1.6/psdm_analysis/models/result/grid/enhanced_node.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/psdm_analysis/models/result/grid/node.py` & `psdm-analysis-0.1.6/psdm_analysis/models/result/grid/node.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/psdm_analysis/models/result/grid/transformer.py` & `psdm-analysis-0.1.6/psdm_analysis/models/result/grid/transformer.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/psdm_analysis/models/result/participant/dict.py` & `psdm-analysis-0.1.6/psdm_analysis/models/result/participant/dict.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/psdm_analysis/models/result/participant/flex_options.py` & `psdm-analysis-0.1.6/psdm_analysis/models/result/participant/flex_options.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/psdm_analysis/models/result/participant/participant.py` & `psdm-analysis-0.1.6/psdm_analysis/models/result/participant/participant.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/psdm_analysis/models/result/participant/participants_res_container.py` & `psdm-analysis-0.1.6/psdm_analysis/models/result/participant/participants_res_container.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/psdm_analysis/models/result/power.py` & `psdm-analysis-0.1.6/psdm_analysis/models/result/power.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/psdm_analysis/models/result/res_container.py` & `psdm-analysis-0.1.6/psdm_analysis/models/result/res_container.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/psdm_analysis/plots/common/bar_plot.py` & `psdm-analysis-0.1.6/psdm_analysis/plots/common/bar_plot.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/psdm_analysis/plots/common/line_plot.py` & `psdm-analysis-0.1.6/psdm_analysis/plots/common/line_plot.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/psdm_analysis/plots/common/utils.py` & `psdm-analysis-0.1.6/psdm_analysis/plots/common/utils.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/psdm_analysis/plots/grid.py` & `psdm-analysis-0.1.6/psdm_analysis/plots/grid.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/psdm_analysis/plots/results/connector_plot.py` & `psdm-analysis-0.1.6/psdm_analysis/plots/results/connector_plot.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/psdm_analysis/plots/results/flex_plot.py` & `psdm-analysis-0.1.6/psdm_analysis/plots/results/flex_plot.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/psdm_analysis/plots/results/nodes.py` & `psdm-analysis-0.1.6/psdm_analysis/plots/results/nodes.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/psdm_analysis/plots/results/power_plot.py` & `psdm-analysis-0.1.6/psdm_analysis/plots/results/power_plot.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/psdm_analysis/plots/results/voltage_plot.py` & `psdm-analysis-0.1.6/psdm_analysis/plots/results/voltage_plot.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/psdm_analysis/processing/dataframe.py` & `psdm-analysis-0.1.6/psdm_analysis/processing/dataframe.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/psdm_analysis/processing/series.py` & `psdm-analysis-0.1.6/psdm_analysis/processing/series.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.5/pyproject.toml` & `psdm-analysis-0.1.6/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "psdm-analysis"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["Thomas Oberliessen <thomas.oberliessen@googlemail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">3.10, <3.12"
 pandas = "2.0.1"
```

### Comparing `psdm-analysis-0.1.5/setup.py` & `psdm-analysis-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
  'requests>=2.27.1,<3.0.0',
  'scipy>=1.10.0,<2.0.0',
  'seaborn>=0.12.1,<0.13.0',
  'shapely>=2.0.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'psdm-analysis',
-    'version': '0.1.5',
+    'version': '0.1.6',
     'description': '',
     'long_description': '# psdm-analysis\n\nThe psdm-analysis tool is meant to parse the [Power System Data Model (PSDM)](https://github.com/ie3-institute/PowerSystemDataModel) as well as provide calculation and plotting utilities to analyze the respective data.\n\nIt is currently under development and therefore highly unstable. So if you want to use it, expect it to change quite frequently for now.',
     'author': 'Thomas Oberliessen',
     'author_email': 'thomas.oberliessen@googlemail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `psdm-analysis-0.1.5/PKG-INFO` & `psdm-analysis-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psdm-analysis
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: Thomas Oberliessen
 Author-email: thomas.oberliessen@googlemail.com
 Requires-Python: >3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: jupyter (>=1.0.0,<2.0.0)
 Requires-Dist: matplotlib (>=3.6.0,<4.0.0)
```

