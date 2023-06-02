# Comparing `tmp/remotemanager-0.6.1.tar.gz` & `tmp/remotemanager-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remotemanager-0.6.1.tar", last modified: Fri May 26 07:15:24 2023, max compression
+gzip compressed data, was "remotemanager-0.6.2.tar", last modified: Fri Jun  2 13:40:16 2023, max compression
```

## Comparing `remotemanager-0.6.1.tar` & `remotemanager-0.6.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 07:15:24.321536 remotemanager-0.6.1/
--rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-20 09:36:43.000000 remotemanager-0.6.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1278 2023-05-26 07:15:24.321536 remotemanager-0.6.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      864 2023-05-15 13:29:14.000000 remotemanager-0.6.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1367 2023-05-26 07:15:10.000000 remotemanager-0.6.1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 07:15:24.317536 remotemanager-0.6.1/remotemanager/
--rw-rw-rw-   0 root         (0) root         (0)      481 2023-05-25 13:31:29.000000 remotemanager-0.6.1/remotemanager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 07:15:24.317536 remotemanager-0.6.1/remotemanager/connection/
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/connection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15152 2023-05-25 13:31:29.000000 remotemanager-0.6.1/remotemanager/connection/cmd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 07:15:24.317536 remotemanager-0.6.1/remotemanager/connection/computers/
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/connection/computers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12341 2023-05-24 13:40:42.000000 remotemanager-0.6.1/remotemanager/connection/computers/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1613 2023-05-24 13:40:42.000000 remotemanager-0.6.1/remotemanager/connection/computers/example.py
--rw-rw-rw-   0 root         (0) root         (0)     2970 2023-05-24 13:40:42.000000 remotemanager-0.6.1/remotemanager/connection/computers/options.py
--rw-rw-rw-   0 root         (0) root         (0)     1503 2023-05-25 07:31:16.000000 remotemanager-0.6.1/remotemanager/connection/computers/parsers.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-24 13:40:42.000000 remotemanager-0.6.1/remotemanager/connection/detect_locale_error.py
--rw-rw-rw-   0 root         (0) root         (0)     6672 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/connection/testing_object.py
--rw-rw-rw-   0 root         (0) root         (0)    24726 2023-05-25 13:31:29.000000 remotemanager-0.6.1/remotemanager/connection/url.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 07:15:24.317536 remotemanager-0.6.1/remotemanager/dataset/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    48903 2023-05-25 13:31:29.000000 remotemanager-0.6.1/remotemanager/dataset/dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     3947 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/dataset/dependency.py
--rw-rw-rw-   0 root         (0) root         (0)    22556 2023-05-25 13:31:29.000000 remotemanager-0.6.1/remotemanager/dataset/runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 07:15:24.317536 remotemanager-0.6.1/remotemanager/jupyter/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-20 09:36:43.000000 remotemanager-0.6.1/remotemanager/jupyter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4873 2023-05-22 10:40:03.000000 remotemanager-0.6.1/remotemanager/jupyter/magic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 07:15:24.317536 remotemanager-0.6.1/remotemanager/logging/
--rw-rw-rw-   0 root         (0) root         (0)     4043 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/logging/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6496 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/logging/log.py
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-20 09:36:43.000000 remotemanager-0.6.1/remotemanager/logging/quiet.py
--rw-rw-rw-   0 root         (0) root         (0)     1943 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/logging/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/logging/verbosity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 07:15:24.321536 remotemanager-0.6.1/remotemanager/serialisation/
--rw-rw-rw-   0 root         (0) root         (0)      497 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/serialisation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4038 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/serialisation/serial.py
--rw-rw-rw-   0 root         (0) root         (0)      402 2023-04-20 09:36:43.000000 remotemanager-0.6.1/remotemanager/serialisation/serialdill.py
--rw-rw-rw-   0 root         (0) root         (0)      427 2023-04-20 09:36:43.000000 remotemanager-0.6.1/remotemanager/serialisation/serialjson.py
--rw-rw-rw-   0 root         (0) root         (0)     1609 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/serialisation/serialjsonpickle.py
--rw-rw-rw-   0 root         (0) root         (0)     1000 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/serialisation/serialyaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 07:15:24.321536 remotemanager-0.6.1/remotemanager/storage/
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5351 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/storage/database.py
--rw-rw-rw-   0 root         (0) root         (0)     4901 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/storage/function.py
--rw-rw-rw-   0 root         (0) root         (0)     1053 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/storage/remotefunction.py
--rw-rw-rw-   0 root         (0) root         (0)    12263 2023-05-25 13:31:29.000000 remotemanager-0.6.1/remotemanager/storage/sendablemixin.py
--rw-rw-rw-   0 root         (0) root         (0)      980 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/storage/trackedfile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 07:15:24.321536 remotemanager-0.6.1/remotemanager/transport/
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/transport/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      541 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/transport/cp.py
--rw-rw-rw-   0 root         (0) root         (0)     2251 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/transport/rsync.py
--rw-rw-rw-   0 root         (0) root         (0)     3202 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/transport/scp.py
--rw-rw-rw-   0 root         (0) root         (0)     9230 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/transport/transport.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 07:15:24.321536 remotemanager-0.6.1/remotemanager/utils/
--rw-rw-rw-   0 root         (0) root         (0)     3860 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4505 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/utils/flags.py
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/utils/uuid.py
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-04-27 10:20:11.000000 remotemanager-0.6.1/remotemanager/utils/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 07:15:24.317536 remotemanager-0.6.1/remotemanager.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1278 2023-05-26 07:15:24.000000 remotemanager-0.6.1/remotemanager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1788 2023-05-26 07:15:24.000000 remotemanager-0.6.1/remotemanager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 07:15:24.000000 remotemanager-0.6.1/remotemanager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      163 2023-05-26 07:15:24.000000 remotemanager-0.6.1/remotemanager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-05-26 07:15:24.000000 remotemanager-0.6.1/remotemanager.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-26 07:15:24.321536 remotemanager-0.6.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-20 09:36:43.000000 remotemanager-0.6.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 13:40:16.220122 remotemanager-0.6.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-18 14:24:27.000000 remotemanager-0.6.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-06-02 13:40:16.220122 remotemanager-0.6.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      864 2023-05-15 12:45:06.000000 remotemanager-0.6.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1367 2023-05-30 02:49:50.000000 remotemanager-0.6.2/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 13:40:16.212123 remotemanager-0.6.2/remotemanager/
+-rw-rw-rw-   0 root         (0) root         (0)      481 2023-05-30 02:49:50.000000 remotemanager-0.6.2/remotemanager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 13:40:16.212123 remotemanager-0.6.2/remotemanager/connection/
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-04-27 12:56:19.000000 remotemanager-0.6.2/remotemanager/connection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15541 2023-05-30 02:49:50.000000 remotemanager-0.6.2/remotemanager/connection/cmd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 13:40:16.212123 remotemanager-0.6.2/remotemanager/connection/computers/
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-27 12:56:19.000000 remotemanager-0.6.2/remotemanager/connection/computers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12674 2023-05-31 07:19:00.000000 remotemanager-0.6.2/remotemanager/connection/computers/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1613 2023-05-24 13:29:09.000000 remotemanager-0.6.2/remotemanager/connection/computers/example.py
+-rw-rw-rw-   0 root         (0) root         (0)     2970 2023-05-24 13:29:09.000000 remotemanager-0.6.2/remotemanager/connection/computers/options.py
+-rw-rw-rw-   0 root         (0) root         (0)     1503 2023-05-25 09:38:01.000000 remotemanager-0.6.2/remotemanager/connection/computers/parsers.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-24 13:29:09.000000 remotemanager-0.6.2/remotemanager/connection/detect_locale_error.py
+-rw-rw-rw-   0 root         (0) root         (0)     6672 2023-04-27 12:56:19.000000 remotemanager-0.6.2/remotemanager/connection/testing_object.py
+-rw-rw-rw-   0 root         (0) root         (0)    24726 2023-05-26 06:15:35.000000 remotemanager-0.6.2/remotemanager/connection/url.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 13:40:16.212123 remotemanager-0.6.2/remotemanager/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-27 12:56:19.000000 remotemanager-0.6.2/remotemanager/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    48903 2023-05-25 09:38:01.000000 remotemanager-0.6.2/remotemanager/dataset/dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     3947 2023-04-27 12:56:19.000000 remotemanager-0.6.2/remotemanager/dataset/dependency.py
+-rw-rw-rw-   0 root         (0) root         (0)    22648 2023-06-01 14:41:40.000000 remotemanager-0.6.2/remotemanager/dataset/runner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 13:40:16.212123 remotemanager-0.6.2/remotemanager/jupyter/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 14:24:27.000000 remotemanager-0.6.2/remotemanager/jupyter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4873 2023-05-25 09:38:01.000000 remotemanager-0.6.2/remotemanager/jupyter/magic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 13:40:16.216122 remotemanager-0.6.2/remotemanager/logging/
+-rw-rw-rw-   0 root         (0) root         (0)     4043 2023-04-27 12:56:19.000000 remotemanager-0.6.2/remotemanager/logging/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6496 2023-04-27 12:56:19.000000 remotemanager-0.6.2/remotemanager/logging/log.py
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-18 14:24:27.000000 remotemanager-0.6.2/remotemanager/logging/quiet.py
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-05-31 11:11:40.000000 remotemanager-0.6.2/remotemanager/logging/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2023-04-27 12:56:19.000000 remotemanager-0.6.2/remotemanager/logging/verbosity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 13:40:16.216122 remotemanager-0.6.2/remotemanager/serialisation/
+-rw-rw-rw-   0 root         (0) root         (0)      497 2023-04-27 12:56:19.000000 remotemanager-0.6.2/remotemanager/serialisation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4038 2023-04-27 12:56:19.000000 remotemanager-0.6.2/remotemanager/serialisation/serial.py
+-rw-rw-rw-   0 root         (0) root         (0)      402 2023-04-18 14:24:27.000000 remotemanager-0.6.2/remotemanager/serialisation/serialdill.py
+-rw-rw-rw-   0 root         (0) root         (0)      427 2023-04-18 14:24:27.000000 remotemanager-0.6.2/remotemanager/serialisation/serialjson.py
+-rw-rw-rw-   0 root         (0) root         (0)     1609 2023-04-27 12:56:19.000000 remotemanager-0.6.2/remotemanager/serialisation/serialjsonpickle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1000 2023-04-27 12:56:19.000000 remotemanager-0.6.2/remotemanager/serialisation/serialyaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 13:40:16.216122 remotemanager-0.6.2/remotemanager/storage/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-27 12:56:19.000000 remotemanager-0.6.2/remotemanager/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5351 2023-04-27 12:56:19.000000 remotemanager-0.6.2/remotemanager/storage/database.py
+-rw-rw-rw-   0 root         (0) root         (0)     5244 2023-05-31 11:11:40.000000 remotemanager-0.6.2/remotemanager/storage/function.py
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2023-04-27 12:56:19.000000 remotemanager-0.6.2/remotemanager/storage/remotefunction.py
+-rw-rw-rw-   0 root         (0) root         (0)    11552 2023-05-31 11:11:40.000000 remotemanager-0.6.2/remotemanager/storage/sendablemixin.py
+-rw-rw-rw-   0 root         (0) root         (0)      980 2023-04-27 12:56:19.000000 remotemanager-0.6.2/remotemanager/storage/trackedfile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 13:40:16.216122 remotemanager-0.6.2/remotemanager/transport/
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-27 12:56:19.000000 remotemanager-0.6.2/remotemanager/transport/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      541 2023-04-27 12:56:19.000000 remotemanager-0.6.2/remotemanager/transport/cp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2251 2023-06-02 09:40:16.000000 remotemanager-0.6.2/remotemanager/transport/rsync.py
+-rw-rw-rw-   0 root         (0) root         (0)     2279 2023-06-02 10:52:35.000000 remotemanager-0.6.2/remotemanager/transport/scp.py
+-rw-rw-rw-   0 root         (0) root         (0)     9262 2023-06-02 09:40:16.000000 remotemanager-0.6.2/remotemanager/transport/transport.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 13:40:16.220122 remotemanager-0.6.2/remotemanager/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     3860 2023-04-27 12:56:19.000000 remotemanager-0.6.2/remotemanager/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4505 2023-04-27 12:56:19.000000 remotemanager-0.6.2/remotemanager/utils/flags.py
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-04-27 12:56:19.000000 remotemanager-0.6.2/remotemanager/utils/uuid.py
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-04-27 12:56:19.000000 remotemanager-0.6.2/remotemanager/utils/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 13:40:16.212123 remotemanager-0.6.2/remotemanager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-06-02 13:40:16.000000 remotemanager-0.6.2/remotemanager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1788 2023-06-02 13:40:16.000000 remotemanager-0.6.2/remotemanager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 13:40:16.000000 remotemanager-0.6.2/remotemanager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      163 2023-06-02 13:40:16.000000 remotemanager-0.6.2/remotemanager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-02 13:40:16.000000 remotemanager-0.6.2/remotemanager.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-02 13:40:16.220122 remotemanager-0.6.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-18 14:24:27.000000 remotemanager-0.6.2/setup.py
```

### Comparing `remotemanager-0.6.1/LICENSE` & `remotemanager-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.1/PKG-INFO` & `remotemanager-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotemanager
-Version: 0.6.1
+Version: 0.6.2
 Summary: remote run management tool
 Author-email: Louis Beal <louis.j.beal@gmail.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dill
```

### Comparing `remotemanager-0.6.1/README.md` & `remotemanager-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.1/pyproject.toml` & `remotemanager-0.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 [tool.pytest.ini_options]
 addopts = "--nbval --cov=remotemanager --cov-report term-missing --cov-append --nbval-sanitize-with ./tests/uuid_sanitise.cfg"
 
 [tool.coverage.report]
 omit = ["remotemanager/connection/computers/*"]
 
 [tool.bumpver]
-current_version = "0.6.1"
+current_version = "0.6.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "[clean] bump version {old_version} -> {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `remotemanager-0.6.1/remotemanager/connection/cmd.py` & `remotemanager-0.6.2/remotemanager/connection/cmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -140,15 +140,16 @@
             self._logger.info("Falling back to communicate()")
             return self.communicate()[attr]
 
         self._logger.info(f"attempting to access the subprocess {attr} attr")
         out = getattr(self._subprocess, attr, None)
         if out is not None:
             try:
-                return out.read()
+                self._stdout = str(out.read().strip())
+                return self._stdout
             except ValueError as E:
                 self._logger.info(f"ValueError on read: {str(E)}")
         self._logger.info("Falling back to communicate()")
 
         return self.communicate()[attr]
 
     @property
@@ -158,27 +159,33 @@
         to communicate with the subprocess in the case of an async run.
 
         Returns None if the command has not been executed yet.
 
         Returns (str):
             the stdout from the command execution
         """
+        if self._stdout is not None:
+            self._logger.info("returning cached stdout")
+            return self._stdout
         return self._get_return_attr("stdout")
 
     @property
     def stderr(self) -> str:
         """
         Directly returns the stderr from the cmd execution. Attempts
         to communicate with the subprocess in the case of an async run.
 
         Returns None if the command has not been executed yet.
 
         Returns (str):
             the stdout from the command execution
         """
+        if self._stderr is not None:
+            self._logger.info("returning cached stderr")
+            return self._stderr
         return self._get_return_attr("stderr")
 
     @property
     def pwd(self) -> str:
         """
         Present working directory at command execution
 
@@ -381,16 +388,18 @@
         elif not self.is_redirected:
             self._logger.info(f"communicating with process {self.pid}")
             std, err = self._communicate()
         else:
             self._logger.info("files are redirected, attempting to read")
             std, err = self._file_communicate()
 
-        self._stdout = std
-        self._stderr = err
+        if std is not None:
+            self._stdout = std.strip()
+        if err is not None:
+            self._stderr = err.strip()
 
         def format_output(string):
             if string is None:
                 return
 
             if len(string.split("\n")) <= 1:
                 return string
```

### Comparing `remotemanager-0.6.1/remotemanager/connection/computers/base.py` & `remotemanager-0.6.2/remotemanager/connection/computers/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,22 +67,23 @@
     @classmethod
     def from_dict(cls, spec: dict, **url_args):
         """
         Create a Computer class from a `spec` dictionary. The required values are:
 
         - resources:
             a dict of required resources for the machine (mpi, nodes, queue, etc)
-        - required_or:
-            list of resources, ONE of which is required. Note that this must be a LIST
         - resource_parser:
             a function which takes a dictionary of {resource: Option}, returning a list
             of valid jobscript lines
 
         You can also provide some optional arguments:
 
+        - required_or:
+            list of resources, ONE of which is required. Note that this must be a
+            _list_ of dicts, one for each or "block"
         - optional_resources:
             as with `resources`, but these will not be stored as required values
         - optional_defaults:
             provide defaults for the names given in optional_resources. When adding the
             optional arg, the optional_defaults will be checked to see if a default is
             provided
         - host:
@@ -242,33 +243,42 @@
 
         if len(optional) > 0:
             spec["optional_resources"] = optional
 
         if len(defaults) > 0:
             spec["optional_defaults"] = defaults
 
-        spec["resource_parser"] = self._parser
+        if isinstance(self._parser, Function):
+            spec["resource_parser"] = self._parser
+        else:
+            spec["resource_parser"] = Function(self.parser)
 
         return spec
 
     @classmethod
     def from_yaml(cls, filepath: str):
-        with open(filepath, "r") as o:
-            data = yaml.safe_load(o)
+        if isinstance(filepath, str):
+            with open(filepath, "r") as o:
+                data = yaml.safe_load(o)
+        else:
+            data = yaml.safe_load(filepath)
 
         # convert the parser back into a function
         data["resource_parser"] = Function.unpack(data["resource_parser"])
 
         return cls.from_dict(data)
 
     def to_yaml(self, filepath):
         data = self.serialise(self.to_dict())
 
-        with open(filepath, "w+") as o:
-            yaml.dump(data, o)
+        if isinstance(filepath, str):
+            with open(filepath, "w+") as o:
+                yaml.dump(data, o)
+        else:
+            yaml.dump(data, filepath)
 
     @classmethod
     def from_repo(
         cls,
         name: str,
         branch: str = "main",
         repo: str = "https://gitlab.com/l_sim/remotemanager-computers/",
@@ -285,17 +295,14 @@
             repo (str):
                 repo web address (defaults to main l_sim repo)
 
         Returns:
             BaseComputer instance
         """
         import requests
-
-        # from bs4 import BeautifulSoup
-
         from remotemanager.utils import ensure_filetype
 
         def download_file(file_url, filename):
             response = requests.get(file_url)
 
             if response.status_code == requests.codes.ok:
                 # Save the file
```

### Comparing `remotemanager-0.6.1/remotemanager/connection/computers/example.py` & `remotemanager-0.6.2/remotemanager/connection/computers/example.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.1/remotemanager/connection/computers/options.py` & `remotemanager-0.6.2/remotemanager/connection/computers/options.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.1/remotemanager/connection/computers/parsers.py` & `remotemanager-0.6.2/remotemanager/connection/computers/parsers.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.1/remotemanager/connection/testing_object.py` & `remotemanager-0.6.2/remotemanager/connection/testing_object.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.1/remotemanager/connection/url.py` & `remotemanager-0.6.2/remotemanager/connection/url.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.1/remotemanager/dataset/dataset.py` & `remotemanager-0.6.2/remotemanager/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.1/remotemanager/dataset/dependency.py` & `remotemanager-0.6.2/remotemanager/dataset/dependency.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.1/remotemanager/dataset/runner.py` & `remotemanager-0.6.2/remotemanager/dataset/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -701,14 +701,16 @@
 
         path = self.jobscript.local
         output = "\n".join(tmp)
         if write_file:
             self._logger.info(f"writing run script to {path}")
             with open(path, "w+") as o:
                 o.write(output)
+                # Make sure the script ends with a line break
+                o.write("\n")
             self.state = "jobscript written"
         else:
             self.state = "jobscript write skipped"
 
         return output
 
     @property
```

### Comparing `remotemanager-0.6.1/remotemanager/jupyter/magic.py` & `remotemanager-0.6.2/remotemanager/jupyter/magic.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.1/remotemanager/logging/__init__.py` & `remotemanager-0.6.2/remotemanager/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.1/remotemanager/logging/log.py` & `remotemanager-0.6.2/remotemanager/logging/log.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.1/remotemanager/logging/utils.py` & `remotemanager-0.6.2/remotemanager/logging/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,16 +40,14 @@
                 if type(v) in dispatch.keys():
                     v = format_iterable(iterable=v, exclude=exclude, indent=indent + 1)
                 ret.append(INDENT_CHAR * (indent - 1) + f"- {v}")
 
         return f"\n" + f"\n".join(ret)
 
     def treat_printable(inp):
-        if inp is None:
-            return "None"
         return f"{inp}"
 
     # can hit empty lists (often in recursion)
     # output looks nicer if they're output without formatting
     try:
         if len(iterable) == 0:
             return "\n" + INDENT_CHAR * indent + f"{iterable}"
```

### Comparing `remotemanager-0.6.1/remotemanager/logging/verbosity.py` & `remotemanager-0.6.2/remotemanager/logging/verbosity.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.1/remotemanager/serialisation/serial.py` & `remotemanager-0.6.2/remotemanager/serialisation/serial.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.1/remotemanager/serialisation/serialjsonpickle.py` & `remotemanager-0.6.2/remotemanager/serialisation/serialjsonpickle.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.1/remotemanager/serialisation/serialyaml.py` & `remotemanager-0.6.2/remotemanager/serialisation/serialyaml.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.1/remotemanager/storage/database.py` & `remotemanager-0.6.2/remotemanager/storage/database.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.1/remotemanager/storage/function.py` & `remotemanager-0.6.2/remotemanager/storage/function.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     Serialise function to an executable python file for transfer
 
     Args:
         func:
             python function for serialisation
     """
 
-    def __init__(self, func: typing.Callable):
+    def __init__(self, func: [typing.Callable, str]):
 
         self._logger.debug(f"creating new serialisable function for {func}")
 
         self._uuid = ""
         try:
             source = inspect.getsource(func)
             source = source.replace("@RemoteFunction", "").strip()
@@ -41,18 +41,28 @@
             self._logger.debug(f"updated signature to {self._signature}")
             rawsig = Function.get_raw_signature(source)
             self._logger.debug(f"raw typed signature detected as" f" {self._signature}")
             source = source.replace(rawsig, self._signature, 1)
 
             self._source = source
             self._fname = func.__name__
+
         except TypeError as e:
             if isinstance(func, str):
                 self._source = func
-                self._fname = "f"
+
+                # need to extract the name
+                name = "f"
+                signature = ")"
+                for line in func.split("\n"):
+                    if line.startswith("def"):
+                        name, signature = line.split("def ")[-1].split("(")
+                self._fname = name
+
+                self._signature = "(" + signature.strip(":")
             else:
                 raise e
         self._uuid = generate_uuid(self._source)
 
     def __call__(self, *args, **kwargs):
         return self.object(*args, **kwargs)
```

### Comparing `remotemanager-0.6.1/remotemanager/storage/remotefunction.py` & `remotemanager-0.6.2/remotemanager/storage/remotefunction.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.1/remotemanager/storage/sendablemixin.py` & `remotemanager-0.6.2/remotemanager/storage/sendablemixin.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,42 +53,26 @@
             (dict):
                 object payload
         """
         # remove any attributes not to be packaged
         # these objects are either not needed, or can be re-created on the
         # recipient end
         never_package = ["_logger", "_logobj"]
-
-        do_not_package = {}
-
         class_storage = get_class_storage(self)
 
         # if the object is a subclass, find the name of the parent by getting
         # the mro of the object, and extracting it from the set
-        parent_class_names = get_mro_classnames(self)
-        sub_block = set(do_not_package) & set(parent_class_names)
-
-        name_to_block = None
-        if class_storage["name"] in do_not_package:
-            # classname has extra attrs to block
-            name_to_block = class_storage["name"]
-        elif len(sub_block) != 0:
-            # parent class has extra attrs to block
-            name_to_block = list(sub_block)[0]
-
-        block = never_package
-        if name_to_block:
-            block += do_not_package[name_to_block]
+        # parent_class_names = get_mro_classnames(self)
 
         # if the class specifies a solo _do_not_package, add that
-        block += getattr(self.__class__, "_do_not_package", [])
+        never_package += getattr(self.__class__, "_do_not_package", [])
 
         payload = {}
         for k, v in self.__dict__.items():
-            if k in block:
+            if k in never_package:
                 payload[k] = {
                     CLASS_STORAGE_KEY: {
                         "mod": "remotemanager.storage.sendablemixin",
                         "name": "Unloaded",
                     }
                 }
                 continue
@@ -135,15 +119,15 @@
         Returns:
             re-created object
         """
 
         if data is None:
             if file is None:
                 raise ValueError(
-                    "please provide a data payload or filepath " "to read from"
+                    "please provide a data payload or filepath to read from"
                 )
             elif not os.path.isfile(file):
                 raise FileNotFoundError(f"could not find file {file}")
 
             with open(file, "r") as o:
                 data = yaml.safe_load(o)
 
@@ -160,19 +144,14 @@
         except IndexError:
             # if there's no keys in data, then we definitely don't have a uuid
             pass
 
         # create a new instance of this class
         new = cls.__new__(cls)
 
-        # update this object with the values extracted from the payload
-        if isinstance(data, str):
-            _logger.debug(f"importing from filename {data}")
-            data = yaml.safe_load(data)
-
         # this is REQUIRED to be separate to the return call
         new.inject_payload(data, limit)
 
         return new
 
     def inject_payload(self, payload: dict, limit: bool = True):
         """
```

### Comparing `remotemanager-0.6.1/remotemanager/storage/trackedfile.py` & `remotemanager-0.6.2/remotemanager/storage/trackedfile.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.1/remotemanager/transport/cp.py` & `remotemanager-0.6.2/remotemanager/transport/cp.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.1/remotemanager/transport/rsync.py` & `remotemanager-0.6.2/remotemanager/transport/rsync.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         if self.url.passfile is not None:
             password = f'--rsh="sshpass -f {self.url.passfile} ssh" '
 
         cmd = self._cmd
         inner_dir = ""
         if len(pathlib.Path(secondary).parts) > 1:
             # the target is a nested dir. If the whole tree doesn't exist,
-            # rsync with throw an error
+            # rsync will throw an error
             if ":" in secondary:
                 # target is a remote folder, use the --rsync-path hack
                 inner_dir = (
                     f'--rsync-path="mkdir -p ' f'{get_remote_dir(secondary)} && rsync" '
                 )
             else:
                 cmd = f"mkdir -p {secondary} && {self._cmd}"
```

### Comparing `remotemanager-0.6.1/remotemanager/transport/transport.py` & `remotemanager-0.6.2/remotemanager/transport/transport.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,29 +3,30 @@
 """
 import os.path
 
 from remotemanager.storage.sendablemixin import SendableMixin
 from remotemanager.utils import ensure_list, ensure_dir
 from remotemanager.logging import LoggingMixin
 from remotemanager.utils.flags import Flags
+from remotemanager.connection import URL
 
 
 class Transport(SendableMixin, LoggingMixin):
     """
     Baseclass for file transfer
 
     Args:
         url (URL):
             url to extract remote address from
     """
 
     def __init__(self, url=None, *args, **kwargs):
 
         self._remote_address = None
-        self._url = None
+        self._url = url if url is not None else URL()
         self.set_remote(url)
 
         self._flags = Flags()
         self._transfers = {}
 
     def queue_for_push(self, files: list, local: str = None, remote: str = None):
         """
@@ -200,15 +201,14 @@
         """
         self._remote_address = remote_address
 
     @property
     def url(self):
         if self._url is not None:
             return self._url
-        from remotemanager import URL
 
         return URL()
 
     @url.setter
     def url(self, url):
         self._url = url
```

### Comparing `remotemanager-0.6.1/remotemanager/utils/__init__.py` & `remotemanager-0.6.2/remotemanager/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.1/remotemanager/utils/flags.py` & `remotemanager-0.6.2/remotemanager/utils/flags.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.1/remotemanager/utils/version.py` & `remotemanager-0.6.2/remotemanager/utils/version.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.1/remotemanager.egg-info/PKG-INFO` & `remotemanager-0.6.2/remotemanager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotemanager
-Version: 0.6.1
+Version: 0.6.2
 Summary: remote run management tool
 Author-email: Louis Beal <louis.j.beal@gmail.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dill
```

### Comparing `remotemanager-0.6.1/remotemanager.egg-info/SOURCES.txt` & `remotemanager-0.6.2/remotemanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

