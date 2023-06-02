# Comparing `tmp/auto-test-common-1.0.4.tar.gz` & `tmp/auto-test-common-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-test-common-1.0.4.tar", last modified: Thu Jun  1 00:49:05 2023, max compression
+gzip compressed data, was "auto-test-common-1.0.5.tar", last modified: Fri Jun  2 00:46:44 2023, max compression
```

## Comparing `auto-test-common-1.0.4.tar` & `auto-test-common-1.0.5.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-01 00:49:05.653901 auto-test-common-1.0.4/
--rw-r--r--   0 edz        (502) staff       (20)      547 2023-06-01 00:49:05.654078 auto-test-common-1.0.4/PKG-INFO
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-01 00:49:05.634508 auto-test-common-1.0.4/auto_test_common.egg-info/
--rw-r--r--   0 edz        (502) staff       (20)      547 2023-06-01 00:49:05.000000 auto-test-common-1.0.4/auto_test_common.egg-info/PKG-INFO
--rw-r--r--   0 edz        (502) staff       (20)     1505 2023-06-01 00:49:05.000000 auto-test-common-1.0.4/auto_test_common.egg-info/SOURCES.txt
--rw-r--r--   0 edz        (502) staff       (20)        1 2023-06-01 00:49:05.000000 auto-test-common-1.0.4/auto_test_common.egg-info/dependency_links.txt
--rw-r--r--   0 edz        (502) staff       (20)       56 2023-06-01 00:49:05.000000 auto-test-common-1.0.4/auto_test_common.egg-info/entry_points.txt
--rw-r--r--   0 edz        (502) staff       (20)      571 2023-06-01 00:49:05.000000 auto-test-common-1.0.4/auto_test_common.egg-info/requires.txt
--rw-r--r--   0 edz        (502) staff       (20)        7 2023-06-01 00:49:05.000000 auto-test-common-1.0.4/auto_test_common.egg-info/top_level.txt
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-01 00:49:05.634897 auto-test-common-1.0.4/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 auto-test-common-1.0.4/common/__init__.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-01 00:49:05.636244 auto-test-common-1.0.4/common/autotest/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 auto-test-common-1.0.4/common/autotest/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     8490 2023-05-09 01:49:15.000000 auto-test-common-1.0.4/common/autotest/base_requests.py
--rw-r--r--   0 edz        (502) staff       (20)     6429 2023-03-22 09:11:00.000000 auto-test-common-1.0.4/common/autotest/handle_allure.py
--rw-r--r--   0 edz        (502) staff       (20)    10703 2023-04-14 00:29:00.000000 auto-test-common-1.0.4/common/autotest/handle_assert.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-01 00:49:05.637543 auto-test-common-1.0.4/common/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 auto-test-common-1.0.4/common/common/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2126 2023-04-23 02:46:40.000000 auto-test-common-1.0.4/common/common/api_driver.py
--rw-r--r--   0 edz        (502) staff       (20)     3612 2023-05-30 05:55:54.000000 auto-test-common-1.0.4/common/common/constant.py
--rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 auto-test-common-1.0.4/common/common/test.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-01 00:49:05.638183 auto-test-common-1.0.4/common/config/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.0.4/common/config/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2429 2022-12-01 00:35:00.000000 auto-test-common-1.0.4/common/config/config.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-01 00:49:05.639230 auto-test-common-1.0.4/common/data/
--rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 auto-test-common-1.0.4/common/data/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    17370 2023-05-24 07:32:32.000000 auto-test-common-1.0.4/common/data/data_process.py
--rw-r--r--   0 edz        (502) staff       (20)     8641 2023-05-30 08:45:37.000000 auto-test-common-1.0.4/common/data/handle_common.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-01 00:49:05.641694 auto-test-common-1.0.4/common/db/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.0.4/common/db/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     3592 2023-05-15 07:43:20.000000 auto-test-common-1.0.4/common/db/handle_db.py
--rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 auto-test-common-1.0.4/common/db/handle_db_batch.py
--rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 auto-test-common-1.0.4/common/db/handle_mysqldb.py
--rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 auto-test-common-1.0.4/common/db/handle_oracle.py
--rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 auto-test-common-1.0.4/common/db/handle_sqlserver.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-01 00:49:05.644734 auto-test-common-1.0.4/common/file/
--rw-r--r--   0 edz        (502) staff       (20)     4508 2023-04-14 00:29:00.000000 auto-test-common-1.0.4/common/file/ReadFile.py
--rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 auto-test-common-1.0.4/common/file/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    11473 2023-05-31 08:51:34.000000 auto-test-common-1.0.4/common/file/handle_excel.py
--rw-r--r--   0 edz        (502) staff       (20)     2265 2023-05-25 07:52:43.000000 auto-test-common-1.0.4/common/file/handle_file.py
--rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 auto-test-common-1.0.4/common/file/handle_reques.py
--rw-r--r--   0 edz        (502) staff       (20)     2201 2022-10-24 01:09:00.000000 auto-test-common-1.0.4/common/file/handle_system.py
--rw-r--r--   0 edz        (502) staff       (20)     1000 2023-04-14 00:29:00.000000 auto-test-common-1.0.4/common/file/handle_yaml.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-01 00:49:05.645588 auto-test-common-1.0.4/common/mq/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.0.4/common/mq/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 auto-test-common-1.0.4/common/mq/handle_rabbit.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-01 00:49:05.648227 auto-test-common-1.0.4/common/plat/
--rw-r--r--   0 edz        (502) staff       (20)     3543 2023-05-31 01:13:42.000000 auto-test-common-1.0.4/common/plat/ATF_platform.py
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 auto-test-common-1.0.4/common/plat/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 auto-test-common-1.0.4/common/plat/jenkin_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     7851 2023-05-30 02:15:47.000000 auto-test-common-1.0.4/common/plat/jira_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     8129 2023-05-30 07:56:22.000000 auto-test-common-1.0.4/common/plat/mysql_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     8826 2023-05-31 01:13:42.000000 auto-test-common-1.0.4/common/plat/service_platform.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-01 00:49:05.653385 auto-test-common-1.0.4/common/plugin/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 auto-test-common-1.0.4/common/plugin/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1330 2023-01-16 07:33:00.000000 auto-test-common-1.0.4/common/plugin/allure_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     2054 2022-07-28 02:48:00.000000 auto-test-common-1.0.4/common/plugin/assert_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     8259 2023-05-31 03:06:08.000000 auto-test-common-1.0.4/common/plugin/atf_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     6768 2023-05-15 07:47:06.000000 auto-test-common-1.0.4/common/plugin/data_bus.py
--rw-r--r--   0 edz        (502) staff       (20)     3654 2023-05-27 02:43:55.000000 auto-test-common-1.0.4/common/plugin/data_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    12176 2023-05-31 03:06:08.000000 auto-test-common-1.0.4/common/plugin/file_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 auto-test-common-1.0.4/common/plugin/hooks_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    13130 2023-05-31 08:41:08.000000 auto-test-common-1.0.4/common/plugin/pytest_playwright.py
--rw-r--r--   0 edz        (502) staff       (20)    17708 2023-05-31 02:35:10.000000 auto-test-common-1.0.4/common/plugin/pytest_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      443 2023-06-01 00:49:05.654957 auto-test-common-1.0.4/setup.cfg
--rw-r--r--   0 edz        (502) staff       (20)     1784 2023-06-01 00:45:28.000000 auto-test-common-1.0.4/setup.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-02 00:46:44.934882 auto-test-common-1.0.5/
+-rw-r--r--   0 edz        (502) staff       (20)      547 2023-06-02 00:46:44.935072 auto-test-common-1.0.5/PKG-INFO
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-02 00:46:44.903854 auto-test-common-1.0.5/auto_test_common.egg-info/
+-rw-r--r--   0 edz        (502) staff       (20)      547 2023-06-02 00:46:44.000000 auto-test-common-1.0.5/auto_test_common.egg-info/PKG-INFO
+-rw-r--r--   0 edz        (502) staff       (20)     1534 2023-06-02 00:46:44.000000 auto-test-common-1.0.5/auto_test_common.egg-info/SOURCES.txt
+-rw-r--r--   0 edz        (502) staff       (20)        1 2023-06-02 00:46:44.000000 auto-test-common-1.0.5/auto_test_common.egg-info/dependency_links.txt
+-rw-r--r--   0 edz        (502) staff       (20)       56 2023-06-02 00:46:44.000000 auto-test-common-1.0.5/auto_test_common.egg-info/entry_points.txt
+-rw-r--r--   0 edz        (502) staff       (20)      571 2023-06-02 00:46:44.000000 auto-test-common-1.0.5/auto_test_common.egg-info/requires.txt
+-rw-r--r--   0 edz        (502) staff       (20)        7 2023-06-02 00:46:44.000000 auto-test-common-1.0.5/auto_test_common.egg-info/top_level.txt
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-02 00:46:44.904219 auto-test-common-1.0.5/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 auto-test-common-1.0.5/common/__init__.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-02 00:46:44.906762 auto-test-common-1.0.5/common/autotest/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 auto-test-common-1.0.5/common/autotest/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     8490 2023-05-09 01:49:15.000000 auto-test-common-1.0.5/common/autotest/base_requests.py
+-rw-r--r--   0 edz        (502) staff       (20)     6429 2023-03-22 09:11:00.000000 auto-test-common-1.0.5/common/autotest/handle_allure.py
+-rw-r--r--   0 edz        (502) staff       (20)    10703 2023-04-14 00:29:00.000000 auto-test-common-1.0.5/common/autotest/handle_assert.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-02 00:46:44.909167 auto-test-common-1.0.5/common/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 auto-test-common-1.0.5/common/common/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2126 2023-04-23 02:46:40.000000 auto-test-common-1.0.5/common/common/api_driver.py
+-rw-r--r--   0 edz        (502) staff       (20)     3612 2023-05-30 05:55:54.000000 auto-test-common-1.0.5/common/common/constant.py
+-rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 auto-test-common-1.0.5/common/common/test.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-02 00:46:44.910123 auto-test-common-1.0.5/common/config/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.0.5/common/config/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2429 2022-12-01 00:35:00.000000 auto-test-common-1.0.5/common/config/config.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-02 00:46:44.912890 auto-test-common-1.0.5/common/data/
+-rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 auto-test-common-1.0.5/common/data/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    17370 2023-05-24 07:32:32.000000 auto-test-common-1.0.5/common/data/data_process.py
+-rw-r--r--   0 edz        (502) staff       (20)     8641 2023-05-30 08:45:37.000000 auto-test-common-1.0.5/common/data/handle_common.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-02 00:46:44.917221 auto-test-common-1.0.5/common/db/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.0.5/common/db/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     3592 2023-05-15 07:43:20.000000 auto-test-common-1.0.5/common/db/handle_db.py
+-rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 auto-test-common-1.0.5/common/db/handle_db_batch.py
+-rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 auto-test-common-1.0.5/common/db/handle_mysqldb.py
+-rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 auto-test-common-1.0.5/common/db/handle_oracle.py
+-rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 auto-test-common-1.0.5/common/db/handle_sqlserver.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-02 00:46:44.922661 auto-test-common-1.0.5/common/file/
+-rw-r--r--   0 edz        (502) staff       (20)     4508 2023-04-14 00:29:00.000000 auto-test-common-1.0.5/common/file/ReadFile.py
+-rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 auto-test-common-1.0.5/common/file/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    11473 2023-05-31 08:51:34.000000 auto-test-common-1.0.5/common/file/handle_excel.py
+-rw-r--r--   0 edz        (502) staff       (20)     2265 2023-05-25 07:52:43.000000 auto-test-common-1.0.5/common/file/handle_file.py
+-rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 auto-test-common-1.0.5/common/file/handle_reques.py
+-rw-r--r--   0 edz        (502) staff       (20)     2201 2022-10-24 01:09:00.000000 auto-test-common-1.0.5/common/file/handle_system.py
+-rw-r--r--   0 edz        (502) staff       (20)      955 2023-06-01 02:02:40.000000 auto-test-common-1.0.5/common/file/handle_yaml.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-02 00:46:44.923573 auto-test-common-1.0.5/common/mq/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.0.5/common/mq/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 auto-test-common-1.0.5/common/mq/handle_rabbit.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-02 00:46:44.927568 auto-test-common-1.0.5/common/plat/
+-rw-r--r--   0 edz        (502) staff       (20)     3543 2023-05-31 01:13:42.000000 auto-test-common-1.0.5/common/plat/ATF_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 auto-test-common-1.0.5/common/plat/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 auto-test-common-1.0.5/common/plat/jenkin_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     7851 2023-05-30 02:15:47.000000 auto-test-common-1.0.5/common/plat/jira_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     8129 2023-05-30 07:56:22.000000 auto-test-common-1.0.5/common/plat/mysql_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     8826 2023-05-31 01:13:42.000000 auto-test-common-1.0.5/common/plat/service_platform.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-02 00:46:44.934555 auto-test-common-1.0.5/common/plugin/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 auto-test-common-1.0.5/common/plugin/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1330 2023-01-16 07:33:00.000000 auto-test-common-1.0.5/common/plugin/allure_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     2054 2022-07-28 02:48:00.000000 auto-test-common-1.0.5/common/plugin/assert_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     8259 2023-05-31 03:06:08.000000 auto-test-common-1.0.5/common/plugin/atf_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     6768 2023-05-15 07:47:06.000000 auto-test-common-1.0.5/common/plugin/data_bus.py
+-rw-r--r--   0 edz        (502) staff       (20)     3654 2023-05-27 02:43:55.000000 auto-test-common-1.0.5/common/plugin/data_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    12176 2023-05-31 03:06:08.000000 auto-test-common-1.0.5/common/plugin/file_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 auto-test-common-1.0.5/common/plugin/hooks_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    13130 2023-05-31 08:41:08.000000 auto-test-common-1.0.5/common/plugin/pytest_playwright.py
+-rw-r--r--   0 edz        (502) staff       (20)    17709 2023-06-02 00:46:37.000000 auto-test-common-1.0.5/common/plugin/pytest_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      617 2023-06-02 00:42:40.000000 auto-test-common-1.0.5/common/plugin/yaml_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      443 2023-06-02 00:46:44.935847 auto-test-common-1.0.5/setup.cfg
+-rw-r--r--   0 edz        (502) staff       (20)     1784 2023-06-01 00:45:28.000000 auto-test-common-1.0.5/setup.py
```

### Comparing `auto-test-common-1.0.4/PKG-INFO` & `auto-test-common-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-test-common
-Version: 1.0.4
+Version: 1.0.5
 Author: shiqiang.ou
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `auto-test-common-1.0.4/auto_test_common.egg-info/PKG-INFO` & `auto-test-common-1.0.5/auto_test_common.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-test-common
-Version: 1.0.4
+Version: 1.0.5
 Author: shiqiang.ou
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `auto-test-common-1.0.4/auto_test_common.egg-info/SOURCES.txt` & `auto-test-common-1.0.5/auto_test_common.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -46,8 +46,9 @@
 common/plugin/assert_plugin.py
 common/plugin/atf_plugin.py
 common/plugin/data_bus.py
 common/plugin/data_plugin.py
 common/plugin/file_plugin.py
 common/plugin/hooks_plugin.py
 common/plugin/pytest_playwright.py
-common/plugin/pytest_plugin.py
+common/plugin/pytest_plugin.py
+common/plugin/yaml_plugin.py
```

### Comparing `auto-test-common-1.0.4/auto_test_common.egg-info/requires.txt` & `auto-test-common-1.0.5/auto_test_common.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.4/common/autotest/base_requests.py` & `auto-test-common-1.0.5/common/autotest/base_requests.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.4/common/autotest/handle_allure.py` & `auto-test-common-1.0.5/common/autotest/handle_allure.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.4/common/autotest/handle_assert.py` & `auto-test-common-1.0.5/common/autotest/handle_assert.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.4/common/common/api_driver.py` & `auto-test-common-1.0.5/common/common/api_driver.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.4/common/common/constant.py` & `auto-test-common-1.0.5/common/common/constant.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.4/common/common/test.py` & `auto-test-common-1.0.5/common/common/test.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.4/common/config/config.py` & `auto-test-common-1.0.5/common/config/config.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.4/common/data/data_process.py` & `auto-test-common-1.0.5/common/data/data_process.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.4/common/data/handle_common.py` & `auto-test-common-1.0.5/common/data/handle_common.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.4/common/db/handle_db.py` & `auto-test-common-1.0.5/common/db/handle_db.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.4/common/db/handle_db_batch.py` & `auto-test-common-1.0.5/common/db/handle_db_batch.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.4/common/db/handle_mysqldb.py` & `auto-test-common-1.0.5/common/db/handle_mysqldb.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.4/common/db/handle_oracle.py` & `auto-test-common-1.0.5/common/db/handle_oracle.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.4/common/db/handle_sqlserver.py` & `auto-test-common-1.0.5/common/db/handle_sqlserver.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.4/common/file/ReadFile.py` & `auto-test-common-1.0.5/common/file/ReadFile.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.4/common/file/handle_excel.py` & `auto-test-common-1.0.5/common/file/handle_excel.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.4/common/file/handle_file.py` & `auto-test-common-1.0.5/common/file/handle_file.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.4/common/file/handle_reques.py` & `auto-test-common-1.0.5/common/file/handle_reques.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.4/common/file/handle_system.py` & `auto-test-common-1.0.5/common/file/handle_system.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.4/common/file/handle_yaml.py` & `auto-test-common-1.0.5/common/file/handle_yaml.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import yaml
 from common.data.handle_common import extractor
 
-from common.config.config import CONFIG_PATH
 from common.file.handle_system import adjust_path
 
 def get_yaml_data(filePath):
     """
     获取yaml文件信息返回JSON数据
     :param filePath: 文件名称
     :return: JOSN数据
```

### Comparing `auto-test-common-1.0.4/common/mq/handle_rabbit.py` & `auto-test-common-1.0.5/common/mq/handle_rabbit.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.4/common/plat/ATF_platform.py` & `auto-test-common-1.0.5/common/plat/ATF_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.4/common/plat/jenkin_platform.py` & `auto-test-common-1.0.5/common/plat/jenkin_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.4/common/plat/jira_platform.py` & `auto-test-common-1.0.5/common/plat/jira_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.4/common/plat/mysql_platform.py` & `auto-test-common-1.0.5/common/plat/mysql_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.4/common/plat/service_platform.py` & `auto-test-common-1.0.5/common/plat/service_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.4/common/plugin/allure_plugin.py` & `auto-test-common-1.0.5/common/plugin/allure_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.4/common/plugin/assert_plugin.py` & `auto-test-common-1.0.5/common/plugin/assert_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.4/common/plugin/atf_plugin.py` & `auto-test-common-1.0.5/common/plugin/atf_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.4/common/plugin/data_bus.py` & `auto-test-common-1.0.5/common/plugin/data_bus.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.4/common/plugin/data_plugin.py` & `auto-test-common-1.0.5/common/plugin/data_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.4/common/plugin/file_plugin.py` & `auto-test-common-1.0.5/common/plugin/file_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.4/common/plugin/hooks_plugin.py` & `auto-test-common-1.0.5/common/plugin/hooks_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.4/common/plugin/pytest_playwright.py` & `auto-test-common-1.0.5/common/plugin/pytest_playwright.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.4/common/plugin/pytest_plugin.py` & `auto-test-common-1.0.5/common/plugin/pytest_plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
             if caseStatus == Constant.STATUS_PRE:
                 info = ATFPlatForm.getCaseInfoByNameOrID(caseId, caseName)
                 scriptURL= info['script']
                 if scriptURL != '':
                     caseUrl = str(scriptURL).replace("(", "").replace(")", "")
                     _scriptPath = path.join(get_system_key(Constant.CURRENT_PATH), caseUrl.split('[')[0], )
                     logger.info(f"------用例信息:{str(_list)}  脚本路径:{_scriptPath}  准备执行-------")
-                    ServicePlatForm.updateByRunid(_list['caserunid'], Constant.STATUS_AUTOTEST, "")
+                    #ServicePlatForm.updateByRunid(_list['caserunid'], Constant.STATUS_AUTOTEST, "")
                     pytest.main(
                         args=['-vs', _scriptPath,f'--alluredir={TEST_TARGET_RESULTS_PATH}'])
                 else:
                     logger.info(f"-------用例信息:{str(_list)}   脚本路径:未关联脚本  无需执行------")
                     MysqlPlatForm.delete_autotest_script(caseId)
             else:
                 logger.info(f"------用例信息:{str(_list)}  执行完成-------")
```

### Comparing `auto-test-common-1.0.4/setup.py` & `auto-test-common-1.0.5/setup.py`

 * *Files identical despite different names*

