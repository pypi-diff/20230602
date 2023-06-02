# Comparing `tmp/most_queue-1.20.tar.gz` & `tmp/most_queue-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "most_queue-1.20.tar", last modified: Fri Jun  2 20:11:58 2023, max compression
+gzip compressed data, was "most_queue-1.3.tar", last modified: Wed May 17 17:44:11 2023, max compression
```

## Comparing `most_queue-1.20.tar` & `most_queue-1.3.tar`

### file list

```diff
@@ -1,92 +1,88 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 20:11:58.170381 most_queue-1.20/
--rw-rw-rw-   0        0        0     1091 2022-09-15 10:35:18.000000 most_queue-1.20/LICENSE
--rw-rw-rw-   0        0        0     6337 2023-06-02 20:11:58.170381 most_queue-1.20/PKG-INFO
--rw-rw-rw-   0        0        0     4545 2023-05-17 17:25:06.000000 most_queue-1.20/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 20:11:58.123708 most_queue-1.20/most_queue/
--rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most_queue-1.20/most_queue/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:11:58.135935 most_queue-1.20/most_queue/sim/
--rw-rw-rw-   0        0        0       78 2023-05-17 17:58:01.000000 most_queue-1.20/most_queue/sim/__init__.py
--rw-rw-rw-   0        0        0    13931 2023-06-02 19:10:20.000000 most_queue-1.20/most_queue/sim/fj_delta_im.py
--rw-rw-rw-   0        0        0    11089 2023-06-02 19:12:14.000000 most_queue-1.20/most_queue/sim/fj_im.py
--rw-rw-rw-   0        0        0    10084 2023-05-17 17:54:25.000000 most_queue-1.20/most_queue/sim/flow_sum_im.py
--rw-rw-rw-   0        0        0     9307 2023-06-02 19:38:06.000000 most_queue-1.20/most_queue/sim/network_im_prty.py
--rw-rw-rw-   0        0        0    12328 2023-06-02 19:38:06.000000 most_queue-1.20/most_queue/sim/queue_finite_source_sim.py
--rw-rw-rw-   0        0        0    37275 2023-05-17 17:54:25.000000 most_queue-1.20/most_queue/sim/rand_destribution.py
--rw-rw-rw-   0        0        0     3800 2023-05-17 17:54:25.000000 most_queue-1.20/most_queue/sim/smo_batch_sim.py
--rw-rw-rw-   0        0        0    31076 2023-06-02 19:34:00.000000 most_queue-1.20/most_queue/sim/smo_im.py
--rw-rw-rw-   0        0        0    37990 2023-06-02 20:04:15.000000 most_queue-1.20/most_queue/sim/smo_im_prty.py
--rw-rw-rw-   0        0        0     7658 2023-05-17 17:57:13.000000 most_queue-1.20/most_queue/sim/smo_impatient_im.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:11:58.148321 most_queue-1.20/most_queue/tests/
--rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most_queue-1.20/most_queue/tests/__init__.py
--rw-rw-rw-   0        0        0     3826 2023-05-17 17:18:04.000000 most_queue-1.20/most_queue/tests/ek_d_n.py
--rw-rw-rw-   0        0        0     5090 2023-05-17 18:17:47.000000 most_queue-1.20/most_queue/tests/fj_calc.py
--rw-rw-rw-   0        0        0     5539 2022-09-16 07:43:39.000000 most_queue-1.20/most_queue/tests/fj_im.py
--rw-rw-rw-   0        0        0     4278 2023-05-11 04:35:32.000000 most_queue-1.20/most_queue/tests/flow_sum.py
--rw-rw-rw-   0        0        0     5122 2022-09-16 08:17:30.000000 most_queue-1.20/most_queue/tests/gi_m_1_calc.py
--rw-rw-rw-   0        0        0     5258 2022-09-16 08:17:30.000000 most_queue-1.20/most_queue/tests/gi_m_n_calc.py
--rw-rw-rw-   0        0        0     2255 2022-09-16 08:20:45.000000 most_queue-1.20/most_queue/tests/m_d_n_calc.py
--rw-rw-rw-   0        0        0     3644 2023-05-17 18:41:32.000000 most_queue-1.20/most_queue/tests/m_h2_h2warm.py
--rw-rw-rw-   0        0        0     6712 2022-09-16 08:52:49.000000 most_queue-1.20/most_queue/tests/m_ph_n_prty.py
--rw-rw-rw-   0        0        0     5267 2022-09-20 18:59:53.000000 most_queue-1.20/most_queue/tests/mg1_calc.py
--rw-rw-rw-   0        0        0      982 2022-09-15 18:04:48.000000 most_queue-1.20/most_queue/tests/mg1_warm_calc.py
--rw-rw-rw-   0        0        0     4747 2023-05-08 07:36:11.000000 most_queue-1.20/most_queue/tests/mgn_tt.py
--rw-rw-rw-   0        0        0     3337 2022-09-15 18:04:48.000000 most_queue-1.20/most_queue/tests/mmn3_pnz_cox_approx.py
--rw-rw-rw-   0        0        0     2830 2022-09-15 18:04:48.000000 most_queue-1.20/most_queue/tests/mmn_prty_pnz_approx.py
--rw-rw-rw-   0        0        0     8149 2022-09-23 20:18:42.000000 most_queue-1.20/most_queue/tests/network_im_prty.py
--rw-rw-rw-   0        0        0    17534 2022-09-15 18:04:48.000000 most_queue-1.20/most_queue/tests/passage_time.py
--rw-rw-rw-   0        0        0     2744 2022-09-23 19:56:01.000000 most_queue-1.20/most_queue/tests/smo_im.py
--rw-rw-rw-   0        0        0     6545 2022-09-23 20:18:42.000000 most_queue-1.20/most_queue/tests/smo_im_prty.py
--rw-rw-rw-   0        0        0      967 2022-09-16 08:52:49.000000 most_queue-1.20/most_queue/tests/weibull.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:11:58.163872 most_queue-1.20/most_queue/theory/
--rw-rw-rw-   0        0        0       76 2023-05-17 17:43:06.000000 most_queue-1.20/most_queue/theory/__init__.py
--rw-rw-rw-   0        0        0     2360 2022-11-30 18:00:26.000000 most_queue-1.20/most_queue/theory/batch_mm1.py
--rw-rw-rw-   0        0        0     1304 2022-09-15 11:45:51.000000 most_queue-1.20/most_queue/theory/diff5dots.py
--rw-rw-rw-   0        0        0     6001 2023-06-02 19:50:03.000000 most_queue-1.20/most_queue/theory/ek_d_n_calc.py
--rw-rw-rw-   0        0        0     4741 2023-06-02 19:50:03.000000 most_queue-1.20/most_queue/theory/engset_model.py
--rw-rw-rw-   0        0        0    19289 2023-05-17 17:46:45.000000 most_queue-1.20/most_queue/theory/fj_calc.py
--rw-rw-rw-   0        0        0    10650 2023-05-17 17:35:09.000000 most_queue-1.20/most_queue/theory/flow_sum.py
--rw-rw-rw-   0        0        0     1626 2022-11-30 19:52:32.000000 most_queue-1.20/most_queue/theory/generate_pareto_noise.py
--rw-rw-rw-   0        0        0     4231 2023-06-02 19:52:43.000000 most_queue-1.20/most_queue/theory/gi_m_1_calc.py
--rw-rw-rw-   0        0        0     6171 2023-06-02 19:55:05.000000 most_queue-1.20/most_queue/theory/gi_m_n_calc.py
--rw-rw-rw-   0        0        0     2135 2022-11-29 13:43:22.000000 most_queue-1.20/most_queue/theory/impatience_calc.py
--rw-rw-rw-   0        0        0     4199 2023-06-02 19:56:01.000000 most_queue-1.20/most_queue/theory/m_d_n_calc.py
--rw-rw-rw-   0        0        0    27804 2023-06-02 20:00:16.000000 most_queue-1.20/most_queue/theory/m_h2_h2warm.py
--rw-rw-rw-   0        0        0    29730 2023-05-17 17:54:25.000000 most_queue-1.20/most_queue/theory/m_ph_n_prty.py
--rw-rw-rw-   0        0        0     4672 2023-06-02 20:00:16.000000 most_queue-1.20/most_queue/theory/mg1_calc.py
--rw-rw-rw-   0        0        0     1354 2023-06-02 20:02:08.000000 most_queue-1.20/most_queue/theory/mg1_warm_calc.py
--rw-rw-rw-   0        0        0    17357 2023-06-02 20:02:08.000000 most_queue-1.20/most_queue/theory/mgn_tt.py
--rw-rw-rw-   0        0        0    18821 2023-06-02 20:03:36.000000 most_queue-1.20/most_queue/theory/mmn3_pnz_cox_approx.py
--rw-rw-rw-   0        0        0    26711 2023-06-02 20:05:31.000000 most_queue-1.20/most_queue/theory/mmn_prty_pnz_approx.py
--rw-rw-rw-   0        0        0     1987 2023-05-17 17:54:25.000000 most_queue-1.20/most_queue/theory/mmnr_calc.py
--rw-rw-rw-   0        0        0     5777 2023-05-17 17:54:25.000000 most_queue-1.20/most_queue/theory/network_calc.py
--rw-rw-rw-   0        0        0     1066 2022-12-04 16:14:36.000000 most_queue-1.20/most_queue/theory/network_viewer.py
--rw-rw-rw-   0        0        0    40877 2023-05-18 21:35:04.000000 most_queue-1.20/most_queue/theory/passage_time.py
--rw-rw-rw-   0        0        0    17662 2023-05-17 17:54:25.000000 most_queue-1.20/most_queue/theory/prty_calc.py
--rw-rw-rw-   0        0        0     2174 2022-09-15 17:05:30.000000 most_queue-1.20/most_queue/theory/q_poisson_arrival_calc.py
--rw-rw-rw-   0        0        0     5396 2022-09-15 11:45:51.000000 most_queue-1.20/most_queue/theory/student_stat.py
--rw-rw-rw-   0        0        0      632 2022-09-15 11:45:51.000000 most_queue-1.20/most_queue/theory/sv_sum_calc.py
--rw-rw-rw-   0        0        0     4079 2022-09-15 12:02:16.000000 most_queue-1.20/most_queue/theory/weibull.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:11:58.165871 most_queue-1.20/most_queue/utils/
--rw-rw-rw-   0        0        0        0 2023-05-17 17:19:33.000000 most_queue-1.20/most_queue/utils/__init__.py
--rw-rw-rw-   0        0        0     2078 2023-05-17 17:18:48.000000 most_queue-1.20/most_queue/utils/approx_cdf_make.py
--rw-rw-rw-   0        0        0      319 2023-05-18 16:11:27.000000 most_queue-1.20/most_queue/utils/binom_probs.py
--rw-rw-rw-   0        0        0       62 2023-05-18 20:41:30.000000 most_queue-1.20/most_queue/utils/difstir.py
--rw-rw-rw-   0        0        0     2761 2023-06-02 20:11:23.000000 most_queue-1.20/most_queue/utils/tables.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:11:58.165871 most_queue-1.20/most_queue/visualisation/
--rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most_queue-1.20/most_queue/visualisation/__init__.py
--rw-rw-rw-   0        0        0    35629 2022-09-30 18:59:24.000000 most_queue-1.20/most_queue/visualisation/smo_im_vis.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:11:58.169383 most_queue-1.20/most_queue/visualisation/utils/
--rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most_queue-1.20/most_queue/visualisation/utils/__init__.py
--rw-rw-rw-   0        0        0     3169 2022-06-17 16:46:09.000000 most_queue-1.20/most_queue/visualisation/utils/result_table.py
--rw-rw-rw-   0        0        0    14872 2022-08-16 20:24:21.000000 most_queue-1.20/most_queue/visualisation/utils/settings_window.py
--rw-rw-rw-   0        0        0     1432 2022-06-03 20:22:54.000000 most_queue-1.20/most_queue/visualisation/utils/splash_screen.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:11:58.127303 most_queue-1.20/most_queue.egg-info/
--rw-rw-rw-   0        0        0     6337 2023-06-02 20:11:58.000000 most_queue-1.20/most_queue.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2594 2023-06-02 20:11:58.000000 most_queue-1.20/most_queue.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 20:11:58.000000 most_queue-1.20/most_queue.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-09-25 20:28:16.000000 most_queue-1.20/most_queue.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      114 2023-06-02 20:11:58.000000 most_queue-1.20/most_queue.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-02 20:11:58.000000 most_queue-1.20/most_queue.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      508 2023-06-02 20:11:38.000000 most_queue-1.20/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-02 20:11:58.170381 most_queue-1.20/setup.cfg
--rw-rw-rw-   0        0        0     1000 2023-06-02 20:11:32.000000 most_queue-1.20/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:44:11.336186 most_queue-1.3/
+-rw-rw-rw-   0        0        0     1091 2022-09-15 10:35:18.000000 most_queue-1.3/LICENSE
+-rw-rw-rw-   0        0        0     6336 2023-05-17 17:44:11.335121 most_queue-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4545 2023-05-17 17:25:06.000000 most_queue-1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 17:44:11.286991 most_queue-1.3/most_queue/
+-rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most_queue-1.3/most_queue/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:44:11.297810 most_queue-1.3/most_queue/sim/
+-rw-rw-rw-   0        0        0        0 2022-09-15 11:45:51.000000 most_queue-1.3/most_queue/sim/__init__.py
+-rw-rw-rw-   0        0        0    14589 2023-05-17 17:16:20.000000 most_queue-1.3/most_queue/sim/fj_delta_im.py
+-rw-rw-rw-   0        0        0    11132 2022-09-23 20:35:51.000000 most_queue-1.3/most_queue/sim/fj_im.py
+-rw-rw-rw-   0        0        0    10099 2022-09-15 12:02:16.000000 most_queue-1.3/most_queue/sim/flow_sum_im.py
+-rw-rw-rw-   0        0        0    10619 2022-12-01 20:31:07.000000 most_queue-1.3/most_queue/sim/network_im_prty.py
+-rw-rw-rw-   0        0        0    13161 2022-11-30 19:30:09.000000 most_queue-1.3/most_queue/sim/queue_finite_source_sim.py
+-rw-rw-rw-   0        0        0    37331 2023-01-25 13:05:08.000000 most_queue-1.3/most_queue/sim/rand_destribution.py
+-rw-rw-rw-   0        0        0     3913 2022-11-30 19:31:29.000000 most_queue-1.3/most_queue/sim/smo_batch_sim.py
+-rw-rw-rw-   0        0        0    25978 2022-11-30 17:51:13.000000 most_queue-1.3/most_queue/sim/smo_im.py
+-rw-rw-rw-   0        0        0    39946 2022-09-25 20:15:14.000000 most_queue-1.3/most_queue/sim/smo_im_prty.py
+-rw-rw-rw-   0        0        0     7724 2022-11-29 20:49:52.000000 most_queue-1.3/most_queue/sim/smo_impatient_im.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:44:11.310410 most_queue-1.3/most_queue/tests/
+-rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most_queue-1.3/most_queue/tests/__init__.py
+-rw-rw-rw-   0        0        0     3826 2023-05-17 17:18:04.000000 most_queue-1.3/most_queue/tests/ek_d_n.py
+-rw-rw-rw-   0        0        0     4997 2022-09-16 07:21:38.000000 most_queue-1.3/most_queue/tests/fj_calc.py
+-rw-rw-rw-   0        0        0     5539 2022-09-16 07:43:39.000000 most_queue-1.3/most_queue/tests/fj_im.py
+-rw-rw-rw-   0        0        0     4278 2023-05-11 04:35:32.000000 most_queue-1.3/most_queue/tests/flow_sum.py
+-rw-rw-rw-   0        0        0     5122 2022-09-16 08:17:30.000000 most_queue-1.3/most_queue/tests/gi_m_1_calc.py
+-rw-rw-rw-   0        0        0     5258 2022-09-16 08:17:30.000000 most_queue-1.3/most_queue/tests/gi_m_n_calc.py
+-rw-rw-rw-   0        0        0     2255 2022-09-16 08:20:45.000000 most_queue-1.3/most_queue/tests/m_d_n_calc.py
+-rw-rw-rw-   0        0        0     6712 2022-09-16 08:52:49.000000 most_queue-1.3/most_queue/tests/m_ph_n_prty.py
+-rw-rw-rw-   0        0        0     5267 2022-09-20 18:59:53.000000 most_queue-1.3/most_queue/tests/mg1_calc.py
+-rw-rw-rw-   0        0        0      982 2022-09-15 18:04:48.000000 most_queue-1.3/most_queue/tests/mg1_warm_calc.py
+-rw-rw-rw-   0        0        0     4747 2023-05-08 07:36:11.000000 most_queue-1.3/most_queue/tests/mgn_tt.py
+-rw-rw-rw-   0        0        0     3337 2022-09-15 18:04:48.000000 most_queue-1.3/most_queue/tests/mmn3_pnz_cox_approx.py
+-rw-rw-rw-   0        0        0     2830 2022-09-15 18:04:48.000000 most_queue-1.3/most_queue/tests/mmn_prty_pnz_approx.py
+-rw-rw-rw-   0        0        0     8149 2022-09-23 20:18:42.000000 most_queue-1.3/most_queue/tests/network_im_prty.py
+-rw-rw-rw-   0        0        0    17534 2022-09-15 18:04:48.000000 most_queue-1.3/most_queue/tests/passage_time.py
+-rw-rw-rw-   0        0        0     2744 2022-09-23 19:56:01.000000 most_queue-1.3/most_queue/tests/smo_im.py
+-rw-rw-rw-   0        0        0     6545 2022-09-23 20:18:42.000000 most_queue-1.3/most_queue/tests/smo_im_prty.py
+-rw-rw-rw-   0        0        0      967 2022-09-16 08:52:49.000000 most_queue-1.3/most_queue/tests/weibull.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:44:11.329668 most_queue-1.3/most_queue/theory/
+-rw-rw-rw-   0        0        0       76 2023-05-17 17:43:06.000000 most_queue-1.3/most_queue/theory/__init__.py
+-rw-rw-rw-   0        0        0     2360 2022-11-30 18:00:26.000000 most_queue-1.3/most_queue/theory/batch_mm1.py
+-rw-rw-rw-   0        0        0     1304 2022-09-15 11:45:51.000000 most_queue-1.3/most_queue/theory/diff5dots.py
+-rw-rw-rw-   0        0        0     6193 2022-09-15 16:51:31.000000 most_queue-1.3/most_queue/theory/ek_d_n_calc.py
+-rw-rw-rw-   0        0        0     4688 2023-05-17 17:43:06.000000 most_queue-1.3/most_queue/theory/engset_model.py
+-rw-rw-rw-   0        0        0    19284 2023-05-17 17:43:30.000000 most_queue-1.3/most_queue/theory/fj_calc.py
+-rw-rw-rw-   0        0        0    10650 2023-05-17 17:35:09.000000 most_queue-1.3/most_queue/theory/flow_sum.py
+-rw-rw-rw-   0        0        0     1626 2022-11-30 19:52:32.000000 most_queue-1.3/most_queue/theory/generate_pareto_noise.py
+-rw-rw-rw-   0        0        0     5877 2023-05-17 17:40:32.000000 most_queue-1.3/most_queue/theory/gi_m_1_calc.py
+-rw-rw-rw-   0        0        0     7888 2022-09-15 16:55:53.000000 most_queue-1.3/most_queue/theory/gi_m_n_calc.py
+-rw-rw-rw-   0        0        0     2135 2022-11-29 13:43:22.000000 most_queue-1.3/most_queue/theory/impatience_calc.py
+-rw-rw-rw-   0        0        0     4474 2022-09-15 16:56:34.000000 most_queue-1.3/most_queue/theory/m_d_n_calc.py
+-rw-rw-rw-   0        0        0    22232 2023-05-17 14:00:37.000000 most_queue-1.3/most_queue/theory/m_h2_h2warm.py
+-rw-rw-rw-   0        0        0    29777 2022-09-15 16:57:11.000000 most_queue-1.3/most_queue/theory/m_ph_n_prty.py
+-rw-rw-rw-   0        0        0     7316 2022-09-15 16:57:53.000000 most_queue-1.3/most_queue/theory/mg1_calc.py
+-rw-rw-rw-   0        0        0     1625 2022-09-15 16:58:37.000000 most_queue-1.3/most_queue/theory/mg1_warm_calc.py
+-rw-rw-rw-   0        0        0    23133 2023-05-16 19:00:21.000000 most_queue-1.3/most_queue/theory/mgn_tt.py
+-rw-rw-rw-   0        0        0    18992 2022-09-15 17:02:09.000000 most_queue-1.3/most_queue/theory/mmn3_pnz_cox_approx.py
+-rw-rw-rw-   0        0        0    26829 2022-09-15 17:03:10.000000 most_queue-1.3/most_queue/theory/mmn_prty_pnz_approx.py
+-rw-rw-rw-   0        0        0     2010 2022-09-15 17:01:13.000000 most_queue-1.3/most_queue/theory/mmnr_calc.py
+-rw-rw-rw-   0        0        0     5816 2022-09-23 20:42:20.000000 most_queue-1.3/most_queue/theory/network_calc.py
+-rw-rw-rw-   0        0        0     1066 2022-12-04 16:14:36.000000 most_queue-1.3/most_queue/theory/network_viewer.py
+-rw-rw-rw-   0        0        0    40783 2022-09-15 17:04:24.000000 most_queue-1.3/most_queue/theory/passage_time.py
+-rw-rw-rw-   0        0        0    17732 2022-09-15 17:05:30.000000 most_queue-1.3/most_queue/theory/prty_calc.py
+-rw-rw-rw-   0        0        0     2174 2022-09-15 17:05:30.000000 most_queue-1.3/most_queue/theory/q_poisson_arrival_calc.py
+-rw-rw-rw-   0        0        0     5396 2022-09-15 11:45:51.000000 most_queue-1.3/most_queue/theory/student_stat.py
+-rw-rw-rw-   0        0        0      632 2022-09-15 11:45:51.000000 most_queue-1.3/most_queue/theory/sv_sum_calc.py
+-rw-rw-rw-   0        0        0     4079 2022-09-15 12:02:16.000000 most_queue-1.3/most_queue/theory/weibull.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:44:11.330442 most_queue-1.3/most_queue/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-17 17:19:33.000000 most_queue-1.3/most_queue/utils/__init__.py
+-rw-rw-rw-   0        0        0     2078 2023-05-17 17:18:48.000000 most_queue-1.3/most_queue/utils/approx_cdf_make.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:44:11.331482 most_queue-1.3/most_queue/visualisation/
+-rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most_queue-1.3/most_queue/visualisation/__init__.py
+-rw-rw-rw-   0        0        0    35629 2022-09-30 18:59:24.000000 most_queue-1.3/most_queue/visualisation/smo_im_vis.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:44:11.333901 most_queue-1.3/most_queue/visualisation/utils/
+-rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most_queue-1.3/most_queue/visualisation/utils/__init__.py
+-rw-rw-rw-   0        0        0     3169 2022-06-17 16:46:09.000000 most_queue-1.3/most_queue/visualisation/utils/result_table.py
+-rw-rw-rw-   0        0        0    14872 2022-08-16 20:24:21.000000 most_queue-1.3/most_queue/visualisation/utils/settings_window.py
+-rw-rw-rw-   0        0        0     1432 2022-06-03 20:22:54.000000 most_queue-1.3/most_queue/visualisation/utils/splash_screen.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:44:11.291816 most_queue-1.3/most_queue.egg-info/
+-rw-rw-rw-   0        0        0     6336 2023-05-17 17:44:11.000000 most_queue-1.3/most_queue.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2475 2023-05-17 17:44:11.000000 most_queue-1.3/most_queue.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 17:44:11.000000 most_queue-1.3/most_queue.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-09-25 20:28:16.000000 most_queue-1.3/most_queue.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      105 2023-05-17 17:44:11.000000 most_queue-1.3/most_queue.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-17 17:44:11.000000 most_queue-1.3/most_queue.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      508 2023-05-17 17:43:52.000000 most_queue-1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-17 17:44:11.336866 most_queue-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      975 2023-05-17 17:43:57.000000 most_queue-1.3/setup.py
```

### Comparing `most_queue-1.20/LICENSE` & `most_queue-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/PKG-INFO` & `most_queue-1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: most_queue
-Version: 1.20
+Version: 1.3
 Summary: Software package for calculation and simulation of queuing systems
 Home-page: https://github.com/xabarov/mps
 Author: Xabarov Roman
 Author-email: Xabarov Roman <xabarov1985@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `most_queue-1.20/README.md` & `most_queue-1.3/README.md`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/sim/fj_delta_im.py` & `most_queue-1.3/most_queue/sim/fj_delta_im.py`

 * *Files 5% similar despite different names*

```diff
@@ -297,18 +297,17 @@
             res += "\nQueue Count " + str(len(self.queue)) + "\n"
 
         return res
 
 
 if __name__ == '__main__':
 
-    from most_queue.theory import mg1_calc
+    from  most_queue.theory import mg1_calc
     from most_queue.theory import fj_calc
     from most_queue.theory import mg1_warm_calc
-    from most_queue.utils.tables import times_print
 
     n = 3
     l = 1.0
     b1 = 0.35
     coev = 1.2
     b1_delta = 0.1
     b_params = rd.H2_dist.get_params_by_mean_and_coev(b1, coev)
@@ -332,16 +331,21 @@
     print("-" * 60)
     print("{:^60s}".format('СМО Split-Join c задержкой начала обслуживания'))
     print("-" * 60)
     print("Коэфф вариации времени обслуживания: ", coev)
     print("Среднее время задежки начала обслуживания: {:4.3f}".format(b1_delta))
     print("Коэфф вариации времени задержки: {:4.3f}".format(coev))
     print("Коэффициент загрузки: {:4.3f}".format(ro))
-
-    times_print(v_im, v_ch, is_w=False)
+    print("Начальные моменты времени пребывания заявок в системе:")
+    print("-" * 60)
+    print("{0:^15s}|{1:^20s}|{2:^20s}".format("№ момента", "Числ", "ИМ"))
+    print("-" * 60)
+    for j in range(min(len(v_ch), len(v_im))):
+        print("{0:^16d}|{1:^20.5g}|{2:^20.5g}".format(j + 1, v_ch[j], v_im[j]))
+    print("-" * 60)
 
     coev = 0.53
     b1 = 0.5
 
     b1_delta = 0.1
     delta_params = rd.Erlang_dist.get_params_by_mean_and_coev(b1_delta, coev)
     b_delta = rd.Erlang_dist.calc_theory_moments(*delta_params)
@@ -360,9 +364,14 @@
     ro = l * b_max[0]
     v_ch = mg1_warm_calc.get_v(l, b_max, b_max_warm)
 
     print("\n\nКоэфф вариации времени обслуживания: ", coev)
     print("Коэффициент загрузки: {:4.3f}".format(ro))
     print("Среднее время задежки начала обслуживания: {:4.3f}".format(b1_delta))
     print("Коэфф вариации времени задержки: {:4.3f}".format(coev))
-
-    times_print(v_im, v_ch, is_w=False)
+    print("Начальные моменты времени пребывания заявок в системе:")
+    print("-" * 60)
+    print("{0:^15s}|{1:^20s}|{2:^20s}".format("№ момента", "Числ", "ИМ"))
+    print("-" * 60)
+    for j in range(min(len(v_ch), len(v_im))):
+        print("{0:^16d}|{1:^20.5g}|{2:^20.5g}".format(j + 1, v_ch[j], v_im[j]))
+    print("-" * 60)
```

### Comparing `most_queue-1.20/most_queue/sim/fj_im.py` & `most_queue-1.3/most_queue/sim/fj_im.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,12 @@
-import rand_destribution as rd
+import most_queue.sim.rand_destribution as rd
 from most_queue.sim import smo_im
 import math
-import sys
 from tqdm import tqdm
-
-from colorama import init
-from colorama import Fore, Style
-
-init()
+import sys
 
 class SubTask:
     """
     Позадача
     """
     sub_task_id = 0
 
@@ -194,34 +189,19 @@
         # Key moment:
 
         if self.arrival_time < serv_earl:
             self.arrival()
         else:
             self.serving(num_of_server_earlier)
 
-    def run(self, total_served, is_real_served=False):
-
-        if is_real_served:
-            served_old = 0
-            while self.served < total_served:
-                self.run_one_step()
-                if (self.served - served_old) % 5000 == 0:
-                    sys.stderr.write('\rStart simulation. Job served: %d/%d' % (self.served, total_served))
-                    sys.stderr.flush()
-                served_old = self.served
-        else:
-            print(Fore.GREEN + '\rStart simulation')
-            print(Style.RESET_ALL)
-            # print(Back.YELLOW + 'на желтом фоне')
-
-            for i in tqdm(range(total_served)):
-                self.run_one_step()
-
-            print(Fore.GREEN + '\rSimulation is finished')
-            print(Style.RESET_ALL)
+    def run(self, total_served):
+        while (self.served < total_served):
+            self.run_one_step()
+            sys.stderr.write('\rStart simulation. Job served: %d/%d' % (self.served, total_served))
+            sys.stderr.flush()
 
     def refresh_v_stat(self, new_a):
         for i in range(3):
             self.v[i] = self.v[i] * (1.0 - (1.0 / self.served)) + math.pow(new_a, i + 1) / self.served
 
     def get_p(self):
         """
@@ -278,15 +258,14 @@
         return text
 
 
 if __name__ == '__main__':
 
     from most_queue.theory import mg1_calc
     from most_queue.theory import fj_calc
-    from most_queue.utils.tables import times_print
 
     n = 3
     l = 1.0
     b1 = 0.37
     coev = 1.5
     params = rd.H2_dist.get_params_by_mean_and_coev(b1, coev)
     b = rd.H2_dist.calc_theory_moments(*params, 4)
@@ -303,15 +282,21 @@
 
     print("\n")
     print("-" * 60)
     print("{:^60s}".format('СМО Split-Join'))
     print("-" * 60)
     print("Коэфф вариации времени обслуживания: ", coev)
     print("Коэффициент загрузки: {:4.3f}".format(ro))
-    times_print(v_im, v_ch, is_w=False)
+    print("Начальные моменты времени пребывания заявок в системе:")
+    print("-" * 60)
+    print("{0:^15s}|{1:^20s}|{2:^20s}".format("№ момента", "Числ", "ИМ"))
+    print("-" * 60)
+    for j in range(min(len(v_ch), len(v_im))):
+        print("{0:^16d}|{1:^20.5g}|{2:^20.5g}".format(j + 1, v_ch[j], v_im[j]))
+    print("-" * 60)
 
     coev = 0.8
     b1 = 0.5
     params = rd.Erlang_dist.get_params_by_mean_and_coev(b1, coev)
     b = rd.Erlang_dist.calc_theory_moments(*params, 4)
 
     smo = SmoFJ(n, n, True)
@@ -322,8 +307,14 @@
 
     b_max = fj_calc.getMaxMoments(n, b, 4)
     ro = l * b_max[0]
     v_ch = mg1_calc.get_v(l, b_max)
 
     print("\n\nКоэфф вариации времени обслуживания: ", coev)
     print("Коэффициент загрузки: {:4.3f}".format(ro))
-    times_print(v_im, v_ch, is_w=False)
+    print("Начальные моменты времени пребывания заявок в системе:")
+    print("-" * 60)
+    print("{0:^15s}|{1:^20s}|{2:^20s}".format("№ момента", "Числ", "ИМ"))
+    print("-" * 60)
+    for j in range(min(len(v_ch), len(v_im))):
+        print("{0:^16d}|{1:^20.5g}|{2:^20.5g}".format(j + 1, v_ch[j], v_im[j]))
+    print("-" * 60)
```

### Comparing `most_queue-1.20/most_queue/sim/flow_sum_im.py` & `most_queue-1.3/most_queue/sim/flow_sum_im.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import rand_destribution as rd
+import most_queue.sim.rand_destribution as rd
 from tqdm import tqdm
 import copy
 import math
 
 
 class SummatorIM:
```

### Comparing `most_queue-1.20/most_queue/sim/network_im_prty.py` & `most_queue-1.3/most_queue/sim/network_im_prty.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,17 @@
-from smo_im_prty import SmoImPrty
-import rand_destribution as rd
+from most_queue.sim.smo_im_prty import SmoImPrty
+import most_queue.sim.rand_destribution as rd
 import numpy as np
 import math
-from smo_im_prty import Task
+from most_queue.sim.smo_im_prty import Task
 from most_queue.theory import network_calc
 import time
 from tqdm import tqdm
 import sys
 
-from colorama import init
-from colorama import Fore, Style
-
-init()
-
 class NetworkPrty:
     """
     Имитационная модель СеМО с многоканальными узлами и приоритетами
     """
 
     def __init__(self, k_num, L, R, n, prty, serv_params, nodes_prty):
 
@@ -134,35 +129,26 @@
             else:
                 next_node_class = self.nodes_prty[next_node][real_class]
 
                 self.smos[next_node].arrival(next_node_class, self.ttek, ts)
 
     def run(self, job_served, is_real_served=False):
         if is_real_served:
-            while sum(self.served) < job_served:
+            while (sum(self.served) < job_served):
                 self.run_one_step()
                 sys.stderr.write('\rStart simulation. Job served: %d/%d' % (sum(self.served), job_served))
                 sys.stderr.flush()
         else:
-            print(Fore.GREEN + '\rStart simulation')
-            print(Style.RESET_ALL)
-            # print(Back.YELLOW + 'на желтом фоне')
-
+            print("Start simulation...\n")
             for i in tqdm(range(job_served)):
                 self.run_one_step()
 
-            print(Fore.GREEN + '\rSimulation is finished')
-            print(Style.RESET_ALL)
-
 
 
 if __name__ == '__main__':
-
-    from most_queue.utils.tables import times_print_with_classes
-
     k_num = 3
     n_num = 5
     n = [3, 2, 3, 4, 3]
     R = []
     b = []  # k, node, j
     for i in range(k_num):
         R.append(np.matrix([
@@ -214,32 +200,84 @@
     print("-" * 60)
     print("{0:^60s}\n{1:^60s}".format("Сравнение данных ИМ и результатов расчета времени пребывания",
                                       "в СеМО с многоканальными узлами и приоритетами"))
     print("-" * 60)
     print("Количество каналов в узлах:")
     for nn in n:
         print("{0:^1d}".format(nn), end=" ")
-    print("\nКоэффициенты загрузки узлов:")
+    print("\nКоэффициенты загрузки узлов :")
     for load in loads:
         print("{0:^1.3f}".format(load), end=" ")
     print("\n")
     print("-" * 60)
     print("{0:^60s}".format("Относительный приоритет"))
 
     print("-" * 60)
-    times_print_with_classes(v_im, v_ch, is_w=False)
+    print("{0:^11s}|{1:^47s}|".format('', 'Номер начального момента'))
+    print("{0:^10s}| ".format('№ кл'), end="")
+    print("-" * 45 + " |")
+
+    print(" " * 11 + "|", end="")
+    for j in range(3):
+        s = str(j + 1)
+        print("{:^15s}|".format(s), end="")
+    print("")
+    print("-" * 60)
+
+    for i in range(k_num):
+        print(" " * 5 + "|", end="")
+        print("{:^5s}|".format("ИМ"), end="")
+        for j in range(3):
+            print("{:^15.3g}|".format(v_im[i][j]), end="")
+        print("")
+        print("{:^5s}".format(str(i + 1)) + "|" + "-" * 54)
+
+        print(" " * 5 + "|", end="")
+        print("{:^5s}|".format("Р"), end="")
+        for j in range(3):
+            print("{:^15.3g}|".format(v_ch[i][j]), end="")
+        print("")
+        print("-" * 60)
+
+    print("\n")
 
     prty = ['PR'] * n_num
     semo_im = NetworkPrty(k_num, L, R, n, prty, serv_params, nodes_prty)
 
     semo_im.run(jobs_num)
 
     v_im = semo_im.v_semo
 
     semo_calc = network_calc.network_prty_calc(R, b, n, L, prty, nodes_prty)
     v_ch = semo_calc['v']
 
     print("-" * 60)
     print("{0:^60s}".format("Абсолютный приоритет"))
+
     print("-" * 60)
+    print("{0:^11s}|{1:^47s}|".format('', 'Номер начального момента'))
+    print("{0:^10s}| ".format('№ кл'), end="")
+    print("-" * 45 + " |")
+
+    print(" " * 11 + "|", end="")
+    for j in range(3):
+        s = str(j + 1)
+        print("{:^15s}|".format(s), end="")
+    print("")
+    print("-" * 60)
+
+    for i in range(k_num):
+        print(" " * 5 + "|", end="")
+        print("{:^5s}|".format("ИМ"), end="")
+        for j in range(3):
+            print("{:^15.3g}|".format(v_im[i][j]), end="")
+        print("")
+        print("{:^5s}".format(str(i + 1)) + "|" + "-" * 54)
+
+        print(" " * 5 + "|", end="")
+        print("{:^5s}|".format("Р"), end="")
+        for j in range(3):
+            print("{:^15.3g}|".format(v_ch[i][j]), end="")
+        print("")
+        print("-" * 60)
 
-    times_print_with_classes(v_im, v_ch, is_w=False)
+    print("\n")
```

### Comparing `most_queue-1.20/most_queue/sim/queue_finite_source_sim.py` & `most_queue-1.3/most_queue/sim/queue_finite_source_sim.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,13 @@
-import rand_destribution as rd
-from smo_im import SmoIm, SetSmoException, Task
+import most_queue.sim.rand_destribution as rd
+import math
+from tqdm import tqdm
+import sys
+import time
+from most_queue.sim.smo_im import SmoIm, SetSmoException, Task
 
 
 class QueueFiniteSourceSim(SmoIm):
     """
     Имитационная модель СМО GI/G/n/r и GI/G/n с конечным числом источников заявок
     """
 
@@ -270,15 +274,14 @@
             res += "\nQueue Count " + str(len(self.queue)) + "\n"
 
         return res
 
 
 if __name__ == '__main__':
     from most_queue.theory.engset_model import Engset
-    from most_queue.utils.tables import probs_print, times_print
 
     lam = 0.9
     mu = 1.0
     m = 4
     n = 1
 
     num_of_jobs = 1000000
@@ -293,11 +296,26 @@
 
     smo.run(num_of_jobs)
 
     v_im = smo.v
     p_im = smo.get_p()
     p_ch = engset.get_p()
 
-    probs_print(p_im, p_ch, 10)
+    print(f'Вероятности состояний системы')
+    header = "{0:^15s}|{1:^15s}|{2:^15s}".format('№', 'Числ', 'ИМ')
+    print('-' * len(header))
+    print(header)
+    print('-' * len(header))
+    for i in range(len(p_im)):
+        print("{0:^15d}|{1:^15.3f}|{2:^15.3f}".format(i, p_ch[i], p_im[i]))
+    print('-' * len(header))
+    print("{0:^15s}|{1:^15.3f}|{2:^15.3f}".format('Сумм', sum(p_ch), sum(p_im)))
+    print('-' * len(header))
 
     print("Time spent ", smo.time_spent)
-    times_print(v_im, v, is_w=False)
+    print("\nЗначения начальных моментов времени пребывания заявок в системе:\n")
+
+    print("{0:^15s}|{1:^15s}|{2:^15s}".format("№ момента", "Числ", "ИМ"))
+    print("-" * 45)
+    for j in range(3):
+        print("{0:^16d}|{1:^15.5g}|{2:^15.5g}".format(j + 1, v[j], v_im[j]))
+    print("\n\nДанные ИМ::\n")
```

### Comparing `most_queue-1.20/most_queue/sim/rand_destribution.py` & `most_queue-1.3/most_queue/sim/rand_destribution.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from scipy import stats
-from numba.cuda.random import xoroshiro128p_uniform_float32
-from numba import cuda
-
 import numpy as np
-import cmath
+import math, cmath
+from scipy import stats
 import scipy.special as sp
+from numba import jit
+from numba.cuda.random import create_xoroshiro128p_states, xoroshiro128p_uniform_float32
+from numba import cuda
 import math
 
 
 @cuda.jit
 def generate_h2_jit(rng_states, y1, mu1, mu2, out):
     """
     Генерация псевдо-случайных чисел, подчиненных гиперэкспоненциальному распределению 2-го порядка
```

### Comparing `most_queue-1.20/most_queue/sim/smo_batch_sim.py` & `most_queue-1.3/most_queue/sim/smo_batch_sim.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-from smo_im import SmoIm, Task
-
+import most_queue.sim.rand_destribution as rd
+import math
+from tqdm import tqdm
+from most_queue.sim.smo_im import SmoIm, SetSmoException, Task
 import numpy as np
 
 
 class SmoBatchSim(SmoIm):
     def __init__(self, num_of_channels, batch_prob, buffer=None, verbose=True):
         super().__init__(num_of_channels, buffer, verbose)
```

### Comparing `most_queue-1.20/most_queue/sim/smo_im.py` & `most_queue-1.3/most_queue/sim/smo_im.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,20 @@
-import numpy as np
-
-import rand_destribution as rd
+import most_queue.sim.rand_destribution as rd
 import math
 from tqdm import tqdm
-import time
 import sys
-
-from colorama import init
-from colorama import Fore, Style
-
-init()
-
+import time
 
 class SmoIm:
     """
     Имитационная модель СМО GI/G/n/r и GI/G/n
     """
 
     def __init__(self, num_of_channels, buffer=None, verbose=True, calc_next_event_time=False, cuda=False):
         """
-        Конструктор
         num_of_channels - количество каналов СМО
         buffer - максимальная длина очереди
         verbose - вывод комментариев в процессе ИМ
         calc_next_event_time - нужно ли осуществлять расчет времени для след события (используется для визуализации)
         cuda - нужно ли использовать ускорение GPU при генерации заявок. Прирост в скорости небольшой, поэтому
         по умолчанию cuda=False
 
@@ -78,65 +69,31 @@
         self.source_types = None
         self.server_params = None
         self.server_types = None
 
         self.is_set_source_params = False
         self.is_set_server_params = False
         self.is_set_warm = False
-        self.is_start_warm = False
-        self.end_warm_time = 1e12
 
-    def set_warm(self, params, types, is_only_first=False):
+    def set_warm(self, params, types):
         """
             Задает тип и параметры распределения времени обслуживания с разогревом
             --------------------------------------------------------------------
             Вид распределения                   Тип[types]     Параметры [params]
             Экспоненциальное                      'М'             [mu]
             Гиперэкспоненциальное 2-го порядка    'Н'         [y1, mu1, mu2]
             Эрланга                               'E'           [r, mu]
             Кокса 2-го порядка                    'C'         [y1, mu1, mu2]
             Парето                                'Pa'         [alpha, K]
             Детерминированное                      'D'         [b]
             Равномерное                         'Uniform'     [mean, half_interval]
             Нормальное                            'Norm'    [mean, standard_deviation]
-
-            is_only_first - True: Разогрев происходит только при прибытии первой заявки в пустую систему.
-                            В таком случае время разогрева - время обслуживания первой заявки
-                            False: Разогрев происходит для всей системы. Каналы не начинают обслуживания до тех пор,
-                            пока не закончится период разогрева
-        """
-        if is_only_first:
-            for i in range(self.n):
-                self.servers[i].set_warm(params, types)
-        else:
-            if types == "M":
-                self.warm_dist = rd.Exp_dist(params)
-            elif types == "H":
-                self.warm_dist = rd.H2_dist(params)
-            elif types == "E":
-                self.warm_dist = rd.Erlang_dist(params)
-            elif types == "Gamma":
-                self.warm_dist = rd.Gamma(params)
-            elif types == "C":
-                self.warm_dist = rd.Cox_dist(params)
-            elif types == "Pa":
-                self.warm_dist = rd.Pareto_dist(params)
-            elif types == "Unifrorm":
-                self.warm_dist = rd.Uniform_dist(params)
-            elif types == "Norm":
-                self.warm_dist = rd.Normal_dist(params)
-            elif types == "D":
-                self.warm_dist = rd.Det_dist(params)
-            else:
-                raise SetSmoException(
-                    "Неправильно задан тип распределения времени обсл с разогревом. Варианты М, Н, Е, С, Pa, Uniform, Norm, D")
-
-        self.is_set_warm = True
-
-        self.is_only_first = is_only_first
+        """
+        for i in range(self.n):
+            self.servers[i].set_warm(params, types)
 
     def set_sources(self, params, types):
         """
         Задает тип и параметры распределения интервала поступления заявок.
         --------------------------------------------------------------------
         Вид распределения                   Тип[types]     Параметры [params]
         Экспоненциальное                      'М'             [mu]
@@ -169,16 +126,15 @@
         elif self.source_types == "Uniform":
             self.source = rd.Uniform_dist(self.source_params)
         elif self.source_types == "Norm":
             self.source = rd.Normal_dist(self.source_params)
         elif self.source_types == "D":
             self.source = rd.Det_dist(self.source_params)
         else:
-            raise SetSmoException(
-                "Неправильно задан тип распределения источника. Варианты М, Н, Е, С, Pa, Norm, Uniform")
+            raise SetSmoException("Неправильно задан тип распределения источника. Варианты М, Н, Е, С, Pa, Norm, Uniform")
         self.arrival_time = self.source.generate()
 
     def set_servers(self, params, types):
         """
         Задает тип и параметры распределения времени обслуживания.
         Вид распределения                   Тип[types]     Параметры [params]
         Экспоненциальное                      'М'             [mu]
@@ -288,45 +244,14 @@
             else:
                 a = self.server_params[0]
                 k = self.server_params[1]
                 b1 = a * k / (a - 1)
 
         return l * b1 / self.n
 
-    def send_task_to_channel(self, is_warm_start):
-        # Отправляет заявку в канал обслуживания
-        # is_warm_start- нужен ли разогрев
-        for s in self.servers:
-            if s.is_free:
-                self.taked += 1
-
-                s.start_service(Task(self.ttek), self.ttek, is_warm_start)
-                self.free_channels -= 1
-
-                # Проверям, не наступил ли ПНЗ:
-                if self.free_channels == 0:
-                    if self.in_sys == self.n:
-                        self.start_ppnz = self.ttek
-
-                break
-
-    def send_task_to_queue(self):
-        if self.buffer == None:  # не задана длина очереди, т.е бесконечная очередь
-            new_tsk = Task(self.ttek)
-            new_tsk.start_waiting_time = self.ttek
-            self.queue.append(new_tsk)
-        else:
-            if len(self.queue) < self.buffer:
-                new_tsk = Task(self.ttek)
-                new_tsk.start_waiting_time = self.ttek
-                self.queue.append(new_tsk)
-            else:
-                self.dropped += 1
-                self.in_sys -= 1
-
     def arrival(self):
 
         """
         Действия по прибытию заявки в СМО.
         """
 
         self.arrived += 1
@@ -340,46 +265,45 @@
             self.tek_source_num += 1
             if self.tek_source_num == len(self.source_random_vars):
                 self.tek_source_num = 0
         else:
             self.arrival_time = self.ttek + self.source.generate()
 
         if self.free_channels == 0:
-            self.send_task_to_queue()
+            if self.buffer == None:  # не задана длина очередиб т.е бесконечная очередь
+                new_tsk = Task(self.ttek)
+                new_tsk.start_waiting_time = self.ttek
+                self.queue.append(new_tsk)
+            else:
+                if len(self.queue) < self.buffer:
+                    new_tsk = Task(self.ttek)
+                    new_tsk.start_waiting_time = self.ttek
+                    self.queue.append(new_tsk)
+                else:
+                    self.dropped += 1
+                    self.in_sys -= 1
 
         else:  # there are free channels:
 
-            # check if it's a warm phase:
-            if self.is_set_warm:
-                # Задан разогрев
-                if self.is_only_first:
-                    # Только первой заявки. Проверяем, не пустая ли система.
-                    # Если пустая - задаем is_warm_start
-                    if len(self.queue) == 0 and self.free_channels == self.n:
-                        is_warm_start = True
-
-                    self.send_task_to_channel(is_warm_start)
-                else:
-                    # Разогрев глобальный.
-                    if self.is_start_warm:
-                        # Уже в режиме разогрева
-                        self.send_task_to_queue()
-                    else:
-                        # Еще нет. Проверяем надо ли запускать разогрев
-                        if len(self.queue) == 0 and self.free_channels == self.n:
-                            self.is_start_warm = True
-                            self.end_warm_time = self.ttek + self.warm_dist.generate()
-                            # Отправляем заявку в очередь. После окончания времени разогрева она начнет обслуживаться
-                            self.send_task_to_queue()
-                        else:
-                            self.send_task_to_channel(False)
-
-            else:
-                # Без разогрева. Отправляем заявку в канал обслуживания
-                self.send_task_to_channel(False)
+            # check if its a warm phase:
+            is_warm_start = False
+            if len(self.queue) == 0 and self.free_channels == self.n and self.is_set_warm:
+                is_warm_start = True
+
+            for s in self.servers:
+                if s.is_free:
+                    self.taked += 1
+                    s.start_service(Task(self.ttek), self.ttek, is_warm_start)
+                    self.free_channels -= 1
+
+                    # Проверям, не наступил ли ПНЗ:
+                    if self.free_channels == 0:
+                        if self.in_sys == self.n:
+                            self.start_ppnz = self.ttek
+                    break
 
     def serving(self, c):
         """
         Дейтсвия по поступлению заявки на обслуживание
         с - номер канала
         """
         time_to_end = self.servers[c].time_to_end_service
@@ -399,132 +323,90 @@
         if len(self.queue) == 0 and self.free_channels == 1:
             if self.in_sys == self.n - 1:
                 # Конец ПНЗ
                 self.ppnz_moments += 1
                 self.refresh_ppnz_stat(self.ttek - self.start_ppnz)
 
         if len(self.queue) != 0:
-            self.send_head_of_queue_to_channel(c)
 
-    def send_head_of_queue_to_channel(self, channel_num):
-        que_ts = self.queue.pop(0)
+            que_ts = self.queue.pop(0)
 
-        if self.free_channels == 1:
-            self.start_ppnz = self.ttek
+            if self.free_channels == 1:
+                self.start_ppnz = self.ttek
 
-        self.taked += 1
-        que_ts.wait_time += self.ttek - que_ts.start_waiting_time
-        self.servers[channel_num].start_service(que_ts, self.ttek)
-        self.free_channels -= 1
+            self.taked += 1
+            que_ts.wait_time += self.ttek - que_ts.start_waiting_time
+            self.servers[c].start_service(que_ts, self.ttek)
+            self.free_channels -= 1
 
     def calc_next_event_time(self):
 
         serv_earl = 1e10
 
         for c in range(self.n):
             if self.servers[c].time_to_end_service < serv_earl:
                 serv_earl = self.servers[c].time_to_end_service
 
         if self.arrival_time < serv_earl:
             self.time_to_next_event = self.arrival_time - self.ttek
         else:
             self.time_to_next_event = serv_earl - self.ttek
 
-    def on_end_warming(self):
-
-        self.p[self.in_sys] += self.end_warm_time - self.t_old
-
-        self.ttek = self.end_warm_time
-        self.t_old = self.ttek
-
-        self.is_start_warm = False
-        self.end_warm_time = 1e12
-
-        # Отправляем n заявок из очереди в каналы
-        for i in range(self.n):
-            if len(self.queue) != 0:
-                self.send_head_of_queue_to_channel(i)
-
     def run_one_step(self):
 
         num_of_server_earlier = -1
         serv_earl = 1e10
 
         for c in range(self.n):
             if self.servers[c].time_to_end_service < serv_earl:
                 serv_earl = self.servers[c].time_to_end_service
                 num_of_server_earlier = c
 
-        if self.is_set_warm and not self.is_only_first:
-            # Задан глобальный разогрев. Нужно отслеживать в том числе момент окончания разогрева
-            times = [serv_earl, self.arrival_time, self.end_warm_time]
-            min_time_num = np.argmin(times)
-            if min_time_num == 0:
-                # Обслуживание. Точно не режим разогрева. Есть в каналах заявки
-                self.serving(num_of_server_earlier)
-            elif min_time_num == 1:
-                # Прибытие. Может быть в режиме разогрева. логика - внутри
-                self.arrival()
-            else:
-                self.on_end_warming()
+        # Key moment:
 
+        if self.arrival_time < serv_earl:
+            self.arrival()
         else:
-            # Разогрев задан первой заявки или не задан вообще. Все штатно
-
-            if self.arrival_time < serv_earl:
-                self.arrival()
-            else:
-                self.serving(num_of_server_earlier)
+            self.serving(num_of_server_earlier)
 
-            if self.is_next_calc:
-                self.calc_next_event_time()
+        if self.is_next_calc:
+            self.calc_next_event_time()
 
-    def run(self, total_served, is_real_served=False):
+    def run(self, total_served):
         start = time.process_time()
         if self.cuda:
-            from numba.cuda.random import create_xoroshiro128p_states
+            from numba.cuda.random import create_xoroshiro128p_states, xoroshiro128p_uniform_float32
             import numpy as np
+            from numba import cuda
             threads_per_block = 512
             blocks = int(total_served / 512)
             rng_states = create_xoroshiro128p_states(threads_per_block * blocks, seed=1)
 
             # source:
             source_out = np.zeros(threads_per_block * blocks, dtype=np.float32)
             if self.source_types == "M":
                 rd.generate_m_jit[blocks, threads_per_block](rng_states, self.source_params, source_out)
             elif self.source_types == "E":
-                rd.generate_e_jit[blocks, threads_per_block](rng_states, self.source_params[0], self.source_params[1],
-                                                             source_out)
+                rd.generate_e_jit[blocks, threads_per_block](rng_states, self.source_params[0],  self.source_params[1], source_out)
             elif self.source_types == "H":
-                rd.generate_h2_jit[blocks, threads_per_block](rng_states, self.source_params[0], self.source_params[1],
-                                                              self.source_params[2], source_out)
+                rd.generate_h2_jit[blocks, threads_per_block](rng_states, self.source_params[0],  self.source_params[1], self.source_params[2], source_out)
             else:
                 for j in range(len(source_out)):
                     source_out[j] = self.source.generate()
 
             self.source_random_vars = source_out
             self.tek_source_num = 0
 
-        if is_real_served:
-            served_old = 0
-            while self.served < total_served:
-                self.run_one_step()
-                if (self.served - served_old) % 5000 == 0:
-                    sys.stderr.write('\rStart simulation. Job served: %d/%d' % (self.served, total_served))
-                    sys.stderr.flush()
-                served_old = self.served
-        else:
-            print(Fore.GREEN + '\rStart simulation')
-            print(Style.RESET_ALL)
-
-            for i in tqdm(range(total_served)):
-                self.run_one_step()
-
-            print(Fore.GREEN + '\rSimulation is finished')
-            print(Style.RESET_ALL)
+        # while (self.served < total_served):
+        #     self.run_one_step()
+        #     sys.stderr.write('\rStart simulation. Job served: %d/%d' % (self.served, total_served))
+        #     sys.stderr.flush()
+        print('\rStart simulation...')
+        for i in tqdm(range(total_served)):
+            self.run_one_step()
 
         self.time_spent = time.process_time() - start
 
     def refresh_ppnz_stat(self, new_a):
         for i in range(3):
             self.ppnz[i] = self.ppnz[i] * (1.0 - (1.0 / self.ppnz_moments)) + math.pow(new_a, i + 1) / self.ppnz_moments
 
@@ -646,16 +528,15 @@
         elif types == "Uniform":
             self.dist = rd.Uniform_dist(params)
         elif types == "Norm":
             self.dist = rd.Normal_dist(params)
         elif types == "D":
             self.dist = rd.Det_dist(params)
         else:
-            raise SetSmoException(
-                "Неправильно задан тип распределения сервера. Варианты М, Н, Е, С, Pa, Norm, Uniform, D")
+            raise SetSmoException("Неправильно задан тип распределения сервера. Варианты М, Н, Е, С, Pa, Norm, Uniform, D")
         self.time_to_end_service = 1e10
         self.is_free = True
         self.tsk_on_service = None
         Server.id += 1
         self.id = Server.id
 
         self.params_warm = None
@@ -712,22 +593,21 @@
             res += "\t" + str(self.tsk_on_service)
         return res
 
 
 if __name__ == '__main__':
     from most_queue.theory import mmnr_calc
     from most_queue.theory import m_d_n_calc
-    from most_queue.utils.tables import times_print, probs_print
 
     n = 3
     l = 1.0
     r = 100
     ro = 0.8
     num_of_jobs = 300000
-    is_cuda = False
+    is_cuda = True
 
     mu = l / (ro * n)
 
     smo = SmoIm(n, buffer=r, cuda=is_cuda)
 
     smo.set_sources(l, 'M')
     smo.set_servers(mu, 'M')
@@ -735,29 +615,36 @@
     smo.run(num_of_jobs)
 
     w = mmnr_calc.M_M_n_formula.get_w(l, mu, n, r)
 
     w_im = smo.w
 
     print("Time spent ", smo.time_spent)
+    print("\nЗначения начальных моментов времени ожидания заявок в системе:\n")
 
-    times_print(w_im, w)
-
+    print("{0:^15s}|{1:^15s}|{2:^15s}".format("№ момента", "Числ", "ИМ"))
+    print("-" * 45)
+    for j in range(3):
+        print("{0:^16d}|{1:^15.5g}|{2:^15.5g}".format(j + 1, w[j], w_im[j]))
     print("\n\nДанные ИМ::\n")
     print(smo)
 
-    print(f"M/D/{n}")
-
     smo = SmoIm(n)
 
     smo.set_sources(l, 'M')
     smo.set_servers(1.0 / mu, 'D')
 
-    smo.run(num_of_jobs, is_real_served=False)
+    smo.run(num_of_jobs)
 
     mdn = m_d_n_calc.M_D_n(l, 1 / mu, n)
     p_ch = mdn.calc_p()
     p_im = smo.get_p()
 
     print("Time spent ", smo.time_spent)
-
-    probs_print(p_im, p_ch, 10)
+    print("-" * 36)
+    print("{0:^36s}".format("Вероятности состояний СМО M/D/{0:d}".format(n)))
+    print("-" * 36)
+    print("{0:^4s}|{1:^15s}|{2:^15s}".format("№", "Числ", "ИМ"))
+    print("-" * 36)
+    for i in range(11):
+        print("{0:^4d}|{1:^15.5g}|{2:^15.5g}".format(i, p_ch[i], p_im[i]))
+    print("-" * 36)
```

### Comparing `most_queue-1.20/most_queue/sim/smo_im_prty.py` & `most_queue-1.3/most_queue/sim/smo_im_prty.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,12 @@
-from most_queue.sim import rand_destribution as rd
-
 import time
-import sys
 from tqdm import tqdm
-
-from colorama import init
-from colorama import Fore, Style
-
+import most_queue.sim.rand_destribution as rd
 import math
-
-init()
+import sys
 
 
 class SmoImPrty:
     """
     Имитационная модель СМО GI/G/n/r и GI/G/n с приоритетами
     """
 
@@ -130,16 +123,15 @@
             elif source_type == "Pa":
                 self.sources.append(rd.Pareto_dist(params))
             elif source_type == "Uniform":
                 self.sources.append(rd.Uniform_dist(params))
             elif self.source_types == "D":
                 self.sources.append(rd.Det_dist(params))
             else:
-                raise SetSmoException(
-                    "Неправильно задан тип распределения источника. Варианты М, Н, Е, С, Pa, Uniform, D")
+                raise SetSmoException("Неправильно задан тип распределения источника. Варианты М, Н, Е, С, Pa, Uniform, D")
             self.arrival_time[i] = self.sources[i].generate()
             time.sleep(0.1)
 
     def set_servers(self, servers_params):
         """
         Задает тип и параметры распределения времени обслуживания.
         servers - список параметров серверов. Каждый элемент списка
@@ -197,16 +189,15 @@
             elif warm_up_type == "Pa":
                 self.warm_up.append(rd.Pareto_dist(params))
             elif warm_up_type == "Uniform":
                 self.warm_up.append(rd.Uniform_dist(params))
             elif warm_up_type == "D":
                 self.warm_up.append(rd.Det_dist(params))
             else:
-                raise SetSmoException(
-                    "Неправильно задан тип распределения разогрева. Варианты М, Н, Е, С, Pa, Uniform, D")
+                raise SetSmoException("Неправильно задан тип распределения разогрева. Варианты М, Н, Е, С, Pa, Uniform, D")
 
     def calc_load(self):
 
         """
         Вычисляет коэффициент загрузки СМО
         """
         l_sum = 0
@@ -250,15 +241,15 @@
                     a = self.sources_params[i]['params'][0]
                     k = self.sources_params[i]['params'][1]
                     f1 = a * k / (a - 1)
                     l_sum += 1.0 / f1
             elif self.sources_params[i]['type'] == "Uniform":
                 f1 = self.sources_params[i]['type'][0]
                 l_sum += 1.0 / f1
-
+            
             elif self.sources_params[i]['type'] == "D":
                 f1 = self.sources_params[i]['type']
                 l_sum += 1.0 / f1
 
             if self.servers_params[i]['type'] == "M":
                 mu = self.servers_params[i]['params']
                 b1_sr += 1.0 / mu
@@ -280,19 +271,19 @@
                 r = self.servers_params[i]['params'][0]
                 mu = self.servers_params[i]['params'][1]
                 b1_sr += r / mu
 
             elif self.servers_params[i]['type'] == "Uniform":
                 f1 = self.servers_params[i]['params'][0]
                 b1_sr += 1.0 / f1
-
+            
             elif self.servers_params[i]['type'] == "D":
                 f1 = self.servers_params[i]['type']
                 b1_sr += 1.0 / f1
-
+                
             elif self.servers_params[i]['type'] == "C":
                 y1 = self.servers_params[i]['params'][0]
                 y2 = 1.0 - y1
                 mu1 = self.servers_params[i]['params'][1]
                 mu2 = self.servers_params[i]['params'][2]
 
                 b1_sr += y2 / mu1 + y1 * (1.0 / mu1 + 1.0 / mu2)
@@ -302,14 +293,15 @@
                 else:
                     a = self.servers_params[i]['params'][0]
                     k = self.servers_params[i]['params'][1]
                     b1_sr += a * k / (a - 1)
 
         return l_sum * b1_sr / (self.n * self.k)
 
+
     def arrival(self, k, moment=None, ts=None):
 
         """
         Действия по прибытию заявки в СМО.
         k - номер класса прибывшей заявки
         если переданы 2 и 3 параметр - значит СМО входит в состав СеМО
         и k - номер класса внутри СМО. Истинный номер класса - в ts.k
@@ -563,31 +555,20 @@
 
         else:
             self.serving(num_of_server_earlier)
 
         if self.is_next_calc:
             self.calc_time_to_next_event()
 
-    def run(self, total_served, is_real_served=False):
-        if is_real_served:
 
-            while sum(self.served) < total_served:
-                self.run_one_step()
-                sys.stderr.write('\rStart simulation. Job served: %d/%d' % (sum(self.served), total_served))
-                sys.stderr.flush()
-
-        else:
-            print(Fore.GREEN + '\rStart simulation')
-            print(Style.RESET_ALL)
-
-            for i in tqdm(range(total_served)):
-                self.run_one_step()
-
-            print(Fore.GREEN + '\rSimulation is finished')
-            print(Style.RESET_ALL)
+    def run(self, total_served):
+        while (sum(self.served) < total_served):
+            self.run_one_step()
+            sys.stderr.write('\rStart simulation. Job served: %d/%d' % (sum(self.served), total_served))
+            sys.stderr.flush()
 
     def refresh_ppnz_stat(self, k, new_a):
         for i in range(3):
             self.ppnz[k][i] = self.ppnz[k][i] * (1.0 - (1.0 / self.ppnz_moments[k])) + \
                               math.pow(new_a, i + 1) / self.ppnz_moments[k]
 
     def refresh_v_stat(self, k, new_a):
@@ -752,16 +733,15 @@
             elif dist_type == "C":
                 self.dist.append(rd.Cox_dist(params))
             elif dist_type == "Pa":
                 self.dist.append(rd.Pareto_dist(params))
             elif dist_type == "Uniform":
                 self.dist.append(rd.Uniform_dist(params))
             else:
-                raise SetSmoException(
-                    "Неправильно задан тип распределения сервера. Варианты М, Н, Е, С, Gamma, Pa, Uniform")
+                raise SetSmoException("Неправильно задан тип распределения сервера. Варианты М, Н, Е, С, Gamma, Pa, Uniform")
         self.time_to_end_service = 1e10
         self.total_time_to_serve = 0
         # Сохранение типа дисциплины обслуживания необходимо для
         # корректного назначения времени обслуживания после прерывания
         self.prty_type = prty_type
         self.is_free = True
         self.class_on_service = None
@@ -809,16 +789,15 @@
             res += "\t\t" + str(self.tsk_on_service.__str__("\t"))
         return res
 
 
 if __name__ == "__main__":
     from most_queue.theory import prty_calc
     import math
-    import rand_destribution as rd
-    from most_queue.utils.tables import times_print_with_classes
+    from most_queue.sim import rand_destribution as rd
 
     n = 5
     k = 3
     l = [0.2, 0.3, 0.4]
     lsum = sum(l)
     num_of_jobs = 100000
     b1 = [0.45 * n, 0.9 * n, 1.35 * n]
@@ -851,20 +830,71 @@
         servers_params.append({'type': 'Gamma', 'params': params[j]})
 
     smo.set_sources(sources)
     smo.set_servers(servers_params)
 
     smo.run(num_of_jobs)
 
+    # v_im = smo.v
+    # calc1pr = prty_calc.calc_pr1(l, b)
+    # v_ch = calc1pr['v']
+    #
+    # #w_ch = prty_calc.climov_w_pr_calc(l, b)
+    # # w_ch_1 = prty_calc.get_w1_pr(l, b)
+    # # for j in range(3):
+    # #     print("{:^15.3g}|".format(w_ch_1[j]), end="")
+    # # print("\n")
+    #
+    # for i in range(k):
+    #     print(" " * 5 + "|", end="")
+    #     print("{:^5s}|".format("ИМ"), end="")
+    #     for j in range(3):
+    #         print("{:^15.3g}|".format(v_im[i][j]), end="")
+    #     print("")
+    #     print("{:^5s}".format(str(i + 1)) + "|" + "-" * 54)
+    #
+    #     print(" " * 5 + "|", end="")
+    #     print("{:^5s}|".format("Р"), end="")
+    #     for j in range(3):
+    #         print("{:^15.3g}|".format(v_ch[i][j]), end="")
+    #     print("")
+    #     print("-" * 60)
+
     v_im = smo.v
 
     v_teor = prty_calc.get_v_prty_invar(l, b, n, 'PR')
 
-    times_print_with_classes(v_im, v_teor, is_w=False)
+    print("-" * 60)
+    print("{0:^11s}|{1:^47s}|".format('', 'Номер начального момента'))
+    print("{0:^10s}| ".format('№ кл'), end="")
+    print("-" * 45 + " |")
+
+    print(" " * 11 + "|", end="")
+    for j in range(3):
+        s = str(j + 1)
+        print("{:^15s}|".format(s), end="")
+    print("")
+    print("-" * 60)
 
+    for i in range(k):
+        print(" " * 5 + "|", end="")
+        print("{:^5s}|".format("ИМ"), end="")
+        for j in range(3):
+            print("{:^15.3g}|".format(v_im[i][j]), end="")
+        print("")
+        print("{:^5s}".format(str(i + 1)) + "|" + "-" * 54)
+
+        print(" " * 5 + "|", end="")
+        print("{:^5s}|".format("Р"), end="")
+        for j in range(3):
+            print("{:^15.3g}|".format(v_teor[i][j]), end="")
+        print("")
+        print("-" * 60)
+
+    print("\n")
     print("Относительный приоритет")
 
     smo = SmoImPrty(n, k, "NP")
     sources = []
     servers_params = []
     for j in range(k):
         sources.append({'type': 'M', 'params': l[j]})
@@ -875,8 +905,33 @@
 
     smo.run(num_of_jobs)
 
     v_im = smo.v
 
     v_teor = prty_calc.get_v_prty_invar(l, b, n, 'NP')
 
-    times_print_with_classes(v_im, v_teor, is_w=False)
+    print("-" * 60)
+    print("{0:^11s}|{1:^47s}|".format('', 'Номер начального момента'))
+    print("{0:^10s}| ".format('№ кл'), end="")
+    print("-" * 45 + " |")
+
+    print(" " * 11 + "|", end="")
+    for j in range(3):
+        s = str(j + 1)
+        print("{:^15s}|".format(s), end="")
+    print("")
+    print("-" * 60)
+
+    for i in range(k):
+        print(" " * 5 + "|", end="")
+        print("{:^5s}|".format("ИМ"), end="")
+        for j in range(3):
+            print("{:^15.3g}|".format(v_im[i][j]), end="")
+        print("")
+        print("{:^5s}".format(str(i + 1)) + "|" + "-" * 54)
+
+        print(" " * 5 + "|", end="")
+        print("{:^5s}|".format("Р"), end="")
+        for j in range(3):
+            print("{:^15.3g}|".format(v_teor[i][j]), end="")
+        print("")
+        print("-" * 60)
```

### Comparing `most_queue-1.20/most_queue/sim/smo_impatient_im.py` & `most_queue-1.3/most_queue/sim/smo_impatient_im.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-import rand_destribution as rd
-from smo_im import SmoIm, SetSmoException, Task
+import most_queue.sim.rand_destribution as rd
+import math
+from tqdm import tqdm
+from most_queue.sim.smo_im import SmoIm, SetSmoException, Task
 
 
 class ImpatientTask(Task):
     def __init__(self, arr_time, moment_to_leave):
         super().__init__(arr_time)
         self.moment_to_leave = moment_to_leave
```

### Comparing `most_queue-1.20/most_queue/tests/ek_d_n.py` & `most_queue-1.3/most_queue/tests/ek_d_n.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/tests/fj_calc.py` & `most_queue-1.3/most_queue/tests/fj_calc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-from most_queue.theory import fj_calc
-from most_queue.sim.fj_im import SmoFJ
-import matplotlib.pyplot as plt
+from most_queue.theory.fj_calc import *
 
 
 def test():
     """
     Тестирование аппроксимаций для системы Fork-Join
     В пакете most_queue.theory.fj_calc модержатся следующие методы:
 
@@ -61,20 +59,21 @@
         # в массив только среднее (первый нач момент)
         v = smo.v
         v_im.append(v[0])
 
         # расчет средних времен пребывания с помощью аппроксимаций. \
         # На вход каждого из методов - l, mu, nn (число каналов СМО)
 
-        v_varki.append(fj_calc.get_v1_fj_varki_merchant(l, mu, nn))
-        v_varma.append(fj_calc.get_v1_fj_varma(l, mu, nn))
-        v_nelson.append(fj_calc.get_v1_fj_nelson_tantawi(l, mu, nn))
+        v_varki.append(get_v1_fj_varki_merchant(l, mu, nn))
+        v_varma.append(get_v1_fj_varma(l, mu, nn))
+        v_nelson.append(get_v1_fj_nelson_tantawi(l, mu, nn))
 
         print(str_f_v.format(v_im[i], v_varki[i], v_varma[i], v_nelson[i]))
 
+
     # строим графики и сохраняем в текущую директорию:
 
     fig, ax = plt.subplots()
 
     linestyles = ["solid", "dotted", "dashed", "dashdot"]
 
     ax.plot(n, v_im, label="ИМ", linestyle=linestyles[0])
```

### Comparing `most_queue-1.20/most_queue/tests/fj_im.py` & `most_queue-1.3/most_queue/tests/fj_im.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/tests/flow_sum.py` & `most_queue-1.3/most_queue/tests/flow_sum.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/tests/gi_m_1_calc.py` & `most_queue-1.3/most_queue/tests/gi_m_1_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/tests/gi_m_n_calc.py` & `most_queue-1.3/most_queue/tests/gi_m_n_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/tests/m_d_n_calc.py` & `most_queue-1.3/most_queue/tests/m_d_n_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/tests/m_h2_h2warm.py` & `most_queue-1.3/most_queue/tests/mmn3_pnz_cox_approx.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,81 +1,79 @@
-from most_queue.theory.m_h2_h2warm import Mh2h2Warm
-from most_queue.sim import smo_im
-from most_queue.sim import rand_destribution as rd
-
-import math
-import time
+from most_queue.sim import smo_im_prty
+from most_queue.theory import mmn_prty_pnz_approx
+from most_queue.theory.mmnr_calc import M_M_n_formula
+from most_queue.theory.mmn3_pnz_cox_approx import Mmn3_pnz_cox
 
 
 def test():
-    n = 3  # число каналов
-    l = 1.0  # интенсивность вх потока
-    ro = 0.7  # коэфф загрузки
-    b1 = n * 0.7  # ср время обслуживания
-    b1_warm = n * 0.9  # ср время разогрева
-    num_of_jobs = 1000000  # число обсл заявок ИМ
-    b_coev = [0.8, 1.5]  # коэфф вариации времени обсл
-    b_coev_warm = 1.2  # коэфф вариации времени разогрева
-    buff = None  # очередь - неограниченная
-    verbose = False  # не выводить пояснения при расчетах
-
-    for k in range(len(b_coev)):
-        b = [0.0] * 3
-        alpha = 1 / (b_coev[k] ** 2)
-        b[0] = b1
-        b[1] = math.pow(b[0], 2) * (math.pow(b_coev[k], 2) + 1)
-        b[2] = b[1] * b[0] * (1.0 + 2 / alpha)
-
-        b_w = [0.0] * 3
-        b_w[0] = b1_warm
-        alpha = 1 / (b_coev_warm ** 2)
-        b_w[1] = math.pow(b_w[0], 2) * (math.pow(b_coev_warm, 2) + 1)
-        b_w[2] = b_w[1] * b_w[0] * (1.0 + 2 / alpha)
-
-        im_start = time.process_time()
-        smo = smo_im.SmoIm(n, buffer=buff)
-        smo.set_sources(l, 'M')
-
-        gamma_params = rd.Gamma.get_mu_alpha(b)
-        gamma_params_warm = rd.Gamma.get_mu_alpha(b_w)
-        smo.set_servers(gamma_params, 'Gamma')
-        smo.set_warm(gamma_params_warm, 'Gamma')
-        smo.run(num_of_jobs)
-        p = smo.get_p()
-        v_im = smo.v
-        im_time = time.process_time() - im_start
-
-        tt_start = time.process_time()
-        tt = Mh2h2Warm(l, b, b_w, n, buffer=buff, verbose=verbose)
-
-        tt.run()
-        p_tt = tt.get_p()
-        v_tt = tt.get_v()
-        tt_time = time.process_time() - tt_start
-
-        num_of_iter = tt.num_of_iter_
-
-        print("\nСравнение результатов расчета методом Такахаси-Таками и ИМ.\n"
-              "ИМ - M/Gamma/{0:^2d}\nТакахаси-Таками - M/H2/{0:^2d}"
-              "с комплексными параметрами\n"
-              "Коэффициент загрузки: {1:^1.2f}".format(n, ro))
-        print(f'Коэффициент вариации времени обслуживания {b_coev[k]:0.3f}')
-        print(f'Коэффициент вариации времени разогрева {b_coev_warm:0.3f}')
-        print("Количество итераций алгоритма Такахаси-Таками: {0:^4d}".format(num_of_iter))
-        print("Время работы алгоритма Такахаси-Таками: {0:^5.3f} c".format(tt_time))
-        print("Время ИМ: {0:^5.3f} c".format(im_time))
-        print("{0:^25s}".format("Первые 10 вероятностей состояний СМО"))
-        print("{0:^3s}|{1:^15s}|{2:^15s}".format("№", "Числ", "ИМ"))
-        print("-" * 32)
-        for i in range(11):
-            print("{0:^4d}|{1:^15.3g}|{2:^15.3g}".format(i, p_tt[i], p[i]))
-
-        print("\n")
-        print("{0:^25s}".format("Начальные моменты времени ожидания в СМО"))
-        print("{0:^3s}|{1:^15s}|{2:^15s}".format("№", "Числ", "ИМ"))
-        print("-" * 32)
-        for i in range(3):
-            print("{0:^4d}|{1:^15.3g}|{2:^15.3g}".format(i + 1, v_tt[i], v_im[i]))
+    num_of_jobs = 200000
+    n = 2  # количество каналов
+    K = 3  # количество классов
+    mu_L = 1.3  # интенсивность обслуживания заявок 3-го класса
+    mu_M = 1.4  # интенсивность обслуживания заявок 2-го класса
+    mu_H = 1.5  # интенсивность обслуживания заявок 1-го класса
+    l_L = 0.7  # интенсивность вх потока заявок 3-го класса
+    l_M = 0.8  # интенсивность вх потока заявок 2-го класса
+    l_H = 0.9  # интенсивность вх потока заявок 1-го класса
+
+    l_sum = l_H + l_M + l_L
+    b1_H = 1 / mu_H
+    b1_L = 1 / mu_L
+    b1_M = 1 / mu_M
+    b_ave = (l_L / l_sum) * b1_L + (l_H / l_sum) * b1_H + (l_M / l_sum) * b1_M
+    ro = l_sum * b_ave / n
+
+    # задание ИМ:
+    smo = smo_im_prty.SmoImPrty(n, K, "PR")
+    sources = []
+    servers_params = []
+    l = [l_H, l_M, l_L]
+    mu = [mu_H, mu_M, mu_L]
+    for j in range(K):
+        sources.append({'type': 'M', 'params': l[j]})
+        servers_params.append({'type': 'M', 'params': mu[j]})
+
+    smo.set_sources(sources)
+    smo.set_servers(servers_params)
+
+    # запуск ИМ:
+    smo.run(num_of_jobs)
+
+    # получение результатов ИМ:
+    p = smo.get_p()
+    v_im = smo.v
+
+    # расчет численным методом:
+    tt = Mmn3_pnz_cox(mu_L, mu_M, mu_H, l_L, l_M, l_H)
+    tt_for_second = mmn_prty_pnz_approx.MMn_PRTY_PNZ_Cox_approx(2, mu_M, mu_H, l_M, l_H)
+    tt_for_second.run()
+
+    tt.run()
+    p_tt = tt.get_p()
+    v_tt = tt.get_low_class_v1()
+    v_2 = tt_for_second.get_second_class_v1()
+
+    v_1 = M_M_n_formula.get_v(l_H, mu_H, 2, 100)[0]
+
+    print("\nСравнение результатов расчета численным методом с аппроксимацией ПНЗ "
+          "\nраспределением Кокса второго порядка и ИМ.")
+    print("Коэффициент загрузки: {0:^1.2f}".format(ro))
+    print("Количество обслуженных заявок для ИМ: {0:d}\n".format(num_of_jobs))
+
+    print("{0:^25s}".format("Вероятности состояний для заявок 3-го класса"))
+    print("{0:^3s}|{1:^15s}|{2:^15s}".format("№", "Числ", "ИМ"))
+    print("-" * 32)
+    for i in range(11):
+        print("{0:^4d}|{1:^15.3g}|{2:^15.3g}".format(i, p_tt[i], p[2][i]))
+
+    print("\n")
+    print("{0:^35s}".format("Средние времена пребывания в СМО"))
+    print("-" * 38)
+    print("{0:^10s}|{1:^15s}|{2:^15s}".format("N класса", "Числ", "ИМ"))
+    print("-" * 38)
+    print("{0:^10d}|{1:^15.3g}|{2:^15.3g}".format(0, v_1, v_im[0][0]))
+    print("{0:^10d}|{1:^15.3g}|{2:^15.3g}".format(1, v_2, v_im[1][0]))
+    print("{0:^10d}|{1:^15.3g}|{2:^15.3g}".format(2, v_tt, v_im[2][0]))
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     test()
```

### Comparing `most_queue-1.20/most_queue/tests/m_ph_n_prty.py` & `most_queue-1.3/most_queue/tests/m_ph_n_prty.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/tests/mg1_calc.py` & `most_queue-1.3/most_queue/tests/mg1_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/tests/mg1_warm_calc.py` & `most_queue-1.3/most_queue/tests/mg1_warm_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/tests/mgn_tt.py` & `most_queue-1.3/most_queue/tests/mgn_tt.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/tests/mmn3_pnz_cox_approx.py` & `most_queue-1.3/most_queue/tests/mmn_prty_pnz_approx.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,31 @@
+from most_queue.theory.mmn_prty_pnz_approx import MMn_PRTY_PNZ_Cox_approx
 from most_queue.sim import smo_im_prty
-from most_queue.theory import mmn_prty_pnz_approx
-from most_queue.theory.mmnr_calc import M_M_n_formula
-from most_queue.theory.mmn3_pnz_cox_approx import Mmn3_pnz_cox
 
 
 def test():
-    num_of_jobs = 200000
-    n = 2  # количество каналов
-    K = 3  # количество классов
-    mu_L = 1.3  # интенсивность обслуживания заявок 3-го класса
-    mu_M = 1.4  # интенсивность обслуживания заявок 2-го класса
+    num_of_jobs = 100000
+    n = 3  # количество каналов
+    K = 2  # количество классов
+    mu_L = 1.3  # интенсивность обслуживания заявок 2-го класса
     mu_H = 1.5  # интенсивность обслуживания заявок 1-го класса
-    l_L = 0.7  # интенсивность вх потока заявок 3-го класса
-    l_M = 0.8  # интенсивность вх потока заявок 2-го класса
-    l_H = 0.9  # интенсивность вх потока заявок 1-го класса
-
-    l_sum = l_H + l_M + l_L
+    l_H = 1.0  # интенсивность вх потока заявок 1-го класса
+    l_L = 1.4  # интенсивность вх потока заявок 2-го класса
+    ro = 0.8
     b1_H = 1 / mu_H
-    b1_L = 1 / mu_L
-    b1_M = 1 / mu_M
-    b_ave = (l_L / l_sum) * b1_L + (l_H / l_sum) * b1_H + (l_M / l_sum) * b1_M
-    ro = l_sum * b_ave / n
+    b1_L = (ro * n - l_H * b1_H) / l_L
+    l_sum = l_H + l_L
+    # b_ave = (l_L / l_sum) * b1_L + (l_H / l_sum) * b1_H
 
     # задание ИМ:
     smo = smo_im_prty.SmoImPrty(n, K, "PR")
     sources = []
     servers_params = []
-    l = [l_H, l_M, l_L]
-    mu = [mu_H, mu_M, mu_L]
+    l = [l_H, l_L]
+    mu = [mu_H, mu_L]
     for j in range(K):
         sources.append({'type': 'M', 'params': l[j]})
         servers_params.append({'type': 'M', 'params': mu[j]})
 
     smo.set_sources(sources)
     smo.set_servers(servers_params)
 
@@ -39,41 +33,36 @@
     smo.run(num_of_jobs)
 
     # получение результатов ИМ:
     p = smo.get_p()
     v_im = smo.v
 
     # расчет численным методом:
-    tt = Mmn3_pnz_cox(mu_L, mu_M, mu_H, l_L, l_M, l_H)
-    tt_for_second = mmn_prty_pnz_approx.MMn_PRTY_PNZ_Cox_approx(2, mu_M, mu_H, l_M, l_H)
-    tt_for_second.run()
-
+    tt = MMn_PRTY_PNZ_Cox_approx(n, mu_L, mu_H, l_L, l_H)
     tt.run()
     p_tt = tt.get_p()
-    v_tt = tt.get_low_class_v1()
-    v_2 = tt_for_second.get_second_class_v1()
-
-    v_1 = M_M_n_formula.get_v(l_H, mu_H, 2, 100)[0]
+    v_tt = tt.get_second_class_v1()
+    # v = tt.calculate_v()
 
     print("\nСравнение результатов расчета численным методом с аппроксимацией ПНЗ "
           "\nраспределением Кокса второго порядка и ИМ.")
     print("Коэффициент загрузки: {0:^1.2f}".format(ro))
     print("Количество обслуженных заявок для ИМ: {0:d}\n".format(num_of_jobs))
 
-    print("{0:^25s}".format("Вероятности состояний для заявок 3-го класса"))
+    print("{0:^25s}".format("Вероятности состояний для заявок 2-го класса"))
     print("{0:^3s}|{1:^15s}|{2:^15s}".format("№", "Числ", "ИМ"))
     print("-" * 32)
     for i in range(11):
-        print("{0:^4d}|{1:^15.3g}|{2:^15.3g}".format(i, p_tt[i], p[2][i]))
+        print("{0:^4d}|{1:^15.3g}|{2:^15.3g}".format(i, p_tt[i], p[1][i]))
 
     print("\n")
-    print("{0:^35s}".format("Средние времена пребывания в СМО"))
-    print("-" * 38)
-    print("{0:^10s}|{1:^15s}|{2:^15s}".format("N класса", "Числ", "ИМ"))
-    print("-" * 38)
-    print("{0:^10d}|{1:^15.3g}|{2:^15.3g}".format(0, v_1, v_im[0][0]))
-    print("{0:^10d}|{1:^15.3g}|{2:^15.3g}".format(1, v_2, v_im[1][0]))
-    print("{0:^10d}|{1:^15.3g}|{2:^15.3g}".format(2, v_tt, v_im[2][0]))
+    print("{0:^25s}".format("Среднее время пребывания в СМО заявок 2-го класса"))
+    print("{0:^15s}|{1:^15s}".format("Числ", "ИМ"))
+    print("-" * 32)
+    print("{0:^15.3g}|{1:^15.3g}".format(v_tt, v_im[1][0]))
+    # print("{0:^15.3g}|{1:^15.3g}".format(v[0].real, v_im[1][0]))
+    # print("{0:^15.3g}|{1:^15.3g}".format(v[1].real, v_im[1][1]))
+    # print("{0:^15.3g}|{1:^15.3g}".format(v[2].real, v_im[1][2]))
 
 
 if __name__ == "__main__":
     test()
```

### Comparing `most_queue-1.20/most_queue/tests/mmn_prty_pnz_approx.py` & `most_queue-1.3/most_queue/tests/smo_im.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,68 +1,69 @@
-from most_queue.theory.mmn_prty_pnz_approx import MMn_PRTY_PNZ_Cox_approx
-from most_queue.sim import smo_im_prty
+from most_queue.sim.smo_im import SmoIm
+from most_queue.theory import mmnr_calc
+from most_queue.theory import m_d_n_calc
 
 
 def test():
-    num_of_jobs = 100000
-    n = 3  # количество каналов
-    K = 2  # количество классов
-    mu_L = 1.3  # интенсивность обслуживания заявок 2-го класса
-    mu_H = 1.5  # интенсивность обслуживания заявок 1-го класса
-    l_H = 1.0  # интенсивность вх потока заявок 1-го класса
-    l_L = 1.4  # интенсивность вх потока заявок 2-го класса
-    ro = 0.8
-    b1_H = 1 / mu_H
-    b1_L = (ro * n - l_H * b1_H) / l_L
-    l_sum = l_H + l_L
-    # b_ave = (l_L / l_sum) * b1_L + (l_H / l_sum) * b1_H
-
-    # задание ИМ:
-    smo = smo_im_prty.SmoImPrty(n, K, "PR")
-    sources = []
-    servers_params = []
-    l = [l_H, l_L]
-    mu = [mu_H, mu_L]
-    for j in range(K):
-        sources.append({'type': 'M', 'params': l[j]})
-        servers_params.append({'type': 'M', 'params': mu[j]})
-
-    smo.set_sources(sources)
-    smo.set_servers(servers_params)
-
-    # запуск ИМ:
-    smo.run(num_of_jobs)
-
-    # получение результатов ИМ:
-    p = smo.get_p()
-    v_im = smo.v
-
-    # расчет численным методом:
-    tt = MMn_PRTY_PNZ_Cox_approx(n, mu_L, mu_H, l_L, l_H)
-    tt.run()
-    p_tt = tt.get_p()
-    v_tt = tt.get_second_class_v1()
-    # v = tt.calculate_v()
-
-    print("\nСравнение результатов расчета численным методом с аппроксимацией ПНЗ "
-          "\nраспределением Кокса второго порядка и ИМ.")
-    print("Коэффициент загрузки: {0:^1.2f}".format(ro))
-    print("Количество обслуженных заявок для ИМ: {0:d}\n".format(num_of_jobs))
-
-    print("{0:^25s}".format("Вероятности состояний для заявок 2-го класса"))
-    print("{0:^3s}|{1:^15s}|{2:^15s}".format("№", "Числ", "ИМ"))
-    print("-" * 32)
+    """
+    Тестирование имитационной модели СМО
+    Для верификации - сравнение с результатами расчета СМО M/M/3, M/D/3
+    """
+    n = 3  # число каналов
+    l = 1.0  # интенсивность вх потока
+    r = 30  # длина очереди
+    ro = 0.8  # коэфф загрузки
+    mu = l / (ro * n)  # интенсивность обслуживания
+
+    # создвем экземпляр класса ИМ
+    smo = SmoIm(n, buffer=r)
+
+    # задаем вх поток - параметры и тип распределения.
+    smo.set_sources(l, 'M')
+    # задаем распределение обслуживания - параметры и тип распределения.
+    smo.set_servers(mu, 'M')
+
+    # запуск ИМ - передаем кол-во заявок для обслуживания
+    smo.run(1000000)
+    # получаем начальные моменты времени ожидания. Также можно получить время пребывания .v,
+    # вероятности состояний .get_p(), периоды непрерывной занятости .pppz
+    w_im = smo.w
+
+    # для сравнения расчитаем теже начальные моменты численно
+    w = mmnr_calc.M_M_n_formula.get_w(l, mu, n, r)
+
+    # вывод результатов
+
+    print("\nЗначения начальных моментов времени ожидания заявок в системе:\n")
+
+    print("{0:^15s}|{1:^15s}|{2:^15s}".format("№ момента", "Числ", "ИМ"))
+    print("-" * 45)
+    for j in range(3):
+        print("{0:^16d}|{1:^15.5g}|{2:^15.5g}".format(j + 1, w[j], w_im[j]))
+    print("\n\nДанные ИМ::\n")
+    print(smo)
+
+    # тоже для детерминированного обслуживания
+
+    smo = SmoIm(n)
+
+    smo.set_sources(l, 'M')
+    smo.set_servers(1.0 / mu, 'D')
+
+    smo.run(1000000)
+
+    mdn = m_d_n_calc.M_D_n(l, 1 / mu, n)
+    p_ch = mdn.calc_p()
+    p_im = smo.get_p()
+
+    print("-" * 36)
+    print("{0:^36s}".format("Вероятности состояний СМО M/D/{0:d}".format(n)))
+    print("-" * 36)
+    print("{0:^4s}|{1:^15s}|{2:^15s}".format("№", "Числ", "ИМ"))
+    print("-" * 36)
     for i in range(11):
-        print("{0:^4d}|{1:^15.3g}|{2:^15.3g}".format(i, p_tt[i], p[1][i]))
-
-    print("\n")
-    print("{0:^25s}".format("Среднее время пребывания в СМО заявок 2-го класса"))
-    print("{0:^15s}|{1:^15s}".format("Числ", "ИМ"))
-    print("-" * 32)
-    print("{0:^15.3g}|{1:^15.3g}".format(v_tt, v_im[1][0]))
-    # print("{0:^15.3g}|{1:^15.3g}".format(v[0].real, v_im[1][0]))
-    # print("{0:^15.3g}|{1:^15.3g}".format(v[1].real, v_im[1][1]))
-    # print("{0:^15.3g}|{1:^15.3g}".format(v[2].real, v_im[1][2]))
+        print("{0:^4d}|{1:^15.5g}|{2:^15.5g}".format(i, p_ch[i], p_im[i]))
+    print("-" * 36)
 
 
 if __name__ == "__main__":
     test()
```

### Comparing `most_queue-1.20/most_queue/tests/network_im_prty.py` & `most_queue-1.3/most_queue/tests/network_im_prty.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/tests/passage_time.py` & `most_queue-1.3/most_queue/tests/passage_time.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/tests/smo_im.py` & `most_queue-1.3/most_queue/theory/q_poisson_arrival_calc.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,69 +1,60 @@
-from most_queue.sim.smo_im import SmoIm
-from most_queue.theory import mmnr_calc
-from most_queue.theory import m_d_n_calc
+import math
+from most_queue.sim import rand_destribution as rd
+import scipy.spatial as sc
 
 
-def test():
+def get_q_Gamma(l, mu, alpha, num=100):
     """
-    Тестирование имитационной модели СМО
-    Для верификации - сравнение с результатами расчета СМО M/M/3, M/D/3
+    Гамма-распределение
+    l - интенсивность входного потока
+    mu и alpha параметры Гамма-распределения
+    num - число возвращаемых q[j]
     """
-    n = 3  # число каналов
-    l = 1.0  # интенсивность вх потока
-    r = 30  # длина очереди
-    ro = 0.8  # коэфф загрузки
-    mu = l / (ro * n)  # интенсивность обслуживания
+    q = [0.0] * num
+    q[0] = math.pow(mu / (mu + l), alpha)
+    for j in range(1, num):
+        q[j] = q[j - 1] * l * (alpha + j - 1) / ((l + mu) * j)
 
-    # создвем экземпляр класса ИМ
-    smo = SmoIm(n, buffer=r)
+    return q
 
-    # задаем вх поток - параметры и тип распределения.
-    smo.set_sources(l, 'M')
-    # задаем распределение обслуживания - параметры и тип распределения.
-    smo.set_servers(mu, 'M')
 
-    # запуск ИМ - передаем кол-во заявок для обслуживания
-    smo.run(1000000)
-    # получаем начальные моменты времени ожидания. Также можно получить время пребывания .v,
-    # вероятности состояний .get_p(), периоды непрерывной занятости .pppz
-    w_im = smo.w
-
-    # для сравнения расчитаем теже начальные моменты численно
-    w = mmnr_calc.M_M_n_formula.get_w(l, mu, n, r)
-
-    # вывод результатов
-
-    print("\nЗначения начальных моментов времени ожидания заявок в системе:\n")
-
-    print("{0:^15s}|{1:^15s}|{2:^15s}".format("№ момента", "Числ", "ИМ"))
-    print("-" * 45)
-    for j in range(3):
-        print("{0:^16d}|{1:^15.5g}|{2:^15.5g}".format(j + 1, w[j], w_im[j]))
-    print("\n\nДанные ИМ::\n")
-    print(smo)
-
-    # тоже для детерминированного обслуживания
-
-    smo = SmoIm(n)
-
-    smo.set_sources(l, 'M')
-    smo.set_servers(1.0 / mu, 'D')
-
-    smo.run(1000000)
+def get_q_uniform(l, mean, half_interval, num=100):
+    """
+    Равномерное распределение на отрезке [mean-half_interval, mean+half_interval
+    l - интенсивность входного потока
+    mean - среднее
+    half_interval - полуинтервал влево и вправо от среднего значения
+    num - число возвращаемых q[j]
+    """
+    q = [0.0] * num
+    for j in range(num):
+        summ1 = 0
+        for i in range(j + 1):
+            summ1 += l * pow(mean - half_interval, i) * math.exp(-l * (mean - half_interval)) / math.factorial(i)
+        summ2 = 0
+        for i in range(j + 1):
+            summ2 += l * pow(mean + half_interval, i) * math.exp(-l * (mean + half_interval)) / math.factorial(i)
+        q[j] = (1.0 / (2 * l * half_interval)) * (summ1 - summ2)
 
-    mdn = m_d_n_calc.M_D_n(l, 1 / mu, n)
-    p_ch = mdn.calc_p()
-    p_im = smo.get_p()
+    return q
 
-    print("-" * 36)
-    print("{0:^36s}".format("Вероятности состояний СМО M/D/{0:d}".format(n)))
-    print("-" * 36)
-    print("{0:^4s}|{1:^15s}|{2:^15s}".format("№", "Числ", "ИМ"))
-    print("-" * 36)
-    for i in range(11):
-        print("{0:^4d}|{1:^15.5g}|{2:^15.5g}".format(i, p_ch[i], p_im[i]))
-    print("-" * 36)
 
+def get_q_Pareto(l, alpha, K, num=100):
+    """
+    Распределение Парето
+    l - интенсивность входного потока
+    K, alpha - параметры распределения Парето
+    num - число возвращаемых q[j]
+    """
+    q = [0.0] * num
+    gammas = [0.0] * num
+    z = l * K
+    gammas[0] = rd.Gamma.get_minus_gamma(alpha) - rd.Gamma.get_gamma_small(-alpha, z)
+
+    for j in range(1, num):
+        gammas[j] = (j - alpha - 1) * gammas[j - 1] + pow(z, j - alpha - 1) * math.exp(-z)
+    forw = alpha * pow(z, alpha)
+    for j in range(num):
+        q[j] = forw * gammas[j] / math.factorial(j)
 
-if __name__ == "__main__":
-    test()
+    return q
```

### Comparing `most_queue-1.20/most_queue/tests/smo_im_prty.py` & `most_queue-1.3/most_queue/tests/smo_im_prty.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/tests/weibull.py` & `most_queue-1.3/most_queue/tests/weibull.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/theory/batch_mm1.py` & `most_queue-1.3/most_queue/theory/batch_mm1.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/theory/diff5dots.py` & `most_queue-1.3/most_queue/theory/diff5dots.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/theory/ek_d_n_calc.py` & `most_queue-1.3/most_queue/theory/ek_d_n_calc.py`

 * *Files 4% similar despite different names*

```diff
@@ -146,15 +146,14 @@
             z[m] = z_old
         self.z_ = z
 
 
 if __name__ == "__main__":
     from most_queue.sim import smo_im
     from most_queue.sim import rand_destribution as rd
-    from most_queue.utils.tables import probs_print
 
     ro = 0.8  # коэффициент загрузки
     a1 = 1  # среднее время между заявками вх потока
     n = 4  # число каналов
     coev_a = 0.56  # коэффициент вариации вх потока
     num_of_jobs = 800000  # количество заявок для ИМ
 
@@ -167,10 +166,14 @@
     smo.set_sources([k, l], "E")
     smo.set_servers(b, "D")
     smo.run(num_of_jobs)
     v_im = smo.v
     p_im = smo.get_p()
 
     print("-" * 36)
-    print("{0:^36s}".format("СМО E{0:d}/D/{1:d}".format(k, n)))
-
-    probs_print(p_im, p_ch, 10)
+    print("{0:^36s}".format("Вероятности состояний СМО E{0:d}/D/{1:d}".format(k, n)))
+    print("-" * 36)
+    print("{0:^4s}|{1:^15s}|{2:^15s}".format("№", "Числ", "ИМ"))
+    print("-" * 36)
+    for i in range(11):
+        print("{0:^4d}|{1:^15.5g}|{2:^15.5g}".format(i, p_ch[i], p_im[i]))
+    print("-" * 36)
```

### Comparing `most_queue-1.20/most_queue/theory/engset_model.py` & `most_queue-1.3/most_queue/theory/engset_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,16 +119,14 @@
         """
         w = self.get_w()
         b = [1.0 / self.mu, 2.0 / pow(self.mu, 2), 6.0 / pow(self.mu, 3)]
         return sv_sum_calc.get_moments(w, b)
 
 
 if __name__ == '__main__':
-    from most_queue.utils.tables import times_print
-
     lam = 0.3
     mu = 1.0
     m = 7
 
     engset = Engset(lam, mu, m)
 
     ps = engset.get_p()
```

### Comparing `most_queue-1.20/most_queue/theory/fj_calc.py` & `most_queue-1.3/most_queue/theory/fj_calc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import mmnr_calc
 import mgn_tt
 import mg1_calc
 import sv_sum_calc
 
 import matplotlib.pyplot as plt
-from most_queue.sim import rand_destribution as rd
+import most_queue.sim.rand_destribution as rd
 import math
 import time
 
 
 def get_lambda(min, max):
     l = np.random.randn()
     while l < min or l > max: \
```

### Comparing `most_queue-1.20/most_queue/theory/flow_sum.py` & `most_queue-1.3/most_queue/theory/flow_sum.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/theory/generate_pareto_noise.py` & `most_queue-1.3/most_queue/theory/generate_pareto_noise.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/theory/gi_m_1_calc.py` & `most_queue-1.3/most_queue/theory/gi_m_1_calc.py`

 * *Files 22% similar despite different names*

```diff
@@ -86,15 +86,14 @@
 
     return 0
 
 
 if __name__ == '__main__':
 
     from most_queue.sim import smo_im
-    from most_queue.utils.tables import times_print, probs_print
 
     l = 1
     a1 = 1 / l
     b1 = 0.9
     mu = 1 / b1
     a_coev = 1.6
     num_of_jobs = 800000
@@ -107,41 +106,66 @@
     smo = smo_im.SmoIm(1)
     smo.set_sources([v, alpha], "Gamma")
     smo.set_servers(mu, "M")
     smo.run(num_of_jobs)
     v_im = smo.v
     p_im = smo.get_p()
 
-    print("\nGamma\n")
+    print("\nGamma. Значения начальных моментов времени пребывания заявок в системе:\n")
 
-    times_print(v_im, v_ch, is_w=False)
+    print("{0:^15s}|{1:^15s}|{2:^15s}".format("№ момента", "Числ", "ИМ"))
+    print("-" * 45)
+    for j in range(3):
+        print("{0:^16d}|{1:^15.5g}|{2:^15.5g}".format(j + 1, v_ch[j], v_im[j]))
 
     w_ch = get_w(a, mu)
     w_im = smo.w
 
-    times_print(w_im, w_ch, is_w=True)
+    print("\nЗначения начальных моментов времени ожидания заявок в системе:\n")
+
+    print("{0:^15s}|{1:^15s}|{2:^15s}".format("№ момента", "Числ", "ИМ"))
+    print("-" * 45)
+    for j in range(3):
+        print("{0:^16d}|{1:^15.5g}|{2:^15.5g}".format(j + 1, w_ch[j], w_im[j]))
+
+    print("{0:^25s}".format("Вероятности состояний СМО"))
+    print("{0:^3s}|{1:^15s}|{2:^15s}".format("№", "Числ", "ИМ"))
+    print("-" * 32)
+    for i in range(11):
+        print("{0:^4d}|{1:^15.3g}|{2:^15.3g}".format(i, p_ch[i], p_im[i]))
 
-    probs_print(p_im, p_ch, 10)
 
     # Pareto test
     alpha, K = rd.Pareto_dist.get_a_k_by_mean_and_coev(a1, a_coev)
     a = rd.Pareto_dist.calc_theory_moments(alpha, K)
     v_ch = get_v(a, mu, approx_distr="Pa")
     p_ch = get_p(a, mu, approx_distr="Pa")
 
     smo = smo_im.SmoIm(1)
     smo.set_sources([alpha, K], "Pa")
     smo.set_servers(mu, "M")
     smo.run(num_of_jobs)
     v_im = smo.v
     p_im = smo.get_p()
 
-    print("\nPareto\n")
+    print("\nPareto. Значения начальных моментов времени пребывания заявок в системе:\n")
 
-    times_print(v_im, v_ch, is_w=False)
+    print("{0:^15s}|{1:^15s}|{2:^15s}".format("№ момента", "Числ", "ИМ"))
+    print("-" * 45)
+    for j in range(3):
+        print("{0:^16d}|{1:^15.5g}|{2:^15.5g}".format(j + 1, v_ch[j], v_im[j]))
 
     w_ch = get_w(a, mu, approx_distr="Pa")
     w_im = smo.w
 
-    times_print(w_im, w_ch, is_w=True)
+    print("\nЗначения начальных моментов времени ожидания заявок в системе:\n")
 
-    probs_print(p_im, p_ch, 10)
+    print("{0:^15s}|{1:^15s}|{2:^15s}".format("№ момента", "Числ", "ИМ"))
+    print("-" * 45)
+    for j in range(3):
+        print("{0:^16d}|{1:^15.5g}|{2:^15.5g}".format(j + 1, w_ch[j], w_im[j]))
+
+    print("{0:^25s}".format("Вероятности состояний СМО"))
+    print("{0:^3s}|{1:^15s}|{2:^15s}".format("№", "Числ", "ИМ"))
+    print("-" * 32)
+    for i in range(11):
+        print("{0:^4d}|{1:^15.3g}|{2:^15.3g}".format(i, p_ch[i], p_im[i]))
```

### Comparing `most_queue-1.20/most_queue/theory/gi_m_n_calc.py` & `most_queue-1.3/most_queue/theory/gi_m_n_calc.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import math
 from most_queue.sim import rand_destribution as rd
-import q_poisson_arrival_calc
-import sv_sum_calc
-import diff5dots
+from most_queue.theory import q_poisson_arrival_calc
+from most_queue.theory import sv_sum_calc
+from most_queue.theory import diff5dots
 
 
 def get_pi(a, mu, n, num=100, e=1e-10, approx_distr="Gamma"):
     """
     Вычисление вероятностей состояний СМО
     a - список начальных моментов распределения интервало рекуррентного вх потока заявок
     mu - интенсивность обслуживания
@@ -144,15 +144,14 @@
 
     return 0
 
 
 if __name__ == '__main__':
 
     from most_queue.sim import smo_im
-    from most_queue.utils.tables import times_print, probs_print
 
     l = 1.0
     a1 = 1.0 / l
     n = 4
     ro = 0.8
     b1 = ro * n / l
     mu = 1 / b1
@@ -168,41 +167,65 @@
     smo = smo_im.SmoIm(n)
     smo.set_sources([v, alpha], "Gamma")
     smo.set_servers(mu, "M")
     smo.run(num_of_jobs)
     v_im = smo.v
     p_im = smo.get_p()
 
-    print("Gamma\n")
+    print("\nGamma. Значения начальных моментов времени пребывания заявок в системе:\n")
 
-    times_print(v_im, v_ch, is_w=False)
+    print("{0:^15s}|{1:^15s}|{2:^15s}".format("№ момента", "Числ", "ИМ"))
+    print("-" * 45)
+    for j in range(3):
+        print("{0:^16d}|{1:^15.5g}|{2:^15.5g}".format(j + 1, v_ch[j], v_im[j]))
 
     w_ch = get_w(a, mu, n)
     w_im = smo.w
 
-    times_print(w_im, w_ch, is_w=True)
+    print("\nЗначения начальных моментов времени ожидания заявок в системе:\n")
 
-    probs_print(p_im, p_ch, 10)
+    print("{0:^15s}|{1:^15s}|{2:^15s}".format("№ момента", "Числ", "ИМ"))
+    print("-" * 45)
+    for j in range(3):
+        print("{0:^16d}|{1:^15.5g}|{2:^15.5g}".format(j + 1, w_ch[j], w_im[j]))
+
+    print("{0:^25s}".format("Вероятности состояний СМО"))
+    print("{0:^3s}|{1:^15s}|{2:^15s}".format("№", "Числ", "ИМ"))
+    print("-" * 32)
+    for i in range(11):
+        print("{0:^4d}|{1:^15.3g}|{2:^15.3g}".format(i, p_ch[i], p_im[i]))
 
     # Pareto test
     alpha, K = rd.Pareto_dist.get_a_k_by_mean_and_coev(a1, a_coev)
     a = rd.Pareto_dist.calc_theory_moments(alpha, K)
     v_ch = get_v(a, mu, n, approx_distr="Pa")
     p_ch = get_p(a, mu, n, approx_distr="Pa")
 
     smo = smo_im.SmoIm(n)
     smo.set_sources([alpha, K], "Pa")
     smo.set_servers(mu, "M")
     smo.run(num_of_jobs)
     v_im = smo.v
     p_im = smo.get_p()
 
-    print("Pareto\n")
+    print("\nPareto. Значения начальных моментов времени пребывания заявок в системе:\n")
 
-    times_print(v_im, v_ch, is_w=False)
+    print("{0:^15s}|{1:^15s}|{2:^15s}".format("№ момента", "Числ", "ИМ"))
+    print("-" * 45)
+    for j in range(3):
+        print("{0:^16d}|{1:^15.5g}|{2:^15.5g}".format(j + 1, v_ch[j], v_im[j]))
 
     w_ch = get_w(a, mu, n, approx_distr="Pa")
     w_im = smo.w
 
-    times_print(w_im, w_ch, is_w=True)
+    print("\nЗначения начальных моментов времени ожидания заявок в системе:\n")
 
-    probs_print(p_im, p_ch, 10)
+    print("{0:^15s}|{1:^15s}|{2:^15s}".format("№ момента", "Числ", "ИМ"))
+    print("-" * 45)
+    for j in range(3):
+        print("{0:^16d}|{1:^15.5g}|{2:^15.5g}".format(j + 1, w_ch[j], w_im[j]))
+
+    print("{0:^25s}".format("Вероятности состояний СМО"))
+    print("{0:^3s}|{1:^15s}|{2:^15s}".format("№", "Числ", "ИМ"))
+    print("-" * 32)
+    for i in range(11):
+        print("{0:^4d}|{1:^15.3g}|{2:^15.3g}".format(i, p_ch[i], p_im[i]))
```

### Comparing `most_queue-1.20/most_queue/theory/impatience_calc.py` & `most_queue-1.3/most_queue/theory/impatience_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/theory/m_d_n_calc.py` & `most_queue-1.3/most_queue/theory/m_d_n_calc.py`

 * *Files 5% similar despite different names*

```diff
@@ -108,15 +108,14 @@
             z[m] = z_old
         self.z_ = z
 
 
 if __name__ == "__main__":
 
     from most_queue.sim import smo_im
-    from most_queue.utils.tables import probs_print
 
     l = 1.0  # интенсивность входного потока
     ro = 0.8  # коэффициент загрузки
     n = 2  # количество каналов обслуживания
     num_of_jobs = 800000  # количество заявок для ИМ
 
     b = ro * n / l
@@ -126,8 +125,15 @@
     smo = smo_im.SmoIm(n)
     smo.set_sources(l, "M")
     smo.set_servers(b, "D")
     smo.run(num_of_jobs)
     v_im = smo.v
     p_im = smo.get_p()
 
-    probs_print(p_im, p_ch, 10)
+    print("-" * 36)
+    print("{0:^36s}".format("Вероятности состояний СМО M/D/{0:d}".format(n)))
+    print("-" * 36)
+    print("{0:^4s}|{1:^15s}|{2:^15s}".format("№", "Числ", "ИМ"))
+    print("-" * 36)
+    for i in range(11):
+        print("{0:^4d}|{1:^15.5g}|{2:^15.5g}".format(i, p_ch[i], p_im[i]))
+    print("-" * 36)
```

### Comparing `most_queue-1.20/most_queue/theory/m_h2_h2warm.py` & `most_queue-1.3/most_queue/theory/m_ph_n_prty.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,332 +1,323 @@
 import numpy as np
 import math
-from tqdm import tqdm
+from most_queue.theory import passage_time 
 from most_queue.sim import rand_destribution as rd
-from scipy import special
-from most_queue.utils.binom_probs import calc_binom_probs
-from diff5dots import diff5dots
-from scipy.misc import derivative
 
 
-class Mh2h2Warm:
+class m_ph_n_prty:
     """
-    Расчет СМО M/H2/n с H2-разогревом численным методом Такахаси-Таками.
-    Используются комплексные параметры, которые позволяют аппроксимировать распределение времени обслуживания
-    с произвольными коэффициентами вариации (>1, <=1)
+    Расчет СМО M/PH, M/n с 2-мя классами заявок, абсолютным приоритетом
+    численным методом Такахаси-Таками на основе аппроксимации ПНЗ распределением Кокса второго порядка
     """
 
-    def __init__(self, l, b, b_warm, n, buffer=None, N=150, accuracy=1e-6, dtype="c16", verbose=False,
-                 is_only_first=False):
+    def __init__(self, mu_L, mu1_H, mu2_H, p_H, l_L, l_H, n, N=250,
+                 accuracy=1e-8, max_iter=300, is_cox=True, approx_ee=0.1, approx_e=0.5, is_fitting=True,
+                 verbose=True):
 
         """
-        n: число каналов
-        l: интенсивность вх. потока
-        b: начальные моменты времени обслуживания
-        b_warm: начальные моменты времени разогрева
-        buffer: максимальная длина очереди. Если не задана - бесконечная очередь
+        Численный расчет СМО M/Ph/n с абсолютным приоритетом на основе аппроксимации периодов непрерывной занятости
+        l_L, l_H: интенсивности вх. потока заявок с низким и высоким приоритетами
+        mu_L: интенсивность обслуживания заявок с низким приоритетом,
+        mu1_H, mu2_H, p_H: параметры Cox2 (H2) - распределения для заявок высокого класса
         N: число ярусов
         accuracy: точность, параметр для остановки итерации
-        dtype: 'c16' - с комплексными параметрами, float - float
-        verbose: отображать ли коммантарии во время расчета
-        is_only_first: разогрев только первой заявки. Заданное время разогрева - время обслуживания первой заявки
-        """
-        self.dt = np.dtype(dtype)
-        if buffer:
-            self.R = buffer + n  # максимальное число заявок в сисетеме - очередь + каналы
-            self.N = self.R + 1  # число ярусов на один больше + нулевое состояние
-        else:
-            self.N = N
-            self.R = None  # для проверки задан ли буфер
-
-        self.is_only_first = is_only_first
-
+        is_cox:
+            True -  для аппроксимации времени обслуживания заявок первого класса используется
+                    распределение Кокса 2-го порядка,
+            False - гиперэкспоненциальное распределение 2-го порядка H2
+        """
+        # self.dt = np.dtype("f8")
+        self.dt = np.dtype("c16")
+        self.n = n  # количество каналов
+        self.N = N
         self.e1 = accuracy
-        self.n = n
-        self.b = b
+        self.l_L = l_L
+        self.l_H = l_H
+        self.mu_L = mu_L
+        self.mu1_H = mu1_H
+        self.mu2_H = mu2_H
+        self.p_H = p_H
+        self.max_iter = max_iter
+        self.is_cox = is_cox
         self.verbose = verbose
-        self.l = l
+        self.approx_ee = approx_ee
+        self.approx_e = approx_e
+        self.is_fitting = is_fitting
+
+        self.busy_periods = []  # список из наборов начальных моментров ПНЗ B1, B2, ...
+        self.busy_periods_coevs = []  # коэффициенты вариации ПНЗ
+        self.alphas = []
+        self.pp = []  # список из вероятностей переходов в ПНЗ
 
-        if self.dt == 'c16':
-            h2_params_service = rd.H2_dist.get_params_clx(b)
-        else:
-            h2_params_service = rd.H2_dist.get_params(b)
-
-        # параметры H2-распределения:
-        self.y = [h2_params_service[0], 1.0 - h2_params_service[0]]
-        self.mu = [h2_params_service[1], h2_params_service[2]]
-
-        self.b_warm = b_warm
-        if self.dt == 'c16':
-            h2_params_warm = rd.H2_dist.get_params_clx(b_warm)
-        else:
-            h2_params_warm = rd.H2_dist.get_params(b_warm)
-        self.y_w = [h2_params_warm[0], 1.0 - h2_params_warm[0]]
-        self.mu_w = [h2_params_warm[1], h2_params_warm[2]]
+        self.calc_busy_periods()
 
         # массив cols хранит число столбцов для каждого яруса, удобней рассчитать его один раз:
         self.cols = [] * N
 
         # переменные
         self.t = []
         self.b1 = []
         self.b2 = []
-        if self.dt == 'c16':
-            self.x = [0.0 + 0.0j] * N
-            self.z = [0.0 + 0.0j] * N
+        self.x = [0.0 + 0.0j] * N
+        self.z = [0.0 + 0.0j] * N
 
-            # искомые вреоятности состояний СМО
-            self.p = [0.0 + 0.0j] * N
-        else:
-            self.x = [0.0] * N
-            self.z = [0.0] * N
-
-            # искомые вреоятности состояний СМО
-            self.p = [0.0] * N
+        # искомые вреоятности состояний СМО
+        self.p = [0.0 + 0.0j] * N
 
         # матрицы переходов
         self.A = []
         self.B = []
         self.C = []
         self.D = []
         self.Y = []
 
-        for i in range(N):
-
-            if self.is_only_first:
-                if i < n + 1:
-                    if i == 0:
-                        self.cols.append(1)  # 00 state
-                    else:
-                        self.cols.append(3 * i + 1)  # w1 w2 01 10
-                else:
-                    self.cols.append(3 * n + 1)
-            else:
-                if i < n + 1:
-                    if i == 0:
-                        self.cols.append(1)  # 00 state
-                    else:
-                        self.cols.append(i + 3)  # w1 w2 01 10, w1 w2 20 11 02, ...
-                else:
-                    self.cols.append(n + 3)
+        # cols зависит от числа каналов. cols = количество всех микросостояний переходов для Cox2 до яруса
+        # с номером N-1 + число ПНЗ * 2. Число ПНЗ = n**2
+        self.cols_length_ = 2 * self.n ** 2
+        for i in range(self.n):
+            self.cols_length_ += i + 1
 
-            self.t.append(np.zeros((1, self.cols[i]), dtype=self.dt))
-            self.b1.append(np.zeros((1, self.cols[i]), dtype=self.dt))
-            self.b2.append(np.zeros((1, self.cols[i]), dtype=self.dt))
-            self.x.append(np.zeros((1, self.cols[i]), dtype=self.dt))
+        for i in range(N):
+            self.t.append(np.zeros((1, self.cols_length_), dtype=self.dt))
+            self.b1.append(np.zeros((1, self.cols_length_), dtype=self.dt))
+            self.b2.append(np.zeros((1, self.cols_length_), dtype=self.dt))
+            self.x.append(np.zeros((1, self.cols_length_), dtype=self.dt))
 
         self.build_matrices()
         self.initial_probabilities()
-        self.key_numbers = self.get_key_numbers(self.n)  # ключи яруса n, для n=3 [(3,0) (2,1) (1,2) (0,3)]
-        self.down_probs = self.calc_down_probs(self.n + 1)
 
-    def get_p(self):
+    def build_A_for_busy_periods(self, num):
         """
-        Возвращает список с вероятностями состояний системы
-        p[k] - вероятность пребывания в системе ровно k заявок
+            Формирует матрицу А(L) для расчета ПНЗ по заданному номеру яруса
+            num - номер яруса
         """
-        for i in range(len(self.p)):
-            self.p[i] = self.p[i].real
-        return self.p
-
-    def pls(self, mu, s):
-        return mu / (mu + s)
-
-    def get_key_numbers(self, level):
-        key_numbers = []
-        for i in range(level + 1):
-            key_numbers.append((self.n - i, i))
-        return np.array(key_numbers, dtype=self.dt)
-
-    def calc_down_probs(self, from_level):
-        if from_level == self.n:
-            return np.eye(self.n + 1)
-        b_matrix = self.B[from_level]
-        probs = []
-        for i in range(2, self.cols[from_level - 1]):
-            probs_on_level = []
-            for j in range(2, self.cols[from_level - 1]):
-                if from_level != 1:
-                    probs_on_level.append(b_matrix[i, j] / sum(b_matrix[i, :]))
-                else:
-                    probs_on_level.append(b_matrix[i, 0] / sum(b_matrix[i, :]))
-            probs.append(probs_on_level)
-        return np.array(probs, dtype=self.dt)
-
-    def matrix_pow(self, matrix, k):
-        res = np.eye(self.n + 1, dtype=self.dt)
-        for i in range(k):
-            res = np.dot(res, matrix)
-        return res
-
-    def calc_w_pls(self, s):
-        w = 0
-        # вероятности попадания в состояния обслуживания, вычисляются с помощью биноминального распределения
-        probs = calc_binom_probs(self.n + 1, self.y[0])
-
-        # Если заявка попала в фазу разогрева, хотя каналы свободны,
-        # ей придется подождать окончание разогрева
-        for k in range(1, self.n):
-            for i in range(2):
-                w += self.Y[k][0, i] * self.pls(self.mu_w[i], s)
+        if num < self.n:
+            col = num + 2
+            row = num + 1
+        elif num == self.n:
+            col = num + 1
+            row = num + 1
+        else:
+            output = self.A_for_busy[self.n]
+            return output
 
-        for k in range(self.n, self.N):
+        output = np.zeros((row, col), dtype=self.dt)
 
-            # Если заявка попала в фазу разогрева и каналы заняты. Также есть k-n заявок в очереди
-            # ей придется подождать окончание разогрева + обслуживание всех накопленных заявок
-            # key_numbers = self.get_key_numbers(self.n)  # ключи яруса n, для n=3 [(3,0) (2,1) (1,2) (0,3)]
+        for i in range(row):
+            output[i, i] = self.l_H
+        return output
 
-            a = np.array(
-                [self.pls(self.key_numbers[j][0] * self.mu[0] + self.key_numbers[j][1] * self.mu[1], s) for j in
-                 range(self.n + 1)])
+    def build_B_for_busy_periods(self, num):
+        """
+            Формирует матрицу B(num) для расчета ПНЗ  по заданному номеру яруса
+            num - номер яруса
+        """
+        if num == 0:
+            output = np.zeros((1, 1), dtype=self.dt)
+            return output
+        elif num <= self.n:
+            col = num
+            row = num + 1
+        elif num == self.n + 1:
+            col = num
+            row = num
+            output = np.zeros((row, col), dtype=self.dt)
+            output[:, :self.n] = self.B_for_busy[self.n]
+            return output
+        else:
+            output = self.B_for_busy[self.n + 1]
+            return output
 
-            P = self.down_probs  # calc_down_probs(k)
-            Pa = np.transpose(self.matrix_pow(P * a, k - self.n))  # n+1 x n+1
+        output = np.zeros((row, col), dtype=self.dt)
 
-            aP_tilda = a * probs
+        mu1 = self.mu1_H
+        mu2 = self.mu2_H
+        qH = 1.0 - self.p_H
 
-            pls_service_total = sum(np.dot(aP_tilda, Pa))
+        for i in range(col):
+            output[i, i] = (num - i) * mu1 * qH
+            output[i + 1, i] = (i + 1) * mu2
+        return output
 
-            for i in range(2):
-                w += self.Y[k][0, i] * self.pls(self.mu_w[i], s) * pls_service_total
+    def build_C_for_busy_periods(self, num):
+        """
+            Формирует матрицу C(num) для расчета ПНЗ по заданному номеру яруса
+            num - номер яруса
+        """
+        if num == 0:
+            output = np.zeros((1, 1), dtype=self.dt)
+            return output
+        elif num <= self.n:
+            col = num + 1
+            row = num + 1
+        else:
+            output = self.C_for_busy[self.n]
+            return output
 
-            # попала в фазу обслуживания
-            Ys = [self.Y[k][0, i + 2] for i in range(len(probs))]
-            aPa = np.dot(a, Pa)
-            for i in range(self.n + 1):
-                w += Ys[i] * aPa[i]
+        output = np.zeros((row, col), dtype=self.dt)
 
-        return w
+        mu1 = self.mu1_H
+        pH = self.p_H
 
-    def calc_residual_b(self, mom_num):
-        res = self.b[mom_num + 1] / (2.0 * self.b[mom_num])
-        return res
+        for i in range(col - 1):
+            output[i, i + 1] = (num - i) * mu1 * pH
+        return output
 
-    def get_w(self):
+    def build_D_for_busy_periods(self, num):
         """
-        Возвращает три первых начальных момента времени ожидания в СМО
+            Формирует матрицу D для ПНЗ по заданному номеру яруса num
         """
-        w = [0.0] * 3
+        if num <= self.n:
+            col = num + 1
+            row = num + 1
+        else:
+            output = self.D_for_busy[self.n]
+            return output
 
-        if self.is_only_first:
+        output = np.zeros((row, col), dtype=self.dt)
 
-            for j in range(1, len(self.p) - self.n):
-                w[0] += j * self.p[self.n + j]
-            for j in range(2, len(self.p) - self.n):
-                w[1] += j * (j - 1) * self.p[self.n + j]
-            for j in range(3, len(self.p) - self.n):
-                w[2] += j * (j - 1) * (j - 2) * self.p[self.n + j]
+        for i in range(row):
+            sumA = 0.0 + 0.0j
+            sumB = 0.0 + 0.0j
+            sumC = 0.0 + 0.0j
 
-            for j in range(3):
-                w[j] /= math.pow(self.l, j + 1)
-                w[j] = w[j].real
+            for j in range(col):
+                sumA += self.A_for_busy[num][i, j]
 
-            return w
+            if num != 0:
+                for j in range(col - 1):
+                    sumB += self.B_for_busy[num][i, j]
 
-        else:
-            for i in range(3):
-                w[i] = derivative(self.calc_w_pls, 0, dx=1e-3 / self.b[0], n=i + 1, order=9)
-            return [-w[0].real, w[1].real, -w[2].real]
-
-    def get_b(self):
-        b_plus_b_warm = [0.0] * 3
-        for i in range(3):
-            b_plus_b_warm[i] = self.b[i] * (1.0 - self.p[0]) + self.p[0] * self.b_warm[i]
-        return b_plus_b_warm
-
-    def get_v(self):
-        """
-        Возвращает три первых начальных момента времени пребывания в СМО
-        """
-        v = [0.0] * 3
-        if self.is_only_first:
-            w = self.get_w()
-            b = self.get_b()
-            v[0] = w[0] + b[0]
-            v[1] = w[1] + 2 * w[0] * b[0] + b[1]
-            v[2] = w[2] + 3 * w[1] * b[0] + 3 * w[0] * b[1] + b[2]
+            for j in range(col):
+                sumC += self.C_for_busy[num][i, j]
 
-        else:
-            w = self.get_w()
-            v[0] = w[0] + self.b[0]
-            v[1] = w[1] + 2 * w[0] * self.b[0] + self.b[1]
-            v[2] = w[2] + 3 * w[1] * self.b[0] + 3 * w[0] * self.b[1] + self.b[2]
+            output[i, i] = sumA + sumB + sumC
 
-        return v
+        return output
 
-    def print_mrx(self, mrx):
-        row = mrx.shape[0]
-        col = mrx.shape[1]
+    def calc_busy_periods(self):
 
-        for i in range(row):
-            for j in range(col):
-                if math.isclose(mrx[i, j].real, 0.0):
-                    print("{0:^5s} | ".format("     "), end="")
+        self.A_for_busy = []
+        self.B_for_busy = []
+        self.C_for_busy = []
+        self.D_for_busy = []
+
+        for i in range(self.n + 2):
+            self.A_for_busy.append(self.build_A_for_busy_periods(i))
+            self.B_for_busy.append(self.build_B_for_busy_periods(i))
+            self.C_for_busy.append(self.build_C_for_busy_periods(i))
+            self.D_for_busy.append(self.build_D_for_busy_periods(i))
+
+        pass_time = passage_time.passage_time_calc(self.A_for_busy, self.B_for_busy,
+                                                   self.C_for_busy, self.D_for_busy, is_clx=True, is_verbose=True)
+        pass_time.calc()
+
+        self.pnz_num_ = self.n ** 2
+
+        for j in range(self.pnz_num_):
+            self.busy_periods.append([0, 0, 0])
+
+        num = 0
+        for i in range(self.n):
+            for j in range(self.n):
+                for r in range(3):
+                    self.busy_periods[num][r] = pass_time.Z[self.n][r][i, j]
+                num = num + 1
+
+        for j in range(self.pnz_num_):
+            under_sqrt = self.busy_periods[j][1] - self.busy_periods[j][0] ** 2
+            if under_sqrt > 0:
+                coev = math.sqrt(under_sqrt.real)
+                self.alphas.append(1 / (coev ** 2))
+                self.busy_periods_coevs.append(coev / self.busy_periods[j][0])
+            else:
+                self.busy_periods_coevs.append(math.inf)
+
+        if self.verbose:
+            print("\nПериоды НЗ:\n")
+            for j in range(self.pnz_num_):
+                for r in range(3):
+                    if math.isclose(self.busy_periods[j][r].imag, 0):
+                        print("{0:^8.3g}".format(self.busy_periods[j][r].real), end=" ")
+                    else:
+                        print("{0:^8.3g}".format(self.busy_periods[j][r]), end=" ")
+                if math.isclose(self.busy_periods_coevs[j].imag, 0):
+                    print("coev = {0:^4.3g}".format(self.busy_periods_coevs[j].real))
+                else:
+                    print("coev = {0:^4.3g}".format(self.busy_periods_coevs[j]))
+
+        # pp - список из n**2 вероятностей переходов
+        for j in range(self.pnz_num_):
+            num = 0
+            for i in range(self.n):
+                for j in range(self.n):
+                    self.pp.append(pass_time.G[self.n][i, j])
+                    num = num + 1
+        if self.verbose:
+            print("\nВероятности переходов в ПНЗ:\n")
+            for j in range(self.pnz_num_):
+                if math.isclose(self.pp[j].imag, 0):
+                    print("{0:^8.3g}".format(self.pp[j].real), end=" ")
                 else:
-                    print("{0:^5.3f} | ".format(mrx[i, j].real), end="")
-            print("\n" + "--------" * col)
+                    print("{0:^8.3g}".format(self.pp[j]), end=" ")
 
-    @staticmethod
-    def binom_calc(a, b, num=3):
-        res = []
-        if num > 0:
-            res.append(a[0] + b[0])
-        if num > 1:
-            res.append(a[1] + 2 * a[0] * b[0] + b[1])
-        if num > 2:
-            res.append(a[2] + 3 * a[1] * b[0] + 3 * b[1] * a[0] + b[2])
-        return res
+    def get_p(self):
+        """
+        Возвращает список с вероятностями состояний системы
+        p[k] - вероятность пребывания в системе ровно k заявок класса L
+        """
+        p_real = [0.0] * self.N
+        for i in range(len(self.p)):
+            p_real[i] = self.p[i].real
+        return p_real
+
+    def get_low_class_v1(self):
+        """
+        Возвращает среднее время пребывания для класса L
+        """
+        l1 = 0
+        p_real = self.get_p()
+        for i in range(self.N):
+            l1 += p_real[i] * i
+        return l1 / self.l_L
 
     def initial_probabilities(self):
         """
         Задаем первоначальные значения вероятностей микросостояний
         """
         # t задаем равновероятными
         for i in range(self.N):
-            for j in range(self.cols[i]):
-                self.t[i][0, j] = 1.0 / self.cols[i]
+            for j in range(self.cols_length_):
+                self.t[i][0, j] = 1.0 / self.cols_length_
         self.x[0] = 0.4
 
-    def norm_probs(self):
-        summ = 0
-        for i in range(self.N):
-            summ += self.p[i]
-
-        for i in range(self.N):
-            self.p[i] /= summ
-
-        if self.verbose:
-            summ = 0
-            for i in range(self.N):
-                summ += self.p[i]
-            print("Summ of probs = {0:.5f}".format(summ))
-
     def calculate_p(self):
         """
         После окончания итераций находим значения вероятностей p по найденным х
         """
         # version 1
-        p_sum = 0
+        p_sum = 0 + 0j
         p0_max = 1.0
         p0_min = 0.0
-
-        while math.fabs(1.0 - p_sum) > 1e-6:
+        iter = 0
+        self.p_iteration_num_ = 0
+        while math.fabs(1.0 - p_sum.real) > 1e-6 and iter < self.max_iter:
+            iter += 1
             p0_ = (p0_max + p0_min) / 2.0
             p_sum = p0_
             self.p[0] = p0_
             for j in range(self.N - 1):
-                self.p[j + 1] = self.p[j] * self.x[j]
+                self.p[j + 1] = np.dot(self.p[j], self.x[j])
                 p_sum += self.p[j + 1]
-
-            if (p_sum > 1.0):
+            if p_sum.real > 1.0:
                 p0_max = p0_
             else:
                 p0_min = p0_
-
-        self.norm_probs()
+        self.p_iteration_num_ = iter
 
     def calculate_y(self):
         for i in range(self.N):
             self.Y.append(np.dot(self.p[i], self.t[i]))
 
     def build_matrices(self):
         """
@@ -334,134 +325,101 @@
         """
         for i in range(self.N):
             self.A.append(self.buildA(i))
             self.B.append(self.buildB(i))
             self.C.append(self.buildC(i))
             self.D.append(self.buildD(i))
 
-    def calc_g_matrices(self):
-        self.G = []
-        for j in range(0, self.N):
-            self.G.append(np.linalg.inv(self.D[j] - self.C[j]))
-
-    def calc_ag_matrices(self):
-        self.AG = [0]
-        for j in range(1, self.N):
-            self.AG.append(np.dot(self.A[j - 1], self.G[j]))
-
-    def calc_bg_matrices(self):
-        self.BG = [0]
-        for j in range(1, self.N):
-            if j != (self.N - 1):
-                self.BG.append(np.dot(self.B[j + 1], self.G[j]))
-            else:
-                self.BG.append(np.dot(self.B[j], self.G[j]))
-
-    def calc_support_matrices(self):
-        self.calc_g_matrices()
-        self.calc_ag_matrices()
-        self.calc_bg_matrices()
-
     def run(self):
         """
-        Запускает расчет
+        Запускает расчет. Алгоритм расчета не зависит от структуры матриц
         """
-        if self.dt == 'c16':
-            self.b1[0][0, 0] = 0.0 + 0.0j
-            self.b2[0][0, 0] = 0.0 + 0.0j
-            x_max1 = 0.0 + 0.0j
-            x_max2 = 0.0 + 0.0j
-        else:
-            self.b1[0][0, 0] = 0.0
-            self.b2[0][0, 0] = 0.0
-            x_max1 = 0.0
-            x_max2 = 0.0
+        self.b1[0][0, 0] = 0.0 + 0.0j
+        self.b2[0][0, 0] = 0.0 + 0.0j
+        
+        is_ave = False
 
-        self.calc_support_matrices()
 
-        self.num_of_iter_ = 0  # кол-во итераций алгоритма
-        for i in range(self.N):
-            if self.x[i].real > x_max1.real:
-                x_max1 = self.x[i]
 
-        while math.fabs(x_max2.real - x_max1.real) >= self.e1:
-            x_max2 = x_max1
-            self.num_of_iter_ += 1
+        iter = 0
+        self.run_iterations_num_ = 0
+        if is_ave:
+            x_ave1 = 0.0 + 0.0j
+            x_ave2 = 0.0 + 0.0j
+            for i in range(self.N):
+                x_ave1 += self.x[i]
+            x_ave1 /= self.N
+        else:
+
+            x_ave1 = 0.0
+            x_ave2 = 0.0
+            for i in range(self.N):
+                if self.x[i].real > x_ave1 :
+                    x_ave1 = self.x[i].real
 
+        while math.fabs(x_ave2.real - x_ave1.real) >= self.e1 and iter < self.max_iter:
+            if self.verbose:
+                print("Start numeric iteration {0:d}".format(iter))
+            iter += 1
+            x_ave2 = x_ave1
             for j in range(1, self.N):  # по всем ярусам, кроме первого.
 
+                G = np.linalg.inv(self.D[j] - self.C[j])
                 # b':
-                self.b1[j] = np.dot(self.t[j - 1], self.AG[j])
+                self.b1[j] = np.dot(self.t[j - 1], np.dot(self.A[j - 1], G))
 
                 # b":
                 if j != (self.N - 1):
-                    self.b2[j] = np.dot(self.t[j + 1], self.BG[j])
+                    self.b2[j] = np.dot(self.t[j + 1], np.dot(self.B[j + 1], G))
                 else:
-                    self.b2[j] = np.dot(self.t[j - 1], self.BG[j])
+                    self.b2[j] = np.dot(self.t[j - 1], np.dot(self.B[j], G))
 
                 c = self.calculate_c(j)
 
                 x_znam = np.dot(c, self.b1[j]) + self.b2[j]
-                if self.dt == 'c16':
-                    self.x[j] = 0.0 + 0.0j
-                else:
-                    self.x[j] = 0.0
+                self.x[j] = 0.0 + 0.0j
                 for k in range(x_znam.shape[1]):
                     self.x[j] += x_znam[0, k]
 
-                if self.dt == 'c16':
-                    self.x[j] = (1.0 + 0.0j) / self.x[j]
-                else:
-                    self.x[j] = (1.0) / self.x[j]
+                self.x[j] = 1.0 / self.x[j]
 
-                if self.R and j == (self.N - 1):
-                    tA = np.dot(self.t[j - 1], self.A[j - 1])
-                    tag = np.dot(tA, self.G[j])
-                    tag_sum = 0
-                    for t_i in range(tag.shape[1]):
-                        tag_sum += tag[0, t_i]
-                    self.z[j] = 1.0 / tag_sum
-                    self.t[j] = self.z[j] * tag
+                self.z[j] = np.dot(c, self.x[j])
+                self.t[j] = np.dot(self.z[j], self.b1[j]) + np.dot(self.x[j], self.b2[j])
 
-                else:
-
-                    self.z[j] = np.dot(c, self.x[j])
-                    self.t[j] = np.dot(self.z[j], self.b1[j]) + np.dot(self.x[j], self.b2[j])
-
-            if self.dt == 'c16':
-                self.x[0] = (1.0 + 0.0j) / self.z[1]
-            else:
-                self.x[0] = 1.0 / self.z[1]
+            self.x[0] = 1.0 / self.z[1]
 
             t1B1 = np.dot(self.t[1], self.B[1])
             self.t[0] = np.dot(self.x[0], t1B1)
-            self.t[0] = np.dot(self.t[0], self.G[0])
+            self.t[0] = np.dot(self.t[0], np.linalg.inv(self.D[0] - self.C[0]))
 
-            if self.dt == 'c16':
-                x_max1 = 0.0 + 0.0j
-            else:
-                x_max1 = 0
 
-            for i in range(self.N):
-                if self.x[i].real > x_max1.real:
-                    x_max1 = self.x[i]
 
-            if self.verbose:
-                print("End iter # {0:d}".format(self.num_of_iter_))
+            if is_ave:
+                x_ave1 = 0.0 + 0.0j
+                for i in range(self.N):
+                    x_ave1 += self.x[i]
+                x_ave1 /= self.N
+
+            else:
+                x_ave1 = 0.0
+                for i in range(self.N):
+                    if self.x[i].real > x_ave1:
+                        x_ave1 = self.x[i].real
 
+        self.run_iterations_num_ = iter
         self.calculate_p()
         self.calculate_y()
 
     def calculate_c(self, j):
         """
         Вычисляет значение переменной с, участвующей в расчете
         """
-        chisl = 0
-        znam = 0
-        znam2 = 0
+        chisl = 0.0 + 0.0j
+        znam = 0.0 + 0.0j
+        znam2 = 0.0 + 0.0j
 
         m = np.dot(self.b2[j], self.B[j])
         for k in range(m.shape[1]):
             chisl += m[0, k]
 
         m = np.dot(self.b1[j], self.B[j])
         for k in range(m.shape[1]):
@@ -469,279 +427,362 @@
 
         m = np.dot(self.t[j - 1], self.A[j - 1])
         for k in range(m.shape[1]):
             znam += m[0, k]
 
         return chisl / (znam - znam2)
 
-    def insert_standart_A_into(self, mass, l, y1, left_pos, bottom_pos, level):
-        row_num = level
-        for i in range(row_num):
-            mass[i + left_pos, i + bottom_pos] = l * y1
-            mass[i + left_pos, i + bottom_pos + 1] = l * (1.0 - y1)
-
     def buildA(self, num):
         """
-        Формирует матрицу А по заданному номеру яруса
+        Формирует матрицу А(L) по заданному номеру яруса num
         """
-        if num < self.n:
-            col = self.cols[num + 1]
-            row = self.cols[num]
-        else:
-            col = self.cols[self.n]
-            row = self.cols[self.n]
+        col = self.cols_length_
+        row = self.cols_length_
 
         output = np.zeros((row, col), dtype=self.dt)
-
-        if num > self.n:
-            output = self.A[self.n]
+        if num > 1:
+            output = self.A[0]
             return output
-        if num == 0:
-            output[0, 0] = self.l * self.y_w[0]
-            output[0, 1] = self.l * self.y_w[1]
-        else:
-
-            if num < self.n:
-                if self.is_only_first:
-                    # first block
-                    self.insert_standart_A_into(output, self.l, self.y[0], 0, 0, level=num)
-                    # second
-                    self.insert_standart_A_into(output, self.l, self.y[0], num, num + 1, level=num)
-                    # third
-                    self.insert_standart_A_into(output, self.l, self.y[0], 2 * num, 2 * (num + 1), level=num + 1)
-                else:
-                    # first block
-                    output[0, 0] = self.l
-                    output[1, 1] = self.l
-                    # second
-                    self.insert_standart_A_into(output, self.l, self.y[0], 2, 2, level=num + 1)
-            else:
-                for i in range(row):
-                    output[i, i] = self.l
-
+        for i in range(row):
+            output[i, i] = self.l_L
         return output
 
-    def insert_standart_B_into(self, mass, y, mu, left_pos, bottom_pos, level, n):
-        col = level
-        for i in range(col):
-            if level <= n:
-                mass[i + left_pos, i + bottom_pos] = (level - i) * mu[0]
-                mass[i + left_pos + 1, i + bottom_pos] = (i + 1) * mu[1]
-            else:
-                mass[i + left_pos, i + bottom_pos] = (level - i - 1) * mu[0] * y[0] + i * mu[1] * y[1]
-                if i != level - 1:
-                    mass[i + left_pos, i + bottom_pos + 1] = (level - i - 1) * mu[0] * y[1]
-                if i != level - 1:
-                    mass[i + + left_pos + 1, i + bottom_pos] = (i + 1) * mu[1] * y[0]
-
     def buildB(self, num):
         """
             Формирует матрицу B по заданному номеру яруса
         """
         if num == 0:
             return np.zeros((1, 1), dtype=self.dt)
 
-        if num <= self.n:
-
-            col = self.cols[num - 1]
-            row = self.cols[num]
-        else:
-            col = self.cols[self.n + 1]
-            row = self.cols[self.n + 1]
-
+        col = self.cols_length_
+        row = self.cols_length_
         output = np.zeros((row, col), dtype=self.dt)
-        if num > self.n + 1:
-            output = self.B[self.n + 1]
-            return output
-
-        if num == 1:
-            output[2, 0] = self.mu[0]
-            output[3, 0] = self.mu[1]
 
-            if self.is_only_first:
-                output[0, 0] = self.mu_w[0]
-                output[1, 0] = self.mu_w[1]
-        else:
-
-            if num < self.n + 1:
-
-                if self.is_only_first:
-                    # first block
-                    self.insert_standart_B_into(output, self.y, self.mu, 0, 0, num - 1, self.n)
-                    # second
-                    self.insert_standart_B_into(output, self.y, self.mu, num, num - 1, num - 1, self.n)
-                    # third
-                    self.insert_standart_B_into(output, self.y, self.mu, 2 * num, 2 * (num - 1), num, self.n)
-
-                    # warm block 1
-                    for i in range(num):
-                        output[i, i + 2 * (num - 1)] = self.mu_w[0]
-
-                    # warm block 2
-                    for i in range(num):
-                        output[i + num, i + 2 * (num - 1)] = self.mu_w[1]
-                else:
-                    self.insert_standart_B_into(output, self.y, self.mu, 2, 2, num, self.n)
-
-            else:
+        if num > self.n:
+            output = self.B[self.n]
+            return output
 
-                if self.is_only_first:
-                    # first block
-                    self.insert_standart_B_into(output, self.y, self.mu, 0, 0, num - 1, self.n - 1)
-                    # second
-                    self.insert_standart_B_into(output, self.y, self.mu, num - 1, num - 1, num - 1, self.n - 1)
-                    # third
-                    self.insert_standart_B_into(output, self.y, self.mu, 2 * (num - 1), 2 * (num - 1), num, self.n)
-
-                    # warm block 1
-                    for i in range(num - 1):
-                        output[i, i + 2 * (num - 1)] = self.mu_w[0] * self.y[0]
-                        output[i, i + 2 * (num - 1) + 1] = self.mu_w[0] * self.y[1]
-
-                    # warm block 2
-                    for i in range(num - 1):
-                        output[i + num - 1, i + 2 * (num - 1)] = self.mu_w[1] * self.y[0]
-                        output[i + num - 1, i + 2 * (num - 1) + 1] = self.mu_w[1] * self.y[1]
-
-                else:
-                    self.insert_standart_B_into(output, self.y, self.mu, 2, 2, num, self.n)
+        # Матрица B - диагональная. Количество ненулевых элементов зависит от числа n.
+        lev = 0
+        for i in range(self.n):  # количество ярусов до перехода в ПНЗ
+            for j in range(i + 1):  # количество микросочтояний в этом ярусе
+                output[lev, lev] = min(self.n - i, num) * self.mu_L
+                lev = lev + 1
 
         return output
 
     def buildC(self, num):
         """
             Формирует матрицу C по заданному номеру яруса
         """
-        if num < self.n:
-            col = self.cols[num]
-            row = col
-        else:
-            col = self.cols[self.n]
-            row = col
+        col = self.cols_length_
+        row = col
 
         output = np.zeros((row, col), dtype=self.dt)
-        if num > self.n:
-            output = self.C[self.n]
+        if num >= 1:
+            output = self.C[0]
             return output
 
-        if not self.is_only_first:
-            if num > 0:
-                probs = calc_binom_probs(num + 1, self.y[0])
-                for i in range(len(probs)):
-                    output[0, 2 + i] = self.mu_w[0] * probs[i]
-                    output[1, 2 + i] = self.mu_w[1] * probs[i]
+        lh = self.l_H
 
+        y1_mass = []
+        m1_mass = []
+        m2_mass = []
+        print("\n")
+
+        for i in range(self.pnz_num_):
+            if not self.is_cox:
+                h2_param = rd.H2_dist.get_params_clx(self.busy_periods[i], ee=self.approx_ee, e=self.approx_e, is_fitting=self.is_fitting)
+                # h2_param = rd.H2_dist.get_params(self.busy_periods[i])
+                y1_mass.append(h2_param[0])
+                m1_mass.append(h2_param[1])
+                m2_mass.append(h2_param[2])
+                if self.verbose:
+                    print("Параметры для B{0}: {1:3.3f}, {2:3.3f}, {3:3.3f}".format(i + 1, h2_param[0], h2_param[1],
+                                                                                    h2_param[2]))
+            else:
+                cox_params = rd.Cox_dist.get_params(self.busy_periods[i], ee=self.approx_ee, e=self.approx_e, is_fitting=self.is_fitting)
+                y1_mass.append(cox_params[0])
+                m1_mass.append(cox_params[1])
+                m2_mass.append(cox_params[2])
+                if self.verbose:
+                    print("Параметры для B{0}: {1:3.3f}, {2:3.3f}, {3:3.3f}".format(i + 1, cox_params[0], cox_params[1],
+                                                                                    cox_params[2]))
+
+        # first quad
+
+        # lH's = A_for_busy. Но поскольку = l_h, проще здесь посчитать заново
+        l_start = 0
+        for i in range(self.n - 1):
+            for j in range(i + 1):
+                output[l_start + j, l_start + j + i + 1] = lh
+            l_start += i + 1
+
+        # B_for_busy
+        l_start = 1
+        l_end = 0
+        for i in range(1, self.n):
+            rows = self.B_for_busy[i].shape[0]
+            cols = self.B_for_busy[i].shape[1]
+            for r in range(rows):
+                for c in range(cols):
+                    output[l_start + r, l_end + c] = self.B_for_busy[i][r, c]
+            l_start += i + 1
+            l_end += i
+
+        # C_for_busy
+        l_start = 1
+        for i in range(1, self.n):
+            rows = self.C_for_busy[i].shape[0]
+            cols = self.C_for_busy[i].shape[1]
+            for r in range(rows):
+                for c in range(cols):
+                    output[l_start + r, l_start + c] = self.C_for_busy[i][r, c]
+            l_start += i + 1
+
+        l_start = 0
+        for i in range(self.n - 1):
+            l_start += i + 1
+
+        l_end = l_start + self.n
+        num = 0
+        for i in range(self.n):
+            for j in range(self.n):
+                if not self.is_cox:
+                    output[l_start + i, l_end] = lh * y1_mass[num] * self.pp[num]
+                    output[l_start + i, l_end + 1] = lh * (1 - y1_mass[num]) * self.pp[num]
+                else:
+                    output[l_start + i, l_end] = lh * self.pp[num]
+                    output[l_start + i, l_end + 1] = 0
+                l_end += 2
+                num += 1
+
+        # left t's blocks
+        row = 0
+        for i in range(self.n):
+            row += i + 1
+
+        col = 0
+        for i in range(self.n - 1):
+            col += i + 1
+        num = 0
+        for i in range(self.n):
+            for j in range(self.n):
+                if not self.is_cox:
+                    output[row, col + j] = m1_mass[num]
+                    output[row + 1, col + j] = m2_mass[num]
+                else:
+                    output[row, col + j] = m1_mass[num] * (1.0 - y1_mass[num])
+                    output[row + 1, col + j] = m2_mass[num]
+                row += 2
+                num += 1
+
+        if self.is_cox:
+            # central T's block
+            row = 0
+            for i in range(self.n):
+                row += i + 1
+
+            col = 0
+            for i in range(self.n):
+                col += i + 1
+            num = 0
+            for i in range(self.n):
+                for j in range(self.n):
+                    output[row, col + 1] = m1_mass[num] * y1_mass[num]
+                    num += 1
+                    row += 2
+                    col += 2
         return output
 
+    def print_mrx(self, mrx, is_short=False):
+        row = mrx.shape[0]
+        col = mrx.shape[1]
+
+        for i in range(row):
+            for j in range(col):
+                if math.isclose(mrx[i, j].real, 0.0):
+                    if is_short:
+                        print("{0:^3s} | ".format(""), end="")
+                    else:
+                        print("{0:^5s} | ".format(""), end="")
+                else:
+                    if is_short:
+                        print("{0:^3.1f} | ".format(mrx[i, j].real), end="")
+                    else:
+                        print("{0:^5.3f} | ".format(mrx[i, j].real), end="")
+            if is_short:
+                print("\n" + "------" * col)
+            else:
+                print("\n" + "--------" * col)
+
     def buildD(self, num):
         """
             Формирует матрицу D по заданному номеру яруса
         """
-        if num < self.n:
-            col = self.cols[num]
-            row = col
-        else:
-            col = self.cols[self.n]
-            row = col
-
+        col = self.cols_length_
+        row = col
         output = np.zeros((row, col), dtype=self.dt)
 
         if num > self.n:
             output = self.D[self.n]
             return output
 
         for i in range(row):
-            if self.dt == 'c16':
-                sumA = 0.0 + 0.0j
-                sumB = 0.0 + 0.0j
-                sumC = 0.0 + 0.0j
-            else:
-                sumA = 0.0
-                sumB = 0.0
-                sumC = 0.0
+            sumA = 0.0 + 0.0j
+            sumB = 0.0 + 0.0j
+            sumC = 0.0 + 0.0j
 
-            for j in range(self.cols[num + 1]):
+            for j in range(self.cols_length_):
                 sumA += self.A[num][i, j]
 
             if num != 0:
-                for j in range(self.cols[num - 1]):
+                for j in range(self.cols_length_):
                     sumB += self.B[num][i, j]
 
-            for j in range(col):
+            for j in range(self.cols_length_):
                 sumC += self.C[num][i, j]
 
             output[i, i] = sumA + sumB + sumC
 
         return output
 
 
 if __name__ == "__main__":
-
-    import smo_im
+    from most_queue.sim import smo_im_prty
     from most_queue.sim import rand_destribution as rd
+    from most_queue.theory import prty_calc
     import time
-    from most_queue.utils.tables import times_print, probs_print
-
-    n = 3
-    # число каналов
-    l = 1.0  # интенсивность вх потока
-    ro = 0.7  # коэфф загрузки
-    b1 = n * ro  # ср время обслуживания
-    b1_warm = n * 0.2  # ср время разогрева
-    num_of_jobs = 1000000  # число обсл заявок ИМ
-    b_coev = [0.34, 1.3]  # коэфф вариации времени обсл
-    b_coev_warm = [0.8, 1.2]  # коэфф вариации времени разогрева
-    buff = None
-    verbose = False
-
-    for k in range(len(b_coev)):
-        b = [0.0] * 3
-        alpha = 1 / (b_coev[k] ** 2)
-        b[0] = b1
-        b[1] = math.pow(b[0], 2) * (math.pow(b_coev[k], 2) + 1)
-        b[2] = b[1] * b[0] * (1.0 + 2 / alpha)
-
-        b_w = [0.0] * 3
-        b_w[0] = b1_warm
-        alpha = 1 / (b_coev_warm[k] ** 2)
-        b_w[1] = math.pow(b_w[0], 2) * (math.pow(b_coev_warm[k], 2) + 1)
-        b_w[2] = b_w[1] * b_w[0] * (1.0 + 2 / alpha)
 
-        h2_params = rd.H2_dist.get_params_clx(b)
+    num_of_jobs = 800000  # число обсл заявок ИМ
 
-        im_start = time.process_time()
-        smo = smo_im.SmoIm(n, buffer=buff)
-        smo.set_sources(l, 'M')
+    is_cox = False  # использовать для аппроксимации ПНЗ распределение Кокса или Н2-распределение
+    max_iter = 100  # максимальное число итераций численного метода
+    # Исследование влияния среднего времени пребывания заявок 2-го класса от коэффициента загрузки
+    n = 4  # количество каналов
+    K = 2  # количество классов
+    ros = 0.75  # коэффициент загрузки СМО
+    bH_to_bL = 2  # время обслуживания класса H меньше L в это число раз
+    lH_to_lL = 1.5  # интенсивность поступления заявок класса H ниже L в это число раз
+    l_H = 1.0  # интенсивность вх потока заявок 1-го класса
+    l_L = lH_to_lL * l_H  # интенсивность вх потока заявок 2-го класса
+    bH_coev = [0.32, 0.63, 0.85, 1.2, 1.5]  # исследуемые коэффициенты вариации обсл заявок 1 класса
+    iteration = 1  # кол-во итераций ИМ для получения более точных оценок ИМ
+
+    v1_im_mass = []
+    v2_im_mass = []
+    v2_tt_mass = []
+    iter_num = []
+    tt_times = []
+    im_times = []
+    invar_times = []
+    v2_invar_mass = []
+
+    for k in range(len(bH_coev)):
+
+        print("coev =  {0:5.3f}".format(bH_coev[k]))
+
+        lsum = l_L + l_H
+        bsr = n * ros / lsum
+        bH1 = lsum * bsr / (l_L * bH_to_bL + l_H)
+        bL1 = bH_to_bL * bH1
+        bH = [0.0] * 3
+        alpha = 1 / (bH_coev[k] ** 2)
+        bH[0] = bH1
+        bH[1] = math.pow(bH[0], 2) * (math.pow(bH_coev[k], 2) + 1)
+        bH[2] = bH[1] * bH[0] * (1.0 + 2 / alpha)
+
+        gamma_params = rd.Gamma.get_mu_alpha([bH[0], bH[1]])
+
+        mu_L = 1.0 / bL1
+
+        # задание ИМ:
+        v1_sum = 0
+        v2_sum = 0
 
-        gamma_params = rd.Gamma.get_mu_alpha(b)
-        gamma_params_warm = rd.Gamma.get_mu_alpha(b_w)
-        smo.set_servers(gamma_params, 'Gamma')
-        smo.set_warm(gamma_params_warm, 'Gamma')
-        smo.run(num_of_jobs)
-        p = smo.get_p()
-        v_im = smo.v  # .w -> wait times
-        im_time = time.process_time() - im_start
+        cox_params = rd.Cox_dist.get_params(bH)
 
+        # расчет численным методом:
         tt_start = time.process_time()
-        tt = Mh2h2Warm(l, b, b_w, n, buffer=buff, verbose=verbose)
-
+        tt = m_ph_n_prty(mu_L, cox_params[1], cox_params[2], cox_params[0], l_L, l_H, n=n, is_cox=is_cox, max_iter=max_iter)
         tt.run()
-        p_tt = tt.get_p()
-        v_tt = tt.get_v()  # .get_w() -> wait times
-        print(v_tt)
+        tt_times.append(time.process_time() - tt_start)
 
-        tt_time = time.process_time() - tt_start
-        num_of_iter = tt.num_of_iter_
+        iter_num.append(tt.run_iterations_num_)
+        p_tt = tt.get_p()
+        v_tt = tt.get_low_class_v1()
+        v2_tt_mass.append(v_tt)
+        print("{0:^25s}".format("Вероятности состояний для заявок 2-го класса"))
+        print("{0:^3s}|{1:^15s}|{2:^15s}".format("№", "Числ", "ИМ"))
+        print("-" * 32)
+        for i in range(11):
+            print("{0:^4d}|{1:^15.3g}|{2:^15.3g}".format(i, p_tt[i], 0))
+        print("{0:^15.3f}|{1:^15.6g}|{2:^15.6g}|{3:^15d}".format(bH_coev[k], v2_tt_mass[k], 0, iter_num[k]))
+
+        mu_L = 1.0 / bL1
+
+        bL = rd.Exp_dist.calc_theory_moments(mu_L, 3)
+
+        b = []
+        b.append(bH)
+        b.append(bL)
+
+        L = [l_H, l_L]
+
+        invar_start = time.process_time()
+        v = prty_calc.get_v_prty_invar(L, b, n=n, type='PR', num=2)
+        v2_invar_mass.append(v[1][0])
+        invar_times.append(time.process_time() - invar_start)
 
-        print("\nСравнение результатов расчета методом Такахаси-Таками и ИМ.\n"
-              "ИМ - M/Gamma/{0:^2d} с Gamma разогревом\nТакахаси-Таками - M/H2/{0:^2d} c H2-разогревом "
-              "с комплексными параметрами\n"
-              "Коэффициент загрузки: {1:^1.2f}".format(n, ro))
-        print(f'Коэффициент вариации времени обслуживания {b_coev[k]:0.3f}')
-        print(f'Коэффициент вариации времени разогрева {b_coev_warm[k]:0.3f}')
-        print("Количество итераций алгоритма Такахаси-Таками: {0:^4d}".format(num_of_iter))
-        print("Время работы алгоритма Такахаси-Таками: {0:^5.3f} c".format(tt_time))
-        print("Время ИМ: {0:^5.3f} c".format(im_time))
+        im_start = time.process_time()
 
-        probs_print(p, p_tt, 10)
+        for i in range(iteration):
+            print("Start IM iteration: {0:d}".format(i + 1))
 
-        times_print(v_im, v_tt, is_w=False)
+            smo = smo_im_prty.SmoImPrty(n, K, "PR")
+            sources = []
+            servers_params = []
+            l = [l_H, l_L]
+
+            sources.append({'type': 'M', 'params': l_H})
+            sources.append({'type': 'M', 'params': l_L})
+            servers_params.append({'type': 'Gamma', 'params': gamma_params})
+            servers_params.append({'type': 'M', 'params': mu_L})
+
+            smo.set_sources(sources)
+            smo.set_servers(servers_params)
+
+            # запуск ИМ:
+            smo.run(num_of_jobs)
+
+            # получение результатов ИМ:
+            p = smo.get_p()
+            v_im = smo.v
+            v1_sum += v_im[0][0]
+            v2_sum += v_im[1][0]
+
+        v1 = v1_sum / iteration
+        v2 = v2_sum / iteration
+        # расчет численным методом:
+        v2_im_mass.append(v2)
+        im_times.append(time.process_time() - im_start)
+
+    print("\nСравнение результатов расчета численным методом с аппроксимацией ПНЗ "
+          "\nраспределением Кокса второго порядка и ИМ.")
+    print("ro: {0:1.2f}".format(ros))
+    print("n : {0:d}".format(n))
+    print("Количество обслуженных заявок для ИМ: {0:d}\n".format(num_of_jobs))
+
+    print("\n")
+    print("{0:^35s}".format("Средние времена пребывания в СМО для заявок 2-го класса"))
+    print("-" * 128)
+    print("{0:^15s}|{1:^15s}|{5:^15s}|{2:^15s}|{3:^15s}|{5:^15s}|{4:^15s}|{5:^15s}".format("coev", "Числ",
+                                                                                           "Кол-во итер алг", "ИМ",
+                                                                                           "Инвар", "t, c"))
+    print("-" * 128)
+    for k in range(len(bH_coev)):
+        print("{0:^15.3f}|{1:^15.6g}|{2:^15.6g}|{3:^15d}|{4:^15.6g}|{5:^15.6g}|{6:^15.6g}|{7:^15.6g}".format(
+            bH_coev[k],
+            v2_tt_mass[k], tt_times[k], iter_num[k],
+            v2_im_mass[k], im_times[k],
+            v2_invar_mass[k], invar_times[k]
+        ))
```

### Comparing `most_queue-1.20/most_queue/theory/m_ph_n_prty.py` & `most_queue-1.3/most_queue/theory/m_h2_h2warm.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,323 +1,222 @@
 import numpy as np
 import math
 import passage_time
-from most_queue.sim import rand_destribution as rd
+from tqdm import tqdm
 
 
-class m_ph_n_prty:
+class Mh2h2Warm:
     """
-    Расчет СМО M/PH, M/n с 2-мя классами заявок, абсолютным приоритетом
-    численным методом Такахаси-Таками на основе аппроксимации ПНЗ распределением Кокса второго порядка
+    Расчет СМО M/H2/H2warm/n с комплексными параметрами численным методом Такахаси-Таками.
+    Комплексные параметры позволяют аппроксимировать распределение времени обслуживания
+    с произволиными коэффициентами вариации (>1, <=1)
     """
 
-    def __init__(self, mu_L, mu1_H, mu2_H, p_H, l_L, l_H, n, N=250,
-                 accuracy=1e-8, max_iter=300, is_cox=True, approx_ee=0.1, approx_e=0.5, is_fitting=True,
-                 verbose=True):
+    def __init__(self, l, b, b_warm, n, buffer=None, N=150, accuracy=1e-6, dtype="c16", verbose=False):
 
         """
-        Численный расчет СМО M/Ph/n с абсолютным приоритетом на основе аппроксимации периодов непрерывной занятости
-        l_L, l_H: интенсивности вх. потока заявок с низким и высоким приоритетами
-        mu_L: интенсивность обслуживания заявок с низким приоритетом,
-        mu1_H, mu2_H, p_H: параметры Cox2 (H2) - распределения для заявок высокого класса
+        n: число каналов
+        l: интенсивность вх. потока
+        b: начальные моменты времени обслуживания
+        b_warm: начальные моменты времени разогрева
         N: число ярусов
         accuracy: точность, параметр для остановки итерации
-        is_cox:
-            True -  для аппроксимации времени обслуживания заявок первого класса используется
-                    распределение Кокса 2-го порядка,
-            False - гиперэкспоненциальное распределение 2-го порядка H2
-        """
-        # self.dt = np.dtype("f8")
-        self.dt = np.dtype("c16")
-        self.n = n  # количество каналов
-        self.N = N
+        """
+        self.dt = np.dtype(dtype)
+        if buffer:
+            self.R = buffer + n  # максимальное число заявок в сисетеме - очередь + каналы
+            self.N = self.R + 1  # число ярусов на один больше + нулевое состояние
+        else:
+            self.N = N
+            self.R = None  # для проверки задан ли буфер
+
         self.e1 = accuracy
-        self.l_L = l_L
-        self.l_H = l_H
-        self.mu_L = mu_L
-        self.mu1_H = mu1_H
-        self.mu2_H = mu2_H
-        self.p_H = p_H
-        self.max_iter = max_iter
-        self.is_cox = is_cox
+        self.n = n
+        self.b = b
         self.verbose = verbose
-        self.approx_ee = approx_ee
-        self.approx_e = approx_e
-        self.is_fitting = is_fitting
-
-        self.busy_periods = []  # список из наборов начальных моментров ПНЗ B1, B2, ...
-        self.busy_periods_coevs = []  # коэффициенты вариации ПНЗ
-        self.alphas = []
-        self.pp = []  # список из вероятностей переходов в ПНЗ
+        self.l = l
 
-        self.calc_busy_periods()
+        if self.dt == 'c16':
+            h2_params_service = rd.H2_dist.get_params_clx(b)
+        else:
+            h2_params_service = rd.H2_dist.get_params(b)
+
+        # параметры H2-распределения:
+        self.y = [h2_params_service[0], 1.0 - h2_params_service[0]]
+        self.mu = [h2_params_service[1], h2_params_service[2]]
+
+        self.b_warm = b_warm
+        if self.dt == 'c16':
+            h2_params_warm = rd.H2_dist.get_params_clx(b_warm)
+        else:
+            h2_params_warm = rd.H2_dist.get_params(b_warm)
+        self.y_w = [h2_params_warm[0], 1.0 - h2_params_warm[0]]
+        self.mu_w = [h2_params_warm[1], h2_params_warm[2]]
 
         # массив cols хранит число столбцов для каждого яруса, удобней рассчитать его один раз:
         self.cols = [] * N
 
         # переменные
         self.t = []
         self.b1 = []
         self.b2 = []
-        self.x = [0.0 + 0.0j] * N
-        self.z = [0.0 + 0.0j] * N
+        if self.dt == 'c16':
+            self.x = [0.0 + 0.0j] * N
+            self.z = [0.0 + 0.0j] * N
 
-        # искомые вреоятности состояний СМО
-        self.p = [0.0 + 0.0j] * N
+            # искомые вреоятности состояний СМО
+            self.p = [0.0 + 0.0j] * N
+        else:
+            self.x = [0.0] * N
+            self.z = [0.0] * N
+
+            # искомые вреоятности состояний СМО
+            self.p = [0.0] * N
 
         # матрицы переходов
         self.A = []
         self.B = []
         self.C = []
         self.D = []
         self.Y = []
 
-        # cols зависит от числа каналов. cols = количество всех микросостояний переходов для Cox2 до яруса
-        # с номером N-1 + число ПНЗ * 2. Число ПНЗ = n**2
-        self.cols_length_ = 2 * self.n ** 2
-        for i in range(self.n):
-            self.cols_length_ += i + 1
-
         for i in range(N):
-            self.t.append(np.zeros((1, self.cols_length_), dtype=self.dt))
-            self.b1.append(np.zeros((1, self.cols_length_), dtype=self.dt))
-            self.b2.append(np.zeros((1, self.cols_length_), dtype=self.dt))
-            self.x.append(np.zeros((1, self.cols_length_), dtype=self.dt))
+            if i < n + 1:
+                if i == 0:
+                    self.cols.append(1)  # 00 state
+                else:
+                    self.cols.append(3 * i + 1)  # w1 w2 01 10
+            else:
+                self.cols.append(3 * n + 1)
+
+            self.t.append(np.zeros((1, self.cols[i]), dtype=self.dt))
+            self.b1.append(np.zeros((1, self.cols[i]), dtype=self.dt))
+            self.b2.append(np.zeros((1, self.cols[i]), dtype=self.dt))
+            self.x.append(np.zeros((1, self.cols[i]), dtype=self.dt))
 
         self.build_matrices()
         self.initial_probabilities()
 
-    def build_A_for_busy_periods(self, num):
+    def get_p(self):
         """
-            Формирует матрицу А(L) для расчета ПНЗ по заданному номеру яруса
-            num - номер яруса
+        Возвращает список с вероятностями состояний системы
+        p[k] - вероятность пребывания в системе ровно k заявок
         """
-        if num < self.n:
-            col = num + 2
-            row = num + 1
-        elif num == self.n:
-            col = num + 1
-            row = num + 1
-        else:
-            output = self.A_for_busy[self.n]
-            return output
-
-        output = np.zeros((row, col), dtype=self.dt)
-
-        for i in range(row):
-            output[i, i] = self.l_H
-        return output
+        for i in range(len(self.p)):
+            self.p[i] = self.p[i].real
+        return self.p
 
-    def build_B_for_busy_periods(self, num):
+    def get_w(self):
         """
-            Формирует матрицу B(num) для расчета ПНЗ  по заданному номеру яруса
-            num - номер яруса
+        Возвращает три первых начальных момента времени ожидания в СМО
         """
-        if num == 0:
-            output = np.zeros((1, 1), dtype=self.dt)
-            return output
-        elif num <= self.n:
-            col = num
-            row = num + 1
-        elif num == self.n + 1:
-            col = num
-            row = num
-            output = np.zeros((row, col), dtype=self.dt)
-            output[:, :self.n] = self.B_for_busy[self.n]
-            return output
-        else:
-            output = self.B_for_busy[self.n + 1]
-            return output
-
-        output = np.zeros((row, col), dtype=self.dt)
-
-        mu1 = self.mu1_H
-        mu2 = self.mu2_H
-        qH = 1.0 - self.p_H
-
-        for i in range(col):
-            output[i, i] = (num - i) * mu1 * qH
-            output[i + 1, i] = (i + 1) * mu2
-        return output
+        w = [0.0] * 3
 
-    def build_C_for_busy_periods(self, num):
-        """
-            Формирует матрицу C(num) для расчета ПНЗ по заданному номеру яруса
-            num - номер яруса
-        """
-        if num == 0:
-            output = np.zeros((1, 1), dtype=self.dt)
-            return output
-        elif num <= self.n:
-            col = num + 1
-            row = num + 1
-        else:
-            output = self.C_for_busy[self.n]
-            return output
+        for j in range(1, len(self.p) - self.n):
+            w[0] += j * self.p[self.n + j]
+        for j in range(2, len(self.p) - self.n):
+            w[1] += j * (j - 1) * self.p[self.n + j]
+        for j in range(3, len(self.p) - self.n):
+            w[2] += j * (j - 1) * (j - 2) * self.p[self.n + j]
 
-        output = np.zeros((row, col), dtype=self.dt)
+        for j in range(3):
+            w[j] /= math.pow(self.l, j + 1)
+            w[j] = w[j].real
 
-        mu1 = self.mu1_H
-        pH = self.p_H
+        return w
 
-        for i in range(col - 1):
-            output[i, i + 1] = (num - i) * mu1 * pH
-        return output
+    def get_b(self):
+        b_plus_b_warm = [0.0]*3
+        for i in range(3):
+            b_plus_b_warm[i] = self.b[i] * (1.0 - self.p[0]) + self.p[0] * self.b_warm[i]
+        return b_plus_b_warm
 
-    def build_D_for_busy_periods(self, num):
+    def get_v(self):
         """
-            Формирует матрицу D для ПНЗ по заданному номеру яруса num
+        Возвращает три первых начальных момента времени пребывания в СМО
         """
-        if num <= self.n:
-            col = num + 1
-            row = num + 1
-        else:
-            output = self.D_for_busy[self.n]
-            return output
-
-        output = np.zeros((row, col), dtype=self.dt)
+        v = [0.0] * 3
+        w = self.get_w()
+        b = self.get_b()
+        v[0] = w[0] + b[0]
+        v[1] = w[1] + 2 * w[0] * b[0] + b[1]
+        v[2] = w[2] + 3 * w[1] * b[0] + 3 * w[0] * b[1] + b[2]
 
-        for i in range(row):
-            sumA = 0.0 + 0.0j
-            sumB = 0.0 + 0.0j
-            sumC = 0.0 + 0.0j
-
-            for j in range(col):
-                sumA += self.A_for_busy[num][i, j]
+        return v
 
-            if num != 0:
-                for j in range(col - 1):
-                    sumB += self.B_for_busy[num][i, j]
+    def print_mrx(self, mrx):
+        row = mrx.shape[0]
+        col = mrx.shape[1]
 
+        for i in range(row):
             for j in range(col):
-                sumC += self.C_for_busy[num][i, j]
-
-            output[i, i] = sumA + sumB + sumC
-
-        return output
-
-    def calc_busy_periods(self):
-
-        self.A_for_busy = []
-        self.B_for_busy = []
-        self.C_for_busy = []
-        self.D_for_busy = []
-
-        for i in range(self.n + 2):
-            self.A_for_busy.append(self.build_A_for_busy_periods(i))
-            self.B_for_busy.append(self.build_B_for_busy_periods(i))
-            self.C_for_busy.append(self.build_C_for_busy_periods(i))
-            self.D_for_busy.append(self.build_D_for_busy_periods(i))
-
-        pass_time = passage_time.passage_time_calc(self.A_for_busy, self.B_for_busy,
-                                                   self.C_for_busy, self.D_for_busy, is_clx=True, is_verbose=True)
-        pass_time.calc()
-
-        self.pnz_num_ = self.n ** 2
-
-        for j in range(self.pnz_num_):
-            self.busy_periods.append([0, 0, 0])
-
-        num = 0
-        for i in range(self.n):
-            for j in range(self.n):
-                for r in range(3):
-                    self.busy_periods[num][r] = pass_time.Z[self.n][r][i, j]
-                num = num + 1
-
-        for j in range(self.pnz_num_):
-            under_sqrt = self.busy_periods[j][1] - self.busy_periods[j][0] ** 2
-            if under_sqrt > 0:
-                coev = math.sqrt(under_sqrt.real)
-                self.alphas.append(1 / (coev ** 2))
-                self.busy_periods_coevs.append(coev / self.busy_periods[j][0])
-            else:
-                self.busy_periods_coevs.append(math.inf)
-
-        if self.verbose:
-            print("\nПериоды НЗ:\n")
-            for j in range(self.pnz_num_):
-                for r in range(3):
-                    if math.isclose(self.busy_periods[j][r].imag, 0):
-                        print("{0:^8.3g}".format(self.busy_periods[j][r].real), end=" ")
-                    else:
-                        print("{0:^8.3g}".format(self.busy_periods[j][r]), end=" ")
-                if math.isclose(self.busy_periods_coevs[j].imag, 0):
-                    print("coev = {0:^4.3g}".format(self.busy_periods_coevs[j].real))
-                else:
-                    print("coev = {0:^4.3g}".format(self.busy_periods_coevs[j]))
-
-        # pp - список из n**2 вероятностей переходов
-        for j in range(self.pnz_num_):
-            num = 0
-            for i in range(self.n):
-                for j in range(self.n):
-                    self.pp.append(pass_time.G[self.n][i, j])
-                    num = num + 1
-        if self.verbose:
-            print("\nВероятности переходов в ПНЗ:\n")
-            for j in range(self.pnz_num_):
-                if math.isclose(self.pp[j].imag, 0):
-                    print("{0:^8.3g}".format(self.pp[j].real), end=" ")
+                if math.isclose(mrx[i, j].real, 0.0):
+                    print("{0:^5s} | ".format("     "), end="")
                 else:
-                    print("{0:^8.3g}".format(self.pp[j]), end=" ")
+                    print("{0:^5.3f} | ".format(mrx[i, j].real), end="")
+            print("\n" + "--------" * col)
 
-    def get_p(self):
-        """
-        Возвращает список с вероятностями состояний системы
-        p[k] - вероятность пребывания в системе ровно k заявок класса L
-        """
-        p_real = [0.0] * self.N
-        for i in range(len(self.p)):
-            p_real[i] = self.p[i].real
-        return p_real
-
-    def get_low_class_v1(self):
-        """
-        Возвращает среднее время пребывания для класса L
-        """
-        l1 = 0
-        p_real = self.get_p()
-        for i in range(self.N):
-            l1 += p_real[i] * i
-        return l1 / self.l_L
+    @staticmethod
+    def binom_calc(a, b, num=3):
+        res = []
+        if num > 0:
+            res.append(a + b)
+        if num > 1:
+            res.append(a[1] + 2 * a[0] * b[0] + b[1])
+        if num > 2:
+            res.append(a[2] + 3 * a[1] * b[0] + 3 * b[1] * a[0] + b[2])
+        return res
 
     def initial_probabilities(self):
         """
         Задаем первоначальные значения вероятностей микросостояний
         """
         # t задаем равновероятными
         for i in range(self.N):
-            for j in range(self.cols_length_):
-                self.t[i][0, j] = 1.0 / self.cols_length_
+            for j in range(self.cols[i]):
+                self.t[i][0, j] = 1.0 / self.cols[i]
         self.x[0] = 0.4
 
+    def norm_probs(self):
+        summ = 0
+        for i in range(self.N):
+            summ += self.p[i]
+
+        for i in range(self.N):
+            self.p[i] /= summ
+
+        if self.verbose:
+            summ = 0
+            for i in range(self.N):
+                summ += self.p[i]
+            print("Summ of probs = {0:.5f}".format(summ))
+
     def calculate_p(self):
         """
         После окончания итераций находим значения вероятностей p по найденным х
         """
         # version 1
-        p_sum = 0 + 0j
+        p_sum = 0
         p0_max = 1.0
         p0_min = 0.0
-        iter = 0
-        self.p_iteration_num_ = 0
-        while math.fabs(1.0 - p_sum.real) > 1e-6 and iter < self.max_iter:
-            iter += 1
+
+        while math.fabs(1.0 - p_sum) > 1e-6:
             p0_ = (p0_max + p0_min) / 2.0
             p_sum = p0_
             self.p[0] = p0_
             for j in range(self.N - 1):
-                self.p[j + 1] = np.dot(self.p[j], self.x[j])
+                self.p[j + 1] = self.p[j] * self.x[j]
                 p_sum += self.p[j + 1]
-            if p_sum.real > 1.0:
+
+            if (p_sum > 1.0):
                 p0_max = p0_
             else:
                 p0_min = p0_
-        self.p_iteration_num_ = iter
+
+        self.norm_probs()
 
     def calculate_y(self):
         for i in range(self.N):
             self.Y.append(np.dot(self.p[i], self.t[i]))
 
     def build_matrices(self):
         """
@@ -325,101 +224,136 @@
         """
         for i in range(self.N):
             self.A.append(self.buildA(i))
             self.B.append(self.buildB(i))
             self.C.append(self.buildC(i))
             self.D.append(self.buildD(i))
 
+        # self.calc_G_passage()
+
+    def calc_g_matrices(self):
+        self.G = []
+        for j in range(0, self.N):
+            self.G.append(np.linalg.inv(self.D[j] - self.C[j]))
+
+    def calc_ag_matrices(self):
+        self.AG = [0]
+        for j in range(1, self.N):
+            self.AG.append(np.dot(self.A[j - 1], self.G[j]))
+
+    def calc_bg_matrices(self):
+        self.BG = [0]
+        for j in range(1, self.N):
+            if j != (self.N - 1):
+                self.BG.append(np.dot(self.B[j + 1], self.G[j]))
+            else:
+                self.BG.append(np.dot(self.B[j], self.G[j]))
+
+    def calc_support_matrices(self):
+        self.calc_g_matrices()
+        self.calc_ag_matrices()
+        self.calc_bg_matrices()
+
     def run(self):
         """
-        Запускает расчет. Алгоритм расчета не зависит от структуры матриц
+        Запускает расчет
         """
-        self.b1[0][0, 0] = 0.0 + 0.0j
-        self.b2[0][0, 0] = 0.0 + 0.0j
-        
-        is_ave = False
-
+        if self.dt == 'c16':
+            self.b1[0][0, 0] = 0.0 + 0.0j
+            self.b2[0][0, 0] = 0.0 + 0.0j
+            x_max1 = 0.0 + 0.0j
+            x_max2 = 0.0 + 0.0j
+        else:
+            self.b1[0][0, 0] = 0.0
+            self.b2[0][0, 0] = 0.0
+            x_max1 = 0.0
+            x_max2 = 0.0
 
+        self.calc_support_matrices()
 
-        iter = 0
-        self.run_iterations_num_ = 0
-        if is_ave:
-            x_ave1 = 0.0 + 0.0j
-            x_ave2 = 0.0 + 0.0j
-            for i in range(self.N):
-                x_ave1 += self.x[i]
-            x_ave1 /= self.N
-        else:
+        self.num_of_iter_ = 0  # кол-во итераций алгоритма
+        for i in range(self.N):
+            if self.x[i].real > x_max1.real:
+                x_max1 = self.x[i]
 
-            x_ave1 = 0.0
-            x_ave2 = 0.0
-            for i in range(self.N):
-                if self.x[i].real > x_ave1 :
-                    x_ave1 = self.x[i].real
+        while math.fabs(x_max2.real - x_max1.real) >= self.e1:
+            x_max2 = x_max1
+            self.num_of_iter_ += 1
 
-        while math.fabs(x_ave2.real - x_ave1.real) >= self.e1 and iter < self.max_iter:
-            if self.verbose:
-                print("Start numeric iteration {0:d}".format(iter))
-            iter += 1
-            x_ave2 = x_ave1
             for j in range(1, self.N):  # по всем ярусам, кроме первого.
 
-                G = np.linalg.inv(self.D[j] - self.C[j])
                 # b':
-                self.b1[j] = np.dot(self.t[j - 1], np.dot(self.A[j - 1], G))
+                self.b1[j] = np.dot(self.t[j - 1], self.AG[j])
 
                 # b":
                 if j != (self.N - 1):
-                    self.b2[j] = np.dot(self.t[j + 1], np.dot(self.B[j + 1], G))
+                    self.b2[j] = np.dot(self.t[j + 1], self.BG[j])
                 else:
-                    self.b2[j] = np.dot(self.t[j - 1], np.dot(self.B[j], G))
+                    self.b2[j] = np.dot(self.t[j - 1], self.BG[j])
 
                 c = self.calculate_c(j)
 
                 x_znam = np.dot(c, self.b1[j]) + self.b2[j]
-                self.x[j] = 0.0 + 0.0j
+                if self.dt == 'c16':
+                    self.x[j] = 0.0 + 0.0j
+                else:
+                    self.x[j] = 0.0
                 for k in range(x_znam.shape[1]):
                     self.x[j] += x_znam[0, k]
 
-                self.x[j] = 1.0 / self.x[j]
+                if self.dt == 'c16':
+                    self.x[j] = (1.0 + 0.0j) / self.x[j]
+                else:
+                    self.x[j] = (1.0) / self.x[j]
+
+                if self.R and j == (self.N - 1):
+                    tA = np.dot(self.t[j - 1], self.A[j - 1])
+                    tag = np.dot(tA, self.G[j])
+                    tag_sum = 0
+                    for t_i in range(tag.shape[1]):
+                        tag_sum += tag[0, t_i]
+                    self.z[j] = 1.0 / tag_sum
+                    self.t[j] = self.z[j] * tag
+
+                else:
 
-                self.z[j] = np.dot(c, self.x[j])
-                self.t[j] = np.dot(self.z[j], self.b1[j]) + np.dot(self.x[j], self.b2[j])
+                    self.z[j] = np.dot(c, self.x[j])
+                    self.t[j] = np.dot(self.z[j], self.b1[j]) + np.dot(self.x[j], self.b2[j])
 
-            self.x[0] = 1.0 / self.z[1]
+            if self.dt == 'c16':
+                self.x[0] = (1.0 + 0.0j) / self.z[1]
+            else:
+                self.x[0] = 1.0 / self.z[1]
 
             t1B1 = np.dot(self.t[1], self.B[1])
             self.t[0] = np.dot(self.x[0], t1B1)
-            self.t[0] = np.dot(self.t[0], np.linalg.inv(self.D[0] - self.C[0]))
-
+            self.t[0] = np.dot(self.t[0], self.G[0])
 
+            if self.dt == 'c16':
+                x_max1 = 0.0 + 0.0j
+            else:
+                x_max1 = 0
 
-            if is_ave:
-                x_ave1 = 0.0 + 0.0j
-                for i in range(self.N):
-                    x_ave1 += self.x[i]
-                x_ave1 /= self.N
+            for i in range(self.N):
+                if self.x[i].real > x_max1.real:
+                    x_max1 = self.x[i]
 
-            else:
-                x_ave1 = 0.0
-                for i in range(self.N):
-                    if self.x[i].real > x_ave1:
-                        x_ave1 = self.x[i].real
+            if self.verbose:
+                print("End iter # {0:d}".format(self.num_of_iter_))
 
-        self.run_iterations_num_ = iter
         self.calculate_p()
         self.calculate_y()
 
     def calculate_c(self, j):
         """
         Вычисляет значение переменной с, участвующей в расчете
         """
-        chisl = 0.0 + 0.0j
-        znam = 0.0 + 0.0j
-        znam2 = 0.0 + 0.0j
+        chisl = 0
+        znam = 0
+        znam2 = 0
 
         m = np.dot(self.b2[j], self.B[j])
         for k in range(m.shape[1]):
             chisl += m[0, k]
 
         m = np.dot(self.b1[j], self.B[j])
         for k in range(m.shape[1]):
@@ -427,362 +361,263 @@
 
         m = np.dot(self.t[j - 1], self.A[j - 1])
         for k in range(m.shape[1]):
             znam += m[0, k]
 
         return chisl / (znam - znam2)
 
-    def buildA(self, num):
+    def insert_standart_A_into(self, mass, l, y1, left_pos, bottom_pos, level):
+        row_num = level
+        for i in range(row_num):
+            mass[i + left_pos, i + bottom_pos] = l * y1
+            mass[i + left_pos, i + bottom_pos + 1] = l * (1.0 - y1)
+
+    def buildA(self, num, is_v_calc=False):
         """
-        Формирует матрицу А(L) по заданному номеру яруса num
+        Формирует матрицу А по заданному номеру яруса
         """
-        col = self.cols_length_
-        row = self.cols_length_
+        if num < self.n:
+            col = self.cols[num + 1]
+            row = self.cols[num]
+        else:
+            col = self.cols[self.n]
+            row = self.cols[self.n]
 
         output = np.zeros((row, col), dtype=self.dt)
-        if num > 1:
-            output = self.A[0]
+
+        if is_v_calc:
             return output
-        for i in range(row):
-            output[i, i] = self.l_L
+        if num > self.n:
+            output = self.A[self.n]
+            return output
+        if num == 0:
+            output[0, 0] = self.l * self.y_w[0]
+            output[0, 1] = self.l * self.y_w[1]
+        else:
+
+            if num < self.n:
+                # first block
+                self.insert_standart_A_into(output, self.l, self.y[0], 0, 0, level=num)
+                # second
+                self.insert_standart_A_into(output, self.l, self.y[0], num, num + 1, level=num)
+                # third
+                self.insert_standart_A_into(output, self.l, self.y[0], 2 * num, 2 * (num + 1), level=num + 1)
+            else:
+                for i in range(row):
+                    output[i, i] = self.l
+
         return output
 
+    def insert_standart_B_into(self, mass, y, mu, left_pos, bottom_pos, level, n):
+        col = level
+        for i in range(col):
+            if level <= n:
+                mass[i + left_pos, i + bottom_pos] = (level - i) * mu[0]
+                mass[i + left_pos + 1, i + bottom_pos] = (i + 1) * mu[1]
+            else:
+                mass[i + left_pos, i + bottom_pos] = (level - i - 1) * mu[0] * y[0] + i * mu[1] * y[1]
+                if i != level - 1:
+                    mass[i + left_pos, i + bottom_pos + 1] = (level - i - 1) * mu[0] * y[1]
+                if i != level - 1:
+                    mass[i + + left_pos + 1, i + bottom_pos] = (i + 1) * mu[1] * y[0]
+
     def buildB(self, num):
         """
             Формирует матрицу B по заданному номеру яруса
         """
         if num == 0:
             return np.zeros((1, 1), dtype=self.dt)
 
-        col = self.cols_length_
-        row = self.cols_length_
-        output = np.zeros((row, col), dtype=self.dt)
+        if num <= self.n:
 
-        if num > self.n:
-            output = self.B[self.n]
+            col = self.cols[num - 1]
+            row = self.cols[num]
+        else:
+            col = self.cols[self.n + 1]
+            row = self.cols[self.n + 1]
+
+        output = np.zeros((row, col), dtype=self.dt)
+        if num > self.n + 1:
+            output = self.B[self.n + 1]
             return output
 
-        # Матрица B - диагональная. Количество ненулевых элементов зависит от числа n.
-        lev = 0
-        for i in range(self.n):  # количество ярусов до перехода в ПНЗ
-            for j in range(i + 1):  # количество микросочтояний в этом ярусе
-                output[lev, lev] = min(self.n - i, num) * self.mu_L
-                lev = lev + 1
+        if num == 1:
+            output[0, 0] = self.mu_w[0]
+            output[1, 0] = self.mu_w[1]
+            output[2, 0] = self.mu[0]
+            output[3, 0] = self.mu[1]
+        else:
+
+            if num < self.n + 1:
+                # first block
+                self.insert_standart_B_into(output, self.y, self.mu, 0, 0, num - 1, self.n)
+                # second
+                self.insert_standart_B_into(output, self.y, self.mu, num, num - 1, num - 1, self.n)
+                # third
+                self.insert_standart_B_into(output, self.y, self.mu, 2 * num, 2 * (num - 1), num, self.n)
+
+                # warm block 1
+                for i in range(num):
+                    output[i, i + 2 * (num - 1)] = self.mu_w[0]
+
+                # warm block 2
+                for i in range(num):
+                    output[i + num, i + 2 * (num - 1)] = self.mu_w[1]
+
+            else:
+                # first block
+                self.insert_standart_B_into(output, self.y, self.mu, 0, 0, num - 1, self.n - 1)
+                # second
+                self.insert_standart_B_into(output, self.y, self.mu, num - 1, num - 1, num - 1, self.n - 1)
+                # third
+                self.insert_standart_B_into(output, self.y, self.mu, 2 * (num - 1), 2 * (num - 1), num, self.n)
+
+                # warm block 1
+                for i in range(num - 1):
+                    output[i, i + 2 * (num - 1)] = self.mu_w[0] * self.y[0]
+                    output[i, i + 2 * (num - 1) + 1] = self.mu_w[0] * self.y[1]
+
+                # warm block 2
+                for i in range(num - 1):
+                    output[i + num - 1, i + 2 * (num - 1)] = self.mu_w[1] * self.y[0]
+                    output[i + num - 1, i + 2 * (num - 1) + 1] = self.mu_w[1] * self.y[1]
 
         return output
 
     def buildC(self, num):
         """
             Формирует матрицу C по заданному номеру яруса
         """
-        col = self.cols_length_
-        row = col
+        if num < self.n:
+            col = self.cols[num]
+            row = col
+        else:
+            col = self.cols[self.n]
+            row = col
 
         output = np.zeros((row, col), dtype=self.dt)
-        if num >= 1:
-            output = self.C[0]
+        if num > self.n:
+            output = self.C[self.n]
             return output
 
-        lh = self.l_H
-
-        y1_mass = []
-        m1_mass = []
-        m2_mass = []
-        print("\n")
-
-        for i in range(self.pnz_num_):
-            if not self.is_cox:
-                h2_param = rd.H2_dist.get_params_clx(self.busy_periods[i], ee=self.approx_ee, e=self.approx_e, is_fitting=self.is_fitting)
-                # h2_param = rd.H2_dist.get_params(self.busy_periods[i])
-                y1_mass.append(h2_param[0])
-                m1_mass.append(h2_param[1])
-                m2_mass.append(h2_param[2])
-                if self.verbose:
-                    print("Параметры для B{0}: {1:3.3f}, {2:3.3f}, {3:3.3f}".format(i + 1, h2_param[0], h2_param[1],
-                                                                                    h2_param[2]))
-            else:
-                cox_params = rd.Cox_dist.get_params(self.busy_periods[i], ee=self.approx_ee, e=self.approx_e, is_fitting=self.is_fitting)
-                y1_mass.append(cox_params[0])
-                m1_mass.append(cox_params[1])
-                m2_mass.append(cox_params[2])
-                if self.verbose:
-                    print("Параметры для B{0}: {1:3.3f}, {2:3.3f}, {3:3.3f}".format(i + 1, cox_params[0], cox_params[1],
-                                                                                    cox_params[2]))
-
-        # first quad
-
-        # lH's = A_for_busy. Но поскольку = l_h, проще здесь посчитать заново
-        l_start = 0
-        for i in range(self.n - 1):
-            for j in range(i + 1):
-                output[l_start + j, l_start + j + i + 1] = lh
-            l_start += i + 1
-
-        # B_for_busy
-        l_start = 1
-        l_end = 0
-        for i in range(1, self.n):
-            rows = self.B_for_busy[i].shape[0]
-            cols = self.B_for_busy[i].shape[1]
-            for r in range(rows):
-                for c in range(cols):
-                    output[l_start + r, l_end + c] = self.B_for_busy[i][r, c]
-            l_start += i + 1
-            l_end += i
-
-        # C_for_busy
-        l_start = 1
-        for i in range(1, self.n):
-            rows = self.C_for_busy[i].shape[0]
-            cols = self.C_for_busy[i].shape[1]
-            for r in range(rows):
-                for c in range(cols):
-                    output[l_start + r, l_start + c] = self.C_for_busy[i][r, c]
-            l_start += i + 1
-
-        l_start = 0
-        for i in range(self.n - 1):
-            l_start += i + 1
-
-        l_end = l_start + self.n
-        num = 0
-        for i in range(self.n):
-            for j in range(self.n):
-                if not self.is_cox:
-                    output[l_start + i, l_end] = lh * y1_mass[num] * self.pp[num]
-                    output[l_start + i, l_end + 1] = lh * (1 - y1_mass[num]) * self.pp[num]
-                else:
-                    output[l_start + i, l_end] = lh * self.pp[num]
-                    output[l_start + i, l_end + 1] = 0
-                l_end += 2
-                num += 1
-
-        # left t's blocks
-        row = 0
-        for i in range(self.n):
-            row += i + 1
-
-        col = 0
-        for i in range(self.n - 1):
-            col += i + 1
-        num = 0
-        for i in range(self.n):
-            for j in range(self.n):
-                if not self.is_cox:
-                    output[row, col + j] = m1_mass[num]
-                    output[row + 1, col + j] = m2_mass[num]
-                else:
-                    output[row, col + j] = m1_mass[num] * (1.0 - y1_mass[num])
-                    output[row + 1, col + j] = m2_mass[num]
-                row += 2
-                num += 1
-
-        if self.is_cox:
-            # central T's block
-            row = 0
-            for i in range(self.n):
-                row += i + 1
-
-            col = 0
-            for i in range(self.n):
-                col += i + 1
-            num = 0
-            for i in range(self.n):
-                for j in range(self.n):
-                    output[row, col + 1] = m1_mass[num] * y1_mass[num]
-                    num += 1
-                    row += 2
-                    col += 2
         return output
 
-    def print_mrx(self, mrx, is_short=False):
-        row = mrx.shape[0]
-        col = mrx.shape[1]
-
-        for i in range(row):
-            for j in range(col):
-                if math.isclose(mrx[i, j].real, 0.0):
-                    if is_short:
-                        print("{0:^3s} | ".format(""), end="")
-                    else:
-                        print("{0:^5s} | ".format(""), end="")
-                else:
-                    if is_short:
-                        print("{0:^3.1f} | ".format(mrx[i, j].real), end="")
-                    else:
-                        print("{0:^5.3f} | ".format(mrx[i, j].real), end="")
-            if is_short:
-                print("\n" + "------" * col)
-            else:
-                print("\n" + "--------" * col)
-
-    def buildD(self, num):
+    def buildD(self, num, is_v_calc=False):
         """
             Формирует матрицу D по заданному номеру яруса
         """
-        col = self.cols_length_
-        row = col
+        if num < self.n:
+            col = self.cols[num]
+            row = col
+        else:
+            col = self.cols[self.n]
+            row = col
+
         output = np.zeros((row, col), dtype=self.dt)
 
         if num > self.n:
-            output = self.D[self.n]
+            if is_v_calc:
+                output = self.buildD(self.n, is_v_calc=True)
+            else:
+                output = self.D[self.n]
             return output
 
         for i in range(row):
-            sumA = 0.0 + 0.0j
-            sumB = 0.0 + 0.0j
-            sumC = 0.0 + 0.0j
+            if self.dt == 'c16':
+                sumA = 0.0 + 0.0j
+                sumB = 0.0 + 0.0j
+                sumC = 0.0 + 0.0j
+            else:
+                sumA = 0.0
+                sumB = 0.0
+                sumC = 0.0
 
-            for j in range(self.cols_length_):
+            for j in range(self.cols[num + 1]):
                 sumA += self.A[num][i, j]
 
             if num != 0:
-                for j in range(self.cols_length_):
+                for j in range(self.cols[num - 1]):
                     sumB += self.B[num][i, j]
 
-            for j in range(self.cols_length_):
+            for j in range(col):
                 sumC += self.C[num][i, j]
 
             output[i, i] = sumA + sumB + sumC
 
         return output
 
 
 if __name__ == "__main__":
-    from most_queue.sim import smo_im_prty
-    from most_queue.sim import rand_destribution as rd
-    import prty_calc
+
+    from sim import smo_im
+    from sim import rand_destribution as rd
     import time
 
-    num_of_jobs = 800000  # число обсл заявок ИМ
+    n = 3  # число каналов
+    l = 1.0  # интенсивность вх потока
+    ro = 0.7  # коэфф загрузки
+    b1 = n * 0.7  # ср время обслуживания
+    b1_warm = n * 0.9  # ср время разогрева
+    num_of_jobs = 1000000  # число обсл заявок ИМ
+    b_coev = [0.8, 1.5]  # коэфф вариации времени обсл
+    b_coev_warm = 1.2  # коэфф вариации времени разогрева
+    buff = None
+    verbose = False
+
+    for k in range(len(b_coev)):
+        b = [0.0] * 3
+        alpha = 1 / (b_coev[k] ** 2)
+        b[0] = b1
+        b[1] = math.pow(b[0], 2) * (math.pow(b_coev[k], 2) + 1)
+        b[2] = b[1] * b[0] * (1.0 + 2 / alpha)
+
+        b_w = [0.0] * 3
+        b_w[0] = b1_warm
+        alpha = 1 / (b_coev_warm ** 2)
+        b_w[1] = math.pow(b_w[0], 2) * (math.pow(b_coev_warm, 2) + 1)
+        b_w[2] = b_w[1] * b_w[0] * (1.0 + 2 / alpha)
 
-    is_cox = False  # использовать для аппроксимации ПНЗ распределение Кокса или Н2-распределение
-    max_iter = 100  # максимальное число итераций численного метода
-    # Исследование влияния среднего времени пребывания заявок 2-го класса от коэффициента загрузки
-    n = 4  # количество каналов
-    K = 2  # количество классов
-    ros = 0.75  # коэффициент загрузки СМО
-    bH_to_bL = 2  # время обслуживания класса H меньше L в это число раз
-    lH_to_lL = 1.5  # интенсивность поступления заявок класса H ниже L в это число раз
-    l_H = 1.0  # интенсивность вх потока заявок 1-го класса
-    l_L = lH_to_lL * l_H  # интенсивность вх потока заявок 2-го класса
-    bH_coev = [0.32, 0.63, 0.85, 1.2, 1.5]  # исследуемые коэффициенты вариации обсл заявок 1 класса
-    iteration = 1  # кол-во итераций ИМ для получения более точных оценок ИМ
-
-    v1_im_mass = []
-    v2_im_mass = []
-    v2_tt_mass = []
-    iter_num = []
-    tt_times = []
-    im_times = []
-    invar_times = []
-    v2_invar_mass = []
-
-    for k in range(len(bH_coev)):
-
-        print("coev =  {0:5.3f}".format(bH_coev[k]))
-
-        lsum = l_L + l_H
-        bsr = n * ros / lsum
-        bH1 = lsum * bsr / (l_L * bH_to_bL + l_H)
-        bL1 = bH_to_bL * bH1
-        bH = [0.0] * 3
-        alpha = 1 / (bH_coev[k] ** 2)
-        bH[0] = bH1
-        bH[1] = math.pow(bH[0], 2) * (math.pow(bH_coev[k], 2) + 1)
-        bH[2] = bH[1] * bH[0] * (1.0 + 2 / alpha)
-
-        gamma_params = rd.Gamma.get_mu_alpha([bH[0], bH[1]])
-
-        mu_L = 1.0 / bL1
-
-        # задание ИМ:
-        v1_sum = 0
-        v2_sum = 0
+        h2_params = rd.H2_dist.get_params_clx(b)
 
-        cox_params = rd.Cox_dist.get_params(bH)
+        im_start = time.process_time()
+        smo = smo_im.SmoIm(n, buffer=buff)
+        smo.set_sources(l, 'M')
+
+        gamma_params = rd.Gamma.get_mu_alpha(b)
+        gamma_params_warm = rd.Gamma.get_mu_alpha(b_w)
+        smo.set_servers(gamma_params, 'Gamma')
+        smo.set_warm(gamma_params_warm, 'Gamma')
+        smo.run(num_of_jobs)
+        p = smo.get_p()
+        v_im = smo.v
+        im_time = time.process_time() - im_start
 
-        # расчет численным методом:
         tt_start = time.process_time()
-        tt = m_ph_n_prty(mu_L, cox_params[1], cox_params[2], cox_params[0], l_L, l_H, n=n, is_cox=is_cox, max_iter=max_iter)
-        tt.run()
-        tt_times.append(time.process_time() - tt_start)
+        tt = Mh2h2Warm(l, b, b_w, n, buffer=buff, verbose=verbose)
 
-        iter_num.append(tt.run_iterations_num_)
+        tt.run()
         p_tt = tt.get_p()
-        v_tt = tt.get_low_class_v1()
-        v2_tt_mass.append(v_tt)
-        print("{0:^25s}".format("Вероятности состояний для заявок 2-го класса"))
+        v_tt = tt.get_v()
+        tt_time = time.process_time() - tt_start
+        num_of_iter = tt.num_of_iter_
+
+        print("\nСравнение результатов расчета методом Такахаси-Таками и ИМ.\n"
+              "ИМ - M/Gamma/{0:^2d}\nТакахаси-Таками - M/H2/{0:^2d}"
+              "с комплексными параметрами\n"
+              "Коэффициент загрузки: {1:^1.2f}".format(n, ro))
+        print(f'Коэффициент вариации времени обслуживания {b_coev[k]:0.3f}')
+        print(f'Коэффициент вариации времени разогрева {b_coev_warm:0.3f}')
+        print("Количество итераций алгоритма Такахаси-Таками: {0:^4d}".format(num_of_iter))
+        print("Время работы алгоритма Такахаси-Таками: {0:^5.3f} c".format(tt_time))
+        print("Время ИМ: {0:^5.3f} c".format(im_time))
+        print("{0:^25s}".format("Первые 10 вероятностей состояний СМО"))
         print("{0:^3s}|{1:^15s}|{2:^15s}".format("№", "Числ", "ИМ"))
         print("-" * 32)
         for i in range(11):
-            print("{0:^4d}|{1:^15.3g}|{2:^15.3g}".format(i, p_tt[i], 0))
-        print("{0:^15.3f}|{1:^15.6g}|{2:^15.6g}|{3:^15d}".format(bH_coev[k], v2_tt_mass[k], 0, iter_num[k]))
-
-        mu_L = 1.0 / bL1
+            print("{0:^4d}|{1:^15.3g}|{2:^15.3g}".format(i, p_tt[i], p[i]))
 
-        bL = rd.Exp_dist.calc_theory_moments(mu_L, 3)
-
-        b = []
-        b.append(bH)
-        b.append(bL)
-
-        L = [l_H, l_L]
-
-        invar_start = time.process_time()
-        v = prty_calc.get_v_prty_invar(L, b, n=n, type='PR', num=2)
-        v2_invar_mass.append(v[1][0])
-        invar_times.append(time.process_time() - invar_start)
-
-        im_start = time.process_time()
-
-        for i in range(iteration):
-            print("Start IM iteration: {0:d}".format(i + 1))
-
-            smo = smo_im_prty.SmoImPrty(n, K, "PR")
-            sources = []
-            servers_params = []
-            l = [l_H, l_L]
-
-            sources.append({'type': 'M', 'params': l_H})
-            sources.append({'type': 'M', 'params': l_L})
-            servers_params.append({'type': 'Gamma', 'params': gamma_params})
-            servers_params.append({'type': 'M', 'params': mu_L})
-
-            smo.set_sources(sources)
-            smo.set_servers(servers_params)
-
-            # запуск ИМ:
-            smo.run(num_of_jobs)
-
-            # получение результатов ИМ:
-            p = smo.get_p()
-            v_im = smo.v
-            v1_sum += v_im[0][0]
-            v2_sum += v_im[1][0]
-
-        v1 = v1_sum / iteration
-        v2 = v2_sum / iteration
-        # расчет численным методом:
-        v2_im_mass.append(v2)
-        im_times.append(time.process_time() - im_start)
-
-    print("\nСравнение результатов расчета численным методом с аппроксимацией ПНЗ "
-          "\nраспределением Кокса второго порядка и ИМ.")
-    print("ro: {0:1.2f}".format(ros))
-    print("n : {0:d}".format(n))
-    print("Количество обслуженных заявок для ИМ: {0:d}\n".format(num_of_jobs))
-
-    print("\n")
-    print("{0:^35s}".format("Средние времена пребывания в СМО для заявок 2-го класса"))
-    print("-" * 128)
-    print("{0:^15s}|{1:^15s}|{5:^15s}|{2:^15s}|{3:^15s}|{5:^15s}|{4:^15s}|{5:^15s}".format("coev", "Числ",
-                                                                                           "Кол-во итер алг", "ИМ",
-                                                                                           "Инвар", "t, c"))
-    print("-" * 128)
-    for k in range(len(bH_coev)):
-        print("{0:^15.3f}|{1:^15.6g}|{2:^15.6g}|{3:^15d}|{4:^15.6g}|{5:^15.6g}|{6:^15.6g}|{7:^15.6g}".format(
-            bH_coev[k],
-            v2_tt_mass[k], tt_times[k], iter_num[k],
-            v2_im_mass[k], im_times[k],
-            v2_invar_mass[k], invar_times[k]
-        ))
+        print("\n")
+        print("{0:^25s}".format("Начальные моменты времени ожидания в СМО"))
+        print("{0:^3s}|{1:^15s}|{2:^15s}".format("№", "Числ", "ИМ"))
+        print("-" * 32)
+        for i in range(3):
+            print("{0:^4d}|{1:^15.3g}|{2:^15.3g}".format(i + 1, v_tt[i], v_im[i]))
```

### Comparing `most_queue-1.20/most_queue/theory/mg1_calc.py` & `most_queue-1.3/most_queue/theory/mg1_calc.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import math
 from most_queue.sim import rand_destribution as rd
 from most_queue.sim import smo_im
-import q_poisson_arrival_calc as q_calc
+from most_queue.theory import q_poisson_arrival_calc as q_calc
 
 
 def get_w(l, b, num=3):
     """
     Расчет начальных моментов времени ожидания для СМО M/G/1
     :param l: интенсивность поступления заявок в СМО
     :param b: нач. моменты времени обслуживания
@@ -73,16 +73,14 @@
         for j in range(1, i):
             summ += p[j] * q[i - j]
         p[i] = (p[i - 1] - p[0] * q[i - 1] - summ) / q[0]
     return p
 
 
 if __name__ == '__main__':
-    from most_queue.utils.tables import times_print, probs_print
-
     l = 1
     b1 = 0.9
     coev = 1.6
     num_of_jobs = 800000
 
     params = rd.H2_dist.get_params_by_mean_and_coev(b1, coev)
     b = rd.H2_dist.calc_theory_moments(*params, 4)
@@ -92,58 +90,100 @@
     smo = smo_im.SmoIm(1)
     smo.set_servers(params, "H")
     smo.set_sources(l, "M")
     smo.run(num_of_jobs)
     w_im = smo.w
     p_im = smo.get_p()
 
-    times_print(w_im, w_ch, True)
+    print("\nH2. Значения начальных моментов времени ожидания заявок в системе:\n")
+
+    print("{0:^15s}|{1:^15s}|{2:^15s}".format("№ момента", "Числ", "ИМ"))
+    print("-" * 45)
+    for j in range(3):
+        print("{0:^16d}|{1:^15.5g}|{2:^15.5g}".format(j + 1, w_ch[j], w_im[j]))
 
     v_ch = get_v(l, b)
     v_im = smo.v
 
-    times_print(v_im, v_ch, False)
+    print("\nЗначения начальных моментов времени пребывания заявок в системе:\n")
 
-    probs_print(p_im, p_ch, 10)
+    print("{0:^15s}|{1:^15s}|{2:^15s}".format("№ момента", "Числ", "ИМ"))
+    print("-" * 45)
+    for j in range(3):
+        print("{0:^16d}|{1:^15.5g}|{2:^15.5g}".format(j + 1, v_ch[j], v_im[j]))
+
+    print("{0:^25s}".format("Вероятности состояний СМО"))
+    print("{0:^3s}|{1:^15s}|{2:^15s}".format("№", "Числ", "ИМ"))
+    print("-" * 32)
+    for i in range(11):
+        print("{0:^4d}|{1:^15.3g}|{2:^15.3g}".format(i, p_ch[i], p_im[i]))
 
     params = rd.Uniform_dist.get_params_by_mean_and_coev(b1, coev)
     b = rd.Uniform_dist.calc_theory_moments(*params, 4)
     w_ch = get_w(l, b)
     p_ch = get_p(l, b, 100, dist_type="Uniform")
 
     smo = smo_im.SmoIm(1)
     smo.set_servers(params, "Uniform")
     smo.set_sources(l, "M")
     smo.run(num_of_jobs)
     w_im = smo.w
     p_im = smo.get_p()
 
-    times_print(w_im, w_ch, True)
+    print("\nUniform. Значения начальных моментов времени ожидания заявок в системе:\n")
+
+    print("{0:^15s}|{1:^15s}|{2:^15s}".format("№ момента", "Числ", "ИМ"))
+    print("-" * 45)
+    for j in range(3):
+        print("{0:^16d}|{1:^15.5g}|{2:^15.5g}".format(j + 1, w_ch[j], w_im[j]))
 
     v_ch = get_v(l, b)
     v_im = smo.v
 
-    times_print(v_im, v_ch, False)
+    print("\nЗначения начальных моментов времени пребывания заявок в системе:\n")
 
-    probs_print(p_im, p_ch, 10)
+    print("{0:^15s}|{1:^15s}|{2:^15s}".format("№ момента", "Числ", "ИМ"))
+    print("-" * 45)
+    for j in range(3):
+        print("{0:^16d}|{1:^15.5g}|{2:^15.5g}".format(j + 1, v_ch[j], v_im[j]))
+
+    print("{0:^25s}".format("Вероятности состояний СМО"))
+    print("{0:^3s}|{1:^15s}|{2:^15s}".format("№", "Числ", "ИМ"))
+    print("-" * 32)
+    for i in range(11):
+        print("{0:^4d}|{1:^15.3g}|{2:^15.3g}".format(i, p_ch[i], p_im[i]))
 
     a, K = rd.Pareto_dist.get_a_k_by_mean_and_coev(b1, coev)
     b = rd.Pareto_dist.calc_theory_moments(a, K, 4)
     w_ch = get_w(l, b)
     p_ch = get_p(l, b, 100, dist_type="Pa")
 
     smo = smo_im.SmoIm(1)
     smo.set_servers([a, K], "Pa")
     smo.set_sources(l, "M")
     smo.run(num_of_jobs)
     w_im = smo.w
     p_im = smo.get_p()
 
-    times_print(w_im, w_ch, True)
+    print("\nPareto. Значения начальных моментов времени ожидания заявок в системе:\n")
+
+    print("{0:^15s}|{1:^15s}|{2:^15s}".format("№ момента", "Числ", "ИМ"))
+    print("-" * 45)
+    for j in range(len(w_ch)):
+        print("{0:^16d}|{1:^15.5g}|{2:^15.5g}".format(j + 1, w_ch[j], w_im[j]))
 
     v_ch = get_v(l, b)
     v_im = smo.v
 
-    times_print(v_im, v_ch, False)
+    print("\nЗначения начальных моментов времени пребывания заявок в системе:\n")
 
-    probs_print(p_im, p_ch, 10)
+    print("{0:^15s}|{1:^15s}|{2:^15s}".format("№ момента", "Числ", "ИМ"))
+    print("-" * 45)
+    for j in range(len(w_ch)):
+        print("{0:^16d}|{1:^15.5g}|{2:^15.5g}".format(j + 1, v_ch[j], v_im[j]))
+
+    print("{0:^25s}".format("Вероятности состояний СМО"))
+    print("{0:^3s}|{1:^15s}|{2:^15s}".format("№", "Числ", "ИМ"))
+    print("-" * 32)
+    for i in range(11):
+        print("{0:^4d}|{1:^15.3g}|{2:^15.3g}".format(i, p_ch[i], p_im[i]))
```

### Comparing `most_queue-1.20/most_queue/theory/mg1_warm_calc.py` & `most_queue-1.3/most_queue/theory/mg1_warm_calc.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from most_queue.sim import rand_destribution as rd
-from diff5dots import diff5dots
+from most_queue.theory.diff5dots import diff5dots
 from most_queue.sim import smo_im
 
 
 def get_v(l, b, b_warm):
     tv = b_warm[0] / (1 - l * b[0])
     p0_star = 1 / (1 + l * tv)
 
@@ -25,16 +25,14 @@
     v[0] = -v[0]
     v[2] = -v[2]
 
     return v
 
 
 if __name__ == '__main__':
-    from most_queue.utils.tables import times_print, probs_print
-
     l = 1
     b1 = 0.8
     b1_warm = 0.9
     coev = 1.3
     b_params = rd.H2_dist.get_params_by_mean_and_coev(b1, coev)
     b = rd.H2_dist.calc_theory_moments(*b_params, 4)
 
@@ -46,8 +44,13 @@
     smo.set_warm(b_warm_params, "H")
     smo.set_sources(l, "M")
     smo.run(100000)
 
     v_ch = get_v(l, b, b_warm)
     v_im = smo.v
 
-    times_print(v_im, v_ch, False)
+    print("\nЗначения начальных моментов времени пребывания заявок в системе:\n")
+
+    print("{0:^15s}|{1:^15s}|{2:^15s}".format("№ момента", "Числ", "ИМ"))
+    print("-" * 45)
+    for j in range(3):
+        print("{0:^16d}|{1:^15.5g}|{2:^15.5g}".format(j + 1, v_ch[j], v_im[j]))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `most_queue-1.20/most_queue/theory/mgn_tt.py` & `most_queue-1.3/most_queue/theory/mgn_tt.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 import math
+from most_queue.theory import passage_time
 from tqdm import tqdm
 from most_queue.sim import rand_destribution as rd
 
 
 class MGnCalc:
     """
     Расчет СМО M/H2/n с комплексными параметрами численным методом Такахаси-Таками.
@@ -108,14 +109,123 @@
         w = self.get_w()
         v[0] = w[0] + self.b[0]
         v[1] = w[1] + 2 * w[0] * self.b[0] + self.b[1]
         v[2] = w[2] + 3 * w[1] * self.b[0] + 3 * w[0] * self.b[1] + self.b[2]
 
         return v
 
+    def get_v_pt(self):
+        """
+        Нахождение высших моментов с помощью алгоритма Ньютса - passage_time
+
+        Согласно теореме PASTA (Poisson Arrivals See Time Averages) пребывающая заявка с вероятностью
+        p[№ яруса, № микрососояния] наблюдает систему в микросостоянии [№ яруса, № микрососояния] и переводит
+        ее в состояние на следующий ярус. Значит, необходимо пройтись по всем микросостояниям
+        [№ яруса, № микрососояния], соответствующие вероятности p[№ яруса, № микрососояния] умножить на сумму
+        вероятностей перехода в состояние [№+1 , № микрососояния] и время перехода из состояния
+        [№+1 , № микрососояния] на 0 ярус. Время перехода вычисляется с помощью алгоритма Ньютса,
+        реализованного в passage_time.py
+        """
+        A = []
+        B = []
+        C = []
+        D = []
+
+        for i in range(self.n + 2):
+            A.append(self.buildA(i, is_v_calc=True))
+            B.append(self.buildB(i))
+            C.append(self.buildC(i))
+            D.append(self.buildD(i, is_v_calc=True))
+
+        pt = passage_time.passage_time_calc(A, B, C, D)
+        pt.calc()
+
+        F = []
+        for num in range(self.n + 1):
+            if num < self.n:
+                col = self.cols[num + 1]
+                row = self.cols[num]
+            else:
+                col = self.cols[self.n]
+                row = self.cols[self.n]
+            output = np.matrix(np.zeros((row, col)), dtype=self.dt)
+
+            for i in range(row):
+                if num < self.n:
+                    output[i, i] = self.y[0]
+                    output[i, i + 1] = self.y[1]
+                else:
+                    output[i, i] = 1
+            F.append(output)
+
+        # Gr_gap = pt.Gr_gap_calc(1, 0)
+        # print("Gr gap mrx from {0:d} to {1:d}".format(1, 0))
+        # b = [0,0,0]
+        # for i in range(3):
+        #     b[i] += F[0][0, 0]*Gr_gap[i][0, 0] + F[0][0, 1]*Gr_gap[i][1, 0]
+        # print("Начальные моменты времени обслуживания b, вычисленные через passage time:")
+        # for i in range(3):
+        #     print("b[{0:d}] = {1:5.3f}".format(i + 1, b[i]))
+
+        # print("Y[0]:")
+        # self.print_mrx(self.Y[0])
+        # print("Y[1]:")
+        # self.print_mrx(self.Y[1])
+        #
+        # self.print_mrx(Gr_gap[0])
+        # Gr_gap = pt.Gr_gap_calc(3, 0)
+        # print("Gr gap mrx from {0:d} to {1:d}".format(3, 0))
+        # self.print_mrx(Gr_gap[0])
+        # Gr_gap = pt.Gr_gap_calc(5, 0)
+        # print("Gr gap mrx from {0:d} to {1:d}".format(5, 0))
+        # self.print_mrx(Gr_gap[0])
+
+        v = [0 + 0j, 0 + 0j, 0 + 0j]
+        print("Calc v")
+        v_old = 0
+        # inter_level_means = []
+        # inter_level_delta_means = []
+
+        for i in tqdm(range(0, self.N - 1)):
+            Zr_gap = pt.Gr_gap_calc(i + 1, 0)
+            # G_gap = pt.G_gap_calc(i+1, 0)
+            # inter_level_means.append(0)
+            # # for j in range(self.cols[i+1]):
+            # #     inter_level_means[i] += self.t[i+1][0, j] * Zr_gap[0][j, 0]
+            # # if i!=0:
+            # #     inter_level_delta_means.append(inter_level_means[i].real-inter_level_means[i-1].real)
+            # for j in range(self.cols[i+1]):
+            #     if i < pt.l_tilda-1:
+            #         inter_level_means[i] += pt.G[i+1][j, 0] * pt.Z[i+1][0][j, 0]
+            #     else:
+            #         inter_level_means[i] += pt.G[pt.l_tilda][j, 0] * pt.Z[pt.l_tilda][0][j, 0]
+            # формируем переходы из состояния [i, j] на ярус ниже
+            # G_gap = pt.G_gap_calc(i+1, 0) == 1, одно состояние
+            for j in range(self.cols[i]):
+                for k in range(self.cols[i + 1]):
+                    if i > self.n:
+                        v[0] = v[0] + F[self.n][j, k] * self.Y[i][0, j] * Zr_gap[0][k, 0]
+                        # v[0] = v[0] + self.Y[i][0, j] * Gr_gap[0][k, 0]
+                    else:
+                        v[0] = v[0] + F[i][j, k] * self.Y[i][0, j] * Zr_gap[0][k, 0]
+                        # v[0] = v[0] + self.Y[i][0, j] * Gr_gap[0][k, 0]
+                # if i >= pt.l_tilda:
+                #     v[0] = v[0] + self.Y[i][0, j] * Gr_gap[0][j, 0]
+                # else:
+                #     v[0] = v[0] + self.Y[i][0, j] * Gr_gap[0][j, 0]
+
+            v_new = v[0]
+            if math.fabs(v_new.real - v_old.real) < 1e-10:
+                print("Stop v calc at i = {0:d}".format(i))
+                break
+            v_old = v_new
+
+        # print(inter_level_means)
+
+        return v
 
     def print_mrx(self, mrx):
         row = mrx.shape[0]
         col = mrx.shape[1]
 
         for i in range(row):
             for j in range(col):
@@ -448,15 +558,14 @@
 
         return output
 
 
 if __name__ == "__main__":
     from most_queue.sim import smo_im
     from most_queue.sim import rand_destribution as rd
-    from most_queue.utils.tables import times_print, probs_print
     import time
 
     n = 3  # число каналов
     l = 1.0  # интенсивность вх потока
     ro = 0.8  # коэфф загрузки
     b1 = n * ro / l  # ср время обслуживания
     num_of_jobs = 1000000  # число обсл заявок ИМ
@@ -497,10 +606,19 @@
               "с комплексными параметрами\n"
               "Коэффициент загрузки: {1:^1.2f}\nКоэффициент вариации времени обслуживания: {2:^1.2f}\n".format(n, ro,
                                                                                                                b_coev[
                                                                                                                    k]))
         print("Количество итераций алгоритма Такахаси-Таками: {0:^4d}".format(num_of_iter))
         print("Время работы алгоритма Такахаси-Таками: {0:^5.3f} c".format(tt_time))
         print("Время работы ИМ: {0:^5.3f} c".format(im_time))
-        probs_print(p, p_tt, 10)
-
-        times_print(v_im, v_tt, False)
+        print("{0:^25s}".format("Первые 10 вероятностей состояний СМО"))
+        print("{0:^3s}|{1:^15s}|{2:^15s}".format("№", "Числ", "ИМ"))
+        print("-" * 32)
+        for i in range(11):
+            print("{0:^4d}|{1:^15.3g}|{2:^15.3g}".format(i, p_tt[i], p[i]))
+
+        print("\n")
+        print("{0:^25s}".format("Начальные моменты времени пребывания в СМО"))
+        print("{0:^3s}|{1:^15s}|{2:^15s}".format("№", "Числ", "ИМ"))
+        print("-" * 32)
+        for i in range(3):
+            print("{0:^4d}|{1:^15.3g}|{2:^15.3g}".format(i + 1, v_tt[i], v_im[i]))
```

### Comparing `most_queue-1.20/most_queue/theory/mmn3_pnz_cox_approx.py` & `most_queue-1.3/most_queue/theory/mmn3_pnz_cox_approx.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import numpy as np
 import math
-import prty_calc
-import passage_time
+from most_queue.theory import prty_calc
+from most_queue.theory import passage_time
 from most_queue.sim import rand_destribution as rd
-import math
 
 class Mmn3_pnz_cox:
     """
     Расчет СМО M/M/2 с 3-мя классами заявок, абсолютным приоритетом
     численным методом Такахаси-Таками на основе аппроксимации ПНЗ распределением Кокса второго порядка
     """
 
@@ -456,18 +455,17 @@
             output[i, i] = sumA + sumB + sumC
 
         return output
 
 
 if __name__ == "__main__":
     from most_queue.sim import smo_im_prty
-    import mmn_prty_pnz_approx
-    from mmnr_calc import M_M_n_formula
+    from most_queue.theory import mmn_prty_pnz_approx
+    from most_queue.theory.mmnr_calc import M_M_n_formula
     from most_queue.sim import rand_destribution as rd
-    from most_queue.utils.tables import times_print, probs_print
 
     num_of_jobs = 200000
     n = 2  # количество каналов
     K = 3  # количество классов
     mu_L = 1.3  # интенсивность обслуживания заявок 3-го класса
     mu_M = 1.4  # интенсивность обслуживания заявок 2-го класса
     mu_H = 1.5  # интенсивность обслуживания заявок 1-го класса
@@ -516,15 +514,18 @@
 
     print("\nСравнение результатов расчета численным методом с аппроксимацией ПНЗ "
           "\nраспределением Кокса второго порядка и ИМ.")
     print("Коэффициент загрузки: {0:^1.2f}".format(ro))
     print("Количество обслуженных заявок для ИМ: {0:d}\n".format(num_of_jobs))
 
     print("{0:^25s}".format("Вероятности состояний для заявок 3-го класса"))
-    probs_print(p[2], p_tt, 10)
+    print("{0:^3s}|{1:^15s}|{2:^15s}".format("№", "Числ", "ИМ"))
+    print("-" * 32)
+    for i in range(11):
+        print("{0:^4d}|{1:^15.3g}|{2:^15.3g}".format(i, p_tt[i], p[2][i]))
 
     print("\n")
     print("{0:^35s}".format("Средние времена пребывания в СМО"))
     print("-" * 38)
     print("{0:^10s}|{1:^15s}|{2:^15s}".format("N класса", "Числ", "ИМ"))
     print("-" * 38)
     print("{0:^10d}|{1:^15.3g}|{2:^15.3g}".format(0, v_1, v_im[0][0]))
```

### Comparing `most_queue-1.20/most_queue/theory/mmn_prty_pnz_approx.py` & `most_queue-1.3/most_queue/theory/mmn_prty_pnz_approx.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import math
 from most_queue.sim import rand_destribution as rd
-import passage_time
+from most_queue.theory import passage_time
 
 
 class MMn_PRTY_PNZ_Cox_approx:
     """
     Расчет СМО M/M/n с абсолютным приоритетом с комплексными параметрами численным методом Такахаси-Таками
     на основе аппроксимации ПНЗ распределением Кокса второго порядка
     Комплексные параметры позволяют аппроксимировать распределение времени обслуживания
@@ -596,16 +596,14 @@
 
         return output
 
 
 if __name__ == "__main__":
     from most_queue.sim import rand_destribution as rd
     from most_queue.sim import smo_im_prty
-    from most_queue.utils.tables import probs_print, times_print
-
 
     num_of_jobs = 100000
     n = 3  # количество каналов
     K = 2  # количество классов
     mu_L = 1.3  # интенсивность обслуживания заявок 2-го класса
     mu_H = 1.5  # интенсивность обслуживания заявок 1-го класса
     l_H = 1.0  # интенсивность вх потока заявок 1-го класса
@@ -645,15 +643,18 @@
 
     print("\nСравнение результатов расчета численным методом с аппроксимацией ПНЗ "
           "\nраспределением Кокса второго порядка и ИМ.")
     print("Коэффициент загрузки: {0:^1.2f}".format(ro))
     print("Количество обслуженных заявок для ИМ: {0:d}\n".format(num_of_jobs))
 
     print("{0:^25s}".format("Вероятности состояний для заявок 2-го класса"))
-    probs_print(p[1], p_tt, 10)
+    print("{0:^3s}|{1:^15s}|{2:^15s}".format("№", "Числ", "ИМ"))
+    print("-" * 32)
+    for i in range(11):
+        print("{0:^4d}|{1:^15.3g}|{2:^15.3g}".format(i, p_tt[i], p[1][i]))
 
     print("\n")
     print("{0:^25s}".format("Среднее время пребывания в СМО заявок 2-го класса"))
     print("{0:^15s}|{1:^15s}".format("Числ", "ИМ"))
     print("-" * 32)
     print("{0:^15.3g}|{1:^15.3g}".format(v_tt, v_im[1][0]))
     # print("{0:^15.3g}|{1:^15.3g}".format(v[0].real, v_im[1][0]))
```

### Comparing `most_queue-1.20/most_queue/theory/mmnr_calc.py` & `most_queue-1.3/most_queue/theory/mmnr_calc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import math
-import sv_sum_calc
+from most_queue.theory import sv_sum_calc
 from most_queue.sim import rand_destribution as rd
 
 class M_M_n_formula:
 
     @staticmethod
     def getPI(l, mu, n, r):
```

### Comparing `most_queue-1.20/most_queue/theory/network_calc.py` & `most_queue-1.3/most_queue/theory/network_calc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from diff5dots import diff5dots
-from most_queue.sim import rand_destribution as rd
-
 import numpy as np
 import math
-import prty_calc
+from most_queue.theory.diff5dots import diff5dots
+from most_queue.theory import prty_calc
+from most_queue.sim import rand_destribution as rd
 
 
 def balance_equation(L, R):
     rows = R.shape[0]
     cols = R.shape[1]
 
     # определяем нулевые строки и столбцы
```

### Comparing `most_queue-1.20/most_queue/theory/network_viewer.py` & `most_queue-1.3/most_queue/theory/network_viewer.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/theory/passage_time.py` & `most_queue-1.3/most_queue/theory/passage_time.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 import numpy as np
 import math
 import copy
 
 
 class passage_time_calc:
-    def __init__(self, A, B, C, D, is_clx=True, is_verbose=False, l_tilda=None):
+    def __init__(self, A, B, C, D, is_clx=True, is_verbose=False):
         self.A_input = A
         self.B_input = B
         self.C_input = C
         self.D_input = D
-        if not l_tilda:
-            self.l_tilda = len(D) - 1  # номер яруса, с которого все матрицы одинаковые
-        else:
-            self.l_tilda = l_tilda
+        self.l_tilda = len(D) - 1  # номер яруса, с которого все матрицы одинаковые
         self.e = 1e-9
         self.F = []
         self.Fr = []
         self.B = []
         self.Br = []
         self.L = []
         self.Lr = []
```

### Comparing `most_queue-1.20/most_queue/theory/prty_calc.py` & `most_queue-1.3/most_queue/theory/prty_calc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from most_queue.sim import rand_destribution as rd
-from diff5dots import diff5dots
-
-import mg1_calc
-import mgn_tt
 import math
+from most_queue.sim import rand_destribution as rd
+from most_queue.theory import mgn_tt
+from most_queue.theory.diff5dots import diff5dots
+from most_queue.theory import mg1_calc
 
 
 def get_w1_pr(l, b):
     """
     Расчет среднего времени ожидания в M/G/1 с абсолютным приоритетом
     :param l: [] - список интенсивностей для каждого класса заявок
     :param b: [k][j] - список начальных моментов для каждого класса
@@ -79,20 +78,20 @@
     z = 1 + l * pnz[0]
     if num > 1:
         pnz.append(b[1] / math.pow(1 - ro, 3))
     if num > 2:
         pnz.append(b[2] / math.pow(1 - ro, 4) + 3 * l * b[1] * b[1] / math.pow(1 - ro, 5))
     if num > 3:
         chisl = b[3] * math.pow(z, 4) + 6 * b[2] * l * pnz[1] * z * z + b[1] * (
-                3 * math.pow(l * pnz[1], 2) + 4 * l * pnz[2] * z)
+                    3 * math.pow(l * pnz[1], 2) + 4 * l * pnz[2] * z)
         pnz.append(chisl / (1 - ro))
     if num > 4:
         chisl = b[4] * math.pow(z, 5) + 10 * b[3] * l * pnz[1] * math.pow(z, 3) + \
                 b[2] * (15 * math.pow(l * pnz[1], 2) * z + 10 * l * pnz[2 * z * z]) + b[1] * (
-                        5 * l * pnz[3] * z + 10 * l * l * pnz[1] * pnz[2])
+                            5 * l * pnz[3] * z + 10 * l * l * pnz[1] * pnz[2])
         pnz.append(chisl / (1 - ro))
 
     return pnz
 
 
 def climov_w_pr_calc(l, b):
     # только два первых момента
```

### Comparing `most_queue-1.20/most_queue/theory/student_stat.py` & `most_queue-1.3/most_queue/theory/student_stat.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/theory/sv_sum_calc.py` & `most_queue-1.3/most_queue/theory/sv_sum_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/theory/weibull.py` & `most_queue-1.3/most_queue/theory/weibull.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/utils/approx_cdf_make.py` & `most_queue-1.3/most_queue/utils/approx_cdf_make.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/visualisation/smo_im_vis.py` & `most_queue-1.3/most_queue/visualisation/smo_im_vis.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/visualisation/utils/result_table.py` & `most_queue-1.3/most_queue/visualisation/utils/result_table.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/visualisation/utils/settings_window.py` & `most_queue-1.3/most_queue/visualisation/utils/settings_window.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/visualisation/utils/splash_screen.py` & `most_queue-1.3/most_queue/visualisation/utils/splash_screen.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue.egg-info/PKG-INFO` & `most_queue-1.3/most_queue.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: most-queue
-Version: 1.20
+Version: 1.3
 Summary: Software package for calculation and simulation of queuing systems
 Home-page: https://github.com/xabarov/mps
 Author: Xabarov Roman
 Author-email: Xabarov Roman <xabarov1985@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `most_queue-1.20/most_queue.egg-info/SOURCES.txt` & `most_queue-1.3/most_queue.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 most_queue/tests/ek_d_n.py
 most_queue/tests/fj_calc.py
 most_queue/tests/fj_im.py
 most_queue/tests/flow_sum.py
 most_queue/tests/gi_m_1_calc.py
 most_queue/tests/gi_m_n_calc.py
 most_queue/tests/m_d_n_calc.py
-most_queue/tests/m_h2_h2warm.py
 most_queue/tests/m_ph_n_prty.py
 most_queue/tests/mg1_calc.py
 most_queue/tests/mg1_warm_calc.py
 most_queue/tests/mgn_tt.py
 most_queue/tests/mmn3_pnz_cox_approx.py
 most_queue/tests/mmn_prty_pnz_approx.py
 most_queue/tests/network_im_prty.py
@@ -66,16 +65,13 @@
 most_queue/theory/prty_calc.py
 most_queue/theory/q_poisson_arrival_calc.py
 most_queue/theory/student_stat.py
 most_queue/theory/sv_sum_calc.py
 most_queue/theory/weibull.py
 most_queue/utils/__init__.py
 most_queue/utils/approx_cdf_make.py
-most_queue/utils/binom_probs.py
-most_queue/utils/difstir.py
-most_queue/utils/tables.py
 most_queue/visualisation/__init__.py
 most_queue/visualisation/smo_im_vis.py
 most_queue/visualisation/utils/__init__.py
 most_queue/visualisation/utils/result_table.py
 most_queue/visualisation/utils/settings_window.py
 most_queue/visualisation/utils/splash_screen.py
```

### Comparing `most_queue-1.20/setup.py` & `most_queue-1.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name='most-queue',
-      version='1.20',
+      version='1.03',
       description="Software package for calculation and simulation of queuing systems",
       author='Xabarov Roman',
       author_email='xabarov1985@gmail.com',
       url='https://github.com/xabarov/mps',
       classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
@@ -22,12 +22,11 @@
             "pandas",
             "scipy",
             "tqdm",
             "tqdm-stubs",
             'PyQt5',
             'qt-material',
             'PySide2',
-            'networkx',
-            'colorama'
+            'networkx'
       ],
       include_package_data=True,
       zip_safe=False)
```

