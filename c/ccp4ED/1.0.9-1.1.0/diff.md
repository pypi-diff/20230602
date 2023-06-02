# Comparing `tmp/ccp4ED-1.0.9.tar.gz` & `tmp/ccp4ED-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccp4ED-1.0.9.tar", last modified: Tue Apr 26 00:02:06 2022, max compression
+gzip compressed data, was "ccp4ED-1.1.0.tar", last modified: Fri Jun  2 11:56:06 2023, max compression
```

## Comparing `ccp4ED-1.0.9.tar` & `ccp4ED-1.1.0.tar`

### file list

```diff
@@ -1,276 +1,281 @@
-drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2022-04-26 00:02:06.982049 ccp4ED-1.0.9/
--rw-rw-r--   0 tarik     (1001) tarik     (1001)      572 2022-02-12 10:36:17.000000 ccp4ED-1.0.9/.gitignore
-drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2022-04-26 00:02:06.926050 ccp4ED-1.0.9/EDutils/
--rw-rw-r--   0 tarik     (1001) tarik     (1001)       22 2021-07-06 22:27:03.000000 ccp4ED-1.0.9/EDutils/__init__.py
--rwxrwxr-x   0 tarik     (1001) tarik     (1001)     1516 2022-02-04 11:05:43.000000 ccp4ED-1.0.9/EDutils/convert_pets.sh
-drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2022-04-26 00:02:06.930050 ccp4ED-1.0.9/EDutils/data/
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     2509 2022-02-15 12:23:20.000000 ccp4ED-1.0.9/EDutils/data/viewer_df.pkl
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     1164 2022-02-15 12:23:20.000000 ccp4ED-1.0.9/EDutils/data/viewer_dict.pkl
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     5413 2022-02-07 12:30:50.000000 ccp4ED-1.0.9/EDutils/display.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)    39768 2022-02-15 12:53:28.000000 ccp4ED-1.0.9/EDutils/gui.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)    10148 2022-02-15 12:23:17.000000 ccp4ED-1.0.9/EDutils/gui_config.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)    28866 2022-04-19 07:20:22.000000 ccp4ED-1.0.9/EDutils/pets.py
--rwxrwxr-x   0 tarik     (1001) tarik     (1001)      589 2021-07-13 11:19:40.000000 ccp4ED-1.0.9/EDutils/pets_ref.sh
--rw-rw-r--   0 tarik     (1001) tarik     (1001)    18652 2022-01-25 13:18:42.000000 ccp4ED-1.0.9/EDutils/rotate_exp.py
-drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2022-04-26 00:02:06.930050 ccp4ED-1.0.9/EDutils/sandbox/
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     1942 2021-07-05 16:06:03.000000 ccp4ED-1.0.9/EDutils/sandbox/convert.py
--rwxrwxr-x   0 tarik     (1001) tarik     (1001)      939 2021-06-10 15:53:10.000000 ccp4ED-1.0.9/EDutils/sandbox/test.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)    16657 2022-04-25 22:37:20.000000 ccp4ED-1.0.9/EDutils/utilities.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)    16042 2022-03-24 15:31:30.000000 ccp4ED-1.0.9/EDutils/viewers.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     4122 2022-04-26 00:02:06.982049 ccp4ED-1.0.9/PKG-INFO
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     3313 2022-04-25 08:58:12.000000 ccp4ED-1.0.9/README.md
-drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2022-04-26 00:02:06.930050 ccp4ED-1.0.9/blochwave/
--rw-rw-r--   0 tarik     (1001) tarik     (1001)       14 2022-01-10 11:09:06.000000 ccp4ED-1.0.9/blochwave/__init__.py
--rw-r--r--   0 tarik     (1001) tarik     (1001)    36950 2022-04-25 23:53:38.000000 ccp4ED-1.0.9/blochwave/bloch.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     8130 2022-04-10 16:14:34.000000 ccp4ED-1.0.9/blochwave/bloch_pp.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     5187 2022-03-29 07:03:13.000000 ccp4ED-1.0.9/blochwave/util.py
-drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2022-04-26 00:02:06.930050 ccp4ED-1.0.9/ccp4ED.egg-info/
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     4122 2022-04-26 00:02:06.000000 ccp4ED-1.0.9/ccp4ED.egg-info/PKG-INFO
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     6661 2022-04-26 00:02:06.000000 ccp4ED-1.0.9/ccp4ED.egg-info/SOURCES.txt
--rw-rw-r--   0 tarik     (1001) tarik     (1001)        1 2022-04-26 00:02:06.000000 ccp4ED-1.0.9/ccp4ED.egg-info/dependency_links.txt
--rw-rw-r--   0 tarik     (1001) tarik     (1001)       98 2022-04-26 00:02:06.000000 ccp4ED-1.0.9/ccp4ED.egg-info/requires.txt
--rw-rw-r--   0 tarik     (1001) tarik     (1001)       57 2022-04-26 00:02:06.000000 ccp4ED-1.0.9/ccp4ED.egg-info/top_level.txt
--rw-rw-r--   0 tarik     (1001) tarik     (1001)      140 2022-01-19 22:47:58.000000 ccp4ED-1.0.9/changelog.md
-drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2022-04-26 00:02:06.930050 ccp4ED-1.0.9/docs/
--rw-rw-r--   0 tarik     (1001) tarik     (1001)      584 2021-11-22 11:52:41.000000 ccp4ED-1.0.9/docs/Makefile
-drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2022-04-26 00:02:06.930050 ccp4ED-1.0.9/docs/source/
-drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2022-04-26 00:02:06.934049 ccp4ED-1.0.9/docs/source/_static/
--rw-rw-r--   0 tarik     (1001) tarik     (1001)   106120 2021-11-22 12:05:43.000000 ccp4ED-1.0.9/docs/source/_static/click.wav
--rw-rw-r--   0 tarik     (1001) tarik     (1001)    47917 2021-11-22 12:05:43.000000 ccp4ED-1.0.9/docs/source/_static/command.png
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     1488 2021-11-22 12:05:43.000000 ccp4ED-1.0.9/docs/source/_static/custom.css
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     3582 2021-11-22 12:20:36.000000 ccp4ED-1.0.9/docs/source/_static/favicon.ico
--rw-rw-r--   0 tarik     (1001) tarik     (1001)    43979 2021-11-22 12:17:11.000000 ccp4ED-1.0.9/docs/source/_static/favicon.png
--rw-rw-r--   0 tarik     (1001) tarik     (1001)    64426 2021-11-22 12:16:11.000000 ccp4ED-1.0.9/docs/source/_static/favicon.svg
--rw-rw-r--   0 tarik     (1001) tarik     (1001)    17981 2021-11-22 12:05:43.000000 ccp4ED-1.0.9/docs/source/_static/pull-requests.png
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     1860 2021-11-22 12:05:43.000000 ccp4ED-1.0.9/docs/source/_static/responsiveSvg.js
--rw-rw-r--   0 tarik     (1001) tarik     (1001)    38198 2021-11-22 12:05:43.000000 ccp4ED-1.0.9/docs/source/_static/select_transifex_repo.png
--rw-rw-r--   0 tarik     (1001) tarik     (1001)   132083 2021-11-22 12:05:43.000000 ccp4ED-1.0.9/docs/source/_static/transifex_explanation.png
-drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2022-04-26 00:02:06.934049 ccp4ED-1.0.9/docs/source/_templates/
-drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2022-04-26 00:02:06.934049 ccp4ED-1.0.9/docs/source/_templates/autosummary/
--rw-rw-r--   0 tarik     (1001) tarik     (1001)      691 2021-11-22 13:08:07.000000 ccp4ED-1.0.9/docs/source/_templates/autosummary/class.rst
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     1124 2021-11-22 13:08:07.000000 ccp4ED-1.0.9/docs/source/_templates/autosummary/module.rst
--rw-rw-r--   0 tarik     (1001) tarik     (1001)      193 2021-11-22 13:08:07.000000 ccp4ED-1.0.9/docs/source/_templates/logo-text.html
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     6825 2021-11-23 16:22:20.000000 ccp4ED-1.0.9/docs/source/conf.py
-drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2022-04-26 00:02:06.934049 ccp4ED-1.0.9/docs/source/examples/
--rw-rw-r--   0 tarik     (1001) tarik     (1001)   230485 2022-04-21 19:03:35.000000 ccp4ED-1.0.9/docs/source/examples/MX_t.png
--rw-rw-r--   0 tarik     (1001) tarik     (1001)      538 2022-04-21 19:03:06.000000 ccp4ED-1.0.9/docs/source/examples/blochwave.rst
--rw-rw-r--   0 tarik     (1001) tarik     (1001)      106 2021-11-23 10:46:27.000000 ccp4ED-1.0.9/docs/source/examples.rst
--rwxrwxr-x   0 tarik     (1001) tarik     (1001)      446 2022-04-21 19:00:03.000000 ccp4ED-1.0.9/docs/source/index.rst
--rw-rw-r--   0 tarik     (1001) tarik     (1001)      149 2021-11-23 14:28:34.000000 ccp4ED-1.0.9/docs/source/reference.rst
-drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2022-04-26 00:02:06.934049 ccp4ED-1.0.9/docs/source/reference_index/
--rw-rw-r--   0 tarik     (1001) tarik     (1001)      141 2022-01-13 10:05:38.000000 ccp4ED-1.0.9/docs/source/reference_index/EDutils.rst
--rw-rw-r--   0 tarik     (1001) tarik     (1001)      118 2021-11-24 11:23:54.000000 ccp4ED-1.0.9/docs/source/reference_index/blochwave.rst
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     2088 2022-02-04 17:13:47.000000 ccp4ED-1.0.9/install.sh
-drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2022-04-26 00:02:06.938049 ccp4ED-1.0.9/multislice/
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     1351 2020-08-24 09:18:53.000000 ccp4ED-1.0.9/multislice/ED_base.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)      260 2021-01-14 16:02:52.000000 ccp4ED-1.0.9/multislice/Makefile
--rw-rw-r--   0 tarik     (1001) tarik     (1001)        0 2021-01-20 10:23:44.000000 ccp4ED-1.0.9/multislice/__init__.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     1509 2021-06-22 11:47:44.000000 ccp4ED-1.0.9/multislice/config.py
--rwxrwxr-x   0 tarik     (1001) tarik     (1001)     1516 2021-07-19 11:11:02.000000 ccp4ED-1.0.9/multislice/convert_pets.sh
-drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2022-04-26 00:02:06.938049 ccp4ED-1.0.9/multislice/data/
--rw-rw-r--   0 tarik     (1001) tarik     (1001)    20536 2021-04-02 17:26:52.000000 ccp4ED-1.0.9/multislice/data/splines.npy
-drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2022-04-26 00:02:06.942049 ccp4ED-1.0.9/multislice/examples/
--rw-rw-r--   0 tarik     (1001) tarik     (1001)       31 2020-12-04 23:47:55.000000 ccp4ED-1.0.9/multislice/examples/.adxv_beam_center
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     2587 2020-12-04 23:47:55.000000 ccp4ED-1.0.9/multislice/examples/Carbone_SC.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     5512 2021-01-29 20:30:26.000000 ccp4ED-1.0.9/multislice/examples/Li.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     3614 2020-12-25 17:35:33.000000 ccp4ED-1.0.9/multislice/examples/biotin_figs.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     5278 2020-12-24 23:08:44.000000 ccp4ED-1.0.9/multislice/examples/biotin_run.py
-drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2022-04-26 00:02:06.954049 ccp4ED-1.0.9/multislice/examples/dat/
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     2810 2021-01-15 11:18:48.000000 ccp4ED-1.0.9/multislice/examples/dat/C.txt
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     2875 2021-01-15 11:17:59.000000 ccp4ED-1.0.9/multislice/examples/dat/H.txt
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     2859 2021-01-15 11:18:39.000000 ccp4ED-1.0.9/multislice/examples/dat/O.txt
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     2768 2021-01-15 11:24:02.000000 ccp4ED-1.0.9/multislice/examples/dat/P.txt
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     2781 2021-01-15 11:24:32.000000 ccp4ED-1.0.9/multislice/examples/dat/S.txt
--rw-rw-r--   0 tarik     (1001) tarik     (1001)  2097280 2020-12-04 23:47:55.000000 ccp4ED-1.0.9/multislice/examples/dat/biotin_m1.npy
--rw-rw-r--   0 tarik     (1001) tarik     (1001)   524800 2020-12-04 23:47:55.000000 ccp4ED-1.0.9/multislice/examples/dat/biotin_m1.smv
--rw-rw-r--   0 tarik     (1001) tarik     (1001)  2097280 2020-12-04 23:47:55.000000 ccp4ED-1.0.9/multislice/examples/dat/biotin_m1.smv.npy
--rw-rw-r--   0 tarik     (1001) tarik     (1001)    18246 2020-10-06 11:49:42.000000 ccp4ED-1.0.9/multislice/examples/dat/test.mp4
--rw-rw-r--   0 tarik     (1001) tarik     (1001)      160 2020-12-04 23:47:55.000000 ccp4ED-1.0.9/multislice/examples/dat/test.npy
--rw-rw-r--   0 tarik     (1001) tarik     (1001)      520 2020-12-04 23:47:55.000000 ccp4ED-1.0.9/multislice/examples/dat/test.smv
--rw-rw-r--   0 tarik     (1001) tarik     (1001)      283 2020-10-06 11:49:42.000000 ccp4ED-1.0.9/multislice/examples/dat/test.xyz
--rw-rw-r--   0 tarik     (1001) tarik     (1001)      869 2021-01-14 08:44:47.000000 ccp4ED-1.0.9/multislice/examples/epicza.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)    12936 2021-03-01 13:34:08.000000 ccp4ED-1.0.9/multislice/examples/ireloh.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)      821 2020-10-06 11:49:42.000000 ccp4ED-1.0.9/multislice/examples/make_crystal.py
--rwxrwxr-x   0 tarik     (1001) tarik     (1001)    25128 2020-12-04 23:47:55.000000 ccp4ED-1.0.9/multislice/examples/npy2smv
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     2661 2020-12-04 23:47:55.000000 ccp4ED-1.0.9/multislice/examples/npy2smv.cpp
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     4680 2020-08-24 09:18:53.000000 ccp4ED-1.0.9/multislice/examples/paracetamol_run.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     3077 2020-08-24 09:18:53.000000 ccp4ED-1.0.9/multislice/examples/silicon_run.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     3829 2021-06-22 12:21:01.000000 ccp4ED-1.0.9/multislice/examples/test_base.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     2138 2020-08-24 09:18:53.000000 ccp4ED-1.0.9/multislice/examples/walltimes.py
--rw-r--r--   0 tarik     (1001) tarik     (1001)     3120 2020-05-04 10:44:48.000000 ccp4ED-1.0.9/multislice/import.py
--rw-r--r--   0 tarik     (1001) tarik     (1001)     1170 2020-05-04 10:44:48.000000 ccp4ED-1.0.9/multislice/interaction_parameter.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)    15713 2021-06-25 12:39:17.000000 ccp4ED-1.0.9/multislice/multi_2D.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)    13174 2021-04-13 11:32:14.000000 ccp4ED-1.0.9/multislice/multi_3D.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)    54121 2021-06-22 11:00:04.000000 ccp4ED-1.0.9/multislice/multislice.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)    43090 2022-02-04 14:06:31.000000 ccp4ED-1.0.9/multislice/mupy_utils.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)    25256 2021-07-21 13:45:32.000000 ccp4ED-1.0.9/multislice/pets.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     8601 2022-03-07 18:03:27.000000 ccp4ED-1.0.9/multislice/postprocess.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     6767 2021-04-12 11:02:48.000000 ccp4ED-1.0.9/multislice/pymultislice.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)    12295 2021-05-14 08:02:57.000000 ccp4ED-1.0.9/multislice/rotating_crystal.py
-drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2022-04-26 00:02:06.958049 ccp4ED-1.0.9/multislice/temsim/
--rw-r--r--   0 tarik     (1001) tarik     (1001)    20465 2020-05-09 11:56:50.000000 ccp4ED-1.0.9/multislice/temsim/atompot.cpp
--rw-r--r--   0 tarik     (1001) tarik     (1001)    37228 2021-08-20 15:03:51.000000 ccp4ED-1.0.9/multislice/temsim/autoslic.cpp
--rw-r--r--   0 tarik     (1001) tarik     (1001)     7595 2021-02-15 22:58:03.000000 ccp4ED-1.0.9/multislice/temsim/autoslic.hpp
--rw-rw-r--   0 tarik     (1001) tarik     (1001)    23174 2021-02-15 22:57:45.000000 ccp4ED-1.0.9/multislice/temsim/autosliccmd.cpp
--rw-r--r--   0 tarik     (1001) tarik     (1001)    56374 2020-05-09 11:56:50.000000 ccp4ED-1.0.9/multislice/temsim/autostem.cpp
--rw-r--r--   0 tarik     (1001) tarik     (1001)    10780 2020-05-09 11:56:50.000000 ccp4ED-1.0.9/multislice/temsim/autostem.hpp
--rw-r--r--   0 tarik     (1001) tarik     (1001)    38770 2020-05-09 11:56:50.000000 ccp4ED-1.0.9/multislice/temsim/autostemcmd.cpp
--rw-r--r--   0 tarik     (1001) tarik     (1001)    14801 2020-05-09 11:56:50.000000 ccp4ED-1.0.9/multislice/temsim/cfpix.cpp
--rw-r--r--   0 tarik     (1001) tarik     (1001)     6822 2020-05-09 11:56:50.000000 ccp4ED-1.0.9/multislice/temsim/cfpix.hpp
--rw-r--r--   0 tarik     (1001) tarik     (1001)    63953 2020-05-09 11:56:50.000000 ccp4ED-1.0.9/multislice/temsim/floatTIFF.cpp
--rw-r--r--   0 tarik     (1001) tarik     (1001)    11975 2020-05-09 11:56:50.000000 ccp4ED-1.0.9/multislice/temsim/floatTIFF.hpp
--rw-r--r--   0 tarik     (1001) tarik     (1001)    27989 2020-05-09 11:56:50.000000 ccp4ED-1.0.9/multislice/temsim/image.cpp
--rw-r--r--   0 tarik     (1001) tarik     (1001)    24071 2020-05-09 11:56:50.000000 ccp4ED-1.0.9/multislice/temsim/incostem.cpp
--rw-r--r--   0 tarik     (1001) tarik     (1001)     3974 2020-05-09 11:56:50.000000 ccp4ED-1.0.9/multislice/temsim/incostem.hpp
--rw-r--r--   0 tarik     (1001) tarik     (1001)    11721 2020-05-09 11:56:50.000000 ccp4ED-1.0.9/multislice/temsim/incostemcmd.cpp
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     2635 2021-08-19 15:11:50.000000 ccp4ED-1.0.9/multislice/temsim/makefile
--rw-r--r--   0 tarik     (1001) tarik     (1001)    29412 2020-05-09 11:56:50.000000 ccp4ED-1.0.9/multislice/temsim/mulslice.cpp
--rw-r--r--   0 tarik     (1001) tarik     (1001)     9574 2020-05-09 11:56:50.000000 ccp4ED-1.0.9/multislice/temsim/probe.cpp
--rw-r--r--   0 tarik     (1001) tarik     (1001)     3159 2020-05-09 11:56:50.000000 ccp4ED-1.0.9/multislice/temsim/probe.hpp
--rw-r--r--   0 tarik     (1001) tarik     (1001)    10167 2020-05-09 11:56:50.000000 ccp4ED-1.0.9/multislice/temsim/probecmd.cpp
--rwxr-xr-x   0 tarik     (1001) tarik     (1001)      741 2020-05-09 11:56:50.000000 ccp4ED-1.0.9/multislice/temsim/run_temsim.sh
--rw-r--r--   0 tarik     (1001) tarik     (1001)   108480 2021-08-24 11:05:52.000000 ccp4ED-1.0.9/multislice/temsim/slicelib.cpp
--rw-r--r--   0 tarik     (1001) tarik     (1001)    30446 2021-08-19 08:30:53.000000 ccp4ED-1.0.9/multislice/temsim/slicelib.hpp
--rw-r--r--   0 tarik     (1001) tarik     (1001)     2209 2021-04-01 14:16:52.000000 ccp4ED-1.0.9/multislice/temsim/slicelib_main.cpp
--rw-r--r--   0 tarik     (1001) tarik     (1001)    31834 2020-05-09 11:56:50.000000 ccp4ED-1.0.9/multislice/temsim/stemslic.cpp
--rw-r--r--   0 tarik     (1001) tarik     (1001)    15883 2020-05-09 11:56:50.000000 ccp4ED-1.0.9/multislice/temsim/sumpix.cpp
-drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2022-04-26 00:02:06.962049 ccp4ED-1.0.9/nearBragg/
--rw-r--r--   0 tarik     (1001) tarik     (1001)      370 2020-08-24 09:18:53.000000 ccp4ED-1.0.9/nearBragg/Makefile
--rw-rw-r--   0 tarik     (1001) tarik     (1001)        0 2021-01-26 13:58:39.000000 ccp4ED-1.0.9/nearBragg/__init__.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)   165825 2020-08-24 09:18:53.000000 ccp4ED-1.0.9/nearBragg/nanobragg.c
--rw-rw-r--   0 tarik     (1001) tarik     (1001)    46234 2020-08-24 09:18:53.000000 ccp4ED-1.0.9/nearBragg/nearBragg.c
--rw-rw-r--   0 tarik     (1001) tarik     (1001)    17628 2021-08-12 11:44:06.000000 ccp4ED-1.0.9/nearBragg/nearBragg.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     2315 2020-08-24 09:18:53.000000 ccp4ED-1.0.9/nearBragg/nearBragg_doc.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)      635 2020-08-24 09:18:53.000000 ccp4ED-1.0.9/nearBragg/proba.py
-drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2022-04-26 00:02:06.962049 ccp4ED-1.0.9/notebooks/
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     3726 2022-02-15 12:15:37.000000 ccp4ED-1.0.9/notebooks/glycine.ipynb
-drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2022-04-26 00:02:06.962049 ccp4ED-1.0.9/notebooks/multislice/
--rw-rw-r--   0 tarik     (1001) tarik     (1001)    29065 2021-05-20 10:49:31.000000 ccp4ED-1.0.9/notebooks/multislice/Silicon.ipynb
--rw-rw-r--   0 tarik     (1001) tarik     (1001)    12603 2021-05-20 10:49:31.000000 ccp4ED-1.0.9/notebooks/multislice/example_0.ipynb
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     7927 2021-05-20 10:49:31.000000 ccp4ED-1.0.9/notebooks/multislice/glycine.ipynb
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     7145 2021-05-20 10:49:31.000000 ccp4ED-1.0.9/notebooks/multislice/pets.ipynb
--rw-rw-r--   0 tarik     (1001) tarik     (1001)      582 2020-08-24 09:18:53.000000 ccp4ED-1.0.9/pydocmd.yml
-drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2022-04-26 00:02:06.926050 ccp4ED-1.0.9/results/
-drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2022-04-26 00:02:06.962049 ccp4ED-1.0.9/results/crambin/
--rw-rw-r--   0 tarik     (1001) tarik     (1001)      202 2021-10-13 08:27:24.000000 ccp4ED-1.0.9/results/crambin/crambin.py
-drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2022-04-26 00:02:06.962049 ccp4ED-1.0.9/results/diamond/
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     2667 2021-09-04 11:52:09.000000 ccp4ED-1.0.9/results/diamond/continuous.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     1244 2021-11-24 00:21:08.000000 ccp4ED-1.0.9/results/diamond/diamond.py
-drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2022-04-26 00:02:06.966049 ccp4ED-1.0.9/results/glycine/
-drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2022-04-26 00:02:06.966049 ccp4ED-1.0.9/results/glycine/dat/
--rw-rw-r--   0 tarik     (1001) tarik     (1001)    11883 2021-07-13 10:54:02.000000 ccp4ED-1.0.9/results/glycine/dat/alpha_glycine.cif
-drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2022-04-26 00:02:06.966049 ccp4ED-1.0.9/results/glycine/dat/figures/
--rw-rw-r--   0 tarik     (1001) tarik     (1001)    58565 2021-06-09 15:54:51.000000 ccp4ED-1.0.9/results/glycine/dat/figures/glycine-103_200keV_bloch.png
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     3227 2022-02-08 11:54:52.000000 ccp4ED-1.0.9/results/glycine/glycine.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     4272 2022-03-29 13:43:42.000000 ccp4ED-1.0.9/results/glycine/glycine_zenodo.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     2614 2021-11-23 16:59:02.000000 ccp4ED-1.0.9/results/glycine/optimize_frame.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     3381 2022-02-08 13:07:47.000000 ccp4ED-1.0.9/results/glycine/pets_ref.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     2288 2022-01-26 01:30:43.000000 ccp4ED-1.0.9/results/glycine/sweep.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)   532800 2022-03-29 13:41:30.000000 ccp4ED-1.0.9/results/glycine/test.tiff
--rw-rw-r--   0 tarik     (1001) tarik     (1001)      940 2021-11-02 15:49:03.000000 ccp4ED-1.0.9/results/glycine/viewer_glycine.py
-drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2022-04-26 00:02:06.966049 ccp4ED-1.0.9/scattering/
--rw-rw-r--   0 tarik     (1001) tarik     (1001)        0 2021-01-20 10:23:54.000000 ccp4ED-1.0.9/scattering/__init__.py
--rw-r--r--   0 tarik     (1001) tarik     (1001)     1492 2020-04-23 20:38:06.000000 ccp4ED-1.0.9/scattering/cmpScattering.py
-drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2022-04-26 00:02:06.970049 ccp4ED-1.0.9/scattering/data/
--rw-r--r--   0 tarik     (1001) tarik     (1001)    10112 2020-04-23 20:38:06.000000 ccp4ED-1.0.9/scattering/data/abcd.npy
--rw-r--r--   0 tarik     (1001) tarik     (1001)    20112 2020-04-23 20:38:06.000000 ccp4ED-1.0.9/scattering/data/elec.pkl
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     4711 2021-04-01 14:18:08.000000 ccp4ED-1.0.9/scattering/data/spline_1.txt
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     4676 2021-04-01 14:51:27.000000 ccp4ED-1.0.9/scattering/data/spline_14.txt
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     4715 2021-04-01 14:19:07.000000 ccp4ED-1.0.9/scattering/data/spline_16.txt
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     4693 2021-04-01 14:18:59.000000 ccp4ED-1.0.9/scattering/data/spline_6.txt
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     4735 2021-04-01 14:19:01.000000 ccp4ED-1.0.9/scattering/data/spline_7.txt
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     4763 2021-04-01 14:19:05.000000 ccp4ED-1.0.9/scattering/data/spline_8.txt
--rw-rw-r--   0 tarik     (1001) tarik     (1001)    20536 2021-04-01 14:53:20.000000 ccp4ED-1.0.9/scattering/data/splines.npy
--rw-r--r--   0 tarik     (1001) tarik     (1001)    20347 2020-04-23 20:38:06.000000 ccp4ED-1.0.9/scattering/data/xray.pkl
--rw-rw-r--   0 tarik     (1001) tarik     (1001)      447 2021-08-21 19:31:55.000000 ccp4ED-1.0.9/scattering/potential.py
--rw-r--r--   0 tarik     (1001) tarik     (1001)     3852 2020-05-04 10:44:48.000000 ccp4ED-1.0.9/scattering/potential_misc.py
--rw-r--r--   0 tarik     (1001) tarik     (1001)     4810 2021-08-04 23:23:32.000000 ccp4ED-1.0.9/scattering/scattering_factors.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)      972 2021-04-08 18:28:59.000000 ccp4ED-1.0.9/scattering/splines.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     7947 2021-08-04 16:29:57.000000 ccp4ED-1.0.9/scattering/structure_factor.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)       38 2022-04-26 00:02:06.986049 ccp4ED-1.0.9/setup.cfg
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     1103 2022-04-26 00:02:05.000000 ccp4ED-1.0.9/setup.py
-drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2022-04-26 00:02:06.970049 ccp4ED-1.0.9/tests/
-drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2022-04-26 00:02:06.970049 ccp4ED-1.0.9/tests/EDutils/
--rw-rw-r--   0 tarik     (1001) tarik     (1001)      369 2021-06-23 09:32:38.000000 ccp4ED-1.0.9/tests/EDutils/keymap.py
-drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2022-04-26 00:02:06.974049 ccp4ED-1.0.9/tests/EDutils/pets/
--rw-rw-r--   0 tarik     (1001) tarik     (1001)    11883 2022-02-04 10:54:24.000000 ccp4ED-1.0.9/tests/EDutils/pets/alpha_glycine.cif
--rw-rw-r--   0 tarik     (1001) tarik     (1001)      435 2022-02-04 10:54:29.000000 ccp4ED-1.0.9/tests/EDutils/pets/glycine.celllist
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     4293 2022-02-04 10:54:29.000000 ccp4ED-1.0.9/tests/EDutils/pets/glycine.cenloc
--rw-rw-r--   0 tarik     (1001) tarik     (1001)    67871 2022-02-04 10:54:29.000000 ccp4ED-1.0.9/tests/EDutils/pets/glycine.cif_pets
--rw-rw-r--   0 tarik     (1001) tarik     (1001)   127790 2022-02-04 10:54:29.000000 ccp4ED-1.0.9/tests/EDutils/pets/glycine.clust
--rw-rw-r--   0 tarik     (1001) tarik     (1001)    57664 2022-02-04 10:54:29.000000 ccp4ED-1.0.9/tests/EDutils/pets/glycine.cml
--rw-rw-r--   0 tarik     (1001) tarik     (1001)   376813 2022-02-04 10:54:29.000000 ccp4ED-1.0.9/tests/EDutils/pets/glycine.cor
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     4309 2022-02-04 10:54:29.000000 ccp4ED-1.0.9/tests/EDutils/pets/glycine.framestats
--rw-rw-r--   0 tarik     (1001) tarik     (1001)    60200 2022-02-04 10:54:29.000000 ccp4ED-1.0.9/tests/EDutils/pets/glycine.hkl
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     8754 2022-02-04 10:54:29.000000 ccp4ED-1.0.9/tests/EDutils/pets/glycine.pts
--rw-rw-r--   0 tarik     (1001) tarik     (1001)    12243 2022-02-04 10:54:29.000000 ccp4ED-1.0.9/tests/EDutils/pets/glycine.resolution
--rw-rw-r--   0 tarik     (1001) tarik     (1001)   377576 2022-02-04 10:54:29.000000 ccp4ED-1.0.9/tests/EDutils/pets/glycine.rpl
--rw-rw-r--   0 tarik     (1001) tarik     (1001)    71205 2022-02-04 10:54:29.000000 ccp4ED-1.0.9/tests/EDutils/pets/glycine.xyz
--rw-rw-r--   0 tarik     (1001) tarik     (1001)   135399 2022-02-04 11:05:26.000000 ccp4ED-1.0.9/tests/EDutils/pets/glycine_dyn.cif_pets
-drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2022-04-26 00:02:06.974049 ccp4ED-1.0.9/tests/EDutils/pets/tiff/
--rw-rw-r--   0 tarik     (1001) tarik     (1001)   533356 2022-02-04 10:54:44.000000 ccp4ED-1.0.9/tests/EDutils/pets/tiff/00001.tiff
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     2788 2022-02-15 12:44:29.000000 ccp4ED-1.0.9/tests/EDutils/test_gui.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     1573 2022-02-12 10:19:12.000000 ccp4ED-1.0.9/tests/EDutils/test_pets.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     3651 2022-02-09 09:56:17.000000 ccp4ED-1.0.9/tests/EDutils/test_utilities.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)      305 2022-02-12 10:19:02.000000 ccp4ED-1.0.9/tests/EDutils/test_viewers.py
-drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2022-04-26 00:02:06.978049 ccp4ED-1.0.9/tests/blochwave/
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     2972 2022-01-12 14:01:46.000000 ccp4ED-1.0.9/tests/blochwave/GaAs_felix.cif
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     2659 2021-07-08 14:47:29.000000 ccp4ED-1.0.9/tests/blochwave/Nbeams_diamond.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)      476 2021-07-22 16:28:24.000000 ccp4ED-1.0.9/tests/blochwave/Si3N4.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)      769 2022-01-20 12:42:11.000000 ccp4ED-1.0.9/tests/blochwave/bloch2D.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)      362 2021-07-27 11:16:29.000000 ccp4ED-1.0.9/tests/blochwave/bloch_viewer.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     2474 2021-08-02 13:02:40.000000 ccp4ED-1.0.9/tests/blochwave/bloch_vs_multi2D_2beam.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     1439 2021-08-02 13:01:17.000000 ccp4ED-1.0.9/tests/blochwave/bloch_vs_multi2D_zone.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     3103 2021-08-03 23:46:34.000000 ccp4ED-1.0.9/tests/blochwave/continuous2D.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     1210 2022-01-20 11:24:29.000000 ccp4ED-1.0.9/tests/blochwave/test2beams.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     3433 2022-02-07 14:25:54.000000 ccp4ED-1.0.9/tests/blochwave/test_bloch_base.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     3329 2022-02-07 14:13:52.000000 ccp4ED-1.0.9/tests/blochwave/test_continuous.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     6388 2022-02-04 16:07:04.000000 ccp4ED-1.0.9/tests/blochwave/test_felix.py
-drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2022-04-26 00:02:06.978049 ccp4ED-1.0.9/tests/multi2D/
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     5231 2021-01-12 11:31:24.000000 ccp4ED-1.0.9/tests/multi2D/2_beam.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     5165 2021-06-25 14:06:08.000000 ccp4ED-1.0.9/tests/multi2D/2_beam_pendullosung.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     1822 2021-04-13 13:30:44.000000 ccp4ED-1.0.9/tests/multi2D/TDS.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     3161 2021-03-31 10:57:34.000000 ccp4ED-1.0.9/tests/multi2D/base_test.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     2459 2021-01-18 18:18:33.000000 ccp4ED-1.0.9/tests/multi2D/padding.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     2596 2020-10-06 11:49:42.000000 ccp4ED-1.0.9/tests/multi2D/pendullosung.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     5093 2021-03-26 09:59:09.000000 ccp4ED-1.0.9/tests/multi2D/single_array.py
-drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2022-04-26 00:02:06.978049 ccp4ED-1.0.9/tests/multislice/
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     1329 2021-04-06 09:20:34.000000 ccp4ED-1.0.9/tests/multislice/base_3D.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)       42 2021-04-06 10:00:44.000000 ccp4ED-1.0.9/tests/multislice/test.pkl
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     3916 2021-04-13 11:32:32.000000 ccp4ED-1.0.9/tests/multislice/test_base.py
-drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2022-04-26 00:02:06.926050 ccp4ED-1.0.9/tests/old/
-drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2022-04-26 00:02:06.978049 ccp4ED-1.0.9/tests/old/nearbragg/
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     2117 2020-12-08 13:53:52.000000 ccp4ED-1.0.9/tests/old/nearbragg/NBkinvsMS.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     1808 2021-08-12 11:44:10.000000 ccp4ED-1.0.9/tests/old/nearbragg/base.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     2588 2020-12-04 23:47:55.000000 ccp4ED-1.0.9/tests/old/nearbragg/cmp_Holton.py
--rw-r--r--   0 tarik     (1001) tarik     (1001)     2822 2021-01-26 08:29:45.000000 ccp4ED-1.0.9/tests/old/nearbragg/fresnel_convolution.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     3399 2020-12-04 23:47:55.000000 ccp4ED-1.0.9/tests/old/nearbragg/near_vs_multi.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     2148 2021-08-23 10:42:26.000000 ccp4ED-1.0.9/tests/old/nearbragg/proba.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     3710 2022-02-07 22:47:04.000000 ccp4ED-1.0.9/tests/reporter.py
-drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2022-04-26 00:02:06.982049 ccp4ED-1.0.9/tests/scattering_lib/
--rw-rw-r--   0 tarik     (1001) tarik     (1001)      432 2021-08-16 12:27:50.000000 ccp4ED-1.0.9/tests/scattering_lib/scat_factor.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)      707 2021-01-15 22:58:30.000000 ccp4ED-1.0.9/tests/scattering_lib/structure_factor.py
-drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2022-04-26 00:02:06.982049 ccp4ED-1.0.9/tests/wallpp/
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     4417 2021-08-03 17:31:48.000000 ccp4ED-1.0.9/tests/wallpp/base.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)      298 2021-07-26 12:36:17.000000 ccp4ED-1.0.9/tests/wallpp/config.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     1700 2021-08-03 17:40:58.000000 ccp4ED-1.0.9/tests/wallpp/gui.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)      491 2021-07-26 11:50:27.000000 ccp4ED-1.0.9/tests/wallpp/lattice.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     1970 2021-08-03 17:46:16.000000 ccp4ED-1.0.9/tests/wallpp/space_groups.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)      791 2021-08-03 17:17:50.000000 ccp4ED-1.0.9/tests/wallpp/wallpps.py
-drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2022-04-26 00:02:06.982049 ccp4ED-1.0.9/wallpp/
--rw-rw-r--   0 tarik     (1001) tarik     (1001)       18 2021-07-23 12:12:03.000000 ccp4ED-1.0.9/wallpp/__init__.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     6092 2021-07-30 12:47:32.000000 ccp4ED-1.0.9/wallpp/config.py
-drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2022-04-26 00:02:06.982049 ccp4ED-1.0.9/wallpp/docs/
--rw-rw-r--   0 tarik     (1001) tarik     (1001)    37453 2020-08-24 09:18:53.000000 ccp4ED-1.0.9/wallpp/docs/Wallpaper_Symmetry.html
--rw-rw-r--   0 tarik     (1001) tarik     (1001)      522 2020-08-24 09:18:53.000000 ccp4ED-1.0.9/wallpp/docs/index.md
--rwxrwxr-x   0 tarik     (1001) tarik     (1001)      313 2020-08-24 09:18:53.000000 ccp4ED-1.0.9/wallpp/docs/mathjaxhelper.js
--rwxrwxr-x   0 tarik     (1001) tarik     (1001)     2275 2020-08-24 09:18:53.000000 ccp4ED-1.0.9/wallpp/docs/mdx_math.py
--rwxrwxr-x   0 tarik     (1001) tarik     (1001)      355 2020-08-24 09:18:53.000000 ccp4ED-1.0.9/wallpp/docs/setup.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     9206 2021-07-30 12:23:54.000000 ccp4ED-1.0.9/wallpp/gui.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     4622 2021-08-03 23:36:31.000000 ccp4ED-1.0.9/wallpp/lattice.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)      515 2020-08-24 09:18:53.000000 ccp4ED-1.0.9/wallpp/mkdocs.yml
--rw-rw-r--   0 tarik     (1001) tarik     (1001)      803 2020-08-24 09:18:53.000000 ccp4ED-1.0.9/wallpp/nodesTri.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)    14716 2021-08-02 12:38:36.000000 ccp4ED-1.0.9/wallpp/plane_group.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     1849 2021-10-18 16:39:24.000000 ccp4ED-1.0.9/wallpp/space_group.py
--rw-rw-r--   0 tarik     (1001) tarik     (1001)   106864 2021-10-18 16:00:46.000000 ccp4ED-1.0.9/wallpp/space_groups.pkl
--rw-rw-r--   0 tarik     (1001) tarik     (1001)     7146 2021-08-03 23:44:52.000000 ccp4ED-1.0.9/wallpp/wallpaper.py
+drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2023-06-02 11:56:06.674197 ccp4ED-1.1.0/
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)      616 2023-06-02 11:55:53.000000 ccp4ED-1.1.0/.gitignore
+drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2023-06-02 11:56:06.590197 ccp4ED-1.1.0/EDutils/
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)       22 2021-07-06 22:27:03.000000 ccp4ED-1.1.0/EDutils/__init__.py
+-rwxrwxr-x   0 tarik     (1001) tarik     (1001)     1516 2022-02-04 11:05:43.000000 ccp4ED-1.1.0/EDutils/convert_pets.sh
+drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2023-06-02 11:56:06.590197 ccp4ED-1.1.0/EDutils/data/
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     2509 2022-02-15 12:23:20.000000 ccp4ED-1.1.0/EDutils/data/viewer_df.pkl
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     1164 2022-02-15 12:23:20.000000 ccp4ED-1.1.0/EDutils/data/viewer_dict.pkl
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     9276 2023-06-02 11:03:09.000000 ccp4ED-1.1.0/EDutils/dials_utils.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     5413 2022-02-07 12:30:50.000000 ccp4ED-1.1.0/EDutils/display.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     8843 2022-06-28 16:22:01.000000 ccp4ED-1.1.0/EDutils/dyn_utils.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)    17409 2023-06-02 11:03:09.000000 ccp4ED-1.1.0/EDutils/felix.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)    39768 2022-02-15 12:53:28.000000 ccp4ED-1.1.0/EDutils/gui.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)    10148 2022-02-15 12:23:17.000000 ccp4ED-1.1.0/EDutils/gui_config.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     4482 2023-06-02 11:03:09.000000 ccp4ED-1.1.0/EDutils/import_ED.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)    37929 2023-06-02 11:03:09.000000 ccp4ED-1.1.0/EDutils/pets.py
+-rwxrwxr-x   0 tarik     (1001) tarik     (1001)      589 2021-07-13 11:19:40.000000 ccp4ED-1.1.0/EDutils/pets_ref.sh
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)    19669 2023-06-02 11:03:09.000000 ccp4ED-1.1.0/EDutils/rotate_exp.py
+drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2023-06-02 11:56:06.590197 ccp4ED-1.1.0/EDutils/sandbox/
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     1942 2021-07-05 16:06:03.000000 ccp4ED-1.1.0/EDutils/sandbox/convert.py
+-rwxrwxr-x   0 tarik     (1001) tarik     (1001)      939 2021-06-10 15:53:10.000000 ccp4ED-1.1.0/EDutils/sandbox/test.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)    20689 2023-06-02 11:03:09.000000 ccp4ED-1.1.0/EDutils/utilities.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)    16042 2022-03-24 15:31:30.000000 ccp4ED-1.1.0/EDutils/viewers.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     5080 2023-06-02 11:03:09.000000 ccp4ED-1.1.0/EDutils/xds.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     4122 2023-06-02 11:56:06.674197 ccp4ED-1.1.0/PKG-INFO
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     3313 2022-04-25 08:58:12.000000 ccp4ED-1.1.0/README.md
+drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2023-06-02 11:56:06.594197 ccp4ED-1.1.0/blochwave/
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)       14 2022-01-10 11:09:06.000000 ccp4ED-1.1.0/blochwave/__init__.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)    45127 2023-06-02 11:03:09.000000 ccp4ED-1.1.0/blochwave/bloch.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)    11348 2023-06-02 11:03:09.000000 ccp4ED-1.1.0/blochwave/bloch_pp.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     6832 2023-06-02 11:03:09.000000 ccp4ED-1.1.0/blochwave/util.py
+drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2023-06-02 11:56:06.594197 ccp4ED-1.1.0/ccp4ED.egg-info/
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     4122 2023-06-02 11:56:06.000000 ccp4ED-1.1.0/ccp4ED.egg-info/PKG-INFO
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     6758 2023-06-02 11:56:06.000000 ccp4ED-1.1.0/ccp4ED.egg-info/SOURCES.txt
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)        1 2023-06-02 11:56:06.000000 ccp4ED-1.1.0/ccp4ED.egg-info/dependency_links.txt
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)      112 2023-06-02 11:56:06.000000 ccp4ED-1.1.0/ccp4ED.egg-info/requires.txt
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)       57 2023-06-02 11:56:06.000000 ccp4ED-1.1.0/ccp4ED.egg-info/top_level.txt
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)      564 2023-06-02 11:03:09.000000 ccp4ED-1.1.0/changelog.md
+drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2023-06-02 11:56:06.594197 ccp4ED-1.1.0/docs/
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)      584 2021-11-22 11:52:41.000000 ccp4ED-1.1.0/docs/Makefile
+drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2023-06-02 11:56:06.594197 ccp4ED-1.1.0/docs/source/
+drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2023-06-02 11:56:06.598197 ccp4ED-1.1.0/docs/source/_static/
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)   106120 2021-11-22 12:05:43.000000 ccp4ED-1.1.0/docs/source/_static/click.wav
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)    47917 2021-11-22 12:05:43.000000 ccp4ED-1.1.0/docs/source/_static/command.png
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     1488 2021-11-22 12:05:43.000000 ccp4ED-1.1.0/docs/source/_static/custom.css
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     3582 2021-11-22 12:20:36.000000 ccp4ED-1.1.0/docs/source/_static/favicon.ico
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)    43979 2021-11-22 12:17:11.000000 ccp4ED-1.1.0/docs/source/_static/favicon.png
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)    64426 2021-11-22 12:16:11.000000 ccp4ED-1.1.0/docs/source/_static/favicon.svg
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)    17981 2021-11-22 12:05:43.000000 ccp4ED-1.1.0/docs/source/_static/pull-requests.png
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     1860 2021-11-22 12:05:43.000000 ccp4ED-1.1.0/docs/source/_static/responsiveSvg.js
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)    38198 2021-11-22 12:05:43.000000 ccp4ED-1.1.0/docs/source/_static/select_transifex_repo.png
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)   132083 2021-11-22 12:05:43.000000 ccp4ED-1.1.0/docs/source/_static/transifex_explanation.png
+drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2023-06-02 11:56:06.598197 ccp4ED-1.1.0/docs/source/_templates/
+drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2023-06-02 11:56:06.598197 ccp4ED-1.1.0/docs/source/_templates/autosummary/
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)      691 2021-11-22 13:08:07.000000 ccp4ED-1.1.0/docs/source/_templates/autosummary/class.rst
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     1124 2021-11-22 13:08:07.000000 ccp4ED-1.1.0/docs/source/_templates/autosummary/module.rst
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)      193 2021-11-22 13:08:07.000000 ccp4ED-1.1.0/docs/source/_templates/logo-text.html
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     6825 2021-11-23 16:22:20.000000 ccp4ED-1.1.0/docs/source/conf.py
+drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2023-06-02 11:56:06.602197 ccp4ED-1.1.0/docs/source/examples/
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)   230485 2022-04-21 19:03:35.000000 ccp4ED-1.1.0/docs/source/examples/MX_t.png
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)      538 2022-04-21 19:03:06.000000 ccp4ED-1.1.0/docs/source/examples/blochwave.rst
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)      106 2021-11-23 10:46:27.000000 ccp4ED-1.1.0/docs/source/examples.rst
+-rwxrwxr-x   0 tarik     (1001) tarik     (1001)      446 2022-04-21 19:00:03.000000 ccp4ED-1.1.0/docs/source/index.rst
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)      149 2021-11-23 14:28:34.000000 ccp4ED-1.1.0/docs/source/reference.rst
+drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2023-06-02 11:56:06.602197 ccp4ED-1.1.0/docs/source/reference_index/
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)      141 2022-01-13 10:05:38.000000 ccp4ED-1.1.0/docs/source/reference_index/EDutils.rst
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)      118 2021-11-24 11:23:54.000000 ccp4ED-1.1.0/docs/source/reference_index/blochwave.rst
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     2088 2022-02-04 17:13:47.000000 ccp4ED-1.1.0/install.sh
+drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2023-06-02 11:56:06.606197 ccp4ED-1.1.0/multislice/
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     1351 2020-08-24 09:18:53.000000 ccp4ED-1.1.0/multislice/ED_base.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)      260 2021-01-14 16:02:52.000000 ccp4ED-1.1.0/multislice/Makefile
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)        0 2021-01-20 10:23:44.000000 ccp4ED-1.1.0/multislice/__init__.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     1509 2021-06-22 11:47:44.000000 ccp4ED-1.1.0/multislice/config.py
+-rwxrwxr-x   0 tarik     (1001) tarik     (1001)     1516 2021-07-19 11:11:02.000000 ccp4ED-1.1.0/multislice/convert_pets.sh
+drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2023-06-02 11:56:06.606197 ccp4ED-1.1.0/multislice/data/
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)    20536 2021-04-02 17:26:52.000000 ccp4ED-1.1.0/multislice/data/splines.npy
+drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2023-06-02 11:56:06.614197 ccp4ED-1.1.0/multislice/examples/
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)       31 2020-12-04 23:47:55.000000 ccp4ED-1.1.0/multislice/examples/.adxv_beam_center
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     2587 2020-12-04 23:47:55.000000 ccp4ED-1.1.0/multislice/examples/Carbone_SC.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     5512 2021-01-29 20:30:26.000000 ccp4ED-1.1.0/multislice/examples/Li.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     3614 2020-12-25 17:35:33.000000 ccp4ED-1.1.0/multislice/examples/biotin_figs.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     5278 2020-12-24 23:08:44.000000 ccp4ED-1.1.0/multislice/examples/biotin_run.py
+drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2023-06-02 11:56:06.622197 ccp4ED-1.1.0/multislice/examples/dat/
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     2810 2021-01-15 11:18:48.000000 ccp4ED-1.1.0/multislice/examples/dat/C.txt
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     2875 2021-01-15 11:17:59.000000 ccp4ED-1.1.0/multislice/examples/dat/H.txt
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     2859 2021-01-15 11:18:39.000000 ccp4ED-1.1.0/multislice/examples/dat/O.txt
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     2768 2021-01-15 11:24:02.000000 ccp4ED-1.1.0/multislice/examples/dat/P.txt
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     2781 2021-01-15 11:24:32.000000 ccp4ED-1.1.0/multislice/examples/dat/S.txt
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)  2097280 2020-12-04 23:47:55.000000 ccp4ED-1.1.0/multislice/examples/dat/biotin_m1.npy
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)   524800 2020-12-04 23:47:55.000000 ccp4ED-1.1.0/multislice/examples/dat/biotin_m1.smv
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)  2097280 2020-12-04 23:47:55.000000 ccp4ED-1.1.0/multislice/examples/dat/biotin_m1.smv.npy
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)    18246 2020-10-06 11:49:42.000000 ccp4ED-1.1.0/multislice/examples/dat/test.mp4
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)      160 2020-12-04 23:47:55.000000 ccp4ED-1.1.0/multislice/examples/dat/test.npy
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)      520 2020-12-04 23:47:55.000000 ccp4ED-1.1.0/multislice/examples/dat/test.smv
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)      283 2020-10-06 11:49:42.000000 ccp4ED-1.1.0/multislice/examples/dat/test.xyz
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)      869 2021-01-14 08:44:47.000000 ccp4ED-1.1.0/multislice/examples/epicza.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)    12936 2021-03-01 13:34:08.000000 ccp4ED-1.1.0/multislice/examples/ireloh.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)      821 2020-10-06 11:49:42.000000 ccp4ED-1.1.0/multislice/examples/make_crystal.py
+-rwxrwxr-x   0 tarik     (1001) tarik     (1001)    25128 2020-12-04 23:47:55.000000 ccp4ED-1.1.0/multislice/examples/npy2smv
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     2661 2020-12-04 23:47:55.000000 ccp4ED-1.1.0/multislice/examples/npy2smv.cpp
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     4680 2020-08-24 09:18:53.000000 ccp4ED-1.1.0/multislice/examples/paracetamol_run.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     3077 2020-08-24 09:18:53.000000 ccp4ED-1.1.0/multislice/examples/silicon_run.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     3829 2021-06-22 12:21:01.000000 ccp4ED-1.1.0/multislice/examples/test_base.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     2138 2020-08-24 09:18:53.000000 ccp4ED-1.1.0/multislice/examples/walltimes.py
+-rw-r--r--   0 tarik     (1001) tarik     (1001)     3120 2020-05-04 10:44:48.000000 ccp4ED-1.1.0/multislice/import.py
+-rw-r--r--   0 tarik     (1001) tarik     (1001)     1170 2020-05-04 10:44:48.000000 ccp4ED-1.1.0/multislice/interaction_parameter.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)    15713 2021-06-25 12:39:17.000000 ccp4ED-1.1.0/multislice/multi_2D.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)    13174 2021-04-13 11:32:14.000000 ccp4ED-1.1.0/multislice/multi_3D.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)    54121 2021-06-22 11:00:04.000000 ccp4ED-1.1.0/multislice/multislice.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)    43090 2022-02-04 14:06:31.000000 ccp4ED-1.1.0/multislice/mupy_utils.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)    25256 2021-07-21 13:45:32.000000 ccp4ED-1.1.0/multislice/pets.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     8601 2022-03-07 18:03:27.000000 ccp4ED-1.1.0/multislice/postprocess.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     6767 2021-04-12 11:02:48.000000 ccp4ED-1.1.0/multislice/pymultislice.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)    12295 2021-05-14 08:02:57.000000 ccp4ED-1.1.0/multislice/rotating_crystal.py
+drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2023-06-02 11:56:06.634197 ccp4ED-1.1.0/multislice/temsim/
+-rw-r--r--   0 tarik     (1001) tarik     (1001)    20465 2020-05-09 11:56:50.000000 ccp4ED-1.1.0/multislice/temsim/atompot.cpp
+-rw-r--r--   0 tarik     (1001) tarik     (1001)    37228 2021-08-20 15:03:51.000000 ccp4ED-1.1.0/multislice/temsim/autoslic.cpp
+-rw-r--r--   0 tarik     (1001) tarik     (1001)     7595 2021-02-15 22:58:03.000000 ccp4ED-1.1.0/multislice/temsim/autoslic.hpp
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)    23174 2021-02-15 22:57:45.000000 ccp4ED-1.1.0/multislice/temsim/autosliccmd.cpp
+-rw-r--r--   0 tarik     (1001) tarik     (1001)    56374 2020-05-09 11:56:50.000000 ccp4ED-1.1.0/multislice/temsim/autostem.cpp
+-rw-r--r--   0 tarik     (1001) tarik     (1001)    10780 2020-05-09 11:56:50.000000 ccp4ED-1.1.0/multislice/temsim/autostem.hpp
+-rw-r--r--   0 tarik     (1001) tarik     (1001)    38770 2020-05-09 11:56:50.000000 ccp4ED-1.1.0/multislice/temsim/autostemcmd.cpp
+-rw-r--r--   0 tarik     (1001) tarik     (1001)    14801 2020-05-09 11:56:50.000000 ccp4ED-1.1.0/multislice/temsim/cfpix.cpp
+-rw-r--r--   0 tarik     (1001) tarik     (1001)     6822 2020-05-09 11:56:50.000000 ccp4ED-1.1.0/multislice/temsim/cfpix.hpp
+-rw-r--r--   0 tarik     (1001) tarik     (1001)    63953 2020-05-09 11:56:50.000000 ccp4ED-1.1.0/multislice/temsim/floatTIFF.cpp
+-rw-r--r--   0 tarik     (1001) tarik     (1001)    11975 2020-05-09 11:56:50.000000 ccp4ED-1.1.0/multislice/temsim/floatTIFF.hpp
+-rw-r--r--   0 tarik     (1001) tarik     (1001)    27989 2020-05-09 11:56:50.000000 ccp4ED-1.1.0/multislice/temsim/image.cpp
+-rw-r--r--   0 tarik     (1001) tarik     (1001)    24071 2020-05-09 11:56:50.000000 ccp4ED-1.1.0/multislice/temsim/incostem.cpp
+-rw-r--r--   0 tarik     (1001) tarik     (1001)     3974 2020-05-09 11:56:50.000000 ccp4ED-1.1.0/multislice/temsim/incostem.hpp
+-rw-r--r--   0 tarik     (1001) tarik     (1001)    11721 2020-05-09 11:56:50.000000 ccp4ED-1.1.0/multislice/temsim/incostemcmd.cpp
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     2635 2021-08-19 15:11:50.000000 ccp4ED-1.1.0/multislice/temsim/makefile
+-rw-r--r--   0 tarik     (1001) tarik     (1001)    29412 2020-05-09 11:56:50.000000 ccp4ED-1.1.0/multislice/temsim/mulslice.cpp
+-rw-r--r--   0 tarik     (1001) tarik     (1001)     9574 2020-05-09 11:56:50.000000 ccp4ED-1.1.0/multislice/temsim/probe.cpp
+-rw-r--r--   0 tarik     (1001) tarik     (1001)     3159 2020-05-09 11:56:50.000000 ccp4ED-1.1.0/multislice/temsim/probe.hpp
+-rw-r--r--   0 tarik     (1001) tarik     (1001)    10167 2020-05-09 11:56:50.000000 ccp4ED-1.1.0/multislice/temsim/probecmd.cpp
+-rwxr-xr-x   0 tarik     (1001) tarik     (1001)      741 2020-05-09 11:56:50.000000 ccp4ED-1.1.0/multislice/temsim/run_temsim.sh
+-rw-r--r--   0 tarik     (1001) tarik     (1001)   108480 2021-08-24 11:05:52.000000 ccp4ED-1.1.0/multislice/temsim/slicelib.cpp
+-rw-r--r--   0 tarik     (1001) tarik     (1001)    30446 2021-08-19 08:30:53.000000 ccp4ED-1.1.0/multislice/temsim/slicelib.hpp
+-rw-r--r--   0 tarik     (1001) tarik     (1001)     2209 2021-04-01 14:16:52.000000 ccp4ED-1.1.0/multislice/temsim/slicelib_main.cpp
+-rw-r--r--   0 tarik     (1001) tarik     (1001)    31834 2020-05-09 11:56:50.000000 ccp4ED-1.1.0/multislice/temsim/stemslic.cpp
+-rw-r--r--   0 tarik     (1001) tarik     (1001)    15883 2020-05-09 11:56:50.000000 ccp4ED-1.1.0/multislice/temsim/sumpix.cpp
+drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2023-06-02 11:56:06.634197 ccp4ED-1.1.0/nearBragg/
+-rw-r--r--   0 tarik     (1001) tarik     (1001)      370 2020-08-24 09:18:53.000000 ccp4ED-1.1.0/nearBragg/Makefile
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)        0 2021-01-26 13:58:39.000000 ccp4ED-1.1.0/nearBragg/__init__.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)   165825 2020-08-24 09:18:53.000000 ccp4ED-1.1.0/nearBragg/nanobragg.c
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)    46234 2020-08-24 09:18:53.000000 ccp4ED-1.1.0/nearBragg/nearBragg.c
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)    17628 2021-08-12 11:44:06.000000 ccp4ED-1.1.0/nearBragg/nearBragg.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     2315 2020-08-24 09:18:53.000000 ccp4ED-1.1.0/nearBragg/nearBragg_doc.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)      635 2020-08-24 09:18:53.000000 ccp4ED-1.1.0/nearBragg/proba.py
+drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2023-06-02 11:56:06.634197 ccp4ED-1.1.0/notebooks/
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     3726 2022-02-15 12:15:37.000000 ccp4ED-1.1.0/notebooks/glycine.ipynb
+drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2023-06-02 11:56:06.638197 ccp4ED-1.1.0/notebooks/multislice/
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)    29065 2021-05-20 10:49:31.000000 ccp4ED-1.1.0/notebooks/multislice/Silicon.ipynb
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)    12603 2021-05-20 10:49:31.000000 ccp4ED-1.1.0/notebooks/multislice/example_0.ipynb
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     7927 2021-05-20 10:49:31.000000 ccp4ED-1.1.0/notebooks/multislice/glycine.ipynb
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     7145 2021-05-20 10:49:31.000000 ccp4ED-1.1.0/notebooks/multislice/pets.ipynb
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)      582 2020-08-24 09:18:53.000000 ccp4ED-1.1.0/pydocmd.yml
+drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2023-06-02 11:56:06.586197 ccp4ED-1.1.0/results/
+drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2023-06-02 11:56:06.638197 ccp4ED-1.1.0/results/crambin/
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)      202 2021-10-13 08:27:24.000000 ccp4ED-1.1.0/results/crambin/crambin.py
+drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2023-06-02 11:56:06.638197 ccp4ED-1.1.0/results/diamond/
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     2667 2021-09-04 11:52:09.000000 ccp4ED-1.1.0/results/diamond/continuous.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     1244 2021-11-24 00:21:08.000000 ccp4ED-1.1.0/results/diamond/diamond.py
+drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2023-06-02 11:56:06.642197 ccp4ED-1.1.0/results/glycine/
+drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2023-06-02 11:56:06.642197 ccp4ED-1.1.0/results/glycine/dat/
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)    11883 2021-07-13 10:54:02.000000 ccp4ED-1.1.0/results/glycine/dat/alpha_glycine.cif
+drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2023-06-02 11:56:06.642197 ccp4ED-1.1.0/results/glycine/dat/figures/
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)    58565 2021-06-09 15:54:51.000000 ccp4ED-1.1.0/results/glycine/dat/figures/glycine-103_200keV_bloch.png
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     3227 2022-02-08 11:54:52.000000 ccp4ED-1.1.0/results/glycine/glycine.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     4272 2022-03-29 13:43:42.000000 ccp4ED-1.1.0/results/glycine/glycine_zenodo.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     2614 2021-11-23 16:59:02.000000 ccp4ED-1.1.0/results/glycine/optimize_frame.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     3381 2022-02-08 13:07:47.000000 ccp4ED-1.1.0/results/glycine/pets_ref.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     2288 2022-01-26 01:30:43.000000 ccp4ED-1.1.0/results/glycine/sweep.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)   532800 2022-03-29 13:41:30.000000 ccp4ED-1.1.0/results/glycine/test.tiff
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)      940 2021-11-02 15:49:03.000000 ccp4ED-1.1.0/results/glycine/viewer_glycine.py
+drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2023-06-02 11:56:06.646197 ccp4ED-1.1.0/scattering/
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)        0 2021-01-20 10:23:54.000000 ccp4ED-1.1.0/scattering/__init__.py
+-rw-r--r--   0 tarik     (1001) tarik     (1001)     1492 2020-04-23 20:38:06.000000 ccp4ED-1.1.0/scattering/cmpScattering.py
+drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2023-06-02 11:56:06.650197 ccp4ED-1.1.0/scattering/data/
+-rw-r--r--   0 tarik     (1001) tarik     (1001)    10112 2020-04-23 20:38:06.000000 ccp4ED-1.1.0/scattering/data/abcd.npy
+-rw-r--r--   0 tarik     (1001) tarik     (1001)    20112 2020-04-23 20:38:06.000000 ccp4ED-1.1.0/scattering/data/elec.pkl
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     4711 2021-04-01 14:18:08.000000 ccp4ED-1.1.0/scattering/data/spline_1.txt
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     4676 2021-04-01 14:51:27.000000 ccp4ED-1.1.0/scattering/data/spline_14.txt
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     4715 2021-04-01 14:19:07.000000 ccp4ED-1.1.0/scattering/data/spline_16.txt
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     4693 2021-04-01 14:18:59.000000 ccp4ED-1.1.0/scattering/data/spline_6.txt
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     4735 2021-04-01 14:19:01.000000 ccp4ED-1.1.0/scattering/data/spline_7.txt
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     4763 2021-04-01 14:19:05.000000 ccp4ED-1.1.0/scattering/data/spline_8.txt
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)    20536 2021-04-01 14:53:20.000000 ccp4ED-1.1.0/scattering/data/splines.npy
+-rw-r--r--   0 tarik     (1001) tarik     (1001)    20347 2020-04-23 20:38:06.000000 ccp4ED-1.1.0/scattering/data/xray.pkl
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)      447 2021-08-21 19:31:55.000000 ccp4ED-1.1.0/scattering/potential.py
+-rw-r--r--   0 tarik     (1001) tarik     (1001)     3852 2020-05-04 10:44:48.000000 ccp4ED-1.1.0/scattering/potential_misc.py
+-rw-r--r--   0 tarik     (1001) tarik     (1001)     4812 2022-05-18 13:22:51.000000 ccp4ED-1.1.0/scattering/scattering_factors.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)      972 2021-04-08 18:28:59.000000 ccp4ED-1.1.0/scattering/splines.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     7947 2021-08-04 16:29:57.000000 ccp4ED-1.1.0/scattering/structure_factor.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)       38 2023-06-02 11:56:06.674197 ccp4ED-1.1.0/setup.cfg
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     1126 2023-06-02 11:05:10.000000 ccp4ED-1.1.0/setup.py
+drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2023-06-02 11:56:06.650197 ccp4ED-1.1.0/tests/
+drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2023-06-02 11:56:06.650197 ccp4ED-1.1.0/tests/EDutils/
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)      369 2021-06-23 09:32:38.000000 ccp4ED-1.1.0/tests/EDutils/keymap.py
+drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2023-06-02 11:56:06.658197 ccp4ED-1.1.0/tests/EDutils/pets/
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)    11883 2022-02-04 10:54:24.000000 ccp4ED-1.1.0/tests/EDutils/pets/alpha_glycine.cif
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)      435 2022-02-04 10:54:29.000000 ccp4ED-1.1.0/tests/EDutils/pets/glycine.celllist
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     4293 2022-02-04 10:54:29.000000 ccp4ED-1.1.0/tests/EDutils/pets/glycine.cenloc
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)    67871 2022-02-04 10:54:29.000000 ccp4ED-1.1.0/tests/EDutils/pets/glycine.cif_pets
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)   127790 2022-02-04 10:54:29.000000 ccp4ED-1.1.0/tests/EDutils/pets/glycine.clust
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)    57664 2022-02-04 10:54:29.000000 ccp4ED-1.1.0/tests/EDutils/pets/glycine.cml
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)   376813 2022-02-04 10:54:29.000000 ccp4ED-1.1.0/tests/EDutils/pets/glycine.cor
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     4309 2022-02-04 10:54:29.000000 ccp4ED-1.1.0/tests/EDutils/pets/glycine.framestats
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)    60200 2022-02-04 10:54:29.000000 ccp4ED-1.1.0/tests/EDutils/pets/glycine.hkl
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     8754 2022-02-04 10:54:29.000000 ccp4ED-1.1.0/tests/EDutils/pets/glycine.pts
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)    12243 2022-02-04 10:54:29.000000 ccp4ED-1.1.0/tests/EDutils/pets/glycine.resolution
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)   377576 2022-02-04 10:54:29.000000 ccp4ED-1.1.0/tests/EDutils/pets/glycine.rpl
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)    71205 2022-02-04 10:54:29.000000 ccp4ED-1.1.0/tests/EDutils/pets/glycine.xyz
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)   135399 2022-02-04 11:05:26.000000 ccp4ED-1.1.0/tests/EDutils/pets/glycine_dyn.cif_pets
+drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2023-06-02 11:56:06.658197 ccp4ED-1.1.0/tests/EDutils/pets/tiff/
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)   533356 2022-02-04 10:54:44.000000 ccp4ED-1.1.0/tests/EDutils/pets/tiff/00001.tiff
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     2788 2022-02-15 12:44:29.000000 ccp4ED-1.1.0/tests/EDutils/test_gui.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     1573 2023-06-02 11:55:53.000000 ccp4ED-1.1.0/tests/EDutils/test_pets.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     3651 2022-02-09 09:56:17.000000 ccp4ED-1.1.0/tests/EDutils/test_utilities.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)      305 2022-02-12 10:19:02.000000 ccp4ED-1.1.0/tests/EDutils/test_viewers.py
+drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2023-06-02 11:56:06.662197 ccp4ED-1.1.0/tests/blochwave/
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     2972 2022-01-12 14:01:46.000000 ccp4ED-1.1.0/tests/blochwave/GaAs_felix.cif
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     2659 2021-07-08 14:47:29.000000 ccp4ED-1.1.0/tests/blochwave/Nbeams_diamond.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)      476 2021-07-22 16:28:24.000000 ccp4ED-1.1.0/tests/blochwave/Si3N4.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)      769 2022-01-20 12:42:11.000000 ccp4ED-1.1.0/tests/blochwave/bloch2D.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)      362 2021-07-27 11:16:29.000000 ccp4ED-1.1.0/tests/blochwave/bloch_viewer.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     2474 2021-08-02 13:02:40.000000 ccp4ED-1.1.0/tests/blochwave/bloch_vs_multi2D_2beam.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     1439 2021-08-02 13:01:17.000000 ccp4ED-1.1.0/tests/blochwave/bloch_vs_multi2D_zone.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     3103 2021-08-03 23:46:34.000000 ccp4ED-1.1.0/tests/blochwave/continuous2D.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     1210 2022-01-20 11:24:29.000000 ccp4ED-1.1.0/tests/blochwave/test2beams.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     3433 2022-02-07 14:25:54.000000 ccp4ED-1.1.0/tests/blochwave/test_bloch_base.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     3329 2022-02-07 14:13:52.000000 ccp4ED-1.1.0/tests/blochwave/test_continuous.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     6388 2022-02-04 16:07:04.000000 ccp4ED-1.1.0/tests/blochwave/test_felix.py
+drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2023-06-02 11:56:06.662197 ccp4ED-1.1.0/tests/multi2D/
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     5231 2021-01-12 11:31:24.000000 ccp4ED-1.1.0/tests/multi2D/2_beam.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     5165 2021-06-25 14:06:08.000000 ccp4ED-1.1.0/tests/multi2D/2_beam_pendullosung.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     1822 2021-04-13 13:30:44.000000 ccp4ED-1.1.0/tests/multi2D/TDS.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     3161 2021-03-31 10:57:34.000000 ccp4ED-1.1.0/tests/multi2D/base_test.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     2459 2021-01-18 18:18:33.000000 ccp4ED-1.1.0/tests/multi2D/padding.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     2596 2020-10-06 11:49:42.000000 ccp4ED-1.1.0/tests/multi2D/pendullosung.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     5093 2021-03-26 09:59:09.000000 ccp4ED-1.1.0/tests/multi2D/single_array.py
+drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2023-06-02 11:56:06.666197 ccp4ED-1.1.0/tests/multislice/
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     1329 2021-04-06 09:20:34.000000 ccp4ED-1.1.0/tests/multislice/base_3D.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)       42 2021-04-06 10:00:44.000000 ccp4ED-1.1.0/tests/multislice/test.pkl
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     3916 2021-04-13 11:32:32.000000 ccp4ED-1.1.0/tests/multislice/test_base.py
+drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2023-06-02 11:56:06.586197 ccp4ED-1.1.0/tests/old/
+drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2023-06-02 11:56:06.666197 ccp4ED-1.1.0/tests/old/nearbragg/
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     2117 2020-12-08 13:53:52.000000 ccp4ED-1.1.0/tests/old/nearbragg/NBkinvsMS.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     1808 2021-08-12 11:44:10.000000 ccp4ED-1.1.0/tests/old/nearbragg/base.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     2588 2020-12-04 23:47:55.000000 ccp4ED-1.1.0/tests/old/nearbragg/cmp_Holton.py
+-rw-r--r--   0 tarik     (1001) tarik     (1001)     2822 2021-01-26 08:29:45.000000 ccp4ED-1.1.0/tests/old/nearbragg/fresnel_convolution.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     3399 2020-12-04 23:47:55.000000 ccp4ED-1.1.0/tests/old/nearbragg/near_vs_multi.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     2148 2021-08-23 10:42:26.000000 ccp4ED-1.1.0/tests/old/nearbragg/proba.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     3710 2022-02-07 22:47:04.000000 ccp4ED-1.1.0/tests/reporter.py
+drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2023-06-02 11:56:06.666197 ccp4ED-1.1.0/tests/scattering_lib/
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)      432 2021-08-16 12:27:50.000000 ccp4ED-1.1.0/tests/scattering_lib/scat_factor.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)      707 2021-01-15 22:58:30.000000 ccp4ED-1.1.0/tests/scattering_lib/structure_factor.py
+drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2023-06-02 11:56:06.670197 ccp4ED-1.1.0/tests/wallpp/
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     4417 2021-08-03 17:31:48.000000 ccp4ED-1.1.0/tests/wallpp/base.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)      298 2021-07-26 12:36:17.000000 ccp4ED-1.1.0/tests/wallpp/config.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     1700 2021-08-03 17:40:58.000000 ccp4ED-1.1.0/tests/wallpp/gui.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)      491 2021-07-26 11:50:27.000000 ccp4ED-1.1.0/tests/wallpp/lattice.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     1970 2021-08-03 17:46:16.000000 ccp4ED-1.1.0/tests/wallpp/space_groups.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)      791 2021-08-03 17:17:50.000000 ccp4ED-1.1.0/tests/wallpp/wallpps.py
+drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2023-06-02 11:56:06.674197 ccp4ED-1.1.0/wallpp/
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)       18 2021-07-23 12:12:03.000000 ccp4ED-1.1.0/wallpp/__init__.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     6092 2021-07-30 12:47:32.000000 ccp4ED-1.1.0/wallpp/config.py
+drwxrwxr-x   0 tarik     (1001) tarik     (1001)        0 2023-06-02 11:56:06.674197 ccp4ED-1.1.0/wallpp/docs/
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)    37453 2020-08-24 09:18:53.000000 ccp4ED-1.1.0/wallpp/docs/Wallpaper_Symmetry.html
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)      522 2020-08-24 09:18:53.000000 ccp4ED-1.1.0/wallpp/docs/index.md
+-rwxrwxr-x   0 tarik     (1001) tarik     (1001)      313 2020-08-24 09:18:53.000000 ccp4ED-1.1.0/wallpp/docs/mathjaxhelper.js
+-rwxrwxr-x   0 tarik     (1001) tarik     (1001)     2275 2020-08-24 09:18:53.000000 ccp4ED-1.1.0/wallpp/docs/mdx_math.py
+-rwxrwxr-x   0 tarik     (1001) tarik     (1001)      355 2020-08-24 09:18:53.000000 ccp4ED-1.1.0/wallpp/docs/setup.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     9206 2021-07-30 12:23:54.000000 ccp4ED-1.1.0/wallpp/gui.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     4622 2021-08-03 23:36:31.000000 ccp4ED-1.1.0/wallpp/lattice.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)      515 2020-08-24 09:18:53.000000 ccp4ED-1.1.0/wallpp/mkdocs.yml
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)      803 2020-08-24 09:18:53.000000 ccp4ED-1.1.0/wallpp/nodesTri.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)    14716 2021-08-02 12:38:36.000000 ccp4ED-1.1.0/wallpp/plane_group.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     1849 2021-10-18 16:39:24.000000 ccp4ED-1.1.0/wallpp/space_group.py
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)   106864 2021-10-18 16:00:46.000000 ccp4ED-1.1.0/wallpp/space_groups.pkl
+-rw-rw-r--   0 tarik     (1001) tarik     (1001)     7146 2021-08-03 23:44:52.000000 ccp4ED-1.1.0/wallpp/wallpaper.py
```

### Comparing `ccp4ED-1.0.9/.gitignore` & `ccp4ED-1.1.0/.gitignore`

 * *Files 13% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 tests/dials
 tests/felix
 tests/*/dat
 #multislice/examples/dat
 multislice/temsim/makefile
 multislice/data_2D
 #blochwave/
+blochwave/dyngo
+blochwave/felix
 **/tiffs
 results/glycine/pets
 
 
 **.ipynb_checkpoints/
 notebooks/Untitled.ipynb
 notebooks/tests/
@@ -36,7 +38,8 @@
 ## Python
 **/__pycache__
 *.egg-info
 **/.coverage
 **/htmlcov
 **/build
 **/dist
+TorchBloch*
```

### Comparing `ccp4ED-1.0.9/EDutils/convert_pets.sh` & `ccp4ED-1.1.0/EDutils/convert_pets.sh`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/EDutils/data/viewer_df.pkl` & `ccp4ED-1.1.0/EDutils/data/viewer_df.pkl`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/EDutils/data/viewer_dict.pkl` & `ccp4ED-1.1.0/EDutils/data/viewer_dict.pkl`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/EDutils/display.py` & `ccp4ED-1.1.0/EDutils/display.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/EDutils/gui.py` & `ccp4ED-1.1.0/EDutils/gui.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/EDutils/gui_config.py` & `ccp4ED-1.1.0/EDutils/gui_config.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/EDutils/pets.py` & `ccp4ED-1.1.0/EDutils/pets.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,52 +1,93 @@
 import importlib as imp
-import os,glob, numpy as np, pandas as pd, tifffile,scipy.optimize as opt
+import os,glob, numpy as np, pandas as pd, tifffile,mrcfile,scipy.optimize as opt
 from typing import TYPE_CHECKING, Dict, Iterable, Optional, Sequence, Union
-from subprocess import Popen,PIPE
+from subprocess import Popen,PIPE,check_output
 from crystals import Crystal,Lattice
 from utils import handler3D as h3D          #;imp.reload(h3D)
 from utils import displayStandards as dsp   #;imp.reload(dsp)
+from utils import glob_colors as colors
 from multislice  import mupy_utils as mut   #;imp.reload(mut)
-from EDutils import viewers as vw           ;imp.reload(vw)
+from EDutils import viewers as vw           #;imp.reload(vw)
 from EDutils import utilities as ut         #;imp.reload(ut)
 from multislice.rotating_crystal import get_crystal_rotation
+from gemmi import cif
+from utils import physicsConstants as cst
+from blochwave import bloch                 #;imp.reload(bloch)
+# from . import import_ED as ED               ;imp.reload(ED)
 
-class Pets:
+
+class Pets():
     def __init__(self,pts_file:str,
         cif_file:Optional[str]=None,gen:bool=False,dyn:bool=False):
         """ Pets importer
 
         parameters
         ----------
             pts_file
-                full path to .pts file
+                full path to .pts file or .cif_pets
             cif_file
                 full path to .cif file (automatically found if None)
             gen
                 force reload if True
             dyn
                 load dyn_cif into .cif if True
         """
-        self.name  = os.path.basename(pts_file).split('.pts')[0] #;print(self.name)
-        self.path  = os.path.dirname(pts_file)
-        self.out   = self.path+'/dat/'
+        self.name = os.path.basename(pts_file).split('.pts')[0] #;print(self.name)
+        self.path = os.path.dirname(pts_file)
+        self.out  = self.path+'/dat/'
 
 
         self.cif_file   = ut.find_cif_file(self.path,cif_file)
         self.crys       = ut.import_crys(self.cif_file)
         self.lat_vec    = np.array(self.crys.lattice_vectors)
         self.lat_vec1   = np.array(self.crys.reciprocal_vectors)/(2*np.pi)
         self.lat_params = self.crys.lattice_parameters
 
         gen |= not os.path.exists(self.out)
         # if os.path.exists(self.out):gen |= not os.path.exists(self.out+'rpl.txt')
         if gen:self._convert_pets()
         self._load_all(dyn)
         self.nFrames = self.uvw.shape[0]
 
+        tiffs = glob.glob(os.path.join(self.path,'tiff','*.tiff'))
+        if len(tiffs):
+            self.nxy = tifffile.imread(tiffs[0]).shape
+
+    def hkl_to_pixels(self,h,frame):
+        hkl = np.array([eval(hkl) for hkl in h])
+        #spot locations in reciprocal crystal frame (with shape 3 x n_refl)
+        rxyz = self.UB.dot(hkl.T).T
+        # print(rxyz)
+        alpha,beta,gamma = self.cif.iloc[frame-1][['alpha','beta','omega']]
+        # print(alpha,beta,gamma)
+        alpha_r,beta_r,gamma_r = -np.deg2rad([alpha,beta,gamma])
+        ctx,stx = np.cos(alpha_r),np.sin(alpha_r)
+        cty,sty = np.cos(beta_r) ,np.sin(beta_r)
+        ctz,stz = np.cos(gamma_r),np.sin(gamma_r)
+
+        Rx = np.array([[1,0,0],[0,ctx,stx],[0,-stx,ctx]])
+        Ry = np.array([[cty,0,sty],[0,1,0],[-sty,0,cty]])
+        Rz = np.array([[ctz,stz,0],[-stz,ctz,0],[0,0,1]])
+        # R = Ry.dot(Rx.dot(Rz))
+        R = Rz.dot(Ry.dot(Rx))
+        qxyz = R.dot(rxyz.T)
+        # print(qxyz)
+        qx,qy = qxyz[:2,:]
+
+        ### convert to pixels
+        df_pxy=pd.DataFrame()
+        cx,cy = self.cen.loc[frame-1, ['px','py']]
+        df_pxy['px'] = qx/self.aper + cx
+        df_pxy['py'] = -qy/self.aper + cy
+        df_pxy.index=h
+        return df_pxy
+
+    def save(self):
+        ut.save_pkl(self, os.path.join(self.path,'pets.pkl'))
 
     def _convert_pets(self):
         cmd = "%s/convert_pets.sh %s %s" %(os.path.dirname(__file__),self.path,self.name)
         p = Popen(cmd,shell=True,stdout=PIPE,stderr=PIPE);p.wait();o,e=p.communicate()
         print(o.decode(),e.decode())
 
         A = np.loadtxt(self.out+'UB.txt')
@@ -59,35 +100,39 @@
 
     def _load_all(self,dyn=1):
         lam,omega,aper = np.loadtxt(self.out+'pts.txt')
         self.omega = omega
         self.aper  = aper
         self.lam   = lam
         self.K0    = 1/self.lam
+        self.keV = cst.lam2keV(self.lam)
 
         self.frames = pd.read_csv(self.out+'iml.txt',sep=',',names=['name','alpha','beta','domega','scale','calibration','ellipA','ellipP','used'])
         self.rpl = pd.read_csv(self.out+'rpl.txt',sep=',',names=['x','y','z','I','i','px','py','rpx','rpy','alpha','Im','F'])
         self.cor = pd.read_csv(self.out+'cor.txt',sep=',',names=['x','y','z','I','i','px','py','rpx','rpy','alpha','Im','F'])
         self.cen = pd.read_csv(self.out+'cenloc.txt',sep=',',names=['px','py','m','n'])
         self.xyz = pd.read_csv(self.out+'xyz.txt',sep=',',names=['x','y','z','I','u0','px','py','F','alpha','Im','u1'])
         self.hkl = pd.read_csv(self.out+'hkl.txt',sep=',',names=['h','k','l','I','i','F','L'])
         self.kin = pd.read_csv(self.out+'cif.txt',sep=',',names=['id','u','v','w','prec','alpha','beta','omega','scale'])
         self.dyn = pd.read_csv(self.out+'dyn.txt',sep=',',names=['id','u','v','w','prec','alpha','beta','omega','scale'])
         self.HKL = pd.read_csv(self.out+'HKL.txt',sep=',',names=['h','k','l','I','sig','F'])
         self.HKL_dyn = pd.read_csv(self.out+'HKL_dyn.txt',sep=',',names=['h','k','l','I','sig','F'])
         self.A   = np.load(self.out+'UB.npy')
+        self.UB  = self.A
         self.lat_params = np.loadtxt(self.out+'cell.txt')[:-1]
         self.lat = np.array(Lattice.from_parameters(*self.lat_params).lattice_vectors)
         self.invA = np.linalg.inv(self.A)
 
         self.cif = [self.kin,self.dyn][dyn]
         uvw   = self.cif[['u','v','w']].values
+
         beams = self.lat.T.dot(uvw.T).T
+
         self.uvw   = uvw #/np.linalg.norm(uvw,axis=1)[:,None]
-        self.uvw0  = beams/np.linalg.norm(beams,axis=1)[:,None]
+        self.uvw0  = -beams/np.linalg.norm(beams,axis=1)[:,None]
         self.beams = self.K0*self.uvw0 #/np.linalg.norm(beams,axis=1)
         self.XYZ   = self.xyz[['x','y','z']].values.T
 
         self._add_hkl(self.rpl)
         self._add_hkl(self.cor)
         self._add_hkl(self.xyz)
 
@@ -104,22 +149,216 @@
         self.hkl['rq'] = rq
 
         # hkl = [str(tuple(h)) for h in self.xyz[['h','k','l']].values]
         # hkl0,idx,cc=np.unique(hkl,return_index=True,return_counts=True)
         # if not len(hkl)==idx.shape[0]:print('warning reflection not unique : ',hkl0[cc>1])
         # self.xyz.index=hkl
 
+        # beams = self.lat.T.dot(dyn.uvw.T).T
+        # self.dyn[['u0','v0','w0']] = beams/np.linalg.norm(beams,axis=1)[:,None]
+
         if dyn:
             hkl,idx=np.unique([str(tuple(h)) for h in self.HKL_dyn[['h','k','l']].values],return_index=True)
             self.HKL_dyn=self.HKL_dyn.iloc[idx]
             self.HKL_dyn.index=hkl
             hkl = self.HKL_dyn[['h','k','l']].values
             self.HKL_dyn['rq'] = np.linalg.norm(hkl.dot(self.lat_vec1),axis=1)
 
 
+    def load_b0(self):
+        return ut.load_pkl(self.b0_path)
+
+    def run_blochwave(self,F,**bargs):
+        Nmax = self.HKL_dyn[['h','k','l']].max().max()
+        self.dyn.set_index('id')
+        u = self.dyn.loc[F,['u','v','w']].values
+
+        u0 = self.lat_vec.T.dot(u)
+        u0 /= np.linalg.norm(u0)
+
+        b_args=dict(Nmax=Nmax,Smax=0.05,path=self.dyngo_path,
+            opts='',name='b_F%d' %F,solve=True)
+        b_args.update(bargs)
+        b0 = bloch.Bloch(self.cif_file,keV=200,
+            u=-u0,**b_args)
+        self.b0_path=b0._get_pkl()
+        return b0
+
+    def make_eldyn(self,
+            sgmax=1,sslim=0.01, outputsgmax=0.1,
+            outputprecfrac=0.6,phisteps=50,F=1,
+            thickness=920.9828,F0=0,bargs={},
+            thr=8,path=None,
+            v=0):
+        ''' Produces a <structure>.eldyn file
+        '''
+
+        UB        = self.A
+        lam       = self.lam
+        pets_dat  = self.dyn.loc[F]
+        hklz      = pets_dat[['u','v','w']].values
+        alpha,beta,omega,scale=pets_dat[['alpha','beta','omega','scale']]
+        phi       = self.dyn.loc[F+1,'alpha']-alpha
+        xnorm, ynorm, keys = 0,0,1000
+
+        #### reflections
+        self.HKL_dyn.index = [str(tuple(h)) for h in self.HKL_dyn[['h','k','l']].values]
+        # hkls = self.HKL_dyn[['h','k','l','I','sig']].copy()
+        # Nmax = self.HKL_dyn[['h','k','l']].max().max()
+
+        structure = os.path.dirname(self.cif_file)[:-4]
+        if not isinstance(path,str):
+            path = os.path.join(self.path,'dyngo')
+        if not os.path.exists(path):os.mkdir(path)
+        eldyn_file=os.path.join(path,'%s.eldyn' %structure)
+        self.dyngo_path=path
+        ###
+        if v:print('...getting structure factor from bloch module...')
+        b0=self.run_blochwave(F,**bargs)
+        # b_args=dict(Nmax=Nmax,Smax=0.05,path=path,opts='',
+        #     name='b_F%d' %F,solve=True)
+        # b_args.update(bargs)
+        # b0 = bloch.Bloch(self.cif_file,keV=200,
+        #     u=-hklz,**b_args)
+        # self.b0_path=b0._get_pkl()
+
+        # Fhkl = b0.Fhkl
+        # V0_idx = np.array([2*Nmax]*3)
+        # Fhkl[tuple(V0_idx)] = 0
+        print('...getting all hkls...')
+        hkls = pd.DataFrame(columns=['h','k','l','A','B','F','I','sig'],
+            index=[ str(tuple(hkl)) for hkl in np.vstack([ i.flatten() for i in b0.hklF]).T],
+            )
+
+        Fhkl = b0.Fhkl.flatten()
+        # Fhkl = np.array([ Fhkl[tuple(hkl_G+V0_idx)]
+        #     for hkl_G in hkls[['h','k','l']].values ])
+        hkls[['h','k','l']] = np.vstack([ i.flatten() for i in b0.hklF]).T
+        hkls['A'] = np.array(Fhkl.real,dtype=float)
+        hkls['B'] = np.array(Fhkl.imag,dtype=float)
+        hkls['F'] = 6
+        hkls['I']   = 0
+        hkls['sig'] = 0
+        # get the reflections to compute the intensities
+        hkl_dyn = self.HKL_dyn[self.HKL_dyn.F==F]
+        idx = hkl_dyn.sort_values('I')[-4:].index ##debug
+        hkls.loc[idx,'F']         = 5
+        hkls.loc[idx,['I','sig']] = hkl_dyn.loc[idx,['I','sig']].values
+        # hkls.drop(str((0,0,0)))
+        hkls = hkls.drop(str((0,0,0)))
+        # print(hkls.loc[str((0,0,0))])
+        print(hkls.loc[idx,'I'])
+
+        fmt0 = lambda x,s,n:(('%'+str(s)+'f') %x).rjust(n)
+        fmt  = lambda x:fmt0(x,6,12)
+
+        # hkls=[
+        #     [1,-2,-1, 0.1,0.2,0.3,0.4, 3,0.1],
+        #     [-3,4,-2, 0.1,0.4,0.5,0.1, 2,0.1],
+        #     ]
+        # df_hkl = pd.DataFrame(hkls,columns=['h','k','l','I1','sig','re','im','d','e'])
+
+
+        header="""int iedt thr %d
+
+Zone# %d
+Noncentrosymmetric         0
+Refinement I
+"""%(thr,F)
+
+        ub='\n'.join(['%s%s%s' %(
+            ('%.6f' %v[0]).rjust(12),
+            ('%.6f' %v[1]).rjust(12),
+            ('%.6f' %v[2]).rjust(12),
+                )
+            for v in UB])
+
+        params = ''.join(fmt(s) for s in
+            [lam,F0,omega,sgmax,sslim, outputsgmax,
+            outputprecfrac]
+            ) + ' %d' %phisteps
+
+        fmt9 = lambda x:fmt0(x,6,9)
+        geo = ''.join([fmt9(s) for s in hklz.tolist()+[alpha,beta,phi]])
+        # '%s %s %s' %(
+        #     ''.join(['%.6f' %x for x in hklz]),
+        #     ''.join(['%.6f' %x for x in [alpha,beta] ]),
+        #     '%.6f' %gamma,
+        #     )
+
+        thick =' '+' '.join([('%1.6f' %x)[:8] for x in [ scale, thickness,xnorm, ynorm]]) + ' '*24 + '%-4d' %keys
+        cor = ' 0.000000 0.000000                                          00'
+
+        msg=''
+        msg+= header
+        msg+= ub        +'\n'
+        msg+= params    +'\n'
+        msg+= geo       +'\n'
+        msg+= thick     +'\n'
+        msg+= cor       +'\n'
+        # msg+=df_hkl.to_csv(float_format='%15.5E',sep='\t',index=False,header=False,line_terminator="\n\n\n")
+        for i,hkl in hkls.iterrows():
+            str_refl = '%s%s%s\n\n\n' %(
+                ''.join(['%4d'    %x for x in hkl[['h','k','l']]]),
+                ''.join(['%15.5E' %x for x in hkl[['I','sig','A','B']]]),
+                ('%d' %hkl['F']).rjust(5) )
+            msg+=str_refl
+        with open(eldyn_file,'w') as f:f.write(msg)
+        if v:
+            print(colors.yellow+eldyn_file+colors.green+" saved"+colors.black)
+            with open(eldyn_file,'r') as f:print(f.read())
+        self.eldyn_file=eldyn_file
+        return eldyn_file
+
+    def run_dyngo(self,bin='dyngo/dyn'):
+        print(check_output('%s %s' %(bin,self.eldyn_file),
+            shell=True).decode())
+
+    def get_edout(self,F=1,opts='a',v=0):
+        #reformat output properly into a file
+        edout = self.eldyn_file.replace('eldyn','edout')
+        out = edout.replace('edout','out')
+        cmd = '''\
+    tail --lines=+2  %s | \
+    sed -E "s/ {1,}/ /g" | sed 's/^ //' | \
+    awk '{getline b; getline c;printf("%%s %%s %%s\\n",$0,b,c)}' |\
+    sed "s/ /,/g" | sed "s/,$//" > %s''' %(edout,out)
+        # print(cmd)
+        print(check_output(cmd,shell=True).decode())
+
+        #import data
+        df = pd.read_csv(out,sep=',',names=['h','k','l','I'] + ['I_%d' %i for i in range(6)],
+            index_col=None)
+
+        print(check_output('rm %s' %out,shell=True).decode())
+        # df[['h','k','l']]=np.array(df[['h','k','l']].values,dtype=int)
+        df.index=[str(tuple(h)) for h in df[['h','k','l']].values]
+
+        if 'a' in opts:
+            df_allint=self.read_allint(F)
+            df['Sw']=np.nan
+            df.loc[df_allint.index,'Sw']=df_allint.Sw
+
+        self.HKL_dyn.loc[df.index,'Icalc'] = df.I
+        if v:
+            print(self.HKL_dyn.loc[df.index,['I','Icalc']])
+        self.save()
+        return df
+
+    def read_allint(self,F,opt=''):
+        '''excitation errors from dyngo'''
+        all_int =self.eldyn_file.replace('.eldyn','_%s.allint' %str(F).zfill(3))
+        if os.path.exists(all_int) :
+            ##the ones that made it to the int>deps
+            df_allint = pd.read_csv(all_int,sep=' +',
+                names=['h','k','l','I','S1','S2','Sw','F'],engine='python')
+            df_allint.index=[str(tuple(h)) for h in df_allint[['h','k','l']].values]
+            if not 'O' in opt:df_allint=df_allint.drop(str((0,0,0)))
+            return df_allint
+
     ###########################################################################
     #### compute :
     ###########################################################################
     def integrate_rpl(self,frames,cond='(I>10)',npx=10):
         """Perform manual integration"""
         if isinstance(frames,int):frames=np.array(frames)
         cond += ' & (F in %s) ' %str(list(frames))
@@ -591,30 +830,29 @@
         plts  = [ [[0,ai[0]],[0,ai[1]],[0,ai[2]],c,'$%s$' %l]  for i,(ai,c,l) in enumerate(zip(lab,['r','g','b'],['x','y','z'])) ]
         # plts += [ [[0,ai[0]],[0,ai[1]],[0,ai[2]],[c,'--'],'$%s$' %l]  for i,(ai,c,l) in enumerate(zip(cry,['r','g','b'],['a','b','c'])) ]
         x0,y0,z0 = [0.5]*3
         plts += [ [[x0,ai[0]+x0],[y0,ai[1]+y0],[z0,ai[2]+z0],[c,'--'],'$%s^{*}$' %l]  for i,(ai,c,l) in enumerate(zip(cr2,['r','g','b'],['a','b','c'])) ]
         # dsp.stddisp(plts,rc='3d',view=[0,0],name='figures/glycine_orient.png',opt='sc')
 
 
-
-
-
 def gauss2D(X, amp, x0, y0, sx,sy,noise):
     x,y = X
     g = noise + amp*np.exp(-((x-x0)/sx)**2 - ((y-y0)/sy)**2)
     return g
 f_gauss2D = lambda X,amp,x0,y0,sx,sy,noise:gauss2D(X,amp, x0, y0, sx,sy,noise).ravel()
 
 
 
 
 def make_pets(pts_file:str,
     aperpixel:float,alphas:Sequence[float]=None,
     deg:float=None,
     ref_cell:Sequence[float]=None,
+    pxy:Optional[tuple] = (256,)*2,
+    dmM:Optional[tuple] = (0.05,3),
     tag:Optional[str]=''):
     """creates a .pts file from info to process a simulated experiment with pets
 
     Parameters
     ----------
     pts_file
         full path to the pts file to write
@@ -627,43 +865,48 @@
     tag
         tag for the tiff images if there is one
     """
     center,pixel_size='AUTO',0.01
     if not deg:deg=alphas[1]-alphas[0]
     phi,omega= deg/2 ,0
     ax,by,cz,alpha,beta,gamma = ref_cell
+    px,py = pxy
+    dm,dM = dmM
     # ax,by,cz,alpha,beta,gamma = 8.1218, 9.977, 17.725, 90.0, 90.0, 90.0
     pts = '''lambda 0.025080
 geometry continuous
 omega  %d
 phi  %.5f
 virtualframes   7 5 1
 
 aperpixel    %.6f
 noiseparameters      2.5000      1.0000
 saturationlimit   20000
 
-center    256.0 256.0
+center    %s %s
 centermode friedelpairs 0
 
 beamstop no
 
-dstarmax  3.0
-dstarmaxps  3.0
+
+dstarmax  3
+dstarmaxps  %s
+dstarmin  %s
 i/sigma    7.00    5.00
 reflectionsize  7
 
 referencecell     %.5f    %.5f     %.5f    %.5f   %.5f    %.5f 1
 
 #List of images
 #columns: file name,alpha,beta,delta omega,frame scale,calibration correction(px/rec.angstrom),ellipt.distortion correction(amplitude),ellipt.distortion correction(phase), use for calculations(0/1)
 imagelist
-'''%(omega,phi,aperpixel,  ax,by,cz,alpha,beta,gamma)
+'''%(omega,phi,aperpixel,px,py,dM,dm,  ax,by,cz,alpha,beta,gamma)
     out = os.path.dirname(pts_file)
     tif_files = np.sort(glob.glob(out+'/tiff/%s*.tiff' %tag))
+    # print(tif_files)
     if type(alphas)==type(None):
         alphas = np.arange(tif_files.size)*deg
 
     for i,tif_file in enumerate(tif_files):
         tif_file = os.path.basename(tif_file)
         pts+='%s %.4f 0.0 0.0 1.0 0 0 0  1\n' %('tiff\\'+tif_file,alphas[i])
     pts+='endimagelist\n'
```

### Comparing `ccp4ED-1.0.9/EDutils/pets_ref.sh` & `ccp4ED-1.1.0/EDutils/pets_ref.sh`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/EDutils/rotate_exp.py` & `ccp4ED-1.1.0/EDutils/rotate_exp.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import tifffile,os,glob,pickle5,subprocess
 import numpy as np,pandas as pd
 from typing import TYPE_CHECKING, Dict, Iterable, Optional, Sequence, Union
 from utils import displayStandards as dsp   #;imp.reload(dsp)
 from utils import glob_colors as colors     #;imp.reload(colors)
 from utils import handler3D as h3D          #;imp.reload(h3D)
 from scipy.integrate import trapz
-from . import utilities as ut               ;imp.reload(ut)
+from . import utilities as ut               #;imp.reload(ut)
 
 class Rocking:
     def __init__(self,Simu:object,
             uvw:list,tag:str,path:str,
             Sargs:dict):
         """ simulate rocking curve
 
@@ -148,15 +148,42 @@
             df_Imax = pd.DataFrame.from_dict({h:Ib[:,0].max() for h,Ib in I.items()},orient='index',columns=['I'])
             hkls = df_Imax.sort_values('I',ascending=False)[:n].index
             I = {h:I[h] for h in hkls}
 
         z = self.load(0).z.copy()[iZs]
         return z,I
 
+    def integrate(self,thick=None):
+        if not thick:
+            return self._integrate_all()
+        else:
+            return self._integrate_thick(thick)
 
+    def _integrate_thick(self,thick):
+        b0 = self.load(0)
+        if not b0.thick==thick:
+            self.do('set_thickness',thick=thick)
+        df_int = pd.DataFrame(0,index=self.beams.index,columns=['I'])
+        for i in range(self.n_simus):
+            b0 = self.load(i)
+            df_int.loc[b0.df_G.index,'I'] += b0.df_G.I
+        # self.save()
+        return df_int
+
+    def _integrate_all(self,z):
+        b0 = self.load(0)
+        thicks=['%.1fA' %z for z in b0.z ]
+        self.z=b0.z
+        self.df_int = pd.DataFrame(0,index=self.beams.index,columns=thicks)
+
+        for i in range(self.n_simus):
+            b0 = self.load(i)
+            self.df_int.loc[b0.df_G.index] += b0.Iz
+        self.save()
+        # print(self.z.shape,self.df_int.values.shape)
     ###########################################################################
     #### Display
     ###########################################################################
     # def QQplot(self,zs=None,iZs=10,refl=[],cond='',
     #     int_opt=True,cmap='Spectral',**kwargs):
     #     if int_opt:self.integrate_rocking(refl,cond)
     #     iZs,nzs  = self._get_iZs(iZs,zs)    #;print(iZs)
@@ -429,14 +456,15 @@
         i
             index of the simu
         ts
             value
         """
         i,ts = self._get_ts(i,ts)
         file = self.df.iloc[i].pkl
+        # file = os.path.join(self.path,os.path.basename(self.df.iloc[i].pkl))
         sim_obj = ut.load_pkl(file)
         return sim_obj
 
     def do(self,f,v=True,**args):
         """ apply function to all simus
         """
         for i in range(self.df.shape[0]):
```

### Comparing `ccp4ED-1.0.9/EDutils/sandbox/convert.py` & `ccp4ED-1.1.0/EDutils/sandbox/convert.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/EDutils/sandbox/test.py` & `ccp4ED-1.1.0/EDutils/sandbox/test.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/EDutils/utilities.py` & `ccp4ED-1.1.0/EDutils/utilities.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import numpy as np,pandas as pd
 from typing import TYPE_CHECKING, Dict, Iterable, Optional, Sequence, Union
 from crystals import Crystal
 from utils import displayStandards as dsp   #;imp.reload(dsp)
 from utils import glob_colors as colors     #;imp.reload(colors)
 # from utils import handler3D as h3D          #;imp.reload(h3D)
 # from . import rotate_exp as exp ;imp.reload(exp)
+import gemmi
 
 def sweep_var(Simu:object,
         params:Sequence[str],vals:Sequence[Sequence],
         tag:str='',path:str='',
         **kwargs,
     ):
     """runs a set of similar simulations Simu with a varying parameter
@@ -76,21 +77,39 @@
 
 def save(obj,file=None,path='',name='unkown.pkl'):
     """save an object"""
     file = get_pkl(file,path,name)
     with open(file,'wb') as out :
         pickle5.dump(obj, out, pickle5.HIGHEST_PROTOCOL)
     print(colors.green+"object saved\n"+colors.yellow+file+colors.black)
+def save_pkl(obj,file):
+    save(obj,file=file)
 
 def load_pkl(file):
     """load an object"""
     with open(file,'rb') as f : obj = pickle5.load(f)
     return obj
 
+def rot(a,axis='x',deg=True):
+    if deg:a = np.deg2rad(a)
+    c,s = np.cos(a),np.sin(a)
+    if   axis=='x':R = np.array([[1,0,0],[0,c,s],[0,-s,c]])
+    elif axis=='y':R = np.array([[c,0,s],[0,1,0],[-s,0,c]])
+    elif axis=='z':R = np.array([[c,s,0],[-s,c,0],[0,0,1]])
+    return R
+
+def rotation_matrix(k,a,deg=True):
+    '''Rotation matrix from a vector'''
+    #https://en.wikipedia.org/wiki/Rodrigues%27_rotation_formula
+    if deg:a = np.deg2rad(a)
+    kx,ky,kz = k
+    K = np.array([[0,-kz,ky],[kz,0,-kx],[-ky,kx,0]])
+    R = np.eye(3) + np.sin(a)*K + (1-np.cos(a))*K.dot(K)
 
+    return R
 #############################################################################
 #### orientation vectors
 #############################################################################
 def get_uvw_cont(u0:Sequence,u1:Sequence,nframes:int=2,show:bool=False,**kwargs):
     """get a list of orientation vectors in a continuously rotated fashion between u0 and u1.
 
     Parameters
@@ -298,30 +317,96 @@
 
 def find_cif_file(path,cif_file=None):
     """find cif file in path"""
     if not cif_file:
         cif_file = _find_files(path,'cif')
     return cif_file
 
-def pdb2npy(pdb,cif_file=''):
+def pdb2npy(pdb,npy_file=''):
     crys=crystals.Crystal.from_pdb(pdb)
     Zxyz=np.array([
         np.array([a.atomic_number,a.coords_fractional%1],dtype=object)
             for a in crys],dtype=object)
-    if not cif_file: cif_file=pdb+'.npy'
-    np.save(cif_file,np.array([Zxyz ,crys.lattice_vectors],dtype=object))
+    if not npy_file: npy_file=pdb+'.npy'
+    np.save(npy_file,np.array([Zxyz ,crys.lattice_vectors],dtype=object))
+    print(colors.green+'file saved : '+colors.yellow+npy_file+colors.black)
+    return npy_file
 
 def import_npy(npy_file):
     (Zxyz,lat) = np.load(npy_file,allow_pickle=True)
     crys=crystals.Crystal(
         crystals.AtomicStructure([
             crystals.Atom(element=Z,coords=xyz) for Z,xyz in Zxyz]),
         lat)
     return crys
 
+def crys2felix(crys,opt='wr',out=None):
+    # crys = Crystal.from_cif(cif_file)
+    cif = """_chemical_formula_sum '%s'
+loop_
+_cell_length_a %.5f
+_cell_length_b %.5f
+_cell_length_c %.5f
+_cell_angle_alpha %.3f
+_cell_angle_beta %.3f
+_cell_angle_gamma %.3f
+_symmetry_Int_Tables_number %d
+_symmetry_space_group_name_Hall '%s'
+loop_
+_atom_site_label
+_atom_site_type_symbol
+_atom_site_fract_x
+_atom_site_fract_y
+_atom_site_fract_z
+_atom_site_B_iso_or_equiv
+_atom_site_occupancy
+""" %(
+        crys.chemical_formula,*crys.lattice_parameters,
+        crys.international_number,crys.hall_symbol)
+    cif += '\n'.join([
+        "%s %s %.5f %.5f %.5f 0.1 1" %("%s%d" %(a.element,i), a.element,*a.coords_fractional)
+            for i,a in enumerate(crys.atoms) if all(a.coords_fractional<0.99)
+        ])
+
+    if not out:out='felix.cif'
+    if 'w' in opt:
+        with open(out,'w') as f : f.write(cif)
+        print(colors.yellow+out+colors.green+" successfully created."+colors.black)
+    if 'r' in opt:
+        if 'w' in opt:
+            print(colors.blue+"Content of "+ colors.yellow +out+colors.black)
+            with open(out,'r') as f : print(''.join(f.readlines()))
+        else:
+            print(cif)
+
+def gemmi_sf(pdb_file:str='',dmin=2):
+    st = gemmi.read_structure(pdb_file)
+    dc = gemmi.DensityCalculatorX()
+    dc.d_min = dmin
+    dc.addends.subtract_z()
+    dc.set_grid_cell_and_spacegroup(st)
+    dc.set_refmac_compatible_blur(st[0])
+    dc.put_model_density_on_grid(st[0])
+    grid = gemmi.transform_map_to_f_phi(dc.grid); print('sf : ',grid.shape)
+    Nmax = (np.array(grid.shape)//2-1).min()
+    Fhkl = np.zeros((2*Nmax+1,)*3,dtype=complex)
+    hklF = np.meshgrid(*[np.arange(-Nmax,Nmax+1)]*3)
+    hkls = np.array([i.flatten() for i in hklF]).T
+    idxs = np.array([i.flatten() for i in np.meshgrid(*[np.arange(2*Nmax+1)]*3)]).T
+    #TODO : multiple size grid
+    # nu2,nv2,nw2 = np.array(grid.shape)//2-1
+    # Fhkl = np.zeros((2*nu2+1,2*nv2+1,2*nw2+1),dtype=complex)
+    # hkls=np.array([i.flatten() for i in np.meshgrid(range(-nu2,nu2+1),range(-nv2,nv2+1),range(-nw2,nw2+1))]).T
+    # idxs=np.array([i.flatten() for i in np.meshgrid(range(2*nu2+1),range(2*nv2+1),range(2*nw2+1))]).T
+    # hkls = pd.DataFrame()
+    print(colors.blue+'...filling...'+colors.black)
+    for idx,hkl in zip(idxs,hkls):
+        Fhkl[tuple(idx)] = dc.mott_bethe_factor(hkl) * grid.get_value(*hkl)
+    return hklF,Fhkl
+
 def import_crys(file:str=''):
     """import a Crystal
 
     Parameters
     ----------
     file
         can be a cif file or a builtin
@@ -483,14 +568,22 @@
 
     Fhkl_0 = df_Sw['Fhkl'].values
     I  = (np.abs(Fhkl_0)*gs)**2
     df_Sw['I'] = I
     return df_Sw
 
 def project_beams(K,qxyz,e0=[1,0,0],v=0):
+    '''pass from reciprocal cartesian coordinates to panel coordinates
+    then uses the `aper` parameter to get values in pixels
+    e0:rotation axis in the panel frame
+    Note:
+        In the images frame, the beam in perpendicular to the images(z axis)
+        and the rotation axis is usually along the x axis of the images
+    '''
+    #build the frames basis
     e3 = K/np.linalg.norm(K)
     e0 = e0/np.linalg.norm(e0)
     e2 = np.cross(e3,e0)
     e1 = np.cross(e2,e3)
 
     px,py = qxyz.dot(e1),qxyz.dot(e2)
     if v:
@@ -515,7 +608,23 @@
     return refl
 
 def show_tiff(file,cutoff=100):
     import tifffile
     im=tifffile.imread(file)
     dsp.stddisp(im=[im],title=file,
         cmap='gray',caxis=[0,cutoff],pOpt='tX')
+
+
+def to_shelx(hkl,file):
+    '''converts to a.hkl file ready to use by shelx
+    hkl: dataframe containing h,k,l,I,sig
+    '''
+    formats = {
+        'h':'{:>4}', 'k':'{:>4}', 'l':'{:>4}',
+        'I':'{:>8.2f}', 'sig':'{:>8}',
+        }
+    formatters = {k: v.format for k, v in formats.items()}
+    content=hkl.to_string(formatters=formatters, index=False, header=False)
+    with open(file, 'w') as f:
+        f.write(content)
+
+    print(colors.green+'file saved : \n'+colors.yellow,file,colors.black)
```

### Comparing `ccp4ED-1.0.9/EDutils/viewers.py` & `ccp4ED-1.1.0/EDutils/viewers.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/PKG-INFO` & `ccp4ED-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccp4ED
-Version: 1.0.9
+Version: 1.1.0
 Summary: Electron diffraction utilities
 Home-page: https://pypi.org/project/ccp4ED
 Author: Tarik Ronan Drevon
 Author-email: tarik.drevon@stfc.ac.uk
 License: UNKNOWN
 Project-URL: Documentation, https://debloch.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/ccp4/electron-diffraction
```

### Comparing `ccp4ED-1.0.9/README.md` & `ccp4ED-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/blochwave/bloch.py` & `ccp4ED-1.1.0/blochwave/bloch.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """Bloch wave solver"""
 import importlib as imp
-import numpy as np,pandas as pd,pickle5,os,glob,tifffile
+import numpy as np,pandas as pd,pickle5,os,glob,tifffile,mrcfile
 from typing import TYPE_CHECKING, Dict, Iterable, Optional, Sequence, Union
-from subprocess import check_output#Popen,PIPE
+from subprocess import check_output,Popen,PIPE
 from crystals import Crystal
 from utils import displayStandards as dsp           #;imp.reload(dsp)
 from utils import physicsConstants as cst           #;imp.reload(cst)
 from utils import glob_colors as colors,handler3D as h3d
 from multislice import postprocess as pp            #;imp.reload(pp)
 from scattering import structure_factor as sf       #;imp.reload(sf)
 from scattering import scattering_factors as scatf  #;imp.reload(scatf)
 from EDutils import viewers                         #;imp.reload(viewers)
 from EDutils import utilities as ut                 #;imp.reload(ut)
+from EDutils import pets as pt                      ;imp.reload(pt)
 from EDutils import display as EDdisp               ;imp.reload(EDdisp)
 from . import util as bloch_util                    ;imp.reload(bloch_util)
+felix='%s/bin/felix' %os.path.dirname(__file__)
 
 class Bloch:
     """
     Bloch wave simulation class
 
     Parameters
     ---------
@@ -35,43 +37,56 @@
         beam direction [ux,uy,uz] in reciprocal space (see :meth:`~Bloch.set_beam`)
     Nmax
         max order of reflections/resolution (see :meth:`~Bloch.update_Nmax`)
     Smax
         maximum excitation error (see :meth:`~Bloch.solve`)
     solve
         solve the system by diagonalizing the Bloch matrix
+    felix
+        Use felix solver
+    nbeams
+        Number of beams to use (using felix only)
     kwargs
         arguments to be passed to :meth:`~Bloch.solve`
     """
     def __init__(self,
         cif_file:str,name:str='',path:str='',
         beam:Optional[dict]={},keV:float=200,u:Sequence[float]=[0,0,1],
-        Nmax:int=1,
+        Nmax:int=1,dmin:int=None,
         Smax:float=0.2,
         solve:bool=True,
+        felix:bool=False,nbeams:int=200,
         eps:float=1,
         **kwargs,
     ):
         self.solved = False
         self.Nmax   = 0
         self.thick  = 100
         self.thicks = self._set_thicks((0,1000,1000))
         self.eps=eps
 
         self._set_structure(cif_file)
-        self.update_Nmax(Nmax)
         beam_args={'keV':keV,'u':u}
         beam_args.update(beam)
         self.set_beam(**beam_args)
         self.set_name(name,path)
-        self._set_excitation_errors(Smax)
-        self._set_Vg()
+        self.nbeams=nbeams
+
+        if solve :
+            self.solve(Smax=Smax,Nmax=Nmax,dmin=dmin,**kwargs)
+        else:
+            if not felix:
+                print(colors.blue+'...Nmax... '+colors.black)
+                self.update_Nmax(Nmax,dmin)
+                print(colors.blue+'...Excitation errors... '+colors.black)
+                self._set_excitation_errors(Smax)
+                print(colors.blue+'...Vg... '+colors.black)
+                self._set_Vg()
+        self.save()
 
-        if solve:
-            self.solve(Smax=Smax,**kwargs)
         # if show_thicks or 't' in opts:
         #     self.show_beams_vs_thickness(strong=['I'])
         # if 's' in opts:
         #     self.save()
 
 
     def set_name(self,name='',path=''):
@@ -92,30 +107,56 @@
         basefile = self.cif_file.replace('.cif','')
         if not name:
             u_str = ''.join(['%d' %np.round(u) for u in self.Kabc0])
             name='%s%s_%dkeV_bloch' %(os.path.basename(basefile),u_str,np.round(self.keV))
         if not path:path=os.path.dirname(basefile)
         self.path = path                #; print(self.path)
         self.name = name                #;print('name:',self.name)
+        if self.pdb_file:
+            check_output('mv %s %s' %(self.cif_file,self.path),shell=True)
 
-    def update_Nmax(self,Nmax:int):
+    def update_Nmax(self,Nmax:int,dmin:int=None):
         """
         Update resolution/max order (lattice and Fhkl)
 
         Parameters
         ----------
         Nmax
             maximum h,k,l order
+        dmin
+            minimum resolution
         """
-        if type(Nmax) in [int,np.int64] :
-            if not Nmax==self.Nmax:
-                self.Nmax=Nmax
-                (h,k,l),(qx,qy,qz) = ut.get_lattice(self.lat_vec,self.Nmax)
-                self.lattice = [(h,k,l),(qx,qy,qz)]
-                self.hklF,self.Fhkl = sf.structure_factor3D(self.pattern, 2*np.pi*self.lat_vec,hklMax=2*self.Nmax)
+
+        if dmin and self.pdb_file:
+            self.hklF,self.Fhkl = ut.gemmi_sf(self.pdb_file,dmin)
+            self.Nmax=np.array(self.Fhkl.shape[0])//4#.min()
+            print('Nmax:',self.Nmax)
+            # gemmi='/home/tarik/Documents/git/github/gemmi/gemmi'
+            # gemmi_cmd="%s sfcalc -v --dmin=%.3f --wavelength=%3.f --for=mott-bethe %s | " %(gemmi,dmin,self.lam,crys)
+            # print(gemmi_cmd)
+            # sed_cmd = r"sed 's/^ //' | sed 's/ /,/g' >>sf.txt"
+            # sf = check_output("%s | %s " %(gemmi_cmd,sed_cmd) ,shell=True).decode()
+            # df = pd.DataFrame('sf.txt',delimiter='\t',index_col=0,names=['index','A','phi'])
+            # sf = check_output("rm sf.txt",shell=True).decode()
+            # df['F'] = df.A*np.exp(1J*np.deg2rad(df.phi))
+            # df[['h','k','l']]=list(map(lambda s:list(eval(s)),df.index))
+            # df[['qx','qy','qz']] = df[['h','k','l']].values.dot(self.lat_vec0)
+            # df['q'] = np.linalg.norm(df[['qx','qy','qz']],axis=1)
+            # df['res']=1/df.q
+
+        else:
+            if type(Nmax) in [int,np.int64] :
+                if not Nmax==self.Nmax:
+                    self.Nmax=Nmax
+                    idx = [i for i,x in enumerate(self.pattern[:,:3]) if all(x<0.99)]
+                    self.pattern=self.pattern[idx,:]
+                    self.hklF,self.Fhkl = sf.structure_factor3D(self.pattern,
+                        2*np.pi*self.lat_vec,hklMax=2*self.Nmax)
+        (h,k,l),(qx,qy,qz) = ut.get_lattice(self.lat_vec,self.Nmax)
+        self.lattice = [(h,k,l),(qx,qy,qz)]
 
     def set_beam(self,
         keV:float=200,
         # lam:float=None,
         u:Sequence[float]=[0,0,1],
         K:Optional[Sequence[float]]=None,
         u0:Optional[Sequence[int]]=None,
@@ -170,144 +211,211 @@
         if self.solved:
             self._set_intensities()
             print('updated intensities')
 
 
     def solve(self,
         Smax:Optional[float]=None,hkl:Optional[Iterable[int]]=None,
-        Nmax:Optional[int]=None,
-        beam:Optional[dict]={},
+        Nmax:Optional[int]=None,dmin:Optional[int]=None,
+        beam:Optional[dict]={},dyngo_args:Optional[dict]={},
         thick:float=None,thicks:Sequence[float]=None,
         opts:str='sv0',
+        felix:bool=False,
+        nbeams:int=None,
     ):
         """ Diagonalize the Blochwave matrix
 
         Parameters
         ----------
         Smax
             maximum excitation error to be included
         hkl
             Beams to include
         Nmax
             max order of reflections/resolution (see :meth:`~Bloch.update_Nmax` )
         beam
             dictionary passed to :meth:`~Bloch.set_beam`
-
+        dyngo_args
+            dict contain dyngo type informations. If not empty, it solves  with Dyngo formulation which is slightly different.
         thick
             thickness of crystal (can be modified without resolving)
         thicks
             range of thickness [z_min,z_max,z_step]
         opts
             s(save) t(show intensities) z(show beam vs thickness) 0(Vopt0) v(verbose) H(show H)
-
+        felix
+            use felix solver
+        nbeams
+            Number of beams when using felix solver
 
         .. note ::
 
             If hkl is specified, Smax is not taken into account
         """
-        if Nmax : self.update_Nmax(Nmax)
-        if beam : self.set_beam(**beam)
-        if Smax or isinstance(hkl,np.ndarray):
-            self._set_excitation_errors(Smax,hkl)
-            self._set_Vg()
-        self._solve_Bloch(show_H='H' in opts,Vopt0='0' in opts,v='v' in opts)
+        if felix:
+            self._prepare_Felix(nbeams=nbeams)
+            self._run_felix() #wait='w' in opts)
+            self._postprocess_felix(show_log='v' in opts)
+            self._set_excitation_errors(hkl=self.df_G[['h','k','l']].values,felix=True)
+            self._set_Vg(felix=True)
+        else:
+            if Nmax or dmin :self.update_Nmax(Nmax,dmin)
+            if beam : self.set_beam(**beam)
+            if Smax or isinstance(hkl,np.ndarray):
+                self._set_excitation_errors(Smax,hkl)
+                self._set_Vg()
+            self._solve_Bloch(show_H='H' in opts,Vopt0='0' in opts,v='v' in opts,
+                dyngo_args=dyngo_args)
         ##### postprocess
         if thick or 't' in opts:
             self.set_thickness(thick)
         if not type(thicks)==type(None) and 'z' in opts:
             self._set_beams_vs_thickness(thicks)#;print('thicks solved')
         if 's' in opts:
             self.save()
 
+    def update(self,keV=None,u=None,Smax=None,Nmax=None,dmin=None,
+            gemmi=False,hkl=None,**kwargs):
+        if not gemmi:dmin=None
+        self.set_beam(keV=keV,u=u)
+        if Nmax or dmin :self.update_Nmax(Nmax,dmin)
+        if Smax or isinstance(hkl,np.ndarray):
+            self._set_excitation_errors(Smax,hkl)
+            self._set_Vg()
+        self.save()
+
     ################################################################################
     #### private
     ################################################################################
-    def _solve_Felix(self,felix_cif,npx=20,nbeams=200,thicks=(10,250,10),show_log=False):
-        felix='%s/bin/felix' %os.path.dirname(__file__)
-        if not os.path.exists(felix):
-            print('Running with Felix not available. You need to install felix in %s :')
-            print(felix)
-
-        inp = bloch_util.get_inp(npx,nbeams,self.u,self.keV,thicks)
-        with open("%s/felix.inp" %self.path,'w') as f:f.write(inp)
-
+    def _prepare_Felix(self,npx=20,nbeams=None,thicks=(0,0,20),show_log=False):
+        """"""
+        if not nbeams:nbeams=self.nbeams
         print(colors.blue+"preparing simulation"+colors.black)
         cmd="""cd %s;
         if [ ! -d felix ];then mkdir felix;fi;
-        cp %s felix/felix.cif;
-        mv felix.inp felix;
-        """ %(self.path,os.path.realpath(felix_cif))
+        """ %(self.path) #,os.path.realpath(felix_cif))
+        # cp %s felix/felix.cif;
+        # mv felix.inp felix;
         # p=Popen(cmd,shell=True)#;p.wait();o,e = p.communicate();if e:print(e)
         p=check_output(cmd,shell=True).decode();print(p)
+        bloch_util.get_inp(npx,nbeams,self.u,self.keV,thicks,out=os.path.join(self.path,'felix','felix.inp'))
+        ut.crys2felix(self.crys,opt='w',out=os.path.join(self.path,'felix','felix.cif'))
+
+    def _run_felix(self,wait=True):
+        if not os.path.exists(felix):
+            print('Error : Running with Felix not available. You need to install felix in %s :' )
+            print(felix)
+            return
 
         print(colors.blue+"... running felix ..."+colors.black)
         cmd="""cd %s;
         cd felix;
         %s > felix.log 2>&1;
         """ %(self.path,felix)#os.path.dirname(__file__))
-        p=check_output(cmd,shell=True).decode() #;print(p)
+        p=Popen(cmd,shell=True,stdout=PIPE,stderr=PIPE);
+        if wait:
+            p.wait();print(p.communicate())
+        else:
+            return p
 
+
+    def _postprocess_felix(self,show_log=False):
         if show_log:
             print(colors.blue+"felix output"+colors.black)
             with open('%s/felix/felix.log' %self.path,'r') as f:print('\n'.join(f.readlines()))
 
-        g = np.loadtxt(os.path.join(self.path,'felix/eigenvals.txt'))
+        eigvals = os.path.join(self.path,'felix/eigenvals.txt')
+        check_output("sed -i -E 's/ {1,}/,/g' %s;sed -i -E 's/^,//' %s" %(eigvals,eigvals) ,shell=True)
+        df = pd.read_csv(eigvals,names=['h','k','l','gr','gi'])
+        self.gammaj = (df.gr+1J*df.gi).values
+        # g = np.loadtxt(os.path.join(self.path,'felix/eigenvals.txt'))
+        # self.gammaj = g[:,3::2]+1J*g[:,4::2];g=g[:,0]
         C = np.loadtxt(os.path.join(self.path,'felix/eigenvec.txt'))
-        self.gammaj = g[:,3::2]+1J*g[:,4::2];g=g[:,0]
         self.CjG = C[:,3::2]+1J*C[:,4::2]
-        self.invCjG=np.conj(C.T)
+        self.invCjG=np.conj(self.CjG.T)
+
+        self.df_G = df[['h','k','l']]
+        self.df_G.index = [str(tuple(h)) for h in self.df_G.values]
+        self.solved=True
 
-    def _solve_Bloch(self,show_H=False,Vopt0=True,v=False):
+    def _solve_Bloch(self,show_H=False,Vopt0=True,dyngo_args={},v=False):
         ''' Diagonalize the Hamiltonian'''
         # Ug is a (2*Nmax+1)^3 tensor :
         # Ug[l] = [U(-N,-N,l) .. U(-N,0,l) .. U(-N,N,l)
         #          U( 0,-N,l) .. U( 0,0,l) .. U( 0,N,l)
         #          U(-N,-N,l) .. U( N,0,l) .. U( N,N,l)]
+        self.dyngo = any(dyngo_args)
 
         hkl = self.df_G[['h','k','l']].values
         Sg  = self.df_G.Sw.values
-        pre = 1/np.sqrt(1-cst.keV2v(self.keV)**2)
+        if self.dyngo:
+            Rmat=dyngo_args['Rmat']
+            self.scale=dyngo_args['scale']
+            surf_norm = Rmat.dot([0,0,1])
+            gn = Rmat.dot(self.df_G[['qx','qy','qz']].T).T.dot(surf_norm)
+            Knorm = self.k0*surf_norm[-1]
+            self.Knorm=Knorm
+            sqrtkg=np.sqrt(1+gn/Knorm)  #dyngo implementation
+            Sg*=2*self.k0/sqrtkg
 
+        pre = 1/np.sqrt(1-cst.keV2v(self.keV)**2)
         Ug = pre*self.Fhkl/(self.crys.volume*np.pi)*self.eps #/3
 
         #####################
         # setting average potential to 0
         # Ug[U0_idx] = U0
         # and Ug(iG,jG) are obtained from Ug[h,k,l] where h,k,l = hlk_iG-hkl_jG
         #####################
         U0_idx = [2*self.Nmax]*3
         Ug[tuple(U0_idx)] = 0
         # if Vopt0 :Ug[tuple(U0_idx)] = 0   #setting average potential to 0
 
+        print(Ug.shape)
         if v:print(colors.blue+'...assembling %dx%d matrix...' %((Sg.shape[0],)*2)+colors.black)
         H = np.diag(Sg+0J)
         for iG,hkl_G in enumerate(hkl) :
             U_iG = np.array([Ug[tuple(hkl_J+U0_idx)] for hkl_J in hkl_G-hkl]) #;print(V_iG.shape)
             # print('G : ',hkl_G)
             # print('U_G:',Ug[tuple(U0_idx+hkl_G)])
             # print('idx iG:',[tuple(hkl_J+U0_idx) for hkl_J in hkl_G-hkl])
             # print(U_iG)
-            H[iG,:] += U_iG/(2*self.k0)  #off diagonal terms as potential
+            if self.dyngo:
+                # qh = np.linalg.norm(self.lat_vec.T.dot((hkl_G-hkl).T),axis=0)
+                qh = Rmat.dot((hkl_G-hkl).T).T.dot(surf_norm)
+                sqrtkh = np.sqrt(1+qh/Knorm)
+                H[iG,:] += U_iG/(sqrtkg[iG]*sqrtkh)  #so dyngo implementation
+            else:
+                H[iG,:] += U_iG/(2*self.k0)  #off diagonal terms as potential
+
+        if self.dyngo:
+            H/=(2*self.k0)
 
-        self.H = H*2*np.pi #to get same as felix
+        H *= 2*np.pi #to get same as felix
+        self.H=H
         if show_H:self.show_H()
 
         if v:print(colors.blue+'...diagonalization...'+colors.black)
         self.gammaj,self.CjG = np.linalg.eigh(self.H) #;print(red+'Ek',lk,black);print(wk)
         self.invCjG = np.linalg.inv(self.CjG)
         self.solved = True
 
     def _set_structure(self,cif_file):
+        pdb_file = ''
+        if cif_file[-3:]=='pdb':
+            pdb_file=cif_file
+            cif_file = ut.pdb2npy(os.path.basename(cif_file[:-4]))
+
         self.cif_file = cif_file
-        self.crys     = ut.import_crys(cif_file)
+        self.pdb_file = pdb_file
+        self.crys     = ut.import_crys(self.cif_file)
         self.lat_vec0 = np.array(self.crys.lattice_vectors)
         self.lat_vec  = np.array(self.crys.reciprocal_vectors)/(2*np.pi)
         self.pattern  = np.array([np.hstack([a.coords_fractional,a.atomic_number]) for a in self.crys.atoms] )
 
-    def _set_excitation_errors(self,Smax=0.02,hkl=None):
+    def _set_excitation_errors(self,Smax=0.02,hkl=None,felix=False):
         """ get excitation errors for Sg<Smax
         - Smax : maximum excitation error to be included
         - hkl : list of tuple or nbeams x 3 ndarray - beams to be included (for comparison with other programs)
         """
         # print(colors.blue+'... setting excitation error ... '+colors.black)
         K,K0 = self.K,self.k0
         if isinstance(hkl,list) or isinstance(hkl,np.ndarray):
@@ -320,52 +428,62 @@
         Kx,Ky,Kz = K
         # Sw = K0-np.sqrt((Kx+qx)**2+(Ky+qy)**2+(Kz+qz)**2)
         Sw_full = (K0**2-((Kx+qx)**2+(Ky+qy)**2+(Kz+qz)**2))/(2*K0)
         Sw = Sw_full #;print(Sw)
         # Gz  = -( qx*Kx+qy*Ky+qz*Kz)/K0
         # GzG = Gz -(qx**2+qy**2+qz**2)/(2*K0)
         # print(Sw.shape,Gz.shape,GzG.shape)
+        q = np.linalg.norm(np.array([qx,qy,qz]).T,axis=1)
+        if felix:
+            self.df_G[['qx','qy','qz','q','Sw','Swa']] = np.array([qx,qy,qz,q,Sw,abs(Sw)]).T
+            self.df_G['I'] = 0
+            self.df_G.loc[str((0,0,0)),'I'] = 1
+            return
+
         # print('ok')
         if Smax:
             idx = abs(Sw)<Smax
             h,k,l = np.array([h[idx],k[idx],l[idx]],dtype=int)
-            qx,qy,qz,Sw = qx[idx],qy[idx],qz[idx],Sw[idx]#,Swa[idx]
+            qx,qy,qz,q,Sw = qx[idx],qy[idx],qz[idx],q[idx],Sw[idx]#,Swa[idx]
             # Gz,GzG = Gz[idx],GzG[idx]
-        q = np.linalg.norm(np.array([qx,qy,qz]).T,axis=1)
         d = dict(zip(['h','k','l','qx','qy','qz','q','Sw','Swa'],[h,k,l,qx,qy,qz,q,Sw,abs(Sw)]))
 
         self.Smax = Smax
         self.nbeams = Sw.size
         self.df_G = pd.DataFrame.from_dict(d)
         self.df_G.index = [str(tuple(h)) for h in self.df_G[['h','k','l']].values]
         self.solved = False
         self.df_G['I'] = 0
         self.df_G.loc[str((0,0,0)),'I'] = 1
         # print(self.df_G['I'].shape)
 
 
-    def _set_Vg(self):#,opt=0):
+    def _set_Vg(self,felix=0):
         ##### opt was used for testing against FELIX
-        # if opt:
-        #     q    = self.df_G['q']
-        #     hkl  = self.df_G[['h','k','l']].values
-        #     xi   = self.pattern[:,:3].T
-        #     Za   = np.array(self.pattern[:,-1],dtype=int)
-        #     fj   = scatf.get_fe(Za,q) #;fj = 1 #testing exp factor alone
-        #     #### Fhkl[nGs] = sum_{natoms} fj [nGs x natoms] * hkl[nGsx3].dot(xi[3,natoms])
-        #     Fhkl = np.sum(fj*np.exp(-2J*np.pi*hkl.dot(xi)),axis=1)
-        # else:
-        hkl  = self.df_G[['h','k','l']].values
-        Fhkl = self.Fhkl.copy()
-        V0_idx = np.array([2*self.Nmax]*3)
-        Fhkl[tuple(V0_idx)] = 0
-        Fhkl = np.array([ Fhkl[tuple(hkl_G+V0_idx)] for hkl_G in hkl])
+        if felix:
+            q    = self.df_G['q']
+            hkl  = self.df_G[['h','k','l']].values
+            idx = [i for i,x in enumerate(self.pattern[:,:3]) if all(x<0.99)]
+            xi   = self.pattern[idx,:3].T
+            # print(xi)
+            Za   = np.array(self.pattern[idx,-1],dtype=int)
+            fj   = scatf.get_fe(Za,q) #;fj = 1 #testing exp factor alone
+            #### Fhkl[nGs] = sum_{natoms} fj [nGs x natoms] * hkl[nGsx3].dot(xi[3,natoms])
+            Fhkl = np.sum(fj*np.exp(-2J*np.pi*hkl.dot(xi)),axis=1)
+            # print(self.crys,xi)
+        else:
+            hkl  = self.df_G[['h','k','l']].values
+            Fhkl = self.Fhkl.copy()
+            V0_idx = np.array([2*self.Nmax]*3)
+            Fhkl[tuple(V0_idx)] = 0
+            Fhkl = np.array([ Fhkl[tuple(hkl_G+V0_idx)] for hkl_G in hkl])
 
         self.pre = 1/np.sqrt(1-cst.keV2v(self.keV)**2)
         Vg_G = Fhkl/(self.crys.volume*np.pi)*self.pre*self.eps
+        Vg_G = Fhkl
         px,py,e0x = ut.project_beams(K=self.K,qxyz=self.get_G(),e0=[1,0,0],v=1)
         self.e0x = e0x
         self.df_G['px'] = px
         self.df_G['py'] = py
         self.df_G['Vg'] = Vg_G
         self.df_G['Vga'] = abs(Vg_G)
         self.df_G['Swl'] = bloch_util.logM(self.df_G['Sw'])
@@ -384,19 +502,24 @@
     def _get_central_beam(self):
         return self.get_beam(refl=[str((0,0,0))],index=True)[0]
 
     def _set_intensities(self):
         """get beam intensities at thickness"""
         id0 = self._get_central_beam()
         gammaj,CjG = self.gammaj,self.CjG
-        S = CjG.dot(np.diag(np.exp(1J*gammaj*self.thick))).dot(self.invCjG)
+        if self.dyngo:
+            S = CjG.dot(np.diag(np.exp(1J*gammaj*self.thick*self.k0/self.Knorm))).dot(self.invCjG)
+        else:
+            S = CjG.dot(np.diag(np.exp(1J*gammaj*self.thick))).dot(self.invCjG)
         # S = S[:,id0]
         S = S[id0,:]
         self.df_G['S'] = S
         self.df_G['I'] = np.abs(S)**2
+        if self.dyngo:
+            self.df_G['I']*=self.scale**2
 
     def _set_I(self,iZ=-1):
         idx=self.get_beam(refl=self.df_G.index)
         self.thick=self.z[iZ]
         self.df_G.I=self.Iz[idx,iZ]
 
     def _set_kinematic(self):
@@ -657,15 +780,15 @@
         if isinstance(iZs,int):iZs=slice(0,None,iZs)
         # iB = self.get_Istrong(out=1)[0]#;print(iB,self.Iz[    iB,iZs],)
         # iB = np.argsort(np.sum(self.Iz,axis=1))[-2]
         z      = self.z.copy()[       iZs]
         Iz_dyn = self.Iz.copy()[    :,iZs]#/self.Iz[    iB,iZs]
         Iz_kin = self.Iz_kin.copy()[:,iZs]#/self.Iz_kin[iB,iZs]#;print(Iz_dyn[Iz_dyn>1e-3])
         nzs = z.size
-        print(Iz_kin.shape,Iz_dyn.shape)
+        # print(Iz_kin.shape,Iz_dyn.shape)
         cs = dsp.getCs(cmap,nzs) #; print(len(cs),Iz_dyn.shape,Iz_kin.shape)
         # scat=tuple( [[I_kin,I_dyn,cs[i]] for i,(I_dyn,I_kin) in enumerate(zip(self.Iz[:,::iZ],self.Iz_kin[:,::iZ]))])
         plts=[[np.log10(I_kin),np.log10(I_dyn),[cs[i],'o'],'$z=%d\AA$' %z] for i,(z,I_dyn,I_kin) in enumerate(zip(z,Iz_dyn.T,Iz_kin.T))]
         # plts+=[ [[0,1],[0,1],[(0.5,)*3,'--'],''] ]
         return dsp.stddisp(plts,labs=['$I_{kin}$','$I_{dyn}$'],sargs={'alpha':0.5},**kwargs)
 
     def show_Fhkl(self,s=None,opts='m',h3D=0,**kwargs):
@@ -703,110 +826,195 @@
     def save(self,file=None,v=1):
         """save this object"""
         file = self._get_pkl(file)
         with open(file,'wb') as out :
             pickle5.dump(self, out, pickle5.HIGHEST_PROTOCOL)
         if v:print(colors.green+"object saved\n"+colors.yellow+file+colors.black)
 
-    def convert2tiff(self,tiff_file:str=None,
-        Imax:int=3e4,
-        Nmax:int=512,aperpixel:Optional[float]=None,
-        fbroad=None,
-        gs3:float=0.1,
-        nX:int=1,
-        rmax:int=0,
-        thick:float=None,
-        iz:int=None,
-        rot:int=0,
-        show:bool=False,
-        tif_writer_args:dict={},
-        **kwargs,
-    ):
-        """Write intensities to a tiff file
+    def _make_img(self,
+            exp:str=None,
+            pred:bool=False,
+            Imax:int=1,
+            Nmax:int=512,
+            rot:int=0,
+            aperpixel:Optional[float]=None,
+            fbroad=None,
+            gs3:float=0.1,
+            nX:int=1,
+            rmax:int=0,
+            thick:float=None,
+            iz:int=None,
+        ):
+        '''Make image
 
         Parameters
         -----------
-        tiff_file
-            name of the file (default name if not provided)
+        exp
+            path to dials or Dials (overrides Nmax,aperpixel)
         Imax
             max value for the intensities
         Nmax
             image resolution in pixel
         aperpixel
             reciprocal size for each pixel (aperture per pixel)
+        rot
+            in plane rotation of the image
+        pred
+            True to use dials predict (ignores rot)
         fbroad
             broadening function f(r2) (default np.exp(-r2/(gs3/3)**2))
         gs3
             Gaussian broadening factor for each reflections
         nX
-            width factor of the Gaussian window
+            width factor of the Gaussian window (in pixels)
         rmax
             radius for the noise to be added
         show
             Show produced image
         kwargs
             args to be passed to the tiff viewer
-
-
-        .. note ::
-            The reciprocal space resolution is aperpixel*Nmax. As a result some of teh
-            high resolution reflections might not appear if aperpixel or Nmax are too small.
-            If aperpixel is not specified, it is automatically so it contains the image
-            will contain all reflections.
-        """
-        Nmax=Nmax//2
+        '''
         thick = self.thick
         if thick:self.set_thickness(thick)
-        px,py,I = self.df_G[['px','py','I']].values.T
-        if rot:
-            ct,st = np.cos(np.deg2rad(rot)),np.sin(np.deg2rad(rot))
-            px,py = ct*px-st*py,st*px+ct*py
+        #dials info
+        if isinstance(exp,str):exp = pt.Dials(exp)
+        if exp:
+            aperpixel=exp.aper
+            Nmax=exp.nxy
+            if not Imax>0 or Imax==1 :
+                Imax=exp.Imax*5000
+                print(colors.red+'setting Imax to %.1E '% Imax+colors.black)
+
+        hkl = self.df_G.index
+        pred = pred and exp
+        if pred :
+            hkl = [h for h in hkl if h in exp.df_pred.index]
+            hkl_lost = np.setdiff1d(self.df_G.index,hkl)
+            if any(hkl_lost):
+                print(colors.red+"warning : reflections ignored "+colors.black)
+                print(self.df_G.loc[hkl_lost].sort_values('I')['I'][-10:])
+            pxy = exp.df_pred.loc[hkl,['px','py']]
 
+        # get intensity
+        px,py,I = self.df_G.loc[hkl,['px','py','I']].values.T
+        Nmax=Nmax//2
         if isinstance(iz,int):
-            idb=self.get_beam(refl=self.df_G.index)
+            idb=self.get_beam(refl=hkl)
             I = self.Iz[idb,iz]
             thick = self.z[iz]
+
+        # pixel locations
         if not aperpixel:
             aperpixel = 1.1*max(px.max(),py.max())/Nmax
-            print('aperpixel set to %.1E A^-1' %aperpixel)
+            print('aperpixel set to %.1E A^-1 ' %(aperpixel))
         dqx,dqy = [aperpixel]*2
+        if pred:
+            i,j = np.array(pxy[['px','py']].values,dtype=int).T
+        else:
+            if rot:
+                ct,st = np.cos(np.deg2rad(rot)),np.sin(np.deg2rad(rot))
+                px,py = ct*px-st*py,st*px+ct*py
+            i,j = np.array([np.round(px/dqx),np.round(py/dqy)],dtype=int)+Nmax
 
 
-        #convert to pixel locations
+        #### kernel (converted to pixel locations)
         if not fbroad:
             fbroad=lambda r2:np.exp(-r2/(gs3/3)**2)
             nx,ny = np.array(np.floor(gs3/np.array([dqx,dqy])),dtype=int)
         else:
             nx,ny=nX,nX
         ix,iy = np.meshgrid(range(-nx,nx+1),range(-ny,ny+1))
         x,y = ix*dqx,iy*dqy
-        i,j = np.array([np.round(px/dqx),np.round(py/dqy)],dtype=int)+Nmax
-
-        #### Gaussian broadening
+        ## Gaussian broadening
         r2 = (x**2+y**2)
-        Pb = fbroad(r2)
-        # dsp.stddisp(im=[x,y,Pb],pOpt='im')
+        Pb = fbroad(r2)#;dsp.stddisp(im=[x,y,Pb],pOpt='im')
         im0 = np.zeros((2*Nmax,)*2)
         for i0,j0,I0 in zip(i,j,I):
             i0x,j0y = i0+ix,j0+iy
             idx     = (i0x>=0) & (j0y>=0)  & (i0x<2*Nmax) & (j0y<2*Nmax)
             i0x,j0y = i0+ix[idx],j0+iy[idx]
             im0[i0x,j0y] += Pb[idx]/Pb[idx].sum()*I0
             # im0[i0,j0]=I0
+
+        #### noise
         if rmax:
             h,k = np.meshgrid(range(-Nmax,Nmax),range(-Nmax,Nmax))
             r = np.sqrt(h**2+k**2);r[r==0]=1
             im0 += rmax*np.random.rand(*im0.shape)#/(rmax*r)
 
+        return im0*Imax
+
+    def convert2img(self,filename,template=None,**kwargs):
+        im0 = self._make_img(**kwargs)#Nmax,fbroad,gs3,nX,rmax,thick,iz,rot)
+        # print(im0.mean())
+        fmt = template.split('.')[-1]
+        if not filename:
+            filename = os.path.join(self.figpath,self.name+'_%dA.%s' %(self.thick,fmt))
+        if template:
+            out = check_output("cp %s %s" %(template,filename),shell=True).decode()
+            if out:print(out)
+        bloch_util.imwrite(filename,im0)
+
+
+
+    def convert2tiff(self,tiff_file:str=None,
+        Imax:int=3e4,
+        Nmax:int=512,aperpixel:Optional[float]=None,
+        fbroad=None,
+        gs3:float=0.1,
+        nX:int=1,
+        rmax:int=0,
+        thick:float=None,
+        iz:int=None,
+        rot:int=0,
+        show:bool=False,
+        tif_writer_args:dict={},
+        **kwargs,
+    ):
+        """Write intensities to a tiff file
+
+        Parameters
+        -----------
+        tiff_file
+            name of the file (default name if not provided)
+        thick
+            Thickness of the simu
+        Imax
+            max value for the intensities
+        Nmax
+            image resolution in pixel
+        aperpixel
+            reciprocal size for each pixel (aperture per pixel)
+        fbroad
+            broadening function f(r2) (default np.exp(-r2/(gs3/3)**2))
+        gs3
+            Gaussian broadening factor for each reflections
+        nX
+            width factor of the Gaussian window
+        rmax
+            radius for the noise to be added
+        show
+            Show produced image
+        kwargs
+            args to be passed to the tiff viewer
+
+
+        .. note ::
+            The reciprocal space resolution is aperpixel*Nmax. As a result some of teh
+            high resolution reflections might not appear if aperpixel or Nmax are too small.
+            If aperpixel is not specified, it is automatically so it contains the image
+            will contain all reflections.
+        """
+        im0 = _make_img(Nmax,fbroad,gs3,nX,rmax,thick,iz,rot)
 
         if not tiff_file:
             tiff_file = os.path.join(self.path,self.name+'_%dA' %thick+'.tiff')
         I = np.array(im0*Imax,dtype='uint16')
 
-        ix,iy = np.meshgrid(range(2*Nmax),range(2*Nmax))
+        # ix,iy = np.meshgrid(range(2*Nmax),range(2*Nmax))
         # dsp.stddisp(im=[ix,iy,I],plots=[j,i,'bo'],xylims=[0,512,0,512],
         #     cmap='gray',caxis=[0,10],imOpt='tX',pargs={'fillstyle':'none'})
 
         tifffile.imwrite(tiff_file,I.T,**tif_writer_args)
         print(colors.yellow+tiff_file+colors.green+' saved'+colors.black)
         if show:
             # v=viewers.Base_Viewer(self.path,frame=1,thick=self.thick,**kwargs)
```

### Comparing `ccp4ED-1.0.9/blochwave/bloch_pp.py` & `ccp4ED-1.1.0/blochwave/bloch_pp.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """Bloch contiuous rotation experiment"""
 import importlib as imp
-import os,numpy as np
-from subprocess import Popen
+import os,glob,numpy as np
+from subprocess import Popen,check_output
 from typing import TYPE_CHECKING, Dict, Iterable, Optional, Sequence, Union
 from utils import displayStandards as dsp#;imp.reload(dsp)
 from utils import glob_colors as colors#;imp.reload(dsp)
 from EDutils import display as EDdisp #;imp.reload(EDdisp)
 from EDutils import rotate_exp        ;imp.reload(rotate_exp)
 from EDutils import utilities as ut   #;imp.reload(ut)
 from EDutils import viewers as vw     #;imp.reload(vw)
 from . import bloch                   ;imp.reload(bloch)
+from . import util as bu              ;imp.reload(bu)
+
+
 
 class Bloch_cont(rotate_exp.Rocking):
     def __init__(self,**kwargs):
         """ Bloch continous rocking curve
 
         Parameters
         ----------
@@ -27,48 +30,124 @@
             Popen('mkdir %s' %self.figpath,shell=True)
         self.save()
 
     def set_beams_vs_thickness(self,thicks,v=1):
         self.do('_set_beams_vs_thickness',thicks=thicks,v=v)
         self.z = self.load(0).z
 
-    def convert2tiff(self,n=0,nmax=0,**kwargs):
-        '''Convert to tiff
+    def sum_images(self,n,fmt='',figpath=None,frames=()):
+        ''' Sums images found in figpath by chuncks of n images
+        and puts them into directory "figpath/sum"
+
+        Parameters
+        ----------
+        n
+            number of images to sum (each side of the central image will be n/2 images)
+        figpath
+            Where the images are located
+        frames
+            The range of frames consider in (f_init,f_end)
+        '''
+        #handle output style
+        if not fmt:fmt = glob.glob(os.path.join(figpath,'*'))[0].split('.')[-1]
+        sum_path=os.path.join(figpath,'sum')
+        pad_n = int(np.ceil(np.log10(np.ceil(self.df.shape[0]/n))))
+        if not os.path.exists(sum_path):
+            Popen('mkdir %s' %sum_path,shell=True)
+
+        # handles min and max frames
+        nmax = self.df.shape[0]
+        n_max = int(np.ceil(nmax/n))
+        if not len(frames)==2:frames=(0,n_max+1)
+        n_init,n_end = frames
+        n_init,n_end=max(0,n_init),min(n_end,n_max)
+        n2 = n//2 #int(np.ceil(n/2))
+
+        ## check images exists
+        nbounds=lambda n0:max(0,min(nmax-1,n0))
+        ni,nf = nbounds(n*n_init-n2),nbounds(n*n_end+n2+1)
+        filenames = np.array([figpath+'/%s.%s' %(self.load(i).name,fmt)
+            for i in [ni,nf]])
+        miss = [not os.path.exists(f) for f in filenames]
+        if any(miss):
+            print(colors.red+'Missing images : \n'+colors.black)
+            print('\n'.join(filenames[miss]))
+            return
+        #get the size of the images
+        nxy = bu.imread(filenames[0]).shape
+        for i in np.arange(n_init,n_end+1):
+            im = np.zeros(nxy)
+            subframes = np.arange(max(0,i*n-n2),min(nmax,i*n+n2+1))
+            print(colors.red,i,subframes,colors.black)
+            for j in subframes:
+                b = self.load(j)
+                img_file=os.path.join(figpath,'%s.%s' %(b.name,fmt))
+                im+=bu.imread(img_file)/n
+            frame_str = str(i).zfill(pad_n)
+            new_file = os.path.join(sum_path,'%s.%s' %(frame_str,fmt))
+            out = check_output("cp %s %s" %(filenames[0],new_file),shell=True).decode()
+            if out:print(out)
+            bu.imwrite(new_file,im.T)#np.fliplr(np.flipud(im)))
+            # print(colors.yellow+new_file+colors.green+' saved'+colors.black)
+
+    def make_img(self,template=None,figpath=None,fmt='',frames=None,**kwargs):
+        if not figpath:figpath=self.figpath
+        nmax=self.df.shape[0]
+        if template and not fmt:fmt=template.split('.')[-1]
+        if type(frames)==type(None):frames=np.arange(nmax)
+        if not os.path.exists(figpath):
+            out=check_output('mkdir -p %s' %figpath,shell=True).decode()
+            if out:print(out)
+        for i in frames:
+            b0 = self.load(i)
+            filename=figpath+'/%s.%s' %(b0.name,fmt)
+            b0.convert2img(filename,template,**kwargs)
+
+
+    def convert2tiff(self,figpath=None,n=0,nmax=0,**kwargs):
+        ''' Generate tiff files
         Parameters
         ------------
-            n : sum n images at a time
-            nmax: max image to consider
+            figpath
+                final name will be figpath+'/%s.tiff' %b.name
+            kwargs
+                passed to Bloch.convert2tiff
+            n
+                if n> 1 sum n images at a time
+            nmax
+                number of frames to consider
         '''
         import tifffile
-        b0=self.load(0)
-        tiff_file=self.figpath+'/%s.tiff' %b0.name
-        im=tifffile.imread(tiff_file)
+        if not figpath:figpath=self.figpath
         if not nmax:nmax=self.df.shape[0]
         if n>1:
-            sum_path=os.path.join(self.figpath,'sum')
+            b0=self.load(0)
+            tiff_file=figpath+'/%s.tiff' %b0.name
+            im=tifffile.imread(tiff_file)
+            sum_path=os.path.join(figpath,'sum')
             # self.sum_path=sum_path
             pad_n = int(np.ceil(np.log10(np.ceil(self.df.shape[0]/n))))
             if not os.path.exists(sum_path):
-                Popen('mkdir %s' %self.sum_path,shell=True)
+                Popen('mkdir %s' %sum_path,shell=True)
 
             for i in range(0,nmax,n):
                 im = np.zeros(im.shape)
                 new_tiff_file = os.path.join(sum_path,'%s.tiff' %(str(i//n).zfill(pad_n)))
                 # for j in range(n):
                 for j in range(max(0,i+n-5),min(nmax-1,i+n+5)):
                     b = self.load(j)
-                    tiff_file=self.figpath+'/%s.tiff' %b.name
+                    tiff_file=figpath+'/%s.tiff' %b.name
                     im+=tifffile.imread(tiff_file)/n
                 tifffile.imwrite(new_tiff_file,im)
                 print(colors.yellow+new_tiff_file+colors.green+' saved'+colors.black)
 
         else:
             for i in range(nmax):
                 b = self.load(i)
-                b.convert2tiff(tiff_file=self.figpath+'/%s.tiff' %b.name,**kwargs)
+                b.convert2tiff(tiff_file=figpath+'/%s.tiff' %b.name,**kwargs)
                 b.save()
 
     def convert2png(self,cutoff=20,n=None,**kwargs):
         import tifffile
         for i in range(self.df[:n].shape[0]):
             b = self.load(i)
             tiff_file=self.figpath+'/%s.tiff' %b.name
```

### Comparing `ccp4ED-1.0.9/blochwave/util.py` & `ccp4ED-1.1.0/blochwave/util.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,57 @@
 import numpy as np
+import mrcfile,tifffile
 from utils import glob_colors as colors
 import os,glob,pickle5
 
+def mrc2tiff(mrc_file,outpath):
+    tiff_file = os.path.basename(mrc_file).replace('.mrc','.tiff')
+    im = imread(mrc_file).copy()
+    im -= im.min()
+    im*=50/im.mean()
+    # im*=1e4/im.max()
+    # im = np.array(im,dtype=np.uint16)
+    imwrite(os.path.join(outpath,tiff_file),im)
+
+#### writer
+def mrc_writer(filename,im0):
+    mrc = mrcfile.open(filename,'r+')
+    mrc.set_data(np.array(im0,dtype=type(mrc.data[0,0])))
+    mrc.flush()
+    mrc.close()
+
+def tiff_writer(tiff_file,im):
+    tifffile.imwrite(tiff_file,im)
+img_writers = {
+    'mrc' : mrc_writer,
+    'tiff': tiff_writer,
+}
+def imwrite(filename,im):
+    fmt=filename.split('.')[-1]
+    img_writers[fmt](filename,im)
+    print(colors.yellow+filename+colors.green+' saved'+colors.black)
+
+
+#### reader
+def tiff_reader(tiff_file)  :
+    with open(tiff_file,'rb') as f:
+        I =tifffile.imread(f)
+    return I
+def mrc_reader(mrc_file):
+    with mrcfile.open(mrc_file) as mrc:
+        return mrc.data
+img_readers = {
+    'mrc' : mrc_reader,
+    'tiff': tiff_reader,
+}
+fmts = list(img_readers.keys())#['mrc','tiff']
+def imread(filename):
+    fmt=filename.split('.')[-1]
+    return img_readers[fmt](filename)
+
 
 def strong_beams(dfG,
         tol:float=1e-2,n:int=10,
         opt:str='F'):
     """keep the n strongest beams, i.e. those with intensity I>tol not including central beam
 
     Parameters
@@ -41,15 +87,15 @@
     for h,hkl in zip(dfM.index,dfM[['h','k','l']].values):
         if not str(tuple(-hkl)) in refl:
             refl.append(h)
     print('removing Friedel pairs')
     dfM=dfM.loc[refl]
     return dfM
 
-def get_inp(npx,nbeams,u,keV,thicks):
+def get_inp(npx,nbeams,u,keV,thicks,out=None):
     inp = """# Input file for Felix version :
 # ------------------------------------
 
 # ------------------------------------
 
 # control flags
 IWriteFLAG                = 0
@@ -106,21 +152,33 @@
 INoofUgs                 = 40
 IAtomicSites             = (1,2)
 IPrint                   = 0
 RSimplexLengthScale      = 20.0
 RExitCriteria            = 0.00001
     """
 
-    return inp
+    if out:
+        with open(out,'w') as f:f.write(inp)
+    else:
+        return inp
 
-def load_bloch(path='',tag='',file='',v=1):
-    """load a saved Bloch object
-    filename : pickle file (.pkl)  """
-    files = [f for f in glob.glob(os.path.join(path,'*.pkl')) if tag in f]
-    if tag:
+def load_bloch(path='',tag=None,file='',v=1):
+    """load a saved Bloch object from
+    path : path to simulation folder
+    tag : identifier for a bloch simu in case there are several possibilities
+        OR
+    filename : directly provide the pickle file (.pkl)
+    """
+    # first tr toget a simu from the tag
+    files = [f for f in glob.glob(os.path.join(path,'*.pkl'))]
+    if not isinstance(tag,type(None)):
+        if isinstance(tag,int):
+            file = files[tag]
+        else:
+            files = [f for f in glob.glob(os.path.join(path,'*.pkl')) if tag in f]
         if len(files)==1:
             file = files[0]
     if file:
         with open(file,'rb') as f : obj = pickle5.load(f)
         if v:print(colors.green+'loaded:' +colors.yellow+file+colors.black);
         return obj
     else:
```

### Comparing `ccp4ED-1.0.9/ccp4ED.egg-info/PKG-INFO` & `ccp4ED-1.1.0/ccp4ED.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccp4ED
-Version: 1.0.9
+Version: 1.1.0
 Summary: Electron diffraction utilities
 Home-page: https://pypi.org/project/ccp4ED
 Author: Tarik Ronan Drevon
 Author-email: tarik.drevon@stfc.ac.uk
 License: UNKNOWN
 Project-URL: Documentation, https://debloch.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/ccp4/electron-diffraction
```

### Comparing `ccp4ED-1.0.9/ccp4ED.egg-info/SOURCES.txt` & `ccp4ED-1.1.0/ccp4ED.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -2,22 +2,27 @@
 README.md
 changelog.md
 install.sh
 pydocmd.yml
 setup.py
 EDutils/__init__.py
 EDutils/convert_pets.sh
+EDutils/dials_utils.py
 EDutils/display.py
+EDutils/dyn_utils.py
+EDutils/felix.py
 EDutils/gui.py
 EDutils/gui_config.py
+EDutils/import_ED.py
 EDutils/pets.py
 EDutils/pets_ref.sh
 EDutils/rotate_exp.py
 EDutils/utilities.py
 EDutils/viewers.py
+EDutils/xds.py
 EDutils/data/viewer_df.pkl
 EDutils/data/viewer_dict.pkl
 EDutils/sandbox/convert.py
 EDutils/sandbox/test.py
 blochwave/__init__.py
 blochwave/bloch.py
 blochwave/bloch_pp.py
```

### Comparing `ccp4ED-1.0.9/docs/Makefile` & `ccp4ED-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/docs/source/_static/click.wav` & `ccp4ED-1.1.0/docs/source/_static/click.wav`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/docs/source/_static/command.png` & `ccp4ED-1.1.0/docs/source/_static/command.png`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/docs/source/_static/custom.css` & `ccp4ED-1.1.0/docs/source/_static/custom.css`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/docs/source/_static/favicon.ico` & `ccp4ED-1.1.0/docs/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/docs/source/_static/favicon.png` & `ccp4ED-1.1.0/docs/source/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/docs/source/_static/favicon.svg` & `ccp4ED-1.1.0/docs/source/_static/favicon.svg`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/docs/source/_static/pull-requests.png` & `ccp4ED-1.1.0/docs/source/_static/pull-requests.png`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/docs/source/_static/responsiveSvg.js` & `ccp4ED-1.1.0/docs/source/_static/responsiveSvg.js`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/docs/source/_static/select_transifex_repo.png` & `ccp4ED-1.1.0/docs/source/_static/select_transifex_repo.png`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/docs/source/_static/transifex_explanation.png` & `ccp4ED-1.1.0/docs/source/_static/transifex_explanation.png`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/docs/source/_templates/autosummary/class.rst` & `ccp4ED-1.1.0/docs/source/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/docs/source/_templates/autosummary/module.rst` & `ccp4ED-1.1.0/docs/source/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/docs/source/conf.py` & `ccp4ED-1.1.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/docs/source/examples/MX_t.png` & `ccp4ED-1.1.0/docs/source/examples/MX_t.png`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/docs/source/examples/blochwave.rst` & `ccp4ED-1.1.0/docs/source/examples/blochwave.rst`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/install.sh` & `ccp4ED-1.1.0/install.sh`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/ED_base.py` & `ccp4ED-1.1.0/multislice/ED_base.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/config.py` & `ccp4ED-1.1.0/multislice/config.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/convert_pets.sh` & `ccp4ED-1.1.0/multislice/convert_pets.sh`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/data/splines.npy` & `ccp4ED-1.1.0/multislice/data/splines.npy`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/examples/Carbone_SC.py` & `ccp4ED-1.1.0/multislice/examples/Carbone_SC.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/examples/Li.py` & `ccp4ED-1.1.0/multislice/examples/Li.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/examples/biotin_figs.py` & `ccp4ED-1.1.0/multislice/examples/biotin_figs.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/examples/biotin_run.py` & `ccp4ED-1.1.0/multislice/examples/biotin_run.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/examples/dat/C.txt` & `ccp4ED-1.1.0/multislice/examples/dat/C.txt`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/examples/dat/H.txt` & `ccp4ED-1.1.0/multislice/examples/dat/H.txt`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/examples/dat/O.txt` & `ccp4ED-1.1.0/multislice/examples/dat/O.txt`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/examples/dat/P.txt` & `ccp4ED-1.1.0/multislice/examples/dat/P.txt`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/examples/dat/S.txt` & `ccp4ED-1.1.0/multislice/examples/dat/S.txt`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/examples/dat/biotin_m1.npy` & `ccp4ED-1.1.0/multislice/examples/dat/biotin_m1.npy`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/examples/dat/biotin_m1.smv` & `ccp4ED-1.1.0/multislice/examples/dat/biotin_m1.smv`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/examples/dat/biotin_m1.smv.npy` & `ccp4ED-1.1.0/multislice/examples/dat/biotin_m1.smv.npy`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/examples/dat/test.mp4` & `ccp4ED-1.1.0/multislice/examples/dat/test.mp4`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/examples/dat/test.smv` & `ccp4ED-1.1.0/multislice/examples/dat/test.smv`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/examples/epicza.py` & `ccp4ED-1.1.0/multislice/examples/epicza.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/examples/ireloh.py` & `ccp4ED-1.1.0/multislice/examples/ireloh.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/examples/make_crystal.py` & `ccp4ED-1.1.0/multislice/examples/make_crystal.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/examples/npy2smv` & `ccp4ED-1.1.0/multislice/examples/npy2smv`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/examples/npy2smv.cpp` & `ccp4ED-1.1.0/multislice/examples/npy2smv.cpp`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/examples/paracetamol_run.py` & `ccp4ED-1.1.0/multislice/examples/paracetamol_run.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/examples/silicon_run.py` & `ccp4ED-1.1.0/multislice/examples/silicon_run.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/examples/test_base.py` & `ccp4ED-1.1.0/multislice/examples/test_base.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/examples/walltimes.py` & `ccp4ED-1.1.0/multislice/examples/walltimes.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/import.py` & `ccp4ED-1.1.0/multislice/import.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/interaction_parameter.py` & `ccp4ED-1.1.0/multislice/interaction_parameter.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/multi_2D.py` & `ccp4ED-1.1.0/multislice/multi_2D.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/multi_3D.py` & `ccp4ED-1.1.0/multislice/multi_3D.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/multislice.py` & `ccp4ED-1.1.0/multislice/multislice.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/mupy_utils.py` & `ccp4ED-1.1.0/multislice/mupy_utils.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/pets.py` & `ccp4ED-1.1.0/multislice/pets.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/postprocess.py` & `ccp4ED-1.1.0/multislice/postprocess.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/pymultislice.py` & `ccp4ED-1.1.0/multislice/pymultislice.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/rotating_crystal.py` & `ccp4ED-1.1.0/multislice/rotating_crystal.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/temsim/atompot.cpp` & `ccp4ED-1.1.0/multislice/temsim/atompot.cpp`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/temsim/autoslic.cpp` & `ccp4ED-1.1.0/multislice/temsim/autoslic.cpp`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/temsim/autoslic.hpp` & `ccp4ED-1.1.0/multislice/temsim/autoslic.hpp`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/temsim/autosliccmd.cpp` & `ccp4ED-1.1.0/multislice/temsim/autosliccmd.cpp`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/temsim/autostem.cpp` & `ccp4ED-1.1.0/multislice/temsim/autostem.cpp`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/temsim/autostem.hpp` & `ccp4ED-1.1.0/multislice/temsim/autostem.hpp`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/temsim/autostemcmd.cpp` & `ccp4ED-1.1.0/multislice/temsim/autostemcmd.cpp`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/temsim/cfpix.cpp` & `ccp4ED-1.1.0/multislice/temsim/cfpix.cpp`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/temsim/cfpix.hpp` & `ccp4ED-1.1.0/multislice/temsim/cfpix.hpp`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/temsim/floatTIFF.cpp` & `ccp4ED-1.1.0/multislice/temsim/floatTIFF.cpp`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/temsim/floatTIFF.hpp` & `ccp4ED-1.1.0/multislice/temsim/floatTIFF.hpp`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/temsim/image.cpp` & `ccp4ED-1.1.0/multislice/temsim/image.cpp`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/temsim/incostem.cpp` & `ccp4ED-1.1.0/multislice/temsim/incostem.cpp`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/temsim/incostem.hpp` & `ccp4ED-1.1.0/multislice/temsim/incostem.hpp`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/temsim/incostemcmd.cpp` & `ccp4ED-1.1.0/multislice/temsim/incostemcmd.cpp`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/temsim/makefile` & `ccp4ED-1.1.0/multislice/temsim/makefile`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/temsim/mulslice.cpp` & `ccp4ED-1.1.0/multislice/temsim/mulslice.cpp`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/temsim/probe.cpp` & `ccp4ED-1.1.0/multislice/temsim/probe.cpp`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/temsim/probe.hpp` & `ccp4ED-1.1.0/multislice/temsim/probe.hpp`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/temsim/probecmd.cpp` & `ccp4ED-1.1.0/multislice/temsim/probecmd.cpp`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/temsim/run_temsim.sh` & `ccp4ED-1.1.0/multislice/temsim/run_temsim.sh`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/temsim/slicelib.cpp` & `ccp4ED-1.1.0/multislice/temsim/slicelib.cpp`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/temsim/slicelib.hpp` & `ccp4ED-1.1.0/multislice/temsim/slicelib.hpp`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/temsim/slicelib_main.cpp` & `ccp4ED-1.1.0/multislice/temsim/slicelib_main.cpp`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/temsim/stemslic.cpp` & `ccp4ED-1.1.0/multislice/temsim/stemslic.cpp`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/multislice/temsim/sumpix.cpp` & `ccp4ED-1.1.0/multislice/temsim/sumpix.cpp`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/nearBragg/nanobragg.c` & `ccp4ED-1.1.0/nearBragg/nanobragg.c`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/nearBragg/nearBragg.c` & `ccp4ED-1.1.0/nearBragg/nearBragg.c`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/nearBragg/nearBragg.py` & `ccp4ED-1.1.0/nearBragg/nearBragg.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/nearBragg/nearBragg_doc.py` & `ccp4ED-1.1.0/nearBragg/nearBragg_doc.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/nearBragg/proba.py` & `ccp4ED-1.1.0/nearBragg/proba.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/notebooks/glycine.ipynb` & `ccp4ED-1.1.0/notebooks/glycine.ipynb`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/notebooks/multislice/Silicon.ipynb` & `ccp4ED-1.1.0/notebooks/multislice/Silicon.ipynb`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/notebooks/multislice/example_0.ipynb` & `ccp4ED-1.1.0/notebooks/multislice/example_0.ipynb`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/notebooks/multislice/glycine.ipynb` & `ccp4ED-1.1.0/notebooks/multislice/glycine.ipynb`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/notebooks/multislice/pets.ipynb` & `ccp4ED-1.1.0/notebooks/multislice/pets.ipynb`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/pydocmd.yml` & `ccp4ED-1.1.0/pydocmd.yml`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/results/diamond/continuous.py` & `ccp4ED-1.1.0/results/diamond/continuous.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/results/diamond/diamond.py` & `ccp4ED-1.1.0/results/diamond/diamond.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/results/glycine/dat/alpha_glycine.cif` & `ccp4ED-1.1.0/results/glycine/dat/alpha_glycine.cif`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/results/glycine/dat/figures/glycine-103_200keV_bloch.png` & `ccp4ED-1.1.0/results/glycine/dat/figures/glycine-103_200keV_bloch.png`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/results/glycine/glycine.py` & `ccp4ED-1.1.0/results/glycine/glycine.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/results/glycine/glycine_zenodo.py` & `ccp4ED-1.1.0/results/glycine/glycine_zenodo.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/results/glycine/optimize_frame.py` & `ccp4ED-1.1.0/results/glycine/optimize_frame.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/results/glycine/pets_ref.py` & `ccp4ED-1.1.0/results/glycine/pets_ref.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/results/glycine/sweep.py` & `ccp4ED-1.1.0/results/glycine/sweep.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/results/glycine/test.tiff` & `ccp4ED-1.1.0/results/glycine/test.tiff`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/results/glycine/viewer_glycine.py` & `ccp4ED-1.1.0/results/glycine/viewer_glycine.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/scattering/cmpScattering.py` & `ccp4ED-1.1.0/scattering/cmpScattering.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/scattering/data/abcd.npy` & `ccp4ED-1.1.0/scattering/data/abcd.npy`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/scattering/data/elec.pkl` & `ccp4ED-1.1.0/scattering/data/elec.pkl`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/scattering/data/spline_1.txt` & `ccp4ED-1.1.0/scattering/data/spline_1.txt`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/scattering/data/spline_14.txt` & `ccp4ED-1.1.0/scattering/data/spline_14.txt`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/scattering/data/spline_16.txt` & `ccp4ED-1.1.0/scattering/data/spline_16.txt`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/scattering/data/spline_6.txt` & `ccp4ED-1.1.0/scattering/data/spline_6.txt`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/scattering/data/spline_7.txt` & `ccp4ED-1.1.0/scattering/data/spline_7.txt`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/scattering/data/spline_8.txt` & `ccp4ED-1.1.0/scattering/data/spline_8.txt`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/scattering/data/splines.npy` & `ccp4ED-1.1.0/scattering/data/splines.npy`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/scattering/data/xray.pkl` & `ccp4ED-1.1.0/scattering/data/xray.pkl`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/scattering/potential_misc.py` & `ccp4ED-1.1.0/scattering/potential_misc.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/scattering/scattering_factors.py` & `ccp4ED-1.1.0/scattering/scattering_factors.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     '''
     if isinstance(elts[0],str) :
         Z = pd.read_pickle(dat_path+'elec.pkl')['Z'][elts].values
     else:
         Z=elts
     if not isinstance(q,np.ndarray) : q = np.linspace(0,qmax,npts)
     #dummy case to disable form factor
-    if Z==[0]:return q,[np.ones(q.shape)]
+    # if Z==[0]:return q,[np.ones(q.shape)]
     q2,fq_e,nelts = q**2,[],len(Z)
 
     fparams = np.load(dat_path+'abcd.npy',allow_pickle=True)
     for elt in range(nelts) :
         a,b=np.reshape(fparams[Z[elt],:6],(3,2)).T
         c,d=np.reshape(fparams[Z[elt],6:],(3,2)).T; #print(a,b,c,d)
         fq = np.zeros(q.shape)
```

### Comparing `ccp4ED-1.0.9/scattering/splines.py` & `ccp4ED-1.1.0/scattering/splines.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/scattering/structure_factor.py` & `ccp4ED-1.1.0/scattering/structure_factor.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/setup.py` & `ccp4ED-1.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
    long_description = fh.read()
 
 setuptools.setup(
     name="ccp4ED",
-    version="1.0.9",
+    version="1.1.0",
     author="Tarik Ronan Drevon",
     author_email="tarik.drevon@stfc.ac.uk",
     description="Electron diffraction utilities",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://pypi.org/project/ccp4ED",
     project_urls={
@@ -24,10 +24,11 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License ",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
     install_requires=['numpy','scipy','matplotlib','colorama','pandas',
-    'cbf','crystals','TarikDrevonUtils','easygui','tifffile','pickle5','bs4',
+    'crystals','TarikDrevonUtils','easygui','tifffile','pickle5','bs4',
+    'cbf','mrcfile','gemmi',
     ],
 )
```

### Comparing `ccp4ED-1.0.9/tests/EDutils/pets/alpha_glycine.cif` & `ccp4ED-1.1.0/tests/EDutils/pets/alpha_glycine.cif`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/EDutils/pets/glycine.cenloc` & `ccp4ED-1.1.0/tests/EDutils/pets/glycine.cenloc`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/EDutils/pets/glycine.cif_pets` & `ccp4ED-1.1.0/tests/EDutils/pets/glycine.cif_pets`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/EDutils/pets/glycine.clust` & `ccp4ED-1.1.0/tests/EDutils/pets/glycine.clust`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/EDutils/pets/glycine.cml` & `ccp4ED-1.1.0/tests/EDutils/pets/glycine.cml`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/EDutils/pets/glycine.cor` & `ccp4ED-1.1.0/tests/EDutils/pets/glycine.cor`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/EDutils/pets/glycine.framestats` & `ccp4ED-1.1.0/tests/EDutils/pets/glycine.framestats`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/EDutils/pets/glycine.hkl` & `ccp4ED-1.1.0/tests/EDutils/pets/glycine.hkl`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/EDutils/pets/glycine.pts` & `ccp4ED-1.1.0/tests/EDutils/pets/glycine.pts`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/EDutils/pets/glycine.resolution` & `ccp4ED-1.1.0/tests/EDutils/pets/glycine.resolution`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/EDutils/pets/glycine.rpl` & `ccp4ED-1.1.0/tests/EDutils/pets/glycine.rpl`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/EDutils/pets/glycine.xyz` & `ccp4ED-1.1.0/tests/EDutils/pets/glycine.xyz`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/EDutils/pets/glycine_dyn.cif_pets` & `ccp4ED-1.1.0/tests/EDutils/pets/glycine_dyn.cif_pets`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/EDutils/pets/tiff/00001.tiff` & `ccp4ED-1.1.0/tests/EDutils/pets/tiff/00001.tiff`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/EDutils/test_gui.py` & `ccp4ED-1.1.0/tests/EDutils/test_gui.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/EDutils/test_pets.py` & `ccp4ED-1.1.0/tests/EDutils/test_pets.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/EDutils/test_utilities.py` & `ccp4ED-1.1.0/tests/EDutils/test_utilities.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/blochwave/GaAs_felix.cif` & `ccp4ED-1.1.0/tests/blochwave/GaAs_felix.cif`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/blochwave/Nbeams_diamond.py` & `ccp4ED-1.1.0/tests/blochwave/Nbeams_diamond.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/blochwave/bloch2D.py` & `ccp4ED-1.1.0/tests/blochwave/bloch2D.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/blochwave/bloch_vs_multi2D_2beam.py` & `ccp4ED-1.1.0/tests/blochwave/bloch_vs_multi2D_2beam.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/blochwave/bloch_vs_multi2D_zone.py` & `ccp4ED-1.1.0/tests/blochwave/bloch_vs_multi2D_zone.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/blochwave/continuous2D.py` & `ccp4ED-1.1.0/tests/blochwave/continuous2D.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/blochwave/test2beams.py` & `ccp4ED-1.1.0/tests/blochwave/test2beams.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/blochwave/test_bloch_base.py` & `ccp4ED-1.1.0/tests/blochwave/test_bloch_base.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/blochwave/test_continuous.py` & `ccp4ED-1.1.0/tests/blochwave/test_continuous.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/blochwave/test_felix.py` & `ccp4ED-1.1.0/tests/blochwave/test_felix.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/multi2D/2_beam.py` & `ccp4ED-1.1.0/tests/multi2D/2_beam.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/multi2D/2_beam_pendullosung.py` & `ccp4ED-1.1.0/tests/multi2D/2_beam_pendullosung.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/multi2D/TDS.py` & `ccp4ED-1.1.0/tests/multi2D/TDS.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/multi2D/base_test.py` & `ccp4ED-1.1.0/tests/multi2D/base_test.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/multi2D/padding.py` & `ccp4ED-1.1.0/tests/multi2D/padding.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/multi2D/pendullosung.py` & `ccp4ED-1.1.0/tests/multi2D/pendullosung.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/multi2D/single_array.py` & `ccp4ED-1.1.0/tests/multi2D/single_array.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/multislice/base_3D.py` & `ccp4ED-1.1.0/tests/multislice/base_3D.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/multislice/test_base.py` & `ccp4ED-1.1.0/tests/multislice/test_base.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/old/nearbragg/NBkinvsMS.py` & `ccp4ED-1.1.0/tests/old/nearbragg/NBkinvsMS.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/old/nearbragg/base.py` & `ccp4ED-1.1.0/tests/old/nearbragg/base.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/old/nearbragg/cmp_Holton.py` & `ccp4ED-1.1.0/tests/old/nearbragg/cmp_Holton.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/old/nearbragg/fresnel_convolution.py` & `ccp4ED-1.1.0/tests/old/nearbragg/fresnel_convolution.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/old/nearbragg/near_vs_multi.py` & `ccp4ED-1.1.0/tests/old/nearbragg/near_vs_multi.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/old/nearbragg/proba.py` & `ccp4ED-1.1.0/tests/old/nearbragg/proba.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/reporter.py` & `ccp4ED-1.1.0/tests/reporter.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/scattering_lib/structure_factor.py` & `ccp4ED-1.1.0/tests/scattering_lib/structure_factor.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/wallpp/base.py` & `ccp4ED-1.1.0/tests/wallpp/base.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/wallpp/gui.py` & `ccp4ED-1.1.0/tests/wallpp/gui.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/wallpp/space_groups.py` & `ccp4ED-1.1.0/tests/wallpp/space_groups.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/tests/wallpp/wallpps.py` & `ccp4ED-1.1.0/tests/wallpp/wallpps.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/wallpp/config.py` & `ccp4ED-1.1.0/wallpp/config.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/wallpp/docs/Wallpaper_Symmetry.html` & `ccp4ED-1.1.0/wallpp/docs/Wallpaper_Symmetry.html`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/wallpp/docs/index.md` & `ccp4ED-1.1.0/wallpp/docs/index.md`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/wallpp/docs/mdx_math.py` & `ccp4ED-1.1.0/wallpp/docs/mdx_math.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/wallpp/gui.py` & `ccp4ED-1.1.0/wallpp/gui.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/wallpp/lattice.py` & `ccp4ED-1.1.0/wallpp/lattice.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/wallpp/mkdocs.yml` & `ccp4ED-1.1.0/wallpp/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/wallpp/nodesTri.py` & `ccp4ED-1.1.0/wallpp/nodesTri.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/wallpp/plane_group.py` & `ccp4ED-1.1.0/wallpp/plane_group.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/wallpp/space_group.py` & `ccp4ED-1.1.0/wallpp/space_group.py`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/wallpp/space_groups.pkl` & `ccp4ED-1.1.0/wallpp/space_groups.pkl`

 * *Files identical despite different names*

### Comparing `ccp4ED-1.0.9/wallpp/wallpaper.py` & `ccp4ED-1.1.0/wallpp/wallpaper.py`

 * *Files identical despite different names*

