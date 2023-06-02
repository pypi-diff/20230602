# Comparing `tmp/not1mm-23.5.9.2.tar.gz` & `tmp/not1mm-23.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "not1mm-23.5.9.2.tar", last modified: Wed May 10 04:06:27 2023, max compression
+gzip compressed data, was "not1mm-23.6.2.tar", last modified: Fri Jun  2 14:44:35 2023, max compression
```

## Comparing `not1mm-23.5.9.2.tar` & `not1mm-23.6.2.tar`

### file list

```diff
@@ -1,137 +1,142 @@
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-10 04:06:27.239200 not1mm-23.5.9.2/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-05-05 15:15:13.000000 not1mm-23.5.9.2/LICENSE
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    25132 2023-05-10 04:06:27.238201 not1mm-23.5.9.2/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    24385 2023-05-10 04:05:08.000000 not1mm-23.5.9.2/README.md
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-10 04:06:26.977197 not1mm-23.5.9.2/not1mm/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.5.9.2/not1mm/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    80096 2023-05-10 03:49:09.000000 not1mm-23.5.9.2/not1mm/__main__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    23860 2023-05-09 20:08:28.000000 not1mm-23.5.9.2/not1mm/bandmap.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-10 04:06:27.032198 not1mm-23.5.9.2/not1mm/data/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    16590 2023-02-15 20:52:35.000000 not1mm-23.5.9.2/not1mm/data/Combinear.qss
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-01-27 16:44:51.000000 not1mm-23.5.9.2/not1mm/data/JetBrainsMono-Regular.ttf
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   542666 2023-02-14 19:22:02.000000 not1mm-23.5.9.2/not1mm/data/MASTER.SCP
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2352 2023-04-10 21:02:17.000000 not1mm-23.5.9.2/not1mm/data/about.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      224 2023-04-18 03:49:58.000000 not1mm-23.5.9.2/not1mm/data/alpha bravo charlie delta.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5246 2023-05-01 15:41:16.000000 not1mm-23.5.9.2/not1mm/data/bandmap.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      387 2023-03-15 16:56:38.000000 not1mm-23.5.9.2/not1mm/data/check.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40156 2023-05-06 20:10:52.000000 not1mm-23.5.9.2/not1mm/data/configuration.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    89307 2023-03-07 17:30:38.000000 not1mm-23.5.9.2/not1mm/data/contests.sql
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)  4534539 2023-02-21 19:49:24.000000 not1mm-23.5.9.2/not1mm/data/cty.json
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      451 2023-04-11 19:54:10.000000 not1mm-23.5.9.2/not1mm/data/cwmacros.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    19280 2023-03-20 20:22:09.000000 not1mm-23.5.9.2/not1mm/data/editcontact.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2273 2023-02-21 14:39:24.000000 not1mm-23.5.9.2/not1mm/data/editmacro.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      474 2023-02-10 02:42:18.000000 not1mm-23.5.9.2/not1mm/data/greendot.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2023-02-09 20:47:40.000000 not1mm-23.5.9.2/not1mm/data/k6gte-not1mm.desktop
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4010 2023-02-09 20:45:38.000000 not1mm-23.5.9.2/not1mm/data/k6gte.not1mm-128.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1108 2023-02-09 20:45:03.000000 not1mm-23.5.9.2/not1mm/data/k6gte.not1mm-32.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2152 2023-02-09 20:45:22.000000 not1mm-23.5.9.2/not1mm/data/k6gte.not1mm-64.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      970 2023-03-23 20:14:51.000000 not1mm-23.5.9.2/not1mm/data/logwindow.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43909 2023-05-08 20:14:41.000000 not1mm-23.5.9.2/not1mm/data/main.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    17963 2023-05-05 12:59:56.000000 not1mm-23.5.9.2/not1mm/data/new_contest.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2018 2023-02-12 17:56:36.000000 not1mm-23.5.9.2/not1mm/data/opon.ui
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-10 04:06:27.134199 not1mm-23.5.9.2/not1mm/data/phonetics/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42590 2023-04-21 20:24:24.000000 not1mm-23.5.9.2/not1mm/data/phonetics/0.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30248 2023-04-21 20:25:33.000000 not1mm-23.5.9.2/not1mm/data/phonetics/1.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    29584 2023-04-21 20:27:16.000000 not1mm-23.5.9.2/not1mm/data/phonetics/2.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32072 2023-04-21 20:29:07.000000 not1mm-23.5.9.2/not1mm/data/phonetics/3.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43052 2023-04-21 20:29:49.000000 not1mm-23.5.9.2/not1mm/data/phonetics/4.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51976 2023-04-21 21:46:26.000000 not1mm-23.5.9.2/not1mm/data/phonetics/5.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58634 2023-04-21 21:08:45.000000 not1mm-23.5.9.2/not1mm/data/phonetics/6.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49154 2023-04-21 21:10:50.000000 not1mm-23.5.9.2/not1mm/data/phonetics/7.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32842 2023-04-21 21:13:51.000000 not1mm-23.5.9.2/not1mm/data/phonetics/73.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35636 2023-04-21 21:11:40.000000 not1mm-23.5.9.2/not1mm/data/phonetics/8.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    39592 2023-04-21 21:12:32.000000 not1mm-23.5.9.2/not1mm/data/phonetics/9.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46800 2023-04-21 21:14:36.000000 not1mm-23.5.9.2/not1mm/data/phonetics/a.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    44594 2023-04-21 21:15:20.000000 not1mm-23.5.9.2/not1mm/data/phonetics/again.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40976 2023-04-21 21:16:10.000000 not1mm-23.5.9.2/not1mm/data/phonetics/b.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46746 2023-04-21 21:17:07.000000 not1mm-23.5.9.2/not1mm/data/phonetics/c.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    62558 2023-04-21 13:38:05.000000 not1mm-23.5.9.2/not1mm/data/phonetics/contest.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    92498 2023-04-21 21:17:54.000000 not1mm-23.5.9.2/not1mm/data/phonetics/cq.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52524 2023-04-21 21:18:24.000000 not1mm-23.5.9.2/not1mm/data/phonetics/d.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    45700 2023-04-21 21:19:02.000000 not1mm-23.5.9.2/not1mm/data/phonetics/e.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    53438 2023-04-21 21:19:38.000000 not1mm-23.5.9.2/not1mm/data/phonetics/f.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42766 2023-04-21 21:20:18.000000 not1mm-23.5.9.2/not1mm/data/phonetics/g.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50040 2023-04-21 21:21:03.000000 not1mm-23.5.9.2/not1mm/data/phonetics/h.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46372 2023-04-21 21:23:33.000000 not1mm-23.5.9.2/not1mm/data/phonetics/i.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43434 2023-04-21 21:24:12.000000 not1mm-23.5.9.2/not1mm/data/phonetics/j.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49066 2023-04-21 21:24:57.000000 not1mm-23.5.9.2/not1mm/data/phonetics/k.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   185562 2023-04-21 21:25:43.000000 not1mm-23.5.9.2/not1mm/data/phonetics/k6gte.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43154 2023-04-21 21:26:21.000000 not1mm-23.5.9.2/not1mm/data/phonetics/l.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    54352 2023-04-21 21:27:07.000000 not1mm-23.5.9.2/not1mm/data/phonetics/m.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56798 2023-04-21 21:27:57.000000 not1mm-23.5.9.2/not1mm/data/phonetics/mynumber.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52204 2023-04-21 21:28:42.000000 not1mm-23.5.9.2/not1mm/data/phonetics/n.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   154544 2023-04-21 21:29:54.000000 not1mm-23.5.9.2/not1mm/data/phonetics/nil.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47440 2023-04-21 21:30:37.000000 not1mm-23.5.9.2/not1mm/data/phonetics/o.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    38300 2023-04-21 21:31:22.000000 not1mm-23.5.9.2/not1mm/data/phonetics/p.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    55288 2023-04-21 21:31:58.000000 not1mm-23.5.9.2/not1mm/data/phonetics/q.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47432 2023-04-21 21:32:39.000000 not1mm-23.5.9.2/not1mm/data/phonetics/r.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46122 2023-04-21 21:33:20.000000 not1mm-23.5.9.2/not1mm/data/phonetics/roger.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    60698 2023-04-21 21:33:59.000000 not1mm-23.5.9.2/not1mm/data/phonetics/s.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    70424 2023-04-17 20:43:04.000000 not1mm-23.5.9.2/not1mm/data/phonetics/space.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58196 2023-04-21 21:35:28.000000 not1mm-23.5.9.2/not1mm/data/phonetics/t.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56320 2023-04-21 21:36:54.000000 not1mm-23.5.9.2/not1mm/data/phonetics/thankyou.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    94980 2023-04-21 21:37:27.000000 not1mm-23.5.9.2/not1mm/data/phonetics/thankyouqrz.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    65922 2023-04-21 21:38:05.000000 not1mm-23.5.9.2/not1mm/data/phonetics/u.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50142 2023-04-21 21:38:37.000000 not1mm-23.5.9.2/not1mm/data/phonetics/v.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    37638 2023-04-21 21:39:21.000000 not1mm-23.5.9.2/not1mm/data/phonetics/w.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    61870 2023-04-21 21:40:02.000000 not1mm-23.5.9.2/not1mm/data/phonetics/x.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56524 2023-04-21 21:40:40.000000 not1mm-23.5.9.2/not1mm/data/phonetics/y.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46510 2023-04-21 21:41:22.000000 not1mm-23.5.9.2/not1mm/data/phonetics/yourcall.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51768 2023-04-21 21:41:59.000000 not1mm-23.5.9.2/not1mm/data/phonetics/z.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1600 2023-04-03 14:20:44.000000 not1mm-23.5.9.2/not1mm/data/pickcontest.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2023-02-10 02:42:40.000000 not1mm-23.5.9.2/not1mm/data/reddot.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35566 2023-04-15 16:43:11.000000 not1mm-23.5.9.2/not1mm/data/settings.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      470 2023-04-18 18:00:45.000000 not1mm-23.5.9.2/not1mm/data/ssbmacros.txt
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-10 04:06:27.178200 not1mm-23.5.9.2/not1mm/lib/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.5.9.2/not1mm/lib/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      379 2023-04-10 20:24:21.000000 not1mm-23.5.9.2/not1mm/lib/about.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13705 2023-05-07 16:50:54.000000 not1mm-23.5.9.2/not1mm/lib/cat_interface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1772 2023-03-17 21:26:43.000000 not1mm-23.5.9.2/not1mm/lib/cwinterface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    34193 2023-05-05 18:13:45.000000 not1mm-23.5.9.2/not1mm/lib/database.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      357 2023-03-20 13:17:21.000000 not1mm-23.5.9.2/not1mm/lib/edit_contact.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      559 2023-03-06 17:59:31.000000 not1mm-23.5.9.2/not1mm/lib/edit_macro.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-06 18:02:53.000000 not1mm-23.5.9.2/not1mm/lib/edit_opon.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1973 2023-04-11 17:58:02.000000 not1mm-23.5.9.2/not1mm/lib/edit_station.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8760 2023-04-05 20:29:02.000000 not1mm-23.5.9.2/not1mm/lib/ham_utility.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13916 2023-03-07 18:49:31.000000 not1mm-23.5.9.2/not1mm/lib/lookup.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1999 2023-04-12 19:58:03.000000 not1mm-23.5.9.2/not1mm/lib/multicast.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4434 2023-03-17 16:20:37.000000 not1mm-23.5.9.2/not1mm/lib/n1mm.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      354 2023-03-28 20:21:24.000000 not1mm-23.5.9.2/not1mm/lib/new_contest.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-31 21:22:27.000000 not1mm-23.5.9.2/not1mm/lib/select_contest.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6188 2023-05-06 20:36:00.000000 not1mm-23.5.9.2/not1mm/lib/settings.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       48 2023-05-10 04:00:32.000000 not1mm-23.5.9.2/not1mm/lib/version.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    30275 2023-05-09 15:02:00.000000 not1mm-23.5.9.2/not1mm/logwindow.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-10 04:06:27.230200 not1mm-23.5.9.2/not1mm/plugins/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13746 2023-05-05 16:08:13.000000 not1mm-23.5.9.2/not1mm/plugins/10_10_fall_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13752 2023-05-05 16:08:31.000000 not1mm-23.5.9.2/not1mm/plugins/10_10_spring_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13759 2023-05-05 16:08:41.000000 not1mm-23.5.9.2/not1mm/plugins/10_10_summer_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13762 2023-05-05 16:08:51.000000 not1mm-23.5.9.2/not1mm/plugins/10_10_winter_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-20 21:20:03.000000 not1mm-23.5.9.2/not1mm/plugins/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14549 2023-05-05 16:08:59.000000 not1mm-23.5.9.2/not1mm/plugins/arrl_dx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14552 2023-05-05 16:09:07.000000 not1mm-23.5.9.2/not1mm/plugins/arrl_dx_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12990 2023-05-05 16:10:17.000000 not1mm-23.5.9.2/not1mm/plugins/arrl_field_day.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2860 2023-05-05 16:10:11.000000 not1mm-23.5.9.2/not1mm/plugins/arrl_rtty_ru.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15941 2023-05-05 19:46:43.000000 not1mm-23.5.9.2/not1mm/plugins/arrl_ss_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15946 2023-05-05 19:54:23.000000 not1mm-23.5.9.2/not1mm/plugins/arrl_ss_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14939 2023-05-08 19:30:37.000000 not1mm-23.5.9.2/not1mm/plugins/cq_wpx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15026 2023-05-05 16:10:01.000000 not1mm-23.5.9.2/not1mm/plugins/cq_wpx_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13895 2023-05-05 16:09:55.000000 not1mm-23.5.9.2/not1mm/plugins/cq_ww_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13899 2023-05-05 16:11:06.000000 not1mm-23.5.9.2/not1mm/plugins/cq_ww_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14753 2023-05-05 16:11:03.000000 not1mm-23.5.9.2/not1mm/plugins/cwt.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7453 2023-05-05 16:10:58.000000 not1mm-23.5.9.2/not1mm/plugins/general_logging.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13854 2023-05-05 16:10:55.000000 not1mm-23.5.9.2/not1mm/plugins/jidx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13855 2023-05-05 16:10:48.000000 not1mm-23.5.9.2/not1mm/plugins/jidx_ph.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3121 2023-05-05 16:11:15.000000 not1mm-23.5.9.2/not1mm/plugins/winter_field_day.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-10 04:06:27.232200 not1mm-23.5.9.2/not1mm/testing/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2023-05-05 15:04:14.000000 not1mm-23.5.9.2/not1mm/testing/test.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-10 04:06:26.980197 not1mm-23.5.9.2/not1mm.egg-info/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    25132 2023-05-10 04:06:26.000000 not1mm-23.5.9.2/not1mm.egg-info/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3443 2023-05-10 04:06:26.000000 not1mm-23.5.9.2/not1mm.egg-info/SOURCES.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-05-10 04:06:26.000000 not1mm-23.5.9.2/not1mm.egg-info/dependency_links.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2023-05-10 04:06:26.000000 not1mm-23.5.9.2/not1mm.egg-info/entry_points.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       64 2023-05-10 04:06:26.000000 not1mm-23.5.9.2/not1mm.egg-info/requires.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       33 2023-05-10 04:06:26.000000 not1mm-23.5.9.2/not1mm.egg-info/top_level.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1219 2023-05-10 04:01:51.000000 not1mm-23.5.9.2/pyproject.toml
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-05-10 04:06:27.241201 not1mm-23.5.9.2/setup.cfg
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-10 04:06:27.234200 not1mm-23.5.9.2/testing/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2248 2023-03-07 22:04:42.000000 not1mm-23.5.9.2/testing/test.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-02 14:44:35.521264 not1mm-23.6.2/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-05-05 15:15:13.000000 not1mm-23.6.2/LICENSE
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    29969 2023-06-02 14:44:35.521264 not1mm-23.6.2/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    29223 2023-06-02 14:30:06.000000 not1mm-23.6.2/README.md
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-02 14:44:35.467265 not1mm-23.6.2/not1mm/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.6.2/not1mm/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    89811 2023-06-02 13:41:52.000000 not1mm-23.6.2/not1mm/__main__.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    25525 2023-06-01 00:41:28.000000 not1mm-23.6.2/not1mm/bandmap.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-02 14:44:35.486265 not1mm-23.6.2/not1mm/data/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-01-27 16:44:51.000000 not1mm-23.6.2/not1mm/data/JetBrainsMono-Regular.ttf
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   542666 2023-02-14 19:22:02.000000 not1mm-23.6.2/not1mm/data/MASTER.SCP
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2067 2023-05-18 23:48:17.000000 not1mm-23.6.2/not1mm/data/about.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      224 2023-04-18 03:49:58.000000 not1mm-23.6.2/not1mm/data/alpha bravo charlie delta.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5246 2023-05-01 15:41:16.000000 not1mm-23.6.2/not1mm/data/bandmap.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      387 2023-03-15 16:56:38.000000 not1mm-23.6.2/not1mm/data/check.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    41522 2023-05-23 20:03:51.000000 not1mm-23.6.2/not1mm/data/configuration.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    89307 2023-03-07 17:30:38.000000 not1mm-23.6.2/not1mm/data/contests.sql
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)  4635080 2023-06-02 13:47:30.000000 not1mm-23.6.2/not1mm/data/cty.json
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)  4534539 2023-06-02 13:43:39.000000 not1mm-23.6.2/not1mm/data/cty_old.json
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      451 2023-04-11 19:54:10.000000 not1mm-23.6.2/not1mm/data/cwmacros.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       78 2023-05-19 04:25:57.000000 not1mm-23.6.2/not1mm/data/donors.html
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    19280 2023-03-20 20:22:09.000000 not1mm-23.6.2/not1mm/data/editcontact.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2273 2023-02-21 14:39:24.000000 not1mm-23.6.2/not1mm/data/editmacro.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      474 2023-02-10 02:42:18.000000 not1mm-23.6.2/not1mm/data/greendot.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2023-02-09 20:47:40.000000 not1mm-23.6.2/not1mm/data/k6gte-not1mm.desktop
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4010 2023-02-09 20:45:38.000000 not1mm-23.6.2/not1mm/data/k6gte.not1mm-128.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1108 2023-02-09 20:45:03.000000 not1mm-23.6.2/not1mm/data/k6gte.not1mm-32.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2152 2023-02-09 20:45:22.000000 not1mm-23.6.2/not1mm/data/k6gte.not1mm-64.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      970 2023-03-23 20:14:51.000000 not1mm-23.6.2/not1mm/data/logwindow.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    44138 2023-05-31 18:11:05.000000 not1mm-23.6.2/not1mm/data/main.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    17963 2023-05-05 12:59:56.000000 not1mm-23.6.2/not1mm/data/new_contest.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2018 2023-02-12 17:56:36.000000 not1mm-23.6.2/not1mm/data/opon.ui
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-02 14:44:35.513264 not1mm-23.6.2/not1mm/data/phonetics/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42590 2023-04-21 20:24:24.000000 not1mm-23.6.2/not1mm/data/phonetics/0.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30248 2023-04-21 20:25:33.000000 not1mm-23.6.2/not1mm/data/phonetics/1.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    29584 2023-04-21 20:27:16.000000 not1mm-23.6.2/not1mm/data/phonetics/2.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32072 2023-04-21 20:29:07.000000 not1mm-23.6.2/not1mm/data/phonetics/3.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43052 2023-04-21 20:29:49.000000 not1mm-23.6.2/not1mm/data/phonetics/4.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51976 2023-04-21 21:46:26.000000 not1mm-23.6.2/not1mm/data/phonetics/5.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58634 2023-04-21 21:08:45.000000 not1mm-23.6.2/not1mm/data/phonetics/6.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49154 2023-04-21 21:10:50.000000 not1mm-23.6.2/not1mm/data/phonetics/7.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32842 2023-04-21 21:13:51.000000 not1mm-23.6.2/not1mm/data/phonetics/73.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35636 2023-04-21 21:11:40.000000 not1mm-23.6.2/not1mm/data/phonetics/8.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    39592 2023-04-21 21:12:32.000000 not1mm-23.6.2/not1mm/data/phonetics/9.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46800 2023-04-21 21:14:36.000000 not1mm-23.6.2/not1mm/data/phonetics/a.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    44594 2023-04-21 21:15:20.000000 not1mm-23.6.2/not1mm/data/phonetics/again.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40976 2023-04-21 21:16:10.000000 not1mm-23.6.2/not1mm/data/phonetics/b.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46746 2023-04-21 21:17:07.000000 not1mm-23.6.2/not1mm/data/phonetics/c.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    62558 2023-04-21 13:38:05.000000 not1mm-23.6.2/not1mm/data/phonetics/contest.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    92498 2023-04-21 21:17:54.000000 not1mm-23.6.2/not1mm/data/phonetics/cq.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52524 2023-04-21 21:18:24.000000 not1mm-23.6.2/not1mm/data/phonetics/d.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    45700 2023-04-21 21:19:02.000000 not1mm-23.6.2/not1mm/data/phonetics/e.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    53438 2023-04-21 21:19:38.000000 not1mm-23.6.2/not1mm/data/phonetics/f.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42766 2023-04-21 21:20:18.000000 not1mm-23.6.2/not1mm/data/phonetics/g.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50040 2023-04-21 21:21:03.000000 not1mm-23.6.2/not1mm/data/phonetics/h.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46372 2023-04-21 21:23:33.000000 not1mm-23.6.2/not1mm/data/phonetics/i.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43434 2023-04-21 21:24:12.000000 not1mm-23.6.2/not1mm/data/phonetics/j.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49066 2023-04-21 21:24:57.000000 not1mm-23.6.2/not1mm/data/phonetics/k.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   185562 2023-04-21 21:25:43.000000 not1mm-23.6.2/not1mm/data/phonetics/k6gte.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43154 2023-04-21 21:26:21.000000 not1mm-23.6.2/not1mm/data/phonetics/l.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    54352 2023-04-21 21:27:07.000000 not1mm-23.6.2/not1mm/data/phonetics/m.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56798 2023-04-21 21:27:57.000000 not1mm-23.6.2/not1mm/data/phonetics/mynumber.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52204 2023-04-21 21:28:42.000000 not1mm-23.6.2/not1mm/data/phonetics/n.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   154544 2023-04-21 21:29:54.000000 not1mm-23.6.2/not1mm/data/phonetics/nil.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47440 2023-04-21 21:30:37.000000 not1mm-23.6.2/not1mm/data/phonetics/o.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    38300 2023-04-21 21:31:22.000000 not1mm-23.6.2/not1mm/data/phonetics/p.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    55288 2023-04-21 21:31:58.000000 not1mm-23.6.2/not1mm/data/phonetics/q.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47432 2023-04-21 21:32:39.000000 not1mm-23.6.2/not1mm/data/phonetics/r.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46122 2023-04-21 21:33:20.000000 not1mm-23.6.2/not1mm/data/phonetics/roger.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    60698 2023-04-21 21:33:59.000000 not1mm-23.6.2/not1mm/data/phonetics/s.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    70424 2023-04-17 20:43:04.000000 not1mm-23.6.2/not1mm/data/phonetics/space.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58196 2023-04-21 21:35:28.000000 not1mm-23.6.2/not1mm/data/phonetics/t.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56320 2023-04-21 21:36:54.000000 not1mm-23.6.2/not1mm/data/phonetics/thankyou.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    94980 2023-04-21 21:37:27.000000 not1mm-23.6.2/not1mm/data/phonetics/thankyouqrz.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    65922 2023-04-21 21:38:05.000000 not1mm-23.6.2/not1mm/data/phonetics/u.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50142 2023-04-21 21:38:37.000000 not1mm-23.6.2/not1mm/data/phonetics/v.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    37638 2023-04-21 21:39:21.000000 not1mm-23.6.2/not1mm/data/phonetics/w.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    61870 2023-04-21 21:40:02.000000 not1mm-23.6.2/not1mm/data/phonetics/x.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56524 2023-04-21 21:40:40.000000 not1mm-23.6.2/not1mm/data/phonetics/y.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46510 2023-04-21 21:41:22.000000 not1mm-23.6.2/not1mm/data/phonetics/yourcall.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51768 2023-04-21 21:41:59.000000 not1mm-23.6.2/not1mm/data/phonetics/z.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1600 2023-04-03 14:20:44.000000 not1mm-23.6.2/not1mm/data/pickcontest.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2023-02-10 02:42:40.000000 not1mm-23.6.2/not1mm/data/reddot.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35566 2023-04-15 16:43:11.000000 not1mm-23.6.2/not1mm/data/settings.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      470 2023-04-18 18:00:45.000000 not1mm-23.6.2/not1mm/data/ssbmacros.txt
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-02 14:44:35.516264 not1mm-23.6.2/not1mm/lib/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.6.2/not1mm/lib/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      379 2023-04-10 20:24:21.000000 not1mm-23.6.2/not1mm/lib/about.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15676 2023-05-22 20:40:03.000000 not1mm-23.6.2/not1mm/lib/cat_interface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3123 2023-05-11 20:24:55.000000 not1mm-23.6.2/not1mm/lib/cwinterface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    34356 2023-05-24 20:24:28.000000 not1mm-23.6.2/not1mm/lib/database.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      357 2023-03-20 13:17:21.000000 not1mm-23.6.2/not1mm/lib/edit_contact.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      559 2023-03-06 17:59:31.000000 not1mm-23.6.2/not1mm/lib/edit_macro.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-06 18:02:53.000000 not1mm-23.6.2/not1mm/lib/edit_opon.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1973 2023-04-11 17:58:02.000000 not1mm-23.6.2/not1mm/lib/edit_station.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8760 2023-04-05 20:29:02.000000 not1mm-23.6.2/not1mm/lib/ham_utility.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13916 2023-03-07 18:49:31.000000 not1mm-23.6.2/not1mm/lib/lookup.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1761 2023-05-12 16:20:09.000000 not1mm-23.6.2/not1mm/lib/multicast.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5713 2023-05-24 14:24:14.000000 not1mm-23.6.2/not1mm/lib/n1mm.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      354 2023-03-28 20:21:24.000000 not1mm-23.6.2/not1mm/lib/new_contest.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-31 21:22:27.000000 not1mm-23.6.2/not1mm/lib/select_contest.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6885 2023-05-23 19:07:39.000000 not1mm-23.6.2/not1mm/lib/settings.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       46 2023-06-02 14:26:27.000000 not1mm-23.6.2/not1mm/lib/version.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1286 2023-05-19 19:40:38.000000 not1mm-23.6.2/not1mm/lib/versiontest.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    33732 2023-05-30 16:14:11.000000 not1mm-23.6.2/not1mm/logwindow.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-02 14:44:35.519264 not1mm-23.6.2/not1mm/plugins/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13883 2023-05-29 18:30:11.000000 not1mm-23.6.2/not1mm/plugins/10_10_fall_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13888 2023-05-29 18:30:48.000000 not1mm-23.6.2/not1mm/plugins/10_10_spring_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13895 2023-05-29 18:31:29.000000 not1mm-23.6.2/not1mm/plugins/10_10_summer_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13898 2023-05-29 18:31:57.000000 not1mm-23.6.2/not1mm/plugins/10_10_winter_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-20 21:20:03.000000 not1mm-23.6.2/not1mm/plugins/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14684 2023-05-29 18:32:51.000000 not1mm-23.6.2/not1mm/plugins/arrl_dx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14687 2023-05-29 18:33:05.000000 not1mm-23.6.2/not1mm/plugins/arrl_dx_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13125 2023-05-29 18:33:21.000000 not1mm-23.6.2/not1mm/plugins/arrl_field_day.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2860 2023-05-05 16:10:11.000000 not1mm-23.6.2/not1mm/plugins/arrl_rtty_ru.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    16077 2023-05-29 18:33:47.000000 not1mm-23.6.2/not1mm/plugins/arrl_ss_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    16082 2023-05-29 18:34:01.000000 not1mm-23.6.2/not1mm/plugins/arrl_ss_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15301 2023-05-29 18:25:56.000000 not1mm-23.6.2/not1mm/plugins/cq_wpx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15323 2023-05-29 18:34:21.000000 not1mm-23.6.2/not1mm/plugins/cq_wpx_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14031 2023-05-29 18:34:36.000000 not1mm-23.6.2/not1mm/plugins/cq_ww_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14035 2023-05-29 18:34:53.000000 not1mm-23.6.2/not1mm/plugins/cq_ww_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14890 2023-05-29 18:35:16.000000 not1mm-23.6.2/not1mm/plugins/cwt.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7453 2023-05-05 16:10:58.000000 not1mm-23.6.2/not1mm/plugins/general_logging.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13854 2023-05-05 16:10:55.000000 not1mm-23.6.2/not1mm/plugins/jidx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13855 2023-05-05 16:10:48.000000 not1mm-23.6.2/not1mm/plugins/jidx_ph.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3121 2023-05-05 16:11:15.000000 not1mm-23.6.2/not1mm/plugins/winter_field_day.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-02 14:44:35.519264 not1mm-23.6.2/not1mm/testing/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2083 2023-05-19 23:10:32.000000 not1mm-23.6.2/not1mm/testing/fakeflrig.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1658 2023-05-19 17:23:54.000000 not1mm-23.6.2/not1mm/testing/flrigclient.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1099 2023-05-24 18:38:16.000000 not1mm-23.6.2/not1mm/testing/n1mm_listener.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1660 2023-05-14 06:26:14.000000 not1mm-23.6.2/not1mm/testing/test.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-02 14:44:35.468265 not1mm-23.6.2/not1mm.egg-info/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    29969 2023-06-02 14:44:35.000000 not1mm-23.6.2/not1mm.egg-info/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3582 2023-06-02 14:44:35.000000 not1mm-23.6.2/not1mm.egg-info/SOURCES.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-06-02 14:44:35.000000 not1mm-23.6.2/not1mm.egg-info/dependency_links.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2023-06-02 14:44:35.000000 not1mm-23.6.2/not1mm.egg-info/entry_points.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       83 2023-06-02 14:44:35.000000 not1mm-23.6.2/not1mm.egg-info/requires.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       33 2023-06-02 14:44:35.000000 not1mm-23.6.2/not1mm.egg-info/top_level.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1261 2023-06-02 14:26:13.000000 not1mm-23.6.2/pyproject.toml
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-06-02 14:44:35.522264 not1mm-23.6.2/setup.cfg
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-02 14:44:35.520264 not1mm-23.6.2/testing/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      176 2023-05-31 20:52:45.000000 not1mm-23.6.2/testing/test.py
```

### Comparing `not1mm-23.5.9.2/LICENSE` & `not1mm-23.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/PKG-INFO` & `not1mm-23.6.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,79 +1,89 @@
 Metadata-Version: 2.1
 Name: not1mm
-Version: 23.5.9.2
+Version: 23.6.2
 Summary: NOT1MM Logger
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/not1mm
 Project-URL: Bug Tracker, https://github.com/mbridak/not1mm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Environment :: X11 Applications :: Qt
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Natural Language :: English
 Classifier: Topic :: Communications :: Ham Radio
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Not1MM
 
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
-[![Python: 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/)
+[![Python: 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/)
 [![Made With:PyQt5](https://img.shields.io/badge/Made%20with-PyQt5-red)](https://pypi.org/project/PyQt5/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/not1mm)](https://pypi.org/project/not1mm/)
 
 ![logo](https://github.com/mbridak/not1mm/raw/master/not1mm/data/k6gte.not1mm.svg)
 
 - [Not1MM](#not1mm)
   - [What and why is Not1MM](#what-and-why-is-not1mm)
   - [Current state](#current-state)
+  - [Thanks to the Contributors](#thanks-to-the-contributors)
+    - [:moneybag: Monitarily](#moneybag-monitarily)
+    - [:cockroach: Bug reports and Feature suggestions](#cockroach-bug-reports-and-feature-suggestions)
   - [List of should be working contests](#list-of-should-be-working-contests)
   - [Changes of note](#changes-of-note)
   - [Installing from PyPi](#installing-from-pypi)
     - [Python and pip](#python-and-pip)
     - [Installing with pip](#installing-with-pip)
-    - [Updating with pip](#updating-with-pip)
+      - [Ubuntu 22.04 LTS](#ubuntu-2204-lts)
+      - [Ubuntu 23.04](#ubuntu-2304)
+      - [Fedora 38](#fedora-38)
+    - [You may or may not get a warning message like](#you-may-or-may-not-get-a-warning-message-like)
+    - [Or this fan favorite](#or-this-fan-favorite)
+    - [Updating with pip/pipx](#updating-with-pippipx)
   - [Other Libraries](#other-libraries)
-  - [Running on Ubuntu LTS 22.04](#running-on-ubuntu-lts-2204)
+    - [Dark mode on Ubuntu](#dark-mode-on-ubuntu)
+  - [Wayland Compositor](#wayland-compositor)
   - [Running from source](#running-from-source)
   - [Various data file locations](#various-data-file-locations)
     - [Data](#data)
     - [Config](#config)
   - [The database](#the-database)
     - [Why](#why)
     - [The first one](#the-first-one)
     - [Why limit yourself](#why-limit-yourself)
     - [Revisiting an old friend](#revisiting-an-old-friend)
   - [Station Settings dialog](#station-settings-dialog)
     - [Changing station information](#changing-station-information)
   - [Adding a contest to the current dababase](#adding-a-contest-to-the-current-dababase)
   - [Selecting an existing contest as the current contest](#selecting-an-existing-contest-as-the-current-contest)
-  - [Editing an existing contest parameters](#editing-an-existing-contest-parameters)
+  - [Editing existing contest parameters](#editing-existing-contest-parameters)
   - [Configuration Settings](#configuration-settings)
     - [Lookup](#lookup)
     - [Soundcard](#soundcard)
     - [CAT](#cat)
     - [CW Keyer interface](#cw-keyer-interface)
     - [Cluster](#cluster)
+    - [N1MM Packets](#n1mm-packets)
   - [Hiding screen elements](#hiding-screen-elements)
   - [Editing macro keys](#editing-macro-keys)
     - [Macro substitutions](#macro-substitutions)
     - [Macro use with voice](#macro-use-with-voice)
   - [cty.dat and QRZ lookups for distance and bearing](#ctydat-and-qrz-lookups-for-distance-and-bearing)
   - [Other uses for the call field](#other-uses-for-the-call-field)
   - [Windows](#windows)
     - [The Main Window](#the-main-window)
       - [Keyboard commands](#keyboard-commands)
     - [Log Display](#log-display)
       - [Editing a contact](#editing-a-contact)
-    - [Bandmap](#bandmap)
   - [Recalulate Mults](#recalulate-mults)
+    - [Bandmap](#bandmap)
   - [Cabrillo](#cabrillo)
   - [ADIF](#adif)
   - [Dupe checking](#dupe-checking)
   - [Contest specific notes](#contest-specific-notes)
     - [ARRL Sweekstakes](#arrl-sweekstakes)
       - [The exchange parser](#the-exchange-parser)
       - [The exchange](#the-exchange)
@@ -93,14 +103,26 @@
 
 ## Current state
 
 The current state is "**BETA**". I've used it for A few contests, and was able to work contacts and submit a cabrillo at the end. I'm not a "Contester". So I'll add contests as/if I work them. I'm only one guy, so if you see a bug let me know. I don't do much of any Data or RTTY operating. This is why you don't see RTTY in the list of working contests. The Lord helps those who burn people at the... I mean who help themselves. Feel free to fill in that hole with a pull request.
 
 ![main screen](https://github.com/mbridak/not1mm/raw/master/pic/main.png)
 
+## Thanks to the Contributors
+
+I wish to thank those who've contributed to the project.
+
+### :moneybag: Monitarily
+
+Brian KB3ORR
+
+### :cockroach: Bug reports and Feature suggestions
+
+Simon G0FCU, Brian KB3ORR, Onno VK6FLAB, Martin OK1RR
+
 ## List of should be working contests
 
 - General Logging
 - 10 10 Fall CW
 - 10 10 Spring CW
 - 10 10 Summer Phone
 - 10 10 Winter Phone
@@ -114,23 +136,48 @@
 - CQ World Wide SSB
 - CWOps CWT
 - Japan International DX CW
 - Japan International DX SSB
 
 ## Changes of note
 
+- [23-6-2] Added an automated check and update of the cty.dat file. Added dependency to `notctyparser`
+
+<details>
+
+<summary>May 2023</summary>
+
+- [23-5-31] updated cty.json ( I need to automate this )
+- [23-5-30] Changed the default multicast group from 224.1.1.1 to 239.1.1.1 This restricts broadcast traffic to the local subnet.
+- [23-5-29] Hide CATEGORY-OVERLAY in Cabrillo file if set to N/A.
+- [23-5-28] Fixed Dupe check on TAB.
+- [23-5-27] Fixed frequency in the ADIF output. Corrected WPX contact points.
+- [23-5-26] Fixed Dark Mode on Ubuntu. Removed the crappy dark css theme and the code to load it. OOPS. Fixed some stuff.
+- [23-5-24] Added contact delete and change n1mm packets.
+- [23-5-23] Reworked N1MM packets. Can now specify multiple destinations for the packets.
+- [23-5-22] Worked on n1mm contactinfo packets. Reduced network beaconing from 100 miliseconds to 10 seconds, Unless the radio state changes.
+- [23-5-20] Got n1mm RadioInfo posting.
+- [23-5-19] Added a version check at startup. Starting work on N1MM packet broadcasts. Corrected flrig return value of bandwidth. Changed get Next/Prev bandmap spot to Arrow Up/Down.
+- [23-5-18] ReInit rigctld CAT when it goes offline and back.
+- [23-5-17] CTRL-G tunes to a spot matching text in the callsign entry field. Thanks to Martin, OK1RR for suggesting this. Bandmap centers on the VFO after frequency change. Set mode on startup based on the mode category set for the contest.
+- [23-5-15] CTRL-S in the main window will send a spot to the cluster.
+- [23-5-12] Bandmap, Reload system preferences before each connect. Increased the minimum Python version to 3.10. Main, Refactored UDP code to remove the use of timers and queues, replaced with readyRead signals.
+- [23-5-11] Added missing numpy package dependency to pyproject.toml. Added install steps for clean images of Fedora and Ubuntu. Entered frequencies when no CAT control are not sent to the bandmap. Added K1EL speed change via xmlrpc. One would need to update the pywinkeyerserial client.
+- [23-5-10] Fix crash in bandmap when No CAT, and using CTRL-PgUp/Down. Add specific Ubuntu install instructions.
 - [23-5-9] Removed 1 second timers in the bandmap and log window, made them UDP readyRead(). Much smoother. Add CTRL-PgUp and CTRL-PgDown keys to jump to the next/prev spots in the bandmap. Fix: Voice not keying on LSB. Fix: calling pttoff when no CAT interface. Fix: Voice not keying on LSB
 - [23-5-8] Bandmap zoom in/out now centers scale to RX Freq.
 - [23-5-7] Added bandwidth marker to the bandmap.
 - [23-5-6] Added AR Cluster filter options for the bandmap. Added a station ID to the multicast packets. This will prevent erratic bevahiour if 2 stations are on the same network.
 - [23-5-5] Re-wrote most of the log window code. Added ARRL Sweepstakes.
 - [23-5-4] Fixed 'Operators' line in WPX cabrillo file. Fix window title not updating if no CAT control.
 - [23-5-3] Added '#' macro.
 - [23-5-1] Added 10 10 CW and Phone contests. Added a `Cluster` TAB for the AR Cluster server/port in the configuration settings.
 
+</details>
+
 <details>
 
 <summary>April 2023</summary>
 
 - [23-4-29] Added callsign and connect button to the bandmap. Fixed rxmarker not updateing.
 - [23-4-28] Added a bandmap window (WIP) to track spots. Clicked spots now tune radio and sets callsign.
 - [23-4-24] CWT now prefills exchange based on past CWT contacts in database. Fixed crash when editing an existing contest that does not exist. Removed legacy stylesheet from configuration settings dialog.
@@ -188,42 +235,88 @@
 
 </details>
 
 ## Installing from PyPi
 
 ### Python and pip
 
-This software is a Python package hosted on PyPi, and installable with the pip command. If this is your first exposure to pip you can get all the details from [The PyPA](https://packaging.python.org/en/latest/tutorials/installing-packages/). In short, most linux distros come with Python pre installed. And pip usually comes with Python as a standard module. If pip is not installed by default, you can usually load it through your package manager. For example `sudo apt install python3-pip` or `sudo dnf install python3-pip`.
+This software is a Python package hosted on PyPi, and installable with the pip or pipx command. If this is your first exposure to pip you can get all the details from [The PyPA](https://packaging.python.org/en/latest/tutorials/installing-packages/). In short, most linux distros come with Python pre installed. If pip is not installed by default, you can usually load it through your package manager. For example `sudo apt install python3-pip` or `sudo dnf install python3-pip`.
 
 ### Installing with pip
 
-But just try `pip install not1mm` in your terminal. Once it's installed just type `not1mm` in the same terminal. On the first run, the program will install a launchable icon, which you can then click on to run like a normal program.
+I've included what installation steps I took to install on fresh images of Ubuntu and Fedora below. YMMV.
 
-### Updating with pip
+#### Ubuntu 22.04 LTS
 
-I've been posting updates just about everyday. Sometimes multiple times a day. It's early days, so there is much to do. You can check for and install updates with `pip install -U not1mm`.
+```bash
+sudo apt update
+sudo apt upgrade
+sudo apt install -y libportaudio2 python3-pip python3-pyqt5 python3-numpy adwaita-qt
+pip install -U not1mm
+```
 
-## Other Libraries
+#### Ubuntu 23.04
 
-The audio library used, uses pipewire/portaudio. You may need to install portaudio. Ubuntu: `sudo apt install libportaudio2`
+```bash
+sudo apt update
+sudo apt upgrade
+sudo apt install -y libportaudio2 adwaita-qt pipx
+pipx install not1mm
+pipx ensurepath
+```
+
+Open a new terminal and type `not1mm`
+
+#### Fedora 38
+
+```bash
+sudo dnf upgrade --refresh
+sudo dnf install python3-pip portaudio
+pip install not1mm
+```
+
+### You may or may not get a warning message like
 
-## Running on Ubuntu LTS 22.04
+```text
+WARNING: The script not1mm is installed in '/home/mbridak/.local/bin' which is not on PATH.
+Consider adding this directory to PATH or, if you prefer to suppress this warning, use --no-warn-script-location.
+```
+
+If you do, just logout and back in, or reboot.
 
-Seems Ubuntu LTS is not a big fan of wayland. When launching from the command line you'll see a message:
+### Or this fan favorite
 
-`Warning: Ignoring XDG_SESSION_TYPE=wayland on Gnome. Use QT_QPA_PLATFORM=wayland to run on Wayland anyway.
+```text
+Warning: Ignoring XDG_SESSION_TYPE=wayland on Gnome. Use QT_QPA_PLATFORM=wayland to run on Wayland anyway.
 qt.qpa.plugin: Could not load the Qt platform plugin "xcb" in "" even though it was found.
-This application failed to start because no Qt platform plugin could be initialized. Reinstalling the application may fix this problem.`
+This application failed to start because no Qt platform plugin could be initialized. Reinstalling the application may fix this problem.
+```
 
 To avoid this you can export an environment variable and launch the app like this:
 
 `mbridak@vm:~$ export QT_QPA_PLATFORM=wayland; not1mm`
 
 For a more permanent solution you can place the line `export QT_QPA_PLATFORM=wayland` in your home directories .bashrc file. Then after logging out and back in you should be able to launch it normally.
 
+### Updating with pip/pipx
+
+I've been posting updates just about everyday. Sometimes multiple times a day. It's early days, so there is much to do. You can check for and install updates with `pip install -U not1mm` or if installed with pipx `pipx upgrade not1mm`.
+
+## Other Libraries
+
+The audio library used, uses pipewire/portaudio. You may need to install portaudio. Ubuntu: `sudo apt install libportaudio2`
+
+### Dark mode on Ubuntu
+
+I believe I figured out dark mode in Ubuntu and have it working on my shack PC that runs Ubuntu 22.04. The secret sauce seems to be installing adwaita-qt with apt, and setting an environment variable `QT_STYLE_OVERRIDE` to `Adwaita-Dark`. I set the environment variable in the start of the program if running on a Gnome platform. So you don't need to do that part.
+
+## Wayland Compositor
+
+One side effect of Wayland is that we are not able to request for a window to regain or retain focus. So if you were to click on a spot in the bandmap window to tune to that spot, you would have to then click on the main window to continue entering contest data. I'm aware of this, but i can not change it.
+
 ## Running from source
 
 Since this is packaged for PyPi, if you want to work on your own source branch, after cloning from github you would:
 
 ```bash
 pip install --upgrade pip
 pip install setuptools
@@ -299,15 +392,15 @@
 
 ## Selecting an existing contest as the current contest
 
 Select `File` > `Open Contest`
 
 ![Open an existing contest](https://github.com/mbridak/not1mm/raw/master/pic/select_contest.png)
 
-## Editing an existing contest parameters
+## Editing existing contest parameters
 
 You can edit the parameters of a previously defined contest by selecting it as the current contest. Then select `File` > `Edit Current Contest`. Click `OK` to save the new values and reload the contest. `Cancel` to keep the existing parameters.
 
 ## Configuration Settings
 
 To setup your CAT control, CW keyer, Callsign lookups, select `File` > `Configuration Settings`
 
@@ -333,14 +426,22 @@
 
 ### Cluster
 
 ![Configuration Settings screen](https://github.com/mbridak/not1mm/raw/master/pic/configuration_cluster.png)
 
   Under the `Cluster` TAB you can change the default AR Cluster server, port and filter settings used for the bandmap window.
 
+### N1MM Packets
+
+Work has started on N1MM udp packets. So far just RadioInfo, contactinfo, contactreplace and contactdelete.
+
+![N1MM Packet Configuration Screen](https://github.com/mbridak/not1mm/blob/master/pic/n1mm_packet_config.png?raw=true)
+
+When entering IP and Ports, enter them with a colon ':' between them. You can enter multiple pairs on the same line if separated by a space ' '.
+
 ## Hiding screen elements
 
 You can show or hide certain buttons/indicators by checking and unchecking their boxes under the view menu. You can then resize the screen to make it more compact.
 
 ![View Menu](https://github.com/mbridak/not1mm/raw/master/pic/view_menu.png)
 
 The your choices will be remembered when you relaunch the program.
@@ -388,27 +489,31 @@
 
 **You must press the SPACE bar after entering any of the above.**
 
 ## Windows
 
 ### The Main Window
 
+![Main screen with callouts](https://github.com/mbridak/not1mm/raw/master/pic/mainwithcallouts.png)
+
 #### Keyboard commands
 
 - [Esc] Clears the input fields of any text.
 - [CTRL-Esc] Stops cwdaemon from sending Morse.
-- [PgUp] Increases the cwdaemon sending speed.
-- [PgDown] Decreases the cwdaemon sending speed.
-- [CTRL-PgUp] Jump to the next spot above the current VFO cursor in the bamdmap window.
-- [CTRL-PgDown] Jump to the next spot below the current VFO cursor in the bamdmap window.
+- [PgUp] Increases the cw sending speed.
+- [PgDown] Decreases the cw sending speed.
+- [Arrow-Up] Jump to the next spot above the current VFO cursor in the bandmap window.
+- [Arrow-Down] Jump to the next spot below the current VFO cursor in the bandmap window.
 - [TAB] Move cursor to the right one field.
 - [Shift-Tab] Move cursor left One field.
 - [SPACE] When in the callsign field, will move the input to the first field needed for the exchange.
 - [Enter] Submits the fields to the log.
 - [F1-F12] Send (CW or Voice) macros.
+- [CTRL-S] Spot Callsign to the cluster.
+- [CTRL-G] Tune to a spot matching partial text in the callsign entry field.
 
 ### Log Display
 
 `Window`>`Log Window`
 
 The Log display gets updated automatically when a contact is entered. The top half is a list of all contacts.
 
@@ -424,28 +529,28 @@
 
 You can also Right-Click on a cell to bring up the edit dialog.
 
 ![right click edit dialog](https://github.com/mbridak/not1mm/raw/master/pic/edit_dialog.png)
 
 You can not directly edit the multiplier status of a contact. Instead see the next section on recalculating mults. If you change the callsign make sure the `WPX` field is still valid.
 
+## Recalulate Mults
+
+After editing a contact and before generating a Cabrillo file. There is a Misc menu option that will recalculate the multipliers incase an edit had caused a change.
+
 ### Bandmap
 
 `Window`>`Bandmap`
 
 Put your callsign in the top and press the connect button.
 
 The bandmap window is, as with everything, a work in progress. The bandmap now follows the VFO. VFO indicator now displays as small triangle in the frequency tickmarks. A small blue rectangle shows the receivers bandwidth. Clicked on spots now tune the radio and set the callsign field.
 
 ![Bandmap Window](https://github.com/mbridak/not1mm/raw/master/pic/bandmap.png)
 
-## Recalulate Mults
-
-After editing a contact and before generating a Cabrillo file. There is a Misc menu option that will recalculate the multipliers incase an edit had caused a change.
-
 ## Cabrillo
 
 Click on `File` > `Generate Cabrillo`
 
 The file will be placed in your home directory. The name will be in the format of:
 
 `StationCall`_`ContestName`.log
```

### Comparing `not1mm-23.5.9.2/README.md` & `not1mm-23.6.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,60 +1,70 @@
 # Not1MM
 
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
-[![Python: 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/)
+[![Python: 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/)
 [![Made With:PyQt5](https://img.shields.io/badge/Made%20with-PyQt5-red)](https://pypi.org/project/PyQt5/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/not1mm)](https://pypi.org/project/not1mm/)
 
 ![logo](https://github.com/mbridak/not1mm/raw/master/not1mm/data/k6gte.not1mm.svg)
 
 - [Not1MM](#not1mm)
   - [What and why is Not1MM](#what-and-why-is-not1mm)
   - [Current state](#current-state)
+  - [Thanks to the Contributors](#thanks-to-the-contributors)
+    - [:moneybag: Monitarily](#moneybag-monitarily)
+    - [:cockroach: Bug reports and Feature suggestions](#cockroach-bug-reports-and-feature-suggestions)
   - [List of should be working contests](#list-of-should-be-working-contests)
   - [Changes of note](#changes-of-note)
   - [Installing from PyPi](#installing-from-pypi)
     - [Python and pip](#python-and-pip)
     - [Installing with pip](#installing-with-pip)
-    - [Updating with pip](#updating-with-pip)
+      - [Ubuntu 22.04 LTS](#ubuntu-2204-lts)
+      - [Ubuntu 23.04](#ubuntu-2304)
+      - [Fedora 38](#fedora-38)
+    - [You may or may not get a warning message like](#you-may-or-may-not-get-a-warning-message-like)
+    - [Or this fan favorite](#or-this-fan-favorite)
+    - [Updating with pip/pipx](#updating-with-pippipx)
   - [Other Libraries](#other-libraries)
-  - [Running on Ubuntu LTS 22.04](#running-on-ubuntu-lts-2204)
+    - [Dark mode on Ubuntu](#dark-mode-on-ubuntu)
+  - [Wayland Compositor](#wayland-compositor)
   - [Running from source](#running-from-source)
   - [Various data file locations](#various-data-file-locations)
     - [Data](#data)
     - [Config](#config)
   - [The database](#the-database)
     - [Why](#why)
     - [The first one](#the-first-one)
     - [Why limit yourself](#why-limit-yourself)
     - [Revisiting an old friend](#revisiting-an-old-friend)
   - [Station Settings dialog](#station-settings-dialog)
     - [Changing station information](#changing-station-information)
   - [Adding a contest to the current dababase](#adding-a-contest-to-the-current-dababase)
   - [Selecting an existing contest as the current contest](#selecting-an-existing-contest-as-the-current-contest)
-  - [Editing an existing contest parameters](#editing-an-existing-contest-parameters)
+  - [Editing existing contest parameters](#editing-existing-contest-parameters)
   - [Configuration Settings](#configuration-settings)
     - [Lookup](#lookup)
     - [Soundcard](#soundcard)
     - [CAT](#cat)
     - [CW Keyer interface](#cw-keyer-interface)
     - [Cluster](#cluster)
+    - [N1MM Packets](#n1mm-packets)
   - [Hiding screen elements](#hiding-screen-elements)
   - [Editing macro keys](#editing-macro-keys)
     - [Macro substitutions](#macro-substitutions)
     - [Macro use with voice](#macro-use-with-voice)
   - [cty.dat and QRZ lookups for distance and bearing](#ctydat-and-qrz-lookups-for-distance-and-bearing)
   - [Other uses for the call field](#other-uses-for-the-call-field)
   - [Windows](#windows)
     - [The Main Window](#the-main-window)
       - [Keyboard commands](#keyboard-commands)
     - [Log Display](#log-display)
       - [Editing a contact](#editing-a-contact)
-    - [Bandmap](#bandmap)
   - [Recalulate Mults](#recalulate-mults)
+    - [Bandmap](#bandmap)
   - [Cabrillo](#cabrillo)
   - [ADIF](#adif)
   - [Dupe checking](#dupe-checking)
   - [Contest specific notes](#contest-specific-notes)
     - [ARRL Sweekstakes](#arrl-sweekstakes)
       - [The exchange parser](#the-exchange-parser)
       - [The exchange](#the-exchange)
@@ -74,14 +84,26 @@
 
 ## Current state
 
 The current state is "**BETA**". I've used it for A few contests, and was able to work contacts and submit a cabrillo at the end. I'm not a "Contester". So I'll add contests as/if I work them. I'm only one guy, so if you see a bug let me know. I don't do much of any Data or RTTY operating. This is why you don't see RTTY in the list of working contests. The Lord helps those who burn people at the... I mean who help themselves. Feel free to fill in that hole with a pull request.
 
 ![main screen](https://github.com/mbridak/not1mm/raw/master/pic/main.png)
 
+## Thanks to the Contributors
+
+I wish to thank those who've contributed to the project.
+
+### :moneybag: Monitarily
+
+Brian KB3ORR
+
+### :cockroach: Bug reports and Feature suggestions
+
+Simon G0FCU, Brian KB3ORR, Onno VK6FLAB, Martin OK1RR
+
 ## List of should be working contests
 
 - General Logging
 - 10 10 Fall CW
 - 10 10 Spring CW
 - 10 10 Summer Phone
 - 10 10 Winter Phone
@@ -95,23 +117,48 @@
 - CQ World Wide SSB
 - CWOps CWT
 - Japan International DX CW
 - Japan International DX SSB
 
 ## Changes of note
 
+- [23-6-2] Added an automated check and update of the cty.dat file. Added dependency to `notctyparser`
+
+<details>
+
+<summary>May 2023</summary>
+
+- [23-5-31] updated cty.json ( I need to automate this )
+- [23-5-30] Changed the default multicast group from 224.1.1.1 to 239.1.1.1 This restricts broadcast traffic to the local subnet.
+- [23-5-29] Hide CATEGORY-OVERLAY in Cabrillo file if set to N/A.
+- [23-5-28] Fixed Dupe check on TAB.
+- [23-5-27] Fixed frequency in the ADIF output. Corrected WPX contact points.
+- [23-5-26] Fixed Dark Mode on Ubuntu. Removed the crappy dark css theme and the code to load it. OOPS. Fixed some stuff.
+- [23-5-24] Added contact delete and change n1mm packets.
+- [23-5-23] Reworked N1MM packets. Can now specify multiple destinations for the packets.
+- [23-5-22] Worked on n1mm contactinfo packets. Reduced network beaconing from 100 miliseconds to 10 seconds, Unless the radio state changes.
+- [23-5-20] Got n1mm RadioInfo posting.
+- [23-5-19] Added a version check at startup. Starting work on N1MM packet broadcasts. Corrected flrig return value of bandwidth. Changed get Next/Prev bandmap spot to Arrow Up/Down.
+- [23-5-18] ReInit rigctld CAT when it goes offline and back.
+- [23-5-17] CTRL-G tunes to a spot matching text in the callsign entry field. Thanks to Martin, OK1RR for suggesting this. Bandmap centers on the VFO after frequency change. Set mode on startup based on the mode category set for the contest.
+- [23-5-15] CTRL-S in the main window will send a spot to the cluster.
+- [23-5-12] Bandmap, Reload system preferences before each connect. Increased the minimum Python version to 3.10. Main, Refactored UDP code to remove the use of timers and queues, replaced with readyRead signals.
+- [23-5-11] Added missing numpy package dependency to pyproject.toml. Added install steps for clean images of Fedora and Ubuntu. Entered frequencies when no CAT control are not sent to the bandmap. Added K1EL speed change via xmlrpc. One would need to update the pywinkeyerserial client.
+- [23-5-10] Fix crash in bandmap when No CAT, and using CTRL-PgUp/Down. Add specific Ubuntu install instructions.
 - [23-5-9] Removed 1 second timers in the bandmap and log window, made them UDP readyRead(). Much smoother. Add CTRL-PgUp and CTRL-PgDown keys to jump to the next/prev spots in the bandmap. Fix: Voice not keying on LSB. Fix: calling pttoff when no CAT interface. Fix: Voice not keying on LSB
 - [23-5-8] Bandmap zoom in/out now centers scale to RX Freq.
 - [23-5-7] Added bandwidth marker to the bandmap.
 - [23-5-6] Added AR Cluster filter options for the bandmap. Added a station ID to the multicast packets. This will prevent erratic bevahiour if 2 stations are on the same network.
 - [23-5-5] Re-wrote most of the log window code. Added ARRL Sweepstakes.
 - [23-5-4] Fixed 'Operators' line in WPX cabrillo file. Fix window title not updating if no CAT control.
 - [23-5-3] Added '#' macro.
 - [23-5-1] Added 10 10 CW and Phone contests. Added a `Cluster` TAB for the AR Cluster server/port in the configuration settings.
 
+</details>
+
 <details>
 
 <summary>April 2023</summary>
 
 - [23-4-29] Added callsign and connect button to the bandmap. Fixed rxmarker not updateing.
 - [23-4-28] Added a bandmap window (WIP) to track spots. Clicked spots now tune radio and sets callsign.
 - [23-4-24] CWT now prefills exchange based on past CWT contacts in database. Fixed crash when editing an existing contest that does not exist. Removed legacy stylesheet from configuration settings dialog.
@@ -169,42 +216,88 @@
 
 </details>
 
 ## Installing from PyPi
 
 ### Python and pip
 
-This software is a Python package hosted on PyPi, and installable with the pip command. If this is your first exposure to pip you can get all the details from [The PyPA](https://packaging.python.org/en/latest/tutorials/installing-packages/). In short, most linux distros come with Python pre installed. And pip usually comes with Python as a standard module. If pip is not installed by default, you can usually load it through your package manager. For example `sudo apt install python3-pip` or `sudo dnf install python3-pip`.
+This software is a Python package hosted on PyPi, and installable with the pip or pipx command. If this is your first exposure to pip you can get all the details from [The PyPA](https://packaging.python.org/en/latest/tutorials/installing-packages/). In short, most linux distros come with Python pre installed. If pip is not installed by default, you can usually load it through your package manager. For example `sudo apt install python3-pip` or `sudo dnf install python3-pip`.
 
 ### Installing with pip
 
-But just try `pip install not1mm` in your terminal. Once it's installed just type `not1mm` in the same terminal. On the first run, the program will install a launchable icon, which you can then click on to run like a normal program.
+I've included what installation steps I took to install on fresh images of Ubuntu and Fedora below. YMMV.
 
-### Updating with pip
+#### Ubuntu 22.04 LTS
 
-I've been posting updates just about everyday. Sometimes multiple times a day. It's early days, so there is much to do. You can check for and install updates with `pip install -U not1mm`.
+```bash
+sudo apt update
+sudo apt upgrade
+sudo apt install -y libportaudio2 python3-pip python3-pyqt5 python3-numpy adwaita-qt
+pip install -U not1mm
+```
 
-## Other Libraries
+#### Ubuntu 23.04
 
-The audio library used, uses pipewire/portaudio. You may need to install portaudio. Ubuntu: `sudo apt install libportaudio2`
+```bash
+sudo apt update
+sudo apt upgrade
+sudo apt install -y libportaudio2 adwaita-qt pipx
+pipx install not1mm
+pipx ensurepath
+```
+
+Open a new terminal and type `not1mm`
+
+#### Fedora 38
+
+```bash
+sudo dnf upgrade --refresh
+sudo dnf install python3-pip portaudio
+pip install not1mm
+```
+
+### You may or may not get a warning message like
 
-## Running on Ubuntu LTS 22.04
+```text
+WARNING: The script not1mm is installed in '/home/mbridak/.local/bin' which is not on PATH.
+Consider adding this directory to PATH or, if you prefer to suppress this warning, use --no-warn-script-location.
+```
+
+If you do, just logout and back in, or reboot.
 
-Seems Ubuntu LTS is not a big fan of wayland. When launching from the command line you'll see a message:
+### Or this fan favorite
 
-`Warning: Ignoring XDG_SESSION_TYPE=wayland on Gnome. Use QT_QPA_PLATFORM=wayland to run on Wayland anyway.
+```text
+Warning: Ignoring XDG_SESSION_TYPE=wayland on Gnome. Use QT_QPA_PLATFORM=wayland to run on Wayland anyway.
 qt.qpa.plugin: Could not load the Qt platform plugin "xcb" in "" even though it was found.
-This application failed to start because no Qt platform plugin could be initialized. Reinstalling the application may fix this problem.`
+This application failed to start because no Qt platform plugin could be initialized. Reinstalling the application may fix this problem.
+```
 
 To avoid this you can export an environment variable and launch the app like this:
 
 `mbridak@vm:~$ export QT_QPA_PLATFORM=wayland; not1mm`
 
 For a more permanent solution you can place the line `export QT_QPA_PLATFORM=wayland` in your home directories .bashrc file. Then after logging out and back in you should be able to launch it normally.
 
+### Updating with pip/pipx
+
+I've been posting updates just about everyday. Sometimes multiple times a day. It's early days, so there is much to do. You can check for and install updates with `pip install -U not1mm` or if installed with pipx `pipx upgrade not1mm`.
+
+## Other Libraries
+
+The audio library used, uses pipewire/portaudio. You may need to install portaudio. Ubuntu: `sudo apt install libportaudio2`
+
+### Dark mode on Ubuntu
+
+I believe I figured out dark mode in Ubuntu and have it working on my shack PC that runs Ubuntu 22.04. The secret sauce seems to be installing adwaita-qt with apt, and setting an environment variable `QT_STYLE_OVERRIDE` to `Adwaita-Dark`. I set the environment variable in the start of the program if running on a Gnome platform. So you don't need to do that part.
+
+## Wayland Compositor
+
+One side effect of Wayland is that we are not able to request for a window to regain or retain focus. So if you were to click on a spot in the bandmap window to tune to that spot, you would have to then click on the main window to continue entering contest data. I'm aware of this, but i can not change it.
+
 ## Running from source
 
 Since this is packaged for PyPi, if you want to work on your own source branch, after cloning from github you would:
 
 ```bash
 pip install --upgrade pip
 pip install setuptools
@@ -280,15 +373,15 @@
 
 ## Selecting an existing contest as the current contest
 
 Select `File` > `Open Contest`
 
 ![Open an existing contest](https://github.com/mbridak/not1mm/raw/master/pic/select_contest.png)
 
-## Editing an existing contest parameters
+## Editing existing contest parameters
 
 You can edit the parameters of a previously defined contest by selecting it as the current contest. Then select `File` > `Edit Current Contest`. Click `OK` to save the new values and reload the contest. `Cancel` to keep the existing parameters.
 
 ## Configuration Settings
 
 To setup your CAT control, CW keyer, Callsign lookups, select `File` > `Configuration Settings`
 
@@ -314,14 +407,22 @@
 
 ### Cluster
 
 ![Configuration Settings screen](https://github.com/mbridak/not1mm/raw/master/pic/configuration_cluster.png)
 
   Under the `Cluster` TAB you can change the default AR Cluster server, port and filter settings used for the bandmap window.
 
+### N1MM Packets
+
+Work has started on N1MM udp packets. So far just RadioInfo, contactinfo, contactreplace and contactdelete.
+
+![N1MM Packet Configuration Screen](https://github.com/mbridak/not1mm/blob/master/pic/n1mm_packet_config.png?raw=true)
+
+When entering IP and Ports, enter them with a colon ':' between them. You can enter multiple pairs on the same line if separated by a space ' '.
+
 ## Hiding screen elements
 
 You can show or hide certain buttons/indicators by checking and unchecking their boxes under the view menu. You can then resize the screen to make it more compact.
 
 ![View Menu](https://github.com/mbridak/not1mm/raw/master/pic/view_menu.png)
 
 The your choices will be remembered when you relaunch the program.
@@ -369,27 +470,31 @@
 
 **You must press the SPACE bar after entering any of the above.**
 
 ## Windows
 
 ### The Main Window
 
+![Main screen with callouts](https://github.com/mbridak/not1mm/raw/master/pic/mainwithcallouts.png)
+
 #### Keyboard commands
 
 - [Esc] Clears the input fields of any text.
 - [CTRL-Esc] Stops cwdaemon from sending Morse.
-- [PgUp] Increases the cwdaemon sending speed.
-- [PgDown] Decreases the cwdaemon sending speed.
-- [CTRL-PgUp] Jump to the next spot above the current VFO cursor in the bamdmap window.
-- [CTRL-PgDown] Jump to the next spot below the current VFO cursor in the bamdmap window.
+- [PgUp] Increases the cw sending speed.
+- [PgDown] Decreases the cw sending speed.
+- [Arrow-Up] Jump to the next spot above the current VFO cursor in the bandmap window.
+- [Arrow-Down] Jump to the next spot below the current VFO cursor in the bandmap window.
 - [TAB] Move cursor to the right one field.
 - [Shift-Tab] Move cursor left One field.
 - [SPACE] When in the callsign field, will move the input to the first field needed for the exchange.
 - [Enter] Submits the fields to the log.
 - [F1-F12] Send (CW or Voice) macros.
+- [CTRL-S] Spot Callsign to the cluster.
+- [CTRL-G] Tune to a spot matching partial text in the callsign entry field.
 
 ### Log Display
 
 `Window`>`Log Window`
 
 The Log display gets updated automatically when a contact is entered. The top half is a list of all contacts.
 
@@ -405,28 +510,28 @@
 
 You can also Right-Click on a cell to bring up the edit dialog.
 
 ![right click edit dialog](https://github.com/mbridak/not1mm/raw/master/pic/edit_dialog.png)
 
 You can not directly edit the multiplier status of a contact. Instead see the next section on recalculating mults. If you change the callsign make sure the `WPX` field is still valid.
 
+## Recalulate Mults
+
+After editing a contact and before generating a Cabrillo file. There is a Misc menu option that will recalculate the multipliers incase an edit had caused a change.
+
 ### Bandmap
 
 `Window`>`Bandmap`
 
 Put your callsign in the top and press the connect button.
 
 The bandmap window is, as with everything, a work in progress. The bandmap now follows the VFO. VFO indicator now displays as small triangle in the frequency tickmarks. A small blue rectangle shows the receivers bandwidth. Clicked on spots now tune the radio and set the callsign field.
 
 ![Bandmap Window](https://github.com/mbridak/not1mm/raw/master/pic/bandmap.png)
 
-## Recalulate Mults
-
-After editing a contact and before generating a Cabrillo file. There is a Misc menu option that will recalculate the multipliers incase an edit had caused a change.
-
 ## Cabrillo
 
 Click on `File` > `Generate Cabrillo`
 
 The file will be placed in your home directory. The name will be in the format of:
 
 `StationCall`_`ContestName`.log
```

### Comparing `not1mm-23.5.9.2/not1mm/__main__.py` & `not1mm-23.6.2/not1mm/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,5003 +4,5611 @@
 00000030: 796c 696e 743a 2064 6973 6162 6c65 3d75  ylint: disable=u
 00000040: 6e75 7365 642d 696d 706f 7274 2c20 632d  nused-import, c-
 00000050: 6578 7465 6e73 696f 6e2d 6e6f 2d6d 656d  extension-no-mem
 00000060: 6265 722c 206e 6f2d 6d65 6d62 6572 2c20  ber, no-member, 
 00000070: 696e 7661 6c69 642d 6e61 6d65 2c20 746f  invalid-name, to
 00000080: 6f2d 6d61 6e79 2d6c 696e 6573 2c20 6e6f  o-many-lines, no
 00000090: 2d6e 616d 652d 696e 2d6d 6f64 756c 650a  -name-in-module.
-000000a0: 0a69 6d70 6f72 7420 696d 706f 7274 6c69  .import importli
-000000b0: 620a 696d 706f 7274 206c 6f67 6769 6e67  b.import logging
-000000c0: 0a69 6d70 6f72 7420 6f73 0a69 6d70 6f72  .import os.impor
-000000d0: 7420 706b 6775 7469 6c0a 696d 706f 7274  t pkgutil.import
-000000e0: 2070 6c61 7466 6f72 6d0a 696d 706f 7274   platform.import
-000000f0: 2071 7565 7565 0a69 6d70 6f72 7420 7265   queue.import re
-00000100: 0a69 6d70 6f72 7420 736f 636b 6574 0a69  .import socket.i
-00000110: 6d70 6f72 7420 7375 6270 726f 6365 7373  mport subprocess
-00000120: 0a69 6d70 6f72 7420 7379 730a 696d 706f  .import sys.impo
-00000130: 7274 2074 6872 6561 6469 6e67 0a69 6d70  rt threading.imp
-00000140: 6f72 7420 7469 6d65 0a69 6d70 6f72 7420  ort time.import 
-00000150: 7575 6964 0a0a 6672 6f6d 2064 6174 6574  uuid..from datet
-00000160: 696d 6520 696d 706f 7274 2064 6174 6574  ime import datet
-00000170: 696d 650a 6672 6f6d 206a 736f 6e20 696d  ime.from json im
-00000180: 706f 7274 2064 756d 7073 2c20 6c6f 6164  port dumps, load
-00000190: 732c 204a 534f 4e44 6563 6f64 6545 7272  s, JSONDecodeErr
-000001a0: 6f72 0a66 726f 6d20 7061 7468 6c69 6220  or.from pathlib 
-000001b0: 696d 706f 7274 2050 6174 680a 6672 6f6d  import Path.from
-000001c0: 2073 6875 7469 6c20 696d 706f 7274 2063   shutil import c
-000001d0: 6f70 7966 696c 650a 6672 6f6d 2078 6d6c  opyfile.from xml
-000001e0: 7270 632e 636c 6965 6e74 2069 6d70 6f72  rpc.client impor
-000001f0: 7420 4572 726f 722c 2053 6572 7665 7250  t Error, ServerP
-00000200: 726f 7879 0a0a 696d 706f 7274 2070 7375  roxy..import psu
-00000210: 7469 6c0a 6672 6f6d 2050 7951 7435 2069  til.from PyQt5 i
-00000220: 6d70 6f72 7420 5174 436f 7265 2c20 5174  mport QtCore, Qt
-00000230: 4775 692c 2051 7457 6964 6765 7473 2c20  Gui, QtWidgets, 
-00000240: 7569 630a 6672 6f6d 2050 7951 7435 2e51  uic.from PyQt5.Q
-00000250: 7457 6964 6765 7473 2069 6d70 6f72 7420  tWidgets import 
-00000260: 5146 696c 6544 6961 6c6f 670a 6672 6f6d  QFileDialog.from
-00000270: 2050 7951 7435 2e51 7443 6f72 6520 696d   PyQt5.QtCore im
-00000280: 706f 7274 2051 506f 696e 7420 2023 2070  port QPoint  # p
-00000290: 796c 696e 743a 2064 6973 6162 6c65 3d6e  ylint: disable=n
-000002a0: 6f2d 6e61 6d65 2d69 6e2d 6d6f 6475 6c65  o-name-in-module
-000002b0: 0a66 726f 6d20 5079 5174 352e 5174 436f  .from PyQt5.QtCo
-000002c0: 7265 2069 6d70 6f72 7420 5144 6972 2c20  re import QDir, 
-000002d0: 5152 6563 742c 2051 5369 7a65 2c20 5174  QRect, QSize, Qt
-000002e0: 0a66 726f 6d20 5079 5174 352e 5174 4775  .from PyQt5.QtGu
-000002f0: 6920 696d 706f 7274 2051 466f 6e74 4461  i import QFontDa
-00000300: 7461 6261 7365 2020 2320 7079 6c69 6e74  tabase  # pylint
-00000310: 3a20 6469 7361 626c 653d 6e6f 2d6e 616d  : disable=no-nam
-00000320: 652d 696e 2d6d 6f64 756c 650a 696d 706f  e-in-module.impo
-00000330: 7274 2073 6f75 6e64 6465 7669 6365 2061  rt sounddevice a
-00000340: 7320 7364 0a69 6d70 6f72 7420 736f 756e  s sd.import soun
-00000350: 6466 696c 6520 6173 2073 660a 0a66 726f  dfile as sf..fro
-00000360: 6d20 6e6f 7431 6d6d 2e6c 6962 2e61 626f  m not1mm.lib.abo
-00000370: 7574 2069 6d70 6f72 7420 4162 6f75 740a  ut import About.
-00000380: 6672 6f6d 206e 6f74 316d 6d2e 6c69 622e  from not1mm.lib.
-00000390: 6361 745f 696e 7465 7266 6163 6520 696d  cat_interface im
-000003a0: 706f 7274 2043 4154 0a66 726f 6d20 6e6f  port CAT.from no
-000003b0: 7431 6d6d 2e6c 6962 2e63 7769 6e74 6572  t1mm.lib.cwinter
-000003c0: 6661 6365 2069 6d70 6f72 7420 4357 0a66  face import CW.f
-000003d0: 726f 6d20 6e6f 7431 6d6d 2e6c 6962 2e64  rom not1mm.lib.d
-000003e0: 6174 6162 6173 6520 696d 706f 7274 2044  atabase import D
-000003f0: 6174 6142 6173 650a 6672 6f6d 206e 6f74  ataBase.from not
-00000400: 316d 6d2e 6c69 622e 6564 6974 5f6d 6163  1mm.lib.edit_mac
-00000410: 726f 2069 6d70 6f72 7420 4564 6974 4d61  ro import EditMa
-00000420: 6372 6f0a 6672 6f6d 206e 6f74 316d 6d2e  cro.from not1mm.
-00000430: 6c69 622e 6564 6974 5f6f 706f 6e20 696d  lib.edit_opon im
-00000440: 706f 7274 204f 704f 6e0a 6672 6f6d 206e  port OpOn.from n
-00000450: 6f74 316d 6d2e 6c69 622e 6564 6974 5f73  ot1mm.lib.edit_s
-00000460: 7461 7469 6f6e 2069 6d70 6f72 7420 4564  tation import Ed
-00000470: 6974 5374 6174 696f 6e0a 6672 6f6d 206e  itStation.from n
-00000480: 6f74 316d 6d2e 6c69 622e 7365 6c65 6374  ot1mm.lib.select
-00000490: 5f63 6f6e 7465 7374 2069 6d70 6f72 7420  _contest import 
-000004a0: 5365 6c65 6374 436f 6e74 6573 740a 6672  SelectContest.fr
-000004b0: 6f6d 206e 6f74 316d 6d2e 6c69 622e 7365  om not1mm.lib.se
-000004c0: 7474 696e 6773 2069 6d70 6f72 7420 5365  ttings import Se
-000004d0: 7474 696e 6773 0a66 726f 6d20 6e6f 7431  ttings.from not1
-000004e0: 6d6d 2e6c 6962 2e68 616d 5f75 7469 6c69  mm.lib.ham_utili
-000004f0: 7479 2069 6d70 6f72 7420 280a 2020 2020  ty import (.    
-00000500: 6265 6172 696e 672c 0a20 2020 2062 6561  bearing,.    bea
-00000510: 7269 6e67 5f77 6974 685f 6c61 746c 6f6e  ring_with_latlon
-00000520: 2c0a 2020 2020 6361 6c63 756c 6174 655f  ,.    calculate_
-00000530: 7770 785f 7072 6566 6978 2c0a 2020 2020  wpx_prefix,.    
-00000540: 6469 7374 616e 6365 2c0a 2020 2020 6469  distance,.    di
-00000550: 7374 616e 6365 5f77 6974 685f 6c61 746c  stance_with_latl
-00000560: 6f6e 2c0a 2020 2020 6765 745f 6c6f 6767  on,.    get_logg
-00000570: 6564 5f62 616e 642c 0a20 2020 2067 6574  ed_band,.    get
-00000580: 6261 6e64 2c0a 2020 2020 7265 6369 7072  band,.    recipr
-00000590: 6f63 6f6c 2c0a 290a 6672 6f6d 206e 6f74  ocol,.).from not
-000005a0: 316d 6d2e 6c69 622e 6c6f 6f6b 7570 2069  1mm.lib.lookup i
-000005b0: 6d70 6f72 7420 5152 5a6c 6f6f 6b75 702c  mport QRZlookup,
-000005c0: 2048 616d 4442 6c6f 6f6b 7570 2c20 4861   HamDBlookup, Ha
-000005d0: 6d51 5448 0a66 726f 6d20 6e6f 7431 6d6d  mQTH.from not1mm
-000005e0: 2e6c 6962 2e6d 756c 7469 6361 7374 2069  .lib.multicast i
-000005f0: 6d70 6f72 7420 4d75 6c74 6963 6173 740a  mport Multicast.
-00000600: 6672 6f6d 206e 6f74 316d 6d2e 6c69 622e  from not1mm.lib.
-00000610: 6e65 775f 636f 6e74 6573 7420 696d 706f  new_contest impo
-00000620: 7274 204e 6577 436f 6e74 6573 740a 6672  rt NewContest.fr
-00000630: 6f6d 206e 6f74 316d 6d2e 6c69 622e 6e31  om not1mm.lib.n1
-00000640: 6d6d 2069 6d70 6f72 7420 4e31 4d4d 0a66  mm import N1MM.f
-00000650: 726f 6d20 6e6f 7431 6d6d 2e6c 6962 2e76  rom not1mm.lib.v
-00000660: 6572 7369 6f6e 2069 6d70 6f72 7420 5f5f  ersion import __
-00000670: 7665 7273 696f 6e5f 5f0a 0a6f 732e 656e  version__..os.en
-00000680: 7669 726f 6e5b 2251 545f 5150 415f 504c  viron["QT_QPA_PL
-00000690: 4154 464f 524d 5448 454d 4522 5d20 3d20  ATFORMTHEME"] = 
-000006a0: 2267 6e6f 6d65 220a 2320 6f73 2e65 6e76  "gnome".# os.env
-000006b0: 6972 6f6e 5b22 5154 5f53 5459 4c45 5f4f  iron["QT_STYLE_O
-000006c0: 5645 5252 4944 4522 5d20 3d20 2261 6477  VERRIDE"] = "adw
-000006d0: 6169 7461 220a 0a6c 6f61 6465 7220 3d20  aita"..loader = 
-000006e0: 706b 6775 7469 6c2e 6765 745f 6c6f 6164  pkgutil.get_load
-000006f0: 6572 2822 6e6f 7431 6d6d 2229 0a57 4f52  er("not1mm").WOR
-00000700: 4b49 4e47 5f50 4154 4820 3d20 6f73 2e70  KING_PATH = os.p
-00000710: 6174 682e 6469 726e 616d 6528 6c6f 6164  ath.dirname(load
-00000720: 6572 2e67 6574 5f66 696c 656e 616d 6528  er.get_filename(
-00000730: 2929 0a0a 6966 2022 5844 475f 4441 5441  ))..if "XDG_DATA
-00000740: 5f48 4f4d 4522 2069 6e20 6f73 2e65 6e76  _HOME" in os.env
-00000750: 6972 6f6e 3a0a 2020 2020 4441 5441 5f50  iron:.    DATA_P
-00000760: 4154 4820 3d20 6f73 2e65 6e76 6972 6f6e  ATH = os.environ
-00000770: 2e67 6574 2822 5844 475f 4441 5441 5f48  .get("XDG_DATA_H
-00000780: 4f4d 4522 290a 656c 7365 3a0a 2020 2020  OME").else:.    
-00000790: 4441 5441 5f50 4154 4820 3d20 7374 7228  DATA_PATH = str(
-000007a0: 5061 7468 2e68 6f6d 6528 2920 2f20 222e  Path.home() / ".
-000007b0: 6c6f 6361 6c22 202f 2022 7368 6172 6522  local" / "share"
-000007c0: 290a 4441 5441 5f50 4154 4820 2b3d 2022  ).DATA_PATH += "
-000007d0: 2f6e 6f74 316d 6d22 0a74 7279 3a0a 2020  /not1mm".try:.  
-000007e0: 2020 6f73 2e6d 6b64 6972 2844 4154 415f    os.mkdir(DATA_
-000007f0: 5041 5448 290a 6578 6365 7074 2046 696c  PATH).except Fil
-00000800: 6545 7869 7374 7345 7272 6f72 3a0a 2020  eExistsError:.  
-00000810: 2020 2e2e 2e0a 0a69 6620 2258 4447 5f43    .....if "XDG_C
-00000820: 4f4e 4649 475f 484f 4d45 2220 696e 206f  ONFIG_HOME" in o
-00000830: 732e 656e 7669 726f 6e3a 0a20 2020 2043  s.environ:.    C
-00000840: 4f4e 4649 475f 5041 5448 203d 206f 732e  ONFIG_PATH = os.
-00000850: 656e 7669 726f 6e2e 6765 7428 2258 4447  environ.get("XDG
-00000860: 5f43 4f4e 4649 475f 484f 4d45 2229 0a65  _CONFIG_HOME").e
-00000870: 6c73 653a 0a20 2020 2043 4f4e 4649 475f  lse:.    CONFIG_
-00000880: 5041 5448 203d 2073 7472 2850 6174 682e  PATH = str(Path.
-00000890: 686f 6d65 2829 202f 2022 2e63 6f6e 6669  home() / ".confi
-000008a0: 6722 290a 434f 4e46 4947 5f50 4154 4820  g").CONFIG_PATH 
-000008b0: 2b3d 2022 2f6e 6f74 316d 6d22 0a74 7279  += "/not1mm".try
-000008c0: 3a0a 2020 2020 6f73 2e6d 6b64 6972 2843  :.    os.mkdir(C
-000008d0: 4f4e 4649 475f 5041 5448 290a 6578 6365  ONFIG_PATH).exce
-000008e0: 7074 2046 696c 6545 7869 7374 7345 7272  pt FileExistsErr
-000008f0: 6f72 3a0a 2020 2020 2e2e 2e0a 0a43 5459  or:.    .....CTY
-00000900: 4649 4c45 203d 207b 7d0a 0a77 6974 6820  FILE = {}..with 
-00000910: 6f70 656e 2857 4f52 4b49 4e47 5f50 4154  open(WORKING_PAT
-00000920: 4820 2b20 222f 6461 7461 2f63 7479 2e6a  H + "/data/cty.j
-00000930: 736f 6e22 2c20 2272 7422 2c20 656e 636f  son", "rt", enco
-00000940: 6469 6e67 3d22 7574 662d 3822 2920 6173  ding="utf-8") as
-00000950: 2063 5f66 696c 653a 0a20 2020 2043 5459   c_file:.    CTY
-00000960: 4649 4c45 203d 206c 6f61 6473 2863 5f66  FILE = loads(c_f
-00000970: 696c 652e 7265 6164 2829 290a 0a44 4152  ile.read())..DAR
-00000980: 4b5f 5354 594c 4553 4845 4554 203d 2022  K_STYLESHEET = "
-00000990: 220a 0a77 6974 6820 6f70 656e 2857 4f52  "..with open(WOR
-000009a0: 4b49 4e47 5f50 4154 4820 2b20 222f 6461  KING_PATH + "/da
-000009b0: 7461 2f43 6f6d 6269 6e65 6172 2e71 7373  ta/Combinear.qss
-000009c0: 222c 2065 6e63 6f64 696e 673d 2275 7466  ", encoding="utf
-000009d0: 2d38 2229 2061 7320 7374 796c 6566 696c  -8") as stylefil
-000009e0: 653a 0a20 2020 2044 4152 4b5f 5354 594c  e:.    DARK_STYL
-000009f0: 4553 4845 4554 203d 2073 7479 6c65 6669  ESHEET = stylefi
-00000a00: 6c65 2e72 6561 6428 290a 0a0a 6465 6620  le.read()...def 
-00000a10: 6368 6563 6b5f 7072 6f63 6573 7328 6e61  check_process(na
-00000a20: 6d65 3a20 7374 7229 202d 3e20 626f 6f6c  me: str) -> bool
-00000a30: 3a0a 2020 2020 2222 2263 6865 636b 7320  :.    """checks 
-00000a40: 746f 2073 6565 2069 6620 7072 6f67 7261  to see if progra
-00000a50: 6d20 6f66 206e 616d 6520 6973 2069 6e20  m of name is in 
-00000a60: 7468 6520 6163 7469 7665 2070 726f 6365  the active proce
-00000a70: 7373 206c 6973 7422 2222 0a20 2020 2066  ss list""".    f
-00000a80: 6f72 2070 726f 6320 696e 2070 7375 7469  or proc in psuti
-00000a90: 6c2e 7072 6f63 6573 735f 6974 6572 2829  l.process_iter()
-00000aa0: 3a0a 2020 2020 2020 2020 6966 206c 656e  :.        if len
-00000ab0: 2870 726f 632e 636d 646c 696e 6528 2929  (proc.cmdline())
-00000ac0: 203d 3d20 323a 0a20 2020 2020 2020 2020   == 2:.         
-00000ad0: 2020 2069 6620 6e61 6d65 2069 6e20 7072     if name in pr
-00000ae0: 6f63 2e63 6d64 6c69 6e65 2829 5b31 5d3a  oc.cmdline()[1]:
-00000af0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000b00: 2072 6574 7572 6e20 5472 7565 0a20 2020   return True.   
-00000b10: 2072 6574 7572 6e20 4661 6c73 650a 0a0a   return False...
-00000b20: 6465 6620 6374 795f 6c6f 6f6b 7570 2863  def cty_lookup(c
-00000b30: 616c 6c73 6967 6e3a 2073 7472 293a 0a20  allsign: str):. 
-00000b40: 2020 2022 2222 4c6f 6f6b 7570 2063 616c     """Lookup cal
-00000b50: 6c73 6967 6e20 696e 2063 7479 2e64 6174  lsign in cty.dat
-00000b60: 2066 696c 6522 2222 0a20 2020 2063 616c   file""".    cal
-00000b70: 6c73 6967 6e20 3d20 6361 6c6c 7369 676e  lsign = callsign
-00000b80: 2e75 7070 6572 2829 0a20 2020 2066 6f72  .upper().    for
-00000b90: 2063 6f75 6e74 2069 6e20 7265 7665 7273   count in revers
-00000ba0: 6564 2872 616e 6765 286c 656e 2863 616c  ed(range(len(cal
-00000bb0: 6c73 6967 6e29 2929 3a0a 2020 2020 2020  lsign))):.      
-00000bc0: 2020 7365 6172 6368 6974 656d 203d 2063    searchitem = c
-00000bd0: 616c 6c73 6967 6e5b 3a20 636f 756e 7420  allsign[: count 
-00000be0: 2b20 315d 0a20 2020 2020 2020 2072 6573  + 1].        res
-00000bf0: 756c 7420 3d20 7b6b 6579 3a20 7661 6c20  ult = {key: val 
-00000c00: 666f 7220 6b65 792c 2076 616c 2069 6e20  for key, val in 
-00000c10: 4354 5946 494c 452e 6974 656d 7328 2920  CTYFILE.items() 
-00000c20: 6966 206b 6579 203d 3d20 7365 6172 6368  if key == search
-00000c30: 6974 656d 7d0a 2020 2020 2020 2020 6966  item}.        if
-00000c40: 206e 6f74 2072 6573 756c 743a 0a20 2020   not result:.   
-00000c50: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-00000c60: 650a 2020 2020 2020 2020 6966 2072 6573  e.        if res
-00000c70: 756c 742e 6765 7428 7365 6172 6368 6974  ult.get(searchit
-00000c80: 656d 292e 6765 7428 2265 7861 6374 5f6d  em).get("exact_m
-00000c90: 6174 6368 2229 3a0a 2020 2020 2020 2020  atch"):.        
-00000ca0: 2020 2020 6966 2073 6561 7263 6869 7465      if searchite
-00000cb0: 6d20 3d3d 2063 616c 6c73 6967 6e3a 0a20  m == callsign:. 
-00000cc0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00000cd0: 6574 7572 6e20 7265 7375 6c74 0a20 2020  eturn result.   
-00000ce0: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-00000cf0: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
-00000d00: 2072 6573 756c 740a 0a0a 636c 6173 7320   result...class 
-00000d10: 4d61 696e 5769 6e64 6f77 2851 7457 6964  MainWindow(QtWid
-00000d20: 6765 7473 2e51 4d61 696e 5769 6e64 6f77  gets.QMainWindow
-00000d30: 293a 0a20 2020 2022 2222 0a20 2020 2054  ):.    """.    T
-00000d40: 6865 206d 6169 6e20 7769 6e64 6f77 0a20  he main window. 
-00000d50: 2020 2022 2222 0a0a 2020 2020 7072 6566     """..    pref
-00000d60: 5f72 6566 203d 207b 0a20 2020 2020 2020  _ref = {.       
-00000d70: 2022 736f 756e 6464 6576 6963 6522 3a20   "sounddevice": 
-00000d80: 2264 6566 6175 6c74 222c 0a20 2020 2020  "default",.     
-00000d90: 2020 2022 7573 6571 727a 223a 2046 616c     "useqrz": Fal
-00000da0: 7365 2c0a 2020 2020 2020 2020 226c 6f6f  se,.        "loo
-00000db0: 6b75 7075 7365 726e 616d 6522 3a20 2275  kupusername": "u
-00000dc0: 7365 726e 616d 6522 2c0a 2020 2020 2020  sername",.      
-00000dd0: 2020 226c 6f6f 6b75 7070 6173 7377 6f72    "lookuppasswor
-00000de0: 6422 3a20 2270 6173 7377 6f72 6422 2c0a  d": "password",.
-00000df0: 2020 2020 2020 2020 2272 756e 5f73 7461          "run_sta
-00000e00: 7465 223a 2054 7275 652c 0a20 2020 2020  te": True,.     
-00000e10: 2020 2022 6461 726b 5f6d 6f64 6522 3a20     "dark_mode": 
-00000e20: 4661 6c73 652c 0a20 2020 2020 2020 2022  False,.        "
-00000e30: 636f 6d6d 616e 645f 6275 7474 6f6e 7322  command_buttons"
-00000e40: 3a20 4661 6c73 652c 0a20 2020 2020 2020  : False,.       
-00000e50: 2022 6377 5f6d 6163 726f 7322 3a20 5472   "cw_macros": Tr
-00000e60: 7565 2c0a 2020 2020 2020 2020 2262 616e  ue,.        "ban
-00000e70: 6473 5f6d 6f64 6573 223a 2054 7275 652c  ds_modes": True,
-00000e80: 0a20 2020 2020 2020 2022 7769 6e64 6f77  .        "window
-00000e90: 5f68 6569 6768 7422 3a20 3230 302c 0a20  _height": 200,. 
-00000ea0: 2020 2020 2020 2022 7769 6e64 6f77 5f77         "window_w
-00000eb0: 6964 7468 223a 2036 3030 2c0a 2020 2020  idth": 600,.    
-00000ec0: 2020 2020 2277 696e 646f 775f 7822 3a20      "window_x": 
-00000ed0: 3132 302c 0a20 2020 2020 2020 2022 7769  120,.        "wi
-00000ee0: 6e64 6f77 5f79 223a 2031 3230 2c0a 2020  ndow_y": 120,.  
-00000ef0: 2020 2020 2020 2263 7572 7265 6e74 5f64        "current_d
-00000f00: 6174 6162 6173 6522 3a20 2268 616d 2e64  atabase": "ham.d
-00000f10: 6222 2c0a 2020 2020 2020 2020 2263 6f6e  b",.        "con
-00000f20: 7465 7374 223a 2022 222c 0a20 2020 2020  test": "",.     
-00000f30: 2020 2022 6d75 6c74 6963 6173 745f 6772     "multicast_gr
-00000f40: 6f75 7022 3a20 2232 3234 2e31 2e31 2e31  oup": "224.1.1.1
-00000f50: 222c 0a20 2020 2020 2020 2022 6d75 6c74  ",.        "mult
-00000f60: 6963 6173 745f 706f 7274 223a 2032 3233  icast_port": 223
-00000f70: 392c 0a20 2020 2020 2020 2022 696e 7465  9,.        "inte
-00000f80: 7266 6163 655f 6970 223a 2022 302e 302e  rface_ip": "0.0.
-00000f90: 302e 3022 2c0a 2020 2020 2020 2020 2273  0.0",.        "s
-00000fa0: 656e 645f 6e31 6d6d 5f70 6163 6b65 7473  end_n1mm_packets
-00000fb0: 223a 2046 616c 7365 2c0a 2020 2020 2020  ": False,.      
-00000fc0: 2020 226e 316d 6d5f 7374 6174 696f 6e5f    "n1mm_station_
-00000fd0: 6e61 6d65 223a 2022 3230 4d20 4357 2054  name": "20M CW T
-00000fe0: 656e 7422 2c0a 2020 2020 2020 2020 226e  ent",.        "n
-00000ff0: 316d 6d5f 6f70 6572 6174 6f72 223a 2022  1mm_operator": "
-00001000: 4265 726e 6965 222c 0a20 2020 2020 2020  Bernie",.       
-00001010: 2022 6e31 6d6d 5f69 7022 3a20 2231 3237   "n1mm_ip": "127
-00001020: 2e30 2e30 2e31 222c 0a20 2020 2020 2020  .0.0.1",.       
-00001030: 2022 6e31 6d6d 5f72 6164 696f 706f 7274   "n1mm_radioport
-00001040: 223a 2031 3230 3630 2c0a 2020 2020 2020  ": 12060,.      
-00001050: 2020 226e 316d 6d5f 636f 6e74 6163 7470    "n1mm_contactp
-00001060: 6f72 7422 3a20 3132 3036 312c 0a20 2020  ort": 12061,.   
-00001070: 2020 2020 2022 6e31 6d6d 5f6c 6f6f 6b75       "n1mm_looku
-00001080: 7070 6f72 7422 3a20 3132 3036 302c 0a20  pport": 12060,. 
-00001090: 2020 2020 2020 2022 6e31 6d6d 5f73 636f         "n1mm_sco
-000010a0: 7265 706f 7274 223a 2031 3230 3632 2c0a  report": 12062,.
-000010b0: 2020 2020 2020 2020 2275 7365 6861 6d64          "usehamd
-000010c0: 6222 3a20 4661 6c73 652c 0a20 2020 2020  b": False,.     
-000010d0: 2020 2022 7573 6568 616d 7174 6822 3a20     "usehamqth": 
-000010e0: 4661 6c73 652c 0a20 2020 2020 2020 2022  False,.        "
-000010f0: 636c 6f75 646c 6f67 223a 2046 616c 7365  cloudlog": False
-00001100: 2c0a 2020 2020 2020 2020 2263 6c6f 7564  ,.        "cloud
-00001110: 6c6f 6761 7069 223a 2022 222c 0a20 2020  logapi": "",.   
-00001120: 2020 2020 2022 636c 6f75 646c 6f67 7572       "cloudlogur
-00001130: 6c22 3a20 2222 2c0a 2020 2020 2020 2020  l": "",.        
-00001140: 2243 4154 5f69 7022 3a20 2231 3237 2e30  "CAT_ip": "127.0
-00001150: 2e30 2e31 222c 0a20 2020 2020 2020 2022  .0.1",.        "
-00001160: 7573 6572 6967 6374 6c64 223a 2046 616c  userigctld": Fal
-00001170: 7365 2c0a 2020 2020 2020 2020 2275 7365  se,.        "use
-00001180: 666c 7269 6722 3a20 4661 6c73 652c 0a20  flrig": False,. 
-00001190: 2020 2020 2020 2022 6377 6970 223a 2022         "cwip": "
-000011a0: 3132 372e 302e 302e 3122 2c0a 2020 2020  127.0.0.1",.    
-000011b0: 2020 2020 2263 7770 6f72 7422 3a20 3637      "cwport": 67
-000011c0: 3839 2c0a 2020 2020 2020 2020 2263 7774  89,.        "cwt
-000011d0: 7970 6522 3a20 302c 0a20 2020 2020 2020  ype": 0,.       
-000011e0: 2022 7573 6573 6572 7665 7222 3a20 4661   "useserver": Fa
-000011f0: 6c73 652c 0a20 2020 2020 2020 2022 4341  lse,.        "CA
-00001200: 545f 706f 7274 223a 2034 3533 322c 0a20  T_port": 4532,. 
-00001210: 2020 2020 2020 2022 636c 7573 7465 725f         "cluster_
-00001220: 7365 7276 6572 223a 2022 6478 632e 6e63  server": "dxc.nc
-00001230: 376a 2e63 6f6d 222c 0a20 2020 2020 2020  7j.com",.       
-00001240: 2022 636c 7573 7465 725f 706f 7274 223a   "cluster_port":
-00001250: 2037 3337 332c 0a20 2020 2020 2020 2022   7373,.        "
-00001260: 636c 7573 7465 725f 6669 6c74 6572 223a  cluster_filter":
-00001270: 2022 5365 7420 4458 2046 696c 7465 7220   "Set DX Filter 
-00001280: 5370 6f74 7465 7243 6f6e 743d 4e41 222c  SpotterCont=NA",
-00001290: 0a20 2020 2020 2020 2022 636c 7573 7465  .        "cluste
-000012a0: 725f 6d6f 6465 223a 2022 4f50 454e 222c  r_mode": "OPEN",
-000012b0: 0a20 2020 207d 0a20 2020 2061 7070 7374  .    }.    appst
-000012c0: 6172 7465 6420 3d20 4661 6c73 650a 2020  arted = False.  
-000012d0: 2020 636f 6e74 6163 7420 3d20 7b7d 0a20    contact = {}. 
-000012e0: 2020 2063 6f6e 7465 7374 203d 204e 6f6e     contest = Non
-000012f0: 650a 2020 2020 636f 6e74 6573 745f 7365  e.    contest_se
-00001300: 7474 696e 6773 203d 207b 7d0a 2020 2020  ttings = {}.    
-00001310: 7072 6566 203d 204e 6f6e 650a 2020 2020  pref = None.    
-00001320: 7374 6174 696f 6e20 3d20 7b7d 0a20 2020  station = {}.   
-00001330: 2063 7572 7265 6e74 5f6f 7020 3d20 2222   current_op = ""
-00001340: 0a20 2020 2063 7572 7265 6e74 5f6d 6f64  .    current_mod
-00001350: 6520 3d20 2222 0a20 2020 2063 7572 7265  e = "".    curre
-00001360: 6e74 5f62 616e 6420 3d20 2222 0a20 2020  nt_band = "".   
-00001370: 2063 7720 3d20 4e6f 6e65 0a20 2020 206c   cw = None.    l
-00001380: 6f6f 6b5f 7570 203d 204e 6f6e 650a 2020  ook_up = None.  
-00001390: 2020 7275 6e5f 7374 6174 6520 3d20 4661    run_state = Fa
-000013a0: 6c73 650a 2020 2020 666b 6579 7320 3d20  lse.    fkeys = 
-000013b0: 7b7d 0a20 2020 2061 626f 7574 5f64 6961  {}.    about_dia
-000013c0: 6c6f 6720 3d20 4e6f 6e65 0a20 2020 2071  log = None.    q
-000013d0: 727a 5f64 6961 6c6f 6720 3d20 4e6f 6e65  rz_dialog = None
-000013e0: 0a20 2020 2073 6574 7469 6e67 735f 6469  .    settings_di
-000013f0: 616c 6f67 203d 204e 6f6e 650a 2020 2020  alog = None.    
-00001400: 6564 6974 5f6d 6163 726f 5f64 6961 6c6f  edit_macro_dialo
-00001410: 6720 3d20 4e6f 6e65 0a20 2020 2063 6f6e  g = None.    con
-00001420: 7465 7374 5f64 6961 6c6f 6720 3d20 4e6f  test_dialog = No
-00001430: 6e65 0a20 2020 2063 6f6e 6669 6775 7261  ne.    configura
-00001440: 7469 6f6e 5f64 6961 6c6f 6720 3d20 4e6f  tion_dialog = No
-00001450: 6e65 0a20 2020 206f 706f 6e5f 6469 616c  ne.    opon_dial
-00001460: 6f67 203d 204e 6f6e 650a 2020 2020 6462  og = None.    db
-00001470: 6e61 6d65 203d 2044 4154 415f 5041 5448  name = DATA_PATH
-00001480: 202b 2022 2f68 616d 2e64 6222 0a20 2020   + "/ham.db".   
-00001490: 2072 6164 696f 5f73 7461 7465 203d 207b   radio_state = {
-000014a0: 7d0a 2020 2020 7269 675f 636f 6e74 726f  }.    rig_contro
-000014b0: 6c20 3d20 4e6f 6e65 0a20 2020 2073 6572  l = None.    ser
-000014c0: 7665 725f 7564 7020 3d20 4e6f 6e65 0a20  ver_udp = None. 
-000014d0: 2020 206d 756c 7469 6361 7374 5f67 726f     multicast_gro
-000014e0: 7570 203d 204e 6f6e 650a 2020 2020 6d75  up = None.    mu
-000014f0: 6c74 6963 6173 745f 706f 7274 203d 204e  lticast_port = N
-00001500: 6f6e 650a 2020 2020 696e 7465 7266 6163  one.    interfac
-00001510: 655f 6970 203d 204e 6f6e 650a 2020 2020  e_ip = None.    
-00001520: 7269 675f 636f 6e74 726f 6c20 3d20 4e6f  rig_control = No
-00001530: 6e65 0a0a 2020 2020 6465 6620 5f5f 696e  ne..    def __in
-00001540: 6974 5f5f 2873 656c 662c 202a 6172 6773  it__(self, *args
-00001550: 2c20 2a2a 6b77 6172 6773 293a 0a20 2020  , **kwargs):.   
-00001560: 2020 2020 2073 7570 6572 2829 2e5f 5f69       super().__i
-00001570: 6e69 745f 5f28 2a61 7267 732c 202a 2a6b  nit__(*args, **k
-00001580: 7761 7267 7329 0a20 2020 2020 2020 206c  wargs).        l
-00001590: 6f67 6765 722e 696e 666f 2822 4d61 696e  ogger.info("Main
-000015a0: 5769 6e64 6f77 3a20 5f5f 696e 6974 5f5f  Window: __init__
-000015b0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-000015c0: 5f75 6470 7761 7463 6820 3d20 4e6f 6e65  _udpwatch = None
-000015d0: 0a20 2020 2020 2020 2073 656c 662e 7564  .        self.ud
-000015e0: 705f 6669 666f 203d 2071 7565 7565 2e51  p_fifo = queue.Q
-000015f0: 7565 7565 2829 0a20 2020 2020 2020 2064  ueue().        d
-00001600: 6174 615f 7061 7468 203d 2057 4f52 4b49  ata_path = WORKI
-00001610: 4e47 5f50 4154 4820 2b20 222f 6461 7461  NG_PATH + "/data
-00001620: 2f6d 6169 6e2e 7569 220a 2020 2020 2020  /main.ui".      
-00001630: 2020 7569 632e 6c6f 6164 5569 2864 6174    uic.loadUi(dat
-00001640: 615f 7061 7468 2c20 7365 6c66 290a 2020  a_path, self).  
-00001650: 2020 2020 2020 7365 6c66 2e6c 6566 7464        self.leftd
-00001660: 6f74 2e68 6964 6528 290a 2020 2020 2020  ot.hide().      
-00001670: 2020 7365 6c66 2e72 6967 6874 646f 742e    self.rightdot.
-00001680: 6869 6465 2829 0a20 2020 2020 2020 2073  hide().        s
-00001690: 656c 662e 6e31 6d6d 203d 204e 314d 4d28  elf.n1mm = N1MM(
-000016a0: 290a 2020 2020 2020 2020 7365 6c66 2e6e  ).        self.n
-000016b0: 6578 745f 6669 656c 6420 3d20 7365 6c66  ext_field = self
-000016c0: 2e6f 7468 6572 5f32 0a20 2020 2020 2020  .other_2.       
-000016d0: 2073 656c 662e 6475 7065 5f69 6e64 6963   self.dupe_indic
-000016e0: 6174 6f72 2e68 6964 6528 290a 2020 2020  ator.hide().    
-000016f0: 2020 2020 7365 6c66 2e63 775f 7370 6565      self.cw_spee
-00001700: 642e 7661 6c75 6543 6861 6e67 6564 2e63  d.valueChanged.c
-00001710: 6f6e 6e65 6374 2873 656c 662e 6377 7370  onnect(self.cwsp
-00001720: 6565 645f 7370 696e 626f 785f 6368 616e  eed_spinbox_chan
-00001730: 6765 6429 0a0a 2020 2020 2020 2020 7365  ged)..        se
-00001740: 6c66 2e61 6374 696f 6e43 575f 4d61 6372  lf.actionCW_Macr
-00001750: 6f73 2e74 7269 6767 6572 6564 2e63 6f6e  os.triggered.con
-00001760: 6e65 6374 2873 656c 662e 6377 5f6d 6163  nect(self.cw_mac
-00001770: 726f 735f 7374 6174 655f 6368 616e 6765  ros_state_change
-00001780: 6429 0a20 2020 2020 2020 2073 656c 662e  d).        self.
-00001790: 6163 7469 6f6e 436f 6d6d 616e 645f 4275  actionCommand_Bu
-000017a0: 7474 6f6e 732e 7472 6967 6765 7265 642e  ttons.triggered.
-000017b0: 636f 6e6e 6563 7428 7365 6c66 2e63 6f6d  connect(self.com
-000017c0: 6d61 6e64 5f62 7574 746f 6e73 5f73 7461  mand_buttons_sta
-000017d0: 7465 5f63 6861 6e67 6529 0a20 2020 2020  te_change).     
-000017e0: 2020 2073 656c 662e 6163 7469 6f6e 4461     self.actionDa
-000017f0: 726b 5f4d 6f64 652e 7472 6967 6765 7265  rk_Mode.triggere
-00001800: 642e 636f 6e6e 6563 7428 7365 6c66 2e64  d.connect(self.d
-00001810: 6172 6b5f 6d6f 6465 5f73 7461 7465 5f63  ark_mode_state_c
-00001820: 6861 6e67 6529 0a20 2020 2020 2020 2073  hange).        s
-00001830: 656c 662e 6163 7469 6f6e 4c6f 675f 5769  elf.actionLog_Wi
-00001840: 6e64 6f77 2e74 7269 6767 6572 6564 2e63  ndow.triggered.c
-00001850: 6f6e 6e65 6374 2873 656c 662e 6c61 756e  onnect(self.laun
-00001860: 6368 5f6c 6f67 5f77 696e 646f 7729 0a20  ch_log_window). 
-00001870: 2020 2020 2020 2073 656c 662e 6163 7469         self.acti
-00001880: 6f6e 4261 6e64 6d61 702e 7472 6967 6765  onBandmap.trigge
-00001890: 7265 642e 636f 6e6e 6563 7428 7365 6c66  red.connect(self
-000018a0: 2e6c 6175 6e63 685f 6261 6e64 6d61 705f  .launch_bandmap_
-000018b0: 7769 6e64 6f77 290a 2020 2020 2020 2020  window).        
-000018c0: 7365 6c66 2e61 6374 696f 6e52 6563 616c  self.actionRecal
-000018d0: 6375 6c61 7465 5f4d 756c 7473 2e74 7269  culate_Mults.tri
-000018e0: 6767 6572 6564 2e63 6f6e 6e65 6374 2873  ggered.connect(s
-000018f0: 656c 662e 7265 6361 6c63 756c 6174 655f  elf.recalculate_
-00001900: 6d75 6c74 7329 0a0a 2020 2020 2020 2020  mults)..        
-00001910: 7365 6c66 2e61 6374 696f 6e47 656e 6572  self.actionGener
-00001920: 6174 655f 4361 6272 696c 6c6f 2e74 7269  ate_Cabrillo.tri
-00001930: 6767 6572 6564 2e63 6f6e 6e65 6374 2873  ggered.connect(s
-00001940: 656c 662e 6765 6e65 7261 7465 5f63 6162  elf.generate_cab
-00001950: 7269 6c6c 6f29 0a20 2020 2020 2020 2073  rillo).        s
-00001960: 656c 662e 6163 7469 6f6e 4765 6e65 7261  elf.actionGenera
-00001970: 7465 5f41 4449 462e 7472 6967 6765 7265  te_ADIF.triggere
-00001980: 642e 636f 6e6e 6563 7428 7365 6c66 2e67  d.connect(self.g
-00001990: 656e 6572 6174 655f 6164 6966 290a 0a20  enerate_adif).. 
-000019a0: 2020 2020 2020 2073 656c 662e 6163 7469         self.acti
-000019b0: 6f6e 436f 6e66 6967 7572 6174 696f 6e5f  onConfiguration_
-000019c0: 5365 7474 696e 6773 2e74 7269 6767 6572  Settings.trigger
-000019d0: 6564 2e63 6f6e 6e65 6374 280a 2020 2020  ed.connect(.    
-000019e0: 2020 2020 2020 2020 7365 6c66 2e65 6469          self.edi
-000019f0: 745f 636f 6e66 6967 7572 6174 696f 6e5f  t_configuration_
-00001a00: 7365 7474 696e 6773 0a20 2020 2020 2020  settings.       
-00001a10: 2029 0a20 2020 2020 2020 2073 656c 662e   ).        self.
-00001a20: 6163 7469 6f6e 5374 6174 696f 6e53 6574  actionStationSet
-00001a30: 7469 6e67 732e 7472 6967 6765 7265 642e  tings.triggered.
-00001a40: 636f 6e6e 6563 7428 7365 6c66 2e65 6469  connect(self.edi
-00001a50: 745f 7374 6174 696f 6e5f 7365 7474 696e  t_station_settin
-00001a60: 6773 290a 0a20 2020 2020 2020 2073 656c  gs)..        sel
-00001a70: 662e 6163 7469 6f6e 4e65 775f 436f 6e74  f.actionNew_Cont
-00001a80: 6573 742e 7472 6967 6765 7265 642e 636f  est.triggered.co
-00001a90: 6e6e 6563 7428 7365 6c66 2e6e 6577 5f63  nnect(self.new_c
-00001aa0: 6f6e 7465 7374 5f64 6961 6c6f 6729 0a20  ontest_dialog). 
-00001ab0: 2020 2020 2020 2073 656c 662e 6163 7469         self.acti
-00001ac0: 6f6e 4f70 656e 5f43 6f6e 7465 7374 2e74  onOpen_Contest.t
-00001ad0: 7269 6767 6572 6564 2e63 6f6e 6e65 6374  riggered.connect
-00001ae0: 2873 656c 662e 6f70 656e 5f63 6f6e 7465  (self.open_conte
-00001af0: 7374 290a 2020 2020 2020 2020 7365 6c66  st).        self
-00001b00: 2e61 6374 696f 6e45 6469 745f 4375 7272  .actionEdit_Curr
-00001b10: 656e 745f 436f 6e74 6573 742e 7472 6967  ent_Contest.trig
-00001b20: 6765 7265 642e 636f 6e6e 6563 7428 7365  gered.connect(se
-00001b30: 6c66 2e65 6469 745f 636f 6e74 6573 7429  lf.edit_contest)
-00001b40: 0a0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
-00001b50: 6374 696f 6e4e 6577 5f44 6174 6162 6173  ctionNew_Databas
-00001b60: 652e 7472 6967 6765 7265 642e 636f 6e6e  e.triggered.conn
-00001b70: 6563 7428 7365 6c66 2e6e 6577 5f64 6174  ect(self.new_dat
-00001b80: 6162 6173 6529 0a20 2020 2020 2020 2073  abase).        s
-00001b90: 656c 662e 6163 7469 6f6e 4f70 656e 5f44  elf.actionOpen_D
-00001ba0: 6174 6162 6173 652e 7472 6967 6765 7265  atabase.triggere
-00001bb0: 642e 636f 6e6e 6563 7428 7365 6c66 2e6f  d.connect(self.o
-00001bc0: 7065 6e5f 6461 7461 6261 7365 290a 0a20  pen_database).. 
-00001bd0: 2020 2020 2020 2073 656c 662e 6163 7469         self.acti
-00001be0: 6f6e 4564 6974 5f4d 6163 726f 732e 7472  onEdit_Macros.tr
-00001bf0: 6967 6765 7265 642e 636f 6e6e 6563 7428  iggered.connect(
-00001c00: 7365 6c66 2e65 6469 745f 6377 5f6d 6163  self.edit_cw_mac
-00001c10: 726f 7329 0a0a 2020 2020 2020 2020 7365  ros)..        se
-00001c20: 6c66 2e61 6374 696f 6e41 626f 7574 2e74  lf.actionAbout.t
-00001c30: 7269 6767 6572 6564 2e63 6f6e 6e65 6374  riggered.connect
-00001c40: 2873 656c 662e 7368 6f77 5f61 626f 7574  (self.show_about
-00001c50: 5f64 6961 6c6f 6729 0a0a 2020 2020 2020  _dialog)..      
-00001c60: 2020 7365 6c66 2e72 6164 696f 4275 7474    self.radioButt
-00001c70: 6f6e 5f72 756e 2e63 6c69 636b 6564 2e63  on_run.clicked.c
-00001c80: 6f6e 6e65 6374 2873 656c 662e 7275 6e5f  onnect(self.run_
-00001c90: 7370 5f62 7574 746f 6e73 5f63 6c69 636b  sp_buttons_click
-00001ca0: 6564 290a 2020 2020 2020 2020 7365 6c66  ed).        self
-00001cb0: 2e72 6164 696f 4275 7474 6f6e 5f73 702e  .radioButton_sp.
-00001cc0: 636c 6963 6b65 642e 636f 6e6e 6563 7428  clicked.connect(
-00001cd0: 7365 6c66 2e72 756e 5f73 705f 6275 7474  self.run_sp_butt
-00001ce0: 6f6e 735f 636c 6963 6b65 6429 0a20 2020  ons_clicked).   
-00001cf0: 2020 2020 2073 656c 662e 7363 6f72 652e       self.score.
-00001d00: 7365 7454 6578 7428 2230 2229 0a20 2020  setText("0").   
-00001d10: 2020 2020 2073 656c 662e 6361 6c6c 7369       self.callsi
-00001d20: 676e 2e74 6578 7445 6469 7465 642e 636f  gn.textEdited.co
-00001d30: 6e6e 6563 7428 7365 6c66 2e63 616c 6c73  nnect(self.calls
-00001d40: 6967 6e5f 6368 616e 6765 6429 0a20 2020  ign_changed).   
-00001d50: 2020 2020 2073 656c 662e 6361 6c6c 7369       self.callsi
-00001d60: 676e 2e72 6574 7572 6e50 7265 7373 6564  gn.returnPressed
-00001d70: 2e63 6f6e 6e65 6374 2873 656c 662e 7361  .connect(self.sa
-00001d80: 7665 5f63 6f6e 7461 6374 290a 2020 2020  ve_contact).    
-00001d90: 2020 2020 7365 6c66 2e73 656e 742e 7265      self.sent.re
-00001da0: 7475 726e 5072 6573 7365 642e 636f 6e6e  turnPressed.conn
-00001db0: 6563 7428 7365 6c66 2e73 6176 655f 636f  ect(self.save_co
-00001dc0: 6e74 6163 7429 0a20 2020 2020 2020 2073  ntact).        s
-00001dd0: 656c 662e 7265 6365 6976 652e 7265 7475  elf.receive.retu
-00001de0: 726e 5072 6573 7365 642e 636f 6e6e 6563  rnPressed.connec
-00001df0: 7428 7365 6c66 2e73 6176 655f 636f 6e74  t(self.save_cont
-00001e00: 6163 7429 0a20 2020 2020 2020 2073 656c  act).        sel
-00001e10: 662e 6f74 6865 725f 312e 7265 7475 726e  f.other_1.return
-00001e20: 5072 6573 7365 642e 636f 6e6e 6563 7428  Pressed.connect(
-00001e30: 7365 6c66 2e73 6176 655f 636f 6e74 6163  self.save_contac
-00001e40: 7429 0a20 2020 2020 2020 2073 656c 662e  t).        self.
-00001e50: 6f74 6865 725f 322e 7265 7475 726e 5072  other_2.returnPr
-00001e60: 6573 7365 642e 636f 6e6e 6563 7428 7365  essed.connect(se
-00001e70: 6c66 2e73 6176 655f 636f 6e74 6163 7429  lf.save_contact)
-00001e80: 0a20 2020 2020 2020 2073 656c 662e 6f74  .        self.ot
-00001e90: 6865 725f 322e 7465 7874 4564 6974 6564  her_2.textEdited
-00001ea0: 2e63 6f6e 6e65 6374 2873 656c 662e 6f74  .connect(self.ot
-00001eb0: 6865 725f 325f 6368 616e 6765 6429 0a20  her_2_changed). 
-00001ec0: 2020 2020 2020 2073 656c 662e 7365 6e74         self.sent
-00001ed0: 2e73 6574 5465 7874 2822 3539 2229 0a20  .setText("59"). 
-00001ee0: 2020 2020 2020 2073 656c 662e 7265 6365         self.rece
-00001ef0: 6976 652e 7365 7454 6578 7428 2235 3922  ive.setText("59"
-00001f00: 290a 2020 2020 2020 2020 6963 6f6e 5f70  ).        icon_p
-00001f10: 6174 6820 3d20 574f 524b 494e 475f 5041  ath = WORKING_PA
-00001f20: 5448 202b 2022 2f64 6174 612f 220a 2020  TH + "/data/".  
-00001f30: 2020 2020 2020 7365 6c66 2e67 7265 656e        self.green
-00001f40: 646f 7420 3d20 5174 4775 692e 5150 6978  dot = QtGui.QPix
-00001f50: 6d61 7028 6963 6f6e 5f70 6174 6820 2b20  map(icon_path + 
-00001f60: 2267 7265 656e 646f 742e 706e 6722 290a  "greendot.png").
-00001f70: 2020 2020 2020 2020 7365 6c66 2e72 6564          self.red
-00001f80: 646f 7420 3d20 5174 4775 692e 5150 6978  dot = QtGui.QPix
-00001f90: 6d61 7028 6963 6f6e 5f70 6174 6820 2b20  map(icon_path + 
-00001fa0: 2272 6564 646f 742e 706e 6722 290a 2020  "reddot.png").  
-00001fb0: 2020 2020 2020 7365 6c66 2e6c 6566 7464        self.leftd
-00001fc0: 6f74 2e73 6574 5069 786d 6170 2873 656c  ot.setPixmap(sel
-00001fd0: 662e 6772 6565 6e64 6f74 290a 2020 2020  f.greendot).    
-00001fe0: 2020 2020 7365 6c66 2e72 6967 6874 646f      self.rightdo
-00001ff0: 742e 7365 7450 6978 6d61 7028 7365 6c66  t.setPixmap(self
-00002000: 2e72 6564 646f 7429 0a0a 2020 2020 2020  .reddot)..      
-00002010: 2020 7365 6c66 2e46 312e 7365 7443 6f6e    self.F1.setCon
-00002020: 7465 7874 4d65 6e75 506f 6c69 6379 2851  textMenuPolicy(Q
-00002030: 7443 6f72 652e 5174 2e43 7573 746f 6d43  tCore.Qt.CustomC
-00002040: 6f6e 7465 7874 4d65 6e75 290a 2020 2020  ontextMenu).    
-00002050: 2020 2020 7365 6c66 2e46 312e 6375 7374      self.F1.cust
-00002060: 6f6d 436f 6e74 6578 744d 656e 7552 6571  omContextMenuReq
-00002070: 7565 7374 6564 2e63 6f6e 6e65 6374 2873  uested.connect(s
-00002080: 656c 662e 6564 6974 5f46 3129 0a20 2020  elf.edit_F1).   
-00002090: 2020 2020 2073 656c 662e 4631 2e63 6c69       self.F1.cli
-000020a0: 636b 6564 2e63 6f6e 6e65 6374 2873 656c  cked.connect(sel
-000020b0: 662e 7365 6e64 6631 290a 2020 2020 2020  f.sendf1).      
-000020c0: 2020 7365 6c66 2e46 322e 7365 7443 6f6e    self.F2.setCon
-000020d0: 7465 7874 4d65 6e75 506f 6c69 6379 2851  textMenuPolicy(Q
-000020e0: 7443 6f72 652e 5174 2e43 7573 746f 6d43  tCore.Qt.CustomC
-000020f0: 6f6e 7465 7874 4d65 6e75 290a 2020 2020  ontextMenu).    
-00002100: 2020 2020 7365 6c66 2e46 322e 6375 7374      self.F2.cust
-00002110: 6f6d 436f 6e74 6578 744d 656e 7552 6571  omContextMenuReq
-00002120: 7565 7374 6564 2e63 6f6e 6e65 6374 2873  uested.connect(s
-00002130: 656c 662e 6564 6974 5f46 3229 0a20 2020  elf.edit_F2).   
-00002140: 2020 2020 2073 656c 662e 4632 2e63 6c69       self.F2.cli
-00002150: 636b 6564 2e63 6f6e 6e65 6374 2873 656c  cked.connect(sel
-00002160: 662e 7365 6e64 6632 290a 2020 2020 2020  f.sendf2).      
-00002170: 2020 7365 6c66 2e46 332e 7365 7443 6f6e    self.F3.setCon
-00002180: 7465 7874 4d65 6e75 506f 6c69 6379 2851  textMenuPolicy(Q
-00002190: 7443 6f72 652e 5174 2e43 7573 746f 6d43  tCore.Qt.CustomC
-000021a0: 6f6e 7465 7874 4d65 6e75 290a 2020 2020  ontextMenu).    
-000021b0: 2020 2020 7365 6c66 2e46 332e 6375 7374      self.F3.cust
-000021c0: 6f6d 436f 6e74 6578 744d 656e 7552 6571  omContextMenuReq
-000021d0: 7565 7374 6564 2e63 6f6e 6e65 6374 2873  uested.connect(s
-000021e0: 656c 662e 6564 6974 5f46 3329 0a20 2020  elf.edit_F3).   
-000021f0: 2020 2020 2073 656c 662e 4633 2e63 6c69       self.F3.cli
-00002200: 636b 6564 2e63 6f6e 6e65 6374 2873 656c  cked.connect(sel
-00002210: 662e 7365 6e64 6633 290a 2020 2020 2020  f.sendf3).      
-00002220: 2020 7365 6c66 2e46 342e 7365 7443 6f6e    self.F4.setCon
-00002230: 7465 7874 4d65 6e75 506f 6c69 6379 2851  textMenuPolicy(Q
-00002240: 7443 6f72 652e 5174 2e43 7573 746f 6d43  tCore.Qt.CustomC
-00002250: 6f6e 7465 7874 4d65 6e75 290a 2020 2020  ontextMenu).    
-00002260: 2020 2020 7365 6c66 2e46 342e 6375 7374      self.F4.cust
-00002270: 6f6d 436f 6e74 6578 744d 656e 7552 6571  omContextMenuReq
-00002280: 7565 7374 6564 2e63 6f6e 6e65 6374 2873  uested.connect(s
-00002290: 656c 662e 6564 6974 5f46 3429 0a20 2020  elf.edit_F4).   
-000022a0: 2020 2020 2073 656c 662e 4634 2e63 6c69       self.F4.cli
-000022b0: 636b 6564 2e63 6f6e 6e65 6374 2873 656c  cked.connect(sel
-000022c0: 662e 7365 6e64 6634 290a 2020 2020 2020  f.sendf4).      
-000022d0: 2020 7365 6c66 2e46 352e 7365 7443 6f6e    self.F5.setCon
-000022e0: 7465 7874 4d65 6e75 506f 6c69 6379 2851  textMenuPolicy(Q
-000022f0: 7443 6f72 652e 5174 2e43 7573 746f 6d43  tCore.Qt.CustomC
-00002300: 6f6e 7465 7874 4d65 6e75 290a 2020 2020  ontextMenu).    
-00002310: 2020 2020 7365 6c66 2e46 352e 6375 7374      self.F5.cust
-00002320: 6f6d 436f 6e74 6578 744d 656e 7552 6571  omContextMenuReq
-00002330: 7565 7374 6564 2e63 6f6e 6e65 6374 2873  uested.connect(s
-00002340: 656c 662e 6564 6974 5f46 3529 0a20 2020  elf.edit_F5).   
-00002350: 2020 2020 2073 656c 662e 4635 2e63 6c69       self.F5.cli
-00002360: 636b 6564 2e63 6f6e 6e65 6374 2873 656c  cked.connect(sel
-00002370: 662e 7365 6e64 6635 290a 2020 2020 2020  f.sendf5).      
-00002380: 2020 7365 6c66 2e46 362e 7365 7443 6f6e    self.F6.setCon
-00002390: 7465 7874 4d65 6e75 506f 6c69 6379 2851  textMenuPolicy(Q
-000023a0: 7443 6f72 652e 5174 2e43 7573 746f 6d43  tCore.Qt.CustomC
-000023b0: 6f6e 7465 7874 4d65 6e75 290a 2020 2020  ontextMenu).    
-000023c0: 2020 2020 7365 6c66 2e46 362e 6375 7374      self.F6.cust
-000023d0: 6f6d 436f 6e74 6578 744d 656e 7552 6571  omContextMenuReq
-000023e0: 7565 7374 6564 2e63 6f6e 6e65 6374 2873  uested.connect(s
-000023f0: 656c 662e 6564 6974 5f46 3629 0a20 2020  elf.edit_F6).   
-00002400: 2020 2020 2073 656c 662e 4636 2e63 6c69       self.F6.cli
-00002410: 636b 6564 2e63 6f6e 6e65 6374 2873 656c  cked.connect(sel
-00002420: 662e 7365 6e64 6636 290a 2020 2020 2020  f.sendf6).      
-00002430: 2020 7365 6c66 2e46 372e 7365 7443 6f6e    self.F7.setCon
-00002440: 7465 7874 4d65 6e75 506f 6c69 6379 2851  textMenuPolicy(Q
-00002450: 7443 6f72 652e 5174 2e43 7573 746f 6d43  tCore.Qt.CustomC
-00002460: 6f6e 7465 7874 4d65 6e75 290a 2020 2020  ontextMenu).    
-00002470: 2020 2020 7365 6c66 2e46 372e 6375 7374      self.F7.cust
-00002480: 6f6d 436f 6e74 6578 744d 656e 7552 6571  omContextMenuReq
-00002490: 7565 7374 6564 2e63 6f6e 6e65 6374 2873  uested.connect(s
-000024a0: 656c 662e 6564 6974 5f46 3729 0a20 2020  elf.edit_F7).   
-000024b0: 2020 2020 2073 656c 662e 4637 2e63 6c69       self.F7.cli
-000024c0: 636b 6564 2e63 6f6e 6e65 6374 2873 656c  cked.connect(sel
-000024d0: 662e 7365 6e64 6637 290a 2020 2020 2020  f.sendf7).      
-000024e0: 2020 7365 6c66 2e46 382e 7365 7443 6f6e    self.F8.setCon
-000024f0: 7465 7874 4d65 6e75 506f 6c69 6379 2851  textMenuPolicy(Q
-00002500: 7443 6f72 652e 5174 2e43 7573 746f 6d43  tCore.Qt.CustomC
-00002510: 6f6e 7465 7874 4d65 6e75 290a 2020 2020  ontextMenu).    
-00002520: 2020 2020 7365 6c66 2e46 382e 6375 7374      self.F8.cust
-00002530: 6f6d 436f 6e74 6578 744d 656e 7552 6571  omContextMenuReq
-00002540: 7565 7374 6564 2e63 6f6e 6e65 6374 2873  uested.connect(s
-00002550: 656c 662e 6564 6974 5f46 3829 0a20 2020  elf.edit_F8).   
-00002560: 2020 2020 2073 656c 662e 4638 2e63 6c69       self.F8.cli
-00002570: 636b 6564 2e63 6f6e 6e65 6374 2873 656c  cked.connect(sel
-00002580: 662e 7365 6e64 6638 290a 2020 2020 2020  f.sendf8).      
-00002590: 2020 7365 6c66 2e46 392e 7365 7443 6f6e    self.F9.setCon
-000025a0: 7465 7874 4d65 6e75 506f 6c69 6379 2851  textMenuPolicy(Q
-000025b0: 7443 6f72 652e 5174 2e43 7573 746f 6d43  tCore.Qt.CustomC
-000025c0: 6f6e 7465 7874 4d65 6e75 290a 2020 2020  ontextMenu).    
-000025d0: 2020 2020 7365 6c66 2e46 392e 6375 7374      self.F9.cust
-000025e0: 6f6d 436f 6e74 6578 744d 656e 7552 6571  omContextMenuReq
-000025f0: 7565 7374 6564 2e63 6f6e 6e65 6374 2873  uested.connect(s
-00002600: 656c 662e 6564 6974 5f46 3929 0a20 2020  elf.edit_F9).   
-00002610: 2020 2020 2073 656c 662e 4639 2e63 6c69       self.F9.cli
-00002620: 636b 6564 2e63 6f6e 6e65 6374 2873 656c  cked.connect(sel
-00002630: 662e 7365 6e64 6639 290a 2020 2020 2020  f.sendf9).      
-00002640: 2020 7365 6c66 2e46 3130 2e73 6574 436f    self.F10.setCo
-00002650: 6e74 6578 744d 656e 7550 6f6c 6963 7928  ntextMenuPolicy(
-00002660: 5174 436f 7265 2e51 742e 4375 7374 6f6d  QtCore.Qt.Custom
-00002670: 436f 6e74 6578 744d 656e 7529 0a20 2020  ContextMenu).   
-00002680: 2020 2020 2073 656c 662e 4631 302e 6375       self.F10.cu
-00002690: 7374 6f6d 436f 6e74 6578 744d 656e 7552  stomContextMenuR
-000026a0: 6571 7565 7374 6564 2e63 6f6e 6e65 6374  equested.connect
-000026b0: 2873 656c 662e 6564 6974 5f46 3130 290a  (self.edit_F10).
-000026c0: 2020 2020 2020 2020 7365 6c66 2e46 3130          self.F10
-000026d0: 2e63 6c69 636b 6564 2e63 6f6e 6e65 6374  .clicked.connect
-000026e0: 2873 656c 662e 7365 6e64 6631 3029 0a20  (self.sendf10). 
-000026f0: 2020 2020 2020 2073 656c 662e 4631 312e         self.F11.
-00002700: 7365 7443 6f6e 7465 7874 4d65 6e75 506f  setContextMenuPo
-00002710: 6c69 6379 2851 7443 6f72 652e 5174 2e43  licy(QtCore.Qt.C
-00002720: 7573 746f 6d43 6f6e 7465 7874 4d65 6e75  ustomContextMenu
-00002730: 290a 2020 2020 2020 2020 7365 6c66 2e46  ).        self.F
-00002740: 3131 2e63 7573 746f 6d43 6f6e 7465 7874  11.customContext
-00002750: 4d65 6e75 5265 7175 6573 7465 642e 636f  MenuRequested.co
-00002760: 6e6e 6563 7428 7365 6c66 2e65 6469 745f  nnect(self.edit_
-00002770: 4631 3129 0a20 2020 2020 2020 2073 656c  F11).        sel
-00002780: 662e 4631 312e 636c 6963 6b65 642e 636f  f.F11.clicked.co
-00002790: 6e6e 6563 7428 7365 6c66 2e73 656e 6466  nnect(self.sendf
-000027a0: 3131 290a 2020 2020 2020 2020 7365 6c66  11).        self
-000027b0: 2e46 3132 2e73 6574 436f 6e74 6578 744d  .F12.setContextM
-000027c0: 656e 7550 6f6c 6963 7928 5174 436f 7265  enuPolicy(QtCore
-000027d0: 2e51 742e 4375 7374 6f6d 436f 6e74 6578  .Qt.CustomContex
-000027e0: 744d 656e 7529 0a20 2020 2020 2020 2073  tMenu).        s
-000027f0: 656c 662e 4631 322e 6375 7374 6f6d 436f  elf.F12.customCo
-00002800: 6e74 6578 744d 656e 7552 6571 7565 7374  ntextMenuRequest
-00002810: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
-00002820: 6564 6974 5f46 3132 290a 2020 2020 2020  edit_F12).      
-00002830: 2020 7365 6c66 2e46 3132 2e63 6c69 636b    self.F12.click
-00002840: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
-00002850: 7365 6e64 6631 3229 0a0a 2020 2020 2020  sendf12)..      
-00002860: 2020 7365 6c66 2e72 6561 6470 7265 6665    self.readprefe
-00002870: 7265 6e63 6573 2829 0a20 2020 2020 2020  rences().       
-00002880: 2073 656c 662e 6462 6e61 6d65 203d 2044   self.dbname = D
-00002890: 4154 415f 5041 5448 202b 2022 2f22 202b  ATA_PATH + "/" +
-000028a0: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
-000028b0: 6375 7272 656e 745f 6461 7461 6261 7365  current_database
-000028c0: 222c 2022 6861 6d2e 6462 2229 0a20 2020  ", "ham.db").   
-000028d0: 2020 2020 2073 656c 662e 6461 7461 6261       self.databa
-000028e0: 7365 203d 2044 6174 6142 6173 6528 7365  se = DataBase(se
-000028f0: 6c66 2e64 626e 616d 652c 2057 4f52 4b49  lf.dbname, WORKI
-00002900: 4e47 5f50 4154 4829 0a20 2020 2020 2020  NG_PATH).       
-00002910: 2073 656c 662e 7374 6174 696f 6e20 3d20   self.station = 
-00002920: 7365 6c66 2e64 6174 6162 6173 652e 6665  self.database.fe
-00002930: 7463 685f 7374 6174 696f 6e28 290a 2020  tch_station().  
-00002940: 2020 2020 2020 6966 2073 656c 662e 7374        if self.st
-00002950: 6174 696f 6e20 6973 204e 6f6e 653a 0a20  ation is None:. 
-00002960: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00002970: 7374 6174 696f 6e20 3d20 7b7d 0a20 2020  station = {}.   
-00002980: 2020 2020 2020 2020 2073 656c 662e 6564           self.ed
-00002990: 6974 5f73 7461 7469 6f6e 5f73 6574 7469  it_station_setti
-000029a0: 6e67 7328 290a 2020 2020 2020 2020 2020  ngs().          
-000029b0: 2020 7365 6c66 2e73 7461 7469 6f6e 203d    self.station =
-000029c0: 2073 656c 662e 6461 7461 6261 7365 2e66   self.database.f
-000029d0: 6574 6368 5f73 7461 7469 6f6e 2829 0a20  etch_station(). 
-000029e0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-000029f0: 6c66 2e73 7461 7469 6f6e 2069 7320 4e6f  lf.station is No
-00002a00: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00002a10: 2020 2020 7365 6c66 2e73 7461 7469 6f6e      self.station
-00002a20: 203d 207b 7d0a 2020 2020 2020 2020 7365   = {}.        se
-00002a30: 6c66 2e63 6f6e 7461 6374 203d 2073 656c  lf.contact = sel
-00002a40: 662e 6461 7461 6261 7365 2e65 6d70 7479  f.database.empty
-00002a50: 5f63 6f6e 7461 6374 0a20 2020 2020 2020  _contact.       
-00002a60: 2073 656c 662e 6375 7272 656e 745f 6f70   self.current_op
-00002a70: 203d 2073 656c 662e 7374 6174 696f 6e2e   = self.station.
-00002a80: 6765 7428 2243 616c 6c22 2c20 2222 290a  get("Call", "").
-00002a90: 2020 2020 2020 2020 7365 6c66 2e6d 616b          self.mak
-00002aa0: 655f 6f70 5f64 6972 2829 0a20 2020 2020  e_op_dir().     
-00002ab0: 2020 2069 6620 7365 6c66 2e70 7265 662e     if self.pref.
-00002ac0: 6765 7428 2263 6f6e 7465 7374 2229 3a0a  get("contest"):.
-00002ad0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00002ae0: 2e6c 6f61 645f 636f 6e74 6573 7428 290a  .load_contest().
-00002af0: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
-00002b00: 6164 5f63 775f 6d61 6372 6f73 2829 0a20  ad_cw_macros(). 
-00002b10: 2020 2020 2020 2073 656c 662e 636c 6561         self.clea
-00002b20: 7269 6e70 7574 7328 290a 2020 2020 2020  rinputs().      
-00002b30: 2020 2320 7365 6c66 2e6c 6175 6e63 685f    # self.launch_
-00002b40: 6c6f 675f 7769 6e64 6f77 2829 0a0a 2020  log_window()..  
-00002b50: 2020 2020 2020 7365 6c66 2e62 616e 645f        self.band_
-00002b60: 696e 6469 6361 746f 7273 5f63 7720 3d20  indicators_cw = 
-00002b70: 7b0a 2020 2020 2020 2020 2020 2020 2231  {.            "1
-00002b80: 3630 223a 2073 656c 662e 6377 5f62 616e  60": self.cw_ban
-00002b90: 645f 3136 302c 0a20 2020 2020 2020 2020  d_160,.         
-00002ba0: 2020 2022 3830 223a 2073 656c 662e 6377     "80": self.cw
-00002bb0: 5f62 616e 645f 3830 2c0a 2020 2020 2020  _band_80,.      
-00002bc0: 2020 2020 2020 2234 3022 3a20 7365 6c66        "40": self
-00002bd0: 2e63 775f 6261 6e64 5f34 302c 0a20 2020  .cw_band_40,.   
-00002be0: 2020 2020 2020 2020 2022 3230 223a 2073           "20": s
-00002bf0: 656c 662e 6377 5f62 616e 645f 3230 2c0a  elf.cw_band_20,.
-00002c00: 2020 2020 2020 2020 2020 2020 2231 3522              "15"
-00002c10: 3a20 7365 6c66 2e63 775f 6261 6e64 5f31  : self.cw_band_1
-00002c20: 352c 0a20 2020 2020 2020 2020 2020 2022  5,.            "
-00002c30: 3130 223a 2073 656c 662e 6377 5f62 616e  10": self.cw_ban
-00002c40: 645f 3130 2c0a 2020 2020 2020 2020 7d0a  d_10,.        }.
-00002c50: 0a20 2020 2020 2020 2073 656c 662e 6261  .        self.ba
-00002c60: 6e64 5f69 6e64 6963 6174 6f72 735f 7373  nd_indicators_ss
-00002c70: 6220 3d20 7b0a 2020 2020 2020 2020 2020  b = {.          
-00002c80: 2020 2231 3630 223a 2073 656c 662e 7373    "160": self.ss
-00002c90: 625f 6261 6e64 5f31 3630 2c0a 2020 2020  b_band_160,.    
-00002ca0: 2020 2020 2020 2020 2238 3022 3a20 7365          "80": se
-00002cb0: 6c66 2e73 7362 5f62 616e 645f 3830 2c0a  lf.ssb_band_80,.
-00002cc0: 2020 2020 2020 2020 2020 2020 2234 3022              "40"
-00002cd0: 3a20 7365 6c66 2e73 7362 5f62 616e 645f  : self.ssb_band_
-00002ce0: 3430 2c0a 2020 2020 2020 2020 2020 2020  40,.            
-00002cf0: 2232 3022 3a20 7365 6c66 2e73 7362 5f62  "20": self.ssb_b
-00002d00: 616e 645f 3230 2c0a 2020 2020 2020 2020  and_20,.        
-00002d10: 2020 2020 2231 3522 3a20 7365 6c66 2e73      "15": self.s
-00002d20: 7362 5f62 616e 645f 3135 2c0a 2020 2020  sb_band_15,.    
-00002d30: 2020 2020 2020 2020 2231 3022 3a20 7365          "10": se
-00002d40: 6c66 2e73 7362 5f62 616e 645f 3130 2c0a  lf.ssb_band_10,.
-00002d50: 2020 2020 2020 2020 7d0a 0a20 2020 2020          }..     
-00002d60: 2020 2073 656c 662e 6261 6e64 5f69 6e64     self.band_ind
-00002d70: 6963 6174 6f72 735f 7274 7479 203d 207b  icators_rtty = {
-00002d80: 0a20 2020 2020 2020 2020 2020 2022 3136  .            "16
-00002d90: 3022 3a20 7365 6c66 2e72 7474 795f 6261  0": self.rtty_ba
-00002da0: 6e64 5f31 3630 2c0a 2020 2020 2020 2020  nd_160,.        
-00002db0: 2020 2020 2238 3022 3a20 7365 6c66 2e72      "80": self.r
-00002dc0: 7474 795f 6261 6e64 5f38 302c 0a20 2020  tty_band_80,.   
-00002dd0: 2020 2020 2020 2020 2022 3430 223a 2073           "40": s
-00002de0: 656c 662e 7274 7479 5f62 616e 645f 3430  elf.rtty_band_40
-00002df0: 2c0a 2020 2020 2020 2020 2020 2020 2232  ,.            "2
-00002e00: 3022 3a20 7365 6c66 2e72 7474 795f 6261  0": self.rtty_ba
-00002e10: 6e64 5f32 302c 0a20 2020 2020 2020 2020  nd_20,.         
-00002e20: 2020 2022 3135 223a 2073 656c 662e 7274     "15": self.rt
-00002e30: 7479 5f62 616e 645f 3135 2c0a 2020 2020  ty_band_15,.    
-00002e40: 2020 2020 2020 2020 2231 3022 3a20 7365          "10": se
-00002e50: 6c66 2e72 7474 795f 6261 6e64 5f31 302c  lf.rtty_band_10,
-00002e60: 0a20 2020 2020 2020 207d 0a0a 2020 2020  .        }..    
-00002e70: 2020 2020 7365 6c66 2e61 6c6c 5f6d 6f64      self.all_mod
-00002e80: 655f 696e 6469 6361 746f 7273 203d 207b  e_indicators = {
-00002e90: 0a20 2020 2020 2020 2020 2020 2022 4357  .            "CW
-00002ea0: 223a 2073 656c 662e 6261 6e64 5f69 6e64  ": self.band_ind
-00002eb0: 6963 6174 6f72 735f 6377 2c0a 2020 2020  icators_cw,.    
-00002ec0: 2020 2020 2020 2020 2253 5342 223a 2073          "SSB": s
-00002ed0: 656c 662e 6261 6e64 5f69 6e64 6963 6174  elf.band_indicat
-00002ee0: 6f72 735f 7373 622c 0a20 2020 2020 2020  ors_ssb,.       
-00002ef0: 2020 2020 2022 5254 5459 223a 2073 656c       "RTTY": sel
-00002f00: 662e 6261 6e64 5f69 6e64 6963 6174 6f72  f.band_indicator
-00002f10: 735f 7274 7479 2c0a 2020 2020 2020 2020  s_rtty,.        
-00002f20: 7d0a 2020 2020 2020 2020 6966 2073 656c  }.        if sel
-00002f30: 662e 5f75 6470 7761 7463 6820 6973 204e  f._udpwatch is N
-00002f40: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00002f50: 2073 656c 662e 5f75 6470 7761 7463 6820   self._udpwatch 
-00002f60: 3d20 7468 7265 6164 696e 672e 5468 7265  = threading.Thre
-00002f70: 6164 280a 2020 2020 2020 2020 2020 2020  ad(.            
-00002f80: 2020 2020 7461 7267 6574 3d73 656c 662e      target=self.
-00002f90: 7761 7463 685f 7564 702c 0a20 2020 2020  watch_udp,.     
-00002fa0: 2020 2020 2020 2020 2020 2064 6165 6d6f             daemo
-00002fb0: 6e3d 5472 7565 2c0a 2020 2020 2020 2020  n=True,.        
-00002fc0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00002fd0: 2020 7365 6c66 2e5f 7564 7077 6174 6368    self._udpwatch
-00002fe0: 2e73 7461 7274 2829 0a0a 2020 2020 4073  .start()..    @s
-00002ff0: 7461 7469 636d 6574 686f 640a 2020 2020  taticmethod.    
-00003000: 6465 6620 6368 6563 6b5f 7072 6f63 6573  def check_proces
-00003010: 7328 6e61 6d65 3a20 7374 7229 202d 3e20  s(name: str) -> 
-00003020: 626f 6f6c 3a0a 2020 2020 2020 2020 2222  bool:.        ""
-00003030: 2263 6865 636b 7320 746f 2073 6565 2069  "checks to see i
-00003040: 6620 7072 6f67 7261 6d20 6f66 206e 616d  f program of nam
-00003050: 6520 6973 2069 6e20 7468 6520 6163 7469  e is in the acti
-00003060: 7665 2070 726f 6365 7373 206c 6973 7422  ve process list"
-00003070: 2222 0a20 2020 2020 2020 2066 6f72 2070  "".        for p
-00003080: 726f 6320 696e 2070 7375 7469 6c2e 7072  roc in psutil.pr
-00003090: 6f63 6573 735f 6974 6572 2829 3a0a 2020  ocess_iter():.  
-000030a0: 2020 2020 2020 2020 2020 6966 2062 6f6f            if boo
-000030b0: 6c28 7265 2e6d 6174 6368 286e 616d 652c  l(re.match(name,
-000030c0: 2070 726f 632e 6e61 6d65 2829 2e6c 6f77   proc.name().low
-000030d0: 6572 2829 2929 3a0a 2020 2020 2020 2020  er())):.        
-000030e0: 2020 2020 2020 2020 7265 7475 726e 2054          return T
-000030f0: 7275 650a 2020 2020 2020 2020 7265 7475  rue.        retu
-00003100: 726e 2046 616c 7365 0a0a 2020 2020 6465  rn False..    de
-00003110: 6620 7368 6f77 5f6d 6573 7361 6765 5f62  f show_message_b
-00003120: 6f78 2873 656c 662c 206d 6573 7361 6765  ox(self, message
-00003130: 3a20 7374 7229 202d 3e20 4e6f 6e65 3a0a  : str) -> None:.
-00003140: 2020 2020 2020 2020 2222 2264 6f63 2222          """doc""
-00003150: 220a 2020 2020 2020 2020 6d65 7373 6167  ".        messag
-00003160: 655f 626f 7820 3d20 5174 5769 6467 6574  e_box = QtWidget
-00003170: 732e 514d 6573 7361 6765 426f 7828 290a  s.QMessageBox().
-00003180: 2020 2020 2020 2020 6d65 7373 6167 655f          message_
-00003190: 626f 782e 7365 7449 636f 6e28 5174 5769  box.setIcon(QtWi
-000031a0: 6467 6574 732e 514d 6573 7361 6765 426f  dgets.QMessageBo
-000031b0: 782e 496e 666f 726d 6174 696f 6e29 0a20  x.Information). 
-000031c0: 2020 2020 2020 206d 6573 7361 6765 5f62         message_b
-000031d0: 6f78 2e73 6574 5465 7874 286d 6573 7361  ox.setText(messa
-000031e0: 6765 290a 2020 2020 2020 2020 6d65 7373  ge).        mess
-000031f0: 6167 655f 626f 782e 7365 7457 696e 646f  age_box.setWindo
-00003200: 7754 6974 6c65 2822 496e 666f 726d 6174  wTitle("Informat
-00003210: 696f 6e22 290a 2020 2020 2020 2020 6d65  ion").        me
-00003220: 7373 6167 655f 626f 782e 7365 7453 7461  ssage_box.setSta
-00003230: 6e64 6172 6442 7574 746f 6e73 2851 7457  ndardButtons(QtW
-00003240: 6964 6765 7473 2e51 4d65 7373 6167 6542  idgets.QMessageB
-00003250: 6f78 2e4f 6b29 0a20 2020 2020 2020 205f  ox.Ok).        _
-00003260: 203d 206d 6573 7361 6765 5f62 6f78 2e65   = message_box.e
-00003270: 7865 635f 2829 0a0a 2020 2020 6465 6620  xec_()..    def 
-00003280: 7368 6f77 5f61 626f 7574 5f64 6961 6c6f  show_about_dialo
-00003290: 6728 7365 6c66 293a 0a20 2020 2020 2020  g(self):.       
-000032a0: 2022 2222 5368 6f77 2061 626f 7574 2064   """Show about d
-000032b0: 6961 6c6f 6722 2222 0a20 2020 2020 2020  ialog""".       
+000000a0: 0a69 6d70 6f72 7420 6461 7465 7469 6d65  .import datetime
+000000b0: 2061 7320 6474 0a69 6d70 6f72 7420 696d   as dt.import im
+000000c0: 706f 7274 6c69 620a 696d 706f 7274 206c  portlib.import l
+000000d0: 6f67 6769 6e67 0a69 6d70 6f72 7420 6f73  ogging.import os
+000000e0: 0a69 6d70 6f72 7420 706b 6775 7469 6c0a  .import pkgutil.
+000000f0: 696d 706f 7274 2070 6c61 7466 6f72 6d0a  import platform.
+00000100: 696d 706f 7274 2072 650a 696d 706f 7274  import re.import
+00000110: 2073 6f63 6b65 740a 696d 706f 7274 2073   socket.import s
+00000120: 7562 7072 6f63 6573 730a 696d 706f 7274  ubprocess.import
+00000130: 2073 7973 0a69 6d70 6f72 7420 7468 7265   sys.import thre
+00000140: 6164 696e 670a 696d 706f 7274 2074 696d  ading.import tim
+00000150: 650a 696d 706f 7274 2075 7569 640a 6672  e.import uuid.fr
+00000160: 6f6d 2064 6174 6574 696d 6520 696d 706f  om datetime impo
+00000170: 7274 2064 6174 6574 696d 650a 6672 6f6d  rt datetime.from
+00000180: 206a 736f 6e20 696d 706f 7274 204a 534f   json import JSO
+00000190: 4e44 6563 6f64 6545 7272 6f72 2c20 6475  NDecodeError, du
+000001a0: 6d70 732c 206c 6f61 6473 0a66 726f 6d20  mps, loads.from 
+000001b0: 7061 7468 6c69 6220 696d 706f 7274 2050  pathlib import P
+000001c0: 6174 680a 6672 6f6d 2073 6875 7469 6c20  ath.from shutil 
+000001d0: 696d 706f 7274 2063 6f70 7966 696c 650a  import copyfile.
+000001e0: 0a69 6d70 6f72 7420 6e6f 7463 7479 7061  .import notctypa
+000001f0: 7273 6572 0a69 6d70 6f72 7420 7073 7574  rser.import psut
+00000200: 696c 0a69 6d70 6f72 7420 736f 756e 6464  il.import soundd
+00000210: 6576 6963 6520 6173 2073 640a 696d 706f  evice as sd.impo
+00000220: 7274 2073 6f75 6e64 6669 6c65 2061 7320  rt soundfile as 
+00000230: 7366 0a66 726f 6d20 5079 5174 3520 696d  sf.from PyQt5 im
+00000240: 706f 7274 2051 7443 6f72 652c 2051 7447  port QtCore, QtG
+00000250: 7569 2c20 5174 5769 6467 6574 732c 2075  ui, QtWidgets, u
+00000260: 6963 0a66 726f 6d20 5079 5174 352e 5174  ic.from PyQt5.Qt
+00000270: 436f 7265 2069 6d70 6f72 7420 5144 6972  Core import QDir
+00000280: 2c20 5150 6f69 6e74 2c20 5152 6563 742c  , QPoint, QRect,
+00000290: 2051 5369 7a65 2c20 5174 0a66 726f 6d20   QSize, Qt.from 
+000002a0: 5079 5174 352e 5174 4775 6920 696d 706f  PyQt5.QtGui impo
+000002b0: 7274 2051 466f 6e74 4461 7461 6261 7365  rt QFontDatabase
+000002c0: 0a66 726f 6d20 5079 5174 352e 5174 5769  .from PyQt5.QtWi
+000002d0: 6467 6574 7320 696d 706f 7274 2051 4669  dgets import QFi
+000002e0: 6c65 4469 616c 6f67 0a0a 6672 6f6d 206e  leDialog..from n
+000002f0: 6f74 316d 6d2e 6c69 622e 6162 6f75 7420  ot1mm.lib.about 
+00000300: 696d 706f 7274 2041 626f 7574 0a66 726f  import About.fro
+00000310: 6d20 6e6f 7431 6d6d 2e6c 6962 2e63 6174  m not1mm.lib.cat
+00000320: 5f69 6e74 6572 6661 6365 2069 6d70 6f72  _interface impor
+00000330: 7420 4341 540a 6672 6f6d 206e 6f74 316d  t CAT.from not1m
+00000340: 6d2e 6c69 622e 6377 696e 7465 7266 6163  m.lib.cwinterfac
+00000350: 6520 696d 706f 7274 2043 570a 6672 6f6d  e import CW.from
+00000360: 206e 6f74 316d 6d2e 6c69 622e 6461 7461   not1mm.lib.data
+00000370: 6261 7365 2069 6d70 6f72 7420 4461 7461  base import Data
+00000380: 4261 7365 0a66 726f 6d20 6e6f 7431 6d6d  Base.from not1mm
+00000390: 2e6c 6962 2e65 6469 745f 6d61 6372 6f20  .lib.edit_macro 
+000003a0: 696d 706f 7274 2045 6469 744d 6163 726f  import EditMacro
+000003b0: 0a66 726f 6d20 6e6f 7431 6d6d 2e6c 6962  .from not1mm.lib
+000003c0: 2e65 6469 745f 6f70 6f6e 2069 6d70 6f72  .edit_opon impor
+000003d0: 7420 4f70 4f6e 0a66 726f 6d20 6e6f 7431  t OpOn.from not1
+000003e0: 6d6d 2e6c 6962 2e65 6469 745f 7374 6174  mm.lib.edit_stat
+000003f0: 696f 6e20 696d 706f 7274 2045 6469 7453  ion import EditS
+00000400: 7461 7469 6f6e 0a66 726f 6d20 6e6f 7431  tation.from not1
+00000410: 6d6d 2e6c 6962 2e68 616d 5f75 7469 6c69  mm.lib.ham_utili
+00000420: 7479 2069 6d70 6f72 7420 280a 2020 2020  ty import (.    
+00000430: 6265 6172 696e 672c 0a20 2020 2062 6561  bearing,.    bea
+00000440: 7269 6e67 5f77 6974 685f 6c61 746c 6f6e  ring_with_latlon
+00000450: 2c0a 2020 2020 6361 6c63 756c 6174 655f  ,.    calculate_
+00000460: 7770 785f 7072 6566 6978 2c0a 2020 2020  wpx_prefix,.    
+00000470: 6469 7374 616e 6365 2c0a 2020 2020 6469  distance,.    di
+00000480: 7374 616e 6365 5f77 6974 685f 6c61 746c  stance_with_latl
+00000490: 6f6e 2c0a 2020 2020 6765 745f 6c6f 6767  on,.    get_logg
+000004a0: 6564 5f62 616e 642c 0a20 2020 2067 6574  ed_band,.    get
+000004b0: 6261 6e64 2c0a 2020 2020 7265 6369 7072  band,.    recipr
+000004c0: 6f63 6f6c 2c0a 290a 6672 6f6d 206e 6f74  ocol,.).from not
+000004d0: 316d 6d2e 6c69 622e 6c6f 6f6b 7570 2069  1mm.lib.lookup i
+000004e0: 6d70 6f72 7420 4861 6d44 426c 6f6f 6b75  mport HamDBlooku
+000004f0: 702c 2048 616d 5154 482c 2051 525a 6c6f  p, HamQTH, QRZlo
+00000500: 6f6b 7570 0a66 726f 6d20 6e6f 7431 6d6d  okup.from not1mm
+00000510: 2e6c 6962 2e6d 756c 7469 6361 7374 2069  .lib.multicast i
+00000520: 6d70 6f72 7420 4d75 6c74 6963 6173 740a  mport Multicast.
+00000530: 6672 6f6d 206e 6f74 316d 6d2e 6c69 622e  from not1mm.lib.
+00000540: 6e31 6d6d 2069 6d70 6f72 7420 4e31 4d4d  n1mm import N1MM
+00000550: 0a66 726f 6d20 6e6f 7431 6d6d 2e6c 6962  .from not1mm.lib
+00000560: 2e6e 6577 5f63 6f6e 7465 7374 2069 6d70  .new_contest imp
+00000570: 6f72 7420 4e65 7743 6f6e 7465 7374 0a66  ort NewContest.f
+00000580: 726f 6d20 6e6f 7431 6d6d 2e6c 6962 2e73  rom not1mm.lib.s
+00000590: 656c 6563 745f 636f 6e74 6573 7420 696d  elect_contest im
+000005a0: 706f 7274 2053 656c 6563 7443 6f6e 7465  port SelectConte
+000005b0: 7374 0a66 726f 6d20 6e6f 7431 6d6d 2e6c  st.from not1mm.l
+000005c0: 6962 2e73 6574 7469 6e67 7320 696d 706f  ib.settings impo
+000005d0: 7274 2053 6574 7469 6e67 730a 6672 6f6d  rt Settings.from
+000005e0: 206e 6f74 316d 6d2e 6c69 622e 7665 7273   not1mm.lib.vers
+000005f0: 696f 6e20 696d 706f 7274 205f 5f76 6572  ion import __ver
+00000600: 7369 6f6e 5f5f 0a66 726f 6d20 6e6f 7431  sion__.from not1
+00000610: 6d6d 2e6c 6962 2e76 6572 7369 6f6e 7465  mm.lib.versionte
+00000620: 7374 2069 6d70 6f72 7420 5665 7273 696f  st import Versio
+00000630: 6e54 6573 740a 0a23 2066 726f 6d20 786d  nTest..# from xm
+00000640: 6c72 7063 2e63 6c69 656e 7420 696d 706f  lrpc.client impo
+00000650: 7274 2045 7272 6f72 2c20 5365 7276 6572  rt Error, Server
+00000660: 5072 6f78 790a 0a0a 2320 6773 6574 7469  Proxy...# gsetti
+00000670: 6e67 7320 6765 7420 6f72 672e 676e 6f6d  ngs get org.gnom
+00000680: 652e 6465 736b 746f 702e 696e 7465 7266  e.desktop.interf
+00000690: 6163 6520 636f 6c6f 722d 7363 6865 6d65  ace color-scheme
+000006a0: 0a23 206f 732e 656e 7669 726f 6e5b 2251  .# os.environ["Q
+000006b0: 545f 5150 415f 504c 4154 464f 524d 225d  T_QPA_PLATFORM"]
+000006c0: 203d 2022 7761 796c 616e 6422 0a23 2063   = "wayland".# c
+000006d0: 6420 3d20 6f73 2e65 6e76 6972 6f6e 2e67  d = os.environ.g
+000006e0: 6574 2822 5844 475f 4355 5252 454e 545f  et("XDG_CURRENT_
+000006f0: 4445 534b 544f 5022 2c20 4661 6c73 6529  DESKTOP", False)
+00000700: 0a23 2069 6620 2247 4e4f 4d45 2220 696e  .# if "GNOME" in
+00000710: 2063 6420 6f72 2022 556e 6974 7922 2069   cd or "Unity" i
+00000720: 6e20 6364 3a0a 2320 2020 2020 6f73 2e65  n cd:.#     os.e
+00000730: 6e76 6972 6f6e 5b22 5154 5f51 5041 5f50  nviron["QT_QPA_P
+00000740: 4c41 5446 4f52 4d54 4845 4d45 225d 203d  LATFORMTHEME"] =
+00000750: 2022 676e 6f6d 6522 0a23 2020 2020 206f   "gnome".#     o
+00000760: 732e 656e 7669 726f 6e5b 2251 545f 5354  s.environ["QT_ST
+00000770: 594c 455f 4f56 4552 5249 4445 225d 203d  YLE_OVERRIDE"] =
+00000780: 2022 4164 7761 6974 612d 4461 726b 220a   "Adwaita-Dark".
+00000790: 0a6c 6f61 6465 7220 3d20 706b 6775 7469  .loader = pkguti
+000007a0: 6c2e 6765 745f 6c6f 6164 6572 2822 6e6f  l.get_loader("no
+000007b0: 7431 6d6d 2229 0a57 4f52 4b49 4e47 5f50  t1mm").WORKING_P
+000007c0: 4154 4820 3d20 6f73 2e70 6174 682e 6469  ATH = os.path.di
+000007d0: 726e 616d 6528 6c6f 6164 6572 2e67 6574  rname(loader.get
+000007e0: 5f66 696c 656e 616d 6528 2929 0a0a 4441  _filename())..DA
+000007f0: 5441 5f50 4154 4820 3d20 6f73 2e65 6e76  TA_PATH = os.env
+00000800: 6972 6f6e 2e67 6574 2822 5844 475f 4441  iron.get("XDG_DA
+00000810: 5441 5f48 4f4d 4522 2c20 7374 7228 5061  TA_HOME", str(Pa
+00000820: 7468 2e68 6f6d 6528 2920 2f20 222e 6c6f  th.home() / ".lo
+00000830: 6361 6c22 202f 2022 7368 6172 6522 2929  cal" / "share"))
+00000840: 0a44 4154 415f 5041 5448 202b 3d20 222f  .DATA_PATH += "/
+00000850: 6e6f 7431 6d6d 220a 0a74 7279 3a0a 2020  not1mm"..try:.  
+00000860: 2020 6f73 2e6d 6b64 6972 2844 4154 415f    os.mkdir(DATA_
+00000870: 5041 5448 290a 6578 6365 7074 2046 696c  PATH).except Fil
+00000880: 6545 7869 7374 7345 7272 6f72 3a0a 2020  eExistsError:.  
+00000890: 2020 2e2e 2e0a 0a43 4f4e 4649 475f 5041    .....CONFIG_PA
+000008a0: 5448 203d 206f 732e 656e 7669 726f 6e2e  TH = os.environ.
+000008b0: 6765 7428 2258 4447 5f43 4f4e 4649 475f  get("XDG_CONFIG_
+000008c0: 484f 4d45 222c 2073 7472 2850 6174 682e  HOME", str(Path.
+000008d0: 686f 6d65 2829 202f 2022 2e63 6f6e 6669  home() / ".confi
+000008e0: 6722 2929 0a43 4f4e 4649 475f 5041 5448  g")).CONFIG_PATH
+000008f0: 202b 3d20 222f 6e6f 7431 6d6d 220a 0a74   += "/not1mm"..t
+00000900: 7279 3a0a 2020 2020 6f73 2e6d 6b64 6972  ry:.    os.mkdir
+00000910: 2843 4f4e 4649 475f 5041 5448 290a 6578  (CONFIG_PATH).ex
+00000920: 6365 7074 2046 696c 6545 7869 7374 7345  cept FileExistsE
+00000930: 7272 6f72 3a0a 2020 2020 2e2e 2e0a 0a0a  rror:.    ......
+00000940: 4354 5946 494c 4520 3d20 7b7d 0a0a 7769  CTYFILE = {}..wi
+00000950: 7468 206f 7065 6e28 574f 524b 494e 475f  th open(WORKING_
+00000960: 5041 5448 202b 2022 2f64 6174 612f 6374  PATH + "/data/ct
+00000970: 792e 6a73 6f6e 222c 2022 7274 222c 2065  y.json", "rt", e
+00000980: 6e63 6f64 696e 673d 2275 7466 2d38 2229  ncoding="utf-8")
+00000990: 2061 7320 635f 6669 6c65 3a0a 2020 2020   as c_file:.    
+000009a0: 4354 5946 494c 4520 3d20 6c6f 6164 7328  CTYFILE = loads(
+000009b0: 635f 6669 6c65 2e72 6561 6428 2929 0a0a  c_file.read())..
+000009c0: 706f 6c6c 5f74 696d 6520 3d20 6461 7465  poll_time = date
+000009d0: 7469 6d65 2e6e 6f77 2829 0a0a 0a64 6566  time.now()...def
+000009e0: 2063 6865 636b 5f70 726f 6365 7373 286e   check_process(n
+000009f0: 616d 653a 2073 7472 2920 2d3e 2062 6f6f  ame: str) -> boo
+00000a00: 6c3a 0a20 2020 2022 2222 6368 6563 6b73  l:.    """checks
+00000a10: 2074 6f20 7365 6520 6966 2070 726f 6772   to see if progr
+00000a20: 616d 206f 6620 6e61 6d65 2069 7320 696e  am of name is in
+00000a30: 2074 6865 2061 6374 6976 6520 7072 6f63   the active proc
+00000a40: 6573 7320 6c69 7374 2222 220a 2020 2020  ess list""".    
+00000a50: 666f 7220 7072 6f63 2069 6e20 7073 7574  for proc in psut
+00000a60: 696c 2e70 726f 6365 7373 5f69 7465 7228  il.process_iter(
+00000a70: 293a 0a20 2020 2020 2020 2069 6620 6c65  ):.        if le
+00000a80: 6e28 7072 6f63 2e63 6d64 6c69 6e65 2829  n(proc.cmdline()
+00000a90: 2920 3d3d 2032 3a0a 2020 2020 2020 2020  ) == 2:.        
+00000aa0: 2020 2020 6966 206e 616d 6520 696e 2070      if name in p
+00000ab0: 726f 632e 636d 646c 696e 6528 295b 315d  roc.cmdline()[1]
+00000ac0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00000ad0: 2020 7265 7475 726e 2054 7275 650a 2020    return True.  
+00000ae0: 2020 7265 7475 726e 2046 616c 7365 0a0a    return False..
+00000af0: 0a64 6566 2063 7479 5f6c 6f6f 6b75 7028  .def cty_lookup(
+00000b00: 6361 6c6c 7369 676e 3a20 7374 7229 3a0a  callsign: str):.
+00000b10: 2020 2020 2222 224c 6f6f 6b75 7020 6361      """Lookup ca
+00000b20: 6c6c 7369 676e 2069 6e20 6374 792e 6461  llsign in cty.da
+00000b30: 7420 6669 6c65 2222 220a 2020 2020 6361  t file""".    ca
+00000b40: 6c6c 7369 676e 203d 2063 616c 6c73 6967  llsign = callsig
+00000b50: 6e2e 7570 7065 7228 290a 2020 2020 666f  n.upper().    fo
+00000b60: 7220 636f 756e 7420 696e 2072 6576 6572  r count in rever
+00000b70: 7365 6428 7261 6e67 6528 6c65 6e28 6361  sed(range(len(ca
+00000b80: 6c6c 7369 676e 2929 293a 0a20 2020 2020  llsign))):.     
+00000b90: 2020 2073 6561 7263 6869 7465 6d20 3d20     searchitem = 
+00000ba0: 6361 6c6c 7369 676e 5b3a 2063 6f75 6e74  callsign[: count
+00000bb0: 202b 2031 5d0a 2020 2020 2020 2020 7265   + 1].        re
+00000bc0: 7375 6c74 203d 207b 6b65 793a 2076 616c  sult = {key: val
+00000bd0: 2066 6f72 206b 6579 2c20 7661 6c20 696e   for key, val in
+00000be0: 2043 5459 4649 4c45 2e69 7465 6d73 2829   CTYFILE.items()
+00000bf0: 2069 6620 6b65 7920 3d3d 2073 6561 7263   if key == searc
+00000c00: 6869 7465 6d7d 0a20 2020 2020 2020 2069  hitem}.        i
+00000c10: 6620 6e6f 7420 7265 7375 6c74 3a0a 2020  f not result:.  
+00000c20: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
+00000c30: 7565 0a20 2020 2020 2020 2069 6620 7265  ue.        if re
+00000c40: 7375 6c74 2e67 6574 2873 6561 7263 6869  sult.get(searchi
+00000c50: 7465 6d29 2e67 6574 2822 6578 6163 745f  tem).get("exact_
+00000c60: 6d61 7463 6822 293a 0a20 2020 2020 2020  match"):.       
+00000c70: 2020 2020 2069 6620 7365 6172 6368 6974       if searchit
+00000c80: 656d 203d 3d20 6361 6c6c 7369 676e 3a0a  em == callsign:.
+00000c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ca0: 7265 7475 726e 2072 6573 756c 740a 2020  return result.  
+00000cb0: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
+00000cc0: 7565 0a20 2020 2020 2020 2072 6574 7572  ue.        retur
+00000cd0: 6e20 7265 7375 6c74 0a0a 0a63 6c61 7373  n result...class
+00000ce0: 204d 6169 6e57 696e 646f 7728 5174 5769   MainWindow(QtWi
+00000cf0: 6467 6574 732e 514d 6169 6e57 696e 646f  dgets.QMainWindo
+00000d00: 7729 3a0a 2020 2020 2222 220a 2020 2020  w):.    """.    
+00000d10: 5468 6520 6d61 696e 2077 696e 646f 770a  The main window.
+00000d20: 2020 2020 2222 220a 0a20 2020 2070 7265      """..    pre
+00000d30: 665f 7265 6620 3d20 7b0a 2020 2020 2020  f_ref = {.      
+00000d40: 2020 2273 6f75 6e64 6465 7669 6365 223a    "sounddevice":
+00000d50: 2022 6465 6661 756c 7422 2c0a 2020 2020   "default",.    
+00000d60: 2020 2020 2275 7365 7172 7a22 3a20 4661      "useqrz": Fa
+00000d70: 6c73 652c 0a20 2020 2020 2020 2022 6c6f  lse,.        "lo
+00000d80: 6f6b 7570 7573 6572 6e61 6d65 223a 2022  okupusername": "
+00000d90: 7573 6572 6e61 6d65 222c 0a20 2020 2020  username",.     
+00000da0: 2020 2022 6c6f 6f6b 7570 7061 7373 776f     "lookuppasswo
+00000db0: 7264 223a 2022 7061 7373 776f 7264 222c  rd": "password",
+00000dc0: 0a20 2020 2020 2020 2022 7275 6e5f 7374  .        "run_st
+00000dd0: 6174 6522 3a20 5472 7565 2c0a 2020 2020  ate": True,.    
+00000de0: 2020 2020 2263 6f6d 6d61 6e64 5f62 7574      "command_but
+00000df0: 746f 6e73 223a 2046 616c 7365 2c0a 2020  tons": False,.  
+00000e00: 2020 2020 2020 2263 775f 6d61 6372 6f73        "cw_macros
+00000e10: 223a 2054 7275 652c 0a20 2020 2020 2020  ": True,.       
+00000e20: 2022 6261 6e64 735f 6d6f 6465 7322 3a20   "bands_modes": 
+00000e30: 5472 7565 2c0a 2020 2020 2020 2020 2277  True,.        "w
+00000e40: 696e 646f 775f 6865 6967 6874 223a 2032  indow_height": 2
+00000e50: 3030 2c0a 2020 2020 2020 2020 2277 696e  00,.        "win
+00000e60: 646f 775f 7769 6474 6822 3a20 3630 302c  dow_width": 600,
+00000e70: 0a20 2020 2020 2020 2022 7769 6e64 6f77  .        "window
+00000e80: 5f78 223a 2031 3230 2c0a 2020 2020 2020  _x": 120,.      
+00000e90: 2020 2277 696e 646f 775f 7922 3a20 3132    "window_y": 12
+00000ea0: 302c 0a20 2020 2020 2020 2022 6375 7272  0,.        "curr
+00000eb0: 656e 745f 6461 7461 6261 7365 223a 2022  ent_database": "
+00000ec0: 6861 6d2e 6462 222c 0a20 2020 2020 2020  ham.db",.       
+00000ed0: 2022 636f 6e74 6573 7422 3a20 2222 2c0a   "contest": "",.
+00000ee0: 2020 2020 2020 2020 226d 756c 7469 6361          "multica
+00000ef0: 7374 5f67 726f 7570 223a 2022 3233 392e  st_group": "239.
+00000f00: 312e 312e 3122 2c0a 2020 2020 2020 2020  1.1.1",.        
+00000f10: 226d 756c 7469 6361 7374 5f70 6f72 7422  "multicast_port"
+00000f20: 3a20 3232 3339 2c0a 2020 2020 2020 2020  : 2239,.        
+00000f30: 2269 6e74 6572 6661 6365 5f69 7022 3a20  "interface_ip": 
+00000f40: 2230 2e30 2e30 2e30 222c 0a20 2020 2020  "0.0.0.0",.     
+00000f50: 2020 2022 7365 6e64 5f6e 316d 6d5f 7061     "send_n1mm_pa
+00000f60: 636b 6574 7322 3a20 4661 6c73 652c 0a20  ckets": False,. 
+00000f70: 2020 2020 2020 2022 6e31 6d6d 5f73 7461         "n1mm_sta
+00000f80: 7469 6f6e 5f6e 616d 6522 3a20 2232 304d  tion_name": "20M
+00000f90: 2043 5720 5465 6e74 222c 0a20 2020 2020   CW Tent",.     
+00000fa0: 2020 2022 6e31 6d6d 5f6f 7065 7261 746f     "n1mm_operato
+00000fb0: 7222 3a20 2242 6572 6e69 6522 2c0a 2020  r": "Bernie",.  
+00000fc0: 2020 2020 2020 226e 316d 6d5f 7261 6469        "n1mm_radi
+00000fd0: 6f70 6f72 7422 3a20 2231 3237 2e30 2e30  oport": "127.0.0
+00000fe0: 2e31 3a31 3230 3630 222c 0a20 2020 2020  .1:12060",.     
+00000ff0: 2020 2022 6e31 6d6d 5f63 6f6e 7461 6374     "n1mm_contact
+00001000: 706f 7274 223a 2022 3132 372e 302e 302e  port": "127.0.0.
+00001010: 313a 3132 3036 3022 2c0a 2020 2020 2020  1:12060",.      
+00001020: 2020 226e 316d 6d5f 6c6f 6f6b 7570 706f    "n1mm_lookuppo
+00001030: 7274 223a 2022 3132 372e 302e 302e 313a  rt": "127.0.0.1:
+00001040: 3132 3036 3022 2c0a 2020 2020 2020 2020  12060",.        
+00001050: 226e 316d 6d5f 7363 6f72 6570 6f72 7422  "n1mm_scoreport"
+00001060: 3a20 2231 3237 2e30 2e30 2e31 3a31 3230  : "127.0.0.1:120
+00001070: 3630 222c 0a20 2020 2020 2020 2022 7573  60",.        "us
+00001080: 6568 616d 6462 223a 2046 616c 7365 2c0a  ehamdb": False,.
+00001090: 2020 2020 2020 2020 2275 7365 6861 6d71          "usehamq
+000010a0: 7468 223a 2046 616c 7365 2c0a 2020 2020  th": False,.    
+000010b0: 2020 2020 2263 6c6f 7564 6c6f 6722 3a20      "cloudlog": 
+000010c0: 4661 6c73 652c 0a20 2020 2020 2020 2022  False,.        "
+000010d0: 636c 6f75 646c 6f67 6170 6922 3a20 2222  cloudlogapi": ""
+000010e0: 2c0a 2020 2020 2020 2020 2263 6c6f 7564  ,.        "cloud
+000010f0: 6c6f 6775 726c 223a 2022 222c 0a20 2020  logurl": "",.   
+00001100: 2020 2020 2022 4341 545f 6970 223a 2022       "CAT_ip": "
+00001110: 3132 372e 302e 302e 3122 2c0a 2020 2020  127.0.0.1",.    
+00001120: 2020 2020 2275 7365 7269 6763 746c 6422      "userigctld"
+00001130: 3a20 4661 6c73 652c 0a20 2020 2020 2020  : False,.       
+00001140: 2022 7573 6566 6c72 6967 223a 2046 616c   "useflrig": Fal
+00001150: 7365 2c0a 2020 2020 2020 2020 2263 7769  se,.        "cwi
+00001160: 7022 3a20 2231 3237 2e30 2e30 2e31 222c  p": "127.0.0.1",
+00001170: 0a20 2020 2020 2020 2022 6377 706f 7274  .        "cwport
+00001180: 223a 2036 3738 392c 0a20 2020 2020 2020  ": 6789,.       
+00001190: 2022 6377 7479 7065 223a 2030 2c0a 2020   "cwtype": 0,.  
+000011a0: 2020 2020 2020 2275 7365 7365 7276 6572        "useserver
+000011b0: 223a 2046 616c 7365 2c0a 2020 2020 2020  ": False,.      
+000011c0: 2020 2243 4154 5f70 6f72 7422 3a20 3435    "CAT_port": 45
+000011d0: 3332 2c0a 2020 2020 2020 2020 2263 6c75  32,.        "clu
+000011e0: 7374 6572 5f73 6572 7665 7222 3a20 2264  ster_server": "d
+000011f0: 7863 2e6e 6337 6a2e 636f 6d22 2c0a 2020  xc.nc7j.com",.  
+00001200: 2020 2020 2020 2263 6c75 7374 6572 5f70        "cluster_p
+00001210: 6f72 7422 3a20 3733 3733 2c0a 2020 2020  ort": 7373,.    
+00001220: 2020 2020 2263 6c75 7374 6572 5f66 696c      "cluster_fil
+00001230: 7465 7222 3a20 2253 6574 2044 5820 4669  ter": "Set DX Fi
+00001240: 6c74 6572 2053 706f 7474 6572 436f 6e74  lter SpotterCont
+00001250: 3d4e 4122 2c0a 2020 2020 2020 2020 2263  =NA",.        "c
+00001260: 6c75 7374 6572 5f6d 6f64 6522 3a20 224f  luster_mode": "O
+00001270: 5045 4e22 2c0a 2020 2020 7d0a 2020 2020  PEN",.    }.    
+00001280: 6170 7073 7461 7274 6564 203d 2046 616c  appstarted = Fal
+00001290: 7365 0a20 2020 2063 6f6e 7461 6374 203d  se.    contact =
+000012a0: 207b 7d0a 2020 2020 636f 6e74 6573 7420   {}.    contest 
+000012b0: 3d20 4e6f 6e65 0a20 2020 2063 6f6e 7465  = None.    conte
+000012c0: 7374 5f73 6574 7469 6e67 7320 3d20 7b7d  st_settings = {}
+000012d0: 0a20 2020 2070 7265 6620 3d20 4e6f 6e65  .    pref = None
+000012e0: 0a20 2020 2073 7461 7469 6f6e 203d 207b  .    station = {
+000012f0: 7d0a 2020 2020 6375 7272 656e 745f 6f70  }.    current_op
+00001300: 203d 2022 220a 2020 2020 6375 7272 656e   = "".    curren
+00001310: 745f 6d6f 6465 203d 2022 220a 2020 2020  t_mode = "".    
+00001320: 6375 7272 656e 745f 6261 6e64 203d 2022  current_band = "
+00001330: 220a 2020 2020 6377 203d 204e 6f6e 650a  ".    cw = None.
+00001340: 2020 2020 6c6f 6f6b 5f75 7020 3d20 4e6f      look_up = No
+00001350: 6e65 0a20 2020 2072 756e 5f73 7461 7465  ne.    run_state
+00001360: 203d 2046 616c 7365 0a20 2020 2066 6b65   = False.    fke
+00001370: 7973 203d 207b 7d0a 2020 2020 6162 6f75  ys = {}.    abou
+00001380: 745f 6469 616c 6f67 203d 204e 6f6e 650a  t_dialog = None.
+00001390: 2020 2020 7172 7a5f 6469 616c 6f67 203d      qrz_dialog =
+000013a0: 204e 6f6e 650a 2020 2020 7365 7474 696e   None.    settin
+000013b0: 6773 5f64 6961 6c6f 6720 3d20 4e6f 6e65  gs_dialog = None
+000013c0: 0a20 2020 2065 6469 745f 6d61 6372 6f5f  .    edit_macro_
+000013d0: 6469 616c 6f67 203d 204e 6f6e 650a 2020  dialog = None.  
+000013e0: 2020 636f 6e74 6573 745f 6469 616c 6f67    contest_dialog
+000013f0: 203d 204e 6f6e 650a 2020 2020 636f 6e66   = None.    conf
+00001400: 6967 7572 6174 696f 6e5f 6469 616c 6f67  iguration_dialog
+00001410: 203d 204e 6f6e 650a 2020 2020 6f70 6f6e   = None.    opon
+00001420: 5f64 6961 6c6f 6720 3d20 4e6f 6e65 0a20  _dialog = None. 
+00001430: 2020 2064 626e 616d 6520 3d20 4441 5441     dbname = DATA
+00001440: 5f50 4154 4820 2b20 222f 6861 6d2e 6462  _PATH + "/ham.db
+00001450: 220a 2020 2020 7261 6469 6f5f 7374 6174  ".    radio_stat
+00001460: 6520 3d20 7b7d 0a20 2020 2072 6967 5f63  e = {}.    rig_c
+00001470: 6f6e 7472 6f6c 203d 204e 6f6e 650a 2020  ontrol = None.  
+00001480: 2020 6d75 6c74 6963 6173 745f 6772 6f75    multicast_grou
+00001490: 7020 3d20 4e6f 6e65 0a20 2020 206d 756c  p = None.    mul
+000014a0: 7469 6361 7374 5f70 6f72 7420 3d20 4e6f  ticast_port = No
+000014b0: 6e65 0a20 2020 2069 6e74 6572 6661 6365  ne.    interface
+000014c0: 5f69 7020 3d20 4e6f 6e65 0a20 2020 2072  _ip = None.    r
+000014d0: 6967 5f63 6f6e 7472 6f6c 203d 204e 6f6e  ig_control = Non
+000014e0: 650a 0a20 2020 2064 6566 205f 5f69 6e69  e..    def __ini
+000014f0: 745f 5f28 7365 6c66 2c20 2a61 7267 732c  t__(self, *args,
+00001500: 202a 2a6b 7761 7267 7329 3a0a 2020 2020   **kwargs):.    
+00001510: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
+00001520: 6974 5f5f 282a 6172 6773 2c20 2a2a 6b77  it__(*args, **kw
+00001530: 6172 6773 290a 2020 2020 2020 2020 6c6f  args).        lo
+00001540: 6767 6572 2e69 6e66 6f28 224d 6169 6e57  gger.info("MainW
+00001550: 696e 646f 773a 205f 5f69 6e69 745f 5f22  indow: __init__"
+00001560: 290a 2020 2020 2020 2020 6461 7461 5f70  ).        data_p
+00001570: 6174 6820 3d20 574f 524b 494e 475f 5041  ath = WORKING_PA
+00001580: 5448 202b 2022 2f64 6174 612f 6d61 696e  TH + "/data/main
+00001590: 2e75 6922 0a20 2020 2020 2020 2075 6963  .ui".        uic
+000015a0: 2e6c 6f61 6455 6928 6461 7461 5f70 6174  .loadUi(data_pat
+000015b0: 682c 2073 656c 6629 0a20 2020 2020 2020  h, self).       
+000015c0: 2073 656c 662e 6c65 6674 646f 742e 6869   self.leftdot.hi
+000015d0: 6465 2829 0a20 2020 2020 2020 2073 656c  de().        sel
+000015e0: 662e 7269 6768 7464 6f74 2e68 6964 6528  f.rightdot.hide(
+000015f0: 290a 2020 2020 2020 2020 7365 6c66 2e6e  ).        self.n
+00001600: 316d 6d20 3d20 4e31 4d4d 2829 0a20 2020  1mm = N1MM().   
+00001610: 2020 2020 2073 656c 662e 6e65 7874 5f66       self.next_f
+00001620: 6965 6c64 203d 2073 656c 662e 6f74 6865  ield = self.othe
+00001630: 725f 320a 2020 2020 2020 2020 7365 6c66  r_2.        self
+00001640: 2e64 7570 655f 696e 6469 6361 746f 722e  .dupe_indicator.
+00001650: 6869 6465 2829 0a20 2020 2020 2020 2073  hide().        s
+00001660: 656c 662e 6377 5f73 7065 6564 2e76 616c  elf.cw_speed.val
+00001670: 7565 4368 616e 6765 642e 636f 6e6e 6563  ueChanged.connec
+00001680: 7428 7365 6c66 2e63 7773 7065 6564 5f73  t(self.cwspeed_s
+00001690: 7069 6e62 6f78 5f63 6861 6e67 6564 290a  pinbox_changed).
+000016a0: 0a20 2020 2020 2020 2073 656c 662e 6163  .        self.ac
+000016b0: 7469 6f6e 4357 5f4d 6163 726f 732e 7472  tionCW_Macros.tr
+000016c0: 6967 6765 7265 642e 636f 6e6e 6563 7428  iggered.connect(
+000016d0: 7365 6c66 2e63 775f 6d61 6372 6f73 5f73  self.cw_macros_s
+000016e0: 7461 7465 5f63 6861 6e67 6564 290a 2020  tate_changed).  
+000016f0: 2020 2020 2020 7365 6c66 2e61 6374 696f        self.actio
+00001700: 6e43 6f6d 6d61 6e64 5f42 7574 746f 6e73  nCommand_Buttons
+00001710: 2e74 7269 6767 6572 6564 2e63 6f6e 6e65  .triggered.conne
+00001720: 6374 2873 656c 662e 636f 6d6d 616e 645f  ct(self.command_
+00001730: 6275 7474 6f6e 735f 7374 6174 655f 6368  buttons_state_ch
+00001740: 616e 6765 290a 2020 2020 2020 2020 7365  ange).        se
+00001750: 6c66 2e61 6374 696f 6e4c 6f67 5f57 696e  lf.actionLog_Win
+00001760: 646f 772e 7472 6967 6765 7265 642e 636f  dow.triggered.co
+00001770: 6e6e 6563 7428 7365 6c66 2e6c 6175 6e63  nnect(self.launc
+00001780: 685f 6c6f 675f 7769 6e64 6f77 290a 2020  h_log_window).  
+00001790: 2020 2020 2020 7365 6c66 2e61 6374 696f        self.actio
+000017a0: 6e42 616e 646d 6170 2e74 7269 6767 6572  nBandmap.trigger
+000017b0: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
+000017c0: 6c61 756e 6368 5f62 616e 646d 6170 5f77  launch_bandmap_w
+000017d0: 696e 646f 7729 0a20 2020 2020 2020 2073  indow).        s
+000017e0: 656c 662e 6163 7469 6f6e 5265 6361 6c63  elf.actionRecalc
+000017f0: 756c 6174 655f 4d75 6c74 732e 7472 6967  ulate_Mults.trig
+00001800: 6765 7265 642e 636f 6e6e 6563 7428 7365  gered.connect(se
+00001810: 6c66 2e72 6563 616c 6375 6c61 7465 5f6d  lf.recalculate_m
+00001820: 756c 7473 290a 0a20 2020 2020 2020 2073  ults)..        s
+00001830: 656c 662e 6163 7469 6f6e 4765 6e65 7261  elf.actionGenera
+00001840: 7465 5f43 6162 7269 6c6c 6f2e 7472 6967  te_Cabrillo.trig
+00001850: 6765 7265 642e 636f 6e6e 6563 7428 7365  gered.connect(se
+00001860: 6c66 2e67 656e 6572 6174 655f 6361 6272  lf.generate_cabr
+00001870: 696c 6c6f 290a 2020 2020 2020 2020 7365  illo).        se
+00001880: 6c66 2e61 6374 696f 6e47 656e 6572 6174  lf.actionGenerat
+00001890: 655f 4144 4946 2e74 7269 6767 6572 6564  e_ADIF.triggered
+000018a0: 2e63 6f6e 6e65 6374 2873 656c 662e 6765  .connect(self.ge
+000018b0: 6e65 7261 7465 5f61 6469 6629 0a0a 2020  nerate_adif)..  
+000018c0: 2020 2020 2020 7365 6c66 2e61 6374 696f        self.actio
+000018d0: 6e43 6f6e 6669 6775 7261 7469 6f6e 5f53  nConfiguration_S
+000018e0: 6574 7469 6e67 732e 7472 6967 6765 7265  ettings.triggere
+000018f0: 642e 636f 6e6e 6563 7428 0a20 2020 2020  d.connect(.     
+00001900: 2020 2020 2020 2073 656c 662e 6564 6974         self.edit
+00001910: 5f63 6f6e 6669 6775 7261 7469 6f6e 5f73  _configuration_s
+00001920: 6574 7469 6e67 730a 2020 2020 2020 2020  ettings.        
+00001930: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+00001940: 6374 696f 6e53 7461 7469 6f6e 5365 7474  ctionStationSett
+00001950: 696e 6773 2e74 7269 6767 6572 6564 2e63  ings.triggered.c
+00001960: 6f6e 6e65 6374 2873 656c 662e 6564 6974  onnect(self.edit
+00001970: 5f73 7461 7469 6f6e 5f73 6574 7469 6e67  _station_setting
+00001980: 7329 0a0a 2020 2020 2020 2020 7365 6c66  s)..        self
+00001990: 2e61 6374 696f 6e4e 6577 5f43 6f6e 7465  .actionNew_Conte
+000019a0: 7374 2e74 7269 6767 6572 6564 2e63 6f6e  st.triggered.con
+000019b0: 6e65 6374 2873 656c 662e 6e65 775f 636f  nect(self.new_co
+000019c0: 6e74 6573 745f 6469 616c 6f67 290a 2020  ntest_dialog).  
+000019d0: 2020 2020 2020 7365 6c66 2e61 6374 696f        self.actio
+000019e0: 6e4f 7065 6e5f 436f 6e74 6573 742e 7472  nOpen_Contest.tr
+000019f0: 6967 6765 7265 642e 636f 6e6e 6563 7428  iggered.connect(
+00001a00: 7365 6c66 2e6f 7065 6e5f 636f 6e74 6573  self.open_contes
+00001a10: 7429 0a20 2020 2020 2020 2073 656c 662e  t).        self.
+00001a20: 6163 7469 6f6e 4564 6974 5f43 7572 7265  actionEdit_Curre
+00001a30: 6e74 5f43 6f6e 7465 7374 2e74 7269 6767  nt_Contest.trigg
+00001a40: 6572 6564 2e63 6f6e 6e65 6374 2873 656c  ered.connect(sel
+00001a50: 662e 6564 6974 5f63 6f6e 7465 7374 290a  f.edit_contest).
+00001a60: 0a20 2020 2020 2020 2073 656c 662e 6163  .        self.ac
+00001a70: 7469 6f6e 4e65 775f 4461 7461 6261 7365  tionNew_Database
+00001a80: 2e74 7269 6767 6572 6564 2e63 6f6e 6e65  .triggered.conne
+00001a90: 6374 2873 656c 662e 6e65 775f 6461 7461  ct(self.new_data
+00001aa0: 6261 7365 290a 2020 2020 2020 2020 7365  base).        se
+00001ab0: 6c66 2e61 6374 696f 6e4f 7065 6e5f 4461  lf.actionOpen_Da
+00001ac0: 7461 6261 7365 2e74 7269 6767 6572 6564  tabase.triggered
+00001ad0: 2e63 6f6e 6e65 6374 2873 656c 662e 6f70  .connect(self.op
+00001ae0: 656e 5f64 6174 6162 6173 6529 0a0a 2020  en_database)..  
+00001af0: 2020 2020 2020 7365 6c66 2e61 6374 696f        self.actio
+00001b00: 6e45 6469 745f 4d61 6372 6f73 2e74 7269  nEdit_Macros.tri
+00001b10: 6767 6572 6564 2e63 6f6e 6e65 6374 2873  ggered.connect(s
+00001b20: 656c 662e 6564 6974 5f63 775f 6d61 6372  elf.edit_cw_macr
+00001b30: 6f73 290a 0a20 2020 2020 2020 2073 656c  os)..        sel
+00001b40: 662e 6163 7469 6f6e 4162 6f75 742e 7472  f.actionAbout.tr
+00001b50: 6967 6765 7265 642e 636f 6e6e 6563 7428  iggered.connect(
+00001b60: 7365 6c66 2e73 686f 775f 6162 6f75 745f  self.show_about_
+00001b70: 6469 616c 6f67 290a 0a20 2020 2020 2020  dialog)..       
+00001b80: 2073 656c 662e 7261 6469 6f42 7574 746f   self.radioButto
+00001b90: 6e5f 7275 6e2e 636c 6963 6b65 642e 636f  n_run.clicked.co
+00001ba0: 6e6e 6563 7428 7365 6c66 2e72 756e 5f73  nnect(self.run_s
+00001bb0: 705f 6275 7474 6f6e 735f 636c 6963 6b65  p_buttons_clicke
+00001bc0: 6429 0a20 2020 2020 2020 2073 656c 662e  d).        self.
+00001bd0: 7261 6469 6f42 7574 746f 6e5f 7370 2e63  radioButton_sp.c
+00001be0: 6c69 636b 6564 2e63 6f6e 6e65 6374 2873  licked.connect(s
+00001bf0: 656c 662e 7275 6e5f 7370 5f62 7574 746f  elf.run_sp_butto
+00001c00: 6e73 5f63 6c69 636b 6564 290a 2020 2020  ns_clicked).    
+00001c10: 2020 2020 7365 6c66 2e73 636f 7265 2e73      self.score.s
+00001c20: 6574 5465 7874 2822 3022 290a 2020 2020  etText("0").    
+00001c30: 2020 2020 7365 6c66 2e63 616c 6c73 6967      self.callsig
+00001c40: 6e2e 7465 7874 4564 6974 6564 2e63 6f6e  n.textEdited.con
+00001c50: 6e65 6374 2873 656c 662e 6361 6c6c 7369  nect(self.callsi
+00001c60: 676e 5f63 6861 6e67 6564 290a 2020 2020  gn_changed).    
+00001c70: 2020 2020 7365 6c66 2e63 616c 6c73 6967      self.callsig
+00001c80: 6e2e 7265 7475 726e 5072 6573 7365 642e  n.returnPressed.
+00001c90: 636f 6e6e 6563 7428 7365 6c66 2e73 6176  connect(self.sav
+00001ca0: 655f 636f 6e74 6163 7429 0a20 2020 2020  e_contact).     
+00001cb0: 2020 2073 656c 662e 7365 6e74 2e72 6574     self.sent.ret
+00001cc0: 7572 6e50 7265 7373 6564 2e63 6f6e 6e65  urnPressed.conne
+00001cd0: 6374 2873 656c 662e 7361 7665 5f63 6f6e  ct(self.save_con
+00001ce0: 7461 6374 290a 2020 2020 2020 2020 7365  tact).        se
+00001cf0: 6c66 2e72 6563 6569 7665 2e72 6574 7572  lf.receive.retur
+00001d00: 6e50 7265 7373 6564 2e63 6f6e 6e65 6374  nPressed.connect
+00001d10: 2873 656c 662e 7361 7665 5f63 6f6e 7461  (self.save_conta
+00001d20: 6374 290a 2020 2020 2020 2020 7365 6c66  ct).        self
+00001d30: 2e6f 7468 6572 5f31 2e72 6574 7572 6e50  .other_1.returnP
+00001d40: 7265 7373 6564 2e63 6f6e 6e65 6374 2873  ressed.connect(s
+00001d50: 656c 662e 7361 7665 5f63 6f6e 7461 6374  elf.save_contact
+00001d60: 290a 2020 2020 2020 2020 7365 6c66 2e6f  ).        self.o
+00001d70: 7468 6572 5f32 2e72 6574 7572 6e50 7265  ther_2.returnPre
+00001d80: 7373 6564 2e63 6f6e 6e65 6374 2873 656c  ssed.connect(sel
+00001d90: 662e 7361 7665 5f63 6f6e 7461 6374 290a  f.save_contact).
+00001da0: 2020 2020 2020 2020 7365 6c66 2e6f 7468          self.oth
+00001db0: 6572 5f32 2e74 6578 7445 6469 7465 642e  er_2.textEdited.
+00001dc0: 636f 6e6e 6563 7428 7365 6c66 2e6f 7468  connect(self.oth
+00001dd0: 6572 5f32 5f63 6861 6e67 6564 290a 0a20  er_2_changed).. 
+00001de0: 2020 2020 2020 2073 656c 662e 7365 6e74         self.sent
+00001df0: 2e73 6574 5465 7874 2822 3539 2229 0a20  .setText("59"). 
+00001e00: 2020 2020 2020 2073 656c 662e 7265 6365         self.rece
+00001e10: 6976 652e 7365 7454 6578 7428 2235 3922  ive.setText("59"
+00001e20: 290a 2020 2020 2020 2020 6963 6f6e 5f70  ).        icon_p
+00001e30: 6174 6820 3d20 574f 524b 494e 475f 5041  ath = WORKING_PA
+00001e40: 5448 202b 2022 2f64 6174 612f 220a 2020  TH + "/data/".  
+00001e50: 2020 2020 2020 7365 6c66 2e67 7265 656e        self.green
+00001e60: 646f 7420 3d20 5174 4775 692e 5150 6978  dot = QtGui.QPix
+00001e70: 6d61 7028 6963 6f6e 5f70 6174 6820 2b20  map(icon_path + 
+00001e80: 2267 7265 656e 646f 742e 706e 6722 290a  "greendot.png").
+00001e90: 2020 2020 2020 2020 7365 6c66 2e72 6564          self.red
+00001ea0: 646f 7420 3d20 5174 4775 692e 5150 6978  dot = QtGui.QPix
+00001eb0: 6d61 7028 6963 6f6e 5f70 6174 6820 2b20  map(icon_path + 
+00001ec0: 2272 6564 646f 742e 706e 6722 290a 2020  "reddot.png").  
+00001ed0: 2020 2020 2020 7365 6c66 2e6c 6566 7464        self.leftd
+00001ee0: 6f74 2e73 6574 5069 786d 6170 2873 656c  ot.setPixmap(sel
+00001ef0: 662e 6772 6565 6e64 6f74 290a 2020 2020  f.greendot).    
+00001f00: 2020 2020 7365 6c66 2e72 6967 6874 646f      self.rightdo
+00001f10: 742e 7365 7450 6978 6d61 7028 7365 6c66  t.setPixmap(self
+00001f20: 2e72 6564 646f 7429 0a0a 2020 2020 2020  .reddot)..      
+00001f30: 2020 7365 6c66 2e46 312e 7365 7443 6f6e    self.F1.setCon
+00001f40: 7465 7874 4d65 6e75 506f 6c69 6379 2851  textMenuPolicy(Q
+00001f50: 7443 6f72 652e 5174 2e43 7573 746f 6d43  tCore.Qt.CustomC
+00001f60: 6f6e 7465 7874 4d65 6e75 290a 2020 2020  ontextMenu).    
+00001f70: 2020 2020 7365 6c66 2e46 312e 6375 7374      self.F1.cust
+00001f80: 6f6d 436f 6e74 6578 744d 656e 7552 6571  omContextMenuReq
+00001f90: 7565 7374 6564 2e63 6f6e 6e65 6374 2873  uested.connect(s
+00001fa0: 656c 662e 6564 6974 5f46 3129 0a20 2020  elf.edit_F1).   
+00001fb0: 2020 2020 2073 656c 662e 4631 2e63 6c69       self.F1.cli
+00001fc0: 636b 6564 2e63 6f6e 6e65 6374 2873 656c  cked.connect(sel
+00001fd0: 662e 7365 6e64 6631 290a 2020 2020 2020  f.sendf1).      
+00001fe0: 2020 7365 6c66 2e46 322e 7365 7443 6f6e    self.F2.setCon
+00001ff0: 7465 7874 4d65 6e75 506f 6c69 6379 2851  textMenuPolicy(Q
+00002000: 7443 6f72 652e 5174 2e43 7573 746f 6d43  tCore.Qt.CustomC
+00002010: 6f6e 7465 7874 4d65 6e75 290a 2020 2020  ontextMenu).    
+00002020: 2020 2020 7365 6c66 2e46 322e 6375 7374      self.F2.cust
+00002030: 6f6d 436f 6e74 6578 744d 656e 7552 6571  omContextMenuReq
+00002040: 7565 7374 6564 2e63 6f6e 6e65 6374 2873  uested.connect(s
+00002050: 656c 662e 6564 6974 5f46 3229 0a20 2020  elf.edit_F2).   
+00002060: 2020 2020 2073 656c 662e 4632 2e63 6c69       self.F2.cli
+00002070: 636b 6564 2e63 6f6e 6e65 6374 2873 656c  cked.connect(sel
+00002080: 662e 7365 6e64 6632 290a 2020 2020 2020  f.sendf2).      
+00002090: 2020 7365 6c66 2e46 332e 7365 7443 6f6e    self.F3.setCon
+000020a0: 7465 7874 4d65 6e75 506f 6c69 6379 2851  textMenuPolicy(Q
+000020b0: 7443 6f72 652e 5174 2e43 7573 746f 6d43  tCore.Qt.CustomC
+000020c0: 6f6e 7465 7874 4d65 6e75 290a 2020 2020  ontextMenu).    
+000020d0: 2020 2020 7365 6c66 2e46 332e 6375 7374      self.F3.cust
+000020e0: 6f6d 436f 6e74 6578 744d 656e 7552 6571  omContextMenuReq
+000020f0: 7565 7374 6564 2e63 6f6e 6e65 6374 2873  uested.connect(s
+00002100: 656c 662e 6564 6974 5f46 3329 0a20 2020  elf.edit_F3).   
+00002110: 2020 2020 2073 656c 662e 4633 2e63 6c69       self.F3.cli
+00002120: 636b 6564 2e63 6f6e 6e65 6374 2873 656c  cked.connect(sel
+00002130: 662e 7365 6e64 6633 290a 2020 2020 2020  f.sendf3).      
+00002140: 2020 7365 6c66 2e46 342e 7365 7443 6f6e    self.F4.setCon
+00002150: 7465 7874 4d65 6e75 506f 6c69 6379 2851  textMenuPolicy(Q
+00002160: 7443 6f72 652e 5174 2e43 7573 746f 6d43  tCore.Qt.CustomC
+00002170: 6f6e 7465 7874 4d65 6e75 290a 2020 2020  ontextMenu).    
+00002180: 2020 2020 7365 6c66 2e46 342e 6375 7374      self.F4.cust
+00002190: 6f6d 436f 6e74 6578 744d 656e 7552 6571  omContextMenuReq
+000021a0: 7565 7374 6564 2e63 6f6e 6e65 6374 2873  uested.connect(s
+000021b0: 656c 662e 6564 6974 5f46 3429 0a20 2020  elf.edit_F4).   
+000021c0: 2020 2020 2073 656c 662e 4634 2e63 6c69       self.F4.cli
+000021d0: 636b 6564 2e63 6f6e 6e65 6374 2873 656c  cked.connect(sel
+000021e0: 662e 7365 6e64 6634 290a 2020 2020 2020  f.sendf4).      
+000021f0: 2020 7365 6c66 2e46 352e 7365 7443 6f6e    self.F5.setCon
+00002200: 7465 7874 4d65 6e75 506f 6c69 6379 2851  textMenuPolicy(Q
+00002210: 7443 6f72 652e 5174 2e43 7573 746f 6d43  tCore.Qt.CustomC
+00002220: 6f6e 7465 7874 4d65 6e75 290a 2020 2020  ontextMenu).    
+00002230: 2020 2020 7365 6c66 2e46 352e 6375 7374      self.F5.cust
+00002240: 6f6d 436f 6e74 6578 744d 656e 7552 6571  omContextMenuReq
+00002250: 7565 7374 6564 2e63 6f6e 6e65 6374 2873  uested.connect(s
+00002260: 656c 662e 6564 6974 5f46 3529 0a20 2020  elf.edit_F5).   
+00002270: 2020 2020 2073 656c 662e 4635 2e63 6c69       self.F5.cli
+00002280: 636b 6564 2e63 6f6e 6e65 6374 2873 656c  cked.connect(sel
+00002290: 662e 7365 6e64 6635 290a 2020 2020 2020  f.sendf5).      
+000022a0: 2020 7365 6c66 2e46 362e 7365 7443 6f6e    self.F6.setCon
+000022b0: 7465 7874 4d65 6e75 506f 6c69 6379 2851  textMenuPolicy(Q
+000022c0: 7443 6f72 652e 5174 2e43 7573 746f 6d43  tCore.Qt.CustomC
+000022d0: 6f6e 7465 7874 4d65 6e75 290a 2020 2020  ontextMenu).    
+000022e0: 2020 2020 7365 6c66 2e46 362e 6375 7374      self.F6.cust
+000022f0: 6f6d 436f 6e74 6578 744d 656e 7552 6571  omContextMenuReq
+00002300: 7565 7374 6564 2e63 6f6e 6e65 6374 2873  uested.connect(s
+00002310: 656c 662e 6564 6974 5f46 3629 0a20 2020  elf.edit_F6).   
+00002320: 2020 2020 2073 656c 662e 4636 2e63 6c69       self.F6.cli
+00002330: 636b 6564 2e63 6f6e 6e65 6374 2873 656c  cked.connect(sel
+00002340: 662e 7365 6e64 6636 290a 2020 2020 2020  f.sendf6).      
+00002350: 2020 7365 6c66 2e46 372e 7365 7443 6f6e    self.F7.setCon
+00002360: 7465 7874 4d65 6e75 506f 6c69 6379 2851  textMenuPolicy(Q
+00002370: 7443 6f72 652e 5174 2e43 7573 746f 6d43  tCore.Qt.CustomC
+00002380: 6f6e 7465 7874 4d65 6e75 290a 2020 2020  ontextMenu).    
+00002390: 2020 2020 7365 6c66 2e46 372e 6375 7374      self.F7.cust
+000023a0: 6f6d 436f 6e74 6578 744d 656e 7552 6571  omContextMenuReq
+000023b0: 7565 7374 6564 2e63 6f6e 6e65 6374 2873  uested.connect(s
+000023c0: 656c 662e 6564 6974 5f46 3729 0a20 2020  elf.edit_F7).   
+000023d0: 2020 2020 2073 656c 662e 4637 2e63 6c69       self.F7.cli
+000023e0: 636b 6564 2e63 6f6e 6e65 6374 2873 656c  cked.connect(sel
+000023f0: 662e 7365 6e64 6637 290a 2020 2020 2020  f.sendf7).      
+00002400: 2020 7365 6c66 2e46 382e 7365 7443 6f6e    self.F8.setCon
+00002410: 7465 7874 4d65 6e75 506f 6c69 6379 2851  textMenuPolicy(Q
+00002420: 7443 6f72 652e 5174 2e43 7573 746f 6d43  tCore.Qt.CustomC
+00002430: 6f6e 7465 7874 4d65 6e75 290a 2020 2020  ontextMenu).    
+00002440: 2020 2020 7365 6c66 2e46 382e 6375 7374      self.F8.cust
+00002450: 6f6d 436f 6e74 6578 744d 656e 7552 6571  omContextMenuReq
+00002460: 7565 7374 6564 2e63 6f6e 6e65 6374 2873  uested.connect(s
+00002470: 656c 662e 6564 6974 5f46 3829 0a20 2020  elf.edit_F8).   
+00002480: 2020 2020 2073 656c 662e 4638 2e63 6c69       self.F8.cli
+00002490: 636b 6564 2e63 6f6e 6e65 6374 2873 656c  cked.connect(sel
+000024a0: 662e 7365 6e64 6638 290a 2020 2020 2020  f.sendf8).      
+000024b0: 2020 7365 6c66 2e46 392e 7365 7443 6f6e    self.F9.setCon
+000024c0: 7465 7874 4d65 6e75 506f 6c69 6379 2851  textMenuPolicy(Q
+000024d0: 7443 6f72 652e 5174 2e43 7573 746f 6d43  tCore.Qt.CustomC
+000024e0: 6f6e 7465 7874 4d65 6e75 290a 2020 2020  ontextMenu).    
+000024f0: 2020 2020 7365 6c66 2e46 392e 6375 7374      self.F9.cust
+00002500: 6f6d 436f 6e74 6578 744d 656e 7552 6571  omContextMenuReq
+00002510: 7565 7374 6564 2e63 6f6e 6e65 6374 2873  uested.connect(s
+00002520: 656c 662e 6564 6974 5f46 3929 0a20 2020  elf.edit_F9).   
+00002530: 2020 2020 2073 656c 662e 4639 2e63 6c69       self.F9.cli
+00002540: 636b 6564 2e63 6f6e 6e65 6374 2873 656c  cked.connect(sel
+00002550: 662e 7365 6e64 6639 290a 2020 2020 2020  f.sendf9).      
+00002560: 2020 7365 6c66 2e46 3130 2e73 6574 436f    self.F10.setCo
+00002570: 6e74 6578 744d 656e 7550 6f6c 6963 7928  ntextMenuPolicy(
+00002580: 5174 436f 7265 2e51 742e 4375 7374 6f6d  QtCore.Qt.Custom
+00002590: 436f 6e74 6578 744d 656e 7529 0a20 2020  ContextMenu).   
+000025a0: 2020 2020 2073 656c 662e 4631 302e 6375       self.F10.cu
+000025b0: 7374 6f6d 436f 6e74 6578 744d 656e 7552  stomContextMenuR
+000025c0: 6571 7565 7374 6564 2e63 6f6e 6e65 6374  equested.connect
+000025d0: 2873 656c 662e 6564 6974 5f46 3130 290a  (self.edit_F10).
+000025e0: 2020 2020 2020 2020 7365 6c66 2e46 3130          self.F10
+000025f0: 2e63 6c69 636b 6564 2e63 6f6e 6e65 6374  .clicked.connect
+00002600: 2873 656c 662e 7365 6e64 6631 3029 0a20  (self.sendf10). 
+00002610: 2020 2020 2020 2073 656c 662e 4631 312e         self.F11.
+00002620: 7365 7443 6f6e 7465 7874 4d65 6e75 506f  setContextMenuPo
+00002630: 6c69 6379 2851 7443 6f72 652e 5174 2e43  licy(QtCore.Qt.C
+00002640: 7573 746f 6d43 6f6e 7465 7874 4d65 6e75  ustomContextMenu
+00002650: 290a 2020 2020 2020 2020 7365 6c66 2e46  ).        self.F
+00002660: 3131 2e63 7573 746f 6d43 6f6e 7465 7874  11.customContext
+00002670: 4d65 6e75 5265 7175 6573 7465 642e 636f  MenuRequested.co
+00002680: 6e6e 6563 7428 7365 6c66 2e65 6469 745f  nnect(self.edit_
+00002690: 4631 3129 0a20 2020 2020 2020 2073 656c  F11).        sel
+000026a0: 662e 4631 312e 636c 6963 6b65 642e 636f  f.F11.clicked.co
+000026b0: 6e6e 6563 7428 7365 6c66 2e73 656e 6466  nnect(self.sendf
+000026c0: 3131 290a 2020 2020 2020 2020 7365 6c66  11).        self
+000026d0: 2e46 3132 2e73 6574 436f 6e74 6578 744d  .F12.setContextM
+000026e0: 656e 7550 6f6c 6963 7928 5174 436f 7265  enuPolicy(QtCore
+000026f0: 2e51 742e 4375 7374 6f6d 436f 6e74 6578  .Qt.CustomContex
+00002700: 744d 656e 7529 0a20 2020 2020 2020 2073  tMenu).        s
+00002710: 656c 662e 4631 322e 6375 7374 6f6d 436f  elf.F12.customCo
+00002720: 6e74 6578 744d 656e 7552 6571 7565 7374  ntextMenuRequest
+00002730: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
+00002740: 6564 6974 5f46 3132 290a 2020 2020 2020  edit_F12).      
+00002750: 2020 7365 6c66 2e46 3132 2e63 6c69 636b    self.F12.click
+00002760: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
+00002770: 7365 6e64 6631 3229 0a0a 2020 2020 2020  sendf12)..      
+00002780: 2020 7365 6c66 2e72 6561 6470 7265 6665    self.readprefe
+00002790: 7265 6e63 6573 2829 0a20 2020 2020 2020  rences().       
+000027a0: 2073 656c 662e 6462 6e61 6d65 203d 2044   self.dbname = D
+000027b0: 4154 415f 5041 5448 202b 2022 2f22 202b  ATA_PATH + "/" +
+000027c0: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
+000027d0: 6375 7272 656e 745f 6461 7461 6261 7365  current_database
+000027e0: 222c 2022 6861 6d2e 6462 2229 0a20 2020  ", "ham.db").   
+000027f0: 2020 2020 2073 656c 662e 6461 7461 6261       self.databa
+00002800: 7365 203d 2044 6174 6142 6173 6528 7365  se = DataBase(se
+00002810: 6c66 2e64 626e 616d 652c 2057 4f52 4b49  lf.dbname, WORKI
+00002820: 4e47 5f50 4154 4829 0a20 2020 2020 2020  NG_PATH).       
+00002830: 2073 656c 662e 7374 6174 696f 6e20 3d20   self.station = 
+00002840: 7365 6c66 2e64 6174 6162 6173 652e 6665  self.database.fe
+00002850: 7463 685f 7374 6174 696f 6e28 290a 2020  tch_station().  
+00002860: 2020 2020 2020 6966 2073 656c 662e 7374        if self.st
+00002870: 6174 696f 6e20 6973 204e 6f6e 653a 0a20  ation is None:. 
+00002880: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00002890: 7374 6174 696f 6e20 3d20 7b7d 0a20 2020  station = {}.   
+000028a0: 2020 2020 2020 2020 2073 656c 662e 6564           self.ed
+000028b0: 6974 5f73 7461 7469 6f6e 5f73 6574 7469  it_station_setti
+000028c0: 6e67 7328 290a 2020 2020 2020 2020 2020  ngs().          
+000028d0: 2020 7365 6c66 2e73 7461 7469 6f6e 203d    self.station =
+000028e0: 2073 656c 662e 6461 7461 6261 7365 2e66   self.database.f
+000028f0: 6574 6368 5f73 7461 7469 6f6e 2829 0a20  etch_station(). 
+00002900: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00002910: 6c66 2e73 7461 7469 6f6e 2069 7320 4e6f  lf.station is No
+00002920: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00002930: 2020 2020 7365 6c66 2e73 7461 7469 6f6e      self.station
+00002940: 203d 207b 7d0a 2020 2020 2020 2020 7365   = {}.        se
+00002950: 6c66 2e63 6f6e 7461 6374 203d 2073 656c  lf.contact = sel
+00002960: 662e 6461 7461 6261 7365 2e65 6d70 7479  f.database.empty
+00002970: 5f63 6f6e 7461 6374 0a20 2020 2020 2020  _contact.       
+00002980: 2073 656c 662e 6375 7272 656e 745f 6f70   self.current_op
+00002990: 203d 2073 656c 662e 7374 6174 696f 6e2e   = self.station.
+000029a0: 6765 7428 2243 616c 6c22 2c20 2222 290a  get("Call", "").
+000029b0: 2020 2020 2020 2020 7365 6c66 2e6d 616b          self.mak
+000029c0: 655f 6f70 5f64 6972 2829 0a20 2020 2020  e_op_dir().     
+000029d0: 2020 2073 656c 662e 7265 6164 5f63 775f     self.read_cw_
+000029e0: 6d61 6372 6f73 2829 0a20 2020 2020 2020  macros().       
+000029f0: 2073 656c 662e 636c 6561 7269 6e70 7574   self.clearinput
+00002a00: 7328 290a 0a20 2020 2020 2020 2073 656c  s()..        sel
+00002a10: 662e 6261 6e64 5f69 6e64 6963 6174 6f72  f.band_indicator
+00002a20: 735f 6377 203d 207b 0a20 2020 2020 2020  s_cw = {.       
+00002a30: 2020 2020 2022 3136 3022 3a20 7365 6c66       "160": self
+00002a40: 2e63 775f 6261 6e64 5f31 3630 2c0a 2020  .cw_band_160,.  
+00002a50: 2020 2020 2020 2020 2020 2238 3022 3a20            "80": 
+00002a60: 7365 6c66 2e63 775f 6261 6e64 5f38 302c  self.cw_band_80,
+00002a70: 0a20 2020 2020 2020 2020 2020 2022 3430  .            "40
+00002a80: 223a 2073 656c 662e 6377 5f62 616e 645f  ": self.cw_band_
+00002a90: 3430 2c0a 2020 2020 2020 2020 2020 2020  40,.            
+00002aa0: 2232 3022 3a20 7365 6c66 2e63 775f 6261  "20": self.cw_ba
+00002ab0: 6e64 5f32 302c 0a20 2020 2020 2020 2020  nd_20,.         
+00002ac0: 2020 2022 3135 223a 2073 656c 662e 6377     "15": self.cw
+00002ad0: 5f62 616e 645f 3135 2c0a 2020 2020 2020  _band_15,.      
+00002ae0: 2020 2020 2020 2231 3022 3a20 7365 6c66        "10": self
+00002af0: 2e63 775f 6261 6e64 5f31 302c 0a20 2020  .cw_band_10,.   
+00002b00: 2020 2020 207d 0a0a 2020 2020 2020 2020       }..        
+00002b10: 7365 6c66 2e62 616e 645f 696e 6469 6361  self.band_indica
+00002b20: 746f 7273 5f73 7362 203d 207b 0a20 2020  tors_ssb = {.   
+00002b30: 2020 2020 2020 2020 2022 3136 3022 3a20           "160": 
+00002b40: 7365 6c66 2e73 7362 5f62 616e 645f 3136  self.ssb_band_16
+00002b50: 302c 0a20 2020 2020 2020 2020 2020 2022  0,.            "
+00002b60: 3830 223a 2073 656c 662e 7373 625f 6261  80": self.ssb_ba
+00002b70: 6e64 5f38 302c 0a20 2020 2020 2020 2020  nd_80,.         
+00002b80: 2020 2022 3430 223a 2073 656c 662e 7373     "40": self.ss
+00002b90: 625f 6261 6e64 5f34 302c 0a20 2020 2020  b_band_40,.     
+00002ba0: 2020 2020 2020 2022 3230 223a 2073 656c         "20": sel
+00002bb0: 662e 7373 625f 6261 6e64 5f32 302c 0a20  f.ssb_band_20,. 
+00002bc0: 2020 2020 2020 2020 2020 2022 3135 223a             "15":
+00002bd0: 2073 656c 662e 7373 625f 6261 6e64 5f31   self.ssb_band_1
+00002be0: 352c 0a20 2020 2020 2020 2020 2020 2022  5,.            "
+00002bf0: 3130 223a 2073 656c 662e 7373 625f 6261  10": self.ssb_ba
+00002c00: 6e64 5f31 302c 0a20 2020 2020 2020 207d  nd_10,.        }
+00002c10: 0a0a 2020 2020 2020 2020 7365 6c66 2e62  ..        self.b
+00002c20: 616e 645f 696e 6469 6361 746f 7273 5f72  and_indicators_r
+00002c30: 7474 7920 3d20 7b0a 2020 2020 2020 2020  tty = {.        
+00002c40: 2020 2020 2231 3630 223a 2073 656c 662e      "160": self.
+00002c50: 7274 7479 5f62 616e 645f 3136 302c 0a20  rtty_band_160,. 
+00002c60: 2020 2020 2020 2020 2020 2022 3830 223a             "80":
+00002c70: 2073 656c 662e 7274 7479 5f62 616e 645f   self.rtty_band_
+00002c80: 3830 2c0a 2020 2020 2020 2020 2020 2020  80,.            
+00002c90: 2234 3022 3a20 7365 6c66 2e72 7474 795f  "40": self.rtty_
+00002ca0: 6261 6e64 5f34 302c 0a20 2020 2020 2020  band_40,.       
+00002cb0: 2020 2020 2022 3230 223a 2073 656c 662e       "20": self.
+00002cc0: 7274 7479 5f62 616e 645f 3230 2c0a 2020  rtty_band_20,.  
+00002cd0: 2020 2020 2020 2020 2020 2231 3522 3a20            "15": 
+00002ce0: 7365 6c66 2e72 7474 795f 6261 6e64 5f31  self.rtty_band_1
+00002cf0: 352c 0a20 2020 2020 2020 2020 2020 2022  5,.            "
+00002d00: 3130 223a 2073 656c 662e 7274 7479 5f62  10": self.rtty_b
+00002d10: 616e 645f 3130 2c0a 2020 2020 2020 2020  and_10,.        
+00002d20: 7d0a 0a20 2020 2020 2020 2073 656c 662e  }..        self.
+00002d30: 616c 6c5f 6d6f 6465 5f69 6e64 6963 6174  all_mode_indicat
+00002d40: 6f72 7320 3d20 7b0a 2020 2020 2020 2020  ors = {.        
+00002d50: 2020 2020 2243 5722 3a20 7365 6c66 2e62      "CW": self.b
+00002d60: 616e 645f 696e 6469 6361 746f 7273 5f63  and_indicators_c
+00002d70: 772c 0a20 2020 2020 2020 2020 2020 2022  w,.            "
+00002d80: 5353 4222 3a20 7365 6c66 2e62 616e 645f  SSB": self.band_
+00002d90: 696e 6469 6361 746f 7273 5f73 7362 2c0a  indicators_ssb,.
+00002da0: 2020 2020 2020 2020 2020 2020 2252 5454              "RTT
+00002db0: 5922 3a20 7365 6c66 2e62 616e 645f 696e  Y": self.band_in
+00002dc0: 6469 6361 746f 7273 5f72 7474 792c 0a20  dicators_rtty,. 
+00002dd0: 2020 2020 2020 207d 0a0a 2020 2020 2020         }..      
+00002de0: 2020 6966 2073 656c 662e 7072 6566 2e67    if self.pref.g
+00002df0: 6574 2822 636f 6e74 6573 7422 293a 0a20  et("contest"):. 
+00002e00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00002e10: 6c6f 6164 5f63 6f6e 7465 7374 2829 0a0a  load_contest()..
+00002e20: 2020 2020 2020 2020 6966 2056 6572 7369          if Versi
+00002e30: 6f6e 5465 7374 285f 5f76 6572 7369 6f6e  onTest(__version
+00002e40: 5f5f 292e 7465 7374 2829 3a0a 2020 2020  __).test():.    
+00002e50: 2020 2020 2020 2020 7365 6c66 2e73 686f          self.sho
+00002e60: 775f 6d65 7373 6167 655f 626f 7828 0a20  w_message_box(. 
+00002e70: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00002e80: 5468 6572 6520 6973 2061 206e 6577 6572  There is a newer
+00002e90: 2076 6572 7369 6f6e 206f 6620 6e6f 7431   version of not1
+00002ea0: 6d6d 2061 7661 696c 6162 6c65 2e5c 6e22  mm available.\n"
+00002eb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002ec0: 2022 596f 7520 6361 6e20 7564 6174 6520   "You can udate 
+00002ed0: 746f 2074 6865 2063 7572 7265 6e74 2076  to the current v
+00002ee0: 6572 7369 6f6e 2062 7920 7573 696e 673a  ersion by using:
+00002ef0: 5c6e 7069 7020 696e 7374 616c 6c20 2d55  \npip install -U
+00002f00: 206e 6f74 316d 6d22 0a20 2020 2020 2020   not1mm".       
+00002f10: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+00002f20: 7365 6c66 2e63 6865 636b 5f66 6f72 5f6e  self.check_for_n
+00002f30: 6577 5f63 7479 2829 0a0a 2020 2020 4073  ew_cty()..    @s
+00002f40: 7461 7469 636d 6574 686f 640a 2020 2020  taticmethod.    
+00002f50: 6465 6620 6368 6563 6b5f 7072 6f63 6573  def check_proces
+00002f60: 7328 6e61 6d65 3a20 7374 7229 202d 3e20  s(name: str) -> 
+00002f70: 626f 6f6c 3a0a 2020 2020 2020 2020 2222  bool:.        ""
+00002f80: 2263 6865 636b 7320 746f 2073 6565 2069  "checks to see i
+00002f90: 6620 7072 6f67 7261 6d20 6f66 206e 616d  f program of nam
+00002fa0: 6520 6973 2069 6e20 7468 6520 6163 7469  e is in the acti
+00002fb0: 7665 2070 726f 6365 7373 206c 6973 7422  ve process list"
+00002fc0: 2222 0a20 2020 2020 2020 2066 6f72 2070  "".        for p
+00002fd0: 726f 6320 696e 2070 7375 7469 6c2e 7072  roc in psutil.pr
+00002fe0: 6f63 6573 735f 6974 6572 2829 3a0a 2020  ocess_iter():.  
+00002ff0: 2020 2020 2020 2020 2020 6966 2062 6f6f            if boo
+00003000: 6c28 7265 2e6d 6174 6368 286e 616d 652c  l(re.match(name,
+00003010: 2070 726f 632e 6e61 6d65 2829 2e6c 6f77   proc.name().low
+00003020: 6572 2829 2929 3a0a 2020 2020 2020 2020  er())):.        
+00003030: 2020 2020 2020 2020 7265 7475 726e 2054          return T
+00003040: 7275 650a 2020 2020 2020 2020 7265 7475  rue.        retu
+00003050: 726e 2046 616c 7365 0a0a 2020 2020 6465  rn False..    de
+00003060: 6620 7368 6f77 5f6d 6573 7361 6765 5f62  f show_message_b
+00003070: 6f78 2873 656c 662c 206d 6573 7361 6765  ox(self, message
+00003080: 3a20 7374 7229 202d 3e20 4e6f 6e65 3a0a  : str) -> None:.
+00003090: 2020 2020 2020 2020 2222 2264 6f63 2222          """doc""
+000030a0: 220a 2020 2020 2020 2020 6d65 7373 6167  ".        messag
+000030b0: 655f 626f 7820 3d20 5174 5769 6467 6574  e_box = QtWidget
+000030c0: 732e 514d 6573 7361 6765 426f 7828 290a  s.QMessageBox().
+000030d0: 2020 2020 2020 2020 6d65 7373 6167 655f          message_
+000030e0: 626f 782e 7365 7449 636f 6e28 5174 5769  box.setIcon(QtWi
+000030f0: 6467 6574 732e 514d 6573 7361 6765 426f  dgets.QMessageBo
+00003100: 782e 496e 666f 726d 6174 696f 6e29 0a20  x.Information). 
+00003110: 2020 2020 2020 206d 6573 7361 6765 5f62         message_b
+00003120: 6f78 2e73 6574 5465 7874 286d 6573 7361  ox.setText(messa
+00003130: 6765 290a 2020 2020 2020 2020 6d65 7373  ge).        mess
+00003140: 6167 655f 626f 782e 7365 7457 696e 646f  age_box.setWindo
+00003150: 7754 6974 6c65 2822 496e 666f 726d 6174  wTitle("Informat
+00003160: 696f 6e22 290a 2020 2020 2020 2020 6d65  ion").        me
+00003170: 7373 6167 655f 626f 782e 7365 7453 7461  ssage_box.setSta
+00003180: 6e64 6172 6442 7574 746f 6e73 2851 7457  ndardButtons(QtW
+00003190: 6964 6765 7473 2e51 4d65 7373 6167 6542  idgets.QMessageB
+000031a0: 6f78 2e4f 6b29 0a20 2020 2020 2020 205f  ox.Ok).        _
+000031b0: 203d 206d 6573 7361 6765 5f62 6f78 2e65   = message_box.e
+000031c0: 7865 635f 2829 0a0a 2020 2020 6465 6620  xec_()..    def 
+000031d0: 7368 6f77 5f61 626f 7574 5f64 6961 6c6f  show_about_dialo
+000031e0: 6728 7365 6c66 293a 0a20 2020 2020 2020  g(self):.       
+000031f0: 2022 2222 5368 6f77 2061 626f 7574 2064   """Show about d
+00003200: 6961 6c6f 6722 2222 0a20 2020 2020 2020  ialog""".       
+00003210: 2073 656c 662e 6162 6f75 745f 6469 616c   self.about_dial
+00003220: 6f67 203d 2041 626f 7574 2857 4f52 4b49  og = About(WORKI
+00003230: 4e47 5f50 4154 4829 0a20 2020 2020 2020  NG_PATH).       
+00003240: 2073 656c 662e 6162 6f75 745f 6469 616c   self.about_dial
+00003250: 6f67 2e64 6f6e 6f72 732e 7365 7453 6f75  og.donors.setSou
+00003260: 7263 6528 0a20 2020 2020 2020 2020 2020  rce(.           
+00003270: 2051 7443 6f72 652e 5155 726c 2e66 726f   QtCore.QUrl.fro
+00003280: 6d4c 6f63 616c 4669 6c65 2857 4f52 4b49  mLocalFile(WORKI
+00003290: 4e47 5f50 4154 4820 2b20 222f 6461 7461  NG_PATH + "/data
+000032a0: 2f64 6f6e 6f72 732e 6874 6d6c 2229 0a20  /donors.html"). 
+000032b0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
 000032c0: 2073 656c 662e 6162 6f75 745f 6469 616c   self.about_dial
-000032d0: 6f67 203d 2041 626f 7574 2857 4f52 4b49  og = About(WORKI
-000032e0: 4e47 5f50 4154 4829 0a20 2020 2020 2020  NG_PATH).       
-000032f0: 2069 6620 7365 6c66 2e70 7265 662e 6765   if self.pref.ge
-00003300: 7428 2264 6172 6b5f 6d6f 6465 2229 3a0a  t("dark_mode"):.
-00003310: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00003320: 2e61 626f 7574 5f64 6961 6c6f 672e 7365  .about_dialog.se
-00003330: 7453 7479 6c65 5368 6565 7428 4441 524b  tStyleSheet(DARK
-00003340: 5f53 5459 4c45 5348 4545 5429 0a20 2020  _STYLESHEET).   
-00003350: 2020 2020 2073 656c 662e 6162 6f75 745f       self.about_
-00003360: 6469 616c 6f67 2e6f 7065 6e28 290a 0a20  dialog.open().. 
-00003370: 2020 2064 6566 2065 6469 745f 636f 6e66     def edit_conf
-00003380: 6967 7572 6174 696f 6e5f 7365 7474 696e  iguration_settin
-00003390: 6773 2873 656c 6629 3a0a 2020 2020 2020  gs(self):.      
-000033a0: 2020 2222 2243 6f6e 6669 6775 7261 7469    """Configurati
-000033b0: 6f6e 2053 6574 7469 6e67 7320 7761 7320  on Settings was 
-000033c0: 636c 6963 6b65 6422 2222 0a20 2020 2020  clicked""".     
-000033d0: 2020 2073 656c 662e 636f 6e66 6967 7572     self.configur
-000033e0: 6174 696f 6e5f 6469 616c 6f67 203d 2053  ation_dialog = S
-000033f0: 6574 7469 6e67 7328 574f 524b 494e 475f  ettings(WORKING_
-00003400: 5041 5448 2c20 434f 4e46 4947 5f50 4154  PATH, CONFIG_PAT
-00003410: 482c 2073 656c 662e 7072 6566 290a 2020  H, self.pref).  
-00003420: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
-00003430: 6566 2e67 6574 2822 6461 726b 5f6d 6f64  ef.get("dark_mod
-00003440: 6522 293a 0a20 2020 2020 2020 2020 2020  e"):.           
-00003450: 2073 656c 662e 636f 6e66 6967 7572 6174   self.configurat
-00003460: 696f 6e5f 6469 616c 6f67 2e73 6574 5374  ion_dialog.setSt
-00003470: 796c 6553 6865 6574 2844 4152 4b5f 5354  yleSheet(DARK_ST
-00003480: 594c 4553 4845 4554 290a 2020 2020 2020  YLESHEET).      
-00003490: 2020 7365 6c66 2e63 6f6e 6669 6775 7261    self.configura
-000034a0: 7469 6f6e 5f64 6961 6c6f 672e 7573 6568  tion_dialog.useh
-000034b0: 616d 6462 5f72 6164 696f 4275 7474 6f6e  amdb_radioButton
-000034c0: 2e68 6964 6528 290a 2020 2020 2020 2020  .hide().        
-000034d0: 2320 7365 6c66 2e63 6f6e 6669 6775 7261  # self.configura
-000034e0: 7469 6f6e 5f64 6961 6c6f 672e 6e31 6d6d  tion_dialog.n1mm
-000034f0: 5f74 6162 2e68 6964 6528 290a 2020 2020  _tab.hide().    
-00003500: 2020 2020 7365 6c66 2e63 6f6e 6669 6775      self.configu
-00003510: 7261 7469 6f6e 5f64 6961 6c6f 672e 7368  ration_dialog.sh
-00003520: 6f77 2829 0a20 2020 2020 2020 2073 656c  ow().        sel
-00003530: 662e 636f 6e66 6967 7572 6174 696f 6e5f  f.configuration_
-00003540: 6469 616c 6f67 2e61 6363 6570 7465 642e  dialog.accepted.
-00003550: 636f 6e6e 6563 7428 7365 6c66 2e65 6469  connect(self.edi
-00003560: 745f 636f 6e66 6967 7572 6174 696f 6e5f  t_configuration_
-00003570: 7265 7475 726e 290a 0a20 2020 2064 6566  return)..    def
-00003580: 2065 6469 745f 636f 6e66 6967 7572 6174   edit_configurat
-00003590: 696f 6e5f 7265 7475 726e 2873 656c 6629  ion_return(self)
-000035a0: 3a0a 2020 2020 2020 2020 2222 2252 6574  :.        """Ret
-000035b0: 7572 6e73 2068 6572 6520 7768 656e 2063  urns here when c
-000035c0: 6f6e 6669 6775 7261 7469 6f6e 2064 6961  onfiguration dia
-000035d0: 6c6f 6720 636c 6f73 6564 2077 6974 6820  log closed with 
-000035e0: 6f6b 6179 2e22 2222 0a20 2020 2020 2020  okay.""".       
-000035f0: 2073 656c 662e 636f 6e66 6967 7572 6174   self.configurat
-00003600: 696f 6e5f 6469 616c 6f67 2e73 6176 655f  ion_dialog.save_
-00003610: 6368 616e 6765 7328 290a 2020 2020 2020  changes().      
-00003620: 2020 7365 6c66 2e77 7269 7465 5f70 7265    self.write_pre
-00003630: 6665 7265 6e63 6528 290a 2020 2020 2020  ference().      
-00003640: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
-00003650: 2573 222c 2066 227b 7365 6c66 2e70 7265  %s", f"{self.pre
-00003660: 667d 2229 0a20 2020 2020 2020 2073 656c  f}").        sel
-00003670: 662e 7265 6164 7072 6566 6572 656e 6365  f.readpreference
-00003680: 7328 290a 0a20 2020 2064 6566 206e 6577  s()..    def new
-00003690: 5f64 6174 6162 6173 6528 7365 6c66 293a  _database(self):
-000036a0: 0a20 2020 2020 2020 2022 2222 4372 6561  .        """Crea
-000036b0: 7465 206e 6577 2064 6174 6162 6173 652e  te new database.
-000036c0: 2222 220a 2020 2020 2020 2020 6669 6c65  """.        file
-000036d0: 6e61 6d65 203d 2073 656c 662e 6669 6c65  name = self.file
-000036e0: 7069 636b 6572 2822 6e65 7722 290a 2020  picker("new").  
-000036f0: 2020 2020 2020 6966 2066 696c 656e 616d        if filenam
-00003700: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
-00003710: 6620 6669 6c65 6e61 6d65 5b2d 333a 5d20  f filename[-3:] 
-00003720: 213d 2022 2e64 6222 3a0a 2020 2020 2020  != ".db":.      
-00003730: 2020 2020 2020 2020 2020 6669 6c65 6e61            filena
-00003740: 6d65 202b 3d20 222e 6462 220a 2020 2020  me += ".db".    
-00003750: 2020 2020 2020 2020 7365 6c66 2e70 7265          self.pre
-00003760: 665b 2263 7572 7265 6e74 5f64 6174 6162  f["current_datab
-00003770: 6173 6522 5d20 3d20 6669 6c65 6e61 6d65  ase"] = filename
-00003780: 2e73 706c 6974 2822 2f22 295b 2d31 3a5d  .split("/")[-1:]
-00003790: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
-000037a0: 7365 6c66 2e77 7269 7465 5f70 7265 6665  self.write_prefe
-000037b0: 7265 6e63 6528 290a 2020 2020 2020 2020  rence().        
-000037c0: 2020 2020 7365 6c66 2e64 626e 616d 6520      self.dbname 
-000037d0: 3d20 4441 5441 5f50 4154 4820 2b20 222f  = DATA_PATH + "/
-000037e0: 2220 2b20 7365 6c66 2e70 7265 662e 6765  " + self.pref.ge
-000037f0: 7428 2263 7572 7265 6e74 5f64 6174 6162  t("current_datab
-00003800: 6173 6522 2c20 2268 616d 2e64 6222 290a  ase", "ham.db").
-00003810: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00003820: 2e64 6174 6162 6173 6520 3d20 4461 7461  .database = Data
-00003830: 4261 7365 2873 656c 662e 6462 6e61 6d65  Base(self.dbname
-00003840: 2c20 574f 524b 494e 475f 5041 5448 290a  , WORKING_PATH).
-00003850: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00003860: 2e63 6f6e 7461 6374 203d 2073 656c 662e  .contact = self.
-00003870: 6461 7461 6261 7365 2e65 6d70 7479 5f63  database.empty_c
-00003880: 6f6e 7461 6374 0a20 2020 2020 2020 2020  ontact.         
-00003890: 2020 2073 656c 662e 7374 6174 696f 6e20     self.station 
-000038a0: 3d20 7365 6c66 2e64 6174 6162 6173 652e  = self.database.
-000038b0: 6665 7463 685f 7374 6174 696f 6e28 290a  fetch_station().
-000038c0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-000038d0: 656c 662e 7374 6174 696f 6e20 6973 204e  elf.station is N
-000038e0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000038f0: 2020 2020 2073 656c 662e 7374 6174 696f       self.statio
-00003900: 6e20 3d20 7b7d 0a20 2020 2020 2020 2020  n = {}.         
-00003910: 2020 2073 656c 662e 6375 7272 656e 745f     self.current_
-00003920: 6f70 203d 2073 656c 662e 7374 6174 696f  op = self.statio
-00003930: 6e2e 6765 7428 2243 616c 6c22 2c20 2222  n.get("Call", ""
-00003940: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00003950: 6c66 2e6d 616b 655f 6f70 5f64 6972 2829  lf.make_op_dir()
-00003960: 0a20 2020 2020 2020 2020 2020 2063 6d64  .            cmd
-00003970: 203d 207b 7d0a 2020 2020 2020 2020 2020   = {}.          
-00003980: 2020 636d 645b 2263 6d64 225d 203d 2022    cmd["cmd"] = "
-00003990: 4e45 5744 4222 0a20 2020 2020 2020 2020  NEWDB".         
-000039a0: 2020 2063 6d64 5b22 7374 6174 696f 6e22     cmd["station"
-000039b0: 5d20 3d20 706c 6174 666f 726d 2e6e 6f64  ] = platform.nod
-000039c0: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
-000039d0: 7365 6c66 2e6d 756c 7469 6361 7374 5f69  self.multicast_i
-000039e0: 6e74 6572 6661 6365 2e73 656e 645f 6173  nterface.send_as
-000039f0: 5f6a 736f 6e28 636d 6429 0a20 2020 2020  _json(cmd).     
-00003a00: 2020 2020 2020 2073 656c 662e 636c 6561         self.clea
-00003a10: 7269 6e70 7574 7328 290a 2020 2020 2020  rinputs().      
-00003a20: 2020 2020 2020 7365 6c66 2e65 6469 745f        self.edit_
-00003a30: 7374 6174 696f 6e5f 7365 7474 696e 6773  station_settings
-00003a40: 2829 0a0a 2020 2020 6465 6620 6f70 656e  ()..    def open
-00003a50: 5f64 6174 6162 6173 6528 7365 6c66 293a  _database(self):
-00003a60: 0a20 2020 2020 2020 2022 2222 4f70 656e  .        """Open
-00003a70: 2065 7869 7374 696e 6720 6461 7461 6261   existing databa
-00003a80: 7365 2e22 2222 0a20 2020 2020 2020 2066  se.""".        f
-00003a90: 696c 656e 616d 6520 3d20 7365 6c66 2e66  ilename = self.f
-00003aa0: 696c 6570 6963 6b65 7228 226f 7065 6e22  ilepicker("open"
-00003ab0: 290a 2020 2020 2020 2020 6966 2066 696c  ).        if fil
-00003ac0: 656e 616d 653a 0a20 2020 2020 2020 2020  ename:.         
-00003ad0: 2020 2073 656c 662e 7072 6566 5b22 6375     self.pref["cu
-00003ae0: 7272 656e 745f 6461 7461 6261 7365 225d  rrent_database"]
-00003af0: 203d 2066 696c 656e 616d 652e 7370 6c69   = filename.spli
-00003b00: 7428 222f 2229 5b2d 313a 5d5b 305d 0a20  t("/")[-1:][0]. 
-00003b10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00003b20: 7772 6974 655f 7072 6566 6572 656e 6365  write_preference
-00003b30: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
-00003b40: 656c 662e 6462 6e61 6d65 203d 2044 4154  elf.dbname = DAT
-00003b50: 415f 5041 5448 202b 2022 2f22 202b 2073  A_PATH + "/" + s
-00003b60: 656c 662e 7072 6566 2e67 6574 2822 6375  elf.pref.get("cu
-00003b70: 7272 656e 745f 6461 7461 6261 7365 222c  rrent_database",
-00003b80: 2022 6861 6d2e 6462 2229 0a20 2020 2020   "ham.db").     
-00003b90: 2020 2020 2020 2073 656c 662e 6461 7461         self.data
-00003ba0: 6261 7365 203d 2044 6174 6142 6173 6528  base = DataBase(
-00003bb0: 7365 6c66 2e64 626e 616d 652c 2057 4f52  self.dbname, WOR
-00003bc0: 4b49 4e47 5f50 4154 4829 0a20 2020 2020  KING_PATH).     
-00003bd0: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
-00003be0: 6163 7420 3d20 7365 6c66 2e64 6174 6162  act = self.datab
-00003bf0: 6173 652e 656d 7074 795f 636f 6e74 6163  ase.empty_contac
-00003c00: 740a 2020 2020 2020 2020 2020 2020 7365  t.            se
-00003c10: 6c66 2e73 7461 7469 6f6e 203d 2073 656c  lf.station = sel
-00003c20: 662e 6461 7461 6261 7365 2e66 6574 6368  f.database.fetch
-00003c30: 5f73 7461 7469 6f6e 2829 0a20 2020 2020  _station().     
-00003c40: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-00003c50: 7461 7469 6f6e 2069 7320 4e6f 6e65 3a0a  tation is None:.
-00003c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c70: 7365 6c66 2e73 7461 7469 6f6e 203d 207b  self.station = {
-00003c80: 7d0a 2020 2020 2020 2020 2020 2020 6966  }.            if
-00003c90: 2073 656c 662e 7374 6174 696f 6e2e 6765   self.station.ge
-00003ca0: 7428 2243 616c 6c22 2c20 2222 2920 3d3d  t("Call", "") ==
-00003cb0: 2022 223a 0a20 2020 2020 2020 2020 2020   "":.           
-00003cc0: 2020 2020 2073 656c 662e 6564 6974 5f73       self.edit_s
-00003cd0: 7461 7469 6f6e 5f73 6574 7469 6e67 7328  tation_settings(
-00003ce0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00003cf0: 6c66 2e63 7572 7265 6e74 5f6f 7020 3d20  lf.current_op = 
-00003d00: 7365 6c66 2e73 7461 7469 6f6e 2e67 6574  self.station.get
-00003d10: 2822 4361 6c6c 222c 2022 2229 0a20 2020  ("Call", "").   
-00003d20: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
-00003d30: 6b65 5f6f 705f 6469 7228 290a 2020 2020  ke_op_dir().    
-00003d40: 2020 2020 2020 2020 636d 6420 3d20 7b7d          cmd = {}
-00003d50: 0a20 2020 2020 2020 2020 2020 2063 6d64  .            cmd
-00003d60: 5b22 636d 6422 5d20 3d20 224e 4557 4442  ["cmd"] = "NEWDB
-00003d70: 220a 2020 2020 2020 2020 2020 2020 636d  ".            cm
-00003d80: 645b 2273 7461 7469 6f6e 225d 203d 2070  d["station"] = p
-00003d90: 6c61 7466 6f72 6d2e 6e6f 6465 2829 0a20  latform.node(). 
-00003da0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00003db0: 6d75 6c74 6963 6173 745f 696e 7465 7266  multicast_interf
-00003dc0: 6163 652e 7365 6e64 5f61 735f 6a73 6f6e  ace.send_as_json
-00003dd0: 2863 6d64 290a 2020 2020 2020 2020 2020  (cmd).          
-00003de0: 2020 7365 6c66 2e63 6c65 6172 696e 7075    self.clearinpu
-00003df0: 7473 2829 0a0a 2020 2020 6465 6620 6e65  ts()..    def ne
-00003e00: 775f 636f 6e74 6573 7428 7365 6c66 293a  w_contest(self):
-00003e10: 0a20 2020 2020 2020 2022 2222 4372 6561  .        """Crea
-00003e20: 7465 206e 6577 2063 6f6e 7465 7374 2069  te new contest i
-00003e30: 6e20 6578 6973 7469 6e67 2064 6174 6162  n existing datab
-00003e40: 6173 652e 2222 220a 0a20 2020 2064 6566  ase."""..    def
-00003e50: 206f 7065 6e5f 636f 6e74 6573 7428 7365   open_contest(se
-00003e60: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00003e70: 5377 6974 6368 2074 6f20 6120 6469 6666  Switch to a diff
-00003e80: 6572 656e 7420 6578 6973 7469 6e67 2063  erent existing c
-00003e90: 6f6e 7465 7374 2069 6e20 6578 6973 7469  ontest in existi
-00003ea0: 6e67 2064 6174 6162 6173 652e 2222 220a  ng database.""".
-00003eb0: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-00003ec0: 6562 7567 2822 4f70 656e 2043 6f6e 7465  ebug("Open Conte
-00003ed0: 7374 2073 656c 6563 7465 6422 290a 2020  st selected").  
-00003ee0: 2020 2020 2020 636f 6e74 6573 7473 203d        contests =
-00003ef0: 2073 656c 662e 6461 7461 6261 7365 2e66   self.database.f
-00003f00: 6574 6368 5f61 6c6c 5f63 6f6e 7465 7374  etch_all_contest
-00003f10: 7328 290a 2020 2020 2020 2020 6c6f 6767  s().        logg
-00003f20: 6572 2e64 6562 7567 2822 2573 222c 2066  er.debug("%s", f
-00003f30: 227b 636f 6e74 6573 7473 7d22 290a 0a20  "{contests}").. 
-00003f40: 2020 2020 2020 2069 6620 636f 6e74 6573         if contes
-00003f50: 7473 3a0a 2020 2020 2020 2020 2020 2020  ts:.            
-00003f60: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
-00003f70: 6c6f 6720 3d20 5365 6c65 6374 436f 6e74  log = SelectCont
-00003f80: 6573 7428 574f 524b 494e 475f 5041 5448  est(WORKING_PATH
-00003f90: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-00003fa0: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
-00003fb0: 6461 726b 5f6d 6f64 6522 293a 0a20 2020  dark_mode"):.   
-00003fc0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00003fd0: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
-00003fe0: 2e73 6574 5374 796c 6553 6865 6574 2844  .setStyleSheet(D
-00003ff0: 4152 4b5f 5354 594c 4553 4845 4554 290a  ARK_STYLESHEET).
-00004000: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00004010: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
-00004020: 636f 6e74 6573 745f 6c69 7374 2e73 6574  contest_list.set
-00004030: 526f 7743 6f75 6e74 2830 290a 2020 2020  RowCount(0).    
-00004040: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-00004050: 7465 7374 5f64 6961 6c6f 672e 636f 6e74  test_dialog.cont
-00004060: 6573 745f 6c69 7374 2e73 6574 436f 6c75  est_list.setColu
-00004070: 6d6e 436f 756e 7428 3429 0a20 2020 2020  mnCount(4).     
-00004080: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
-00004090: 6573 745f 6469 616c 6f67 2e63 6f6e 7465  est_dialog.conte
-000040a0: 7374 5f6c 6973 742e 7665 7274 6963 616c  st_list.vertical
-000040b0: 4865 6164 6572 2829 2e73 6574 5669 7369  Header().setVisi
-000040c0: 626c 6528 4661 6c73 6529 0a20 2020 2020  ble(False).     
-000040d0: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
-000040e0: 6573 745f 6469 616c 6f67 2e63 6f6e 7465  est_dialog.conte
-000040f0: 7374 5f6c 6973 742e 7365 7443 6f6c 756d  st_list.setColum
-00004100: 6e57 6964 7468 2831 2c20 3230 3029 0a20  nWidth(1, 200). 
-00004110: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00004120: 636f 6e74 6573 745f 6469 616c 6f67 2e63  contest_dialog.c
-00004130: 6f6e 7465 7374 5f6c 6973 742e 7365 7443  ontest_list.setC
-00004140: 6f6c 756d 6e57 6964 7468 2832 2c20 3230  olumnWidth(2, 20
-00004150: 3029 0a20 2020 2020 2020 2020 2020 2073  0).            s
-00004160: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-00004170: 6f67 2e63 6f6e 7465 7374 5f6c 6973 742e  og.contest_list.
-00004180: 7365 7448 6f72 697a 6f6e 7461 6c48 6561  setHorizontalHea
-00004190: 6465 7249 7465 6d28 0a20 2020 2020 2020  derItem(.       
-000041a0: 2020 2020 2020 2020 2030 2c20 5174 5769           0, QtWi
-000041b0: 6467 6574 732e 5154 6162 6c65 5769 6467  dgets.QTableWidg
-000041c0: 6574 4974 656d 2822 436f 6e74 6573 7420  etItem("Contest 
-000041d0: 4e72 2229 0a20 2020 2020 2020 2020 2020  Nr").           
-000041e0: 2029 0a20 2020 2020 2020 2020 2020 2073   ).            s
-000041f0: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-00004200: 6f67 2e63 6f6e 7465 7374 5f6c 6973 742e  og.contest_list.
-00004210: 7365 7448 6f72 697a 6f6e 7461 6c48 6561  setHorizontalHea
-00004220: 6465 7249 7465 6d28 0a20 2020 2020 2020  derItem(.       
-00004230: 2020 2020 2020 2020 2031 2c20 5174 5769           1, QtWi
-00004240: 6467 6574 732e 5154 6162 6c65 5769 6467  dgets.QTableWidg
-00004250: 6574 4974 656d 2822 436f 6e74 6573 7420  etItem("Contest 
-00004260: 4e61 6d65 2229 0a20 2020 2020 2020 2020  Name").         
-00004270: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00004280: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
-00004290: 616c 6f67 2e63 6f6e 7465 7374 5f6c 6973  alog.contest_lis
-000042a0: 742e 7365 7448 6f72 697a 6f6e 7461 6c48  t.setHorizontalH
-000042b0: 6561 6465 7249 7465 6d28 0a20 2020 2020  eaderItem(.     
-000042c0: 2020 2020 2020 2020 2020 2032 2c20 5174             2, Qt
-000042d0: 5769 6467 6574 732e 5154 6162 6c65 5769  Widgets.QTableWi
-000042e0: 6467 6574 4974 656d 2822 436f 6e74 6573  dgetItem("Contes
-000042f0: 7420 5374 6172 7422 290a 2020 2020 2020  t Start").      
-00004300: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00004310: 2020 2020 7365 6c66 2e63 6f6e 7465 7374      self.contest
-00004320: 5f64 6961 6c6f 672e 636f 6e74 6573 745f  _dialog.contest_
-00004330: 6c69 7374 2e73 6574 486f 7269 7a6f 6e74  list.setHorizont
-00004340: 616c 4865 6164 6572 4974 656d 280a 2020  alHeaderItem(.  
-00004350: 2020 2020 2020 2020 2020 2020 2020 332c                3,
-00004360: 2051 7457 6964 6765 7473 2e51 5461 626c   QtWidgets.QTabl
-00004370: 6557 6964 6765 7449 7465 6d28 224e 6f74  eWidgetItem("Not
-00004380: 2055 4973 6564 2229 0a20 2020 2020 2020   UIsed").       
-00004390: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-000043a0: 2020 2073 656c 662e 636f 6e74 6573 745f     self.contest_
-000043b0: 6469 616c 6f67 2e63 6f6e 7465 7374 5f6c  dialog.contest_l
-000043c0: 6973 742e 7365 7443 6f6c 756d 6e48 6964  ist.setColumnHid
-000043d0: 6465 6e28 302c 2054 7275 6529 0a20 2020  den(0, True).   
-000043e0: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
-000043f0: 6e74 6573 745f 6469 616c 6f67 2e63 6f6e  ntest_dialog.con
-00004400: 7465 7374 5f6c 6973 742e 7365 7443 6f6c  test_list.setCol
-00004410: 756d 6e48 6964 6465 6e28 332c 2054 7275  umnHidden(3, Tru
-00004420: 6529 0a20 2020 2020 2020 2020 2020 2073  e).            s
-00004430: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-00004440: 6f67 2e61 6363 6570 7465 642e 636f 6e6e  og.accepted.conn
-00004450: 6563 7428 7365 6c66 2e6f 7065 6e5f 636f  ect(self.open_co
-00004460: 6e74 6573 745f 7265 7475 726e 290a 2020  ntest_return).  
-00004470: 2020 2020 2020 2020 2020 666f 7220 636f            for co
-00004480: 6e74 6573 7420 696e 2063 6f6e 7465 7374  ntest in contest
-00004490: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-000044a0: 2020 206e 756d 6265 725f 6f66 5f72 6f77     number_of_row
-000044b0: 7320 3d20 7365 6c66 2e63 6f6e 7465 7374  s = self.contest
-000044c0: 5f64 6961 6c6f 672e 636f 6e74 6573 745f  _dialog.contest_
-000044d0: 6c69 7374 2e72 6f77 436f 756e 7428 290a  list.rowCount().
-000044e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000044f0: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
-00004500: 6c6f 672e 636f 6e74 6573 745f 6c69 7374  log.contest_list
-00004510: 2e69 6e73 6572 7452 6f77 286e 756d 6265  .insertRow(numbe
-00004520: 725f 6f66 5f72 6f77 7329 0a20 2020 2020  r_of_rows).     
-00004530: 2020 2020 2020 2020 2020 2063 6f6e 7465             conte
-00004540: 7374 5f69 6420 3d20 7374 7228 636f 6e74  st_id = str(cont
-00004550: 6573 742e 6765 7428 2243 6f6e 7465 7374  est.get("Contest
-00004560: 4944 222c 2031 2929 0a20 2020 2020 2020  ID", 1)).       
-00004570: 2020 2020 2020 2020 2063 6f6e 7465 7374           contest
-00004580: 5f6e 616d 6520 3d20 636f 6e74 6573 742e  _name = contest.
-00004590: 6765 7428 2243 6f6e 7465 7374 4e61 6d65  get("ContestName
-000045a0: 222c 2031 290a 2020 2020 2020 2020 2020  ", 1).          
-000045b0: 2020 2020 2020 7374 6172 745f 6461 7465        start_date
-000045c0: 203d 2063 6f6e 7465 7374 2e67 6574 2822   = contest.get("
-000045d0: 5374 6172 7444 6174 6522 2c20 3129 0a20  StartDate", 1). 
-000045e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000045f0: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-00004600: 6f67 2e63 6f6e 7465 7374 5f6c 6973 742e  og.contest_list.
-00004610: 7365 7449 7465 6d28 0a20 2020 2020 2020  setItem(.       
-00004620: 2020 2020 2020 2020 2020 2020 206e 756d               num
-00004630: 6265 725f 6f66 5f72 6f77 732c 2030 2c20  ber_of_rows, 0, 
-00004640: 5174 5769 6467 6574 732e 5154 6162 6c65  QtWidgets.QTable
-00004650: 5769 6467 6574 4974 656d 2863 6f6e 7465  WidgetItem(conte
-00004660: 7374 5f69 6429 0a20 2020 2020 2020 2020  st_id).         
-00004670: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00004680: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
-00004690: 6e74 6573 745f 6469 616c 6f67 2e63 6f6e  ntest_dialog.con
-000046a0: 7465 7374 5f6c 6973 742e 7365 7449 7465  test_list.setIte
-000046b0: 6d28 0a20 2020 2020 2020 2020 2020 2020  m(.             
-000046c0: 2020 2020 2020 206e 756d 6265 725f 6f66         number_of
-000046d0: 5f72 6f77 732c 2031 2c20 5174 5769 6467  _rows, 1, QtWidg
-000046e0: 6574 732e 5154 6162 6c65 5769 6467 6574  ets.QTableWidget
-000046f0: 4974 656d 2863 6f6e 7465 7374 5f6e 616d  Item(contest_nam
-00004700: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
-00004710: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00004720: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
-00004730: 745f 6469 616c 6f67 2e63 6f6e 7465 7374  t_dialog.contest
-00004740: 5f6c 6973 742e 7365 7449 7465 6d28 0a20  _list.setItem(. 
-00004750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004760: 2020 206e 756d 6265 725f 6f66 5f72 6f77     number_of_row
-00004770: 732c 2032 2c20 5174 5769 6467 6574 732e  s, 2, QtWidgets.
-00004780: 5154 6162 6c65 5769 6467 6574 4974 656d  QTableWidgetItem
-00004790: 2873 7461 7274 5f64 6174 6529 0a20 2020  (start_date).   
-000047a0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-000047b0: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
-000047c0: 6573 745f 6469 616c 6f67 2e73 686f 7728  est_dialog.show(
-000047d0: 290a 0a20 2020 2064 6566 206f 7065 6e5f  )..    def open_
-000047e0: 636f 6e74 6573 745f 7265 7475 726e 2873  contest_return(s
-000047f0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-00004800: 2243 616c 6c65 6420 6279 206f 7065 6e5f  "Called by open_
-00004810: 636f 6e74 6573 7422 2222 0a20 2020 2020  contest""".     
-00004820: 2020 2073 656c 6563 7465 645f 726f 7720     selected_row 
-00004830: 3d20 7365 6c66 2e63 6f6e 7465 7374 5f64  = self.contest_d
-00004840: 6961 6c6f 672e 636f 6e74 6573 745f 6c69  ialog.contest_li
-00004850: 7374 2e63 7572 7265 6e74 526f 7728 290a  st.currentRow().
-00004860: 2020 2020 2020 2020 636f 6e74 6573 7420          contest 
-00004870: 3d20 7365 6c66 2e63 6f6e 7465 7374 5f64  = self.contest_d
-00004880: 6961 6c6f 672e 636f 6e74 6573 745f 6c69  ialog.contest_li
-00004890: 7374 2e69 7465 6d28 7365 6c65 6374 6564  st.item(selected
-000048a0: 5f72 6f77 2c20 3029 2e74 6578 7428 290a  _row, 0).text().
-000048b0: 2020 2020 2020 2020 7365 6c66 2e70 7265          self.pre
-000048c0: 665b 2263 6f6e 7465 7374 225d 203d 2063  f["contest"] = c
-000048d0: 6f6e 7465 7374 0a20 2020 2020 2020 2073  ontest.        s
-000048e0: 656c 662e 7772 6974 655f 7072 6566 6572  elf.write_prefer
-000048f0: 656e 6365 2829 0a20 2020 2020 2020 206c  ence().        l
-00004900: 6f67 6765 722e 6465 6275 6728 2253 656c  ogger.debug("Sel
-00004910: 6563 7465 6420 636f 6e74 6573 743a 2025  ected contest: %
-00004920: 7322 2c20 6622 7b63 6f6e 7465 7374 7d22  s", f"{contest}"
-00004930: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
-00004940: 6f61 645f 636f 6e74 6573 7428 290a 0a20  oad_contest().. 
-00004950: 2020 2064 6566 2072 6566 696c 6c5f 6472     def refill_dr
-00004960: 6f70 646f 776e 2873 656c 662c 2074 6172  opdown(self, tar
-00004970: 6765 742c 2073 6f75 7263 6529 3a0a 2020  get, source):.  
-00004980: 2020 2020 2020 2222 2252 6566 696c 6c20        """Refill 
-00004990: 5143 6f6d 626f 626f 7820 7769 6467 6574  QCombobox widget
-000049a0: 2077 6974 6820 7661 6c75 652e 2222 220a   with value.""".
-000049b0: 2020 2020 2020 2020 696e 6465 7820 3d20          index = 
-000049c0: 7461 7267 6574 2e66 696e 6454 6578 7428  target.findText(
-000049d0: 736f 7572 6365 290a 2020 2020 2020 2020  source).        
-000049e0: 7461 7267 6574 2e73 6574 4375 7272 656e  target.setCurren
-000049f0: 7449 6e64 6578 2869 6e64 6578 290a 0a20  tIndex(index).. 
-00004a00: 2020 2064 6566 2065 6469 745f 636f 6e74     def edit_cont
-00004a10: 6573 7428 7365 6c66 293a 0a20 2020 2020  est(self):.     
-00004a20: 2020 2022 2222 4564 6974 2074 6865 2063     """Edit the c
-00004a30: 7572 7265 6e74 2063 6f6e 7465 7374 2222  urrent contest""
-00004a40: 220a 2020 2020 2020 2020 6c6f 6767 6572  ".        logger
-00004a50: 2e64 6562 7567 2822 4564 6974 2063 6f6e  .debug("Edit con
-00004a60: 7465 7374 2044 6961 6c6f 6722 290a 2020  test Dialog").  
-00004a70: 2020 2020 2020 6966 2073 656c 662e 636f        if self.co
-00004a80: 6e74 6573 745f 7365 7474 696e 6773 2069  ntest_settings i
-00004a90: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00004aa0: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-00004ab0: 2020 2073 656c 662e 636f 6e74 6573 745f     self.contest_
-00004ac0: 6469 616c 6f67 203d 204e 6577 436f 6e74  dialog = NewCont
-00004ad0: 6573 7428 574f 524b 494e 475f 5041 5448  est(WORKING_PATH
-00004ae0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-00004af0: 662e 7072 6566 2e67 6574 2822 6461 726b  f.pref.get("dark
-00004b00: 5f6d 6f64 6522 293a 0a20 2020 2020 2020  _mode"):.       
-00004b10: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
-00004b20: 745f 6469 616c 6f67 2e73 6574 5374 796c  t_dialog.setStyl
-00004b30: 6553 6865 6574 2844 4152 4b5f 5354 594c  eSheet(DARK_STYL
-00004b40: 4553 4845 4554 290a 2020 2020 2020 2020  ESHEET).        
-00004b50: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
-00004b60: 6c6f 672e 7365 7457 696e 646f 7754 6974  log.setWindowTit
-00004b70: 6c65 2822 4564 6974 2043 6f6e 7465 7374  le("Edit Contest
-00004b80: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00004b90: 636f 6e74 6573 745f 6469 616c 6f67 2e74  contest_dialog.t
-00004ba0: 6974 6c65 2e73 6574 5465 7874 2822 2229  itle.setText("")
-00004bb0: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
-00004bc0: 6e74 6573 745f 6469 616c 6f67 2e61 6363  ntest_dialog.acc
-00004bd0: 6570 7465 642e 636f 6e6e 6563 7428 7365  epted.connect(se
-00004be0: 6c66 2e73 6176 655f 6564 6974 6564 5f63  lf.save_edited_c
-00004bf0: 6f6e 7465 7374 290a 2020 2020 2020 2020  ontest).        
-00004c00: 6966 2073 656c 662e 7072 6566 2e67 6574  if self.pref.get
-00004c10: 2822 6461 726b 5f6d 6f64 6522 293a 0a20  ("dark_mode"):. 
-00004c20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00004c30: 636f 6e74 6573 745f 6469 616c 6f67 2e73  contest_dialog.s
-00004c40: 6574 5374 796c 6553 6865 6574 2844 4152  etStyleSheet(DAR
-00004c50: 4b5f 5354 594c 4553 4845 4554 290a 0a20  K_STYLESHEET).. 
-00004c60: 2020 2020 2020 2076 616c 7565 203d 2073         value = s
-00004c70: 656c 662e 636f 6e74 6573 745f 7365 7474  elf.contest_sett
-00004c80: 696e 6773 2e67 6574 2822 436f 6e74 6573  ings.get("Contes
-00004c90: 744e 616d 6522 292e 7570 7065 7228 292e  tName").upper().
-00004ca0: 7265 706c 6163 6528 225f 222c 2022 2022  replace("_", " "
-00004cb0: 290a 2020 2020 2020 2020 6966 2076 616c  ).        if val
-00004cc0: 7565 203d 3d20 2247 454e 4552 414c 204c  ue == "GENERAL L
-00004cd0: 4f47 4749 4e47 223a 0a20 2020 2020 2020  OGGING":.       
-00004ce0: 2020 2020 2076 616c 7565 203d 2022 4765       value = "Ge
-00004cf0: 6e65 7261 6c20 4c6f 6767 696e 6722 0a20  neral Logging". 
-00004d00: 2020 2020 2020 2073 656c 662e 7265 6669         self.refi
-00004d10: 6c6c 5f64 726f 7064 6f77 6e28 7365 6c66  ll_dropdown(self
-00004d20: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
-00004d30: 636f 6e74 6573 742c 2076 616c 7565 290a  contest, value).
-00004d40: 2020 2020 2020 2020 7661 6c75 6520 3d20          value = 
-00004d50: 7365 6c66 2e63 6f6e 7465 7374 5f73 6574  self.contest_set
-00004d60: 7469 6e67 732e 6765 7428 224f 7065 7261  tings.get("Opera
-00004d70: 746f 7243 6174 6567 6f72 7922 290a 2020  torCategory").  
-00004d80: 2020 2020 2020 7365 6c66 2e72 6566 696c        self.refil
-00004d90: 6c5f 6472 6f70 646f 776e 2873 656c 662e  l_dropdown(self.
-00004da0: 636f 6e74 6573 745f 6469 616c 6f67 2e6f  contest_dialog.o
-00004db0: 7065 7261 746f 725f 636c 6173 732c 2076  perator_class, v
-00004dc0: 616c 7565 290a 2020 2020 2020 2020 7661  alue).        va
-00004dd0: 6c75 6520 3d20 7365 6c66 2e63 6f6e 7465  lue = self.conte
-00004de0: 7374 5f73 6574 7469 6e67 732e 6765 7428  st_settings.get(
-00004df0: 2242 616e 6443 6174 6567 6f72 7922 290a  "BandCategory").
-00004e00: 2020 2020 2020 2020 7365 6c66 2e72 6566          self.ref
-00004e10: 696c 6c5f 6472 6f70 646f 776e 2873 656c  ill_dropdown(sel
-00004e20: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
-00004e30: 2e62 616e 642c 2076 616c 7565 290a 2020  .band, value).  
-00004e40: 2020 2020 2020 7661 6c75 6520 3d20 7365        value = se
-00004e50: 6c66 2e63 6f6e 7465 7374 5f73 6574 7469  lf.contest_setti
-00004e60: 6e67 732e 6765 7428 2250 6f77 6572 4361  ngs.get("PowerCa
-00004e70: 7465 676f 7279 2229 0a20 2020 2020 2020  tegory").       
-00004e80: 2073 656c 662e 7265 6669 6c6c 5f64 726f   self.refill_dro
-00004e90: 7064 6f77 6e28 7365 6c66 2e63 6f6e 7465  pdown(self.conte
-00004ea0: 7374 5f64 6961 6c6f 672e 706f 7765 722c  st_dialog.power,
-00004eb0: 2076 616c 7565 290a 2020 2020 2020 2020   value).        
-00004ec0: 7661 6c75 6520 3d20 7365 6c66 2e63 6f6e  value = self.con
-00004ed0: 7465 7374 5f73 6574 7469 6e67 732e 6765  test_settings.ge
-00004ee0: 7428 224d 6f64 6543 6174 6567 6f72 7922  t("ModeCategory"
-00004ef0: 290a 2020 2020 2020 2020 7365 6c66 2e72  ).        self.r
-00004f00: 6566 696c 6c5f 6472 6f70 646f 776e 2873  efill_dropdown(s
-00004f10: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-00004f20: 6f67 2e6d 6f64 652c 2076 616c 7565 290a  og.mode, value).
-00004f30: 2020 2020 2020 2020 7661 6c75 6520 3d20          value = 
-00004f40: 7365 6c66 2e63 6f6e 7465 7374 5f73 6574  self.contest_set
-00004f50: 7469 6e67 732e 6765 7428 224f 7665 726c  tings.get("Overl
-00004f60: 6179 4361 7465 676f 7279 2229 0a20 2020  ayCategory").   
-00004f70: 2020 2020 2073 656c 662e 7265 6669 6c6c       self.refill
-00004f80: 5f64 726f 7064 6f77 6e28 7365 6c66 2e63  _dropdown(self.c
-00004f90: 6f6e 7465 7374 5f64 6961 6c6f 672e 6f76  ontest_dialog.ov
-00004fa0: 6572 6c61 792c 2076 616c 7565 290a 2020  erlay, value).  
-00004fb0: 2020 2020 2020 7365 6c66 2e63 6f6e 7465        self.conte
-00004fc0: 7374 5f64 6961 6c6f 672e 6f70 6572 6174  st_dialog.operat
-00004fd0: 6f72 732e 7365 7454 6578 7428 7365 6c66  ors.setText(self
-00004fe0: 2e63 6f6e 7465 7374 5f73 6574 7469 6e67  .contest_setting
-00004ff0: 732e 6765 7428 224f 7065 7261 746f 7273  s.get("Operators
-00005000: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
-00005010: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
-00005020: 736f 6170 626f 782e 7365 7450 6c61 696e  soapbox.setPlain
-00005030: 5465 7874 2873 656c 662e 636f 6e74 6573  Text(self.contes
-00005040: 745f 7365 7474 696e 6773 2e67 6574 2822  t_settings.get("
-00005050: 536f 6170 626f 7822 2929 0a20 2020 2020  Soapbox")).     
-00005060: 2020 2073 656c 662e 636f 6e74 6573 745f     self.contest_
-00005070: 6469 616c 6f67 2e65 7863 6861 6e67 652e  dialog.exchange.
-00005080: 7365 7454 6578 7428 7365 6c66 2e63 6f6e  setText(self.con
-00005090: 7465 7374 5f73 6574 7469 6e67 732e 6765  test_settings.ge
-000050a0: 7428 2253 656e 7445 7863 6861 6e67 6522  t("SentExchange"
-000050b0: 2929 0a20 2020 2020 2020 2076 616c 7565  )).        value
-000050c0: 203d 2073 656c 662e 636f 6e74 6573 745f   = self.contest_
-000050d0: 7365 7474 696e 6773 2e67 6574 2822 5374  settings.get("St
-000050e0: 6174 696f 6e43 6174 6567 6f72 7922 290a  ationCategory").
-000050f0: 2020 2020 2020 2020 7365 6c66 2e72 6566          self.ref
-00005100: 696c 6c5f 6472 6f70 646f 776e 2873 656c  ill_dropdown(sel
-00005110: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
-00005120: 2e73 7461 7469 6f6e 2c20 7661 6c75 6529  .station, value)
-00005130: 0a20 2020 2020 2020 2076 616c 7565 203d  .        value =
-00005140: 2073 656c 662e 636f 6e74 6573 745f 7365   self.contest_se
-00005150: 7474 696e 6773 2e67 6574 2822 4173 7369  ttings.get("Assi
-00005160: 7374 6564 4361 7465 676f 7279 2229 0a20  stedCategory"). 
-00005170: 2020 2020 2020 2073 656c 662e 7265 6669         self.refi
-00005180: 6c6c 5f64 726f 7064 6f77 6e28 7365 6c66  ll_dropdown(self
-00005190: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
-000051a0: 6173 7369 7374 6564 2c20 7661 6c75 6529  assisted, value)
-000051b0: 0a20 2020 2020 2020 2076 616c 7565 203d  .        value =
-000051c0: 2073 656c 662e 636f 6e74 6573 745f 7365   self.contest_se
-000051d0: 7474 696e 6773 2e67 6574 2822 5472 616e  ttings.get("Tran
-000051e0: 736d 6974 7465 7243 6174 6567 6f72 7922  smitterCategory"
-000051f0: 290a 2020 2020 2020 2020 7365 6c66 2e72  ).        self.r
-00005200: 6566 696c 6c5f 6472 6f70 646f 776e 2873  efill_dropdown(s
-00005210: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-00005220: 6f67 2e74 7261 6e73 6d69 7474 6572 2c20  og.transmitter, 
-00005230: 7661 6c75 6529 0a20 2020 2020 2020 2076  value).        v
-00005240: 616c 7565 203d 2073 656c 662e 636f 6e74  alue = self.cont
-00005250: 6573 745f 7365 7474 696e 6773 2e67 6574  est_settings.get
-00005260: 2822 5374 6172 7444 6174 6522 290a 2020  ("StartDate").  
-00005270: 2020 2020 2020 7468 655f 6461 7465 2c20        the_date, 
-00005280: 7468 655f 7469 6d65 203d 2076 616c 7565  the_time = value
-00005290: 2e73 706c 6974 2829 0a20 2020 2020 2020  .split().       
-000052a0: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
-000052b0: 616c 6f67 2e64 6174 6554 696d 6545 6469  alog.dateTimeEdi
-000052c0: 742e 7365 7444 6174 6528 0a20 2020 2020  t.setDate(.     
-000052d0: 2020 2020 2020 2051 7443 6f72 652e 5144         QtCore.QD
-000052e0: 6174 652e 6672 6f6d 5374 7269 6e67 2874  ate.fromString(t
-000052f0: 6865 5f64 6174 652c 2022 7979 7979 2d4d  he_date, "yyyy-M
-00005300: 4d2d 6464 2229 0a20 2020 2020 2020 2029  M-dd").        )
-00005310: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
-00005320: 6e74 6573 745f 6469 616c 6f67 2e64 6174  ntest_dialog.dat
-00005330: 6554 696d 6545 6469 742e 7365 7443 616c  eTimeEdit.setCal
-00005340: 656e 6461 7250 6f70 7570 2854 7275 6529  endarPopup(True)
-00005350: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
-00005360: 6e74 6573 745f 6469 616c 6f67 2e64 6174  ntest_dialog.dat
-00005370: 6554 696d 6545 6469 742e 7365 7454 696d  eTimeEdit.setTim
-00005380: 6528 0a20 2020 2020 2020 2020 2020 2051  e(.            Q
-00005390: 7443 6f72 652e 5154 696d 652e 6672 6f6d  tCore.QTime.from
-000053a0: 5374 7269 6e67 2874 6865 5f74 696d 652c  String(the_time,
-000053b0: 2022 6868 3a6d 6d3a 7373 2229 0a20 2020   "hh:mm:ss").   
-000053c0: 2020 2020 2029 0a20 2020 2020 2020 2073       ).        s
-000053d0: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-000053e0: 6f67 2e6f 7065 6e28 290a 0a20 2020 2064  og.open()..    d
-000053f0: 6566 2073 6176 655f 6564 6974 6564 5f63  ef save_edited_c
-00005400: 6f6e 7465 7374 2873 656c 6629 3a0a 2020  ontest(self):.  
-00005410: 2020 2020 2020 2222 2253 6176 6520 7468        """Save th
-00005420: 6520 6564 6974 6564 2063 6f6e 7465 7374  e edited contest
-00005430: 2222 220a 2020 2020 2020 2020 636f 6e74  """.        cont
-00005440: 6573 7420 3d20 7b7d 0a20 2020 2020 2020  est = {}.       
-00005450: 2063 6f6e 7465 7374 5b22 436f 6e74 6573   contest["Contes
-00005460: 744e 616d 6522 5d20 3d20 280a 2020 2020  tName"] = (.    
-00005470: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-00005480: 7465 7374 5f64 6961 6c6f 672e 636f 6e74  test_dialog.cont
-00005490: 6573 742e 6375 7272 656e 7454 6578 7428  est.currentText(
-000054a0: 292e 6c6f 7765 7228 292e 7265 706c 6163  ).lower().replac
-000054b0: 6528 2220 222c 2022 5f22 290a 2020 2020  e(" ", "_").    
-000054c0: 2020 2020 290a 2020 2020 2020 2020 636f      ).        co
-000054d0: 6e74 6573 745b 2253 7461 7274 4461 7465  ntest["StartDate
-000054e0: 225d 203d 2073 656c 662e 636f 6e74 6573  "] = self.contes
-000054f0: 745f 6469 616c 6f67 2e64 6174 6554 696d  t_dialog.dateTim
-00005500: 6545 6469 742e 6461 7465 5469 6d65 2829  eEdit.dateTime()
-00005510: 2e74 6f53 7472 696e 6728 0a20 2020 2020  .toString(.     
-00005520: 2020 2020 2020 2022 7979 7979 2d4d 4d2d         "yyyy-MM-
-00005530: 6464 2068 683a 6d6d 3a73 7322 0a20 2020  dd hh:mm:ss".   
-00005540: 2020 2020 2029 0a20 2020 2020 2020 2063       ).        c
-00005550: 6f6e 7465 7374 5b22 4f70 6572 6174 6f72  ontest["Operator
-00005560: 4361 7465 676f 7279 225d 203d 2073 656c  Category"] = sel
-00005570: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
-00005580: 2e6f 7065 7261 746f 725f 636c 6173 732e  .operator_class.
-00005590: 6375 7272 656e 7454 6578 7428 290a 2020  currentText().  
-000055a0: 2020 2020 2020 636f 6e74 6573 745b 2242        contest["B
-000055b0: 616e 6443 6174 6567 6f72 7922 5d20 3d20  andCategory"] = 
-000055c0: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
-000055d0: 6c6f 672e 6261 6e64 2e63 7572 7265 6e74  log.band.current
-000055e0: 5465 7874 2829 0a20 2020 2020 2020 2063  Text().        c
-000055f0: 6f6e 7465 7374 5b22 506f 7765 7243 6174  ontest["PowerCat
-00005600: 6567 6f72 7922 5d20 3d20 7365 6c66 2e63  egory"] = self.c
-00005610: 6f6e 7465 7374 5f64 6961 6c6f 672e 706f  ontest_dialog.po
-00005620: 7765 722e 6375 7272 656e 7454 6578 7428  wer.currentText(
-00005630: 290a 2020 2020 2020 2020 636f 6e74 6573  ).        contes
-00005640: 745b 224d 6f64 6543 6174 6567 6f72 7922  t["ModeCategory"
-00005650: 5d20 3d20 7365 6c66 2e63 6f6e 7465 7374  ] = self.contest
-00005660: 5f64 6961 6c6f 672e 6d6f 6465 2e63 7572  _dialog.mode.cur
-00005670: 7265 6e74 5465 7874 2829 0a20 2020 2020  rentText().     
-00005680: 2020 2063 6f6e 7465 7374 5b22 4f76 6572     contest["Over
-00005690: 6c61 7943 6174 6567 6f72 7922 5d20 3d20  layCategory"] = 
-000056a0: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
-000056b0: 6c6f 672e 6f76 6572 6c61 792e 6375 7272  log.overlay.curr
-000056c0: 656e 7454 6578 7428 290a 2020 2020 2020  entText().      
-000056d0: 2020 636f 6e74 6573 745b 224f 7065 7261    contest["Opera
-000056e0: 746f 7273 225d 203d 2073 656c 662e 636f  tors"] = self.co
-000056f0: 6e74 6573 745f 6469 616c 6f67 2e6f 7065  ntest_dialog.ope
-00005700: 7261 746f 7273 2e74 6578 7428 290a 2020  rators.text().  
-00005710: 2020 2020 2020 636f 6e74 6573 745b 2253        contest["S
-00005720: 6f61 7062 6f78 225d 203d 2073 656c 662e  oapbox"] = self.
-00005730: 636f 6e74 6573 745f 6469 616c 6f67 2e73  contest_dialog.s
-00005740: 6f61 7062 6f78 2e74 6f50 6c61 696e 5465  oapbox.toPlainTe
-00005750: 7874 2829 0a20 2020 2020 2020 2063 6f6e  xt().        con
-00005760: 7465 7374 5b22 5365 6e74 4578 6368 616e  test["SentExchan
-00005770: 6765 225d 203d 2073 656c 662e 636f 6e74  ge"] = self.cont
-00005780: 6573 745f 6469 616c 6f67 2e65 7863 6861  est_dialog.excha
-00005790: 6e67 652e 7465 7874 2829 0a20 2020 2020  nge.text().     
-000057a0: 2020 2063 6f6e 7465 7374 5b22 436f 6e74     contest["Cont
-000057b0: 6573 744e 5222 5d20 3d20 7365 6c66 2e70  estNR"] = self.p
-000057c0: 7265 662e 6765 7428 2263 6f6e 7465 7374  ref.get("contest
-000057d0: 222c 2031 290a 2020 2020 2020 2020 636f  ", 1).        co
-000057e0: 6e74 6573 745b 2253 7461 7469 6f6e 4361  ntest["StationCa
-000057f0: 7465 676f 7279 225d 203d 2073 656c 662e  tegory"] = self.
-00005800: 636f 6e74 6573 745f 6469 616c 6f67 2e73  contest_dialog.s
-00005810: 7461 7469 6f6e 2e63 7572 7265 6e74 5465  tation.currentTe
-00005820: 7874 2829 0a20 2020 2020 2020 2063 6f6e  xt().        con
-00005830: 7465 7374 5b22 4173 7369 7374 6564 4361  test["AssistedCa
-00005840: 7465 676f 7279 225d 203d 2073 656c 662e  tegory"] = self.
-00005850: 636f 6e74 6573 745f 6469 616c 6f67 2e61  contest_dialog.a
-00005860: 7373 6973 7465 642e 6375 7272 656e 7454  ssisted.currentT
-00005870: 6578 7428 290a 2020 2020 2020 2020 636f  ext().        co
-00005880: 6e74 6573 745b 2254 7261 6e73 6d69 7474  ntest["Transmitt
-00005890: 6572 4361 7465 676f 7279 225d 203d 2073  erCategory"] = s
-000058a0: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-000058b0: 6f67 2e74 7261 6e73 6d69 7474 6572 2e63  og.transmitter.c
-000058c0: 7572 7265 6e74 5465 7874 2829 0a0a 2020  urrentText()..  
-000058d0: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-000058e0: 7567 2822 2573 222c 2066 227b 636f 6e74  ug("%s", f"{cont
-000058f0: 6573 747d 2229 0a20 2020 2020 2020 2073  est}").        s
-00005900: 656c 662e 6461 7461 6261 7365 2e75 7064  elf.database.upd
-00005910: 6174 655f 636f 6e74 6573 7428 636f 6e74  ate_contest(cont
-00005920: 6573 7429 0a20 2020 2020 2020 2073 656c  est).        sel
-00005930: 662e 7772 6974 655f 7072 6566 6572 656e  f.write_preferen
-00005940: 6365 2829 0a20 2020 2020 2020 2073 656c  ce().        sel
-00005950: 662e 6c6f 6164 5f63 6f6e 7465 7374 2829  f.load_contest()
-00005960: 0a0a 2020 2020 6465 6620 6c6f 6164 5f63  ..    def load_c
-00005970: 6f6e 7465 7374 2873 656c 6629 3a0a 2020  ontest(self):.  
-00005980: 2020 2020 2020 2222 226c 6f61 6420 6120        """load a 
-00005990: 636f 6e74 6573 7422 2222 0a20 2020 2020  contest""".     
-000059a0: 2020 2069 6620 7365 6c66 2e70 7265 662e     if self.pref.
-000059b0: 6765 7428 2263 6f6e 7465 7374 2229 3a0a  get("contest"):.
-000059c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000059d0: 2e63 6f6e 7465 7374 5f73 6574 7469 6e67  .contest_setting
-000059e0: 7320 3d20 7365 6c66 2e64 6174 6162 6173  s = self.databas
-000059f0: 652e 6665 7463 685f 636f 6e74 6573 745f  e.fetch_contest_
-00005a00: 6279 5f69 6428 0a20 2020 2020 2020 2020  by_id(.         
-00005a10: 2020 2020 2020 2073 656c 662e 7072 6566         self.pref
-00005a20: 2e67 6574 2822 636f 6e74 6573 7422 290a  .get("contest").
-00005a30: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00005a40: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00005a50: 662e 636f 6e74 6573 745f 7365 7474 696e  f.contest_settin
-00005a60: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-00005a70: 2020 2020 7365 6c66 2e64 6174 6162 6173      self.databas
-00005a80: 652e 6375 7272 656e 745f 636f 6e74 6573  e.current_contes
-00005a90: 7420 3d20 7365 6c66 2e70 7265 662e 6765  t = self.pref.ge
-00005aa0: 7428 2263 6f6e 7465 7374 2229 0a20 2020  t("contest").   
-00005ab0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00005ac0: 7365 6c66 2e63 6f6e 7465 7374 5f73 6574  self.contest_set
-00005ad0: 7469 6e67 732e 6765 7428 2243 6f6e 7465  tings.get("Conte
-00005ae0: 7374 4e61 6d65 2229 3a0a 2020 2020 2020  stName"):.      
-00005af0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00005b00: 6c66 2e63 6f6e 7465 7374 203d 2064 6f69  lf.contest = doi
-00005b10: 6d70 2873 656c 662e 636f 6e74 6573 745f  mp(self.contest_
-00005b20: 7365 7474 696e 6773 2e67 6574 2822 436f  settings.get("Co
-00005b30: 6e74 6573 744e 616d 6522 2929 0a20 2020  ntestName")).   
-00005b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b50: 206c 6f67 6765 722e 6465 6275 6728 224c   logger.debug("L
-00005b60: 6f61 6465 6420 436f 6e74 6573 7420 4e61  oaded Contest Na
-00005b70: 6d65 203d 2025 7322 2c20 7365 6c66 2e63  me = %s", self.c
-00005b80: 6f6e 7465 7374 2e6e 616d 6529 0a20 2020  ontest.name).   
-00005b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ba0: 2073 656c 662e 7365 745f 7769 6e64 6f77   self.set_window
-00005bb0: 5f74 6974 6c65 2829 0a20 2020 2020 2020  _title().       
-00005bc0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00005bd0: 662e 636f 6e74 6573 742e 696e 6974 5f63  f.contest.init_c
-00005be0: 6f6e 7465 7374 2873 656c 6629 0a20 2020  ontest(self).   
-00005bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c00: 2073 656c 662e 6869 6465 5f62 616e 645f   self.hide_band_
-00005c10: 6d6f 6465 2873 656c 662e 636f 6e74 6573  mode(self.contes
-00005c20: 745f 7365 7474 696e 6773 2e67 6574 2822  t_settings.get("
-00005c30: 4d6f 6465 4361 7465 676f 7279 222c 2022  ModeCategory", "
-00005c40: 2229 290a 0a20 2020 2020 2020 2020 2020  "))..           
-00005c50: 2020 2020 2069 6620 6861 7361 7474 7228       if hasattr(
-00005c60: 7365 6c66 2e63 6f6e 7465 7374 2c20 226d  self.contest, "m
-00005c70: 6f64 6522 293a 0a20 2020 2020 2020 2020  ode"):.         
-00005c80: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00005c90: 6c66 2e63 6f6e 7465 7374 2e6d 6f64 6520  lf.contest.mode 
-00005ca0: 696e 205b 2243 5722 2c20 2242 4f54 4822  in ["CW", "BOTH"
-00005cb0: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
-00005cc0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00005cd0: 6377 5f73 7065 6564 2e73 686f 7728 290a  cw_speed.show().
-00005ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005cf0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00005d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d10: 2020 7365 6c66 2e63 775f 7370 6565 642e    self.cw_speed.
-00005d20: 6869 6465 2829 0a0a 2020 2020 2020 2020  hide()..        
-00005d30: 2020 2020 2020 2020 636d 6420 3d20 7b7d          cmd = {}
-00005d40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005d50: 2063 6d64 5b22 636d 6422 5d20 3d20 224e   cmd["cmd"] = "N
-00005d60: 4557 4442 220a 2020 2020 2020 2020 2020  EWDB".          
-00005d70: 2020 2020 2020 636d 645b 2273 7461 7469        cmd["stati
-00005d80: 6f6e 225d 203d 2070 6c61 7466 6f72 6d2e  on"] = platform.
-00005d90: 6e6f 6465 2829 0a20 2020 2020 2020 2020  node().         
-00005da0: 2020 2020 2020 2073 656c 662e 6d75 6c74         self.mult
-00005db0: 6963 6173 745f 696e 7465 7266 6163 652e  icast_interface.
-00005dc0: 7365 6e64 5f61 735f 6a73 6f6e 2863 6d64  send_as_json(cmd
-00005dd0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00005de0: 2020 6966 2068 6173 6174 7472 2873 656c    if hasattr(sel
-00005df0: 662e 636f 6e74 6573 742c 2022 636f 6c75  f.contest, "colu
-00005e00: 6d6e 7322 293a 0a20 2020 2020 2020 2020  mns"):.         
-00005e10: 2020 2020 2020 2020 2020 2063 6d64 203d             cmd =
-00005e20: 207b 7d0a 2020 2020 2020 2020 2020 2020   {}.            
-00005e30: 2020 2020 2020 2020 636d 645b 2263 6d64          cmd["cmd
-00005e40: 225d 203d 2022 5348 4f57 434f 4c55 4d4e  "] = "SHOWCOLUMN
-00005e50: 5322 0a20 2020 2020 2020 2020 2020 2020  S".             
-00005e60: 2020 2020 2020 2063 6d64 5b22 7374 6174         cmd["stat
-00005e70: 696f 6e22 5d20 3d20 706c 6174 666f 726d  ion"] = platform
-00005e80: 2e6e 6f64 6528 290a 2020 2020 2020 2020  .node().        
-00005e90: 2020 2020 2020 2020 2020 2020 636d 645b              cmd[
-00005ea0: 2243 4f4c 554d 4e53 225d 203d 2073 656c  "COLUMNS"] = sel
-00005eb0: 662e 636f 6e74 6573 742e 636f 6c75 6d6e  f.contest.column
-00005ec0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-00005ed0: 2020 2020 2020 7365 6c66 2e6d 756c 7469        self.multi
-00005ee0: 6361 7374 5f69 6e74 6572 6661 6365 2e73  cast_interface.s
-00005ef0: 656e 645f 6173 5f6a 736f 6e28 636d 6429  end_as_json(cmd)
-00005f00: 0a0a 2020 2020 6465 6620 6869 6465 5f62  ..    def hide_b
-00005f10: 616e 645f 6d6f 6465 2873 656c 662c 2074  and_mode(self, t
-00005f20: 6865 5f6d 6f64 653a 2073 7472 2920 2d3e  he_mode: str) ->
-00005f30: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-00005f40: 2222 6869 6465 2222 220a 2020 2020 2020  ""hide""".      
-00005f50: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
-00005f60: 2573 222c 2066 227b 7468 655f 6d6f 6465  %s", f"{the_mode
-00005f70: 7d22 290a 2020 2020 2020 2020 7365 6c66  }").        self
-00005f80: 2e42 616e 645f 4d6f 6465 5f46 7261 6d65  .Band_Mode_Frame
-00005f90: 5f43 572e 6869 6465 2829 0a20 2020 2020  _CW.hide().     
-00005fa0: 2020 2073 656c 662e 4261 6e64 5f4d 6f64     self.Band_Mod
-00005fb0: 655f 4672 616d 655f 5353 422e 6869 6465  e_Frame_SSB.hide
-00005fc0: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-00005fd0: 4261 6e64 5f4d 6f64 655f 4672 616d 655f  Band_Mode_Frame_
-00005fe0: 5254 5459 2e68 6964 6528 290a 2020 2020  RTTY.hide().    
-00005ff0: 2020 2020 6d6f 6465 7320 3d20 7b0a 2020      modes = {.  
-00006000: 2020 2020 2020 2020 2020 2243 5722 3a20            "CW": 
-00006010: 2873 656c 662e 4261 6e64 5f4d 6f64 655f  (self.Band_Mode_
-00006020: 4672 616d 655f 4357 2c29 2c0a 2020 2020  Frame_CW,),.    
-00006030: 2020 2020 2020 2020 2253 5342 223a 2028          "SSB": (
-00006040: 7365 6c66 2e42 616e 645f 4d6f 6465 5f46  self.Band_Mode_F
-00006050: 7261 6d65 5f53 5342 2c29 2c0a 2020 2020  rame_SSB,),.    
-00006060: 2020 2020 2020 2020 2252 5454 5922 3a20          "RTTY": 
-00006070: 2873 656c 662e 4261 6e64 5f4d 6f64 655f  (self.Band_Mode_
-00006080: 4672 616d 655f 5254 5459 2c29 2c0a 2020  Frame_RTTY,),.  
-00006090: 2020 2020 2020 2020 2020 2250 534b 223a            "PSK":
-000060a0: 2028 7365 6c66 2e42 616e 645f 4d6f 6465   (self.Band_Mode
-000060b0: 5f46 7261 6d65 5f52 5454 592c 292c 0a20  _Frame_RTTY,),. 
-000060c0: 2020 2020 2020 2020 2020 2022 5353 422b             "SSB+
-000060d0: 4357 223a 2028 7365 6c66 2e42 616e 645f  CW": (self.Band_
-000060e0: 4d6f 6465 5f46 7261 6d65 5f43 572c 2073  Mode_Frame_CW, s
-000060f0: 656c 662e 4261 6e64 5f4d 6f64 655f 4672  elf.Band_Mode_Fr
-00006100: 616d 655f 5353 4229 2c0a 2020 2020 2020  ame_SSB),.      
-00006110: 2020 2020 2020 2242 4f54 4822 3a20 2873        "BOTH": (s
-00006120: 656c 662e 4261 6e64 5f4d 6f64 655f 4672  elf.Band_Mode_Fr
-00006130: 616d 655f 4357 2c20 7365 6c66 2e42 616e  ame_CW, self.Ban
-00006140: 645f 4d6f 6465 5f46 7261 6d65 5f53 5342  d_Mode_Frame_SSB
-00006150: 292c 0a20 2020 2020 2020 2020 2020 2022  ),.            "
-00006160: 4449 4749 5441 4c22 3a20 2873 656c 662e  DIGITAL": (self.
-00006170: 4261 6e64 5f4d 6f64 655f 4672 616d 655f  Band_Mode_Frame_
-00006180: 5254 5459 2c29 2c0a 2020 2020 2020 2020  RTTY,),.        
-00006190: 2020 2020 2253 5342 2b43 572b 4449 4749      "SSB+CW+DIGI
-000061a0: 5441 4c22 3a20 280a 2020 2020 2020 2020  TAL": (.        
-000061b0: 2020 2020 2020 2020 7365 6c66 2e42 616e          self.Ban
-000061c0: 645f 4d6f 6465 5f46 7261 6d65 5f52 5454  d_Mode_Frame_RTT
-000061d0: 592c 0a20 2020 2020 2020 2020 2020 2020  Y,.             
-000061e0: 2020 2073 656c 662e 4261 6e64 5f4d 6f64     self.Band_Mod
-000061f0: 655f 4672 616d 655f 4357 2c0a 2020 2020  e_Frame_CW,.    
-00006200: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00006210: 2e42 616e 645f 4d6f 6465 5f46 7261 6d65  .Band_Mode_Frame
-00006220: 5f53 5342 2c0a 2020 2020 2020 2020 2020  _SSB,.          
-00006230: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
-00006240: 2022 464d 223a 2028 7365 6c66 2e42 616e   "FM": (self.Ban
-00006250: 645f 4d6f 6465 5f46 7261 6d65 5f53 5342  d_Mode_Frame_SSB
-00006260: 2c29 2c0a 2020 2020 2020 2020 7d0a 2020  ,),.        }.  
-00006270: 2020 2020 2020 6672 616d 6573 203d 206d        frames = m
-00006280: 6f64 6573 2e67 6574 2874 6865 5f6d 6f64  odes.get(the_mod
-00006290: 6529 0a20 2020 2020 2020 2069 6620 6672  e).        if fr
-000062a0: 616d 6573 3a0a 2020 2020 2020 2020 2020  ames:.          
-000062b0: 2020 666f 7220 6672 616d 6520 696e 2066    for frame in f
-000062c0: 7261 6d65 733a 0a20 2020 2020 2020 2020  rames:.         
-000062d0: 2020 2020 2020 2066 7261 6d65 2e73 686f         frame.sho
-000062e0: 7728 290a 0a20 2020 2064 6566 2066 696c  w()..    def fil
-000062f0: 6570 6963 6b65 7228 7365 6c66 2c20 6163  epicker(self, ac
-00006300: 7469 6f6e 3a20 7374 7229 202d 3e20 7374  tion: str) -> st
-00006310: 723a 0a20 2020 2020 2020 2022 2222 0a20  r:.        """. 
-00006320: 2020 2020 2020 2047 6574 2061 2066 696c         Get a fil
-00006330: 656e 616d 650a 2020 2020 2020 2020 6163  ename.        ac
-00006340: 7469 6f6e 3a20 226e 6577 2220 6f72 2022  tion: "new" or "
-00006350: 6f70 656e 220a 2020 2020 2020 2020 2222  open".        ""
-00006360: 220a 2020 2020 2020 2020 6f70 7469 6f6e  ".        option
-00006370: 7320 3d20 5146 696c 6544 6961 6c6f 672e  s = QFileDialog.
-00006380: 4f70 7469 6f6e 7328 290a 2020 2020 2020  Options().      
-00006390: 2020 6f70 7469 6f6e 7320 7c3d 2051 4669    options |= QFi
-000063a0: 6c65 4469 616c 6f67 2e44 6f6e 7455 7365  leDialog.DontUse
-000063b0: 4e61 7469 7665 4469 616c 6f67 0a20 2020  NativeDialog.   
-000063c0: 2020 2020 206f 7074 696f 6e73 207c 3d20       options |= 
-000063d0: 5146 696c 6544 6961 6c6f 672e 446f 6e74  QFileDialog.Dont
-000063e0: 436f 6e66 6972 6d4f 7665 7277 7269 7465  ConfirmOverwrite
-000063f0: 0a20 2020 2020 2020 2023 2070 6963 6b65  .        # picke
-00006400: 7220 3d20 5146 696c 6544 6961 6c6f 6728  r = QFileDialog(
-00006410: 7365 6c66 290a 2020 2020 2020 2020 6966  self).        if
-00006420: 2061 6374 696f 6e20 3d3d 2022 6e65 7722   action == "new"
-00006430: 3a0a 2020 2020 2020 2020 2020 2020 6669  :.            fi
-00006440: 6c65 2c20 5f20 3d20 5146 696c 6544 6961  le, _ = QFileDia
-00006450: 6c6f 672e 6765 7453 6176 6546 696c 654e  log.getSaveFileN
-00006460: 616d 6528 0a20 2020 2020 2020 2020 2020  ame(.           
-00006470: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-00006480: 2020 2020 2020 2020 2020 2022 4368 6f6f             "Choo
-00006490: 7365 2061 2044 6174 6162 6173 6522 2c0a  se a Database",.
-000064a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000064b0: 4441 5441 5f50 4154 482c 0a20 2020 2020  DATA_PATH,.     
-000064c0: 2020 2020 2020 2020 2020 2022 4461 7461             "Data
-000064d0: 6261 7365 2028 2a2e 6462 2922 2c0a 2020  base (*.db)",.  
-000064e0: 2020 2020 2020 2020 2020 2020 2020 6f70                op
-000064f0: 7469 6f6e 733d 6f70 7469 6f6e 732c 0a20  tions=options,. 
-00006500: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00006510: 2020 2020 2069 6620 6163 7469 6f6e 203d       if action =
-00006520: 3d20 226f 7065 6e22 3a0a 2020 2020 2020  = "open":.      
-00006530: 2020 2020 2020 6669 6c65 2c20 5f20 3d20        file, _ = 
-00006540: 5146 696c 6544 6961 6c6f 672e 6765 744f  QFileDialog.getO
-00006550: 7065 6e46 696c 654e 616d 6528 0a20 2020  penFileName(.   
-00006560: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00006570: 662c 0a20 2020 2020 2020 2020 2020 2020  f,.             
-00006580: 2020 2022 4368 6f6f 7365 2061 2044 6174     "Choose a Dat
-00006590: 6162 6173 6522 2c0a 2020 2020 2020 2020  abase",.        
-000065a0: 2020 2020 2020 2020 4441 5441 5f50 4154          DATA_PAT
-000065b0: 482c 0a20 2020 2020 2020 2020 2020 2020  H,.             
-000065c0: 2020 2022 4461 7461 6261 7365 2028 2a2e     "Database (*.
-000065d0: 6462 2922 2c0a 2020 2020 2020 2020 2020  db)",.          
-000065e0: 2020 2020 2020 6f70 7469 6f6e 733d 6f70        options=op
-000065f0: 7469 6f6e 732c 0a20 2020 2020 2020 2020  tions,.         
-00006600: 2020 2029 0a20 2020 2020 2020 2072 6574     ).        ret
-00006610: 7572 6e20 6669 6c65 0a0a 2020 2020 6465  urn file..    de
-00006620: 6620 7265 6361 6c63 756c 6174 655f 6d75  f recalculate_mu
-00006630: 6c74 7328 7365 6c66 293a 0a20 2020 2020  lts(self):.     
-00006640: 2020 2022 2222 5265 6361 6c63 756c 6174     """Recalculat
-00006650: 6520 4d75 6c74 6970 6c69 6572 7322 2222  e Multipliers"""
-00006660: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
-00006670: 6e74 6573 742e 7265 6361 6c63 756c 6174  ntest.recalculat
-00006680: 655f 6d75 6c74 7328 7365 6c66 290a 0a20  e_mults(self).. 
-00006690: 2020 2064 6566 206c 6175 6e63 685f 6c6f     def launch_lo
-000066a0: 675f 7769 6e64 6f77 2873 656c 6629 3a0a  g_window(self):.
-000066b0: 2020 2020 2020 2020 2222 226c 6175 6e63          """launc
-000066c0: 6820 7468 6520 4c6f 6720 5769 6e64 6f77  h the Log Window
-000066d0: 2222 220a 2020 2020 2020 2020 6966 206e  """.        if n
-000066e0: 6f74 2063 6865 636b 5f70 726f 6365 7373  ot check_process
-000066f0: 2822 6c6f 6777 696e 646f 772e 7079 2229  ("logwindow.py")
-00006700: 3a0a 2020 2020 2020 2020 2020 2020 5f20  :.            _ 
-00006710: 3d20 7375 6270 726f 6365 7373 2e50 6f70  = subprocess.Pop
-00006720: 656e 285b 7379 732e 6578 6563 7574 6162  en([sys.executab
-00006730: 6c65 2c20 574f 524b 494e 475f 5041 5448  le, WORKING_PATH
-00006740: 202b 2022 2f6c 6f67 7769 6e64 6f77 2e70   + "/logwindow.p
-00006750: 7922 5d29 0a0a 2020 2020 6465 6620 6c61  y"])..    def la
-00006760: 756e 6368 5f62 616e 646d 6170 5f77 696e  unch_bandmap_win
-00006770: 646f 7728 7365 6c66 293a 0a20 2020 2020  dow(self):.     
-00006780: 2020 2022 2222 6c61 756e 6368 2074 6865     """launch the
-00006790: 204c 6f67 2057 696e 646f 7722 2222 0a20   Log Window""". 
-000067a0: 2020 2020 2020 2069 6620 6e6f 7420 6368         if not ch
-000067b0: 6563 6b5f 7072 6f63 6573 7328 2262 616e  eck_process("ban
-000067c0: 646d 6170 2e70 7922 293a 0a20 2020 2020  dmap.py"):.     
-000067d0: 2020 2020 2020 205f 203d 2073 7562 7072         _ = subpr
-000067e0: 6f63 6573 732e 506f 7065 6e28 5b73 7973  ocess.Popen([sys
-000067f0: 2e65 7865 6375 7461 626c 652c 2057 4f52  .executable, WOR
-00006800: 4b49 4e47 5f50 4154 4820 2b20 222f 6261  KING_PATH + "/ba
-00006810: 6e64 6d61 702e 7079 225d 290a 0a20 2020  ndmap.py"])..   
-00006820: 2064 6566 2063 6c65 6172 5f62 616e 645f   def clear_band_
-00006830: 696e 6469 6361 746f 7273 2873 656c 6629  indicators(self)
-00006840: 3a0a 2020 2020 2020 2020 2222 2243 6c65  :.        """Cle
-00006850: 6172 2074 6865 2069 6e64 6963 6174 6f72  ar the indicator
-00006860: 7322 2222 0a20 2020 2020 2020 2066 6f72  s""".        for
-00006870: 205f 2c20 696e 6469 6361 746f 7273 2069   _, indicators i
-00006880: 6e20 7365 6c66 2e61 6c6c 5f6d 6f64 655f  n self.all_mode_
-00006890: 696e 6469 6361 746f 7273 2e69 7465 6d73  indicators.items
-000068a0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-000068b0: 666f 7220 5f2c 2069 6e64 6963 6174 6f72  for _, indicator
-000068c0: 2069 6e20 696e 6469 6361 746f 7273 2e69   in indicators.i
-000068d0: 7465 6d73 2829 3a0a 2020 2020 2020 2020  tems():.        
-000068e0: 2020 2020 2020 2020 696e 6469 6361 746f          indicato
-000068f0: 722e 7365 7446 7261 6d65 5368 6170 6528  r.setFrameShape(
-00006900: 5174 5769 6467 6574 732e 5146 7261 6d65  QtWidgets.QFrame
-00006910: 2e4e 6f46 7261 6d65 290a 0a20 2020 2064  .NoFrame)..    d
-00006920: 6566 2073 6574 5f62 616e 645f 696e 6469  ef set_band_indi
-00006930: 6361 746f 7228 7365 6c66 2c20 6261 6e64  cator(self, band
-00006940: 3a20 7374 7229 202d 3e20 4e6f 6e65 3a0a  : str) -> None:.
-00006950: 2020 2020 2020 2020 2222 2253 6574 2074          """Set t
-00006960: 6865 2062 616e 6420 696e 6469 6361 746f  he band indicato
-00006970: 7222 2222 0a20 2020 2020 2020 206c 6f67  r""".        log
-00006980: 6765 722e 6465 6275 6728 2225 7322 2c20  ger.debug("%s", 
-00006990: 6622 6261 6e64 3a7b 6261 6e64 7d20 6d6f  f"band:{band} mo
-000069a0: 6465 3a20 7b73 656c 662e 6375 7272 656e  de: {self.curren
-000069b0: 745f 6d6f 6465 7d22 290a 2020 2020 2020  t_mode}").      
-000069c0: 2020 6966 2062 616e 6420 616e 6420 7365    if band and se
-000069d0: 6c66 2e63 7572 7265 6e74 5f6d 6f64 653a  lf.current_mode:
-000069e0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000069f0: 662e 636c 6561 725f 6261 6e64 5f69 6e64  f.clear_band_ind
-00006a00: 6963 6174 6f72 7328 290a 2020 2020 2020  icators().      
-00006a10: 2020 2020 2020 696e 6469 6361 746f 7220        indicator 
-00006a20: 3d20 7365 6c66 2e61 6c6c 5f6d 6f64 655f  = self.all_mode_
-00006a30: 696e 6469 6361 746f 7273 5b73 656c 662e  indicators[self.
-00006a40: 6375 7272 656e 745f 6d6f 6465 5d2e 6765  current_mode].ge
-00006a50: 7428 6261 6e64 2c20 4e6f 6e65 290a 2020  t(band, None).  
-00006a60: 2020 2020 2020 2020 2020 6966 2069 6e64            if ind
-00006a70: 6963 6174 6f72 3a0a 2020 2020 2020 2020  icator:.        
-00006a80: 2020 2020 2020 2020 696e 6469 6361 746f          indicato
-00006a90: 722e 7365 7446 7261 6d65 5368 6170 6528  r.setFrameShape(
-00006aa0: 5174 5769 6467 6574 732e 5146 7261 6d65  QtWidgets.QFrame
-00006ab0: 2e42 6f78 290a 0a20 2020 2064 6566 2063  .Box)..    def c
-00006ac0: 6c6f 7365 4576 656e 7428 7365 6c66 2c20  loseEvent(self, 
-00006ad0: 5f65 7665 6e74 293a 0a20 2020 2020 2020  _event):.       
-00006ae0: 2022 2222 0a20 2020 2020 2020 2057 7269   """.        Wri
-00006af0: 7465 2077 696e 646f 7720 7369 7a65 2061  te window size a
-00006b00: 6e64 2070 6f73 6974 696f 6e20 746f 2063  nd position to c
-00006b10: 6f6e 6669 6720 6669 6c65 0a20 2020 2020  onfig file.     
-00006b20: 2020 2022 2222 0a20 2020 2020 2020 2073     """.        s
-00006b30: 656c 662e 7072 6566 5b22 7769 6e64 6f77  elf.pref["window
-00006b40: 5f77 6964 7468 225d 203d 2073 656c 662e  _width"] = self.
-00006b50: 7369 7a65 2829 2e77 6964 7468 2829 0a20  size().width(). 
-00006b60: 2020 2020 2020 2073 656c 662e 7072 6566         self.pref
-00006b70: 5b22 7769 6e64 6f77 5f68 6569 6768 7422  ["window_height"
-00006b80: 5d20 3d20 7365 6c66 2e73 697a 6528 292e  ] = self.size().
-00006b90: 6865 6967 6874 2829 0a20 2020 2020 2020  height().       
-00006ba0: 2073 656c 662e 7072 6566 5b22 7769 6e64   self.pref["wind
-00006bb0: 6f77 5f78 225d 203d 2073 656c 662e 706f  ow_x"] = self.po
-00006bc0: 7328 292e 7828 290a 2020 2020 2020 2020  s().x().        
-00006bd0: 7365 6c66 2e70 7265 665b 2277 696e 646f  self.pref["windo
-00006be0: 775f 7922 5d20 3d20 7365 6c66 2e70 6f73  w_y"] = self.pos
-00006bf0: 2829 2e79 2829 0a20 2020 2020 2020 2073  ().y().        s
-00006c00: 656c 662e 7772 6974 655f 7072 6566 6572  elf.write_prefer
-00006c10: 656e 6365 2829 0a0a 2020 2020 6465 6620  ence()..    def 
-00006c20: 6374 795f 6c6f 6f6b 7570 2873 656c 662c  cty_lookup(self,
-00006c30: 2063 616c 6c73 6967 6e3a 2073 7472 293a   callsign: str):
-00006c40: 0a20 2020 2020 2020 2022 2222 4c6f 6f6b  .        """Look
-00006c50: 7570 2063 616c 6c73 6967 6e20 696e 2063  up callsign in c
-00006c60: 7479 2e64 6174 2066 696c 6522 2222 0a20  ty.dat file""". 
-00006c70: 2020 2020 2020 2063 616c 6c73 6967 6e20         callsign 
-00006c80: 3d20 6361 6c6c 7369 676e 2e75 7070 6572  = callsign.upper
-00006c90: 2829 0a20 2020 2020 2020 2066 6f72 2063  ().        for c
-00006ca0: 6f75 6e74 2069 6e20 7265 7665 7273 6564  ount in reversed
-00006cb0: 2872 616e 6765 286c 656e 2863 616c 6c73  (range(len(calls
-00006cc0: 6967 6e29 2929 3a0a 2020 2020 2020 2020  ign))):.        
-00006cd0: 2020 2020 7365 6172 6368 6974 656d 203d      searchitem =
-00006ce0: 2063 616c 6c73 6967 6e5b 3a20 636f 756e   callsign[: coun
-00006cf0: 7420 2b20 315d 0a20 2020 2020 2020 2020  t + 1].         
-00006d00: 2020 2072 6573 756c 7420 3d20 7b6b 6579     result = {key
-00006d10: 3a20 7661 6c20 666f 7220 6b65 792c 2076  : val for key, v
-00006d20: 616c 2069 6e20 4354 5946 494c 452e 6974  al in CTYFILE.it
-00006d30: 656d 7328 2920 6966 206b 6579 203d 3d20  ems() if key == 
-00006d40: 7365 6172 6368 6974 656d 7d0a 2020 2020  searchitem}.    
-00006d50: 2020 2020 2020 2020 6966 206e 6f74 2072          if not r
-00006d60: 6573 756c 743a 0a20 2020 2020 2020 2020  esult:.         
-00006d70: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
-00006d80: 2020 2020 2020 2020 2020 2020 6966 2072              if r
-00006d90: 6573 756c 742e 6765 7428 7365 6172 6368  esult.get(search
-00006da0: 6974 656d 292e 6765 7428 2265 7861 6374  item).get("exact
-00006db0: 5f6d 6174 6368 2229 3a0a 2020 2020 2020  _match"):.      
-00006dc0: 2020 2020 2020 2020 2020 6966 2073 6561            if sea
-00006dd0: 7263 6869 7465 6d20 3d3d 2063 616c 6c73  rchitem == calls
-00006de0: 6967 6e3a 0a20 2020 2020 2020 2020 2020  ign:.           
-00006df0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00006e00: 7265 7375 6c74 0a20 2020 2020 2020 2020  result.         
-00006e10: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
-00006e20: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00006e30: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
-00006e40: 6566 2063 7773 7065 6564 5f73 7069 6e62  ef cwspeed_spinb
-00006e50: 6f78 5f63 6861 6e67 6564 2873 656c 6629  ox_changed(self)
-00006e60: 3a0a 2020 2020 2020 2020 2222 2274 7269  :.        """tri
-00006e70: 6767 6572 6564 2077 6865 6e20 7661 6c75  ggered when valu
-00006e80: 6520 6f66 2043 5720 7370 6565 6420 696e  e of CW speed in
-00006e90: 2074 6865 2073 7069 6e62 6f78 2063 6861   the spinbox cha
-00006ea0: 6e67 6573 2e22 2222 0a20 2020 2020 2020  nges.""".       
-00006eb0: 2069 6620 7365 6c66 2e63 772e 7365 7276   if self.cw.serv
-00006ec0: 6572 7479 7065 203d 3d20 313a 0a20 2020  ertype == 1:.   
-00006ed0: 2020 2020 2020 2020 2073 656c 662e 6377           self.cw
-00006ee0: 2e73 7065 6564 203d 2073 656c 662e 6377  .speed = self.cw
-00006ef0: 5f73 7065 6564 2e76 616c 7565 2829 0a20  _speed.value(). 
-00006f00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00006f10: 6377 2e73 656e 6463 7728 6622 5c78 3162  cw.sendcw(f"\x1b
-00006f20: 327b 7365 6c66 2e63 772e 7370 6565 647d  2{self.cw.speed}
-00006f30: 2229 0a0a 2020 2020 6465 6620 6b65 7950  ")..    def keyP
-00006f40: 7265 7373 4576 656e 7428 7365 6c66 2c20  ressEvent(self, 
-00006f50: 6576 656e 7429 3a20 2023 2070 796c 696e  event):  # pylin
-00006f60: 743a 2064 6973 6162 6c65 3d69 6e76 616c  t: disable=inval
-00006f70: 6964 2d6e 616d 650a 2020 2020 2020 2020  id-name.        
-00006f80: 2222 2254 6869 7320 6f76 6572 7269 6465  """This override
-00006f90: 7320 5174 206b 6579 2065 7665 6e74 2e22  s Qt key event."
-00006fa0: 2222 0a20 2020 2020 2020 206d 6f64 6966  "".        modif
-00006fb0: 6965 7220 3d20 6576 656e 742e 6d6f 6469  ier = event.modi
-00006fc0: 6669 6572 7328 290a 2020 2020 2020 2020  fiers().        
-00006fd0: 6966 2028 0a20 2020 2020 2020 2020 2020  if (.           
-00006fe0: 2065 7665 6e74 2e6b 6579 2829 203d 3d20   event.key() == 
-00006ff0: 5174 2e4b 6579 2e4b 6579 5f45 7363 6170  Qt.Key.Key_Escap
-00007000: 6520 616e 6420 6d6f 6469 6669 6572 2021  e and modifier !
-00007010: 3d20 5174 2e43 6f6e 7472 6f6c 4d6f 6469  = Qt.ControlModi
-00007020: 6669 6572 0a20 2020 2020 2020 2029 3a20  fier.        ): 
-00007030: 2023 2070 796c 696e 743a 2064 6973 6162   # pylint: disab
-00007040: 6c65 3d6e 6f2d 6d65 6d62 6572 0a20 2020  le=no-member.   
-00007050: 2020 2020 2020 2020 2073 656c 662e 636c           self.cl
-00007060: 6561 7269 6e70 7574 7328 290a 2020 2020  earinputs().    
-00007070: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
-00007080: 2020 2020 2020 2069 6620 6576 656e 742e         if event.
-00007090: 6b65 7928 2920 3d3d 2051 742e 4b65 792e  key() == Qt.Key.
-000070a0: 4b65 795f 4573 6361 7065 2061 6e64 206d  Key_Escape and m
-000070b0: 6f64 6966 6965 7220 3d3d 2051 742e 436f  odifier == Qt.Co
-000070c0: 6e74 726f 6c4d 6f64 6966 6965 723a 0a20  ntrolModifier:. 
-000070d0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-000070e0: 6c66 2e63 7720 6973 206e 6f74 204e 6f6e  lf.cw is not Non
-000070f0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00007100: 2020 2069 6620 7365 6c66 2e63 772e 7365     if self.cw.se
-00007110: 7276 6572 7479 7065 203d 3d20 313a 0a20  rvertype == 1:. 
-00007120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007130: 2020 2073 656c 662e 6377 2e73 656e 6463     self.cw.sendc
-00007140: 7728 225c 7831 6234 2229 0a20 2020 2020  w("\x1b4").     
-00007150: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00007160: 6574 7572 6e0a 2020 2020 2020 2020 6966  eturn.        if
-00007170: 2065 7665 6e74 2e6b 6579 2829 203d 3d20   event.key() == 
-00007180: 5174 2e4b 6579 2e4b 6579 5f50 6167 6555  Qt.Key.Key_PageU
-00007190: 7020 616e 6420 6d6f 6469 6669 6572 203d  p and modifier =
-000071a0: 3d20 5174 2e43 6f6e 7472 6f6c 4d6f 6469  = Qt.ControlModi
-000071b0: 6669 6572 3a0a 2020 2020 2020 2020 2020  fier:.          
-000071c0: 2020 636d 6420 3d20 7b7d 0a20 2020 2020    cmd = {}.     
-000071d0: 2020 2020 2020 2063 6d64 5b22 636d 6422         cmd["cmd"
-000071e0: 5d20 3d20 2250 5245 5653 504f 5422 0a20  ] = "PREVSPOT". 
-000071f0: 2020 2020 2020 2020 2020 2063 6d64 5b22             cmd["
-00007200: 7374 6174 696f 6e22 5d20 3d20 706c 6174  station"] = plat
-00007210: 666f 726d 2e6e 6f64 6528 290a 2020 2020  form.node().    
-00007220: 2020 2020 2020 2020 7365 6c66 2e6d 756c          self.mul
-00007230: 7469 6361 7374 5f69 6e74 6572 6661 6365  ticast_interface
-00007240: 2e73 656e 645f 6173 5f6a 736f 6e28 636d  .send_as_json(cm
-00007250: 6429 0a20 2020 2020 2020 2020 2020 2072  d).            r
-00007260: 6574 7572 6e0a 2020 2020 2020 2020 6966  eturn.        if
-00007270: 2065 7665 6e74 2e6b 6579 2829 203d 3d20   event.key() == 
-00007280: 5174 2e4b 6579 2e4b 6579 5f50 6167 6544  Qt.Key.Key_PageD
-00007290: 6f77 6e20 616e 6420 6d6f 6469 6669 6572  own and modifier
-000072a0: 203d 3d20 5174 2e43 6f6e 7472 6f6c 4d6f   == Qt.ControlMo
-000072b0: 6469 6669 6572 3a0a 2020 2020 2020 2020  difier:.        
-000072c0: 2020 2020 636d 6420 3d20 7b7d 0a20 2020      cmd = {}.   
-000072d0: 2020 2020 2020 2020 2063 6d64 5b22 636d           cmd["cm
-000072e0: 6422 5d20 3d20 224e 4558 5453 504f 5422  d"] = "NEXTSPOT"
-000072f0: 0a20 2020 2020 2020 2020 2020 2063 6d64  .            cmd
-00007300: 5b22 7374 6174 696f 6e22 5d20 3d20 706c  ["station"] = pl
-00007310: 6174 666f 726d 2e6e 6f64 6528 290a 2020  atform.node().  
-00007320: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00007330: 756c 7469 6361 7374 5f69 6e74 6572 6661  ulticast_interfa
-00007340: 6365 2e73 656e 645f 6173 5f6a 736f 6e28  ce.send_as_json(
-00007350: 636d 6429 0a20 2020 2020 2020 2020 2020  cmd).           
-00007360: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
-00007370: 6966 2065 7665 6e74 2e6b 6579 2829 203d  if event.key() =
-00007380: 3d20 5174 2e4b 6579 2e4b 6579 5f50 6167  = Qt.Key.Key_Pag
-00007390: 6555 7020 616e 6420 6d6f 6469 6669 6572  eUp and modifier
-000073a0: 2021 3d20 5174 2e43 6f6e 7472 6f6c 4d6f   != Qt.ControlMo
-000073b0: 6469 6669 6572 3a0a 2020 2020 2020 2020  difier:.        
-000073c0: 2020 2020 6966 2073 656c 662e 6377 2069      if self.cw i
-000073d0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000073e0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-000073f0: 656c 662e 6377 2e73 6572 7665 7274 7970  elf.cw.servertyp
-00007400: 6520 3d3d 2031 3a0a 2020 2020 2020 2020  e == 1:.        
-00007410: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00007420: 2e63 772e 7370 6565 6420 2b3d 2031 0a20  .cw.speed += 1. 
-00007430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007440: 2020 2073 656c 662e 6377 5f73 7065 6564     self.cw_speed
-00007450: 2e73 6574 5661 6c75 6528 7365 6c66 2e63  .setValue(self.c
-00007460: 772e 7370 6565 6429 0a20 2020 2020 2020  w.speed).       
-00007470: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00007480: 662e 6377 2e73 656e 6463 7728 6622 5c78  f.cw.sendcw(f"\x
-00007490: 3162 327b 7365 6c66 2e63 772e 7370 6565  1b2{self.cw.spee
-000074a0: 647d 2229 0a20 2020 2020 2020 2020 2020  d}").           
-000074b0: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
-000074c0: 2020 2020 2020 2020 6966 2065 7665 6e74          if event
-000074d0: 2e6b 6579 2829 203d 3d20 5174 2e4b 6579  .key() == Qt.Key
-000074e0: 2e4b 6579 5f50 6167 6544 6f77 6e20 616e  .Key_PageDown an
-000074f0: 6420 6d6f 6469 6669 6572 2021 3d20 5174  d modifier != Qt
-00007500: 2e43 6f6e 7472 6f6c 4d6f 6469 6669 6572  .ControlModifier
-00007510: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00007520: 2073 656c 662e 6377 2069 7320 6e6f 7420   self.cw is not 
-00007530: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00007540: 2020 2020 2020 6966 2073 656c 662e 6377        if self.cw
-00007550: 2e73 6572 7665 7274 7970 6520 3d3d 2031  .servertype == 1
-00007560: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00007570: 2020 2020 2020 7365 6c66 2e63 772e 7370        self.cw.sp
-00007580: 6565 6420 2d3d 2031 0a20 2020 2020 2020  eed -= 1.       
-00007590: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000075a0: 662e 6377 5f73 7065 6564 2e73 6574 5661  f.cw_speed.setVa
-000075b0: 6c75 6528 7365 6c66 2e63 772e 7370 6565  lue(self.cw.spee
-000075c0: 6429 0a20 2020 2020 2020 2020 2020 2020  d).             
-000075d0: 2020 2020 2020 2073 656c 662e 6377 2e73         self.cw.s
-000075e0: 656e 6463 7728 6622 5c78 3162 327b 7365  endcw(f"\x1b2{se
-000075f0: 6c66 2e63 772e 7370 6565 647d 2229 0a20  lf.cw.speed}"). 
-00007600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007610: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
-00007620: 2020 2320 6966 2065 7665 6e74 2e6b 6579    # if event.key
-00007630: 2829 203d 3d20 5174 2e4b 6579 2e4b 6579  () == Qt.Key.Key
-00007640: 5f45 6e74 6572 3a0a 2020 2020 2020 2020  _Enter:.        
-00007650: 2320 2020 2020 7365 6c66 2e73 6176 655f  #     self.save_
-00007660: 636f 6e74 6163 7428 290a 2020 2020 2020  contact().      
-00007670: 2020 6966 2065 7665 6e74 2e6b 6579 2829    if event.key()
-00007680: 203d 3d20 5174 2e4b 6579 2e4b 6579 5f54   == Qt.Key.Key_T
-00007690: 6162 206f 7220 6576 656e 742e 6b65 7928  ab or event.key(
-000076a0: 2920 3d3d 2051 742e 4b65 792e 4b65 795f  ) == Qt.Key.Key_
-000076b0: 4261 636b 7461 623a 0a20 2020 2020 2020  Backtab:.       
-000076c0: 2020 2020 2069 6620 7365 6c66 2e73 656e       if self.sen
-000076d0: 742e 6861 7346 6f63 7573 2829 3a0a 2020  t.hasFocus():.  
-000076e0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-000076f0: 6767 6572 2e64 6562 7567 2822 4672 6f6d  gger.debug("From
-00007700: 2073 656e 7422 290a 2020 2020 2020 2020   sent").        
-00007710: 2020 2020 2020 2020 6966 206d 6f64 6966          if modif
-00007720: 6965 7220 3d3d 2051 742e 5368 6966 744d  ier == Qt.ShiftM
-00007730: 6f64 6966 6965 723a 0a20 2020 2020 2020  odifier:.       
-00007740: 2020 2020 2020 2020 2020 2020 2070 7265               pre
-00007750: 765f 7461 6220 3d20 7365 6c66 2e74 6162  v_tab = self.tab
-00007760: 5f70 7265 762e 6765 7428 7365 6c66 2e73  _prev.get(self.s
-00007770: 656e 7429 0a20 2020 2020 2020 2020 2020  ent).           
-00007780: 2020 2020 2020 2020 2070 7265 765f 7461           prev_ta
-00007790: 622e 7365 7446 6f63 7573 2829 0a20 2020  b.setFocus().   
-000077a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000077b0: 2070 7265 765f 7461 622e 6465 7365 6c65   prev_tab.desele
-000077c0: 6374 2829 0a20 2020 2020 2020 2020 2020  ct().           
-000077d0: 2020 2020 2020 2020 2070 7265 765f 7461           prev_ta
-000077e0: 622e 656e 6428 4661 6c73 6529 0a20 2020  b.end(False).   
-000077f0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-00007800: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00007810: 2020 2020 2020 206e 6578 745f 7461 6220         next_tab 
-00007820: 3d20 7365 6c66 2e74 6162 5f6e 6578 742e  = self.tab_next.
-00007830: 6765 7428 7365 6c66 2e73 656e 7429 0a20  get(self.sent). 
-00007840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007850: 2020 206e 6578 745f 7461 622e 7365 7446     next_tab.setF
-00007860: 6f63 7573 2829 0a20 2020 2020 2020 2020  ocus().         
-00007870: 2020 2020 2020 2020 2020 206e 6578 745f             next_
-00007880: 7461 622e 6465 7365 6c65 6374 2829 0a20  tab.deselect(). 
-00007890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078a0: 2020 206e 6578 745f 7461 622e 656e 6428     next_tab.end(
-000078b0: 4661 6c73 6529 0a20 2020 2020 2020 2020  False).         
-000078c0: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
-000078d0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-000078e0: 662e 7265 6365 6976 652e 6861 7346 6f63  f.receive.hasFoc
-000078f0: 7573 2829 3a0a 2020 2020 2020 2020 2020  us():.          
-00007900: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-00007910: 7567 2822 4672 6f6d 2072 6563 6569 7665  ug("From receive
-00007920: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-00007930: 2020 2069 6620 6d6f 6469 6669 6572 203d     if modifier =
-00007940: 3d20 5174 2e53 6869 6674 4d6f 6469 6669  = Qt.ShiftModifi
-00007950: 6572 3a0a 2020 2020 2020 2020 2020 2020  er:.            
-00007960: 2020 2020 2020 2020 7072 6576 5f74 6162          prev_tab
-00007970: 203d 2073 656c 662e 7461 625f 7072 6576   = self.tab_prev
-00007980: 2e67 6574 2873 656c 662e 7265 6365 6976  .get(self.receiv
-00007990: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
-000079a0: 2020 2020 2020 2070 7265 765f 7461 622e         prev_tab.
-000079b0: 7365 7446 6f63 7573 2829 0a20 2020 2020  setFocus().     
-000079c0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-000079d0: 7265 765f 7461 622e 6465 7365 6c65 6374  rev_tab.deselect
-000079e0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-000079f0: 2020 2020 2020 2070 7265 765f 7461 622e         prev_tab.
-00007a00: 656e 6428 4661 6c73 6529 0a20 2020 2020  end(False).     
-00007a10: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00007a20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007a30: 2020 2020 206e 6578 745f 7461 6220 3d20       next_tab = 
-00007a40: 7365 6c66 2e74 6162 5f6e 6578 742e 6765  self.tab_next.ge
-00007a50: 7428 7365 6c66 2e72 6563 6569 7665 290a  t(self.receive).
-00007a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a70: 2020 2020 6e65 7874 5f74 6162 2e73 6574      next_tab.set
-00007a80: 466f 6375 7328 290a 2020 2020 2020 2020  Focus().        
-00007a90: 2020 2020 2020 2020 2020 2020 6e65 7874              next
-00007aa0: 5f74 6162 2e64 6573 656c 6563 7428 290a  _tab.deselect().
-00007ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ac0: 2020 2020 6e65 7874 5f74 6162 2e65 6e64      next_tab.end
-00007ad0: 2846 616c 7365 290a 2020 2020 2020 2020  (False).        
-00007ae0: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
-00007af0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00007b00: 6c66 2e6f 7468 6572 5f31 2e68 6173 466f  lf.other_1.hasFo
-00007b10: 6375 7328 293a 0a20 2020 2020 2020 2020  cus():.         
-00007b20: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-00007b30: 6275 6728 2246 726f 6d20 6f74 6865 725f  bug("From other_
-00007b40: 3122 290a 2020 2020 2020 2020 2020 2020  1").            
-00007b50: 2020 2020 6966 206d 6f64 6966 6965 7220      if modifier 
-00007b60: 3d3d 2051 742e 5368 6966 744d 6f64 6966  == Qt.ShiftModif
-00007b70: 6965 723a 0a20 2020 2020 2020 2020 2020  ier:.           
-00007b80: 2020 2020 2020 2020 2070 7265 765f 7461           prev_ta
-00007b90: 6220 3d20 7365 6c66 2e74 6162 5f70 7265  b = self.tab_pre
-00007ba0: 762e 6765 7428 7365 6c66 2e6f 7468 6572  v.get(self.other
-00007bb0: 5f31 290a 2020 2020 2020 2020 2020 2020  _1).            
-00007bc0: 2020 2020 2020 2020 7072 6576 5f74 6162          prev_tab
-00007bd0: 2e73 6574 466f 6375 7328 290a 2020 2020  .setFocus().    
-00007be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007bf0: 7072 6576 5f74 6162 2e64 6573 656c 6563  prev_tab.deselec
-00007c00: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
-00007c10: 2020 2020 2020 2020 7072 6576 5f74 6162          prev_tab
-00007c20: 2e65 6e64 2846 616c 7365 290a 2020 2020  .end(False).    
-00007c30: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00007c40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00007c50: 2020 2020 2020 6e65 7874 5f74 6162 203d        next_tab =
-00007c60: 2073 656c 662e 7461 625f 6e65 7874 2e67   self.tab_next.g
-00007c70: 6574 2873 656c 662e 6f74 6865 725f 3129  et(self.other_1)
-00007c80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007c90: 2020 2020 206e 6578 745f 7461 622e 7365       next_tab.se
-00007ca0: 7446 6f63 7573 2829 0a20 2020 2020 2020  tFocus().       
-00007cb0: 2020 2020 2020 2020 2020 2020 206e 6578               nex
-00007cc0: 745f 7461 622e 6465 7365 6c65 6374 2829  t_tab.deselect()
-00007cd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007ce0: 2020 2020 206e 6578 745f 7461 622e 656e       next_tab.en
-00007cf0: 6428 4661 6c73 6529 0a20 2020 2020 2020  d(False).       
-00007d00: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
-00007d10: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00007d20: 656c 662e 6f74 6865 725f 322e 6861 7346  elf.other_2.hasF
-00007d30: 6f63 7573 2829 3a0a 2020 2020 2020 2020  ocus():.        
-00007d40: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-00007d50: 6562 7567 2822 4672 6f6d 206f 7468 6572  ebug("From other
-00007d60: 5f32 2229 0a20 2020 2020 2020 2020 2020  _2").           
-00007d70: 2020 2020 2069 6620 6d6f 6469 6669 6572       if modifier
-00007d80: 203d 3d20 5174 2e53 6869 6674 4d6f 6469   == Qt.ShiftModi
-00007d90: 6669 6572 3a0a 2020 2020 2020 2020 2020  fier:.          
-00007da0: 2020 2020 2020 2020 2020 7072 6576 5f74            prev_t
-00007db0: 6162 203d 2073 656c 662e 7461 625f 7072  ab = self.tab_pr
-00007dc0: 6576 2e67 6574 2873 656c 662e 6f74 6865  ev.get(self.othe
-00007dd0: 725f 3229 0a20 2020 2020 2020 2020 2020  r_2).           
-00007de0: 2020 2020 2020 2020 2070 7265 765f 7461           prev_ta
-00007df0: 622e 7365 7446 6f63 7573 2829 0a20 2020  b.setFocus().   
-00007e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e10: 2070 7265 765f 7461 622e 6465 7365 6c65   prev_tab.desele
-00007e20: 6374 2829 0a20 2020 2020 2020 2020 2020  ct().           
-00007e30: 2020 2020 2020 2020 2070 7265 765f 7461           prev_ta
-00007e40: 622e 656e 6428 4661 6c73 6529 0a20 2020  b.end(False).   
-00007e50: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-00007e60: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00007e70: 2020 2020 2020 206e 6578 745f 7461 6220         next_tab 
-00007e80: 3d20 7365 6c66 2e74 6162 5f6e 6578 742e  = self.tab_next.
-00007e90: 6765 7428 7365 6c66 2e6f 7468 6572 5f32  get(self.other_2
-00007ea0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00007eb0: 2020 2020 2020 6e65 7874 5f74 6162 2e73        next_tab.s
-00007ec0: 6574 466f 6375 7328 290a 2020 2020 2020  etFocus().      
-00007ed0: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
-00007ee0: 7874 5f74 6162 2e64 6573 656c 6563 7428  xt_tab.deselect(
-00007ef0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00007f00: 2020 2020 2020 6e65 7874 5f74 6162 2e65        next_tab.e
-00007f10: 6e64 2846 616c 7365 290a 2020 2020 2020  nd(False).      
-00007f20: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00007f30: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00007f40: 7365 6c66 2e63 616c 6c73 6967 6e2e 6861  self.callsign.ha
-00007f50: 7346 6f63 7573 2829 3a0a 2020 2020 2020  sFocus():.      
-00007f60: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-00007f70: 2e64 6562 7567 2822 4672 6f6d 2063 616c  .debug("From cal
-00007f80: 6c73 6967 6e22 290a 2020 2020 2020 2020  lsign").        
-00007f90: 2020 2020 2020 2020 6966 206d 6f64 6966          if modif
-00007fa0: 6965 7220 3d3d 2051 742e 5368 6966 744d  ier == Qt.ShiftM
-00007fb0: 6f64 6966 6965 723a 0a20 2020 2020 2020  odifier:.       
-00007fc0: 2020 2020 2020 2020 2020 2020 2070 7265               pre
-00007fd0: 765f 7461 6220 3d20 7365 6c66 2e74 6162  v_tab = self.tab
-00007fe0: 5f70 7265 762e 6765 7428 7365 6c66 2e63  _prev.get(self.c
-00007ff0: 616c 6c73 6967 6e29 0a20 2020 2020 2020  allsign).       
-00008000: 2020 2020 2020 2020 2020 2020 2070 7265               pre
-00008010: 765f 7461 622e 7365 7446 6f63 7573 2829  v_tab.setFocus()
-00008020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008030: 2020 2020 2070 7265 765f 7461 622e 6465       prev_tab.de
-00008040: 7365 6c65 6374 2829 0a20 2020 2020 2020  select().       
-00008050: 2020 2020 2020 2020 2020 2020 2070 7265               pre
-00008060: 765f 7461 622e 656e 6428 4661 6c73 6529  v_tab.end(False)
-00008070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008080: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00008090: 2020 2020 2020 2020 2020 2074 6578 7420             text 
-000080a0: 3d20 7365 6c66 2e63 616c 6c73 6967 6e2e  = self.callsign.
-000080b0: 7465 7874 2829 0a20 2020 2020 2020 2020  text().         
-000080c0: 2020 2020 2020 2020 2020 2074 6578 7420             text 
-000080d0: 3d20 7465 7874 2e75 7070 6572 2829 0a20  = text.upper(). 
-000080e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000080f0: 2020 205f 7468 6574 6872 6561 6420 3d20     _thethread = 
-00008100: 7468 7265 6164 696e 672e 5468 7265 6164  threading.Thread
-00008110: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00008120: 2020 2020 2020 2020 2020 7461 7267 6574            target
-00008130: 3d73 656c 662e 6368 6563 6b5f 6361 6c6c  =self.check_call
-00008140: 7369 676e 322c 0a20 2020 2020 2020 2020  sign2,.         
-00008150: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00008160: 7267 733d 2874 6578 742c 292c 0a20 2020  rgs=(text,),.   
-00008170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008180: 2020 2020 2064 6165 6d6f 6e3d 5472 7565       daemon=True
-00008190: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000081a0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000081b0: 2020 2020 2020 2020 2020 2020 5f74 6865              _the
-000081c0: 7468 7265 6164 2e73 7461 7274 2829 0a20  thread.start(). 
-000081d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000081e0: 2020 206e 6578 745f 7461 6220 3d20 7365     next_tab = se
-000081f0: 6c66 2e74 6162 5f6e 6578 742e 6765 7428  lf.tab_next.get(
-00008200: 7365 6c66 2e63 616c 6c73 6967 6e29 0a20  self.callsign). 
-00008210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008220: 2020 206e 6578 745f 7461 622e 7365 7446     next_tab.setF
-00008230: 6f63 7573 2829 0a20 2020 2020 2020 2020  ocus().         
-00008240: 2020 2020 2020 2020 2020 206e 6578 745f             next_
-00008250: 7461 622e 6465 7365 6c65 6374 2829 0a20  tab.deselect(). 
-00008260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008270: 2020 206e 6578 745f 7461 622e 656e 6428     next_tab.end(
-00008280: 4661 6c73 6529 0a20 2020 2020 2020 2020  False).         
-00008290: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
-000082a0: 2020 2020 2020 6966 2065 7665 6e74 2e6b        if event.k
-000082b0: 6579 2829 203d 3d20 5174 2e4b 6579 5f46  ey() == Qt.Key_F
-000082c0: 313a 0a20 2020 2020 2020 2020 2020 2073  1:.            s
-000082d0: 656c 662e 7365 6e64 6631 2829 0a20 2020  elf.sendf1().   
-000082e0: 2020 2020 2069 6620 6576 656e 742e 6b65       if event.ke
-000082f0: 7928 2920 3d3d 2051 742e 4b65 795f 4632  y() == Qt.Key_F2
-00008300: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00008310: 6c66 2e73 656e 6466 3228 290a 2020 2020  lf.sendf2().    
-00008320: 2020 2020 6966 2065 7665 6e74 2e6b 6579      if event.key
-00008330: 2829 203d 3d20 5174 2e4b 6579 5f46 333a  () == Qt.Key_F3:
-00008340: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00008350: 662e 7365 6e64 6633 2829 0a20 2020 2020  f.sendf3().     
-00008360: 2020 2069 6620 6576 656e 742e 6b65 7928     if event.key(
-00008370: 2920 3d3d 2051 742e 4b65 795f 4634 3a0a  ) == Qt.Key_F4:.
-00008380: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00008390: 2e73 656e 6466 3428 290a 2020 2020 2020  .sendf4().      
-000083a0: 2020 6966 2065 7665 6e74 2e6b 6579 2829    if event.key()
-000083b0: 203d 3d20 5174 2e4b 6579 5f46 353a 0a20   == Qt.Key_F5:. 
-000083c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000083d0: 7365 6e64 6635 2829 0a20 2020 2020 2020  sendf5().       
-000083e0: 2069 6620 6576 656e 742e 6b65 7928 2920   if event.key() 
-000083f0: 3d3d 2051 742e 4b65 795f 4636 3a0a 2020  == Qt.Key_F6:.  
-00008400: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-00008410: 656e 6466 3628 290a 2020 2020 2020 2020  endf6().        
-00008420: 6966 2065 7665 6e74 2e6b 6579 2829 203d  if event.key() =
-00008430: 3d20 5174 2e4b 6579 5f46 373a 0a20 2020  = Qt.Key_F7:.   
-00008440: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-00008450: 6e64 6637 2829 0a20 2020 2020 2020 2069  ndf7().        i
-00008460: 6620 6576 656e 742e 6b65 7928 2920 3d3d  f event.key() ==
-00008470: 2051 742e 4b65 795f 4638 3a0a 2020 2020   Qt.Key_F8:.    
-00008480: 2020 2020 2020 2020 7365 6c66 2e73 656e          self.sen
-00008490: 6466 3828 290a 2020 2020 2020 2020 6966  df8().        if
-000084a0: 2065 7665 6e74 2e6b 6579 2829 203d 3d20   event.key() == 
-000084b0: 5174 2e4b 6579 5f46 393a 0a20 2020 2020  Qt.Key_F9:.     
-000084c0: 2020 2020 2020 2073 656c 662e 7365 6e64         self.send
-000084d0: 6639 2829 0a20 2020 2020 2020 2069 6620  f9().        if 
-000084e0: 6576 656e 742e 6b65 7928 2920 3d3d 2051  event.key() == Q
-000084f0: 742e 4b65 795f 4631 303a 0a20 2020 2020  t.Key_F10:.     
-00008500: 2020 2020 2020 2073 656c 662e 7365 6e64         self.send
-00008510: 6631 3028 290a 2020 2020 2020 2020 6966  f10().        if
-00008520: 2065 7665 6e74 2e6b 6579 2829 203d 3d20   event.key() == 
-00008530: 5174 2e4b 6579 5f46 3131 3a0a 2020 2020  Qt.Key_F11:.    
-00008540: 2020 2020 2020 2020 7365 6c66 2e73 656e          self.sen
-00008550: 6466 3131 2829 0a20 2020 2020 2020 2069  df11().        i
-00008560: 6620 6576 656e 742e 6b65 7928 2920 3d3d  f event.key() ==
-00008570: 2051 742e 4b65 795f 4631 323a 0a20 2020   Qt.Key_F12:.   
-00008580: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-00008590: 6e64 6631 3228 290a 0a20 2020 2064 6566  ndf12()..    def
-000085a0: 2073 6574 5f77 696e 646f 775f 7469 746c   set_window_titl
-000085b0: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-000085c0: 2022 2222 5365 7420 7769 6e64 6f77 2074   """Set window t
-000085d0: 6974 6c65 2222 220a 2020 2020 2020 2020  itle""".        
-000085e0: 7666 6f61 203d 2073 656c 662e 7261 6469  vfoa = self.radi
-000085f0: 6f5f 7374 6174 652e 6765 7428 2276 666f  o_state.get("vfo
-00008600: 6122 2c20 2222 290a 2020 2020 2020 2020  a", "").        
-00008610: 6966 2076 666f 613a 0a20 2020 2020 2020  if vfoa:.       
-00008620: 2020 2020 2076 666f 6120 3d20 696e 7428       vfoa = int(
-00008630: 7666 6f61 2920 2f20 3130 3030 0a20 2020  vfoa) / 1000.   
-00008640: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00008650: 2020 2020 2020 2076 666f 6120 3d20 302e         vfoa = 0.
-00008660: 300a 2020 2020 2020 2020 636f 6e74 6573  0.        contes
-00008670: 745f 6e61 6d65 203d 2022 220a 2020 2020  t_name = "".    
-00008680: 2020 2020 6966 2073 656c 662e 636f 6e74      if self.cont
-00008690: 6573 743a 0a20 2020 2020 2020 2020 2020  est:.           
-000086a0: 2063 6f6e 7465 7374 5f6e 616d 6520 3d20   contest_name = 
-000086b0: 7365 6c66 2e63 6f6e 7465 7374 2e6e 616d  self.contest.nam
-000086c0: 650a 2020 2020 2020 2020 6c69 6e65 203d  e.        line =
-000086d0: 2028 0a20 2020 2020 2020 2020 2020 2066   (.            f
-000086e0: 2276 666f 613a 7b72 6f75 6e64 2876 666f  "vfoa:{round(vfo
-000086f0: 612c 3229 7d20 220a 2020 2020 2020 2020  a,2)} ".        
-00008700: 2020 2020 6622 6d6f 6465 3a7b 7365 6c66      f"mode:{self
-00008710: 2e72 6164 696f 5f73 7461 7465 2e67 6574  .radio_state.get
-00008720: 2827 6d6f 6465 272c 2027 2729 7d20 220a  ('mode', '')} ".
-00008730: 2020 2020 2020 2020 2020 2020 6622 4f50              f"OP
-00008740: 3a7b 7365 6c66 2e63 7572 7265 6e74 5f6f  :{self.current_o
-00008750: 707d 207b 636f 6e74 6573 745f 6e61 6d65  p} {contest_name
-00008760: 7d20 220a 2020 2020 2020 2020 2020 2020  } ".            
-00008770: 6622 2d20 4e6f 7431 4d4d 2076 7b5f 5f76  f"- Not1MM v{__v
-00008780: 6572 7369 6f6e 5f5f 7d22 0a20 2020 2020  ersion__}".     
-00008790: 2020 2029 0a20 2020 2020 2020 206c 6f67     ).        log
-000087a0: 6765 722e 6465 6275 6728 2225 7322 2c20  ger.debug("%s", 
-000087b0: 6c69 6e65 290a 2020 2020 2020 2020 7365  line).        se
-000087c0: 6c66 2e73 6574 5769 6e64 6f77 5469 746c  lf.setWindowTitl
-000087d0: 6528 6c69 6e65 290a 0a20 2020 2064 6566  e(line)..    def
-000087e0: 2063 6c65 6172 696e 7075 7473 2873 656c   clearinputs(sel
-000087f0: 6629 3a0a 2020 2020 2020 2020 2222 2243  f):.        """C
-00008800: 6c65 6172 7320 7468 6520 7465 7874 2069  lears the text i
-00008810: 6e70 7574 2066 6965 6c64 7320 616e 6420  nput fields and 
-00008820: 7365 7473 2066 6f63 7573 2074 6f20 6361  sets focus to ca
-00008830: 6c6c 7369 676e 2066 6965 6c64 2e22 2222  llsign field."""
-00008840: 0a20 2020 2020 2020 2073 656c 662e 6475  .        self.du
-00008850: 7065 5f69 6e64 6963 6174 6f72 2e68 6964  pe_indicator.hid
-00008860: 6528 290a 2020 2020 2020 2020 7365 6c66  e().        self
-00008870: 2e63 6f6e 7461 6374 203d 2073 656c 662e  .contact = self.
-00008880: 6461 7461 6261 7365 2e65 6d70 7479 5f63  database.empty_c
-00008890: 6f6e 7461 6374 0a20 2020 2020 2020 2073  ontact.        s
-000088a0: 656c 662e 6865 6164 696e 675f 6469 7374  elf.heading_dist
-000088b0: 616e 6365 2e73 6574 5465 7874 2822 2229  ance.setText("")
-000088c0: 0a20 2020 2020 2020 2073 656c 662e 6478  .        self.dx
-000088d0: 5f65 6e74 6974 792e 7365 7454 6578 7428  _entity.setText(
-000088e0: 2222 290a 2020 2020 2020 2020 6966 2073  "").        if s
-000088f0: 656c 662e 636f 6e74 6573 743a 0a20 2020  elf.contest:.   
-00008900: 2020 2020 2020 2020 206d 756c 7473 203d           mults =
-00008910: 2073 656c 662e 636f 6e74 6573 742e 7368   self.contest.sh
-00008920: 6f77 5f6d 756c 7473 2873 656c 6629 0a20  ow_mults(self). 
-00008930: 2020 2020 2020 2020 2020 2071 736f 7320             qsos 
-00008940: 3d20 7365 6c66 2e63 6f6e 7465 7374 2e73  = self.contest.s
-00008950: 686f 775f 7173 6f28 7365 6c66 290a 2020  how_qso(self).  
-00008960: 2020 2020 2020 2020 2020 6d75 6c74 7374            multst
-00008970: 7269 6e67 203d 2066 227b 7173 6f73 7d2f  ring = f"{qsos}/
-00008980: 7b6d 756c 7473 7d22 0a20 2020 2020 2020  {mults}".       
-00008990: 2020 2020 2073 656c 662e 6d75 6c74 732e       self.mults.
-000089a0: 7365 7454 6578 7428 6d75 6c74 7374 7269  setText(multstri
-000089b0: 6e67 290a 2020 2020 2020 2020 2020 2020  ng).            
-000089c0: 7363 6f72 6520 3d20 7365 6c66 2e63 6f6e  score = self.con
-000089d0: 7465 7374 2e63 616c 635f 7363 6f72 6528  test.calc_score(
-000089e0: 7365 6c66 290a 2020 2020 2020 2020 2020  self).          
-000089f0: 2020 7365 6c66 2e73 636f 7265 2e73 6574    self.score.set
-00008a00: 5465 7874 2873 7472 2873 636f 7265 2929  Text(str(score))
-00008a10: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00008a20: 662e 636f 6e74 6573 742e 7265 7365 745f  f.contest.reset_
-00008a30: 6c61 6265 6c28 7365 6c66 290a 2020 2020  label(self).    
-00008a40: 2020 2020 7365 6c66 2e63 616c 6c73 6967      self.callsig
-00008a50: 6e2e 636c 6561 7228 290a 2020 2020 2020  n.clear().      
-00008a60: 2020 6966 2073 656c 662e 6375 7272 656e    if self.curren
-00008a70: 745f 6d6f 6465 203d 3d20 2243 5722 3a0a  t_mode == "CW":.
-00008a80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00008a90: 2e73 656e 742e 7365 7454 6578 7428 2235  .sent.setText("5
-00008aa0: 3939 2229 0a20 2020 2020 2020 2020 2020  99").           
-00008ab0: 2073 656c 662e 7265 6365 6976 652e 7365   self.receive.se
-00008ac0: 7454 6578 7428 2235 3939 2229 0a20 2020  tText("599").   
-00008ad0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00008ae0: 2020 2020 2020 2073 656c 662e 7365 6e74         self.sent
-00008af0: 2e73 6574 5465 7874 2822 3539 2229 0a20  .setText("59"). 
-00008b00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00008b10: 7265 6365 6976 652e 7365 7454 6578 7428  receive.setText(
-00008b20: 2235 3922 290a 2020 2020 2020 2020 7365  "59").        se
-00008b30: 6c66 2e6f 7468 6572 5f31 2e63 6c65 6172  lf.other_1.clear
-00008b40: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-00008b50: 6f74 6865 725f 322e 636c 6561 7228 290a  other_2.clear().
-00008b60: 2020 2020 2020 2020 7365 6c66 2e63 616c          self.cal
-00008b70: 6c73 6967 6e2e 7365 7446 6f63 7573 2829  lsign.setFocus()
-00008b80: 0a20 2020 2020 2020 2063 6d64 203d 207b  .        cmd = {
-00008b90: 7d0a 2020 2020 2020 2020 636d 645b 2263  }.        cmd["c
-00008ba0: 6d64 225d 203d 2022 4341 4c4c 4348 414e  md"] = "CALLCHAN
-00008bb0: 4745 4422 0a20 2020 2020 2020 2063 6d64  GED".        cmd
-00008bc0: 5b22 7374 6174 696f 6e22 5d20 3d20 706c  ["station"] = pl
-00008bd0: 6174 666f 726d 2e6e 6f64 6528 290a 2020  atform.node().  
-00008be0: 2020 2020 2020 636d 645b 2263 616c 6c22        cmd["call"
-00008bf0: 5d20 3d20 2222 0a20 2020 2020 2020 2073  ] = "".        s
-00008c00: 656c 662e 6d75 6c74 6963 6173 745f 696e  elf.multicast_in
-00008c10: 7465 7266 6163 652e 7365 6e64 5f61 735f  terface.send_as_
-00008c20: 6a73 6f6e 2863 6d64 290a 0a20 2020 2064  json(cmd)..    d
-00008c30: 6566 2073 6176 655f 636f 6e74 6163 7428  ef save_contact(
-00008c40: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-00008c50: 2222 5361 7665 2074 6f20 6462 2222 220a  ""Save to db""".
-00008c60: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-00008c70: 6562 7567 2822 7361 7669 6e67 2063 6f6e  ebug("saving con
-00008c80: 7461 6374 2229 0a20 2020 2020 2020 2069  tact").        i
-00008c90: 6620 6c65 6e28 7365 6c66 2e63 616c 6c73  f len(self.calls
-00008ca0: 6967 6e2e 7465 7874 2829 2920 3c20 333a  ign.text()) < 3:
-00008cb0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00008cc0: 7572 6e0a 2020 2020 2020 2020 6966 206e  urn.        if n
-00008cd0: 6f74 2061 6e79 2863 6861 722e 6973 6469  ot any(char.isdi
-00008ce0: 6769 7428 2920 666f 7220 6368 6172 2069  git() for char i
-00008cf0: 6e20 7365 6c66 2e63 616c 6c73 6967 6e2e  n self.callsign.
-00008d00: 7465 7874 2829 293a 0a20 2020 2020 2020  text()):.       
-00008d10: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
-00008d20: 2020 2020 6966 206e 6f74 2061 6e79 2863      if not any(c
-00008d30: 6861 722e 6973 616c 7068 6128 2920 666f  har.isalpha() fo
-00008d40: 7220 6368 6172 2069 6e20 7365 6c66 2e63  r char in self.c
-00008d50: 616c 6c73 6967 6e2e 7465 7874 2829 293a  allsign.text()):
-00008d60: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00008d70: 7572 6e0a 0a20 2020 2020 2020 2073 656c  urn..        sel
-00008d80: 662e 636f 6e74 6163 745b 2254 5322 5d20  f.contact["TS"] 
-00008d90: 3d20 6461 7465 7469 6d65 2e75 7463 6e6f  = datetime.utcno
-00008da0: 7728 292e 6973 6f66 6f72 6d61 7428 2220  w().isoformat(" 
-00008db0: 2229 5b3a 3139 5d0a 2020 2020 2020 2020  ")[:19].        
-00008dc0: 7365 6c66 2e63 6f6e 7461 6374 5b22 4361  self.contact["Ca
-00008dd0: 6c6c 225d 203d 2073 656c 662e 6361 6c6c  ll"] = self.call
-00008de0: 7369 676e 2e74 6578 7428 290a 2020 2020  sign.text().    
-00008df0: 2020 2020 7365 6c66 2e63 6f6e 7461 6374      self.contact
-00008e00: 5b22 4672 6571 225d 203d 2072 6f75 6e64  ["Freq"] = round
-00008e10: 2866 6c6f 6174 2873 656c 662e 7261 6469  (float(self.radi
-00008e20: 6f5f 7374 6174 652e 6765 7428 2276 666f  o_state.get("vfo
-00008e30: 6122 2c20 302e 3029 2920 2f20 3130 3030  a", 0.0)) / 1000
-00008e40: 2c20 3229 0a20 2020 2020 2020 2073 656c  , 2).        sel
-00008e50: 662e 636f 6e74 6163 745b 2251 5358 4672  f.contact["QSXFr
-00008e60: 6571 225d 203d 2072 6f75 6e64 280a 2020  eq"] = round(.  
-00008e70: 2020 2020 2020 2020 2020 666c 6f61 7428            float(
-00008e80: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
-00008e90: 2e67 6574 2822 7666 6f61 222c 2030 2e30  .get("vfoa", 0.0
-00008ea0: 2929 202f 2031 3030 302c 2032 0a20 2020  )) / 1000, 2.   
-00008eb0: 2020 2020 2029 0a20 2020 2020 2020 2073       ).        s
-00008ec0: 656c 662e 636f 6e74 6163 745b 224d 6f64  elf.contact["Mod
-00008ed0: 6522 5d20 3d20 7365 6c66 2e72 6164 696f  e"] = self.radio
-00008ee0: 5f73 7461 7465 2e67 6574 2822 6d6f 6465  _state.get("mode
-00008ef0: 222c 2022 2229 0a20 2020 2020 2020 2073  ", "").        s
-00008f00: 656c 662e 636f 6e74 6163 745b 2243 6f6e  elf.contact["Con
-00008f10: 7465 7374 4e61 6d65 225d 203d 2073 656c  testName"] = sel
-00008f20: 662e 636f 6e74 6573 742e 6361 6272 696c  f.contest.cabril
-00008f30: 6c6f 5f6e 616d 650a 2020 2020 2020 2020  lo_name.        
-00008f40: 7365 6c66 2e63 6f6e 7461 6374 5b22 436f  self.contact["Co
-00008f50: 6e74 6573 744e 5222 5d20 3d20 7365 6c66  ntestNR"] = self
-00008f60: 2e70 7265 662e 6765 7428 2263 6f6e 7465  .pref.get("conte
-00008f70: 7374 222c 2022 3022 290a 2020 2020 2020  st", "0").      
-00008f80: 2020 7365 6c66 2e63 6f6e 7461 6374 5b22    self.contact["
-00008f90: 5374 6174 696f 6e50 7265 6669 7822 5d20  StationPrefix"] 
-00008fa0: 3d20 7365 6c66 2e73 7461 7469 6f6e 2e67  = self.station.g
-00008fb0: 6574 2822 4361 6c6c 222c 2022 2229 0a20  et("Call", ""). 
-00008fc0: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
-00008fd0: 6163 745b 2257 5058 5072 6566 6978 225d  act["WPXPrefix"]
-00008fe0: 203d 2063 616c 6375 6c61 7465 5f77 7078   = calculate_wpx
-00008ff0: 5f70 7265 6669 7828 7365 6c66 2e63 616c  _prefix(self.cal
-00009000: 6c73 6967 6e2e 7465 7874 2829 290a 2020  lsign.text()).  
-00009010: 2020 2020 2020 7365 6c66 2e63 6f6e 7461        self.conta
-00009020: 6374 5b22 4973 5275 6e51 534f 225d 203d  ct["IsRunQSO"] =
-00009030: 2073 656c 662e 7261 6469 6f42 7574 746f   self.radioButto
-00009040: 6e5f 7275 6e2e 6973 4368 6563 6b65 6428  n_run.isChecked(
-00009050: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
-00009060: 6f6e 7461 6374 5b22 4f70 6572 6174 6f72  ontact["Operator
-00009070: 225d 203d 2073 656c 662e 6375 7272 656e  "] = self.curren
-00009080: 745f 6f70 0a20 2020 2020 2020 2073 656c  t_op.        sel
-00009090: 662e 636f 6e74 6163 745b 224e 6574 4269  f.contact["NetBi
-000090a0: 6f73 4e61 6d65 225d 203d 2073 6f63 6b65  osName"] = socke
-000090b0: 742e 6765 7468 6f73 746e 616d 6528 290a  t.gethostname().
-000090c0: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-000090d0: 7461 6374 5b22 4973 4f72 6967 696e 616c  tact["IsOriginal
-000090e0: 225d 203d 2031 0a20 2020 2020 2020 2073  "] = 1.        s
-000090f0: 656c 662e 636f 6e74 6163 745b 2249 4422  elf.contact["ID"
-00009100: 5d20 3d20 7575 6964 2e75 7569 6434 2829  ] = uuid.uuid4()
-00009110: 2e68 6578 0a20 2020 2020 2020 2073 656c  .hex.        sel
-00009120: 662e 636f 6e74 6573 742e 7365 745f 636f  f.contest.set_co
-00009130: 6e74 6163 745f 7661 7273 2873 656c 6629  ntact_vars(self)
-00009140: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
-00009150: 6e74 6163 745b 2250 6f69 6e74 7322 5d20  ntact["Points"] 
-00009160: 3d20 7365 6c66 2e63 6f6e 7465 7374 2e70  = self.contest.p
-00009170: 6f69 6e74 7328 7365 6c66 290a 2020 2020  oints(self).    
-00009180: 2020 2020 6465 6275 675f 6f75 7470 7574      debug_output
-00009190: 203d 2066 227b 7365 6c66 2e63 6f6e 7461   = f"{self.conta
-000091a0: 6374 7d22 0a20 2020 2020 2020 206c 6f67  ct}".        log
-000091b0: 6765 722e 6465 6275 6728 6465 6275 675f  ger.debug(debug_
-000091c0: 6f75 7470 7574 290a 2020 2020 2020 2020  output).        
-000091d0: 7365 6c66 2e64 6174 6162 6173 652e 6c6f  self.database.lo
-000091e0: 675f 636f 6e74 6163 7428 7365 6c66 2e63  g_contact(self.c
-000091f0: 6f6e 7461 6374 290a 2020 2020 2020 2020  ontact).        
-00009200: 7365 6c66 2e6e 316d 6d2e 7365 6e64 5f63  self.n1mm.send_c
-00009210: 6f6e 7461 6374 5f69 6e66 6f28 290a 2020  ontact_info().  
-00009220: 2020 2020 2020 7365 6c66 2e63 6c65 6172        self.clear
-00009230: 696e 7075 7473 2829 0a20 2020 2020 2020  inputs().       
-00009240: 2063 6d64 203d 207b 7d0a 2020 2020 2020   cmd = {}.      
-00009250: 2020 636d 645b 2263 6d64 225d 203d 2022    cmd["cmd"] = "
-00009260: 5550 4441 5445 4c4f 4722 0a20 2020 2020  UPDATELOG".     
-00009270: 2020 2063 6d64 5b22 7374 6174 696f 6e22     cmd["station"
-00009280: 5d20 3d20 706c 6174 666f 726d 2e6e 6f64  ] = platform.nod
-00009290: 6528 290a 2020 2020 2020 2020 7365 6c66  e().        self
-000092a0: 2e6d 756c 7469 6361 7374 5f69 6e74 6572  .multicast_inter
-000092b0: 6661 6365 2e73 656e 645f 6173 5f6a 736f  face.send_as_jso
-000092c0: 6e28 636d 6429 0a20 2020 2020 2020 2023  n(cmd).        #
-000092d0: 2073 656c 662e 636f 6e74 6163 745b 2243   self.contact["C
-000092e0: 6f6e 7465 7374 4e61 6d65 225d 203d 2073  ontestName"] = s
-000092f0: 656c 662e 636f 6e74 6573 742e 6e61 6d65  elf.contest.name
-00009300: 0a20 2020 2020 2020 2023 2073 656c 662e  .        # self.
-00009310: 636f 6e74 6163 745b 2253 4e54 225d 203d  contact["SNT"] =
-00009320: 2073 656c 662e 7365 6e74 2e74 6578 7428   self.sent.text(
-00009330: 290a 2020 2020 2020 2020 2320 7365 6c66  ).        # self
-00009340: 2e63 6f6e 7461 6374 5b22 5243 5622 5d20  .contact["RCV"] 
-00009350: 3d20 7365 6c66 2e72 6563 6569 7665 2e74  = self.receive.t
-00009360: 6578 7428 290a 2020 2020 2020 2020 2320  ext().        # 
-00009370: 7365 6c66 2e63 6f6e 7461 6374 5b22 436f  self.contact["Co
-00009380: 756e 7472 7950 7265 6669 7822 5d0a 2020  untryPrefix"].  
-00009390: 2020 2020 2020 2320 7365 6c66 2e63 6f6e        # self.con
-000093a0: 7461 6374 5b22 5374 6174 696f 6e50 7265  tact["StationPre
-000093b0: 6669 7822 5d20 3d20 7365 6c66 2e70 7265  fix"] = self.pre
-000093c0: 662e 6765 7428 2263 616c 6c73 6967 6e22  f.get("callsign"
-000093d0: 2c20 2222 290a 2020 2020 2020 2020 2320  , "").        # 
-000093e0: 7365 6c66 2e63 6f6e 7461 6374 5b22 5154  self.contact["QT
-000093f0: 4822 5d0a 2020 2020 2020 2020 2320 7365  H"].        # se
-00009400: 6c66 2e63 6f6e 7461 6374 5b22 4e61 6d65  lf.contact["Name
-00009410: 225d 203d 2073 656c 662e 6f74 6865 725f  "] = self.other_
-00009420: 312e 7465 7874 2829 0a20 2020 2020 2020  1.text().       
-00009430: 2023 2073 656c 662e 636f 6e74 6163 745b   # self.contact[
-00009440: 2243 6f6d 6d65 6e74 225d 203d 2073 656c  "Comment"] = sel
-00009450: 662e 6f74 6865 725f 322e 7465 7874 2829  f.other_2.text()
-00009460: 0a20 2020 2020 2020 2023 2073 656c 662e  .        # self.
-00009470: 636f 6e74 6163 745b 224e 5222 5d0a 2020  contact["NR"].  
-00009480: 2020 2020 2020 2320 7365 6c66 2e63 6f6e        # self.con
-00009490: 7461 6374 5b22 5365 6374 225d 0a20 2020  tact["Sect"].   
-000094a0: 2020 2020 2023 2073 656c 662e 636f 6e74       # self.cont
-000094b0: 6163 745b 2250 7265 6322 5d0a 2020 2020  act["Prec"].    
-000094c0: 2020 2020 2320 7365 6c66 2e63 6f6e 7461      # self.conta
-000094d0: 6374 5b22 434b 225d 0a20 2020 2020 2020  ct["CK"].       
-000094e0: 2023 2073 656c 662e 636f 6e74 6163 745b   # self.contact[
-000094f0: 225a 4e22 5d0a 2020 2020 2020 2020 2320  "ZN"].        # 
-00009500: 7365 6c66 2e63 6f6e 7461 6374 5b22 5365  self.contact["Se
-00009510: 6e74 4e72 225d 0a20 2020 2020 2020 2023  ntNr"].        #
-00009520: 2073 656c 662e 636f 6e74 6163 745b 2250   self.contact["P
-00009530: 6f69 6e74 7322 5d0a 2020 2020 2020 2020  oints"].        
-00009540: 2320 7365 6c66 2e63 6f6e 7461 6374 5b22  # self.contact["
-00009550: 4973 4d75 6c74 6970 6c69 6572 3122 5d0a  IsMultiplier1"].
-00009560: 2020 2020 2020 2020 2320 7365 6c66 2e63          # self.c
-00009570: 6f6e 7461 6374 5b22 4973 4d75 6c74 6970  ontact["IsMultip
-00009580: 6c69 6572 3222 5d0a 2020 2020 2020 2020  lier2"].        
-00009590: 2320 7365 6c66 2e63 6f6e 7461 6374 5b22  # self.contact["
-000095a0: 506f 7765 7222 5d0a 2020 2020 2020 2020  Power"].        
-000095b0: 2320 7365 6c66 2e63 6f6e 7461 6374 5b22  # self.contact["
-000095c0: 4261 6e64 225d 0a20 2020 2020 2020 2023  Band"].        #
-000095d0: 2073 656c 662e 636f 6e74 6163 745b 2257   self.contact["W
-000095e0: 5058 5072 6566 6978 225d 203d 2063 616c  PXPrefix"] = cal
-000095f0: 6375 6c61 7465 5f77 7078 5f70 7265 6669  culate_wpx_prefi
-00009600: 7828 7365 6c66 2e63 616c 6c73 6967 6e2e  x(self.callsign.
-00009610: 7465 7874 2829 290a 2020 2020 2020 2020  text()).        
-00009620: 2320 7365 6c66 2e63 6f6e 7461 6374 5b22  # self.contact["
-00009630: 4578 6368 616e 6765 3122 5d0a 2020 2020  Exchange1"].    
-00009640: 2020 2020 2320 7365 6c66 2e63 6f6e 7461      # self.conta
-00009650: 6374 5b22 5261 6469 6f4e 5222 5d0a 2020  ct["RadioNR"].  
-00009660: 2020 2020 2020 2320 7365 6c66 2e63 6f6e        # self.con
-00009670: 7461 6374 5b22 6973 4d75 6c74 6970 6c69  tact["isMultipli
-00009680: 6572 3322 5d0a 2020 2020 2020 2020 2320  er3"].        # 
-00009690: 7365 6c66 2e63 6f6e 7461 6374 5b22 4d69  self.contact["Mi
-000096a0: 7363 5465 7874 225d 0a20 2020 2020 2020  scText"].       
-000096b0: 2023 2073 656c 662e 636f 6e74 6163 745b   # self.contact[
-000096c0: 2243 6f6e 7461 6374 5479 7065 225d 0a20  "ContactType"]. 
-000096d0: 2020 2020 2020 2023 2073 656c 662e 636f         # self.co
-000096e0: 6e74 6163 745b 2252 756e 3152 756e 3222  ntact["Run1Run2"
-000096f0: 5d0a 2020 2020 2020 2020 2320 7365 6c66  ].        # self
-00009700: 2e63 6f6e 7461 6374 5b22 4772 6964 5371  .contact["GridSq
-00009710: 7561 7265 225d 0a20 2020 2020 2020 2023  uare"].        #
-00009720: 2073 656c 662e 636f 6e74 6163 745b 2243   self.contact["C
-00009730: 6f6e 7469 6e65 6e74 225d 0a20 2020 2020  ontinent"].     
-00009740: 2020 2023 2073 656c 662e 636f 6e74 6163     # self.contac
-00009750: 745b 2252 6f76 6572 4c6f 6361 7469 6f6e  t["RoverLocation
-00009760: 225d 0a20 2020 2020 2020 2023 2073 656c  "].        # sel
-00009770: 662e 636f 6e74 6163 745b 2252 6164 696f  f.contact["Radio
-00009780: 496e 7465 7266 6163 6564 225d 0a20 2020  Interfaced"].   
-00009790: 2020 2020 2023 2073 656c 662e 636f 6e74       # self.cont
-000097a0: 6163 745b 224e 6574 776f 726b 6564 436f  act["NetworkedCo
-000097b0: 6d70 4e72 225d 0a20 2020 2020 2020 2023  mpNr"].        #
-000097c0: 2073 656c 662e 636f 6e74 6163 745b 2243   self.contact["C
-000097d0: 4c41 494d 4544 5153 4f22 5d0a 0a20 2020  LAIMEDQSO"]..   
-000097e0: 2064 6566 206e 6577 5f63 6f6e 7465 7374   def new_contest
-000097f0: 5f64 6961 6c6f 6728 7365 6c66 293a 0a20  _dialog(self):. 
-00009800: 2020 2020 2020 2022 2222 5368 6f77 206e         """Show n
-00009810: 6577 2063 6f6e 7465 7374 2064 6961 6c6f  ew contest dialo
-00009820: 6722 2222 0a20 2020 2020 2020 206c 6f67  g""".        log
-00009830: 6765 722e 6465 6275 6728 224e 6577 2063  ger.debug("New c
-00009840: 6f6e 7465 7374 2044 6961 6c6f 6722 290a  ontest Dialog").
-00009850: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-00009860: 7465 7374 5f64 6961 6c6f 6720 3d20 4e65  test_dialog = Ne
-00009870: 7743 6f6e 7465 7374 2857 4f52 4b49 4e47  wContest(WORKING
-00009880: 5f50 4154 4829 0a20 2020 2020 2020 2073  _PATH).        s
-00009890: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-000098a0: 6f67 2e61 6363 6570 7465 642e 636f 6e6e  og.accepted.conn
-000098b0: 6563 7428 7365 6c66 2e73 6176 655f 636f  ect(self.save_co
-000098c0: 6e74 6573 7429 0a20 2020 2020 2020 2069  ntest).        i
-000098d0: 6620 7365 6c66 2e70 7265 662e 6765 7428  f self.pref.get(
-000098e0: 2264 6172 6b5f 6d6f 6465 2229 3a0a 2020  "dark_mode"):.  
-000098f0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00009900: 6f6e 7465 7374 5f64 6961 6c6f 672e 7365  ontest_dialog.se
-00009910: 7453 7479 6c65 5368 6565 7428 4441 524b  tStyleSheet(DARK
-00009920: 5f53 5459 4c45 5348 4545 5429 0a20 2020  _STYLESHEET).   
-00009930: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
-00009940: 745f 6469 616c 6f67 2e64 6174 6554 696d  t_dialog.dateTim
-00009950: 6545 6469 742e 7365 7444 6174 6528 5174  eEdit.setDate(Qt
-00009960: 436f 7265 2e51 4461 7465 2e63 7572 7265  Core.QDate.curre
-00009970: 6e74 4461 7465 2829 290a 2020 2020 2020  ntDate()).      
-00009980: 2020 7365 6c66 2e63 6f6e 7465 7374 5f64    self.contest_d
-00009990: 6961 6c6f 672e 6461 7465 5469 6d65 4564  ialog.dateTimeEd
-000099a0: 6974 2e73 6574 4361 6c65 6e64 6172 506f  it.setCalendarPo
-000099b0: 7075 7028 5472 7565 290a 2020 2020 2020  pup(True).      
-000099c0: 2020 7365 6c66 2e63 6f6e 7465 7374 5f64    self.contest_d
-000099d0: 6961 6c6f 672e 6461 7465 5469 6d65 4564  ialog.dateTimeEd
-000099e0: 6974 2e73 6574 5469 6d65 2851 7443 6f72  it.setTime(QtCor
-000099f0: 652e 5154 696d 6528 302c 2030 2929 0a20  e.QTime(0, 0)). 
-00009a00: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
-00009a10: 6573 745f 6469 616c 6f67 2e70 6f77 6572  est_dialog.power
-00009a20: 2e73 6574 4375 7272 656e 7454 6578 7428  .setCurrentText(
-00009a30: 224c 4f57 2229 0a20 2020 2020 2020 2073  "LOW").        s
-00009a40: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-00009a50: 6f67 2e73 7461 7469 6f6e 2e73 6574 4375  og.station.setCu
-00009a60: 7272 656e 7454 6578 7428 2246 4958 4544  rrentText("FIXED
-00009a70: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00009a80: 636f 6e74 6573 745f 6469 616c 6f67 2e6f  contest_dialog.o
-00009a90: 7065 6e28 290a 0a20 2020 2064 6566 2073  pen()..    def s
-00009aa0: 6176 655f 636f 6e74 6573 7428 7365 6c66  ave_contest(self
-00009ab0: 293a 0a20 2020 2020 2020 2022 2222 5361  ):.        """Sa
-00009ac0: 7665 2043 6f6e 7465 7374 2222 220a 2020  ve Contest""".  
-00009ad0: 2020 2020 2020 6e65 7874 5f6e 756d 6265        next_numbe
-00009ae0: 7220 3d20 7365 6c66 2e64 6174 6162 6173  r = self.databas
-00009af0: 652e 6765 745f 6e65 7874 5f63 6f6e 7465  e.get_next_conte
-00009b00: 7374 5f6e 7228 290a 2020 2020 2020 2020  st_nr().        
-00009b10: 636f 6e74 6573 7420 3d20 7b7d 0a20 2020  contest = {}.   
-00009b20: 2020 2020 2063 6f6e 7465 7374 5b22 436f       contest["Co
-00009b30: 6e74 6573 744e 616d 6522 5d20 3d20 280a  ntestName"] = (.
-00009b40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00009b50: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
-00009b60: 636f 6e74 6573 742e 6375 7272 656e 7454  contest.currentT
-00009b70: 6578 7428 292e 6c6f 7765 7228 292e 7265  ext().lower().re
-00009b80: 706c 6163 6528 2220 222c 2022 5f22 290a  place(" ", "_").
-00009b90: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00009ba0: 2020 636f 6e74 6573 745b 2253 7461 7274    contest["Start
-00009bb0: 4461 7465 225d 203d 2073 656c 662e 636f  Date"] = self.co
-00009bc0: 6e74 6573 745f 6469 616c 6f67 2e64 6174  ntest_dialog.dat
-00009bd0: 6554 696d 6545 6469 742e 6461 7465 5469  eTimeEdit.dateTi
-00009be0: 6d65 2829 2e74 6f53 7472 696e 6728 0a20  me().toString(. 
-00009bf0: 2020 2020 2020 2020 2020 2022 7979 7979             "yyyy
-00009c00: 2d4d 4d2d 6464 2068 683a 6d6d 3a73 7322  -MM-dd hh:mm:ss"
-00009c10: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-00009c20: 2020 2063 6f6e 7465 7374 5b22 4f70 6572     contest["Oper
-00009c30: 6174 6f72 4361 7465 676f 7279 225d 203d  atorCategory"] =
-00009c40: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
-00009c50: 616c 6f67 2e6f 7065 7261 746f 725f 636c  alog.operator_cl
-00009c60: 6173 732e 6375 7272 656e 7454 6578 7428  ass.currentText(
-00009c70: 290a 2020 2020 2020 2020 636f 6e74 6573  ).        contes
-00009c80: 745b 2242 616e 6443 6174 6567 6f72 7922  t["BandCategory"
-00009c90: 5d20 3d20 7365 6c66 2e63 6f6e 7465 7374  ] = self.contest
-00009ca0: 5f64 6961 6c6f 672e 6261 6e64 2e63 7572  _dialog.band.cur
-00009cb0: 7265 6e74 5465 7874 2829 0a20 2020 2020  rentText().     
-00009cc0: 2020 2063 6f6e 7465 7374 5b22 506f 7765     contest["Powe
-00009cd0: 7243 6174 6567 6f72 7922 5d20 3d20 7365  rCategory"] = se
-00009ce0: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
-00009cf0: 672e 706f 7765 722e 6375 7272 656e 7454  g.power.currentT
-00009d00: 6578 7428 290a 2020 2020 2020 2020 636f  ext().        co
-00009d10: 6e74 6573 745b 224d 6f64 6543 6174 6567  ntest["ModeCateg
-00009d20: 6f72 7922 5d20 3d20 7365 6c66 2e63 6f6e  ory"] = self.con
-00009d30: 7465 7374 5f64 6961 6c6f 672e 6d6f 6465  test_dialog.mode
-00009d40: 2e63 7572 7265 6e74 5465 7874 2829 0a20  .currentText(). 
-00009d50: 2020 2020 2020 2063 6f6e 7465 7374 5b22         contest["
-00009d60: 4f76 6572 6c61 7943 6174 6567 6f72 7922  OverlayCategory"
-00009d70: 5d20 3d20 7365 6c66 2e63 6f6e 7465 7374  ] = self.contest
-00009d80: 5f64 6961 6c6f 672e 6f76 6572 6c61 792e  _dialog.overlay.
-00009d90: 6375 7272 656e 7454 6578 7428 290a 2020  currentText().  
-00009da0: 2020 2020 2020 2320 636f 6e74 6573 745b        # contest[
-00009db0: 2743 6c61 696d 6564 5363 6f72 6527 5d20  'ClaimedScore'] 
-00009dc0: 3d20 7365 6c66 2e63 6f6e 7465 7374 5f64  = self.contest_d
-00009dd0: 6961 6c6f 672e 0a20 2020 2020 2020 2063  ialog..        c
-00009de0: 6f6e 7465 7374 5b22 4f70 6572 6174 6f72  ontest["Operator
-00009df0: 7322 5d20 3d20 7365 6c66 2e63 6f6e 7465  s"] = self.conte
-00009e00: 7374 5f64 6961 6c6f 672e 6f70 6572 6174  st_dialog.operat
-00009e10: 6f72 732e 7465 7874 2829 0a20 2020 2020  ors.text().     
-00009e20: 2020 2063 6f6e 7465 7374 5b22 536f 6170     contest["Soap
-00009e30: 626f 7822 5d20 3d20 7365 6c66 2e63 6f6e  box"] = self.con
-00009e40: 7465 7374 5f64 6961 6c6f 672e 736f 6170  test_dialog.soap
-00009e50: 626f 782e 746f 506c 6169 6e54 6578 7428  box.toPlainText(
-00009e60: 290a 2020 2020 2020 2020 636f 6e74 6573  ).        contes
-00009e70: 745b 2253 656e 7445 7863 6861 6e67 6522  t["SentExchange"
-00009e80: 5d20 3d20 7365 6c66 2e63 6f6e 7465 7374  ] = self.contest
-00009e90: 5f64 6961 6c6f 672e 6578 6368 616e 6765  _dialog.exchange
-00009ea0: 2e74 6578 7428 290a 2020 2020 2020 2020  .text().        
-00009eb0: 636f 6e74 6573 745b 2243 6f6e 7465 7374  contest["Contest
-00009ec0: 4e52 225d 203d 206e 6578 745f 6e75 6d62  NR"] = next_numb
-00009ed0: 6572 2e67 6574 2822 636f 756e 7422 2c20  er.get("count", 
-00009ee0: 3129 0a20 2020 2020 2020 2073 656c 662e  1).        self.
-00009ef0: 7072 6566 5b22 636f 6e74 6573 7422 5d20  pref["contest"] 
-00009f00: 3d20 6e65 7874 5f6e 756d 6265 722e 6765  = next_number.ge
-00009f10: 7428 2263 6f75 6e74 222c 2031 290a 2020  t("count", 1).  
-00009f20: 2020 2020 2020 2320 636f 6e74 6573 745b        # contest[
-00009f30: 2753 7562 5479 7065 275d 203d 2073 656c  'SubType'] = sel
-00009f40: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
-00009f50: 2e0a 2020 2020 2020 2020 636f 6e74 6573  ..        contes
-00009f60: 745b 2253 7461 7469 6f6e 4361 7465 676f  t["StationCatego
-00009f70: 7279 225d 203d 2073 656c 662e 636f 6e74  ry"] = self.cont
-00009f80: 6573 745f 6469 616c 6f67 2e73 7461 7469  est_dialog.stati
-00009f90: 6f6e 2e63 7572 7265 6e74 5465 7874 2829  on.currentText()
-00009fa0: 0a20 2020 2020 2020 2063 6f6e 7465 7374  .        contest
-00009fb0: 5b22 4173 7369 7374 6564 4361 7465 676f  ["AssistedCatego
-00009fc0: 7279 225d 203d 2073 656c 662e 636f 6e74  ry"] = self.cont
-00009fd0: 6573 745f 6469 616c 6f67 2e61 7373 6973  est_dialog.assis
-00009fe0: 7465 642e 6375 7272 656e 7454 6578 7428  ted.currentText(
-00009ff0: 290a 2020 2020 2020 2020 636f 6e74 6573  ).        contes
-0000a000: 745b 2254 7261 6e73 6d69 7474 6572 4361  t["TransmitterCa
-0000a010: 7465 676f 7279 225d 203d 2073 656c 662e  tegory"] = self.
-0000a020: 636f 6e74 6573 745f 6469 616c 6f67 2e74  contest_dialog.t
-0000a030: 7261 6e73 6d69 7474 6572 2e63 7572 7265  ransmitter.curre
-0000a040: 6e74 5465 7874 2829 0a20 2020 2020 2020  ntText().       
-0000a050: 2023 2063 6f6e 7465 7374 5b27 5469 6d65   # contest['Time
-0000a060: 4361 7465 676f 7279 275d 203d 2073 656c  Category'] = sel
-0000a070: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
-0000a080: 2e0a 2020 2020 2020 2020 6c6f 6767 6572  ..        logger
-0000a090: 2e64 6562 7567 2822 2573 222c 2066 227b  .debug("%s", f"{
-0000a0a0: 636f 6e74 6573 747d 2229 0a20 2020 2020  contest}").     
-0000a0b0: 2020 2073 656c 662e 6461 7461 6261 7365     self.database
-0000a0c0: 2e61 6464 5f63 6f6e 7465 7374 2863 6f6e  .add_contest(con
-0000a0d0: 7465 7374 290a 2020 2020 2020 2020 7365  test).        se
-0000a0e0: 6c66 2e77 7269 7465 5f70 7265 6665 7265  lf.write_prefere
-0000a0f0: 6e63 6528 290a 2020 2020 2020 2020 7365  nce().        se
-0000a100: 6c66 2e6c 6f61 645f 636f 6e74 6573 7428  lf.load_contest(
-0000a110: 290a 0a20 2020 2064 6566 2065 6469 745f  )..    def edit_
-0000a120: 7374 6174 696f 6e5f 7365 7474 696e 6773  station_settings
-0000a130: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000a140: 2222 2253 686f 7720 7365 7474 696e 6773  """Show settings
-0000a150: 2064 6961 6c6f 6722 2222 0a20 2020 2020   dialog""".     
-0000a160: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-0000a170: 2253 7461 7469 6f6e 2053 6574 7469 6e67  "Station Setting
-0000a180: 7320 7365 6c65 6374 6564 2229 0a20 2020  s selected").   
-0000a190: 2020 2020 2073 656c 662e 7365 7474 696e       self.settin
-0000a1a0: 6773 5f64 6961 6c6f 6720 3d20 4564 6974  gs_dialog = Edit
-0000a1b0: 5374 6174 696f 6e28 574f 524b 494e 475f  Station(WORKING_
-0000a1c0: 5041 5448 290a 2020 2020 2020 2020 6966  PATH).        if
-0000a1d0: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
-0000a1e0: 6461 726b 5f6d 6f64 6522 293a 0a20 2020  dark_mode"):.   
-0000a1f0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-0000a200: 7474 696e 6773 5f64 6961 6c6f 672e 7365  ttings_dialog.se
-0000a210: 7453 7479 6c65 5368 6565 7428 4441 524b  tStyleSheet(DARK
-0000a220: 5f53 5459 4c45 5348 4545 5429 0a20 2020  _STYLESHEET).   
-0000a230: 2020 2020 2073 656c 662e 7365 7474 696e       self.settin
-0000a240: 6773 5f64 6961 6c6f 672e 6163 6365 7074  gs_dialog.accept
-0000a250: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
-0000a260: 7361 7665 5f73 6574 7469 6e67 7329 0a20  save_settings). 
-0000a270: 2020 2020 2020 2023 2069 6620 7365 6c66         # if self
-0000a280: 2e70 7265 662e 6765 7428 2264 6172 6b5f  .pref.get("dark_
-0000a290: 6d6f 6465 2229 3a0a 2020 2020 2020 2020  mode"):.        
-0000a2a0: 2320 2020 2020 7365 6c66 2e73 6574 7469  #     self.setti
-0000a2b0: 6e67 735f 6469 616c 6f67 2e73 6574 5374  ngs_dialog.setSt
-0000a2c0: 796c 6553 6865 6574 2844 4152 4b5f 5354  yleSheet(DARK_ST
-0000a2d0: 594c 4553 4845 4554 290a 0a20 2020 2020  YLESHEET)..     
-0000a2e0: 2020 2073 656c 662e 7365 7474 696e 6773     self.settings
-0000a2f0: 5f64 6961 6c6f 672e 4361 6c6c 2e73 6574  _dialog.Call.set
-0000a300: 5465 7874 2873 656c 662e 7374 6174 696f  Text(self.statio
-0000a310: 6e2e 6765 7428 2243 616c 6c22 2c20 2222  n.get("Call", ""
-0000a320: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-0000a330: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
-0000a340: 4e61 6d65 2e73 6574 5465 7874 2873 656c  Name.setText(sel
-0000a350: 662e 7374 6174 696f 6e2e 6765 7428 224e  f.station.get("N
-0000a360: 616d 6522 2c20 2222 2929 0a20 2020 2020  ame", "")).     
-0000a370: 2020 2073 656c 662e 7365 7474 696e 6773     self.settings
-0000a380: 5f64 6961 6c6f 672e 4164 6472 6573 7331  _dialog.Address1
-0000a390: 2e73 6574 5465 7874 2873 656c 662e 7374  .setText(self.st
-0000a3a0: 6174 696f 6e2e 6765 7428 2253 7472 6565  ation.get("Stree
-0000a3b0: 7431 222c 2022 2229 290a 2020 2020 2020  t1", "")).      
-0000a3c0: 2020 7365 6c66 2e73 6574 7469 6e67 735f    self.settings_
-0000a3d0: 6469 616c 6f67 2e41 6464 7265 7373 322e  dialog.Address2.
-0000a3e0: 7365 7454 6578 7428 7365 6c66 2e73 7461  setText(self.sta
-0000a3f0: 7469 6f6e 2e67 6574 2822 5374 7265 6574  tion.get("Street
-0000a400: 3222 2c20 2222 2929 0a20 2020 2020 2020  2", "")).       
-0000a410: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
-0000a420: 6961 6c6f 672e 4369 7479 2e73 6574 5465  ialog.City.setTe
-0000a430: 7874 2873 656c 662e 7374 6174 696f 6e2e  xt(self.station.
-0000a440: 6765 7428 2243 6974 7922 2c20 2222 2929  get("City", ""))
-0000a450: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-0000a460: 7474 696e 6773 5f64 6961 6c6f 672e 5374  ttings_dialog.St
-0000a470: 6174 652e 7365 7454 6578 7428 7365 6c66  ate.setText(self
-0000a480: 2e73 7461 7469 6f6e 2e67 6574 2822 5374  .station.get("St
-0000a490: 6174 6522 2c20 2222 2929 0a20 2020 2020  ate", "")).     
-0000a4a0: 2020 2073 656c 662e 7365 7474 696e 6773     self.settings
-0000a4b0: 5f64 6961 6c6f 672e 5a69 702e 7365 7454  _dialog.Zip.setT
-0000a4c0: 6578 7428 7365 6c66 2e73 7461 7469 6f6e  ext(self.station
-0000a4d0: 2e67 6574 2822 5a69 7022 2c20 2222 2929  .get("Zip", ""))
-0000a4e0: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-0000a4f0: 7474 696e 6773 5f64 6961 6c6f 672e 436f  ttings_dialog.Co
-0000a500: 756e 7472 792e 7365 7454 6578 7428 7365  untry.setText(se
-0000a510: 6c66 2e73 7461 7469 6f6e 2e67 6574 2822  lf.station.get("
-0000a520: 436f 756e 7472 7922 2c20 2222 2929 0a20  Country", "")). 
-0000a530: 2020 2020 2020 2073 656c 662e 7365 7474         self.sett
-0000a540: 696e 6773 5f64 6961 6c6f 672e 4772 6964  ings_dialog.Grid
-0000a550: 5371 7561 7265 2e73 6574 5465 7874 2873  Square.setText(s
-0000a560: 656c 662e 7374 6174 696f 6e2e 6765 7428  elf.station.get(
-0000a570: 2247 7269 6453 7175 6172 6522 2c20 2222  "GridSquare", ""
-0000a580: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-0000a590: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
-0000a5a0: 4351 5a6f 6e65 2e73 6574 5465 7874 2873  CQZone.setText(s
-0000a5b0: 7472 2873 656c 662e 7374 6174 696f 6e2e  tr(self.station.
-0000a5c0: 6765 7428 2243 515a 6f6e 6522 2c20 2222  get("CQZone", ""
-0000a5d0: 2929 290a 2020 2020 2020 2020 7365 6c66  ))).        self
-0000a5e0: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
-0000a5f0: 2e49 5455 5a6f 6e65 2e73 6574 5465 7874  .ITUZone.setText
-0000a600: 2873 7472 2873 656c 662e 7374 6174 696f  (str(self.statio
-0000a610: 6e2e 6765 7428 2249 4152 555a 6f6e 6522  n.get("IARUZone"
-0000a620: 2c20 2222 2929 290a 2020 2020 2020 2020  , ""))).        
-0000a630: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
-0000a640: 616c 6f67 2e4c 6963 656e 7365 2e73 6574  alog.License.set
-0000a650: 5465 7874 2873 656c 662e 7374 6174 696f  Text(self.statio
-0000a660: 6e2e 6765 7428 224c 6963 656e 7365 436c  n.get("LicenseCl
-0000a670: 6173 7322 2c20 2222 2929 0a20 2020 2020  ass", "")).     
-0000a680: 2020 2073 656c 662e 7365 7474 696e 6773     self.settings
-0000a690: 5f64 6961 6c6f 672e 4c61 7469 7475 6465  _dialog.Latitude
-0000a6a0: 2e73 6574 5465 7874 2873 7472 2873 656c  .setText(str(sel
-0000a6b0: 662e 7374 6174 696f 6e2e 6765 7428 224c  f.station.get("L
-0000a6c0: 6174 6974 7564 6522 2c20 2222 2929 290a  atitude", ""))).
-0000a6d0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-0000a6e0: 7469 6e67 735f 6469 616c 6f67 2e4c 6f6e  tings_dialog.Lon
-0000a6f0: 6769 7475 6465 2e73 6574 5465 7874 2873  gitude.setText(s
-0000a700: 7472 2873 656c 662e 7374 6174 696f 6e2e  tr(self.station.
-0000a710: 6765 7428 224c 6f6e 6769 7475 6465 222c  get("Longitude",
-0000a720: 2022 2229 2929 0a20 2020 2020 2020 2073   ""))).        s
-0000a730: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
-0000a740: 6c6f 672e 5374 6174 696f 6e54 5852 582e  log.StationTXRX.
-0000a750: 7365 7454 6578 7428 7365 6c66 2e73 7461  setText(self.sta
-0000a760: 7469 6f6e 2e67 6574 2822 7374 6174 696f  tion.get("statio
-0000a770: 6e74 7872 7822 2c20 2222 2929 0a20 2020  ntxrx", "")).   
-0000a780: 2020 2020 2073 656c 662e 7365 7474 696e       self.settin
-0000a790: 6773 5f64 6961 6c6f 672e 506f 7765 722e  gs_dialog.Power.
-0000a7a0: 7365 7454 6578 7428 7365 6c66 2e73 7461  setText(self.sta
-0000a7b0: 7469 6f6e 2e67 6574 2822 5350 6f77 6522  tion.get("SPowe"
-0000a7c0: 2c20 2222 2929 0a20 2020 2020 2020 2073  , "")).        s
-0000a7d0: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
-0000a7e0: 6c6f 672e 416e 7465 6e6e 612e 7365 7454  log.Antenna.setT
-0000a7f0: 6578 7428 7365 6c66 2e73 7461 7469 6f6e  ext(self.station
-0000a800: 2e67 6574 2822 5341 6e74 6522 2c20 2222  .get("SAnte", ""
-0000a810: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-0000a820: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
-0000a830: 416e 7448 6569 6768 742e 7365 7454 6578  AntHeight.setTex
-0000a840: 7428 7365 6c66 2e73 7461 7469 6f6e 2e67  t(self.station.g
-0000a850: 6574 2822 5341 6e74 4831 222c 2022 2229  et("SAntH1", "")
-0000a860: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
-0000a870: 6574 7469 6e67 735f 6469 616c 6f67 2e41  ettings_dialog.A
-0000a880: 534c 2e73 6574 5465 7874 2873 656c 662e  SL.setText(self.
-0000a890: 7374 6174 696f 6e2e 6765 7428 2253 416e  station.get("SAn
-0000a8a0: 7448 3222 2c20 2222 2929 0a20 2020 2020  tH2", "")).     
-0000a8b0: 2020 2073 656c 662e 7365 7474 696e 6773     self.settings
-0000a8c0: 5f64 6961 6c6f 672e 4152 524c 5365 6374  _dialog.ARRLSect
-0000a8d0: 696f 6e2e 7365 7454 6578 7428 7365 6c66  ion.setText(self
-0000a8e0: 2e73 7461 7469 6f6e 2e67 6574 2822 4152  .station.get("AR
-0000a8f0: 524c 5365 6374 696f 6e22 2c20 2222 2929  RLSection", ""))
-0000a900: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-0000a910: 7474 696e 6773 5f64 6961 6c6f 672e 526f  ttings_dialog.Ro
-0000a920: 7665 7251 5448 2e73 6574 5465 7874 2873  verQTH.setText(s
-0000a930: 656c 662e 7374 6174 696f 6e2e 6765 7428  elf.station.get(
-0000a940: 2252 6f76 6572 5154 4822 2c20 2222 2929  "RoverQTH", ""))
-0000a950: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-0000a960: 7474 696e 6773 5f64 6961 6c6f 672e 436c  ttings_dialog.Cl
-0000a970: 7562 2e73 6574 5465 7874 2873 656c 662e  ub.setText(self.
-0000a980: 7374 6174 696f 6e2e 6765 7428 2243 6c75  station.get("Clu
-0000a990: 6222 2c20 2222 2929 0a20 2020 2020 2020  b", "")).       
-0000a9a0: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
-0000a9b0: 6961 6c6f 672e 456d 6169 6c2e 7365 7454  ialog.Email.setT
-0000a9c0: 6578 7428 7365 6c66 2e73 7461 7469 6f6e  ext(self.station
-0000a9d0: 2e67 6574 2822 456d 6169 6c22 2c20 2222  .get("Email", ""
-0000a9e0: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-0000a9f0: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
-0000aa00: 6f70 656e 2829 0a0a 2020 2020 6465 6620  open()..    def 
-0000aa10: 7361 7665 5f73 6574 7469 6e67 7328 7365  save_settings(se
-0000aa20: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-0000aa30: 5361 7665 2073 6574 7469 6e67 7322 2222  Save settings"""
-0000aa40: 0a20 2020 2020 2020 2063 7320 3d20 7365  .        cs = se
-0000aa50: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
-0000aa60: 6f67 2e43 616c 6c2e 7465 7874 2829 0a20  og.Call.text(). 
-0000aa70: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
-0000aa80: 696f 6e20 3d20 7b7d 0a20 2020 2020 2020  ion = {}.       
-0000aa90: 2073 656c 662e 7374 6174 696f 6e5b 2243   self.station["C
-0000aaa0: 616c 6c22 5d20 3d20 6373 2e75 7070 6572  all"] = cs.upper
-0000aab0: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-0000aac0: 7374 6174 696f 6e5b 224e 616d 6522 5d20  station["Name"] 
-0000aad0: 3d20 7365 6c66 2e73 6574 7469 6e67 735f  = self.settings_
-0000aae0: 6469 616c 6f67 2e4e 616d 652e 7465 7874  dialog.Name.text
-0000aaf0: 2829 2e74 6974 6c65 2829 0a20 2020 2020  ().title().     
-0000ab00: 2020 2073 656c 662e 7374 6174 696f 6e5b     self.station[
-0000ab10: 2253 7472 6565 7431 225d 203d 2073 656c  "Street1"] = sel
-0000ab20: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
-0000ab30: 672e 4164 6472 6573 7331 2e74 6578 7428  g.Address1.text(
-0000ab40: 292e 7469 746c 6528 290a 2020 2020 2020  ).title().      
-0000ab50: 2020 7365 6c66 2e73 7461 7469 6f6e 5b22    self.station["
-0000ab60: 5374 7265 6574 3222 5d20 3d20 7365 6c66  Street2"] = self
-0000ab70: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
-0000ab80: 2e41 6464 7265 7373 322e 7465 7874 2829  .Address2.text()
-0000ab90: 2e74 6974 6c65 2829 0a20 2020 2020 2020  .title().       
-0000aba0: 2073 656c 662e 7374 6174 696f 6e5b 2243   self.station["C
-0000abb0: 6974 7922 5d20 3d20 7365 6c66 2e73 6574  ity"] = self.set
-0000abc0: 7469 6e67 735f 6469 616c 6f67 2e43 6974  tings_dialog.Cit
-0000abd0: 792e 7465 7874 2829 2e74 6974 6c65 2829  y.text().title()
-0000abe0: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
-0000abf0: 6174 696f 6e5b 2253 7461 7465 225d 203d  ation["State"] =
-0000ac00: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
-0000ac10: 6961 6c6f 672e 5374 6174 652e 7465 7874  ialog.State.text
-0000ac20: 2829 2e75 7070 6572 2829 0a20 2020 2020  ().upper().     
-0000ac30: 2020 2073 656c 662e 7374 6174 696f 6e5b     self.station[
-0000ac40: 225a 6970 225d 203d 2073 656c 662e 7365  "Zip"] = self.se
-0000ac50: 7474 696e 6773 5f64 6961 6c6f 672e 5a69  ttings_dialog.Zi
-0000ac60: 702e 7465 7874 2829 0a20 2020 2020 2020  p.text().       
-0000ac70: 2073 656c 662e 7374 6174 696f 6e5b 2243   self.station["C
-0000ac80: 6f75 6e74 7279 225d 203d 2073 656c 662e  ountry"] = self.
-0000ac90: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
-0000aca0: 436f 756e 7472 792e 7465 7874 2829 2e74  Country.text().t
-0000acb0: 6974 6c65 2829 0a20 2020 2020 2020 2073  itle().        s
-0000acc0: 656c 662e 7374 6174 696f 6e5b 2247 7269  elf.station["Gri
-0000acd0: 6453 7175 6172 6522 5d20 3d20 7365 6c66  dSquare"] = self
-0000ace0: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
-0000acf0: 2e47 7269 6453 7175 6172 652e 7465 7874  .GridSquare.text
-0000ad00: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-0000ad10: 7374 6174 696f 6e5b 2243 515a 6f6e 6522  station["CQZone"
-0000ad20: 5d20 3d20 7365 6c66 2e73 6574 7469 6e67  ] = self.setting
-0000ad30: 735f 6469 616c 6f67 2e43 515a 6f6e 652e  s_dialog.CQZone.
-0000ad40: 7465 7874 2829 0a20 2020 2020 2020 2073  text().        s
-0000ad50: 656c 662e 7374 6174 696f 6e5b 2249 4152  elf.station["IAR
-0000ad60: 555a 6f6e 6522 5d20 3d20 7365 6c66 2e73  UZone"] = self.s
-0000ad70: 6574 7469 6e67 735f 6469 616c 6f67 2e49  ettings_dialog.I
-0000ad80: 5455 5a6f 6e65 2e74 6578 7428 290a 2020  TUZone.text().  
-0000ad90: 2020 2020 2020 7365 6c66 2e73 7461 7469        self.stati
-0000ada0: 6f6e 5b22 4c69 6365 6e73 6543 6c61 7373  on["LicenseClass
-0000adb0: 225d 203d 2073 656c 662e 7365 7474 696e  "] = self.settin
-0000adc0: 6773 5f64 6961 6c6f 672e 4c69 6365 6e73  gs_dialog.Licens
-0000add0: 652e 7465 7874 2829 2e74 6974 6c65 2829  e.text().title()
-0000ade0: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
-0000adf0: 6174 696f 6e5b 224c 6174 6974 7564 6522  ation["Latitude"
-0000ae00: 5d20 3d20 7365 6c66 2e73 6574 7469 6e67  ] = self.setting
-0000ae10: 735f 6469 616c 6f67 2e4c 6174 6974 7564  s_dialog.Latitud
-0000ae20: 652e 7465 7874 2829 0a20 2020 2020 2020  e.text().       
-0000ae30: 2073 656c 662e 7374 6174 696f 6e5b 224c   self.station["L
-0000ae40: 6f6e 6769 7475 6465 225d 203d 2073 656c  ongitude"] = sel
-0000ae50: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
-0000ae60: 672e 4c6f 6e67 6974 7564 652e 7465 7874  g.Longitude.text
-0000ae70: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-0000ae80: 7374 6174 696f 6e5b 2253 5458 6571 225d  station["STXeq"]
-0000ae90: 203d 2073 656c 662e 7365 7474 696e 6773   = self.settings
-0000aea0: 5f64 6961 6c6f 672e 5374 6174 696f 6e54  _dialog.StationT
-0000aeb0: 5852 582e 7465 7874 2829 0a20 2020 2020  XRX.text().     
-0000aec0: 2020 2073 656c 662e 7374 6174 696f 6e5b     self.station[
-0000aed0: 2253 506f 7765 225d 203d 2073 656c 662e  "SPowe"] = self.
-0000aee0: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
-0000aef0: 506f 7765 722e 7465 7874 2829 0a20 2020  Power.text().   
-0000af00: 2020 2020 2073 656c 662e 7374 6174 696f       self.statio
-0000af10: 6e5b 2253 416e 7465 225d 203d 2073 656c  n["SAnte"] = sel
-0000af20: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
-0000af30: 672e 416e 7465 6e6e 612e 7465 7874 2829  g.Antenna.text()
-0000af40: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
-0000af50: 6174 696f 6e5b 2253 416e 7448 3122 5d20  ation["SAntH1"] 
-0000af60: 3d20 7365 6c66 2e73 6574 7469 6e67 735f  = self.settings_
-0000af70: 6469 616c 6f67 2e41 6e74 4865 6967 6874  dialog.AntHeight
-0000af80: 2e74 6578 7428 290a 2020 2020 2020 2020  .text().        
-0000af90: 7365 6c66 2e73 7461 7469 6f6e 5b22 5341  self.station["SA
-0000afa0: 6e74 4832 225d 203d 2073 656c 662e 7365  ntH2"] = self.se
-0000afb0: 7474 696e 6773 5f64 6961 6c6f 672e 4153  ttings_dialog.AS
-0000afc0: 4c2e 7465 7874 2829 0a20 2020 2020 2020  L.text().       
-0000afd0: 2073 656c 662e 7374 6174 696f 6e5b 2241   self.station["A
-0000afe0: 5252 4c53 6563 7469 6f6e 225d 203d 2073  RRLSection"] = s
-0000aff0: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
-0000b000: 6c6f 672e 4152 524c 5365 6374 696f 6e2e  log.ARRLSection.
-0000b010: 7465 7874 2829 2e75 7070 6572 2829 0a20  text().upper(). 
-0000b020: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
-0000b030: 696f 6e5b 2252 6f76 6572 5154 4822 5d20  ion["RoverQTH"] 
-0000b040: 3d20 7365 6c66 2e73 6574 7469 6e67 735f  = self.settings_
-0000b050: 6469 616c 6f67 2e52 6f76 6572 5154 482e  dialog.RoverQTH.
-0000b060: 7465 7874 2829 0a20 2020 2020 2020 2073  text().        s
-0000b070: 656c 662e 7374 6174 696f 6e5b 2243 6c75  elf.station["Clu
-0000b080: 6222 5d20 3d20 7365 6c66 2e73 6574 7469  b"] = self.setti
-0000b090: 6e67 735f 6469 616c 6f67 2e43 6c75 622e  ngs_dialog.Club.
-0000b0a0: 7465 7874 2829 2e74 6974 6c65 2829 0a20  text().title(). 
-0000b0b0: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
-0000b0c0: 696f 6e5b 2245 6d61 696c 225d 203d 2073  ion["Email"] = s
-0000b0d0: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
-0000b0e0: 6c6f 672e 456d 6169 6c2e 7465 7874 2829  log.Email.text()
-0000b0f0: 0a20 2020 2020 2020 2073 656c 662e 6461  .        self.da
-0000b100: 7461 6261 7365 2e61 6464 5f73 7461 7469  tabase.add_stati
-0000b110: 6f6e 2873 656c 662e 7374 6174 696f 6e29  on(self.station)
-0000b120: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-0000b130: 7474 696e 6773 5f64 6961 6c6f 672e 636c  ttings_dialog.cl
-0000b140: 6f73 6528 290a 2020 2020 2020 2020 6966  ose().        if
-0000b150: 2073 656c 662e 6375 7272 656e 745f 6f70   self.current_op
-0000b160: 203d 3d20 2222 3a0a 2020 2020 2020 2020   == "":.        
-0000b170: 2020 2020 7365 6c66 2e63 7572 7265 6e74      self.current
-0000b180: 5f6f 7020 3d20 7365 6c66 2e73 7461 7469  _op = self.stati
-0000b190: 6f6e 2e67 6574 2822 4361 6c6c 222c 2022  on.get("Call", "
-0000b1a0: 2229 0a20 2020 2020 2020 2020 2020 2073  ").            s
-0000b1b0: 656c 662e 6d61 6b65 5f6f 705f 6469 7228  elf.make_op_dir(
-0000b1c0: 290a 2020 2020 2020 2020 636f 6e74 6573  ).        contes
-0000b1d0: 745f 636f 756e 7420 3d20 7365 6c66 2e64  t_count = self.d
-0000b1e0: 6174 6162 6173 652e 6665 7463 685f 616c  atabase.fetch_al
-0000b1f0: 6c5f 636f 6e74 6573 7473 2829 0a20 2020  l_contests().   
-0000b200: 2020 2020 2069 6620 6c65 6e28 636f 6e74       if len(cont
-0000b210: 6573 745f 636f 756e 7429 203d 3d20 303a  est_count) == 0:
-0000b220: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000b230: 662e 6e65 775f 636f 6e74 6573 745f 6469  f.new_contest_di
-0000b240: 616c 6f67 2829 0a0a 2020 2020 6465 6620  alog()..    def 
-0000b250: 6564 6974 5f6d 6163 726f 2873 656c 662c  edit_macro(self,
-0000b260: 2066 756e 6374 696f 6e5f 6b65 7929 3a0a   function_key):.
-0000b270: 2020 2020 2020 2020 2222 2253 686f 7720          """Show 
-0000b280: 6564 6974 206d 6163 726f 2064 6961 6c6f  edit macro dialo
-0000b290: 6722 2222 0a20 2020 2020 2020 2073 656c  g""".        sel
-0000b2a0: 662e 6564 6974 5f6d 6163 726f 5f64 6961  f.edit_macro_dia
-0000b2b0: 6c6f 6720 3d20 4564 6974 4d61 6372 6f28  log = EditMacro(
-0000b2c0: 6675 6e63 7469 6f6e 5f6b 6579 2c20 574f  function_key, WO
-0000b2d0: 524b 494e 475f 5041 5448 290a 2020 2020  RKING_PATH).    
-0000b2e0: 2020 2020 7365 6c66 2e65 6469 745f 6d61      self.edit_ma
-0000b2f0: 6372 6f5f 6469 616c 6f67 2e61 6363 6570  cro_dialog.accep
-0000b300: 7465 642e 636f 6e6e 6563 7428 7365 6c66  ted.connect(self
-0000b310: 2e65 6469 7465 645f 6d61 6372 6f29 0a20  .edited_macro). 
-0000b320: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
-0000b330: 7265 662e 6765 7428 2264 6172 6b5f 6d6f  ref.get("dark_mo
-0000b340: 6465 2229 3a0a 2020 2020 2020 2020 2020  de"):.          
-0000b350: 2020 7365 6c66 2e65 6469 745f 6d61 6372    self.edit_macr
-0000b360: 6f5f 6469 616c 6f67 2e73 6574 5374 796c  o_dialog.setStyl
-0000b370: 6553 6865 6574 2844 4152 4b5f 5354 594c  eSheet(DARK_STYL
-0000b380: 4553 4845 4554 290a 2020 2020 2020 2020  ESHEET).        
-0000b390: 7365 6c66 2e65 6469 745f 6d61 6372 6f5f  self.edit_macro_
-0000b3a0: 6469 616c 6f67 2e6f 7065 6e28 290a 0a20  dialog.open().. 
-0000b3b0: 2020 2064 6566 2065 6469 7465 645f 6d61     def edited_ma
-0000b3c0: 6372 6f28 7365 6c66 293a 0a20 2020 2020  cro(self):.     
-0000b3d0: 2020 2022 2222 5361 7665 2065 6469 7465     """Save edite
-0000b3e0: 6420 6d61 6372 6f22 2222 0a20 2020 2020  d macro""".     
-0000b3f0: 2020 2073 656c 662e 6564 6974 5f6d 6163     self.edit_mac
-0000b400: 726f 5f64 6961 6c6f 672e 6675 6e63 7469  ro_dialog.functi
-0000b410: 6f6e 5f6b 6579 2e73 6574 5465 7874 280a  on_key.setText(.
-0000b420: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000b430: 2e65 6469 745f 6d61 6372 6f5f 6469 616c  .edit_macro_dial
-0000b440: 6f67 2e6d 6163 726f 5f6c 6162 656c 2e74  og.macro_label.t
-0000b450: 6578 7428 290a 2020 2020 2020 2020 290a  ext().        ).
-0000b460: 2020 2020 2020 2020 7365 6c66 2e65 6469          self.edi
-0000b470: 745f 6d61 6372 6f5f 6469 616c 6f67 2e66  t_macro_dialog.f
-0000b480: 756e 6374 696f 6e5f 6b65 792e 7365 7454  unction_key.setT
-0000b490: 6f6f 6c54 6970 280a 2020 2020 2020 2020  oolTip(.        
-0000b4a0: 2020 2020 7365 6c66 2e65 6469 745f 6d61      self.edit_ma
-0000b4b0: 6372 6f5f 6469 616c 6f67 2e74 6865 5f6d  cro_dialog.the_m
-0000b4c0: 6163 726f 2e74 6578 7428 290a 2020 2020  acro.text().    
-0000b4d0: 2020 2020 290a 2020 2020 2020 2020 7365      ).        se
-0000b4e0: 6c66 2e65 6469 745f 6d61 6372 6f5f 6469  lf.edit_macro_di
-0000b4f0: 616c 6f67 2e63 6c6f 7365 2829 0a0a 2020  alog.close()..  
-0000b500: 2020 6465 6620 6564 6974 5f46 3128 7365    def edit_F1(se
-0000b510: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-0000b520: 7374 7562 2222 220a 2020 2020 2020 2020  stub""".        
-0000b530: 6c6f 6767 6572 2e64 6562 7567 2822 4631  logger.debug("F1
-0000b540: 2052 6967 6874 2043 6c69 636b 6564 2e22   Right Clicked."
-0000b550: 290a 2020 2020 2020 2020 7365 6c66 2e65  ).        self.e
-0000b560: 6469 745f 6d61 6372 6f28 7365 6c66 2e46  dit_macro(self.F
-0000b570: 3129 0a0a 2020 2020 6465 6620 6564 6974  1)..    def edit
-0000b580: 5f46 3228 7365 6c66 293a 0a20 2020 2020  _F2(self):.     
-0000b590: 2020 2022 2222 7374 7562 2222 220a 2020     """stub""".  
-0000b5a0: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-0000b5b0: 7567 2822 4632 2052 6967 6874 2043 6c69  ug("F2 Right Cli
-0000b5c0: 636b 6564 2e22 290a 2020 2020 2020 2020  cked.").        
-0000b5d0: 7365 6c66 2e65 6469 745f 6d61 6372 6f28  self.edit_macro(
-0000b5e0: 7365 6c66 2e46 3229 0a0a 2020 2020 6465  self.F2)..    de
-0000b5f0: 6620 6564 6974 5f46 3328 7365 6c66 293a  f edit_F3(self):
-0000b600: 0a20 2020 2020 2020 2022 2222 7374 7562  .        """stub
-0000b610: 2222 220a 2020 2020 2020 2020 6c6f 6767  """.        logg
-0000b620: 6572 2e64 6562 7567 2822 4633 2052 6967  er.debug("F3 Rig
-0000b630: 6874 2043 6c69 636b 6564 2e22 290a 2020  ht Clicked.").  
-0000b640: 2020 2020 2020 7365 6c66 2e65 6469 745f        self.edit_
-0000b650: 6d61 6372 6f28 7365 6c66 2e46 3329 0a0a  macro(self.F3)..
-0000b660: 2020 2020 6465 6620 6564 6974 5f46 3428      def edit_F4(
-0000b670: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-0000b680: 2222 7374 7562 2222 220a 2020 2020 2020  ""stub""".      
-0000b690: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
-0000b6a0: 4634 2052 6967 6874 2043 6c69 636b 6564  F4 Right Clicked
-0000b6b0: 2e22 290a 2020 2020 2020 2020 7365 6c66  .").        self
-0000b6c0: 2e65 6469 745f 6d61 6372 6f28 7365 6c66  .edit_macro(self
-0000b6d0: 2e46 3429 0a0a 2020 2020 6465 6620 6564  .F4)..    def ed
-0000b6e0: 6974 5f46 3528 7365 6c66 293a 0a20 2020  it_F5(self):.   
-0000b6f0: 2020 2020 2022 2222 7374 7562 2222 220a       """stub""".
-0000b700: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-0000b710: 6562 7567 2822 4635 2052 6967 6874 2043  ebug("F5 Right C
-0000b720: 6c69 636b 6564 2e22 290a 2020 2020 2020  licked.").      
-0000b730: 2020 7365 6c66 2e65 6469 745f 6d61 6372    self.edit_macr
-0000b740: 6f28 7365 6c66 2e46 3529 0a0a 2020 2020  o(self.F5)..    
-0000b750: 6465 6620 6564 6974 5f46 3628 7365 6c66  def edit_F6(self
-0000b760: 293a 0a20 2020 2020 2020 2022 2222 7374  ):.        """st
-0000b770: 7562 2222 220a 2020 2020 2020 2020 6c6f  ub""".        lo
-0000b780: 6767 6572 2e64 6562 7567 2822 4636 2052  gger.debug("F6 R
-0000b790: 6967 6874 2043 6c69 636b 6564 2e22 290a  ight Clicked.").
-0000b7a0: 2020 2020 2020 2020 7365 6c66 2e65 6469          self.edi
-0000b7b0: 745f 6d61 6372 6f28 7365 6c66 2e46 3629  t_macro(self.F6)
-0000b7c0: 0a0a 2020 2020 6465 6620 6564 6974 5f46  ..    def edit_F
-0000b7d0: 3728 7365 6c66 293a 0a20 2020 2020 2020  7(self):.       
-0000b7e0: 2022 2222 7374 7562 2222 220a 2020 2020   """stub""".    
-0000b7f0: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
-0000b800: 2822 4637 2052 6967 6874 2043 6c69 636b  ("F7 Right Click
-0000b810: 6564 2e22 290a 2020 2020 2020 2020 7365  ed.").        se
-0000b820: 6c66 2e65 6469 745f 6d61 6372 6f28 7365  lf.edit_macro(se
-0000b830: 6c66 2e46 3729 0a0a 2020 2020 6465 6620  lf.F7)..    def 
-0000b840: 6564 6974 5f46 3828 7365 6c66 293a 0a20  edit_F8(self):. 
-0000b850: 2020 2020 2020 2022 2222 7374 7562 2222         """stub""
-0000b860: 220a 2020 2020 2020 2020 6c6f 6767 6572  ".        logger
-0000b870: 2e64 6562 7567 2822 4638 2052 6967 6874  .debug("F8 Right
-0000b880: 2043 6c69 636b 6564 2e22 290a 2020 2020   Clicked.").    
-0000b890: 2020 2020 7365 6c66 2e65 6469 745f 6d61      self.edit_ma
-0000b8a0: 6372 6f28 7365 6c66 2e46 3829 0a0a 2020  cro(self.F8)..  
-0000b8b0: 2020 6465 6620 6564 6974 5f46 3928 7365    def edit_F9(se
-0000b8c0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-0000b8d0: 7374 7562 2222 220a 2020 2020 2020 2020  stub""".        
-0000b8e0: 6c6f 6767 6572 2e64 6562 7567 2822 4639  logger.debug("F9
-0000b8f0: 2052 6967 6874 2043 6c69 636b 6564 2e22   Right Clicked."
-0000b900: 290a 2020 2020 2020 2020 7365 6c66 2e65  ).        self.e
-0000b910: 6469 745f 6d61 6372 6f28 7365 6c66 2e46  dit_macro(self.F
-0000b920: 3929 0a0a 2020 2020 6465 6620 6564 6974  9)..    def edit
-0000b930: 5f46 3130 2873 656c 6629 3a0a 2020 2020  _F10(self):.    
-0000b940: 2020 2020 2222 2273 7475 6222 2222 0a20      """stub""". 
-0000b950: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-0000b960: 6275 6728 2246 3130 2052 6967 6874 2043  bug("F10 Right C
-0000b970: 6c69 636b 6564 2e22 290a 2020 2020 2020  licked.").      
-0000b980: 2020 7365 6c66 2e65 6469 745f 6d61 6372    self.edit_macr
-0000b990: 6f28 7365 6c66 2e46 3130 290a 0a20 2020  o(self.F10)..   
-0000b9a0: 2064 6566 2065 6469 745f 4631 3128 7365   def edit_F11(se
-0000b9b0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-0000b9c0: 7374 7562 2222 220a 2020 2020 2020 2020  stub""".        
-0000b9d0: 6c6f 6767 6572 2e64 6562 7567 2822 4631  logger.debug("F1
-0000b9e0: 3120 5269 6768 7420 436c 6963 6b65 642e  1 Right Clicked.
-0000b9f0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-0000ba00: 6564 6974 5f6d 6163 726f 2873 656c 662e  edit_macro(self.
-0000ba10: 4631 3129 0a0a 2020 2020 6465 6620 6564  F11)..    def ed
-0000ba20: 6974 5f46 3132 2873 656c 6629 3a0a 2020  it_F12(self):.  
-0000ba30: 2020 2020 2020 2222 2273 7475 6222 2222        """stub"""
-0000ba40: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
-0000ba50: 6465 6275 6728 2246 3132 2052 6967 6874  debug("F12 Right
-0000ba60: 2043 6c69 636b 6564 2e22 290a 2020 2020   Clicked.").    
-0000ba70: 2020 2020 7365 6c66 2e65 6469 745f 6d61      self.edit_ma
-0000ba80: 6372 6f28 7365 6c66 2e46 3132 290a 0a20  cro(self.F12).. 
-0000ba90: 2020 2064 6566 2070 726f 6365 7373 5f6d     def process_m
-0000baa0: 6163 726f 2873 656c 662c 206d 6163 726f  acro(self, macro
-0000bab0: 3a20 7374 7229 202d 3e20 7374 723a 0a20  : str) -> str:. 
-0000bac0: 2020 2020 2020 2022 2222 5072 6f63 6573         """Proces
-0000bad0: 7320 4357 206d 6163 726f 2073 7562 7374  s CW macro subst
-0000bae0: 6974 7574 696f 6e73 2222 220a 2020 2020  itutions""".    
-0000baf0: 2020 2020 7265 7375 6c74 203d 2073 656c      result = sel
-0000bb00: 662e 6461 7461 6261 7365 2e67 6574 5f73  f.database.get_s
-0000bb10: 6572 6961 6c28 290a 2020 2020 2020 2020  erial().        
-0000bb20: 6e65 7874 5f73 6572 6961 6c20 3d20 7374  next_serial = st
-0000bb30: 7228 7265 7375 6c74 2e67 6574 2822 7365  r(result.get("se
-0000bb40: 7269 616c 5f6e 7222 2c20 2231 2229 290a  rial_nr", "1")).
-0000bb50: 2020 2020 2020 2020 6966 206e 6578 745f          if next_
-0000bb60: 7365 7269 616c 203d 3d20 224e 6f6e 6522  serial == "None"
-0000bb70: 3a0a 2020 2020 2020 2020 2020 2020 6e65  :.            ne
-0000bb80: 7874 5f73 6572 6961 6c20 3d20 2231 220a  xt_serial = "1".
-0000bb90: 2020 2020 2020 2020 6d61 6372 6f20 3d20          macro = 
-0000bba0: 6d61 6372 6f2e 7570 7065 7228 290a 2020  macro.upper().  
-0000bbb0: 2020 2020 2020 6d61 6372 6f20 3d20 6d61        macro = ma
-0000bbc0: 6372 6f2e 7265 706c 6163 6528 2223 222c  cro.replace("#",
-0000bbd0: 206e 6578 745f 7365 7269 616c 290a 2020   next_serial).  
-0000bbe0: 2020 2020 2020 6d61 6372 6f20 3d20 6d61        macro = ma
-0000bbf0: 6372 6f2e 7265 706c 6163 6528 227b 4d59  cro.replace("{MY
-0000bc00: 4341 4c4c 7d22 2c20 7365 6c66 2e73 7461  CALL}", self.sta
-0000bc10: 7469 6f6e 2e67 6574 2822 4361 6c6c 222c  tion.get("Call",
-0000bc20: 2022 2229 290a 2020 2020 2020 2020 6d61   "")).        ma
-0000bc30: 6372 6f20 3d20 6d61 6372 6f2e 7265 706c  cro = macro.repl
-0000bc40: 6163 6528 227b 4849 5343 414c 4c7d 222c  ace("{HISCALL}",
-0000bc50: 2073 656c 662e 6361 6c6c 7369 676e 2e74   self.callsign.t
-0000bc60: 6578 7428 2929 0a20 2020 2020 2020 2069  ext()).        i
-0000bc70: 6620 7365 6c66 2e72 6164 696f 5f73 7461  f self.radio_sta
-0000bc80: 7465 2e67 6574 2822 6d6f 6465 2229 203d  te.get("mode") =
-0000bc90: 3d20 2243 5722 3a0a 2020 2020 2020 2020  = "CW":.        
-0000bca0: 2020 2020 6d61 6372 6f20 3d20 6d61 6372      macro = macr
-0000bcb0: 6f2e 7265 706c 6163 6528 227b 534e 547d  o.replace("{SNT}
-0000bcc0: 222c 2073 656c 662e 7365 6e74 2e74 6578  ", self.sent.tex
-0000bcd0: 7428 292e 7265 706c 6163 6528 2239 222c  t().replace("9",
-0000bce0: 2022 6e22 2929 0a20 2020 2020 2020 2065   "n")).        e
-0000bcf0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000bd00: 206d 6163 726f 203d 206d 6163 726f 2e72   macro = macro.r
-0000bd10: 6570 6c61 6365 2822 7b53 4e54 7d22 2c20  eplace("{SNT}", 
-0000bd20: 7365 6c66 2e73 656e 742e 7465 7874 2829  self.sent.text()
-0000bd30: 290a 2020 2020 2020 2020 6d61 6372 6f20  ).        macro 
-0000bd40: 3d20 6d61 6372 6f2e 7265 706c 6163 6528  = macro.replace(
-0000bd50: 227b 5345 4e54 4e52 7d22 2c20 7365 6c66  "{SENTNR}", self
-0000bd60: 2e6f 7468 6572 5f31 2e74 6578 7428 2929  .other_1.text())
-0000bd70: 0a20 2020 2020 2020 206d 6163 726f 203d  .        macro =
-0000bd80: 206d 6163 726f 2e72 6570 6c61 6365 280a   macro.replace(.
-0000bd90: 2020 2020 2020 2020 2020 2020 227b 4558              "{EX
-0000bda0: 4348 7d22 2c20 7365 6c66 2e63 6f6e 7465  CH}", self.conte
-0000bdb0: 7374 5f73 6574 7469 6e67 732e 6765 7428  st_settings.get(
-0000bdc0: 2253 656e 7445 7863 6861 6e67 6522 2c20  "SentExchange", 
-0000bdd0: 2278 7878 2229 0a20 2020 2020 2020 2029  "xxx").        )
-0000bde0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000bdf0: 6d61 6372 6f0a 0a20 2020 2064 6566 2076  macro..    def v
-0000be00: 6f69 6365 5f73 7472 696e 6728 7365 6c66  oice_string(self
-0000be10: 2c20 7468 655f 7374 7269 6e67 3a20 7374  , the_string: st
-0000be20: 7229 202d 3e20 4e6f 6e65 3a0a 2020 2020  r) -> None:.    
-0000be30: 2020 2020 2222 2276 6f69 6365 7320 7374      """voices st
-0000be40: 7269 6e67 2075 7369 6e67 206e 6174 6f20  ring using nato 
-0000be50: 7068 6f6e 6574 6963 7322 2222 0a20 2020  phonetics""".   
-0000be60: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-0000be70: 6728 2256 6f69 6369 6e67 3a20 2573 222c  g("Voicing: %s",
-0000be80: 2074 6865 5f73 7472 696e 6729 0a20 2020   the_string).   
-0000be90: 2020 2020 206f 705f 7061 7468 203d 2050       op_path = P
-0000bea0: 6174 6828 4441 5441 5f50 4154 4829 202f  ath(DATA_PATH) /
-0000beb0: 2073 656c 662e 6375 7272 656e 745f 6f70   self.current_op
-0000bec0: 0a20 2020 2020 2020 2069 6620 225b 2220  .        if "[" 
-0000bed0: 696e 2074 6865 5f73 7472 696e 673a 0a20  in the_string:. 
-0000bee0: 2020 2020 2020 2020 2020 2073 7562 5f73             sub_s
-0000bef0: 7472 696e 6720 3d20 7468 655f 7374 7269  tring = the_stri
-0000bf00: 6e67 2e73 7472 6970 2822 5b5d 2229 2e6c  ng.strip("[]").l
-0000bf10: 6f77 6572 2829 0a20 2020 2020 2020 2020  ower().         
-0000bf20: 2020 2066 696c 656e 616d 6520 3d20 6622     filename = f"
-0000bf30: 7b73 7472 286f 705f 7061 7468 297d 2f7b  {str(op_path)}/{
-0000bf40: 7375 625f 7374 7269 6e67 7d2e 7761 7622  sub_string}.wav"
-0000bf50: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000bf60: 5061 7468 2866 696c 656e 616d 6529 2e69  Path(filename).i
-0000bf70: 735f 6669 6c65 2829 3a0a 2020 2020 2020  s_file():.      
-0000bf80: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-0000bf90: 2e64 6562 7567 2822 566f 6963 696e 673a  .debug("Voicing:
-0000bfa0: 2025 7322 2c20 6669 6c65 6e61 6d65 290a   %s", filename).
-0000bfb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bfc0: 6461 7461 2c20 5f66 7320 3d20 7366 2e72  data, _fs = sf.r
-0000bfd0: 6561 6428 6669 6c65 6e61 6d65 2c20 6474  ead(filename, dt
-0000bfe0: 7970 653d 2266 6c6f 6174 3332 2229 0a20  ype="float32"). 
-0000bff0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000c000: 656c 662e 7074 745f 6f6e 2829 0a20 2020  elf.ptt_on().   
-0000c010: 2020 2020 2020 2020 2020 2020 2074 7279               try
-0000c020: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000c030: 2020 2020 2020 7364 2e64 6566 6175 6c74        sd.default
-0000c040: 2e64 6576 6963 6520 3d20 7365 6c66 2e70  .device = self.p
-0000c050: 7265 662e 6765 7428 2273 6f75 6e64 6465  ref.get("soundde
-0000c060: 7669 6365 222c 2022 6465 6661 756c 7422  vice", "default"
-0000c070: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000c080: 2020 2020 2020 7364 2e64 6566 6175 6c74        sd.default
-0000c090: 2e73 616d 706c 6572 6174 6520 3d20 3434  .samplerate = 44
-0000c0a0: 3130 302e 300a 2020 2020 2020 2020 2020  100.0.          
-0000c0b0: 2020 2020 2020 2020 2020 7364 2e70 6c61            sd.pla
-0000c0c0: 7928 6461 7461 290a 2020 2020 2020 2020  y(data).        
-0000c0d0: 2020 2020 2020 2020 2020 2020 5f73 7461              _sta
-0000c0e0: 7475 7320 3d20 7364 2e77 6169 7428 290a  tus = sd.wait().
-0000c0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c100: 2020 2020 2320 6874 7470 733a 2f2f 736e      # https://sn
-0000c110: 796b 2e69 6f2f 6164 7669 736f 722f 7079  yk.io/advisor/py
-0000c120: 7468 6f6e 2f73 6f75 6e64 6465 7669 6365  thon/sounddevice
-0000c130: 2f66 756e 6374 696f 6e73 2f73 6f75 6e64  /functions/sound
-0000c140: 6465 7669 6365 2e50 6f72 7441 7564 696f  device.PortAudio
-0000c150: 4572 726f 720a 2020 2020 2020 2020 2020  Error.          
-0000c160: 2020 2020 2020 6578 6365 7074 2073 642e        except sd.
-0000c170: 506f 7274 4175 6469 6f45 7272 6f72 2061  PortAudioError a
-0000c180: 7320 6572 723a 0a20 2020 2020 2020 2020  s err:.         
-0000c190: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-0000c1a0: 722e 6465 6275 6728 2225 7322 2c20 6622  r.debug("%s", f"
-0000c1b0: 7b65 7272 7d22 290a 0a20 2020 2020 2020  {err}")..       
-0000c1c0: 2020 2020 2020 2020 2073 656c 662e 7074           self.pt
-0000c1d0: 745f 6f66 6628 290a 2020 2020 2020 2020  t_off().        
-0000c1e0: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-0000c1f0: 2020 2073 656c 662e 7074 745f 6f6e 2829     self.ptt_on()
-0000c200: 0a20 2020 2020 2020 2066 6f72 206c 6574  .        for let
-0000c210: 7465 7220 696e 2074 6865 5f73 7472 696e  ter in the_strin
-0000c220: 672e 6c6f 7765 7228 293a 0a20 2020 2020  g.lower():.     
-0000c230: 2020 2020 2020 2069 6620 6c65 7474 6572         if letter
-0000c240: 2069 6e20 2261 6263 6465 6667 6869 6a6b   in "abcdefghijk
-0000c250: 6c6d 6e6f 7071 7273 7475 7677 7879 7a20  lmnopqrstuvwxyz 
-0000c260: 3132 3334 3536 3738 3930 223a 0a20 2020  1234567890":.   
-0000c270: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000c280: 6c65 7474 6572 203d 3d20 2220 223a 0a20  letter == " ":. 
-0000c290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c2a0: 2020 206c 6574 7465 7220 3d20 2273 7061     letter = "spa
-0000c2b0: 6365 220a 2020 2020 2020 2020 2020 2020  ce".            
-0000c2c0: 2020 2020 6669 6c65 6e61 6d65 203d 2066      filename = f
-0000c2d0: 227b 7374 7228 6f70 5f70 6174 6829 7d2f  "{str(op_path)}/
-0000c2e0: 7b6c 6574 7465 727d 2e77 6176 220a 2020  {letter}.wav".  
-0000c2f0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000c300: 2050 6174 6828 6669 6c65 6e61 6d65 292e   Path(filename).
-0000c310: 6973 5f66 696c 6528 293a 0a20 2020 2020  is_file():.     
-0000c320: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-0000c330: 6f67 6765 722e 6465 6275 6728 2256 6f69  ogger.debug("Voi
-0000c340: 6369 6e67 3a20 2573 222c 2066 696c 656e  cing: %s", filen
-0000c350: 616d 6529 0a20 2020 2020 2020 2020 2020  ame).           
-0000c360: 2020 2020 2020 2020 2064 6174 612c 205f           data, _
-0000c370: 6673 203d 2073 662e 7265 6164 2866 696c  fs = sf.read(fil
-0000c380: 656e 616d 652c 2064 7479 7065 3d22 666c  ename, dtype="fl
-0000c390: 6f61 7433 3222 290a 2020 2020 2020 2020  oat32").        
-0000c3a0: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-0000c3b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c3c0: 2020 2020 2020 2020 2073 642e 6465 6661           sd.defa
-0000c3d0: 756c 742e 6465 7669 6365 203d 2073 656c  ult.device = sel
-0000c3e0: 662e 7072 6566 2e67 6574 2822 736f 756e  f.pref.get("soun
-0000c3f0: 6464 6576 6963 6522 2c20 2264 6566 6175  ddevice", "defau
-0000c400: 6c74 2229 0a20 2020 2020 2020 2020 2020  lt").           
-0000c410: 2020 2020 2020 2020 2020 2020 2073 642e               sd.
-0000c420: 6465 6661 756c 742e 7361 6d70 6c65 7261  default.samplera
-0000c430: 7465 203d 2034 3431 3030 2e30 0a20 2020  te = 44100.0.   
-0000c440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c450: 2020 2020 2073 642e 706c 6179 2864 6174       sd.play(dat
-0000c460: 6129 0a20 2020 2020 2020 2020 2020 2020  a).             
-0000c470: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-0000c480: 722e 6465 6275 6728 2225 7322 2c20 6622  r.debug("%s", f"
-0000c490: 7b73 642e 7761 6974 2829 7d22 290a 2020  {sd.wait()}").  
-0000c4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c4b0: 2020 6578 6365 7074 2073 642e 506f 7274    except sd.Port
-0000c4c0: 4175 6469 6f45 7272 6f72 2061 7320 6572  AudioError as er
-0000c4d0: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
-0000c4e0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-0000c4f0: 722e 6465 6275 6728 2225 7322 2c20 6622  r.debug("%s", f"
-0000c500: 7b65 7272 7d22 290a 2020 2020 2020 2020  {err}").        
-0000c510: 7365 6c66 2e70 7474 5f6f 6666 2829 0a0a  self.ptt_off()..
-0000c520: 2020 2020 6465 6620 7074 745f 6f6e 2873      def ptt_on(s
-0000c530: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-0000c540: 2274 7572 6e20 6f6e 2070 7474 2222 220a  "turn on ptt""".
-0000c550: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000c560: 7269 675f 636f 6e74 726f 6c3a 0a20 2020  rig_control:.   
-0000c570: 2020 2020 2020 2020 2073 656c 662e 6c65           self.le
-0000c580: 6674 646f 742e 7365 7450 6978 6d61 7028  ftdot.setPixmap(
-0000c590: 7365 6c66 2e67 7265 656e 646f 7429 0a20  self.greendot). 
-0000c5a0: 2020 2020 2020 2020 2020 2061 7070 2e70             app.p
-0000c5b0: 726f 6365 7373 4576 656e 7473 2829 0a20  rocessEvents(). 
-0000c5c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000c5d0: 7269 675f 636f 6e74 726f 6c2e 7074 745f  rig_control.ptt_
-0000c5e0: 6f6e 2829 0a0a 2020 2020 6465 6620 7074  on()..    def pt
-0000c5f0: 745f 6f66 6628 7365 6c66 293a 0a20 2020  t_off(self):.   
-0000c600: 2020 2020 2022 2222 7475 726e 206f 6666       """turn off
-0000c610: 2070 7474 2222 220a 2020 2020 2020 2020   ptt""".        
-0000c620: 6966 2073 656c 662e 7269 675f 636f 6e74  if self.rig_cont
-0000c630: 726f 6c3a 0a20 2020 2020 2020 2020 2020  rol:.           
-0000c640: 2073 656c 662e 6c65 6674 646f 742e 7365   self.leftdot.se
-0000c650: 7450 6978 6d61 7028 7365 6c66 2e72 6564  tPixmap(self.red
-0000c660: 646f 7429 0a20 2020 2020 2020 2020 2020  dot).           
-0000c670: 2061 7070 2e70 726f 6365 7373 4576 656e   app.processEven
-0000c680: 7473 2829 0a20 2020 2020 2020 2020 2020  ts().           
-0000c690: 2073 656c 662e 7269 675f 636f 6e74 726f   self.rig_contro
-0000c6a0: 6c2e 7074 745f 6f66 6628 290a 0a20 2020  l.ptt_off()..   
-0000c6b0: 2064 6566 2073 656e 6466 3128 7365 6c66   def sendf1(self
-0000c6c0: 293a 0a20 2020 2020 2020 2022 2222 7374  ):.        """st
-0000c6d0: 7562 2222 220a 2020 2020 2020 2020 6c6f  ub""".        lo
-0000c6e0: 6767 6572 2e64 6562 7567 2822 4631 2043  gger.debug("F1 C
-0000c6f0: 6c69 636b 6564 2229 0a20 2020 2020 2020  licked").       
-0000c700: 2069 6620 7365 6c66 2e72 6164 696f 5f73   if self.radio_s
-0000c710: 7461 7465 2e67 6574 2822 6d6f 6465 2229  tate.get("mode")
-0000c720: 2069 6e20 5b22 4c53 4222 2c20 2255 5342   in ["LSB", "USB
-0000c730: 222c 2022 5353 4222 5d3a 0a20 2020 2020  ", "SSB"]:.     
-0000c740: 2020 2020 2020 2073 656c 662e 766f 6963         self.voic
-0000c750: 655f 7374 7269 6e67 2873 656c 662e 7072  e_string(self.pr
-0000c760: 6f63 6573 735f 6d61 6372 6f28 7365 6c66  ocess_macro(self
-0000c770: 2e46 312e 746f 6f6c 5469 7028 2929 290a  .F1.toolTip())).
-0000c780: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000c790: 726e 0a20 2020 2020 2020 2069 6620 7365  rn.        if se
-0000c7a0: 6c66 2e63 773a 0a20 2020 2020 2020 2020  lf.cw:.         
-0000c7b0: 2020 2023 2069 6620 7365 6c66 2e70 7265     # if self.pre
-0000c7c0: 6665 7265 6e63 652e 6765 7428 2273 656e  ference.get("sen
-0000c7d0: 645f 6e31 6d6d 5f70 6163 6b65 7473 2229  d_n1mm_packets")
-0000c7e0: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-0000c7f0: 2020 2020 7365 6c66 2e6e 316d 6d2e 7261      self.n1mm.ra
-0000c800: 6469 6f5f 696e 666f 5b22 4675 6e63 7469  dio_info["Functi
-0000c810: 6f6e 4b65 7943 6170 7469 6f6e 225d 203d  onKeyCaption"] =
-0000c820: 2073 656c 662e 4631 2e74 6578 7428 290a   self.F1.text().
-0000c830: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000c840: 2e63 772e 7365 6e64 6377 2873 656c 662e  .cw.sendcw(self.
-0000c850: 7072 6f63 6573 735f 6d61 6372 6f28 7365  process_macro(se
-0000c860: 6c66 2e46 312e 746f 6f6c 5469 7028 2929  lf.F1.toolTip())
-0000c870: 290a 0a20 2020 2064 6566 2073 656e 6466  )..    def sendf
-0000c880: 3228 7365 6c66 293a 0a20 2020 2020 2020  2(self):.       
-0000c890: 2022 2222 7374 7562 2222 220a 2020 2020   """stub""".    
-0000c8a0: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
-0000c8b0: 2822 4632 2043 6c69 636b 6564 2229 0a20  ("F2 Clicked"). 
-0000c8c0: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
-0000c8d0: 6164 696f 5f73 7461 7465 2e67 6574 2822  adio_state.get("
-0000c8e0: 6d6f 6465 2229 2069 6e20 5b22 4c53 4222  mode") in ["LSB"
-0000c8f0: 2c20 2255 5342 222c 2022 5353 4222 5d3a  , "USB", "SSB"]:
-0000c900: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000c910: 662e 766f 6963 655f 7374 7269 6e67 2873  f.voice_string(s
-0000c920: 656c 662e 7072 6f63 6573 735f 6d61 6372  elf.process_macr
-0000c930: 6f28 7365 6c66 2e46 322e 746f 6f6c 5469  o(self.F2.toolTi
-0000c940: 7028 2929 290a 2020 2020 2020 2020 2020  p())).          
-0000c950: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
-0000c960: 2069 6620 7365 6c66 2e63 773a 0a20 2020   if self.cw:.   
-0000c970: 2020 2020 2020 2020 2073 656c 662e 6377           self.cw
-0000c980: 2e73 656e 6463 7728 7365 6c66 2e70 726f  .sendcw(self.pro
-0000c990: 6365 7373 5f6d 6163 726f 2873 656c 662e  cess_macro(self.
-0000c9a0: 4632 2e74 6f6f 6c54 6970 2829 2929 0a0a  F2.toolTip()))..
-0000c9b0: 2020 2020 6465 6620 7365 6e64 6633 2873      def sendf3(s
-0000c9c0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-0000c9d0: 2273 7475 6222 2222 0a20 2020 2020 2020  "stub""".       
-0000c9e0: 206c 6f67 6765 722e 6465 6275 6728 2246   logger.debug("F
-0000c9f0: 3320 436c 6963 6b65 6422 290a 2020 2020  3 Clicked").    
-0000ca00: 2020 2020 6966 2073 656c 662e 7261 6469      if self.radi
-0000ca10: 6f5f 7374 6174 652e 6765 7428 226d 6f64  o_state.get("mod
-0000ca20: 6522 2920 696e 205b 224c 5342 222c 2022  e") in ["LSB", "
-0000ca30: 5553 4222 2c20 2253 5342 225d 3a0a 2020  USB", "SSB"]:.  
-0000ca40: 2020 2020 2020 2020 2020 7365 6c66 2e76            self.v
-0000ca50: 6f69 6365 5f73 7472 696e 6728 7365 6c66  oice_string(self
-0000ca60: 2e70 726f 6365 7373 5f6d 6163 726f 2873  .process_macro(s
-0000ca70: 656c 662e 4633 2e74 6f6f 6c54 6970 2829  elf.F3.toolTip()
-0000ca80: 2929 0a20 2020 2020 2020 2020 2020 2072  )).            r
-0000ca90: 6574 7572 6e0a 2020 2020 2020 2020 6966  eturn.        if
-0000caa0: 2073 656c 662e 6377 3a0a 2020 2020 2020   self.cw:.      
-0000cab0: 2020 2020 2020 7365 6c66 2e63 772e 7365        self.cw.se
-0000cac0: 6e64 6377 2873 656c 662e 7072 6f63 6573  ndcw(self.proces
-0000cad0: 735f 6d61 6372 6f28 7365 6c66 2e46 332e  s_macro(self.F3.
-0000cae0: 746f 6f6c 5469 7028 2929 290a 0a20 2020  toolTip()))..   
-0000caf0: 2064 6566 2073 656e 6466 3428 7365 6c66   def sendf4(self
-0000cb00: 293a 0a20 2020 2020 2020 2022 2222 7374  ):.        """st
-0000cb10: 7562 2222 220a 2020 2020 2020 2020 6c6f  ub""".        lo
-0000cb20: 6767 6572 2e64 6562 7567 2822 4634 2043  gger.debug("F4 C
-0000cb30: 6c69 636b 6564 2229 0a20 2020 2020 2020  licked").       
-0000cb40: 2069 6620 7365 6c66 2e72 6164 696f 5f73   if self.radio_s
-0000cb50: 7461 7465 2e67 6574 2822 6d6f 6465 2229  tate.get("mode")
-0000cb60: 2069 6e20 5b22 4c53 4222 2c20 2255 5342   in ["LSB", "USB
-0000cb70: 222c 2022 5353 4222 5d3a 0a20 2020 2020  ", "SSB"]:.     
-0000cb80: 2020 2020 2020 2073 656c 662e 766f 6963         self.voic
-0000cb90: 655f 7374 7269 6e67 2873 656c 662e 7072  e_string(self.pr
-0000cba0: 6f63 6573 735f 6d61 6372 6f28 7365 6c66  ocess_macro(self
-0000cbb0: 2e46 342e 746f 6f6c 5469 7028 2929 290a  .F4.toolTip())).
-0000cbc0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000cbd0: 726e 0a20 2020 2020 2020 2069 6620 7365  rn.        if se
-0000cbe0: 6c66 2e63 773a 0a20 2020 2020 2020 2020  lf.cw:.         
-0000cbf0: 2020 2073 656c 662e 6377 2e73 656e 6463     self.cw.sendc
-0000cc00: 7728 7365 6c66 2e70 726f 6365 7373 5f6d  w(self.process_m
-0000cc10: 6163 726f 2873 656c 662e 4634 2e74 6f6f  acro(self.F4.too
-0000cc20: 6c54 6970 2829 2929 0a0a 2020 2020 6465  lTip()))..    de
-0000cc30: 6620 7365 6e64 6635 2873 656c 6629 3a0a  f sendf5(self):.
-0000cc40: 2020 2020 2020 2020 2222 2273 7475 6222          """stub"
-0000cc50: 2222 0a20 2020 2020 2020 206c 6f67 6765  "".        logge
-0000cc60: 722e 6465 6275 6728 2246 3520 436c 6963  r.debug("F5 Clic
-0000cc70: 6b65 6422 290a 2020 2020 2020 2020 6966  ked").        if
-0000cc80: 2073 656c 662e 7261 6469 6f5f 7374 6174   self.radio_stat
-0000cc90: 652e 6765 7428 226d 6f64 6522 2920 696e  e.get("mode") in
-0000cca0: 205b 224c 5342 222c 2022 5553 4222 2c20   ["LSB", "USB", 
-0000ccb0: 2253 5342 225d 3a0a 2020 2020 2020 2020  "SSB"]:.        
-0000ccc0: 2020 2020 7365 6c66 2e76 6f69 6365 5f73      self.voice_s
-0000ccd0: 7472 696e 6728 7365 6c66 2e70 726f 6365  tring(self.proce
-0000cce0: 7373 5f6d 6163 726f 2873 656c 662e 4635  ss_macro(self.F5
-0000ccf0: 2e74 6f6f 6c54 6970 2829 2929 0a20 2020  .toolTip())).   
-0000cd00: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
-0000cd10: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000cd20: 6377 3a0a 2020 2020 2020 2020 2020 2020  cw:.            
-0000cd30: 7365 6c66 2e63 772e 7365 6e64 6377 2873  self.cw.sendcw(s
-0000cd40: 656c 662e 7072 6f63 6573 735f 6d61 6372  elf.process_macr
-0000cd50: 6f28 7365 6c66 2e46 352e 746f 6f6c 5469  o(self.F5.toolTi
-0000cd60: 7028 2929 290a 0a20 2020 2064 6566 2073  p()))..    def s
-0000cd70: 656e 6466 3628 7365 6c66 293a 0a20 2020  endf6(self):.   
-0000cd80: 2020 2020 2022 2222 7374 7562 2222 220a       """stub""".
-0000cd90: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-0000cda0: 6562 7567 2822 4636 2043 6c69 636b 6564  ebug("F6 Clicked
-0000cdb0: 2229 0a20 2020 2020 2020 2069 6620 7365  ").        if se
-0000cdc0: 6c66 2e72 6164 696f 5f73 7461 7465 2e67  lf.radio_state.g
-0000cdd0: 6574 2822 6d6f 6465 2229 2069 6e20 5b22  et("mode") in ["
-0000cde0: 4c53 4222 2c20 2255 5342 222c 2022 5353  LSB", "USB", "SS
-0000cdf0: 4222 5d3a 0a20 2020 2020 2020 2020 2020  B"]:.           
-0000ce00: 2073 656c 662e 766f 6963 655f 7374 7269   self.voice_stri
-0000ce10: 6e67 2873 656c 662e 7072 6f63 6573 735f  ng(self.process_
-0000ce20: 6d61 6372 6f28 7365 6c66 2e46 362e 746f  macro(self.F6.to
-0000ce30: 6f6c 5469 7028 2929 290a 2020 2020 2020  olTip())).      
-0000ce40: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
-0000ce50: 2020 2020 2069 6620 7365 6c66 2e63 773a       if self.cw:
-0000ce60: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000ce70: 662e 6377 2e73 656e 6463 7728 7365 6c66  f.cw.sendcw(self
-0000ce80: 2e70 726f 6365 7373 5f6d 6163 726f 2873  .process_macro(s
-0000ce90: 656c 662e 4636 2e74 6f6f 6c54 6970 2829  elf.F6.toolTip()
-0000cea0: 2929 0a0a 2020 2020 6465 6620 7365 6e64  ))..    def send
-0000ceb0: 6637 2873 656c 6629 3a0a 2020 2020 2020  f7(self):.      
-0000cec0: 2020 2222 2273 7475 6222 2222 0a20 2020    """stub""".   
-0000ced0: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-0000cee0: 6728 2246 3720 436c 6963 6b65 6422 290a  g("F7 Clicked").
-0000cef0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000cf00: 7261 6469 6f5f 7374 6174 652e 6765 7428  radio_state.get(
-0000cf10: 226d 6f64 6522 2920 696e 205b 224c 5342  "mode") in ["LSB
-0000cf20: 222c 2022 5553 4222 2c20 2253 5342 225d  ", "USB", "SSB"]
-0000cf30: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000cf40: 6c66 2e76 6f69 6365 5f73 7472 696e 6728  lf.voice_string(
-0000cf50: 7365 6c66 2e70 726f 6365 7373 5f6d 6163  self.process_mac
-0000cf60: 726f 2873 656c 662e 4637 2e74 6f6f 6c54  ro(self.F7.toolT
-0000cf70: 6970 2829 2929 0a20 2020 2020 2020 2020  ip())).         
-0000cf80: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
-0000cf90: 2020 6966 2073 656c 662e 6377 3a0a 2020    if self.cw:.  
-0000cfa0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-0000cfb0: 772e 7365 6e64 6377 2873 656c 662e 7072  w.sendcw(self.pr
-0000cfc0: 6f63 6573 735f 6d61 6372 6f28 7365 6c66  ocess_macro(self
-0000cfd0: 2e46 372e 746f 6f6c 5469 7028 2929 290a  .F7.toolTip())).
-0000cfe0: 0a20 2020 2064 6566 2073 656e 6466 3828  .    def sendf8(
-0000cff0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-0000d000: 2222 7374 7562 2222 220a 2020 2020 2020  ""stub""".      
-0000d010: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
-0000d020: 4638 2043 6c69 636b 6564 2229 0a20 2020  F8 Clicked").   
-0000d030: 2020 2020 2069 6620 7365 6c66 2e72 6164       if self.rad
-0000d040: 696f 5f73 7461 7465 2e67 6574 2822 6d6f  io_state.get("mo
-0000d050: 6465 2229 2069 6e20 5b22 4c53 4222 2c20  de") in ["LSB", 
-0000d060: 2255 5342 222c 2022 5353 4222 5d3a 0a20  "USB", "SSB"]:. 
-0000d070: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000d080: 766f 6963 655f 7374 7269 6e67 2873 656c  voice_string(sel
-0000d090: 662e 7072 6f63 6573 735f 6d61 6372 6f28  f.process_macro(
-0000d0a0: 7365 6c66 2e46 382e 746f 6f6c 5469 7028  self.F8.toolTip(
-0000d0b0: 2929 290a 2020 2020 2020 2020 2020 2020  ))).            
-0000d0c0: 7265 7475 726e 0a20 2020 2020 2020 2069  return.        i
-0000d0d0: 6620 7365 6c66 2e63 773a 0a20 2020 2020  f self.cw:.     
-0000d0e0: 2020 2020 2020 2073 656c 662e 6377 2e73         self.cw.s
-0000d0f0: 656e 6463 7728 7365 6c66 2e70 726f 6365  endcw(self.proce
-0000d100: 7373 5f6d 6163 726f 2873 656c 662e 4638  ss_macro(self.F8
-0000d110: 2e74 6f6f 6c54 6970 2829 2929 0a0a 2020  .toolTip()))..  
-0000d120: 2020 6465 6620 7365 6e64 6639 2873 656c    def sendf9(sel
-0000d130: 6629 3a0a 2020 2020 2020 2020 2222 2273  f):.        """s
-0000d140: 7475 6222 2222 0a20 2020 2020 2020 206c  tub""".        l
-0000d150: 6f67 6765 722e 6465 6275 6728 2246 3920  ogger.debug("F9 
-0000d160: 436c 6963 6b65 6422 290a 2020 2020 2020  Clicked").      
-0000d170: 2020 6966 2073 656c 662e 7261 6469 6f5f    if self.radio_
-0000d180: 7374 6174 652e 6765 7428 226d 6f64 6522  state.get("mode"
-0000d190: 2920 696e 205b 224c 5342 222c 2022 5553  ) in ["LSB", "US
-0000d1a0: 4222 2c20 2253 5342 225d 3a0a 2020 2020  B", "SSB"]:.    
-0000d1b0: 2020 2020 2020 2020 7365 6c66 2e76 6f69          self.voi
-0000d1c0: 6365 5f73 7472 696e 6728 7365 6c66 2e70  ce_string(self.p
-0000d1d0: 726f 6365 7373 5f6d 6163 726f 2873 656c  rocess_macro(sel
-0000d1e0: 662e 4639 2e74 6f6f 6c54 6970 2829 2929  f.F9.toolTip()))
-0000d1f0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000d200: 7572 6e0a 2020 2020 2020 2020 6966 2073  urn.        if s
-0000d210: 656c 662e 6377 3a0a 2020 2020 2020 2020  elf.cw:.        
-0000d220: 2020 2020 7365 6c66 2e63 772e 7365 6e64      self.cw.send
-0000d230: 6377 2873 656c 662e 7072 6f63 6573 735f  cw(self.process_
-0000d240: 6d61 6372 6f28 7365 6c66 2e46 392e 746f  macro(self.F9.to
-0000d250: 6f6c 5469 7028 2929 290a 0a20 2020 2064  olTip()))..    d
-0000d260: 6566 2073 656e 6466 3130 2873 656c 6629  ef sendf10(self)
-0000d270: 3a0a 2020 2020 2020 2020 2222 2273 7475  :.        """stu
-0000d280: 6222 2222 0a20 2020 2020 2020 206c 6f67  b""".        log
-0000d290: 6765 722e 6465 6275 6728 2246 3130 2043  ger.debug("F10 C
-0000d2a0: 6c69 636b 6564 2229 0a20 2020 2020 2020  licked").       
-0000d2b0: 2069 6620 7365 6c66 2e72 6164 696f 5f73   if self.radio_s
-0000d2c0: 7461 7465 2e67 6574 2822 6d6f 6465 2229  tate.get("mode")
-0000d2d0: 2069 6e20 5b22 4c53 4222 2c20 2255 5342   in ["LSB", "USB
-0000d2e0: 222c 2022 5353 4222 5d3a 0a20 2020 2020  ", "SSB"]:.     
-0000d2f0: 2020 2020 2020 2073 656c 662e 766f 6963         self.voic
-0000d300: 655f 7374 7269 6e67 2873 656c 662e 7072  e_string(self.pr
-0000d310: 6f63 6573 735f 6d61 6372 6f28 7365 6c66  ocess_macro(self
-0000d320: 2e46 3130 2e74 6f6f 6c54 6970 2829 2929  .F10.toolTip()))
-0000d330: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000d340: 7572 6e0a 2020 2020 2020 2020 6966 2073  urn.        if s
-0000d350: 656c 662e 6377 3a0a 2020 2020 2020 2020  elf.cw:.        
-0000d360: 2020 2020 7365 6c66 2e63 772e 7365 6e64      self.cw.send
-0000d370: 6377 2873 656c 662e 7072 6f63 6573 735f  cw(self.process_
-0000d380: 6d61 6372 6f28 7365 6c66 2e46 3130 2e74  macro(self.F10.t
-0000d390: 6f6f 6c54 6970 2829 2929 0a0a 2020 2020  oolTip()))..    
-0000d3a0: 6465 6620 7365 6e64 6631 3128 7365 6c66  def sendf11(self
-0000d3b0: 293a 0a20 2020 2020 2020 2022 2222 7374  ):.        """st
-0000d3c0: 7562 2222 220a 2020 2020 2020 2020 6c6f  ub""".        lo
-0000d3d0: 6767 6572 2e64 6562 7567 2822 4631 3120  gger.debug("F11 
-0000d3e0: 436c 6963 6b65 6422 290a 2020 2020 2020  Clicked").      
-0000d3f0: 2020 6966 2073 656c 662e 7261 6469 6f5f    if self.radio_
-0000d400: 7374 6174 652e 6765 7428 226d 6f64 6522  state.get("mode"
-0000d410: 2920 696e 205b 224c 5342 222c 2022 5553  ) in ["LSB", "US
-0000d420: 4222 2c20 2253 5342 225d 3a0a 2020 2020  B", "SSB"]:.    
-0000d430: 2020 2020 2020 2020 7365 6c66 2e76 6f69          self.voi
-0000d440: 6365 5f73 7472 696e 6728 7365 6c66 2e70  ce_string(self.p
-0000d450: 726f 6365 7373 5f6d 6163 726f 2873 656c  rocess_macro(sel
-0000d460: 662e 4631 312e 746f 6f6c 5469 7028 2929  f.F11.toolTip())
-0000d470: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-0000d480: 7475 726e 0a20 2020 2020 2020 2069 6620  turn.        if 
-0000d490: 7365 6c66 2e63 773a 0a20 2020 2020 2020  self.cw:.       
-0000d4a0: 2020 2020 2073 656c 662e 6377 2e73 656e       self.cw.sen
-0000d4b0: 6463 7728 7365 6c66 2e70 726f 6365 7373  dcw(self.process
-0000d4c0: 5f6d 6163 726f 2873 656c 662e 4631 312e  _macro(self.F11.
-0000d4d0: 746f 6f6c 5469 7028 2929 290a 0a20 2020  toolTip()))..   
-0000d4e0: 2064 6566 2073 656e 6466 3132 2873 656c   def sendf12(sel
-0000d4f0: 6629 3a0a 2020 2020 2020 2020 2222 2273  f):.        """s
-0000d500: 7475 6222 2222 0a20 2020 2020 2020 206c  tub""".        l
-0000d510: 6f67 6765 722e 6465 6275 6728 2246 3132  ogger.debug("F12
-0000d520: 2043 6c69 636b 6564 2229 0a20 2020 2020   Clicked").     
-0000d530: 2020 2069 6620 7365 6c66 2e72 6164 696f     if self.radio
-0000d540: 5f73 7461 7465 2e67 6574 2822 6d6f 6465  _state.get("mode
-0000d550: 2229 2069 6e20 5b22 4c53 4222 2c20 2255  ") in ["LSB", "U
-0000d560: 5342 222c 2022 5353 4222 5d3a 0a20 2020  SB", "SSB"]:.   
-0000d570: 2020 2020 2020 2020 2073 656c 662e 766f           self.vo
-0000d580: 6963 655f 7374 7269 6e67 2873 656c 662e  ice_string(self.
-0000d590: 7072 6f63 6573 735f 6d61 6372 6f28 7365  process_macro(se
-0000d5a0: 6c66 2e46 3132 2e74 6f6f 6c54 6970 2829  lf.F12.toolTip()
-0000d5b0: 2929 0a20 2020 2020 2020 2020 2020 2072  )).            r
-0000d5c0: 6574 7572 6e0a 2020 2020 2020 2020 6966  eturn.        if
-0000d5d0: 2073 656c 662e 6377 3a0a 2020 2020 2020   self.cw:.      
-0000d5e0: 2020 2020 2020 7365 6c66 2e63 772e 7365        self.cw.se
-0000d5f0: 6e64 6377 2873 656c 662e 7072 6f63 6573  ndcw(self.proces
-0000d600: 735f 6d61 6372 6f28 7365 6c66 2e46 3132  s_macro(self.F12
-0000d610: 2e74 6f6f 6c54 6970 2829 2929 0a0a 2020  .toolTip()))..  
-0000d620: 2020 6465 6620 7275 6e5f 7370 5f62 7574    def run_sp_but
-0000d630: 746f 6e73 5f63 6c69 636b 6564 2873 656c  tons_clicked(sel
-0000d640: 6629 3a0a 2020 2020 2020 2020 2222 2248  f):.        """H
-0000d650: 616e 646c 6520 7275 6e2f 7326 7020 6d6f  andle run/s&p mo
-0000d660: 6465 2222 220a 2020 2020 2020 2020 7365  de""".        se
-0000d670: 6c66 2e70 7265 665b 2272 756e 5f73 7461  lf.pref["run_sta
-0000d680: 7465 225d 203d 2073 656c 662e 7261 6469  te"] = self.radi
-0000d690: 6f42 7574 746f 6e5f 7275 6e2e 6973 4368  oButton_run.isCh
-0000d6a0: 6563 6b65 6428 290a 2020 2020 2020 2020  ecked().        
-0000d6b0: 7365 6c66 2e77 7269 7465 5f70 7265 6665  self.write_prefe
-0000d6c0: 7265 6e63 6528 290a 2020 2020 2020 2020  rence().        
-0000d6d0: 7365 6c66 2e72 6561 645f 6377 5f6d 6163  self.read_cw_mac
-0000d6e0: 726f 7328 290a 0a20 2020 2064 6566 2077  ros()..    def w
-0000d6f0: 7269 7465 5f70 7265 6665 7265 6e63 6528  rite_preference(
-0000d700: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-0000d710: 2222 0a20 2020 2020 2020 2057 7269 7465  "".        Write
-0000d720: 2070 7265 6665 7265 6e63 6573 2074 6f20   preferences to 
-0000d730: 6a73 6f6e 2066 696c 652e 0a20 2020 2020  json file..     
-0000d740: 2020 2022 2222 0a20 2020 2020 2020 2074     """.        t
-0000d750: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-0000d760: 7769 7468 206f 7065 6e28 0a20 2020 2020  with open(.     
-0000d770: 2020 2020 2020 2020 2020 2043 4f4e 4649             CONFI
-0000d780: 475f 5041 5448 202b 2022 2f6e 6f74 316d  G_PATH + "/not1m
-0000d790: 6d2e 6a73 6f6e 222c 2022 7774 222c 2065  m.json", "wt", e
-0000d7a0: 6e63 6f64 696e 673d 2275 7466 2d38 220a  ncoding="utf-8".
-0000d7b0: 2020 2020 2020 2020 2020 2020 2920 6173              ) as
-0000d7c0: 2066 696c 655f 6465 7363 7269 7074 6f72   file_descriptor
-0000d7d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000d7e0: 2020 6669 6c65 5f64 6573 6372 6970 746f    file_descripto
-0000d7f0: 722e 7772 6974 6528 6475 6d70 7328 7365  r.write(dumps(se
-0000d800: 6c66 2e70 7265 662c 2069 6e64 656e 743d  lf.pref, indent=
-0000d810: 3429 290a 2020 2020 2020 2020 2020 2020  4)).            
-0000d820: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
-0000d830: 2277 7269 7469 6e67 3a20 2573 222c 2073  "writing: %s", s
-0000d840: 656c 662e 7072 6566 290a 2020 2020 2020  elf.pref).      
-0000d850: 2020 6578 6365 7074 2049 4f45 7272 6f72    except IOError
-0000d860: 2061 7320 6578 6365 7074 696f 6e3a 0a20   as exception:. 
-0000d870: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-0000d880: 722e 6372 6974 6963 616c 2822 7772 6974  r.critical("writ
-0000d890: 6570 7265 6665 7265 6e63 6573 3a20 2573  epreferences: %s
-0000d8a0: 222c 2065 7863 6570 7469 6f6e 290a 0a20  ", exception).. 
-0000d8b0: 2020 2064 6566 2072 6561 6470 7265 6665     def readprefe
-0000d8c0: 7265 6e63 6573 2873 656c 6629 3a0a 2020  rences(self):.  
-0000d8d0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000d8e0: 2020 5265 7374 6f72 6520 7072 6566 6572    Restore prefer
-0000d8f0: 656e 6365 7320 6966 2074 6865 7920 6578  ences if they ex
-0000d900: 6973 742c 206f 7468 6572 7769 7365 2063  ist, otherwise c
-0000d910: 7265 6174 6520 736f 6d65 2073 616e 6520  reate some sane 
-0000d920: 6465 6661 756c 7473 2e0a 2020 2020 2020  defaults..      
-0000d930: 2020 2222 220a 2020 2020 2020 2020 7472    """.        tr
-0000d940: 793a 0a20 2020 2020 2020 2020 2020 2069  y:.            i
-0000d950: 6620 6f73 2e70 6174 682e 6578 6973 7473  f os.path.exists
-0000d960: 2843 4f4e 4649 475f 5041 5448 202b 2022  (CONFIG_PATH + "
-0000d970: 2f6e 6f74 316d 6d2e 6a73 6f6e 2229 3a0a  /not1mm.json"):.
-0000d980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d990: 7769 7468 206f 7065 6e28 0a20 2020 2020  with open(.     
-0000d9a0: 2020 2020 2020 2020 2020 2020 2020 2043                 C
-0000d9b0: 4f4e 4649 475f 5041 5448 202b 2022 2f6e  ONFIG_PATH + "/n
-0000d9c0: 6f74 316d 6d2e 6a73 6f6e 222c 2022 7274  ot1mm.json", "rt
-0000d9d0: 222c 2065 6e63 6f64 696e 673d 2275 7466  ", encoding="utf
-0000d9e0: 2d38 220a 2020 2020 2020 2020 2020 2020  -8".            
-0000d9f0: 2020 2020 2920 6173 2066 696c 655f 6465      ) as file_de
-0000da00: 7363 7269 7074 6f72 3a0a 2020 2020 2020  scriptor:.      
-0000da10: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000da20: 6c66 2e70 7265 6620 3d20 6c6f 6164 7328  lf.pref = loads(
-0000da30: 6669 6c65 5f64 6573 6372 6970 746f 722e  file_descriptor.
-0000da40: 7265 6164 2829 290a 2020 2020 2020 2020  read()).        
-0000da50: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-0000da60: 6572 2e69 6e66 6f28 2225 7322 2c20 7365  er.info("%s", se
-0000da70: 6c66 2e70 7265 6629 0a20 2020 2020 2020  lf.pref).       
-0000da80: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000da90: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-0000daa0: 722e 696e 666f 2822 4e6f 2070 7265 6665  r.info("No prefe
-0000dab0: 7265 6e63 6520 6669 6c65 2e20 5772 6974  rence file. Writ
-0000dac0: 696e 6720 7072 6566 6572 656e 6365 2e22  ing preference."
-0000dad0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000dae0: 2020 7769 7468 206f 7065 6e28 0a20 2020    with open(.   
+000032d0: 6f67 2e6f 7065 6e28 290a 0a20 2020 2064  og.open()..    d
+000032e0: 6566 2065 6469 745f 636f 6e66 6967 7572  ef edit_configur
+000032f0: 6174 696f 6e5f 7365 7474 696e 6773 2873  ation_settings(s
+00003300: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+00003310: 2243 6f6e 6669 6775 7261 7469 6f6e 2053  "Configuration S
+00003320: 6574 7469 6e67 7320 7761 7320 636c 6963  ettings was clic
+00003330: 6b65 6422 2222 0a20 2020 2020 2020 2073  ked""".        s
+00003340: 656c 662e 636f 6e66 6967 7572 6174 696f  elf.configuratio
+00003350: 6e5f 6469 616c 6f67 203d 2053 6574 7469  n_dialog = Setti
+00003360: 6e67 7328 574f 524b 494e 475f 5041 5448  ngs(WORKING_PATH
+00003370: 2c20 434f 4e46 4947 5f50 4154 482c 2073  , CONFIG_PATH, s
+00003380: 656c 662e 7072 6566 290a 2020 2020 2020  elf.pref).      
+00003390: 2020 7365 6c66 2e63 6f6e 6669 6775 7261    self.configura
+000033a0: 7469 6f6e 5f64 6961 6c6f 672e 7573 6568  tion_dialog.useh
+000033b0: 616d 6462 5f72 6164 696f 4275 7474 6f6e  amdb_radioButton
+000033c0: 2e68 6964 6528 290a 2020 2020 2020 2020  .hide().        
+000033d0: 7365 6c66 2e63 6f6e 6669 6775 7261 7469  self.configurati
+000033e0: 6f6e 5f64 6961 6c6f 672e 7368 6f77 2829  on_dialog.show()
+000033f0: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
+00003400: 6e66 6967 7572 6174 696f 6e5f 6469 616c  nfiguration_dial
+00003410: 6f67 2e61 6363 6570 7465 642e 636f 6e6e  og.accepted.conn
+00003420: 6563 7428 7365 6c66 2e65 6469 745f 636f  ect(self.edit_co
+00003430: 6e66 6967 7572 6174 696f 6e5f 7265 7475  nfiguration_retu
+00003440: 726e 290a 0a20 2020 2064 6566 2065 6469  rn)..    def edi
+00003450: 745f 636f 6e66 6967 7572 6174 696f 6e5f  t_configuration_
+00003460: 7265 7475 726e 2873 656c 6629 3a0a 2020  return(self):.  
+00003470: 2020 2020 2020 2222 2252 6574 7572 6e73        """Returns
+00003480: 2068 6572 6520 7768 656e 2063 6f6e 6669   here when confi
+00003490: 6775 7261 7469 6f6e 2064 6961 6c6f 6720  guration dialog 
+000034a0: 636c 6f73 6564 2077 6974 6820 6f6b 6179  closed with okay
+000034b0: 2e22 2222 0a20 2020 2020 2020 2073 656c  .""".        sel
+000034c0: 662e 636f 6e66 6967 7572 6174 696f 6e5f  f.configuration_
+000034d0: 6469 616c 6f67 2e73 6176 655f 6368 616e  dialog.save_chan
+000034e0: 6765 7328 290a 2020 2020 2020 2020 7365  ges().        se
+000034f0: 6c66 2e77 7269 7465 5f70 7265 6665 7265  lf.write_prefere
+00003500: 6e63 6528 290a 2020 2020 2020 2020 6c6f  nce().        lo
+00003510: 6767 6572 2e64 6562 7567 2822 2573 222c  gger.debug("%s",
+00003520: 2066 227b 7365 6c66 2e70 7265 667d 2229   f"{self.pref}")
+00003530: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+00003540: 6164 7072 6566 6572 656e 6365 7328 290a  adpreferences().
+00003550: 0a20 2020 2064 6566 206e 6577 5f64 6174  .    def new_dat
+00003560: 6162 6173 6528 7365 6c66 293a 0a20 2020  abase(self):.   
+00003570: 2020 2020 2022 2222 4372 6561 7465 206e       """Create n
+00003580: 6577 2064 6174 6162 6173 652e 2222 220a  ew database.""".
+00003590: 2020 2020 2020 2020 6669 6c65 6e61 6d65          filename
+000035a0: 203d 2073 656c 662e 6669 6c65 7069 636b   = self.filepick
+000035b0: 6572 2822 6e65 7722 290a 2020 2020 2020  er("new").      
+000035c0: 2020 6966 2066 696c 656e 616d 653a 0a20    if filename:. 
+000035d0: 2020 2020 2020 2020 2020 2069 6620 6669             if fi
+000035e0: 6c65 6e61 6d65 5b2d 333a 5d20 213d 2022  lename[-3:] != "
+000035f0: 2e64 6222 3a0a 2020 2020 2020 2020 2020  .db":.          
+00003600: 2020 2020 2020 6669 6c65 6e61 6d65 202b        filename +
+00003610: 3d20 222e 6462 220a 2020 2020 2020 2020  = ".db".        
+00003620: 2020 2020 7365 6c66 2e70 7265 665b 2263      self.pref["c
+00003630: 7572 7265 6e74 5f64 6174 6162 6173 6522  urrent_database"
+00003640: 5d20 3d20 6669 6c65 6e61 6d65 2e73 706c  ] = filename.spl
+00003650: 6974 2822 2f22 295b 2d31 3a5d 5b30 5d0a  it("/")[-1:][0].
+00003660: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00003670: 2e77 7269 7465 5f70 7265 6665 7265 6e63  .write_preferenc
+00003680: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+00003690: 7365 6c66 2e64 626e 616d 6520 3d20 4441  self.dbname = DA
+000036a0: 5441 5f50 4154 4820 2b20 222f 2220 2b20  TA_PATH + "/" + 
+000036b0: 7365 6c66 2e70 7265 662e 6765 7428 2263  self.pref.get("c
+000036c0: 7572 7265 6e74 5f64 6174 6162 6173 6522  urrent_database"
+000036d0: 2c20 2268 616d 2e64 6222 290a 2020 2020  , "ham.db").    
+000036e0: 2020 2020 2020 2020 7365 6c66 2e64 6174          self.dat
+000036f0: 6162 6173 6520 3d20 4461 7461 4261 7365  abase = DataBase
+00003700: 2873 656c 662e 6462 6e61 6d65 2c20 574f  (self.dbname, WO
+00003710: 524b 494e 475f 5041 5448 290a 2020 2020  RKING_PATH).    
+00003720: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+00003730: 7461 6374 203d 2073 656c 662e 6461 7461  tact = self.data
+00003740: 6261 7365 2e65 6d70 7479 5f63 6f6e 7461  base.empty_conta
+00003750: 6374 0a20 2020 2020 2020 2020 2020 2073  ct.            s
+00003760: 656c 662e 7374 6174 696f 6e20 3d20 7365  elf.station = se
+00003770: 6c66 2e64 6174 6162 6173 652e 6665 7463  lf.database.fetc
+00003780: 685f 7374 6174 696f 6e28 290a 2020 2020  h_station().    
+00003790: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000037a0: 7374 6174 696f 6e20 6973 204e 6f6e 653a  station is None:
+000037b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000037c0: 2073 656c 662e 7374 6174 696f 6e20 3d20   self.station = 
+000037d0: 7b7d 0a20 2020 2020 2020 2020 2020 2073  {}.            s
+000037e0: 656c 662e 6375 7272 656e 745f 6f70 203d  elf.current_op =
+000037f0: 2073 656c 662e 7374 6174 696f 6e2e 6765   self.station.ge
+00003800: 7428 2243 616c 6c22 2c20 2222 290a 2020  t("Call", "").  
+00003810: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00003820: 616b 655f 6f70 5f64 6972 2829 0a20 2020  ake_op_dir().   
+00003830: 2020 2020 2020 2020 2063 6d64 203d 207b           cmd = {
+00003840: 7d0a 2020 2020 2020 2020 2020 2020 636d  }.            cm
+00003850: 645b 2263 6d64 225d 203d 2022 4e45 5744  d["cmd"] = "NEWD
+00003860: 4222 0a20 2020 2020 2020 2020 2020 2063  B".            c
+00003870: 6d64 5b22 7374 6174 696f 6e22 5d20 3d20  md["station"] = 
+00003880: 706c 6174 666f 726d 2e6e 6f64 6528 290a  platform.node().
+00003890: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000038a0: 2e6d 756c 7469 6361 7374 5f69 6e74 6572  .multicast_inter
+000038b0: 6661 6365 2e73 656e 645f 6173 5f6a 736f  face.send_as_jso
+000038c0: 6e28 636d 6429 0a20 2020 2020 2020 2020  n(cmd).         
+000038d0: 2020 2073 656c 662e 636c 6561 7269 6e70     self.clearinp
+000038e0: 7574 7328 290a 2020 2020 2020 2020 2020  uts().          
+000038f0: 2020 7365 6c66 2e65 6469 745f 7374 6174    self.edit_stat
+00003900: 696f 6e5f 7365 7474 696e 6773 2829 0a0a  ion_settings()..
+00003910: 2020 2020 6465 6620 6f70 656e 5f64 6174      def open_dat
+00003920: 6162 6173 6528 7365 6c66 293a 0a20 2020  abase(self):.   
+00003930: 2020 2020 2022 2222 4f70 656e 2065 7869       """Open exi
+00003940: 7374 696e 6720 6461 7461 6261 7365 2e22  sting database."
+00003950: 2222 0a20 2020 2020 2020 2066 696c 656e  "".        filen
+00003960: 616d 6520 3d20 7365 6c66 2e66 696c 6570  ame = self.filep
+00003970: 6963 6b65 7228 226f 7065 6e22 290a 2020  icker("open").  
+00003980: 2020 2020 2020 6966 2066 696c 656e 616d        if filenam
+00003990: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+000039a0: 656c 662e 7072 6566 5b22 6375 7272 656e  elf.pref["curren
+000039b0: 745f 6461 7461 6261 7365 225d 203d 2066  t_database"] = f
+000039c0: 696c 656e 616d 652e 7370 6c69 7428 222f  ilename.split("/
+000039d0: 2229 5b2d 313a 5d5b 305d 0a20 2020 2020  ")[-1:][0].     
+000039e0: 2020 2020 2020 2073 656c 662e 7772 6974         self.writ
+000039f0: 655f 7072 6566 6572 656e 6365 2829 0a20  e_preference(). 
+00003a00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00003a10: 6462 6e61 6d65 203d 2044 4154 415f 5041  dbname = DATA_PA
+00003a20: 5448 202b 2022 2f22 202b 2073 656c 662e  TH + "/" + self.
+00003a30: 7072 6566 2e67 6574 2822 6375 7272 656e  pref.get("curren
+00003a40: 745f 6461 7461 6261 7365 222c 2022 6861  t_database", "ha
+00003a50: 6d2e 6462 2229 0a20 2020 2020 2020 2020  m.db").         
+00003a60: 2020 2073 656c 662e 6461 7461 6261 7365     self.database
+00003a70: 203d 2044 6174 6142 6173 6528 7365 6c66   = DataBase(self
+00003a80: 2e64 626e 616d 652c 2057 4f52 4b49 4e47  .dbname, WORKING
+00003a90: 5f50 4154 4829 0a20 2020 2020 2020 2020  _PATH).         
+00003aa0: 2020 2073 656c 662e 636f 6e74 6163 7420     self.contact 
+00003ab0: 3d20 7365 6c66 2e64 6174 6162 6173 652e  = self.database.
+00003ac0: 656d 7074 795f 636f 6e74 6163 740a 2020  empty_contact.  
+00003ad0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00003ae0: 7461 7469 6f6e 203d 2073 656c 662e 6461  tation = self.da
+00003af0: 7461 6261 7365 2e66 6574 6368 5f73 7461  tabase.fetch_sta
+00003b00: 7469 6f6e 2829 0a20 2020 2020 2020 2020  tion().         
+00003b10: 2020 2069 6620 7365 6c66 2e73 7461 7469     if self.stati
+00003b20: 6f6e 2069 7320 4e6f 6e65 3a0a 2020 2020  on is None:.    
+00003b30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00003b40: 2e73 7461 7469 6f6e 203d 207b 7d0a 2020  .station = {}.  
+00003b50: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00003b60: 662e 7374 6174 696f 6e2e 6765 7428 2243  f.station.get("C
+00003b70: 616c 6c22 2c20 2222 2920 3d3d 2022 223a  all", "") == "":
+00003b80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003b90: 2073 656c 662e 6564 6974 5f73 7461 7469   self.edit_stati
+00003ba0: 6f6e 5f73 6574 7469 6e67 7328 290a 2020  on_settings().  
+00003bb0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00003bc0: 7572 7265 6e74 5f6f 7020 3d20 7365 6c66  urrent_op = self
+00003bd0: 2e73 7461 7469 6f6e 2e67 6574 2822 4361  .station.get("Ca
+00003be0: 6c6c 222c 2022 2229 0a20 2020 2020 2020  ll", "").       
+00003bf0: 2020 2020 2073 656c 662e 6d61 6b65 5f6f       self.make_o
+00003c00: 705f 6469 7228 290a 2020 2020 2020 2020  p_dir().        
+00003c10: 2020 2020 636d 6420 3d20 7b7d 0a20 2020      cmd = {}.   
+00003c20: 2020 2020 2020 2020 2063 6d64 5b22 636d           cmd["cm
+00003c30: 6422 5d20 3d20 224e 4557 4442 220a 2020  d"] = "NEWDB".  
+00003c40: 2020 2020 2020 2020 2020 636d 645b 2273            cmd["s
+00003c50: 7461 7469 6f6e 225d 203d 2070 6c61 7466  tation"] = platf
+00003c60: 6f72 6d2e 6e6f 6465 2829 0a20 2020 2020  orm.node().     
+00003c70: 2020 2020 2020 2073 656c 662e 6d75 6c74         self.mult
+00003c80: 6963 6173 745f 696e 7465 7266 6163 652e  icast_interface.
+00003c90: 7365 6e64 5f61 735f 6a73 6f6e 2863 6d64  send_as_json(cmd
+00003ca0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00003cb0: 6c66 2e63 6c65 6172 696e 7075 7473 2829  lf.clearinputs()
+00003cc0: 0a0a 2020 2020 6465 6620 6e65 775f 636f  ..    def new_co
+00003cd0: 6e74 6573 7428 7365 6c66 293a 0a20 2020  ntest(self):.   
+00003ce0: 2020 2020 2022 2222 4372 6561 7465 206e       """Create n
+00003cf0: 6577 2063 6f6e 7465 7374 2069 6e20 6578  ew contest in ex
+00003d00: 6973 7469 6e67 2064 6174 6162 6173 652e  isting database.
+00003d10: 2222 220a 0a20 2020 2064 6566 206f 7065  """..    def ope
+00003d20: 6e5f 636f 6e74 6573 7428 7365 6c66 293a  n_contest(self):
+00003d30: 0a20 2020 2020 2020 2022 2222 5377 6974  .        """Swit
+00003d40: 6368 2074 6f20 6120 6469 6666 6572 656e  ch to a differen
+00003d50: 7420 6578 6973 7469 6e67 2063 6f6e 7465  t existing conte
+00003d60: 7374 2069 6e20 6578 6973 7469 6e67 2064  st in existing d
+00003d70: 6174 6162 6173 652e 2222 220a 2020 2020  atabase.""".    
+00003d80: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+00003d90: 2822 4f70 656e 2043 6f6e 7465 7374 2073  ("Open Contest s
+00003da0: 656c 6563 7465 6422 290a 2020 2020 2020  elected").      
+00003db0: 2020 636f 6e74 6573 7473 203d 2073 656c    contests = sel
+00003dc0: 662e 6461 7461 6261 7365 2e66 6574 6368  f.database.fetch
+00003dd0: 5f61 6c6c 5f63 6f6e 7465 7374 7328 290a  _all_contests().
+00003de0: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+00003df0: 6562 7567 2822 2573 222c 2066 227b 636f  ebug("%s", f"{co
+00003e00: 6e74 6573 7473 7d22 290a 0a20 2020 2020  ntests}")..     
+00003e10: 2020 2069 6620 636f 6e74 6573 7473 3a0a     if contests:.
+00003e20: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00003e30: 2e63 6f6e 7465 7374 5f64 6961 6c6f 6720  .contest_dialog 
+00003e40: 3d20 5365 6c65 6374 436f 6e74 6573 7428  = SelectContest(
+00003e50: 574f 524b 494e 475f 5041 5448 290a 2020  WORKING_PATH).  
+00003e60: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00003e70: 6f6e 7465 7374 5f64 6961 6c6f 672e 636f  ontest_dialog.co
+00003e80: 6e74 6573 745f 6c69 7374 2e73 6574 526f  ntest_list.setRo
+00003e90: 7743 6f75 6e74 2830 290a 2020 2020 2020  wCount(0).      
+00003ea0: 2020 2020 2020 7365 6c66 2e63 6f6e 7465        self.conte
+00003eb0: 7374 5f64 6961 6c6f 672e 636f 6e74 6573  st_dialog.contes
+00003ec0: 745f 6c69 7374 2e73 6574 436f 6c75 6d6e  t_list.setColumn
+00003ed0: 436f 756e 7428 3429 0a20 2020 2020 2020  Count(4).       
+00003ee0: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
+00003ef0: 745f 6469 616c 6f67 2e63 6f6e 7465 7374  t_dialog.contest
+00003f00: 5f6c 6973 742e 7665 7274 6963 616c 4865  _list.verticalHe
+00003f10: 6164 6572 2829 2e73 6574 5669 7369 626c  ader().setVisibl
+00003f20: 6528 4661 6c73 6529 0a20 2020 2020 2020  e(False).       
+00003f30: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
+00003f40: 745f 6469 616c 6f67 2e63 6f6e 7465 7374  t_dialog.contest
+00003f50: 5f6c 6973 742e 7365 7443 6f6c 756d 6e57  _list.setColumnW
+00003f60: 6964 7468 2831 2c20 3230 3029 0a20 2020  idth(1, 200).   
+00003f70: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+00003f80: 6e74 6573 745f 6469 616c 6f67 2e63 6f6e  ntest_dialog.con
+00003f90: 7465 7374 5f6c 6973 742e 7365 7443 6f6c  test_list.setCol
+00003fa0: 756d 6e57 6964 7468 2832 2c20 3230 3029  umnWidth(2, 200)
+00003fb0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00003fc0: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
+00003fd0: 2e63 6f6e 7465 7374 5f6c 6973 742e 7365  .contest_list.se
+00003fe0: 7448 6f72 697a 6f6e 7461 6c48 6561 6465  tHorizontalHeade
+00003ff0: 7249 7465 6d28 0a20 2020 2020 2020 2020  rItem(.         
+00004000: 2020 2020 2020 2030 2c20 5174 5769 6467         0, QtWidg
+00004010: 6574 732e 5154 6162 6c65 5769 6467 6574  ets.QTableWidget
+00004020: 4974 656d 2822 436f 6e74 6573 7420 4e72  Item("Contest Nr
+00004030: 2229 0a20 2020 2020 2020 2020 2020 2029  ").            )
+00004040: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00004050: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
+00004060: 2e63 6f6e 7465 7374 5f6c 6973 742e 7365  .contest_list.se
+00004070: 7448 6f72 697a 6f6e 7461 6c48 6561 6465  tHorizontalHeade
+00004080: 7249 7465 6d28 0a20 2020 2020 2020 2020  rItem(.         
+00004090: 2020 2020 2020 2031 2c20 5174 5769 6467         1, QtWidg
+000040a0: 6574 732e 5154 6162 6c65 5769 6467 6574  ets.QTableWidget
+000040b0: 4974 656d 2822 436f 6e74 6573 7420 4e61  Item("Contest Na
+000040c0: 6d65 2229 0a20 2020 2020 2020 2020 2020  me").           
+000040d0: 2029 0a20 2020 2020 2020 2020 2020 2073   ).            s
+000040e0: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
+000040f0: 6f67 2e63 6f6e 7465 7374 5f6c 6973 742e  og.contest_list.
+00004100: 7365 7448 6f72 697a 6f6e 7461 6c48 6561  setHorizontalHea
+00004110: 6465 7249 7465 6d28 0a20 2020 2020 2020  derItem(.       
+00004120: 2020 2020 2020 2020 2032 2c20 5174 5769           2, QtWi
+00004130: 6467 6574 732e 5154 6162 6c65 5769 6467  dgets.QTableWidg
+00004140: 6574 4974 656d 2822 436f 6e74 6573 7420  etItem("Contest 
+00004150: 5374 6172 7422 290a 2020 2020 2020 2020  Start").        
+00004160: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00004170: 2020 7365 6c66 2e63 6f6e 7465 7374 5f64    self.contest_d
+00004180: 6961 6c6f 672e 636f 6e74 6573 745f 6c69  ialog.contest_li
+00004190: 7374 2e73 6574 486f 7269 7a6f 6e74 616c  st.setHorizontal
+000041a0: 4865 6164 6572 4974 656d 280a 2020 2020  HeaderItem(.    
+000041b0: 2020 2020 2020 2020 2020 2020 332c 2051              3, Q
+000041c0: 7457 6964 6765 7473 2e51 5461 626c 6557  tWidgets.QTableW
+000041d0: 6964 6765 7449 7465 6d28 224e 6f74 2055  idgetItem("Not U
+000041e0: 4973 6564 2229 0a20 2020 2020 2020 2020  Ised").         
+000041f0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00004200: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
+00004210: 616c 6f67 2e63 6f6e 7465 7374 5f6c 6973  alog.contest_lis
+00004220: 742e 7365 7443 6f6c 756d 6e48 6964 6465  t.setColumnHidde
+00004230: 6e28 302c 2054 7275 6529 0a20 2020 2020  n(0, True).     
+00004240: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
+00004250: 6573 745f 6469 616c 6f67 2e63 6f6e 7465  est_dialog.conte
+00004260: 7374 5f6c 6973 742e 7365 7443 6f6c 756d  st_list.setColum
+00004270: 6e48 6964 6465 6e28 332c 2054 7275 6529  nHidden(3, True)
+00004280: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00004290: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
+000042a0: 2e61 6363 6570 7465 642e 636f 6e6e 6563  .accepted.connec
+000042b0: 7428 7365 6c66 2e6f 7065 6e5f 636f 6e74  t(self.open_cont
+000042c0: 6573 745f 7265 7475 726e 290a 2020 2020  est_return).    
+000042d0: 2020 2020 2020 2020 666f 7220 636f 6e74          for cont
+000042e0: 6573 7420 696e 2063 6f6e 7465 7374 733a  est in contests:
+000042f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004300: 206e 756d 6265 725f 6f66 5f72 6f77 7320   number_of_rows 
+00004310: 3d20 7365 6c66 2e63 6f6e 7465 7374 5f64  = self.contest_d
+00004320: 6961 6c6f 672e 636f 6e74 6573 745f 6c69  ialog.contest_li
+00004330: 7374 2e72 6f77 436f 756e 7428 290a 2020  st.rowCount().  
+00004340: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00004350: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
+00004360: 672e 636f 6e74 6573 745f 6c69 7374 2e69  g.contest_list.i
+00004370: 6e73 6572 7452 6f77 286e 756d 6265 725f  nsertRow(number_
+00004380: 6f66 5f72 6f77 7329 0a20 2020 2020 2020  of_rows).       
+00004390: 2020 2020 2020 2020 2063 6f6e 7465 7374           contest
+000043a0: 5f69 6420 3d20 7374 7228 636f 6e74 6573  _id = str(contes
+000043b0: 742e 6765 7428 2243 6f6e 7465 7374 4944  t.get("ContestID
+000043c0: 222c 2031 2929 0a20 2020 2020 2020 2020  ", 1)).         
+000043d0: 2020 2020 2020 2063 6f6e 7465 7374 5f6e         contest_n
+000043e0: 616d 6520 3d20 636f 6e74 6573 742e 6765  ame = contest.ge
+000043f0: 7428 2243 6f6e 7465 7374 4e61 6d65 222c  t("ContestName",
+00004400: 2031 290a 2020 2020 2020 2020 2020 2020   1).            
+00004410: 2020 2020 7374 6172 745f 6461 7465 203d      start_date =
+00004420: 2063 6f6e 7465 7374 2e67 6574 2822 5374   contest.get("St
+00004430: 6172 7444 6174 6522 2c20 3129 0a20 2020  artDate", 1).   
+00004440: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00004450: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
+00004460: 2e63 6f6e 7465 7374 5f6c 6973 742e 7365  .contest_list.se
+00004470: 7449 7465 6d28 0a20 2020 2020 2020 2020  tItem(.         
+00004480: 2020 2020 2020 2020 2020 206e 756d 6265             numbe
+00004490: 725f 6f66 5f72 6f77 732c 2030 2c20 5174  r_of_rows, 0, Qt
+000044a0: 5769 6467 6574 732e 5154 6162 6c65 5769  Widgets.QTableWi
+000044b0: 6467 6574 4974 656d 2863 6f6e 7465 7374  dgetItem(contest
+000044c0: 5f69 6429 0a20 2020 2020 2020 2020 2020  _id).           
+000044d0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+000044e0: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
+000044f0: 6573 745f 6469 616c 6f67 2e63 6f6e 7465  est_dialog.conte
+00004500: 7374 5f6c 6973 742e 7365 7449 7465 6d28  st_list.setItem(
+00004510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004520: 2020 2020 206e 756d 6265 725f 6f66 5f72       number_of_r
+00004530: 6f77 732c 2031 2c20 5174 5769 6467 6574  ows, 1, QtWidget
+00004540: 732e 5154 6162 6c65 5769 6467 6574 4974  s.QTableWidgetIt
+00004550: 656d 2863 6f6e 7465 7374 5f6e 616d 6529  em(contest_name)
+00004560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004570: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+00004580: 2020 2073 656c 662e 636f 6e74 6573 745f     self.contest_
+00004590: 6469 616c 6f67 2e63 6f6e 7465 7374 5f6c  dialog.contest_l
+000045a0: 6973 742e 7365 7449 7465 6d28 0a20 2020  ist.setItem(.   
+000045b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000045c0: 206e 756d 6265 725f 6f66 5f72 6f77 732c   number_of_rows,
+000045d0: 2032 2c20 5174 5769 6467 6574 732e 5154   2, QtWidgets.QT
+000045e0: 6162 6c65 5769 6467 6574 4974 656d 2873  ableWidgetItem(s
+000045f0: 7461 7274 5f64 6174 6529 0a20 2020 2020  tart_date).     
+00004600: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00004610: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
+00004620: 745f 6469 616c 6f67 2e73 686f 7728 290a  t_dialog.show().
+00004630: 0a20 2020 2064 6566 206f 7065 6e5f 636f  .    def open_co
+00004640: 6e74 6573 745f 7265 7475 726e 2873 656c  ntest_return(sel
+00004650: 6629 3a0a 2020 2020 2020 2020 2222 2243  f):.        """C
+00004660: 616c 6c65 6420 6279 206f 7065 6e5f 636f  alled by open_co
+00004670: 6e74 6573 7422 2222 0a20 2020 2020 2020  ntest""".       
+00004680: 2073 656c 6563 7465 645f 726f 7720 3d20   selected_row = 
+00004690: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
+000046a0: 6c6f 672e 636f 6e74 6573 745f 6c69 7374  log.contest_list
+000046b0: 2e63 7572 7265 6e74 526f 7728 290a 2020  .currentRow().  
+000046c0: 2020 2020 2020 636f 6e74 6573 7420 3d20        contest = 
+000046d0: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
+000046e0: 6c6f 672e 636f 6e74 6573 745f 6c69 7374  log.contest_list
+000046f0: 2e69 7465 6d28 7365 6c65 6374 6564 5f72  .item(selected_r
+00004700: 6f77 2c20 3029 2e74 6578 7428 290a 2020  ow, 0).text().  
+00004710: 2020 2020 2020 7365 6c66 2e70 7265 665b        self.pref[
+00004720: 2263 6f6e 7465 7374 225d 203d 2063 6f6e  "contest"] = con
+00004730: 7465 7374 0a20 2020 2020 2020 2073 656c  test.        sel
+00004740: 662e 7772 6974 655f 7072 6566 6572 656e  f.write_preferen
+00004750: 6365 2829 0a20 2020 2020 2020 206c 6f67  ce().        log
+00004760: 6765 722e 6465 6275 6728 2253 656c 6563  ger.debug("Selec
+00004770: 7465 6420 636f 6e74 6573 743a 2025 7322  ted contest: %s"
+00004780: 2c20 6622 7b63 6f6e 7465 7374 7d22 290a  , f"{contest}").
+00004790: 2020 2020 2020 2020 7365 6c66 2e6c 6f61          self.loa
+000047a0: 645f 636f 6e74 6573 7428 290a 0a20 2020  d_contest()..   
+000047b0: 2064 6566 2072 6566 696c 6c5f 6472 6f70   def refill_drop
+000047c0: 646f 776e 2873 656c 662c 2074 6172 6765  down(self, targe
+000047d0: 742c 2073 6f75 7263 6529 3a0a 2020 2020  t, source):.    
+000047e0: 2020 2020 2222 2252 6566 696c 6c20 5143      """Refill QC
+000047f0: 6f6d 626f 626f 7820 7769 6467 6574 2077  ombobox widget w
+00004800: 6974 6820 7661 6c75 652e 2222 220a 2020  ith value.""".  
+00004810: 2020 2020 2020 696e 6465 7820 3d20 7461        index = ta
+00004820: 7267 6574 2e66 696e 6454 6578 7428 736f  rget.findText(so
+00004830: 7572 6365 290a 2020 2020 2020 2020 7461  urce).        ta
+00004840: 7267 6574 2e73 6574 4375 7272 656e 7449  rget.setCurrentI
+00004850: 6e64 6578 2869 6e64 6578 290a 0a20 2020  ndex(index)..   
+00004860: 2064 6566 2065 6469 745f 636f 6e74 6573   def edit_contes
+00004870: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
+00004880: 2022 2222 4564 6974 2074 6865 2063 7572   """Edit the cur
+00004890: 7265 6e74 2063 6f6e 7465 7374 2222 220a  rent contest""".
+000048a0: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+000048b0: 6562 7567 2822 4564 6974 2063 6f6e 7465  ebug("Edit conte
+000048c0: 7374 2044 6961 6c6f 6722 290a 2020 2020  st Dialog").    
+000048d0: 2020 2020 6966 2073 656c 662e 636f 6e74      if self.cont
+000048e0: 6573 745f 7365 7474 696e 6773 2069 7320  est_settings is 
+000048f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00004900: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+00004910: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
+00004920: 616c 6f67 203d 204e 6577 436f 6e74 6573  alog = NewContes
+00004930: 7428 574f 524b 494e 475f 5041 5448 290a  t(WORKING_PATH).
+00004940: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+00004950: 7465 7374 5f64 6961 6c6f 672e 7365 7457  test_dialog.setW
+00004960: 696e 646f 7754 6974 6c65 2822 4564 6974  indowTitle("Edit
+00004970: 2043 6f6e 7465 7374 2229 0a20 2020 2020   Contest").     
+00004980: 2020 2073 656c 662e 636f 6e74 6573 745f     self.contest_
+00004990: 6469 616c 6f67 2e74 6974 6c65 2e73 6574  dialog.title.set
+000049a0: 5465 7874 2822 2229 0a20 2020 2020 2020  Text("").       
+000049b0: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
+000049c0: 616c 6f67 2e61 6363 6570 7465 642e 636f  alog.accepted.co
+000049d0: 6e6e 6563 7428 7365 6c66 2e73 6176 655f  nnect(self.save_
+000049e0: 6564 6974 6564 5f63 6f6e 7465 7374 290a  edited_contest).
+000049f0: 2020 2020 2020 2020 7661 6c75 6520 3d20          value = 
+00004a00: 7365 6c66 2e63 6f6e 7465 7374 5f73 6574  self.contest_set
+00004a10: 7469 6e67 732e 6765 7428 2243 6f6e 7465  tings.get("Conte
+00004a20: 7374 4e61 6d65 2229 2e75 7070 6572 2829  stName").upper()
+00004a30: 2e72 6570 6c61 6365 2822 5f22 2c20 2220  .replace("_", " 
+00004a40: 2229 0a20 2020 2020 2020 2069 6620 7661  ").        if va
+00004a50: 6c75 6520 3d3d 2022 4745 4e45 5241 4c20  lue == "GENERAL 
+00004a60: 4c4f 4747 494e 4722 3a0a 2020 2020 2020  LOGGING":.      
+00004a70: 2020 2020 2020 7661 6c75 6520 3d20 2247        value = "G
+00004a80: 656e 6572 616c 204c 6f67 6769 6e67 220a  eneral Logging".
+00004a90: 2020 2020 2020 2020 7365 6c66 2e72 6566          self.ref
+00004aa0: 696c 6c5f 6472 6f70 646f 776e 2873 656c  ill_dropdown(sel
+00004ab0: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
+00004ac0: 2e63 6f6e 7465 7374 2c20 7661 6c75 6529  .contest, value)
+00004ad0: 0a20 2020 2020 2020 2076 616c 7565 203d  .        value =
+00004ae0: 2073 656c 662e 636f 6e74 6573 745f 7365   self.contest_se
+00004af0: 7474 696e 6773 2e67 6574 2822 4f70 6572  ttings.get("Oper
+00004b00: 6174 6f72 4361 7465 676f 7279 2229 0a20  atorCategory"). 
+00004b10: 2020 2020 2020 2073 656c 662e 7265 6669         self.refi
+00004b20: 6c6c 5f64 726f 7064 6f77 6e28 7365 6c66  ll_dropdown(self
+00004b30: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
+00004b40: 6f70 6572 6174 6f72 5f63 6c61 7373 2c20  operator_class, 
+00004b50: 7661 6c75 6529 0a20 2020 2020 2020 2076  value).        v
+00004b60: 616c 7565 203d 2073 656c 662e 636f 6e74  alue = self.cont
+00004b70: 6573 745f 7365 7474 696e 6773 2e67 6574  est_settings.get
+00004b80: 2822 4261 6e64 4361 7465 676f 7279 2229  ("BandCategory")
+00004b90: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+00004ba0: 6669 6c6c 5f64 726f 7064 6f77 6e28 7365  fill_dropdown(se
+00004bb0: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
+00004bc0: 672e 6261 6e64 2c20 7661 6c75 6529 0a20  g.band, value). 
+00004bd0: 2020 2020 2020 2076 616c 7565 203d 2073         value = s
+00004be0: 656c 662e 636f 6e74 6573 745f 7365 7474  elf.contest_sett
+00004bf0: 696e 6773 2e67 6574 2822 506f 7765 7243  ings.get("PowerC
+00004c00: 6174 6567 6f72 7922 290a 2020 2020 2020  ategory").      
+00004c10: 2020 7365 6c66 2e72 6566 696c 6c5f 6472    self.refill_dr
+00004c20: 6f70 646f 776e 2873 656c 662e 636f 6e74  opdown(self.cont
+00004c30: 6573 745f 6469 616c 6f67 2e70 6f77 6572  est_dialog.power
+00004c40: 2c20 7661 6c75 6529 0a20 2020 2020 2020  , value).       
+00004c50: 2076 616c 7565 203d 2073 656c 662e 636f   value = self.co
+00004c60: 6e74 6573 745f 7365 7474 696e 6773 2e67  ntest_settings.g
+00004c70: 6574 2822 4d6f 6465 4361 7465 676f 7279  et("ModeCategory
+00004c80: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+00004c90: 7265 6669 6c6c 5f64 726f 7064 6f77 6e28  refill_dropdown(
+00004ca0: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
+00004cb0: 6c6f 672e 6d6f 6465 2c20 7661 6c75 6529  log.mode, value)
+00004cc0: 0a20 2020 2020 2020 2076 616c 7565 203d  .        value =
+00004cd0: 2073 656c 662e 636f 6e74 6573 745f 7365   self.contest_se
+00004ce0: 7474 696e 6773 2e67 6574 2822 4f76 6572  ttings.get("Over
+00004cf0: 6c61 7943 6174 6567 6f72 7922 290a 2020  layCategory").  
+00004d00: 2020 2020 2020 7365 6c66 2e72 6566 696c        self.refil
+00004d10: 6c5f 6472 6f70 646f 776e 2873 656c 662e  l_dropdown(self.
+00004d20: 636f 6e74 6573 745f 6469 616c 6f67 2e6f  contest_dialog.o
+00004d30: 7665 726c 6179 2c20 7661 6c75 6529 0a20  verlay, value). 
+00004d40: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
+00004d50: 6573 745f 6469 616c 6f67 2e6f 7065 7261  est_dialog.opera
+00004d60: 746f 7273 2e73 6574 5465 7874 2873 656c  tors.setText(sel
+00004d70: 662e 636f 6e74 6573 745f 7365 7474 696e  f.contest_settin
+00004d80: 6773 2e67 6574 2822 4f70 6572 6174 6f72  gs.get("Operator
+00004d90: 7322 2929 0a20 2020 2020 2020 2073 656c  s")).        sel
+00004da0: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
+00004db0: 2e73 6f61 7062 6f78 2e73 6574 506c 6169  .soapbox.setPlai
+00004dc0: 6e54 6578 7428 7365 6c66 2e63 6f6e 7465  nText(self.conte
+00004dd0: 7374 5f73 6574 7469 6e67 732e 6765 7428  st_settings.get(
+00004de0: 2253 6f61 7062 6f78 2229 290a 2020 2020  "Soapbox")).    
+00004df0: 2020 2020 7365 6c66 2e63 6f6e 7465 7374      self.contest
+00004e00: 5f64 6961 6c6f 672e 6578 6368 616e 6765  _dialog.exchange
+00004e10: 2e73 6574 5465 7874 2873 656c 662e 636f  .setText(self.co
+00004e20: 6e74 6573 745f 7365 7474 696e 6773 2e67  ntest_settings.g
+00004e30: 6574 2822 5365 6e74 4578 6368 616e 6765  et("SentExchange
+00004e40: 2229 290a 2020 2020 2020 2020 7661 6c75  ")).        valu
+00004e50: 6520 3d20 7365 6c66 2e63 6f6e 7465 7374  e = self.contest
+00004e60: 5f73 6574 7469 6e67 732e 6765 7428 2253  _settings.get("S
+00004e70: 7461 7469 6f6e 4361 7465 676f 7279 2229  tationCategory")
+00004e80: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+00004e90: 6669 6c6c 5f64 726f 7064 6f77 6e28 7365  fill_dropdown(se
+00004ea0: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
+00004eb0: 672e 7374 6174 696f 6e2c 2076 616c 7565  g.station, value
+00004ec0: 290a 2020 2020 2020 2020 7661 6c75 6520  ).        value 
+00004ed0: 3d20 7365 6c66 2e63 6f6e 7465 7374 5f73  = self.contest_s
+00004ee0: 6574 7469 6e67 732e 6765 7428 2241 7373  ettings.get("Ass
+00004ef0: 6973 7465 6443 6174 6567 6f72 7922 290a  istedCategory").
+00004f00: 2020 2020 2020 2020 7365 6c66 2e72 6566          self.ref
+00004f10: 696c 6c5f 6472 6f70 646f 776e 2873 656c  ill_dropdown(sel
+00004f20: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
+00004f30: 2e61 7373 6973 7465 642c 2076 616c 7565  .assisted, value
+00004f40: 290a 2020 2020 2020 2020 7661 6c75 6520  ).        value 
+00004f50: 3d20 7365 6c66 2e63 6f6e 7465 7374 5f73  = self.contest_s
+00004f60: 6574 7469 6e67 732e 6765 7428 2254 7261  ettings.get("Tra
+00004f70: 6e73 6d69 7474 6572 4361 7465 676f 7279  nsmitterCategory
+00004f80: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+00004f90: 7265 6669 6c6c 5f64 726f 7064 6f77 6e28  refill_dropdown(
+00004fa0: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
+00004fb0: 6c6f 672e 7472 616e 736d 6974 7465 722c  log.transmitter,
+00004fc0: 2076 616c 7565 290a 2020 2020 2020 2020   value).        
+00004fd0: 7661 6c75 6520 3d20 7365 6c66 2e63 6f6e  value = self.con
+00004fe0: 7465 7374 5f73 6574 7469 6e67 732e 6765  test_settings.ge
+00004ff0: 7428 2253 7461 7274 4461 7465 2229 0a20  t("StartDate"). 
+00005000: 2020 2020 2020 2074 6865 5f64 6174 652c         the_date,
+00005010: 2074 6865 5f74 696d 6520 3d20 7661 6c75   the_time = valu
+00005020: 652e 7370 6c69 7428 290a 2020 2020 2020  e.split().      
+00005030: 2020 7365 6c66 2e63 6f6e 7465 7374 5f64    self.contest_d
+00005040: 6961 6c6f 672e 6461 7465 5469 6d65 4564  ialog.dateTimeEd
+00005050: 6974 2e73 6574 4461 7465 280a 2020 2020  it.setDate(.    
+00005060: 2020 2020 2020 2020 5174 436f 7265 2e51          QtCore.Q
+00005070: 4461 7465 2e66 726f 6d53 7472 696e 6728  Date.fromString(
+00005080: 7468 655f 6461 7465 2c20 2279 7979 792d  the_date, "yyyy-
+00005090: 4d4d 2d64 6422 290a 2020 2020 2020 2020  MM-dd").        
+000050a0: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
+000050b0: 6f6e 7465 7374 5f64 6961 6c6f 672e 6461  ontest_dialog.da
+000050c0: 7465 5469 6d65 4564 6974 2e73 6574 4361  teTimeEdit.setCa
+000050d0: 6c65 6e64 6172 506f 7075 7028 5472 7565  lendarPopup(True
+000050e0: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
+000050f0: 6f6e 7465 7374 5f64 6961 6c6f 672e 6461  ontest_dialog.da
+00005100: 7465 5469 6d65 4564 6974 2e73 6574 5469  teTimeEdit.setTi
+00005110: 6d65 280a 2020 2020 2020 2020 2020 2020  me(.            
+00005120: 5174 436f 7265 2e51 5469 6d65 2e66 726f  QtCore.QTime.fro
+00005130: 6d53 7472 696e 6728 7468 655f 7469 6d65  mString(the_time
+00005140: 2c20 2268 683a 6d6d 3a73 7322 290a 2020  , "hh:mm:ss").  
+00005150: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00005160: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
+00005170: 6c6f 672e 6f70 656e 2829 0a0a 2020 2020  log.open()..    
+00005180: 6465 6620 7361 7665 5f65 6469 7465 645f  def save_edited_
+00005190: 636f 6e74 6573 7428 7365 6c66 293a 0a20  contest(self):. 
+000051a0: 2020 2020 2020 2022 2222 5361 7665 2074         """Save t
+000051b0: 6865 2065 6469 7465 6420 636f 6e74 6573  he edited contes
+000051c0: 7422 2222 0a20 2020 2020 2020 2063 6f6e  t""".        con
+000051d0: 7465 7374 203d 207b 7d0a 2020 2020 2020  test = {}.      
+000051e0: 2020 636f 6e74 6573 745b 2243 6f6e 7465    contest["Conte
+000051f0: 7374 4e61 6d65 225d 203d 2028 0a20 2020  stName"] = (.   
+00005200: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+00005210: 6e74 6573 745f 6469 616c 6f67 2e63 6f6e  ntest_dialog.con
+00005220: 7465 7374 2e63 7572 7265 6e74 5465 7874  test.currentText
+00005230: 2829 2e6c 6f77 6572 2829 2e72 6570 6c61  ().lower().repla
+00005240: 6365 2822 2022 2c20 225f 2229 0a20 2020  ce(" ", "_").   
+00005250: 2020 2020 2029 0a20 2020 2020 2020 2063       ).        c
+00005260: 6f6e 7465 7374 5b22 5374 6172 7444 6174  ontest["StartDat
+00005270: 6522 5d20 3d20 7365 6c66 2e63 6f6e 7465  e"] = self.conte
+00005280: 7374 5f64 6961 6c6f 672e 6461 7465 5469  st_dialog.dateTi
+00005290: 6d65 4564 6974 2e64 6174 6554 696d 6528  meEdit.dateTime(
+000052a0: 292e 746f 5374 7269 6e67 280a 2020 2020  ).toString(.    
+000052b0: 2020 2020 2020 2020 2279 7979 792d 4d4d          "yyyy-MM
+000052c0: 2d64 6420 6868 3a6d 6d3a 7373 220a 2020  -dd hh:mm:ss".  
+000052d0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+000052e0: 636f 6e74 6573 745b 224f 7065 7261 746f  contest["Operato
+000052f0: 7243 6174 6567 6f72 7922 5d20 3d20 7365  rCategory"] = se
+00005300: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
+00005310: 672e 6f70 6572 6174 6f72 5f63 6c61 7373  g.operator_class
+00005320: 2e63 7572 7265 6e74 5465 7874 2829 0a20  .currentText(). 
+00005330: 2020 2020 2020 2063 6f6e 7465 7374 5b22         contest["
+00005340: 4261 6e64 4361 7465 676f 7279 225d 203d  BandCategory"] =
+00005350: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
+00005360: 616c 6f67 2e62 616e 642e 6375 7272 656e  alog.band.curren
+00005370: 7454 6578 7428 290a 2020 2020 2020 2020  tText().        
+00005380: 636f 6e74 6573 745b 2250 6f77 6572 4361  contest["PowerCa
+00005390: 7465 676f 7279 225d 203d 2073 656c 662e  tegory"] = self.
+000053a0: 636f 6e74 6573 745f 6469 616c 6f67 2e70  contest_dialog.p
+000053b0: 6f77 6572 2e63 7572 7265 6e74 5465 7874  ower.currentText
+000053c0: 2829 0a20 2020 2020 2020 2063 6f6e 7465  ().        conte
+000053d0: 7374 5b22 4d6f 6465 4361 7465 676f 7279  st["ModeCategory
+000053e0: 225d 203d 2073 656c 662e 636f 6e74 6573  "] = self.contes
+000053f0: 745f 6469 616c 6f67 2e6d 6f64 652e 6375  t_dialog.mode.cu
+00005400: 7272 656e 7454 6578 7428 290a 2020 2020  rrentText().    
+00005410: 2020 2020 636f 6e74 6573 745b 224f 7665      contest["Ove
+00005420: 726c 6179 4361 7465 676f 7279 225d 203d  rlayCategory"] =
+00005430: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
+00005440: 616c 6f67 2e6f 7665 726c 6179 2e63 7572  alog.overlay.cur
+00005450: 7265 6e74 5465 7874 2829 0a20 2020 2020  rentText().     
+00005460: 2020 2063 6f6e 7465 7374 5b22 4f70 6572     contest["Oper
+00005470: 6174 6f72 7322 5d20 3d20 7365 6c66 2e63  ators"] = self.c
+00005480: 6f6e 7465 7374 5f64 6961 6c6f 672e 6f70  ontest_dialog.op
+00005490: 6572 6174 6f72 732e 7465 7874 2829 0a20  erators.text(). 
+000054a0: 2020 2020 2020 2063 6f6e 7465 7374 5b22         contest["
+000054b0: 536f 6170 626f 7822 5d20 3d20 7365 6c66  Soapbox"] = self
+000054c0: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
+000054d0: 736f 6170 626f 782e 746f 506c 6169 6e54  soapbox.toPlainT
+000054e0: 6578 7428 290a 2020 2020 2020 2020 636f  ext().        co
+000054f0: 6e74 6573 745b 2253 656e 7445 7863 6861  ntest["SentExcha
+00005500: 6e67 6522 5d20 3d20 7365 6c66 2e63 6f6e  nge"] = self.con
+00005510: 7465 7374 5f64 6961 6c6f 672e 6578 6368  test_dialog.exch
+00005520: 616e 6765 2e74 6578 7428 290a 2020 2020  ange.text().    
+00005530: 2020 2020 636f 6e74 6573 745b 2243 6f6e      contest["Con
+00005540: 7465 7374 4e52 225d 203d 2073 656c 662e  testNR"] = self.
+00005550: 7072 6566 2e67 6574 2822 636f 6e74 6573  pref.get("contes
+00005560: 7422 2c20 3129 0a20 2020 2020 2020 2063  t", 1).        c
+00005570: 6f6e 7465 7374 5b22 5374 6174 696f 6e43  ontest["StationC
+00005580: 6174 6567 6f72 7922 5d20 3d20 7365 6c66  ategory"] = self
+00005590: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
+000055a0: 7374 6174 696f 6e2e 6375 7272 656e 7454  station.currentT
+000055b0: 6578 7428 290a 2020 2020 2020 2020 636f  ext().        co
+000055c0: 6e74 6573 745b 2241 7373 6973 7465 6443  ntest["AssistedC
+000055d0: 6174 6567 6f72 7922 5d20 3d20 7365 6c66  ategory"] = self
+000055e0: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
+000055f0: 6173 7369 7374 6564 2e63 7572 7265 6e74  assisted.current
+00005600: 5465 7874 2829 0a20 2020 2020 2020 2063  Text().        c
+00005610: 6f6e 7465 7374 5b22 5472 616e 736d 6974  ontest["Transmit
+00005620: 7465 7243 6174 6567 6f72 7922 5d20 3d20  terCategory"] = 
+00005630: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
+00005640: 6c6f 672e 7472 616e 736d 6974 7465 722e  log.transmitter.
+00005650: 6375 7272 656e 7454 6578 7428 290a 0a20  currentText().. 
+00005660: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
+00005670: 6275 6728 2225 7322 2c20 6622 7b63 6f6e  bug("%s", f"{con
+00005680: 7465 7374 7d22 290a 2020 2020 2020 2020  test}").        
+00005690: 7365 6c66 2e64 6174 6162 6173 652e 7570  self.database.up
+000056a0: 6461 7465 5f63 6f6e 7465 7374 2863 6f6e  date_contest(con
+000056b0: 7465 7374 290a 2020 2020 2020 2020 7365  test).        se
+000056c0: 6c66 2e77 7269 7465 5f70 7265 6665 7265  lf.write_prefere
+000056d0: 6e63 6528 290a 2020 2020 2020 2020 7365  nce().        se
+000056e0: 6c66 2e6c 6f61 645f 636f 6e74 6573 7428  lf.load_contest(
+000056f0: 290a 0a20 2020 2064 6566 206c 6f61 645f  )..    def load_
+00005700: 636f 6e74 6573 7428 7365 6c66 293a 0a20  contest(self):. 
+00005710: 2020 2020 2020 2022 2222 6c6f 6164 2061         """load a
+00005720: 2063 6f6e 7465 7374 2222 220a 2020 2020   contest""".    
+00005730: 2020 2020 6966 2073 656c 662e 7072 6566      if self.pref
+00005740: 2e67 6574 2822 636f 6e74 6573 7422 293a  .get("contest"):
+00005750: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00005760: 662e 636f 6e74 6573 745f 7365 7474 696e  f.contest_settin
+00005770: 6773 203d 2073 656c 662e 6461 7461 6261  gs = self.databa
+00005780: 7365 2e66 6574 6368 5f63 6f6e 7465 7374  se.fetch_contest
+00005790: 5f62 795f 6964 280a 2020 2020 2020 2020  _by_id(.        
+000057a0: 2020 2020 2020 2020 7365 6c66 2e70 7265          self.pre
+000057b0: 662e 6765 7428 2263 6f6e 7465 7374 2229  f.get("contest")
+000057c0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+000057d0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+000057e0: 6c66 2e63 6f6e 7465 7374 5f73 6574 7469  lf.contest_setti
+000057f0: 6e67 733a 0a20 2020 2020 2020 2020 2020  ngs:.           
+00005800: 2020 2020 2073 656c 662e 6461 7461 6261       self.databa
+00005810: 7365 2e63 7572 7265 6e74 5f63 6f6e 7465  se.current_conte
+00005820: 7374 203d 2073 656c 662e 7072 6566 2e67  st = self.pref.g
+00005830: 6574 2822 636f 6e74 6573 7422 290a 2020  et("contest").  
+00005840: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00005850: 2073 656c 662e 636f 6e74 6573 745f 7365   self.contest_se
+00005860: 7474 696e 6773 2e67 6574 2822 436f 6e74  ttings.get("Cont
+00005870: 6573 744e 616d 6522 293a 0a20 2020 2020  estName"):.     
+00005880: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00005890: 656c 662e 636f 6e74 6573 7420 3d20 646f  elf.contest = do
+000058a0: 696d 7028 7365 6c66 2e63 6f6e 7465 7374  imp(self.contest
+000058b0: 5f73 6574 7469 6e67 732e 6765 7428 2243  _settings.get("C
+000058c0: 6f6e 7465 7374 4e61 6d65 2229 290a 2020  ontestName")).  
+000058d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000058e0: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
+000058f0: 4c6f 6164 6564 2043 6f6e 7465 7374 204e  Loaded Contest N
+00005900: 616d 6520 3d20 2573 222c 2073 656c 662e  ame = %s", self.
+00005910: 636f 6e74 6573 742e 6e61 6d65 290a 2020  contest.name).  
+00005920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005930: 2020 7365 6c66 2e73 6574 5f77 696e 646f    self.set_windo
+00005940: 775f 7469 746c 6528 290a 2020 2020 2020  w_title().      
+00005950: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00005960: 6c66 2e63 6f6e 7465 7374 2e69 6e69 745f  lf.contest.init_
+00005970: 636f 6e74 6573 7428 7365 6c66 290a 2020  contest(self).  
+00005980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005990: 2020 7365 6c66 2e68 6964 655f 6261 6e64    self.hide_band
+000059a0: 5f6d 6f64 6528 7365 6c66 2e63 6f6e 7465  _mode(self.conte
+000059b0: 7374 5f73 6574 7469 6e67 732e 6765 7428  st_settings.get(
+000059c0: 224d 6f64 6543 6174 6567 6f72 7922 2c20  "ModeCategory", 
+000059d0: 2222 2929 0a20 2020 2020 2020 2020 2020  "")).           
+000059e0: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+000059f0: 6465 6275 6728 2225 7322 2c20 6622 7b73  debug("%s", f"{s
+00005a00: 656c 662e 636f 6e74 6573 745f 7365 7474  elf.contest_sett
+00005a10: 696e 6773 7d22 290a 2020 2020 2020 2020  ings}").        
+00005a20: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00005a30: 656c 662e 636f 6e74 6573 745f 7365 7474  elf.contest_sett
+00005a40: 696e 6773 2e67 6574 2822 4d6f 6465 4361  ings.get("ModeCa
+00005a50: 7465 676f 7279 222c 2022 2229 203d 3d20  tegory", "") == 
+00005a60: 2243 5722 3a0a 2020 2020 2020 2020 2020  "CW":.          
+00005a70: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00005a80: 6c66 2e73 6574 6d6f 6465 2822 4357 2229  lf.setmode("CW")
+00005a90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005aa0: 2020 2020 2020 2020 2073 656c 662e 7261           self.ra
+00005ab0: 6469 6f5f 7374 6174 655b 226d 6f64 6522  dio_state["mode"
+00005ac0: 5d20 3d20 2243 5722 0a20 2020 2020 2020  ] = "CW".       
+00005ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ae0: 2069 6620 7365 6c66 2e72 6967 5f63 6f6e   if self.rig_con
+00005af0: 7472 6f6c 3a0a 2020 2020 2020 2020 2020  trol:.          
+00005b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b10: 2020 6966 2073 656c 662e 7269 675f 636f    if self.rig_co
+00005b20: 6e74 726f 6c2e 6f6e 6c69 6e65 3a0a 2020  ntrol.online:.  
+00005b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b40: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00005b50: 6c66 2e72 6967 5f63 6f6e 7472 6f6c 2e73  lf.rig_control.s
+00005b60: 6574 5f6d 6f64 6528 2243 5722 290a 2020  et_mode("CW").  
+00005b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b80: 2020 2020 2020 6261 6e64 203d 2067 6574        band = get
+00005b90: 6261 6e64 2873 7472 2873 656c 662e 7261  band(str(self.ra
+00005ba0: 6469 6f5f 7374 6174 652e 6765 7428 2276  dio_state.get("v
+00005bb0: 666f 6122 2c20 2230 2e30 2229 2929 0a20  foa", "0.0"))). 
+00005bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005bd0: 2020 2020 2020 2073 656c 662e 7365 745f         self.set_
+00005be0: 6261 6e64 5f69 6e64 6963 6174 6f72 2862  band_indicator(b
+00005bf0: 616e 6429 0a20 2020 2020 2020 2020 2020  and).           
+00005c00: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00005c10: 662e 7365 745f 7769 6e64 6f77 5f74 6974  f.set_window_tit
+00005c20: 6c65 2829 0a20 2020 2020 2020 2020 2020  le().           
+00005c30: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00005c40: 2e63 6f6e 7465 7374 5f73 6574 7469 6e67  .contest_setting
+00005c50: 732e 6765 7428 224d 6f64 6543 6174 6567  s.get("ModeCateg
+00005c60: 6f72 7922 2c20 2222 2920 3d3d 2022 5353  ory", "") == "SS
+00005c70: 4222 3a0a 2020 2020 2020 2020 2020 2020  B":.            
+00005c80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00005c90: 2e73 6574 6d6f 6465 2822 5353 4222 290a  .setmode("SSB").
+00005ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005cb0: 2020 2020 2020 2020 6966 2069 6e74 2873          if int(s
+00005cc0: 656c 662e 7261 6469 6f5f 7374 6174 652e  elf.radio_state.
+00005cd0: 6765 7428 2276 666f 6122 2c20 3029 2920  get("vfoa", 0)) 
+00005ce0: 3e20 3130 3030 3030 3030 3a0a 2020 2020  > 10000000:.    
+00005cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d00: 2020 2020 2020 2020 7365 6c66 2e72 6164          self.rad
+00005d10: 696f 5f73 7461 7465 5b22 6d6f 6465 225d  io_state["mode"]
+00005d20: 203d 2022 5553 4222 0a20 2020 2020 2020   = "USB".       
+00005d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d40: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00005d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d60: 2020 2073 656c 662e 7261 6469 6f5f 7374     self.radio_st
+00005d70: 6174 655b 226d 6f64 6522 5d20 3d20 224c  ate["mode"] = "L
+00005d80: 5342 220a 2020 2020 2020 2020 2020 2020  SB".            
+00005d90: 2020 2020 2020 2020 2020 2020 6261 6e64              band
+00005da0: 203d 2067 6574 6261 6e64 2873 7472 2873   = getband(str(s
+00005db0: 656c 662e 7261 6469 6f5f 7374 6174 652e  elf.radio_state.
+00005dc0: 6765 7428 2276 666f 6122 2c20 2230 2e30  get("vfoa", "0.0
+00005dd0: 2229 2929 0a20 2020 2020 2020 2020 2020  "))).           
+00005de0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00005df0: 662e 7365 745f 6261 6e64 5f69 6e64 6963  f.set_band_indic
+00005e00: 6174 6f72 2862 616e 6429 0a20 2020 2020  ator(band).     
+00005e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e20: 2020 2073 656c 662e 7365 745f 7769 6e64     self.set_wind
+00005e30: 6f77 5f74 6974 6c65 2829 0a20 2020 2020  ow_title().     
+00005e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e50: 2020 2069 6620 7365 6c66 2e72 6967 5f63     if self.rig_c
+00005e60: 6f6e 7472 6f6c 3a0a 2020 2020 2020 2020  ontrol:.        
+00005e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e80: 2020 2020 7365 6c66 2e72 6967 5f63 6f6e      self.rig_con
+00005e90: 7472 6f6c 2e73 6574 5f6d 6f64 6528 7365  trol.set_mode(se
+00005ea0: 6c66 2e72 6164 696f 5f73 7461 7465 2e67  lf.radio_state.g
+00005eb0: 6574 2822 6d6f 6465 2229 290a 0a20 2020  et("mode"))..   
+00005ec0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00005ed0: 6861 7361 7474 7228 7365 6c66 2e63 6f6e  hasattr(self.con
+00005ee0: 7465 7374 2c20 226d 6f64 6522 293a 0a20  test, "mode"):. 
+00005ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f00: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+00005f10: 2225 7322 2c20 6622 2020 2a2a 2a2a 2020  "%s", f"  ****  
+00005f20: 7b73 656c 662e 636f 6e74 6573 747d 2229  {self.contest}")
+00005f30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005f40: 2020 2020 2069 6620 7365 6c66 2e63 6f6e       if self.con
+00005f50: 7465 7374 2e6d 6f64 6520 696e 205b 2243  test.mode in ["C
+00005f60: 5722 2c20 2242 4f54 4822 5d3a 0a20 2020  W", "BOTH"]:.   
+00005f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f80: 2020 2020 2073 656c 662e 6377 5f73 7065       self.cw_spe
+00005f90: 6564 2e73 686f 7728 290a 2020 2020 2020  ed.show().      
+00005fa0: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00005fb0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00005fc0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00005fd0: 2e63 775f 7370 6565 642e 6869 6465 2829  .cw_speed.hide()
+00005fe0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005ff0: 2020 636d 6420 3d20 7b7d 0a20 2020 2020    cmd = {}.     
+00006000: 2020 2020 2020 2020 2020 2063 6d64 5b22             cmd["
+00006010: 636d 6422 5d20 3d20 224e 4557 4442 220a  cmd"] = "NEWDB".
+00006020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006030: 636d 645b 2273 7461 7469 6f6e 225d 203d  cmd["station"] =
+00006040: 2070 6c61 7466 6f72 6d2e 6e6f 6465 2829   platform.node()
+00006050: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006060: 2073 656c 662e 6d75 6c74 6963 6173 745f   self.multicast_
+00006070: 696e 7465 7266 6163 652e 7365 6e64 5f61  interface.send_a
+00006080: 735f 6a73 6f6e 2863 6d64 290a 2020 2020  s_json(cmd).    
+00006090: 2020 2020 2020 2020 2020 2020 6966 2068              if h
+000060a0: 6173 6174 7472 2873 656c 662e 636f 6e74  asattr(self.cont
+000060b0: 6573 742c 2022 636f 6c75 6d6e 7322 293a  est, "columns"):
+000060c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000060d0: 2020 2020 2063 6d64 203d 207b 7d0a 2020       cmd = {}.  
+000060e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000060f0: 2020 636d 645b 2263 6d64 225d 203d 2022    cmd["cmd"] = "
+00006100: 5348 4f57 434f 4c55 4d4e 5322 0a20 2020  SHOWCOLUMNS".   
+00006110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006120: 2063 6d64 5b22 7374 6174 696f 6e22 5d20   cmd["station"] 
+00006130: 3d20 706c 6174 666f 726d 2e6e 6f64 6528  = platform.node(
+00006140: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00006150: 2020 2020 2020 636d 645b 2243 4f4c 554d        cmd["COLUM
+00006160: 4e53 225d 203d 2073 656c 662e 636f 6e74  NS"] = self.cont
+00006170: 6573 742e 636f 6c75 6d6e 730a 2020 2020  est.columns.    
+00006180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006190: 7365 6c66 2e6d 756c 7469 6361 7374 5f69  self.multicast_i
+000061a0: 6e74 6572 6661 6365 2e73 656e 645f 6173  nterface.send_as
+000061b0: 5f6a 736f 6e28 636d 6429 0a0a 2020 2020  _json(cmd)..    
+000061c0: 6465 6620 6368 6563 6b5f 666f 725f 6e65  def check_for_ne
+000061d0: 775f 6374 7928 7365 6c66 293a 0a20 2020  w_cty(self):.   
+000061e0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000061f0: 2043 6865 636b 7320 666f 7220 6120 6e65   Checks for a ne
+00006200: 7720 6374 792e 6461 7420 6669 6c65 2e0a  w cty.dat file..
+00006210: 2020 2020 2020 2020 4c6f 6164 7320 6974          Loads it
+00006220: 2069 6620 6176 6169 6c61 626c 652e 0a20   if available.. 
+00006230: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00006240: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+00006250: 2020 2020 6374 7920 3d20 6e6f 7463 7479      cty = notcty
+00006260: 7061 7273 6572 2e42 6967 4374 7928 574f  parser.BigCty(WO
+00006270: 524b 494e 475f 5041 5448 202b 2022 2f64  RKING_PATH + "/d
+00006280: 6174 612f 6374 792e 6a73 6f6e 2229 0a20  ata/cty.json"). 
+00006290: 2020 2020 2020 2020 2020 2075 7064 6174             updat
+000062a0: 655f 6176 6169 6c61 626c 6520 3d20 6374  e_available = ct
+000062b0: 792e 6368 6563 6b5f 7570 6461 7465 2829  y.check_update()
+000062c0: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
+000062d0: 4578 6365 7074 696f 6e20 6173 2074 6865  Exception as the
+000062e0: 5f65 7272 6f72 3a0a 2020 2020 2020 2020  _error:.        
+000062f0: 2020 2020 6374 7920 3d20 4e6f 6e65 2020      cty = None  
+00006300: 2320 6672 6565 2075 7020 7468 6520 6d65  # free up the me
+00006310: 6d6f 7279 0a20 2020 2020 2020 2020 2020  mory.           
+00006320: 206c 6f67 6765 722e 6465 6275 6728 2263   logger.debug("c
+00006330: 7479 2070 6172 7365 7220 7265 7475 726e  ty parser return
+00006340: 6564 2061 6e20 6572 726f 723a 2025 7322  ed an error: %s"
+00006350: 2c20 7468 655f 6572 726f 7229 0a20 2020  , the_error).   
+00006360: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+00006370: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+00006380: 6562 7567 2822 4e65 7765 7220 6374 7920  ebug("Newer cty 
+00006390: 6669 6c65 2061 7661 696c 6162 6c65 2025  file available %
+000063a0: 7322 2c20 7374 7228 7570 6461 7465 5f61  s", str(update_a
+000063b0: 7661 696c 6162 6c65 2929 0a0a 2020 2020  vailable))..    
+000063c0: 2020 2020 6966 2075 7064 6174 655f 6176      if update_av
+000063d0: 6169 6c61 626c 653a 0a20 2020 2020 2020  ailable:.       
+000063e0: 2020 2020 2073 656c 662e 7368 6f77 5f6d       self.show_m
+000063f0: 6573 7361 6765 5f62 6f78 2822 5570 6461  essage_box("Upda
+00006400: 7469 6e67 2063 7479 2066 696c 652e 2e22  ting cty file.."
+00006410: 290a 2020 2020 2020 2020 2020 2020 7472  ).            tr
+00006420: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
+00006430: 2020 2075 7064 6174 6564 203d 2063 7479     updated = cty
+00006440: 2e75 7064 6174 6528 290a 2020 2020 2020  .update().      
+00006450: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
+00006460: 6570 7469 6f6e 2061 7320 7468 655f 6572  eption as the_er
+00006470: 726f 723a 0a20 2020 2020 2020 2020 2020  ror:.           
+00006480: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
+00006490: 6728 2263 7479 2070 6172 7365 7220 7265  g("cty parser re
+000064a0: 7475 726e 6564 2061 6e20 6572 726f 723a  turned an error:
+000064b0: 2025 7322 2c20 7468 655f 6572 726f 7229   %s", the_error)
+000064c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000064d0: 2063 7479 203d 204e 6f6e 6520 2023 2066   cty = None  # f
+000064e0: 7265 6520 7570 2074 6865 206d 656d 6f72  ree up the memor
+000064f0: 790a 2020 2020 2020 2020 2020 2020 2020  y.              
+00006500: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+00006510: 2020 2020 2069 6620 7570 6461 7465 643a       if updated:
+00006520: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006530: 2063 7479 2e64 756d 7028 574f 524b 494e   cty.dump(WORKIN
+00006540: 475f 5041 5448 202b 2022 2f64 6174 612f  G_PATH + "/data/
+00006550: 6374 792e 6a73 6f6e 2229 0a20 2020 2020  cty.json").     
+00006560: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00006570: 7368 6f77 5f6d 6573 7361 6765 5f62 6f78  show_message_box
+00006580: 2822 6374 7920 6669 6c65 2075 7064 6174  ("cty file updat
+00006590: 6564 2e22 290a 2020 2020 2020 2020 2020  ed.").          
+000065a0: 2020 2020 2020 7769 7468 206f 7065 6e28        with open(
+000065b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000065c0: 2020 2020 2057 4f52 4b49 4e47 5f50 4154       WORKING_PAT
+000065d0: 4820 2b20 222f 6461 7461 2f63 7479 2e6a  H + "/data/cty.j
+000065e0: 736f 6e22 2c20 2272 7422 2c20 656e 636f  son", "rt", enco
+000065f0: 6469 6e67 3d22 7574 662d 3822 0a20 2020  ding="utf-8".   
+00006600: 2020 2020 2020 2020 2020 2020 2029 2061               ) a
+00006610: 7320 635f 6669 6c65 3a0a 2020 2020 2020  s c_file:.      
+00006620: 2020 2020 2020 2020 2020 2020 2020 676c                gl
+00006630: 6f62 616c 7328 295b 2243 5459 4649 4c45  obals()["CTYFILE
+00006640: 225d 203d 206c 6f61 6473 2863 5f66 696c  "] = loads(c_fil
+00006650: 652e 7265 6164 2829 290a 2020 2020 2020  e.read()).      
+00006660: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00006670: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00006680: 2e73 686f 775f 6d65 7373 6167 655f 626f  .show_message_bo
+00006690: 7828 2241 6e20 4572 726f 7220 6f63 6375  x("An Error occu
+000066a0: 7265 6420 7570 6461 7469 6e67 2066 696c  red updating fil
+000066b0: 652e 2229 0a20 2020 2020 2020 2063 7479  e.").        cty
+000066c0: 203d 204e 6f6e 6520 2023 2066 7265 6520   = None  # free 
+000066d0: 7570 2074 6865 206d 656d 6f72 790a 0a20  up the memory.. 
+000066e0: 2020 2064 6566 2068 6964 655f 6261 6e64     def hide_band
+000066f0: 5f6d 6f64 6528 7365 6c66 2c20 7468 655f  _mode(self, the_
+00006700: 6d6f 6465 3a20 7374 7229 202d 3e20 4e6f  mode: str) -> No
+00006710: 6e65 3a0a 2020 2020 2020 2020 2222 2268  ne:.        """h
+00006720: 6964 6522 2222 0a20 2020 2020 2020 206c  ide""".        l
+00006730: 6f67 6765 722e 6465 6275 6728 2225 7322  ogger.debug("%s"
+00006740: 2c20 6622 7b74 6865 5f6d 6f64 657d 2229  , f"{the_mode}")
+00006750: 0a20 2020 2020 2020 2073 656c 662e 4261  .        self.Ba
+00006760: 6e64 5f4d 6f64 655f 4672 616d 655f 4357  nd_Mode_Frame_CW
+00006770: 2e68 6964 6528 290a 2020 2020 2020 2020  .hide().        
+00006780: 7365 6c66 2e42 616e 645f 4d6f 6465 5f46  self.Band_Mode_F
+00006790: 7261 6d65 5f53 5342 2e68 6964 6528 290a  rame_SSB.hide().
+000067a0: 2020 2020 2020 2020 7365 6c66 2e42 616e          self.Ban
+000067b0: 645f 4d6f 6465 5f46 7261 6d65 5f52 5454  d_Mode_Frame_RTT
+000067c0: 592e 6869 6465 2829 0a20 2020 2020 2020  Y.hide().       
+000067d0: 206d 6f64 6573 203d 207b 0a20 2020 2020   modes = {.     
+000067e0: 2020 2020 2020 2022 4357 223a 2028 7365         "CW": (se
+000067f0: 6c66 2e42 616e 645f 4d6f 6465 5f46 7261  lf.Band_Mode_Fra
+00006800: 6d65 5f43 572c 292c 0a20 2020 2020 2020  me_CW,),.       
+00006810: 2020 2020 2022 5353 4222 3a20 2873 656c       "SSB": (sel
+00006820: 662e 4261 6e64 5f4d 6f64 655f 4672 616d  f.Band_Mode_Fram
+00006830: 655f 5353 422c 292c 0a20 2020 2020 2020  e_SSB,),.       
+00006840: 2020 2020 2022 5254 5459 223a 2028 7365       "RTTY": (se
+00006850: 6c66 2e42 616e 645f 4d6f 6465 5f46 7261  lf.Band_Mode_Fra
+00006860: 6d65 5f52 5454 592c 292c 0a20 2020 2020  me_RTTY,),.     
+00006870: 2020 2020 2020 2022 5053 4b22 3a20 2873         "PSK": (s
+00006880: 656c 662e 4261 6e64 5f4d 6f64 655f 4672  elf.Band_Mode_Fr
+00006890: 616d 655f 5254 5459 2c29 2c0a 2020 2020  ame_RTTY,),.    
+000068a0: 2020 2020 2020 2020 2253 5342 2b43 5722          "SSB+CW"
+000068b0: 3a20 2873 656c 662e 4261 6e64 5f4d 6f64  : (self.Band_Mod
+000068c0: 655f 4672 616d 655f 4357 2c20 7365 6c66  e_Frame_CW, self
+000068d0: 2e42 616e 645f 4d6f 6465 5f46 7261 6d65  .Band_Mode_Frame
+000068e0: 5f53 5342 292c 0a20 2020 2020 2020 2020  _SSB),.         
+000068f0: 2020 2022 424f 5448 223a 2028 7365 6c66     "BOTH": (self
+00006900: 2e42 616e 645f 4d6f 6465 5f46 7261 6d65  .Band_Mode_Frame
+00006910: 5f43 572c 2073 656c 662e 4261 6e64 5f4d  _CW, self.Band_M
+00006920: 6f64 655f 4672 616d 655f 5353 4229 2c0a  ode_Frame_SSB),.
+00006930: 2020 2020 2020 2020 2020 2020 2244 4947              "DIG
+00006940: 4954 414c 223a 2028 7365 6c66 2e42 616e  ITAL": (self.Ban
+00006950: 645f 4d6f 6465 5f46 7261 6d65 5f52 5454  d_Mode_Frame_RTT
+00006960: 592c 292c 0a20 2020 2020 2020 2020 2020  Y,),.           
+00006970: 2022 5353 422b 4357 2b44 4947 4954 414c   "SSB+CW+DIGITAL
+00006980: 223a 2028 0a20 2020 2020 2020 2020 2020  ": (.           
+00006990: 2020 2020 2073 656c 662e 4261 6e64 5f4d       self.Band_M
+000069a0: 6f64 655f 4672 616d 655f 5254 5459 2c0a  ode_Frame_RTTY,.
+000069b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000069c0: 7365 6c66 2e42 616e 645f 4d6f 6465 5f46  self.Band_Mode_F
+000069d0: 7261 6d65 5f43 572c 0a20 2020 2020 2020  rame_CW,.       
+000069e0: 2020 2020 2020 2020 2073 656c 662e 4261           self.Ba
+000069f0: 6e64 5f4d 6f64 655f 4672 616d 655f 5353  nd_Mode_Frame_SS
+00006a00: 422c 0a20 2020 2020 2020 2020 2020 2029  B,.            )
+00006a10: 2c0a 2020 2020 2020 2020 2020 2020 2246  ,.            "F
+00006a20: 4d22 3a20 2873 656c 662e 4261 6e64 5f4d  M": (self.Band_M
+00006a30: 6f64 655f 4672 616d 655f 5353 422c 292c  ode_Frame_SSB,),
+00006a40: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
+00006a50: 2020 2066 7261 6d65 7320 3d20 6d6f 6465     frames = mode
+00006a60: 732e 6765 7428 7468 655f 6d6f 6465 290a  s.get(the_mode).
+00006a70: 2020 2020 2020 2020 6966 2066 7261 6d65          if frame
+00006a80: 733a 0a20 2020 2020 2020 2020 2020 2066  s:.            f
+00006a90: 6f72 2066 7261 6d65 2069 6e20 6672 616d  or frame in fram
+00006aa0: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+00006ab0: 2020 2020 6672 616d 652e 7368 6f77 2829      frame.show()
+00006ac0: 0a0a 2020 2020 6465 6620 6669 6c65 7069  ..    def filepi
+00006ad0: 636b 6572 2873 656c 662c 2061 6374 696f  cker(self, actio
+00006ae0: 6e3a 2073 7472 2920 2d3e 2073 7472 3a0a  n: str) -> str:.
+00006af0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00006b00: 2020 2020 4765 7420 6120 6669 6c65 6e61      Get a filena
+00006b10: 6d65 0a20 2020 2020 2020 2061 6374 696f  me.        actio
+00006b20: 6e3a 2022 6e65 7722 206f 7220 226f 7065  n: "new" or "ope
+00006b30: 6e22 0a20 2020 2020 2020 2022 2222 0a20  n".        """. 
+00006b40: 2020 2020 2020 206f 7074 696f 6e73 203d         options =
+00006b50: 2051 4669 6c65 4469 616c 6f67 2e4f 7074   QFileDialog.Opt
+00006b60: 696f 6e73 2829 0a20 2020 2020 2020 206f  ions().        o
+00006b70: 7074 696f 6e73 207c 3d20 5146 696c 6544  ptions |= QFileD
+00006b80: 6961 6c6f 672e 446f 6e74 5573 654e 6174  ialog.DontUseNat
+00006b90: 6976 6544 6961 6c6f 670a 2020 2020 2020  iveDialog.      
+00006ba0: 2020 6f70 7469 6f6e 7320 7c3d 2051 4669    options |= QFi
+00006bb0: 6c65 4469 616c 6f67 2e44 6f6e 7443 6f6e  leDialog.DontCon
+00006bc0: 6669 726d 4f76 6572 7772 6974 650a 2020  firmOverwrite.  
+00006bd0: 2020 2020 2020 6966 2061 6374 696f 6e20        if action 
+00006be0: 3d3d 2022 6e65 7722 3a0a 2020 2020 2020  == "new":.      
+00006bf0: 2020 2020 2020 6669 6c65 2c20 5f20 3d20        file, _ = 
+00006c00: 5146 696c 6544 6961 6c6f 672e 6765 7453  QFileDialog.getS
+00006c10: 6176 6546 696c 654e 616d 6528 0a20 2020  aveFileName(.   
+00006c20: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00006c30: 662c 0a20 2020 2020 2020 2020 2020 2020  f,.             
+00006c40: 2020 2022 4368 6f6f 7365 2061 2044 6174     "Choose a Dat
+00006c50: 6162 6173 6522 2c0a 2020 2020 2020 2020  abase",.        
+00006c60: 2020 2020 2020 2020 4441 5441 5f50 4154          DATA_PAT
+00006c70: 482c 0a20 2020 2020 2020 2020 2020 2020  H,.             
+00006c80: 2020 2022 4461 7461 6261 7365 2028 2a2e     "Database (*.
+00006c90: 6462 2922 2c0a 2020 2020 2020 2020 2020  db)",.          
+00006ca0: 2020 2020 2020 6f70 7469 6f6e 733d 6f70        options=op
+00006cb0: 7469 6f6e 732c 0a20 2020 2020 2020 2020  tions,.         
+00006cc0: 2020 2029 0a20 2020 2020 2020 2069 6620     ).        if 
+00006cd0: 6163 7469 6f6e 203d 3d20 226f 7065 6e22  action == "open"
+00006ce0: 3a0a 2020 2020 2020 2020 2020 2020 6669  :.            fi
+00006cf0: 6c65 2c20 5f20 3d20 5146 696c 6544 6961  le, _ = QFileDia
+00006d00: 6c6f 672e 6765 744f 7065 6e46 696c 654e  log.getOpenFileN
+00006d10: 616d 6528 0a20 2020 2020 2020 2020 2020  ame(.           
+00006d20: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+00006d30: 2020 2020 2020 2020 2020 2022 4368 6f6f             "Choo
+00006d40: 7365 2061 2044 6174 6162 6173 6522 2c0a  se a Database",.
+00006d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d60: 4441 5441 5f50 4154 482c 0a20 2020 2020  DATA_PATH,.     
+00006d70: 2020 2020 2020 2020 2020 2022 4461 7461             "Data
+00006d80: 6261 7365 2028 2a2e 6462 2922 2c0a 2020  base (*.db)",.  
+00006d90: 2020 2020 2020 2020 2020 2020 2020 6f70                op
+00006da0: 7469 6f6e 733d 6f70 7469 6f6e 732c 0a20  tions=options,. 
+00006db0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00006dc0: 2020 2020 2072 6574 7572 6e20 6669 6c65       return file
+00006dd0: 0a0a 2020 2020 6465 6620 7265 6361 6c63  ..    def recalc
+00006de0: 756c 6174 655f 6d75 6c74 7328 7365 6c66  ulate_mults(self
+00006df0: 293a 0a20 2020 2020 2020 2022 2222 5265  ):.        """Re
+00006e00: 6361 6c63 756c 6174 6520 4d75 6c74 6970  calculate Multip
+00006e10: 6c69 6572 7322 2222 0a20 2020 2020 2020  liers""".       
+00006e20: 2073 656c 662e 636f 6e74 6573 742e 7265   self.contest.re
+00006e30: 6361 6c63 756c 6174 655f 6d75 6c74 7328  calculate_mults(
+00006e40: 7365 6c66 290a 0a20 2020 2064 6566 206c  self)..    def l
+00006e50: 6175 6e63 685f 6c6f 675f 7769 6e64 6f77  aunch_log_window
+00006e60: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00006e70: 2222 226c 6175 6e63 6820 7468 6520 4c6f  """launch the Lo
+00006e80: 6720 5769 6e64 6f77 2222 220a 2020 2020  g Window""".    
+00006e90: 2020 2020 6966 206e 6f74 2063 6865 636b      if not check
+00006ea0: 5f70 726f 6365 7373 2822 6c6f 6777 696e  _process("logwin
+00006eb0: 646f 772e 7079 2229 3a0a 2020 2020 2020  dow.py"):.      
+00006ec0: 2020 2020 2020 5f20 3d20 7375 6270 726f        _ = subpro
+00006ed0: 6365 7373 2e50 6f70 656e 285b 7379 732e  cess.Popen([sys.
+00006ee0: 6578 6563 7574 6162 6c65 2c20 574f 524b  executable, WORK
+00006ef0: 494e 475f 5041 5448 202b 2022 2f6c 6f67  ING_PATH + "/log
+00006f00: 7769 6e64 6f77 2e70 7922 5d29 0a0a 2020  window.py"])..  
+00006f10: 2020 6465 6620 6c61 756e 6368 5f62 616e    def launch_ban
+00006f20: 646d 6170 5f77 696e 646f 7728 7365 6c66  dmap_window(self
+00006f30: 293a 0a20 2020 2020 2020 2022 2222 6c61  ):.        """la
+00006f40: 756e 6368 2074 6865 204c 6f67 2057 696e  unch the Log Win
+00006f50: 646f 7722 2222 0a20 2020 2020 2020 2069  dow""".        i
+00006f60: 6620 6e6f 7420 6368 6563 6b5f 7072 6f63  f not check_proc
+00006f70: 6573 7328 2262 616e 646d 6170 2e70 7922  ess("bandmap.py"
+00006f80: 293a 0a20 2020 2020 2020 2020 2020 205f  ):.            _
+00006f90: 203d 2073 7562 7072 6f63 6573 732e 506f   = subprocess.Po
+00006fa0: 7065 6e28 5b73 7973 2e65 7865 6375 7461  pen([sys.executa
+00006fb0: 626c 652c 2057 4f52 4b49 4e47 5f50 4154  ble, WORKING_PAT
+00006fc0: 4820 2b20 222f 6261 6e64 6d61 702e 7079  H + "/bandmap.py
+00006fd0: 225d 290a 0a20 2020 2064 6566 2063 6c65  "])..    def cle
+00006fe0: 6172 5f62 616e 645f 696e 6469 6361 746f  ar_band_indicato
+00006ff0: 7273 2873 656c 6629 3a0a 2020 2020 2020  rs(self):.      
+00007000: 2020 2222 2243 6c65 6172 2074 6865 2069    """Clear the i
+00007010: 6e64 6963 6174 6f72 7322 2222 0a20 2020  ndicators""".   
+00007020: 2020 2020 2066 6f72 205f 2c20 696e 6469       for _, indi
+00007030: 6361 746f 7273 2069 6e20 7365 6c66 2e61  cators in self.a
+00007040: 6c6c 5f6d 6f64 655f 696e 6469 6361 746f  ll_mode_indicato
+00007050: 7273 2e69 7465 6d73 2829 3a0a 2020 2020  rs.items():.    
+00007060: 2020 2020 2020 2020 666f 7220 5f2c 2069          for _, i
+00007070: 6e64 6963 6174 6f72 2069 6e20 696e 6469  ndicator in indi
+00007080: 6361 746f 7273 2e69 7465 6d73 2829 3a0a  cators.items():.
+00007090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000070a0: 696e 6469 6361 746f 722e 7365 7446 7261  indicator.setFra
+000070b0: 6d65 5368 6170 6528 5174 5769 6467 6574  meShape(QtWidget
+000070c0: 732e 5146 7261 6d65 2e4e 6f46 7261 6d65  s.QFrame.NoFrame
+000070d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000070e0: 2020 696e 6469 6361 746f 722e 7365 7453    indicator.setS
+000070f0: 7479 6c65 5368 6565 7428 2266 6f6e 742d  tyleSheet("font-
+00007100: 6661 6d69 6c79 3a20 4a65 7442 7261 696e  family: JetBrain
+00007110: 7320 4d6f 6e6f 3b22 290a 0a20 2020 2064  s Mono;")..    d
+00007120: 6566 2073 6574 5f62 616e 645f 696e 6469  ef set_band_indi
+00007130: 6361 746f 7228 7365 6c66 2c20 6261 6e64  cator(self, band
+00007140: 3a20 7374 7229 202d 3e20 4e6f 6e65 3a0a  : str) -> None:.
+00007150: 2020 2020 2020 2020 2222 2253 6574 2074          """Set t
+00007160: 6865 2062 616e 6420 696e 6469 6361 746f  he band indicato
+00007170: 7222 2222 0a20 2020 2020 2020 2023 206c  r""".        # l
+00007180: 6f67 6765 722e 6465 6275 6728 2225 7322  ogger.debug("%s"
+00007190: 2c20 6622 6261 6e64 3a7b 6261 6e64 7d20  , f"band:{band} 
+000071a0: 6d6f 6465 3a20 7b73 656c 662e 6375 7272  mode: {self.curr
+000071b0: 656e 745f 6d6f 6465 7d22 290a 2020 2020  ent_mode}").    
+000071c0: 2020 2020 6966 2062 616e 6420 616e 6420      if band and 
+000071d0: 7365 6c66 2e63 7572 7265 6e74 5f6d 6f64  self.current_mod
+000071e0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+000071f0: 656c 662e 636c 6561 725f 6261 6e64 5f69  elf.clear_band_i
+00007200: 6e64 6963 6174 6f72 7328 290a 2020 2020  ndicators().    
+00007210: 2020 2020 2020 2020 696e 6469 6361 746f          indicato
+00007220: 7220 3d20 7365 6c66 2e61 6c6c 5f6d 6f64  r = self.all_mod
+00007230: 655f 696e 6469 6361 746f 7273 5b73 656c  e_indicators[sel
+00007240: 662e 6375 7272 656e 745f 6d6f 6465 5d2e  f.current_mode].
+00007250: 6765 7428 6261 6e64 2c20 4e6f 6e65 290a  get(band, None).
+00007260: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+00007270: 6e64 6963 6174 6f72 3a0a 2020 2020 2020  ndicator:.      
+00007280: 2020 2020 2020 2020 2020 696e 6469 6361            indica
+00007290: 746f 722e 7365 7446 7261 6d65 5368 6170  tor.setFrameShap
+000072a0: 6528 5174 5769 6467 6574 732e 5146 7261  e(QtWidgets.QFra
+000072b0: 6d65 2e42 6f78 290a 2020 2020 2020 2020  me.Box).        
+000072c0: 2020 2020 2020 2020 696e 6469 6361 746f          indicato
+000072d0: 722e 7365 7453 7479 6c65 5368 6565 7428  r.setStyleSheet(
+000072e0: 2266 6f6e 742d 6661 6d69 6c79 3a20 4a65  "font-family: Je
+000072f0: 7442 7261 696e 7320 4d6f 6e6f 3b20 636f  tBrains Mono; co
+00007300: 6c6f 723a 2067 7265 656e 3b22 290a 0a20  lor: green;").. 
+00007310: 2020 2064 6566 2063 6c6f 7365 4576 656e     def closeEven
+00007320: 7428 7365 6c66 2c20 5f65 7665 6e74 293a  t(self, _event):
+00007330: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00007340: 2020 2020 2057 7269 7465 2077 696e 646f       Write windo
+00007350: 7720 7369 7a65 2061 6e64 2070 6f73 6974  w size and posit
+00007360: 696f 6e20 746f 2063 6f6e 6669 6720 6669  ion to config fi
+00007370: 6c65 0a20 2020 2020 2020 2022 2222 0a20  le.        """. 
+00007380: 2020 2020 2020 2073 656c 662e 7072 6566         self.pref
+00007390: 5b22 7769 6e64 6f77 5f77 6964 7468 225d  ["window_width"]
+000073a0: 203d 2073 656c 662e 7369 7a65 2829 2e77   = self.size().w
+000073b0: 6964 7468 2829 0a20 2020 2020 2020 2073  idth().        s
+000073c0: 656c 662e 7072 6566 5b22 7769 6e64 6f77  elf.pref["window
+000073d0: 5f68 6569 6768 7422 5d20 3d20 7365 6c66  _height"] = self
+000073e0: 2e73 697a 6528 292e 6865 6967 6874 2829  .size().height()
+000073f0: 0a20 2020 2020 2020 2073 656c 662e 7072  .        self.pr
+00007400: 6566 5b22 7769 6e64 6f77 5f78 225d 203d  ef["window_x"] =
+00007410: 2073 656c 662e 706f 7328 292e 7828 290a   self.pos().x().
+00007420: 2020 2020 2020 2020 7365 6c66 2e70 7265          self.pre
+00007430: 665b 2277 696e 646f 775f 7922 5d20 3d20  f["window_y"] = 
+00007440: 7365 6c66 2e70 6f73 2829 2e79 2829 0a20  self.pos().y(). 
+00007450: 2020 2020 2020 2073 656c 662e 7772 6974         self.writ
+00007460: 655f 7072 6566 6572 656e 6365 2829 0a0a  e_preference()..
+00007470: 2020 2020 6465 6620 6374 795f 6c6f 6f6b      def cty_look
+00007480: 7570 2873 656c 662c 2063 616c 6c73 6967  up(self, callsig
+00007490: 6e3a 2073 7472 293a 0a20 2020 2020 2020  n: str):.       
+000074a0: 2022 2222 4c6f 6f6b 7570 2063 616c 6c73   """Lookup calls
+000074b0: 6967 6e20 696e 2063 7479 2e64 6174 2066  ign in cty.dat f
+000074c0: 696c 6522 2222 0a20 2020 2020 2020 2063  ile""".        c
+000074d0: 616c 6c73 6967 6e20 3d20 6361 6c6c 7369  allsign = callsi
+000074e0: 676e 2e75 7070 6572 2829 0a20 2020 2020  gn.upper().     
+000074f0: 2020 2066 6f72 2063 6f75 6e74 2069 6e20     for count in 
+00007500: 7265 7665 7273 6564 2872 616e 6765 286c  reversed(range(l
+00007510: 656e 2863 616c 6c73 6967 6e29 2929 3a0a  en(callsign))):.
+00007520: 2020 2020 2020 2020 2020 2020 7365 6172              sear
+00007530: 6368 6974 656d 203d 2063 616c 6c73 6967  chitem = callsig
+00007540: 6e5b 3a20 636f 756e 7420 2b20 315d 0a20  n[: count + 1]. 
+00007550: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00007560: 7420 3d20 7b6b 6579 3a20 7661 6c20 666f  t = {key: val fo
+00007570: 7220 6b65 792c 2076 616c 2069 6e20 4354  r key, val in CT
+00007580: 5946 494c 452e 6974 656d 7328 2920 6966  YFILE.items() if
+00007590: 206b 6579 203d 3d20 7365 6172 6368 6974   key == searchit
+000075a0: 656d 7d0a 2020 2020 2020 2020 2020 2020  em}.            
+000075b0: 6966 206e 6f74 2072 6573 756c 743a 0a20  if not result:. 
+000075c0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000075d0: 6f6e 7469 6e75 650a 2020 2020 2020 2020  ontinue.        
+000075e0: 2020 2020 6966 2072 6573 756c 742e 6765      if result.ge
+000075f0: 7428 7365 6172 6368 6974 656d 292e 6765  t(searchitem).ge
+00007600: 7428 2265 7861 6374 5f6d 6174 6368 2229  t("exact_match")
+00007610: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00007620: 2020 6966 2073 6561 7263 6869 7465 6d20    if searchitem 
+00007630: 3d3d 2063 616c 6c73 6967 6e3a 0a20 2020  == callsign:.   
+00007640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007650: 2072 6574 7572 6e20 7265 7375 6c74 0a20   return result. 
+00007660: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00007670: 6f6e 7469 6e75 650a 2020 2020 2020 2020  ontinue.        
+00007680: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+00007690: 740a 0a20 2020 2064 6566 2063 7773 7065  t..    def cwspe
+000076a0: 6564 5f73 7069 6e62 6f78 5f63 6861 6e67  ed_spinbox_chang
+000076b0: 6564 2873 656c 6629 3a0a 2020 2020 2020  ed(self):.      
+000076c0: 2020 2222 2274 7269 6767 6572 6564 2077    """triggered w
+000076d0: 6865 6e20 7661 6c75 6520 6f66 2043 5720  hen value of CW 
+000076e0: 7370 6565 6420 696e 2074 6865 2073 7069  speed in the spi
+000076f0: 6e62 6f78 2063 6861 6e67 6573 2e22 2222  nbox changes."""
+00007700: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00007710: 2e63 772e 7365 7276 6572 7479 7065 203d  .cw.servertype =
+00007720: 3d20 313a 0a20 2020 2020 2020 2020 2020  = 1:.           
+00007730: 2073 656c 662e 6377 2e73 7065 6564 203d   self.cw.speed =
+00007740: 2073 656c 662e 6377 5f73 7065 6564 2e76   self.cw_speed.v
+00007750: 616c 7565 2829 0a20 2020 2020 2020 2020  alue().         
+00007760: 2020 2073 656c 662e 6377 2e73 656e 6463     self.cw.sendc
+00007770: 7728 6622 5c78 3162 327b 7365 6c66 2e63  w(f"\x1b2{self.c
+00007780: 772e 7370 6565 647d 2229 0a20 2020 2020  w.speed}").     
+00007790: 2020 2069 6620 7365 6c66 2e63 772e 7365     if self.cw.se
+000077a0: 7276 6572 7479 7065 203d 3d20 323a 0a20  rvertype == 2:. 
+000077b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000077c0: 6377 2e73 6574 5f77 696e 6b65 7965 725f  cw.set_winkeyer_
+000077d0: 7370 6565 6428 7365 6c66 2e63 775f 7370  speed(self.cw_sp
+000077e0: 6565 642e 7661 6c75 6528 2929 0a0a 2020  eed.value())..  
+000077f0: 2020 6465 6620 6b65 7950 7265 7373 4576    def keyPressEv
+00007800: 656e 7428 7365 6c66 2c20 6576 656e 7429  ent(self, event)
+00007810: 3a20 2023 2070 796c 696e 743a 2064 6973  :  # pylint: dis
+00007820: 6162 6c65 3d69 6e76 616c 6964 2d6e 616d  able=invalid-nam
+00007830: 650a 2020 2020 2020 2020 2222 2254 6869  e.        """Thi
+00007840: 7320 6f76 6572 7269 6465 7320 5174 206b  s overrides Qt k
+00007850: 6579 2065 7665 6e74 2e22 2222 0a20 2020  ey event.""".   
+00007860: 2020 2020 206d 6f64 6966 6965 7220 3d20       modifier = 
+00007870: 6576 656e 742e 6d6f 6469 6669 6572 7328  event.modifiers(
+00007880: 290a 2020 2020 2020 2020 6966 2065 7665  ).        if eve
+00007890: 6e74 2e6b 6579 2829 203d 3d20 5174 2e4b  nt.key() == Qt.K
+000078a0: 6579 5f53 2061 6e64 206d 6f64 6966 6965  ey_S and modifie
+000078b0: 7220 3d3d 2051 742e 436f 6e74 726f 6c4d  r == Qt.ControlM
+000078c0: 6f64 6966 6965 723a 0a20 2020 2020 2020  odifier:.       
+000078d0: 2020 2020 2066 7265 7120 3d20 7365 6c66       freq = self
+000078e0: 2e72 6164 696f 5f73 7461 7465 2e67 6574  .radio_state.get
+000078f0: 2822 7666 6f61 2229 0a20 2020 2020 2020  ("vfoa").       
+00007900: 2020 2020 2064 7820 3d20 7365 6c66 2e63       dx = self.c
+00007910: 616c 6c73 6967 6e2e 7465 7874 2829 0a20  allsign.text(). 
+00007920: 2020 2020 2020 2020 2020 2069 6620 6672             if fr
+00007930: 6571 2061 6e64 2064 783a 0a20 2020 2020  eq and dx:.     
+00007940: 2020 2020 2020 2020 2020 2063 6d64 203d             cmd =
+00007950: 207b 7d0a 2020 2020 2020 2020 2020 2020   {}.            
+00007960: 2020 2020 636d 645b 2263 6d64 225d 203d      cmd["cmd"] =
+00007970: 2022 5350 4f54 4458 220a 2020 2020 2020   "SPOTDX".      
+00007980: 2020 2020 2020 2020 2020 636d 645b 2273            cmd["s
+00007990: 7461 7469 6f6e 225d 203d 2070 6c61 7466  tation"] = platf
+000079a0: 6f72 6d2e 6e6f 6465 2829 0a20 2020 2020  orm.node().     
+000079b0: 2020 2020 2020 2020 2020 2063 6d64 5b22             cmd["
+000079c0: 6478 225d 203d 2064 780a 2020 2020 2020  dx"] = dx.      
+000079d0: 2020 2020 2020 2020 2020 636d 645b 2266            cmd["f
+000079e0: 7265 7122 5d20 3d20 666c 6f61 7428 696e  req"] = float(in
+000079f0: 7428 6672 6571 2920 2f20 3130 3030 290a  t(freq) / 1000).
+00007a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a10: 7365 6c66 2e6d 756c 7469 6361 7374 5f69  self.multicast_i
+00007a20: 6e74 6572 6661 6365 2e73 656e 645f 6173  nterface.send_as
+00007a30: 5f6a 736f 6e28 636d 6429 0a20 2020 2020  _json(cmd).     
+00007a40: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+00007a50: 2020 2020 2020 6966 2065 7665 6e74 2e6b        if event.k
+00007a60: 6579 2829 203d 3d20 5174 2e4b 6579 5f47  ey() == Qt.Key_G
+00007a70: 2061 6e64 206d 6f64 6966 6965 7220 3d3d   and modifier ==
+00007a80: 2051 742e 436f 6e74 726f 6c4d 6f64 6966   Qt.ControlModif
+00007a90: 6965 723a 0a20 2020 2020 2020 2020 2020  ier:.           
+00007aa0: 2064 7820 3d20 7365 6c66 2e63 616c 6c73   dx = self.calls
+00007ab0: 6967 6e2e 7465 7874 2829 0a20 2020 2020  ign.text().     
+00007ac0: 2020 2020 2020 2069 6620 6478 3a0a 2020         if dx:.  
+00007ad0: 2020 2020 2020 2020 2020 2020 2020 636d                cm
+00007ae0: 6420 3d20 7b7d 0a20 2020 2020 2020 2020  d = {}.         
+00007af0: 2020 2020 2020 2063 6d64 5b22 636d 6422         cmd["cmd"
+00007b00: 5d20 3d20 2246 494e 4444 5822 0a20 2020  ] = "FINDDX".   
+00007b10: 2020 2020 2020 2020 2020 2020 2063 6d64               cmd
+00007b20: 5b22 7374 6174 696f 6e22 5d20 3d20 706c  ["station"] = pl
+00007b30: 6174 666f 726d 2e6e 6f64 6528 290a 2020  atform.node().  
+00007b40: 2020 2020 2020 2020 2020 2020 2020 636d                cm
+00007b50: 645b 2264 7822 5d20 3d20 6478 0a20 2020  d["dx"] = dx.   
+00007b60: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00007b70: 662e 6d75 6c74 6963 6173 745f 696e 7465  f.multicast_inte
+00007b80: 7266 6163 652e 7365 6e64 5f61 735f 6a73  rface.send_as_js
+00007b90: 6f6e 2863 6d64 290a 2020 2020 2020 2020  on(cmd).        
+00007ba0: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+00007bb0: 2020 2069 6620 280a 2020 2020 2020 2020     if (.        
+00007bc0: 2020 2020 6576 656e 742e 6b65 7928 2920      event.key() 
+00007bd0: 3d3d 2051 742e 4b65 792e 4b65 795f 4573  == Qt.Key.Key_Es
+00007be0: 6361 7065 2061 6e64 206d 6f64 6966 6965  cape and modifie
+00007bf0: 7220 213d 2051 742e 436f 6e74 726f 6c4d  r != Qt.ControlM
+00007c00: 6f64 6966 6965 720a 2020 2020 2020 2020  odifier.        
+00007c10: 293a 2020 2320 7079 6c69 6e74 3a20 6469  ):  # pylint: di
+00007c20: 7361 626c 653d 6e6f 2d6d 656d 6265 720a  sable=no-member.
+00007c30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00007c40: 2e63 6c65 6172 696e 7075 7473 2829 0a20  .clearinputs(). 
+00007c50: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00007c60: 6e0a 2020 2020 2020 2020 6966 2065 7665  n.        if eve
+00007c70: 6e74 2e6b 6579 2829 203d 3d20 5174 2e4b  nt.key() == Qt.K
+00007c80: 6579 2e4b 6579 5f45 7363 6170 6520 616e  ey.Key_Escape an
+00007c90: 6420 6d6f 6469 6669 6572 203d 3d20 5174  d modifier == Qt
+00007ca0: 2e43 6f6e 7472 6f6c 4d6f 6469 6669 6572  .ControlModifier
+00007cb0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00007cc0: 2073 656c 662e 6377 2069 7320 6e6f 7420   self.cw is not 
+00007cd0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00007ce0: 2020 2020 2020 6966 2073 656c 662e 6377        if self.cw
+00007cf0: 2e73 6572 7665 7274 7970 6520 3d3d 2031  .servertype == 1
+00007d00: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00007d10: 2020 2020 2020 7365 6c66 2e63 772e 7365        self.cw.se
+00007d20: 6e64 6377 2822 5c78 3162 3422 290a 2020  ndcw("\x1b4").  
+00007d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d40: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+00007d50: 2069 6620 6576 656e 742e 6b65 7928 2920   if event.key() 
+00007d60: 3d3d 2051 742e 4b65 792e 4b65 795f 5570  == Qt.Key.Key_Up
+00007d70: 3a0a 2020 2020 2020 2020 2020 2020 636d  :.            cm
+00007d80: 6420 3d20 7b7d 0a20 2020 2020 2020 2020  d = {}.         
+00007d90: 2020 2063 6d64 5b22 636d 6422 5d20 3d20     cmd["cmd"] = 
+00007da0: 2250 5245 5653 504f 5422 0a20 2020 2020  "PREVSPOT".     
+00007db0: 2020 2020 2020 2063 6d64 5b22 7374 6174         cmd["stat
+00007dc0: 696f 6e22 5d20 3d20 706c 6174 666f 726d  ion"] = platform
+00007dd0: 2e6e 6f64 6528 290a 2020 2020 2020 2020  .node().        
+00007de0: 2020 2020 7365 6c66 2e6d 756c 7469 6361      self.multica
+00007df0: 7374 5f69 6e74 6572 6661 6365 2e73 656e  st_interface.sen
+00007e00: 645f 6173 5f6a 736f 6e28 636d 6429 0a20  d_as_json(cmd). 
+00007e10: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00007e20: 6e0a 2020 2020 2020 2020 6966 2065 7665  n.        if eve
+00007e30: 6e74 2e6b 6579 2829 203d 3d20 5174 2e4b  nt.key() == Qt.K
+00007e40: 6579 2e4b 6579 5f44 6f77 6e3a 0a20 2020  ey.Key_Down:.   
+00007e50: 2020 2020 2020 2020 2063 6d64 203d 207b           cmd = {
+00007e60: 7d0a 2020 2020 2020 2020 2020 2020 636d  }.            cm
+00007e70: 645b 2263 6d64 225d 203d 2022 4e45 5854  d["cmd"] = "NEXT
+00007e80: 5350 4f54 220a 2020 2020 2020 2020 2020  SPOT".          
+00007e90: 2020 636d 645b 2273 7461 7469 6f6e 225d    cmd["station"]
+00007ea0: 203d 2070 6c61 7466 6f72 6d2e 6e6f 6465   = platform.node
+00007eb0: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
+00007ec0: 656c 662e 6d75 6c74 6963 6173 745f 696e  elf.multicast_in
+00007ed0: 7465 7266 6163 652e 7365 6e64 5f61 735f  terface.send_as_
+00007ee0: 6a73 6f6e 2863 6d64 290a 2020 2020 2020  json(cmd).      
+00007ef0: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
+00007f00: 2020 2020 2069 6620 6576 656e 742e 6b65       if event.ke
+00007f10: 7928 2920 3d3d 2051 742e 4b65 792e 4b65  y() == Qt.Key.Ke
+00007f20: 795f 5061 6765 5570 2061 6e64 206d 6f64  y_PageUp and mod
+00007f30: 6966 6965 7220 213d 2051 742e 436f 6e74  ifier != Qt.Cont
+00007f40: 726f 6c4d 6f64 6966 6965 723a 0a20 2020  rolModifier:.   
+00007f50: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00007f60: 2e63 7720 6973 206e 6f74 204e 6f6e 653a  .cw is not None:
+00007f70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007f80: 2073 656c 662e 6377 2e73 7065 6564 202b   self.cw.speed +
+00007f90: 3d20 310a 2020 2020 2020 2020 2020 2020  = 1.            
+00007fa0: 2020 2020 7365 6c66 2e63 775f 7370 6565      self.cw_spee
+00007fb0: 642e 7365 7456 616c 7565 2873 656c 662e  d.setValue(self.
+00007fc0: 6377 2e73 7065 6564 290a 2020 2020 2020  cw.speed).      
+00007fd0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00007fe0: 662e 6377 2e73 6572 7665 7274 7970 6520  f.cw.servertype 
+00007ff0: 3d3d 2031 3a0a 2020 2020 2020 2020 2020  == 1:.          
+00008000: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00008010: 772e 7365 6e64 6377 2866 225c 7831 6232  w.sendcw(f"\x1b2
+00008020: 7b73 656c 662e 6377 2e73 7065 6564 7d22  {self.cw.speed}"
+00008030: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00008040: 2020 6966 2073 656c 662e 6377 2e73 6572    if self.cw.ser
+00008050: 7665 7274 7970 6520 3d3d 2032 3a0a 2020  vertype == 2:.  
+00008060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008070: 2020 7365 6c66 2e63 772e 7365 745f 7769    self.cw.set_wi
+00008080: 6e6b 6579 6572 5f73 7065 6564 2873 656c  nkeyer_speed(sel
+00008090: 662e 6377 5f73 7065 6564 2e76 616c 7565  f.cw_speed.value
+000080a0: 2829 290a 2020 2020 2020 2020 2020 2020  ()).            
+000080b0: 7265 7475 726e 0a20 2020 2020 2020 2069  return.        i
+000080c0: 6620 6576 656e 742e 6b65 7928 2920 3d3d  f event.key() ==
+000080d0: 2051 742e 4b65 792e 4b65 795f 5061 6765   Qt.Key.Key_Page
+000080e0: 446f 776e 2061 6e64 206d 6f64 6966 6965  Down and modifie
+000080f0: 7220 213d 2051 742e 436f 6e74 726f 6c4d  r != Qt.ControlM
+00008100: 6f64 6966 6965 723a 0a20 2020 2020 2020  odifier:.       
+00008110: 2020 2020 2069 6620 7365 6c66 2e63 7720       if self.cw 
+00008120: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00008130: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00008140: 662e 6377 2e73 7065 6564 202d 3d20 310a  f.cw.speed -= 1.
+00008150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008160: 7365 6c66 2e63 775f 7370 6565 642e 7365  self.cw_speed.se
+00008170: 7456 616c 7565 2873 656c 662e 6377 2e73  tValue(self.cw.s
+00008180: 7065 6564 290a 2020 2020 2020 2020 2020  peed).          
+00008190: 2020 2020 2020 6966 2073 656c 662e 6377        if self.cw
+000081a0: 2e73 6572 7665 7274 7970 6520 3d3d 2031  .servertype == 1
+000081b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000081c0: 2020 2020 2020 7365 6c66 2e63 772e 7365        self.cw.se
+000081d0: 6e64 6377 2866 225c 7831 6232 7b73 656c  ndcw(f"\x1b2{sel
+000081e0: 662e 6377 2e73 7065 6564 7d22 290a 2020  f.cw.speed}").  
+000081f0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00008200: 2073 656c 662e 6377 2e73 6572 7665 7274   self.cw.servert
+00008210: 7970 6520 3d3d 2032 3a0a 2020 2020 2020  ype == 2:.      
+00008220: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00008230: 6c66 2e63 772e 7365 745f 7769 6e6b 6579  lf.cw.set_winkey
+00008240: 6572 5f73 7065 6564 2873 656c 662e 6377  er_speed(self.cw
+00008250: 5f73 7065 6564 2e76 616c 7565 2829 290a  _speed.value()).
+00008260: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00008270: 726e 0a20 2020 2020 2020 2023 2069 6620  rn.        # if 
+00008280: 6576 656e 742e 6b65 7928 2920 3d3d 2051  event.key() == Q
+00008290: 742e 4b65 792e 4b65 795f 456e 7465 723a  t.Key.Key_Enter:
+000082a0: 0a20 2020 2020 2020 2023 2020 2020 2073  .        #     s
+000082b0: 656c 662e 7361 7665 5f63 6f6e 7461 6374  elf.save_contact
+000082c0: 2829 0a20 2020 2020 2020 2069 6620 6576  ().        if ev
+000082d0: 656e 742e 6b65 7928 2920 3d3d 2051 742e  ent.key() == Qt.
+000082e0: 4b65 792e 4b65 795f 5461 6220 6f72 2065  Key.Key_Tab or e
+000082f0: 7665 6e74 2e6b 6579 2829 203d 3d20 5174  vent.key() == Qt
+00008300: 2e4b 6579 2e4b 6579 5f42 6163 6b74 6162  .Key.Key_Backtab
+00008310: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00008320: 2073 656c 662e 7365 6e74 2e68 6173 466f   self.sent.hasFo
+00008330: 6375 7328 293a 0a20 2020 2020 2020 2020  cus():.         
+00008340: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
+00008350: 6275 6728 2246 726f 6d20 7365 6e74 2229  bug("From sent")
+00008360: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008370: 2069 6620 6d6f 6469 6669 6572 203d 3d20   if modifier == 
+00008380: 5174 2e53 6869 6674 4d6f 6469 6669 6572  Qt.ShiftModifier
+00008390: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000083a0: 2020 2020 2020 7072 6576 5f74 6162 203d        prev_tab =
+000083b0: 2073 656c 662e 7461 625f 7072 6576 2e67   self.tab_prev.g
+000083c0: 6574 2873 656c 662e 7365 6e74 290a 2020  et(self.sent).  
+000083d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000083e0: 2020 7072 6576 5f74 6162 2e73 6574 466f    prev_tab.setFo
+000083f0: 6375 7328 290a 2020 2020 2020 2020 2020  cus().          
+00008400: 2020 2020 2020 2020 2020 7072 6576 5f74            prev_t
+00008410: 6162 2e64 6573 656c 6563 7428 290a 2020  ab.deselect().  
+00008420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008430: 2020 7072 6576 5f74 6162 2e65 6e64 2846    prev_tab.end(F
+00008440: 616c 7365 290a 2020 2020 2020 2020 2020  alse).          
+00008450: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00008460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008470: 6e65 7874 5f74 6162 203d 2073 656c 662e  next_tab = self.
+00008480: 7461 625f 6e65 7874 2e67 6574 2873 656c  tab_next.get(sel
+00008490: 662e 7365 6e74 290a 2020 2020 2020 2020  f.sent).        
+000084a0: 2020 2020 2020 2020 2020 2020 6e65 7874              next
+000084b0: 5f74 6162 2e73 6574 466f 6375 7328 290a  _tab.setFocus().
+000084c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000084d0: 2020 2020 6e65 7874 5f74 6162 2e64 6573      next_tab.des
+000084e0: 656c 6563 7428 290a 2020 2020 2020 2020  elect().        
+000084f0: 2020 2020 2020 2020 2020 2020 6e65 7874              next
+00008500: 5f74 6162 2e65 6e64 2846 616c 7365 290a  _tab.end(False).
+00008510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008520: 7265 7475 726e 0a20 2020 2020 2020 2020  return.         
+00008530: 2020 2069 6620 7365 6c66 2e72 6563 6569     if self.recei
+00008540: 7665 2e68 6173 466f 6375 7328 293a 0a20  ve.hasFocus():. 
+00008550: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00008560: 6f67 6765 722e 6465 6275 6728 2246 726f  ogger.debug("Fro
+00008570: 6d20 7265 6365 6976 6522 290a 2020 2020  m receive").    
+00008580: 2020 2020 2020 2020 2020 2020 6966 206d              if m
+00008590: 6f64 6966 6965 7220 3d3d 2051 742e 5368  odifier == Qt.Sh
+000085a0: 6966 744d 6f64 6966 6965 723a 0a20 2020  iftModifier:.   
+000085b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000085c0: 2070 7265 765f 7461 6220 3d20 7365 6c66   prev_tab = self
+000085d0: 2e74 6162 5f70 7265 762e 6765 7428 7365  .tab_prev.get(se
+000085e0: 6c66 2e72 6563 6569 7665 290a 2020 2020  lf.receive).    
+000085f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008600: 7072 6576 5f74 6162 2e73 6574 466f 6375  prev_tab.setFocu
+00008610: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
+00008620: 2020 2020 2020 2020 7072 6576 5f74 6162          prev_tab
+00008630: 2e64 6573 656c 6563 7428 290a 2020 2020  .deselect().    
+00008640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008650: 7072 6576 5f74 6162 2e65 6e64 2846 616c  prev_tab.end(Fal
+00008660: 7365 290a 2020 2020 2020 2020 2020 2020  se).            
+00008670: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00008680: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
+00008690: 7874 5f74 6162 203d 2073 656c 662e 7461  xt_tab = self.ta
+000086a0: 625f 6e65 7874 2e67 6574 2873 656c 662e  b_next.get(self.
+000086b0: 7265 6365 6976 6529 0a20 2020 2020 2020  receive).       
+000086c0: 2020 2020 2020 2020 2020 2020 206e 6578               nex
+000086d0: 745f 7461 622e 7365 7446 6f63 7573 2829  t_tab.setFocus()
+000086e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000086f0: 2020 2020 206e 6578 745f 7461 622e 6465       next_tab.de
+00008700: 7365 6c65 6374 2829 0a20 2020 2020 2020  select().       
+00008710: 2020 2020 2020 2020 2020 2020 206e 6578               nex
+00008720: 745f 7461 622e 656e 6428 4661 6c73 6529  t_tab.end(False)
+00008730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008740: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
+00008750: 2020 2020 6966 2073 656c 662e 6f74 6865      if self.othe
+00008760: 725f 312e 6861 7346 6f63 7573 2829 3a0a  r_1.hasFocus():.
+00008770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008780: 6c6f 6767 6572 2e64 6562 7567 2822 4672  logger.debug("Fr
+00008790: 6f6d 206f 7468 6572 5f31 2229 0a20 2020  om other_1").   
+000087a0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000087b0: 6d6f 6469 6669 6572 203d 3d20 5174 2e53  modifier == Qt.S
+000087c0: 6869 6674 4d6f 6469 6669 6572 3a0a 2020  hiftModifier:.  
+000087d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000087e0: 2020 7072 6576 5f74 6162 203d 2073 656c    prev_tab = sel
+000087f0: 662e 7461 625f 7072 6576 2e67 6574 2873  f.tab_prev.get(s
+00008800: 656c 662e 6f74 6865 725f 3129 0a20 2020  elf.other_1).   
+00008810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008820: 2070 7265 765f 7461 622e 7365 7446 6f63   prev_tab.setFoc
+00008830: 7573 2829 0a20 2020 2020 2020 2020 2020  us().           
+00008840: 2020 2020 2020 2020 2070 7265 765f 7461           prev_ta
+00008850: 622e 6465 7365 6c65 6374 2829 0a20 2020  b.deselect().   
+00008860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008870: 2070 7265 765f 7461 622e 656e 6428 4661   prev_tab.end(Fa
+00008880: 6c73 6529 0a20 2020 2020 2020 2020 2020  lse).           
+00008890: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+000088a0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+000088b0: 6578 745f 7461 6220 3d20 7365 6c66 2e74  ext_tab = self.t
+000088c0: 6162 5f6e 6578 742e 6765 7428 7365 6c66  ab_next.get(self
+000088d0: 2e6f 7468 6572 5f31 290a 2020 2020 2020  .other_1).      
+000088e0: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
+000088f0: 7874 5f74 6162 2e73 6574 466f 6375 7328  xt_tab.setFocus(
+00008900: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00008910: 2020 2020 2020 6e65 7874 5f74 6162 2e64        next_tab.d
+00008920: 6573 656c 6563 7428 290a 2020 2020 2020  eselect().      
+00008930: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
+00008940: 7874 5f74 6162 2e65 6e64 2846 616c 7365  xt_tab.end(False
+00008950: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00008960: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+00008970: 2020 2020 2069 6620 7365 6c66 2e6f 7468       if self.oth
+00008980: 6572 5f32 2e68 6173 466f 6375 7328 293a  er_2.hasFocus():
+00008990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000089a0: 206c 6f67 6765 722e 6465 6275 6728 2246   logger.debug("F
+000089b0: 726f 6d20 6f74 6865 725f 3222 290a 2020  rom other_2").  
+000089c0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000089d0: 206d 6f64 6966 6965 7220 3d3d 2051 742e   modifier == Qt.
+000089e0: 5368 6966 744d 6f64 6966 6965 723a 0a20  ShiftModifier:. 
+000089f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a00: 2020 2070 7265 765f 7461 6220 3d20 7365     prev_tab = se
+00008a10: 6c66 2e74 6162 5f70 7265 762e 6765 7428  lf.tab_prev.get(
+00008a20: 7365 6c66 2e6f 7468 6572 5f32 290a 2020  self.other_2).  
+00008a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a40: 2020 7072 6576 5f74 6162 2e73 6574 466f    prev_tab.setFo
+00008a50: 6375 7328 290a 2020 2020 2020 2020 2020  cus().          
+00008a60: 2020 2020 2020 2020 2020 7072 6576 5f74            prev_t
+00008a70: 6162 2e64 6573 656c 6563 7428 290a 2020  ab.deselect().  
+00008a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a90: 2020 7072 6576 5f74 6162 2e65 6e64 2846    prev_tab.end(F
+00008aa0: 616c 7365 290a 2020 2020 2020 2020 2020  alse).          
+00008ab0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00008ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ad0: 6e65 7874 5f74 6162 203d 2073 656c 662e  next_tab = self.
+00008ae0: 7461 625f 6e65 7874 2e67 6574 2873 656c  tab_next.get(sel
+00008af0: 662e 6f74 6865 725f 3229 0a20 2020 2020  f.other_2).     
+00008b00: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00008b10: 6578 745f 7461 622e 7365 7446 6f63 7573  ext_tab.setFocus
+00008b20: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00008b30: 2020 2020 2020 206e 6578 745f 7461 622e         next_tab.
+00008b40: 6465 7365 6c65 6374 2829 0a20 2020 2020  deselect().     
+00008b50: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00008b60: 6578 745f 7461 622e 656e 6428 4661 6c73  ext_tab.end(Fals
+00008b70: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+00008b80: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
+00008b90: 2020 2020 2020 6966 2073 656c 662e 6361        if self.ca
+00008ba0: 6c6c 7369 676e 2e68 6173 466f 6375 7328  llsign.hasFocus(
+00008bb0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00008bc0: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+00008bd0: 2246 726f 6d20 6361 6c6c 7369 676e 2229  "From callsign")
+00008be0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008bf0: 2073 656c 662e 6368 6563 6b5f 6361 6c6c   self.check_call
+00008c00: 7369 676e 2873 656c 662e 6361 6c6c 7369  sign(self.callsi
+00008c10: 676e 2e74 6578 7428 2929 0a20 2020 2020  gn.text()).     
+00008c20: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00008c30: 6c66 2e63 6865 636b 5f64 7570 6528 7365  lf.check_dupe(se
+00008c40: 6c66 2e63 616c 6c73 6967 6e2e 7465 7874  lf.callsign.text
+00008c50: 2829 293a 0a20 2020 2020 2020 2020 2020  ()):.           
+00008c60: 2020 2020 2020 2020 2073 656c 662e 6475           self.du
+00008c70: 7065 5f69 6e64 6963 6174 6f72 2e73 686f  pe_indicator.sho
+00008c80: 7728 290a 2020 2020 2020 2020 2020 2020  w().            
+00008c90: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00008ca0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00008cb0: 6c66 2e64 7570 655f 696e 6469 6361 746f  lf.dupe_indicato
+00008cc0: 722e 6869 6465 2829 0a20 2020 2020 2020  r.hide().       
+00008cd0: 2020 2020 2020 2020 2069 6620 6d6f 6469           if modi
+00008ce0: 6669 6572 203d 3d20 5174 2e53 6869 6674  fier == Qt.Shift
+00008cf0: 4d6f 6469 6669 6572 3a0a 2020 2020 2020  Modifier:.      
+00008d00: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00008d10: 6576 5f74 6162 203d 2073 656c 662e 7461  ev_tab = self.ta
+00008d20: 625f 7072 6576 2e67 6574 2873 656c 662e  b_prev.get(self.
+00008d30: 6361 6c6c 7369 676e 290a 2020 2020 2020  callsign).      
+00008d40: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00008d50: 6576 5f74 6162 2e73 6574 466f 6375 7328  ev_tab.setFocus(
+00008d60: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00008d70: 2020 2020 2020 7072 6576 5f74 6162 2e64        prev_tab.d
+00008d80: 6573 656c 6563 7428 290a 2020 2020 2020  eselect().      
+00008d90: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00008da0: 6576 5f74 6162 2e65 6e64 2846 616c 7365  ev_tab.end(False
+00008db0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00008dc0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00008dd0: 2020 2020 2020 2020 2020 2020 7465 7874              text
+00008de0: 203d 2073 656c 662e 6361 6c6c 7369 676e   = self.callsign
+00008df0: 2e74 6578 7428 290a 2020 2020 2020 2020  .text().        
+00008e00: 2020 2020 2020 2020 2020 2020 7465 7874              text
+00008e10: 203d 2074 6578 742e 7570 7065 7228 290a   = text.upper().
+00008e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e30: 2020 2020 5f74 6865 7468 7265 6164 203d      _thethread =
+00008e40: 2074 6872 6561 6469 6e67 2e54 6872 6561   threading.Threa
+00008e50: 6428 0a20 2020 2020 2020 2020 2020 2020  d(.             
+00008e60: 2020 2020 2020 2020 2020 2074 6172 6765             targe
+00008e70: 743d 7365 6c66 2e63 6865 636b 5f63 616c  t=self.check_cal
+00008e80: 6c73 6967 6e32 2c0a 2020 2020 2020 2020  lsign2,.        
+00008e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ea0: 6172 6773 3d28 7465 7874 2c29 2c0a 2020  args=(text,),.  
+00008eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ec0: 2020 2020 2020 6461 656d 6f6e 3d54 7275        daemon=Tru
+00008ed0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00008ee0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00008ef0: 2020 2020 2020 2020 2020 2020 205f 7468               _th
+00008f00: 6574 6872 6561 642e 7374 6172 7428 290a  ethread.start().
+00008f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f20: 2020 2020 6e65 7874 5f74 6162 203d 2073      next_tab = s
+00008f30: 656c 662e 7461 625f 6e65 7874 2e67 6574  elf.tab_next.get
+00008f40: 2873 656c 662e 6361 6c6c 7369 676e 290a  (self.callsign).
+00008f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f60: 2020 2020 6e65 7874 5f74 6162 2e73 6574      next_tab.set
+00008f70: 466f 6375 7328 290a 2020 2020 2020 2020  Focus().        
+00008f80: 2020 2020 2020 2020 2020 2020 6e65 7874              next
+00008f90: 5f74 6162 2e64 6573 656c 6563 7428 290a  _tab.deselect().
+00008fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008fb0: 2020 2020 6e65 7874 5f74 6162 2e65 6e64      next_tab.end
+00008fc0: 2846 616c 7365 290a 2020 2020 2020 2020  (False).        
+00008fd0: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+00008fe0: 2020 2020 2020 2069 6620 6576 656e 742e         if event.
+00008ff0: 6b65 7928 2920 3d3d 2051 742e 4b65 795f  key() == Qt.Key_
+00009000: 4631 3a0a 2020 2020 2020 2020 2020 2020  F1:.            
+00009010: 7365 6c66 2e73 656e 6466 3128 290a 2020  self.sendf1().  
+00009020: 2020 2020 2020 6966 2065 7665 6e74 2e6b        if event.k
+00009030: 6579 2829 203d 3d20 5174 2e4b 6579 5f46  ey() == Qt.Key_F
+00009040: 323a 0a20 2020 2020 2020 2020 2020 2073  2:.            s
+00009050: 656c 662e 7365 6e64 6632 2829 0a20 2020  elf.sendf2().   
+00009060: 2020 2020 2069 6620 6576 656e 742e 6b65       if event.ke
+00009070: 7928 2920 3d3d 2051 742e 4b65 795f 4633  y() == Qt.Key_F3
+00009080: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00009090: 6c66 2e73 656e 6466 3328 290a 2020 2020  lf.sendf3().    
+000090a0: 2020 2020 6966 2065 7665 6e74 2e6b 6579      if event.key
+000090b0: 2829 203d 3d20 5174 2e4b 6579 5f46 343a  () == Qt.Key_F4:
+000090c0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000090d0: 662e 7365 6e64 6634 2829 0a20 2020 2020  f.sendf4().     
+000090e0: 2020 2069 6620 6576 656e 742e 6b65 7928     if event.key(
+000090f0: 2920 3d3d 2051 742e 4b65 795f 4635 3a0a  ) == Qt.Key_F5:.
+00009100: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00009110: 2e73 656e 6466 3528 290a 2020 2020 2020  .sendf5().      
+00009120: 2020 6966 2065 7665 6e74 2e6b 6579 2829    if event.key()
+00009130: 203d 3d20 5174 2e4b 6579 5f46 363a 0a20   == Qt.Key_F6:. 
+00009140: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00009150: 7365 6e64 6636 2829 0a20 2020 2020 2020  sendf6().       
+00009160: 2069 6620 6576 656e 742e 6b65 7928 2920   if event.key() 
+00009170: 3d3d 2051 742e 4b65 795f 4637 3a0a 2020  == Qt.Key_F7:.  
+00009180: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00009190: 656e 6466 3728 290a 2020 2020 2020 2020  endf7().        
+000091a0: 6966 2065 7665 6e74 2e6b 6579 2829 203d  if event.key() =
+000091b0: 3d20 5174 2e4b 6579 5f46 383a 0a20 2020  = Qt.Key_F8:.   
+000091c0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+000091d0: 6e64 6638 2829 0a20 2020 2020 2020 2069  ndf8().        i
+000091e0: 6620 6576 656e 742e 6b65 7928 2920 3d3d  f event.key() ==
+000091f0: 2051 742e 4b65 795f 4639 3a0a 2020 2020   Qt.Key_F9:.    
+00009200: 2020 2020 2020 2020 7365 6c66 2e73 656e          self.sen
+00009210: 6466 3928 290a 2020 2020 2020 2020 6966  df9().        if
+00009220: 2065 7665 6e74 2e6b 6579 2829 203d 3d20   event.key() == 
+00009230: 5174 2e4b 6579 5f46 3130 3a0a 2020 2020  Qt.Key_F10:.    
+00009240: 2020 2020 2020 2020 7365 6c66 2e73 656e          self.sen
+00009250: 6466 3130 2829 0a20 2020 2020 2020 2069  df10().        i
+00009260: 6620 6576 656e 742e 6b65 7928 2920 3d3d  f event.key() ==
+00009270: 2051 742e 4b65 795f 4631 313a 0a20 2020   Qt.Key_F11:.   
+00009280: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+00009290: 6e64 6631 3128 290a 2020 2020 2020 2020  ndf11().        
+000092a0: 6966 2065 7665 6e74 2e6b 6579 2829 203d  if event.key() =
+000092b0: 3d20 5174 2e4b 6579 5f46 3132 3a0a 2020  = Qt.Key_F12:.  
+000092c0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+000092d0: 656e 6466 3132 2829 0a0a 2020 2020 6465  endf12()..    de
+000092e0: 6620 7365 745f 7769 6e64 6f77 5f74 6974  f set_window_tit
+000092f0: 6c65 2873 656c 6629 3a0a 2020 2020 2020  le(self):.      
+00009300: 2020 2222 2253 6574 2077 696e 646f 7720    """Set window 
+00009310: 7469 746c 6522 2222 0a20 2020 2020 2020  title""".       
+00009320: 2076 666f 6120 3d20 7365 6c66 2e72 6164   vfoa = self.rad
+00009330: 696f 5f73 7461 7465 2e67 6574 2822 7666  io_state.get("vf
+00009340: 6f61 222c 2022 2229 0a20 2020 2020 2020  oa", "").       
+00009350: 2069 6620 7666 6f61 3a0a 2020 2020 2020   if vfoa:.      
+00009360: 2020 2020 2020 7666 6f61 203d 2069 6e74        vfoa = int
+00009370: 2876 666f 6129 202f 2031 3030 300a 2020  (vfoa) / 1000.  
+00009380: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00009390: 2020 2020 2020 2020 7666 6f61 203d 2030          vfoa = 0
+000093a0: 2e30 0a20 2020 2020 2020 2063 6f6e 7465  .0.        conte
+000093b0: 7374 5f6e 616d 6520 3d20 2222 0a20 2020  st_name = "".   
+000093c0: 2020 2020 2069 6620 7365 6c66 2e63 6f6e       if self.con
+000093d0: 7465 7374 3a0a 2020 2020 2020 2020 2020  test:.          
+000093e0: 2020 636f 6e74 6573 745f 6e61 6d65 203d    contest_name =
+000093f0: 2073 656c 662e 636f 6e74 6573 742e 6e61   self.contest.na
+00009400: 6d65 0a20 2020 2020 2020 206c 696e 6520  me.        line 
+00009410: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+00009420: 6622 7666 6f61 3a7b 726f 756e 6428 7666  f"vfoa:{round(vf
+00009430: 6f61 2c32 297d 2022 0a20 2020 2020 2020  oa,2)} ".       
+00009440: 2020 2020 2066 226d 6f64 653a 7b73 656c       f"mode:{sel
+00009450: 662e 7261 6469 6f5f 7374 6174 652e 6765  f.radio_state.ge
+00009460: 7428 276d 6f64 6527 2c20 2727 297d 2022  t('mode', '')} "
+00009470: 0a20 2020 2020 2020 2020 2020 2066 224f  .            f"O
+00009480: 503a 7b73 656c 662e 6375 7272 656e 745f  P:{self.current_
+00009490: 6f70 7d20 7b63 6f6e 7465 7374 5f6e 616d  op} {contest_nam
+000094a0: 657d 2022 0a20 2020 2020 2020 2020 2020  e} ".           
+000094b0: 2066 222d 204e 6f74 314d 4d20 767b 5f5f   f"- Not1MM v{__
+000094c0: 7665 7273 696f 6e5f 5f7d 220a 2020 2020  version__}".    
+000094d0: 2020 2020 290a 2020 2020 2020 2020 7365      ).        se
+000094e0: 6c66 2e73 6574 5769 6e64 6f77 5469 746c  lf.setWindowTitl
+000094f0: 6528 6c69 6e65 290a 0a20 2020 2064 6566  e(line)..    def
+00009500: 2063 6c65 6172 696e 7075 7473 2873 656c   clearinputs(sel
+00009510: 6629 3a0a 2020 2020 2020 2020 2222 2243  f):.        """C
+00009520: 6c65 6172 7320 7468 6520 7465 7874 2069  lears the text i
+00009530: 6e70 7574 2066 6965 6c64 7320 616e 6420  nput fields and 
+00009540: 7365 7473 2066 6f63 7573 2074 6f20 6361  sets focus to ca
+00009550: 6c6c 7369 676e 2066 6965 6c64 2e22 2222  llsign field."""
+00009560: 0a20 2020 2020 2020 2073 656c 662e 6475  .        self.du
+00009570: 7065 5f69 6e64 6963 6174 6f72 2e68 6964  pe_indicator.hid
+00009580: 6528 290a 2020 2020 2020 2020 7365 6c66  e().        self
+00009590: 2e63 6f6e 7461 6374 203d 2073 656c 662e  .contact = self.
+000095a0: 6461 7461 6261 7365 2e65 6d70 7479 5f63  database.empty_c
+000095b0: 6f6e 7461 6374 0a20 2020 2020 2020 2073  ontact.        s
+000095c0: 656c 662e 6865 6164 696e 675f 6469 7374  elf.heading_dist
+000095d0: 616e 6365 2e73 6574 5465 7874 2822 2229  ance.setText("")
+000095e0: 0a20 2020 2020 2020 2073 656c 662e 6478  .        self.dx
+000095f0: 5f65 6e74 6974 792e 7365 7454 6578 7428  _entity.setText(
+00009600: 2222 290a 2020 2020 2020 2020 6966 2073  "").        if s
+00009610: 656c 662e 636f 6e74 6573 743a 0a20 2020  elf.contest:.   
+00009620: 2020 2020 2020 2020 206d 756c 7473 203d           mults =
+00009630: 2073 656c 662e 636f 6e74 6573 742e 7368   self.contest.sh
+00009640: 6f77 5f6d 756c 7473 2873 656c 6629 0a20  ow_mults(self). 
+00009650: 2020 2020 2020 2020 2020 2071 736f 7320             qsos 
+00009660: 3d20 7365 6c66 2e63 6f6e 7465 7374 2e73  = self.contest.s
+00009670: 686f 775f 7173 6f28 7365 6c66 290a 2020  how_qso(self).  
+00009680: 2020 2020 2020 2020 2020 6d75 6c74 7374            multst
+00009690: 7269 6e67 203d 2066 227b 7173 6f73 7d2f  ring = f"{qsos}/
+000096a0: 7b6d 756c 7473 7d22 0a20 2020 2020 2020  {mults}".       
+000096b0: 2020 2020 2073 656c 662e 6d75 6c74 732e       self.mults.
+000096c0: 7365 7454 6578 7428 6d75 6c74 7374 7269  setText(multstri
+000096d0: 6e67 290a 2020 2020 2020 2020 2020 2020  ng).            
+000096e0: 7363 6f72 6520 3d20 7365 6c66 2e63 6f6e  score = self.con
+000096f0: 7465 7374 2e63 616c 635f 7363 6f72 6528  test.calc_score(
+00009700: 7365 6c66 290a 2020 2020 2020 2020 2020  self).          
+00009710: 2020 7365 6c66 2e73 636f 7265 2e73 6574    self.score.set
+00009720: 5465 7874 2873 7472 2873 636f 7265 2929  Text(str(score))
+00009730: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00009740: 662e 636f 6e74 6573 742e 7265 7365 745f  f.contest.reset_
+00009750: 6c61 6265 6c28 7365 6c66 290a 2020 2020  label(self).    
+00009760: 2020 2020 7365 6c66 2e63 616c 6c73 6967      self.callsig
+00009770: 6e2e 636c 6561 7228 290a 2020 2020 2020  n.clear().      
+00009780: 2020 6966 2073 656c 662e 6375 7272 656e    if self.curren
+00009790: 745f 6d6f 6465 203d 3d20 2243 5722 3a0a  t_mode == "CW":.
+000097a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000097b0: 2e73 656e 742e 7365 7454 6578 7428 2235  .sent.setText("5
+000097c0: 3939 2229 0a20 2020 2020 2020 2020 2020  99").           
+000097d0: 2073 656c 662e 7265 6365 6976 652e 7365   self.receive.se
+000097e0: 7454 6578 7428 2235 3939 2229 0a20 2020  tText("599").   
+000097f0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00009800: 2020 2020 2020 2073 656c 662e 7365 6e74         self.sent
+00009810: 2e73 6574 5465 7874 2822 3539 2229 0a20  .setText("59"). 
+00009820: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00009830: 7265 6365 6976 652e 7365 7454 6578 7428  receive.setText(
+00009840: 2235 3922 290a 2020 2020 2020 2020 7365  "59").        se
+00009850: 6c66 2e6f 7468 6572 5f31 2e63 6c65 6172  lf.other_1.clear
+00009860: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+00009870: 6f74 6865 725f 322e 636c 6561 7228 290a  other_2.clear().
+00009880: 2020 2020 2020 2020 7365 6c66 2e63 616c          self.cal
+00009890: 6c73 6967 6e2e 7365 7446 6f63 7573 2829  lsign.setFocus()
+000098a0: 0a20 2020 2020 2020 2063 6d64 203d 207b  .        cmd = {
+000098b0: 7d0a 2020 2020 2020 2020 636d 645b 2263  }.        cmd["c
+000098c0: 6d64 225d 203d 2022 4341 4c4c 4348 414e  md"] = "CALLCHAN
+000098d0: 4745 4422 0a20 2020 2020 2020 2063 6d64  GED".        cmd
+000098e0: 5b22 7374 6174 696f 6e22 5d20 3d20 706c  ["station"] = pl
+000098f0: 6174 666f 726d 2e6e 6f64 6528 290a 2020  atform.node().  
+00009900: 2020 2020 2020 636d 645b 2263 616c 6c22        cmd["call"
+00009910: 5d20 3d20 2222 0a20 2020 2020 2020 2073  ] = "".        s
+00009920: 656c 662e 6d75 6c74 6963 6173 745f 696e  elf.multicast_in
+00009930: 7465 7266 6163 652e 7365 6e64 5f61 735f  terface.send_as_
+00009940: 6a73 6f6e 2863 6d64 290a 0a20 2020 2064  json(cmd)..    d
+00009950: 6566 2073 6176 655f 636f 6e74 6163 7428  ef save_contact(
+00009960: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+00009970: 2222 5361 7665 2074 6f20 6462 2222 220a  ""Save to db""".
+00009980: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+00009990: 6562 7567 2822 7361 7669 6e67 2063 6f6e  ebug("saving con
+000099a0: 7461 6374 2229 0a20 2020 2020 2020 2069  tact").        i
+000099b0: 6620 6c65 6e28 7365 6c66 2e63 616c 6c73  f len(self.calls
+000099c0: 6967 6e2e 7465 7874 2829 2920 3c20 333a  ign.text()) < 3:
+000099d0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000099e0: 7572 6e0a 2020 2020 2020 2020 6966 206e  urn.        if n
+000099f0: 6f74 2061 6e79 2863 6861 722e 6973 6469  ot any(char.isdi
+00009a00: 6769 7428 2920 666f 7220 6368 6172 2069  git() for char i
+00009a10: 6e20 7365 6c66 2e63 616c 6c73 6967 6e2e  n self.callsign.
+00009a20: 7465 7874 2829 293a 0a20 2020 2020 2020  text()):.       
+00009a30: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+00009a40: 2020 2020 6966 206e 6f74 2061 6e79 2863      if not any(c
+00009a50: 6861 722e 6973 616c 7068 6128 2920 666f  har.isalpha() fo
+00009a60: 7220 6368 6172 2069 6e20 7365 6c66 2e63  r char in self.c
+00009a70: 616c 6c73 6967 6e2e 7465 7874 2829 293a  allsign.text()):
+00009a80: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00009a90: 7572 6e0a 0a20 2020 2020 2020 2073 656c  urn..        sel
+00009aa0: 662e 636f 6e74 6163 745b 2254 5322 5d20  f.contact["TS"] 
+00009ab0: 3d20 6461 7465 7469 6d65 2e75 7463 6e6f  = datetime.utcno
+00009ac0: 7728 292e 6973 6f66 6f72 6d61 7428 2220  w().isoformat(" 
+00009ad0: 2229 5b3a 3139 5d0a 2020 2020 2020 2020  ")[:19].        
+00009ae0: 7365 6c66 2e63 6f6e 7461 6374 5b22 4361  self.contact["Ca
+00009af0: 6c6c 225d 203d 2073 656c 662e 6361 6c6c  ll"] = self.call
+00009b00: 7369 676e 2e74 6578 7428 290a 2020 2020  sign.text().    
+00009b10: 2020 2020 7365 6c66 2e63 6f6e 7461 6374      self.contact
+00009b20: 5b22 4672 6571 225d 203d 2072 6f75 6e64  ["Freq"] = round
+00009b30: 2866 6c6f 6174 2873 656c 662e 7261 6469  (float(self.radi
+00009b40: 6f5f 7374 6174 652e 6765 7428 2276 666f  o_state.get("vfo
+00009b50: 6122 2c20 302e 3029 2920 2f20 3130 3030  a", 0.0)) / 1000
+00009b60: 2c20 3229 0a20 2020 2020 2020 2073 656c  , 2).        sel
+00009b70: 662e 636f 6e74 6163 745b 2251 5358 4672  f.contact["QSXFr
+00009b80: 6571 225d 203d 2072 6f75 6e64 280a 2020  eq"] = round(.  
+00009b90: 2020 2020 2020 2020 2020 666c 6f61 7428            float(
+00009ba0: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
+00009bb0: 2e67 6574 2822 7666 6f61 222c 2030 2e30  .get("vfoa", 0.0
+00009bc0: 2929 202f 2031 3030 302c 2032 0a20 2020  )) / 1000, 2.   
+00009bd0: 2020 2020 2029 0a20 2020 2020 2020 2073       ).        s
+00009be0: 656c 662e 636f 6e74 6163 745b 224d 6f64  elf.contact["Mod
+00009bf0: 6522 5d20 3d20 7365 6c66 2e72 6164 696f  e"] = self.radio
+00009c00: 5f73 7461 7465 2e67 6574 2822 6d6f 6465  _state.get("mode
+00009c10: 222c 2022 2229 0a20 2020 2020 2020 2073  ", "").        s
+00009c20: 656c 662e 636f 6e74 6163 745b 2243 6f6e  elf.contact["Con
+00009c30: 7465 7374 4e61 6d65 225d 203d 2073 656c  testName"] = sel
+00009c40: 662e 636f 6e74 6573 742e 6361 6272 696c  f.contest.cabril
+00009c50: 6c6f 5f6e 616d 650a 2020 2020 2020 2020  lo_name.        
+00009c60: 7365 6c66 2e63 6f6e 7461 6374 5b22 436f  self.contact["Co
+00009c70: 6e74 6573 744e 5222 5d20 3d20 7365 6c66  ntestNR"] = self
+00009c80: 2e70 7265 662e 6765 7428 2263 6f6e 7465  .pref.get("conte
+00009c90: 7374 222c 2022 3022 290a 2020 2020 2020  st", "0").      
+00009ca0: 2020 7365 6c66 2e63 6f6e 7461 6374 5b22    self.contact["
+00009cb0: 5374 6174 696f 6e50 7265 6669 7822 5d20  StationPrefix"] 
+00009cc0: 3d20 7365 6c66 2e73 7461 7469 6f6e 2e67  = self.station.g
+00009cd0: 6574 2822 4361 6c6c 222c 2022 2229 0a20  et("Call", ""). 
+00009ce0: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
+00009cf0: 6163 745b 2257 5058 5072 6566 6978 225d  act["WPXPrefix"]
+00009d00: 203d 2063 616c 6375 6c61 7465 5f77 7078   = calculate_wpx
+00009d10: 5f70 7265 6669 7828 7365 6c66 2e63 616c  _prefix(self.cal
+00009d20: 6c73 6967 6e2e 7465 7874 2829 290a 2020  lsign.text()).  
+00009d30: 2020 2020 2020 7365 6c66 2e63 6f6e 7461        self.conta
+00009d40: 6374 5b22 4973 5275 6e51 534f 225d 203d  ct["IsRunQSO"] =
+00009d50: 2073 656c 662e 7261 6469 6f42 7574 746f   self.radioButto
+00009d60: 6e5f 7275 6e2e 6973 4368 6563 6b65 6428  n_run.isChecked(
+00009d70: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
+00009d80: 6f6e 7461 6374 5b22 4f70 6572 6174 6f72  ontact["Operator
+00009d90: 225d 203d 2073 656c 662e 6375 7272 656e  "] = self.curren
+00009da0: 745f 6f70 0a20 2020 2020 2020 2073 656c  t_op.        sel
+00009db0: 662e 636f 6e74 6163 745b 224e 6574 4269  f.contact["NetBi
+00009dc0: 6f73 4e61 6d65 225d 203d 2073 6f63 6b65  osName"] = socke
+00009dd0: 742e 6765 7468 6f73 746e 616d 6528 290a  t.gethostname().
+00009de0: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+00009df0: 7461 6374 5b22 4973 4f72 6967 696e 616c  tact["IsOriginal
+00009e00: 225d 203d 2031 0a20 2020 2020 2020 2073  "] = 1.        s
+00009e10: 656c 662e 636f 6e74 6163 745b 2249 4422  elf.contact["ID"
+00009e20: 5d20 3d20 7575 6964 2e75 7569 6434 2829  ] = uuid.uuid4()
+00009e30: 2e68 6578 0a20 2020 2020 2020 2073 656c  .hex.        sel
+00009e40: 662e 636f 6e74 6573 742e 7365 745f 636f  f.contest.set_co
+00009e50: 6e74 6163 745f 7661 7273 2873 656c 6629  ntact_vars(self)
+00009e60: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
+00009e70: 6e74 6163 745b 2250 6f69 6e74 7322 5d20  ntact["Points"] 
+00009e80: 3d20 7365 6c66 2e63 6f6e 7465 7374 2e70  = self.contest.p
+00009e90: 6f69 6e74 7328 7365 6c66 290a 2020 2020  oints(self).    
+00009ea0: 2020 2020 6465 6275 675f 6f75 7470 7574      debug_output
+00009eb0: 203d 2066 227b 7365 6c66 2e63 6f6e 7461   = f"{self.conta
+00009ec0: 6374 7d22 0a20 2020 2020 2020 206c 6f67  ct}".        log
+00009ed0: 6765 722e 6465 6275 6728 6465 6275 675f  ger.debug(debug_
+00009ee0: 6f75 7470 7574 290a 0a20 2020 2020 2020  output)..       
+00009ef0: 2069 6620 7365 6c66 2e6e 316d 6d3a 0a20   if self.n1mm:. 
+00009f00: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+00009f10: 722e 6465 6275 6728 2270 6163 6b65 7473  r.debug("packets
+00009f20: 2025 7322 2c20 6622 7b73 656c 662e 6e31   %s", f"{self.n1
+00009f30: 6d6d 2e73 656e 645f 636f 6e74 6163 745f  mm.send_contact_
+00009f40: 7061 636b 6574 737d 2229 0a20 2020 2020  packets}").     
+00009f50: 2020 2020 2020 2069 6620 7365 6c66 2e6e         if self.n
+00009f60: 316d 6d2e 7365 6e64 5f63 6f6e 7461 6374  1mm.send_contact
+00009f70: 5f70 6163 6b65 7473 3a0a 2020 2020 2020  _packets:.      
+00009f80: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+00009f90: 316d 6d2e 636f 6e74 6163 745f 696e 666f  1mm.contact_info
+00009fa0: 5b22 7469 6d65 7374 616d 7022 5d20 3d20  ["timestamp"] = 
+00009fb0: 7365 6c66 2e63 6f6e 7461 6374 5b22 5453  self.contact["TS
+00009fc0: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
+00009fd0: 2020 2073 656c 662e 6e31 6d6d 2e63 6f6e     self.n1mm.con
+00009fe0: 7461 6374 5f69 6e66 6f5b 226f 6c64 6361  tact_info["oldca
+00009ff0: 6c6c 225d 203d 2073 656c 662e 6e31 6d6d  ll"] = self.n1mm
+0000a000: 2e63 6f6e 7461 6374 5f69 6e66 6f5b 0a20  .contact_info[. 
+0000a010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a020: 2020 2022 6361 6c6c 220a 2020 2020 2020     "call".      
+0000a030: 2020 2020 2020 2020 2020 5d20 3d20 7365            ] = se
+0000a040: 6c66 2e63 6f6e 7461 6374 5b22 4361 6c6c  lf.contact["Call
+0000a050: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
+0000a060: 2020 2073 656c 662e 6e31 6d6d 2e63 6f6e     self.n1mm.con
+0000a070: 7461 6374 5f69 6e66 6f5b 2274 7866 7265  tact_info["txfre
+0000a080: 7122 5d20 3d20 7365 6c66 2e6e 316d 6d2e  q"] = self.n1mm.
+0000a090: 636f 6e74 6163 745f 696e 666f 5b0a 2020  contact_info[.  
+0000a0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a0b0: 2020 2272 7866 7265 7122 0a20 2020 2020    "rxfreq".     
+0000a0c0: 2020 2020 2020 2020 2020 205d 203d 2073             ] = s
+0000a0d0: 656c 662e 6e31 6d6d 2e72 6164 696f 5f69  elf.n1mm.radio_i
+0000a0e0: 6e66 6f5b 2246 7265 7122 5d0a 2020 2020  nfo["Freq"].    
+0000a0f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000a100: 2e6e 316d 6d2e 636f 6e74 6163 745f 696e  .n1mm.contact_in
+0000a110: 666f 5b22 6d6f 6465 225d 203d 2073 656c  fo["mode"] = sel
+0000a120: 662e 636f 6e74 6163 745b 224d 6f64 6522  f.contact["Mode"
+0000a130: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+0000a140: 2020 7365 6c66 2e6e 316d 6d2e 636f 6e74    self.n1mm.cont
+0000a150: 6163 745f 696e 666f 5b22 636f 6e74 6573  act_info["contes
+0000a160: 746e 616d 6522 5d20 3d20 7365 6c66 2e63  tname"] = self.c
+0000a170: 6f6e 7461 6374 5b0a 2020 2020 2020 2020  ontact[.        
+0000a180: 2020 2020 2020 2020 2020 2020 2243 6f6e              "Con
+0000a190: 7465 7374 4e61 6d65 220a 2020 2020 2020  testName".      
+0000a1a0: 2020 2020 2020 2020 2020 5d2e 7265 706c            ].repl
+0000a1b0: 6163 6528 222d 222c 2022 2229 0a20 2020  ace("-", "").   
+0000a1c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000a1d0: 662e 6e31 6d6d 2e63 6f6e 7461 6374 5f69  f.n1mm.contact_i
+0000a1e0: 6e66 6f5b 2263 6f6e 7465 7374 6e72 225d  nfo["contestnr"]
+0000a1f0: 203d 2073 656c 662e 636f 6e74 6163 745b   = self.contact[
+0000a200: 2243 6f6e 7465 7374 4e52 225d 0a20 2020  "ContestNR"].   
+0000a210: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000a220: 662e 6e31 6d6d 2e63 6f6e 7461 6374 5f69  f.n1mm.contact_i
+0000a230: 6e66 6f5b 2273 7461 7469 6f6e 7072 6566  nfo["stationpref
+0000a240: 6978 225d 203d 2073 656c 662e 636f 6e74  ix"] = self.cont
+0000a250: 6163 745b 2253 7461 7469 6f6e 5072 6566  act["StationPref
+0000a260: 6978 225d 0a20 2020 2020 2020 2020 2020  ix"].           
+0000a270: 2020 2020 2073 656c 662e 6e31 6d6d 2e63       self.n1mm.c
+0000a280: 6f6e 7461 6374 5f69 6e66 6f5b 2277 7078  ontact_info["wpx
+0000a290: 7072 6566 6978 225d 203d 2073 656c 662e  prefix"] = self.
+0000a2a0: 636f 6e74 6163 745b 2257 5058 5072 6566  contact["WPXPref
+0000a2b0: 6978 225d 0a20 2020 2020 2020 2020 2020  ix"].           
+0000a2c0: 2020 2020 2073 656c 662e 6e31 6d6d 2e63       self.n1mm.c
+0000a2d0: 6f6e 7461 6374 5f69 6e66 6f5b 2249 7352  ontact_info["IsR
+0000a2e0: 756e 5153 4f22 5d20 3d20 7365 6c66 2e63  unQSO"] = self.c
+0000a2f0: 6f6e 7461 6374 5b22 4973 5275 6e51 534f  ontact["IsRunQSO
+0000a300: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
+0000a310: 2020 2073 656c 662e 6e31 6d6d 2e63 6f6e     self.n1mm.con
+0000a320: 7461 6374 5f69 6e66 6f5b 226f 7065 7261  tact_info["opera
+0000a330: 746f 7222 5d20 3d20 7365 6c66 2e63 6f6e  tor"] = self.con
+0000a340: 7461 6374 5b22 4f70 6572 6174 6f72 225d  tact["Operator"]
+0000a350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a360: 2073 656c 662e 6e31 6d6d 2e63 6f6e 7461   self.n1mm.conta
+0000a370: 6374 5f69 6e66 6f5b 226d 7963 616c 6c22  ct_info["mycall"
+0000a380: 5d20 3d20 7365 6c66 2e63 6f6e 7461 6374  ] = self.contact
+0000a390: 5b22 4f70 6572 6174 6f72 225d 0a20 2020  ["Operator"].   
+0000a3a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000a3b0: 662e 6e31 6d6d 2e63 6f6e 7461 6374 5f69  f.n1mm.contact_i
+0000a3c0: 6e66 6f5b 2253 7461 7469 6f6e 4e61 6d65  nfo["StationName
+0000a3d0: 225d 203d 2073 656c 662e 6e31 6d6d 2e63  "] = self.n1mm.c
+0000a3e0: 6f6e 7461 6374 5f69 6e66 6f5b 0a20 2020  ontact_info[.   
+0000a3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a400: 2022 4e65 7442 696f 734e 616d 6522 0a20   "NetBiosName". 
+0000a410: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
+0000a420: 203d 2073 656c 662e 636f 6e74 6163 745b   = self.contact[
+0000a430: 224e 6574 4269 6f73 4e61 6d65 225d 0a20  "NetBiosName"]. 
+0000a440: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000a450: 656c 662e 6e31 6d6d 2e63 6f6e 7461 6374  elf.n1mm.contact
+0000a460: 5f69 6e66 6f5b 2249 734f 7269 6769 6e61  _info["IsOrigina
+0000a470: 6c22 5d20 3d20 7365 6c66 2e63 6f6e 7461  l"] = self.conta
+0000a480: 6374 5b22 4973 4f72 6967 696e 616c 225d  ct["IsOriginal"]
+0000a490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a4a0: 2073 656c 662e 6e31 6d6d 2e63 6f6e 7461   self.n1mm.conta
+0000a4b0: 6374 5f69 6e66 6f5b 2249 4422 5d20 3d20  ct_info["ID"] = 
+0000a4c0: 7365 6c66 2e63 6f6e 7461 6374 5b22 4944  self.contact["ID
+0000a4d0: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
+0000a4e0: 2020 2073 656c 662e 6e31 6d6d 2e63 6f6e     self.n1mm.con
+0000a4f0: 7461 6374 5f69 6e66 6f5b 2270 6f69 6e74  tact_info["point
+0000a500: 7322 5d20 3d20 7365 6c66 2e63 6f6e 7461  s"] = self.conta
+0000a510: 6374 5b22 506f 696e 7473 225d 0a20 2020  ct["Points"].   
+0000a520: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000a530: 662e 6e31 6d6d 2e63 6f6e 7461 6374 5f69  f.n1mm.contact_i
+0000a540: 6e66 6f5b 2273 6e74 225d 203d 2073 656c  nfo["snt"] = sel
+0000a550: 662e 636f 6e74 6163 745b 2253 4e54 225d  f.contact["SNT"]
+0000a560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a570: 2073 656c 662e 6e31 6d6d 2e63 6f6e 7461   self.n1mm.conta
+0000a580: 6374 5f69 6e66 6f5b 2272 6376 225d 203d  ct_info["rcv"] =
+0000a590: 2073 656c 662e 636f 6e74 6163 745b 2252   self.contact["R
+0000a5a0: 4356 225d 0a20 2020 2020 2020 2020 2020  CV"].           
+0000a5b0: 2020 2020 2073 656c 662e 6e31 6d6d 2e63       self.n1mm.c
+0000a5c0: 6f6e 7461 6374 5f69 6e66 6f5b 2273 6e74  ontact_info["snt
+0000a5d0: 6e72 225d 203d 2073 656c 662e 636f 6e74  nr"] = self.cont
+0000a5e0: 6163 745b 2253 656e 744e 7222 5d0a 2020  act["SentNr"].  
+0000a5f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000a600: 6c66 2e6e 316d 6d2e 636f 6e74 6163 745f  lf.n1mm.contact_
+0000a610: 696e 666f 5b22 7263 766e 7222 5d20 3d20  info["rcvnr"] = 
+0000a620: 7365 6c66 2e63 6f6e 7461 6374 5b22 4e52  self.contact["NR
+0000a630: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
+0000a640: 2020 2073 656c 662e 6e31 6d6d 2e63 6f6e     self.n1mm.con
+0000a650: 7461 6374 5f69 6e66 6f5b 2269 736d 756c  tact_info["ismul
+0000a660: 7469 706c 6965 7231 225d 203d 2073 656c  tiplier1"] = sel
+0000a670: 662e 636f 6e74 6163 742e 6765 7428 0a20  f.contact.get(. 
+0000a680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a690: 2020 2022 4973 4d75 6c74 6970 6c69 6572     "IsMultiplier
+0000a6a0: 3122 2c20 300a 2020 2020 2020 2020 2020  1", 0.          
+0000a6b0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000a6c0: 2020 2020 2020 2020 7365 6c66 2e6e 316d          self.n1m
+0000a6d0: 6d2e 636f 6e74 6163 745f 696e 666f 5b22  m.contact_info["
+0000a6e0: 6973 6d75 6c74 6970 6c69 6572 3222 5d20  ismultiplier2"] 
+0000a6f0: 3d20 7365 6c66 2e63 6f6e 7461 6374 2e67  = self.contact.g
+0000a700: 6574 280a 2020 2020 2020 2020 2020 2020  et(.            
+0000a710: 2020 2020 2020 2020 2249 734d 756c 7469          "IsMulti
+0000a720: 706c 6965 7232 222c 2030 0a20 2020 2020  plier2", 0.     
+0000a730: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000a740: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000a750: 662e 6e31 6d6d 2e63 6f6e 7461 6374 5f69  f.n1mm.contact_i
+0000a760: 6e66 6f5b 2269 736d 756c 7469 706c 6965  nfo["ismultiplie
+0000a770: 7233 225d 203d 2073 656c 662e 636f 6e74  r3"] = self.cont
+0000a780: 6163 742e 6765 7428 0a20 2020 2020 2020  act.get(.       
+0000a790: 2020 2020 2020 2020 2020 2020 2022 4973               "Is
+0000a7a0: 4d75 6c74 6970 6c69 6572 3322 2c20 2230  Multiplier3", "0
+0000a7b0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0000a7c0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0000a7d0: 2020 2020 7365 6c66 2e6e 316d 6d2e 636f      self.n1mm.co
+0000a7e0: 6e74 6163 745f 696e 666f 5b22 7365 6374  ntact_info["sect
+0000a7f0: 696f 6e22 5d20 3d20 7365 6c66 2e63 6f6e  ion"] = self.con
+0000a800: 7461 6374 5b22 5365 6374 225d 0a20 2020  tact["Sect"].   
+0000a810: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000a820: 662e 6e31 6d6d 2e63 6f6e 7461 6374 5f69  f.n1mm.contact_i
+0000a830: 6e66 6f5b 2270 7265 6322 5d20 3d20 7365  nfo["prec"] = se
+0000a840: 6c66 2e63 6f6e 7461 6374 5b22 5072 6563  lf.contact["Prec
+0000a850: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
+0000a860: 2020 2073 656c 662e 6e31 6d6d 2e63 6f6e     self.n1mm.con
+0000a870: 7461 6374 5f69 6e66 6f5b 2263 6b22 5d20  tact_info["ck"] 
+0000a880: 3d20 7365 6c66 2e63 6f6e 7461 6374 5b22  = self.contact["
+0000a890: 434b 225d 0a20 2020 2020 2020 2020 2020  CK"].           
+0000a8a0: 2020 2020 2073 656c 662e 6e31 6d6d 2e63       self.n1mm.c
+0000a8b0: 6f6e 7461 6374 5f69 6e66 6f5b 227a 6e22  ontact_info["zn"
+0000a8c0: 5d20 3d20 7365 6c66 2e63 6f6e 7461 6374  ] = self.contact
+0000a8d0: 5b22 5a4e 225d 0a20 2020 2020 2020 2020  ["ZN"].         
+0000a8e0: 2020 2020 2020 2073 656c 662e 6e31 6d6d         self.n1mm
+0000a8f0: 2e63 6f6e 7461 6374 5f69 6e66 6f5b 2270  .contact_info["p
+0000a900: 6f77 6572 225d 203d 2073 656c 662e 636f  ower"] = self.co
+0000a910: 6e74 6163 745b 2250 6f77 6572 225d 0a20  ntact["Power"]. 
+0000a920: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000a930: 656c 662e 6e31 6d6d 2e63 6f6e 7461 6374  elf.n1mm.contact
+0000a940: 5f69 6e66 6f5b 2262 616e 6422 5d20 3d20  _info["band"] = 
+0000a950: 7365 6c66 2e63 6f6e 7461 6374 5b22 4261  self.contact["Ba
+0000a960: 6e64 225d 0a20 2020 2020 2020 2020 2020  nd"].           
+0000a970: 2020 2020 2023 2073 656c 662e 6e31 6d6d       # self.n1mm
+0000a980: 2e63 6f6e 7461 6374 5f69 6e66 6f5b 2727  .contact_info[''
+0000a990: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+0000a9a0: 2020 2320 7365 6c66 2e6e 316d 6d2e 636f    # self.n1mm.co
+0000a9b0: 6e74 6163 745f 696e 666f 5b27 275d 0a20  ntact_info['']. 
+0000a9c0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000a9d0: 2073 656c 662e 6e31 6d6d 2e63 6f6e 7461   self.n1mm.conta
+0000a9e0: 6374 5f69 6e66 6f5b 2727 5d0a 2020 2020  ct_info[''].    
+0000a9f0: 2020 2020 2020 2020 2020 2020 2320 7365              # se
+0000aa00: 6c66 2e6e 316d 6d2e 636f 6e74 6163 745f  lf.n1mm.contact_
+0000aa10: 696e 666f 5b27 275d 0a20 2020 2020 2020  info[''].       
+0000aa20: 2020 2020 2020 2020 2023 2073 656c 662e           # self.
+0000aa30: 6e31 6d6d 2e63 6f6e 7461 6374 5f69 6e66  n1mm.contact_inf
+0000aa40: 6f5b 2727 5d0a 2020 2020 2020 2020 2020  o[''].          
+0000aa50: 2020 2020 2020 2320 7365 6c66 2e6e 316d        # self.n1m
+0000aa60: 6d2e 636f 6e74 6163 745f 696e 666f 5b27  m.contact_info['
+0000aa70: 275d 0a20 2020 2020 2020 2020 2020 2020  '].             
+0000aa80: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+0000aa90: 2225 7322 2c20 6622 7b73 656c 662e 6e31  "%s", f"{self.n1
+0000aaa0: 6d6d 2e63 6f6e 7461 6374 5f69 6e66 6f7d  mm.contact_info}
+0000aab0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+0000aac0: 2020 2073 656c 662e 6e31 6d6d 2e73 656e     self.n1mm.sen
+0000aad0: 645f 636f 6e74 6163 745f 696e 666f 2829  d_contact_info()
+0000aae0: 0a0a 2020 2020 2020 2020 7365 6c66 2e64  ..        self.d
+0000aaf0: 6174 6162 6173 652e 6c6f 675f 636f 6e74  atabase.log_cont
+0000ab00: 6163 7428 7365 6c66 2e63 6f6e 7461 6374  act(self.contact
+0000ab10: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
+0000ab20: 6c65 6172 696e 7075 7473 2829 0a20 2020  learinputs().   
+0000ab30: 2020 2020 2063 6d64 203d 207b 7d0a 2020       cmd = {}.  
+0000ab40: 2020 2020 2020 636d 645b 2263 6d64 225d        cmd["cmd"]
+0000ab50: 203d 2022 5550 4441 5445 4c4f 4722 0a20   = "UPDATELOG". 
+0000ab60: 2020 2020 2020 2063 6d64 5b22 7374 6174         cmd["stat
+0000ab70: 696f 6e22 5d20 3d20 706c 6174 666f 726d  ion"] = platform
+0000ab80: 2e6e 6f64 6528 290a 2020 2020 2020 2020  .node().        
+0000ab90: 7365 6c66 2e6d 756c 7469 6361 7374 5f69  self.multicast_i
+0000aba0: 6e74 6572 6661 6365 2e73 656e 645f 6173  nterface.send_as
+0000abb0: 5f6a 736f 6e28 636d 6429 0a20 2020 2020  _json(cmd).     
+0000abc0: 2020 2023 2073 656c 662e 636f 6e74 6163     # self.contac
+0000abd0: 745b 2243 6f6e 7465 7374 4e61 6d65 225d  t["ContestName"]
+0000abe0: 203d 2073 656c 662e 636f 6e74 6573 742e   = self.contest.
+0000abf0: 6e61 6d65 0a20 2020 2020 2020 2023 2073  name.        # s
+0000ac00: 656c 662e 636f 6e74 6163 745b 2253 4e54  elf.contact["SNT
+0000ac10: 225d 203d 2073 656c 662e 7365 6e74 2e74  "] = self.sent.t
+0000ac20: 6578 7428 290a 2020 2020 2020 2020 2320  ext().        # 
+0000ac30: 7365 6c66 2e63 6f6e 7461 6374 5b22 5243  self.contact["RC
+0000ac40: 5622 5d20 3d20 7365 6c66 2e72 6563 6569  V"] = self.recei
+0000ac50: 7665 2e74 6578 7428 290a 2020 2020 2020  ve.text().      
+0000ac60: 2020 2320 7365 6c66 2e63 6f6e 7461 6374    # self.contact
+0000ac70: 5b22 436f 756e 7472 7950 7265 6669 7822  ["CountryPrefix"
+0000ac80: 5d0a 2020 2020 2020 2020 2320 7365 6c66  ].        # self
+0000ac90: 2e63 6f6e 7461 6374 5b22 5374 6174 696f  .contact["Statio
+0000aca0: 6e50 7265 6669 7822 5d20 3d20 7365 6c66  nPrefix"] = self
+0000acb0: 2e70 7265 662e 6765 7428 2263 616c 6c73  .pref.get("calls
+0000acc0: 6967 6e22 2c20 2222 290a 2020 2020 2020  ign", "").      
+0000acd0: 2020 2320 7365 6c66 2e63 6f6e 7461 6374    # self.contact
+0000ace0: 5b22 5154 4822 5d0a 2020 2020 2020 2020  ["QTH"].        
+0000acf0: 2320 7365 6c66 2e63 6f6e 7461 6374 5b22  # self.contact["
+0000ad00: 4e61 6d65 225d 203d 2073 656c 662e 6f74  Name"] = self.ot
+0000ad10: 6865 725f 312e 7465 7874 2829 0a20 2020  her_1.text().   
+0000ad20: 2020 2020 2023 2073 656c 662e 636f 6e74       # self.cont
+0000ad30: 6163 745b 2243 6f6d 6d65 6e74 225d 203d  act["Comment"] =
+0000ad40: 2073 656c 662e 6f74 6865 725f 322e 7465   self.other_2.te
+0000ad50: 7874 2829 0a20 2020 2020 2020 2023 2073  xt().        # s
+0000ad60: 656c 662e 636f 6e74 6163 745b 224e 5222  elf.contact["NR"
+0000ad70: 5d0a 2020 2020 2020 2020 2320 7365 6c66  ].        # self
+0000ad80: 2e63 6f6e 7461 6374 5b22 5365 6374 225d  .contact["Sect"]
+0000ad90: 0a20 2020 2020 2020 2023 2073 656c 662e  .        # self.
+0000ada0: 636f 6e74 6163 745b 2250 7265 6322 5d0a  contact["Prec"].
+0000adb0: 2020 2020 2020 2020 2320 7365 6c66 2e63          # self.c
+0000adc0: 6f6e 7461 6374 5b22 434b 225d 0a20 2020  ontact["CK"].   
+0000add0: 2020 2020 2023 2073 656c 662e 636f 6e74       # self.cont
+0000ade0: 6163 745b 225a 4e22 5d0a 2020 2020 2020  act["ZN"].      
+0000adf0: 2020 2320 7365 6c66 2e63 6f6e 7461 6374    # self.contact
+0000ae00: 5b22 5365 6e74 4e72 225d 0a20 2020 2020  ["SentNr"].     
+0000ae10: 2020 2023 2073 656c 662e 636f 6e74 6163     # self.contac
+0000ae20: 745b 2250 6f69 6e74 7322 5d0a 2020 2020  t["Points"].    
+0000ae30: 2020 2020 2320 7365 6c66 2e63 6f6e 7461      # self.conta
+0000ae40: 6374 5b22 4973 4d75 6c74 6970 6c69 6572  ct["IsMultiplier
+0000ae50: 3122 5d0a 2020 2020 2020 2020 2320 7365  1"].        # se
+0000ae60: 6c66 2e63 6f6e 7461 6374 5b22 4973 4d75  lf.contact["IsMu
+0000ae70: 6c74 6970 6c69 6572 3222 5d0a 2020 2020  ltiplier2"].    
+0000ae80: 2020 2020 2320 7365 6c66 2e63 6f6e 7461      # self.conta
+0000ae90: 6374 5b22 506f 7765 7222 5d0a 2020 2020  ct["Power"].    
+0000aea0: 2020 2020 2320 7365 6c66 2e63 6f6e 7461      # self.conta
+0000aeb0: 6374 5b22 4261 6e64 225d 0a20 2020 2020  ct["Band"].     
+0000aec0: 2020 2023 2073 656c 662e 636f 6e74 6163     # self.contac
+0000aed0: 745b 2257 5058 5072 6566 6978 225d 203d  t["WPXPrefix"] =
+0000aee0: 2063 616c 6375 6c61 7465 5f77 7078 5f70   calculate_wpx_p
+0000aef0: 7265 6669 7828 7365 6c66 2e63 616c 6c73  refix(self.calls
+0000af00: 6967 6e2e 7465 7874 2829 290a 2020 2020  ign.text()).    
+0000af10: 2020 2020 2320 7365 6c66 2e63 6f6e 7461      # self.conta
+0000af20: 6374 5b22 4578 6368 616e 6765 3122 5d0a  ct["Exchange1"].
+0000af30: 2020 2020 2020 2020 2320 7365 6c66 2e63          # self.c
+0000af40: 6f6e 7461 6374 5b22 5261 6469 6f4e 5222  ontact["RadioNR"
+0000af50: 5d0a 2020 2020 2020 2020 2320 7365 6c66  ].        # self
+0000af60: 2e63 6f6e 7461 6374 5b22 6973 4d75 6c74  .contact["isMult
+0000af70: 6970 6c69 6572 3322 5d0a 2020 2020 2020  iplier3"].      
+0000af80: 2020 2320 7365 6c66 2e63 6f6e 7461 6374    # self.contact
+0000af90: 5b22 4d69 7363 5465 7874 225d 0a20 2020  ["MiscText"].   
+0000afa0: 2020 2020 2023 2073 656c 662e 636f 6e74       # self.cont
+0000afb0: 6163 745b 2243 6f6e 7461 6374 5479 7065  act["ContactType
+0000afc0: 225d 0a20 2020 2020 2020 2023 2073 656c  "].        # sel
+0000afd0: 662e 636f 6e74 6163 745b 2252 756e 3152  f.contact["Run1R
+0000afe0: 756e 3222 5d0a 2020 2020 2020 2020 2320  un2"].        # 
+0000aff0: 7365 6c66 2e63 6f6e 7461 6374 5b22 4772  self.contact["Gr
+0000b000: 6964 5371 7561 7265 225d 0a20 2020 2020  idSquare"].     
+0000b010: 2020 2023 2073 656c 662e 636f 6e74 6163     # self.contac
+0000b020: 745b 2243 6f6e 7469 6e65 6e74 225d 0a20  t["Continent"]. 
+0000b030: 2020 2020 2020 2023 2073 656c 662e 636f         # self.co
+0000b040: 6e74 6163 745b 2252 6f76 6572 4c6f 6361  ntact["RoverLoca
+0000b050: 7469 6f6e 225d 0a20 2020 2020 2020 2023  tion"].        #
+0000b060: 2073 656c 662e 636f 6e74 6163 745b 2252   self.contact["R
+0000b070: 6164 696f 496e 7465 7266 6163 6564 225d  adioInterfaced"]
+0000b080: 0a20 2020 2020 2020 2023 2073 656c 662e  .        # self.
+0000b090: 636f 6e74 6163 745b 224e 6574 776f 726b  contact["Network
+0000b0a0: 6564 436f 6d70 4e72 225d 0a20 2020 2020  edCompNr"].     
+0000b0b0: 2020 2023 2073 656c 662e 636f 6e74 6163     # self.contac
+0000b0c0: 745b 2243 4c41 494d 4544 5153 4f22 5d0a  t["CLAIMEDQSO"].
+0000b0d0: 0a20 2020 2064 6566 206e 6577 5f63 6f6e  .    def new_con
+0000b0e0: 7465 7374 5f64 6961 6c6f 6728 7365 6c66  test_dialog(self
+0000b0f0: 293a 0a20 2020 2020 2020 2022 2222 5368  ):.        """Sh
+0000b100: 6f77 206e 6577 2063 6f6e 7465 7374 2064  ow new contest d
+0000b110: 6961 6c6f 6722 2222 0a20 2020 2020 2020  ialog""".       
+0000b120: 206c 6f67 6765 722e 6465 6275 6728 224e   logger.debug("N
+0000b130: 6577 2063 6f6e 7465 7374 2044 6961 6c6f  ew contest Dialo
+0000b140: 6722 290a 2020 2020 2020 2020 7365 6c66  g").        self
+0000b150: 2e63 6f6e 7465 7374 5f64 6961 6c6f 6720  .contest_dialog 
+0000b160: 3d20 4e65 7743 6f6e 7465 7374 2857 4f52  = NewContest(WOR
+0000b170: 4b49 4e47 5f50 4154 4829 0a20 2020 2020  KING_PATH).     
+0000b180: 2020 2073 656c 662e 636f 6e74 6573 745f     self.contest_
+0000b190: 6469 616c 6f67 2e61 6363 6570 7465 642e  dialog.accepted.
+0000b1a0: 636f 6e6e 6563 7428 7365 6c66 2e73 6176  connect(self.sav
+0000b1b0: 655f 636f 6e74 6573 7429 0a20 2020 2020  e_contest).     
+0000b1c0: 2020 2073 656c 662e 636f 6e74 6573 745f     self.contest_
+0000b1d0: 6469 616c 6f67 2e64 6174 6554 696d 6545  dialog.dateTimeE
+0000b1e0: 6469 742e 7365 7444 6174 6528 5174 436f  dit.setDate(QtCo
+0000b1f0: 7265 2e51 4461 7465 2e63 7572 7265 6e74  re.QDate.current
+0000b200: 4461 7465 2829 290a 2020 2020 2020 2020  Date()).        
+0000b210: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
+0000b220: 6c6f 672e 6461 7465 5469 6d65 4564 6974  log.dateTimeEdit
+0000b230: 2e73 6574 4361 6c65 6e64 6172 506f 7075  .setCalendarPopu
+0000b240: 7028 5472 7565 290a 2020 2020 2020 2020  p(True).        
+0000b250: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
+0000b260: 6c6f 672e 6461 7465 5469 6d65 4564 6974  log.dateTimeEdit
+0000b270: 2e73 6574 5469 6d65 2851 7443 6f72 652e  .setTime(QtCore.
+0000b280: 5154 696d 6528 302c 2030 2929 0a20 2020  QTime(0, 0)).   
+0000b290: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
+0000b2a0: 745f 6469 616c 6f67 2e70 6f77 6572 2e73  t_dialog.power.s
+0000b2b0: 6574 4375 7272 656e 7454 6578 7428 224c  etCurrentText("L
+0000b2c0: 4f57 2229 0a20 2020 2020 2020 2073 656c  OW").        sel
+0000b2d0: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
+0000b2e0: 2e73 7461 7469 6f6e 2e73 6574 4375 7272  .station.setCurr
+0000b2f0: 656e 7454 6578 7428 2246 4958 4544 2229  entText("FIXED")
+0000b300: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
+0000b310: 6e74 6573 745f 6469 616c 6f67 2e6f 7065  ntest_dialog.ope
+0000b320: 6e28 290a 0a20 2020 2064 6566 2073 6176  n()..    def sav
+0000b330: 655f 636f 6e74 6573 7428 7365 6c66 293a  e_contest(self):
+0000b340: 0a20 2020 2020 2020 2022 2222 5361 7665  .        """Save
+0000b350: 2043 6f6e 7465 7374 2222 220a 2020 2020   Contest""".    
+0000b360: 2020 2020 6e65 7874 5f6e 756d 6265 7220      next_number 
+0000b370: 3d20 7365 6c66 2e64 6174 6162 6173 652e  = self.database.
+0000b380: 6765 745f 6e65 7874 5f63 6f6e 7465 7374  get_next_contest
+0000b390: 5f6e 7228 290a 2020 2020 2020 2020 636f  _nr().        co
+0000b3a0: 6e74 6573 7420 3d20 7b7d 0a20 2020 2020  ntest = {}.     
+0000b3b0: 2020 2063 6f6e 7465 7374 5b22 436f 6e74     contest["Cont
+0000b3c0: 6573 744e 616d 6522 5d20 3d20 280a 2020  estName"] = (.  
+0000b3d0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+0000b3e0: 6f6e 7465 7374 5f64 6961 6c6f 672e 636f  ontest_dialog.co
+0000b3f0: 6e74 6573 742e 6375 7272 656e 7454 6578  ntest.currentTex
+0000b400: 7428 292e 6c6f 7765 7228 292e 7265 706c  t().lower().repl
+0000b410: 6163 6528 2220 222c 2022 5f22 290a 2020  ace(" ", "_").  
+0000b420: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000b430: 636f 6e74 6573 745b 2253 7461 7274 4461  contest["StartDa
+0000b440: 7465 225d 203d 2073 656c 662e 636f 6e74  te"] = self.cont
+0000b450: 6573 745f 6469 616c 6f67 2e64 6174 6554  est_dialog.dateT
+0000b460: 696d 6545 6469 742e 6461 7465 5469 6d65  imeEdit.dateTime
+0000b470: 2829 2e74 6f53 7472 696e 6728 0a20 2020  ().toString(.   
+0000b480: 2020 2020 2020 2020 2022 7979 7979 2d4d           "yyyy-M
+0000b490: 4d2d 6464 2068 683a 6d6d 3a73 7322 0a20  M-dd hh:mm:ss". 
+0000b4a0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000b4b0: 2063 6f6e 7465 7374 5b22 4f70 6572 6174   contest["Operat
+0000b4c0: 6f72 4361 7465 676f 7279 225d 203d 2073  orCategory"] = s
+0000b4d0: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
+0000b4e0: 6f67 2e6f 7065 7261 746f 725f 636c 6173  og.operator_clas
+0000b4f0: 732e 6375 7272 656e 7454 6578 7428 290a  s.currentText().
+0000b500: 2020 2020 2020 2020 636f 6e74 6573 745b          contest[
+0000b510: 2242 616e 6443 6174 6567 6f72 7922 5d20  "BandCategory"] 
+0000b520: 3d20 7365 6c66 2e63 6f6e 7465 7374 5f64  = self.contest_d
+0000b530: 6961 6c6f 672e 6261 6e64 2e63 7572 7265  ialog.band.curre
+0000b540: 6e74 5465 7874 2829 0a20 2020 2020 2020  ntText().       
+0000b550: 2063 6f6e 7465 7374 5b22 506f 7765 7243   contest["PowerC
+0000b560: 6174 6567 6f72 7922 5d20 3d20 7365 6c66  ategory"] = self
+0000b570: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
+0000b580: 706f 7765 722e 6375 7272 656e 7454 6578  power.currentTex
+0000b590: 7428 290a 2020 2020 2020 2020 636f 6e74  t().        cont
+0000b5a0: 6573 745b 224d 6f64 6543 6174 6567 6f72  est["ModeCategor
+0000b5b0: 7922 5d20 3d20 7365 6c66 2e63 6f6e 7465  y"] = self.conte
+0000b5c0: 7374 5f64 6961 6c6f 672e 6d6f 6465 2e63  st_dialog.mode.c
+0000b5d0: 7572 7265 6e74 5465 7874 2829 0a20 2020  urrentText().   
+0000b5e0: 2020 2020 2063 6f6e 7465 7374 5b22 4f76       contest["Ov
+0000b5f0: 6572 6c61 7943 6174 6567 6f72 7922 5d20  erlayCategory"] 
+0000b600: 3d20 7365 6c66 2e63 6f6e 7465 7374 5f64  = self.contest_d
+0000b610: 6961 6c6f 672e 6f76 6572 6c61 792e 6375  ialog.overlay.cu
+0000b620: 7272 656e 7454 6578 7428 290a 2020 2020  rrentText().    
+0000b630: 2020 2020 2320 636f 6e74 6573 745b 2743      # contest['C
+0000b640: 6c61 696d 6564 5363 6f72 6527 5d20 3d20  laimedScore'] = 
+0000b650: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
+0000b660: 6c6f 672e 0a20 2020 2020 2020 2063 6f6e  log..        con
+0000b670: 7465 7374 5b22 4f70 6572 6174 6f72 7322  test["Operators"
+0000b680: 5d20 3d20 7365 6c66 2e63 6f6e 7465 7374  ] = self.contest
+0000b690: 5f64 6961 6c6f 672e 6f70 6572 6174 6f72  _dialog.operator
+0000b6a0: 732e 7465 7874 2829 0a20 2020 2020 2020  s.text().       
+0000b6b0: 2063 6f6e 7465 7374 5b22 536f 6170 626f   contest["Soapbo
+0000b6c0: 7822 5d20 3d20 7365 6c66 2e63 6f6e 7465  x"] = self.conte
+0000b6d0: 7374 5f64 6961 6c6f 672e 736f 6170 626f  st_dialog.soapbo
+0000b6e0: 782e 746f 506c 6169 6e54 6578 7428 290a  x.toPlainText().
+0000b6f0: 2020 2020 2020 2020 636f 6e74 6573 745b          contest[
+0000b700: 2253 656e 7445 7863 6861 6e67 6522 5d20  "SentExchange"] 
+0000b710: 3d20 7365 6c66 2e63 6f6e 7465 7374 5f64  = self.contest_d
+0000b720: 6961 6c6f 672e 6578 6368 616e 6765 2e74  ialog.exchange.t
+0000b730: 6578 7428 290a 2020 2020 2020 2020 636f  ext().        co
+0000b740: 6e74 6573 745b 2243 6f6e 7465 7374 4e52  ntest["ContestNR
+0000b750: 225d 203d 206e 6578 745f 6e75 6d62 6572  "] = next_number
+0000b760: 2e67 6574 2822 636f 756e 7422 2c20 3129  .get("count", 1)
+0000b770: 0a20 2020 2020 2020 2073 656c 662e 7072  .        self.pr
+0000b780: 6566 5b22 636f 6e74 6573 7422 5d20 3d20  ef["contest"] = 
+0000b790: 6e65 7874 5f6e 756d 6265 722e 6765 7428  next_number.get(
+0000b7a0: 2263 6f75 6e74 222c 2031 290a 2020 2020  "count", 1).    
+0000b7b0: 2020 2020 2320 636f 6e74 6573 745b 2753      # contest['S
+0000b7c0: 7562 5479 7065 275d 203d 2073 656c 662e  ubType'] = self.
+0000b7d0: 636f 6e74 6573 745f 6469 616c 6f67 2e0a  contest_dialog..
+0000b7e0: 2020 2020 2020 2020 636f 6e74 6573 745b          contest[
+0000b7f0: 2253 7461 7469 6f6e 4361 7465 676f 7279  "StationCategory
+0000b800: 225d 203d 2073 656c 662e 636f 6e74 6573  "] = self.contes
+0000b810: 745f 6469 616c 6f67 2e73 7461 7469 6f6e  t_dialog.station
+0000b820: 2e63 7572 7265 6e74 5465 7874 2829 0a20  .currentText(). 
+0000b830: 2020 2020 2020 2063 6f6e 7465 7374 5b22         contest["
+0000b840: 4173 7369 7374 6564 4361 7465 676f 7279  AssistedCategory
+0000b850: 225d 203d 2073 656c 662e 636f 6e74 6573  "] = self.contes
+0000b860: 745f 6469 616c 6f67 2e61 7373 6973 7465  t_dialog.assiste
+0000b870: 642e 6375 7272 656e 7454 6578 7428 290a  d.currentText().
+0000b880: 2020 2020 2020 2020 636f 6e74 6573 745b          contest[
+0000b890: 2254 7261 6e73 6d69 7474 6572 4361 7465  "TransmitterCate
+0000b8a0: 676f 7279 225d 203d 2073 656c 662e 636f  gory"] = self.co
+0000b8b0: 6e74 6573 745f 6469 616c 6f67 2e74 7261  ntest_dialog.tra
+0000b8c0: 6e73 6d69 7474 6572 2e63 7572 7265 6e74  nsmitter.current
+0000b8d0: 5465 7874 2829 0a20 2020 2020 2020 2023  Text().        #
+0000b8e0: 2063 6f6e 7465 7374 5b27 5469 6d65 4361   contest['TimeCa
+0000b8f0: 7465 676f 7279 275d 203d 2073 656c 662e  tegory'] = self.
+0000b900: 636f 6e74 6573 745f 6469 616c 6f67 2e0a  contest_dialog..
+0000b910: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+0000b920: 6562 7567 2822 2573 222c 2066 227b 636f  ebug("%s", f"{co
+0000b930: 6e74 6573 747d 2229 0a20 2020 2020 2020  ntest}").       
+0000b940: 2073 656c 662e 6461 7461 6261 7365 2e61   self.database.a
+0000b950: 6464 5f63 6f6e 7465 7374 2863 6f6e 7465  dd_contest(conte
+0000b960: 7374 290a 2020 2020 2020 2020 7365 6c66  st).        self
+0000b970: 2e77 7269 7465 5f70 7265 6665 7265 6e63  .write_preferenc
+0000b980: 6528 290a 2020 2020 2020 2020 7365 6c66  e().        self
+0000b990: 2e6c 6f61 645f 636f 6e74 6573 7428 290a  .load_contest().
+0000b9a0: 0a20 2020 2064 6566 2065 6469 745f 7374  .    def edit_st
+0000b9b0: 6174 696f 6e5f 7365 7474 696e 6773 2873  ation_settings(s
+0000b9c0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+0000b9d0: 2253 686f 7720 7365 7474 696e 6773 2064  "Show settings d
+0000b9e0: 6961 6c6f 6722 2222 0a20 2020 2020 2020  ialog""".       
+0000b9f0: 206c 6f67 6765 722e 6465 6275 6728 2253   logger.debug("S
+0000ba00: 7461 7469 6f6e 2053 6574 7469 6e67 7320  tation Settings 
+0000ba10: 7365 6c65 6374 6564 2229 0a20 2020 2020  selected").     
+0000ba20: 2020 2073 656c 662e 7365 7474 696e 6773     self.settings
+0000ba30: 5f64 6961 6c6f 6720 3d20 4564 6974 5374  _dialog = EditSt
+0000ba40: 6174 696f 6e28 574f 524b 494e 475f 5041  ation(WORKING_PA
+0000ba50: 5448 290a 2020 2020 2020 2020 7365 6c66  TH).        self
+0000ba60: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
+0000ba70: 2e61 6363 6570 7465 642e 636f 6e6e 6563  .accepted.connec
+0000ba80: 7428 7365 6c66 2e73 6176 655f 7365 7474  t(self.save_sett
+0000ba90: 696e 6773 290a 2020 2020 2020 2020 7365  ings).        se
+0000baa0: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
+0000bab0: 6f67 2e43 616c 6c2e 7365 7454 6578 7428  og.Call.setText(
+0000bac0: 7365 6c66 2e73 7461 7469 6f6e 2e67 6574  self.station.get
+0000bad0: 2822 4361 6c6c 222c 2022 2229 290a 2020  ("Call", "")).  
+0000bae0: 2020 2020 2020 7365 6c66 2e73 6574 7469        self.setti
+0000baf0: 6e67 735f 6469 616c 6f67 2e4e 616d 652e  ngs_dialog.Name.
+0000bb00: 7365 7454 6578 7428 7365 6c66 2e73 7461  setText(self.sta
+0000bb10: 7469 6f6e 2e67 6574 2822 4e61 6d65 222c  tion.get("Name",
+0000bb20: 2022 2229 290a 2020 2020 2020 2020 7365   "")).        se
+0000bb30: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
+0000bb40: 6f67 2e41 6464 7265 7373 312e 7365 7454  og.Address1.setT
+0000bb50: 6578 7428 7365 6c66 2e73 7461 7469 6f6e  ext(self.station
+0000bb60: 2e67 6574 2822 5374 7265 6574 3122 2c20  .get("Street1", 
+0000bb70: 2222 2929 0a20 2020 2020 2020 2073 656c  "")).        sel
+0000bb80: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
+0000bb90: 672e 4164 6472 6573 7332 2e73 6574 5465  g.Address2.setTe
+0000bba0: 7874 2873 656c 662e 7374 6174 696f 6e2e  xt(self.station.
+0000bbb0: 6765 7428 2253 7472 6565 7432 222c 2022  get("Street2", "
+0000bbc0: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
+0000bbd0: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
+0000bbe0: 2e43 6974 792e 7365 7454 6578 7428 7365  .City.setText(se
+0000bbf0: 6c66 2e73 7461 7469 6f6e 2e67 6574 2822  lf.station.get("
+0000bc00: 4369 7479 222c 2022 2229 290a 2020 2020  City", "")).    
+0000bc10: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
+0000bc20: 735f 6469 616c 6f67 2e53 7461 7465 2e73  s_dialog.State.s
+0000bc30: 6574 5465 7874 2873 656c 662e 7374 6174  etText(self.stat
+0000bc40: 696f 6e2e 6765 7428 2253 7461 7465 222c  ion.get("State",
+0000bc50: 2022 2229 290a 2020 2020 2020 2020 7365   "")).        se
+0000bc60: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
+0000bc70: 6f67 2e5a 6970 2e73 6574 5465 7874 2873  og.Zip.setText(s
+0000bc80: 656c 662e 7374 6174 696f 6e2e 6765 7428  elf.station.get(
+0000bc90: 225a 6970 222c 2022 2229 290a 2020 2020  "Zip", "")).    
+0000bca0: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
+0000bcb0: 735f 6469 616c 6f67 2e43 6f75 6e74 7279  s_dialog.Country
+0000bcc0: 2e73 6574 5465 7874 2873 656c 662e 7374  .setText(self.st
+0000bcd0: 6174 696f 6e2e 6765 7428 2243 6f75 6e74  ation.get("Count
+0000bce0: 7279 222c 2022 2229 290a 2020 2020 2020  ry", "")).      
+0000bcf0: 2020 7365 6c66 2e73 6574 7469 6e67 735f    self.settings_
+0000bd00: 6469 616c 6f67 2e47 7269 6453 7175 6172  dialog.GridSquar
+0000bd10: 652e 7365 7454 6578 7428 7365 6c66 2e73  e.setText(self.s
+0000bd20: 7461 7469 6f6e 2e67 6574 2822 4772 6964  tation.get("Grid
+0000bd30: 5371 7561 7265 222c 2022 2229 290a 2020  Square", "")).  
+0000bd40: 2020 2020 2020 7365 6c66 2e73 6574 7469        self.setti
+0000bd50: 6e67 735f 6469 616c 6f67 2e43 515a 6f6e  ngs_dialog.CQZon
+0000bd60: 652e 7365 7454 6578 7428 7374 7228 7365  e.setText(str(se
+0000bd70: 6c66 2e73 7461 7469 6f6e 2e67 6574 2822  lf.station.get("
+0000bd80: 4351 5a6f 6e65 222c 2022 2229 2929 0a20  CQZone", ""))). 
+0000bd90: 2020 2020 2020 2073 656c 662e 7365 7474         self.sett
+0000bda0: 696e 6773 5f64 6961 6c6f 672e 4954 555a  ings_dialog.ITUZ
+0000bdb0: 6f6e 652e 7365 7454 6578 7428 7374 7228  one.setText(str(
+0000bdc0: 7365 6c66 2e73 7461 7469 6f6e 2e67 6574  self.station.get
+0000bdd0: 2822 4941 5255 5a6f 6e65 222c 2022 2229  ("IARUZone", "")
+0000bde0: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+0000bdf0: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
+0000be00: 4c69 6365 6e73 652e 7365 7454 6578 7428  License.setText(
+0000be10: 7365 6c66 2e73 7461 7469 6f6e 2e67 6574  self.station.get
+0000be20: 2822 4c69 6365 6e73 6543 6c61 7373 222c  ("LicenseClass",
+0000be30: 2022 2229 290a 2020 2020 2020 2020 7365   "")).        se
+0000be40: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
+0000be50: 6f67 2e4c 6174 6974 7564 652e 7365 7454  og.Latitude.setT
+0000be60: 6578 7428 7374 7228 7365 6c66 2e73 7461  ext(str(self.sta
+0000be70: 7469 6f6e 2e67 6574 2822 4c61 7469 7475  tion.get("Latitu
+0000be80: 6465 222c 2022 2229 2929 0a20 2020 2020  de", ""))).     
+0000be90: 2020 2073 656c 662e 7365 7474 696e 6773     self.settings
+0000bea0: 5f64 6961 6c6f 672e 4c6f 6e67 6974 7564  _dialog.Longitud
+0000beb0: 652e 7365 7454 6578 7428 7374 7228 7365  e.setText(str(se
+0000bec0: 6c66 2e73 7461 7469 6f6e 2e67 6574 2822  lf.station.get("
+0000bed0: 4c6f 6e67 6974 7564 6522 2c20 2222 2929  Longitude", ""))
+0000bee0: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+0000bef0: 6574 7469 6e67 735f 6469 616c 6f67 2e53  ettings_dialog.S
+0000bf00: 7461 7469 6f6e 5458 5258 2e73 6574 5465  tationTXRX.setTe
+0000bf10: 7874 2873 656c 662e 7374 6174 696f 6e2e  xt(self.station.
+0000bf20: 6765 7428 2273 7461 7469 6f6e 7478 7278  get("stationtxrx
+0000bf30: 222c 2022 2229 290a 2020 2020 2020 2020  ", "")).        
+0000bf40: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
+0000bf50: 616c 6f67 2e50 6f77 6572 2e73 6574 5465  alog.Power.setTe
+0000bf60: 7874 2873 656c 662e 7374 6174 696f 6e2e  xt(self.station.
+0000bf70: 6765 7428 2253 506f 7765 222c 2022 2229  get("SPowe", "")
+0000bf80: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+0000bf90: 6574 7469 6e67 735f 6469 616c 6f67 2e41  ettings_dialog.A
+0000bfa0: 6e74 656e 6e61 2e73 6574 5465 7874 2873  ntenna.setText(s
+0000bfb0: 656c 662e 7374 6174 696f 6e2e 6765 7428  elf.station.get(
+0000bfc0: 2253 416e 7465 222c 2022 2229 290a 2020  "SAnte", "")).  
+0000bfd0: 2020 2020 2020 7365 6c66 2e73 6574 7469        self.setti
+0000bfe0: 6e67 735f 6469 616c 6f67 2e41 6e74 4865  ngs_dialog.AntHe
+0000bff0: 6967 6874 2e73 6574 5465 7874 2873 656c  ight.setText(sel
+0000c000: 662e 7374 6174 696f 6e2e 6765 7428 2253  f.station.get("S
+0000c010: 416e 7448 3122 2c20 2222 2929 0a20 2020  AntH1", "")).   
+0000c020: 2020 2020 2073 656c 662e 7365 7474 696e       self.settin
+0000c030: 6773 5f64 6961 6c6f 672e 4153 4c2e 7365  gs_dialog.ASL.se
+0000c040: 7454 6578 7428 7365 6c66 2e73 7461 7469  tText(self.stati
+0000c050: 6f6e 2e67 6574 2822 5341 6e74 4832 222c  on.get("SAntH2",
+0000c060: 2022 2229 290a 2020 2020 2020 2020 7365   "")).        se
+0000c070: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
+0000c080: 6f67 2e41 5252 4c53 6563 7469 6f6e 2e73  og.ARRLSection.s
+0000c090: 6574 5465 7874 2873 656c 662e 7374 6174  etText(self.stat
+0000c0a0: 696f 6e2e 6765 7428 2241 5252 4c53 6563  ion.get("ARRLSec
+0000c0b0: 7469 6f6e 222c 2022 2229 290a 2020 2020  tion", "")).    
+0000c0c0: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
+0000c0d0: 735f 6469 616c 6f67 2e52 6f76 6572 5154  s_dialog.RoverQT
+0000c0e0: 482e 7365 7454 6578 7428 7365 6c66 2e73  H.setText(self.s
+0000c0f0: 7461 7469 6f6e 2e67 6574 2822 526f 7665  tation.get("Rove
+0000c100: 7251 5448 222c 2022 2229 290a 2020 2020  rQTH", "")).    
+0000c110: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
+0000c120: 735f 6469 616c 6f67 2e43 6c75 622e 7365  s_dialog.Club.se
+0000c130: 7454 6578 7428 7365 6c66 2e73 7461 7469  tText(self.stati
+0000c140: 6f6e 2e67 6574 2822 436c 7562 222c 2022  on.get("Club", "
+0000c150: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
+0000c160: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
+0000c170: 2e45 6d61 696c 2e73 6574 5465 7874 2873  .Email.setText(s
+0000c180: 656c 662e 7374 6174 696f 6e2e 6765 7428  elf.station.get(
+0000c190: 2245 6d61 696c 222c 2022 2229 290a 2020  "Email", "")).  
+0000c1a0: 2020 2020 2020 7365 6c66 2e73 6574 7469        self.setti
+0000c1b0: 6e67 735f 6469 616c 6f67 2e6f 7065 6e28  ngs_dialog.open(
+0000c1c0: 290a 0a20 2020 2064 6566 2073 6176 655f  )..    def save_
+0000c1d0: 7365 7474 696e 6773 2873 656c 6629 3a0a  settings(self):.
+0000c1e0: 2020 2020 2020 2020 2222 2253 6176 6520          """Save 
+0000c1f0: 7365 7474 696e 6773 2222 220a 2020 2020  settings""".    
+0000c200: 2020 2020 6373 203d 2073 656c 662e 7365      cs = self.se
+0000c210: 7474 696e 6773 5f64 6961 6c6f 672e 4361  ttings_dialog.Ca
+0000c220: 6c6c 2e74 6578 7428 290a 2020 2020 2020  ll.text().      
+0000c230: 2020 7365 6c66 2e73 7461 7469 6f6e 203d    self.station =
+0000c240: 207b 7d0a 2020 2020 2020 2020 7365 6c66   {}.        self
+0000c250: 2e73 7461 7469 6f6e 5b22 4361 6c6c 225d  .station["Call"]
+0000c260: 203d 2063 732e 7570 7065 7228 290a 2020   = cs.upper().  
+0000c270: 2020 2020 2020 7365 6c66 2e73 7461 7469        self.stati
+0000c280: 6f6e 5b22 4e61 6d65 225d 203d 2073 656c  on["Name"] = sel
+0000c290: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
+0000c2a0: 672e 4e61 6d65 2e74 6578 7428 292e 7469  g.Name.text().ti
+0000c2b0: 746c 6528 290a 2020 2020 2020 2020 7365  tle().        se
+0000c2c0: 6c66 2e73 7461 7469 6f6e 5b22 5374 7265  lf.station["Stre
+0000c2d0: 6574 3122 5d20 3d20 7365 6c66 2e73 6574  et1"] = self.set
+0000c2e0: 7469 6e67 735f 6469 616c 6f67 2e41 6464  tings_dialog.Add
+0000c2f0: 7265 7373 312e 7465 7874 2829 2e74 6974  ress1.text().tit
+0000c300: 6c65 2829 0a20 2020 2020 2020 2073 656c  le().        sel
+0000c310: 662e 7374 6174 696f 6e5b 2253 7472 6565  f.station["Stree
+0000c320: 7432 225d 203d 2073 656c 662e 7365 7474  t2"] = self.sett
+0000c330: 696e 6773 5f64 6961 6c6f 672e 4164 6472  ings_dialog.Addr
+0000c340: 6573 7332 2e74 6578 7428 292e 7469 746c  ess2.text().titl
+0000c350: 6528 290a 2020 2020 2020 2020 7365 6c66  e().        self
+0000c360: 2e73 7461 7469 6f6e 5b22 4369 7479 225d  .station["City"]
+0000c370: 203d 2073 656c 662e 7365 7474 696e 6773   = self.settings
+0000c380: 5f64 6961 6c6f 672e 4369 7479 2e74 6578  _dialog.City.tex
+0000c390: 7428 292e 7469 746c 6528 290a 2020 2020  t().title().    
+0000c3a0: 2020 2020 7365 6c66 2e73 7461 7469 6f6e      self.station
+0000c3b0: 5b22 5374 6174 6522 5d20 3d20 7365 6c66  ["State"] = self
+0000c3c0: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
+0000c3d0: 2e53 7461 7465 2e74 6578 7428 292e 7570  .State.text().up
+0000c3e0: 7065 7228 290a 2020 2020 2020 2020 7365  per().        se
+0000c3f0: 6c66 2e73 7461 7469 6f6e 5b22 5a69 7022  lf.station["Zip"
+0000c400: 5d20 3d20 7365 6c66 2e73 6574 7469 6e67  ] = self.setting
+0000c410: 735f 6469 616c 6f67 2e5a 6970 2e74 6578  s_dialog.Zip.tex
+0000c420: 7428 290a 2020 2020 2020 2020 7365 6c66  t().        self
+0000c430: 2e73 7461 7469 6f6e 5b22 436f 756e 7472  .station["Countr
+0000c440: 7922 5d20 3d20 7365 6c66 2e73 6574 7469  y"] = self.setti
+0000c450: 6e67 735f 6469 616c 6f67 2e43 6f75 6e74  ngs_dialog.Count
+0000c460: 7279 2e74 6578 7428 292e 7469 746c 6528  ry.text().title(
+0000c470: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+0000c480: 7461 7469 6f6e 5b22 4772 6964 5371 7561  tation["GridSqua
+0000c490: 7265 225d 203d 2073 656c 662e 7365 7474  re"] = self.sett
+0000c4a0: 696e 6773 5f64 6961 6c6f 672e 4772 6964  ings_dialog.Grid
+0000c4b0: 5371 7561 7265 2e74 6578 7428 290a 2020  Square.text().  
+0000c4c0: 2020 2020 2020 7365 6c66 2e73 7461 7469        self.stati
+0000c4d0: 6f6e 5b22 4351 5a6f 6e65 225d 203d 2073  on["CQZone"] = s
+0000c4e0: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
+0000c4f0: 6c6f 672e 4351 5a6f 6e65 2e74 6578 7428  log.CQZone.text(
+0000c500: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+0000c510: 7461 7469 6f6e 5b22 4941 5255 5a6f 6e65  tation["IARUZone
+0000c520: 225d 203d 2073 656c 662e 7365 7474 696e  "] = self.settin
+0000c530: 6773 5f64 6961 6c6f 672e 4954 555a 6f6e  gs_dialog.ITUZon
+0000c540: 652e 7465 7874 2829 0a20 2020 2020 2020  e.text().       
+0000c550: 2073 656c 662e 7374 6174 696f 6e5b 224c   self.station["L
+0000c560: 6963 656e 7365 436c 6173 7322 5d20 3d20  icenseClass"] = 
+0000c570: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
+0000c580: 616c 6f67 2e4c 6963 656e 7365 2e74 6578  alog.License.tex
+0000c590: 7428 292e 7469 746c 6528 290a 2020 2020  t().title().    
+0000c5a0: 2020 2020 7365 6c66 2e73 7461 7469 6f6e      self.station
+0000c5b0: 5b22 4c61 7469 7475 6465 225d 203d 2073  ["Latitude"] = s
+0000c5c0: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
+0000c5d0: 6c6f 672e 4c61 7469 7475 6465 2e74 6578  log.Latitude.tex
+0000c5e0: 7428 290a 2020 2020 2020 2020 7365 6c66  t().        self
+0000c5f0: 2e73 7461 7469 6f6e 5b22 4c6f 6e67 6974  .station["Longit
+0000c600: 7564 6522 5d20 3d20 7365 6c66 2e73 6574  ude"] = self.set
+0000c610: 7469 6e67 735f 6469 616c 6f67 2e4c 6f6e  tings_dialog.Lon
+0000c620: 6769 7475 6465 2e74 6578 7428 290a 2020  gitude.text().  
+0000c630: 2020 2020 2020 7365 6c66 2e73 7461 7469        self.stati
+0000c640: 6f6e 5b22 5354 5865 7122 5d20 3d20 7365  on["STXeq"] = se
+0000c650: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
+0000c660: 6f67 2e53 7461 7469 6f6e 5458 5258 2e74  og.StationTXRX.t
+0000c670: 6578 7428 290a 2020 2020 2020 2020 7365  ext().        se
+0000c680: 6c66 2e73 7461 7469 6f6e 5b22 5350 6f77  lf.station["SPow
+0000c690: 6522 5d20 3d20 7365 6c66 2e73 6574 7469  e"] = self.setti
+0000c6a0: 6e67 735f 6469 616c 6f67 2e50 6f77 6572  ngs_dialog.Power
+0000c6b0: 2e74 6578 7428 290a 2020 2020 2020 2020  .text().        
+0000c6c0: 7365 6c66 2e73 7461 7469 6f6e 5b22 5341  self.station["SA
+0000c6d0: 6e74 6522 5d20 3d20 7365 6c66 2e73 6574  nte"] = self.set
+0000c6e0: 7469 6e67 735f 6469 616c 6f67 2e41 6e74  tings_dialog.Ant
+0000c6f0: 656e 6e61 2e74 6578 7428 290a 2020 2020  enna.text().    
+0000c700: 2020 2020 7365 6c66 2e73 7461 7469 6f6e      self.station
+0000c710: 5b22 5341 6e74 4831 225d 203d 2073 656c  ["SAntH1"] = sel
+0000c720: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
+0000c730: 672e 416e 7448 6569 6768 742e 7465 7874  g.AntHeight.text
+0000c740: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+0000c750: 7374 6174 696f 6e5b 2253 416e 7448 3222  station["SAntH2"
+0000c760: 5d20 3d20 7365 6c66 2e73 6574 7469 6e67  ] = self.setting
+0000c770: 735f 6469 616c 6f67 2e41 534c 2e74 6578  s_dialog.ASL.tex
+0000c780: 7428 290a 2020 2020 2020 2020 7365 6c66  t().        self
+0000c790: 2e73 7461 7469 6f6e 5b22 4152 524c 5365  .station["ARRLSe
+0000c7a0: 6374 696f 6e22 5d20 3d20 7365 6c66 2e73  ction"] = self.s
+0000c7b0: 6574 7469 6e67 735f 6469 616c 6f67 2e41  ettings_dialog.A
+0000c7c0: 5252 4c53 6563 7469 6f6e 2e74 6578 7428  RRLSection.text(
+0000c7d0: 292e 7570 7065 7228 290a 2020 2020 2020  ).upper().      
+0000c7e0: 2020 7365 6c66 2e73 7461 7469 6f6e 5b22    self.station["
+0000c7f0: 526f 7665 7251 5448 225d 203d 2073 656c  RoverQTH"] = sel
+0000c800: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
+0000c810: 672e 526f 7665 7251 5448 2e74 6578 7428  g.RoverQTH.text(
+0000c820: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+0000c830: 7461 7469 6f6e 5b22 436c 7562 225d 203d  tation["Club"] =
+0000c840: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
+0000c850: 6961 6c6f 672e 436c 7562 2e74 6578 7428  ialog.Club.text(
+0000c860: 292e 7469 746c 6528 290a 2020 2020 2020  ).title().      
+0000c870: 2020 7365 6c66 2e73 7461 7469 6f6e 5b22    self.station["
+0000c880: 456d 6169 6c22 5d20 3d20 7365 6c66 2e73  Email"] = self.s
+0000c890: 6574 7469 6e67 735f 6469 616c 6f67 2e45  ettings_dialog.E
+0000c8a0: 6d61 696c 2e74 6578 7428 290a 2020 2020  mail.text().    
+0000c8b0: 2020 2020 7365 6c66 2e64 6174 6162 6173      self.databas
+0000c8c0: 652e 6164 645f 7374 6174 696f 6e28 7365  e.add_station(se
+0000c8d0: 6c66 2e73 7461 7469 6f6e 290a 2020 2020  lf.station).    
+0000c8e0: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
+0000c8f0: 735f 6469 616c 6f67 2e63 6c6f 7365 2829  s_dialog.close()
+0000c900: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0000c910: 2e63 7572 7265 6e74 5f6f 7020 3d3d 2022  .current_op == "
+0000c920: 223a 0a20 2020 2020 2020 2020 2020 2073  ":.            s
+0000c930: 656c 662e 6375 7272 656e 745f 6f70 203d  elf.current_op =
+0000c940: 2073 656c 662e 7374 6174 696f 6e2e 6765   self.station.ge
+0000c950: 7428 2243 616c 6c22 2c20 2222 290a 2020  t("Call", "").  
+0000c960: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+0000c970: 616b 655f 6f70 5f64 6972 2829 0a20 2020  ake_op_dir().   
+0000c980: 2020 2020 2063 6f6e 7465 7374 5f63 6f75       contest_cou
+0000c990: 6e74 203d 2073 656c 662e 6461 7461 6261  nt = self.databa
+0000c9a0: 7365 2e66 6574 6368 5f61 6c6c 5f63 6f6e  se.fetch_all_con
+0000c9b0: 7465 7374 7328 290a 2020 2020 2020 2020  tests().        
+0000c9c0: 6966 206c 656e 2863 6f6e 7465 7374 5f63  if len(contest_c
+0000c9d0: 6f75 6e74 2920 3d3d 2030 3a0a 2020 2020  ount) == 0:.    
+0000c9e0: 2020 2020 2020 2020 7365 6c66 2e6e 6577          self.new
+0000c9f0: 5f63 6f6e 7465 7374 5f64 6961 6c6f 6728  _contest_dialog(
+0000ca00: 290a 0a20 2020 2064 6566 2065 6469 745f  )..    def edit_
+0000ca10: 6d61 6372 6f28 7365 6c66 2c20 6675 6e63  macro(self, func
+0000ca20: 7469 6f6e 5f6b 6579 293a 0a20 2020 2020  tion_key):.     
+0000ca30: 2020 2022 2222 5368 6f77 2065 6469 7420     """Show edit 
+0000ca40: 6d61 6372 6f20 6469 616c 6f67 2222 220a  macro dialog""".
+0000ca50: 2020 2020 2020 2020 7365 6c66 2e65 6469          self.edi
+0000ca60: 745f 6d61 6372 6f5f 6469 616c 6f67 203d  t_macro_dialog =
+0000ca70: 2045 6469 744d 6163 726f 2866 756e 6374   EditMacro(funct
+0000ca80: 696f 6e5f 6b65 792c 2057 4f52 4b49 4e47  ion_key, WORKING
+0000ca90: 5f50 4154 4829 0a20 2020 2020 2020 2073  _PATH).        s
+0000caa0: 656c 662e 6564 6974 5f6d 6163 726f 5f64  elf.edit_macro_d
+0000cab0: 6961 6c6f 672e 6163 6365 7074 6564 2e63  ialog.accepted.c
+0000cac0: 6f6e 6e65 6374 2873 656c 662e 6564 6974  onnect(self.edit
+0000cad0: 6564 5f6d 6163 726f 290a 2020 2020 2020  ed_macro).      
+0000cae0: 2020 7365 6c66 2e65 6469 745f 6d61 6372    self.edit_macr
+0000caf0: 6f5f 6469 616c 6f67 2e6f 7065 6e28 290a  o_dialog.open().
+0000cb00: 0a20 2020 2064 6566 2065 6469 7465 645f  .    def edited_
+0000cb10: 6d61 6372 6f28 7365 6c66 293a 0a20 2020  macro(self):.   
+0000cb20: 2020 2020 2022 2222 5361 7665 2065 6469       """Save edi
+0000cb30: 7465 6420 6d61 6372 6f22 2222 0a20 2020  ted macro""".   
+0000cb40: 2020 2020 2073 656c 662e 6564 6974 5f6d       self.edit_m
+0000cb50: 6163 726f 5f64 6961 6c6f 672e 6675 6e63  acro_dialog.func
+0000cb60: 7469 6f6e 5f6b 6579 2e73 6574 5465 7874  tion_key.setText
+0000cb70: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
+0000cb80: 6c66 2e65 6469 745f 6d61 6372 6f5f 6469  lf.edit_macro_di
+0000cb90: 616c 6f67 2e6d 6163 726f 5f6c 6162 656c  alog.macro_label
+0000cba0: 2e74 6578 7428 290a 2020 2020 2020 2020  .text().        
+0000cbb0: 290a 2020 2020 2020 2020 7365 6c66 2e65  ).        self.e
+0000cbc0: 6469 745f 6d61 6372 6f5f 6469 616c 6f67  dit_macro_dialog
+0000cbd0: 2e66 756e 6374 696f 6e5f 6b65 792e 7365  .function_key.se
+0000cbe0: 7454 6f6f 6c54 6970 280a 2020 2020 2020  tToolTip(.      
+0000cbf0: 2020 2020 2020 7365 6c66 2e65 6469 745f        self.edit_
+0000cc00: 6d61 6372 6f5f 6469 616c 6f67 2e74 6865  macro_dialog.the
+0000cc10: 5f6d 6163 726f 2e74 6578 7428 290a 2020  _macro.text().  
+0000cc20: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000cc30: 7365 6c66 2e65 6469 745f 6d61 6372 6f5f  self.edit_macro_
+0000cc40: 6469 616c 6f67 2e63 6c6f 7365 2829 0a0a  dialog.close()..
+0000cc50: 2020 2020 6465 6620 6564 6974 5f46 3128      def edit_F1(
+0000cc60: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+0000cc70: 2222 7374 7562 2222 220a 2020 2020 2020  ""stub""".      
+0000cc80: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
+0000cc90: 4631 2052 6967 6874 2043 6c69 636b 6564  F1 Right Clicked
+0000cca0: 2e22 290a 2020 2020 2020 2020 7365 6c66  .").        self
+0000ccb0: 2e65 6469 745f 6d61 6372 6f28 7365 6c66  .edit_macro(self
+0000ccc0: 2e46 3129 0a0a 2020 2020 6465 6620 6564  .F1)..    def ed
+0000ccd0: 6974 5f46 3228 7365 6c66 293a 0a20 2020  it_F2(self):.   
+0000cce0: 2020 2020 2022 2222 7374 7562 2222 220a       """stub""".
+0000ccf0: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+0000cd00: 6562 7567 2822 4632 2052 6967 6874 2043  ebug("F2 Right C
+0000cd10: 6c69 636b 6564 2e22 290a 2020 2020 2020  licked.").      
+0000cd20: 2020 7365 6c66 2e65 6469 745f 6d61 6372    self.edit_macr
+0000cd30: 6f28 7365 6c66 2e46 3229 0a0a 2020 2020  o(self.F2)..    
+0000cd40: 6465 6620 6564 6974 5f46 3328 7365 6c66  def edit_F3(self
+0000cd50: 293a 0a20 2020 2020 2020 2022 2222 7374  ):.        """st
+0000cd60: 7562 2222 220a 2020 2020 2020 2020 6c6f  ub""".        lo
+0000cd70: 6767 6572 2e64 6562 7567 2822 4633 2052  gger.debug("F3 R
+0000cd80: 6967 6874 2043 6c69 636b 6564 2e22 290a  ight Clicked.").
+0000cd90: 2020 2020 2020 2020 7365 6c66 2e65 6469          self.edi
+0000cda0: 745f 6d61 6372 6f28 7365 6c66 2e46 3329  t_macro(self.F3)
+0000cdb0: 0a0a 2020 2020 6465 6620 6564 6974 5f46  ..    def edit_F
+0000cdc0: 3428 7365 6c66 293a 0a20 2020 2020 2020  4(self):.       
+0000cdd0: 2022 2222 7374 7562 2222 220a 2020 2020   """stub""".    
+0000cde0: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+0000cdf0: 2822 4634 2052 6967 6874 2043 6c69 636b  ("F4 Right Click
+0000ce00: 6564 2e22 290a 2020 2020 2020 2020 7365  ed.").        se
+0000ce10: 6c66 2e65 6469 745f 6d61 6372 6f28 7365  lf.edit_macro(se
+0000ce20: 6c66 2e46 3429 0a0a 2020 2020 6465 6620  lf.F4)..    def 
+0000ce30: 6564 6974 5f46 3528 7365 6c66 293a 0a20  edit_F5(self):. 
+0000ce40: 2020 2020 2020 2022 2222 7374 7562 2222         """stub""
+0000ce50: 220a 2020 2020 2020 2020 6c6f 6767 6572  ".        logger
+0000ce60: 2e64 6562 7567 2822 4635 2052 6967 6874  .debug("F5 Right
+0000ce70: 2043 6c69 636b 6564 2e22 290a 2020 2020   Clicked.").    
+0000ce80: 2020 2020 7365 6c66 2e65 6469 745f 6d61      self.edit_ma
+0000ce90: 6372 6f28 7365 6c66 2e46 3529 0a0a 2020  cro(self.F5)..  
+0000cea0: 2020 6465 6620 6564 6974 5f46 3628 7365    def edit_F6(se
+0000ceb0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+0000cec0: 7374 7562 2222 220a 2020 2020 2020 2020  stub""".        
+0000ced0: 6c6f 6767 6572 2e64 6562 7567 2822 4636  logger.debug("F6
+0000cee0: 2052 6967 6874 2043 6c69 636b 6564 2e22   Right Clicked."
+0000cef0: 290a 2020 2020 2020 2020 7365 6c66 2e65  ).        self.e
+0000cf00: 6469 745f 6d61 6372 6f28 7365 6c66 2e46  dit_macro(self.F
+0000cf10: 3629 0a0a 2020 2020 6465 6620 6564 6974  6)..    def edit
+0000cf20: 5f46 3728 7365 6c66 293a 0a20 2020 2020  _F7(self):.     
+0000cf30: 2020 2022 2222 7374 7562 2222 220a 2020     """stub""".  
+0000cf40: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
+0000cf50: 7567 2822 4637 2052 6967 6874 2043 6c69  ug("F7 Right Cli
+0000cf60: 636b 6564 2e22 290a 2020 2020 2020 2020  cked.").        
+0000cf70: 7365 6c66 2e65 6469 745f 6d61 6372 6f28  self.edit_macro(
+0000cf80: 7365 6c66 2e46 3729 0a0a 2020 2020 6465  self.F7)..    de
+0000cf90: 6620 6564 6974 5f46 3828 7365 6c66 293a  f edit_F8(self):
+0000cfa0: 0a20 2020 2020 2020 2022 2222 7374 7562  .        """stub
+0000cfb0: 2222 220a 2020 2020 2020 2020 6c6f 6767  """.        logg
+0000cfc0: 6572 2e64 6562 7567 2822 4638 2052 6967  er.debug("F8 Rig
+0000cfd0: 6874 2043 6c69 636b 6564 2e22 290a 2020  ht Clicked.").  
+0000cfe0: 2020 2020 2020 7365 6c66 2e65 6469 745f        self.edit_
+0000cff0: 6d61 6372 6f28 7365 6c66 2e46 3829 0a0a  macro(self.F8)..
+0000d000: 2020 2020 6465 6620 6564 6974 5f46 3928      def edit_F9(
+0000d010: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+0000d020: 2222 7374 7562 2222 220a 2020 2020 2020  ""stub""".      
+0000d030: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
+0000d040: 4639 2052 6967 6874 2043 6c69 636b 6564  F9 Right Clicked
+0000d050: 2e22 290a 2020 2020 2020 2020 7365 6c66  .").        self
+0000d060: 2e65 6469 745f 6d61 6372 6f28 7365 6c66  .edit_macro(self
+0000d070: 2e46 3929 0a0a 2020 2020 6465 6620 6564  .F9)..    def ed
+0000d080: 6974 5f46 3130 2873 656c 6629 3a0a 2020  it_F10(self):.  
+0000d090: 2020 2020 2020 2222 2273 7475 6222 2222        """stub"""
+0000d0a0: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
+0000d0b0: 6465 6275 6728 2246 3130 2052 6967 6874  debug("F10 Right
+0000d0c0: 2043 6c69 636b 6564 2e22 290a 2020 2020   Clicked.").    
+0000d0d0: 2020 2020 7365 6c66 2e65 6469 745f 6d61      self.edit_ma
+0000d0e0: 6372 6f28 7365 6c66 2e46 3130 290a 0a20  cro(self.F10).. 
+0000d0f0: 2020 2064 6566 2065 6469 745f 4631 3128     def edit_F11(
+0000d100: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+0000d110: 2222 7374 7562 2222 220a 2020 2020 2020  ""stub""".      
+0000d120: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
+0000d130: 4631 3120 5269 6768 7420 436c 6963 6b65  F11 Right Clicke
+0000d140: 642e 2229 0a20 2020 2020 2020 2073 656c  d.").        sel
+0000d150: 662e 6564 6974 5f6d 6163 726f 2873 656c  f.edit_macro(sel
+0000d160: 662e 4631 3129 0a0a 2020 2020 6465 6620  f.F11)..    def 
+0000d170: 6564 6974 5f46 3132 2873 656c 6629 3a0a  edit_F12(self):.
+0000d180: 2020 2020 2020 2020 2222 2273 7475 6222          """stub"
+0000d190: 2222 0a20 2020 2020 2020 206c 6f67 6765  "".        logge
+0000d1a0: 722e 6465 6275 6728 2246 3132 2052 6967  r.debug("F12 Rig
+0000d1b0: 6874 2043 6c69 636b 6564 2e22 290a 2020  ht Clicked.").  
+0000d1c0: 2020 2020 2020 7365 6c66 2e65 6469 745f        self.edit_
+0000d1d0: 6d61 6372 6f28 7365 6c66 2e46 3132 290a  macro(self.F12).
+0000d1e0: 0a20 2020 2064 6566 2070 726f 6365 7373  .    def process
+0000d1f0: 5f6d 6163 726f 2873 656c 662c 206d 6163  _macro(self, mac
+0000d200: 726f 3a20 7374 7229 202d 3e20 7374 723a  ro: str) -> str:
+0000d210: 0a20 2020 2020 2020 2022 2222 5072 6f63  .        """Proc
+0000d220: 6573 7320 4357 206d 6163 726f 2073 7562  ess CW macro sub
+0000d230: 7374 6974 7574 696f 6e73 2222 220a 2020  stitutions""".  
+0000d240: 2020 2020 2020 7265 7375 6c74 203d 2073        result = s
+0000d250: 656c 662e 6461 7461 6261 7365 2e67 6574  elf.database.get
+0000d260: 5f73 6572 6961 6c28 290a 2020 2020 2020  _serial().      
+0000d270: 2020 6e65 7874 5f73 6572 6961 6c20 3d20    next_serial = 
+0000d280: 7374 7228 7265 7375 6c74 2e67 6574 2822  str(result.get("
+0000d290: 7365 7269 616c 5f6e 7222 2c20 2231 2229  serial_nr", "1")
+0000d2a0: 290a 2020 2020 2020 2020 6966 206e 6578  ).        if nex
+0000d2b0: 745f 7365 7269 616c 203d 3d20 224e 6f6e  t_serial == "Non
+0000d2c0: 6522 3a0a 2020 2020 2020 2020 2020 2020  e":.            
+0000d2d0: 6e65 7874 5f73 6572 6961 6c20 3d20 2231  next_serial = "1
+0000d2e0: 220a 2020 2020 2020 2020 6d61 6372 6f20  ".        macro 
+0000d2f0: 3d20 6d61 6372 6f2e 7570 7065 7228 290a  = macro.upper().
+0000d300: 2020 2020 2020 2020 6d61 6372 6f20 3d20          macro = 
+0000d310: 6d61 6372 6f2e 7265 706c 6163 6528 2223  macro.replace("#
+0000d320: 222c 206e 6578 745f 7365 7269 616c 290a  ", next_serial).
+0000d330: 2020 2020 2020 2020 6d61 6372 6f20 3d20          macro = 
+0000d340: 6d61 6372 6f2e 7265 706c 6163 6528 227b  macro.replace("{
+0000d350: 4d59 4341 4c4c 7d22 2c20 7365 6c66 2e73  MYCALL}", self.s
+0000d360: 7461 7469 6f6e 2e67 6574 2822 4361 6c6c  tation.get("Call
+0000d370: 222c 2022 2229 290a 2020 2020 2020 2020  ", "")).        
+0000d380: 6d61 6372 6f20 3d20 6d61 6372 6f2e 7265  macro = macro.re
+0000d390: 706c 6163 6528 227b 4849 5343 414c 4c7d  place("{HISCALL}
+0000d3a0: 222c 2073 656c 662e 6361 6c6c 7369 676e  ", self.callsign
+0000d3b0: 2e74 6578 7428 2929 0a20 2020 2020 2020  .text()).       
+0000d3c0: 2069 6620 7365 6c66 2e72 6164 696f 5f73   if self.radio_s
+0000d3d0: 7461 7465 2e67 6574 2822 6d6f 6465 2229  tate.get("mode")
+0000d3e0: 203d 3d20 2243 5722 3a0a 2020 2020 2020   == "CW":.      
+0000d3f0: 2020 2020 2020 6d61 6372 6f20 3d20 6d61        macro = ma
+0000d400: 6372 6f2e 7265 706c 6163 6528 227b 534e  cro.replace("{SN
+0000d410: 547d 222c 2073 656c 662e 7365 6e74 2e74  T}", self.sent.t
+0000d420: 6578 7428 292e 7265 706c 6163 6528 2239  ext().replace("9
+0000d430: 222c 2022 6e22 2929 0a20 2020 2020 2020  ", "n")).       
+0000d440: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000d450: 2020 206d 6163 726f 203d 206d 6163 726f     macro = macro
+0000d460: 2e72 6570 6c61 6365 2822 7b53 4e54 7d22  .replace("{SNT}"
+0000d470: 2c20 7365 6c66 2e73 656e 742e 7465 7874  , self.sent.text
+0000d480: 2829 290a 2020 2020 2020 2020 6d61 6372  ()).        macr
+0000d490: 6f20 3d20 6d61 6372 6f2e 7265 706c 6163  o = macro.replac
+0000d4a0: 6528 227b 5345 4e54 4e52 7d22 2c20 7365  e("{SENTNR}", se
+0000d4b0: 6c66 2e6f 7468 6572 5f31 2e74 6578 7428  lf.other_1.text(
+0000d4c0: 2929 0a20 2020 2020 2020 206d 6163 726f  )).        macro
+0000d4d0: 203d 206d 6163 726f 2e72 6570 6c61 6365   = macro.replace
+0000d4e0: 280a 2020 2020 2020 2020 2020 2020 227b  (.            "{
+0000d4f0: 4558 4348 7d22 2c20 7365 6c66 2e63 6f6e  EXCH}", self.con
+0000d500: 7465 7374 5f73 6574 7469 6e67 732e 6765  test_settings.ge
+0000d510: 7428 2253 656e 7445 7863 6861 6e67 6522  t("SentExchange"
+0000d520: 2c20 2278 7878 2229 0a20 2020 2020 2020  , "xxx").       
+0000d530: 2029 0a20 2020 2020 2020 2072 6574 7572   ).        retur
+0000d540: 6e20 6d61 6372 6f0a 0a20 2020 2064 6566  n macro..    def
+0000d550: 2076 6f69 6365 5f73 7472 696e 6728 7365   voice_string(se
+0000d560: 6c66 2c20 7468 655f 7374 7269 6e67 3a20  lf, the_string: 
+0000d570: 7374 7229 202d 3e20 4e6f 6e65 3a0a 2020  str) -> None:.  
+0000d580: 2020 2020 2020 2222 2276 6f69 6365 7320        """voices 
+0000d590: 7374 7269 6e67 2075 7369 6e67 206e 6174  string using nat
+0000d5a0: 6f20 7068 6f6e 6574 6963 7322 2222 0a20  o phonetics""". 
+0000d5b0: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
+0000d5c0: 6275 6728 2256 6f69 6369 6e67 3a20 2573  bug("Voicing: %s
+0000d5d0: 222c 2074 6865 5f73 7472 696e 6729 0a20  ", the_string). 
+0000d5e0: 2020 2020 2020 206f 705f 7061 7468 203d         op_path =
+0000d5f0: 2050 6174 6828 4441 5441 5f50 4154 4829   Path(DATA_PATH)
+0000d600: 202f 2073 656c 662e 6375 7272 656e 745f   / self.current_
+0000d610: 6f70 0a20 2020 2020 2020 2069 6620 225b  op.        if "[
+0000d620: 2220 696e 2074 6865 5f73 7472 696e 673a  " in the_string:
+0000d630: 0a20 2020 2020 2020 2020 2020 2073 7562  .            sub
+0000d640: 5f73 7472 696e 6720 3d20 7468 655f 7374  _string = the_st
+0000d650: 7269 6e67 2e73 7472 6970 2822 5b5d 2229  ring.strip("[]")
+0000d660: 2e6c 6f77 6572 2829 0a20 2020 2020 2020  .lower().       
+0000d670: 2020 2020 2066 696c 656e 616d 6520 3d20       filename = 
+0000d680: 6622 7b73 7472 286f 705f 7061 7468 297d  f"{str(op_path)}
+0000d690: 2f7b 7375 625f 7374 7269 6e67 7d2e 7761  /{sub_string}.wa
+0000d6a0: 7622 0a20 2020 2020 2020 2020 2020 2069  v".            i
+0000d6b0: 6620 5061 7468 2866 696c 656e 616d 6529  f Path(filename)
+0000d6c0: 2e69 735f 6669 6c65 2829 3a0a 2020 2020  .is_file():.    
+0000d6d0: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+0000d6e0: 6572 2e64 6562 7567 2822 566f 6963 696e  er.debug("Voicin
+0000d6f0: 673a 2025 7322 2c20 6669 6c65 6e61 6d65  g: %s", filename
+0000d700: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000d710: 2020 6461 7461 2c20 5f66 7320 3d20 7366    data, _fs = sf
+0000d720: 2e72 6561 6428 6669 6c65 6e61 6d65 2c20  .read(filename, 
+0000d730: 6474 7970 653d 2266 6c6f 6174 3332 2229  dtype="float32")
+0000d740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d750: 2073 656c 662e 7074 745f 6f6e 2829 0a20   self.ptt_on(). 
+0000d760: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000d770: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+0000d780: 2020 2020 2020 2020 7364 2e64 6566 6175          sd.defau
+0000d790: 6c74 2e64 6576 6963 6520 3d20 7365 6c66  lt.device = self
+0000d7a0: 2e70 7265 662e 6765 7428 2273 6f75 6e64  .pref.get("sound
+0000d7b0: 6465 7669 6365 222c 2022 6465 6661 756c  device", "defaul
+0000d7c0: 7422 290a 2020 2020 2020 2020 2020 2020  t").            
+0000d7d0: 2020 2020 2020 2020 7364 2e64 6566 6175          sd.defau
+0000d7e0: 6c74 2e73 616d 706c 6572 6174 6520 3d20  lt.samplerate = 
+0000d7f0: 3434 3130 302e 300a 2020 2020 2020 2020  44100.0.        
+0000d800: 2020 2020 2020 2020 2020 2020 7364 2e70              sd.p
+0000d810: 6c61 7928 6461 7461 290a 2020 2020 2020  lay(data).      
+0000d820: 2020 2020 2020 2020 2020 2020 2020 5f73                _s
+0000d830: 7461 7475 7320 3d20 7364 2e77 6169 7428  tatus = sd.wait(
+0000d840: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000d850: 2020 2020 2020 2320 6874 7470 733a 2f2f        # https://
+0000d860: 736e 796b 2e69 6f2f 6164 7669 736f 722f  snyk.io/advisor/
+0000d870: 7079 7468 6f6e 2f73 6f75 6e64 6465 7669  python/sounddevi
+0000d880: 6365 2f66 756e 6374 696f 6e73 2f73 6f75  ce/functions/sou
+0000d890: 6e64 6465 7669 6365 2e50 6f72 7441 7564  nddevice.PortAud
+0000d8a0: 696f 4572 726f 720a 2020 2020 2020 2020  ioError.        
+0000d8b0: 2020 2020 2020 2020 6578 6365 7074 2073          except s
+0000d8c0: 642e 506f 7274 4175 6469 6f45 7272 6f72  d.PortAudioError
+0000d8d0: 2061 7320 6572 723a 0a20 2020 2020 2020   as err:.       
+0000d8e0: 2020 2020 2020 2020 2020 2020 206c 6f67               log
+0000d8f0: 6765 722e 7761 726e 696e 6728 2225 7322  ger.warning("%s"
+0000d900: 2c20 6622 7b65 7272 7d22 290a 0a20 2020  , f"{err}")..   
+0000d910: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000d920: 662e 7074 745f 6f66 6628 290a 2020 2020  f.ptt_off().    
+0000d930: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+0000d940: 2020 2020 2020 2073 656c 662e 7074 745f         self.ptt_
+0000d950: 6f6e 2829 0a20 2020 2020 2020 2066 6f72  on().        for
+0000d960: 206c 6574 7465 7220 696e 2074 6865 5f73   letter in the_s
+0000d970: 7472 696e 672e 6c6f 7765 7228 293a 0a20  tring.lower():. 
+0000d980: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
+0000d990: 7474 6572 2069 6e20 2261 6263 6465 6667  tter in "abcdefg
+0000d9a0: 6869 6a6b 6c6d 6e6f 7071 7273 7475 7677  hijklmnopqrstuvw
+0000d9b0: 7879 7a20 3132 3334 3536 3738 3930 223a  xyz 1234567890":
+0000d9c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d9d0: 2069 6620 6c65 7474 6572 203d 3d20 2220   if letter == " 
+0000d9e0: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
+0000d9f0: 2020 2020 2020 206c 6574 7465 7220 3d20         letter = 
+0000da00: 2273 7061 6365 220a 2020 2020 2020 2020  "space".        
+0000da10: 2020 2020 2020 2020 6669 6c65 6e61 6d65          filename
+0000da20: 203d 2066 227b 7374 7228 6f70 5f70 6174   = f"{str(op_pat
+0000da30: 6829 7d2f 7b6c 6574 7465 727d 2e77 6176  h)}/{letter}.wav
+0000da40: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0000da50: 2020 6966 2050 6174 6828 6669 6c65 6e61    if Path(filena
+0000da60: 6d65 292e 6973 5f66 696c 6528 293a 0a20  me).is_file():. 
+0000da70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da80: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+0000da90: 2256 6f69 6369 6e67 3a20 2573 222c 2066  "Voicing: %s", f
+0000daa0: 696c 656e 616d 6529 0a20 2020 2020 2020  ilename).       
+0000dab0: 2020 2020 2020 2020 2020 2020 2064 6174               dat
+0000dac0: 612c 205f 6673 203d 2073 662e 7265 6164  a, _fs = sf.read
+0000dad0: 2866 696c 656e 616d 652c 2064 7479 7065  (filename, dtype
+0000dae0: 3d22 666c 6f61 7433 3222 290a 2020 2020  ="float32").    
 0000daf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db00: 2043 4f4e 4649 475f 5041 5448 202b 2022   CONFIG_PATH + "
-0000db10: 2f6e 6f74 316d 6d2e 6a73 6f6e 222c 2022  /not1mm.json", "
-0000db20: 7774 222c 2065 6e63 6f64 696e 673d 2275  wt", encoding="u
-0000db30: 7466 2d38 220a 2020 2020 2020 2020 2020  tf-8".          
-0000db40: 2020 2020 2020 2920 6173 2066 696c 655f        ) as file_
-0000db50: 6465 7363 7269 7074 6f72 3a0a 2020 2020  descriptor:.    
+0000db00: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+0000db10: 2020 2020 2020 2020 2020 2020 2073 642e               sd.
+0000db20: 6465 6661 756c 742e 6465 7669 6365 203d  default.device =
+0000db30: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
+0000db40: 736f 756e 6464 6576 6963 6522 2c20 2264  sounddevice", "d
+0000db50: 6566 6175 6c74 2229 0a20 2020 2020 2020  efault").       
 0000db60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db70: 7365 6c66 2e70 7265 6620 3d20 7365 6c66  self.pref = self
-0000db80: 2e70 7265 665f 7265 662e 636f 7079 2829  .pref_ref.copy()
+0000db70: 2073 642e 6465 6661 756c 742e 7361 6d70   sd.default.samp
+0000db80: 6c65 7261 7465 203d 2034 3431 3030 2e30  lerate = 44100.0
 0000db90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dba0: 2020 2020 2066 696c 655f 6465 7363 7269       file_descri
-0000dbb0: 7074 6f72 2e77 7269 7465 2864 756d 7073  ptor.write(dumps
-0000dbc0: 2873 656c 662e 7072 6566 2c20 696e 6465  (self.pref, inde
-0000dbd0: 6e74 3d34 2929 0a20 2020 2020 2020 2020  nt=4)).         
-0000dbe0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-0000dbf0: 722e 696e 666f 2822 2573 222c 2073 656c  r.info("%s", sel
-0000dc00: 662e 7072 6566 290a 2020 2020 2020 2020  f.pref).        
-0000dc10: 6578 6365 7074 2049 4f45 7272 6f72 2061  except IOError a
-0000dc20: 7320 6578 6365 7074 696f 6e3a 0a20 2020  s exception:.   
-0000dc30: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-0000dc40: 6372 6974 6963 616c 2822 4572 726f 723a  critical("Error:
-0000dc50: 2025 7322 2c20 6578 6365 7074 696f 6e29   %s", exception)
-0000dc60: 0a0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-0000dc70: 6f6f 6b5f 7570 203d 204e 6f6e 650a 2020  ook_up = None.  
-0000dc80: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
-0000dc90: 6566 2e67 6574 2822 7573 6571 727a 2229  ef.get("useqrz")
-0000dca0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000dcb0: 6c66 2e6c 6f6f 6b5f 7570 203d 2051 525a  lf.look_up = QRZ
-0000dcc0: 6c6f 6f6b 7570 280a 2020 2020 2020 2020  lookup(.        
-0000dcd0: 2020 2020 2020 2020 7365 6c66 2e70 7265          self.pre
-0000dce0: 662e 6765 7428 226c 6f6f 6b75 7075 7365  f.get("lookupuse
-0000dcf0: 726e 616d 6522 292c 0a20 2020 2020 2020  rname"),.       
-0000dd00: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
-0000dd10: 6566 2e67 6574 2822 6c6f 6f6b 7570 7061  ef.get("lookuppa
-0000dd20: 7373 776f 7264 2229 2c0a 2020 2020 2020  ssword"),.      
-0000dd30: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0000dd40: 2320 6966 2073 656c 662e 7072 6566 2e67  # if self.pref.g
-0000dd50: 6574 2822 7573 6568 616d 6462 2229 3a0a  et("usehamdb"):.
-0000dd60: 2020 2020 2020 2020 2320 2020 2020 7365          #     se
-0000dd70: 6c66 2e6c 6f6f 6b5f 7570 203d 2048 616d  lf.look_up = Ham
-0000dd80: 4442 6c6f 6f6b 7570 2829 0a20 2020 2020  DBlookup().     
-0000dd90: 2020 2069 6620 7365 6c66 2e70 7265 662e     if self.pref.
-0000dda0: 6765 7428 2275 7365 6861 6d71 7468 2229  get("usehamqth")
-0000ddb0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000ddc0: 6c66 2e6c 6f6f 6b5f 7570 203d 2048 616d  lf.look_up = Ham
-0000ddd0: 5154 4828 0a20 2020 2020 2020 2020 2020  QTH(.           
-0000dde0: 2020 2020 2073 656c 662e 7072 6566 2e67       self.pref.g
-0000ddf0: 6574 2822 6c6f 6f6b 7570 7573 6572 6e61  et("lookupuserna
-0000de00: 6d65 2229 2c0a 2020 2020 2020 2020 2020  me"),.          
-0000de10: 2020 2020 2020 7365 6c66 2e70 7265 662e        self.pref.
-0000de20: 6765 7428 226c 6f6f 6b75 7070 6173 7377  get("lookuppassw
-0000de30: 6f72 6422 292c 0a20 2020 2020 2020 2020  ord"),.         
-0000de40: 2020 2029 0a0a 2020 2020 2020 2020 6966     )..        if
-0000de50: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
-0000de60: 7275 6e5f 7374 6174 6522 293a 0a20 2020  run_state"):.   
-0000de70: 2020 2020 2020 2020 2073 656c 662e 7261           self.ra
-0000de80: 6469 6f42 7574 746f 6e5f 7275 6e2e 7365  dioButton_run.se
-0000de90: 7443 6865 636b 6564 2854 7275 6529 0a20  tChecked(True). 
-0000dea0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0000deb0: 2020 2020 2020 2020 2073 656c 662e 7261           self.ra
-0000dec0: 6469 6f42 7574 746f 6e5f 7370 2e73 6574  dioButton_sp.set
-0000ded0: 4368 6563 6b65 6428 5472 7565 290a 0a20  Checked(True).. 
-0000dee0: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
-0000def0: 7265 662e 6765 7428 2264 6172 6b5f 6d6f  ref.get("dark_mo
-0000df00: 6465 2229 3a0a 2020 2020 2020 2020 2020  de"):.          
-0000df10: 2020 7365 6c66 2e61 6374 696f 6e44 6172    self.actionDar
-0000df20: 6b5f 4d6f 6465 2e73 6574 4368 6563 6b65  k_Mode.setChecke
-0000df30: 6428 5472 7565 290a 2020 2020 2020 2020  d(True).        
-0000df40: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000df50: 2020 7365 6c66 2e61 6374 696f 6e44 6172    self.actionDar
-0000df60: 6b5f 4d6f 6465 2e73 6574 4368 6563 6b65  k_Mode.setChecke
-0000df70: 6428 4661 6c73 6529 0a0a 2020 2020 2020  d(False)..      
-0000df80: 2020 6966 2073 656c 662e 7072 6566 2e67    if self.pref.g
-0000df90: 6574 2822 636f 6d6d 616e 645f 6275 7474  et("command_butt
-0000dfa0: 6f6e 7322 293a 0a20 2020 2020 2020 2020  ons"):.         
-0000dfb0: 2020 2073 656c 662e 6163 7469 6f6e 436f     self.actionCo
-0000dfc0: 6d6d 616e 645f 4275 7474 6f6e 732e 7365  mmand_Buttons.se
-0000dfd0: 7443 6865 636b 6564 2854 7275 6529 0a20  tChecked(True). 
-0000dfe0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0000dff0: 2020 2020 2020 2020 2073 656c 662e 6163           self.ac
-0000e000: 7469 6f6e 436f 6d6d 616e 645f 4275 7474  tionCommand_Butt
-0000e010: 6f6e 732e 7365 7443 6865 636b 6564 2846  ons.setChecked(F
-0000e020: 616c 7365 290a 0a20 2020 2020 2020 2069  alse)..        i
-0000e030: 6620 7365 6c66 2e70 7265 662e 6765 7428  f self.pref.get(
-0000e040: 2263 775f 6d61 6372 6f73 2229 3a0a 2020  "cw_macros"):.  
-0000e050: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-0000e060: 6374 696f 6e43 575f 4d61 6372 6f73 2e73  ctionCW_Macros.s
-0000e070: 6574 4368 6563 6b65 6428 5472 7565 290a  etChecked(True).
-0000e080: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000e090: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-0000e0a0: 6374 696f 6e43 575f 4d61 6372 6f73 2e73  ctionCW_Macros.s
-0000e0b0: 6574 4368 6563 6b65 6428 4661 6c73 6529  etChecked(False)
-0000e0c0: 0a0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
-0000e0d0: 662e 7072 6566 2e67 6574 2822 6261 6e64  f.pref.get("band
-0000e0e0: 735f 6d6f 6465 7322 293a 0a20 2020 2020  s_modes"):.     
-0000e0f0: 2020 2020 2020 2073 656c 662e 6163 7469         self.acti
-0000e100: 6f6e 4d6f 6465 5f61 6e64 5f42 616e 6473  onMode_and_Bands
-0000e110: 2e73 6574 4368 6563 6b65 6428 5472 7565  .setChecked(True
-0000e120: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-0000e130: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000e140: 2e61 6374 696f 6e4d 6f64 655f 616e 645f  .actionMode_and_
-0000e150: 4261 6e64 732e 7365 7443 6865 636b 6564  Bands.setChecked
-0000e160: 2846 616c 7365 290a 0a20 2020 2020 2020  (False)..       
-0000e170: 206d 756c 7469 6361 7374 5f67 726f 7570   multicast_group
-0000e180: 203d 2073 656c 662e 7072 6566 2e67 6574   = self.pref.get
-0000e190: 2822 6d75 6c74 6963 6173 745f 6772 6f75  ("multicast_grou
-0000e1a0: 7022 2c20 2232 3234 2e31 2e31 2e31 2229  p", "224.1.1.1")
-0000e1b0: 0a20 2020 2020 2020 206d 756c 7469 6361  .        multica
-0000e1c0: 7374 5f70 6f72 7420 3d20 7365 6c66 2e70  st_port = self.p
-0000e1d0: 7265 662e 6765 7428 226d 756c 7469 6361  ref.get("multica
-0000e1e0: 7374 5f70 6f72 7422 2c20 3232 3339 290a  st_port", 2239).
-0000e1f0: 2020 2020 2020 2020 696e 7465 7266 6163          interfac
-0000e200: 655f 6970 203d 2073 656c 662e 7072 6566  e_ip = self.pref
-0000e210: 2e67 6574 2822 696e 7465 7266 6163 655f  .get("interface_
-0000e220: 6970 222c 2022 302e 302e 302e 3022 290a  ip", "0.0.0.0").
-0000e230: 2020 2020 2020 2020 7365 6c66 2e6d 756c          self.mul
-0000e240: 7469 6361 7374 5f69 6e74 6572 6661 6365  ticast_interface
-0000e250: 203d 204d 756c 7469 6361 7374 280a 2020   = Multicast(.  
-0000e260: 2020 2020 2020 2020 2020 6d75 6c74 6963            multic
-0000e270: 6173 745f 6772 6f75 702c 206d 756c 7469  ast_group, multi
-0000e280: 6361 7374 5f70 6f72 742c 2069 6e74 6572  cast_port, inter
-0000e290: 6661 6365 5f69 700a 2020 2020 2020 2020  face_ip.        
-0000e2a0: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-0000e2b0: 7269 675f 636f 6e74 726f 6c20 3d20 4e6f  rig_control = No
-0000e2c0: 6e65 0a0a 2020 2020 2020 2020 6966 2073  ne..        if s
-0000e2d0: 656c 662e 7072 6566 2e67 6574 2822 7573  elf.pref.get("us
-0000e2e0: 6566 6c72 6967 222c 2046 616c 7365 293a  eflrig", False):
-0000e2f0: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
-0000e300: 6765 722e 6465 6275 6728 0a20 2020 2020  ger.debug(.     
-0000e310: 2020 2020 2020 2020 2020 2022 5573 696e             "Usin
-0000e320: 6720 666c 7269 673a 2025 7322 2c0a 2020  g flrig: %s",.  
-0000e330: 2020 2020 2020 2020 2020 2020 2020 6622                f"
-0000e340: 7b73 656c 662e 7072 6566 2e67 6574 2827  {self.pref.get('
-0000e350: 4341 545f 6970 2729 7d20 7b73 656c 662e  CAT_ip')} {self.
-0000e360: 7072 6566 2e67 6574 2827 4341 545f 706f  pref.get('CAT_po
-0000e370: 7274 2729 7d22 2c0a 2020 2020 2020 2020  rt')}",.        
-0000e380: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-0000e390: 2020 7365 6c66 2e72 6967 5f63 6f6e 7472    self.rig_contr
-0000e3a0: 6f6c 203d 2043 4154 280a 2020 2020 2020  ol = CAT(.      
-0000e3b0: 2020 2020 2020 2020 2020 2266 6c72 6967            "flrig
-0000e3c0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-0000e3d0: 2020 2073 656c 662e 7072 6566 2e67 6574     self.pref.get
-0000e3e0: 2822 4341 545f 6970 222c 2022 3132 372e  ("CAT_ip", "127.
-0000e3f0: 302e 302e 3122 292c 0a20 2020 2020 2020  0.0.1"),.       
-0000e400: 2020 2020 2020 2020 2069 6e74 2873 656c           int(sel
-0000e410: 662e 7072 6566 2e67 6574 2822 4341 545f  f.pref.get("CAT_
-0000e420: 706f 7274 222c 2031 3233 3435 2929 2c0a  port", 12345)),.
-0000e430: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0000e440: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
-0000e450: 6566 2e67 6574 2822 7573 6572 6967 6374  ef.get("userigct
-0000e460: 6c64 222c 2046 616c 7365 293a 0a20 2020  ld", False):.   
-0000e470: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-0000e480: 6465 6275 6728 0a20 2020 2020 2020 2020  debug(.         
-0000e490: 2020 2020 2020 2022 5573 696e 6720 7269         "Using ri
-0000e4a0: 6763 746c 643a 2025 7322 2c0a 2020 2020  gctld: %s",.    
-0000e4b0: 2020 2020 2020 2020 2020 2020 6622 7b73              f"{s
-0000e4c0: 656c 662e 7072 6566 2e67 6574 2827 4341  elf.pref.get('CA
-0000e4d0: 545f 6970 2729 7d20 7b73 656c 662e 7072  T_ip')} {self.pr
-0000e4e0: 6566 2e67 6574 2827 4341 545f 706f 7274  ef.get('CAT_port
-0000e4f0: 2729 7d22 2c0a 2020 2020 2020 2020 2020  ')}",.          
-0000e500: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-0000e510: 7365 6c66 2e72 6967 5f63 6f6e 7472 6f6c  self.rig_control
-0000e520: 203d 2043 4154 280a 2020 2020 2020 2020   = CAT(.        
-0000e530: 2020 2020 2020 2020 2272 6967 6374 6c64          "rigctld
-0000e540: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-0000e550: 2020 2073 656c 662e 7072 6566 2e67 6574     self.pref.get
-0000e560: 2822 4341 545f 6970 222c 2022 3132 372e  ("CAT_ip", "127.
-0000e570: 302e 302e 3122 292c 0a20 2020 2020 2020  0.0.1"),.       
-0000e580: 2020 2020 2020 2020 2069 6e74 2873 656c           int(sel
-0000e590: 662e 7072 6566 2e67 6574 2822 4341 545f  f.pref.get("CAT_
-0000e5a0: 706f 7274 222c 2034 3533 3229 292c 0a20  port", 4532)),. 
-0000e5b0: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-0000e5c0: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
-0000e5d0: 6566 2e67 6574 2822 6377 7479 7065 222c  ef.get("cwtype",
-0000e5e0: 2030 2920 3d3d 2030 3a0a 2020 2020 2020   0) == 0:.      
-0000e5f0: 2020 2020 2020 7365 6c66 2e63 7720 3d20        self.cw = 
-0000e600: 4e6f 6e65 0a20 2020 2020 2020 2065 6c73  None.        els
-0000e610: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0000e620: 656c 662e 6377 203d 2043 5728 0a20 2020  elf.cw = CW(.   
-0000e630: 2020 2020 2020 2020 2020 2020 2069 6e74               int
-0000e640: 2873 656c 662e 7072 6566 2e67 6574 2822  (self.pref.get("
-0000e650: 6377 7479 7065 2229 292c 0a20 2020 2020  cwtype")),.     
-0000e660: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000e670: 7072 6566 2e67 6574 2822 6377 6970 2229  pref.get("cwip")
-0000e680: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000e690: 2020 696e 7428 7365 6c66 2e70 7265 662e    int(self.pref.
-0000e6a0: 6765 7428 2263 7770 6f72 7422 2c20 3637  get("cwport", 67
-0000e6b0: 3839 2929 2c0a 2020 2020 2020 2020 2020  89)),.          
-0000e6c0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-0000e6d0: 7365 6c66 2e63 772e 7370 6565 6420 3d20  self.cw.speed = 
-0000e6e0: 3230 0a0a 2020 2020 2020 2020 7365 6c66  20..        self
-0000e6f0: 2e64 6172 6b5f 6d6f 6465 2829 0a20 2020  .dark_mode().   
-0000e700: 2020 2020 2073 656c 662e 7368 6f77 5f63       self.show_c
-0000e710: 6f6d 6d61 6e64 5f62 7574 746f 6e73 2829  ommand_buttons()
-0000e720: 0a20 2020 2020 2020 2073 656c 662e 7368  .        self.sh
-0000e730: 6f77 5f43 575f 6d61 6372 6f73 2829 0a20  ow_CW_macros(). 
-0000e740: 2020 2020 2020 2023 2073 656c 662e 7368         # self.sh
-0000e750: 6f77 5f62 616e 645f 6d6f 6465 2829 0a0a  ow_band_mode()..
-0000e760: 2020 2020 6465 6620 7761 7463 685f 7564      def watch_ud
-0000e770: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
-0000e780: 2022 2222 5075 7473 2055 4450 2064 6174   """Puts UDP dat
-0000e790: 6167 7261 6d73 2069 6e20 6120 4649 464f  agrams in a FIFO
-0000e7a0: 2071 7565 7565 2222 220a 2020 2020 2020   queue""".      
-0000e7b0: 2020 7768 696c 6520 5472 7565 3a0a 2020    while True:.  
-0000e7c0: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
-0000e7d0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-0000e7e0: 6174 6167 7261 6d20 3d20 7365 6c66 2e6d  atagram = self.m
-0000e7f0: 756c 7469 6361 7374 5f69 6e74 6572 6661  ulticast_interfa
-0000e800: 6365 2e73 6572 7665 725f 7564 702e 7265  ce.server_udp.re
-0000e810: 6376 2831 3530 3029 0a20 2020 2020 2020  cv(1500).       
-0000e820: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-0000e830: 6465 6275 6728 6461 7461 6772 616d 2e64  debug(datagram.d
-0000e840: 6563 6f64 6528 2929 0a20 2020 2020 2020  ecode()).       
-0000e850: 2020 2020 2065 7863 6570 7420 736f 636b       except sock
-0000e860: 6574 2e74 696d 656f 7574 3a0a 2020 2020  et.timeout:.    
-0000e870: 2020 2020 2020 2020 2020 2020 7469 6d65              time
-0000e880: 2e73 6c65 6570 2830 2e31 290a 2020 2020  .sleep(0.1).    
-0000e890: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-0000e8a0: 696e 7565 0a20 2020 2020 2020 2020 2020  inue.           
-0000e8b0: 2069 6620 6461 7461 6772 616d 3a0a 2020   if datagram:.  
-0000e8c0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000e8d0: 6c66 2e75 6470 5f66 6966 6f2e 7075 7428  lf.udp_fifo.put(
-0000e8e0: 6461 7461 6772 616d 290a 0a20 2020 2064  datagram)..    d
-0000e8f0: 6566 2063 6865 636b 5f75 6470 5f74 7261  ef check_udp_tra
-0000e900: 6666 6963 2873 656c 6629 3a0a 2020 2020  ffic(self):.    
-0000e910: 2020 2020 2222 2243 6865 636b 7320 5544      """Checks UD
-0000e920: 5020 5472 6166 6669 6322 2222 0a20 2020  P Traffic""".   
-0000e930: 2020 2020 2077 6869 6c65 206e 6f74 2073       while not s
-0000e940: 656c 662e 7564 705f 6669 666f 2e65 6d70  elf.udp_fifo.emp
-0000e950: 7479 2829 3a0a 2020 2020 2020 2020 2020  ty():.          
-0000e960: 2020 6461 7461 6772 616d 203d 2073 656c    datagram = sel
-0000e970: 662e 7564 705f 6669 666f 2e67 6574 2829  f.udp_fifo.get()
-0000e980: 0a20 2020 2020 2020 2020 2020 2074 7279  .            try
-0000e990: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000e9a0: 2020 6465 6275 675f 696e 666f 203d 2066    debug_info = f
-0000e9b0: 227b 6461 7461 6772 616d 2e64 6563 6f64  "{datagram.decod
-0000e9c0: 6528 297d 220a 2020 2020 2020 2020 2020  e()}".          
-0000e9d0: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-0000e9e0: 7567 2864 6562 7567 5f69 6e66 6f29 0a20  ug(debug_info). 
-0000e9f0: 2020 2020 2020 2020 2020 2020 2020 206a                 j
-0000ea00: 736f 6e5f 6461 7461 203d 206c 6f61 6473  son_data = loads
-0000ea10: 2864 6174 6167 7261 6d2e 6465 636f 6465  (datagram.decode
-0000ea20: 2829 290a 2020 2020 2020 2020 2020 2020  ()).            
-0000ea30: 6578 6365 7074 2055 6e69 636f 6465 4465  except UnicodeDe
-0000ea40: 636f 6465 4572 726f 7220 6173 2065 7272  codeError as err
-0000ea50: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000ea60: 2020 7468 655f 6572 726f 7220 3d20 6622    the_error = f"
-0000ea70: 4e6f 7420 556e 6963 6f64 653a 207b 6572  Not Unicode: {er
-0000ea80: 727d 5c6e 7b64 6174 6167 7261 6d7d 220a  r}\n{datagram}".
-0000ea90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eaa0: 6c6f 6767 6572 2e64 6562 7567 2874 6865  logger.debug(the
-0000eab0: 5f65 7272 6f72 290a 2020 2020 2020 2020  _error).        
-0000eac0: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
-0000ead0: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
-0000eae0: 6570 7420 4a53 4f4e 4465 636f 6465 4572  ept JSONDecodeEr
-0000eaf0: 726f 7220 6173 2065 7272 3a0a 2020 2020  ror as err:.    
-0000eb00: 2020 2020 2020 2020 2020 2020 7468 655f              the_
-0000eb10: 6572 726f 7220 3d20 6622 4e6f 7420 4a53  error = f"Not JS
-0000eb20: 4f4e 3a20 7b65 7272 7d5c 6e7b 6461 7461  ON: {err}\n{data
-0000eb30: 6772 616d 7d22 0a20 2020 2020 2020 2020  gram}".         
-0000eb40: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-0000eb50: 6275 6728 7468 655f 6572 726f 7229 0a20  bug(the_error). 
-0000eb60: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000eb70: 6f6e 7469 6e75 650a 2020 2020 2020 2020  ontinue.        
-0000eb80: 2020 2020 6966 2028 0a20 2020 2020 2020      if (.       
-0000eb90: 2020 2020 2020 2020 206a 736f 6e5f 6461           json_da
-0000eba0: 7461 2e67 6574 2822 636d 6422 2c20 2222  ta.get("cmd", ""
-0000ebb0: 2920 3d3d 2022 4745 5443 4f4c 554d 4e53  ) == "GETCOLUMNS
-0000ebc0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-0000ebd0: 2020 616e 6420 6a73 6f6e 5f64 6174 612e    and json_data.
-0000ebe0: 6765 7428 2273 7461 7469 6f6e 222c 2022  get("station", "
-0000ebf0: 2229 203d 3d20 706c 6174 666f 726d 2e6e  ") == platform.n
-0000ec00: 6f64 6528 290a 2020 2020 2020 2020 2020  ode().          
-0000ec10: 2020 293a 0a20 2020 2020 2020 2020 2020    ):.           
-0000ec20: 2020 2020 2069 6620 6861 7361 7474 7228       if hasattr(
-0000ec30: 7365 6c66 2e63 6f6e 7465 7374 2c20 2263  self.contest, "c
-0000ec40: 6f6c 756d 6e73 2229 3a0a 2020 2020 2020  olumns"):.      
-0000ec50: 2020 2020 2020 2020 2020 2020 2020 636d                cm
-0000ec60: 6420 3d20 7b7d 0a20 2020 2020 2020 2020  d = {}.         
-0000ec70: 2020 2020 2020 2020 2020 2063 6d64 5b22             cmd["
-0000ec80: 636d 6422 5d20 3d20 2253 484f 5743 4f4c  cmd"] = "SHOWCOL
-0000ec90: 554d 4e53 220a 2020 2020 2020 2020 2020  UMNS".          
-0000eca0: 2020 2020 2020 2020 2020 636d 645b 2273            cmd["s
-0000ecb0: 7461 7469 6f6e 225d 203d 2070 6c61 7466  tation"] = platf
-0000ecc0: 6f72 6d2e 6e6f 6465 2829 0a20 2020 2020  orm.node().     
-0000ecd0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000ece0: 6d64 5b22 434f 4c55 4d4e 5322 5d20 3d20  md["COLUMNS"] = 
-0000ecf0: 7365 6c66 2e63 6f6e 7465 7374 2e63 6f6c  self.contest.col
-0000ed00: 756d 6e73 0a20 2020 2020 2020 2020 2020  umns.           
-0000ed10: 2020 2020 2020 2020 2073 656c 662e 6d75           self.mu
-0000ed20: 6c74 6963 6173 745f 696e 7465 7266 6163  lticast_interfac
-0000ed30: 652e 7365 6e64 5f61 735f 6a73 6f6e 2863  e.send_as_json(c
-0000ed40: 6d64 290a 2020 2020 2020 2020 2020 2020  md).            
-0000ed50: 6966 2028 0a20 2020 2020 2020 2020 2020  if (.           
-0000ed60: 2020 2020 206a 736f 6e5f 6461 7461 2e67       json_data.g
-0000ed70: 6574 2822 636d 6422 2c20 2222 2920 3d3d  et("cmd", "") ==
-0000ed80: 2022 5455 4e45 220a 2020 2020 2020 2020   "TUNE".        
-0000ed90: 2020 2020 2020 2020 616e 6420 6a73 6f6e          and json
-0000eda0: 5f64 6174 612e 6765 7428 2273 7461 7469  _data.get("stati
-0000edb0: 6f6e 222c 2022 2229 203d 3d20 706c 6174  on", "") == plat
-0000edc0: 666f 726d 2e6e 6f64 6528 290a 2020 2020  form.node().    
-0000edd0: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
-0000ede0: 2020 2020 2020 2020 2020 2023 2062 277b             # b'{
-0000edf0: 2263 6d64 223a 2022 5455 4e45 222c 2022  "cmd": "TUNE", "
-0000ee00: 6672 6571 223a 2037 2e30 3233 352c 2022  freq": 7.0235, "
-0000ee10: 7370 6f74 223a 2022 4d4d 3044 4749 227d  spot": "MM0DGI"}
-0000ee20: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
-0000ee30: 2020 7666 6f20 3d20 6a73 6f6e 5f64 6174    vfo = json_dat
-0000ee40: 612e 6765 7428 2266 7265 7122 290a 2020  a.get("freq").  
-0000ee50: 2020 2020 2020 2020 2020 2020 2020 7666                vf
-0000ee60: 6f20 3d20 666c 6f61 7428 7666 6f29 202a  o = float(vfo) *
-0000ee70: 2031 3030 3030 3030 0a20 2020 2020 2020   1000000.       
-0000ee80: 2020 2020 2020 2020 2073 656c 662e 7261           self.ra
-0000ee90: 6469 6f5f 7374 6174 655b 2276 666f 6122  dio_state["vfoa"
-0000eea0: 5d20 3d20 696e 7428 7666 6f29 0a20 2020  ] = int(vfo).   
-0000eeb0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000eec0: 7365 6c66 2e72 6967 5f63 6f6e 7472 6f6c  self.rig_control
-0000eed0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000eee0: 2020 2020 2020 7365 6c66 2e72 6967 5f63        self.rig_c
-0000eef0: 6f6e 7472 6f6c 2e73 6574 5f76 666f 2869  ontrol.set_vfo(i
-0000ef00: 6e74 2876 666f 2929 0a20 2020 2020 2020  nt(vfo)).       
-0000ef10: 2020 2020 2020 2020 2073 706f 7420 3d20           spot = 
-0000ef20: 6a73 6f6e 5f64 6174 612e 6765 7428 2273  json_data.get("s
-0000ef30: 706f 7422 2c20 2222 290a 2020 2020 2020  pot", "").      
-0000ef40: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-0000ef50: 616c 6c73 6967 6e2e 7365 7454 6578 7428  allsign.setText(
-0000ef60: 7370 6f74 290a 2020 2020 2020 2020 2020  spot).          
-0000ef70: 2020 2020 2020 7365 6c66 2e63 616c 6c73        self.calls
-0000ef80: 6967 6e5f 6368 616e 6765 6428 290a 2020  ign_changed().  
-0000ef90: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000efa0: 6c66 2e63 616c 6c73 6967 6e2e 7365 7446  lf.callsign.setF
-0000efb0: 6f63 7573 2829 0a20 2020 2020 2020 2020  ocus().         
-0000efc0: 2020 2020 2020 2073 656c 662e 6361 6c6c         self.call
-0000efd0: 7369 676e 2e61 6374 6976 6174 6557 696e  sign.activateWin
-0000efe0: 646f 7728 290a 2020 2020 2020 2020 2020  dow().          
-0000eff0: 2020 2020 2020 7769 6e64 6f77 2e72 6169        window.rai
-0000f000: 7365 5f28 290a 0a20 2020 2064 6566 2064  se_()..    def d
-0000f010: 6172 6b5f 6d6f 6465 5f73 7461 7465 5f63  ark_mode_state_c
-0000f020: 6861 6e67 6528 7365 6c66 293a 0a20 2020  hange(self):.   
-0000f030: 2020 2020 2022 2222 6461 726b 6d6f 6465       """darkmode
-0000f040: 2064 726f 7064 6f77 6e20 6368 6563 6b6d   dropdown checkm
-0000f050: 6172 6b20 6368 616e 6765 6422 2222 0a20  ark changed""". 
-0000f060: 2020 2020 2020 2073 656c 662e 7072 6566         self.pref
-0000f070: 5b22 6461 726b 5f6d 6f64 6522 5d20 3d20  ["dark_mode"] = 
-0000f080: 7365 6c66 2e61 6374 696f 6e44 6172 6b5f  self.actionDark_
-0000f090: 4d6f 6465 2e69 7343 6865 636b 6564 2829  Mode.isChecked()
-0000f0a0: 0a20 2020 2020 2020 2073 656c 662e 7772  .        self.wr
-0000f0b0: 6974 655f 7072 6566 6572 656e 6365 2829  ite_preference()
-0000f0c0: 0a20 2020 2020 2020 2073 656c 662e 6461  .        self.da
-0000f0d0: 726b 5f6d 6f64 6528 290a 0a20 2020 2064  rk_mode()..    d
-0000f0e0: 6566 2064 6172 6b5f 6d6f 6465 2873 656c  ef dark_mode(sel
-0000f0f0: 6629 3a0a 2020 2020 2020 2020 2222 2263  f):.        """c
-0000f100: 6861 6e67 6520 6469 7370 6c61 7920 6d6f  hange display mo
-0000f110: 6465 2222 220a 2020 2020 2020 2020 6966  de""".        if
-0000f120: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
-0000f130: 6461 726b 5f6d 6f64 6522 293a 0a20 2020  dark_mode"):.   
-0000f140: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-0000f150: 7453 7479 6c65 5368 6565 7428 4441 524b  tStyleSheet(DARK
-0000f160: 5f53 5459 4c45 5348 4545 5429 0a20 2020  _STYLESHEET).   
-0000f170: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000f180: 2020 2020 2020 2073 656c 662e 7365 7453         self.setS
-0000f190: 7479 6c65 5368 6565 7428 2222 290a 0a20  tyleSheet("").. 
-0000f1a0: 2020 2064 6566 2063 775f 6d61 6372 6f73     def cw_macros
-0000f1b0: 5f73 7461 7465 5f63 6861 6e67 6564 2873  _state_changed(s
-0000f1c0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-0000f1d0: 224d 656e 7520 6974 656d 2074 6f20 7368  "Menu item to sh
-0000f1e0: 6f77 2f68 6964 6520 6d61 6372 6f20 6275  ow/hide macro bu
-0000f1f0: 7474 6f6e 7322 2222 0a20 2020 2020 2020  ttons""".       
-0000f200: 2073 656c 662e 7072 6566 5b22 6377 5f6d   self.pref["cw_m
-0000f210: 6163 726f 7322 5d20 3d20 7365 6c66 2e61  acros"] = self.a
-0000f220: 6374 696f 6e43 575f 4d61 6372 6f73 2e69  ctionCW_Macros.i
-0000f230: 7343 6865 636b 6564 2829 0a20 2020 2020  sChecked().     
-0000f240: 2020 2073 656c 662e 7772 6974 655f 7072     self.write_pr
-0000f250: 6566 6572 656e 6365 2829 0a20 2020 2020  eference().     
-0000f260: 2020 2073 656c 662e 7368 6f77 5f43 575f     self.show_CW_
-0000f270: 6d61 6372 6f73 2829 0a0a 2020 2020 6465  macros()..    de
-0000f280: 6620 7368 6f77 5f43 575f 6d61 6372 6f73  f show_CW_macros
-0000f290: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000f2a0: 2222 226d 6163 726f 2062 7574 746f 6e20  """macro button 
-0000f2b0: 7374 6174 6520 6368 616e 6765 2222 220a  state change""".
-0000f2c0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000f2d0: 7072 6566 2e67 6574 2822 6377 5f6d 6163  pref.get("cw_mac
-0000f2e0: 726f 7322 293a 0a20 2020 2020 2020 2020  ros"):.         
-0000f2f0: 2020 2073 656c 662e 4275 7474 6f6e 5f52     self.Button_R
-0000f300: 6f77 312e 7368 6f77 2829 0a20 2020 2020  ow1.show().     
-0000f310: 2020 2020 2020 2073 656c 662e 4275 7474         self.Butt
-0000f320: 6f6e 5f52 6f77 322e 7368 6f77 2829 0a20  on_Row2.show(). 
-0000f330: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0000f340: 2020 2020 2020 2020 2073 656c 662e 4275           self.Bu
-0000f350: 7474 6f6e 5f52 6f77 312e 6869 6465 2829  tton_Row1.hide()
-0000f360: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000f370: 662e 4275 7474 6f6e 5f52 6f77 322e 6869  f.Button_Row2.hi
-0000f380: 6465 2829 0a0a 2020 2020 6465 6620 636f  de()..    def co
-0000f390: 6d6d 616e 645f 6275 7474 6f6e 735f 7374  mmand_buttons_st
-0000f3a0: 6174 655f 6368 616e 6765 2873 656c 6629  ate_change(self)
-0000f3b0: 3a0a 2020 2020 2020 2020 2222 224d 656e  :.        """Men
-0000f3c0: 7520 6974 656d 2074 6f20 7368 6f77 2f68  u item to show/h
-0000f3d0: 6964 6520 636f 6d6d 616e 6420 6275 7474  ide command butt
-0000f3e0: 6f6e 7322 2222 0a20 2020 2020 2020 2073  ons""".        s
-0000f3f0: 656c 662e 7072 6566 5b22 636f 6d6d 616e  elf.pref["comman
-0000f400: 645f 6275 7474 6f6e 7322 5d20 3d20 7365  d_buttons"] = se
-0000f410: 6c66 2e61 6374 696f 6e43 6f6d 6d61 6e64  lf.actionCommand
-0000f420: 5f42 7574 746f 6e73 2e69 7343 6865 636b  _Buttons.isCheck
-0000f430: 6564 2829 0a20 2020 2020 2020 2073 656c  ed().        sel
-0000f440: 662e 7772 6974 655f 7072 6566 6572 656e  f.write_preferen
-0000f450: 6365 2829 0a20 2020 2020 2020 2073 656c  ce().        sel
-0000f460: 662e 7368 6f77 5f63 6f6d 6d61 6e64 5f62  f.show_command_b
-0000f470: 7574 746f 6e73 2829 0a0a 2020 2020 6465  uttons()..    de
-0000f480: 6620 7368 6f77 5f63 6f6d 6d61 6e64 5f62  f show_command_b
-0000f490: 7574 746f 6e73 2873 656c 6629 3a0a 2020  uttons(self):.  
-0000f4a0: 2020 2020 2020 2222 2263 6f6d 6d61 6e64        """command
-0000f4b0: 2062 7574 746f 6e20 7374 6174 6520 6368   button state ch
-0000f4c0: 616e 6765 2222 220a 2020 2020 2020 2020  ange""".        
-0000f4d0: 6966 2073 656c 662e 7072 6566 2e67 6574  if self.pref.get
-0000f4e0: 2822 636f 6d6d 616e 645f 6275 7474 6f6e  ("command_button
-0000f4f0: 7322 293a 0a20 2020 2020 2020 2020 2020  s"):.           
-0000f500: 2073 656c 662e 436f 6d6d 616e 645f 4275   self.Command_Bu
-0000f510: 7474 6f6e 732e 7368 6f77 2829 0a20 2020  ttons.show().   
-0000f520: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000f530: 2020 2020 2020 2073 656c 662e 436f 6d6d         self.Comm
-0000f540: 616e 645f 4275 7474 6f6e 732e 6869 6465  and_Buttons.hide
-0000f550: 2829 0a0a 2020 2020 6465 6620 6973 5f66  ()..    def is_f
-0000f560: 6c6f 6174 6162 6c65 2873 656c 662c 2069  loatable(self, i
-0000f570: 7465 6d3a 2073 7472 2920 2d3e 2062 6f6f  tem: str) -> boo
-0000f580: 6c3a 0a20 2020 2020 2020 2022 2222 6368  l:.        """ch
-0000f590: 6563 6b20 746f 2073 6565 2069 6620 7374  eck to see if st
-0000f5a0: 7269 6e67 2063 616e 2062 6520 6120 666c  ring can be a fl
-0000f5b0: 6f61 7422 2222 0a20 2020 2020 2020 2069  oat""".        i
-0000f5c0: 6620 6974 656d 2e69 736e 756d 6572 6963  f item.isnumeric
-0000f5d0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-0000f5e0: 7265 7475 726e 2054 7275 650a 2020 2020  return True.    
-0000f5f0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-0000f600: 2020 2020 205f 7465 7374 203d 2066 6c6f       _test = flo
-0000f610: 6174 2869 7465 6d29 0a20 2020 2020 2020  at(item).       
-0000f620: 2065 7863 6570 7420 5661 6c75 6545 7272   except ValueErr
-0000f630: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
-0000f640: 7265 7475 726e 2046 616c 7365 0a20 2020  return False.   
-0000f650: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
-0000f660: 0a0a 2020 2020 6465 6620 6f74 6865 725f  ..    def other_
-0000f670: 325f 6368 616e 6765 6428 7365 6c66 293a  2_changed(self):
-0000f680: 0a20 2020 2020 2020 2022 2222 4361 6c6c  .        """Call
-0000f690: 6564 2077 6865 6e20 7765 206e 6565 6420  ed when we need 
-0000f6a0: 746f 2070 6172 7365 2053 5320 6578 6368  to parse SS exch
-0000f6b0: 616e 6765 2e22 2222 0a20 2020 2020 2020  ange.""".       
-0000f6c0: 2069 6620 7365 6c66 2e63 6f6e 7465 7374   if self.contest
-0000f6d0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-0000f6e0: 2022 4152 524c 2053 7765 6570 7374 616b   "ARRL Sweepstak
-0000f6f0: 6573 2220 696e 2073 656c 662e 636f 6e74  es" in self.cont
-0000f700: 6573 742e 6e61 6d65 3a0a 2020 2020 2020  est.name:.      
-0000f710: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-0000f720: 6f6e 7465 7374 2e70 6172 7365 5f65 7863  ontest.parse_exc
-0000f730: 6861 6e67 6528 7365 6c66 290a 0a20 2020  hange(self)..   
-0000f740: 2064 6566 2063 616c 6c73 6967 6e5f 6368   def callsign_ch
-0000f750: 616e 6765 6428 7365 6c66 293a 0a20 2020  anged(self):.   
-0000f760: 2020 2020 2022 2222 4361 6c6c 6564 2077       """Called w
-0000f770: 6865 6e20 7465 7874 2069 6e20 7468 6520  hen text in the 
-0000f780: 6361 6c6c 7369 676e 2066 6965 6c64 2068  callsign field h
-0000f790: 6173 2063 6861 6e67 6564 2222 220a 2020  as changed""".  
-0000f7a0: 2020 2020 2020 7465 7874 203d 2073 656c        text = sel
-0000f7b0: 662e 6361 6c6c 7369 676e 2e74 6578 7428  f.callsign.text(
-0000f7c0: 290a 2020 2020 2020 2020 7465 7874 203d  ).        text =
-0000f7d0: 2074 6578 742e 7570 7065 7228 290a 2020   text.upper().  
-0000f7e0: 2020 2020 2020 706f 7369 7469 6f6e 203d        position =
-0000f7f0: 2073 656c 662e 6361 6c6c 7369 676e 2e63   self.callsign.c
-0000f800: 7572 736f 7250 6f73 6974 696f 6e28 290a  ursorPosition().
-0000f810: 2020 2020 2020 2020 7374 7269 7070 6564          stripped
-0000f820: 5f74 6578 7420 3d20 7465 7874 2e73 7472  _text = text.str
-0000f830: 6970 2829 2e72 6570 6c61 6365 2822 2022  ip().replace(" "
-0000f840: 2c20 2222 290a 2020 2020 2020 2020 7365  , "").        se
-0000f850: 6c66 2e63 616c 6c73 6967 6e2e 7365 7454  lf.callsign.setT
-0000f860: 6578 7428 7374 7269 7070 6564 5f74 6578  ext(stripped_tex
-0000f870: 7429 0a20 2020 2020 2020 2073 656c 662e  t).        self.
-0000f880: 6361 6c6c 7369 676e 2e73 6574 4375 7273  callsign.setCurs
-0000f890: 6f72 506f 7369 7469 6f6e 2870 6f73 6974  orPosition(posit
-0000f8a0: 696f 6e29 0a0a 2020 2020 2020 2020 6966  ion)..        if
-0000f8b0: 2022 2022 2069 6e20 7465 7874 3a0a 2020   " " in text:.  
-0000f8c0: 2020 2020 2020 2020 2020 6966 2073 7472            if str
-0000f8d0: 6970 7065 645f 7465 7874 203d 3d20 2243  ipped_text == "C
-0000f8e0: 5722 3a0a 2020 2020 2020 2020 2020 2020  W":.            
-0000f8f0: 2020 2020 7365 6c66 2e73 6574 6d6f 6465      self.setmode
-0000f900: 2822 4357 2229 0a20 2020 2020 2020 2020  ("CW").         
-0000f910: 2020 2020 2020 2073 656c 662e 7261 6469         self.radi
-0000f920: 6f5f 7374 6174 655b 226d 6f64 6522 5d20  o_state["mode"] 
-0000f930: 3d20 2243 5722 0a20 2020 2020 2020 2020  = "CW".         
-0000f940: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
-0000f950: 6967 5f63 6f6e 7472 6f6c 3a0a 2020 2020  ig_control:.    
-0000f960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f970: 6966 2073 656c 662e 7269 675f 636f 6e74  if self.rig_cont
-0000f980: 726f 6c2e 6f6e 6c69 6e65 3a0a 2020 2020  rol.online:.    
-0000f990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f9a0: 2020 2020 7365 6c66 2e72 6967 5f63 6f6e      self.rig_con
-0000f9b0: 7472 6f6c 2e73 6574 5f6d 6f64 6528 2243  trol.set_mode("C
-0000f9c0: 5722 290a 2020 2020 2020 2020 2020 2020  W").            
-0000f9d0: 2020 2020 7365 6c66 2e73 6574 5f77 696e      self.set_win
-0000f9e0: 646f 775f 7469 746c 6528 290a 2020 2020  dow_title().    
-0000f9f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000fa00: 2e63 6c65 6172 696e 7075 7473 2829 0a20  .clearinputs(). 
-0000fa10: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000fa20: 656c 662e 7265 6164 5f63 775f 6d61 6372  elf.read_cw_macr
-0000fa30: 6f73 2829 0a20 2020 2020 2020 2020 2020  os().           
-0000fa40: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
-0000fa50: 2020 2020 2020 2020 6966 2073 7472 6970          if strip
-0000fa60: 7065 645f 7465 7874 203d 3d20 2252 5454  ped_text == "RTT
-0000fa70: 5922 3a0a 2020 2020 2020 2020 2020 2020  Y":.            
-0000fa80: 2020 2020 7365 6c66 2e73 6574 6d6f 6465      self.setmode
-0000fa90: 2822 5254 5459 2229 0a20 2020 2020 2020  ("RTTY").       
-0000faa0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-0000fab0: 2e72 6967 5f63 6f6e 7472 6f6c 3a0a 2020  .rig_control:.  
-0000fac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fad0: 2020 6966 2073 656c 662e 7269 675f 636f    if self.rig_co
-0000fae0: 6e74 726f 6c2e 6f6e 6c69 6e65 3a0a 2020  ntrol.online:.  
-0000faf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fb00: 2020 2020 2020 7365 6c66 2e72 6967 5f63        self.rig_c
-0000fb10: 6f6e 7472 6f6c 2e73 6574 5f6d 6f64 6528  ontrol.set_mode(
-0000fb20: 2252 5454 5922 290a 2020 2020 2020 2020  "RTTY").        
-0000fb30: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0000fb40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000fb50: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-0000fb60: 6164 696f 5f73 7461 7465 5b22 6d6f 6465  adio_state["mode
-0000fb70: 225d 203d 2022 5254 5459 220a 2020 2020  "] = "RTTY".    
-0000fb80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000fb90: 2e73 6574 5f77 696e 646f 775f 7469 746c  .set_window_titl
-0000fba0: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
-0000fbb0: 2020 2020 7365 6c66 2e63 6c65 6172 696e      self.clearin
-0000fbc0: 7075 7473 2829 0a20 2020 2020 2020 2020  puts().         
-0000fbd0: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
-0000fbe0: 2020 2020 2020 2020 2020 6966 2073 7472            if str
-0000fbf0: 6970 7065 645f 7465 7874 203d 3d20 2253  ipped_text == "S
-0000fc00: 5342 223a 0a20 2020 2020 2020 2020 2020  SB":.           
-0000fc10: 2020 2020 2073 656c 662e 7365 746d 6f64       self.setmod
-0000fc20: 6528 2253 5342 2229 0a20 2020 2020 2020  e("SSB").       
-0000fc30: 2020 2020 2020 2020 2069 6620 696e 7428           if int(
-0000fc40: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
-0000fc50: 2e67 6574 2822 7666 6f61 222c 2030 2929  .get("vfoa", 0))
-0000fc60: 203e 2031 3030 3030 3030 303a 0a20 2020   > 10000000:.   
-0000fc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fc80: 2073 656c 662e 7261 6469 6f5f 7374 6174   self.radio_stat
-0000fc90: 655b 226d 6f64 6522 5d20 3d20 2255 5342  e["mode"] = "USB
-0000fca0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-0000fcb0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000fcc0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000fcd0: 2e72 6164 696f 5f73 7461 7465 5b22 6d6f  .radio_state["mo
-0000fce0: 6465 225d 203d 2022 4c53 4222 0a20 2020  de"] = "LSB".   
-0000fcf0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000fd00: 662e 7365 745f 7769 6e64 6f77 5f74 6974  f.set_window_tit
-0000fd10: 6c65 2829 0a20 2020 2020 2020 2020 2020  le().           
-0000fd20: 2020 2020 2069 6620 7365 6c66 2e72 6967       if self.rig
-0000fd30: 5f63 6f6e 7472 6f6c 3a0a 2020 2020 2020  _control:.      
-0000fd40: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000fd50: 6c66 2e72 6967 5f63 6f6e 7472 6f6c 2e73  lf.rig_control.s
-0000fd60: 6574 5f6d 6f64 6528 7365 6c66 2e72 6164  et_mode(self.rad
-0000fd70: 696f 5f73 7461 7465 2e67 6574 2822 6d6f  io_state.get("mo
-0000fd80: 6465 2229 290a 2020 2020 2020 2020 2020  de")).          
-0000fd90: 2020 2020 2020 7365 6c66 2e63 6c65 6172        self.clear
-0000fda0: 696e 7075 7473 2829 0a20 2020 2020 2020  inputs().       
-0000fdb0: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
-0000fdc0: 6164 5f63 775f 6d61 6372 6f73 2829 0a20  ad_cw_macros(). 
-0000fdd0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000fde0: 6574 7572 6e0a 2020 2020 2020 2020 2020  eturn.          
-0000fdf0: 2020 6966 2073 7472 6970 7065 645f 7465    if stripped_te
-0000fe00: 7874 203d 3d20 224f 504f 4e22 3a0a 2020  xt == "OPON":.  
-0000fe10: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000fe20: 6c66 2e67 6574 5f6f 706f 6e28 290a 2020  lf.get_opon().  
-0000fe30: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000fe40: 6c66 2e63 6c65 6172 696e 7075 7473 2829  lf.clearinputs()
-0000fe50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fe60: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
-0000fe70: 2020 2020 6966 2073 7472 6970 7065 645f      if stripped_
-0000fe80: 7465 7874 203d 3d20 2254 4553 5422 3a0a  text == "TEST":.
-0000fe90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fea0: 7365 6c66 2e73 686f 775f 6d65 7373 6167  self.show_messag
-0000feb0: 655f 626f 7828 2254 6869 7320 6973 2061  e_box("This is a
-0000fec0: 2074 6573 7422 290a 2020 2020 2020 2020   test").        
-0000fed0: 2020 2020 2020 2020 7365 6c66 2e63 6c65          self.cle
-0000fee0: 6172 696e 7075 7473 2829 0a20 2020 2020  arinputs().     
-0000fef0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000ff00: 6e0a 2020 2020 2020 2020 2020 2020 6966  n.            if
-0000ff10: 2073 656c 662e 6973 5f66 6c6f 6174 6162   self.is_floatab
-0000ff20: 6c65 2873 7472 6970 7065 645f 7465 7874  le(stripped_text
-0000ff30: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000ff40: 2020 2076 666f 203d 2066 6c6f 6174 2873     vfo = float(s
-0000ff50: 7472 6970 7065 645f 7465 7874 290a 2020  tripped_text).  
-0000ff60: 2020 2020 2020 2020 2020 2020 2020 7666                vf
-0000ff70: 6f20 3d20 696e 7428 7666 6f20 2a20 3130  o = int(vfo * 10
-0000ff80: 3030 290a 2020 2020 2020 2020 2020 2020  00).            
-0000ff90: 2020 2020 6261 6e64 203d 2067 6574 6261      band = getba
-0000ffa0: 6e64 2873 7472 2876 666f 2929 0a20 2020  nd(str(vfo)).   
-0000ffb0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000ffc0: 662e 7365 745f 6261 6e64 5f69 6e64 6963  f.set_band_indic
-0000ffd0: 6174 6f72 2862 616e 6429 0a20 2020 2020  ator(band).     
-0000ffe0: 2020 2020 2020 2020 2020 2023 2073 656c             # sel
-0000fff0: 662e 636f 6e74 6163 745b 2242 616e 6422  f.contact["Band"
-00010000: 5d20 3d20 6765 745f 6c6f 6767 6564 5f62  ] = get_logged_b
-00010010: 616e 6428 7374 7228 7365 6c66 2e72 6164  and(str(self.rad
-00010020: 696f 5f73 7461 7465 2e67 6574 2822 7666  io_state.get("vf
-00010030: 6f61 222c 2030 2e30 2929 290a 2020 2020  oa", 0.0))).    
-00010040: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00010050: 2e72 6164 696f 5f73 7461 7465 5b22 7666  .radio_state["vf
-00010060: 6f61 225d 203d 2076 666f 0a20 2020 2020  oa"] = vfo.     
-00010070: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00010080: 7365 745f 7769 6e64 6f77 5f74 6974 6c65  set_window_title
-00010090: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-000100a0: 2020 2073 656c 662e 636c 6561 7269 6e70     self.clearinp
-000100b0: 7574 7328 290a 2020 2020 2020 2020 2020  uts().          
-000100c0: 2020 2020 2020 6966 2073 656c 662e 7269        if self.ri
-000100d0: 675f 636f 6e74 726f 6c3a 0a20 2020 2020  g_control:.     
-000100e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000100f0: 656c 662e 7269 675f 636f 6e74 726f 6c2e  elf.rig_control.
-00010100: 7365 745f 7666 6f28 7666 6f29 0a20 2020  set_vfo(vfo).   
-00010110: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00010120: 7572 6e0a 0a20 2020 2020 2020 2020 2020  urn..           
-00010130: 2073 656c 662e 6368 6563 6b5f 6361 6c6c   self.check_call
-00010140: 7369 676e 2873 7472 6970 7065 645f 7465  sign(stripped_te
-00010150: 7874 290a 2020 2020 2020 2020 2020 2020  xt).            
-00010160: 6966 2073 656c 662e 6368 6563 6b5f 6475  if self.check_du
-00010170: 7065 2873 7472 6970 7065 645f 7465 7874  pe(stripped_text
-00010180: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00010190: 2020 2073 656c 662e 6475 7065 5f69 6e64     self.dupe_ind
-000101a0: 6963 6174 6f72 2e73 686f 7728 290a 2020  icator.show().  
-000101b0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-000101c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000101d0: 7365 6c66 2e64 7570 655f 696e 6469 6361  self.dupe_indica
-000101e0: 746f 722e 6869 6465 2829 0a20 2020 2020  tor.hide().     
-000101f0: 2020 2020 2020 205f 7468 6574 6872 6561         _thethrea
-00010200: 6420 3d20 7468 7265 6164 696e 672e 5468  d = threading.Th
-00010210: 7265 6164 280a 2020 2020 2020 2020 2020  read(.          
-00010220: 2020 2020 2020 7461 7267 6574 3d73 656c        target=sel
-00010230: 662e 6368 6563 6b5f 6361 6c6c 7369 676e  f.check_callsign
-00010240: 322c 0a20 2020 2020 2020 2020 2020 2020  2,.             
-00010250: 2020 2061 7267 733d 2874 6578 742c 292c     args=(text,),
-00010260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010270: 2064 6165 6d6f 6e3d 5472 7565 2c0a 2020   daemon=True,.  
-00010280: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00010290: 2020 2020 2020 2020 5f74 6865 7468 7265          _thethre
-000102a0: 6164 2e73 7461 7274 2829 0a20 2020 2020  ad.start().     
-000102b0: 2020 2020 2020 2073 656c 662e 6e65 7874         self.next
-000102c0: 5f66 6965 6c64 2e73 6574 466f 6375 7328  _field.setFocus(
-000102d0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-000102e0: 7475 726e 0a20 2020 2020 2020 2063 6d64  turn.        cmd
-000102f0: 203d 207b 7d0a 2020 2020 2020 2020 636d   = {}.        cm
-00010300: 645b 2263 6d64 225d 203d 2022 4341 4c4c  d["cmd"] = "CALL
-00010310: 4348 414e 4745 4422 0a20 2020 2020 2020  CHANGED".       
-00010320: 2063 6d64 5b22 7374 6174 696f 6e22 5d20   cmd["station"] 
-00010330: 3d20 706c 6174 666f 726d 2e6e 6f64 6528  = platform.node(
-00010340: 290a 2020 2020 2020 2020 636d 645b 2263  ).        cmd["c
-00010350: 616c 6c22 5d20 3d20 7374 7269 7070 6564  all"] = stripped
-00010360: 5f74 6578 740a 2020 2020 2020 2020 7365  _text.        se
-00010370: 6c66 2e6d 756c 7469 6361 7374 5f69 6e74  lf.multicast_int
-00010380: 6572 6661 6365 2e73 656e 645f 6173 5f6a  erface.send_as_j
-00010390: 736f 6e28 636d 6429 0a20 2020 2020 2020  son(cmd).       
-000103a0: 2073 656c 662e 6368 6563 6b5f 6361 6c6c   self.check_call
-000103b0: 7369 676e 2873 7472 6970 7065 645f 7465  sign(stripped_te
-000103c0: 7874 290a 0a20 2020 2064 6566 2063 6865  xt)..    def che
-000103d0: 636b 5f63 616c 6c73 6967 6e28 7365 6c66  ck_callsign(self
-000103e0: 2c20 6361 6c6c 7369 676e 293a 0a20 2020  , callsign):.   
-000103f0: 2020 2020 2022 2222 4368 6563 6b20 6361       """Check ca
-00010400: 6c6c 2061 7320 656e 7465 7265 6422 2222  ll as entered"""
-00010410: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-00010420: 3d20 6374 795f 6c6f 6f6b 7570 2863 616c  = cty_lookup(cal
-00010430: 6c73 6967 6e29 0a20 2020 2020 2020 2064  lsign).        d
-00010440: 6562 7567 5f72 6573 756c 7420 3d20 6622  ebug_result = f"
-00010450: 7b72 6573 756c 747d 220a 2020 2020 2020  {result}".      
-00010460: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
-00010470: 2573 222c 2064 6562 7567 5f72 6573 756c  %s", debug_resul
-00010480: 7429 0a20 2020 2020 2020 2069 6620 7265  t).        if re
-00010490: 7375 6c74 3a0a 2020 2020 2020 2020 2020  sult:.          
-000104a0: 2020 666f 7220 6120 696e 2072 6573 756c    for a in resul
-000104b0: 742e 6974 656d 7328 293a 0a20 2020 2020  t.items():.     
-000104c0: 2020 2020 2020 2020 2020 2065 6e74 6974             entit
-000104d0: 7920 3d20 615b 315d 2e67 6574 2822 656e  y = a[1].get("en
-000104e0: 7469 7479 222c 2022 2229 0a20 2020 2020  tity", "").     
-000104f0: 2020 2020 2020 2020 2020 2063 7120 3d20             cq = 
-00010500: 615b 315d 2e67 6574 2822 6371 222c 2022  a[1].get("cq", "
-00010510: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-00010520: 2020 2069 7475 203d 2061 5b31 5d2e 6765     itu = a[1].ge
-00010530: 7428 2269 7475 222c 2022 2229 0a20 2020  t("itu", "").   
-00010540: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-00010550: 7469 6e65 6e74 203d 2061 5b31 5d2e 6765  tinent = a[1].ge
-00010560: 7428 2263 6f6e 7469 6e65 6e74 2229 0a20  t("continent"). 
-00010570: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00010580: 6174 203d 2066 6c6f 6174 2861 5b31 5d2e  at = float(a[1].
-00010590: 6765 7428 226c 6174 222c 2022 302e 3022  get("lat", "0.0"
-000105a0: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-000105b0: 2020 206c 6f6e 203d 2066 6c6f 6174 2861     lon = float(a
-000105c0: 5b31 5d2e 6765 7428 226c 6f6e 6722 2c20  [1].get("long", 
-000105d0: 2230 2e30 2229 290a 2020 2020 2020 2020  "0.0")).        
-000105e0: 2020 2020 2020 2020 6c6f 6e20 3d20 6c6f          lon = lo
-000105f0: 6e20 2a20 2d31 2020 2320 6374 792e 6461  n * -1  # cty.da
-00010600: 7420 6669 6c65 2069 6e76 6572 7473 206c  t file inverts l
-00010610: 6f6e 6769 7475 6465 730a 2020 2020 2020  ongitudes.      
-00010620: 2020 2020 2020 2020 2020 7072 696d 6172            primar
-00010630: 795f 7066 7820 3d20 615b 315d 2e67 6574  y_pfx = a[1].get
-00010640: 2822 7072 696d 6172 795f 7066 7822 2c20  ("primary_pfx", 
-00010650: 2222 290a 2020 2020 2020 2020 2020 2020  "").            
-00010660: 2020 2020 6865 6164 696e 6720 3d20 6265      heading = be
-00010670: 6172 696e 675f 7769 7468 5f6c 6174 6c6f  aring_with_latlo
-00010680: 6e28 7365 6c66 2e73 7461 7469 6f6e 2e67  n(self.station.g
-00010690: 6574 2822 4772 6964 5371 7561 7265 2229  et("GridSquare")
-000106a0: 2c20 6c61 742c 206c 6f6e 290a 2020 2020  , lat, lon).    
-000106b0: 2020 2020 2020 2020 2020 2020 6b69 6c6f              kilo
-000106c0: 6d65 7465 7273 203d 2064 6973 7461 6e63  meters = distanc
-000106d0: 655f 7769 7468 5f6c 6174 6c6f 6e28 0a20  e_with_latlon(. 
-000106e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000106f0: 2020 2073 656c 662e 7374 6174 696f 6e2e     self.station.
-00010700: 6765 7428 2247 7269 6453 7175 6172 6522  get("GridSquare"
-00010710: 292c 206c 6174 2c20 6c6f 6e0a 2020 2020  ), lat, lon.    
-00010720: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00010730: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00010740: 6c66 2e68 6561 6469 6e67 5f64 6973 7461  lf.heading_dista
-00010750: 6e63 652e 7365 7454 6578 7428 0a20 2020  nce.setText(.   
-00010760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010770: 2066 2252 6567 696f 6e61 6c20 4864 6720   f"Regional Hdg 
-00010780: 7b68 6561 6469 6e67 7dc2 b020 4c50 207b  {heading}.. LP {
-00010790: 7265 6369 7072 6f63 6f6c 2868 6561 6469  reciprocol(headi
-000107a0: 6e67 297d c2b0 202f 2022 0a20 2020 2020  ng)}.. / ".     
-000107b0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-000107c0: 2264 6973 7461 6e63 6520 7b69 6e74 286b  "distance {int(k
-000107d0: 696c 6f6d 6574 6572 732a 302e 3632 3133  ilometers*0.6213
-000107e0: 3731 297d 6d69 207b 6b69 6c6f 6d65 7465  71)}mi {kilomete
-000107f0: 7273 7d6b 6d22 0a20 2020 2020 2020 2020  rs}km".         
-00010800: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00010810: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
-00010820: 6e74 6163 745b 2243 6f75 6e74 7279 5072  ntact["CountryPr
-00010830: 6566 6978 225d 203d 2070 7269 6d61 7279  efix"] = primary
-00010840: 5f70 6678 0a20 2020 2020 2020 2020 2020  _pfx.           
-00010850: 2020 2020 2073 656c 662e 636f 6e74 6163       self.contac
-00010860: 745b 225a 4e22 5d20 3d20 696e 7428 6371  t["ZN"] = int(cq
-00010870: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00010880: 2020 7365 6c66 2e63 6f6e 7461 6374 5b22    self.contact["
-00010890: 436f 6e74 696e 656e 7422 5d20 3d20 636f  Continent"] = co
-000108a0: 6e74 696e 656e 740a 2020 2020 2020 2020  ntinent.        
-000108b0: 2020 2020 2020 2020 7365 6c66 2e64 785f          self.dx_
-000108c0: 656e 7469 7479 2e73 6574 5465 7874 280a  entity.setText(.
-000108d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108e0: 2020 2020 6622 7b70 7269 6d61 7279 5f70      f"{primary_p
-000108f0: 6678 7d3a 207b 636f 6e74 696e 656e 747d  fx}: {continent}
-00010900: 2f7b 656e 7469 7479 7d20 6371 3a7b 6371  /{entity} cq:{cq
-00010910: 7d20 6974 753a 7b69 7475 7d22 0a20 2020  } itu:{itu}".   
-00010920: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-00010930: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00010940: 6620 6c65 6e28 6361 6c6c 7369 676e 2920  f len(callsign) 
-00010950: 3e20 323a 0a20 2020 2020 2020 2020 2020  > 2:.           
-00010960: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00010970: 2e63 6f6e 7465 7374 3a0a 2020 2020 2020  .contest:.      
-00010980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010990: 2020 7365 6c66 2e63 6f6e 7465 7374 2e70    self.contest.p
-000109a0: 7265 6669 6c6c 2873 656c 6629 0a0a 2020  refill(self)..  
-000109b0: 2020 6465 6620 6368 6563 6b5f 6361 6c6c    def check_call
-000109c0: 7369 676e 3228 7365 6c66 2c20 6361 6c6c  sign2(self, call
-000109d0: 7369 676e 293a 0a20 2020 2020 2020 2022  sign):.        "
-000109e0: 2222 4368 6563 6b20 6361 6c6c 206f 6e63  ""Check call onc
-000109f0: 6520 656e 7465 7265 6422 2222 0a20 2020  e entered""".   
-00010a00: 2020 2020 2063 616c 6c73 6967 6e20 3d20       callsign = 
-00010a10: 6361 6c6c 7369 676e 2e73 7472 6970 2829  callsign.strip()
-00010a20: 0a20 2020 2020 2020 2064 6562 7567 5f6c  .        debug_l
-00010a30: 6f6f 6b75 7020 3d20 6622 7b73 656c 662e  ookup = f"{self.
-00010a40: 6c6f 6f6b 5f75 707d 220a 2020 2020 2020  look_up}".      
-00010a50: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
-00010a60: 2573 2c20 2573 222c 2063 616c 6c73 6967  %s, %s", callsig
-00010a70: 6e2c 2064 6562 7567 5f6c 6f6f 6b75 7029  n, debug_lookup)
-00010a80: 0a20 2020 2020 2020 2069 6620 6861 7361  .        if hasa
-00010a90: 7474 7228 7365 6c66 2e6c 6f6f 6b5f 7570  ttr(self.look_up
-00010aa0: 2c20 2273 6573 7369 6f6e 2229 3a0a 2020  , "session"):.  
-00010ab0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00010ac0: 662e 6c6f 6f6b 5f75 702e 7365 7373 696f  f.look_up.sessio
-00010ad0: 6e3a 0a20 2020 2020 2020 2020 2020 2020  n:.             
-00010ae0: 2020 2072 6573 706f 6e73 6520 3d20 7365     response = se
-00010af0: 6c66 2e6c 6f6f 6b5f 7570 2e6c 6f6f 6b75  lf.look_up.looku
-00010b00: 7028 6361 6c6c 7369 676e 290a 2020 2020  p(callsign).    
-00010b10: 2020 2020 2020 2020 2020 2020 6465 6275              debu
-00010b20: 675f 7265 7370 6f6e 7365 203d 2066 227b  g_response = f"{
-00010b30: 7265 7370 6f6e 7365 7d22 0a20 2020 2020  response}".     
-00010b40: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-00010b50: 722e 6465 6275 6728 2254 6865 2052 6573  r.debug("The Res
-00010b60: 706f 6e73 653a 2025 735c 6e22 2c20 6465  ponse: %s\n", de
-00010b70: 6275 675f 7265 7370 6f6e 7365 290a 2020  bug_response).  
-00010b80: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00010b90: 2072 6573 706f 6e73 653a 0a20 2020 2020   response:.     
-00010ba0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00010bb0: 6865 6972 6772 6964 203d 2072 6573 706f  heirgrid = respo
-00010bc0: 6e73 652e 6765 7428 2267 7269 6422 290a  nse.get("grid").
+0000dba0: 2020 2020 2020 2020 2073 642e 706c 6179           sd.play
+0000dbb0: 2864 6174 6129 0a20 2020 2020 2020 2020  (data).         
+0000dbc0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+0000dbd0: 6f67 6765 722e 6465 6275 6728 2225 7322  ogger.debug("%s"
+0000dbe0: 2c20 6622 7b73 642e 7761 6974 2829 7d22  , f"{sd.wait()}"
+0000dbf0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000dc00: 2020 2020 2020 6578 6365 7074 2073 642e        except sd.
+0000dc10: 506f 7274 4175 6469 6f45 7272 6f72 2061  PortAudioError a
+0000dc20: 7320 6572 723a 0a20 2020 2020 2020 2020  s err:.         
+0000dc30: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+0000dc40: 6f67 6765 722e 7761 726e 696e 6728 2225  ogger.warning("%
+0000dc50: 7322 2c20 6622 7b65 7272 7d22 290a 2020  s", f"{err}").  
+0000dc60: 2020 2020 2020 7365 6c66 2e70 7474 5f6f        self.ptt_o
+0000dc70: 6666 2829 0a0a 2020 2020 6465 6620 7074  ff()..    def pt
+0000dc80: 745f 6f6e 2873 656c 6629 3a0a 2020 2020  t_on(self):.    
+0000dc90: 2020 2020 2222 2274 7572 6e20 6f6e 2070      """turn on p
+0000dca0: 7474 2222 220a 2020 2020 2020 2020 6966  tt""".        if
+0000dcb0: 2073 656c 662e 7269 675f 636f 6e74 726f   self.rig_contro
+0000dcc0: 6c3a 0a20 2020 2020 2020 2020 2020 2073  l:.            s
+0000dcd0: 656c 662e 6c65 6674 646f 742e 7365 7450  elf.leftdot.setP
+0000dce0: 6978 6d61 7028 7365 6c66 2e67 7265 656e  ixmap(self.green
+0000dcf0: 646f 7429 0a20 2020 2020 2020 2020 2020  dot).           
+0000dd00: 2061 7070 2e70 726f 6365 7373 4576 656e   app.processEven
+0000dd10: 7473 2829 0a20 2020 2020 2020 2020 2020  ts().           
+0000dd20: 2073 656c 662e 7269 675f 636f 6e74 726f   self.rig_contro
+0000dd30: 6c2e 7074 745f 6f6e 2829 0a0a 2020 2020  l.ptt_on()..    
+0000dd40: 6465 6620 7074 745f 6f66 6628 7365 6c66  def ptt_off(self
+0000dd50: 293a 0a20 2020 2020 2020 2022 2222 7475  ):.        """tu
+0000dd60: 726e 206f 6666 2070 7474 2222 220a 2020  rn off ptt""".  
+0000dd70: 2020 2020 2020 6966 2073 656c 662e 7269        if self.ri
+0000dd80: 675f 636f 6e74 726f 6c3a 0a20 2020 2020  g_control:.     
+0000dd90: 2020 2020 2020 2073 656c 662e 6c65 6674         self.left
+0000dda0: 646f 742e 7365 7450 6978 6d61 7028 7365  dot.setPixmap(se
+0000ddb0: 6c66 2e72 6564 646f 7429 0a20 2020 2020  lf.reddot).     
+0000ddc0: 2020 2020 2020 2061 7070 2e70 726f 6365         app.proce
+0000ddd0: 7373 4576 656e 7473 2829 0a20 2020 2020  ssEvents().     
+0000dde0: 2020 2020 2020 2073 656c 662e 7269 675f         self.rig_
+0000ddf0: 636f 6e74 726f 6c2e 7074 745f 6f66 6628  control.ptt_off(
+0000de00: 290a 0a20 2020 2064 6566 2073 656e 6466  )..    def sendf
+0000de10: 3128 7365 6c66 293a 0a20 2020 2020 2020  1(self):.       
+0000de20: 2022 2222 7374 7562 2222 220a 2020 2020   """stub""".    
+0000de30: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+0000de40: 2822 4631 2043 6c69 636b 6564 2229 0a20  ("F1 Clicked"). 
+0000de50: 2020 2020 2020 2069 6620 7365 6c66 2e6e         if self.n
+0000de60: 316d 6d3a 0a20 2020 2020 2020 2020 2020  1mm:.           
+0000de70: 2073 656c 662e 6e31 6d6d 2e72 6164 696f   self.n1mm.radio
+0000de80: 5f69 6e66 6f5b 2246 756e 6374 696f 6e4b  _info["FunctionK
+0000de90: 6579 4361 7074 696f 6e22 5d20 3d20 7365  eyCaption"] = se
+0000dea0: 6c66 2e46 312e 746f 6f6c 5469 7028 290a  lf.F1.toolTip().
+0000deb0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000dec0: 7261 6469 6f5f 7374 6174 652e 6765 7428  radio_state.get(
+0000ded0: 226d 6f64 6522 2920 696e 205b 224c 5342  "mode") in ["LSB
+0000dee0: 222c 2022 5553 4222 2c20 2253 5342 225d  ", "USB", "SSB"]
+0000def0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000df00: 6c66 2e76 6f69 6365 5f73 7472 696e 6728  lf.voice_string(
+0000df10: 7365 6c66 2e70 726f 6365 7373 5f6d 6163  self.process_mac
+0000df20: 726f 2873 656c 662e 4631 2e74 6f6f 6c54  ro(self.F1.toolT
+0000df30: 6970 2829 2929 0a20 2020 2020 2020 2020  ip())).         
+0000df40: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
+0000df50: 2020 6966 2073 656c 662e 6377 3a0a 2020    if self.cw:.  
+0000df60: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+0000df70: 772e 7365 6e64 6377 2873 656c 662e 7072  w.sendcw(self.pr
+0000df80: 6f63 6573 735f 6d61 6372 6f28 7365 6c66  ocess_macro(self
+0000df90: 2e46 312e 746f 6f6c 5469 7028 2929 290a  .F1.toolTip())).
+0000dfa0: 0a20 2020 2064 6566 2073 656e 6466 3228  .    def sendf2(
+0000dfb0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+0000dfc0: 2222 7374 7562 2222 220a 2020 2020 2020  ""stub""".      
+0000dfd0: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
+0000dfe0: 4632 2043 6c69 636b 6564 2229 0a20 2020  F2 Clicked").   
+0000dff0: 2020 2020 2069 6620 7365 6c66 2e6e 316d       if self.n1m
+0000e000: 6d3a 0a20 2020 2020 2020 2020 2020 2073  m:.            s
+0000e010: 656c 662e 6e31 6d6d 2e72 6164 696f 5f69  elf.n1mm.radio_i
+0000e020: 6e66 6f5b 2246 756e 6374 696f 6e4b 6579  nfo["FunctionKey
+0000e030: 4361 7074 696f 6e22 5d20 3d20 7365 6c66  Caption"] = self
+0000e040: 2e46 322e 746f 6f6c 5469 7028 290a 2020  .F2.toolTip().  
+0000e050: 2020 2020 2020 6966 2073 656c 662e 7261        if self.ra
+0000e060: 6469 6f5f 7374 6174 652e 6765 7428 226d  dio_state.get("m
+0000e070: 6f64 6522 2920 696e 205b 224c 5342 222c  ode") in ["LSB",
+0000e080: 2022 5553 4222 2c20 2253 5342 225d 3a0a   "USB", "SSB"]:.
+0000e090: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000e0a0: 2e76 6f69 6365 5f73 7472 696e 6728 7365  .voice_string(se
+0000e0b0: 6c66 2e70 726f 6365 7373 5f6d 6163 726f  lf.process_macro
+0000e0c0: 2873 656c 662e 4632 2e74 6f6f 6c54 6970  (self.F2.toolTip
+0000e0d0: 2829 2929 0a20 2020 2020 2020 2020 2020  ())).           
+0000e0e0: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
+0000e0f0: 6966 2073 656c 662e 6377 3a0a 2020 2020  if self.cw:.    
+0000e100: 2020 2020 2020 2020 7365 6c66 2e63 772e          self.cw.
+0000e110: 7365 6e64 6377 2873 656c 662e 7072 6f63  sendcw(self.proc
+0000e120: 6573 735f 6d61 6372 6f28 7365 6c66 2e46  ess_macro(self.F
+0000e130: 322e 746f 6f6c 5469 7028 2929 290a 0a20  2.toolTip())).. 
+0000e140: 2020 2064 6566 2073 656e 6466 3328 7365     def sendf3(se
+0000e150: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+0000e160: 7374 7562 2222 220a 2020 2020 2020 2020  stub""".        
+0000e170: 6c6f 6767 6572 2e64 6562 7567 2822 4633  logger.debug("F3
+0000e180: 2043 6c69 636b 6564 2229 0a20 2020 2020   Clicked").     
+0000e190: 2020 2069 6620 7365 6c66 2e6e 316d 6d3a     if self.n1mm:
+0000e1a0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000e1b0: 662e 6e31 6d6d 2e72 6164 696f 5f69 6e66  f.n1mm.radio_inf
+0000e1c0: 6f5b 2246 756e 6374 696f 6e4b 6579 4361  o["FunctionKeyCa
+0000e1d0: 7074 696f 6e22 5d20 3d20 7365 6c66 2e46  ption"] = self.F
+0000e1e0: 332e 746f 6f6c 5469 7028 290a 2020 2020  3.toolTip().    
+0000e1f0: 2020 2020 6966 2073 656c 662e 7261 6469      if self.radi
+0000e200: 6f5f 7374 6174 652e 6765 7428 226d 6f64  o_state.get("mod
+0000e210: 6522 2920 696e 205b 224c 5342 222c 2022  e") in ["LSB", "
+0000e220: 5553 4222 2c20 2253 5342 225d 3a0a 2020  USB", "SSB"]:.  
+0000e230: 2020 2020 2020 2020 2020 7365 6c66 2e76            self.v
+0000e240: 6f69 6365 5f73 7472 696e 6728 7365 6c66  oice_string(self
+0000e250: 2e70 726f 6365 7373 5f6d 6163 726f 2873  .process_macro(s
+0000e260: 656c 662e 4633 2e74 6f6f 6c54 6970 2829  elf.F3.toolTip()
+0000e270: 2929 0a20 2020 2020 2020 2020 2020 2072  )).            r
+0000e280: 6574 7572 6e0a 2020 2020 2020 2020 6966  eturn.        if
+0000e290: 2073 656c 662e 6377 3a0a 2020 2020 2020   self.cw:.      
+0000e2a0: 2020 2020 2020 7365 6c66 2e63 772e 7365        self.cw.se
+0000e2b0: 6e64 6377 2873 656c 662e 7072 6f63 6573  ndcw(self.proces
+0000e2c0: 735f 6d61 6372 6f28 7365 6c66 2e46 332e  s_macro(self.F3.
+0000e2d0: 746f 6f6c 5469 7028 2929 290a 0a20 2020  toolTip()))..   
+0000e2e0: 2064 6566 2073 656e 6466 3428 7365 6c66   def sendf4(self
+0000e2f0: 293a 0a20 2020 2020 2020 2022 2222 7374  ):.        """st
+0000e300: 7562 2222 220a 2020 2020 2020 2020 6c6f  ub""".        lo
+0000e310: 6767 6572 2e64 6562 7567 2822 4634 2043  gger.debug("F4 C
+0000e320: 6c69 636b 6564 2229 0a20 2020 2020 2020  licked").       
+0000e330: 2069 6620 7365 6c66 2e6e 316d 6d3a 0a20   if self.n1mm:. 
+0000e340: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000e350: 6e31 6d6d 2e72 6164 696f 5f69 6e66 6f5b  n1mm.radio_info[
+0000e360: 2246 756e 6374 696f 6e4b 6579 4361 7074  "FunctionKeyCapt
+0000e370: 696f 6e22 5d20 3d20 7365 6c66 2e46 342e  ion"] = self.F4.
+0000e380: 746f 6f6c 5469 7028 290a 2020 2020 2020  toolTip().      
+0000e390: 2020 6966 2073 656c 662e 7261 6469 6f5f    if self.radio_
+0000e3a0: 7374 6174 652e 6765 7428 226d 6f64 6522  state.get("mode"
+0000e3b0: 2920 696e 205b 224c 5342 222c 2022 5553  ) in ["LSB", "US
+0000e3c0: 4222 2c20 2253 5342 225d 3a0a 2020 2020  B", "SSB"]:.    
+0000e3d0: 2020 2020 2020 2020 7365 6c66 2e76 6f69          self.voi
+0000e3e0: 6365 5f73 7472 696e 6728 7365 6c66 2e70  ce_string(self.p
+0000e3f0: 726f 6365 7373 5f6d 6163 726f 2873 656c  rocess_macro(sel
+0000e400: 662e 4634 2e74 6f6f 6c54 6970 2829 2929  f.F4.toolTip()))
+0000e410: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000e420: 7572 6e0a 2020 2020 2020 2020 6966 2073  urn.        if s
+0000e430: 656c 662e 6377 3a0a 2020 2020 2020 2020  elf.cw:.        
+0000e440: 2020 2020 7365 6c66 2e63 772e 7365 6e64      self.cw.send
+0000e450: 6377 2873 656c 662e 7072 6f63 6573 735f  cw(self.process_
+0000e460: 6d61 6372 6f28 7365 6c66 2e46 342e 746f  macro(self.F4.to
+0000e470: 6f6c 5469 7028 2929 290a 0a20 2020 2064  olTip()))..    d
+0000e480: 6566 2073 656e 6466 3528 7365 6c66 293a  ef sendf5(self):
+0000e490: 0a20 2020 2020 2020 2022 2222 7374 7562  .        """stub
+0000e4a0: 2222 220a 2020 2020 2020 2020 6c6f 6767  """.        logg
+0000e4b0: 6572 2e64 6562 7567 2822 4635 2043 6c69  er.debug("F5 Cli
+0000e4c0: 636b 6564 2229 0a20 2020 2020 2020 2069  cked").        i
+0000e4d0: 6620 7365 6c66 2e6e 316d 6d3a 0a20 2020  f self.n1mm:.   
+0000e4e0: 2020 2020 2020 2020 2073 656c 662e 6e31           self.n1
+0000e4f0: 6d6d 2e72 6164 696f 5f69 6e66 6f5b 2246  mm.radio_info["F
+0000e500: 756e 6374 696f 6e4b 6579 4361 7074 696f  unctionKeyCaptio
+0000e510: 6e22 5d20 3d20 7365 6c66 2e46 352e 746f  n"] = self.F5.to
+0000e520: 6f6c 5469 7028 290a 2020 2020 2020 2020  olTip().        
+0000e530: 6966 2073 656c 662e 7261 6469 6f5f 7374  if self.radio_st
+0000e540: 6174 652e 6765 7428 226d 6f64 6522 2920  ate.get("mode") 
+0000e550: 696e 205b 224c 5342 222c 2022 5553 4222  in ["LSB", "USB"
+0000e560: 2c20 2253 5342 225d 3a0a 2020 2020 2020  , "SSB"]:.      
+0000e570: 2020 2020 2020 7365 6c66 2e76 6f69 6365        self.voice
+0000e580: 5f73 7472 696e 6728 7365 6c66 2e70 726f  _string(self.pro
+0000e590: 6365 7373 5f6d 6163 726f 2873 656c 662e  cess_macro(self.
+0000e5a0: 4635 2e74 6f6f 6c54 6970 2829 2929 0a20  F5.toolTip())). 
+0000e5b0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000e5c0: 6e0a 2020 2020 2020 2020 6966 2073 656c  n.        if sel
+0000e5d0: 662e 6377 3a0a 2020 2020 2020 2020 2020  f.cw:.          
+0000e5e0: 2020 7365 6c66 2e63 772e 7365 6e64 6377    self.cw.sendcw
+0000e5f0: 2873 656c 662e 7072 6f63 6573 735f 6d61  (self.process_ma
+0000e600: 6372 6f28 7365 6c66 2e46 352e 746f 6f6c  cro(self.F5.tool
+0000e610: 5469 7028 2929 290a 0a20 2020 2064 6566  Tip()))..    def
+0000e620: 2073 656e 6466 3628 7365 6c66 293a 0a20   sendf6(self):. 
+0000e630: 2020 2020 2020 2022 2222 7374 7562 2222         """stub""
+0000e640: 220a 2020 2020 2020 2020 6c6f 6767 6572  ".        logger
+0000e650: 2e64 6562 7567 2822 4636 2043 6c69 636b  .debug("F6 Click
+0000e660: 6564 2229 0a20 2020 2020 2020 2069 6620  ed").        if 
+0000e670: 7365 6c66 2e6e 316d 6d3a 0a20 2020 2020  self.n1mm:.     
+0000e680: 2020 2020 2020 2073 656c 662e 6e31 6d6d         self.n1mm
+0000e690: 2e72 6164 696f 5f69 6e66 6f5b 2246 756e  .radio_info["Fun
+0000e6a0: 6374 696f 6e4b 6579 4361 7074 696f 6e22  ctionKeyCaption"
+0000e6b0: 5d20 3d20 7365 6c66 2e46 362e 746f 6f6c  ] = self.F6.tool
+0000e6c0: 5469 7028 290a 2020 2020 2020 2020 6966  Tip().        if
+0000e6d0: 2073 656c 662e 7261 6469 6f5f 7374 6174   self.radio_stat
+0000e6e0: 652e 6765 7428 226d 6f64 6522 2920 696e  e.get("mode") in
+0000e6f0: 205b 224c 5342 222c 2022 5553 4222 2c20   ["LSB", "USB", 
+0000e700: 2253 5342 225d 3a0a 2020 2020 2020 2020  "SSB"]:.        
+0000e710: 2020 2020 7365 6c66 2e76 6f69 6365 5f73      self.voice_s
+0000e720: 7472 696e 6728 7365 6c66 2e70 726f 6365  tring(self.proce
+0000e730: 7373 5f6d 6163 726f 2873 656c 662e 4636  ss_macro(self.F6
+0000e740: 2e74 6f6f 6c54 6970 2829 2929 0a20 2020  .toolTip())).   
+0000e750: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+0000e760: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000e770: 6377 3a0a 2020 2020 2020 2020 2020 2020  cw:.            
+0000e780: 7365 6c66 2e63 772e 7365 6e64 6377 2873  self.cw.sendcw(s
+0000e790: 656c 662e 7072 6f63 6573 735f 6d61 6372  elf.process_macr
+0000e7a0: 6f28 7365 6c66 2e46 362e 746f 6f6c 5469  o(self.F6.toolTi
+0000e7b0: 7028 2929 290a 0a20 2020 2064 6566 2073  p()))..    def s
+0000e7c0: 656e 6466 3728 7365 6c66 293a 0a20 2020  endf7(self):.   
+0000e7d0: 2020 2020 2022 2222 7374 7562 2222 220a       """stub""".
+0000e7e0: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+0000e7f0: 6562 7567 2822 4637 2043 6c69 636b 6564  ebug("F7 Clicked
+0000e800: 2229 0a20 2020 2020 2020 2069 6620 7365  ").        if se
+0000e810: 6c66 2e6e 316d 6d3a 0a20 2020 2020 2020  lf.n1mm:.       
+0000e820: 2020 2020 2073 656c 662e 6e31 6d6d 2e72       self.n1mm.r
+0000e830: 6164 696f 5f69 6e66 6f5b 2246 756e 6374  adio_info["Funct
+0000e840: 696f 6e4b 6579 4361 7074 696f 6e22 5d20  ionKeyCaption"] 
+0000e850: 3d20 7365 6c66 2e46 372e 746f 6f6c 5469  = self.F7.toolTi
+0000e860: 7028 290a 2020 2020 2020 2020 6966 2073  p().        if s
+0000e870: 656c 662e 7261 6469 6f5f 7374 6174 652e  elf.radio_state.
+0000e880: 6765 7428 226d 6f64 6522 2920 696e 205b  get("mode") in [
+0000e890: 224c 5342 222c 2022 5553 4222 2c20 2253  "LSB", "USB", "S
+0000e8a0: 5342 225d 3a0a 2020 2020 2020 2020 2020  SB"]:.          
+0000e8b0: 2020 7365 6c66 2e76 6f69 6365 5f73 7472    self.voice_str
+0000e8c0: 696e 6728 7365 6c66 2e70 726f 6365 7373  ing(self.process
+0000e8d0: 5f6d 6163 726f 2873 656c 662e 4637 2e74  _macro(self.F7.t
+0000e8e0: 6f6f 6c54 6970 2829 2929 0a20 2020 2020  oolTip())).     
+0000e8f0: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+0000e900: 2020 2020 2020 6966 2073 656c 662e 6377        if self.cw
+0000e910: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000e920: 6c66 2e63 772e 7365 6e64 6377 2873 656c  lf.cw.sendcw(sel
+0000e930: 662e 7072 6f63 6573 735f 6d61 6372 6f28  f.process_macro(
+0000e940: 7365 6c66 2e46 372e 746f 6f6c 5469 7028  self.F7.toolTip(
+0000e950: 2929 290a 0a20 2020 2064 6566 2073 656e  )))..    def sen
+0000e960: 6466 3828 7365 6c66 293a 0a20 2020 2020  df8(self):.     
+0000e970: 2020 2022 2222 7374 7562 2222 220a 2020     """stub""".  
+0000e980: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
+0000e990: 7567 2822 4638 2043 6c69 636b 6564 2229  ug("F8 Clicked")
+0000e9a0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0000e9b0: 2e6e 316d 6d3a 0a20 2020 2020 2020 2020  .n1mm:.         
+0000e9c0: 2020 2073 656c 662e 6e31 6d6d 2e72 6164     self.n1mm.rad
+0000e9d0: 696f 5f69 6e66 6f5b 2246 756e 6374 696f  io_info["Functio
+0000e9e0: 6e4b 6579 4361 7074 696f 6e22 5d20 3d20  nKeyCaption"] = 
+0000e9f0: 7365 6c66 2e46 382e 746f 6f6c 5469 7028  self.F8.toolTip(
+0000ea00: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+0000ea10: 662e 7261 6469 6f5f 7374 6174 652e 6765  f.radio_state.ge
+0000ea20: 7428 226d 6f64 6522 2920 696e 205b 224c  t("mode") in ["L
+0000ea30: 5342 222c 2022 5553 4222 2c20 2253 5342  SB", "USB", "SSB
+0000ea40: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
+0000ea50: 7365 6c66 2e76 6f69 6365 5f73 7472 696e  self.voice_strin
+0000ea60: 6728 7365 6c66 2e70 726f 6365 7373 5f6d  g(self.process_m
+0000ea70: 6163 726f 2873 656c 662e 4638 2e74 6f6f  acro(self.F8.too
+0000ea80: 6c54 6970 2829 2929 0a20 2020 2020 2020  lTip())).       
+0000ea90: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+0000eaa0: 2020 2020 6966 2073 656c 662e 6377 3a0a      if self.cw:.
+0000eab0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000eac0: 2e63 772e 7365 6e64 6377 2873 656c 662e  .cw.sendcw(self.
+0000ead0: 7072 6f63 6573 735f 6d61 6372 6f28 7365  process_macro(se
+0000eae0: 6c66 2e46 382e 746f 6f6c 5469 7028 2929  lf.F8.toolTip())
+0000eaf0: 290a 0a20 2020 2064 6566 2073 656e 6466  )..    def sendf
+0000eb00: 3928 7365 6c66 293a 0a20 2020 2020 2020  9(self):.       
+0000eb10: 2022 2222 7374 7562 2222 220a 2020 2020   """stub""".    
+0000eb20: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+0000eb30: 2822 4639 2043 6c69 636b 6564 2229 0a20  ("F9 Clicked"). 
+0000eb40: 2020 2020 2020 2069 6620 7365 6c66 2e6e         if self.n
+0000eb50: 316d 6d3a 0a20 2020 2020 2020 2020 2020  1mm:.           
+0000eb60: 2073 656c 662e 6e31 6d6d 2e72 6164 696f   self.n1mm.radio
+0000eb70: 5f69 6e66 6f5b 2246 756e 6374 696f 6e4b  _info["FunctionK
+0000eb80: 6579 4361 7074 696f 6e22 5d20 3d20 7365  eyCaption"] = se
+0000eb90: 6c66 2e46 392e 746f 6f6c 5469 7028 290a  lf.F9.toolTip().
+0000eba0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000ebb0: 7261 6469 6f5f 7374 6174 652e 6765 7428  radio_state.get(
+0000ebc0: 226d 6f64 6522 2920 696e 205b 224c 5342  "mode") in ["LSB
+0000ebd0: 222c 2022 5553 4222 2c20 2253 5342 225d  ", "USB", "SSB"]
+0000ebe0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000ebf0: 6c66 2e76 6f69 6365 5f73 7472 696e 6728  lf.voice_string(
+0000ec00: 7365 6c66 2e70 726f 6365 7373 5f6d 6163  self.process_mac
+0000ec10: 726f 2873 656c 662e 4639 2e74 6f6f 6c54  ro(self.F9.toolT
+0000ec20: 6970 2829 2929 0a20 2020 2020 2020 2020  ip())).         
+0000ec30: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
+0000ec40: 2020 6966 2073 656c 662e 6377 3a0a 2020    if self.cw:.  
+0000ec50: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+0000ec60: 772e 7365 6e64 6377 2873 656c 662e 7072  w.sendcw(self.pr
+0000ec70: 6f63 6573 735f 6d61 6372 6f28 7365 6c66  ocess_macro(self
+0000ec80: 2e46 392e 746f 6f6c 5469 7028 2929 290a  .F9.toolTip())).
+0000ec90: 0a20 2020 2064 6566 2073 656e 6466 3130  .    def sendf10
+0000eca0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000ecb0: 2222 2273 7475 6222 2222 0a20 2020 2020  """stub""".     
+0000ecc0: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+0000ecd0: 2246 3130 2043 6c69 636b 6564 2229 0a20  "F10 Clicked"). 
+0000ece0: 2020 2020 2020 2069 6620 7365 6c66 2e6e         if self.n
+0000ecf0: 316d 6d3a 0a20 2020 2020 2020 2020 2020  1mm:.           
+0000ed00: 2073 656c 662e 6e31 6d6d 2e72 6164 696f   self.n1mm.radio
+0000ed10: 5f69 6e66 6f5b 2246 756e 6374 696f 6e4b  _info["FunctionK
+0000ed20: 6579 4361 7074 696f 6e22 5d20 3d20 7365  eyCaption"] = se
+0000ed30: 6c66 2e46 3130 2e74 6f6f 6c54 6970 2829  lf.F10.toolTip()
+0000ed40: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0000ed50: 2e72 6164 696f 5f73 7461 7465 2e67 6574  .radio_state.get
+0000ed60: 2822 6d6f 6465 2229 2069 6e20 5b22 4c53  ("mode") in ["LS
+0000ed70: 4222 2c20 2255 5342 222c 2022 5353 4222  B", "USB", "SSB"
+0000ed80: 5d3a 0a20 2020 2020 2020 2020 2020 2073  ]:.            s
+0000ed90: 656c 662e 766f 6963 655f 7374 7269 6e67  elf.voice_string
+0000eda0: 2873 656c 662e 7072 6f63 6573 735f 6d61  (self.process_ma
+0000edb0: 6372 6f28 7365 6c66 2e46 3130 2e74 6f6f  cro(self.F10.too
+0000edc0: 6c54 6970 2829 2929 0a20 2020 2020 2020  lTip())).       
+0000edd0: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+0000ede0: 2020 2020 6966 2073 656c 662e 6377 3a0a      if self.cw:.
+0000edf0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000ee00: 2e63 772e 7365 6e64 6377 2873 656c 662e  .cw.sendcw(self.
+0000ee10: 7072 6f63 6573 735f 6d61 6372 6f28 7365  process_macro(se
+0000ee20: 6c66 2e46 3130 2e74 6f6f 6c54 6970 2829  lf.F10.toolTip()
+0000ee30: 2929 0a0a 2020 2020 6465 6620 7365 6e64  ))..    def send
+0000ee40: 6631 3128 7365 6c66 293a 0a20 2020 2020  f11(self):.     
+0000ee50: 2020 2022 2222 7374 7562 2222 220a 2020     """stub""".  
+0000ee60: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
+0000ee70: 7567 2822 4631 3120 436c 6963 6b65 6422  ug("F11 Clicked"
+0000ee80: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+0000ee90: 662e 6e31 6d6d 3a0a 2020 2020 2020 2020  f.n1mm:.        
+0000eea0: 2020 2020 7365 6c66 2e6e 316d 6d2e 7261      self.n1mm.ra
+0000eeb0: 6469 6f5f 696e 666f 5b22 4675 6e63 7469  dio_info["Functi
+0000eec0: 6f6e 4b65 7943 6170 7469 6f6e 225d 203d  onKeyCaption"] =
+0000eed0: 2073 656c 662e 4631 312e 746f 6f6c 5469   self.F11.toolTi
+0000eee0: 7028 290a 2020 2020 2020 2020 6966 2073  p().        if s
+0000eef0: 656c 662e 7261 6469 6f5f 7374 6174 652e  elf.radio_state.
+0000ef00: 6765 7428 226d 6f64 6522 2920 696e 205b  get("mode") in [
+0000ef10: 224c 5342 222c 2022 5553 4222 2c20 2253  "LSB", "USB", "S
+0000ef20: 5342 225d 3a0a 2020 2020 2020 2020 2020  SB"]:.          
+0000ef30: 2020 7365 6c66 2e76 6f69 6365 5f73 7472    self.voice_str
+0000ef40: 696e 6728 7365 6c66 2e70 726f 6365 7373  ing(self.process
+0000ef50: 5f6d 6163 726f 2873 656c 662e 4631 312e  _macro(self.F11.
+0000ef60: 746f 6f6c 5469 7028 2929 290a 2020 2020  toolTip())).    
+0000ef70: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+0000ef80: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
+0000ef90: 773a 0a20 2020 2020 2020 2020 2020 2073  w:.            s
+0000efa0: 656c 662e 6377 2e73 656e 6463 7728 7365  elf.cw.sendcw(se
+0000efb0: 6c66 2e70 726f 6365 7373 5f6d 6163 726f  lf.process_macro
+0000efc0: 2873 656c 662e 4631 312e 746f 6f6c 5469  (self.F11.toolTi
+0000efd0: 7028 2929 290a 0a20 2020 2064 6566 2073  p()))..    def s
+0000efe0: 656e 6466 3132 2873 656c 6629 3a0a 2020  endf12(self):.  
+0000eff0: 2020 2020 2020 2222 2273 7475 6222 2222        """stub"""
+0000f000: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
+0000f010: 6465 6275 6728 2246 3132 2043 6c69 636b  debug("F12 Click
+0000f020: 6564 2229 0a20 2020 2020 2020 2069 6620  ed").        if 
+0000f030: 7365 6c66 2e6e 316d 6d3a 0a20 2020 2020  self.n1mm:.     
+0000f040: 2020 2020 2020 2073 656c 662e 6e31 6d6d         self.n1mm
+0000f050: 2e72 6164 696f 5f69 6e66 6f5b 2246 756e  .radio_info["Fun
+0000f060: 6374 696f 6e4b 6579 4361 7074 696f 6e22  ctionKeyCaption"
+0000f070: 5d20 3d20 7365 6c66 2e46 3132 2e74 6f6f  ] = self.F12.too
+0000f080: 6c54 6970 2829 0a20 2020 2020 2020 2069  lTip().        i
+0000f090: 6620 7365 6c66 2e72 6164 696f 5f73 7461  f self.radio_sta
+0000f0a0: 7465 2e67 6574 2822 6d6f 6465 2229 2069  te.get("mode") i
+0000f0b0: 6e20 5b22 4c53 4222 2c20 2255 5342 222c  n ["LSB", "USB",
+0000f0c0: 2022 5353 4222 5d3a 0a20 2020 2020 2020   "SSB"]:.       
+0000f0d0: 2020 2020 2073 656c 662e 766f 6963 655f       self.voice_
+0000f0e0: 7374 7269 6e67 2873 656c 662e 7072 6f63  string(self.proc
+0000f0f0: 6573 735f 6d61 6372 6f28 7365 6c66 2e46  ess_macro(self.F
+0000f100: 3132 2e74 6f6f 6c54 6970 2829 2929 0a20  12.toolTip())). 
+0000f110: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000f120: 6e0a 2020 2020 2020 2020 6966 2073 656c  n.        if sel
+0000f130: 662e 6377 3a0a 2020 2020 2020 2020 2020  f.cw:.          
+0000f140: 2020 7365 6c66 2e63 772e 7365 6e64 6377    self.cw.sendcw
+0000f150: 2873 656c 662e 7072 6f63 6573 735f 6d61  (self.process_ma
+0000f160: 6372 6f28 7365 6c66 2e46 3132 2e74 6f6f  cro(self.F12.too
+0000f170: 6c54 6970 2829 2929 0a0a 2020 2020 6465  lTip()))..    de
+0000f180: 6620 7275 6e5f 7370 5f62 7574 746f 6e73  f run_sp_buttons
+0000f190: 5f63 6c69 636b 6564 2873 656c 6629 3a0a  _clicked(self):.
+0000f1a0: 2020 2020 2020 2020 2222 2248 616e 646c          """Handl
+0000f1b0: 6520 7275 6e2f 7326 7020 6d6f 6465 2222  e run/s&p mode""
+0000f1c0: 220a 2020 2020 2020 2020 7365 6c66 2e70  ".        self.p
+0000f1d0: 7265 665b 2272 756e 5f73 7461 7465 225d  ref["run_state"]
+0000f1e0: 203d 2073 656c 662e 7261 6469 6f42 7574   = self.radioBut
+0000f1f0: 746f 6e5f 7275 6e2e 6973 4368 6563 6b65  ton_run.isChecke
+0000f200: 6428 290a 2020 2020 2020 2020 7365 6c66  d().        self
+0000f210: 2e77 7269 7465 5f70 7265 6665 7265 6e63  .write_preferenc
+0000f220: 6528 290a 2020 2020 2020 2020 7365 6c66  e().        self
+0000f230: 2e72 6561 645f 6377 5f6d 6163 726f 7328  .read_cw_macros(
+0000f240: 290a 0a20 2020 2064 6566 2077 7269 7465  )..    def write
+0000f250: 5f70 7265 6665 7265 6e63 6528 7365 6c66  _preference(self
+0000f260: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+0000f270: 2020 2020 2020 2057 7269 7465 2070 7265         Write pre
+0000f280: 6665 7265 6e63 6573 2074 6f20 6a73 6f6e  ferences to json
+0000f290: 2066 696c 652e 0a20 2020 2020 2020 2022   file..        "
+0000f2a0: 2222 0a20 2020 2020 2020 2074 7279 3a0a  "".        try:.
+0000f2b0: 2020 2020 2020 2020 2020 2020 7769 7468              with
+0000f2c0: 206f 7065 6e28 0a20 2020 2020 2020 2020   open(.         
+0000f2d0: 2020 2020 2020 2043 4f4e 4649 475f 5041         CONFIG_PA
+0000f2e0: 5448 202b 2022 2f6e 6f74 316d 6d2e 6a73  TH + "/not1mm.js
+0000f2f0: 6f6e 222c 2022 7774 222c 2065 6e63 6f64  on", "wt", encod
+0000f300: 696e 673d 2275 7466 2d38 220a 2020 2020  ing="utf-8".    
+0000f310: 2020 2020 2020 2020 2920 6173 2066 696c          ) as fil
+0000f320: 655f 6465 7363 7269 7074 6f72 3a0a 2020  e_descriptor:.  
+0000f330: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+0000f340: 6c65 5f64 6573 6372 6970 746f 722e 7772  le_descriptor.wr
+0000f350: 6974 6528 6475 6d70 7328 7365 6c66 2e70  ite(dumps(self.p
+0000f360: 7265 662c 2069 6e64 656e 743d 3429 290a  ref, indent=4)).
+0000f370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f380: 6c6f 6767 6572 2e69 6e66 6f28 2277 7269  logger.info("wri
+0000f390: 7469 6e67 3a20 2573 222c 2073 656c 662e  ting: %s", self.
+0000f3a0: 7072 6566 290a 2020 2020 2020 2020 6578  pref).        ex
+0000f3b0: 6365 7074 2049 4f45 7272 6f72 2061 7320  cept IOError as 
+0000f3c0: 6578 6365 7074 696f 6e3a 0a20 2020 2020  exception:.     
+0000f3d0: 2020 2020 2020 206c 6f67 6765 722e 6372         logger.cr
+0000f3e0: 6974 6963 616c 2822 7772 6974 6570 7265  itical("writepre
+0000f3f0: 6665 7265 6e63 6573 3a20 2573 222c 2065  ferences: %s", e
+0000f400: 7863 6570 7469 6f6e 290a 0a20 2020 2064  xception)..    d
+0000f410: 6566 2072 6561 6470 7265 6665 7265 6e63  ef readpreferenc
+0000f420: 6573 2873 656c 6629 3a0a 2020 2020 2020  es(self):.      
+0000f430: 2020 2222 220a 2020 2020 2020 2020 5265    """.        Re
+0000f440: 7374 6f72 6520 7072 6566 6572 656e 6365  store preference
+0000f450: 7320 6966 2074 6865 7920 6578 6973 742c  s if they exist,
+0000f460: 206f 7468 6572 7769 7365 2063 7265 6174   otherwise creat
+0000f470: 6520 736f 6d65 2073 616e 6520 6465 6661  e some sane defa
+0000f480: 756c 7473 2e0a 2020 2020 2020 2020 2222  ults..        ""
+0000f490: 220a 2020 2020 2020 2020 7472 793a 0a20  ".        try:. 
+0000f4a0: 2020 2020 2020 2020 2020 2069 6620 6f73             if os
+0000f4b0: 2e70 6174 682e 6578 6973 7473 2843 4f4e  .path.exists(CON
+0000f4c0: 4649 475f 5041 5448 202b 2022 2f6e 6f74  FIG_PATH + "/not
+0000f4d0: 316d 6d2e 6a73 6f6e 2229 3a0a 2020 2020  1mm.json"):.    
+0000f4e0: 2020 2020 2020 2020 2020 2020 7769 7468              with
+0000f4f0: 206f 7065 6e28 0a20 2020 2020 2020 2020   open(.         
+0000f500: 2020 2020 2020 2020 2020 2043 4f4e 4649             CONFI
+0000f510: 475f 5041 5448 202b 2022 2f6e 6f74 316d  G_PATH + "/not1m
+0000f520: 6d2e 6a73 6f6e 222c 2022 7274 222c 2065  m.json", "rt", e
+0000f530: 6e63 6f64 696e 673d 2275 7466 2d38 220a  ncoding="utf-8".
+0000f540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f550: 2920 6173 2066 696c 655f 6465 7363 7269  ) as file_descri
+0000f560: 7074 6f72 3a0a 2020 2020 2020 2020 2020  ptor:.          
+0000f570: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
+0000f580: 7265 6620 3d20 6c6f 6164 7328 6669 6c65  ref = loads(file
+0000f590: 5f64 6573 6372 6970 746f 722e 7265 6164  _descriptor.read
+0000f5a0: 2829 290a 2020 2020 2020 2020 2020 2020  ()).            
+0000f5b0: 2020 2020 2020 2020 6c6f 6767 6572 2e69          logger.i
+0000f5c0: 6e66 6f28 2225 7322 2c20 7365 6c66 2e70  nfo("%s", self.p
+0000f5d0: 7265 6629 0a20 2020 2020 2020 2020 2020  ref).           
+0000f5e0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000f5f0: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
+0000f600: 666f 2822 4e6f 2070 7265 6665 7265 6e63  fo("No preferenc
+0000f610: 6520 6669 6c65 2e20 5772 6974 696e 6720  e file. Writing 
+0000f620: 7072 6566 6572 656e 6365 2e22 290a 2020  preference.").  
+0000f630: 2020 2020 2020 2020 2020 2020 2020 7769                wi
+0000f640: 7468 206f 7065 6e28 0a20 2020 2020 2020  th open(.       
+0000f650: 2020 2020 2020 2020 2020 2020 2043 4f4e               CON
+0000f660: 4649 475f 5041 5448 202b 2022 2f6e 6f74  FIG_PATH + "/not
+0000f670: 316d 6d2e 6a73 6f6e 222c 2022 7774 222c  1mm.json", "wt",
+0000f680: 2065 6e63 6f64 696e 673d 2275 7466 2d38   encoding="utf-8
+0000f690: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0000f6a0: 2020 2920 6173 2066 696c 655f 6465 7363    ) as file_desc
+0000f6b0: 7269 7074 6f72 3a0a 2020 2020 2020 2020  riptor:.        
+0000f6c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000f6d0: 2e70 7265 6620 3d20 7365 6c66 2e70 7265  .pref = self.pre
+0000f6e0: 665f 7265 662e 636f 7079 2829 0a20 2020  f_ref.copy().   
+0000f6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f700: 2066 696c 655f 6465 7363 7269 7074 6f72   file_descriptor
+0000f710: 2e77 7269 7465 2864 756d 7073 2873 656c  .write(dumps(sel
+0000f720: 662e 7072 6566 2c20 696e 6465 6e74 3d34  f.pref, indent=4
+0000f730: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+0000f740: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
+0000f750: 666f 2822 2573 222c 2073 656c 662e 7072  fo("%s", self.pr
+0000f760: 6566 290a 2020 2020 2020 2020 6578 6365  ef).        exce
+0000f770: 7074 2049 4f45 7272 6f72 2061 7320 6578  pt IOError as ex
+0000f780: 6365 7074 696f 6e3a 0a20 2020 2020 2020  ception:.       
+0000f790: 2020 2020 206c 6f67 6765 722e 6372 6974       logger.crit
+0000f7a0: 6963 616c 2822 4572 726f 723a 2025 7322  ical("Error: %s"
+0000f7b0: 2c20 6578 6365 7074 696f 6e29 0a0a 2020  , exception)..  
+0000f7c0: 2020 2020 2020 7365 6c66 2e6c 6f6f 6b5f        self.look_
+0000f7d0: 7570 203d 204e 6f6e 650a 2020 2020 2020  up = None.      
+0000f7e0: 2020 6966 2073 656c 662e 7072 6566 2e67    if self.pref.g
+0000f7f0: 6574 2822 7573 6571 727a 2229 3a0a 2020  et("useqrz"):.  
+0000f800: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
+0000f810: 6f6f 6b5f 7570 203d 2051 525a 6c6f 6f6b  ook_up = QRZlook
+0000f820: 7570 280a 2020 2020 2020 2020 2020 2020  up(.            
+0000f830: 2020 2020 7365 6c66 2e70 7265 662e 6765      self.pref.ge
+0000f840: 7428 226c 6f6f 6b75 7075 7365 726e 616d  t("lookupusernam
+0000f850: 6522 292c 0a20 2020 2020 2020 2020 2020  e"),.           
+0000f860: 2020 2020 2073 656c 662e 7072 6566 2e67       self.pref.g
+0000f870: 6574 2822 6c6f 6f6b 7570 7061 7373 776f  et("lookuppasswo
+0000f880: 7264 2229 2c0a 2020 2020 2020 2020 2020  rd"),.          
+0000f890: 2020 290a 2020 2020 2020 2020 2320 6966    ).        # if
+0000f8a0: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
+0000f8b0: 7573 6568 616d 6462 2229 3a0a 2020 2020  usehamdb"):.    
+0000f8c0: 2020 2020 2320 2020 2020 7365 6c66 2e6c      #     self.l
+0000f8d0: 6f6f 6b5f 7570 203d 2048 616d 4442 6c6f  ook_up = HamDBlo
+0000f8e0: 6f6b 7570 2829 0a20 2020 2020 2020 2069  okup().        i
+0000f8f0: 6620 7365 6c66 2e70 7265 662e 6765 7428  f self.pref.get(
+0000f900: 2275 7365 6861 6d71 7468 2229 3a0a 2020  "usehamqth"):.  
+0000f910: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
+0000f920: 6f6f 6b5f 7570 203d 2048 616d 5154 4828  ook_up = HamQTH(
+0000f930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f940: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
+0000f950: 6c6f 6f6b 7570 7573 6572 6e61 6d65 2229  lookupusername")
+0000f960: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000f970: 2020 7365 6c66 2e70 7265 662e 6765 7428    self.pref.get(
+0000f980: 226c 6f6f 6b75 7070 6173 7377 6f72 6422  "lookuppassword"
+0000f990: 292c 0a20 2020 2020 2020 2020 2020 2029  ),.            )
+0000f9a0: 0a0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
+0000f9b0: 662e 7072 6566 2e67 6574 2822 7275 6e5f  f.pref.get("run_
+0000f9c0: 7374 6174 6522 293a 0a20 2020 2020 2020  state"):.       
+0000f9d0: 2020 2020 2073 656c 662e 7261 6469 6f42       self.radioB
+0000f9e0: 7574 746f 6e5f 7275 6e2e 7365 7443 6865  utton_run.setChe
+0000f9f0: 636b 6564 2854 7275 6529 0a20 2020 2020  cked(True).     
+0000fa00: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000fa10: 2020 2020 2073 656c 662e 7261 6469 6f42       self.radioB
+0000fa20: 7574 746f 6e5f 7370 2e73 6574 4368 6563  utton_sp.setChec
+0000fa30: 6b65 6428 5472 7565 290a 0a20 2020 2020  ked(True)..     
+0000fa40: 2020 2069 6620 7365 6c66 2e70 7265 662e     if self.pref.
+0000fa50: 6765 7428 2263 6f6d 6d61 6e64 5f62 7574  get("command_but
+0000fa60: 746f 6e73 2229 3a0a 2020 2020 2020 2020  tons"):.        
+0000fa70: 2020 2020 7365 6c66 2e61 6374 696f 6e43      self.actionC
+0000fa80: 6f6d 6d61 6e64 5f42 7574 746f 6e73 2e73  ommand_Buttons.s
+0000fa90: 6574 4368 6563 6b65 6428 5472 7565 290a  etChecked(True).
+0000faa0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000fab0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+0000fac0: 6374 696f 6e43 6f6d 6d61 6e64 5f42 7574  ctionCommand_But
+0000fad0: 746f 6e73 2e73 6574 4368 6563 6b65 6428  tons.setChecked(
+0000fae0: 4661 6c73 6529 0a0a 2020 2020 2020 2020  False)..        
+0000faf0: 6966 2073 656c 662e 7072 6566 2e67 6574  if self.pref.get
+0000fb00: 2822 6377 5f6d 6163 726f 7322 293a 0a20  ("cw_macros"):. 
+0000fb10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000fb20: 6163 7469 6f6e 4357 5f4d 6163 726f 732e  actionCW_Macros.
+0000fb30: 7365 7443 6865 636b 6564 2854 7275 6529  setChecked(True)
+0000fb40: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+0000fb50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000fb60: 6163 7469 6f6e 4357 5f4d 6163 726f 732e  actionCW_Macros.
+0000fb70: 7365 7443 6865 636b 6564 2846 616c 7365  setChecked(False
+0000fb80: 290a 0a20 2020 2020 2020 2069 6620 7365  )..        if se
+0000fb90: 6c66 2e70 7265 662e 6765 7428 2262 616e  lf.pref.get("ban
+0000fba0: 6473 5f6d 6f64 6573 2229 3a0a 2020 2020  ds_modes"):.    
+0000fbb0: 2020 2020 2020 2020 7365 6c66 2e61 6374          self.act
+0000fbc0: 696f 6e4d 6f64 655f 616e 645f 4261 6e64  ionMode_and_Band
+0000fbd0: 732e 7365 7443 6865 636b 6564 2854 7275  s.setChecked(Tru
+0000fbe0: 6529 0a20 2020 2020 2020 2065 6c73 653a  e).        else:
+0000fbf0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000fc00: 662e 6163 7469 6f6e 4d6f 6465 5f61 6e64  f.actionMode_and
+0000fc10: 5f42 616e 6473 2e73 6574 4368 6563 6b65  _Bands.setChecke
+0000fc20: 6428 4661 6c73 6529 0a0a 2020 2020 2020  d(False)..      
+0000fc30: 2020 6d75 6c74 6963 6173 745f 6772 6f75    multicast_grou
+0000fc40: 7020 3d20 7365 6c66 2e70 7265 662e 6765  p = self.pref.ge
+0000fc50: 7428 226d 756c 7469 6361 7374 5f67 726f  t("multicast_gro
+0000fc60: 7570 222c 2022 3233 392e 312e 312e 3122  up", "239.1.1.1"
+0000fc70: 290a 2020 2020 2020 2020 6d75 6c74 6963  ).        multic
+0000fc80: 6173 745f 706f 7274 203d 2073 656c 662e  ast_port = self.
+0000fc90: 7072 6566 2e67 6574 2822 6d75 6c74 6963  pref.get("multic
+0000fca0: 6173 745f 706f 7274 222c 2032 3233 3929  ast_port", 2239)
+0000fcb0: 0a20 2020 2020 2020 2069 6e74 6572 6661  .        interfa
+0000fcc0: 6365 5f69 7020 3d20 7365 6c66 2e70 7265  ce_ip = self.pre
+0000fcd0: 662e 6765 7428 2269 6e74 6572 6661 6365  f.get("interface
+0000fce0: 5f69 7022 2c20 2230 2e30 2e30 2e30 2229  _ip", "0.0.0.0")
+0000fcf0: 0a20 2020 2020 2020 2073 656c 662e 6d75  .        self.mu
+0000fd00: 6c74 6963 6173 745f 696e 7465 7266 6163  lticast_interfac
+0000fd10: 6520 3d20 4d75 6c74 6963 6173 7428 0a20  e = Multicast(. 
+0000fd20: 2020 2020 2020 2020 2020 206d 756c 7469             multi
+0000fd30: 6361 7374 5f67 726f 7570 2c20 6d75 6c74  cast_group, mult
+0000fd40: 6963 6173 745f 706f 7274 2c20 696e 7465  icast_port, inte
+0000fd50: 7266 6163 655f 6970 0a20 2020 2020 2020  rface_ip.       
+0000fd60: 2029 0a20 2020 2020 2020 2073 656c 662e   ).        self.
+0000fd70: 6d75 6c74 6963 6173 745f 696e 7465 7266  multicast_interf
+0000fd80: 6163 652e 7265 6164 795f 7265 6164 5f63  ace.ready_read_c
+0000fd90: 6f6e 6e65 6374 2873 656c 662e 7761 7463  onnect(self.watc
+0000fda0: 685f 7564 7029 0a0a 2020 2020 2020 2020  h_udp)..        
+0000fdb0: 7365 6c66 2e72 6967 5f63 6f6e 7472 6f6c  self.rig_control
+0000fdc0: 203d 204e 6f6e 650a 0a20 2020 2020 2020   = None..       
+0000fdd0: 2069 6620 7365 6c66 2e70 7265 662e 6765   if self.pref.ge
+0000fde0: 7428 2275 7365 666c 7269 6722 2c20 4661  t("useflrig", Fa
+0000fdf0: 6c73 6529 3a0a 2020 2020 2020 2020 2020  lse):.          
+0000fe00: 2020 6c6f 6767 6572 2e64 6562 7567 280a    logger.debug(.
+0000fe10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fe20: 2255 7369 6e67 2066 6c72 6967 3a20 2573  "Using flrig: %s
+0000fe30: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+0000fe40: 2020 2066 227b 7365 6c66 2e70 7265 662e     f"{self.pref.
+0000fe50: 6765 7428 2743 4154 5f69 7027 297d 207b  get('CAT_ip')} {
+0000fe60: 7365 6c66 2e70 7265 662e 6765 7428 2743  self.pref.get('C
+0000fe70: 4154 5f70 6f72 7427 297d 222c 0a20 2020  AT_port')}",.   
+0000fe80: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0000fe90: 2020 2020 2020 2073 656c 662e 7269 675f         self.rig_
+0000fea0: 636f 6e74 726f 6c20 3d20 4341 5428 0a20  control = CAT(. 
+0000feb0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0000fec0: 666c 7269 6722 2c0a 2020 2020 2020 2020  flrig",.        
+0000fed0: 2020 2020 2020 2020 7365 6c66 2e70 7265          self.pre
+0000fee0: 662e 6765 7428 2243 4154 5f69 7022 2c20  f.get("CAT_ip", 
+0000fef0: 2231 3237 2e30 2e30 2e31 2229 2c0a 2020  "127.0.0.1"),.  
+0000ff00: 2020 2020 2020 2020 2020 2020 2020 696e                in
+0000ff10: 7428 7365 6c66 2e70 7265 662e 6765 7428  t(self.pref.get(
+0000ff20: 2243 4154 5f70 6f72 7422 2c20 3132 3334  "CAT_port", 1234
+0000ff30: 3529 292c 0a20 2020 2020 2020 2020 2020  5)),.           
+0000ff40: 2029 0a20 2020 2020 2020 2069 6620 7365   ).        if se
+0000ff50: 6c66 2e70 7265 662e 6765 7428 2275 7365  lf.pref.get("use
+0000ff60: 7269 6763 746c 6422 2c20 4661 6c73 6529  rigctld", False)
+0000ff70: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
+0000ff80: 6767 6572 2e64 6562 7567 280a 2020 2020  gger.debug(.    
+0000ff90: 2020 2020 2020 2020 2020 2020 2255 7369              "Usi
+0000ffa0: 6e67 2072 6967 6374 6c64 3a20 2573 222c  ng rigctld: %s",
+0000ffb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ffc0: 2066 227b 7365 6c66 2e70 7265 662e 6765   f"{self.pref.ge
+0000ffd0: 7428 2743 4154 5f69 7027 297d 207b 7365  t('CAT_ip')} {se
+0000ffe0: 6c66 2e70 7265 662e 6765 7428 2743 4154  lf.pref.get('CAT
+0000fff0: 5f70 6f72 7427 297d 222c 0a20 2020 2020  _port')}",.     
+00010000: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00010010: 2020 2020 2073 656c 662e 7269 675f 636f       self.rig_co
+00010020: 6e74 726f 6c20 3d20 4341 5428 0a20 2020  ntrol = CAT(.   
+00010030: 2020 2020 2020 2020 2020 2020 2022 7269               "ri
+00010040: 6763 746c 6422 2c0a 2020 2020 2020 2020  gctld",.        
+00010050: 2020 2020 2020 2020 7365 6c66 2e70 7265          self.pre
+00010060: 662e 6765 7428 2243 4154 5f69 7022 2c20  f.get("CAT_ip", 
+00010070: 2231 3237 2e30 2e30 2e31 2229 2c0a 2020  "127.0.0.1"),.  
+00010080: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00010090: 7428 7365 6c66 2e70 7265 662e 6765 7428  t(self.pref.get(
+000100a0: 2243 4154 5f70 6f72 7422 2c20 3435 3332  "CAT_port", 4532
+000100b0: 2929 2c0a 2020 2020 2020 2020 2020 2020  )),.            
+000100c0: 290a 0a20 2020 2020 2020 2069 6620 7365  )..        if se
+000100d0: 6c66 2e70 7265 662e 6765 7428 2263 7774  lf.pref.get("cwt
+000100e0: 7970 6522 2c20 3029 203d 3d20 303a 0a20  ype", 0) == 0:. 
+000100f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00010100: 6377 203d 204e 6f6e 650a 2020 2020 2020  cw = None.      
+00010110: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00010120: 2020 2020 7365 6c66 2e63 7720 3d20 4357      self.cw = CW
+00010130: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00010140: 2020 696e 7428 7365 6c66 2e70 7265 662e    int(self.pref.
+00010150: 6765 7428 2263 7774 7970 6522 2929 2c0a  get("cwtype")),.
+00010160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010170: 7365 6c66 2e70 7265 662e 6765 7428 2263  self.pref.get("c
+00010180: 7769 7022 292c 0a20 2020 2020 2020 2020  wip"),.         
+00010190: 2020 2020 2020 2069 6e74 2873 656c 662e         int(self.
+000101a0: 7072 6566 2e67 6574 2822 6377 706f 7274  pref.get("cwport
+000101b0: 222c 2036 3738 3929 292c 0a20 2020 2020  ", 6789)),.     
+000101c0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+000101d0: 2020 2020 2073 656c 662e 6377 2e73 7065       self.cw.spe
+000101e0: 6564 203d 2032 300a 2020 2020 2020 2020  ed = 20.        
+000101f0: 2020 2020 6966 2073 656c 662e 6377 2e73      if self.cw.s
+00010200: 6572 7665 7274 7970 6520 3d3d 2032 3a0a  ervertype == 2:.
+00010210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010220: 7365 6c66 2e63 772e 7365 745f 7769 6e6b  self.cw.set_wink
+00010230: 6579 6572 5f73 7065 6564 2832 3029 0a0a  eyer_speed(20)..
+00010240: 2020 2020 2020 2020 7365 6c66 2e6e 316d          self.n1m
+00010250: 6d20 3d20 4e6f 6e65 0a20 2020 2020 2020  m = None.       
+00010260: 2069 6620 7365 6c66 2e70 7265 662e 6765   if self.pref.ge
+00010270: 7428 2273 656e 645f 6e31 6d6d 5f70 6163  t("send_n1mm_pac
+00010280: 6b65 7473 222c 2046 616c 7365 293a 0a20  kets", False):. 
+00010290: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
+000102a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000102b0: 7365 6c66 2e6e 316d 6d20 3d20 4e31 4d4d  self.n1mm = N1MM
+000102c0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000102d0: 2020 2020 2020 7365 6c66 2e70 7265 662e        self.pref.
+000102e0: 6765 7428 226e 316d 6d5f 7261 6469 6f70  get("n1mm_radiop
+000102f0: 6f72 7422 2c20 2231 3237 2e30 2e30 2e31  ort", "127.0.0.1
+00010300: 3a31 3230 3630 2229 2c0a 2020 2020 2020  :12060"),.      
+00010310: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00010320: 6c66 2e70 7265 662e 6765 7428 226e 316d  lf.pref.get("n1m
+00010330: 6d5f 636f 6e74 6163 7470 6f72 7422 2c20  m_contactport", 
+00010340: 2231 3237 2e30 2e30 2e31 3a31 3230 3631  "127.0.0.1:12061
+00010350: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
+00010360: 2020 2020 2020 2020 7365 6c66 2e70 7265          self.pre
+00010370: 662e 6765 7428 226e 316d 6d5f 6c6f 6f6b  f.get("n1mm_look
+00010380: 7570 706f 7274 222c 2022 3132 372e 302e  upport", "127.0.
+00010390: 302e 313a 3132 3036 3022 292c 0a20 2020  0.1:12060"),.   
+000103a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000103b0: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
+000103c0: 6e31 6d6d 5f73 636f 7265 706f 7274 222c  n1mm_scoreport",
+000103d0: 2022 3132 372e 302e 302e 313a 3132 3036   "127.0.0.1:1206
+000103e0: 3022 292c 0a20 2020 2020 2020 2020 2020  0"),.           
+000103f0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00010400: 2020 2065 7863 6570 7420 5661 6c75 6545     except ValueE
+00010410: 7272 6f72 3a0a 2020 2020 2020 2020 2020  rror:.          
+00010420: 2020 2020 2020 6c6f 6767 6572 2e77 6172        logger.war
+00010430: 6e69 6e67 2822 2573 222c 2066 227b 5661  ning("%s", f"{Va
+00010440: 6c75 6545 7272 6f72 7d22 290a 2020 2020  lueError}").    
+00010450: 2020 2020 2020 2020 7365 6c66 2e6e 316d          self.n1m
+00010460: 6d2e 7365 6e64 5f72 6164 696f 5f70 6163  m.send_radio_pac
+00010470: 6b65 7473 203d 2073 656c 662e 7072 6566  kets = self.pref
+00010480: 2e67 6574 2822 7365 6e64 5f6e 316d 6d5f  .get("send_n1mm_
+00010490: 7261 6469 6f22 2c20 4661 6c73 6529 0a20  radio", False). 
+000104a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000104b0: 6e31 6d6d 2e73 656e 645f 636f 6e74 6163  n1mm.send_contac
+000104c0: 745f 7061 636b 6574 7320 3d20 7365 6c66  t_packets = self
+000104d0: 2e70 7265 662e 6765 7428 2273 656e 645f  .pref.get("send_
+000104e0: 6e31 6d6d 5f63 6f6e 7461 6374 222c 2046  n1mm_contact", F
+000104f0: 616c 7365 290a 2020 2020 2020 2020 2020  alse).          
+00010500: 2020 7365 6c66 2e6e 316d 6d2e 7365 6e64    self.n1mm.send
+00010510: 5f6c 6f6f 6b75 705f 7061 636b 6574 7320  _lookup_packets 
+00010520: 3d20 7365 6c66 2e70 7265 662e 6765 7428  = self.pref.get(
+00010530: 2273 656e 645f 6e31 6d6d 5f6c 6f6f 6b75  "send_n1mm_looku
+00010540: 7022 2c20 4661 6c73 6529 0a20 2020 2020  p", False).     
+00010550: 2020 2020 2020 2073 656c 662e 6e31 6d6d         self.n1mm
+00010560: 2e73 656e 645f 7363 6f72 655f 7061 636b  .send_score_pack
+00010570: 6574 7320 3d20 7365 6c66 2e70 7265 662e  ets = self.pref.
+00010580: 6765 7428 2273 656e 645f 6e31 6d6d 5f73  get("send_n1mm_s
+00010590: 636f 7265 222c 2046 616c 7365 290a 2020  core", False).  
+000105a0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+000105b0: 316d 6d2e 7261 6469 6f5f 696e 666f 5b22  1mm.radio_info["
+000105c0: 5374 6174 696f 6e4e 616d 6522 5d20 3d20  StationName"] = 
+000105d0: 7365 6c66 2e70 7265 662e 6765 7428 226e  self.pref.get("n
+000105e0: 316d 6d5f 7374 6174 696f 6e5f 6e61 6d65  1mm_station_name
+000105f0: 222c 2022 2229 0a0a 2020 2020 2020 2020  ", "")..        
+00010600: 7365 6c66 2e73 686f 775f 636f 6d6d 616e  self.show_comman
+00010610: 645f 6275 7474 6f6e 7328 290a 2020 2020  d_buttons().    
+00010620: 2020 2020 7365 6c66 2e73 686f 775f 4357      self.show_CW
+00010630: 5f6d 6163 726f 7328 290a 2020 2020 2020  _macros().      
+00010640: 2020 2320 7365 6c66 2e73 686f 775f 6261    # self.show_ba
+00010650: 6e64 5f6d 6f64 6528 290a 0a20 2020 2064  nd_mode()..    d
+00010660: 6566 2077 6174 6368 5f75 6470 2873 656c  ef watch_udp(sel
+00010670: 6629 3a0a 2020 2020 2020 2020 2222 2250  f):.        """P
+00010680: 726f 6365 7373 2055 4450 2064 6174 6167  rocess UDP datag
+00010690: 7261 6d73 2e22 2222 0a20 2020 2020 2020  rams.""".       
+000106a0: 2077 6869 6c65 2073 656c 662e 6d75 6c74   while self.mult
+000106b0: 6963 6173 745f 696e 7465 7266 6163 652e  icast_interface.
+000106c0: 7365 7276 6572 5f75 6470 2e68 6173 5065  server_udp.hasPe
+000106d0: 6e64 696e 6744 6174 6167 7261 6d73 2829  ndingDatagrams()
+000106e0: 3a0a 2020 2020 2020 2020 2020 2020 6275  :.            bu
+000106f0: 6e64 6c65 203d 2073 656c 662e 6d75 6c74  ndle = self.mult
+00010700: 6963 6173 745f 696e 7465 7266 6163 652e  icast_interface.
+00010710: 7365 7276 6572 5f75 6470 2e72 6561 6444  server_udp.readD
+00010720: 6174 6167 7261 6d28 0a20 2020 2020 2020  atagram(.       
+00010730: 2020 2020 2020 2020 2073 656c 662e 6d75           self.mu
+00010740: 6c74 6963 6173 745f 696e 7465 7266 6163  lticast_interfac
+00010750: 652e 7365 7276 6572 5f75 6470 2e70 656e  e.server_udp.pen
+00010760: 6469 6e67 4461 7461 6772 616d 5369 7a65  dingDatagramSize
+00010770: 2829 0a20 2020 2020 2020 2020 2020 2029  ().            )
+00010780: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+00010790: 6167 7261 6d2c 205f 2c20 5f20 3d20 6275  agram, _, _ = bu
+000107a0: 6e64 6c65 0a20 2020 2020 2020 2020 2020  ndle.           
+000107b0: 2023 206c 6f67 6765 722e 6465 6275 6728   # logger.debug(
+000107c0: 6461 7461 6772 616d 2e64 6563 6f64 6528  datagram.decode(
+000107d0: 2929 0a20 2020 2020 2020 2020 2020 2069  )).            i
+000107e0: 6620 6461 7461 6772 616d 3a0a 2020 2020  f datagram:.    
+000107f0: 2020 2020 2020 2020 2020 2020 7472 793a              try:
+00010800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010810: 2020 2020 2023 2064 6562 7567 5f69 6e66       # debug_inf
+00010820: 6f20 3d20 6622 7b64 6174 6167 7261 6d2e  o = f"{datagram.
+00010830: 6465 636f 6465 2829 7d22 0a20 2020 2020  decode()}".     
+00010840: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00010850: 206c 6f67 6765 722e 6465 6275 6728 6465   logger.debug(de
+00010860: 6275 675f 696e 666f 290a 2020 2020 2020  bug_info).      
+00010870: 2020 2020 2020 2020 2020 2020 2020 6a73                js
+00010880: 6f6e 5f64 6174 6120 3d20 6c6f 6164 7328  on_data = loads(
+00010890: 6461 7461 6772 616d 2e64 6563 6f64 6528  datagram.decode(
+000108a0: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+000108b0: 2020 2065 7863 6570 7420 556e 6963 6f64     except Unicod
+000108c0: 6544 6563 6f64 6545 7272 6f72 2061 7320  eDecodeError as 
+000108d0: 6572 723a 0a20 2020 2020 2020 2020 2020  err:.           
+000108e0: 2020 2020 2020 2020 2074 6865 5f65 7272           the_err
+000108f0: 6f72 203d 2066 224e 6f74 2055 6e69 636f  or = f"Not Unico
+00010900: 6465 3a20 7b65 7272 7d5c 6e7b 6461 7461  de: {err}\n{data
+00010910: 6772 616d 7d22 0a20 2020 2020 2020 2020  gram}".         
+00010920: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+00010930: 722e 7761 726e 696e 6728 7468 655f 6572  r.warning(the_er
+00010940: 726f 7229 0a20 2020 2020 2020 2020 2020  ror).           
+00010950: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
+00010960: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00010970: 2020 6578 6365 7074 204a 534f 4e44 6563    except JSONDec
+00010980: 6f64 6545 7272 6f72 2061 7320 6572 723a  odeError as err:
+00010990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000109a0: 2020 2020 2074 6865 5f65 7272 6f72 203d       the_error =
+000109b0: 2066 224e 6f74 204a 534f 4e3a 207b 6572   f"Not JSON: {er
+000109c0: 727d 5c6e 7b64 6174 6167 7261 6d7d 220a  r}\n{datagram}".
+000109d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000109e0: 2020 2020 6c6f 6767 6572 2e77 6172 6e69      logger.warni
+000109f0: 6e67 2874 6865 5f65 7272 6f72 290a 2020  ng(the_error).  
+00010a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a10: 2020 636f 6e74 696e 7565 0a20 2020 2020    continue.     
+00010a20: 2020 2020 2020 2020 2020 2069 6620 280a             if (.
+00010a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a40: 2020 2020 6a73 6f6e 5f64 6174 612e 6765      json_data.ge
+00010a50: 7428 2263 6d64 222c 2022 2229 203d 3d20  t("cmd", "") == 
+00010a60: 2247 4554 434f 4c55 4d4e 5322 0a20 2020  "GETCOLUMNS".   
+00010a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a80: 2061 6e64 206a 736f 6e5f 6461 7461 2e67   and json_data.g
+00010a90: 6574 2822 7374 6174 696f 6e22 2c20 2222  et("station", ""
+00010aa0: 2920 3d3d 2070 6c61 7466 6f72 6d2e 6e6f  ) == platform.no
+00010ab0: 6465 2829 0a20 2020 2020 2020 2020 2020  de().           
+00010ac0: 2020 2020 2029 3a0a 2020 2020 2020 2020       ):.        
+00010ad0: 2020 2020 2020 2020 2020 2020 6966 2068              if h
+00010ae0: 6173 6174 7472 2873 656c 662e 636f 6e74  asattr(self.cont
+00010af0: 6573 742c 2022 636f 6c75 6d6e 7322 293a  est, "columns"):
+00010b00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010b10: 2020 2020 2020 2020 2063 6d64 203d 207b           cmd = {
+00010b20: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00010b30: 2020 2020 2020 2020 2020 636d 645b 2263            cmd["c
+00010b40: 6d64 225d 203d 2022 5348 4f57 434f 4c55  md"] = "SHOWCOLU
+00010b50: 4d4e 5322 0a20 2020 2020 2020 2020 2020  MNS".           
+00010b60: 2020 2020 2020 2020 2020 2020 2063 6d64               cmd
+00010b70: 5b22 7374 6174 696f 6e22 5d20 3d20 706c  ["station"] = pl
+00010b80: 6174 666f 726d 2e6e 6f64 6528 290a 2020  atform.node().  
+00010b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ba0: 2020 2020 2020 636d 645b 2243 4f4c 554d        cmd["COLUM
+00010bb0: 4e53 225d 203d 2073 656c 662e 636f 6e74  NS"] = self.cont
+00010bc0: 6573 742e 636f 6c75 6d6e 730a 2020 2020  est.columns.    
 00010bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010be0: 2020 2020 7365 6c66 2e63 6f6e 7461 6374      self.contact
-00010bf0: 5b22 4772 6964 5371 7561 7265 225d 203d  ["GridSquare"] =
-00010c00: 2074 6865 6972 6772 6964 0a20 2020 2020   theirgrid.     
-00010c10: 2020 2020 2020 2020 2020 2020 2020 205f                 _
-00010c20: 7468 6569 7263 6f75 6e74 7279 203d 2072  theircountry = r
-00010c30: 6573 706f 6e73 652e 6765 7428 2263 6f75  esponse.get("cou
-00010c40: 6e74 7279 2229 0a20 2020 2020 2020 2020  ntry").         
-00010c50: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00010c60: 6c66 2e73 7461 7469 6f6e 2e67 6574 2822  lf.station.get("
-00010c70: 4772 6964 5371 7561 7265 222c 2022 2229  GridSquare", "")
-00010c80: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00010c90: 2020 2020 2020 2020 2020 6865 6164 696e            headin
-00010ca0: 6720 3d20 6265 6172 696e 6728 7365 6c66  g = bearing(self
-00010cb0: 2e73 7461 7469 6f6e 2e67 6574 2822 4772  .station.get("Gr
-00010cc0: 6964 5371 7561 7265 222c 2022 2229 2c20  idSquare", ""), 
-00010cd0: 7468 6569 7267 7269 6429 0a20 2020 2020  theirgrid).     
-00010ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010cf0: 2020 206b 696c 6f6d 6574 6572 7320 3d20     kilometers = 
-00010d00: 6469 7374 616e 6365 2873 656c 662e 7374  distance(self.st
-00010d10: 6174 696f 6e2e 6765 7428 2247 7269 6453  ation.get("GridS
-00010d20: 7175 6172 6522 292c 2074 6865 6972 6772  quare"), theirgr
-00010d30: 6964 290a 2020 2020 2020 2020 2020 2020  id).            
-00010d40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00010d50: 2e68 6561 6469 6e67 5f64 6973 7461 6e63  .heading_distanc
-00010d60: 652e 7365 7454 6578 7428 0a20 2020 2020  e.setText(.     
-00010d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d80: 2020 2020 2020 2066 227b 7468 6569 7267         f"{theirg
-00010d90: 7269 647d 2048 6467 207b 6865 6164 696e  rid} Hdg {headin
-00010da0: 677d c2b0 204c 5020 7b72 6563 6970 726f  g}.. LP {recipro
-00010db0: 636f 6c28 6865 6164 696e 6729 7dc2 b020  col(heading)}.. 
-00010dc0: 2f20 220a 2020 2020 2020 2020 2020 2020  / ".            
-00010dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010de0: 6622 6469 7374 616e 6365 207b 696e 7428  f"distance {int(
-00010df0: 6b69 6c6f 6d65 7465 7273 2a30 2e36 3231  kilometers*0.621
-00010e00: 3337 3129 7d6d 6920 7b6b 696c 6f6d 6574  371)}mi {kilomet
-00010e10: 6572 737d 6b6d 220a 2020 2020 2020 2020  ers}km".        
-00010e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e30: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00010e40: 2020 2020 2020 2320 7365 6c66 2e64 785f        # self.dx_
-00010e50: 656e 7469 7479 2e73 6574 5465 7874 2866  entity.setText(f
-00010e60: 227b 7468 6569 7263 6f75 6e74 7279 7d22  "{theircountry}"
-00010e70: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00010e80: 2020 2320 656c 7365 3a0a 2020 2020 2020    # else:.      
-00010e90: 2020 2020 2020 2020 2020 2320 7365 6c66            # self
-00010ea0: 2e68 6561 6469 6e67 5f64 6973 7461 6e63  .heading_distanc
-00010eb0: 652e 7365 7454 6578 7428 224c 6f6f 6b75  e.setText("Looku
-00010ec0: 7020 6661 696c 6564 2e22 290a 0a20 2020  p failed.")..   
-00010ed0: 2064 6566 2063 6865 636b 5f64 7570 6528   def check_dupe(
-00010ee0: 7365 6c66 2c20 6361 6c6c 3a20 7374 7229  self, call: str)
-00010ef0: 202d 3e20 626f 6f6c 3a0a 2020 2020 2020   -> bool:.      
-00010f00: 2020 2222 2243 6865 636b 7320 6966 2061    """Checks if a
-00010f10: 2063 616c 6c73 6967 6e20 6973 2061 2064   callsign is a d
-00010f20: 7570 6520 6f6e 2063 7572 7265 6e74 2062  upe on current b
-00010f30: 616e 642f 6d6f 6465 2e22 2222 0a20 2020  and/mode.""".   
-00010f40: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
-00010f50: 742e 7072 6564 7570 6528 7365 6c66 290a  t.predupe(self).
-00010f60: 2020 2020 2020 2020 6261 6e64 203d 2066          band = f
-00010f70: 6c6f 6174 2867 6574 5f6c 6f67 6765 645f  loat(get_logged_
-00010f80: 6261 6e64 2873 7472 2873 656c 662e 7261  band(str(self.ra
-00010f90: 6469 6f5f 7374 6174 652e 6765 7428 2276  dio_state.get("v
-00010fa0: 666f 6122 2c20 302e 3029 2929 290a 2020  foa", 0.0)))).  
-00010fb0: 2020 2020 2020 6d6f 6465 203d 2073 656c        mode = sel
-00010fc0: 662e 7261 6469 6f5f 7374 6174 652e 6765  f.radio_state.ge
-00010fd0: 7428 226d 6f64 6522 2c20 2222 290a 2020  t("mode", "").  
-00010fe0: 2020 2020 2020 6465 6275 676c 696e 6520        debugline 
-00010ff0: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-00011000: 6622 4361 6c6c 3a20 7b63 616c 6c7d 2042  f"Call: {call} B
-00011010: 616e 643a 207b 6261 6e64 7d20 4d6f 6465  and: {band} Mode
-00011020: 3a20 7b6d 6f64 657d 2044 7570 6574 7970  : {mode} Dupetyp
-00011030: 653a 207b 7365 6c66 2e63 6f6e 7465 7374  e: {self.contest
-00011040: 2e64 7570 655f 7479 7065 7d22 0a20 2020  .dupe_type}".   
-00011050: 2020 2020 2029 0a20 2020 2020 2020 206c       ).        l
-00011060: 6f67 6765 722e 6465 6275 6728 2225 7322  ogger.debug("%s"
-00011070: 2c20 6465 6275 676c 696e 6529 0a20 2020  , debugline).   
-00011080: 2020 2020 2069 6620 7365 6c66 2e63 6f6e       if self.con
-00011090: 7465 7374 2e64 7570 655f 7479 7065 203d  test.dupe_type =
-000110a0: 3d20 313a 0a20 2020 2020 2020 2020 2020  = 1:.           
-000110b0: 2072 6573 756c 7420 3d20 7365 6c66 2e64   result = self.d
-000110c0: 6174 6162 6173 652e 6368 6563 6b5f 6475  atabase.check_du
-000110d0: 7065 2863 616c 6c29 0a20 2020 2020 2020  pe(call).       
-000110e0: 2069 6620 7365 6c66 2e63 6f6e 7465 7374   if self.contest
-000110f0: 2e64 7570 655f 7479 7065 203d 3d20 323a  .dupe_type == 2:
-00011100: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00011110: 756c 7420 3d20 7365 6c66 2e64 6174 6162  ult = self.datab
-00011120: 6173 652e 6368 6563 6b5f 6475 7065 5f6f  ase.check_dupe_o
-00011130: 6e5f 6261 6e64 2863 616c 6c2c 2062 616e  n_band(call, ban
-00011140: 6429 0a20 2020 2020 2020 2069 6620 7365  d).        if se
-00011150: 6c66 2e63 6f6e 7465 7374 2e64 7570 655f  lf.contest.dupe_
-00011160: 7479 7065 203d 3d20 333a 0a20 2020 2020  type == 3:.     
-00011170: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-00011180: 7365 6c66 2e64 6174 6162 6173 652e 6368  self.database.ch
-00011190: 6563 6b5f 6475 7065 5f6f 6e5f 6261 6e64  eck_dupe_on_band
-000111a0: 5f6d 6f64 6528 6361 6c6c 2c20 6261 6e64  _mode(call, band
-000111b0: 2c20 6d6f 6465 290a 2020 2020 2020 2020  , mode).        
-000111c0: 6966 2073 656c 662e 636f 6e74 6573 742e  if self.contest.
-000111d0: 6475 7065 5f74 7970 6520 3d3d 2034 3a0a  dupe_type == 4:.
-000111e0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-000111f0: 6c74 203d 207b 2269 7364 7570 6522 3a20  lt = {"isdupe": 
-00011200: 4661 6c73 657d 0a20 2020 2020 2020 2064  False}.        d
-00011210: 6562 7567 6c69 6e65 203d 2066 227b 7265  ebugline = f"{re
-00011220: 7375 6c74 7d22 0a20 2020 2020 2020 206c  sult}".        l
-00011230: 6f67 6765 722e 6465 6275 6728 2225 7322  ogger.debug("%s"
-00011240: 2c20 6465 6275 676c 696e 6529 0a20 2020  , debugline).   
-00011250: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
-00011260: 6c74 2e67 6574 2822 6973 6475 7065 222c  lt.get("isdupe",
-00011270: 2046 616c 7365 290a 0a20 2020 2064 6566   False)..    def
-00011280: 2073 6574 6d6f 6465 2873 656c 662c 206d   setmode(self, m
-00011290: 6f64 653a 2073 7472 2920 2d3e 204e 6f6e  ode: str) -> Non
-000112a0: 653a 0a20 2020 2020 2020 2022 2222 7374  e:.        """st
-000112b0: 7562 2066 6f72 2077 6865 6e20 7468 6520  ub for when the 
-000112c0: 6d6f 6465 2063 6861 6e67 6573 2e22 2222  mode changes."""
-000112d0: 0a20 2020 2020 2020 2069 6620 6d6f 6465  .        if mode
-000112e0: 203d 3d20 2243 5722 3a0a 2020 2020 2020   == "CW":.      
-000112f0: 2020 2020 2020 7365 6c66 2e63 7572 7265        self.curre
-00011300: 6e74 5f6d 6f64 6520 3d20 2243 5722 0a20  nt_mode = "CW". 
-00011310: 2020 2020 2020 2020 2020 2023 2073 656c             # sel
-00011320: 662e 6d6f 6465 2e73 6574 5465 7874 2822  f.mode.setText("
-00011330: 4357 2229 0a20 2020 2020 2020 2020 2020  CW").           
-00011340: 2073 656c 662e 7365 6e74 2e73 6574 5465   self.sent.setTe
-00011350: 7874 2822 3539 3922 290a 2020 2020 2020  xt("599").      
-00011360: 2020 2020 2020 7365 6c66 2e72 6563 6569        self.recei
-00011370: 7665 2e73 6574 5465 7874 2822 3539 3922  ve.setText("599"
-00011380: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00011390: 6c66 2e72 6561 645f 6377 5f6d 6163 726f  lf.read_cw_macro
-000113a0: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
-000113b0: 7265 7475 726e 0a20 2020 2020 2020 2069  return.        i
-000113c0: 6620 6d6f 6465 203d 3d20 2253 5342 223a  f mode == "SSB":
-000113d0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000113e0: 662e 6375 7272 656e 745f 6d6f 6465 203d  f.current_mode =
-000113f0: 2022 5353 4222 0a20 2020 2020 2020 2020   "SSB".         
-00011400: 2020 2023 2073 656c 662e 6d6f 6465 2e73     # self.mode.s
-00011410: 6574 5465 7874 2822 5353 4222 290a 2020  etText("SSB").  
-00011420: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-00011430: 656e 742e 7365 7454 6578 7428 2235 3922  ent.setText("59"
-00011440: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00011450: 6c66 2e72 6563 6569 7665 2e73 6574 5465  lf.receive.setTe
-00011460: 7874 2822 3539 2229 0a20 2020 2020 2020  xt("59").       
-00011470: 2020 2020 2073 656c 662e 7265 6164 5f63       self.read_c
-00011480: 775f 6d61 6372 6f73 2829 0a20 2020 2020  w_macros().     
-00011490: 2020 2069 6620 6d6f 6465 203d 3d20 2252     if mode == "R
-000114a0: 5454 5922 3a0a 2020 2020 2020 2020 2020  TTY":.          
-000114b0: 2020 7365 6c66 2e63 7572 7265 6e74 5f6d    self.current_m
-000114c0: 6f64 6520 3d20 2252 5454 5922 0a20 2020  ode = "RTTY".   
-000114d0: 2020 2020 2020 2020 2023 2073 656c 662e           # self.
-000114e0: 6d6f 6465 2e73 6574 5465 7874 2822 5254  mode.setText("RT
-000114f0: 5459 2229 0a20 2020 2020 2020 2020 2020  TY").           
-00011500: 2073 656c 662e 7365 6e74 2e73 6574 5465   self.sent.setTe
-00011510: 7874 2822 3539 2229 0a20 2020 2020 2020  xt("59").       
-00011520: 2020 2020 2073 656c 662e 7265 6365 6976       self.receiv
-00011530: 652e 7365 7454 6578 7428 2235 3922 290a  e.setText("59").
-00011540: 0a20 2020 2064 6566 2067 6574 5f6f 706f  .    def get_opo
-00011550: 6e28 7365 6c66 293a 0a20 2020 2020 2020  n(self):.       
-00011560: 2022 2222 4374 726c 2b4f 206f 7220 4f50   """Ctrl+O or OP
-00011570: 4f4e 2064 6961 6c6f 6722 2222 0a20 2020  ON dialog""".   
-00011580: 2020 2020 2073 656c 662e 6f70 6f6e 5f64       self.opon_d
-00011590: 6961 6c6f 6720 3d20 4f70 4f6e 2857 4f52  ialog = OpOn(WOR
-000115a0: 4b49 4e47 5f50 4154 4829 0a20 2020 2020  KING_PATH).     
-000115b0: 2020 2073 656c 662e 6f70 6f6e 5f64 6961     self.opon_dia
-000115c0: 6c6f 672e 6163 6365 7074 6564 2e63 6f6e  log.accepted.con
-000115d0: 6e65 6374 2873 656c 662e 6e65 775f 6f70  nect(self.new_op
-000115e0: 290a 2020 2020 2020 2020 7365 6c66 2e6f  ).        self.o
-000115f0: 706f 6e5f 6469 616c 6f67 2e6f 7065 6e28  pon_dialog.open(
-00011600: 290a 0a20 2020 2064 6566 206e 6577 5f6f  )..    def new_o
-00011610: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
-00011620: 2022 2222 5361 7665 206e 6577 204f 5022   """Save new OP"
-00011630: 2222 0a20 2020 2020 2020 2069 6620 7365  "".        if se
-00011640: 6c66 2e6f 706f 6e5f 6469 616c 6f67 2e4e  lf.opon_dialog.N
-00011650: 6577 4f70 6572 6174 6f72 2e74 6578 7428  ewOperator.text(
-00011660: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-00011670: 656c 662e 6375 7272 656e 745f 6f70 203d  elf.current_op =
-00011680: 2073 656c 662e 6f70 6f6e 5f64 6961 6c6f   self.opon_dialo
-00011690: 672e 4e65 774f 7065 7261 746f 722e 7465  g.NewOperator.te
-000116a0: 7874 2829 2e75 7070 6572 2829 0a20 2020  xt().upper().   
-000116b0: 2020 2020 2073 656c 662e 6f70 6f6e 5f64       self.opon_d
-000116c0: 6961 6c6f 672e 636c 6f73 6528 290a 2020  ialog.close().  
-000116d0: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-000116e0: 7567 2822 4e65 7720 4f70 3a20 2573 222c  ug("New Op: %s",
-000116f0: 2073 656c 662e 6375 7272 656e 745f 6f70   self.current_op
-00011700: 290a 2020 2020 2020 2020 7365 6c66 2e6d  ).        self.m
-00011710: 616b 655f 6f70 5f64 6972 2829 0a0a 2020  ake_op_dir()..  
-00011720: 2020 6465 6620 6d61 6b65 5f6f 705f 6469    def make_op_di
-00011730: 7228 7365 6c66 293a 0a20 2020 2020 2020  r(self):.       
-00011740: 2022 2222 4372 6561 7465 204f 5020 6469   """Create OP di
-00011750: 7265 6374 6f72 7920 6966 2069 7420 646f  rectory if it do
-00011760: 6573 206e 6f74 2065 7869 7374 2e22 2222  es not exist."""
-00011770: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00011780: 2e63 7572 7265 6e74 5f6f 703a 0a20 2020  .current_op:.   
-00011790: 2020 2020 2020 2020 206f 705f 7061 7468           op_path
-000117a0: 203d 2050 6174 6828 4441 5441 5f50 4154   = Path(DATA_PAT
-000117b0: 4829 202f 2073 656c 662e 6375 7272 656e  H) / self.curren
-000117c0: 745f 6f70 0a20 2020 2020 2020 2020 2020  t_op.           
-000117d0: 206c 6f67 6765 722e 6465 6275 6728 226f   logger.debug("o
-000117e0: 705f 7061 7468 3a20 2573 222c 2073 7472  p_path: %s", str
-000117f0: 286f 705f 7061 7468 2929 0a20 2020 2020  (op_path)).     
-00011800: 2020 2020 2020 2069 6620 6f70 5f70 6174         if op_pat
-00011810: 682e 6973 5f64 6972 2829 2069 7320 4661  h.is_dir() is Fa
-00011820: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00011830: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-00011840: 6728 2243 7265 6174 696e 6720 4f70 2044  g("Creating Op D
-00011850: 6972 6563 746f 7279 3a20 2573 222c 2073  irectory: %s", s
-00011860: 7472 286f 705f 7061 7468 2929 0a20 2020  tr(op_path)).   
-00011870: 2020 2020 2020 2020 2020 2020 206f 732e               os.
-00011880: 6d6b 6469 7228 7374 7228 6f70 5f70 6174  mkdir(str(op_pat
-00011890: 6829 290a 2020 2020 2020 2020 2020 2020  h)).            
-000118a0: 6966 206f 705f 7061 7468 2e69 735f 6469  if op_path.is_di
-000118b0: 7228 293a 0a20 2020 2020 2020 2020 2020  r():.           
-000118c0: 2020 2020 2073 6f75 7263 655f 7061 7468       source_path
-000118d0: 203d 2050 6174 6828 574f 524b 494e 475f   = Path(WORKING_
-000118e0: 5041 5448 2920 2f20 2264 6174 6122 202f  PATH) / "data" /
-000118f0: 2022 7068 6f6e 6574 6963 7322 0a20 2020   "phonetics".   
-00011900: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-00011910: 6765 722e 6465 6275 6728 2273 6f75 7263  ger.debug("sourc
-00011920: 655f 7061 7468 3a20 2573 222c 2073 7472  e_path: %s", str
-00011930: 2873 6f75 7263 655f 7061 7468 2929 0a20  (source_path)). 
-00011940: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00011950: 6f72 2063 6869 6c64 2069 6e20 736f 7572  or child in sour
-00011960: 6365 5f70 6174 682e 6974 6572 6469 7228  ce_path.iterdir(
-00011970: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00011980: 2020 2020 2020 2064 6573 7469 6e61 7469         destinati
-00011990: 6f6e 5f66 696c 6520 3d20 6f70 5f70 6174  on_file = op_pat
-000119a0: 6820 2f20 6368 696c 642e 6e61 6d65 0a20  h / child.name. 
-000119b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000119c0: 2020 2069 6620 6465 7374 696e 6174 696f     if destinatio
-000119d0: 6e5f 6669 6c65 2e69 735f 6669 6c65 2829  n_file.is_file()
-000119e0: 2069 7320 4661 6c73 653a 0a20 2020 2020   is False:.     
-000119f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a00: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-00011a10: 2244 6573 7469 6e61 7469 6f6e 3a20 2573  "Destination: %s
-00011a20: 222c 2073 7472 2864 6573 7469 6e61 7469  ", str(destinati
-00011a30: 6f6e 5f66 696c 6529 290a 2020 2020 2020  on_file)).      
-00011a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a50: 2020 6465 7374 696e 6174 696f 6e5f 6669    destination_fi
-00011a60: 6c65 2e77 7269 7465 5f62 7974 6573 2863  le.write_bytes(c
-00011a70: 6869 6c64 2e72 6561 645f 6279 7465 7328  hild.read_bytes(
-00011a80: 2929 0a0a 2020 2020 6465 6620 706f 6c6c  ))..    def poll
-00011a90: 5f72 6164 696f 2873 656c 6629 3a0a 2020  _radio(self):.  
-00011aa0: 2020 2020 2020 2222 2273 7475 6222 2222        """stub"""
-00011ab0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00011ac0: 2e72 6967 5f63 6f6e 7472 6f6c 3a0a 2020  .rig_control:.  
-00011ad0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00011ae0: 662e 7269 675f 636f 6e74 726f 6c2e 6f6e  f.rig_control.on
-00011af0: 6c69 6e65 3a0a 2020 2020 2020 2020 2020  line:.          
-00011b00: 2020 2020 2020 7666 6f20 3d20 7365 6c66        vfo = self
-00011b10: 2e72 6967 5f63 6f6e 7472 6f6c 2e67 6574  .rig_control.get
-00011b20: 5f76 666f 2829 0a20 2020 2020 2020 2020  _vfo().         
-00011b30: 2020 2020 2020 206d 6f64 6520 3d20 7365         mode = se
-00011b40: 6c66 2e72 6967 5f63 6f6e 7472 6f6c 2e67  lf.rig_control.g
-00011b50: 6574 5f6d 6f64 6528 290a 2020 2020 2020  et_mode().      
-00011b60: 2020 2020 2020 2020 2020 6277 203d 2073            bw = s
-00011b70: 656c 662e 7269 675f 636f 6e74 726f 6c2e  elf.rig_control.
-00011b80: 6765 745f 6277 2829 0a20 2020 2020 2020  get_bw().       
-00011b90: 2020 2020 2020 2020 2023 2073 656c 662e           # self.
-00011ba0: 7261 6469 6f5f 7374 6174 655b 2270 7474  radio_state["ptt
-00011bb0: 225d 203d 2073 656c 662e 7269 675f 636f  "] = self.rig_co
-00011bc0: 6e74 726f 6c2e 6765 745f 7074 7428 290a  ntrol.get_ptt().
-00011bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011be0: 2320 6966 2073 656c 662e 7261 6469 6f5f  # if self.radio_
-00011bf0: 7374 6174 652e 6765 7428 2270 7474 222c  state.get("ptt",
-00011c00: 2030 2920 3d3d 2031 3a0a 2020 2020 2020   0) == 1:.      
-00011c10: 2020 2020 2020 2020 2020 2320 2020 2020            #     
-00011c20: 7365 6c66 2e6c 6566 7464 6f74 2e73 6574  self.leftdot.set
-00011c30: 5069 786d 6170 2873 656c 662e 6772 6565  Pixmap(self.gree
-00011c40: 6e64 6f74 290a 2020 2020 2020 2020 2020  ndot).          
-00011c50: 2020 2020 2020 2320 656c 7365 3a0a 2020        # else:.  
-00011c60: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00011c70: 2020 2020 7365 6c66 2e6c 6566 7464 6f74      self.leftdot
-00011c80: 2e73 6574 5069 786d 6170 2873 656c 662e  .setPixmap(self.
-00011c90: 7265 6464 6f74 290a 2020 2020 2020 2020  reddot).        
-00011ca0: 2020 2020 2020 2020 6966 206d 6f64 6520          if mode 
-00011cb0: 3d3d 2022 4357 223a 0a20 2020 2020 2020  == "CW":.       
-00011cc0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00011cd0: 662e 7365 746d 6f64 6528 6d6f 6465 290a  f.setmode(mode).
-00011ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011cf0: 6966 206d 6f64 6520 3d3d 2022 4c53 4222  if mode == "LSB"
-00011d00: 206f 7220 6d6f 6465 203d 3d20 2255 5342   or mode == "USB
-00011d10: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
-00011d20: 2020 2020 2020 2073 656c 662e 7365 746d         self.setm
-00011d30: 6f64 6528 2253 5342 2229 0a20 2020 2020  ode("SSB").     
-00011d40: 2020 2020 2020 2020 2020 2069 6620 6d6f             if mo
-00011d50: 6465 203d 3d20 2252 5454 5922 3a0a 2020  de == "RTTY":.  
-00011d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d70: 2020 7365 6c66 2e73 6574 6d6f 6465 2822    self.setmode("
-00011d80: 5254 5459 2229 0a20 2020 2020 2020 2020  RTTY").         
-00011d90: 2020 2020 2020 2073 656c 662e 7261 6469         self.radi
-00011da0: 6f5f 7374 6174 655b 2276 666f 6122 5d20  o_state["vfoa"] 
-00011db0: 3d20 7666 6f0a 2020 2020 2020 2020 2020  = vfo.          
-00011dc0: 2020 2020 2020 6261 6e64 203d 2067 6574        band = get
-00011dd0: 6261 6e64 2873 7472 2876 666f 2929 0a20  band(str(vfo)). 
-00011de0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00011df0: 656c 662e 7261 6469 6f5f 7374 6174 655b  elf.radio_state[
-00011e00: 2262 616e 6422 5d20 3d20 6261 6e64 0a20  "band"] = band. 
-00011e10: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00011e20: 656c 662e 636f 6e74 6163 745b 2242 616e  elf.contact["Ban
-00011e30: 6422 5d20 3d20 6765 745f 6c6f 6767 6564  d"] = get_logged
-00011e40: 5f62 616e 6428 7374 7228 7666 6f29 290a  _band(str(vfo)).
-00011e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e60: 7365 6c66 2e73 6574 5f62 616e 645f 696e  self.set_band_in
-00011e70: 6469 6361 746f 7228 6261 6e64 290a 2020  dicator(band).  
-00011e80: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00011e90: 6c66 2e72 6164 696f 5f73 7461 7465 5b22  lf.radio_state["
-00011ea0: 6d6f 6465 225d 203d 206d 6f64 650a 2020  mode"] = mode.  
-00011eb0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00011ec0: 6c66 2e72 6164 696f 5f73 7461 7465 5b22  lf.radio_state["
-00011ed0: 6277 225d 203d 2062 770a 2020 2020 2020  bw"] = bw.      
-00011ee0: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-00011ef0: 2e64 6562 7567 2822 5646 4f3a 2025 7320  .debug("VFO: %s 
-00011f00: 204d 4f44 453a 2025 7320 4257 3a20 2573   MODE: %s BW: %s
-00011f10: 222c 2076 666f 2c20 6d6f 6465 2c20 6277  ", vfo, mode, bw
-00011f20: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00011f30: 2020 7365 6c66 2e73 6574 5f77 696e 646f    self.set_windo
-00011f40: 775f 7469 746c 6528 290a 2020 2020 2020  w_title().      
-00011f50: 2020 2020 2020 2020 2020 636d 6420 3d20            cmd = 
-00011f60: 7b7d 0a20 2020 2020 2020 2020 2020 2020  {}.             
-00011f70: 2020 2063 6d64 5b22 636d 6422 5d20 3d20     cmd["cmd"] = 
-00011f80: 2252 4144 494f 5f53 5441 5445 220a 2020  "RADIO_STATE".  
-00011f90: 2020 2020 2020 2020 2020 2020 2020 636d                cm
-00011fa0: 645b 2273 7461 7469 6f6e 225d 203d 2070  d["station"] = p
-00011fb0: 6c61 7466 6f72 6d2e 6e6f 6465 2829 0a20  latform.node(). 
-00011fc0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00011fd0: 6d64 5b22 6261 6e64 225d 203d 2062 616e  md["band"] = ban
-00011fe0: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
-00011ff0: 2020 636d 645b 2276 666f 6122 5d20 3d20    cmd["vfoa"] = 
-00012000: 7666 6f0a 2020 2020 2020 2020 2020 2020  vfo.            
-00012010: 2020 2020 636d 645b 226d 6f64 6522 5d20      cmd["mode"] 
-00012020: 3d20 6d6f 6465 0a20 2020 2020 2020 2020  = mode.         
-00012030: 2020 2020 2020 2063 6d64 5b22 6277 225d         cmd["bw"]
-00012040: 203d 2062 770a 2020 2020 2020 2020 2020   = bw.          
-00012050: 2020 2020 2020 7365 6c66 2e6d 756c 7469        self.multi
-00012060: 6361 7374 5f69 6e74 6572 6661 6365 2e73  cast_interface.s
-00012070: 656e 645f 6173 5f6a 736f 6e28 636d 6429  end_as_json(cmd)
-00012080: 0a0a 2020 2020 6465 6620 6564 6974 5f63  ..    def edit_c
-00012090: 775f 6d61 6372 6f73 2873 656c 6629 202d  w_macros(self) -
-000120a0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-000120b0: 2222 220a 2020 2020 2020 2020 4361 6c6c  """.        Call
-000120c0: 7320 7468 6520 6465 6661 756c 7420 7465  s the default te
-000120d0: 7874 2065 6469 746f 7220 746f 2065 6469  xt editor to edi
-000120e0: 7420 7468 6520 4357 206d 6163 726f 2066  t the CW macro f
-000120f0: 696c 652e 0a20 2020 2020 2020 2022 2222  ile..        """
-00012100: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00012110: 2e72 6164 696f 5f73 7461 7465 2e67 6574  .radio_state.get
-00012120: 2822 6d6f 6465 2229 203d 3d20 2243 5722  ("mode") == "CW"
-00012130: 3a0a 2020 2020 2020 2020 2020 2020 6d61  :.            ma
-00012140: 6372 6f5f 6669 6c65 203d 2022 2f63 776d  cro_file = "/cwm
-00012150: 6163 726f 732e 7478 7422 0a20 2020 2020  acros.txt".     
-00012160: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00012170: 2020 2020 206d 6163 726f 5f66 696c 6520       macro_file 
-00012180: 3d20 222f 7373 626d 6163 726f 732e 7478  = "/ssbmacros.tx
-00012190: 7422 0a20 2020 2020 2020 2069 6620 6e6f  t".        if no
-000121a0: 7420 5061 7468 2844 4154 415f 5041 5448  t Path(DATA_PATH
-000121b0: 202b 206d 6163 726f 5f66 696c 6529 2e65   + macro_file).e
-000121c0: 7869 7374 7328 293a 0a20 2020 2020 2020  xists():.       
-000121d0: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-000121e0: 6728 2272 6561 645f 6377 5f6d 6163 726f  g("read_cw_macro
-000121f0: 733a 2063 6f70 7969 6e67 2064 6566 6175  s: copying defau
-00012200: 6c74 206d 6163 726f 2066 696c 652e 2229  lt macro file.")
-00012210: 0a20 2020 2020 2020 2020 2020 2063 6f70  .            cop
-00012220: 7966 696c 6528 574f 524b 494e 475f 5041  yfile(WORKING_PA
-00012230: 5448 202b 2022 2f64 6174 6122 202b 206d  TH + "/data" + m
-00012240: 6163 726f 5f66 696c 652c 2044 4154 415f  acro_file, DATA_
-00012250: 5041 5448 202b 206d 6163 726f 5f66 696c  PATH + macro_fil
-00012260: 6529 0a20 2020 2020 2020 206f 732e 7379  e).        os.sy
-00012270: 7374 656d 2866 2278 6467 2d6f 7065 6e20  stem(f"xdg-open 
-00012280: 7b44 4154 415f 5041 5448 7d7b 6d61 6372  {DATA_PATH}{macr
-00012290: 6f5f 6669 6c65 7d22 290a 0a20 2020 2064  o_file}")..    d
-000122a0: 6566 2072 6561 645f 6377 5f6d 6163 726f  ef read_cw_macro
-000122b0: 7328 7365 6c66 2920 2d3e 204e 6f6e 653a  s(self) -> None:
-000122c0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000122d0: 2020 2020 2052 6561 6473 2069 6e20 7468       Reads in th
-000122e0: 6520 4357 206d 6163 726f 732c 2066 6972  e CW macros, fir
-000122f0: 7374 7320 6974 2063 6865 636b 7320 746f  sts it checks to
-00012300: 2073 6565 2069 6620 7468 6520 6669 6c65   see if the file
-00012310: 2065 7869 7374 732e 2049 6620 6974 2064   exists. If it d
-00012320: 6f65 7320 6e6f 742c 0a20 2020 2020 2020  oes not,.       
-00012330: 2061 6e64 2074 6869 7320 6861 7320 6265   and this has be
-00012340: 656e 2070 6163 6b61 6765 6420 7769 7468  en packaged with
-00012350: 2070 7969 6e73 7461 6c6c 6572 2069 7420   pyinstaller it 
-00012360: 7769 6c6c 2063 6f70 7920 7468 6520 6465  will copy the de
-00012370: 6661 756c 7420 6669 6c65 2066 726f 6d20  fault file from 
-00012380: 7468 650a 2020 2020 2020 2020 7465 6d70  the.        temp
-00012390: 2064 6972 6563 746f 7279 2074 6869 7320   directory this 
-000123a0: 6973 2072 756e 6e69 6e67 2066 726f 6d2e  is running from.
-000123b0: 2e2e 2049 6e20 7468 656f 7279 2e0a 2020  .. In theory..  
-000123c0: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
-000123d0: 2020 2069 6620 7365 6c66 2e72 6164 696f     if self.radio
-000123e0: 5f73 7461 7465 2e67 6574 2822 6d6f 6465  _state.get("mode
-000123f0: 2229 203d 3d20 2243 5722 3a0a 2020 2020  ") == "CW":.    
-00012400: 2020 2020 2020 2020 6d61 6372 6f5f 6669          macro_fi
-00012410: 6c65 203d 2022 2f63 776d 6163 726f 732e  le = "/cwmacros.
-00012420: 7478 7422 0a20 2020 2020 2020 2065 6c73  txt".        els
-00012430: 653a 0a20 2020 2020 2020 2020 2020 206d  e:.            m
-00012440: 6163 726f 5f66 696c 6520 3d20 222f 7373  acro_file = "/ss
-00012450: 626d 6163 726f 732e 7478 7422 0a0a 2020  bmacros.txt"..  
-00012460: 2020 2020 2020 6966 206e 6f74 2050 6174        if not Pat
-00012470: 6828 4441 5441 5f50 4154 4820 2b20 6d61  h(DATA_PATH + ma
-00012480: 6372 6f5f 6669 6c65 292e 6578 6973 7473  cro_file).exists
-00012490: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-000124a0: 6c6f 6767 6572 2e64 6562 7567 2822 7265  logger.debug("re
-000124b0: 6164 5f63 775f 6d61 6372 6f73 3a20 636f  ad_cw_macros: co
-000124c0: 7079 696e 6720 6465 6661 756c 7420 6d61  pying default ma
-000124d0: 6372 6f20 6669 6c65 2e22 290a 2020 2020  cro file.").    
-000124e0: 2020 2020 2020 2020 636f 7079 6669 6c65          copyfile
-000124f0: 2857 4f52 4b49 4e47 5f50 4154 4820 2b20  (WORKING_PATH + 
-00012500: 222f 6461 7461 2220 2b20 6d61 6372 6f5f  "/data" + macro_
-00012510: 6669 6c65 2c20 4441 5441 5f50 4154 4820  file, DATA_PATH 
-00012520: 2b20 6d61 6372 6f5f 6669 6c65 290a 2020  + macro_file).  
-00012530: 2020 2020 2020 7769 7468 206f 7065 6e28        with open(
-00012540: 4441 5441 5f50 4154 4820 2b20 6d61 6372  DATA_PATH + macr
-00012550: 6f5f 6669 6c65 2c20 2272 222c 2065 6e63  o_file, "r", enc
-00012560: 6f64 696e 673d 2275 7466 2d38 2229 2061  oding="utf-8") a
-00012570: 7320 6669 6c65 5f64 6573 6372 6970 746f  s file_descripto
-00012580: 723a 0a20 2020 2020 2020 2020 2020 2066  r:.            f
-00012590: 6f72 206c 696e 6520 696e 2066 696c 655f  or line in file_
-000125a0: 6465 7363 7269 7074 6f72 3a0a 2020 2020  descriptor:.    
-000125b0: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-000125c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000125d0: 2020 2020 206d 6f64 652c 2066 6b65 792c       mode, fkey,
-000125e0: 2062 7574 746f 6e6e 616d 652c 2063 7774   buttonname, cwt
-000125f0: 6578 7420 3d20 6c69 6e65 2e73 706c 6974  ext = line.split
-00012600: 2822 7c22 290a 2020 2020 2020 2020 2020  ("|").          
-00012610: 2020 2020 2020 2020 2020 6966 206d 6f64            if mod
-00012620: 652e 7374 7269 7028 292e 7570 7065 7228  e.strip().upper(
-00012630: 2920 3d3d 2022 5222 2061 6e64 2073 656c  ) == "R" and sel
-00012640: 662e 7072 6566 2e67 6574 2822 7275 6e5f  f.pref.get("run_
-00012650: 7374 6174 6522 293a 0a20 2020 2020 2020  state"):.       
-00012660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012670: 2073 656c 662e 666b 6579 735b 666b 6579   self.fkeys[fkey
-00012680: 2e73 7472 6970 2829 5d20 3d20 2862 7574  .strip()] = (but
-00012690: 746f 6e6e 616d 652e 7374 7269 7028 292c  tonname.strip(),
-000126a0: 2063 7774 6578 742e 7374 7269 7028 2929   cwtext.strip())
-000126b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000126c0: 2020 2020 2069 6620 6d6f 6465 2e73 7472       if mode.str
-000126d0: 6970 2829 2e75 7070 6572 2829 2021 3d20  ip().upper() != 
-000126e0: 2252 2220 616e 6420 6e6f 7420 7365 6c66  "R" and not self
-000126f0: 2e70 7265 662e 6765 7428 2272 756e 5f73  .pref.get("run_s
-00012700: 7461 7465 2229 3a0a 2020 2020 2020 2020  tate"):.        
-00012710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012720: 7365 6c66 2e66 6b65 7973 5b66 6b65 792e  self.fkeys[fkey.
-00012730: 7374 7269 7028 295d 203d 2028 6275 7474  strip()] = (butt
-00012740: 6f6e 6e61 6d65 2e73 7472 6970 2829 2c20  onname.strip(), 
-00012750: 6377 7465 7874 2e73 7472 6970 2829 290a  cwtext.strip()).
-00012760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012770: 6578 6365 7074 2056 616c 7565 4572 726f  except ValueErro
-00012780: 7220 6173 2065 7272 3a0a 2020 2020 2020  r as err:.      
-00012790: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-000127a0: 6767 6572 2e69 6e66 6f28 2272 6561 645f  gger.info("read_
-000127b0: 6377 5f6d 6163 726f 733a 2025 7322 2c20  cw_macros: %s", 
-000127c0: 6572 7229 0a20 2020 2020 2020 206b 6579  err).        key
-000127d0: 7320 3d20 7365 6c66 2e66 6b65 7973 2e6b  s = self.fkeys.k
-000127e0: 6579 7328 290a 2020 2020 2020 2020 6966  eys().        if
-000127f0: 2022 4631 2220 696e 206b 6579 733a 0a20   "F1" in keys:. 
-00012800: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00012810: 4631 2e73 6574 5465 7874 2866 2246 313a  F1.setText(f"F1:
-00012820: 207b 7365 6c66 2e66 6b65 7973 5b27 4631   {self.fkeys['F1
-00012830: 275d 5b30 5d7d 2229 0a20 2020 2020 2020  '][0]}").       
-00012840: 2020 2020 2073 656c 662e 4631 2e73 6574       self.F1.set
-00012850: 546f 6f6c 5469 7028 7365 6c66 2e66 6b65  ToolTip(self.fke
-00012860: 7973 5b22 4631 225d 5b31 5d29 0a20 2020  ys["F1"][1]).   
-00012870: 2020 2020 2069 6620 2246 3222 2069 6e20       if "F2" in 
-00012880: 6b65 7973 3a0a 2020 2020 2020 2020 2020  keys:.          
-00012890: 2020 7365 6c66 2e46 322e 7365 7454 6578    self.F2.setTex
-000128a0: 7428 6622 4632 3a20 7b73 656c 662e 666b  t(f"F2: {self.fk
-000128b0: 6579 735b 2746 3227 5d5b 305d 7d22 290a  eys['F2'][0]}").
-000128c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000128d0: 2e46 322e 7365 7454 6f6f 6c54 6970 2873  .F2.setToolTip(s
-000128e0: 656c 662e 666b 6579 735b 2246 3222 5d5b  elf.fkeys["F2"][
-000128f0: 315d 290a 2020 2020 2020 2020 6966 2022  1]).        if "
-00012900: 4633 2220 696e 206b 6579 733a 0a20 2020  F3" in keys:.   
-00012910: 2020 2020 2020 2020 2073 656c 662e 4633           self.F3
-00012920: 2e73 6574 5465 7874 2866 2246 333a 207b  .setText(f"F3: {
-00012930: 7365 6c66 2e66 6b65 7973 5b27 4633 275d  self.fkeys['F3']
-00012940: 5b30 5d7d 2229 0a20 2020 2020 2020 2020  [0]}").         
-00012950: 2020 2073 656c 662e 4633 2e73 6574 546f     self.F3.setTo
-00012960: 6f6c 5469 7028 7365 6c66 2e66 6b65 7973  olTip(self.fkeys
-00012970: 5b22 4633 225d 5b31 5d29 0a20 2020 2020  ["F3"][1]).     
-00012980: 2020 2069 6620 2246 3422 2069 6e20 6b65     if "F4" in ke
-00012990: 7973 3a0a 2020 2020 2020 2020 2020 2020  ys:.            
-000129a0: 7365 6c66 2e46 342e 7365 7454 6578 7428  self.F4.setText(
-000129b0: 6622 4634 3a20 7b73 656c 662e 666b 6579  f"F4: {self.fkey
-000129c0: 735b 2746 3427 5d5b 305d 7d22 290a 2020  s['F4'][0]}").  
-000129d0: 2020 2020 2020 2020 2020 7365 6c66 2e46            self.F
-000129e0: 342e 7365 7454 6f6f 6c54 6970 2873 656c  4.setToolTip(sel
-000129f0: 662e 666b 6579 735b 2246 3422 5d5b 315d  f.fkeys["F4"][1]
-00012a00: 290a 2020 2020 2020 2020 6966 2022 4635  ).        if "F5
-00012a10: 2220 696e 206b 6579 733a 0a20 2020 2020  " in keys:.     
-00012a20: 2020 2020 2020 2073 656c 662e 4635 2e73         self.F5.s
-00012a30: 6574 5465 7874 2866 2246 353a 207b 7365  etText(f"F5: {se
-00012a40: 6c66 2e66 6b65 7973 5b27 4635 275d 5b30  lf.fkeys['F5'][0
-00012a50: 5d7d 2229 0a20 2020 2020 2020 2020 2020  ]}").           
-00012a60: 2073 656c 662e 4635 2e73 6574 546f 6f6c   self.F5.setTool
-00012a70: 5469 7028 7365 6c66 2e66 6b65 7973 5b22  Tip(self.fkeys["
-00012a80: 4635 225d 5b31 5d29 0a20 2020 2020 2020  F5"][1]).       
-00012a90: 2069 6620 2246 3622 2069 6e20 6b65 7973   if "F6" in keys
-00012aa0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00012ab0: 6c66 2e46 362e 7365 7454 6578 7428 6622  lf.F6.setText(f"
-00012ac0: 4636 3a20 7b73 656c 662e 666b 6579 735b  F6: {self.fkeys[
-00012ad0: 2746 3627 5d5b 305d 7d22 290a 2020 2020  'F6'][0]}").    
-00012ae0: 2020 2020 2020 2020 7365 6c66 2e46 362e          self.F6.
-00012af0: 7365 7454 6f6f 6c54 6970 2873 656c 662e  setToolTip(self.
-00012b00: 666b 6579 735b 2246 3622 5d5b 315d 290a  fkeys["F6"][1]).
-00012b10: 2020 2020 2020 2020 6966 2022 4637 2220          if "F7" 
-00012b20: 696e 206b 6579 733a 0a20 2020 2020 2020  in keys:.       
-00012b30: 2020 2020 2073 656c 662e 4637 2e73 6574       self.F7.set
-00012b40: 5465 7874 2866 2246 373a 207b 7365 6c66  Text(f"F7: {self
-00012b50: 2e66 6b65 7973 5b27 4637 275d 5b30 5d7d  .fkeys['F7'][0]}
-00012b60: 2229 0a20 2020 2020 2020 2020 2020 2073  ").            s
-00012b70: 656c 662e 4637 2e73 6574 546f 6f6c 5469  elf.F7.setToolTi
-00012b80: 7028 7365 6c66 2e66 6b65 7973 5b22 4637  p(self.fkeys["F7
-00012b90: 225d 5b31 5d29 0a20 2020 2020 2020 2069  "][1]).        i
-00012ba0: 6620 2246 3822 2069 6e20 6b65 7973 3a0a  f "F8" in keys:.
-00012bb0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00012bc0: 2e46 382e 7365 7454 6578 7428 6622 4638  .F8.setText(f"F8
-00012bd0: 3a20 7b73 656c 662e 666b 6579 735b 2746  : {self.fkeys['F
-00012be0: 3827 5d5b 305d 7d22 290a 2020 2020 2020  8'][0]}").      
-00012bf0: 2020 2020 2020 7365 6c66 2e46 382e 7365        self.F8.se
-00012c00: 7454 6f6f 6c54 6970 2873 656c 662e 666b  tToolTip(self.fk
-00012c10: 6579 735b 2246 3822 5d5b 315d 290a 2020  eys["F8"][1]).  
-00012c20: 2020 2020 2020 6966 2022 4639 2220 696e        if "F9" in
-00012c30: 206b 6579 733a 0a20 2020 2020 2020 2020   keys:.         
-00012c40: 2020 2073 656c 662e 4639 2e73 6574 5465     self.F9.setTe
-00012c50: 7874 2866 2246 393a 207b 7365 6c66 2e66  xt(f"F9: {self.f
-00012c60: 6b65 7973 5b27 4639 275d 5b30 5d7d 2229  keys['F9'][0]}")
-00012c70: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00012c80: 662e 4639 2e73 6574 546f 6f6c 5469 7028  f.F9.setToolTip(
-00012c90: 7365 6c66 2e66 6b65 7973 5b22 4639 225d  self.fkeys["F9"]
-00012ca0: 5b31 5d29 0a20 2020 2020 2020 2069 6620  [1]).        if 
-00012cb0: 2246 3130 2220 696e 206b 6579 733a 0a20  "F10" in keys:. 
-00012cc0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00012cd0: 4631 302e 7365 7454 6578 7428 6622 4631  F10.setText(f"F1
-00012ce0: 303a 207b 7365 6c66 2e66 6b65 7973 5b27  0: {self.fkeys['
-00012cf0: 4631 3027 5d5b 305d 7d22 290a 2020 2020  F10'][0]}").    
-00012d00: 2020 2020 2020 2020 7365 6c66 2e46 3130          self.F10
-00012d10: 2e73 6574 546f 6f6c 5469 7028 7365 6c66  .setToolTip(self
-00012d20: 2e66 6b65 7973 5b22 4631 3022 5d5b 315d  .fkeys["F10"][1]
-00012d30: 290a 2020 2020 2020 2020 6966 2022 4631  ).        if "F1
-00012d40: 3122 2069 6e20 6b65 7973 3a0a 2020 2020  1" in keys:.    
-00012d50: 2020 2020 2020 2020 7365 6c66 2e46 3131          self.F11
-00012d60: 2e73 6574 5465 7874 2866 2246 3131 3a20  .setText(f"F11: 
-00012d70: 7b73 656c 662e 666b 6579 735b 2746 3131  {self.fkeys['F11
-00012d80: 275d 5b30 5d7d 2229 0a20 2020 2020 2020  '][0]}").       
-00012d90: 2020 2020 2073 656c 662e 4631 312e 7365       self.F11.se
-00012da0: 7454 6f6f 6c54 6970 2873 656c 662e 666b  tToolTip(self.fk
-00012db0: 6579 735b 2246 3131 225d 5b31 5d29 0a20  eys["F11"][1]). 
-00012dc0: 2020 2020 2020 2069 6620 2246 3132 2220         if "F12" 
-00012dd0: 696e 206b 6579 733a 0a20 2020 2020 2020  in keys:.       
-00012de0: 2020 2020 2073 656c 662e 4631 322e 7365       self.F12.se
-00012df0: 7454 6578 7428 6622 4631 323a 207b 7365  tText(f"F12: {se
-00012e00: 6c66 2e66 6b65 7973 5b27 4631 3227 5d5b  lf.fkeys['F12'][
-00012e10: 305d 7d22 290a 2020 2020 2020 2020 2020  0]}").          
-00012e20: 2020 7365 6c66 2e46 3132 2e73 6574 546f    self.F12.setTo
-00012e30: 6f6c 5469 7028 7365 6c66 2e66 6b65 7973  olTip(self.fkeys
-00012e40: 5b22 4631 3222 5d5b 315d 290a 0a20 2020  ["F12"][1])..   
-00012e50: 2064 6566 2067 656e 6572 6174 655f 6164   def generate_ad
-00012e60: 6966 2873 656c 6629 3a0a 2020 2020 2020  if(self):.      
-00012e70: 2020 2222 2247 656e 6572 6174 6520 4144    """Generate AD
-00012e80: 4946 2222 220a 2020 2020 2020 2020 6c6f  IF""".        lo
-00012e90: 6767 6572 2e64 6562 7567 2822 2a2a 2a2a  gger.debug("****
-00012ea0: 2a2a 4144 4946 2a2a 2a2a 2a22 290a 2020  **ADIF*****").  
-00012eb0: 2020 2020 2020 7365 6c66 2e63 6f6e 7465        self.conte
-00012ec0: 7374 2e61 6469 6628 7365 6c66 290a 0a20  st.adif(self).. 
-00012ed0: 2020 2064 6566 2067 656e 6572 6174 655f     def generate_
-00012ee0: 6361 6272 696c 6c6f 2873 656c 6629 3a0a  cabrillo(self):.
-00012ef0: 2020 2020 2020 2020 2222 2247 656e 6572          """Gener
-00012f00: 6174 6573 2043 6162 7269 6c6c 6f20 6669  ates Cabrillo fi
-00012f10: 6c65 2e20 4d61 7962 652e 2222 220a 2020  le. Maybe.""".  
-00012f20: 2020 2020 2020 2320 6874 7470 733a 2f2f        # https://
-00012f30: 7777 772e 6371 7770 782e 636f 6d2f 6361  www.cqwpx.com/ca
-00012f40: 6272 696c 6c6f 2e68 746d 0a20 2020 2020  brillo.htm.     
-00012f50: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-00012f60: 222a 2a2a 2a2a 2a43 6162 7269 6c6c 6f2a  "******Cabrillo*
-00012f70: 2a2a 2a2a 2229 0a20 2020 2020 2020 2073  ****").        s
-00012f80: 656c 662e 636f 6e74 6573 742e 6361 6272  elf.contest.cabr
-00012f90: 696c 6c6f 2873 656c 6629 0a0a 0a64 6566  illo(self)...def
-00012fa0: 206c 6f61 645f 666f 6e74 735f 6672 6f6d   load_fonts_from
-00012fb0: 5f64 6972 2864 6972 6563 746f 7279 3a20  _dir(directory: 
-00012fc0: 7374 7229 202d 3e20 7365 743a 0a20 2020  str) -> set:.   
-00012fd0: 2022 2222 0a20 2020 2057 656c 6c20 6974   """.    Well it
-00012fe0: 206c 6f61 6473 2066 6f6e 7473 2066 726f   loads fonts fro
-00012ff0: 6d20 6120 6469 7265 6374 6f72 792e 2e2e  m a directory...
-00013000: 0a20 2020 2022 2222 0a20 2020 2066 6f6e  .    """.    fon
-00013010: 745f 6661 6d69 6c69 6573 203d 2073 6574  t_families = set
-00013020: 2829 0a20 2020 2066 6f72 205f 6669 2069  ().    for _fi i
-00013030: 6e20 5144 6972 2864 6972 6563 746f 7279  n QDir(directory
-00013040: 292e 656e 7472 7949 6e66 6f4c 6973 7428  ).entryInfoList(
-00013050: 5b22 2a2e 7474 6622 2c20 222a 2e77 6f66  ["*.ttf", "*.wof
-00013060: 6622 2c20 222a 2e77 6f66 6632 225d 293a  f", "*.woff2"]):
-00013070: 0a20 2020 2020 2020 205f 6964 203d 2051  .        _id = Q
-00013080: 466f 6e74 4461 7461 6261 7365 2e61 6464  FontDatabase.add
-00013090: 4170 706c 6963 6174 696f 6e46 6f6e 7428  ApplicationFont(
-000130a0: 5f66 692e 6162 736f 6c75 7465 4669 6c65  _fi.absoluteFile
-000130b0: 5061 7468 2829 290a 2020 2020 2020 2020  Path()).        
-000130c0: 666f 6e74 5f66 616d 696c 6965 7320 7c3d  font_families |=
-000130d0: 2073 6574 2851 466f 6e74 4461 7461 6261   set(QFontDataba
-000130e0: 7365 2e61 7070 6c69 6361 7469 6f6e 466f  se.applicationFo
-000130f0: 6e74 4661 6d69 6c69 6573 285f 6964 2929  ntFamilies(_id))
-00013100: 0a20 2020 2072 6574 7572 6e20 666f 6e74  .    return font
-00013110: 5f66 616d 696c 6965 730a 0a0a 6465 6620  _families...def 
-00013120: 696e 7374 616c 6c5f 6963 6f6e 7328 293a  install_icons():
-00013130: 0a20 2020 2022 2222 496e 7374 616c 6c20  .    """Install 
-00013140: 6963 6f6e 7322 2222 0a20 2020 206f 732e  icons""".    os.
-00013150: 7379 7374 656d 280a 2020 2020 2020 2020  system(.        
-00013160: 2278 6467 2d69 636f 6e2d 7265 736f 7572  "xdg-icon-resour
-00013170: 6365 2069 6e73 7461 6c6c 202d 2d73 697a  ce install --siz
-00013180: 6520 3332 202d 2d63 6f6e 7465 7874 2061  e 32 --context a
-00013190: 7070 7320 2d2d 6d6f 6465 2075 7365 7220  pps --mode user 
-000131a0: 220a 2020 2020 2020 2020 6622 7b57 4f52  ".        f"{WOR
-000131b0: 4b49 4e47 5f50 4154 487d 2f64 6174 612f  KING_PATH}/data/
-000131c0: 6b36 6774 652e 6e6f 7431 6d6d 2d33 322e  k6gte.not1mm-32.
-000131d0: 706e 6720 6b36 6774 652d 6e6f 7431 6d6d  png k6gte-not1mm
-000131e0: 220a 2020 2020 290a 2020 2020 6f73 2e73  ".    ).    os.s
-000131f0: 7973 7465 6d28 0a20 2020 2020 2020 2022  ystem(.        "
-00013200: 7864 672d 6963 6f6e 2d72 6573 6f75 7263  xdg-icon-resourc
-00013210: 6520 696e 7374 616c 6c20 2d2d 7369 7a65  e install --size
-00013220: 2036 3420 2d2d 636f 6e74 6578 7420 6170   64 --context ap
-00013230: 7073 202d 2d6d 6f64 6520 7573 6572 2022  ps --mode user "
-00013240: 0a20 2020 2020 2020 2066 227b 574f 524b  .        f"{WORK
-00013250: 494e 475f 5041 5448 7d2f 6461 7461 2f6b  ING_PATH}/data/k
-00013260: 3667 7465 2e6e 6f74 316d 6d2d 3634 2e70  6gte.not1mm-64.p
-00013270: 6e67 206b 3667 7465 2d6e 6f74 316d 6d22  ng k6gte-not1mm"
-00013280: 0a20 2020 2029 0a20 2020 206f 732e 7379  .    ).    os.sy
-00013290: 7374 656d 280a 2020 2020 2020 2020 2278  stem(.        "x
-000132a0: 6467 2d69 636f 6e2d 7265 736f 7572 6365  dg-icon-resource
-000132b0: 2069 6e73 7461 6c6c 202d 2d73 697a 6520   install --size 
-000132c0: 3132 3820 2d2d 636f 6e74 6578 7420 6170  128 --context ap
-000132d0: 7073 202d 2d6d 6f64 6520 7573 6572 2022  ps --mode user "
-000132e0: 0a20 2020 2020 2020 2066 227b 574f 524b  .        f"{WORK
-000132f0: 494e 475f 5041 5448 7d2f 6461 7461 2f6b  ING_PATH}/data/k
-00013300: 3667 7465 2e6e 6f74 316d 6d2d 3132 382e  6gte.not1mm-128.
-00013310: 706e 6720 6b36 6774 652d 6e6f 7431 6d6d  png k6gte-not1mm
-00013320: 220a 2020 2020 290a 2020 2020 6f73 2e73  ".    ).    os.s
-00013330: 7973 7465 6d28 6622 7864 672d 6465 736b  ystem(f"xdg-desk
-00013340: 746f 702d 6d65 6e75 2069 6e73 7461 6c6c  top-menu install
-00013350: 207b 574f 524b 494e 475f 5041 5448 7d2f   {WORKING_PATH}/
-00013360: 6461 7461 2f6b 3667 7465 2d6e 6f74 316d  data/k6gte-not1m
-00013370: 6d2e 6465 736b 746f 7022 290a 0a0a 6465  m.desktop")...de
-00013380: 6620 646f 696d 7028 6d6f 646e 616d 6529  f doimp(modname)
-00013390: 3a0a 2020 2020 2222 2272 6574 7572 6e20  :.    """return 
-000133a0: 6d6f 6475 6c65 2070 6174 6822 2222 0a20  module path""". 
-000133b0: 2020 2072 6574 7572 6e20 696d 706f 7274     return import
-000133c0: 6c69 622e 696d 706f 7274 5f6d 6f64 756c  lib.import_modul
-000133d0: 6528 6622 6e6f 7431 6d6d 2e70 6c75 6769  e(f"not1mm.plugi
-000133e0: 6e73 2e7b 6d6f 646e 616d 657d 2229 0a0a  ns.{modname}")..
-000133f0: 0a64 6566 2072 756e 2829 3a0a 2020 2020  .def run():.    
-00013400: 2222 220a 2020 2020 4d61 696e 2045 6e74  """.    Main Ent
-00013410: 7279 0a20 2020 2022 2222 0a0a 2020 2020  ry.    """..    
-00013420: 696e 7374 616c 6c5f 6963 6f6e 7328 290a  install_icons().
-00013430: 2020 2020 7469 6d65 722e 7374 6172 7428      timer.start(
-00013440: 3130 3029 0a20 2020 2074 696d 6572 322e  100).    timer2.
-00013450: 7374 6172 7428 3235 3029 0a0a 2020 2020  start(250)..    
-00013460: 7379 732e 6578 6974 2861 7070 2e65 7865  sys.exit(app.exe
-00013470: 6328 2929 0a0a 0a6c 6f67 6765 7220 3d20  c())...logger = 
-00013480: 6c6f 6767 696e 672e 6765 744c 6f67 6765  logging.getLogge
-00013490: 7228 225f 5f6d 6169 6e5f 5f22 290a 6861  r("__main__").ha
-000134a0: 6e64 6c65 7220 3d20 6c6f 6767 696e 672e  ndler = logging.
-000134b0: 5374 7265 616d 4861 6e64 6c65 7228 290a  StreamHandler().
-000134c0: 666f 726d 6174 7465 7220 3d20 6c6f 6767  formatter = logg
-000134d0: 696e 672e 466f 726d 6174 7465 7228 0a20  ing.Formatter(. 
-000134e0: 2020 2064 6174 6566 6d74 3d22 2548 3a25     datefmt="%H:%
-000134f0: 4d3a 2553 222c 0a20 2020 2066 6d74 3d22  M:%S",.    fmt="
-00013500: 5b25 2861 7363 7469 6d65 2973 5d20 2528  [%(asctime)s] %(
-00013510: 6c65 7665 6c6e 616d 6529 7320 2528 6d6f  levelname)s %(mo
-00013520: 6475 6c65 2973 202d 2025 2866 756e 634e  dule)s - %(funcN
-00013530: 616d 6529 7320 4c69 6e65 2025 286c 696e  ame)s Line %(lin
-00013540: 656e 6f29 643a 2025 286d 6573 7361 6765  eno)d: %(message
-00013550: 2973 222c 0a29 0a68 616e 646c 6572 2e73  )s",.).handler.s
-00013560: 6574 466f 726d 6174 7465 7228 666f 726d  etFormatter(form
-00013570: 6174 7465 7229 0a6c 6f67 6765 722e 6164  atter).logger.ad
-00013580: 6448 616e 646c 6572 2868 616e 646c 6572  dHandler(handler
-00013590: 290a 0a69 6620 5061 7468 2822 2e2f 6465  )..if Path("./de
-000135a0: 6275 6722 292e 6578 6973 7473 2829 3a0a  bug").exists():.
-000135b0: 2020 2020 6c6f 6767 6572 2e73 6574 4c65      logger.setLe
-000135c0: 7665 6c28 6c6f 6767 696e 672e 4445 4255  vel(logging.DEBU
-000135d0: 4729 0a20 2020 206c 6f67 6765 722e 6465  G).    logger.de
-000135e0: 6275 6728 2264 6562 7567 6769 6e67 206f  bug("debugging o
-000135f0: 6e22 290a 656c 7365 3a0a 2020 2020 6c6f  n").else:.    lo
-00013600: 6767 6572 2e73 6574 4c65 7665 6c28 6c6f  gger.setLevel(lo
-00013610: 6767 696e 672e 5741 524e 494e 4729 0a20  gging.WARNING). 
-00013620: 2020 206c 6f67 6765 722e 7761 726e 696e     logger.warnin
-00013630: 6728 2264 6562 7567 6769 6e67 206f 6666  g("debugging off
-00013640: 2229 0a0a 6170 7020 3d20 5174 5769 6467  ")..app = QtWidg
-00013650: 6574 732e 5141 7070 6c69 6361 7469 6f6e  ets.QApplication
-00013660: 2873 7973 2e61 7267 7629 0a23 2061 7070  (sys.argv).# app
-00013670: 2e73 6574 5374 796c 6528 2246 7573 696f  .setStyle("Fusio
-00013680: 6e22 290a 666f 6e74 5f70 6174 6820 3d20  n").font_path = 
-00013690: 574f 524b 494e 475f 5041 5448 202b 2022  WORKING_PATH + "
-000136a0: 2f64 6174 6122 0a66 616d 696c 6965 7320  /data".families 
-000136b0: 3d20 6c6f 6164 5f66 6f6e 7473 5f66 726f  = load_fonts_fro
-000136c0: 6d5f 6469 7228 6f73 2e66 7370 6174 6828  m_dir(os.fspath(
-000136d0: 666f 6e74 5f70 6174 6829 290a 6c6f 6767  font_path)).logg
-000136e0: 6572 2e69 6e66 6f28 6661 6d69 6c69 6573  er.info(families
-000136f0: 290a 7769 6e64 6f77 203d 204d 6169 6e57  ).window = MainW
-00013700: 696e 646f 7728 290a 6865 6967 6874 203d  indow().height =
-00013710: 2077 696e 646f 772e 7072 6566 2e67 6574   window.pref.get
-00013720: 2822 7769 6e64 6f77 5f68 6569 6768 7422  ("window_height"
-00013730: 2c20 3330 3029 0a77 6964 7468 203d 2077  , 300).width = w
-00013740: 696e 646f 772e 7072 6566 2e67 6574 2822  indow.pref.get("
-00013750: 7769 6e64 6f77 5f77 6964 7468 222c 2037  window_width", 7
-00013760: 3030 290a 7820 3d20 7769 6e64 6f77 2e70  00).x = window.p
-00013770: 7265 662e 6765 7428 2277 696e 646f 775f  ref.get("window_
-00013780: 7822 2c20 2d31 290a 7920 3d20 7769 6e64  x", -1).y = wind
-00013790: 6f77 2e70 7265 662e 6765 7428 2277 696e  ow.pref.get("win
-000137a0: 646f 775f 7922 2c20 2d31 290a 7769 6e64  dow_y", -1).wind
-000137b0: 6f77 2e73 6574 4765 6f6d 6574 7279 2878  ow.setGeometry(x
-000137c0: 2c20 792c 2077 6964 7468 2c20 6865 6967  , y, width, heig
-000137d0: 6874 290a 2320 7769 6e64 6f77 2e73 6574  ht).# window.set
-000137e0: 5769 6e64 6f77 5469 746c 6528 6622 4e6f  WindowTitle(f"No
-000137f0: 7431 4d4d 2076 7b5f 5f76 6572 7369 6f6e  t1MM v{__version
-00013800: 5f5f 7d22 290a 7769 6e64 6f77 2e63 616c  __}").window.cal
-00013810: 6c73 6967 6e2e 7365 7446 6f63 7573 2829  lsign.setFocus()
-00013820: 0a77 696e 646f 772e 7368 6f77 2829 0a74  .window.show().t
-00013830: 696d 6572 203d 2051 7443 6f72 652e 5154  imer = QtCore.QT
-00013840: 696d 6572 2829 0a74 696d 6572 2e74 696d  imer().timer.tim
-00013850: 656f 7574 2e63 6f6e 6e65 6374 2877 696e  eout.connect(win
-00013860: 646f 772e 706f 6c6c 5f72 6164 696f 290a  dow.poll_radio).
-00013870: 7469 6d65 7232 203d 2051 7443 6f72 652e  timer2 = QtCore.
-00013880: 5154 696d 6572 2829 0a74 696d 6572 322e  QTimer().timer2.
-00013890: 7469 6d65 6f75 742e 636f 6e6e 6563 7428  timeout.connect(
-000138a0: 7769 6e64 6f77 2e63 6865 636b 5f75 6470  window.check_udp
-000138b0: 5f74 7261 6666 6963 290a 0a69 6620 5f5f  _traffic)..if __
-000138c0: 6e61 6d65 5f5f 203d 3d20 225f 5f6d 6169  name__ == "__mai
-000138d0: 6e5f 5f22 3a0a 2020 2020 7275 6e28 290a  n__":.    run().
+00010be0: 2020 2020 7365 6c66 2e6d 756c 7469 6361      self.multica
+00010bf0: 7374 5f69 6e74 6572 6661 6365 2e73 656e  st_interface.sen
+00010c00: 645f 6173 5f6a 736f 6e28 636d 6429 0a20  d_as_json(cmd). 
+00010c10: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00010c20: 6620 280a 2020 2020 2020 2020 2020 2020  f (.            
+00010c30: 2020 2020 2020 2020 6a73 6f6e 5f64 6174          json_dat
+00010c40: 612e 6765 7428 2263 6d64 222c 2022 2229  a.get("cmd", "")
+00010c50: 203d 3d20 2254 554e 4522 0a20 2020 2020   == "TUNE".     
+00010c60: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00010c70: 6e64 206a 736f 6e5f 6461 7461 2e67 6574  nd json_data.get
+00010c80: 2822 7374 6174 696f 6e22 2c20 2222 2920  ("station", "") 
+00010c90: 3d3d 2070 6c61 7466 6f72 6d2e 6e6f 6465  == platform.node
+00010ca0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00010cb0: 2020 2029 3a0a 2020 2020 2020 2020 2020     ):.          
+00010cc0: 2020 2020 2020 2020 2020 2320 6227 7b22            # b'{"
+00010cd0: 636d 6422 3a20 2254 554e 4522 2c20 2266  cmd": "TUNE", "f
+00010ce0: 7265 7122 3a20 372e 3032 3335 2c20 2273  req": 7.0235, "s
+00010cf0: 706f 7422 3a20 224d 4d30 4447 4922 7d27  pot": "MM0DGI"}'
+00010d00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010d10: 2020 2020 2076 666f 203d 206a 736f 6e5f       vfo = json_
+00010d20: 6461 7461 2e67 6574 2822 6672 6571 2229  data.get("freq")
+00010d30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010d40: 2020 2020 2076 666f 203d 2066 6c6f 6174       vfo = float
+00010d50: 2876 666f 2920 2a20 3130 3030 3030 300a  (vfo) * 1000000.
+00010d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d70: 2020 2020 7365 6c66 2e72 6164 696f 5f73      self.radio_s
+00010d80: 7461 7465 5b22 7666 6f61 225d 203d 2069  tate["vfoa"] = i
+00010d90: 6e74 2876 666f 290a 2020 2020 2020 2020  nt(vfo).        
+00010da0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00010db0: 656c 662e 7269 675f 636f 6e74 726f 6c3a  elf.rig_control:
+00010dc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010dd0: 2020 2020 2020 2020 2073 656c 662e 7269           self.ri
+00010de0: 675f 636f 6e74 726f 6c2e 7365 745f 7666  g_control.set_vf
+00010df0: 6f28 696e 7428 7666 6f29 290a 2020 2020  o(int(vfo)).    
+00010e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e10: 7370 6f74 203d 206a 736f 6e5f 6461 7461  spot = json_data
+00010e20: 2e67 6574 2822 7370 6f74 222c 2022 2229  .get("spot", "")
+00010e30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010e40: 2020 2020 2073 656c 662e 6361 6c6c 7369       self.callsi
+00010e50: 676e 2e73 6574 5465 7874 2873 706f 7429  gn.setText(spot)
+00010e60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010e70: 2020 2020 2073 656c 662e 6361 6c6c 7369       self.callsi
+00010e80: 676e 5f63 6861 6e67 6564 2829 0a20 2020  gn_changed().   
+00010e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ea0: 2073 656c 662e 6361 6c6c 7369 676e 2e73   self.callsign.s
+00010eb0: 6574 466f 6375 7328 290a 2020 2020 2020  etFocus().      
+00010ec0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00010ed0: 6c66 2e63 616c 6c73 6967 6e2e 6163 7469  lf.callsign.acti
+00010ee0: 7661 7465 5769 6e64 6f77 2829 0a20 2020  vateWindow().   
+00010ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f00: 2077 696e 646f 772e 7261 6973 655f 2829   window.raise_()
+00010f10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010f20: 2020 2020 2023 2066 6720 3d20 7769 6e64       # fg = wind
+00010f30: 6f77 2e66 7261 6d65 4765 6f6d 6574 7279  ow.frameGeometry
+00010f40: 2829 2e74 6f70 4c65 6674 0a20 2020 2020  ().topLeft.     
+00010f50: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00010f60: 2023 205f 7769 6474 6820 3d20 7365 6c66   # _width = self
+00010f70: 2e73 697a 6528 292e 7769 6474 6828 290a  .size().width().
+00010f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f90: 2020 2020 2320 2320 5f68 6569 6768 7420      # # _height 
+00010fa0: 3d20 7365 6c66 2e73 697a 6528 292e 6865  = self.size().he
+00010fb0: 6967 6874 2829 0a20 2020 2020 2020 2020  ight().         
+00010fc0: 2020 2020 2020 2020 2020 2023 2023 205f             # # _
+00010fd0: 7820 3d20 7365 6c66 2e70 6f73 2829 2e78  x = self.pos().x
+00010fe0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00010ff0: 2020 2020 2020 2023 2023 205f 7920 3d20         # # _y = 
+00011000: 7365 6c66 2e70 6f73 2829 2e79 2829 0a20  self.pos().y(). 
+00011010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011020: 2020 2023 2023 2070 7269 6e74 2866 222a     # # print(f"*
+00011030: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00011040: 2a2a 2a2a 2a2a 2a2a 2a2a 2a20 7820 7b5f  *********** x {_
+00011050: 787d 2079 207b 5f79 7d22 290a 2020 2020  x} y {_y}").    
+00011060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011070: 2320 2320 7769 6e64 6f77 2e68 6964 6528  # # window.hide(
+00011080: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00011090: 2020 2020 2020 2320 2320 7769 6e64 6f77        # # window
+000110a0: 2e73 686f 7728 290a 2020 2020 2020 2020  .show().        
+000110b0: 2020 2020 2020 2020 2020 2020 2320 2320              # # 
+000110c0: 7769 6e64 6f77 2e73 6574 4765 6f6d 6574  window.setGeomet
+000110d0: 7279 2830 2c20 302c 205f 7769 6474 682c  ry(0, 0, _width,
+000110e0: 205f 6865 6967 6874 290a 2020 2020 2020   _height).      
+000110f0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00011100: 7769 6e64 6f77 2e73 686f 7728 290a 2020  window.show().  
+00011110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011120: 2020 2320 7769 6e64 6f77 2e67 656f 6d65    # window.geome
+00011130: 7472 7928 292e 7365 7458 2831 3030 290a  try().setX(100).
+00011140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011150: 2020 2020 2320 7769 6e64 6f77 2e67 656f      # window.geo
+00011160: 6d65 7472 7928 292e 7365 7459 2831 3030  metry().setY(100
+00011170: 290a 0a20 2020 2064 6566 2063 775f 6d61  )..    def cw_ma
+00011180: 6372 6f73 5f73 7461 7465 5f63 6861 6e67  cros_state_chang
+00011190: 6564 2873 656c 6629 3a0a 2020 2020 2020  ed(self):.      
+000111a0: 2020 2222 224d 656e 7520 6974 656d 2074    """Menu item t
+000111b0: 6f20 7368 6f77 2f68 6964 6520 6d61 6372  o show/hide macr
+000111c0: 6f20 6275 7474 6f6e 7322 2222 0a20 2020  o buttons""".   
+000111d0: 2020 2020 2073 656c 662e 7072 6566 5b22       self.pref["
+000111e0: 6377 5f6d 6163 726f 7322 5d20 3d20 7365  cw_macros"] = se
+000111f0: 6c66 2e61 6374 696f 6e43 575f 4d61 6372  lf.actionCW_Macr
+00011200: 6f73 2e69 7343 6865 636b 6564 2829 0a20  os.isChecked(). 
+00011210: 2020 2020 2020 2073 656c 662e 7772 6974         self.writ
+00011220: 655f 7072 6566 6572 656e 6365 2829 0a20  e_preference(). 
+00011230: 2020 2020 2020 2073 656c 662e 7368 6f77         self.show
+00011240: 5f43 575f 6d61 6372 6f73 2829 0a0a 2020  _CW_macros()..  
+00011250: 2020 6465 6620 7368 6f77 5f43 575f 6d61    def show_CW_ma
+00011260: 6372 6f73 2873 656c 6629 3a0a 2020 2020  cros(self):.    
+00011270: 2020 2020 2222 226d 6163 726f 2062 7574      """macro but
+00011280: 746f 6e20 7374 6174 6520 6368 616e 6765  ton state change
+00011290: 2222 220a 2020 2020 2020 2020 6966 2073  """.        if s
+000112a0: 656c 662e 7072 6566 2e67 6574 2822 6377  elf.pref.get("cw
+000112b0: 5f6d 6163 726f 7322 293a 0a20 2020 2020  _macros"):.     
+000112c0: 2020 2020 2020 2073 656c 662e 4275 7474         self.Butt
+000112d0: 6f6e 5f52 6f77 312e 7368 6f77 2829 0a20  on_Row1.show(). 
+000112e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000112f0: 4275 7474 6f6e 5f52 6f77 322e 7368 6f77  Button_Row2.show
+00011300: 2829 0a20 2020 2020 2020 2065 6c73 653a  ().        else:
+00011310: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00011320: 662e 4275 7474 6f6e 5f52 6f77 312e 6869  f.Button_Row1.hi
+00011330: 6465 2829 0a20 2020 2020 2020 2020 2020  de().           
+00011340: 2073 656c 662e 4275 7474 6f6e 5f52 6f77   self.Button_Row
+00011350: 322e 6869 6465 2829 0a0a 2020 2020 6465  2.hide()..    de
+00011360: 6620 636f 6d6d 616e 645f 6275 7474 6f6e  f command_button
+00011370: 735f 7374 6174 655f 6368 616e 6765 2873  s_state_change(s
+00011380: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+00011390: 224d 656e 7520 6974 656d 2074 6f20 7368  "Menu item to sh
+000113a0: 6f77 2f68 6964 6520 636f 6d6d 616e 6420  ow/hide command 
+000113b0: 6275 7474 6f6e 7322 2222 0a20 2020 2020  buttons""".     
+000113c0: 2020 2073 656c 662e 7072 6566 5b22 636f     self.pref["co
+000113d0: 6d6d 616e 645f 6275 7474 6f6e 7322 5d20  mmand_buttons"] 
+000113e0: 3d20 7365 6c66 2e61 6374 696f 6e43 6f6d  = self.actionCom
+000113f0: 6d61 6e64 5f42 7574 746f 6e73 2e69 7343  mand_Buttons.isC
+00011400: 6865 636b 6564 2829 0a20 2020 2020 2020  hecked().       
+00011410: 2073 656c 662e 7772 6974 655f 7072 6566   self.write_pref
+00011420: 6572 656e 6365 2829 0a20 2020 2020 2020  erence().       
+00011430: 2073 656c 662e 7368 6f77 5f63 6f6d 6d61   self.show_comma
+00011440: 6e64 5f62 7574 746f 6e73 2829 0a0a 2020  nd_buttons()..  
+00011450: 2020 6465 6620 7368 6f77 5f63 6f6d 6d61    def show_comma
+00011460: 6e64 5f62 7574 746f 6e73 2873 656c 6629  nd_buttons(self)
+00011470: 3a0a 2020 2020 2020 2020 2222 2263 6f6d  :.        """com
+00011480: 6d61 6e64 2062 7574 746f 6e20 7374 6174  mand button stat
+00011490: 6520 6368 616e 6765 2222 220a 2020 2020  e change""".    
+000114a0: 2020 2020 6966 2073 656c 662e 7072 6566      if self.pref
+000114b0: 2e67 6574 2822 636f 6d6d 616e 645f 6275  .get("command_bu
+000114c0: 7474 6f6e 7322 293a 0a20 2020 2020 2020  ttons"):.       
+000114d0: 2020 2020 2073 656c 662e 436f 6d6d 616e       self.Comman
+000114e0: 645f 4275 7474 6f6e 732e 7368 6f77 2829  d_Buttons.show()
+000114f0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00011500: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00011510: 436f 6d6d 616e 645f 4275 7474 6f6e 732e  Command_Buttons.
+00011520: 6869 6465 2829 0a0a 2020 2020 6465 6620  hide()..    def 
+00011530: 6973 5f66 6c6f 6174 6162 6c65 2873 656c  is_floatable(sel
+00011540: 662c 2069 7465 6d3a 2073 7472 2920 2d3e  f, item: str) ->
+00011550: 2062 6f6f 6c3a 0a20 2020 2020 2020 2022   bool:.        "
+00011560: 2222 6368 6563 6b20 746f 2073 6565 2069  ""check to see i
+00011570: 6620 7374 7269 6e67 2063 616e 2062 6520  f string can be 
+00011580: 6120 666c 6f61 7422 2222 0a20 2020 2020  a float""".     
+00011590: 2020 2069 6620 6974 656d 2e69 736e 756d     if item.isnum
+000115a0: 6572 6963 2829 3a0a 2020 2020 2020 2020  eric():.        
+000115b0: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
+000115c0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+000115d0: 2020 2020 2020 2020 205f 7465 7374 203d           _test =
+000115e0: 2066 6c6f 6174 2869 7465 6d29 0a20 2020   float(item).   
+000115f0: 2020 2020 2065 7863 6570 7420 5661 6c75       except Valu
+00011600: 6545 7272 6f72 3a0a 2020 2020 2020 2020  eError:.        
+00011610: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+00011620: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00011630: 5472 7565 0a0a 2020 2020 6465 6620 6f74  True..    def ot
+00011640: 6865 725f 325f 6368 616e 6765 6428 7365  her_2_changed(se
+00011650: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+00011660: 4361 6c6c 6564 2077 6865 6e20 7765 206e  Called when we n
+00011670: 6565 6420 746f 2070 6172 7365 2053 5320  eed to parse SS 
+00011680: 6578 6368 616e 6765 2e22 2222 0a20 2020  exchange.""".   
+00011690: 2020 2020 2069 6620 7365 6c66 2e63 6f6e       if self.con
+000116a0: 7465 7374 3a0a 2020 2020 2020 2020 2020  test:.          
+000116b0: 2020 6966 2022 4152 524c 2053 7765 6570    if "ARRL Sweep
+000116c0: 7374 616b 6573 2220 696e 2073 656c 662e  stakes" in self.
+000116d0: 636f 6e74 6573 742e 6e61 6d65 3a0a 2020  contest.name:.  
+000116e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000116f0: 6c66 2e63 6f6e 7465 7374 2e70 6172 7365  lf.contest.parse
+00011700: 5f65 7863 6861 6e67 6528 7365 6c66 290a  _exchange(self).
+00011710: 0a20 2020 2064 6566 2063 616c 6c73 6967  .    def callsig
+00011720: 6e5f 6368 616e 6765 6428 7365 6c66 293a  n_changed(self):
+00011730: 0a20 2020 2020 2020 2022 2222 4361 6c6c  .        """Call
+00011740: 6564 2077 6865 6e20 7465 7874 2069 6e20  ed when text in 
+00011750: 7468 6520 6361 6c6c 7369 676e 2066 6965  the callsign fie
+00011760: 6c64 2068 6173 2063 6861 6e67 6564 2222  ld has changed""
+00011770: 220a 2020 2020 2020 2020 7465 7874 203d  ".        text =
+00011780: 2073 656c 662e 6361 6c6c 7369 676e 2e74   self.callsign.t
+00011790: 6578 7428 290a 2020 2020 2020 2020 7465  ext().        te
+000117a0: 7874 203d 2074 6578 742e 7570 7065 7228  xt = text.upper(
+000117b0: 290a 2020 2020 2020 2020 706f 7369 7469  ).        positi
+000117c0: 6f6e 203d 2073 656c 662e 6361 6c6c 7369  on = self.callsi
+000117d0: 676e 2e63 7572 736f 7250 6f73 6974 696f  gn.cursorPositio
+000117e0: 6e28 290a 2020 2020 2020 2020 7374 7269  n().        stri
+000117f0: 7070 6564 5f74 6578 7420 3d20 7465 7874  pped_text = text
+00011800: 2e73 7472 6970 2829 2e72 6570 6c61 6365  .strip().replace
+00011810: 2822 2022 2c20 2222 290a 2020 2020 2020  (" ", "").      
+00011820: 2020 7365 6c66 2e63 616c 6c73 6967 6e2e    self.callsign.
+00011830: 7365 7454 6578 7428 7374 7269 7070 6564  setText(stripped
+00011840: 5f74 6578 7429 0a20 2020 2020 2020 2073  _text).        s
+00011850: 656c 662e 6361 6c6c 7369 676e 2e73 6574  elf.callsign.set
+00011860: 4375 7273 6f72 506f 7369 7469 6f6e 2870  CursorPosition(p
+00011870: 6f73 6974 696f 6e29 0a0a 2020 2020 2020  osition)..      
+00011880: 2020 6966 2022 2022 2069 6e20 7465 7874    if " " in text
+00011890: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+000118a0: 2073 7472 6970 7065 645f 7465 7874 203d   stripped_text =
+000118b0: 3d20 2243 5722 3a0a 2020 2020 2020 2020  = "CW":.        
+000118c0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+000118d0: 6d6f 6465 2822 4357 2229 0a20 2020 2020  mode("CW").     
+000118e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000118f0: 7261 6469 6f5f 7374 6174 655b 226d 6f64  radio_state["mod
+00011900: 6522 5d20 3d20 2243 5722 0a20 2020 2020  e"] = "CW".     
+00011910: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00011920: 6c66 2e72 6967 5f63 6f6e 7472 6f6c 3a0a  lf.rig_control:.
+00011930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011940: 2020 2020 6966 2073 656c 662e 7269 675f      if self.rig_
+00011950: 636f 6e74 726f 6c2e 6f6e 6c69 6e65 3a0a  control.online:.
+00011960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011970: 2020 2020 2020 2020 7365 6c66 2e72 6967          self.rig
+00011980: 5f63 6f6e 7472 6f6c 2e73 6574 5f6d 6f64  _control.set_mod
+00011990: 6528 2243 5722 290a 2020 2020 2020 2020  e("CW").        
+000119a0: 2020 2020 2020 2020 6261 6e64 203d 2067          band = g
+000119b0: 6574 6261 6e64 2873 7472 2873 656c 662e  etband(str(self.
+000119c0: 7261 6469 6f5f 7374 6174 652e 6765 7428  radio_state.get(
+000119d0: 2276 666f 6122 2c20 2230 2e30 2229 2929  "vfoa", "0.0")))
+000119e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000119f0: 2073 656c 662e 7365 745f 6261 6e64 5f69   self.set_band_i
+00011a00: 6e64 6963 6174 6f72 2862 616e 6429 0a20  ndicator(band). 
+00011a10: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00011a20: 656c 662e 7365 745f 7769 6e64 6f77 5f74  elf.set_window_t
+00011a30: 6974 6c65 2829 0a20 2020 2020 2020 2020  itle().         
+00011a40: 2020 2020 2020 2073 656c 662e 636c 6561         self.clea
+00011a50: 7269 6e70 7574 7328 290a 2020 2020 2020  rinputs().      
+00011a60: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+00011a70: 6561 645f 6377 5f6d 6163 726f 7328 290a  ead_cw_macros().
+00011a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a90: 7265 7475 726e 0a20 2020 2020 2020 2020  return.         
+00011aa0: 2020 2069 6620 7374 7269 7070 6564 5f74     if stripped_t
+00011ab0: 6578 7420 3d3d 2022 5254 5459 223a 0a20  ext == "RTTY":. 
+00011ac0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00011ad0: 656c 662e 7365 746d 6f64 6528 2252 5454  elf.setmode("RTT
+00011ae0: 5922 290a 2020 2020 2020 2020 2020 2020  Y").            
+00011af0: 2020 2020 6966 2073 656c 662e 7269 675f      if self.rig_
+00011b00: 636f 6e74 726f 6c3a 0a20 2020 2020 2020  control:.       
+00011b10: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00011b20: 7365 6c66 2e72 6967 5f63 6f6e 7472 6f6c  self.rig_control
+00011b30: 2e6f 6e6c 696e 653a 0a20 2020 2020 2020  .online:.       
+00011b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b50: 2073 656c 662e 7269 675f 636f 6e74 726f   self.rig_contro
+00011b60: 6c2e 7365 745f 6d6f 6465 2822 5254 5459  l.set_mode("RTTY
+00011b70: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+00011b80: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00011b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ba0: 2020 2020 2073 656c 662e 7261 6469 6f5f       self.radio_
+00011bb0: 7374 6174 655b 226d 6f64 6522 5d20 3d20  state["mode"] = 
+00011bc0: 2252 5454 5922 0a20 2020 2020 2020 2020  "RTTY".         
+00011bd0: 2020 2020 2020 2062 616e 6420 3d20 6765         band = ge
+00011be0: 7462 616e 6428 7374 7228 7365 6c66 2e72  tband(str(self.r
+00011bf0: 6164 696f 5f73 7461 7465 2e67 6574 2822  adio_state.get("
+00011c00: 7666 6f61 222c 2022 302e 3022 2929 290a  vfoa", "0.0"))).
+00011c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c20: 7365 6c66 2e73 6574 5f62 616e 645f 696e  self.set_band_in
+00011c30: 6469 6361 746f 7228 6261 6e64 290a 2020  dicator(band).  
+00011c40: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00011c50: 6c66 2e73 6574 5f77 696e 646f 775f 7469  lf.set_window_ti
+00011c60: 746c 6528 290a 2020 2020 2020 2020 2020  tle().          
+00011c70: 2020 2020 2020 7365 6c66 2e63 6c65 6172        self.clear
+00011c80: 696e 7075 7473 2829 0a20 2020 2020 2020  inputs().       
+00011c90: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+00011ca0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00011cb0: 7472 6970 7065 645f 7465 7874 203d 3d20  tripped_text == 
+00011cc0: 2253 5342 223a 0a20 2020 2020 2020 2020  "SSB":.         
+00011cd0: 2020 2020 2020 2073 656c 662e 7365 746d         self.setm
+00011ce0: 6f64 6528 2253 5342 2229 0a20 2020 2020  ode("SSB").     
+00011cf0: 2020 2020 2020 2020 2020 2069 6620 696e             if in
+00011d00: 7428 7365 6c66 2e72 6164 696f 5f73 7461  t(self.radio_sta
+00011d10: 7465 2e67 6574 2822 7666 6f61 222c 2030  te.get("vfoa", 0
+00011d20: 2929 203e 2031 3030 3030 3030 303a 0a20  )) > 10000000:. 
+00011d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d40: 2020 2073 656c 662e 7261 6469 6f5f 7374     self.radio_st
+00011d50: 6174 655b 226d 6f64 6522 5d20 3d20 2255  ate["mode"] = "U
+00011d60: 5342 220a 2020 2020 2020 2020 2020 2020  SB".            
+00011d70: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00011d80: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00011d90: 6c66 2e72 6164 696f 5f73 7461 7465 5b22  lf.radio_state["
+00011da0: 6d6f 6465 225d 203d 2022 4c53 4222 0a20  mode"] = "LSB". 
+00011db0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+00011dc0: 616e 6420 3d20 6765 7462 616e 6428 7374  and = getband(st
+00011dd0: 7228 7365 6c66 2e72 6164 696f 5f73 7461  r(self.radio_sta
+00011de0: 7465 2e67 6574 2822 7666 6f61 222c 2022  te.get("vfoa", "
+00011df0: 302e 3022 2929 290a 2020 2020 2020 2020  0.0"))).        
+00011e00: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+00011e10: 5f62 616e 645f 696e 6469 6361 746f 7228  _band_indicator(
+00011e20: 6261 6e64 290a 2020 2020 2020 2020 2020  band).          
+00011e30: 2020 2020 2020 7365 6c66 2e73 6574 5f77        self.set_w
+00011e40: 696e 646f 775f 7469 746c 6528 290a 2020  indow_title().  
+00011e50: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00011e60: 2073 656c 662e 7269 675f 636f 6e74 726f   self.rig_contro
+00011e70: 6c3a 0a20 2020 2020 2020 2020 2020 2020  l:.             
+00011e80: 2020 2020 2020 2073 656c 662e 7269 675f         self.rig_
+00011e90: 636f 6e74 726f 6c2e 7365 745f 6d6f 6465  control.set_mode
+00011ea0: 2873 656c 662e 7261 6469 6f5f 7374 6174  (self.radio_stat
+00011eb0: 652e 6765 7428 226d 6f64 6522 2929 0a20  e.get("mode")). 
+00011ec0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00011ed0: 656c 662e 636c 6561 7269 6e70 7574 7328  elf.clearinputs(
+00011ee0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00011ef0: 2020 7365 6c66 2e72 6561 645f 6377 5f6d    self.read_cw_m
+00011f00: 6163 726f 7328 290a 2020 2020 2020 2020  acros().        
+00011f10: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+00011f20: 2020 2020 2020 2020 2020 2069 6620 7374             if st
+00011f30: 7269 7070 6564 5f74 6578 7420 3d3d 2022  ripped_text == "
+00011f40: 4f50 4f4e 223a 0a20 2020 2020 2020 2020  OPON":.         
+00011f50: 2020 2020 2020 2073 656c 662e 6765 745f         self.get_
+00011f60: 6f70 6f6e 2829 0a20 2020 2020 2020 2020  opon().         
+00011f70: 2020 2020 2020 2073 656c 662e 636c 6561         self.clea
+00011f80: 7269 6e70 7574 7328 290a 2020 2020 2020  rinputs().      
+00011f90: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00011fa0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00011fb0: 7374 7269 7070 6564 5f74 6578 7420 3d3d  stripped_text ==
+00011fc0: 2022 5445 5354 223a 0a20 2020 2020 2020   "TEST":.       
+00011fd0: 2020 2020 2020 2020 2073 656c 662e 7368           self.sh
+00011fe0: 6f77 5f6d 6573 7361 6765 5f62 6f78 2822  ow_message_box("
+00011ff0: 5468 6973 2069 7320 6120 7465 7374 2229  This is a test")
+00012000: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012010: 2073 656c 662e 636c 6561 7269 6e70 7574   self.clearinput
+00012020: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
+00012030: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+00012040: 2020 2020 2020 2069 6620 7365 6c66 2e69         if self.i
+00012050: 735f 666c 6f61 7461 626c 6528 7374 7269  s_floatable(stri
+00012060: 7070 6564 5f74 6578 7429 3a0a 2020 2020  pped_text):.    
+00012070: 2020 2020 2020 2020 2020 2020 7666 6f20              vfo 
+00012080: 3d20 666c 6f61 7428 7374 7269 7070 6564  = float(stripped
+00012090: 5f74 6578 7429 0a20 2020 2020 2020 2020  _text).         
+000120a0: 2020 2020 2020 2076 666f 203d 2069 6e74         vfo = int
+000120b0: 2876 666f 202a 2031 3030 3029 0a20 2020  (vfo * 1000).   
+000120c0: 2020 2020 2020 2020 2020 2020 2062 616e               ban
+000120d0: 6420 3d20 6765 7462 616e 6428 7374 7228  d = getband(str(
+000120e0: 7666 6f29 290a 2020 2020 2020 2020 2020  vfo)).          
+000120f0: 2020 2020 2020 7365 6c66 2e73 6574 5f62        self.set_b
+00012100: 616e 645f 696e 6469 6361 746f 7228 6261  and_indicator(ba
+00012110: 6e64 290a 2020 2020 2020 2020 2020 2020  nd).            
+00012120: 2020 2020 2320 7365 6c66 2e63 6f6e 7461      # self.conta
+00012130: 6374 5b22 4261 6e64 225d 203d 2067 6574  ct["Band"] = get
+00012140: 5f6c 6f67 6765 645f 6261 6e64 2873 7472  _logged_band(str
+00012150: 2873 656c 662e 7261 6469 6f5f 7374 6174  (self.radio_stat
+00012160: 652e 6765 7428 2276 666f 6122 2c20 302e  e.get("vfoa", 0.
+00012170: 3029 2929 0a20 2020 2020 2020 2020 2020  0))).           
+00012180: 2020 2020 2073 656c 662e 7261 6469 6f5f       self.radio_
+00012190: 7374 6174 655b 2276 666f 6122 5d20 3d20  state["vfoa"] = 
+000121a0: 7666 6f0a 2020 2020 2020 2020 2020 2020  vfo.            
+000121b0: 2020 2020 7365 6c66 2e73 6574 5f77 696e      self.set_win
+000121c0: 646f 775f 7469 746c 6528 290a 2020 2020  dow_title().    
+000121d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000121e0: 2e63 6c65 6172 696e 7075 7473 2829 0a20  .clearinputs(). 
+000121f0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00012200: 6620 7365 6c66 2e72 6967 5f63 6f6e 7472  f self.rig_contr
+00012210: 6f6c 3a0a 2020 2020 2020 2020 2020 2020  ol:.            
+00012220: 2020 2020 2020 2020 7365 6c66 2e72 6967          self.rig
+00012230: 5f63 6f6e 7472 6f6c 2e73 6574 5f76 666f  _control.set_vfo
+00012240: 2876 666f 290a 2020 2020 2020 2020 2020  (vfo).          
+00012250: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00012260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012270: 2063 6d64 203d 207b 7d0a 2020 2020 2020   cmd = {}.      
+00012280: 2020 2020 2020 2020 2020 636d 645b 2263            cmd["c
+00012290: 6d64 225d 203d 2022 5241 4449 4f5f 5354  md"] = "RADIO_ST
+000122a0: 4154 4522 0a20 2020 2020 2020 2020 2020  ATE".           
+000122b0: 2020 2020 2063 6d64 5b22 7374 6174 696f       cmd["statio
+000122c0: 6e22 5d20 3d20 706c 6174 666f 726d 2e6e  n"] = platform.n
+000122d0: 6f64 6528 290a 2020 2020 2020 2020 2020  ode().          
+000122e0: 2020 2020 2020 636d 645b 2262 616e 6422        cmd["band"
+000122f0: 5d20 3d20 6261 6e64 0a20 2020 2020 2020  ] = band.       
+00012300: 2020 2020 2020 2020 2063 6d64 5b22 7666           cmd["vf
+00012310: 6f61 225d 203d 2076 666f 0a20 2020 2020  oa"] = vfo.     
+00012320: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00012330: 6d75 6c74 6963 6173 745f 696e 7465 7266  multicast_interf
+00012340: 6163 652e 7365 6e64 5f61 735f 6a73 6f6e  ace.send_as_json
+00012350: 2863 6d64 290a 2020 2020 2020 2020 2020  (cmd).          
+00012360: 2020 2020 2020 7265 7475 726e 0a0a 2020        return..  
+00012370: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00012380: 6865 636b 5f63 616c 6c73 6967 6e28 7374  heck_callsign(st
+00012390: 7269 7070 6564 5f74 6578 7429 0a20 2020  ripped_text).   
+000123a0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+000123b0: 2e63 6865 636b 5f64 7570 6528 7374 7269  .check_dupe(stri
+000123c0: 7070 6564 5f74 6578 7429 3a0a 2020 2020  pped_text):.    
+000123d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000123e0: 2e64 7570 655f 696e 6469 6361 746f 722e  .dupe_indicator.
+000123f0: 7368 6f77 2829 0a20 2020 2020 2020 2020  show().         
+00012400: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00012410: 2020 2020 2020 2020 2073 656c 662e 6475           self.du
+00012420: 7065 5f69 6e64 6963 6174 6f72 2e68 6964  pe_indicator.hid
+00012430: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+00012440: 5f74 6865 7468 7265 6164 203d 2074 6872  _thethread = thr
+00012450: 6561 6469 6e67 2e54 6872 6561 6428 0a20  eading.Thread(. 
+00012460: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00012470: 6172 6765 743d 7365 6c66 2e63 6865 636b  arget=self.check
+00012480: 5f63 616c 6c73 6967 6e32 2c0a 2020 2020  _callsign2,.    
+00012490: 2020 2020 2020 2020 2020 2020 6172 6773              args
+000124a0: 3d28 7465 7874 2c29 2c0a 2020 2020 2020  =(text,),.      
+000124b0: 2020 2020 2020 2020 2020 6461 656d 6f6e            daemon
+000124c0: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
+000124d0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+000124e0: 205f 7468 6574 6872 6561 642e 7374 6172   _thethread.star
+000124f0: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
+00012500: 7365 6c66 2e6e 6578 745f 6669 656c 642e  self.next_field.
+00012510: 7365 7446 6f63 7573 2829 0a20 2020 2020  setFocus().     
+00012520: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+00012530: 2020 2020 2020 636d 6420 3d20 7b7d 0a20        cmd = {}. 
+00012540: 2020 2020 2020 2063 6d64 5b22 636d 6422         cmd["cmd"
+00012550: 5d20 3d20 2243 414c 4c43 4841 4e47 4544  ] = "CALLCHANGED
+00012560: 220a 2020 2020 2020 2020 636d 645b 2273  ".        cmd["s
+00012570: 7461 7469 6f6e 225d 203d 2070 6c61 7466  tation"] = platf
+00012580: 6f72 6d2e 6e6f 6465 2829 0a20 2020 2020  orm.node().     
+00012590: 2020 2063 6d64 5b22 6361 6c6c 225d 203d     cmd["call"] =
+000125a0: 2073 7472 6970 7065 645f 7465 7874 0a20   stripped_text. 
+000125b0: 2020 2020 2020 2073 656c 662e 6d75 6c74         self.mult
+000125c0: 6963 6173 745f 696e 7465 7266 6163 652e  icast_interface.
+000125d0: 7365 6e64 5f61 735f 6a73 6f6e 2863 6d64  send_as_json(cmd
+000125e0: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
+000125f0: 6865 636b 5f63 616c 6c73 6967 6e28 7374  heck_callsign(st
+00012600: 7269 7070 6564 5f74 6578 7429 0a0a 2020  ripped_text)..  
+00012610: 2020 6465 6620 6368 6563 6b5f 6361 6c6c    def check_call
+00012620: 7369 676e 2873 656c 662c 2063 616c 6c73  sign(self, calls
+00012630: 6967 6e29 3a0a 2020 2020 2020 2020 2222  ign):.        ""
+00012640: 2243 6865 636b 2063 616c 6c20 6173 2065  "Check call as e
+00012650: 6e74 6572 6564 2222 220a 2020 2020 2020  ntered""".      
+00012660: 2020 7265 7375 6c74 203d 2063 7479 5f6c    result = cty_l
+00012670: 6f6f 6b75 7028 6361 6c6c 7369 676e 290a  ookup(callsign).
+00012680: 2020 2020 2020 2020 6465 6275 675f 7265          debug_re
+00012690: 7375 6c74 203d 2066 227b 7265 7375 6c74  sult = f"{result
+000126a0: 7d22 0a20 2020 2020 2020 206c 6f67 6765  }".        logge
+000126b0: 722e 6465 6275 6728 2225 7322 2c20 6465  r.debug("%s", de
+000126c0: 6275 675f 7265 7375 6c74 290a 2020 2020  bug_result).    
+000126d0: 2020 2020 6966 2072 6573 756c 743a 0a20      if result:. 
+000126e0: 2020 2020 2020 2020 2020 2066 6f72 2061             for a
+000126f0: 2069 6e20 7265 7375 6c74 2e69 7465 6d73   in result.items
+00012700: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00012710: 2020 2020 656e 7469 7479 203d 2061 5b31      entity = a[1
+00012720: 5d2e 6765 7428 2265 6e74 6974 7922 2c20  ].get("entity", 
+00012730: 2222 290a 2020 2020 2020 2020 2020 2020  "").            
+00012740: 2020 2020 6371 203d 2061 5b31 5d2e 6765      cq = a[1].ge
+00012750: 7428 2263 7122 2c20 2222 290a 2020 2020  t("cq", "").    
+00012760: 2020 2020 2020 2020 2020 2020 6974 7520              itu 
+00012770: 3d20 615b 315d 2e67 6574 2822 6974 7522  = a[1].get("itu"
+00012780: 2c20 2222 290a 2020 2020 2020 2020 2020  , "").          
+00012790: 2020 2020 2020 636f 6e74 696e 656e 7420        continent 
+000127a0: 3d20 615b 315d 2e67 6574 2822 636f 6e74  = a[1].get("cont
+000127b0: 696e 656e 7422 290a 2020 2020 2020 2020  inent").        
+000127c0: 2020 2020 2020 2020 6c61 7420 3d20 666c          lat = fl
+000127d0: 6f61 7428 615b 315d 2e67 6574 2822 6c61  oat(a[1].get("la
+000127e0: 7422 2c20 2230 2e30 2229 290a 2020 2020  t", "0.0")).    
+000127f0: 2020 2020 2020 2020 2020 2020 6c6f 6e20              lon 
+00012800: 3d20 666c 6f61 7428 615b 315d 2e67 6574  = float(a[1].get
+00012810: 2822 6c6f 6e67 222c 2022 302e 3022 2929  ("long", "0.0"))
+00012820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012830: 206c 6f6e 203d 206c 6f6e 202a 202d 3120   lon = lon * -1 
+00012840: 2023 2063 7479 2e64 6174 2066 696c 6520   # cty.dat file 
+00012850: 696e 7665 7274 7320 6c6f 6e67 6974 7564  inverts longitud
+00012860: 6573 0a20 2020 2020 2020 2020 2020 2020  es.             
+00012870: 2020 2070 7269 6d61 7279 5f70 6678 203d     primary_pfx =
+00012880: 2061 5b31 5d2e 6765 7428 2270 7269 6d61   a[1].get("prima
+00012890: 7279 5f70 6678 222c 2022 2229 0a20 2020  ry_pfx", "").   
+000128a0: 2020 2020 2020 2020 2020 2020 2068 6561               hea
+000128b0: 6469 6e67 203d 2062 6561 7269 6e67 5f77  ding = bearing_w
+000128c0: 6974 685f 6c61 746c 6f6e 2873 656c 662e  ith_latlon(self.
+000128d0: 7374 6174 696f 6e2e 6765 7428 2247 7269  station.get("Gri
+000128e0: 6453 7175 6172 6522 292c 206c 6174 2c20  dSquare"), lat, 
+000128f0: 6c6f 6e29 0a20 2020 2020 2020 2020 2020  lon).           
+00012900: 2020 2020 206b 696c 6f6d 6574 6572 7320       kilometers 
+00012910: 3d20 6469 7374 616e 6365 5f77 6974 685f  = distance_with_
+00012920: 6c61 746c 6f6e 280a 2020 2020 2020 2020  latlon(.        
+00012930: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00012940: 2e73 7461 7469 6f6e 2e67 6574 2822 4772  .station.get("Gr
+00012950: 6964 5371 7561 7265 2229 2c20 6c61 742c  idSquare"), lat,
+00012960: 206c 6f6e 0a20 2020 2020 2020 2020 2020   lon.           
+00012970: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00012980: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
+00012990: 696e 675f 6469 7374 616e 6365 2e73 6574  ing_distance.set
+000129a0: 5465 7874 280a 2020 2020 2020 2020 2020  Text(.          
+000129b0: 2020 2020 2020 2020 2020 6622 5265 6769            f"Regi
+000129c0: 6f6e 616c 2048 6467 207b 6865 6164 696e  onal Hdg {headin
+000129d0: 677d c2b0 204c 5020 7b72 6563 6970 726f  g}.. LP {recipro
+000129e0: 636f 6c28 6865 6164 696e 6729 7dc2 b020  col(heading)}.. 
+000129f0: 2f20 220a 2020 2020 2020 2020 2020 2020  / ".            
+00012a00: 2020 2020 2020 2020 6622 6469 7374 616e          f"distan
+00012a10: 6365 207b 696e 7428 6b69 6c6f 6d65 7465  ce {int(kilomete
+00012a20: 7273 2a30 2e36 3231 3337 3129 7d6d 6920  rs*0.621371)}mi 
+00012a30: 7b6b 696c 6f6d 6574 6572 737d 6b6d 220a  {kilometers}km".
+00012a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012a50: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00012a60: 2020 7365 6c66 2e63 6f6e 7461 6374 5b22    self.contact["
+00012a70: 436f 756e 7472 7950 7265 6669 7822 5d20  CountryPrefix"] 
+00012a80: 3d20 7072 696d 6172 795f 7066 780a 2020  = primary_pfx.  
+00012a90: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00012aa0: 6c66 2e63 6f6e 7461 6374 5b22 5a4e 225d  lf.contact["ZN"]
+00012ab0: 203d 2069 6e74 2863 7129 0a20 2020 2020   = int(cq).     
+00012ac0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00012ad0: 636f 6e74 6163 745b 2243 6f6e 7469 6e65  contact["Contine
+00012ae0: 6e74 225d 203d 2063 6f6e 7469 6e65 6e74  nt"] = continent
+00012af0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012b00: 2073 656c 662e 6478 5f65 6e74 6974 792e   self.dx_entity.
+00012b10: 7365 7454 6578 7428 0a20 2020 2020 2020  setText(.       
+00012b20: 2020 2020 2020 2020 2020 2020 2066 227b               f"{
+00012b30: 7072 696d 6172 795f 7066 787d 3a20 7b63  primary_pfx}: {c
+00012b40: 6f6e 7469 6e65 6e74 7d2f 7b65 6e74 6974  ontinent}/{entit
+00012b50: 797d 2063 713a 7b63 717d 2069 7475 3a7b  y} cq:{cq} itu:{
+00012b60: 6974 757d 220a 2020 2020 2020 2020 2020  itu}".          
+00012b70: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00012b80: 2020 2020 2020 2020 6966 206c 656e 2863          if len(c
+00012b90: 616c 6c73 6967 6e29 203e 2032 3a0a 2020  allsign) > 2:.  
+00012ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012bb0: 2020 6966 2073 656c 662e 636f 6e74 6573    if self.contes
+00012bc0: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+00012bd0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00012be0: 636f 6e74 6573 742e 7072 6566 696c 6c28  contest.prefill(
+00012bf0: 7365 6c66 290a 0a20 2020 2064 6566 2063  self)..    def c
+00012c00: 6865 636b 5f63 616c 6c73 6967 6e32 2873  heck_callsign2(s
+00012c10: 656c 662c 2063 616c 6c73 6967 6e29 3a0a  elf, callsign):.
+00012c20: 2020 2020 2020 2020 2222 2243 6865 636b          """Check
+00012c30: 2063 616c 6c20 6f6e 6365 2065 6e74 6572   call once enter
+00012c40: 6564 2222 220a 2020 2020 2020 2020 6361  ed""".        ca
+00012c50: 6c6c 7369 676e 203d 2063 616c 6c73 6967  llsign = callsig
+00012c60: 6e2e 7374 7269 7028 290a 2020 2020 2020  n.strip().      
+00012c70: 2020 6465 6275 675f 6c6f 6f6b 7570 203d    debug_lookup =
+00012c80: 2066 227b 7365 6c66 2e6c 6f6f 6b5f 7570   f"{self.look_up
+00012c90: 7d22 0a20 2020 2020 2020 206c 6f67 6765  }".        logge
+00012ca0: 722e 6465 6275 6728 2225 732c 2025 7322  r.debug("%s, %s"
+00012cb0: 2c20 6361 6c6c 7369 676e 2c20 6465 6275  , callsign, debu
+00012cc0: 675f 6c6f 6f6b 7570 290a 2020 2020 2020  g_lookup).      
+00012cd0: 2020 6966 2068 6173 6174 7472 2873 656c    if hasattr(sel
+00012ce0: 662e 6c6f 6f6b 5f75 702c 2022 7365 7373  f.look_up, "sess
+00012cf0: 696f 6e22 293a 0a20 2020 2020 2020 2020  ion"):.         
+00012d00: 2020 2069 6620 7365 6c66 2e6c 6f6f 6b5f     if self.look_
+00012d10: 7570 2e73 6573 7369 6f6e 3a0a 2020 2020  up.session:.    
+00012d20: 2020 2020 2020 2020 2020 2020 7265 7370              resp
+00012d30: 6f6e 7365 203d 2073 656c 662e 6c6f 6f6b  onse = self.look
+00012d40: 5f75 702e 6c6f 6f6b 7570 2863 616c 6c73  _up.lookup(calls
+00012d50: 6967 6e29 0a20 2020 2020 2020 2020 2020  ign).           
+00012d60: 2020 2020 2064 6562 7567 5f72 6573 706f       debug_respo
+00012d70: 6e73 6520 3d20 6622 7b72 6573 706f 6e73  nse = f"{respons
+00012d80: 657d 220a 2020 2020 2020 2020 2020 2020  e}".            
+00012d90: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+00012da0: 2822 5468 6520 5265 7370 6f6e 7365 3a20  ("The Response: 
+00012db0: 2573 5c6e 222c 2064 6562 7567 5f72 6573  %s\n", debug_res
+00012dc0: 706f 6e73 6529 0a20 2020 2020 2020 2020  ponse).         
+00012dd0: 2020 2020 2020 2069 6620 7265 7370 6f6e         if respon
+00012de0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00012df0: 2020 2020 2020 2020 7468 6569 7267 7269          theirgri
+00012e00: 6420 3d20 7265 7370 6f6e 7365 2e67 6574  d = response.get
+00012e10: 2822 6772 6964 2229 0a20 2020 2020 2020  ("grid").       
+00012e20: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00012e30: 662e 636f 6e74 6163 745b 2247 7269 6453  f.contact["GridS
+00012e40: 7175 6172 6522 5d20 3d20 7468 6569 7267  quare"] = theirg
+00012e50: 7269 640a 2020 2020 2020 2020 2020 2020  rid.            
+00012e60: 2020 2020 2020 2020 5f74 6865 6972 636f          _theirco
+00012e70: 756e 7472 7920 3d20 7265 7370 6f6e 7365  untry = response
+00012e80: 2e67 6574 2822 636f 756e 7472 7922 290a  .get("country").
+00012e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ea0: 2020 2020 6966 2073 656c 662e 7374 6174      if self.stat
+00012eb0: 696f 6e2e 6765 7428 2247 7269 6453 7175  ion.get("GridSqu
+00012ec0: 6172 6522 2c20 2222 293a 0a20 2020 2020  are", ""):.     
+00012ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ee0: 2020 2068 6561 6469 6e67 203d 2062 6561     heading = bea
+00012ef0: 7269 6e67 2873 656c 662e 7374 6174 696f  ring(self.statio
+00012f00: 6e2e 6765 7428 2247 7269 6453 7175 6172  n.get("GridSquar
+00012f10: 6522 2c20 2222 292c 2074 6865 6972 6772  e", ""), theirgr
+00012f20: 6964 290a 2020 2020 2020 2020 2020 2020  id).            
+00012f30: 2020 2020 2020 2020 2020 2020 6b69 6c6f              kilo
+00012f40: 6d65 7465 7273 203d 2064 6973 7461 6e63  meters = distanc
+00012f50: 6528 7365 6c66 2e73 7461 7469 6f6e 2e67  e(self.station.g
+00012f60: 6574 2822 4772 6964 5371 7561 7265 2229  et("GridSquare")
+00012f70: 2c20 7468 6569 7267 7269 6429 0a20 2020  , theirgrid).   
+00012f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012f90: 2020 2020 2073 656c 662e 6865 6164 696e       self.headin
+00012fa0: 675f 6469 7374 616e 6365 2e73 6574 5465  g_distance.setTe
+00012fb0: 7874 280a 2020 2020 2020 2020 2020 2020  xt(.            
+00012fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012fd0: 6622 7b74 6865 6972 6772 6964 7d20 4864  f"{theirgrid} Hd
+00012fe0: 6720 7b68 6561 6469 6e67 7dc2 b020 4c50  g {heading}.. LP
+00012ff0: 207b 7265 6369 7072 6f63 6f6c 2868 6561   {reciprocol(hea
+00013000: 6469 6e67 297d c2b0 202f 2022 0a20 2020  ding)}.. / ".   
+00013010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013020: 2020 2020 2020 2020 2066 2264 6973 7461           f"dista
+00013030: 6e63 6520 7b69 6e74 286b 696c 6f6d 6574  nce {int(kilomet
+00013040: 6572 732a 302e 3632 3133 3731 297d 6d69  ers*0.621371)}mi
+00013050: 207b 6b69 6c6f 6d65 7465 7273 7d6b 6d22   {kilometers}km"
+00013060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013070: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00013080: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00013090: 2073 656c 662e 6478 5f65 6e74 6974 792e   self.dx_entity.
+000130a0: 7365 7454 6578 7428 6622 7b74 6865 6972  setText(f"{their
+000130b0: 636f 756e 7472 797d 2229 0a20 2020 2020  country}").     
+000130c0: 2020 2020 2020 2020 2020 2023 2065 6c73             # els
+000130d0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+000130e0: 2020 2023 2073 656c 662e 6865 6164 696e     # self.headin
+000130f0: 675f 6469 7374 616e 6365 2e73 6574 5465  g_distance.setTe
+00013100: 7874 2822 4c6f 6f6b 7570 2066 6169 6c65  xt("Lookup faile
+00013110: 642e 2229 0a0a 2020 2020 6465 6620 6368  d.")..    def ch
+00013120: 6563 6b5f 6475 7065 2873 656c 662c 2063  eck_dupe(self, c
+00013130: 616c 6c3a 2073 7472 2920 2d3e 2062 6f6f  all: str) -> boo
+00013140: 6c3a 0a20 2020 2020 2020 2022 2222 4368  l:.        """Ch
+00013150: 6563 6b73 2069 6620 6120 6361 6c6c 7369  ecks if a callsi
+00013160: 676e 2069 7320 6120 6475 7065 206f 6e20  gn is a dupe on 
+00013170: 6375 7272 656e 7420 6261 6e64 2f6d 6f64  current band/mod
+00013180: 652e 2222 220a 2020 2020 2020 2020 7365  e.""".        se
+00013190: 6c66 2e63 6f6e 7465 7374 2e70 7265 6475  lf.contest.predu
+000131a0: 7065 2873 656c 6629 0a20 2020 2020 2020  pe(self).       
+000131b0: 2062 616e 6420 3d20 666c 6f61 7428 6765   band = float(ge
+000131c0: 745f 6c6f 6767 6564 5f62 616e 6428 7374  t_logged_band(st
+000131d0: 7228 7365 6c66 2e72 6164 696f 5f73 7461  r(self.radio_sta
+000131e0: 7465 2e67 6574 2822 7666 6f61 222c 2030  te.get("vfoa", 0
+000131f0: 2e30 2929 2929 0a20 2020 2020 2020 206d  .0)))).        m
+00013200: 6f64 6520 3d20 7365 6c66 2e72 6164 696f  ode = self.radio
+00013210: 5f73 7461 7465 2e67 6574 2822 6d6f 6465  _state.get("mode
+00013220: 222c 2022 2229 0a20 2020 2020 2020 2064  ", "").        d
+00013230: 6562 7567 6c69 6e65 203d 2028 0a20 2020  ebugline = (.   
+00013240: 2020 2020 2020 2020 2066 2243 616c 6c3a           f"Call:
+00013250: 207b 6361 6c6c 7d20 4261 6e64 3a20 7b62   {call} Band: {b
+00013260: 616e 647d 204d 6f64 653a 207b 6d6f 6465  and} Mode: {mode
+00013270: 7d20 4475 7065 7479 7065 3a20 7b73 656c  } Dupetype: {sel
+00013280: 662e 636f 6e74 6573 742e 6475 7065 5f74  f.contest.dupe_t
+00013290: 7970 657d 220a 2020 2020 2020 2020 290a  ype}".        ).
+000132a0: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+000132b0: 6562 7567 2822 2573 222c 2064 6562 7567  ebug("%s", debug
+000132c0: 6c69 6e65 290a 2020 2020 2020 2020 6966  line).        if
+000132d0: 2073 656c 662e 636f 6e74 6573 742e 6475   self.contest.du
+000132e0: 7065 5f74 7970 6520 3d3d 2031 3a0a 2020  pe_type == 1:.  
+000132f0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00013300: 203d 2073 656c 662e 6461 7461 6261 7365   = self.database
+00013310: 2e63 6865 636b 5f64 7570 6528 6361 6c6c  .check_dupe(call
+00013320: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+00013330: 662e 636f 6e74 6573 742e 6475 7065 5f74  f.contest.dupe_t
+00013340: 7970 6520 3d3d 2032 3a0a 2020 2020 2020  ype == 2:.      
+00013350: 2020 2020 2020 7265 7375 6c74 203d 2073        result = s
+00013360: 656c 662e 6461 7461 6261 7365 2e63 6865  elf.database.che
+00013370: 636b 5f64 7570 655f 6f6e 5f62 616e 6428  ck_dupe_on_band(
+00013380: 6361 6c6c 2c20 6261 6e64 290a 2020 2020  call, band).    
+00013390: 2020 2020 6966 2073 656c 662e 636f 6e74      if self.cont
+000133a0: 6573 742e 6475 7065 5f74 7970 6520 3d3d  est.dupe_type ==
+000133b0: 2033 3a0a 2020 2020 2020 2020 2020 2020   3:.            
+000133c0: 7265 7375 6c74 203d 2073 656c 662e 6461  result = self.da
+000133d0: 7461 6261 7365 2e63 6865 636b 5f64 7570  tabase.check_dup
+000133e0: 655f 6f6e 5f62 616e 645f 6d6f 6465 2863  e_on_band_mode(c
+000133f0: 616c 6c2c 2062 616e 642c 206d 6f64 6529  all, band, mode)
+00013400: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00013410: 2e63 6f6e 7465 7374 2e64 7570 655f 7479  .contest.dupe_ty
+00013420: 7065 203d 3d20 343a 0a20 2020 2020 2020  pe == 4:.       
+00013430: 2020 2020 2072 6573 756c 7420 3d20 7b22       result = {"
+00013440: 6973 6475 7065 223a 2046 616c 7365 7d0a  isdupe": False}.
+00013450: 2020 2020 2020 2020 6465 6275 676c 696e          debuglin
+00013460: 6520 3d20 6622 7b72 6573 756c 747d 220a  e = f"{result}".
+00013470: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+00013480: 6562 7567 2822 2573 222c 2064 6562 7567  ebug("%s", debug
+00013490: 6c69 6e65 290a 2020 2020 2020 2020 7265  line).        re
+000134a0: 7475 726e 2072 6573 756c 742e 6765 7428  turn result.get(
+000134b0: 2269 7364 7570 6522 2c20 4661 6c73 6529  "isdupe", False)
+000134c0: 0a0a 2020 2020 6465 6620 7365 746d 6f64  ..    def setmod
+000134d0: 6528 7365 6c66 2c20 6d6f 6465 3a20 7374  e(self, mode: st
+000134e0: 7229 202d 3e20 4e6f 6e65 3a0a 2020 2020  r) -> None:.    
+000134f0: 2020 2020 2222 2273 7475 6220 666f 7220      """stub for 
+00013500: 7768 656e 2074 6865 206d 6f64 6520 6368  when the mode ch
+00013510: 616e 6765 732e 2222 220a 2020 2020 2020  anges.""".      
+00013520: 2020 6966 206d 6f64 6520 3d3d 2022 4357    if mode == "CW
+00013530: 223a 0a20 2020 2020 2020 2020 2020 2073  ":.            s
+00013540: 656c 662e 6375 7272 656e 745f 6d6f 6465  elf.current_mode
+00013550: 203d 2022 4357 220a 2020 2020 2020 2020   = "CW".        
+00013560: 2020 2020 2320 7365 6c66 2e6d 6f64 652e      # self.mode.
+00013570: 7365 7454 6578 7428 2243 5722 290a 2020  setText("CW").  
+00013580: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00013590: 656e 742e 7365 7454 6578 7428 2235 3939  ent.setText("599
+000135a0: 2229 0a20 2020 2020 2020 2020 2020 2073  ").            s
+000135b0: 656c 662e 7265 6365 6976 652e 7365 7454  elf.receive.setT
+000135c0: 6578 7428 2235 3939 2229 0a20 2020 2020  ext("599").     
+000135d0: 2020 2020 2020 2073 656c 662e 7265 6164         self.read
+000135e0: 5f63 775f 6d61 6372 6f73 2829 0a20 2020  _cw_macros().   
+000135f0: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+00013600: 2020 2020 2020 2020 6966 206d 6f64 6520          if mode 
+00013610: 3d3d 2022 5353 4222 3a0a 2020 2020 2020  == "SSB":.      
+00013620: 2020 2020 2020 7365 6c66 2e63 7572 7265        self.curre
+00013630: 6e74 5f6d 6f64 6520 3d20 2253 5342 220a  nt_mode = "SSB".
+00013640: 2020 2020 2020 2020 2020 2020 2320 7365              # se
+00013650: 6c66 2e6d 6f64 652e 7365 7454 6578 7428  lf.mode.setText(
+00013660: 2253 5342 2229 0a20 2020 2020 2020 2020  "SSB").         
+00013670: 2020 2073 656c 662e 7365 6e74 2e73 6574     self.sent.set
+00013680: 5465 7874 2822 3539 2229 0a20 2020 2020  Text("59").     
+00013690: 2020 2020 2020 2073 656c 662e 7265 6365         self.rece
+000136a0: 6976 652e 7365 7454 6578 7428 2235 3922  ive.setText("59"
+000136b0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+000136c0: 6c66 2e72 6561 645f 6377 5f6d 6163 726f  lf.read_cw_macro
+000136d0: 7328 290a 2020 2020 2020 2020 6966 206d  s().        if m
+000136e0: 6f64 6520 3d3d 2022 5254 5459 223a 0a20  ode == "RTTY":. 
+000136f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00013700: 6375 7272 656e 745f 6d6f 6465 203d 2022  current_mode = "
+00013710: 5254 5459 220a 2020 2020 2020 2020 2020  RTTY".          
+00013720: 2020 2320 7365 6c66 2e6d 6f64 652e 7365    # self.mode.se
+00013730: 7454 6578 7428 2252 5454 5922 290a 2020  tText("RTTY").  
+00013740: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00013750: 656e 742e 7365 7454 6578 7428 2235 3922  ent.setText("59"
+00013760: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00013770: 6c66 2e72 6563 6569 7665 2e73 6574 5465  lf.receive.setTe
+00013780: 7874 2822 3539 2229 0a0a 2020 2020 6465  xt("59")..    de
+00013790: 6620 6765 745f 6f70 6f6e 2873 656c 6629  f get_opon(self)
+000137a0: 3a0a 2020 2020 2020 2020 2222 2243 7472  :.        """Ctr
+000137b0: 6c2b 4f20 6f72 204f 504f 4e20 6469 616c  l+O or OPON dial
+000137c0: 6f67 2222 220a 2020 2020 2020 2020 7365  og""".        se
+000137d0: 6c66 2e6f 706f 6e5f 6469 616c 6f67 203d  lf.opon_dialog =
+000137e0: 204f 704f 6e28 574f 524b 494e 475f 5041   OpOn(WORKING_PA
+000137f0: 5448 290a 2020 2020 2020 2020 7365 6c66  TH).        self
+00013800: 2e6f 706f 6e5f 6469 616c 6f67 2e61 6363  .opon_dialog.acc
+00013810: 6570 7465 642e 636f 6e6e 6563 7428 7365  epted.connect(se
+00013820: 6c66 2e6e 6577 5f6f 7029 0a20 2020 2020  lf.new_op).     
+00013830: 2020 2073 656c 662e 6f70 6f6e 5f64 6961     self.opon_dia
+00013840: 6c6f 672e 6f70 656e 2829 0a0a 2020 2020  log.open()..    
+00013850: 6465 6620 6e65 775f 6f70 2873 656c 6629  def new_op(self)
+00013860: 3a0a 2020 2020 2020 2020 2222 2253 6176  :.        """Sav
+00013870: 6520 6e65 7720 4f50 2222 220a 2020 2020  e new OP""".    
+00013880: 2020 2020 6966 2073 656c 662e 6f70 6f6e      if self.opon
+00013890: 5f64 6961 6c6f 672e 4e65 774f 7065 7261  _dialog.NewOpera
+000138a0: 746f 722e 7465 7874 2829 3a0a 2020 2020  tor.text():.    
+000138b0: 2020 2020 2020 2020 7365 6c66 2e63 7572          self.cur
+000138c0: 7265 6e74 5f6f 7020 3d20 7365 6c66 2e6f  rent_op = self.o
+000138d0: 706f 6e5f 6469 616c 6f67 2e4e 6577 4f70  pon_dialog.NewOp
+000138e0: 6572 6174 6f72 2e74 6578 7428 292e 7570  erator.text().up
+000138f0: 7065 7228 290a 2020 2020 2020 2020 7365  per().        se
+00013900: 6c66 2e6f 706f 6e5f 6469 616c 6f67 2e63  lf.opon_dialog.c
+00013910: 6c6f 7365 2829 0a20 2020 2020 2020 206c  lose().        l
+00013920: 6f67 6765 722e 6465 6275 6728 224e 6577  ogger.debug("New
+00013930: 204f 703a 2025 7322 2c20 7365 6c66 2e63   Op: %s", self.c
+00013940: 7572 7265 6e74 5f6f 7029 0a20 2020 2020  urrent_op).     
+00013950: 2020 2073 656c 662e 6d61 6b65 5f6f 705f     self.make_op_
+00013960: 6469 7228 290a 0a20 2020 2064 6566 206d  dir()..    def m
+00013970: 616b 655f 6f70 5f64 6972 2873 656c 6629  ake_op_dir(self)
+00013980: 3a0a 2020 2020 2020 2020 2222 2243 7265  :.        """Cre
+00013990: 6174 6520 4f50 2064 6972 6563 746f 7279  ate OP directory
+000139a0: 2069 6620 6974 2064 6f65 7320 6e6f 7420   if it does not 
+000139b0: 6578 6973 742e 2222 220a 2020 2020 2020  exist.""".      
+000139c0: 2020 6966 2073 656c 662e 6375 7272 656e    if self.curren
+000139d0: 745f 6f70 3a0a 2020 2020 2020 2020 2020  t_op:.          
+000139e0: 2020 6f70 5f70 6174 6820 3d20 5061 7468    op_path = Path
+000139f0: 2844 4154 415f 5041 5448 2920 2f20 7365  (DATA_PATH) / se
+00013a00: 6c66 2e63 7572 7265 6e74 5f6f 700a 2020  lf.current_op.  
+00013a10: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+00013a20: 2e64 6562 7567 2822 6f70 5f70 6174 683a  .debug("op_path:
+00013a30: 2025 7322 2c20 7374 7228 6f70 5f70 6174   %s", str(op_pat
+00013a40: 6829 290a 2020 2020 2020 2020 2020 2020  h)).            
+00013a50: 6966 206f 705f 7061 7468 2e69 735f 6469  if op_path.is_di
+00013a60: 7228 2920 6973 2046 616c 7365 3a0a 2020  r() is False:.  
+00013a70: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+00013a80: 6767 6572 2e64 6562 7567 2822 4372 6561  gger.debug("Crea
+00013a90: 7469 6e67 204f 7020 4469 7265 6374 6f72  ting Op Director
+00013aa0: 793a 2025 7322 2c20 7374 7228 6f70 5f70  y: %s", str(op_p
+00013ab0: 6174 6829 290a 2020 2020 2020 2020 2020  ath)).          
+00013ac0: 2020 2020 2020 6f73 2e6d 6b64 6972 2873        os.mkdir(s
+00013ad0: 7472 286f 705f 7061 7468 2929 0a20 2020  tr(op_path)).   
+00013ae0: 2020 2020 2020 2020 2069 6620 6f70 5f70           if op_p
+00013af0: 6174 682e 6973 5f64 6972 2829 3a0a 2020  ath.is_dir():.  
+00013b00: 2020 2020 2020 2020 2020 2020 2020 736f                so
+00013b10: 7572 6365 5f70 6174 6820 3d20 5061 7468  urce_path = Path
+00013b20: 2857 4f52 4b49 4e47 5f50 4154 4829 202f  (WORKING_PATH) /
+00013b30: 2022 6461 7461 2220 2f20 2270 686f 6e65   "data" / "phone
+00013b40: 7469 6373 220a 2020 2020 2020 2020 2020  tics".          
+00013b50: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
+00013b60: 7567 2822 736f 7572 6365 5f70 6174 683a  ug("source_path:
+00013b70: 2025 7322 2c20 7374 7228 736f 7572 6365   %s", str(source
+00013b80: 5f70 6174 6829 290a 2020 2020 2020 2020  _path)).        
+00013b90: 2020 2020 2020 2020 666f 7220 6368 696c          for chil
+00013ba0: 6420 696e 2073 6f75 7263 655f 7061 7468  d in source_path
+00013bb0: 2e69 7465 7264 6972 2829 3a0a 2020 2020  .iterdir():.    
+00013bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013bd0: 6465 7374 696e 6174 696f 6e5f 6669 6c65  destination_file
+00013be0: 203d 206f 705f 7061 7468 202f 2063 6869   = op_path / chi
+00013bf0: 6c64 2e6e 616d 650a 2020 2020 2020 2020  ld.name.        
+00013c00: 2020 2020 2020 2020 2020 2020 6966 2064              if d
+00013c10: 6573 7469 6e61 7469 6f6e 5f66 696c 652e  estination_file.
+00013c20: 6973 5f66 696c 6528 2920 6973 2046 616c  is_file() is Fal
+00013c30: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00013c40: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+00013c50: 6572 2e64 6562 7567 2822 4465 7374 696e  er.debug("Destin
+00013c60: 6174 696f 6e3a 2025 7322 2c20 7374 7228  ation: %s", str(
+00013c70: 6465 7374 696e 6174 696f 6e5f 6669 6c65  destination_file
+00013c80: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+00013c90: 2020 2020 2020 2020 2020 2064 6573 7469             desti
+00013ca0: 6e61 7469 6f6e 5f66 696c 652e 7772 6974  nation_file.writ
+00013cb0: 655f 6279 7465 7328 6368 696c 642e 7265  e_bytes(child.re
+00013cc0: 6164 5f62 7974 6573 2829 290a 0a20 2020  ad_bytes())..   
+00013cd0: 2064 6566 2070 6f6c 6c5f 7261 6469 6f28   def poll_radio(
+00013ce0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+00013cf0: 2222 7374 7562 2222 220a 2020 2020 2020  ""stub""".      
+00013d00: 2020 6966 2073 656c 662e 7269 675f 636f    if self.rig_co
+00013d10: 6e74 726f 6c3a 0a20 2020 2020 2020 2020  ntrol:.         
+00013d20: 2020 2069 6620 7365 6c66 2e72 6967 5f63     if self.rig_c
+00013d30: 6f6e 7472 6f6c 2e6f 6e6c 696e 6520 6973  ontrol.online is
+00013d40: 2046 616c 7365 3a0a 2020 2020 2020 2020   False:.        
+00013d50: 2020 2020 2020 2020 7365 6c66 2e72 6967          self.rig
+00013d60: 5f63 6f6e 7472 6f6c 2e72 6569 6e69 7428  _control.reinit(
+00013d70: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00013d80: 2073 656c 662e 7269 675f 636f 6e74 726f   self.rig_contro
+00013d90: 6c2e 6f6e 6c69 6e65 3a0a 2020 2020 2020  l.online:.      
+00013da0: 2020 2020 2020 2020 2020 696e 666f 5f64            info_d
+00013db0: 6972 7479 203d 2046 616c 7365 0a20 2020  irty = False.   
+00013dc0: 2020 2020 2020 2020 2020 2020 2076 666f               vfo
+00013dd0: 203d 2073 656c 662e 7269 675f 636f 6e74   = self.rig_cont
+00013de0: 726f 6c2e 6765 745f 7666 6f28 290a 2020  rol.get_vfo().  
+00013df0: 2020 2020 2020 2020 2020 2020 2020 6d6f                mo
+00013e00: 6465 203d 2073 656c 662e 7269 675f 636f  de = self.rig_co
+00013e10: 6e74 726f 6c2e 6765 745f 6d6f 6465 2829  ntrol.get_mode()
+00013e20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013e30: 2062 7720 3d20 7365 6c66 2e72 6967 5f63   bw = self.rig_c
+00013e40: 6f6e 7472 6f6c 2e67 6574 5f62 7728 290a  ontrol.get_bw().
+00013e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013e60: 2320 7365 6c66 2e72 6164 696f 5f73 7461  # self.radio_sta
+00013e70: 7465 5b22 7074 7422 5d20 3d20 7365 6c66  te["ptt"] = self
+00013e80: 2e72 6967 5f63 6f6e 7472 6f6c 2e67 6574  .rig_control.get
+00013e90: 5f70 7474 2829 0a0a 2020 2020 2020 2020  _ptt()..        
+00013ea0: 2020 2020 2020 2020 6966 206d 6f64 6520          if mode 
+00013eb0: 3d3d 2022 4357 223a 0a20 2020 2020 2020  == "CW":.       
+00013ec0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00013ed0: 662e 7365 746d 6f64 6528 6d6f 6465 290a  f.setmode(mode).
+00013ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ef0: 6966 206d 6f64 6520 3d3d 2022 4c53 4222  if mode == "LSB"
+00013f00: 206f 7220 6d6f 6465 203d 3d20 2255 5342   or mode == "USB
+00013f10: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
+00013f20: 2020 2020 2020 2073 656c 662e 7365 746d         self.setm
+00013f30: 6f64 6528 2253 5342 2229 0a20 2020 2020  ode("SSB").     
+00013f40: 2020 2020 2020 2020 2020 2069 6620 6d6f             if mo
+00013f50: 6465 203d 3d20 2252 5454 5922 3a0a 2020  de == "RTTY":.  
+00013f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013f70: 2020 7365 6c66 2e73 6574 6d6f 6465 2822    self.setmode("
+00013f80: 5254 5459 2229 0a0a 2020 2020 2020 2020  RTTY")..        
+00013f90: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00013fa0: 7261 6469 6f5f 7374 6174 652e 6765 7428  radio_state.get(
+00013fb0: 2276 666f 6122 2920 213d 2076 666f 3a0a  "vfoa") != vfo:.
+00013fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013fd0: 2020 2020 696e 666f 5f64 6972 7479 203d      info_dirty =
+00013fe0: 2054 7275 650a 2020 2020 2020 2020 2020   True.          
+00013ff0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+00014000: 6164 696f 5f73 7461 7465 5b22 7666 6f61  adio_state["vfoa
+00014010: 225d 203d 2076 666f 0a20 2020 2020 2020  "] = vfo.       
+00014020: 2020 2020 2020 2020 2062 616e 6420 3d20           band = 
+00014030: 6765 7462 616e 6428 7374 7228 7666 6f29  getband(str(vfo)
+00014040: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00014050: 2020 7365 6c66 2e72 6164 696f 5f73 7461    self.radio_sta
+00014060: 7465 5b22 6261 6e64 225d 203d 2062 616e  te["band"] = ban
+00014070: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
+00014080: 2020 7365 6c66 2e63 6f6e 7461 6374 5b22    self.contact["
+00014090: 4261 6e64 225d 203d 2067 6574 5f6c 6f67  Band"] = get_log
+000140a0: 6765 645f 6261 6e64 2873 7472 2876 666f  ged_band(str(vfo
+000140b0: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+000140c0: 2020 2073 656c 662e 7365 745f 6261 6e64     self.set_band
+000140d0: 5f69 6e64 6963 6174 6f72 2862 616e 6429  _indicator(band)
+000140e0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000140f0: 2020 6966 2073 656c 662e 7261 6469 6f5f    if self.radio_
+00014100: 7374 6174 652e 6765 7428 226d 6f64 6522  state.get("mode"
+00014110: 2920 213d 206d 6f64 653a 0a20 2020 2020  ) != mode:.     
+00014120: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00014130: 6e66 6f5f 6469 7274 7920 3d20 5472 7565  nfo_dirty = True
+00014140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014150: 2020 2020 2073 656c 662e 7261 6469 6f5f       self.radio_
+00014160: 7374 6174 655b 226d 6f64 6522 5d20 3d20  state["mode"] = 
+00014170: 6d6f 6465 0a0a 2020 2020 2020 2020 2020  mode..          
+00014180: 2020 2020 2020 6966 2073 656c 662e 7261        if self.ra
+00014190: 6469 6f5f 7374 6174 652e 6765 7428 2262  dio_state.get("b
+000141a0: 7722 2920 213d 2062 773a 0a20 2020 2020  w") != bw:.     
+000141b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000141c0: 6e66 6f5f 6469 7274 7920 3d20 5472 7565  nfo_dirty = True
+000141d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000141e0: 2020 2020 2073 656c 662e 7261 6469 6f5f       self.radio_
+000141f0: 7374 6174 655b 2262 7722 5d20 3d20 6277  state["bw"] = bw
+00014200: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014210: 2020 6966 2064 6174 6574 696d 652e 6e6f    if datetime.no
+00014220: 7728 2920 3e20 676c 6f62 616c 7328 295b  w() > globals()[
+00014230: 2270 6f6c 6c5f 7469 6d65 225d 206f 7220  "poll_time"] or 
+00014240: 696e 666f 5f64 6972 7479 3a0a 2020 2020  info_dirty:.    
+00014250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014260: 6c6f 6767 6572 2e64 6562 7567 2822 5646  logger.debug("VF
+00014270: 4f3a 2025 7320 204d 4f44 453a 2025 7320  O: %s  MODE: %s 
+00014280: 4257 3a20 2573 222c 2076 666f 2c20 6d6f  BW: %s", vfo, mo
+00014290: 6465 2c20 6277 290a 2020 2020 2020 2020  de, bw).        
+000142a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000142b0: 2e73 6574 5f77 696e 646f 775f 7469 746c  .set_window_titl
+000142c0: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+000142d0: 2020 2020 2020 2020 636d 6420 3d20 7b7d          cmd = {}
+000142e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000142f0: 2020 2020 2063 6d64 5b22 636d 6422 5d20       cmd["cmd"] 
+00014300: 3d20 2252 4144 494f 5f53 5441 5445 220a  = "RADIO_STATE".
+00014310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014320: 2020 2020 636d 645b 2273 7461 7469 6f6e      cmd["station
+00014330: 225d 203d 2070 6c61 7466 6f72 6d2e 6e6f  "] = platform.no
+00014340: 6465 2829 0a20 2020 2020 2020 2020 2020  de().           
+00014350: 2020 2020 2020 2020 2063 6d64 5b22 6261           cmd["ba
+00014360: 6e64 225d 203d 2062 616e 640a 2020 2020  nd"] = band.    
+00014370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014380: 636d 645b 2276 666f 6122 5d20 3d20 7666  cmd["vfoa"] = vf
+00014390: 6f0a 2020 2020 2020 2020 2020 2020 2020  o.              
+000143a0: 2020 2020 2020 636d 645b 226d 6f64 6522        cmd["mode"
+000143b0: 5d20 3d20 6d6f 6465 0a20 2020 2020 2020  ] = mode.       
+000143c0: 2020 2020 2020 2020 2020 2020 2063 6d64               cmd
+000143d0: 5b22 6277 225d 203d 2062 770a 2020 2020  ["bw"] = bw.    
+000143e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000143f0: 7365 6c66 2e6d 756c 7469 6361 7374 5f69  self.multicast_i
+00014400: 6e74 6572 6661 6365 2e73 656e 645f 6173  nterface.send_as
+00014410: 5f6a 736f 6e28 636d 6429 0a20 2020 2020  _json(cmd).     
+00014420: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00014430: 6620 7365 6c66 2e6e 316d 6d3a 0a20 2020  f self.n1mm:.   
+00014440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014450: 2020 2020 2069 6620 7365 6c66 2e6e 316d       if self.n1m
+00014460: 6d2e 7365 6e64 5f72 6164 696f 5f70 6163  m.send_radio_pac
+00014470: 6b65 7473 3a0a 2020 2020 2020 2020 2020  kets:.          
+00014480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014490: 2020 7365 6c66 2e6e 316d 6d2e 7261 6469    self.n1mm.radi
+000144a0: 6f5f 696e 666f 5b22 4672 6571 225d 203d  o_info["Freq"] =
+000144b0: 2076 666f 5b3a 2d31 5d0a 2020 2020 2020   vfo[:-1].      
+000144c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000144d0: 2020 2020 2020 7365 6c66 2e6e 316d 6d2e        self.n1mm.
+000144e0: 7261 6469 6f5f 696e 666f 5b22 5458 4672  radio_info["TXFr
+000144f0: 6571 225d 203d 2076 666f 5b3a 2d31 5d0a  eq"] = vfo[:-1].
+00014500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014510: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00014520: 2e6e 316d 6d2e 7261 6469 6f5f 696e 666f  .n1mm.radio_info
+00014530: 5b22 4d6f 6465 225d 203d 206d 6f64 650a  ["Mode"] = mode.
+00014540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014550: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00014560: 2e6e 316d 6d2e 7261 6469 6f5f 696e 666f  .n1mm.radio_info
+00014570: 5b22 4f70 4361 6c6c 225d 203d 2073 656c  ["OpCall"] = sel
+00014580: 662e 6375 7272 656e 745f 6f70 0a20 2020  f.current_op.   
+00014590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000145a0: 2020 2020 2020 2020 2073 656c 662e 6e31           self.n1
+000145b0: 6d6d 2e72 6164 696f 5f69 6e66 6f5b 2249  mm.radio_info["I
+000145c0: 7352 756e 6e69 6e67 225d 203d 2073 7472  sRunning"] = str
+000145d0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000145e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000145f0: 2020 7365 6c66 2e70 7265 662e 6765 7428    self.pref.get(
+00014600: 2272 756e 5f73 7461 7465 222c 2046 616c  "run_state", Fal
+00014610: 7365 290a 2020 2020 2020 2020 2020 2020  se).            
+00014620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014630: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00014640: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00014650: 6c66 2e6e 316d 6d2e 7365 6e64 5f72 6164  lf.n1mm.send_rad
+00014660: 696f 2829 0a20 2020 2020 2020 2020 2020  io().           
+00014670: 2020 2020 2020 2020 2067 6c6f 6261 6c73           globals
+00014680: 2829 5b22 706f 6c6c 5f74 696d 6522 5d20  ()["poll_time"] 
+00014690: 3d20 6461 7465 7469 6d65 2e6e 6f77 2829  = datetime.now()
+000146a0: 202b 2064 742e 7469 6d65 6465 6c74 6128   + dt.timedelta(
+000146b0: 7365 636f 6e64 733d 3130 290a 0a20 2020  seconds=10)..   
+000146c0: 2064 6566 2065 6469 745f 6377 5f6d 6163   def edit_cw_mac
+000146d0: 726f 7328 7365 6c66 2920 2d3e 204e 6f6e  ros(self) -> Non
+000146e0: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
+000146f0: 2020 2020 2020 2043 616c 6c73 2074 6865         Calls the
+00014700: 2064 6566 6175 6c74 2074 6578 7420 6564   default text ed
+00014710: 6974 6f72 2074 6f20 6564 6974 2074 6865  itor to edit the
+00014720: 2043 5720 6d61 6372 6f20 6669 6c65 2e0a   CW macro file..
+00014730: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00014740: 2020 2020 6966 2073 656c 662e 7261 6469      if self.radi
+00014750: 6f5f 7374 6174 652e 6765 7428 226d 6f64  o_state.get("mod
+00014760: 6522 2920 3d3d 2022 4357 223a 0a20 2020  e") == "CW":.   
+00014770: 2020 2020 2020 2020 206d 6163 726f 5f66           macro_f
+00014780: 696c 6520 3d20 222f 6377 6d61 6372 6f73  ile = "/cwmacros
+00014790: 2e74 7874 220a 2020 2020 2020 2020 656c  .txt".        el
+000147a0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+000147b0: 6d61 6372 6f5f 6669 6c65 203d 2022 2f73  macro_file = "/s
+000147c0: 7362 6d61 6372 6f73 2e74 7874 220a 2020  sbmacros.txt".  
+000147d0: 2020 2020 2020 6966 206e 6f74 2050 6174        if not Pat
+000147e0: 6828 4441 5441 5f50 4154 4820 2b20 6d61  h(DATA_PATH + ma
+000147f0: 6372 6f5f 6669 6c65 292e 6578 6973 7473  cro_file).exists
+00014800: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00014810: 6c6f 6767 6572 2e64 6562 7567 2822 7265  logger.debug("re
+00014820: 6164 5f63 775f 6d61 6372 6f73 3a20 636f  ad_cw_macros: co
+00014830: 7079 696e 6720 6465 6661 756c 7420 6d61  pying default ma
+00014840: 6372 6f20 6669 6c65 2e22 290a 2020 2020  cro file.").    
+00014850: 2020 2020 2020 2020 636f 7079 6669 6c65          copyfile
+00014860: 2857 4f52 4b49 4e47 5f50 4154 4820 2b20  (WORKING_PATH + 
+00014870: 222f 6461 7461 2220 2b20 6d61 6372 6f5f  "/data" + macro_
+00014880: 6669 6c65 2c20 4441 5441 5f50 4154 4820  file, DATA_PATH 
+00014890: 2b20 6d61 6372 6f5f 6669 6c65 290a 2020  + macro_file).  
+000148a0: 2020 2020 2020 6f73 2e73 7973 7465 6d28        os.system(
+000148b0: 6622 7864 672d 6f70 656e 207b 4441 5441  f"xdg-open {DATA
+000148c0: 5f50 4154 487d 7b6d 6163 726f 5f66 696c  _PATH}{macro_fil
+000148d0: 657d 2229 0a0a 2020 2020 6465 6620 7265  e}")..    def re
+000148e0: 6164 5f63 775f 6d61 6372 6f73 2873 656c  ad_cw_macros(sel
+000148f0: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
+00014900: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00014910: 5265 6164 7320 696e 2074 6865 2043 5720  Reads in the CW 
+00014920: 6d61 6372 6f73 2c20 6669 7273 7473 2069  macros, firsts i
+00014930: 7420 6368 6563 6b73 2074 6f20 7365 6520  t checks to see 
+00014940: 6966 2074 6865 2066 696c 6520 6578 6973  if the file exis
+00014950: 7473 2e20 4966 2069 7420 646f 6573 206e  ts. If it does n
+00014960: 6f74 2c0a 2020 2020 2020 2020 616e 6420  ot,.        and 
+00014970: 7468 6973 2068 6173 2062 6565 6e20 7061  this has been pa
+00014980: 636b 6167 6564 2077 6974 6820 7079 696e  ckaged with pyin
+00014990: 7374 616c 6c65 7220 6974 2077 696c 6c20  staller it will 
+000149a0: 636f 7079 2074 6865 2064 6566 6175 6c74  copy the default
+000149b0: 2066 696c 6520 6672 6f6d 2074 6865 0a20   file from the. 
+000149c0: 2020 2020 2020 2074 656d 7020 6469 7265         temp dire
+000149d0: 6374 6f72 7920 7468 6973 2069 7320 7275  ctory this is ru
+000149e0: 6e6e 696e 6720 6672 6f6d 2e2e 2e20 496e  nning from... In
+000149f0: 2074 6865 6f72 792e 0a20 2020 2020 2020   theory..       
+00014a00: 2022 2222 0a0a 2020 2020 2020 2020 6966   """..        if
+00014a10: 2073 656c 662e 7261 6469 6f5f 7374 6174   self.radio_stat
+00014a20: 652e 6765 7428 226d 6f64 6522 2920 3d3d  e.get("mode") ==
+00014a30: 2022 4357 223a 0a20 2020 2020 2020 2020   "CW":.         
+00014a40: 2020 206d 6163 726f 5f66 696c 6520 3d20     macro_file = 
+00014a50: 222f 6377 6d61 6372 6f73 2e74 7874 220a  "/cwmacros.txt".
+00014a60: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00014a70: 2020 2020 2020 2020 2020 6d61 6372 6f5f            macro_
+00014a80: 6669 6c65 203d 2022 2f73 7362 6d61 6372  file = "/ssbmacr
+00014a90: 6f73 2e74 7874 220a 0a20 2020 2020 2020  os.txt"..       
+00014aa0: 2069 6620 6e6f 7420 5061 7468 2844 4154   if not Path(DAT
+00014ab0: 415f 5041 5448 202b 206d 6163 726f 5f66  A_PATH + macro_f
+00014ac0: 696c 6529 2e65 7869 7374 7328 293a 0a20  ile).exists():. 
+00014ad0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+00014ae0: 722e 6465 6275 6728 2272 6561 645f 6377  r.debug("read_cw
+00014af0: 5f6d 6163 726f 733a 2063 6f70 7969 6e67  _macros: copying
+00014b00: 2064 6566 6175 6c74 206d 6163 726f 2066   default macro f
+00014b10: 696c 652e 2229 0a20 2020 2020 2020 2020  ile.").         
+00014b20: 2020 2063 6f70 7966 696c 6528 574f 524b     copyfile(WORK
+00014b30: 494e 475f 5041 5448 202b 2022 2f64 6174  ING_PATH + "/dat
+00014b40: 6122 202b 206d 6163 726f 5f66 696c 652c  a" + macro_file,
+00014b50: 2044 4154 415f 5041 5448 202b 206d 6163   DATA_PATH + mac
+00014b60: 726f 5f66 696c 6529 0a20 2020 2020 2020  ro_file).       
+00014b70: 2077 6974 6820 6f70 656e 2844 4154 415f   with open(DATA_
+00014b80: 5041 5448 202b 206d 6163 726f 5f66 696c  PATH + macro_fil
+00014b90: 652c 2022 7222 2c20 656e 636f 6469 6e67  e, "r", encoding
+00014ba0: 3d22 7574 662d 3822 2920 6173 2066 696c  ="utf-8") as fil
+00014bb0: 655f 6465 7363 7269 7074 6f72 3a0a 2020  e_descriptor:.  
+00014bc0: 2020 2020 2020 2020 2020 666f 7220 6c69            for li
+00014bd0: 6e65 2069 6e20 6669 6c65 5f64 6573 6372  ne in file_descr
+00014be0: 6970 746f 723a 0a20 2020 2020 2020 2020  iptor:.         
+00014bf0: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+00014c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014c10: 6d6f 6465 2c20 666b 6579 2c20 6275 7474  mode, fkey, butt
+00014c20: 6f6e 6e61 6d65 2c20 6377 7465 7874 203d  onname, cwtext =
+00014c30: 206c 696e 652e 7370 6c69 7428 227c 2229   line.split("|")
+00014c40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014c50: 2020 2020 2069 6620 6d6f 6465 2e73 7472       if mode.str
+00014c60: 6970 2829 2e75 7070 6572 2829 203d 3d20  ip().upper() == 
+00014c70: 2252 2220 616e 6420 7365 6c66 2e70 7265  "R" and self.pre
+00014c80: 662e 6765 7428 2272 756e 5f73 7461 7465  f.get("run_state
+00014c90: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
+00014ca0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00014cb0: 2e66 6b65 7973 5b66 6b65 792e 7374 7269  .fkeys[fkey.stri
+00014cc0: 7028 295d 203d 2028 6275 7474 6f6e 6e61  p()] = (buttonna
+00014cd0: 6d65 2e73 7472 6970 2829 2c20 6377 7465  me.strip(), cwte
+00014ce0: 7874 2e73 7472 6970 2829 290a 2020 2020  xt.strip()).    
+00014cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014d00: 6966 206d 6f64 652e 7374 7269 7028 292e  if mode.strip().
+00014d10: 7570 7065 7228 2920 213d 2022 5222 2061  upper() != "R" a
+00014d20: 6e64 206e 6f74 2073 656c 662e 7072 6566  nd not self.pref
+00014d30: 2e67 6574 2822 7275 6e5f 7374 6174 6522  .get("run_state"
+00014d40: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00014d50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00014d60: 666b 6579 735b 666b 6579 2e73 7472 6970  fkeys[fkey.strip
+00014d70: 2829 5d20 3d20 2862 7574 746f 6e6e 616d  ()] = (buttonnam
+00014d80: 652e 7374 7269 7028 292c 2063 7774 6578  e.strip(), cwtex
+00014d90: 742e 7374 7269 7028 2929 0a20 2020 2020  t.strip()).     
+00014da0: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+00014db0: 7420 5661 6c75 6545 7272 6f72 2061 7320  t ValueError as 
+00014dc0: 6572 723a 0a20 2020 2020 2020 2020 2020  err:.           
+00014dd0: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+00014de0: 696e 666f 2822 7265 6164 5f63 775f 6d61  info("read_cw_ma
+00014df0: 6372 6f73 3a20 2573 222c 2065 7272 290a  cros: %s", err).
+00014e00: 2020 2020 2020 2020 6b65 7973 203d 2073          keys = s
+00014e10: 656c 662e 666b 6579 732e 6b65 7973 2829  elf.fkeys.keys()
+00014e20: 0a20 2020 2020 2020 2069 6620 2246 3122  .        if "F1"
+00014e30: 2069 6e20 6b65 7973 3a0a 2020 2020 2020   in keys:.      
+00014e40: 2020 2020 2020 7365 6c66 2e46 312e 7365        self.F1.se
+00014e50: 7454 6578 7428 6622 4631 3a20 7b73 656c  tText(f"F1: {sel
+00014e60: 662e 666b 6579 735b 2746 3127 5d5b 305d  f.fkeys['F1'][0]
+00014e70: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
+00014e80: 7365 6c66 2e46 312e 7365 7454 6f6f 6c54  self.F1.setToolT
+00014e90: 6970 2873 656c 662e 666b 6579 735b 2246  ip(self.fkeys["F
+00014ea0: 3122 5d5b 315d 290a 2020 2020 2020 2020  1"][1]).        
+00014eb0: 6966 2022 4632 2220 696e 206b 6579 733a  if "F2" in keys:
+00014ec0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00014ed0: 662e 4632 2e73 6574 5465 7874 2866 2246  f.F2.setText(f"F
+00014ee0: 323a 207b 7365 6c66 2e66 6b65 7973 5b27  2: {self.fkeys['
+00014ef0: 4632 275d 5b30 5d7d 2229 0a20 2020 2020  F2'][0]}").     
+00014f00: 2020 2020 2020 2073 656c 662e 4632 2e73         self.F2.s
+00014f10: 6574 546f 6f6c 5469 7028 7365 6c66 2e66  etToolTip(self.f
+00014f20: 6b65 7973 5b22 4632 225d 5b31 5d29 0a20  keys["F2"][1]). 
+00014f30: 2020 2020 2020 2069 6620 2246 3322 2069         if "F3" i
+00014f40: 6e20 6b65 7973 3a0a 2020 2020 2020 2020  n keys:.        
+00014f50: 2020 2020 7365 6c66 2e46 332e 7365 7454      self.F3.setT
+00014f60: 6578 7428 6622 4633 3a20 7b73 656c 662e  ext(f"F3: {self.
+00014f70: 666b 6579 735b 2746 3327 5d5b 305d 7d22  fkeys['F3'][0]}"
+00014f80: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00014f90: 6c66 2e46 332e 7365 7454 6f6f 6c54 6970  lf.F3.setToolTip
+00014fa0: 2873 656c 662e 666b 6579 735b 2246 3322  (self.fkeys["F3"
+00014fb0: 5d5b 315d 290a 2020 2020 2020 2020 6966  ][1]).        if
+00014fc0: 2022 4634 2220 696e 206b 6579 733a 0a20   "F4" in keys:. 
+00014fd0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00014fe0: 4634 2e73 6574 5465 7874 2866 2246 343a  F4.setText(f"F4:
+00014ff0: 207b 7365 6c66 2e66 6b65 7973 5b27 4634   {self.fkeys['F4
+00015000: 275d 5b30 5d7d 2229 0a20 2020 2020 2020  '][0]}").       
+00015010: 2020 2020 2073 656c 662e 4634 2e73 6574       self.F4.set
+00015020: 546f 6f6c 5469 7028 7365 6c66 2e66 6b65  ToolTip(self.fke
+00015030: 7973 5b22 4634 225d 5b31 5d29 0a20 2020  ys["F4"][1]).   
+00015040: 2020 2020 2069 6620 2246 3522 2069 6e20       if "F5" in 
+00015050: 6b65 7973 3a0a 2020 2020 2020 2020 2020  keys:.          
+00015060: 2020 7365 6c66 2e46 352e 7365 7454 6578    self.F5.setTex
+00015070: 7428 6622 4635 3a20 7b73 656c 662e 666b  t(f"F5: {self.fk
+00015080: 6579 735b 2746 3527 5d5b 305d 7d22 290a  eys['F5'][0]}").
+00015090: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000150a0: 2e46 352e 7365 7454 6f6f 6c54 6970 2873  .F5.setToolTip(s
+000150b0: 656c 662e 666b 6579 735b 2246 3522 5d5b  elf.fkeys["F5"][
+000150c0: 315d 290a 2020 2020 2020 2020 6966 2022  1]).        if "
+000150d0: 4636 2220 696e 206b 6579 733a 0a20 2020  F6" in keys:.   
+000150e0: 2020 2020 2020 2020 2073 656c 662e 4636           self.F6
+000150f0: 2e73 6574 5465 7874 2866 2246 363a 207b  .setText(f"F6: {
+00015100: 7365 6c66 2e66 6b65 7973 5b27 4636 275d  self.fkeys['F6']
+00015110: 5b30 5d7d 2229 0a20 2020 2020 2020 2020  [0]}").         
+00015120: 2020 2073 656c 662e 4636 2e73 6574 546f     self.F6.setTo
+00015130: 6f6c 5469 7028 7365 6c66 2e66 6b65 7973  olTip(self.fkeys
+00015140: 5b22 4636 225d 5b31 5d29 0a20 2020 2020  ["F6"][1]).     
+00015150: 2020 2069 6620 2246 3722 2069 6e20 6b65     if "F7" in ke
+00015160: 7973 3a0a 2020 2020 2020 2020 2020 2020  ys:.            
+00015170: 7365 6c66 2e46 372e 7365 7454 6578 7428  self.F7.setText(
+00015180: 6622 4637 3a20 7b73 656c 662e 666b 6579  f"F7: {self.fkey
+00015190: 735b 2746 3727 5d5b 305d 7d22 290a 2020  s['F7'][0]}").  
+000151a0: 2020 2020 2020 2020 2020 7365 6c66 2e46            self.F
+000151b0: 372e 7365 7454 6f6f 6c54 6970 2873 656c  7.setToolTip(sel
+000151c0: 662e 666b 6579 735b 2246 3722 5d5b 315d  f.fkeys["F7"][1]
+000151d0: 290a 2020 2020 2020 2020 6966 2022 4638  ).        if "F8
+000151e0: 2220 696e 206b 6579 733a 0a20 2020 2020  " in keys:.     
+000151f0: 2020 2020 2020 2073 656c 662e 4638 2e73         self.F8.s
+00015200: 6574 5465 7874 2866 2246 383a 207b 7365  etText(f"F8: {se
+00015210: 6c66 2e66 6b65 7973 5b27 4638 275d 5b30  lf.fkeys['F8'][0
+00015220: 5d7d 2229 0a20 2020 2020 2020 2020 2020  ]}").           
+00015230: 2073 656c 662e 4638 2e73 6574 546f 6f6c   self.F8.setTool
+00015240: 5469 7028 7365 6c66 2e66 6b65 7973 5b22  Tip(self.fkeys["
+00015250: 4638 225d 5b31 5d29 0a20 2020 2020 2020  F8"][1]).       
+00015260: 2069 6620 2246 3922 2069 6e20 6b65 7973   if "F9" in keys
+00015270: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00015280: 6c66 2e46 392e 7365 7454 6578 7428 6622  lf.F9.setText(f"
+00015290: 4639 3a20 7b73 656c 662e 666b 6579 735b  F9: {self.fkeys[
+000152a0: 2746 3927 5d5b 305d 7d22 290a 2020 2020  'F9'][0]}").    
+000152b0: 2020 2020 2020 2020 7365 6c66 2e46 392e          self.F9.
+000152c0: 7365 7454 6f6f 6c54 6970 2873 656c 662e  setToolTip(self.
+000152d0: 666b 6579 735b 2246 3922 5d5b 315d 290a  fkeys["F9"][1]).
+000152e0: 2020 2020 2020 2020 6966 2022 4631 3022          if "F10"
+000152f0: 2069 6e20 6b65 7973 3a0a 2020 2020 2020   in keys:.      
+00015300: 2020 2020 2020 7365 6c66 2e46 3130 2e73        self.F10.s
+00015310: 6574 5465 7874 2866 2246 3130 3a20 7b73  etText(f"F10: {s
+00015320: 656c 662e 666b 6579 735b 2746 3130 275d  elf.fkeys['F10']
+00015330: 5b30 5d7d 2229 0a20 2020 2020 2020 2020  [0]}").         
+00015340: 2020 2073 656c 662e 4631 302e 7365 7454     self.F10.setT
+00015350: 6f6f 6c54 6970 2873 656c 662e 666b 6579  oolTip(self.fkey
+00015360: 735b 2246 3130 225d 5b31 5d29 0a20 2020  s["F10"][1]).   
+00015370: 2020 2020 2069 6620 2246 3131 2220 696e       if "F11" in
+00015380: 206b 6579 733a 0a20 2020 2020 2020 2020   keys:.         
+00015390: 2020 2073 656c 662e 4631 312e 7365 7454     self.F11.setT
+000153a0: 6578 7428 6622 4631 313a 207b 7365 6c66  ext(f"F11: {self
+000153b0: 2e66 6b65 7973 5b27 4631 3127 5d5b 305d  .fkeys['F11'][0]
+000153c0: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
+000153d0: 7365 6c66 2e46 3131 2e73 6574 546f 6f6c  self.F11.setTool
+000153e0: 5469 7028 7365 6c66 2e66 6b65 7973 5b22  Tip(self.fkeys["
+000153f0: 4631 3122 5d5b 315d 290a 2020 2020 2020  F11"][1]).      
+00015400: 2020 6966 2022 4631 3222 2069 6e20 6b65    if "F12" in ke
+00015410: 7973 3a0a 2020 2020 2020 2020 2020 2020  ys:.            
+00015420: 7365 6c66 2e46 3132 2e73 6574 5465 7874  self.F12.setText
+00015430: 2866 2246 3132 3a20 7b73 656c 662e 666b  (f"F12: {self.fk
+00015440: 6579 735b 2746 3132 275d 5b30 5d7d 2229  eys['F12'][0]}")
+00015450: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00015460: 662e 4631 322e 7365 7454 6f6f 6c54 6970  f.F12.setToolTip
+00015470: 2873 656c 662e 666b 6579 735b 2246 3132  (self.fkeys["F12
+00015480: 225d 5b31 5d29 0a0a 2020 2020 6465 6620  "][1])..    def 
+00015490: 6765 6e65 7261 7465 5f61 6469 6628 7365  generate_adif(se
+000154a0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+000154b0: 4765 6e65 7261 7465 2041 4449 4622 2222  Generate ADIF"""
+000154c0: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
+000154d0: 6465 6275 6728 222a 2a2a 2a2a 2a41 4449  debug("******ADI
+000154e0: 462a 2a2a 2a2a 2229 0a20 2020 2020 2020  F*****").       
+000154f0: 2073 656c 662e 636f 6e74 6573 742e 6164   self.contest.ad
+00015500: 6966 2873 656c 6629 0a0a 2020 2020 6465  if(self)..    de
+00015510: 6620 6765 6e65 7261 7465 5f63 6162 7269  f generate_cabri
+00015520: 6c6c 6f28 7365 6c66 293a 0a20 2020 2020  llo(self):.     
+00015530: 2020 2022 2222 4765 6e65 7261 7465 7320     """Generates 
+00015540: 4361 6272 696c 6c6f 2066 696c 652e 204d  Cabrillo file. M
+00015550: 6179 6265 2e22 2222 0a20 2020 2020 2020  aybe.""".       
+00015560: 2023 2068 7474 7073 3a2f 2f77 7777 2e63   # https://www.c
+00015570: 7177 7078 2e63 6f6d 2f63 6162 7269 6c6c  qwpx.com/cabrill
+00015580: 6f2e 6874 6d0a 2020 2020 2020 2020 6c6f  o.htm.        lo
+00015590: 6767 6572 2e64 6562 7567 2822 2a2a 2a2a  gger.debug("****
+000155a0: 2a2a 4361 6272 696c 6c6f 2a2a 2a2a 2a22  **Cabrillo*****"
+000155b0: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
+000155c0: 6f6e 7465 7374 2e63 6162 7269 6c6c 6f28  ontest.cabrillo(
+000155d0: 7365 6c66 290a 0a0a 6465 6620 6c6f 6164  self)...def load
+000155e0: 5f66 6f6e 7473 5f66 726f 6d5f 6469 7228  _fonts_from_dir(
+000155f0: 6469 7265 6374 6f72 793a 2073 7472 2920  directory: str) 
+00015600: 2d3e 2073 6574 3a0a 2020 2020 2222 220a  -> set:.    """.
+00015610: 2020 2020 5765 6c6c 2069 7420 6c6f 6164      Well it load
+00015620: 7320 666f 6e74 7320 6672 6f6d 2061 2064  s fonts from a d
+00015630: 6972 6563 746f 7279 2e2e 2e0a 2020 2020  irectory....    
+00015640: 2222 220a 2020 2020 666f 6e74 5f66 616d  """.    font_fam
+00015650: 696c 6965 7320 3d20 7365 7428 290a 2020  ilies = set().  
+00015660: 2020 666f 7220 5f66 6920 696e 2051 4469    for _fi in QDi
+00015670: 7228 6469 7265 6374 6f72 7929 2e65 6e74  r(directory).ent
+00015680: 7279 496e 666f 4c69 7374 285b 222a 2e74  ryInfoList(["*.t
+00015690: 7466 222c 2022 2a2e 776f 6666 222c 2022  tf", "*.woff", "
+000156a0: 2a2e 776f 6666 3222 5d29 3a0a 2020 2020  *.woff2"]):.    
+000156b0: 2020 2020 5f69 6420 3d20 5146 6f6e 7444      _id = QFontD
+000156c0: 6174 6162 6173 652e 6164 6441 7070 6c69  atabase.addAppli
+000156d0: 6361 7469 6f6e 466f 6e74 285f 6669 2e61  cationFont(_fi.a
+000156e0: 6273 6f6c 7574 6546 696c 6550 6174 6828  bsoluteFilePath(
+000156f0: 2929 0a20 2020 2020 2020 2066 6f6e 745f  )).        font_
+00015700: 6661 6d69 6c69 6573 207c 3d20 7365 7428  families |= set(
+00015710: 5146 6f6e 7444 6174 6162 6173 652e 6170  QFontDatabase.ap
+00015720: 706c 6963 6174 696f 6e46 6f6e 7446 616d  plicationFontFam
+00015730: 696c 6965 7328 5f69 6429 290a 2020 2020  ilies(_id)).    
+00015740: 7265 7475 726e 2066 6f6e 745f 6661 6d69  return font_fami
+00015750: 6c69 6573 0a0a 0a64 6566 2069 6e73 7461  lies...def insta
+00015760: 6c6c 5f69 636f 6e73 2829 3a0a 2020 2020  ll_icons():.    
+00015770: 2222 2249 6e73 7461 6c6c 2069 636f 6e73  """Install icons
+00015780: 2222 220a 2020 2020 6f73 2e73 7973 7465  """.    os.syste
+00015790: 6d28 0a20 2020 2020 2020 2022 7864 672d  m(.        "xdg-
+000157a0: 6963 6f6e 2d72 6573 6f75 7263 6520 696e  icon-resource in
+000157b0: 7374 616c 6c20 2d2d 7369 7a65 2033 3220  stall --size 32 
+000157c0: 2d2d 636f 6e74 6578 7420 6170 7073 202d  --context apps -
+000157d0: 2d6d 6f64 6520 7573 6572 2022 0a20 2020  -mode user ".   
+000157e0: 2020 2020 2066 227b 574f 524b 494e 475f       f"{WORKING_
+000157f0: 5041 5448 7d2f 6461 7461 2f6b 3667 7465  PATH}/data/k6gte
+00015800: 2e6e 6f74 316d 6d2d 3332 2e70 6e67 206b  .not1mm-32.png k
+00015810: 3667 7465 2d6e 6f74 316d 6d22 0a20 2020  6gte-not1mm".   
+00015820: 2029 0a20 2020 206f 732e 7379 7374 656d   ).    os.system
+00015830: 280a 2020 2020 2020 2020 2278 6467 2d69  (.        "xdg-i
+00015840: 636f 6e2d 7265 736f 7572 6365 2069 6e73  con-resource ins
+00015850: 7461 6c6c 202d 2d73 697a 6520 3634 202d  tall --size 64 -
+00015860: 2d63 6f6e 7465 7874 2061 7070 7320 2d2d  -context apps --
+00015870: 6d6f 6465 2075 7365 7220 220a 2020 2020  mode user ".    
+00015880: 2020 2020 6622 7b57 4f52 4b49 4e47 5f50      f"{WORKING_P
+00015890: 4154 487d 2f64 6174 612f 6b36 6774 652e  ATH}/data/k6gte.
+000158a0: 6e6f 7431 6d6d 2d36 342e 706e 6720 6b36  not1mm-64.png k6
+000158b0: 6774 652d 6e6f 7431 6d6d 220a 2020 2020  gte-not1mm".    
+000158c0: 290a 2020 2020 6f73 2e73 7973 7465 6d28  ).    os.system(
+000158d0: 0a20 2020 2020 2020 2022 7864 672d 6963  .        "xdg-ic
+000158e0: 6f6e 2d72 6573 6f75 7263 6520 696e 7374  on-resource inst
+000158f0: 616c 6c20 2d2d 7369 7a65 2031 3238 202d  all --size 128 -
+00015900: 2d63 6f6e 7465 7874 2061 7070 7320 2d2d  -context apps --
+00015910: 6d6f 6465 2075 7365 7220 220a 2020 2020  mode user ".    
+00015920: 2020 2020 6622 7b57 4f52 4b49 4e47 5f50      f"{WORKING_P
+00015930: 4154 487d 2f64 6174 612f 6b36 6774 652e  ATH}/data/k6gte.
+00015940: 6e6f 7431 6d6d 2d31 3238 2e70 6e67 206b  not1mm-128.png k
+00015950: 3667 7465 2d6e 6f74 316d 6d22 0a20 2020  6gte-not1mm".   
+00015960: 2029 0a20 2020 206f 732e 7379 7374 656d   ).    os.system
+00015970: 2866 2278 6467 2d64 6573 6b74 6f70 2d6d  (f"xdg-desktop-m
+00015980: 656e 7520 696e 7374 616c 6c20 7b57 4f52  enu install {WOR
+00015990: 4b49 4e47 5f50 4154 487d 2f64 6174 612f  KING_PATH}/data/
+000159a0: 6b36 6774 652d 6e6f 7431 6d6d 2e64 6573  k6gte-not1mm.des
+000159b0: 6b74 6f70 2229 0a0a 0a64 6566 2064 6f69  ktop")...def doi
+000159c0: 6d70 286d 6f64 6e61 6d65 293a 0a20 2020  mp(modname):.   
+000159d0: 2022 2222 7265 7475 726e 206d 6f64 756c   """return modul
+000159e0: 6520 7061 7468 2222 220a 2020 2020 7265  e path""".    re
+000159f0: 7475 726e 2069 6d70 6f72 746c 6962 2e69  turn importlib.i
+00015a00: 6d70 6f72 745f 6d6f 6475 6c65 2866 226e  mport_module(f"n
+00015a10: 6f74 316d 6d2e 706c 7567 696e 732e 7b6d  ot1mm.plugins.{m
+00015a20: 6f64 6e61 6d65 7d22 290a 0a0a 6465 6620  odname}")...def 
+00015a30: 7275 6e28 293a 0a20 2020 2022 2222 0a20  run():.    """. 
+00015a40: 2020 204d 6169 6e20 456e 7472 790a 2020     Main Entry.  
+00015a50: 2020 2222 220a 2020 2020 696e 7374 616c    """.    instal
+00015a60: 6c5f 6963 6f6e 7328 290a 2020 2020 7469  l_icons().    ti
+00015a70: 6d65 722e 7374 6172 7428 3235 3029 0a20  mer.start(250). 
+00015a80: 2020 2073 7973 2e65 7869 7428 6170 702e     sys.exit(app.
+00015a90: 6578 6563 2829 290a 0a0a 6c6f 6767 6572  exec())...logger
+00015aa0: 203d 206c 6f67 6769 6e67 2e67 6574 4c6f   = logging.getLo
+00015ab0: 6767 6572 2822 5f5f 6d61 696e 5f5f 2229  gger("__main__")
+00015ac0: 0a68 616e 646c 6572 203d 206c 6f67 6769  .handler = loggi
+00015ad0: 6e67 2e53 7472 6561 6d48 616e 646c 6572  ng.StreamHandler
+00015ae0: 2829 0a66 6f72 6d61 7474 6572 203d 206c  ().formatter = l
+00015af0: 6f67 6769 6e67 2e46 6f72 6d61 7474 6572  ogging.Formatter
+00015b00: 280a 2020 2020 6461 7465 666d 743d 2225  (.    datefmt="%
+00015b10: 483a 254d 3a25 5322 2c0a 2020 2020 666d  H:%M:%S",.    fm
+00015b20: 743d 225b 2528 6173 6374 696d 6529 735d  t="[%(asctime)s]
+00015b30: 2025 286c 6576 656c 6e61 6d65 2973 2025   %(levelname)s %
+00015b40: 286d 6f64 756c 6529 7320 2d20 2528 6675  (module)s - %(fu
+00015b50: 6e63 4e61 6d65 2973 204c 696e 6520 2528  ncName)s Line %(
+00015b60: 6c69 6e65 6e6f 2964 3a20 2528 6d65 7373  lineno)d: %(mess
+00015b70: 6167 6529 7322 2c0a 290a 6861 6e64 6c65  age)s",.).handle
+00015b80: 722e 7365 7446 6f72 6d61 7474 6572 2866  r.setFormatter(f
+00015b90: 6f72 6d61 7474 6572 290a 6c6f 6767 6572  ormatter).logger
+00015ba0: 2e61 6464 4861 6e64 6c65 7228 6861 6e64  .addHandler(hand
+00015bb0: 6c65 7229 0a0a 4245 5441 5f54 4553 5420  ler)..BETA_TEST 
+00015bc0: 3d20 4661 6c73 650a 6966 2050 6174 6828  = False.if Path(
+00015bd0: 222e 2f62 6574 6174 6573 7422 292e 6578  "./betatest").ex
+00015be0: 6973 7473 2829 3a0a 2020 2020 4245 5441  ists():.    BETA
+00015bf0: 5f54 4553 5420 3d20 5472 7565 0a0a 6966  _TEST = True..if
+00015c00: 2050 6174 6828 222e 2f64 6562 7567 2229   Path("./debug")
+00015c10: 2e65 7869 7374 7328 293a 0a20 2020 206c  .exists():.    l
+00015c20: 6f67 6765 722e 7365 744c 6576 656c 286c  ogger.setLevel(l
+00015c30: 6f67 6769 6e67 2e44 4542 5547 290a 2020  ogging.DEBUG).  
+00015c40: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
+00015c50: 6465 6275 6767 696e 6720 6f6e 2229 0a65  debugging on").e
+00015c60: 6c73 653a 0a20 2020 206c 6f67 6765 722e  lse:.    logger.
+00015c70: 7365 744c 6576 656c 286c 6f67 6769 6e67  setLevel(logging
+00015c80: 2e57 4152 4e49 4e47 290a 2020 2020 6c6f  .WARNING).    lo
+00015c90: 6767 6572 2e77 6172 6e69 6e67 2822 6465  gger.warning("de
+00015ca0: 6275 6767 696e 6720 6f66 6622 290a 0a61  bugging off")..a
+00015cb0: 7070 203d 2051 7457 6964 6765 7473 2e51  pp = QtWidgets.Q
+00015cc0: 4170 706c 6963 6174 696f 6e28 7379 732e  Application(sys.
+00015cd0: 6172 6776 290a 6170 702e 7365 7453 7479  argv).app.setSty
+00015ce0: 6c65 2822 4164 7761 6974 612d 4461 726b  le("Adwaita-Dark
+00015cf0: 2229 0a66 6f6e 745f 7061 7468 203d 2057  ").font_path = W
+00015d00: 4f52 4b49 4e47 5f50 4154 4820 2b20 222f  ORKING_PATH + "/
+00015d10: 6461 7461 220a 6661 6d69 6c69 6573 203d  data".families =
+00015d20: 206c 6f61 645f 666f 6e74 735f 6672 6f6d   load_fonts_from
+00015d30: 5f64 6972 286f 732e 6673 7061 7468 2866  _dir(os.fspath(f
+00015d40: 6f6e 745f 7061 7468 2929 0a6c 6f67 6765  ont_path)).logge
+00015d50: 722e 696e 666f 2866 616d 696c 6965 7329  r.info(families)
+00015d60: 0a77 696e 646f 7720 3d20 4d61 696e 5769  .window = MainWi
+00015d70: 6e64 6f77 2829 0a68 6569 6768 7420 3d20  ndow().height = 
+00015d80: 7769 6e64 6f77 2e70 7265 662e 6765 7428  window.pref.get(
+00015d90: 2277 696e 646f 775f 6865 6967 6874 222c  "window_height",
+00015da0: 2033 3030 290a 7769 6474 6820 3d20 7769   300).width = wi
+00015db0: 6e64 6f77 2e70 7265 662e 6765 7428 2277  ndow.pref.get("w
+00015dc0: 696e 646f 775f 7769 6474 6822 2c20 3730  indow_width", 70
+00015dd0: 3029 0a78 203d 2077 696e 646f 772e 7072  0).x = window.pr
+00015de0: 6566 2e67 6574 2822 7769 6e64 6f77 5f78  ef.get("window_x
+00015df0: 222c 202d 3129 0a79 203d 2077 696e 646f  ", -1).y = windo
+00015e00: 772e 7072 6566 2e67 6574 2822 7769 6e64  w.pref.get("wind
+00015e10: 6f77 5f79 222c 202d 3129 0a77 696e 646f  ow_y", -1).windo
+00015e20: 772e 7365 7447 656f 6d65 7472 7928 782c  w.setGeometry(x,
+00015e30: 2079 2c20 7769 6474 682c 2068 6569 6768   y, width, heigh
+00015e40: 7429 0a77 696e 646f 772e 6361 6c6c 7369  t).window.callsi
+00015e50: 676e 2e73 6574 466f 6375 7328 290a 7769  gn.setFocus().wi
+00015e60: 6e64 6f77 2e73 686f 7728 290a 7469 6d65  ndow.show().time
+00015e70: 7220 3d20 5174 436f 7265 2e51 5469 6d65  r = QtCore.QTime
+00015e80: 7228 290a 7469 6d65 722e 7469 6d65 6f75  r().timer.timeou
+00015e90: 742e 636f 6e6e 6563 7428 7769 6e64 6f77  t.connect(window
+00015ea0: 2e70 6f6c 6c5f 7261 6469 6f29 0a0a 6966  .poll_radio)..if
+00015eb0: 205f 5f6e 616d 655f 5f20 3d3d 2022 5f5f   __name__ == "__
+00015ec0: 6d61 696e 5f5f 223a 0a20 2020 2072 756e  main__":.    run
+00015ed0: 2829 0a                                  ().
```

### Comparing `not1mm-23.5.9.2/not1mm/bandmap.py` & `not1mm-23.6.2/not1mm/bandmap.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 Email: michael.bridak@gmail.com
 GPL V3
 """
 
 # pylint: disable=unused-import, c-extension-no-member, no-member, invalid-name, too-many-lines
 
 from datetime import datetime
+from decimal import Decimal
 from json import JSONDecodeError, loads, dumps
 from pathlib import Path
 
 import logging
 import os
 import pkgutil
 import platform
@@ -42,59 +43,37 @@
     CONFIG_PATH = os.environ.get("XDG_CONFIG_HOME")
 else:
     CONFIG_PATH = str(Path.home() / ".config")
 CONFIG_PATH += "/not1mm"
 
 DARK_STYLESHEET = ""
 
-with open(WORKING_PATH + "/data/Combinear.qss", encoding="utf-8") as stylefile:
-    DARK_STYLESHEET = stylefile.read()
-
 MULTICAST_PORT = 2239
-MULTICAST_GROUP = "224.1.1.1"
+MULTICAST_GROUP = "239.1.1.1"
 INTERFACE_IP = "0.0.0.0"
 
 PREF = {}
 if os.path.exists(CONFIG_PATH + "/not1mm.json"):
     with open(CONFIG_PATH + "/not1mm.json", "rt", encoding="utf-8") as file_descriptor:
         PREF = loads(file_descriptor.read())
 
 
-# CTYFILE = {}
-
-# with open(WORKING_PATH + "/data/cty.json", "rt", encoding="utf-8") as c_file:
-#     CTYFILE = loads(c_file.read())
-
-
-# def cty_lookup(callsign: str):
-#     """Lookup callsign in cty.dat file"""
-#     callsign = callsign.upper()
-#     for count in reversed(range(len(callsign))):
-#         searchitem = callsign[: count + 1]
-#         result = {key: val for key, val in CTYFILE.items() if key == searchitem}
-#         if not result:
-#             continue
-#         if result.get(searchitem).get("exact_match"):
-#             if searchitem == callsign:
-#                 return result
-#             continue
-#         return result
-
-
 class Band:
     """the band"""
 
     bands = {
         "160m": (1.8, 2),
         "80m": (3.5, 4),
         "60m": (5.102, 5.4065),
         "40m": (7.0, 7.3),
         "30m": (10.1, 10.15),
         "20m": (14.0, 14.35),
+        "17m": (18.069, 18.168),
         "15m": (21.0, 21.45),
+        "12m": (24.89, 25.0),
         "10m": (28.0, 29.7),
         "6m": (50.0, 54.0),
         "4m": (70.0, 71.0),
         "2m": (144.0, 148.0),
     }
 
     def __init__(self, band: str) -> None:
@@ -155,15 +134,15 @@
                 values.append(spot[key])
                 placeholders += "?,"
             post = f") VALUES({placeholders[:-1]});"
 
             sql = f"{pre}{columns[:-1]}{post}"
             self.cursor.execute(sql, tuple(values))
             self.db.commit()
-        except:
+        except sqlite3.IntegrityError:
             ...
 
     def getspots(self) -> list:
         """returns a list of dicts."""
         try:
             self.cursor.execute("select * from spots order by freq ASC;")
             return self.cursor.fetchall()
@@ -180,14 +159,21 @@
     def get_next_spot(self, current: float, limit: float) -> dict:
         """ "return a list of dict where freq range is defined"""
         self.cursor.execute(
             f"select * from spots where freq > {current} and freq <= {limit} order by freq ASC;"
         )
         return self.cursor.fetchone()
 
+    def get_matching_spot(self, dx: str, start: float, end: float) -> dict:
+        """Return the first spot matching supplied dx partial call"""
+        self.cursor.execute(
+            f"select * from spots where freq >= {start} and freq <= {end} and callsign like '%{dx}%';"
+        )
+        return self.cursor.fetchone()
+
     def get_prev_spot(self, current: float, limit: float) -> dict:
         """ "return a list of dict where freq range is defined"""
         self.cursor.execute(
             f"select * from spots where freq < {current} and freq >= {limit} order by freq DESC;"
         )
         return self.cursor.fetchone()
 
@@ -259,14 +245,19 @@
         """doc"""
         if self.connected is True:
             self.socket.close()
             self.connected = False
             self.connectButton.setStyleSheet("color: red;")
             self.connectButton.setText("Closed")
             return
+        if os.path.exists(CONFIG_PATH + "/not1mm.json"):
+            with open(
+                CONFIG_PATH + "/not1mm.json", "rt", encoding="utf-8"
+            ) as _file_descriptor:
+                globals()["PREF"] = loads(_file_descriptor.read())
         server = PREF.get("cluster_server", "dxc.nc7j.com")
         port = PREF.get("cluster_port", 7373)
         self.socket.connectToHost(server, port)
         self.connectButton.setStyleSheet("color: white;")
         self.connectButton.setText("Connecting")
         self.connected = True
 
@@ -287,22 +278,27 @@
                 logger.debug(the_error)
                 continue
             if (
                 packet.get("cmd", "") == "RADIO_STATE"
                 and packet.get("station", "") == platform.node()
             ):
                 self.set_band(packet.get("band") + "m", False)
-                self.rx_freq = float(packet.get("vfoa")) / 1000000
-                self.tx_freq = self.rx_freq
+                if self.rx_freq != float(packet.get("vfoa")) / 1000000:
+                    self.rx_freq = float(packet.get("vfoa")) / 1000000
+                    self.tx_freq = self.rx_freq
+                    self.center_on_rxfreq()
                 self.bandwidth = int(packet.get("bw", "0"))
                 step, _ = self.determine_step_digits()
                 self.drawTXRXMarks(step)
+                continue
+
             if (
                 packet.get("cmd", "") == "NEXTSPOT"
                 and packet.get("station", "") == platform.node()
+                and self.rx_freq
             ):
                 spot = self.spots.get_next_spot(
                     self.rx_freq + 0.000001, self.currentBand.end
                 )
                 if spot:
                     cmd = {}
                     cmd["cmd"] = "TUNE"
@@ -314,14 +310,15 @@
                         packet, QtNetwork.QHostAddress(MULTICAST_GROUP), MULTICAST_PORT
                     )
                 continue
 
             if (
                 packet.get("cmd", "") == "PREVSPOT"
                 and packet.get("station", "") == platform.node()
+                and self.rx_freq
             ):
                 spot = self.spots.get_prev_spot(
                     self.rx_freq - 0.000001, self.currentBand.start
                 )
                 if spot:
                     cmd = {}
                     cmd["cmd"] = "TUNE"
@@ -329,14 +326,41 @@
                     cmd["freq"] = spot.get("freq", self.rx_freq)
                     cmd["spot"] = spot.get("callsign", "")
                     packet = bytes(dumps(cmd), encoding="ascii")
                     self.udpsocket.writeDatagram(
                         packet, QtNetwork.QHostAddress(MULTICAST_GROUP), MULTICAST_PORT
                     )
                 continue
+            if (
+                packet.get("cmd", "") == "SPOTDX"
+                and packet.get("station", "") == platform.node()
+            ):
+                dx = packet.get("dx", "")
+                freq = packet.get("freq", 0.0)
+                spotdx = f"dx {dx} {freq}"
+                self.send_command(spotdx)
+                continue
+            if (
+                packet.get("cmd", "") == "FINDDX"
+                and packet.get("station", "") == platform.node()
+            ):
+                dx = packet.get("dx", "")
+                spot = self.spots.get_matching_spot(
+                    dx, self.currentBand.start, self.currentBand.end
+                )
+                if spot:
+                    cmd = {}
+                    cmd["cmd"] = "TUNE"
+                    cmd["station"] = platform.node()
+                    cmd["freq"] = spot.get("freq", self.rx_freq)
+                    cmd["spot"] = spot.get("callsign", "")
+                    packet = bytes(dumps(cmd), encoding="ascii")
+                    self.udpsocket.writeDatagram(
+                        packet, QtNetwork.QHostAddress(MULTICAST_GROUP), MULTICAST_PORT
+                    )
 
     def spot_clicked(self):
         """dunno"""
         items = self.bandmap_scene.selectedItems()
         for item in items:
             if item:
                 cmd = {}
@@ -423,34 +447,42 @@
 
     def Freq2ScenePos(self, freq: float):
         """doc"""
         if freq < self.currentBand.start or freq > self.currentBand.end:
             return QtCore.QPointF()
         step, _digits = self.determine_step_digits()
         ret = QtCore.QPointF(
-            0, ((freq - self.currentBand.start) / step) * PIXELSPERSTEP
+            0,
+            (
+                (Decimal(str(freq)) - Decimal(str(self.currentBand.start)))
+                / Decimal(str(step))
+            )
+            * PIXELSPERSTEP,
         )
         return ret
 
     def center_on_rxfreq(self):
         """doc"""
         freq_pos = self.Freq2ScenePos(self.rx_freq).y()
+        # self.graphicsView.verticalScrollBar().setSliderPosition(
+        #     int(freq_pos - (self.height() / 2) + 80)
+        # )
         self.scrollArea.verticalScrollBar().setValue(
             int(freq_pos - (self.height() / 2) + 80)
         )
         # This does not work... Have no idea why.
         # anim = QtCore.QPropertyAnimation(
         #     self.scrollArea.verticalScrollBar(), "value".encode()
         # )
         # anim.setDuration(300)
         # anim.setStartValue(self.scrollArea.verticalScrollBar().value())
         # anim.setEndValue(int(freq_pos - (self.height() / 2) + 80))
         # anim.start(QtCore.QAbstractAnimation.DeletionPolicy.DeleteWhenStopped)
 
-    def drawfreqmark(self, freq, step, color, currentPolygon):
+    def drawfreqmark(self, freq, _step, color, currentPolygon):
         """doc"""
 
         self.clear_freq_mark(currentPolygon)
         # do not show the freq mark if it is outside the bandmap
         if freq < self.currentBand.start or freq > self.currentBand.end:
             return
 
@@ -461,24 +493,26 @@
         poly.append(QtCore.QPointF(21, Yposition))
         poly.append(QtCore.QPointF(10, Yposition - 7))
         poly.append(QtCore.QPointF(10, Yposition + 7))
         pen = QtGui.QPen()
         brush = QtGui.QBrush(color)
         currentPolygon.append(self.bandmap_scene.addPolygon(poly, pen, brush))
 
-    def draw_bandwidth(self, freq, step, color, currentPolygon):
+    def draw_bandwidth(self, freq, _step, color, currentPolygon):
         """bandwidth"""
         logger.debug("%s", f"mark:{currentPolygon} f:{freq} b:{self.bandwidth}")
         self.clear_freq_mark(currentPolygon)
         if freq < self.currentBand.start or freq > self.currentBand.end:
             return
         if freq and self.bandwidth:
             # color = QtGui.QColor(30, 30, 180)
-            bw_start = freq - ((self.bandwidth / 2) / 1000000)
-            bw_end = freq + ((self.bandwidth / 2) / 1000000)
+            bw_start = Decimal(str(freq)) - (
+                (Decimal(str(self.bandwidth)) / 2) / 1000000
+            )
+            bw_end = Decimal(str(freq)) + ((Decimal(str(self.bandwidth)) / 2) / 1000000)
             logger.debug("%s", f"s:{bw_start} e:{bw_end}")
             Yposition_neg = self.Freq2ScenePos(bw_start).y()
             Yposition_pos = self.Freq2ScenePos(bw_end).y()
             poly = QtGui.QPolygonF()
             poly.append(QtCore.QPointF(15, Yposition_neg))
             poly.append(QtCore.QPointF(20, Yposition_neg))
             poly.append(QtCore.QPointF(20, Yposition_pos))
@@ -527,15 +561,16 @@
                     | text.flags()
                 )
                 text.setProperty("freq", items.get("freq"))
                 text.setToolTip(items.get("comment"))
 
                 min_y = text_y + text.boundingRect().height() / 2
 
-                # textColor = Data::statusToColor(lower.value().status, qApp->palette().color(QPalette::Text));
+                # textColor = Data::statusToColor(lower.value().status,
+                # qApp->palette().color(QPalette::Text));
                 # text->setDefaultTextColor(textColor);
                 self.textItemList.append(text)
 
     def determine_step_digits(self):
         """doc"""
         return_zoom = {
             1: (0.0001, 4),
@@ -684,12 +719,12 @@
 else:
     logger.setLevel(logging.WARNING)
     logger.warning("debugging off")
 
 app = QtWidgets.QApplication(sys.argv)
 
 
-# app.setStyle("Fusion")
+app.setStyle("Adwaita-Dark")
 window = MainWindow()
 window.show()
 if __name__ == "__main__":
     run()
```

### Comparing `not1mm-23.5.9.2/not1mm/data/JetBrainsMono-Regular.ttf` & `not1mm-23.6.2/not1mm/data/JetBrainsMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/MASTER.SCP` & `not1mm-23.6.2/not1mm/data/MASTER.SCP`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/about.ui` & `not1mm-23.6.2/not1mm/data/about.ui`

 * *Files 2% similar despite different names*

#### Comparing `not1mm-23.5.9.2/not1mm/data/about.ui` & `not1mm-23.6.2/not1mm/data/about.ui`

```diff
@@ -3,15 +3,15 @@
   <class>Dialog</class>
   <widget class="QDialog" name="Dialog">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
         <width>345</width>
-        <height>176</height>
+        <height>376</height>
       </rect>
     </property>
     <property name="windowTitle">
       <string>About</string>
     </property>
     <layout class="QGridLayout" name="gridLayout">
       <item row="0" column="0">
@@ -29,42 +29,30 @@
             <string>Not1MM</string>
           </property>
           <property name="alignment">
             <set>Qt::AlignCenter</set>
           </property>
         </widget>
       </item>
-      <item row="1" column="0">
-        <widget class="QLabel" name="label_2">
-          <property name="font">
-            <font>
-              <family>JetBrains Mono</family>
-            </font>
-          </property>
-          <property name="text">
-            <string>You're Welcome</string>
-          </property>
-          <property name="alignment">
-            <set>Qt::AlignCenter</set>
-          </property>
-        </widget>
-      </item>
       <item row="2" column="0">
         <widget class="QDialogButtonBox" name="buttonBox">
           <property name="orientation">
             <enum>Qt::Horizontal</enum>
           </property>
           <property name="standardButtons">
             <set>QDialogButtonBox::Close</set>
           </property>
           <property name="centerButtons">
             <bool>true</bool>
           </property>
         </widget>
       </item>
+      <item row="1" column="0">
+        <widget class="QTextBrowser" name="donors"/>
+      </item>
     </layout>
   </widget>
   <resources/>
   <connections>
     <connection>
       <sender>buttonBox</sender>
       <signal>accepted()</signal>
```

### Comparing `not1mm-23.5.9.2/not1mm/data/bandmap.ui` & `not1mm-23.6.2/not1mm/data/bandmap.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/configuration.ui` & `not1mm-23.6.2/not1mm/data/configuration.ui`

 * *Files 4% similar despite different names*

#### Comparing `not1mm-23.5.9.2/not1mm/data/configuration.ui` & `not1mm-23.6.2/not1mm/data/configuration.ui`

```diff
@@ -2,15 +2,15 @@
 <ui version="4.0">
   <class>Dialog</class>
   <widget class="QDialog" name="Dialog">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
-        <width>512</width>
+        <width>636</width>
         <height>395</height>
       </rect>
     </property>
     <property name="font">
       <font>
         <family>JetBrains Mono</family>
       </font>
@@ -18,15 +18,15 @@
     <property name="windowTitle">
       <string>Configuration Settings</string>
     </property>
     <property name="styleSheet">
       <string notr="true"/>
     </property>
     <layout class="QGridLayout" name="gridLayout">
-      <item row="1" column="1" alignment="Qt::AlignHCenter">
+      <item row="2" column="1" alignment="Qt::AlignHCenter">
         <widget class="QDialogButtonBox" name="buttonBox">
           <property name="sizePolicy">
             <sizepolicy hsizetype="Maximum" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
@@ -47,15 +47,15 @@
             <set>QDialogButtonBox::Cancel|QDialogButtonBox::Save</set>
           </property>
           <property name="centerButtons">
             <bool>true</bool>
           </property>
         </widget>
       </item>
-      <item row="0" column="1">
+      <item row="1" column="1">
         <widget class="QTabWidget" name="tabWidget">
           <property name="enabled">
             <bool>true</bool>
           </property>
           <property name="font">
             <font>
               <family>JetBrains Mono</family>
@@ -995,188 +995,227 @@
                   </property>
                 </widget>
               </item>
             </layout>
           </widget>
           <widget class="QWidget" name="n1mm_tab">
             <property name="enabled">
-              <bool>false</bool>
+              <bool>true</bool>
             </property>
             <property name="font">
               <font>
                 <family>JetBrains Mono</family>
                 <pointsize>12</pointsize>
                 <strikeout>false</strikeout>
               </font>
             </property>
             <attribute name="title">
               <string>N1MM</string>
             </attribute>
             <layout class="QGridLayout" name="gridLayout_8">
-              <item row="1" column="0">
-                <widget class="QLabel" name="label_13">
+              <item row="1" column="5">
+                <widget class="QLabel" name="label_14">
                   <property name="font">
                     <font>
                       <family>JetBrains Mono</family>
                       <pointsize>12</pointsize>
                       <strikeout>false</strikeout>
                     </font>
                   </property>
                   <property name="text">
-                    <string>Station Name:</string>
+                    <string>Operator Name:</string>
                   </property>
                 </widget>
               </item>
-              <item row="1" column="1" colspan="2">
-                <widget class="QLineEdit" name="n1mm_station_name">
+              <item row="1" column="6">
+                <widget class="QLineEdit" name="n1mm_operator">
                   <property name="font">
                     <font>
                       <family>JetBrains Mono</family>
                       <pointsize>12</pointsize>
                       <strikeout>false</strikeout>
                     </font>
                   </property>
                   <property name="placeholderText">
                     <string/>
                   </property>
                 </widget>
               </item>
-              <item row="1" column="3">
-                <widget class="QLabel" name="label_14">
+              <item row="0" column="0" colspan="7" alignment="Qt::AlignHCenter">
+                <widget class="QCheckBox" name="send_n1mm_packets">
                   <property name="font">
                     <font>
                       <family>JetBrains Mono</family>
                       <pointsize>12</pointsize>
                       <strikeout>false</strikeout>
                     </font>
                   </property>
+                  <property name="styleSheet">
+                    <string notr="true"/>
+                  </property>
                   <property name="text">
-                    <string>Operator Name:</string>
+                    <string>Send N1MM packets</string>
                   </property>
                 </widget>
               </item>
-              <item row="1" column="4">
-                <widget class="QLineEdit" name="n1mm_operator">
+              <item row="1" column="0">
+                <widget class="QLabel" name="label_13">
                   <property name="font">
                     <font>
                       <family>JetBrains Mono</family>
                       <pointsize>12</pointsize>
                       <strikeout>false</strikeout>
                     </font>
                   </property>
-                  <property name="placeholderText">
-                    <string/>
+                  <property name="text">
+                    <string>Station Name:</string>
                   </property>
                 </widget>
               </item>
-              <item row="2" column="0" colspan="2" alignment="Qt::AlignRight">
-                <widget class="QLabel" name="label_15">
+              <item row="1" column="1" colspan="4">
+                <widget class="QLineEdit" name="n1mm_station_name">
                   <property name="font">
                     <font>
                       <family>JetBrains Mono</family>
                       <pointsize>12</pointsize>
                       <strikeout>false</strikeout>
                     </font>
                   </property>
-                  <property name="text">
-                    <string>Destination Adderess:</string>
+                  <property name="placeholderText">
+                    <string/>
                   </property>
                 </widget>
               </item>
-              <item row="4" column="0" colspan="2" alignment="Qt::AlignRight">
-                <widget class="QLabel" name="label_17">
+              <item row="2" column="0">
+                <widget class="QLabel" name="label_16">
                   <property name="font">
                     <font>
                       <family>JetBrains Mono</family>
                       <pointsize>12</pointsize>
                       <strikeout>false</strikeout>
                     </font>
                   </property>
                   <property name="text">
-                    <string>Contact Port:</string>
+                    <string>Radio:</string>
+                  </property>
+                  <property name="alignment">
+                    <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
                   </property>
                 </widget>
               </item>
-              <item row="5" column="1" alignment="Qt::AlignRight">
-                <widget class="QLabel" name="label_18">
+              <item row="3" column="0">
+                <widget class="QLabel" name="label_17">
                   <property name="font">
                     <font>
                       <family>JetBrains Mono</family>
                       <pointsize>12</pointsize>
                       <strikeout>false</strikeout>
                     </font>
                   </property>
                   <property name="text">
-                    <string>Lookup Port:</string>
+                    <string>Contact:</string>
+                  </property>
+                  <property name="alignment">
+                    <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
                   </property>
                 </widget>
               </item>
-              <item row="6" column="1" alignment="Qt::AlignRight">
-                <widget class="QLabel" name="label_19">
+              <item row="6" column="0">
+                <widget class="QLabel" name="label_18">
                   <property name="font">
                     <font>
                       <family>JetBrains Mono</family>
                       <pointsize>12</pointsize>
                       <strikeout>false</strikeout>
                     </font>
                   </property>
                   <property name="text">
-                    <string>Score Port:</string>
+                    <string>Lookup:</string>
+                  </property>
+                  <property name="alignment">
+                    <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
                   </property>
                 </widget>
               </item>
-              <item row="0" column="0" colspan="5" alignment="Qt::AlignHCenter">
-                <widget class="QCheckBox" name="send_n1mm_packets">
+              <item row="7" column="0">
+                <widget class="QLabel" name="label_19">
                   <property name="font">
                     <font>
                       <family>JetBrains Mono</family>
                       <pointsize>12</pointsize>
                       <strikeout>false</strikeout>
                     </font>
                   </property>
-                  <property name="styleSheet">
-                    <string notr="true"/>
+                  <property name="text">
+                    <string>Score:</string>
+                  </property>
+                  <property name="alignment">
+                    <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
+                  </property>
+                </widget>
+              </item>
+              <item row="2" column="1">
+                <widget class="QCheckBox" name="send_n1mm_radio">
+                  <property name="maximumSize">
+                    <size>
+                      <width>22</width>
+                      <height>16777215</height>
+                    </size>
                   </property>
                   <property name="text">
-                    <string>Send N1MM packets</string>
+                    <string/>
                   </property>
                 </widget>
               </item>
-              <item row="3" column="0" colspan="2" alignment="Qt::AlignRight">
-                <widget class="QLabel" name="label_16">
-                  <property name="font">
-                    <font>
-                      <family>JetBrains Mono</family>
-                      <pointsize>12</pointsize>
-                      <strikeout>false</strikeout>
-                    </font>
+              <item row="3" column="1">
+                <widget class="QCheckBox" name="send_n1mm_contact">
+                  <property name="maximumSize">
+                    <size>
+                      <width>22</width>
+                      <height>16777215</height>
+                    </size>
                   </property>
                   <property name="text">
-                    <string>Radio Port:</string>
+                    <string/>
                   </property>
                 </widget>
               </item>
-              <item row="2" column="2" colspan="3">
-                <widget class="QLineEdit" name="n1mm_ip">
-                  <property name="font">
-                    <font>
-                      <family>JetBrains Mono</family>
-                      <pointsize>12</pointsize>
-                      <strikeout>false</strikeout>
-                    </font>
+              <item row="6" column="1">
+                <widget class="QCheckBox" name="send_n1mm_lookup">
+                  <property name="maximumSize">
+                    <size>
+                      <width>22</width>
+                      <height>16777215</height>
+                    </size>
                   </property>
                   <property name="text">
                     <string/>
                   </property>
-                  <property name="placeholderText">
+                </widget>
+              </item>
+              <item row="7" column="1">
+                <widget class="QCheckBox" name="send_n1mm_score">
+                  <property name="sizePolicy">
+                    <sizepolicy hsizetype="Minimum" vsizetype="Fixed">
+                      <horstretch>0</horstretch>
+                      <verstretch>0</verstretch>
+                    </sizepolicy>
+                  </property>
+                  <property name="maximumSize">
+                    <size>
+                      <width>23</width>
+                      <height>16777215</height>
+                    </size>
+                  </property>
+                  <property name="text">
                     <string/>
                   </property>
                 </widget>
               </item>
-              <item row="3" column="2" colspan="3">
+              <item row="2" column="2" colspan="5">
                 <widget class="QLineEdit" name="n1mm_radioport">
                   <property name="font">
                     <font>
                       <family>JetBrains Mono</family>
                       <pointsize>12</pointsize>
                       <strikeout>false</strikeout>
                     </font>
@@ -1188,15 +1227,15 @@
                     <string/>
                   </property>
                   <property name="placeholderText">
                     <string/>
                   </property>
                 </widget>
               </item>
-              <item row="4" column="2" colspan="3">
+              <item row="3" column="2" colspan="5">
                 <widget class="QLineEdit" name="n1mm_contactport">
                   <property name="font">
                     <font>
                       <family>JetBrains Mono</family>
                       <pointsize>12</pointsize>
                       <strikeout>false</strikeout>
                     </font>
@@ -1208,15 +1247,15 @@
                     <string/>
                   </property>
                   <property name="placeholderText">
                     <string/>
                   </property>
                 </widget>
               </item>
-              <item row="5" column="2" colspan="3">
+              <item row="6" column="2" colspan="5">
                 <widget class="QLineEdit" name="n1mm_lookupport">
                   <property name="font">
                     <font>
                       <family>JetBrains Mono</family>
                       <pointsize>12</pointsize>
                       <strikeout>false</strikeout>
                     </font>
@@ -1228,15 +1267,15 @@
                     <string/>
                   </property>
                   <property name="placeholderText">
                     <string/>
                   </property>
                 </widget>
               </item>
-              <item row="6" column="2" colspan="3">
+              <item row="7" column="2" colspan="5">
                 <widget class="QLineEdit" name="n1mm_scoreport">
                   <property name="font">
                     <font>
                       <family>JetBrains Mono</family>
                       <pointsize>12</pointsize>
                       <strikeout>false</strikeout>
                     </font>
@@ -1255,15 +1294,14 @@
             </layout>
           </widget>
         </widget>
       </item>
     </layout>
   </widget>
   <tabstops>
-    <tabstop>tabWidget</tabstop>
     <tabstop>usehamqth_radioButton</tabstop>
     <tabstop>useqrz_radioButton</tabstop>
     <tabstop>radioButton_3</tabstop>
     <tabstop>lookup_user_name_field</tabstop>
     <tabstop>usehamdb_radioButton</tabstop>
     <tabstop>lookup_password_field</tabstop>
     <tabstop>sounddevice</tabstop>
@@ -1280,15 +1318,14 @@
     <tabstop>connect_to_server</tabstop>
     <tabstop>multicast_group</tabstop>
     <tabstop>multicast_port</tabstop>
     <tabstop>interface_ip</tabstop>
     <tabstop>n1mm_station_name</tabstop>
     <tabstop>n1mm_operator</tabstop>
     <tabstop>send_n1mm_packets</tabstop>
-    <tabstop>n1mm_ip</tabstop>
     <tabstop>n1mm_radioport</tabstop>
     <tabstop>n1mm_contactport</tabstop>
     <tabstop>n1mm_lookupport</tabstop>
     <tabstop>n1mm_scoreport</tabstop>
   </tabstops>
   <resources/>
   <connections>
@@ -1321,12 +1358,29 @@
         <hint type="destinationlabel">
           <x>286</x>
           <y>274</y>
         </hint>
       </hints>
     </connection>
   </connections>
+  <designerdata>
+    <property name="gridDeltaX">
+      <number>5</number>
+    </property>
+    <property name="gridDeltaY">
+      <number>5</number>
+    </property>
+    <property name="gridSnapX">
+      <bool>true</bool>
+    </property>
+    <property name="gridSnapY">
+      <bool>true</bool>
+    </property>
+    <property name="gridVisible">
+      <bool>true</bool>
+    </property>
+  </designerdata>
   <buttongroups>
     <buttongroup name="buttonGroup"/>
     <buttongroup name="buttonGroup_2"/>
   </buttongroups>
 </ui>
```

### Comparing `not1mm-23.5.9.2/not1mm/data/contests.sql` & `not1mm-23.6.2/not1mm/data/contests.sql`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/cty.json` & `not1mm-23.6.2/not1mm/data/cty_old.json`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/editcontact.ui` & `not1mm-23.6.2/not1mm/data/editcontact.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/editmacro.ui` & `not1mm-23.6.2/not1mm/data/editmacro.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/k6gte.not1mm-128.png` & `not1mm-23.6.2/not1mm/data/k6gte.not1mm-128.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/k6gte.not1mm-32.png` & `not1mm-23.6.2/not1mm/data/k6gte.not1mm-32.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/k6gte.not1mm-64.png` & `not1mm-23.6.2/not1mm/data/k6gte.not1mm-64.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/logwindow.ui` & `not1mm-23.6.2/not1mm/data/logwindow.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/main.ui` & `not1mm-23.6.2/not1mm/data/main.ui`

 * *Files 1% similar despite different names*

#### Comparing `not1mm-23.5.9.2/not1mm/data/main.ui` & `not1mm-23.6.2/not1mm/data/main.ui`

```diff
@@ -1,38 +1,44 @@
 <?xml version="1.0" encoding="utf-8"?>
 <ui version="4.0">
   <class>MainWindow</class>
   <widget class="QMainWindow" name="MainWindow">
+    <property name="windowModality">
+      <enum>Qt::NonModal</enum>
+    </property>
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
-        <width>1731</width>
-        <height>358</height>
+        <width>866</width>
+        <height>366</height>
       </rect>
     </property>
     <property name="sizePolicy">
-      <sizepolicy hsizetype="Minimum" vsizetype="Minimum">
+      <sizepolicy hsizetype="Preferred" vsizetype="Preferred">
         <horstretch>0</horstretch>
         <verstretch>0</verstretch>
       </sizepolicy>
     </property>
     <property name="font">
       <font>
         <family>JetBrains Mono</family>
         <pointsize>11</pointsize>
       </font>
     </property>
     <property name="focusPolicy">
       <enum>Qt::NoFocus</enum>
     </property>
     <property name="windowTitle">
-      <string>NOT1MM</string>
+      <string>Not1MM</string>
     </property>
     <widget class="QWidget" name="centralwidget">
+      <property name="enabled">
+        <bool>true</bool>
+      </property>
       <property name="focusPolicy">
         <enum>Qt::NoFocus</enum>
       </property>
       <layout class="QGridLayout" name="gridLayout">
         <property name="leftMargin">
           <number>10</number>
         </property>
@@ -641,14 +647,15 @@
                             <property name="enabled">
                               <bool>true</bool>
                             </property>
                             <property name="font">
                               <font>
                                 <family>JetBrains Mono</family>
                                 <pointsize>20</pointsize>
+                                <weight>75</weight>
                                 <bold>true</bold>
                               </font>
                             </property>
                             <property name="styleSheet">
                               <string notr="true">color: rgb(246, 10, 10);</string>
                             </property>
                             <property name="text">
@@ -1014,25 +1021,26 @@
       </layout>
     </widget>
     <widget class="QMenuBar" name="menubar">
       <property name="geometry">
         <rect>
           <x>0</x>
           <y>0</y>
-          <width>1731</width>
-          <height>30</height>
+          <width>866</width>
+          <height>31</height>
         </rect>
       </property>
       <property name="nativeMenuBar">
         <bool>true</bool>
       </property>
       <widget class="QMenu" name="menuFile">
         <property name="font">
           <font>
             <family>JetBrains Mono</family>
+            <pointsize>11</pointsize>
           </font>
         </property>
         <property name="title">
           <string>File</string>
         </property>
         <addaction name="actionNew_Database"/>
         <addaction name="actionOpen_Database"/>
@@ -1055,17 +1063,15 @@
         </property>
         <addaction name="actionAbout"/>
       </widget>
       <widget class="QMenu" name="menuView">
         <property name="title">
           <string>View</string>
         </property>
-        <addaction name="actionCommand_Buttons"/>
         <addaction name="actionCW_Macros"/>
-        <addaction name="actionDark_Mode"/>
       </widget>
       <widget class="QMenu" name="menuWindow">
         <property name="title">
           <string>Window</string>
         </property>
         <addaction name="actionLog_Window"/>
         <addaction name="actionBandmap"/>
@@ -1423,14 +1429,19 @@
         <bool>false</bool>
       </property>
     </action>
     <action name="actionEdit_Current_Contest">
       <property name="text">
         <string>Edit Current Contest</string>
       </property>
+      <property name="font">
+        <font>
+          <family>JetBrains Mono</family>
+        </font>
+      </property>
     </action>
     <action name="actionBandmap">
       <property name="text">
         <string>Bandmap</string>
       </property>
       <property name="font">
         <font>
```

### Comparing `not1mm-23.5.9.2/not1mm/data/new_contest.ui` & `not1mm-23.6.2/not1mm/data/new_contest.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/opon.ui` & `not1mm-23.6.2/not1mm/data/opon.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/0.wav` & `not1mm-23.6.2/not1mm/data/phonetics/0.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/1.wav` & `not1mm-23.6.2/not1mm/data/phonetics/1.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/2.wav` & `not1mm-23.6.2/not1mm/data/phonetics/2.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/3.wav` & `not1mm-23.6.2/not1mm/data/phonetics/3.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/4.wav` & `not1mm-23.6.2/not1mm/data/phonetics/4.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/5.wav` & `not1mm-23.6.2/not1mm/data/phonetics/5.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/6.wav` & `not1mm-23.6.2/not1mm/data/phonetics/6.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/7.wav` & `not1mm-23.6.2/not1mm/data/phonetics/7.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/73.wav` & `not1mm-23.6.2/not1mm/data/phonetics/73.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/8.wav` & `not1mm-23.6.2/not1mm/data/phonetics/8.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/9.wav` & `not1mm-23.6.2/not1mm/data/phonetics/9.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/a.wav` & `not1mm-23.6.2/not1mm/data/phonetics/a.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/again.wav` & `not1mm-23.6.2/not1mm/data/phonetics/again.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/b.wav` & `not1mm-23.6.2/not1mm/data/phonetics/b.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/c.wav` & `not1mm-23.6.2/not1mm/data/phonetics/c.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/contest.wav` & `not1mm-23.6.2/not1mm/data/phonetics/contest.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/cq.wav` & `not1mm-23.6.2/not1mm/data/phonetics/cq.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/d.wav` & `not1mm-23.6.2/not1mm/data/phonetics/d.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/e.wav` & `not1mm-23.6.2/not1mm/data/phonetics/e.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/f.wav` & `not1mm-23.6.2/not1mm/data/phonetics/f.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/g.wav` & `not1mm-23.6.2/not1mm/data/phonetics/g.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/h.wav` & `not1mm-23.6.2/not1mm/data/phonetics/h.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/i.wav` & `not1mm-23.6.2/not1mm/data/phonetics/i.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/j.wav` & `not1mm-23.6.2/not1mm/data/phonetics/j.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/k.wav` & `not1mm-23.6.2/not1mm/data/phonetics/k.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/k6gte.wav` & `not1mm-23.6.2/not1mm/data/phonetics/k6gte.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/l.wav` & `not1mm-23.6.2/not1mm/data/phonetics/l.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/m.wav` & `not1mm-23.6.2/not1mm/data/phonetics/m.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/mynumber.wav` & `not1mm-23.6.2/not1mm/data/phonetics/mynumber.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/n.wav` & `not1mm-23.6.2/not1mm/data/phonetics/n.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/nil.wav` & `not1mm-23.6.2/not1mm/data/phonetics/nil.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/o.wav` & `not1mm-23.6.2/not1mm/data/phonetics/o.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/p.wav` & `not1mm-23.6.2/not1mm/data/phonetics/p.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/q.wav` & `not1mm-23.6.2/not1mm/data/phonetics/q.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/r.wav` & `not1mm-23.6.2/not1mm/data/phonetics/r.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/roger.wav` & `not1mm-23.6.2/not1mm/data/phonetics/roger.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/s.wav` & `not1mm-23.6.2/not1mm/data/phonetics/s.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/space.wav` & `not1mm-23.6.2/not1mm/data/phonetics/space.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/t.wav` & `not1mm-23.6.2/not1mm/data/phonetics/t.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/thankyou.wav` & `not1mm-23.6.2/not1mm/data/phonetics/thankyou.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/thankyouqrz.wav` & `not1mm-23.6.2/not1mm/data/phonetics/thankyouqrz.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/u.wav` & `not1mm-23.6.2/not1mm/data/phonetics/u.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/v.wav` & `not1mm-23.6.2/not1mm/data/phonetics/v.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/w.wav` & `not1mm-23.6.2/not1mm/data/phonetics/w.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/x.wav` & `not1mm-23.6.2/not1mm/data/phonetics/x.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/y.wav` & `not1mm-23.6.2/not1mm/data/phonetics/y.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/yourcall.wav` & `not1mm-23.6.2/not1mm/data/phonetics/yourcall.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/phonetics/z.wav` & `not1mm-23.6.2/not1mm/data/phonetics/z.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/pickcontest.ui` & `not1mm-23.6.2/not1mm/data/pickcontest.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/reddot.png` & `not1mm-23.6.2/not1mm/data/reddot.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/data/settings.ui` & `not1mm-23.6.2/not1mm/data/settings.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/lib/cat_interface.py` & `not1mm-23.6.2/not1mm/lib/cat_interface.py`

 * *Files 14% similar despite different names*

```diff
@@ -57,32 +57,43 @@
         self.port = port
         self.online = False
         if self.interface == "flrig":
             target = f"http://{host}:{port}"
             logger.debug("%s", target)
             self.server = xmlrpc.client.ServerProxy(target)
             self.online = True
+            try:
+                _ = self.server.main.get_version()
+            except ConnectionRefusedError:
+                self.online = False
+            except xmlrpc.client.Fault:
+                self.online = False
         if self.interface == "rigctld":
             self.__initialize_rigctrld()
 
     def __initialize_rigctrld(self):
         try:
             self.rigctrlsocket = socket.socket()
             self.rigctrlsocket.settimeout(0.5)
             self.rigctrlsocket.connect((self.host, self.port))
             logger.debug("Connected to rigctrld")
             self.online = True
         except ConnectionRefusedError as exception:
             self.rigctrlsocket = None
             self.online = False
-            logger.debug("%s", exception)
+            logger.debug("%s", f"{exception}")
         except TimeoutError as exception:
             self.rigctrlsocket = None
             self.online = False
-            logger.debug("%s", exception)
+            logger.debug("%s", f"{exception}")
+
+    def reinit(self):
+        """reinitialise rigctl"""
+        if self.interface == "rigctld":
+            self.__initialize_rigctrld()
 
     def get_vfo(self) -> str:
         """Poll the radio for current vfo using the interface"""
         vfo = ""
         if self.interface == "flrig":
             vfo = self.__getvfo_flrig()
         if self.interface == "rigctld":
@@ -94,27 +105,30 @@
     def __getvfo_flrig(self) -> str:
         """Poll the radio using flrig"""
         try:
             self.online = True
             return self.server.rig.get_vfo()
         except ConnectionRefusedError as exception:
             self.online = False
-            logger.debug("getvfo_flrig: %s", exception)
+            logger.debug("getvfo_flrig: %s", f"{exception}")
+        except xmlrpc.client.Fault as exception:
+            self.online = False
+            logger.debug("getvfo_flrig: %s", f"{exception}")
         return ""
 
     def __getvfo_rigctld(self) -> str:
         """Returns VFO freq returned from rigctld"""
         if self.rigctrlsocket:
             try:
                 self.online = True
                 self.rigctrlsocket.send(b"\nf\n")
                 return self.rigctrlsocket.recv(1024).decode().strip()
             except socket.error as exception:
                 self.online = False
-                logger.debug("getvfo_rigctld: %s", exception)
+                logger.debug("getvfo_rigctld: %s", f"{exception}")
                 self.rigctrlsocket = None
             return ""
 
         self.__initialize_rigctrld()
         return ""
 
     def get_mode(self) -> str:
@@ -129,70 +143,78 @@
     def __getmode_flrig(self) -> str:
         """Returns mode via flrig"""
         try:
             self.online = True
             return self.server.rig.get_mode()
         except ConnectionRefusedError as exception:
             self.online = False
-            logger.debug("%s", exception)
+            logger.debug("%s", f"{exception}")
+        except xmlrpc.client.Fault as exception:
+            self.online = False
+            logger.debug("%s", f"{exception}")
         return ""
 
     def __getmode_rigctld(self) -> str:
         """Returns mode vai rigctld"""
         if self.rigctrlsocket:
             try:
                 self.online = True
                 self.rigctrlsocket.send(b"m\n")
                 mode = self.rigctrlsocket.recv(1024).decode()
                 mode = mode.strip().split()[0]
-                logger.debug("%s", mode)
+                # logger.debug("%s", mode)
                 return mode
             except IndexError as exception:
-                logger.debug("%s", exception)
+                logger.debug("%s", f"{exception}")
             except socket.error as exception:
                 self.online = False
-                logger.debug("%s", exception)
+                logger.debug("%s", f"{exception}")
                 self.rigctrlsocket = None
             return ""
         self.__initialize_rigctrld()
         return ""
 
     def get_bw(self):
         """Get current vfo bandwidth"""
         if self.interface == "flrig":
             return self.__getbw_flrig()
         if self.interface == "rigctld":
             return self.__getbw_rigctld()
         return False
 
     def __getbw_flrig(self):
-        """ccc"""
+        """return bandwidth"""
         try:
             self.online = True
-            return self.server.rig.get_bw()
+            bandwidth = self.server.rig.get_bw()
+            return bandwidth[0]
         except ConnectionRefusedError as exception:
             self.online = False
-            logger.debug("getbw_flrig: %s", exception)
+            logger.debug("getbw_flrig: %s", f"{exception}")
+            return ""
+        except xmlrpc.client.Fault as exception:
+            self.online = False
+            logger.debug("getbw_flrig: %s", f"{exception}")
             return ""
 
     def __getbw_rigctld(self):
-        """ccc"""
+        """return bandwidth"""
         if self.rigctrlsocket:
             try:
                 self.online = True
                 self.rigctrlsocket.send(b"m\n")
                 mode = self.rigctrlsocket.recv(1024).decode()
                 mode = mode.strip().split()[1]
-                logger.debug("%s", mode)
+                # logger.debug("%s", mode)
                 return mode
             except IndexError as exception:
-                logger.debug("%s", exception)
+                logger.debug("%s", f"{exception}")
             except socket.error as exception:
                 self.online = False
-                logger.debug("%s", exception)
+                logger.debug("%s", f"{exception}")
                 self.rigctrlsocket = None
             return ""
         self.__initialize_rigctrld()
         return ""
 
     def get_power(self):
         """Get power level from rig"""
@@ -204,26 +226,30 @@
 
     def __getpower_flrig(self):
         try:
             self.online = True
             return self.server.rig.get_power()
         except ConnectionRefusedError as exception:
             self.online = False
-            logger.debug("getpower_flrig: %s", exception)
+            logger.debug("getpower_flrig: %s", f"{exception}")
+            return ""
+        except xmlrpc.client.Fault as exception:
+            self.online = False
+            logger.debug("getpower_flrig: %s", f"{exception}")
             return ""
 
     def __getpower_rigctld(self):
         if self.rigctrlsocket:
             try:
                 self.online = True
                 self.rigctrlsocket.send(b"l RFPOWER\n")
                 return int(float(self.rigctrlsocket.recv(1024).decode().strip()) * 100)
             except socket.error as exception:
                 self.online = False
-                logger.debug("getpower_rigctld: %s", exception)
+                logger.debug("getpower_rigctld: %s", f"{exception}")
                 self.rigctrlsocket = None
             return ""
 
     def get_ptt(self):
         """Get PTT state"""
         if self.interface == "flrig":
             return self.__getptt_flrig()
@@ -234,30 +260,33 @@
     def __getptt_flrig(self):
         """Returns ptt state via flrig"""
         try:
             self.online = True
             return self.server.rig.get_ptt()
         except ConnectionRefusedError as exception:
             self.online = False
-            logger.debug("%s", exception)
+            logger.debug("%s", f"{exception}")
+        except xmlrpc.client.Fault as exception:
+            self.online = False
+            logger.debug("%s", f"{exception}")
         return "0"
 
     def __getptt_rigctld(self):
         """Returns ptt state via rigctld"""
         if self.rigctrlsocket:
             try:
                 self.online = True
                 self.rigctrlsocket.send(b"t\n")
                 ptt = self.rigctrlsocket.recv(1024).decode()
                 logger.debug("%s", ptt)
                 ptt = ptt.strip()
                 return ptt
             except socket.error as exception:
                 self.online = False
-                logger.debug("%s", exception)
+                logger.debug("%s", f"{exception}")
                 self.rigctrlsocket = None
         return "0"
 
     def set_vfo(self, freq: str) -> bool:
         """Sets the radios vfo"""
         if self.interface == "flrig":
             return self.__setvfo_flrig(freq)
@@ -268,28 +297,31 @@
     def __setvfo_flrig(self, freq: str) -> bool:
         """Sets the radios vfo"""
         try:
             self.online = True
             return self.server.rig.set_frequency(float(freq))
         except ConnectionRefusedError as exception:
             self.online = False
-            logger.debug("setvfo_flrig: %s", exception)
+            logger.debug("setvfo_flrig: %s", f"{exception}")
+        except xmlrpc.client.Fault as exception:
+            self.online = False
+            logger.debug("setvfo_flrig: %s", f"{exception}")
         return False
 
     def __setvfo_rigctld(self, freq: str) -> bool:
         """sets the radios vfo"""
         if self.rigctrlsocket:
             try:
                 self.online = True
                 self.rigctrlsocket.send(bytes(f"F {freq}\n", "utf-8"))
                 _ = self.rigctrlsocket.recv(1024).decode().strip()
                 return True
             except socket.error as exception:
                 self.online = False
-                logger.debug("setvfo_rigctld: %s", exception)
+                logger.debug("setvfo_rigctld: %s", f"{exception}")
                 self.rigctrlsocket = None
                 return False
         self.__initialize_rigctrld()
         return False
 
     def set_mode(self, mode: str) -> bool:
         """Sets the radios mode"""
@@ -302,28 +334,31 @@
     def __setmode_flrig(self, mode: str) -> bool:
         """Sets the radios mode"""
         try:
             self.online = True
             return self.server.rig.set_mode(mode)
         except ConnectionRefusedError as exception:
             self.online = False
-            logger.debug("setmode_flrig: %s", exception)
+            logger.debug("setmode_flrig: %s", f"{exception}")
+        except xmlrpc.client.Fault as exception:
+            self.online = False
+            logger.debug("setmode_flrig: %s", f"{exception}")
         return False
 
     def __setmode_rigctld(self, mode: str) -> bool:
         """sets the radios mode"""
         if self.rigctrlsocket:
             try:
                 self.online = True
                 self.rigctrlsocket.send(bytes(f"M {mode} 0\n", "utf-8"))
                 _ = self.rigctrlsocket.recv(1024).decode().strip()
                 return True
             except socket.error as exception:
                 self.online = False
-                logger.debug("setmode_rigctld: %s", exception)
+                logger.debug("setmode_rigctld: %s", f"{exception}")
                 self.rigctrlsocket = None
                 return False
         self.__initialize_rigctrld()
         return False
 
     def set_power(self, power):
         """Sets the radios power"""
@@ -335,15 +370,19 @@
 
     def __setpower_flrig(self, power):
         try:
             self.online = True
             return self.server.rig.set_power(power)
         except ConnectionRefusedError as exception:
             self.online = False
-            logger.debug("setmode_flrig: %s", exception)
+            logger.debug("setpower_flrig: %s", f"{exception}")
+            return False
+        except xmlrpc.client.Fault as exception:
+            self.online = False
+            logger.debug("setpower_flrig: %s", f"{exception}")
             return False
 
     def __setpower_rigctld(self, power):
         if power.isnumeric() and int(power) >= 1 and int(power) <= 100:
             rig_cmd = bytes(f"L RFPOWER {str(float(power) / 100)}\n", "utf-8")
             try:
                 self.online = True
@@ -385,15 +424,18 @@
     def __ptt_on_flrig(self):
         """Toggle PTT state on"""
         try:
             self.online = True
             return self.server.rig.set_ptt(1)
         except ConnectionRefusedError as exception:
             self.online = False
-            logger.debug("%s", exception)
+            logger.debug("%s", f"{exception}")
+        except xmlrpc.client.Fault as exception:
+            self.online = False
+            logger.debug("%s", f"{exception}")
         return "0"
 
     def ptt_off(self):
         """turn ptt on/off"""
         if self.interface == "flrig":
             return self.__ptt_off_flrig()
         if self.interface == "rigctld":
@@ -415,9 +457,12 @@
     def __ptt_off_flrig(self):
         """Toggle PTT state off"""
         try:
             self.online = True
             return self.server.rig.set_ptt(0)
         except ConnectionRefusedError as exception:
             self.online = False
-            logger.debug("%s", exception)
+            logger.debug("%s", f"{exception}")
+        except xmlrpc.client.Fault as exception:
+            self.online = False
+            logger.debug("%s", f"{exception}")
         return "0"
```

### Comparing `not1mm-23.5.9.2/not1mm/lib/cwinterface.py` & `not1mm-23.6.2/not1mm/lib/cwinterface.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,14 +18,31 @@
     """An interface to cwdaemon and PyWinkeyerSerial"""
 
     def __init__(self, servertype: int, host: str, port: int) -> None:
         self.servertype = servertype
         self.host = host
         self.port = port
         self.speed = 20
+        self.winkeyer_functions = []
+        if self.servertype == 2:
+            with ServerProxy(f"http://{self.host}:{self.port}") as proxy:
+                try:
+                    self.winkeyer_functions = proxy.system.listMethods()
+                    logger.debug("%s", f"{self.winkeyer_functions}")
+                except Error as exception:
+                    logger.info(
+                        "http://%s:%s, xmlrpc error: %s",
+                        self.host,
+                        self.port,
+                        exception,
+                    )
+                except ConnectionRefusedError:
+                    logger.info(
+                        "http://%s:%s, xmlrpc Connection Refused", self.host, self.port
+                    )
 
     def sendcw(self, texttosend):
         """sends cw to k1el"""
         logger.info("sendcw: %s", texttosend)
         if self.servertype == 2:
             self._sendcw_xmlrpc(texttosend)
         if self.servertype == 1:
@@ -49,7 +66,22 @@
     def _sendcw_udp(self, texttosend):
         """send cw to udp port"""
         logger.info("UDP: %s", texttosend)
         server_address_port = (self.host, self.port)
         # bufferSize          = 1024
         udp_client_socket = socket.socket(family=socket.AF_INET, type=socket.SOCK_DGRAM)
         udp_client_socket.sendto(bytes(texttosend, "utf-8"), server_address_port)
+
+    def set_winkeyer_speed(self, speed):
+        """doc"""
+        with ServerProxy(f"http://{self.host}:{self.port}") as proxy:
+            try:
+                if "setspeed" in self.winkeyer_functions:
+                    proxy.setspeed(speed)
+            except Error as exception:
+                logger.info(
+                    "http://%s:%s, xmlrpc error: %s", self.host, self.port, exception
+                )
+            except ConnectionRefusedError:
+                logger.info(
+                    "http://%s:%s, xmlrpc Connection Refused", self.host, self.port
+                )
```

### Comparing `not1mm-23.5.9.2/not1mm/lib/database.py` & `not1mm-23.6.2/not1mm/lib/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,51 +100,51 @@
                 cursor = conn.cursor()
                 sql_command = (
                     "CREATE TABLE IF NOT EXISTS DXLOG ("
                     "TS DATETIME NOT NULL, "
                     "Call VARCHAR(15) NOT NULL, "
                     "Freq DOUBLE NULL, "
                     "QSXFreq DOUBLE NULL DEFAULT 0, "
-                    "Mode VARCHAR(6), "
+                    "Mode VARCHAR(6) DEFAULT '', "
                     "ContestName VARCHAR(10) DEFAULT 'NORMAL', "
-                    "SNT VARCHAR(10), "
-                    "RCV VARCHAR(15), "
+                    "SNT VARCHAR(10) DEFAULT '', "
+                    "RCV VARCHAR(15) DEFAULT '', "
                     "CountryPrefix VARCHAR(8) DEFAULT '', "
                     "StationPrefix VARCHAR(15) DEFAULT '', "
                     "QTH VARCHAR(25) DEFAULT '', "
                     "Name VARCHAR(20) DEFAULT '', "
                     "Comment VARCHAR(60) DEFAULT '', "
                     "NR INTEGER DEFAULT 0, "
                     "Sect VARCHAR(8) DEFAULT '', "
                     "Prec VARCHAR(1) DEFAULT '', "
                     "CK TINYINT DEFAULT 0, "
                     "ZN TINYINT DEFAULT 0, "
                     "SentNr INTEGER DEFAULT 0, "
                     "Points INTEGER DEFAULT 0, "
                     "IsMultiplier1 TINYINT DEFAULT 0, "
                     "IsMultiplier2 INTEGER DEFAULT 0, "
-                    "Power VARCHAR(8), "
+                    "Power VARCHAR(8) DEFAULT '', "
                     "Band FLOAT NULL DEFAULT 0, "
-                    "WPXPrefix VARCHAR(8), "
-                    "Exchange1 VARCHAR(20), "
+                    "WPXPrefix VARCHAR(8) DEFAULT '', "
+                    "Exchange1 VARCHAR(20) DEFAULT '', "
                     "RadioNR TINYINT DEFAULT 1, "
                     "ContestNR INTEGER, "
-                    "isMultiplier3 INTEGER, "
-                    "MiscText VARCHAR(20), "
+                    "isMultiplier3 INTEGER DEFAULT 0, "
+                    "MiscText VARCHAR(20) DEFAULT '', "
                     "IsRunQSO TINYINT(1) DEFAULT 0, "
-                    "ContactType VARCHAR(1), "
+                    "ContactType VARCHAR(1) DEFAULT '', "
                     "Run1Run2 TINYINT NOT NULL, "
-                    "GridSquare VARCHAR(6), "
-                    "Operator VARCHAR(20), "
-                    "Continent VARCHAR(2), "
-                    "RoverLocation VARCHAR(10), "
+                    "GridSquare VARCHAR(6) DEFAULT '', "
+                    "Operator VARCHAR(20) DEFAULT '', "
+                    "Continent VARCHAR(2) DEFAULT '', "
+                    "RoverLocation VARCHAR(10) DEFAULT '', "
                     "RadioInterfaced INTEGER, "
                     "NetworkedCompNr INTEGER, NetBiosName varchar (255), "
                     "IsOriginal Boolean, "
-                    "ID TEXT(16) NOT NULL DEFAULT '0000000000000000', "
+                    "ID TEXT(32) NOT NULL DEFAULT '00000000000000000000000000000000', "
                     "CLAIMEDQSO INTEGER DEFAULT 1,"
                     "PRIMARY KEY (`TS`, `Call`) );"
                 )
                 cursor.execute(sql_command)
                 conn.commit()
         except sqlite3.OperationalError as exception:
             logger.debug("%s", exception)
@@ -427,20 +427,20 @@
         pre = "UPDATE dxlog set "
         for key in qso.keys():
             pre += f"{key} = '{qso[key]}',"
         sql = f"{pre[:-1]} where ID='{qso['ID']}';"
 
         try:
             with sqlite3.connect(self.database) as conn:
-                logger.info("%s\n%s", sql, qso)
+                logger.debug("%s\n%s", sql, qso)
                 cur = conn.cursor()
                 cur.execute(sql)
                 conn.commit()
         except sqlite3.Error as exception:
-            logger.info("DataBase change_contact: %s", exception)
+            logger.critical("DataBase change_contact: %s", exception)
 
     def delete_contact(self, unique_id: str) -> None:
         """Deletes a contact from the db."""
         if unique_id:
             try:
                 with sqlite3.connect(self.database) as conn:
                     sql = f"delete from dxlog where ID='{unique_id}';"
```

### Comparing `not1mm-23.5.9.2/not1mm/lib/edit_macro.py` & `not1mm-23.6.2/not1mm/lib/edit_macro.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/lib/edit_station.py` & `not1mm-23.6.2/not1mm/lib/edit_station.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/lib/ham_utility.py` & `not1mm-23.6.2/not1mm/lib/ham_utility.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/lib/lookup.py` & `not1mm-23.6.2/not1mm/lib/lookup.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/lib/multicast.py` & `not1mm-23.6.2/not1mm/lib/multicast.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,52 @@
 """
 K6GTE, multicast broadcast interface
 Email: michael.bridak@gmail.com
 GPL V3
 """
 # pylint: disable=unused-import
 import logging
-import socket
 from json import JSONDecodeError, dumps, loads
 
 from dicttoxml import dicttoxml
 
+from PyQt5 import QtNetwork
+
 logger = logging.getLogger("__main__")
 
 if __name__ == "__main__":
     print("I'm not the program you are looking for.")
 
 
 class Multicast:
     """Sets up multicast connection"""
 
     def __init__(self, multicast_group: str, multicast_port: int, interface_ip: str):
         self.multicast_group = multicast_group
-        self.multicast_port = multicast_port
+        self.multicast_port = int(multicast_port)
         self.interface_ip = interface_ip
-        self.server_udp = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
-        self.server_udp.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
-        self.server_udp.bind(("", int(self.multicast_port)))
-        mreq = socket.inet_aton(self.multicast_group) + socket.inet_aton(
-            self.interface_ip
-        )
-        self.server_udp.setsockopt(
-            socket.IPPROTO_IP, socket.IP_ADD_MEMBERSHIP, bytes(mreq)
+        self.server_udp = QtNetwork.QUdpSocket()
+        self.server_udp.bind(
+            QtNetwork.QHostAddress.AnyIPv4,
+            int(self.multicast_port),
+            QtNetwork.QUdpSocket.ShareAddress,
         )
-        self.server_udp.settimeout(0.01)
+        self.server_udp.joinMulticastGroup(QtNetwork.QHostAddress(self.multicast_group))
+
+    def ready_read_connect(self, watcher):
+        """pass in function to watch traffic"""
+        self.server_udp.readyRead.connect(watcher)
 
     def send_as_json(self, dict_object: dict):
         """Send dict as json encoded packet"""
-        bytes_to_send = bytes(dumps(dict_object), encoding="ascii")
+        packet = bytes(dumps(dict_object), encoding="ascii")
         logger.debug("%s", f"{dict_object}")
-        try:
-            self.server_udp.sendto(
-                bytes_to_send,
-                (self.multicast_group, int(self.multicast_port)),
-            )
-        except OSError as err:
-            logger.warning("%s", err)
+        self.server_udp.writeDatagram(
+            packet, QtNetwork.QHostAddress(self.multicast_group), self.multicast_port
+        )
 
     def send_as_xml(self, dict_object: dict, package_name: str):
         """Send dict as XML encoded packet"""
-        bytes_to_send = dicttoxml(
-            dict_object, custom_root=package_name, attr_type=False
+        packet = dicttoxml(dict_object, custom_root=package_name, attr_type=False)
+        self.server_udp.writeDatagram(
+            packet, QtNetwork.QHostAddress(self.multicast_group), self.multicast_port
         )
-        try:
-            self.server_udp.sendto(
-                bytes_to_send,
-                (self.multicast_group, int(self.multicast_port)),
-            )
-        except OSError as err:
-            logger.warning("%s", err)
```

### Comparing `not1mm-23.5.9.2/not1mm/lib/settings.py` & `not1mm-23.6.2/not1mm/lib/settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -58,19 +58,26 @@
         self.send_n1mm_packets.setChecked(
             bool(self.preference.get("send_n1mm_packets"))
         )
         self.n1mm_station_name.setText(
             str(self.preference.get("n1mm_station_name", ""))
         )
         self.n1mm_operator.setText(str(self.preference.get("n1mm_operator", "")))
-        self.n1mm_ip.setText(str(self.preference.get("n1mm_ip", "")))
+        # self.n1mm_ip.setText(str(self.preference.get("n1mm_ip", "")))
         self.n1mm_radioport.setText(str(self.preference.get("n1mm_radioport", "")))
         self.n1mm_contactport.setText(str(self.preference.get("n1mm_contactport", "")))
         self.n1mm_lookupport.setText(str(self.preference.get("n1mm_lookupport", "")))
         self.n1mm_scoreport.setText(str(self.preference.get("n1mm_scoreport", "")))
+        self.send_n1mm_radio.setChecked(bool(self.preference.get("send_n1mm_radio")))
+        self.send_n1mm_contact.setChecked(
+            bool(self.preference.get("send_n1mm_contact"))
+        )
+        self.send_n1mm_lookup.setChecked(bool(self.preference.get("send_n1mm_lookup")))
+        self.send_n1mm_score.setChecked(bool(self.preference.get("send_n1mm_score")))
+
         self.cluster_server_field.setText(
             str(self.preference.get("cluster_server", "dxc.nc7j.com"))
         )
         self.cluster_port_field.setText(str(self.preference.get("cluster_port", 7373)))
         self.cluster_filter.setText(self.preference.get("cluster_filter", ""))
         value = self.preference.get("cluster_mode", "")
         index = self.cluster_mode.findText(value)
@@ -106,17 +113,23 @@
             self.preference["cwtype"] = 2
         self.preference["useserver"] = self.connect_to_server.isChecked()
         self.preference["multicast_group"] = self.multicast_group.text()
         self.preference["multicast_port"] = self.multicast_port.text()
         self.preference["interface_ip"] = self.interface_ip.text()
 
         self.preference["send_n1mm_packets"] = self.send_n1mm_packets.isChecked()
+
+        self.preference["send_n1mm_radio"] = self.send_n1mm_radio.isChecked()
+        self.preference["send_n1mm_contact"] = self.send_n1mm_contact.isChecked()
+        self.preference["send_n1mm_lookup"] = self.send_n1mm_lookup.isChecked()
+        self.preference["send_n1mm_score"] = self.send_n1mm_score.isChecked()
+
         self.preference["n1mm_station_name"] = self.n1mm_station_name.text()
         self.preference["n1mm_operator"] = self.n1mm_operator.text()
-        self.preference["n1mm_ip"] = self.n1mm_ip.text()
+        # self.preference["n1mm_ip"] = self.n1mm_ip.text()
         self.preference["n1mm_radioport"] = self.n1mm_radioport.text()
         self.preference["n1mm_contactport"] = self.n1mm_contactport.text()
         self.preference["n1mm_lookupport"] = self.n1mm_lookupport.text()
         self.preference["n1mm_scoreport"] = self.n1mm_scoreport.text()
         self.preference["cluster_server"] = self.cluster_server_field.text()
         self.preference["cluster_port"] = int(self.cluster_port_field.text())
         self.preference["cluster_filter"] = self.cluster_filter.text()
```

### Comparing `not1mm-23.5.9.2/not1mm/logwindow.py` & `not1mm-23.6.2/not1mm/logwindow.py`

 * *Files 22% similar despite different names*

```diff
@@ -23,16 +23,15 @@
 from PyQt5.QtCore import QDir, QItemSelectionModel
 from PyQt5 import QtNetwork
 from PyQt5.QtGui import QFontDatabase
 
 from not1mm.lib.database import DataBase
 from not1mm.lib.multicast import Multicast
 from not1mm.lib.edit_contact import EditContact
-
-# from not1mm.lib.n1mm import N1MM
+from not1mm.lib.n1mm import N1MM
 
 os.environ["QT_QPA_PLATFORMTHEME"] = "gnome"
 
 loader = pkgutil.get_loader("not1mm")
 WORKING_PATH = os.path.dirname(loader.get_filename())
 
 if "XDG_DATA_HOME" in os.environ:
@@ -45,32 +44,25 @@
     CONFIG_PATH = os.environ.get("XDG_CONFIG_HOME")
 else:
     CONFIG_PATH = str(Path.home() / ".config")
 CONFIG_PATH += "/not1mm"
 
 DARK_STYLESHEET = ""
 
-with open(WORKING_PATH + "/data/Combinear.qss", encoding="utf-8") as stylefile:
-    DARK_STYLESHEET = stylefile.read()
 
 MULTICAST_PORT = 2239
-MULTICAST_GROUP = "224.1.1.1"
+MULTICAST_GROUP = "239.1.1.1"
 INTERFACE_IP = "0.0.0.0"
-# NODE_RED_SERVER_IP = "127.0.0.1"
-# NODE_RED_SERVER_PORT = 12062
-
-# n1mm_socket = socket.socket(family=socket.AF_INET, type=socket.SOCK_DGRAM)
 
 
 class MainWindow(QtWidgets.QMainWindow):
     """
     The main window
     """
 
-    # dbname = DATA_PATH + "/ham.db"
     dbname = None
     edit_contact_dialog = None
     pref = {}
     columns = {
         0: "YYYY-MM-DD HH:MM:SS",
         1: "Call",
         2: "Freq",
@@ -92,16 +84,18 @@
         18: "Name",
         19: "Comment",
         20: "UUID",
     }
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
+        self.table_loading = True
         self._udpwatch = None
         self.udp_fifo = queue.Queue()
+        self.n1mm = None
         self.load_pref()
         if self.pref.get("dark_mode"):
             self.setStyleSheet(DARK_STYLESHEET)
         self.dbname = DATA_PATH + "/" + self.pref.get("current_database", "ham.db")
         self.database = DataBase(self.dbname, WORKING_PATH)
         self.database.current_contest = self.pref.get("contest", 0)
         self.contact = self.database.empty_contact
@@ -164,19 +158,14 @@
         cmd["cmd"] = "GETCOLUMNS"
         cmd["station"] = platform.node()
 
         packet = bytes(dumps(cmd), encoding="ascii")
         self.udpsocket.writeDatagram(
             packet, QtNetwork.QHostAddress(MULTICAST_GROUP), MULTICAST_PORT
         )
-        # self.n1mm = N1MM(
-        #     ip_address=self.preference.get("n1mm_ip"),
-        #     radioport=self.preference.get("n1mm_radioport"),
-        #     contactport=self.preference.get("n1mm_contactport"),
-        # )
 
     def get_column(self, name: str) -> int:
         """returns the column number of the given column name."""
         for key, value in self.columns.items():
             if value == name:
                 return key
 
@@ -191,14 +180,29 @@
                     logger.info("%s", self.pref)
             else:
                 self.pref["current_database"] = "ham.db"
 
         except IOError as exception:
             logger.critical("Error: %s", exception)
 
+        try:
+            self.n1mm = N1MM(
+                self.pref.get("n1mm_radioport", "127.0.0.1:12060"),
+                self.pref.get("n1mm_contactport", "127.0.0.1:12061"),
+                self.pref.get("n1mm_lookupport", "127.0.0.1:12060"),
+                self.pref.get("n1mm_scoreport", "127.0.0.1:12060"),
+            )
+        except ValueError:
+            logger.warning("%s", f"{ValueError}")
+        self.n1mm.send_radio_packets = self.pref.get("send_n1mm_radio", False)
+        self.n1mm.send_contact_packets = self.pref.get("send_n1mm_contact", False)
+        self.n1mm.send_lookup_packets = self.pref.get("send_n1mm_lookup", False)
+        self.n1mm.send_score_packets = self.pref.get("send_n1mm_score", False)
+        self.n1mm.radio_info["StationName"] = self.pref.get("n1mm_station_name", "")
+
     def load_new_db(self):
         """if db changes reload it."""
         self.load_pref()
         self.dbname = DATA_PATH + "/" + self.pref.get("current_database", "ham.db")
         self.database = DataBase(self.dbname, WORKING_PATH)
         self.database.current_contest = self.pref.get("contest", 0)
         self.contact = self.database.empty_contact
@@ -211,16 +215,18 @@
         """Slot for doubleclick event"""
         if self.table_loading:
             return
         logger.debug("DoubleClicked")
 
     def cell_changed(self, row, column):
         """Slot for changed cell"""
-        if self.table_loading:
-            return
+        logger.debug("Cell Changed")
+        self.contact = self.database.fetch_contact_by_uuid(
+            self.generalLog.item(row, self.get_column("UUID")).text()
+        )
         db_record = {
             "TS": self.generalLog.item(
                 row, self.get_column("YYYY-MM-DD HH:MM:SS")
             ).text(),
             "Call": self.generalLog.item(row, self.get_column("Call")).text().upper(),
             "Freq": self.generalLog.item(row, self.get_column("Freq")).text(),
             "SNT": self.generalLog.item(row, self.get_column("Snt")).text(),
@@ -241,14 +247,58 @@
             "CountryPrefix": self.generalLog.item(row, self.get_column("PFX")).text(),
             "Points": self.generalLog.item(row, self.get_column("PTS")).text(),
             "Name": self.generalLog.item(row, self.get_column("Name")).text(),
             "Comment": self.generalLog.item(row, self.get_column("Comment")).text(),
             "ID": self.generalLog.item(row, self.get_column("UUID")).text(),
         }
         self.database.change_contact(db_record)
+
+        if self.n1mm.send_contact_packets:
+            self.n1mm.contact_info["timestamp"] = db_record["TS"]
+            self.n1mm.contact_info["contestname"] = self.contact["ContestName"].replace(
+                "-", ""
+            )
+            self.n1mm.contact_info["contestnr"] = self.contact["ContestNR"]
+            self.n1mm.contact_info["operator"] = self.contact["Operator"]
+            self.n1mm.contact_info["mycall"] = self.contact["Operator"]
+            # self.n1mm.contact_info[""] = self.contact[""]
+            self.n1mm.contact_info["band"] = self.contact["Band"]
+            self.n1mm.contact_info["mode"] = self.contact["Mode"]
+            self.n1mm.contact_info["stationprefix"] = self.contact["StationPrefix"]
+            self.n1mm.contact_info["continent"] = self.contact["Continent"]
+            self.n1mm.contact_info["gridsquare"] = self.contact["GridSquare"]
+            self.n1mm.contact_info["ismultiplier1"] = self.contact["IsMultiplier1"]
+            self.n1mm.contact_info["ismultiplier2"] = self.contact["IsMultiplier2"]
+
+            self.n1mm.contact_info["call"] = db_record["Call"]
+            self.n1mm.contact_info["oldcall"] = self.contact["Call"]
+
+            self.n1mm.contact_info["rxfreq"] = self.n1mm.contact_info["txfreq"] = str(
+                int(float(db_record["Freq"]) * 100)
+            )
+            self.n1mm.contact_info["snt"] = db_record["SNT"]
+            self.n1mm.contact_info["rcv"] = db_record["RCV"]
+            self.n1mm.contact_info["sntnr"] = db_record["SentNr"]
+            self.n1mm.contact_info["rcvnr"] = db_record["NR"]
+            self.n1mm.contact_info["exchange1"] = db_record.get("Exchange1", "")
+            self.n1mm.contact_info["ck"] = db_record["CK"]
+            self.n1mm.contact_info["prec"] = db_record["Prec"]
+            self.n1mm.contact_info["section"] = db_record["Sect"]
+            self.n1mm.contact_info["wpxprefix"] = db_record["WPXPrefix"]
+            self.n1mm.contact_info["power"] = db_record["Power"]
+
+            self.n1mm.contact_info["zone"] = db_record["ZN"]
+
+            self.n1mm.contact_info["countryprefix"] = db_record["CountryPrefix"]
+            self.n1mm.contact_info["points"] = db_record["Points"]
+            self.n1mm.contact_info["name"] = db_record["Name"]
+            self.n1mm.contact_info["misctext"] = db_record["Comment"]
+            self.n1mm.contact_info["ID"] = db_record["ID"]
+            self.n1mm.send_contactreplace()
+
         self.get_log()
         self.generalLog.scrollToItem(self.generalLog.item(row, column))
 
     def dummy(self):
         """the dummy"""
 
     def edit_focused_contact_selected(self, clicked_cell):
@@ -368,14 +418,24 @@
         self.database.change_contact(self.contact)
         self.get_log()
         self.show_like_calls(self.contact.get("Call", ""))
 
     def delete_contact(self):
         """Delete Contact"""
         self.database.delete_contact(self.contact.get("ID", ""))
+        if self.n1mm:
+            if self.n1mm.send_contact_packets:
+                self.n1mm.contactdelete["timestamp"] = self.contact.get("TS", "")
+                self.n1mm.contactdelete["call"] = self.contact.get("Call", "")
+                self.n1mm.contactdelete["contestnr"] = self.contact.get("ContestNR", 1)
+                self.n1mm.contactdelete["StationName"] = self.pref.get(
+                    "n1mm_station_name"
+                )
+                self.n1mm.contactdelete["ID"] = self.contact.get("ID", "")
+                self.n1mm.send_contact_delete()
         self.edit_contact_dialog.close()
         self.get_log()
         self.show_like_calls(self.contact.get("Call", ""))
 
     def get_log(self):
         """Get Log, Show it."""
 
@@ -391,16 +451,16 @@
 
         # Constant	Value	Description
         # Qt::AlignTop	0x0020	Aligns with the top.
         # Qt::AlignBottom	0x0040	Aligns with the bottom.
         # Qt::AlignVCenter	0x0080	Centers vertically in the available space.
         # Qt::AlignBaseline	0x0100	Aligns with the baseline.
 
-        self.generalLog.cellChanged.connect(self.dummy)
-        self.table_loading = True
+        logger.debug("Getting Log")
+        self.generalLog.blockSignals(True)
         current_log = self.database.fetch_all_contacts_asc()
         self.generalLog.setRowCount(0)
         for log_item in current_log:
             number_of_rows = self.generalLog.rowCount()
             self.generalLog.insertRow(number_of_rows)
             time_stamp = log_item.get("TS", "YY-MM-DD HH:MM:SS")
             first_item = QtWidgets.QTableWidgetItem(time_stamp)
@@ -515,16 +575,15 @@
                 QtWidgets.QTableWidgetItem(str(log_item.get("Comment", ""))),
             )
             self.generalLog.setItem(
                 number_of_rows,
                 self.get_column("UUID"),
                 QtWidgets.QTableWidgetItem(str(log_item.get("ID", ""))),
             )
-        self.table_loading = False
-        self.generalLog.cellChanged.connect(self.cell_changed)
+        self.generalLog.blockSignals(False)
 
     def watch_udp(self):
         """Puts UDP datagrams in a FIFO queue"""
         while self.udpsocket.hasPendingDatagrams():
             datagram, _, _ = self.udpsocket.readDatagram(
                 self.udpsocket.pendingDatagramSize()
             )
@@ -723,14 +782,15 @@
     logger.setLevel(logging.DEBUG)
     logger.debug("debugging on")
 else:
     logger.setLevel(logging.WARNING)
     logger.warning("debugging off")
 
 app = QtWidgets.QApplication(sys.argv)
+app.setStyle("Adwaita-Dark")
 font_path = WORKING_PATH + "/data"
 _families = load_fonts_from_dir(os.fspath(font_path))
 window = MainWindow()
 window.show()
 
 if __name__ == "__main__":
     main()
```

### Comparing `not1mm-23.5.9.2/not1mm/plugins/10_10_fall_cw.py` & `not1mm-23.6.2/not1mm/plugins/10_10_fall_cw.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 import logging
 from pathlib import Path
 
 from PyQt5 import QtWidgets
 from not1mm.lib.version import __version__
 
+from decimal import Decimal
+
 logger = logging.getLogger("__main__")
 
 name = "10 10 FALL CW"
 cabrillo_name = "10-10-FALL-CW"
 mode = "CW"  # CW SSB BOTH RTTY
 # columns = [0, 1, 2, 3, 4, 5, 6, 15]
 columns = [
@@ -179,15 +181,15 @@
             print("<ADIF_VER:5>2.2.0", end="\r\n", file=file_descriptor)
             print("<EOH>", end="\r\n", file=file_descriptor)
             for contact in log:
                 hiscall = contact.get("Call", "")
                 the_date_and_time = contact.get("TS")
                 # band = contact.get("Band")
                 themode = contact.get("Mode")
-                frequency = str(contact.get("Freq", 0) / 1000)
+                frequency = str(Decimal(str(contact.get("Freq", 0))) / 1000)
                 sentrst = contact.get("SNT", "")
                 rcvrst = contact.get("RCV", "")
                 sentnr = str(contact.get("SentNr", ""))
                 rcvnr = str(contact.get("NR", ""))
                 grid = contact.get("GridSquare", "")
                 comment = contact.get("ContestName", "")
                 loggeddate = the_date_and_time[:10]
@@ -326,19 +328,20 @@
                 file=file_descriptor,
             )
             print(
                 f"CATEGORY-TRANSMITTER: {self.contest_settings.get('TransmitterCategory','')}",
                 end="\r\n",
                 file=file_descriptor,
             )
-            print(
-                f"CATEGORY-OVERLAY: {self.contest_settings.get('OverlayCategory','')}",
-                end="\r\n",
-                file=file_descriptor,
-            )
+            if self.contest_settings.get("OverlayCategory", "") != "N/A":
+                print(
+                    f"CATEGORY-OVERLAY: {self.contest_settings.get('OverlayCategory','')}",
+                    end="\r\n",
+                    file=file_descriptor,
+                )
             print(
                 f"GRID-LOCATOR: {self.station.get('GridSquare','')}",
                 end="\r\n",
                 file=file_descriptor,
             )
             # print(
             #     f"CATEGORY: {None}",
```

### Comparing `not1mm-23.5.9.2/not1mm/plugins/10_10_spring_cw.py` & `not1mm-23.6.2/not1mm/plugins/10_10_spring_cw.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # pylint: disable=invalid-name, unused-argument, unused-variable
 
 import logging
 from pathlib import Path
 
 from PyQt5 import QtWidgets
 from not1mm.lib.version import __version__
+from decimal import Decimal
 
 logger = logging.getLogger("__main__")
 
 name = "10 10 SPRING CW"
 cabrillo_name = "10-10-SPRING-CW"
 mode = "CW"  # CW SSB BOTH RTTY
 # columns = [0, 1, 2, 3, 4, 5, 6, 15]
@@ -179,15 +180,15 @@
             print("<ADIF_VER:5>2.2.0", end="\r\n", file=file_descriptor)
             print("<EOH>", end="\r\n", file=file_descriptor)
             for contact in log:
                 hiscall = contact.get("Call", "")
                 the_date_and_time = contact.get("TS")
                 # band = contact.get("Band")
                 themode = contact.get("Mode")
-                frequency = str(contact.get("Freq", 0) / 1000)
+                frequency = str(Decimal(str(contact.get("Freq", 0))) / 1000)
                 sentrst = contact.get("SNT", "")
                 rcvrst = contact.get("RCV", "")
                 sentnr = str(contact.get("SentNr", ""))
                 rcvnr = str(contact.get("NR", ""))
                 grid = contact.get("GridSquare", "")
                 comment = contact.get("ContestName", "")
                 loggeddate = the_date_and_time[:10]
@@ -326,19 +327,20 @@
                 file=file_descriptor,
             )
             print(
                 f"CATEGORY-TRANSMITTER: {self.contest_settings.get('TransmitterCategory','')}",
                 end="\r\n",
                 file=file_descriptor,
             )
-            print(
-                f"CATEGORY-OVERLAY: {self.contest_settings.get('OverlayCategory','')}",
-                end="\r\n",
-                file=file_descriptor,
-            )
+            if self.contest_settings.get("OverlayCategory", "") != "N/A":
+                print(
+                    f"CATEGORY-OVERLAY: {self.contest_settings.get('OverlayCategory','')}",
+                    end="\r\n",
+                    file=file_descriptor,
+                )
             print(
                 f"GRID-LOCATOR: {self.station.get('GridSquare','')}",
                 end="\r\n",
                 file=file_descriptor,
             )
             # print(
             #     f"CATEGORY: {None}",
```

### Comparing `not1mm-23.5.9.2/not1mm/plugins/10_10_summer_phone.py` & `not1mm-23.6.2/not1mm/plugins/10_10_summer_phone.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # pylint: disable=invalid-name, unused-argument, unused-variable
 
 import logging
 from pathlib import Path
 
 from PyQt5 import QtWidgets
 from not1mm.lib.version import __version__
+from decimal import Decimal
 
 logger = logging.getLogger("__main__")
 
 name = "10 10 SUMMER PHONE"
 cabrillo_name = "10-10-SUMMER-PHONE"
 mode = "SSB"  # CW SSB BOTH RTTY
 # columns = [0, 1, 2, 3, 4, 5, 6, 15]
@@ -179,15 +180,15 @@
             print("<ADIF_VER:5>2.2.0", end="\r\n", file=file_descriptor)
             print("<EOH>", end="\r\n", file=file_descriptor)
             for contact in log:
                 hiscall = contact.get("Call", "")
                 the_date_and_time = contact.get("TS")
                 # band = contact.get("Band")
                 themode = contact.get("Mode")
-                frequency = str(contact.get("Freq", 0) / 1000)
+                frequency = str(Decimal(str(contact.get("Freq", 0))) / 1000)
                 sentrst = contact.get("SNT", "")
                 rcvrst = contact.get("RCV", "")
                 sentnr = str(contact.get("SentNr", ""))
                 rcvnr = str(contact.get("NR", ""))
                 grid = contact.get("GridSquare", "")
                 comment = contact.get("ContestName", "")
                 loggeddate = the_date_and_time[:10]
@@ -326,19 +327,20 @@
                 file=file_descriptor,
             )
             print(
                 f"CATEGORY-TRANSMITTER: {self.contest_settings.get('TransmitterCategory','')}",
                 end="\r\n",
                 file=file_descriptor,
             )
-            print(
-                f"CATEGORY-OVERLAY: {self.contest_settings.get('OverlayCategory','')}",
-                end="\r\n",
-                file=file_descriptor,
-            )
+            if self.contest_settings.get("OverlayCategory", "") != "N/A":
+                print(
+                    f"CATEGORY-OVERLAY: {self.contest_settings.get('OverlayCategory','')}",
+                    end="\r\n",
+                    file=file_descriptor,
+                )
             print(
                 f"GRID-LOCATOR: {self.station.get('GridSquare','')}",
                 end="\r\n",
                 file=file_descriptor,
             )
             # print(
             #     f"CATEGORY: {None}",
```

### Comparing `not1mm-23.5.9.2/not1mm/plugins/10_10_winter_phone.py` & `not1mm-23.6.2/not1mm/plugins/10_10_winter_phone.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """10 10 winter phone plugin"""
 
 # pylint: disable=invalid-name, unused-argument, unused-variable
 
 import logging
 from pathlib import Path
-
+from decimal import Decimal
 from PyQt5 import QtWidgets
 from not1mm.lib.version import __version__
 
+
 logger = logging.getLogger("__main__")
 
 name = "10 10 WINTER PHONE"
 cabrillo_name = "10-10-SPRING-PHONE"
 mode = "SSB"  # CW SSB BOTH RTTY
 # columns = [0, 1, 2, 3, 4, 5, 6, 15]
 columns = [
@@ -179,15 +180,15 @@
             print("<ADIF_VER:5>2.2.0", end="\r\n", file=file_descriptor)
             print("<EOH>", end="\r\n", file=file_descriptor)
             for contact in log:
                 hiscall = contact.get("Call", "")
                 the_date_and_time = contact.get("TS")
                 # band = contact.get("Band")
                 themode = contact.get("Mode")
-                frequency = str(contact.get("Freq", 0) / 1000)
+                frequency = str(Decimal(str(contact.get("Freq", 0))) / 1000)
                 sentrst = contact.get("SNT", "")
                 rcvrst = contact.get("RCV", "")
                 sentnr = str(contact.get("SentNr", ""))
                 rcvnr = str(contact.get("NR", ""))
                 grid = contact.get("GridSquare", "")
                 comment = contact.get("ContestName", "")
                 loggeddate = the_date_and_time[:10]
@@ -326,19 +327,20 @@
                 file=file_descriptor,
             )
             print(
                 f"CATEGORY-TRANSMITTER: {self.contest_settings.get('TransmitterCategory','')}",
                 end="\r\n",
                 file=file_descriptor,
             )
-            print(
-                f"CATEGORY-OVERLAY: {self.contest_settings.get('OverlayCategory','')}",
-                end="\r\n",
-                file=file_descriptor,
-            )
+            if self.contest_settings.get("OverlayCategory", "") != "N/A":
+                print(
+                    f"CATEGORY-OVERLAY: {self.contest_settings.get('OverlayCategory','')}",
+                    end="\r\n",
+                    file=file_descriptor,
+                )
             print(
                 f"GRID-LOCATOR: {self.station.get('GridSquare','')}",
                 end="\r\n",
                 file=file_descriptor,
             )
             # print(
             #     f"CATEGORY: {None}",
```

### Comparing `not1mm-23.5.9.2/not1mm/plugins/arrl_dx_cw.py` & `not1mm-23.6.2/not1mm/plugins/arrl_dx_cw.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ARRL plugin"""
 
 # pylint: disable=invalid-name, unused-argument, unused-variable
 
 import logging
 from pathlib import Path
-
+from decimal import Decimal
 from PyQt5 import QtWidgets
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger("__main__")
 
 name = "ARRL DX CW"
 cabrillo_name = "ARRL-DX-CW"
@@ -178,15 +178,15 @@
             print("<ADIF_VER:5>2.2.0", end="\r\n", file=file_descriptor)
             print("<EOH>", end="\r\n", file=file_descriptor)
             for contact in log:
                 hiscall = contact.get("Call", "")
                 the_date_and_time = contact.get("TS")
                 # band = contact.get("Band")
                 themode = contact.get("Mode")
-                frequency = str(contact.get("Freq", 0) / 1000)
+                frequency = str(Decimal(str(contact.get("Freq", 0))) / 1000)
                 sentrst = contact.get("SNT", "")
                 rcvrst = contact.get("RCV", "")
                 sentnr = str(contact.get("SentNr", ""))
                 rcvnr = str(contact.get("NR", ""))
                 grid = contact.get("GridSquare", "")
                 comment = contact.get("ContestName", "")
                 loggeddate = the_date_and_time[:10]
@@ -325,19 +325,20 @@
                 file=file_descriptor,
             )
             print(
                 f"CATEGORY-TRANSMITTER: {self.contest_settings.get('TransmitterCategory','')}",
                 end="\r\n",
                 file=file_descriptor,
             )
-            print(
-                f"CATEGORY-OVERLAY: {self.contest_settings.get('OverlayCategory','')}",
-                end="\r\n",
-                file=file_descriptor,
-            )
+            if self.contest_settings.get("OverlayCategory", "") != "N/A":
+                print(
+                    f"CATEGORY-OVERLAY: {self.contest_settings.get('OverlayCategory','')}",
+                    end="\r\n",
+                    file=file_descriptor,
+                )
             print(
                 f"GRID-LOCATOR: {self.station.get('GridSquare','')}",
                 end="\r\n",
                 file=file_descriptor,
             )
             # print(
             #     f"CATEGORY: {None}",
```

### Comparing `not1mm-23.5.9.2/not1mm/plugins/arrl_dx_ssb.py` & `not1mm-23.6.2/not1mm/plugins/arrl_dx_ssb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ARRL plugin"""
 
 # pylint: disable=invalid-name, unused-argument, unused-variable
 
 import logging
 from pathlib import Path
-
+from decimal import Decimal
 from PyQt5 import QtWidgets
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger("__main__")
 
 name = "ARRL DX SSB"
 cabrillo_name = "ARRL-DX-SSB"
@@ -178,15 +178,15 @@
             print("<ADIF_VER:5>2.2.0", end="\r\n", file=file_descriptor)
             print("<EOH>", end="\r\n", file=file_descriptor)
             for contact in log:
                 hiscall = contact.get("Call", "")
                 the_date_and_time = contact.get("TS")
                 # band = contact.get("Band")
                 themode = contact.get("Mode")
-                frequency = str(contact.get("Freq", 0) / 1000)
+                frequency = str(Decimal(str(contact.get("Freq", 0))) / 1000)
                 sentrst = contact.get("SNT", "")
                 rcvrst = contact.get("RCV", "")
                 sentnr = str(contact.get("SentNr", ""))
                 rcvnr = str(contact.get("NR", ""))
                 grid = contact.get("GridSquare", "")
                 comment = contact.get("ContestName", "")
                 loggeddate = the_date_and_time[:10]
@@ -325,19 +325,20 @@
                 file=file_descriptor,
             )
             print(
                 f"CATEGORY-TRANSMITTER: {self.contest_settings.get('TransmitterCategory','')}",
                 end="\r\n",
                 file=file_descriptor,
             )
-            print(
-                f"CATEGORY-OVERLAY: {self.contest_settings.get('OverlayCategory','')}",
-                end="\r\n",
-                file=file_descriptor,
-            )
+            if self.contest_settings.get("OverlayCategory", "") != "N/A":
+                print(
+                    f"CATEGORY-OVERLAY: {self.contest_settings.get('OverlayCategory','')}",
+                    end="\r\n",
+                    file=file_descriptor,
+                )
             print(
                 f"GRID-LOCATOR: {self.station.get('GridSquare','')}",
                 end="\r\n",
                 file=file_descriptor,
             )
             # print(
             #     f"CATEGORY: {None}",
```

### Comparing `not1mm-23.5.9.2/not1mm/plugins/arrl_field_day.py` & `not1mm-23.6.2/not1mm/plugins/arrl_field_day.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """ARRL Field Day plugin"""
 
 # pylint: disable=invalid-name, unused-argument, unused-variable
 
 import logging
-
+from decimal import Decimal
 from pathlib import Path
 from PyQt5 import QtWidgets
 
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger("__main__")
 
@@ -168,15 +168,15 @@
             print("<ADIF_VER:5>2.2.0", end="\r\n", file=file_descriptor)
             print("<EOH>", end="\r\n", file=file_descriptor)
             for contact in log:
                 hiscall = contact.get("Call", "")
                 the_date_and_time = contact.get("TS")
                 # band = contact.get("Band")
                 themode = contact.get("Mode")
-                frequency = str(contact.get("Freq", 0) / 1000)
+                frequency = str(Decimal(str(contact.get("Freq", 0))) / 1000)
                 sentrst = contact.get("SNT", "")
                 rcvrst = contact.get("RCV", "")
                 sentnr = self.contest_settings.get("SentExchange", "")
                 rcvnr = f"{contact.get('Exchange1', '')} {contact.get('Sect', '')}"
                 grid = contact.get("GridSquare", "")
                 comment = contact.get("ContestName", "")
                 loggeddate = the_date_and_time[:10]
@@ -315,19 +315,20 @@
                 file=file_descriptor,
             )
             print(
                 f"CATEGORY-TRANSMITTER: {self.contest_settings.get('TransmitterCategory','')}",
                 end="\r\n",
                 file=file_descriptor,
             )
-            print(
-                f"CATEGORY-OVERLAY: {self.contest_settings.get('OverlayCategory','')}",
-                end="\r\n",
-                file=file_descriptor,
-            )
+            if self.contest_settings.get("OverlayCategory", "") != "N/A":
+                print(
+                    f"CATEGORY-OVERLAY: {self.contest_settings.get('OverlayCategory','')}",
+                    end="\r\n",
+                    file=file_descriptor,
+                )
             print(
                 f"GRID-LOCATOR: {self.station.get('GridSquare','')}",
                 end="\r\n",
                 file=file_descriptor,
             )
             # print(
             #     f"CATEGORY: {None}",
```

### Comparing `not1mm-23.5.9.2/not1mm/plugins/arrl_rtty_ru.py` & `not1mm-23.6.2/not1mm/plugins/arrl_rtty_ru.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/plugins/arrl_ss_cw.py` & `not1mm-23.6.2/not1mm/plugins/arrl_ss_cw.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """ARRL plugin"""
 
 # pylint: disable=invalid-name, unused-argument, unused-variable
 
 import logging
+from decimal import Decimal
 from pathlib import Path
 from PyQt5 import QtWidgets
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger("__main__")
 
 name = "ARRL Sweepstakes CW"
@@ -177,15 +178,15 @@
             print("<ADIF_VER:5>2.2.0", end="\r\n", file=file_descriptor)
             print("<EOH>", end="\r\n", file=file_descriptor)
             for contact in log:
                 hiscall = contact.get("Call", "")
                 the_date_and_time = contact.get("TS")
                 # band = contact.get("Band")
                 themode = contact.get("Mode")
-                frequency = str(contact.get("Freq", 0) / 1000)
+                frequency = str(Decimal(str(contact.get("Freq", 0))) / 1000)
                 sentrst = contact.get("SNT", "")
                 rcvrst = contact.get("RCV", "")
                 sentnr = f'{contact.get("SentNr", "")} {self.contest_settings.get("SentExchange","")}'
                 rcvnr = f'{contact.get("NR", "")} {contact.get("Prec", "")} {contact.get("Call", "")} {contact.get("CK", "")} {contact.get("Sect", "")}'
                 grid = contact.get("GridSquare", "")
                 comment = contact.get("ContestName", "")
                 loggeddate = the_date_and_time[:10]
@@ -324,19 +325,20 @@
                 file=file_descriptor,
             )
             print(
                 f"CATEGORY-TRANSMITTER: {self.contest_settings.get('TransmitterCategory','')}",
                 end="\r\n",
                 file=file_descriptor,
             )
-            print(
-                f"CATEGORY-OVERLAY: {self.contest_settings.get('OverlayCategory','')}",
-                end="\r\n",
-                file=file_descriptor,
-            )
+            if self.contest_settings.get("OverlayCategory", "") != "N/A":
+                print(
+                    f"CATEGORY-OVERLAY: {self.contest_settings.get('OverlayCategory','')}",
+                    end="\r\n",
+                    file=file_descriptor,
+                )
             print(
                 f"GRID-LOCATOR: {self.station.get('GridSquare','')}",
                 end="\r\n",
                 file=file_descriptor,
             )
             # print(
             #     f"CATEGORY: {None}",
```

### Comparing `not1mm-23.5.9.2/not1mm/plugins/arrl_ss_phone.py` & `not1mm-23.6.2/not1mm/plugins/arrl_ss_phone.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """ARRL plugin"""
 
 # pylint: disable=invalid-name, unused-argument, unused-variable
 
 import logging
+from decimal import Decimal
 from pathlib import Path
 from PyQt5 import QtWidgets
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger("__main__")
 
 name = "ARRL Sweepstakes Phone"
@@ -177,15 +178,15 @@
             print("<ADIF_VER:5>2.2.0", end="\r\n", file=file_descriptor)
             print("<EOH>", end="\r\n", file=file_descriptor)
             for contact in log:
                 hiscall = contact.get("Call", "")
                 the_date_and_time = contact.get("TS")
                 # band = contact.get("Band")
                 themode = contact.get("Mode")
-                frequency = str(contact.get("Freq", 0) / 1000)
+                frequency = str(Decimal(str(contact.get("Freq", 0))) / 1000)
                 sentrst = contact.get("SNT", "")
                 rcvrst = contact.get("RCV", "")
                 sentnr = f'{contact.get("SentNr", "")} {self.contest_settings.get("SentExchange","")}'
                 rcvnr = f'{contact.get("NR", "")} {contact.get("Prec", "")} {contact.get("Call", "")} {contact.get("CK", "")} {contact.get("Sect", "")}'
                 grid = contact.get("GridSquare", "")
                 comment = contact.get("ContestName", "")
                 loggeddate = the_date_and_time[:10]
@@ -324,19 +325,20 @@
                 file=file_descriptor,
             )
             print(
                 f"CATEGORY-TRANSMITTER: {self.contest_settings.get('TransmitterCategory','')}",
                 end="\r\n",
                 file=file_descriptor,
             )
-            print(
-                f"CATEGORY-OVERLAY: {self.contest_settings.get('OverlayCategory','')}",
-                end="\r\n",
-                file=file_descriptor,
-            )
+            if self.contest_settings.get("OverlayCategory", "") != "N/A":
+                print(
+                    f"CATEGORY-OVERLAY: {self.contest_settings.get('OverlayCategory','')}",
+                    end="\r\n",
+                    file=file_descriptor,
+                )
             print(
                 f"GRID-LOCATOR: {self.station.get('GridSquare','')}",
                 end="\r\n",
                 file=file_descriptor,
             )
             # print(
             #     f"CATEGORY: {None}",
```

### Comparing `not1mm-23.5.9.2/not1mm/plugins/cq_wpx_cw.py` & `not1mm-23.6.2/not1mm/plugins/cq_wpx_cw.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """CQ WPX CW plugin"""
 
 # pylint: disable=invalid-name
 import logging
+from decimal import Decimal
 from pathlib import Path
 
 from PyQt5 import QtWidgets
 
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger("__main__")
@@ -125,24 +126,32 @@
             mycontinent = item[1].get("continent", "")
     result = self.cty_lookup(self.contact.get("Call", ""))
     band = int(int(float(self.contact.get("Freq"))) / 1000)
     if result:
         for item in result.items():
             entity = item[1].get("entity", "")
             continent = item[1].get("continent", "")
-            if mycountry.upper() == entity.upper():
-                return 1
-            if mycontinent and continent == "NA":
+
+            # If both are in North America
+            if mycontinent == "NA" and continent == "NA":
                 if band in [28, 21, 14]:
                     return 2
                 return 4
+
+            # Not NA, Both in same country
+            if mycountry.upper() == entity.upper():
+                return 1
+
+            # Same Continent
             if mycontinent == continent:
                 if band in [28, 21, 14]:
                     return 1
                 return 2
+
+            # Different Continent
             if band in [28, 21, 14]:
                 return 3
             return 6
     return 0
 
 
 def show_mults(self):
@@ -198,15 +207,16 @@
             print("<ADIF_VER:5>2.2.0", end="\r\n", file=file_descriptor)
             print("<EOH>", end="\r\n", file=file_descriptor)
             for contact in log:
                 hiscall = contact.get("Call", "")
                 the_date_and_time = contact.get("TS")
                 # band = contact.get("Band")
                 themode = contact.get("Mode")
-                frequency = str(contact.get("Freq", 0) / 1000)
+                frequency = str(Decimal(str(contact.get("Freq", 0))) / 1000)
+                # frequency = str(contact.get("Freq", 0) / 1000)
                 sentrst = contact.get("SNT", "")
                 rcvrst = contact.get("RCV", "")
                 sentnr = str(contact.get("SentNr", "59"))
                 rcvnr = str(contact.get("NR", "59"))
                 grid = contact.get("GridSquare", "")
                 comment = contact.get("ContestName", "")
                 loggeddate = the_date_and_time[:10]
@@ -345,19 +355,20 @@
                 file=file_descriptor,
             )
             print(
                 f"CATEGORY-TRANSMITTER: {self.contest_settings.get('TransmitterCategory','')}",
                 end="\r\n",
                 file=file_descriptor,
             )
-            print(
-                f"CATEGORY-OVERLAY: {self.contest_settings.get('OverlayCategory','')}",
-                end="\r\n",
-                file=file_descriptor,
-            )
+            if self.contest_settings.get("OverlayCategory", "") != "N/A":
+                print(
+                    f"CATEGORY-OVERLAY: {self.contest_settings.get('OverlayCategory','')}",
+                    end="\r\n",
+                    file=file_descriptor,
+                )
             print(
                 f"GRID-LOCATOR: {self.station.get('GridSquare','')}",
                 end="\r\n",
                 file=file_descriptor,
             )
             # print(
             #     f"CATEGORY: {None}",
```

### Comparing `not1mm-23.5.9.2/not1mm/plugins/cq_wpx_ssb.py` & `not1mm-23.6.2/not1mm/plugins/cq_wpx_ssb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """CQ WPX SSB plugin"""
 
 # pylint: disable=invalid-name
 import logging
+from decimal import Decimal
 from pathlib import Path
 
 from PyQt5 import QtWidgets
 
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger("__main__")
@@ -127,24 +128,32 @@
             mycontinent = item[1].get("continent", "")
     result = self.cty_lookup(self.contact.get("Call", ""))
     band = int(int(float(self.contact.get("Freq"))) / 1000)
     if result:
         for item in result.items():
             entity = item[1].get("entity", "")
             continent = item[1].get("continent", "")
-            if mycountry.upper() == entity.upper():
-                return 1
-            if mycontinent and continent == "NA":
+
+            # If both are in North America
+            if mycontinent == "NA" and continent == "NA":
                 if band in [28, 21, 14]:
                     return 2
                 return 4
+
+            # Not NA, Both in same country
+            if mycountry.upper() == entity.upper():
+                return 1
+
+            # Same Continent
             if mycontinent == continent:
                 if band in [28, 21, 14]:
                     return 1
                 return 2
+
+            # Different Continent
             if band in [28, 21, 14]:
                 return 3
             return 6
     return 0
 
 
 def show_mults(self):
@@ -200,15 +209,15 @@
             print("<ADIF_VER:5>2.2.0", end="\r\n", file=file_descriptor)
             print("<EOH>", end="\r\n", file=file_descriptor)
             for contact in log:
                 hiscall = contact.get("Call", "")
                 the_date_and_time = contact.get("TS")
                 # band = contact.get("Band")
                 themode = contact.get("Mode")
-                frequency = str(contact.get("Freq", 0) / 1000)
+                frequency = str(Decimal(str(contact.get("Freq", 0))) / 1000)
                 sentrst = contact.get("SNT", "")
                 rcvrst = contact.get("RCV", "")
                 sentnr = str(contact.get("SentNr", "59"))
                 rcvnr = str(contact.get("NR", "59"))
                 grid = contact.get("GridSquare", "")
                 comment = contact.get("ContestName", "")
                 loggeddate = the_date_and_time[:10]
@@ -347,19 +356,20 @@
                 file=file_descriptor,
             )
             print(
                 f"CATEGORY-TRANSMITTER: {self.contest_settings.get('TransmitterCategory','')}",
                 end="\r\n",
                 file=file_descriptor,
             )
-            print(
-                f"CATEGORY-OVERLAY: {self.contest_settings.get('OverlayCategory','')}",
-                end="\r\n",
-                file=file_descriptor,
-            )
+            if self.contest_settings.get("OverlayCategory", "") != "N/A":
+                print(
+                    f"CATEGORY-OVERLAY: {self.contest_settings.get('OverlayCategory','')}",
+                    end="\r\n",
+                    file=file_descriptor,
+                )
             print(
                 f"GRID-LOCATOR: {self.station.get('GridSquare','')}",
                 end="\r\n",
                 file=file_descriptor,
             )
             # print(
             #     f"CATEGORY: {None}",
```

### Comparing `not1mm-23.5.9.2/not1mm/plugins/cq_ww_cw.py` & `not1mm-23.6.2/not1mm/plugins/cq_ww_ssb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-"""CQ World Wide DX CW plugin"""
+"""CQ World Wide DX SSB plugin"""
 
 # pylint: disable=invalid-name, unused-argument, unused-variable
 
 import logging
+from decimal import Decimal
 from pathlib import Path
 
 from PyQt5 import QtWidgets
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger("__main__")
 
-name = "CQ WW CW"
-cabrillo_name = "CQ-WW-CW"
-mode = "CW"  # CW SSB BOTH RTTY
+name = "CQ WW SSB"
+cabrillo_name = "CQ-WW-SSB"
+mode = "SSB"  # CW SSB BOTH RTTY
 # columns = [0, 1, 2, 3, 4, 5, 6, 15]
 columns = [
     "YYYY-MM-DD HH:MM:SS",
     "Call",
     "Freq",
     "Snt",
     "Rcv",
@@ -178,15 +179,15 @@
             print("<ADIF_VER:5>2.2.0", end="\r\n", file=file_descriptor)
             print("<EOH>", end="\r\n", file=file_descriptor)
             for contact in log:
                 hiscall = contact.get("Call", "")
                 the_date_and_time = contact.get("TS")
                 # band = contact.get("Band")
                 themode = contact.get("Mode")
-                frequency = str(contact.get("Freq", 0) / 1000)
+                frequency = str(Decimal(str(contact.get("Freq", 0))) / 1000)
                 sentrst = contact.get("SNT", "")
                 rcvrst = contact.get("RCV", "")
                 sentnr = str(contact.get("SentNr", ""))
                 rcvnr = str(contact.get("NR", ""))
                 grid = contact.get("GridSquare", "")
                 comment = contact.get("ContestName", "")
                 loggeddate = the_date_and_time[:10]
@@ -325,19 +326,20 @@
                 file=file_descriptor,
             )
             print(
                 f"CATEGORY-TRANSMITTER: {self.contest_settings.get('TransmitterCategory','')}",
                 end="\r\n",
                 file=file_descriptor,
             )
-            print(
-                f"CATEGORY-OVERLAY: {self.contest_settings.get('OverlayCategory','')}",
-                end="\r\n",
-                file=file_descriptor,
-            )
+            if self.contest_settings.get("OverlayCategory", "") != "N/A":
+                print(
+                    f"CATEGORY-OVERLAY: {self.contest_settings.get('OverlayCategory','')}",
+                    end="\r\n",
+                    file=file_descriptor,
+                )
             print(
                 f"GRID-LOCATOR: {self.station.get('GridSquare','')}",
                 end="\r\n",
                 file=file_descriptor,
             )
             # print(
             #     f"CATEGORY: {None}",
```

### Comparing `not1mm-23.5.9.2/not1mm/plugins/cq_ww_ssb.py` & `not1mm-23.6.2/not1mm/plugins/cq_ww_cw.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-"""CQ World Wide DX SSB plugin"""
+"""CQ World Wide DX CW plugin"""
 
 # pylint: disable=invalid-name, unused-argument, unused-variable
 
 import logging
+from decimal import Decimal
 from pathlib import Path
 
 from PyQt5 import QtWidgets
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger("__main__")
 
-name = "CQ WW SSB"
-cabrillo_name = "CQ-WW-SSB"
-mode = "SSB"  # CW SSB BOTH RTTY
+name = "CQ WW CW"
+cabrillo_name = "CQ-WW-CW"
+mode = "CW"  # CW SSB BOTH RTTY
 # columns = [0, 1, 2, 3, 4, 5, 6, 15]
 columns = [
     "YYYY-MM-DD HH:MM:SS",
     "Call",
     "Freq",
     "Snt",
     "Rcv",
@@ -178,15 +179,15 @@
             print("<ADIF_VER:5>2.2.0", end="\r\n", file=file_descriptor)
             print("<EOH>", end="\r\n", file=file_descriptor)
             for contact in log:
                 hiscall = contact.get("Call", "")
                 the_date_and_time = contact.get("TS")
                 # band = contact.get("Band")
                 themode = contact.get("Mode")
-                frequency = str(contact.get("Freq", 0) / 1000)
+                frequency = str(Decimal(str(contact.get("Freq", 0))) / 1000)
                 sentrst = contact.get("SNT", "")
                 rcvrst = contact.get("RCV", "")
                 sentnr = str(contact.get("SentNr", ""))
                 rcvnr = str(contact.get("NR", ""))
                 grid = contact.get("GridSquare", "")
                 comment = contact.get("ContestName", "")
                 loggeddate = the_date_and_time[:10]
@@ -325,19 +326,20 @@
                 file=file_descriptor,
             )
             print(
                 f"CATEGORY-TRANSMITTER: {self.contest_settings.get('TransmitterCategory','')}",
                 end="\r\n",
                 file=file_descriptor,
             )
-            print(
-                f"CATEGORY-OVERLAY: {self.contest_settings.get('OverlayCategory','')}",
-                end="\r\n",
-                file=file_descriptor,
-            )
+            if self.contest_settings.get("OverlayCategory", "") != "N/A":
+                print(
+                    f"CATEGORY-OVERLAY: {self.contest_settings.get('OverlayCategory','')}",
+                    end="\r\n",
+                    file=file_descriptor,
+                )
             print(
                 f"GRID-LOCATOR: {self.station.get('GridSquare','')}",
                 end="\r\n",
                 file=file_descriptor,
             )
             # print(
             #     f"CATEGORY: {None}",
```

### Comparing `not1mm-23.5.9.2/not1mm/plugins/cwt.py` & `not1mm-23.6.2/not1mm/plugins/cwt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """CWT plugin"""
 
 # pylint: disable=invalid-name, unused-argument, unused-variable
 
 import logging
+
+from decimal import Decimal
 from pathlib import Path
 
 from PyQt5 import QtWidgets
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger("__main__")
 name = "CWT"
@@ -180,15 +182,15 @@
             print("<ADIF_VER:5>2.2.0", end="\r\n", file=file_descriptor)
             print("<EOH>", end="\r\n", file=file_descriptor)
             for contact in log:
                 hiscall = contact.get("Call", "")
                 the_date_and_time = contact.get("TS")
                 # band = contact.get("Band")
                 themode = contact.get("Mode")
-                frequency = str(contact.get("Freq", 0) / 1000)
+                frequency = str(Decimal(str(contact.get("Freq", 0))) / 1000)
                 sentrst = contact.get("SNT", "")
                 rcvrst = contact.get("RCV", "")
                 sentnr = str(contact.get("SentNr", "").upper())
                 rcvnr = str(contact.get("NR", "").upper())
                 grid = contact.get("GridSquare", "")
                 comment = contact.get("ContestName", "")
                 loggeddate = the_date_and_time[:10]
@@ -327,19 +329,20 @@
                 file=file_descriptor,
             )
             print(
                 f"CATEGORY-TRANSMITTER: {self.contest_settings.get('TransmitterCategory','')}",
                 end="\r\n",
                 file=file_descriptor,
             )
-            print(
-                f"CATEGORY-OVERLAY: {self.contest_settings.get('OverlayCategory','')}",
-                end="\r\n",
-                file=file_descriptor,
-            )
+            if self.contest_settings.get("OverlayCategory", "") != "N/A":
+                print(
+                    f"CATEGORY-OVERLAY: {self.contest_settings.get('OverlayCategory','')}",
+                    end="\r\n",
+                    file=file_descriptor,
+                )
             print(
                 f"GRID-LOCATOR: {self.station.get('GridSquare','')}",
                 end="\r\n",
                 file=file_descriptor,
             )
             # print(
             #     f"CATEGORY: {None}",
```

### Comparing `not1mm-23.5.9.2/not1mm/plugins/general_logging.py` & `not1mm-23.6.2/not1mm/plugins/general_logging.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/plugins/jidx_cw.py` & `not1mm-23.6.2/not1mm/plugins/jidx_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/plugins/jidx_ph.py` & `not1mm-23.6.2/not1mm/plugins/jidx_ph.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm/plugins/winter_field_day.py` & `not1mm-23.6.2/not1mm/plugins/winter_field_day.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.2/not1mm.egg-info/PKG-INFO` & `not1mm-23.6.2/not1mm.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,79 +1,89 @@
 Metadata-Version: 2.1
 Name: not1mm
-Version: 23.5.9.2
+Version: 23.6.2
 Summary: NOT1MM Logger
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/not1mm
 Project-URL: Bug Tracker, https://github.com/mbridak/not1mm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Environment :: X11 Applications :: Qt
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Natural Language :: English
 Classifier: Topic :: Communications :: Ham Radio
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Not1MM
 
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
-[![Python: 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/)
+[![Python: 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/)
 [![Made With:PyQt5](https://img.shields.io/badge/Made%20with-PyQt5-red)](https://pypi.org/project/PyQt5/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/not1mm)](https://pypi.org/project/not1mm/)
 
 ![logo](https://github.com/mbridak/not1mm/raw/master/not1mm/data/k6gte.not1mm.svg)
 
 - [Not1MM](#not1mm)
   - [What and why is Not1MM](#what-and-why-is-not1mm)
   - [Current state](#current-state)
+  - [Thanks to the Contributors](#thanks-to-the-contributors)
+    - [:moneybag: Monitarily](#moneybag-monitarily)
+    - [:cockroach: Bug reports and Feature suggestions](#cockroach-bug-reports-and-feature-suggestions)
   - [List of should be working contests](#list-of-should-be-working-contests)
   - [Changes of note](#changes-of-note)
   - [Installing from PyPi](#installing-from-pypi)
     - [Python and pip](#python-and-pip)
     - [Installing with pip](#installing-with-pip)
-    - [Updating with pip](#updating-with-pip)
+      - [Ubuntu 22.04 LTS](#ubuntu-2204-lts)
+      - [Ubuntu 23.04](#ubuntu-2304)
+      - [Fedora 38](#fedora-38)
+    - [You may or may not get a warning message like](#you-may-or-may-not-get-a-warning-message-like)
+    - [Or this fan favorite](#or-this-fan-favorite)
+    - [Updating with pip/pipx](#updating-with-pippipx)
   - [Other Libraries](#other-libraries)
-  - [Running on Ubuntu LTS 22.04](#running-on-ubuntu-lts-2204)
+    - [Dark mode on Ubuntu](#dark-mode-on-ubuntu)
+  - [Wayland Compositor](#wayland-compositor)
   - [Running from source](#running-from-source)
   - [Various data file locations](#various-data-file-locations)
     - [Data](#data)
     - [Config](#config)
   - [The database](#the-database)
     - [Why](#why)
     - [The first one](#the-first-one)
     - [Why limit yourself](#why-limit-yourself)
     - [Revisiting an old friend](#revisiting-an-old-friend)
   - [Station Settings dialog](#station-settings-dialog)
     - [Changing station information](#changing-station-information)
   - [Adding a contest to the current dababase](#adding-a-contest-to-the-current-dababase)
   - [Selecting an existing contest as the current contest](#selecting-an-existing-contest-as-the-current-contest)
-  - [Editing an existing contest parameters](#editing-an-existing-contest-parameters)
+  - [Editing existing contest parameters](#editing-existing-contest-parameters)
   - [Configuration Settings](#configuration-settings)
     - [Lookup](#lookup)
     - [Soundcard](#soundcard)
     - [CAT](#cat)
     - [CW Keyer interface](#cw-keyer-interface)
     - [Cluster](#cluster)
+    - [N1MM Packets](#n1mm-packets)
   - [Hiding screen elements](#hiding-screen-elements)
   - [Editing macro keys](#editing-macro-keys)
     - [Macro substitutions](#macro-substitutions)
     - [Macro use with voice](#macro-use-with-voice)
   - [cty.dat and QRZ lookups for distance and bearing](#ctydat-and-qrz-lookups-for-distance-and-bearing)
   - [Other uses for the call field](#other-uses-for-the-call-field)
   - [Windows](#windows)
     - [The Main Window](#the-main-window)
       - [Keyboard commands](#keyboard-commands)
     - [Log Display](#log-display)
       - [Editing a contact](#editing-a-contact)
-    - [Bandmap](#bandmap)
   - [Recalulate Mults](#recalulate-mults)
+    - [Bandmap](#bandmap)
   - [Cabrillo](#cabrillo)
   - [ADIF](#adif)
   - [Dupe checking](#dupe-checking)
   - [Contest specific notes](#contest-specific-notes)
     - [ARRL Sweekstakes](#arrl-sweekstakes)
       - [The exchange parser](#the-exchange-parser)
       - [The exchange](#the-exchange)
@@ -93,14 +103,26 @@
 
 ## Current state
 
 The current state is "**BETA**". I've used it for A few contests, and was able to work contacts and submit a cabrillo at the end. I'm not a "Contester". So I'll add contests as/if I work them. I'm only one guy, so if you see a bug let me know. I don't do much of any Data or RTTY operating. This is why you don't see RTTY in the list of working contests. The Lord helps those who burn people at the... I mean who help themselves. Feel free to fill in that hole with a pull request.
 
 ![main screen](https://github.com/mbridak/not1mm/raw/master/pic/main.png)
 
+## Thanks to the Contributors
+
+I wish to thank those who've contributed to the project.
+
+### :moneybag: Monitarily
+
+Brian KB3ORR
+
+### :cockroach: Bug reports and Feature suggestions
+
+Simon G0FCU, Brian KB3ORR, Onno VK6FLAB, Martin OK1RR
+
 ## List of should be working contests
 
 - General Logging
 - 10 10 Fall CW
 - 10 10 Spring CW
 - 10 10 Summer Phone
 - 10 10 Winter Phone
@@ -114,23 +136,48 @@
 - CQ World Wide SSB
 - CWOps CWT
 - Japan International DX CW
 - Japan International DX SSB
 
 ## Changes of note
 
+- [23-6-2] Added an automated check and update of the cty.dat file. Added dependency to `notctyparser`
+
+<details>
+
+<summary>May 2023</summary>
+
+- [23-5-31] updated cty.json ( I need to automate this )
+- [23-5-30] Changed the default multicast group from 224.1.1.1 to 239.1.1.1 This restricts broadcast traffic to the local subnet.
+- [23-5-29] Hide CATEGORY-OVERLAY in Cabrillo file if set to N/A.
+- [23-5-28] Fixed Dupe check on TAB.
+- [23-5-27] Fixed frequency in the ADIF output. Corrected WPX contact points.
+- [23-5-26] Fixed Dark Mode on Ubuntu. Removed the crappy dark css theme and the code to load it. OOPS. Fixed some stuff.
+- [23-5-24] Added contact delete and change n1mm packets.
+- [23-5-23] Reworked N1MM packets. Can now specify multiple destinations for the packets.
+- [23-5-22] Worked on n1mm contactinfo packets. Reduced network beaconing from 100 miliseconds to 10 seconds, Unless the radio state changes.
+- [23-5-20] Got n1mm RadioInfo posting.
+- [23-5-19] Added a version check at startup. Starting work on N1MM packet broadcasts. Corrected flrig return value of bandwidth. Changed get Next/Prev bandmap spot to Arrow Up/Down.
+- [23-5-18] ReInit rigctld CAT when it goes offline and back.
+- [23-5-17] CTRL-G tunes to a spot matching text in the callsign entry field. Thanks to Martin, OK1RR for suggesting this. Bandmap centers on the VFO after frequency change. Set mode on startup based on the mode category set for the contest.
+- [23-5-15] CTRL-S in the main window will send a spot to the cluster.
+- [23-5-12] Bandmap, Reload system preferences before each connect. Increased the minimum Python version to 3.10. Main, Refactored UDP code to remove the use of timers and queues, replaced with readyRead signals.
+- [23-5-11] Added missing numpy package dependency to pyproject.toml. Added install steps for clean images of Fedora and Ubuntu. Entered frequencies when no CAT control are not sent to the bandmap. Added K1EL speed change via xmlrpc. One would need to update the pywinkeyerserial client.
+- [23-5-10] Fix crash in bandmap when No CAT, and using CTRL-PgUp/Down. Add specific Ubuntu install instructions.
 - [23-5-9] Removed 1 second timers in the bandmap and log window, made them UDP readyRead(). Much smoother. Add CTRL-PgUp and CTRL-PgDown keys to jump to the next/prev spots in the bandmap. Fix: Voice not keying on LSB. Fix: calling pttoff when no CAT interface. Fix: Voice not keying on LSB
 - [23-5-8] Bandmap zoom in/out now centers scale to RX Freq.
 - [23-5-7] Added bandwidth marker to the bandmap.
 - [23-5-6] Added AR Cluster filter options for the bandmap. Added a station ID to the multicast packets. This will prevent erratic bevahiour if 2 stations are on the same network.
 - [23-5-5] Re-wrote most of the log window code. Added ARRL Sweepstakes.
 - [23-5-4] Fixed 'Operators' line in WPX cabrillo file. Fix window title not updating if no CAT control.
 - [23-5-3] Added '#' macro.
 - [23-5-1] Added 10 10 CW and Phone contests. Added a `Cluster` TAB for the AR Cluster server/port in the configuration settings.
 
+</details>
+
 <details>
 
 <summary>April 2023</summary>
 
 - [23-4-29] Added callsign and connect button to the bandmap. Fixed rxmarker not updateing.
 - [23-4-28] Added a bandmap window (WIP) to track spots. Clicked spots now tune radio and sets callsign.
 - [23-4-24] CWT now prefills exchange based on past CWT contacts in database. Fixed crash when editing an existing contest that does not exist. Removed legacy stylesheet from configuration settings dialog.
@@ -188,42 +235,88 @@
 
 </details>
 
 ## Installing from PyPi
 
 ### Python and pip
 
-This software is a Python package hosted on PyPi, and installable with the pip command. If this is your first exposure to pip you can get all the details from [The PyPA](https://packaging.python.org/en/latest/tutorials/installing-packages/). In short, most linux distros come with Python pre installed. And pip usually comes with Python as a standard module. If pip is not installed by default, you can usually load it through your package manager. For example `sudo apt install python3-pip` or `sudo dnf install python3-pip`.
+This software is a Python package hosted on PyPi, and installable with the pip or pipx command. If this is your first exposure to pip you can get all the details from [The PyPA](https://packaging.python.org/en/latest/tutorials/installing-packages/). In short, most linux distros come with Python pre installed. If pip is not installed by default, you can usually load it through your package manager. For example `sudo apt install python3-pip` or `sudo dnf install python3-pip`.
 
 ### Installing with pip
 
-But just try `pip install not1mm` in your terminal. Once it's installed just type `not1mm` in the same terminal. On the first run, the program will install a launchable icon, which you can then click on to run like a normal program.
+I've included what installation steps I took to install on fresh images of Ubuntu and Fedora below. YMMV.
 
-### Updating with pip
+#### Ubuntu 22.04 LTS
 
-I've been posting updates just about everyday. Sometimes multiple times a day. It's early days, so there is much to do. You can check for and install updates with `pip install -U not1mm`.
+```bash
+sudo apt update
+sudo apt upgrade
+sudo apt install -y libportaudio2 python3-pip python3-pyqt5 python3-numpy adwaita-qt
+pip install -U not1mm
+```
 
-## Other Libraries
+#### Ubuntu 23.04
 
-The audio library used, uses pipewire/portaudio. You may need to install portaudio. Ubuntu: `sudo apt install libportaudio2`
+```bash
+sudo apt update
+sudo apt upgrade
+sudo apt install -y libportaudio2 adwaita-qt pipx
+pipx install not1mm
+pipx ensurepath
+```
+
+Open a new terminal and type `not1mm`
+
+#### Fedora 38
+
+```bash
+sudo dnf upgrade --refresh
+sudo dnf install python3-pip portaudio
+pip install not1mm
+```
+
+### You may or may not get a warning message like
 
-## Running on Ubuntu LTS 22.04
+```text
+WARNING: The script not1mm is installed in '/home/mbridak/.local/bin' which is not on PATH.
+Consider adding this directory to PATH or, if you prefer to suppress this warning, use --no-warn-script-location.
+```
+
+If you do, just logout and back in, or reboot.
 
-Seems Ubuntu LTS is not a big fan of wayland. When launching from the command line you'll see a message:
+### Or this fan favorite
 
-`Warning: Ignoring XDG_SESSION_TYPE=wayland on Gnome. Use QT_QPA_PLATFORM=wayland to run on Wayland anyway.
+```text
+Warning: Ignoring XDG_SESSION_TYPE=wayland on Gnome. Use QT_QPA_PLATFORM=wayland to run on Wayland anyway.
 qt.qpa.plugin: Could not load the Qt platform plugin "xcb" in "" even though it was found.
-This application failed to start because no Qt platform plugin could be initialized. Reinstalling the application may fix this problem.`
+This application failed to start because no Qt platform plugin could be initialized. Reinstalling the application may fix this problem.
+```
 
 To avoid this you can export an environment variable and launch the app like this:
 
 `mbridak@vm:~$ export QT_QPA_PLATFORM=wayland; not1mm`
 
 For a more permanent solution you can place the line `export QT_QPA_PLATFORM=wayland` in your home directories .bashrc file. Then after logging out and back in you should be able to launch it normally.
 
+### Updating with pip/pipx
+
+I've been posting updates just about everyday. Sometimes multiple times a day. It's early days, so there is much to do. You can check for and install updates with `pip install -U not1mm` or if installed with pipx `pipx upgrade not1mm`.
+
+## Other Libraries
+
+The audio library used, uses pipewire/portaudio. You may need to install portaudio. Ubuntu: `sudo apt install libportaudio2`
+
+### Dark mode on Ubuntu
+
+I believe I figured out dark mode in Ubuntu and have it working on my shack PC that runs Ubuntu 22.04. The secret sauce seems to be installing adwaita-qt with apt, and setting an environment variable `QT_STYLE_OVERRIDE` to `Adwaita-Dark`. I set the environment variable in the start of the program if running on a Gnome platform. So you don't need to do that part.
+
+## Wayland Compositor
+
+One side effect of Wayland is that we are not able to request for a window to regain or retain focus. So if you were to click on a spot in the bandmap window to tune to that spot, you would have to then click on the main window to continue entering contest data. I'm aware of this, but i can not change it.
+
 ## Running from source
 
 Since this is packaged for PyPi, if you want to work on your own source branch, after cloning from github you would:
 
 ```bash
 pip install --upgrade pip
 pip install setuptools
@@ -299,15 +392,15 @@
 
 ## Selecting an existing contest as the current contest
 
 Select `File` > `Open Contest`
 
 ![Open an existing contest](https://github.com/mbridak/not1mm/raw/master/pic/select_contest.png)
 
-## Editing an existing contest parameters
+## Editing existing contest parameters
 
 You can edit the parameters of a previously defined contest by selecting it as the current contest. Then select `File` > `Edit Current Contest`. Click `OK` to save the new values and reload the contest. `Cancel` to keep the existing parameters.
 
 ## Configuration Settings
 
 To setup your CAT control, CW keyer, Callsign lookups, select `File` > `Configuration Settings`
 
@@ -333,14 +426,22 @@
 
 ### Cluster
 
 ![Configuration Settings screen](https://github.com/mbridak/not1mm/raw/master/pic/configuration_cluster.png)
 
   Under the `Cluster` TAB you can change the default AR Cluster server, port and filter settings used for the bandmap window.
 
+### N1MM Packets
+
+Work has started on N1MM udp packets. So far just RadioInfo, contactinfo, contactreplace and contactdelete.
+
+![N1MM Packet Configuration Screen](https://github.com/mbridak/not1mm/blob/master/pic/n1mm_packet_config.png?raw=true)
+
+When entering IP and Ports, enter them with a colon ':' between them. You can enter multiple pairs on the same line if separated by a space ' '.
+
 ## Hiding screen elements
 
 You can show or hide certain buttons/indicators by checking and unchecking their boxes under the view menu. You can then resize the screen to make it more compact.
 
 ![View Menu](https://github.com/mbridak/not1mm/raw/master/pic/view_menu.png)
 
 The your choices will be remembered when you relaunch the program.
@@ -388,27 +489,31 @@
 
 **You must press the SPACE bar after entering any of the above.**
 
 ## Windows
 
 ### The Main Window
 
+![Main screen with callouts](https://github.com/mbridak/not1mm/raw/master/pic/mainwithcallouts.png)
+
 #### Keyboard commands
 
 - [Esc] Clears the input fields of any text.
 - [CTRL-Esc] Stops cwdaemon from sending Morse.
-- [PgUp] Increases the cwdaemon sending speed.
-- [PgDown] Decreases the cwdaemon sending speed.
-- [CTRL-PgUp] Jump to the next spot above the current VFO cursor in the bamdmap window.
-- [CTRL-PgDown] Jump to the next spot below the current VFO cursor in the bamdmap window.
+- [PgUp] Increases the cw sending speed.
+- [PgDown] Decreases the cw sending speed.
+- [Arrow-Up] Jump to the next spot above the current VFO cursor in the bandmap window.
+- [Arrow-Down] Jump to the next spot below the current VFO cursor in the bandmap window.
 - [TAB] Move cursor to the right one field.
 - [Shift-Tab] Move cursor left One field.
 - [SPACE] When in the callsign field, will move the input to the first field needed for the exchange.
 - [Enter] Submits the fields to the log.
 - [F1-F12] Send (CW or Voice) macros.
+- [CTRL-S] Spot Callsign to the cluster.
+- [CTRL-G] Tune to a spot matching partial text in the callsign entry field.
 
 ### Log Display
 
 `Window`>`Log Window`
 
 The Log display gets updated automatically when a contact is entered. The top half is a list of all contacts.
 
@@ -424,28 +529,28 @@
 
 You can also Right-Click on a cell to bring up the edit dialog.
 
 ![right click edit dialog](https://github.com/mbridak/not1mm/raw/master/pic/edit_dialog.png)
 
 You can not directly edit the multiplier status of a contact. Instead see the next section on recalculating mults. If you change the callsign make sure the `WPX` field is still valid.
 
+## Recalulate Mults
+
+After editing a contact and before generating a Cabrillo file. There is a Misc menu option that will recalculate the multipliers incase an edit had caused a change.
+
 ### Bandmap
 
 `Window`>`Bandmap`
 
 Put your callsign in the top and press the connect button.
 
 The bandmap window is, as with everything, a work in progress. The bandmap now follows the VFO. VFO indicator now displays as small triangle in the frequency tickmarks. A small blue rectangle shows the receivers bandwidth. Clicked on spots now tune the radio and set the callsign field.
 
 ![Bandmap Window](https://github.com/mbridak/not1mm/raw/master/pic/bandmap.png)
 
-## Recalulate Mults
-
-After editing a contact and before generating a Cabrillo file. There is a Misc menu option that will recalculate the multipliers incase an edit had caused a change.
-
 ## Cabrillo
 
 Click on `File` > `Generate Cabrillo`
 
 The file will be placed in your home directory. The name will be in the format of:
 
 `StationCall`_`ContestName`.log
```

### Comparing `not1mm-23.5.9.2/not1mm.egg-info/SOURCES.txt` & `not1mm-23.6.2/not1mm.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,25 +7,26 @@
 not1mm/logwindow.py
 not1mm.egg-info/PKG-INFO
 not1mm.egg-info/SOURCES.txt
 not1mm.egg-info/dependency_links.txt
 not1mm.egg-info/entry_points.txt
 not1mm.egg-info/requires.txt
 not1mm.egg-info/top_level.txt
-not1mm/data/Combinear.qss
 not1mm/data/JetBrainsMono-Regular.ttf
 not1mm/data/MASTER.SCP
 not1mm/data/about.ui
 not1mm/data/alpha bravo charlie delta.txt
 not1mm/data/bandmap.ui
 not1mm/data/check.png
 not1mm/data/configuration.ui
 not1mm/data/contests.sql
 not1mm/data/cty.json
+not1mm/data/cty_old.json
 not1mm/data/cwmacros.txt
+not1mm/data/donors.html
 not1mm/data/editcontact.ui
 not1mm/data/editmacro.ui
 not1mm/data/greendot.png
 not1mm/data/k6gte-not1mm.desktop
 not1mm/data/k6gte.not1mm-128.png
 not1mm/data/k6gte.not1mm-32.png
 not1mm/data/k6gte.not1mm-64.png
@@ -98,14 +99,15 @@
 not1mm/lib/lookup.py
 not1mm/lib/multicast.py
 not1mm/lib/n1mm.py
 not1mm/lib/new_contest.py
 not1mm/lib/select_contest.py
 not1mm/lib/settings.py
 not1mm/lib/version.py
+not1mm/lib/versiontest.py
 not1mm/plugins/10_10_fall_cw.py
 not1mm/plugins/10_10_spring_cw.py
 not1mm/plugins/10_10_summer_phone.py
 not1mm/plugins/10_10_winter_phone.py
 not1mm/plugins/__init__.py
 not1mm/plugins/arrl_dx_cw.py
 not1mm/plugins/arrl_dx_ssb.py
@@ -118,9 +120,12 @@
 not1mm/plugins/cq_ww_cw.py
 not1mm/plugins/cq_ww_ssb.py
 not1mm/plugins/cwt.py
 not1mm/plugins/general_logging.py
 not1mm/plugins/jidx_cw.py
 not1mm/plugins/jidx_ph.py
 not1mm/plugins/winter_field_day.py
+not1mm/testing/fakeflrig.py
+not1mm/testing/flrigclient.py
+not1mm/testing/n1mm_listener.py
 not1mm/testing/test.py
 testing/test.py
```

### Comparing `not1mm-23.5.9.2/pyproject.toml` & `not1mm-23.6.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "not1mm" 
-version = "23.5.9.2"
+version = "23.6.2"
 description = "NOT1MM Logger"
 readme = "README.md"
-requires-python = ">=3.9"
+requires-python = ">=3.10"
 authors = [
   { name="Michael Bridak", email="michael.bridak@gmail.com" },
 ]
 dependencies = [
     "PyQt5",
     "requests",
     "dicttoxml",
     "xmltodict",
     "psutil",
     "sounddevice",
     "soundfile",
+    "numpy",
+    "notctyparser",
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Environment :: X11 Applications :: Qt",
     "Operating System :: POSIX :: Linux",
@@ -35,13 +37,13 @@
 "Homepage" = "https://github.com/mbridak/not1mm"
 "Bug Tracker" = "https://github.com/mbridak/not1mm/issues"
 
 [tool.setuptools.packages.find]
 where = ["."]
 
 [tool.setuptools.package-data]
-"not1mm.data" = ["*.json", "*.txt", "*.SCP", "*.ui", "*.ttf", "*.desktop", "*.png", "*.qss", "*.sql",]
+"not1mm.data" = ["*.json", "*.txt", "*.SCP", "*.ui", "*.ttf", "*.desktop", "*.png", "*.qss", "*.sql", "*.html",]
 "not1mm.data.phonetics" = ["*.wav",]
 "not1mm.icon" = ["*.png",]
 
 [project.scripts]
 not1mm = "not1mm.__main__:run"
```

