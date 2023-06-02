# Comparing `tmp/nonebot_plugin_l4d2_server-0.5.5.1.tar.gz` & `tmp/nonebot_plugin_l4d2_server-0.5.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_l4d2_server-0.5.5.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_l4d2_server-0.5.5.2.tar", max compression
```

## Comparing `nonebot_plugin_l4d2_server-0.5.5.1.tar` & `nonebot_plugin_l4d2_server-0.5.5.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0    35149 2023-05-28 14:28:09.257050 nonebot_plugin_l4d2_server-0.5.5.1/LICENSE
--rw-r--r--   0        0        0    11703 2023-05-28 14:28:09.257050 nonebot_plugin_l4d2_server-0.5.5.1/README.md
--rw-r--r--   0        0        0    17532 2023-05-28 14:28:09.261050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/__init__.py
--rw-r--r--   0        0        0   158357 2023-05-28 14:28:09.261050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
--rw-r--r--   0        0        0   631630 2023-05-28 14:28:09.261050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
--rw-r--r--   0        0        0   405369 2023-05-28 14:28:09.265050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
--rw-r--r--   0        0        0     1590 2023-05-28 14:28:09.265050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
--rw-r--r--   0        0        0   242997 2023-05-28 14:28:09.265050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
--rw-r--r--   0        0        0     2135 2023-05-28 14:28:09.265050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
--rw-r--r--   0        0        0     6135 2023-05-28 14:28:09.265050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
--rw-r--r--   0        0        0     6170 2023-05-28 14:28:09.265050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
--rw-r--r--   0        0        0     1523 2023-05-28 14:28:09.265050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
--rw-r--r--   0        0        0     5506 2023-05-28 14:28:09.265050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
--rw-r--r--   0        0        0     2408 2023-05-28 14:28:09.265050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
--rw-r--r--   0        0        0     7874 2023-05-28 14:28:09.265050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
--rw-r--r--   0        0        0      486 2023-05-28 14:28:09.265050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
--rw-r--r--   0        0        0     1350 2023-05-28 14:28:09.265050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/data/img/white.png
--rw-r--r--   0        0        0     8734 2023-05-28 14:28:09.265050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
--rw-r--r--   0        0        0     1610 2023-05-28 14:28:09.265050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
--rw-r--r--   0        0        0     3010 2023-05-28 14:28:09.269050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
--rw-r--r--   0        0        0     1694 2023-05-28 14:28:09.269050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_anne/server.py
--rw-r--r--   0        0        0      359 2023-05-28 14:28:09.269050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
--rw-r--r--   0        0        0     3252 2023-05-28 14:28:09.269050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
--rw-r--r--   0        0        0      468 2023-05-28 14:28:09.269050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_data/config.py
--rw-r--r--   0        0        0        0 2023-05-28 14:28:09.269050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_data/database.py
--rw-r--r--   0        0        0     3232 2023-05-28 14:28:09.269050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_data/players.py
--rw-r--r--   0        0        0     1295 2023-05-28 14:28:09.269050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
--rw-r--r--   0        0        0     4097 2023-05-28 14:28:09.269050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
--rw-r--r--   0        0        0     1906 2023-05-28 14:28:09.269050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
--rw-r--r--   0        0        0     1860 2023-05-28 14:28:09.269050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_file/input_json.py
--rw-r--r--   0        0        0     2688 2023-05-28 14:28:09.269050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_file/remote.py
--rw-r--r--   0        0        0     4148 2023-05-28 14:28:09.269050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
--rw-r--r--   0        0        0     4007 2023-05-28 14:28:09.269050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_image/download.py
--rw-r--r--   0        0        0     1038 2023-05-28 14:28:09.269050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
--rw-r--r--   0        0        0     9524 2023-05-28 14:28:09.269050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_image/image.py
--rw-r--r--   0        0        0     1073 2023-05-28 14:28:09.269050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_image/one.py
--rw-r--r--   0        0        0      936 2023-05-28 14:28:09.269050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
--rw-r--r--   0        0        0     3799 2023-05-28 14:28:09.269050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_image/steam.py
--rw-r--r--   0        0        0     1387 2023-05-28 14:28:09.269050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
--rw-r--r--   0        0        0     7415 2023-05-28 14:28:09.269050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_push/__init__.py
--rw-r--r--   0        0        0     3735 2023-05-28 14:28:09.269050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
--rw-r--r--   0        0        0     1157 2023-05-28 14:28:09.269050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_queries/api.py
--rw-r--r--   0        0        0     1191 2023-05-28 14:28:09.269050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
--rw-r--r--   0        0        0    10855 2023-05-28 14:28:09.269050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
--rw-r--r--   0        0        0     1615 2023-05-28 14:28:09.269050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 14:28:09.269050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_server/index.py
--rw-r--r--   0        0        0     1248 2023-05-28 14:28:09.269050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
--rw-r--r--   0        0        0     1359 2023-05-28 14:28:09.269050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
--rw-r--r--   0        0        0     4113 2023-05-28 14:28:09.269050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_update/__init__.py
--rw-r--r--   0        0        0     1175 2023-05-28 14:28:09.269050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py
--rw-r--r--   0        0        0     2024 2023-05-28 14:28:09.269050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_update/restart.py
--rw-r--r--   0        0        0     1417 2023-05-28 14:28:09.269050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_update/update.py
--rw-r--r--   0        0        0     9768 2023-05-28 14:28:09.269050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_utils/command.py
--rw-r--r--   0        0        0     6275 2023-05-28 14:28:09.269050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_utils/config.py
--rw-r--r--   0        0        0     1620 2023-05-28 14:28:09.269050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_utils/message.py
--rw-r--r--   0        0        0      337 2023-05-28 14:28:09.269050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_utils/rule.py
--rw-r--r--   0        0        0      992 2023-05-28 14:28:09.269050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_utils/seach.py
--rw-r--r--   0        0        0     2133 2023-05-28 14:28:09.269050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py
--rw-r--r--   0        0        0     8928 2023-05-28 14:28:09.269050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_utils/utils.py
--rw-r--r--   0        0        0     8575 2023-05-28 14:28:09.273050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_web/web.py
--rw-r--r--   0        0        0    14159 2023-05-28 14:28:09.273050 nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
--rw-r--r--   0        0        0     1452 2023-05-28 14:28:09.273050 nonebot_plugin_l4d2_server-0.5.5.1/pyproject.toml
--rw-r--r--   0        0        0    13580 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.5.5.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-02 03:01:33.088849 nonebot_plugin_l4d2_server-0.5.5.2/LICENSE
+-rw-r--r--   0        0        0    11703 2023-06-02 03:01:33.088849 nonebot_plugin_l4d2_server-0.5.5.2/README.md
+-rw-r--r--   0        0        0    17532 2023-06-02 03:01:33.092849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/__init__.py
+-rw-r--r--   0        0        0   158357 2023-06-02 03:01:33.096850 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
+-rw-r--r--   0        0        0   631630 2023-06-02 03:01:33.096850 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
+-rw-r--r--   0        0        0   405369 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
+-rw-r--r--   0        0        0     1590 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
+-rw-r--r--   0        0        0   242997 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
+-rw-r--r--   0        0        0     2135 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
+-rw-r--r--   0        0        0     6135 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
+-rw-r--r--   0        0        0     6170 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
+-rw-r--r--   0        0        0     1523 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
+-rw-r--r--   0        0        0     5506 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
+-rw-r--r--   0        0        0     2408 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
+-rw-r--r--   0        0        0     7874 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
+-rw-r--r--   0        0        0      486 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
+-rw-r--r--   0        0        0     1350 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/img/white.png
+-rw-r--r--   0        0        0     8734 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
+-rw-r--r--   0        0        0     1610 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
+-rw-r--r--   0        0        0     3010 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
+-rw-r--r--   0        0        0     1694 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_anne/server.py
+-rw-r--r--   0        0        0      359 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
+-rw-r--r--   0        0        0     3252 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
+-rw-r--r--   0        0        0      468 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_data/config.py
+-rw-r--r--   0        0        0        0 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_data/database.py
+-rw-r--r--   0        0        0     3232 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_data/players.py
+-rw-r--r--   0        0        0     1295 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
+-rw-r--r--   0        0        0     4097 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
+-rw-r--r--   0        0        0     1906 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
+-rw-r--r--   0        0        0     1860 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_file/input_json.py
+-rw-r--r--   0        0        0     2688 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_file/remote.py
+-rw-r--r--   0        0        0     4148 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
+-rw-r--r--   0        0        0     4007 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_image/download.py
+-rw-r--r--   0        0        0     1038 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
+-rw-r--r--   0        0        0     9524 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_image/image.py
+-rw-r--r--   0        0        0     1073 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_image/one.py
+-rw-r--r--   0        0        0      936 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
+-rw-r--r--   0        0        0     3799 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_image/steam.py
+-rw-r--r--   0        0        0     1387 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
+-rw-r--r--   0        0        0     7415 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_push/__init__.py
+-rw-r--r--   0        0        0     3735 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
+-rw-r--r--   0        0        0     1157 2023-06-02 03:01:33.104850 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_queries/api.py
+-rw-r--r--   0        0        0     1191 2023-06-02 03:01:33.104850 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
+-rw-r--r--   0        0        0    10855 2023-06-02 03:01:33.104850 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
+-rw-r--r--   0        0        0     1615 2023-06-02 03:01:33.104850 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-02 03:01:33.104850 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_server/index.py
+-rw-r--r--   0        0        0     1248 2023-06-02 03:01:33.104850 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
+-rw-r--r--   0        0        0     1359 2023-06-02 03:01:33.104850 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
+-rw-r--r--   0        0        0     4113 2023-06-02 03:01:33.104850 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_update/__init__.py
+-rw-r--r--   0        0        0     1175 2023-06-02 03:01:33.104850 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py
+-rw-r--r--   0        0        0     2024 2023-06-02 03:01:33.104850 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_update/restart.py
+-rw-r--r--   0        0        0     1417 2023-06-02 03:01:33.104850 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_update/update.py
+-rw-r--r--   0        0        0     9724 2023-06-02 03:01:33.104850 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_utils/command.py
+-rw-r--r--   0        0        0     6275 2023-06-02 03:01:33.104850 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_utils/config.py
+-rw-r--r--   0        0        0     1620 2023-06-02 03:01:33.104850 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_utils/message.py
+-rw-r--r--   0        0        0      337 2023-06-02 03:01:33.104850 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_utils/rule.py
+-rw-r--r--   0        0        0      992 2023-06-02 03:01:33.104850 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_utils/seach.py
+-rw-r--r--   0        0        0     2133 2023-06-02 03:01:33.104850 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py
+-rw-r--r--   0        0        0     8928 2023-06-02 03:01:33.104850 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_utils/utils.py
+-rw-r--r--   0        0        0     8575 2023-06-02 03:01:33.104850 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_web/web.py
+-rw-r--r--   0        0        0    14159 2023-06-02 03:01:33.104850 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
+-rw-r--r--   0        0        0     1453 2023-06-02 03:01:33.104850 nonebot_plugin_l4d2_server-0.5.5.2/pyproject.toml
+-rw-r--r--   0        0        0    13572 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.5.5.2/PKG-INFO
```

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/LICENSE` & `nonebot_plugin_l4d2_server-0.5.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/README.md` & `nonebot_plugin_l4d2_server-0.5.5.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/data/img/white.png` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/img/white.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_anne/server.py` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_anne/server.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_data/__init__.py` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_data/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_data/players.py` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_data/players.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_data/serverip.py` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_data/serverip.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_file/__init__.py` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_file/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_file/input_json.py` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_file/input_json.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_file/remote.py` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_file/remote.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_image/__init__.py` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_image/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_image/download.py` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_image/download.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_image/image.py` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_image/image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_image/one.py` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_image/one.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_image/steam.py` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_image/steam.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_push/__init__.py` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_push/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_queries/api.py` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_queries/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_server/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_server/rcon.py` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_server/rcon.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_server/workshop.py` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_server/workshop.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_update/__init__.py` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_update/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_update/restart.py` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_update/restart.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_update/update.py` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_update/update.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_utils/command.py` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_utils/command.py`

 * *Files 3% similar despite different names*

```diff
@@ -175,38 +175,37 @@
         
     
     
 async def get_read_ip(ip_anne_list):    
     get_ip = on_command('anne',aliases=server_key(),priority=80,block=True)
     @get_ip.handle()
     async def _(matcher:Matcher,start:str = CommandStart(),command: str = RawCommand(),args:Message = CommandArg()):
-        global matchers
-        if get_ip.plugin_name not in matchers:
-            matchers[get_ip.plugin_name] = []
-        matchers[get_ip.plugin_name].append(get_ip)
+        # global matchers
+        # if get_ip.plugin_name not in matchers:
+        #     matchers[get_ip.plugin_name] = []
+        # matchers[get_ip.plugin_name].append(get_ip)
         if start:
             command = command.replace(start,'')
         if command == 'anne':
             command = '云'
         msg:str = args.extract_plain_text()
         push_msg = await get_ip_to_mes(msg, command)
         if isinstance(push_msg ,bytes):
             await matcher.finish(MessageSegment.image(push_msg))
         elif msg and isinstance(push_msg ,list):
             await matcher.finish(MessageSegment.image(push_msg[0]) + Message(push_msg[-1]))
         elif msg and isinstance(push_msg ,str):
-            try:
-                await matcher.finish(push_msg)
-            except nonebot.adapters.onebot.v11.exception.ActionFailed:
+            if l4_config.l4_image:
                 lines = push_msg.splitlines()
                 first_str = lines[0]
                 last_str = lines[-1]
                 push_msg = '\n'.join(lines[1:-1])
                 await matcher.finish(mode_txt_to_img(first_str,push_msg)+Message(last_str))
-                
+            else:
+                await matcher.finish(push_msg)
 
 async def get_ip_to_mes(msg:str ,command: str = ''):   
     if not msg:
         # 以图片输出全部当前
         igr = False
         if command in gamemode_list:
             this_ips = [d for l in ALL_HOST.values() for d in l if d.get('version') == command]
```

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_utils/config.py` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_utils/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_utils/message.py` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_utils/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_utils/seach.py` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_utils/seach.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_utils/utils.py` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_utils/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_web/web.py` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_web/web.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/nonebot_plugin_l4d2_server/l4d2_web/webUI.py` & `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_web/webUI.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/pyproject.toml` & `nonebot_plugin_l4d2_server-0.5.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-l4d2-server"
-version = "0.5.5.1"
+version = "0.5.5.2"
 description = "L4D2 server related operations plugin for NoneBot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 repository = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 keywords = ["steam", "game", "l4d2", "nonebot2", "plugin"]
@@ -26,15 +26,15 @@
 nonebot-adapter-onebot = ">=2.1.5"
 nonebot_plugin_htmlrender = "^0.2.0.1"
 nonebot_plugin_txt2img = ">=0.3.0"
 nonebot_plugin_apscheduler = "^0.2.0"
 asyncio = ">=3.4.3"
 jinja2 = ">=3.0.0"
 srctools="^2.3.9"
-httpx = "^0.23.3"
+httpx = ">=0.23.3"
 beautifulsoup4 = ">=4.8.0"
 rcon = "^2.1.0"
 pillow = "^9.3.0"
 aiohttp = "^3.8.3"
 pyunpack = "^0.3.0"
 "ruamel.yaml" = "^0.17.21"
 rarfile = "^4.0"
```

### Comparing `nonebot_plugin_l4d2_server-0.5.5.1/PKG-INFO` & `nonebot_plugin_l4d2_server-0.5.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-l4d2-server
-Version: 0.5.5.1
+Version: 0.5.5.2
 Summary: L4D2 server related operations plugin for NoneBot2
 Home-page: https://github.com/Agnes4m/nonebot_plugin_l4d2_server
 License: GPLv3
 Keywords: steam,game,l4d2,nonebot2,plugin
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Requires-Dist: amis-python (>=1.0.6,<2.0.0)
 Requires-Dist: asyncio (>=3.4.3)
 Requires-Dist: attrs (>=23.1.0,<24.0.0)
 Requires-Dist: beautifulsoup4 (>=4.8.0)
 Requires-Dist: gitpython (>=3.1.27)
-Requires-Dist: httpx (>=0.23.3,<0.24.0)
+Requires-Dist: httpx (>=0.23.3)
 Requires-Dist: jieba (>=0.42.1,<0.43.0)
 Requires-Dist: jinja2 (>=3.0.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.1.5)
 Requires-Dist: nonebot2 (>=2.0.0rc4,<3.0.0)
 Requires-Dist: nonebot_plugin_apscheduler (>=0.2.0,<0.3.0)
 Requires-Dist: nonebot_plugin_htmlrender (>=0.2.0.1,<0.3.0.0)
 Requires-Dist: nonebot_plugin_txt2img (>=0.3.0)
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.5.5.1
+Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.5.5.2
 Summary: L4D2 server related operations plugin for NoneBot2 Home-page: https://
 github.com/Agnes4m/nonebot_plugin_l4d2_server License: GPLv3 Keywords:
 steam,game,l4d2,nonebot2,plugin Author: Agnes_Digital Author-email:
 Z735803792@163.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0) Requires-Dist: amis-python
 (>=1.0.6,<2.0.0) Requires-Dist: asyncio (>=3.4.3) Requires-Dist: attrs
 (>=23.1.0,<24.0.0) Requires-Dist: beautifulsoup4 (>=4.8.0) Requires-Dist:
-gitpython (>=3.1.27) Requires-Dist: httpx (>=0.23.3,<0.24.0) Requires-Dist:
-jieba (>=0.42.1,<0.43.0) Requires-Dist: jinja2 (>=3.0.0) Requires-Dist:
-nonebot-adapter-onebot (>=2.1.5) Requires-Dist: nonebot2 (>=2.0.0rc4,<3.0.0)
-Requires-Dist: nonebot_plugin_apscheduler (>=0.2.0,<0.3.0) Requires-Dist:
+gitpython (>=3.1.27) Requires-Dist: httpx (>=0.23.3) Requires-Dist: jieba
+(>=0.42.1,<0.43.0) Requires-Dist: jinja2 (>=3.0.0) Requires-Dist: nonebot-
+adapter-onebot (>=2.1.5) Requires-Dist: nonebot2 (>=2.0.0rc4,<3.0.0) Requires-
+Dist: nonebot_plugin_apscheduler (>=0.2.0,<0.3.0) Requires-Dist:
 nonebot_plugin_htmlrender (>=0.2.0.1,<0.3.0.0) Requires-Dist:
 nonebot_plugin_txt2img (>=0.3.0) Requires-Dist: pandas (>=1.5.2) Requires-Dist:
 patool (>=1.12,<2.0) Requires-Dist: pillow (>=9.3.0,<10.0.0) Requires-Dist:
 python-a2s (>=1.3.0,<2.0.0) Requires-Dist: python-jose (>=3.3.0,<4.0.0)
 Requires-Dist: pyunpack (>=0.3.0,<0.4.0) Requires-Dist: rarfile (>=4.0,<5.0)
 Requires-Dist: rcon (>=2.1.0,<3.0.0) Requires-Dist: ruamel.yaml
 (>=0.17.21,<0.18.0) Requires-Dist: srctools (>=2.3.9,<3.0.0) Project-URL:
```

