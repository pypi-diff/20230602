# Comparing `tmp/slitflow-0.1.2.tar.gz` & `tmp/slitflow-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slitflow-0.1.2.tar", last modified: Fri May 19 07:29:17 2023, max compression
+gzip compressed data, was "slitflow-0.1.3.tar", last modified: Fri Jun  2 07:02:57 2023, max compression
```

## Comparing `slitflow-0.1.2.tar` & `slitflow-0.1.3.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 07:29:17.790159 slitflow-0.1.2/
--rw-rw-rw-   0        0        0     1543 2023-02-02 03:40:43.000000 slitflow-0.1.2/LICENCE
--rw-rw-rw-   0        0        0     3462 2023-05-19 07:29:17.791159 slitflow-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2931 2023-03-06 08:58:47.000000 slitflow-0.1.2/README.md
--rw-rw-rw-   0        0        0      151 2022-07-27 10:08:19.000000 slitflow-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0      974 2023-05-19 07:29:17.799158 slitflow-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0       39 2022-07-27 10:08:19.000000 slitflow-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 07:29:17.291603 slitflow-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-19 07:29:17.342930 slitflow-0.1.2/src/slitflow/
--rw-rw-rw-   0        0        0      486 2023-05-19 04:54:58.000000 slitflow-0.1.2/src/slitflow/__init__.py
--rw-rw-rw-   0        0        0     8061 2023-02-17 12:47:03.000000 slitflow-0.1.2/src/slitflow/data.py
-drwxrwxrwx   0        0        0        0 2023-05-19 07:29:17.417900 slitflow-0.1.2/src/slitflow/fig/
--rw-rw-rw-   0        0        0      225 2023-02-01 11:16:51.000000 slitflow-0.1.2/src/slitflow/fig/__init__.py
--rw-rw-rw-   0        0        0     8592 2023-03-02 07:52:33.000000 slitflow-0.1.2/src/slitflow/fig/bar.py
--rw-rw-rw-   0        0        0     5063 2023-05-19 06:18:31.000000 slitflow-0.1.2/src/slitflow/fig/figure.py
--rw-rw-rw-   0        0        0     2417 2023-02-17 12:47:03.000000 slitflow-0.1.2/src/slitflow/fig/image.py
--rw-rw-rw-   0        0        0     7882 2023-03-02 07:52:39.000000 slitflow-0.1.2/src/slitflow/fig/line.py
--rw-rw-rw-   0        0        0     2599 2023-02-28 04:20:41.000000 slitflow-0.1.2/src/slitflow/fig/scatter.py
--rw-rw-rw-   0        0        0    41578 2023-03-06 04:01:37.000000 slitflow-0.1.2/src/slitflow/fig/style.py
--rw-rw-rw-   0        0        0     4212 2023-02-28 04:21:06.000000 slitflow-0.1.2/src/slitflow/fig/trajectory.py
-drwxrwxrwx   0        0        0        0 2023-05-19 07:29:17.439896 slitflow-0.1.2/src/slitflow/fun/
--rw-rw-rw-   0        0        0      124 2023-02-01 11:16:51.000000 slitflow-0.1.2/src/slitflow/fun/__init__.py
--rw-rw-rw-   0        0        0     1228 2023-02-17 12:47:03.000000 slitflow-0.1.2/src/slitflow/fun/img.py
--rw-rw-rw-   0        0        0      541 2023-02-01 11:16:51.000000 slitflow-0.1.2/src/slitflow/fun/misc.py
--rw-rw-rw-   0        0        0     5531 2023-02-17 12:47:03.000000 slitflow-0.1.2/src/slitflow/fun/palette.py
--rw-rw-rw-   0        0        0      242 2023-02-01 11:16:51.000000 slitflow-0.1.2/src/slitflow/fun/sort.py
-drwxrwxrwx   0        0        0        0 2023-05-19 07:29:17.483179 slitflow-0.1.2/src/slitflow/img/
--rw-rw-rw-   0        0        0      290 2023-05-18 01:18:17.000000 slitflow-0.1.2/src/slitflow/img/__init__.py
--rw-rw-rw-   0        0        0     1693 2023-02-17 12:47:03.000000 slitflow-0.1.2/src/slitflow/img/calc.py
--rw-rw-rw-   0        0        0     5437 2023-02-17 12:47:03.000000 slitflow-0.1.2/src/slitflow/img/convert.py
--rw-rw-rw-   0        0        0     8470 2023-05-18 02:33:03.000000 slitflow-0.1.2/src/slitflow/img/create.py
--rw-rw-rw-   0        0        0    10820 2023-02-17 12:47:03.000000 slitflow-0.1.2/src/slitflow/img/filter.py
--rw-rw-rw-   0        0        0     7959 2023-05-18 02:33:03.000000 slitflow-0.1.2/src/slitflow/img/image.py
--rw-rw-rw-   0        0        0     5471 2023-02-17 12:47:03.000000 slitflow-0.1.2/src/slitflow/img/montage.py
--rw-rw-rw-   0        0        0     1956 2023-02-17 12:47:03.000000 slitflow-0.1.2/src/slitflow/img/noise.py
--rw-rw-rw-   0        0        0     5648 2023-02-17 12:47:03.000000 slitflow-0.1.2/src/slitflow/img/plot.py
--rw-rw-rw-   0        0        0     3703 2023-05-18 01:17:03.000000 slitflow-0.1.2/src/slitflow/img/proc.py
--rw-rw-rw-   0        0        0    25481 2023-05-18 02:33:03.000000 slitflow-0.1.2/src/slitflow/info.py
-drwxrwxrwx   0        0        0        0 2023-05-19 07:29:17.496199 slitflow-0.1.2/src/slitflow/load/
--rw-rw-rw-   0        0        0       70 2023-02-01 11:16:51.000000 slitflow-0.1.2/src/slitflow/load/__init__.py
--rw-rw-rw-   0        0        0     1365 2023-02-17 12:47:03.000000 slitflow-0.1.2/src/slitflow/load/table.py
--rw-rw-rw-   0        0        0     9465 2023-05-19 04:47:43.000000 slitflow-0.1.2/src/slitflow/load/tif.py
-drwxrwxrwx   0        0        0        0 2023-05-19 07:29:17.517168 slitflow-0.1.2/src/slitflow/loc/
--rw-rw-rw-   0        0        0      128 2023-02-01 11:16:51.000000 slitflow-0.1.2/src/slitflow/loc/__init__.py
--rw-rw-rw-   0        0        0     6508 2023-02-17 12:47:04.000000 slitflow-0.1.2/src/slitflow/loc/convert.py
--rw-rw-rw-   0        0        0     9074 2023-02-01 11:16:51.000000 slitflow-0.1.2/src/slitflow/loc/fit.py
--rw-rw-rw-   0        0        0     7263 2023-05-18 02:05:33.000000 slitflow-0.1.2/src/slitflow/loc/mask.py
--rw-rw-rw-   0        0        0     3792 2023-02-17 12:47:04.000000 slitflow-0.1.2/src/slitflow/loc/random.py
--rw-rw-rw-   0        0        0    31206 2023-03-06 06:20:02.000000 slitflow-0.1.2/src/slitflow/manager.py
--rw-rw-rw-   0        0        0     6363 2023-02-17 12:47:04.000000 slitflow-0.1.2/src/slitflow/name.py
--rw-rw-rw-   0        0        0     2616 2023-05-18 01:22:50.000000 slitflow-0.1.2/src/slitflow/setindex.py
--rw-rw-rw-   0        0        0     8668 2023-05-18 02:05:33.000000 slitflow-0.1.2/src/slitflow/setreqs.py
-drwxrwxrwx   0        0        0        0 2023-05-19 07:29:17.554173 slitflow-0.1.2/src/slitflow/tbl/
--rw-rw-rw-   0        0        0      217 2023-05-18 01:23:36.000000 slitflow-0.1.2/src/slitflow/tbl/__init__.py
--rw-rw-rw-   0        0        0     7528 2023-05-18 01:23:59.000000 slitflow-0.1.2/src/slitflow/tbl/convert.py
--rw-rw-rw-   0        0        0     4279 2023-02-17 12:47:04.000000 slitflow-0.1.2/src/slitflow/tbl/create.py
--rw-rw-rw-   0        0        0     2608 2023-02-17 12:47:04.000000 slitflow-0.1.2/src/slitflow/tbl/filter.py
--rw-rw-rw-   0        0        0    10153 2023-02-17 12:47:04.000000 slitflow-0.1.2/src/slitflow/tbl/math.py
--rw-rw-rw-   0        0        0     6303 2023-05-18 01:17:19.000000 slitflow-0.1.2/src/slitflow/tbl/proc.py
--rw-rw-rw-   0        0        0    14129 2023-02-17 12:47:04.000000 slitflow-0.1.2/src/slitflow/tbl/stat.py
--rw-rw-rw-   0        0        0     3478 2023-05-18 01:39:32.000000 slitflow-0.1.2/src/slitflow/tbl/table.py
-drwxrwxrwx   0        0        0        0 2023-05-19 07:29:17.584198 slitflow-0.1.2/src/slitflow/trj/
--rw-rw-rw-   0        0        0      204 2023-02-01 11:16:51.000000 slitflow-0.1.2/src/slitflow/trj/__init__.py
--rw-rw-rw-   0        0        0     3356 2023-02-17 12:47:04.000000 slitflow-0.1.2/src/slitflow/trj/filter.py
--rw-rw-rw-   0        0        0    24916 2023-02-17 12:47:04.000000 slitflow-0.1.2/src/slitflow/trj/msd.py
--rw-rw-rw-   0        0        0    15950 2023-02-17 12:47:04.000000 slitflow-0.1.2/src/slitflow/trj/random.py
--rw-rw-rw-   0        0        0    32297 2023-05-18 07:08:13.000000 slitflow-0.1.2/src/slitflow/trj/wfastspt.py
--rw-rw-rw-   0        0        0    12180 2023-02-17 12:47:04.000000 slitflow-0.1.2/src/slitflow/trj/wtrackpy.py
--rw-rw-rw-   0        0        0     9667 2023-02-28 08:32:50.000000 slitflow-0.1.2/src/slitflow/trj/wtramway.py
-drwxrwxrwx   0        0        0        0 2023-05-19 07:29:17.592178 slitflow-0.1.2/src/slitflow/user/
--rw-rw-rw-   0        0        0      307 2023-02-01 11:16:51.000000 slitflow-0.1.2/src/slitflow/user/__init__.py
--rw-rw-rw-   0        0        0     1728 2023-02-01 11:16:51.000000 slitflow-0.1.2/src/slitflow/user/template.py
-drwxrwxrwx   0        0        0        0 2023-05-19 07:29:17.381929 slitflow-0.1.2/src/slitflow.egg-info/
--rw-rw-rw-   0        0        0     3462 2023-05-19 07:29:17.000000 slitflow-0.1.2/src/slitflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2879 2023-05-19 07:29:17.000000 slitflow-0.1.2/src/slitflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 07:29:17.000000 slitflow-0.1.2/src/slitflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      240 2023-05-19 07:29:17.000000 slitflow-0.1.2/src/slitflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-19 07:29:17.000000 slitflow-0.1.2/src/slitflow.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-19 07:29:17.786160 slitflow-0.1.2/src/tests/
--rw-rw-rw-   0        0        0        0 2023-03-02 07:56:26.000000 slitflow-0.1.2/src/tests/__init__.py
--rw-rw-rw-   0        0        0     2815 2023-03-02 07:56:28.000000 slitflow-0.1.2/src/tests/test_data.py
--rw-rw-rw-   0        0        0     4148 2023-03-02 07:56:30.000000 slitflow-0.1.2/src/tests/test_fig_bar.py
--rw-rw-rw-   0        0        0     1177 2023-03-02 07:56:32.000000 slitflow-0.1.2/src/tests/test_fig_figure.py
--rw-rw-rw-   0        0        0      639 2023-03-02 07:56:35.000000 slitflow-0.1.2/src/tests/test_fig_image.py
--rw-rw-rw-   0        0        0     2485 2023-03-02 07:56:37.000000 slitflow-0.1.2/src/tests/test_fig_line.py
--rw-rw-rw-   0        0        0     1204 2023-03-02 07:56:39.000000 slitflow-0.1.2/src/tests/test_fig_scatter.py
--rw-rw-rw-   0        0        0    18945 2023-03-06 04:03:32.000000 slitflow-0.1.2/src/tests/test_fig_style.py
--rw-rw-rw-   0        0        0     1517 2023-03-02 07:56:44.000000 slitflow-0.1.2/src/tests/test_fig_trajectory.py
--rw-rw-rw-   0        0        0     3499 2023-03-02 07:56:46.000000 slitflow-0.1.2/src/tests/test_fun.py
--rw-rw-rw-   0        0        0     1634 2023-03-06 04:03:36.000000 slitflow-0.1.2/src/tests/test_getting_started.py
--rw-rw-rw-   0        0        0      549 2023-03-02 07:56:48.000000 slitflow-0.1.2/src/tests/test_img_calc.py
--rw-rw-rw-   0        0        0     1343 2023-05-18 02:33:03.000000 slitflow-0.1.2/src/tests/test_img_create.py
--rw-rw-rw-   0        0        0     1098 2023-03-02 07:56:53.000000 slitflow-0.1.2/src/tests/test_img_filter.py
--rw-rw-rw-   0        0        0     3260 2023-05-18 05:27:15.000000 slitflow-0.1.2/src/tests/test_img_image.py
--rw-rw-rw-   0        0        0      952 2023-03-02 07:56:58.000000 slitflow-0.1.2/src/tests/test_img_montage.py
--rw-rw-rw-   0        0        0      607 2023-03-06 04:03:46.000000 slitflow-0.1.2/src/tests/test_img_noise.py
--rw-rw-rw-   0        0        0      732 2023-03-06 04:03:51.000000 slitflow-0.1.2/src/tests/test_img_plot.py
--rw-rw-rw-   0        0        0     1191 2023-05-18 01:25:03.000000 slitflow-0.1.2/src/tests/test_img_proc.py
--rw-rw-rw-   0        0        0     6763 2023-03-06 04:03:57.000000 slitflow-0.1.2/src/tests/test_info.py
--rw-rw-rw-   0        0        0      533 2023-03-02 07:57:07.000000 slitflow-0.1.2/src/tests/test_load_table.py
--rw-rw-rw-   0        0        0      976 2023-03-02 07:57:10.000000 slitflow-0.1.2/src/tests/test_load_tif.py
--rw-rw-rw-   0        0        0     2191 2023-03-02 07:57:11.000000 slitflow-0.1.2/src/tests/test_loc_convert.py
--rw-rw-rw-   0        0        0     1252 2023-03-02 07:57:13.000000 slitflow-0.1.2/src/tests/test_loc_fit.py
--rw-rw-rw-   0        0        0     1598 2023-03-02 07:57:16.000000 slitflow-0.1.2/src/tests/test_loc_mask.py
--rw-rw-rw-   0        0        0      592 2023-03-02 07:57:17.000000 slitflow-0.1.2/src/tests/test_loc_random.py
--rw-rw-rw-   0        0        0    14806 2023-03-06 04:04:03.000000 slitflow-0.1.2/src/tests/test_manager.py
--rw-rw-rw-   0        0        0     3058 2023-03-06 04:04:08.000000 slitflow-0.1.2/src/tests/test_name.py
--rw-rw-rw-   0        0        0     1659 2023-03-06 04:04:16.000000 slitflow-0.1.2/src/tests/test_setindex.py
--rw-rw-rw-   0        0        0     2533 2023-03-02 07:57:27.000000 slitflow-0.1.2/src/tests/test_setreqs.py
--rw-rw-rw-   0        0        0     2620 2023-05-18 01:26:28.000000 slitflow-0.1.2/src/tests/test_tbl_convert.py
--rw-rw-rw-   0        0        0     1237 2023-03-02 07:57:32.000000 slitflow-0.1.2/src/tests/test_tbl_create.py
--rw-rw-rw-   0        0        0      541 2023-03-02 07:57:34.000000 slitflow-0.1.2/src/tests/test_tbl_filter.py
--rw-rw-rw-   0        0        0     1860 2023-03-02 07:57:36.000000 slitflow-0.1.2/src/tests/test_tbl_math.py
--rw-rw-rw-   0        0        0     1195 2023-05-18 01:26:37.000000 slitflow-0.1.2/src/tests/test_tbl_proc.py
--rw-rw-rw-   0        0        0     1134 2023-03-02 07:57:38.000000 slitflow-0.1.2/src/tests/test_tbl_stat.py
--rw-rw-rw-   0        0        0      957 2023-03-02 07:57:40.000000 slitflow-0.1.2/src/tests/test_tbl_table.py
--rw-rw-rw-   0        0        0     1317 2023-03-02 07:57:41.000000 slitflow-0.1.2/src/tests/test_trj_filter.py
--rw-rw-rw-   0        0        0     4269 2023-03-02 07:57:43.000000 slitflow-0.1.2/src/tests/test_trj_msd.py
--rw-rw-rw-   0        0        0     1276 2023-03-06 04:04:20.000000 slitflow-0.1.2/src/tests/test_trj_random.py
--rw-rw-rw-   0        0        0     7154 2023-03-02 07:57:47.000000 slitflow-0.1.2/src/tests/test_trj_wfastspt.py
--rw-rw-rw-   0        0        0     1194 2023-03-02 07:57:48.000000 slitflow-0.1.2/src/tests/test_trj_wtrackpy.py
--rw-rw-rw-   0        0        0     1635 2023-03-02 07:53:40.000000 slitflow-0.1.2/src/tests/test_trj_wtramway.py
+drwxrwxrwx   0        0        0        0 2023-06-02 07:02:57.060186 slitflow-0.1.3/
+-rw-rw-rw-   0        0        0     1543 2023-02-02 03:40:43.000000 slitflow-0.1.3/LICENCE
+-rw-rw-rw-   0        0        0     3462 2023-06-02 07:02:57.061186 slitflow-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2931 2023-03-06 08:58:47.000000 slitflow-0.1.3/README.md
+-rw-rw-rw-   0        0        0      151 2022-07-27 10:08:19.000000 slitflow-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0      974 2023-06-02 07:02:57.067187 slitflow-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0       39 2022-07-27 10:08:19.000000 slitflow-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 07:02:56.555186 slitflow-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-02 07:02:56.604186 slitflow-0.1.3/src/slitflow/
+-rw-rw-rw-   0        0        0      486 2023-06-02 06:41:20.000000 slitflow-0.1.3/src/slitflow/__init__.py
+-rw-rw-rw-   0        0        0     8061 2023-02-17 12:47:03.000000 slitflow-0.1.3/src/slitflow/data.py
+drwxrwxrwx   0        0        0        0 2023-06-02 07:02:56.673187 slitflow-0.1.3/src/slitflow/fig/
+-rw-rw-rw-   0        0        0      225 2023-02-01 11:16:51.000000 slitflow-0.1.3/src/slitflow/fig/__init__.py
+-rw-rw-rw-   0        0        0     8592 2023-03-02 07:52:33.000000 slitflow-0.1.3/src/slitflow/fig/bar.py
+-rw-rw-rw-   0        0        0     5063 2023-05-19 06:18:31.000000 slitflow-0.1.3/src/slitflow/fig/figure.py
+-rw-rw-rw-   0        0        0     2417 2023-02-17 12:47:03.000000 slitflow-0.1.3/src/slitflow/fig/image.py
+-rw-rw-rw-   0        0        0     7882 2023-03-02 07:52:39.000000 slitflow-0.1.3/src/slitflow/fig/line.py
+-rw-rw-rw-   0        0        0     2599 2023-02-28 04:20:41.000000 slitflow-0.1.3/src/slitflow/fig/scatter.py
+-rw-rw-rw-   0        0        0    41578 2023-03-06 04:01:37.000000 slitflow-0.1.3/src/slitflow/fig/style.py
+-rw-rw-rw-   0        0        0     4212 2023-02-28 04:21:06.000000 slitflow-0.1.3/src/slitflow/fig/trajectory.py
+drwxrwxrwx   0        0        0        0 2023-06-02 07:02:56.697198 slitflow-0.1.3/src/slitflow/fun/
+-rw-rw-rw-   0        0        0      124 2023-02-01 11:16:51.000000 slitflow-0.1.3/src/slitflow/fun/__init__.py
+-rw-rw-rw-   0        0        0     1228 2023-02-17 12:47:03.000000 slitflow-0.1.3/src/slitflow/fun/img.py
+-rw-rw-rw-   0        0        0      541 2023-02-01 11:16:51.000000 slitflow-0.1.3/src/slitflow/fun/misc.py
+-rw-rw-rw-   0        0        0     5531 2023-02-17 12:47:03.000000 slitflow-0.1.3/src/slitflow/fun/palette.py
+-rw-rw-rw-   0        0        0      242 2023-02-01 11:16:51.000000 slitflow-0.1.3/src/slitflow/fun/sort.py
+drwxrwxrwx   0        0        0        0 2023-06-02 07:02:56.741187 slitflow-0.1.3/src/slitflow/img/
+-rw-rw-rw-   0        0        0      290 2023-05-18 01:18:17.000000 slitflow-0.1.3/src/slitflow/img/__init__.py
+-rw-rw-rw-   0        0        0     1693 2023-02-17 12:47:03.000000 slitflow-0.1.3/src/slitflow/img/calc.py
+-rw-rw-rw-   0        0        0     5437 2023-02-17 12:47:03.000000 slitflow-0.1.3/src/slitflow/img/convert.py
+-rw-rw-rw-   0        0        0     8470 2023-05-18 02:33:03.000000 slitflow-0.1.3/src/slitflow/img/create.py
+-rw-rw-rw-   0        0        0    10820 2023-02-17 12:47:03.000000 slitflow-0.1.3/src/slitflow/img/filter.py
+-rw-rw-rw-   0        0        0     7959 2023-05-18 02:33:03.000000 slitflow-0.1.3/src/slitflow/img/image.py
+-rw-rw-rw-   0        0        0     5471 2023-02-17 12:47:03.000000 slitflow-0.1.3/src/slitflow/img/montage.py
+-rw-rw-rw-   0        0        0     1956 2023-02-17 12:47:03.000000 slitflow-0.1.3/src/slitflow/img/noise.py
+-rw-rw-rw-   0        0        0     5648 2023-02-17 12:47:03.000000 slitflow-0.1.3/src/slitflow/img/plot.py
+-rw-rw-rw-   0        0        0     3703 2023-05-18 01:17:03.000000 slitflow-0.1.3/src/slitflow/img/proc.py
+-rw-rw-rw-   0        0        0    25479 2023-06-02 06:38:37.000000 slitflow-0.1.3/src/slitflow/info.py
+drwxrwxrwx   0        0        0        0 2023-06-02 07:02:56.753187 slitflow-0.1.3/src/slitflow/load/
+-rw-rw-rw-   0        0        0       70 2023-02-01 11:16:51.000000 slitflow-0.1.3/src/slitflow/load/__init__.py
+-rw-rw-rw-   0        0        0     1365 2023-02-17 12:47:03.000000 slitflow-0.1.3/src/slitflow/load/table.py
+-rw-rw-rw-   0        0        0     9465 2023-05-19 04:47:43.000000 slitflow-0.1.3/src/slitflow/load/tif.py
+drwxrwxrwx   0        0        0        0 2023-06-02 07:02:56.782188 slitflow-0.1.3/src/slitflow/loc/
+-rw-rw-rw-   0        0        0      128 2023-02-01 11:16:51.000000 slitflow-0.1.3/src/slitflow/loc/__init__.py
+-rw-rw-rw-   0        0        0     6508 2023-02-17 12:47:04.000000 slitflow-0.1.3/src/slitflow/loc/convert.py
+-rw-rw-rw-   0        0        0     9074 2023-02-01 11:16:51.000000 slitflow-0.1.3/src/slitflow/loc/fit.py
+-rw-rw-rw-   0        0        0     7263 2023-05-18 02:05:33.000000 slitflow-0.1.3/src/slitflow/loc/mask.py
+-rw-rw-rw-   0        0        0     3792 2023-02-17 12:47:04.000000 slitflow-0.1.3/src/slitflow/loc/random.py
+-rw-rw-rw-   0        0        0    31206 2023-03-06 06:20:02.000000 slitflow-0.1.3/src/slitflow/manager.py
+-rw-rw-rw-   0        0        0     6363 2023-02-17 12:47:04.000000 slitflow-0.1.3/src/slitflow/name.py
+-rw-rw-rw-   0        0        0     2616 2023-05-18 01:22:50.000000 slitflow-0.1.3/src/slitflow/setindex.py
+-rw-rw-rw-   0        0        0     8668 2023-05-18 02:05:33.000000 slitflow-0.1.3/src/slitflow/setreqs.py
+drwxrwxrwx   0        0        0        0 2023-06-02 07:02:56.824187 slitflow-0.1.3/src/slitflow/tbl/
+-rw-rw-rw-   0        0        0      217 2023-05-18 01:23:36.000000 slitflow-0.1.3/src/slitflow/tbl/__init__.py
+-rw-rw-rw-   0        0        0     7528 2023-05-18 01:23:59.000000 slitflow-0.1.3/src/slitflow/tbl/convert.py
+-rw-rw-rw-   0        0        0     4279 2023-02-17 12:47:04.000000 slitflow-0.1.3/src/slitflow/tbl/create.py
+-rw-rw-rw-   0        0        0     2608 2023-02-17 12:47:04.000000 slitflow-0.1.3/src/slitflow/tbl/filter.py
+-rw-rw-rw-   0        0        0    10153 2023-02-17 12:47:04.000000 slitflow-0.1.3/src/slitflow/tbl/math.py
+-rw-rw-rw-   0        0        0     6303 2023-05-18 01:17:19.000000 slitflow-0.1.3/src/slitflow/tbl/proc.py
+-rw-rw-rw-   0        0        0    14129 2023-02-17 12:47:04.000000 slitflow-0.1.3/src/slitflow/tbl/stat.py
+-rw-rw-rw-   0        0        0     3478 2023-05-18 01:39:32.000000 slitflow-0.1.3/src/slitflow/tbl/table.py
+drwxrwxrwx   0        0        0        0 2023-06-02 07:02:56.854187 slitflow-0.1.3/src/slitflow/trj/
+-rw-rw-rw-   0        0        0      204 2023-02-01 11:16:51.000000 slitflow-0.1.3/src/slitflow/trj/__init__.py
+-rw-rw-rw-   0        0        0     3356 2023-02-17 12:47:04.000000 slitflow-0.1.3/src/slitflow/trj/filter.py
+-rw-rw-rw-   0        0        0    24916 2023-02-17 12:47:04.000000 slitflow-0.1.3/src/slitflow/trj/msd.py
+-rw-rw-rw-   0        0        0    15950 2023-02-17 12:47:04.000000 slitflow-0.1.3/src/slitflow/trj/random.py
+-rw-rw-rw-   0        0        0    32297 2023-05-18 07:08:13.000000 slitflow-0.1.3/src/slitflow/trj/wfastspt.py
+-rw-rw-rw-   0        0        0    12180 2023-02-17 12:47:04.000000 slitflow-0.1.3/src/slitflow/trj/wtrackpy.py
+-rw-rw-rw-   0        0        0     9667 2023-02-28 08:32:50.000000 slitflow-0.1.3/src/slitflow/trj/wtramway.py
+drwxrwxrwx   0        0        0        0 2023-06-02 07:02:56.862188 slitflow-0.1.3/src/slitflow/user/
+-rw-rw-rw-   0        0        0      307 2023-02-01 11:16:51.000000 slitflow-0.1.3/src/slitflow/user/__init__.py
+-rw-rw-rw-   0        0        0     1728 2023-02-01 11:16:51.000000 slitflow-0.1.3/src/slitflow/user/template.py
+drwxrwxrwx   0        0        0        0 2023-06-02 07:02:56.637187 slitflow-0.1.3/src/slitflow.egg-info/
+-rw-rw-rw-   0        0        0     3462 2023-06-02 07:02:56.000000 slitflow-0.1.3/src/slitflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2879 2023-06-02 07:02:56.000000 slitflow-0.1.3/src/slitflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 07:02:56.000000 slitflow-0.1.3/src/slitflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      240 2023-06-02 07:02:56.000000 slitflow-0.1.3/src/slitflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-02 07:02:56.000000 slitflow-0.1.3/src/slitflow.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 07:02:57.057187 slitflow-0.1.3/src/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-02 07:56:26.000000 slitflow-0.1.3/src/tests/__init__.py
+-rw-rw-rw-   0        0        0     2815 2023-03-02 07:56:28.000000 slitflow-0.1.3/src/tests/test_data.py
+-rw-rw-rw-   0        0        0     4148 2023-03-02 07:56:30.000000 slitflow-0.1.3/src/tests/test_fig_bar.py
+-rw-rw-rw-   0        0        0     1177 2023-03-02 07:56:32.000000 slitflow-0.1.3/src/tests/test_fig_figure.py
+-rw-rw-rw-   0        0        0      639 2023-03-02 07:56:35.000000 slitflow-0.1.3/src/tests/test_fig_image.py
+-rw-rw-rw-   0        0        0     2485 2023-03-02 07:56:37.000000 slitflow-0.1.3/src/tests/test_fig_line.py
+-rw-rw-rw-   0        0        0     1204 2023-03-02 07:56:39.000000 slitflow-0.1.3/src/tests/test_fig_scatter.py
+-rw-rw-rw-   0        0        0    18945 2023-03-06 04:03:32.000000 slitflow-0.1.3/src/tests/test_fig_style.py
+-rw-rw-rw-   0        0        0     1517 2023-03-02 07:56:44.000000 slitflow-0.1.3/src/tests/test_fig_trajectory.py
+-rw-rw-rw-   0        0        0     3499 2023-03-02 07:56:46.000000 slitflow-0.1.3/src/tests/test_fun.py
+-rw-rw-rw-   0        0        0     1634 2023-03-06 04:03:36.000000 slitflow-0.1.3/src/tests/test_getting_started.py
+-rw-rw-rw-   0        0        0      549 2023-03-02 07:56:48.000000 slitflow-0.1.3/src/tests/test_img_calc.py
+-rw-rw-rw-   0        0        0     1343 2023-05-18 02:33:03.000000 slitflow-0.1.3/src/tests/test_img_create.py
+-rw-rw-rw-   0        0        0     1098 2023-03-02 07:56:53.000000 slitflow-0.1.3/src/tests/test_img_filter.py
+-rw-rw-rw-   0        0        0     3260 2023-05-18 05:27:15.000000 slitflow-0.1.3/src/tests/test_img_image.py
+-rw-rw-rw-   0        0        0      952 2023-03-02 07:56:58.000000 slitflow-0.1.3/src/tests/test_img_montage.py
+-rw-rw-rw-   0        0        0      607 2023-03-06 04:03:46.000000 slitflow-0.1.3/src/tests/test_img_noise.py
+-rw-rw-rw-   0        0        0      732 2023-03-06 04:03:51.000000 slitflow-0.1.3/src/tests/test_img_plot.py
+-rw-rw-rw-   0        0        0     1191 2023-05-18 01:25:03.000000 slitflow-0.1.3/src/tests/test_img_proc.py
+-rw-rw-rw-   0        0        0     6751 2023-06-02 06:38:37.000000 slitflow-0.1.3/src/tests/test_info.py
+-rw-rw-rw-   0        0        0      533 2023-03-02 07:57:07.000000 slitflow-0.1.3/src/tests/test_load_table.py
+-rw-rw-rw-   0        0        0      976 2023-03-02 07:57:10.000000 slitflow-0.1.3/src/tests/test_load_tif.py
+-rw-rw-rw-   0        0        0     2191 2023-03-02 07:57:11.000000 slitflow-0.1.3/src/tests/test_loc_convert.py
+-rw-rw-rw-   0        0        0     1252 2023-03-02 07:57:13.000000 slitflow-0.1.3/src/tests/test_loc_fit.py
+-rw-rw-rw-   0        0        0     1598 2023-03-02 07:57:16.000000 slitflow-0.1.3/src/tests/test_loc_mask.py
+-rw-rw-rw-   0        0        0      592 2023-03-02 07:57:17.000000 slitflow-0.1.3/src/tests/test_loc_random.py
+-rw-rw-rw-   0        0        0    14806 2023-03-06 04:04:03.000000 slitflow-0.1.3/src/tests/test_manager.py
+-rw-rw-rw-   0        0        0     3058 2023-03-06 04:04:08.000000 slitflow-0.1.3/src/tests/test_name.py
+-rw-rw-rw-   0        0        0     1659 2023-03-06 04:04:16.000000 slitflow-0.1.3/src/tests/test_setindex.py
+-rw-rw-rw-   0        0        0     2533 2023-03-02 07:57:27.000000 slitflow-0.1.3/src/tests/test_setreqs.py
+-rw-rw-rw-   0        0        0     2620 2023-05-18 01:26:28.000000 slitflow-0.1.3/src/tests/test_tbl_convert.py
+-rw-rw-rw-   0        0        0     1237 2023-03-02 07:57:32.000000 slitflow-0.1.3/src/tests/test_tbl_create.py
+-rw-rw-rw-   0        0        0      541 2023-03-02 07:57:34.000000 slitflow-0.1.3/src/tests/test_tbl_filter.py
+-rw-rw-rw-   0        0        0     1860 2023-03-02 07:57:36.000000 slitflow-0.1.3/src/tests/test_tbl_math.py
+-rw-rw-rw-   0        0        0     1195 2023-05-18 01:26:37.000000 slitflow-0.1.3/src/tests/test_tbl_proc.py
+-rw-rw-rw-   0        0        0     1134 2023-03-02 07:57:38.000000 slitflow-0.1.3/src/tests/test_tbl_stat.py
+-rw-rw-rw-   0        0        0      957 2023-03-02 07:57:40.000000 slitflow-0.1.3/src/tests/test_tbl_table.py
+-rw-rw-rw-   0        0        0     1317 2023-03-02 07:57:41.000000 slitflow-0.1.3/src/tests/test_trj_filter.py
+-rw-rw-rw-   0        0        0     4269 2023-03-02 07:57:43.000000 slitflow-0.1.3/src/tests/test_trj_msd.py
+-rw-rw-rw-   0        0        0     1276 2023-03-06 04:04:20.000000 slitflow-0.1.3/src/tests/test_trj_random.py
+-rw-rw-rw-   0        0        0     7154 2023-03-02 07:57:47.000000 slitflow-0.1.3/src/tests/test_trj_wfastspt.py
+-rw-rw-rw-   0        0        0     1194 2023-03-02 07:57:48.000000 slitflow-0.1.3/src/tests/test_trj_wtrackpy.py
+-rw-rw-rw-   0        0        0     1635 2023-03-02 07:53:40.000000 slitflow-0.1.3/src/tests/test_trj_wtramway.py
```

### Comparing `slitflow-0.1.2/LICENCE` & `slitflow-0.1.3/LICENCE`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/PKG-INFO` & `slitflow-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slitflow
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python framework for single-molecule dynamics and localization analysis
 Author: Yuma Ito
 Author-email: yitou@bio.titech.ac.jp
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `slitflow-0.1.2/README.md` & `slitflow-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/setup.cfg` & `slitflow-0.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/slitflow/data.py` & `slitflow-0.1.3/src/slitflow/data.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/slitflow/fig/bar.py` & `slitflow-0.1.3/src/slitflow/fig/bar.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/slitflow/fig/figure.py` & `slitflow-0.1.3/src/slitflow/fig/figure.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/slitflow/fig/image.py` & `slitflow-0.1.3/src/slitflow/fig/image.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/slitflow/fig/line.py` & `slitflow-0.1.3/src/slitflow/fig/line.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/slitflow/fig/scatter.py` & `slitflow-0.1.3/src/slitflow/fig/scatter.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/slitflow/fig/style.py` & `slitflow-0.1.3/src/slitflow/fig/style.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/slitflow/fig/trajectory.py` & `slitflow-0.1.3/src/slitflow/fig/trajectory.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/slitflow/fun/img.py` & `slitflow-0.1.3/src/slitflow/fun/img.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/slitflow/fun/misc.py` & `slitflow-0.1.3/src/slitflow/fun/misc.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/slitflow/fun/palette.py` & `slitflow-0.1.3/src/slitflow/fun/palette.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/slitflow/img/calc.py` & `slitflow-0.1.3/src/slitflow/img/calc.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/slitflow/img/convert.py` & `slitflow-0.1.3/src/slitflow/img/convert.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/slitflow/img/create.py` & `slitflow-0.1.3/src/slitflow/img/create.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/slitflow/img/filter.py` & `slitflow-0.1.3/src/slitflow/img/filter.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/slitflow/img/image.py` & `slitflow-0.1.3/src/slitflow/img/image.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/slitflow/img/montage.py` & `slitflow-0.1.3/src/slitflow/img/montage.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/slitflow/img/noise.py` & `slitflow-0.1.3/src/slitflow/img/noise.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/slitflow/img/plot.py` & `slitflow-0.1.3/src/slitflow/img/plot.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/slitflow/img/proc.py` & `slitflow-0.1.3/src/slitflow/img/proc.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/slitflow/info.py` & `slitflow-0.1.3/src/slitflow/info.py`

 * *Files 0% similar despite different names*

```diff
@@ -680,15 +680,15 @@
                 reqs_dict["req_" + str(i)] = req.info.get_dict()
         now = datetime.datetime.now().strftime("%Y/%m/%d %H:%M:%S")
         dict = {"version": __version__, "class": fullname(self.Data),
                 "description": self.Data.__class__.__doc__.splitlines()[0],
                 "datetime": now, "path": self.path, "reqs": reqs_dict}
         self.meta = dict
 
-    def to_string(self):
+    def to_json(self):
         """Returns a string representation of info file to export.
 
         .. caution::
 
             Private parameters will be removed.
 
         Returns:
```

### Comparing `slitflow-0.1.2/src/slitflow/load/table.py` & `slitflow-0.1.3/src/slitflow/load/table.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/slitflow/load/tif.py` & `slitflow-0.1.3/src/slitflow/load/tif.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/slitflow/loc/convert.py` & `slitflow-0.1.3/src/slitflow/loc/convert.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/slitflow/loc/fit.py` & `slitflow-0.1.3/src/slitflow/loc/fit.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/slitflow/loc/mask.py` & `slitflow-0.1.3/src/slitflow/loc/mask.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/slitflow/loc/random.py` & `slitflow-0.1.3/src/slitflow/loc/random.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/slitflow/manager.py` & `slitflow-0.1.3/src/slitflow/manager.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/slitflow/name.py` & `slitflow-0.1.3/src/slitflow/name.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/slitflow/setindex.py` & `slitflow-0.1.3/src/slitflow/setindex.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/slitflow/setreqs.py` & `slitflow-0.1.3/src/slitflow/setreqs.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/slitflow/tbl/convert.py` & `slitflow-0.1.3/src/slitflow/tbl/convert.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/slitflow/tbl/create.py` & `slitflow-0.1.3/src/slitflow/tbl/create.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/slitflow/tbl/filter.py` & `slitflow-0.1.3/src/slitflow/tbl/filter.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/slitflow/tbl/math.py` & `slitflow-0.1.3/src/slitflow/tbl/math.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/slitflow/tbl/proc.py` & `slitflow-0.1.3/src/slitflow/tbl/proc.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/slitflow/tbl/stat.py` & `slitflow-0.1.3/src/slitflow/tbl/stat.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/slitflow/tbl/table.py` & `slitflow-0.1.3/src/slitflow/tbl/table.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/slitflow/trj/filter.py` & `slitflow-0.1.3/src/slitflow/trj/filter.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/slitflow/trj/msd.py` & `slitflow-0.1.3/src/slitflow/trj/msd.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/slitflow/trj/random.py` & `slitflow-0.1.3/src/slitflow/trj/random.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/slitflow/trj/wfastspt.py` & `slitflow-0.1.3/src/slitflow/trj/wfastspt.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/slitflow/trj/wtrackpy.py` & `slitflow-0.1.3/src/slitflow/trj/wtrackpy.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/slitflow/trj/wtramway.py` & `slitflow-0.1.3/src/slitflow/trj/wtramway.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/slitflow/user/template.py` & `slitflow-0.1.3/src/slitflow/user/template.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/slitflow.egg-info/PKG-INFO` & `slitflow-0.1.3/src/slitflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slitflow
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python framework for single-molecule dynamics and localization analysis
 Author: Yuma Ito
 Author-email: yitou@bio.titech.ac.jp
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `slitflow-0.1.2/src/slitflow.egg-info/SOURCES.txt` & `slitflow-0.1.3/src/slitflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/tests/test_data.py` & `slitflow-0.1.3/src/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/tests/test_fig_bar.py` & `slitflow-0.1.3/src/tests/test_fig_bar.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/tests/test_fig_figure.py` & `slitflow-0.1.3/src/tests/test_fig_figure.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/tests/test_fig_image.py` & `slitflow-0.1.3/src/tests/test_fig_image.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/tests/test_fig_line.py` & `slitflow-0.1.3/src/tests/test_fig_line.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/tests/test_fig_scatter.py` & `slitflow-0.1.3/src/tests/test_fig_scatter.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/tests/test_fig_style.py` & `slitflow-0.1.3/src/tests/test_fig_style.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/tests/test_fig_trajectory.py` & `slitflow-0.1.3/src/tests/test_fig_trajectory.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/tests/test_fun.py` & `slitflow-0.1.3/src/tests/test_fun.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/tests/test_getting_started.py` & `slitflow-0.1.3/src/tests/test_getting_started.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/tests/test_img_calc.py` & `slitflow-0.1.3/src/tests/test_img_calc.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/tests/test_img_create.py` & `slitflow-0.1.3/src/tests/test_img_create.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/tests/test_img_filter.py` & `slitflow-0.1.3/src/tests/test_img_filter.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/tests/test_img_image.py` & `slitflow-0.1.3/src/tests/test_img_image.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/tests/test_img_montage.py` & `slitflow-0.1.3/src/tests/test_img_montage.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/tests/test_img_noise.py` & `slitflow-0.1.3/src/tests/test_img_noise.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/tests/test_img_plot.py` & `slitflow-0.1.3/src/tests/test_img_plot.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/tests/test_img_proc.py` & `slitflow-0.1.3/src/tests/test_img_proc.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/tests/test_info.py` & `slitflow-0.1.3/src/tests/test_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,20 +29,20 @@
     sys.stdout = sys.__stdout__
     print_text = open(os.path.join(tmpdir, "stdout_with_path.txt"), "r").read()
     print(print_text)
     assert "Data: slitflow.tbl.create.Index" in print_text \
            and "Path: " + os.path.join(
                tmpdir, "g1_grp", "a1_ana", "test_grp_ana.sf") in print_text
 
-    to_string = D.info.to_string()
-    assert to_string.find('"meta": {') == 781
+    to_json = D.info.to_json()
+    assert to_json.find('"meta": {') == 781
 
     D.info.meta = {}
-    to_string = D.info.to_string()
-    assert to_string.find('"meta": {') == 781
+    to_json = D.info.to_json()
+    assert to_json.find('"meta": {') == 781
 
 
 def test_Info_set_path(tmpdir):
     D = sf.tbl.create.Index(ipath(tmpdir, 1, 1, "test", "ana", "grp"))
     D.run([], {"index_counts": [1, 1], "type": "trajectory",
                "split_depth": 0})
     D.info.set_path("test_path")
```

### Comparing `slitflow-0.1.2/src/tests/test_load_table.py` & `slitflow-0.1.3/src/tests/test_load_table.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/tests/test_load_tif.py` & `slitflow-0.1.3/src/tests/test_load_tif.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/tests/test_loc_convert.py` & `slitflow-0.1.3/src/tests/test_loc_convert.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/tests/test_loc_fit.py` & `slitflow-0.1.3/src/tests/test_loc_fit.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/tests/test_loc_mask.py` & `slitflow-0.1.3/src/tests/test_loc_mask.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/tests/test_loc_random.py` & `slitflow-0.1.3/src/tests/test_loc_random.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/tests/test_manager.py` & `slitflow-0.1.3/src/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/tests/test_name.py` & `slitflow-0.1.3/src/tests/test_name.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/tests/test_setindex.py` & `slitflow-0.1.3/src/tests/test_setindex.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/tests/test_setreqs.py` & `slitflow-0.1.3/src/tests/test_setreqs.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/tests/test_tbl_convert.py` & `slitflow-0.1.3/src/tests/test_tbl_convert.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/tests/test_tbl_create.py` & `slitflow-0.1.3/src/tests/test_tbl_create.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/tests/test_tbl_filter.py` & `slitflow-0.1.3/src/tests/test_tbl_filter.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/tests/test_tbl_math.py` & `slitflow-0.1.3/src/tests/test_tbl_math.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/tests/test_tbl_proc.py` & `slitflow-0.1.3/src/tests/test_tbl_proc.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/tests/test_tbl_stat.py` & `slitflow-0.1.3/src/tests/test_tbl_stat.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/tests/test_tbl_table.py` & `slitflow-0.1.3/src/tests/test_tbl_table.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/tests/test_trj_filter.py` & `slitflow-0.1.3/src/tests/test_trj_filter.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/tests/test_trj_msd.py` & `slitflow-0.1.3/src/tests/test_trj_msd.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/tests/test_trj_random.py` & `slitflow-0.1.3/src/tests/test_trj_random.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/tests/test_trj_wfastspt.py` & `slitflow-0.1.3/src/tests/test_trj_wfastspt.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/tests/test_trj_wtrackpy.py` & `slitflow-0.1.3/src/tests/test_trj_wtrackpy.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.2/src/tests/test_trj_wtramway.py` & `slitflow-0.1.3/src/tests/test_trj_wtramway.py`

 * *Files identical despite different names*

