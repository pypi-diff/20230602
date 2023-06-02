# Comparing `tmp/sqla_inspect-0.7.4.tar.gz` & `tmp/sqla_inspect-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqla_inspect-0.7.4.tar", last modified: Tue Oct 18 09:47:57 2022, max compression
+gzip compressed data, was "sqla_inspect-0.7.5.tar", last modified: Fri Jun  2 07:59:04 2023, max compression
```

## Comparing `sqla_inspect-0.7.4.tar` & `sqla_inspect-0.7.5.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2022-10-18 09:47:57.888628 sqla_inspect-0.7.4/
--rw-r--r--   0 gas       (1000) gas       (1000)    35147 2020-09-22 12:42:13.000000 sqla_inspect-0.7.4/LICENSE.txt
--rw-r--r--   0 gas       (1000) gas       (1000)      103 2020-09-22 12:42:13.000000 sqla_inspect-0.7.4/MANIFEST.in
--rw-r--r--   0 gas       (1000) gas       (1000)      602 2022-10-18 09:47:57.888628 sqla_inspect-0.7.4/PKG-INFO
--rw-r--r--   0 gas       (1000) gas       (1000)      616 2020-10-02 10:07:10.000000 sqla_inspect-0.7.4/README.rst
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2022-10-18 09:47:57.874628 sqla_inspect-0.7.4/docs/
--rw-r--r--   0 gas       (1000) gas       (1000)     5944 2020-09-22 12:42:13.000000 sqla_inspect-0.7.4/docs/Makefile
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2022-10-18 09:47:57.875628 sqla_inspect-0.7.4/docs/source/
--rw-r--r--   0 gas       (1000) gas       (1000)     8336 2020-09-22 12:42:13.000000 sqla_inspect-0.7.4/docs/source/conf.py
--rw-r--r--   0 gas       (1000) gas       (1000)     8329 2021-06-08 16:30:38.000000 sqla_inspect-0.7.4/docs/source/export.rst
--rw-r--r--   0 gas       (1000) gas       (1000)      476 2020-09-22 12:42:13.000000 sqla_inspect-0.7.4/docs/source/index.rst
--rw-r--r--   0 gas       (1000) gas       (1000)       73 2020-09-22 12:42:13.000000 sqla_inspect-0.7.4/docs/source/modules.rst
--rw-r--r--   0 gas       (1000) gas       (1000)     1116 2020-09-22 12:42:13.000000 sqla_inspect-0.7.4/docs/source/sqla_inspect.rst
--rw-r--r--   0 gas       (1000) gas       (1000)      380 2020-09-22 12:42:13.000000 sqla_inspect-0.7.4/docs/source/sqla_inspect.tests.rst
--rw-r--r--   0 gas       (1000) gas       (1000)       77 2021-06-14 12:45:32.000000 sqla_inspect-0.7.4/requirements.txt
--rw-r--r--   0 gas       (1000) gas       (1000)      184 2022-10-18 09:47:57.888628 sqla_inspect-0.7.4/setup.cfg
--rw-r--r--   0 gas       (1000) gas       (1000)     1133 2022-10-18 09:47:28.000000 sqla_inspect-0.7.4/setup.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2022-10-18 09:47:57.876628 sqla_inspect-0.7.4/sqla_inspect/
--rw-r--r--   0 gas       (1000) gas       (1000)       22 2022-10-14 14:46:56.000000 sqla_inspect-0.7.4/sqla_inspect/__init__.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2022-10-18 09:47:57.886628 sqla_inspect-0.7.4/sqla_inspect/__pycache__/
--rw-r--r--   0 gas       (1000) gas       (1000)      278 2021-10-25 11:27:03.000000 sqla_inspect-0.7.4/sqla_inspect/__pycache__/__init__.cpython-37-pytest-6.2.1.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)      160 2021-06-08 15:13:32.000000 sqla_inspect-0.7.4/sqla_inspect/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)      164 2020-09-23 09:42:43.000000 sqla_inspect-0.7.4/sqla_inspect/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)      278 2022-10-14 14:41:17.000000 sqla_inspect-0.7.4/sqla_inspect/__pycache__/__init__.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)      164 2022-10-14 16:57:54.000000 sqla_inspect-0.7.4/sqla_inspect/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     2663 2021-06-08 15:13:34.000000 sqla_inspect-0.7.4/sqla_inspect/__pycache__/ascii.cpython-37.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     2693 2020-10-02 16:03:04.000000 sqla_inspect-0.7.4/sqla_inspect/__pycache__/ascii.cpython-38.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     2797 2022-10-14 14:46:16.000000 sqla_inspect-0.7.4/sqla_inspect/__pycache__/ascii.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     2688 2022-10-14 16:58:06.000000 sqla_inspect-0.7.4/sqla_inspect/__pycache__/ascii.cpython-39.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     3914 2021-10-25 11:27:03.000000 sqla_inspect-0.7.4/sqla_inspect/__pycache__/base.cpython-37-pytest-6.2.1.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     3801 2021-06-08 15:13:32.000000 sqla_inspect-0.7.4/sqla_inspect/__pycache__/base.cpython-37.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     3856 2020-09-23 09:42:43.000000 sqla_inspect-0.7.4/sqla_inspect/__pycache__/base.cpython-38.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     3973 2022-10-14 14:46:16.000000 sqla_inspect-0.7.4/sqla_inspect/__pycache__/base.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     3864 2022-10-14 16:57:54.000000 sqla_inspect-0.7.4/sqla_inspect/__pycache__/base.cpython-39.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     6469 2021-10-25 11:27:04.000000 sqla_inspect-0.7.4/sqla_inspect/__pycache__/csv.cpython-37-pytest-6.2.1.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     6356 2021-06-08 15:13:32.000000 sqla_inspect-0.7.4/sqla_inspect/__pycache__/csv.cpython-37.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     5950 2020-10-02 16:03:02.000000 sqla_inspect-0.7.4/sqla_inspect/__pycache__/csv.cpython-38.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     6287 2022-10-14 14:46:16.000000 sqla_inspect-0.7.4/sqla_inspect/__pycache__/csv.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     6178 2022-10-14 16:57:54.000000 sqla_inspect-0.7.4/sqla_inspect/__pycache__/csv.cpython-39.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     8832 2021-10-25 11:27:04.000000 sqla_inspect-0.7.4/sqla_inspect/__pycache__/excel.cpython-37-pytest-6.2.1.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     8719 2021-07-20 10:08:28.000000 sqla_inspect-0.7.4/sqla_inspect/__pycache__/excel.cpython-37.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     8820 2020-10-02 16:03:02.000000 sqla_inspect-0.7.4/sqla_inspect/__pycache__/excel.cpython-38.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     9072 2022-10-14 14:46:16.000000 sqla_inspect-0.7.4/sqla_inspect/__pycache__/excel.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     8963 2022-10-14 16:57:54.000000 sqla_inspect-0.7.4/sqla_inspect/__pycache__/excel.cpython-39.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)    10946 2021-10-25 11:27:04.000000 sqla_inspect-0.7.4/sqla_inspect/__pycache__/export.cpython-37-pytest-6.2.1.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)    10833 2021-06-08 15:13:32.000000 sqla_inspect-0.7.4/sqla_inspect/__pycache__/export.cpython-37.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)    10737 2020-10-02 16:03:02.000000 sqla_inspect-0.7.4/sqla_inspect/__pycache__/export.cpython-38.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)    11020 2022-10-14 14:46:16.000000 sqla_inspect-0.7.4/sqla_inspect/__pycache__/export.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)    10911 2022-10-14 16:57:54.000000 sqla_inspect-0.7.4/sqla_inspect/__pycache__/export.cpython-39.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     7045 2021-10-25 11:27:03.000000 sqla_inspect-0.7.4/sqla_inspect/__pycache__/ods.cpython-37-pytest-6.2.1.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     6932 2021-06-08 15:13:32.000000 sqla_inspect-0.7.4/sqla_inspect/__pycache__/ods.cpython-37.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     6979 2020-10-02 16:03:02.000000 sqla_inspect-0.7.4/sqla_inspect/__pycache__/ods.cpython-38.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     7378 2022-10-14 14:46:16.000000 sqla_inspect-0.7.4/sqla_inspect/__pycache__/ods.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     7269 2022-10-14 16:57:54.000000 sqla_inspect-0.7.4/sqla_inspect/__pycache__/ods.cpython-39.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     9453 2021-06-08 15:13:34.000000 sqla_inspect-0.7.4/sqla_inspect/__pycache__/py3o.cpython-37.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     9513 2020-11-02 22:35:23.000000 sqla_inspect-0.7.4/sqla_inspect/__pycache__/py3o.cpython-38.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     9609 2022-10-14 14:46:17.000000 sqla_inspect-0.7.4/sqla_inspect/__pycache__/py3o.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     9500 2022-10-14 16:58:11.000000 sqla_inspect-0.7.4/sqla_inspect/__pycache__/py3o.cpython-39.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     4333 2021-06-08 15:13:34.000000 sqla_inspect-0.7.4/sqla_inspect/__pycache__/py3o_tmpl.cpython-37.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     4337 2020-09-25 08:35:12.000000 sqla_inspect-0.7.4/sqla_inspect/__pycache__/py3o_tmpl.cpython-38.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     4451 2022-10-14 14:46:17.000000 sqla_inspect-0.7.4/sqla_inspect/__pycache__/py3o_tmpl.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     4337 2022-10-14 16:58:11.000000 sqla_inspect-0.7.4/sqla_inspect/__pycache__/py3o_tmpl.cpython-39.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     2360 2022-10-14 14:45:01.000000 sqla_inspect-0.7.4/sqla_inspect/ascii.py
--rw-r--r--   0 gas       (1000) gas       (1000)     3043 2022-10-14 14:45:59.000000 sqla_inspect-0.7.4/sqla_inspect/base.py
--rw-r--r--   0 gas       (1000) gas       (1000)     6354 2022-10-14 14:46:03.000000 sqla_inspect-0.7.4/sqla_inspect/csv.py
--rw-r--r--   0 gas       (1000) gas       (1000)     9465 2022-10-18 09:47:01.000000 sqla_inspect-0.7.4/sqla_inspect/excel.py
--rw-r--r--   0 gas       (1000) gas       (1000)    13654 2022-10-14 14:46:07.000000 sqla_inspect-0.7.4/sqla_inspect/export.py
--rw-r--r--   0 gas       (1000) gas       (1000)     7252 2022-10-14 14:46:08.000000 sqla_inspect-0.7.4/sqla_inspect/ods.py
--rw-r--r--   0 gas       (1000) gas       (1000)    12084 2022-10-14 14:46:11.000000 sqla_inspect-0.7.4/sqla_inspect/py3o.py
--rw-r--r--   0 gas       (1000) gas       (1000)     4185 2022-10-14 14:46:09.000000 sqla_inspect-0.7.4/sqla_inspect/py3o_tmpl.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2022-10-18 09:47:57.887628 sqla_inspect-0.7.4/sqla_inspect/tests/
--rw-r--r--   0 gas       (1000) gas       (1000)        0 2020-09-22 12:42:13.000000 sqla_inspect-0.7.4/sqla_inspect/tests/__init__.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2022-10-18 09:47:57.888628 sqla_inspect-0.7.4/sqla_inspect/tests/__pycache__/
--rw-r--r--   0 gas       (1000) gas       (1000)      149 2022-10-14 14:41:20.000000 sqla_inspect-0.7.4/sqla_inspect/tests/__pycache__/__init__.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     1480 2022-10-14 14:46:17.000000 sqla_inspect-0.7.4/sqla_inspect/tests/__pycache__/models.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     3803 2022-10-14 14:46:17.000000 sqla_inspect-0.7.4/sqla_inspect/tests/__pycache__/test_ascii.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     2800 2022-10-14 14:46:17.000000 sqla_inspect-0.7.4/sqla_inspect/tests/__pycache__/test_base.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     2149 2022-10-14 14:46:17.000000 sqla_inspect-0.7.4/sqla_inspect/tests/__pycache__/test_csv.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     4176 2022-10-14 14:46:17.000000 sqla_inspect-0.7.4/sqla_inspect/tests/__pycache__/test_export.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     1157 2022-10-14 14:45:25.000000 sqla_inspect-0.7.4/sqla_inspect/tests/models.py
--rw-r--r--   0 gas       (1000) gas       (1000)      703 2022-10-14 14:45:22.000000 sqla_inspect-0.7.4/sqla_inspect/tests/test_ascii.py
--rw-r--r--   0 gas       (1000) gas       (1000)      682 2022-10-14 14:45:18.000000 sqla_inspect-0.7.4/sqla_inspect/tests/test_base.py
--rw-r--r--   0 gas       (1000) gas       (1000)      803 2022-10-14 14:45:10.000000 sqla_inspect-0.7.4/sqla_inspect/tests/test_csv.py
--rw-r--r--   0 gas       (1000) gas       (1000)     1866 2022-10-14 14:45:13.000000 sqla_inspect-0.7.4/sqla_inspect/tests/test_export.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2022-10-18 09:47:57.877628 sqla_inspect-0.7.4/sqla_inspect.egg-info/
--rw-r--r--   0 gas       (1000) gas       (1000)      602 2022-10-18 09:47:57.000000 sqla_inspect-0.7.4/sqla_inspect.egg-info/PKG-INFO
--rw-r--r--   0 gas       (1000) gas       (1000)     3352 2022-10-18 09:47:57.000000 sqla_inspect-0.7.4/sqla_inspect.egg-info/SOURCES.txt
--rw-r--r--   0 gas       (1000) gas       (1000)        1 2022-10-18 09:47:57.000000 sqla_inspect-0.7.4/sqla_inspect.egg-info/dependency_links.txt
--rw-r--r--   0 gas       (1000) gas       (1000)       77 2022-10-18 09:47:57.000000 sqla_inspect-0.7.4/sqla_inspect.egg-info/requires.txt
--rw-r--r--   0 gas       (1000) gas       (1000)       13 2022-10-18 09:47:57.000000 sqla_inspect-0.7.4/sqla_inspect.egg-info/top_level.txt
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-02 07:59:04.120932 sqla_inspect-0.7.5/
+-rw-r--r--   0 gas       (1000) gas       (1000)    35147 2020-09-22 12:42:13.000000 sqla_inspect-0.7.5/LICENSE.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)      103 2020-09-22 12:42:13.000000 sqla_inspect-0.7.5/MANIFEST.in
+-rw-r--r--   0 gas       (1000) gas       (1000)      574 2023-06-02 07:59:04.120932 sqla_inspect-0.7.5/PKG-INFO
+-rw-r--r--   0 gas       (1000) gas       (1000)      616 2020-10-02 10:07:10.000000 sqla_inspect-0.7.5/README.rst
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-02 07:59:04.105932 sqla_inspect-0.7.5/docs/
+-rw-r--r--   0 gas       (1000) gas       (1000)     5944 2020-09-22 12:42:13.000000 sqla_inspect-0.7.5/docs/Makefile
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-02 07:59:04.107932 sqla_inspect-0.7.5/docs/source/
+-rw-r--r--   0 gas       (1000) gas       (1000)     8336 2020-09-22 12:42:13.000000 sqla_inspect-0.7.5/docs/source/conf.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     8329 2021-06-08 16:30:38.000000 sqla_inspect-0.7.5/docs/source/export.rst
+-rw-r--r--   0 gas       (1000) gas       (1000)      476 2020-09-22 12:42:13.000000 sqla_inspect-0.7.5/docs/source/index.rst
+-rw-r--r--   0 gas       (1000) gas       (1000)       73 2020-09-22 12:42:13.000000 sqla_inspect-0.7.5/docs/source/modules.rst
+-rw-r--r--   0 gas       (1000) gas       (1000)     1116 2020-09-22 12:42:13.000000 sqla_inspect-0.7.5/docs/source/sqla_inspect.rst
+-rw-r--r--   0 gas       (1000) gas       (1000)      380 2020-09-22 12:42:13.000000 sqla_inspect-0.7.5/docs/source/sqla_inspect.tests.rst
+-rw-r--r--   0 gas       (1000) gas       (1000)       77 2021-06-14 12:45:32.000000 sqla_inspect-0.7.5/requirements.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)      184 2023-06-02 07:59:04.121932 sqla_inspect-0.7.5/setup.cfg
+-rw-r--r--   0 gas       (1000) gas       (1000)     1133 2023-06-02 07:55:59.000000 sqla_inspect-0.7.5/setup.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-02 07:59:04.108932 sqla_inspect-0.7.5/sqla_inspect/
+-rw-r--r--   0 gas       (1000) gas       (1000)       22 2022-10-14 14:46:56.000000 sqla_inspect-0.7.5/sqla_inspect/__init__.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-02 07:59:04.119932 sqla_inspect-0.7.5/sqla_inspect/__pycache__/
+-rw-r--r--   0 gas       (1000) gas       (1000)      278 2021-10-25 11:27:03.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/__init__.cpython-37-pytest-6.2.1.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)      160 2021-06-08 15:13:32.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)      164 2020-09-23 09:42:43.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)      278 2023-06-02 07:55:13.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/__init__.cpython-39-pytest-6.2.5.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)      164 2022-10-14 16:57:54.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     2663 2021-06-08 15:13:34.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/ascii.cpython-37.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     2693 2020-10-02 16:03:04.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/ascii.cpython-38.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     2797 2022-10-14 14:46:16.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/ascii.cpython-39-pytest-6.2.5.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     2688 2022-10-14 16:58:06.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/ascii.cpython-39.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     3914 2021-10-25 11:27:03.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/base.cpython-37-pytest-6.2.1.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     3801 2021-06-08 15:13:32.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/base.cpython-37.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     3856 2020-09-23 09:42:43.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/base.cpython-38.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     3973 2022-10-14 14:46:16.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/base.cpython-39-pytest-6.2.5.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     3864 2022-10-14 16:57:54.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     6469 2021-10-25 11:27:04.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/csv.cpython-37-pytest-6.2.1.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     6356 2021-06-08 15:13:32.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/csv.cpython-37.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     5950 2020-10-02 16:03:02.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/csv.cpython-38.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     6287 2022-10-14 14:46:16.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/csv.cpython-39-pytest-6.2.5.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     6178 2022-10-14 16:57:54.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/csv.cpython-39.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     8832 2021-10-25 11:27:04.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/excel.cpython-37-pytest-6.2.1.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     8719 2021-07-20 10:08:28.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/excel.cpython-37.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     8820 2020-10-02 16:03:02.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/excel.cpython-38.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     9120 2023-06-02 07:55:13.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/excel.cpython-39-pytest-6.2.5.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     9011 2023-06-02 07:55:05.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/excel.cpython-39.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)    10946 2021-10-25 11:27:04.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/export.cpython-37-pytest-6.2.1.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)    10833 2021-06-08 15:13:32.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/export.cpython-37.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)    10737 2020-10-02 16:03:02.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/export.cpython-38.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)    11020 2022-10-14 14:46:16.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/export.cpython-39-pytest-6.2.5.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)    10911 2022-10-14 16:57:54.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/export.cpython-39.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     7045 2021-10-25 11:27:03.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/ods.cpython-37-pytest-6.2.1.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     6932 2021-06-08 15:13:32.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/ods.cpython-37.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     6979 2020-10-02 16:03:02.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/ods.cpython-38.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     7378 2022-10-14 14:46:16.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/ods.cpython-39-pytest-6.2.5.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     7269 2022-10-14 16:57:54.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/ods.cpython-39.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     9453 2021-06-08 15:13:34.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/py3o.cpython-37.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     9513 2020-11-02 22:35:23.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/py3o.cpython-38.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     9609 2022-10-14 14:46:17.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/py3o.cpython-39-pytest-6.2.5.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     9500 2022-10-14 16:58:11.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/py3o.cpython-39.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     4333 2021-06-08 15:13:34.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/py3o_tmpl.cpython-37.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     4337 2020-09-25 08:35:12.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/py3o_tmpl.cpython-38.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     4451 2022-10-14 14:46:17.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/py3o_tmpl.cpython-39-pytest-6.2.5.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     4337 2022-10-14 16:58:11.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/py3o_tmpl.cpython-39.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     2360 2023-06-02 07:55:40.000000 sqla_inspect-0.7.5/sqla_inspect/ascii.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     3043 2022-10-14 14:45:59.000000 sqla_inspect-0.7.5/sqla_inspect/base.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     6354 2022-10-14 14:46:03.000000 sqla_inspect-0.7.5/sqla_inspect/csv.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     9613 2023-06-02 07:57:58.000000 sqla_inspect-0.7.5/sqla_inspect/excel.py
+-rw-r--r--   0 gas       (1000) gas       (1000)    13654 2022-10-14 14:46:07.000000 sqla_inspect-0.7.5/sqla_inspect/export.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     7252 2022-10-14 14:46:08.000000 sqla_inspect-0.7.5/sqla_inspect/ods.py
+-rw-r--r--   0 gas       (1000) gas       (1000)    12084 2022-10-14 14:46:11.000000 sqla_inspect-0.7.5/sqla_inspect/py3o.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     4185 2022-10-14 14:46:09.000000 sqla_inspect-0.7.5/sqla_inspect/py3o_tmpl.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-02 07:59:04.120932 sqla_inspect-0.7.5/sqla_inspect/tests/
+-rw-r--r--   0 gas       (1000) gas       (1000)        0 2020-09-22 12:42:13.000000 sqla_inspect-0.7.5/sqla_inspect/tests/__init__.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-02 07:59:04.120932 sqla_inspect-0.7.5/sqla_inspect/tests/__pycache__/
+-rw-r--r--   0 gas       (1000) gas       (1000)      149 2022-10-14 14:41:20.000000 sqla_inspect-0.7.5/sqla_inspect/tests/__pycache__/__init__.cpython-39-pytest-6.2.5.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     1480 2022-10-14 14:46:17.000000 sqla_inspect-0.7.5/sqla_inspect/tests/__pycache__/models.cpython-39-pytest-6.2.5.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     3803 2022-10-14 14:46:17.000000 sqla_inspect-0.7.5/sqla_inspect/tests/__pycache__/test_ascii.cpython-39-pytest-6.2.5.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     2800 2022-10-14 14:46:17.000000 sqla_inspect-0.7.5/sqla_inspect/tests/__pycache__/test_base.cpython-39-pytest-6.2.5.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     2149 2022-10-14 14:46:17.000000 sqla_inspect-0.7.5/sqla_inspect/tests/__pycache__/test_csv.cpython-39-pytest-6.2.5.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     4176 2022-10-14 14:46:17.000000 sqla_inspect-0.7.5/sqla_inspect/tests/__pycache__/test_export.cpython-39-pytest-6.2.5.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     1157 2022-10-14 14:45:25.000000 sqla_inspect-0.7.5/sqla_inspect/tests/models.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      703 2022-10-14 14:45:22.000000 sqla_inspect-0.7.5/sqla_inspect/tests/test_ascii.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      682 2022-10-14 14:45:18.000000 sqla_inspect-0.7.5/sqla_inspect/tests/test_base.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      803 2022-10-14 14:45:10.000000 sqla_inspect-0.7.5/sqla_inspect/tests/test_csv.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     1866 2022-10-14 14:45:13.000000 sqla_inspect-0.7.5/sqla_inspect/tests/test_export.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-02 07:59:04.109932 sqla_inspect-0.7.5/sqla_inspect.egg-info/
+-rw-r--r--   0 gas       (1000) gas       (1000)      574 2023-06-02 07:59:03.000000 sqla_inspect-0.7.5/sqla_inspect.egg-info/PKG-INFO
+-rw-r--r--   0 gas       (1000) gas       (1000)     3352 2023-06-02 07:59:04.000000 sqla_inspect-0.7.5/sqla_inspect.egg-info/SOURCES.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)        1 2023-06-02 07:59:03.000000 sqla_inspect-0.7.5/sqla_inspect.egg-info/dependency_links.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)       77 2023-06-02 07:59:03.000000 sqla_inspect-0.7.5/sqla_inspect.egg-info/requires.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)       13 2023-06-02 07:59:03.000000 sqla_inspect-0.7.5/sqla_inspect.egg-info/top_level.txt
```

### Comparing `sqla_inspect-0.7.4/LICENSE.txt` & `sqla_inspect-0.7.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/PKG-INFO` & `sqla_inspect-0.7.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 Metadata-Version: 2.1
 Name: sqla_inspect
-Version: 0.7.4
+Version: 0.7.5
 Summary: Usefull tools for setting/getting datas from SQLAlchemy models
 Home-page: https://github.com/majerteam/sqla_inspect
 Author: Gaston Tjebbes - Majerti
 Author-email: tech@majerti.fr
 License: GPLv3
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Database
 License-File: LICENSE.txt
-
-UNKNOWN
-
```

### Comparing `sqla_inspect-0.7.4/README.rst` & `sqla_inspect-0.7.5/README.rst`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/docs/Makefile` & `sqla_inspect-0.7.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/docs/source/conf.py` & `sqla_inspect-0.7.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/docs/source/export.rst` & `sqla_inspect-0.7.5/docs/source/export.rst`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/docs/source/sqla_inspect.rst` & `sqla_inspect-0.7.5/docs/source/sqla_inspect.rst`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/setup.py` & `sqla_inspect-0.7.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     requires = f.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='sqla_inspect',
-    version='0.7.4',
+    version='0.7.5',
     packages=['sqla_inspect'],
     include_package_data=True,
     license='GPLv3',
     description='Usefull tools for setting/getting datas from SQLAlchemy models',
     url='https://github.com/majerteam/sqla_inspect',
     author='Gaston Tjebbes - Majerti',
     author_email='tech@majerti.fr',
```

### Comparing `sqla_inspect-0.7.4/sqla_inspect/__pycache__/ascii.cpython-37.pyc` & `sqla_inspect-0.7.5/sqla_inspect/__pycache__/ascii.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/__pycache__/ascii.cpython-38.pyc` & `sqla_inspect-0.7.5/sqla_inspect/__pycache__/ascii.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/__pycache__/ascii.cpython-39-pytest-6.2.5.pyc` & `sqla_inspect-0.7.5/sqla_inspect/__pycache__/ascii.cpython-39-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/__pycache__/ascii.cpython-39.pyc` & `sqla_inspect-0.7.5/sqla_inspect/__pycache__/ascii.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/__pycache__/base.cpython-37-pytest-6.2.1.pyc` & `sqla_inspect-0.7.5/sqla_inspect/__pycache__/base.cpython-37-pytest-6.2.1.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/__pycache__/base.cpython-37.pyc` & `sqla_inspect-0.7.5/sqla_inspect/__pycache__/base.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/__pycache__/base.cpython-38.pyc` & `sqla_inspect-0.7.5/sqla_inspect/__pycache__/base.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/__pycache__/base.cpython-39-pytest-6.2.5.pyc` & `sqla_inspect-0.7.5/sqla_inspect/__pycache__/base.cpython-39-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/__pycache__/base.cpython-39.pyc` & `sqla_inspect-0.7.5/sqla_inspect/__pycache__/base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/__pycache__/csv.cpython-37-pytest-6.2.1.pyc` & `sqla_inspect-0.7.5/sqla_inspect/__pycache__/csv.cpython-37-pytest-6.2.1.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/__pycache__/csv.cpython-37.pyc` & `sqla_inspect-0.7.5/sqla_inspect/__pycache__/csv.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/__pycache__/csv.cpython-38.pyc` & `sqla_inspect-0.7.5/sqla_inspect/__pycache__/csv.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/__pycache__/csv.cpython-39-pytest-6.2.5.pyc` & `sqla_inspect-0.7.5/sqla_inspect/__pycache__/csv.cpython-39-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/__pycache__/csv.cpython-39.pyc` & `sqla_inspect-0.7.5/sqla_inspect/__pycache__/csv.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/__pycache__/excel.cpython-37-pytest-6.2.1.pyc` & `sqla_inspect-0.7.5/sqla_inspect/__pycache__/excel.cpython-37-pytest-6.2.1.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/__pycache__/excel.cpython-37.pyc` & `sqla_inspect-0.7.5/sqla_inspect/__pycache__/excel.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/__pycache__/excel.cpython-38.pyc` & `sqla_inspect-0.7.5/sqla_inspect/__pycache__/excel.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/__pycache__/excel.cpython-39-pytest-6.2.5.pyc` & `sqla_inspect-0.7.5/sqla_inspect/__pycache__/excel.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Oct 14 14:46:05 2022 UTC, .py size: 9452 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,567 +1,564 @@
-00000000: 610d 0d0a 0000 0000 2d76 4963 ec24 0000  a.......-vIc.$..
+00000000: 610d 0d0a 0000 0000 27a0 7964 7b25 0000  a.......'.yd{%..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0007 0000 0040 0000 0073 ea00 0000 6400  .....@...s....d.
-00000030: 5a00 6401 6402 6c01 5a02 6401 6402 6c03  Z.d.d.l.Z.d.d.l.
-00000040: 6d04 0200 0100 6d05 5a06 0100 6401 6402  m.....m.Z...d.d.
-00000050: 6c07 5a07 6401 6402 6c08 5a08 6401 6402  l.Z.d.d.l.Z.d.d.
-00000060: 6c09 5a09 6401 6403 6c0a 6d0b 5a0b 6d0c  l.Z.d.d.l.m.Z.m.
-00000070: 5a0c 0100 6401 6402 6c0d 5a0d 6401 6404  Z...d.d.l.Z.d.d.
-00000080: 6c0e 6d0f 5a0f 0100 6401 6405 6c10 6d11  l.m.Z...d.d.l.m.
-00000090: 5a11 6d12 5a12 0100 6401 6406 6c13 6d14  Z.m.Z...d.d.l.m.
-000000a0: 5a14 0100 6508 a015 6516 a101 5a17 6518  Z...e...e...Z.e.
-000000b0: 650f 8301 6518 6407 6408 8400 6507 a019  e...e.d.d...e...
-000000c0: 650f 6409 a102 4400 8301 8301 1700 5a1a  e.d...D.......Z.
-000000d0: 6514 8300 5a1b 4700 640a 640b 8400 640b  e...Z.G.d.d...d.
-000000e0: 651c 8303 5a1d 6412 640c 640d 8401 5a1e  e...Z.d.d.d...Z.
-000000f0: 4700 640e 640f 8400 640f 651d 6512 8304  G.d.d...d.e.e...
-00000100: 5a1f 4700 6410 6411 8400 6411 651d 6511  Z.G.d.d...d.e.e.
-00000110: 8304 5a20 6402 5300 2913 7a1a 0a45 7863  ..Z d.S.).z..Exc
-00000120: 656c 2065 7870 6f72 7461 7469 6f6e 206d  el exportation m
-00000130: 6f64 756c 650a e900 0000 004e 2902 da05  odule......N)...
-00000140: 436f 6c6f 72da 0446 6f6e 7429 01da 0f61  Color..Font)...a
-00000150: 7363 6969 5f75 7070 6572 6361 7365 2902  scii_uppercase).
-00000160: da0c 4261 7365 4578 706f 7274 6572 da0c  ..BaseExporter..
-00000170: 5371 6c61 4578 706f 7274 6572 2901 da08  SqlaExporter)...
-00000180: 5265 6769 7374 7279 6301 0000 0000 0000  Registryc.......
-00000190: 0000 0000 0002 0000 0004 0000 0063 0000  .............c..
-000001a0: 0073 1800 0000 7c00 5d10 7d01 6400 a000  .s....|.].}.d...
-000001b0: 7c01 a101 5600 0100 7102 6401 5300 2902  |...V...q.d.S.).
-000001c0: da00 4e29 01da 046a 6f69 6e29 02da 022e  ..N)...join)....
-000001d0: 305a 0564 7570 6c65 a900 720b 0000 00fa  0Z.duple..r.....
-000001e0: 312f 686f 6d65 2f67 6173 2f65 6e64 692f  1/home/gas/endi/
-000001f0: 7371 6c61 5f69 6e73 7065 6374 2f73 716c  sqla_inspect/sql
-00000200: 615f 696e 7370 6563 742f 6578 6365 6c2e  a_inspect/excel.
-00000210: 7079 da09 3c67 656e 6578 7072 3e20 0000  py..<genexpr> ..
-00000220: 0073 0400 0000 0402 02ff 720d 0000 00e9  .s........r.....
-00000230: 0200 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00000240: 0000 0000 0003 0000 0040 0000 0073 7a00  .........@...sz.
-00000250: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
-00000260: 5a04 641b 6404 6405 8401 5a05 641c 6406  Z.d.d.d...Z.d.d.
-00000270: 6407 8401 5a06 6408 6409 8400 5a07 6508  d...Z.d.d...Z.e.
-00000280: 6508 640a 9c02 640b 640c 8404 5a09 640d  e.d...d.d...Z.d.
-00000290: 640e 8400 5a0a 640f 6410 8400 5a0b 641d  d...Z.d.d...Z.d.
-000002a0: 6411 6412 8401 5a0c 6413 6414 8400 5a0d  d.d...Z.d.d...Z.
-000002b0: 6415 6416 8400 5a0e 6417 6418 8400 5a0f  d.d...Z.d.d...Z.
-000002c0: 6419 641a 8400 5a10 6403 5300 291e da09  d.d...Z.d.S.)...
-000002d0: 586c 7357 7269 7465 7261 9401 0000 0a20  XlsWritera..... 
-000002e0: 2020 2043 6c61 7373 2070 726f 7669 6469     Class providi
-000002f0: 6e67 2063 6f6d 6d6f 6e20 746f 6f6c 7320  ng common tools 
-00000300: 746f 2077 7269 7465 2065 7863 656c 2066  to write excel f
-00000310: 696c 6573 2066 726f 6d20 7461 6275 6c61  iles from tabula
-00000320: 7220 6461 7461 730a 0a20 2020 2048 6173  r datas..    Has
-00000330: 2074 6f20 6265 2073 7562 636c 6173 7365   to be subclasse
-00000340: 642c 2074 6865 2073 7562 636c 6173 7320  d, the subclass 
-00000350: 7368 6f75 6c64 2070 726f 7669 6465 2061  should provide a
-00000360: 205f 6461 7461 7320 616e 6420 6120 6865   _datas and a he
-00000370: 6164 6572 730a 2020 2020 6174 7472 6962  aders.    attrib
-00000380: 7574 6520 7468 6174 2063 6f6e 7461 696e  ute that contain
-00000390: 7320 7468 6520 6461 7461 7320 746f 2072  s the datas to r
-000003a0: 656e 6465 7220 616e 6420 7468 6520 6865  ender and the he
-000003b0: 6164 6572 730a 0a20 2020 2020 2020 205f  aders..        _
-000003c0: 6461 7461 730a 0a20 2020 2020 2020 2020  datas..         
-000003d0: 2020 206c 6973 7420 6f66 2074 7570 6c65     list of tuple
-000003e0: 7320 2865 6163 6820 7475 706c 6520 6973  s (each tuple is
-000003f0: 2061 2072 6f77 290a 0a20 2020 2020 2020   a row)..       
-00000400: 2068 6561 6465 7273 0a0a 2020 2020 2020   headers..      
-00000410: 2020 2020 2020 6c69 7374 206f 6620 6469        list of di
-00000420: 6374 2063 6f6e 7461 696e 696e 6720 7468  ct containing th
-00000430: 6520 6c61 6265 6c20 6f66 2065 6163 6820  e label of each 
-00000440: 636f 6c75 6d6e 3a0a 2020 2020 2020 2020  column:.        
-00000450: 2020 2020 2020 2020 7b27 6c61 6265 6c27          {'label'
-00000460: 3a20 3c61 206c 6162 656c 3e7d 0a0a 2020  : <a label>}..  
-00000470: 2020 5a06 4578 706f 7274 4e63 0200 0000    Z.ExportNc....
-00000480: 0000 0000 0000 0000 0300 0000 0200 0000  ................
-00000490: 4b00 0000 7342 0000 007c 0164 0075 0072  K...sB...|.d.u.r
-000004a0: 2a74 006a 01a0 02a1 007c 005f 037c 006a  *t.j.....|._.|.j
-000004b0: 036a 047c 005f 057c 006a 067c 006a 055f  .j.|._.|.j.|.j._
-000004c0: 066e 0e7c 017c 005f 057c 016a 077c 005f  .n.|.|._.|.j.|._
-000004d0: 037c 027c 005f 0864 0053 00a9 014e 2909  .|.|._.d.S...N).
-000004e0: da08 6f70 656e 7079 786c 5a08 776f 726b  ..openpyxlZ.work
-000004f0: 626f 6f6b 5a08 576f 726b 626f 6f6b da04  bookZ.Workbook..
-00000500: 626f 6f6b da06 6163 7469 7665 da09 776f  book..active..wo
-00000510: 726b 7368 6565 74da 0574 6974 6c65 da06  rksheet..title..
-00000520: 7061 7265 6e74 da07 6f70 7469 6f6e 7329  parent..options)
-00000530: 03da 0473 656c 6672 1400 0000 da02 6b77  ...selfr......kw
-00000540: 720b 0000 0072 0b00 0000 720c 0000 00da  r....r....r.....
-00000550: 085f 5f69 6e69 745f 5f3d 0000 0073 0e00  .__init__=...s..
-00000560: 0000 0001 0801 0c01 0a01 0c02 0601 0801  ................
-00000570: 7a12 586c 7357 7269 7465 722e 5f5f 696e  z.XlsWriter.__in
-00000580: 6974 5f5f 6302 0000 0000 0000 0000 0000  it__c...........
-00000590: 0002 0000 0005 0000 0043 0000 0073 3400  .........C...s4.
-000005a0: 0000 7c01 6401 7500 7210 7400 a001 a100  ..|.d.u.r.t.....
-000005b0: 7d01 7c01 a002 7403 6a04 6a05 a006 7c00  }.|...t.j.j...|.
-000005c0: 6a07 a101 a101 0100 7c01 a008 6402 a101  j.......|...d...
-000005d0: 0100 7c01 5300 2903 7a9a 0a20 2020 2020  ..|.S.).z..     
+00000020: 0007 0000 0040 0000 0073 d000 0000 6400  .....@...s....d.
+00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
+00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
+00000050: 6d05 5a05 6d06 5a06 0100 6401 6402 6c07  m.Z.m.Z...d.d.l.
+00000060: 5a07 6401 6404 6c08 6d09 5a09 0100 6401  Z.d.d.l.m.Z...d.
+00000070: 6405 6c0a 6d0b 5a0b 6d0c 5a0c 0100 6401  d.l.m.Z.m.Z...d.
+00000080: 6406 6c0d 6d0e 5a0e 0100 6502 a00f 6510  d.l.m.Z...e...e.
+00000090: a101 5a11 6512 6509 8301 6512 6407 6408  ..Z.e.e...e.d.d.
+000000a0: 8400 6501 a013 6509 6409 a102 4400 8301  ..e...e.d...D...
+000000b0: 8301 1700 5a14 650e 8300 5a15 4700 640a  ....Z.e...Z.G.d.
+000000c0: 640b 8400 640b 6516 8303 5a17 6412 640c  d...d.e...Z.d.d.
+000000d0: 640d 8401 5a18 4700 640e 640f 8400 640f  d...Z.G.d.d...d.
+000000e0: 6517 650c 8304 5a19 4700 6410 6411 8400  e.e...Z.G.d.d...
+000000f0: 6411 6517 650b 8304 5a1a 6402 5300 2913  d.e.e...Z.d.S.).
+00000100: 7a1a 0a45 7863 656c 2065 7870 6f72 7461  z..Excel exporta
+00000110: 7469 6f6e 206d 6f64 756c 650a e900 0000  tion module.....
+00000120: 004e 2902 da05 436f 6c6f 72da 0446 6f6e  .N)...Color..Fon
+00000130: 7429 01da 0f61 7363 6969 5f75 7070 6572  t)...ascii_upper
+00000140: 6361 7365 2902 da0c 4261 7365 4578 706f  case)...BaseExpo
+00000150: 7274 6572 da0c 5371 6c61 4578 706f 7274  rter..SqlaExport
+00000160: 6572 2901 da08 5265 6769 7374 7279 6301  er)...Registryc.
+00000170: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00000180: 0000 0063 0000 0073 1800 0000 7c00 5d10  ...c...s....|.].
+00000190: 7d01 6400 a000 7c01 a101 5600 0100 7102  }.d...|...V...q.
+000001a0: 6401 5300 2902 da00 4e29 01da 046a 6f69  d.S.)...N)...joi
+000001b0: 6e29 02da 022e 305a 0564 7570 6c65 a900  n)....0Z.duple..
+000001c0: 720b 0000 00fa 312f 686f 6d65 2f67 6173  r.....1/home/gas
+000001d0: 2f65 6e64 692f 7371 6c61 5f69 6e73 7065  /endi/sqla_inspe
+000001e0: 6374 2f73 716c 615f 696e 7370 6563 742f  ct/sqla_inspect/
+000001f0: 6578 6365 6c2e 7079 da09 3c67 656e 6578  excel.py..<genex
+00000200: 7072 3e20 0000 0073 0400 0000 0402 02ff  pr> ...s........
+00000210: 720d 0000 00e9 0200 0000 6300 0000 0000  r.........c.....
+00000220: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
+00000230: 0000 0073 7a00 0000 6500 5a01 6400 5a02  ...sz...e.Z.d.Z.
+00000240: 6401 5a03 6402 5a04 641b 6404 6405 8401  d.Z.d.Z.d.d.d...
+00000250: 5a05 641c 6406 6407 8401 5a06 6408 6409  Z.d.d.d...Z.d.d.
+00000260: 8400 5a07 6508 6508 640a 9c02 640b 640c  ..Z.e.e.d...d.d.
+00000270: 8404 5a09 640d 640e 8400 5a0a 640f 6410  ..Z.d.d...Z.d.d.
+00000280: 8400 5a0b 641d 6411 6412 8401 5a0c 6413  ..Z.d.d.d...Z.d.
+00000290: 6414 8400 5a0d 6415 6416 8400 5a0e 6417  d...Z.d.d...Z.d.
+000002a0: 6418 8400 5a0f 6419 641a 8400 5a10 6403  d...Z.d.d...Z.d.
+000002b0: 5300 291e da09 586c 7357 7269 7465 7261  S.)...XlsWritera
+000002c0: 9401 0000 0a20 2020 2043 6c61 7373 2070  .....    Class p
+000002d0: 726f 7669 6469 6e67 2063 6f6d 6d6f 6e20  roviding common 
+000002e0: 746f 6f6c 7320 746f 2077 7269 7465 2065  tools to write e
+000002f0: 7863 656c 2066 696c 6573 2066 726f 6d20  xcel files from 
+00000300: 7461 6275 6c61 7220 6461 7461 730a 0a20  tabular datas.. 
+00000310: 2020 2048 6173 2074 6f20 6265 2073 7562     Has to be sub
+00000320: 636c 6173 7365 642c 2074 6865 2073 7562  classed, the sub
+00000330: 636c 6173 7320 7368 6f75 6c64 2070 726f  class should pro
+00000340: 7669 6465 2061 205f 6461 7461 7320 616e  vide a _datas an
+00000350: 6420 6120 6865 6164 6572 730a 2020 2020  d a headers.    
+00000360: 6174 7472 6962 7574 6520 7468 6174 2063  attribute that c
+00000370: 6f6e 7461 696e 7320 7468 6520 6461 7461  ontains the data
+00000380: 7320 746f 2072 656e 6465 7220 616e 6420  s to render and 
+00000390: 7468 6520 6865 6164 6572 730a 0a20 2020  the headers..   
+000003a0: 2020 2020 205f 6461 7461 730a 0a20 2020       _datas..   
+000003b0: 2020 2020 2020 2020 206c 6973 7420 6f66           list of
+000003c0: 2074 7570 6c65 7320 2865 6163 6820 7475   tuples (each tu
+000003d0: 706c 6520 6973 2061 2072 6f77 290a 0a20  ple is a row).. 
+000003e0: 2020 2020 2020 2068 6561 6465 7273 0a0a         headers..
+000003f0: 2020 2020 2020 2020 2020 2020 6c69 7374              list
+00000400: 206f 6620 6469 6374 2063 6f6e 7461 696e   of dict contain
+00000410: 696e 6720 7468 6520 6c61 6265 6c20 6f66  ing the label of
+00000420: 2065 6163 6820 636f 6c75 6d6e 3a0a 2020   each column:.  
+00000430: 2020 2020 2020 2020 2020 2020 2020 7b27                {'
+00000440: 6c61 6265 6c27 3a20 3c61 206c 6162 656c  label': <a label
+00000450: 3e7d 0a0a 2020 2020 da06 4578 706f 7274  >}..    ..Export
+00000460: 4e63 0200 0000 0000 0000 0000 0000 0300  Nc..............
+00000470: 0000 0200 0000 4b00 0000 7342 0000 007c  ......K...sB...|
+00000480: 0164 0075 0072 2a74 006a 01a0 02a1 007c  .d.u.r*t.j.....|
+00000490: 005f 037c 006a 036a 047c 005f 057c 006a  ._.|.j.j.|._.|.j
+000004a0: 067c 006a 055f 066e 0e7c 017c 005f 057c  .|.j._.n.|.|._.|
+000004b0: 016a 077c 005f 037c 027c 005f 0864 0053  .j.|._.|.|._.d.S
+000004c0: 00a9 014e 2909 da08 6f70 656e 7079 786c  ...N)...openpyxl
+000004d0: 5a08 776f 726b 626f 6f6b 5a08 576f 726b  Z.workbookZ.Work
+000004e0: 626f 6f6b da04 626f 6f6b da06 6163 7469  book..book..acti
+000004f0: 7665 da09 776f 726b 7368 6565 74da 0574  ve..worksheet..t
+00000500: 6974 6c65 da06 7061 7265 6e74 da07 6f70  itle..parent..op
+00000510: 7469 6f6e 7329 03da 0473 656c 6672 1500  tions)...selfr..
+00000520: 0000 da02 6b77 720b 0000 0072 0b00 0000  ....kwr....r....
+00000530: 720c 0000 00da 085f 5f69 6e69 745f 5f3d  r......__init__=
+00000540: 0000 0073 0e00 0000 0001 0801 0c01 0a01  ...s............
+00000550: 0c02 0601 0801 7a12 586c 7357 7269 7465  ......z.XlsWrite
+00000560: 722e 5f5f 696e 6974 5f5f 6302 0000 0000  r.__init__c.....
+00000570: 0000 0000 0000 0002 0000 0005 0000 0043  ...............C
+00000580: 0000 0073 4e00 0000 7c01 6401 7500 7210  ...sN...|.d.u.r.
+00000590: 7400 a001 a100 7d01 7402 7c00 6a03 6402  t.....}.t.|.j.d.
+000005a0: 8302 722a 7c00 6a03 a004 7c01 a101 0100  ..r*|.j...|.....
+000005b0: 6e16 7c01 a005 7406 6a07 6a08 a009 7c00  n.|...t.j.j...|.
+000005c0: 6a03 a101 a101 0100 7c01 a00a 6403 a101  j.......|...d...
+000005d0: 0100 7c01 5300 2904 7a9a 0a20 2020 2020  ..|.S.).z..     
 000005e0: 2020 2052 6574 7572 6e20 6120 6669 6c65     Return a file
 000005f0: 2062 7566 6665 7220 636f 6e74 6169 6e69   buffer containi
 00000600: 6e67 2074 6865 2072 6573 756c 7469 6e67  ng the resulting
 00000610: 2078 6c73 0a0a 2020 2020 2020 2020 3a70   xls..        :p
 00000620: 6172 616d 206f 626a 2066 5f62 7566 3a20  aram obj f_buf: 
 00000630: 4120 6669 6c65 2062 7566 6665 7220 7375  A file buffer su
 00000640: 7070 6f72 7469 6e67 2074 6865 2077 7269  pporting the wri
 00000650: 7465 2061 6e64 2073 6565 6b0a 2020 2020  te and seek.    
 00000660: 2020 2020 6d65 7468 6f64 730a 2020 2020      methods.    
-00000670: 2020 2020 4e72 0100 0000 2909 da02 696f      Nr....)...io
-00000680: da07 4279 7465 7349 4fda 0577 7269 7465  ..BytesIO..write
-00000690: 7211 0000 00da 0677 7269 7465 72da 0565  r......writer..e
-000006a0: 7863 656c 5a15 7361 7665 5f76 6972 7475  xcelZ.save_virtu
-000006b0: 616c 5f77 6f72 6b62 6f6f 6b72 1200 0000  al_workbookr....
-000006c0: da04 7365 656b a902 7218 0000 00da 0566  ..seek..r......f
-000006d0: 5f62 7566 720b 0000 0072 0b00 0000 720c  _bufr....r....r.
-000006e0: 0000 00da 0973 6176 655f 626f 6f6b 4700  .....save_bookG.
-000006f0: 0000 730a 0000 0000 0708 0108 0116 010a  ..s.............
-00000700: 017a 1358 6c73 5772 6974 6572 2e73 6176  .z.XlsWriter.sav
-00000710: 655f 626f 6f6b 6303 0000 0000 0000 0000  e_bookc.........
-00000720: 0000 0003 0000 0004 0000 0043 0000 0073  ...........C...s
-00000730: 1600 0000 7400 7401 7c02 6401 8d01 6402  ....t.t.|.d...d.
-00000740: 8d01 7c01 5f02 6403 5300 2904 7aa8 0a20  ..|._.d.S.).z.. 
-00000750: 2020 2020 2020 2053 6574 2074 6865 2067         Set the g
-00000760: 6976 656e 2063 6f6c 6f72 2074 6f20 7468  iven color to th
-00000770: 6520 7072 6f76 6964 6564 2063 656c 6c0a  e provided cell.
-00000780: 0a20 2020 2020 2020 2020 2020 2063 656c  .            cel
-00000790: 6c0a 0a20 2020 2020 2020 2020 2020 2020  l..             
-000007a0: 2020 2041 2078 6c73 2063 656c 6c20 6f62     A xls cell ob
-000007b0: 6a65 6374 0a0a 2020 2020 2020 2020 2020  ject..          
-000007c0: 2020 636f 6c6f 720a 0a20 2020 2020 2020    color..       
-000007d0: 2020 2020 2020 2020 2041 206f 7065 6e70           A openp
-000007e0: 7978 6c20 636f 6c6f 7220 7661 720a 2020  yxl color var.  
-000007f0: 2020 2020 2020 2901 da03 7267 6229 01da        )...rgb)..
-00000800: 0563 6f6c 6f72 4e29 0372 0300 0000 7202  .colorN).r....r.
-00000810: 0000 005a 0466 6f6e 7429 0372 1800 0000  ...Z.font).r....
-00000820: da04 6365 6c6c 7225 0000 0072 0b00 0000  ..cellr%...r....
-00000830: 720b 0000 0072 0c00 0000 da09 7365 745f  r....r......set_
-00000840: 636f 6c6f 7254 0000 0073 0200 0000 000c  colorT...s......
-00000850: 7a13 586c 7357 7269 7465 722e 7365 745f  z.XlsWriter.set_
-00000860: 636f 6c6f 7229 02da 0b63 6f6c 756d 6e5f  color)...column_
-00000870: 6e61 6d65 da05 7661 6c75 6563 0300 0000  name..valuec....
-00000880: 0000 0000 0000 0000 0300 0000 0400 0000  ................
-00000890: 4300 0000 7324 0000 0074 007c 0064 017c  C...s$...t.|.d.|
-000008a0: 0116 0083 0272 2074 017c 0064 017c 0116  .....r t.|.d.|..
-000008b0: 0083 027c 0283 017d 027c 0253 0029 027a  ...|...}.|.S.).z
-000008c0: 1f0a 2020 2020 2020 2020 466f 726d 6174  ..        Format
-000008d0: 2061 2063 656c 6c0a 2020 2020 2020 2020   a cell.        
-000008e0: 7a09 666f 726d 6174 5f25 7329 02da 0768  z.format_%s)...h
-000008f0: 6173 6174 7472 da07 6765 7461 7474 7229  asattr..getattr)
-00000900: 0372 1800 0000 7228 0000 0072 2900 0000  .r....r(...r)...
-00000910: 720b 0000 0072 0b00 0000 720c 0000 00da  r....r....r.....
-00000920: 0b66 6f72 6d61 745f 6365 6c6c 6200 0000  .format_cellb...
-00000930: 7306 0000 0000 040e 0112 017a 1558 6c73  s..........z.Xls
-00000940: 5772 6974 6572 2e66 6f72 6d61 745f 6365  Writer.format_ce
-00000950: 6c6c 6302 0000 0000 0000 0000 0000 0007  llc.............
-00000960: 0000 0005 0000 0043 0000 0073 4600 0000  .......C...sF...
-00000970: 6700 7d02 7400 7c00 6401 6700 8303 7d03  g.}.t.|.d.g...}.
-00000980: 7c03 4400 5d2c 7d04 7c04 6402 1900 7d05  |.D.],}.|.d...}.
-00000990: 7c01 a001 7c05 6403 a102 7d06 7c00 a002  |...|.d...}.|...
-000009a0: 7c06 a101 7d06 7c02 a003 7c06 a101 0100  |...}.|...|.....
-000009b0: 7114 7c02 5300 2904 7a96 0a20 2020 2020  q.|.S.).z..     
-000009c0: 2020 2054 6865 2072 656e 6465 7220 6d65     The render me
-000009d0: 7468 6f64 2065 7870 6563 7473 2072 6f77  thod expects row
-000009e0: 7320 6173 206c 6973 7473 2c20 6865 7265  s as lists, here
-000009f0: 2077 6520 7377 6974 6368 206f 7572 2072   we switch our r
-00000a00: 6f77 2066 6f72 6d61 740a 2020 2020 2020  ow format.      
-00000a10: 2020 6672 6f6d 2064 6963 7420 746f 206c    from dict to l
-00000a20: 6973 7420 7265 7370 6563 7469 6e67 2074  ist respecting t
-00000a30: 6865 206f 7264 6572 206f 6620 7468 6520  he order of the 
-00000a40: 6865 6164 6572 730a 2020 2020 2020 2020  headers.        
-00000a50: da07 6865 6164 6572 73da 046e 616d 6572  ..headers..namer
-00000a60: 0800 0000 2904 722b 0000 00da 0367 6574  ....).r+.....get
-00000a70: 722c 0000 00da 0661 7070 656e 6429 0772  r,.....append).r
-00000a80: 1800 0000 da03 726f 77da 0372 6573 722d  ......row..resr-
-00000a90: 0000 00da 0663 6f6c 756d 6e72 2800 0000  .....columnr(...
-00000aa0: 7229 0000 0072 0b00 0000 720b 0000 0072  r)...r....r....r
-00000ab0: 0c00 0000 da0a 666f 726d 6174 5f72 6f77  ......format_row
-00000ac0: 6a00 0000 7310 0000 0000 0504 010c 0108  j...s...........
-00000ad0: 0108 010c 010a 010c 017a 1458 6c73 5772  .........z.XlsWr
-00000ae0: 6974 6572 2e66 6f72 6d61 745f 726f 7763  iter.format_rowc
-00000af0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00000b00: 0200 0000 4300 0000 7314 0000 007c 00a0  ....C...s....|..
-00000b10: 00a1 0001 007c 00a0 01a1 0001 0064 0153  .....|.......d.S
-00000b20: 0029 027a 430a 2020 2020 2020 2020 506f  .).zC.        Po
-00000b30: 7075 6c61 7465 2068 6561 6465 7273 2061  pulate headers a
-00000b40: 6e64 2072 6f77 7320 6265 666f 7265 2077  nd rows before w
-00000b50: 7269 7469 6e67 206f 7572 2062 6f6f 6b0a  riting our book.
-00000b60: 2020 2020 2020 2020 4e29 02da 0f5f 7265          N)..._re
-00000b70: 6e64 6572 5f68 6561 6465 7273 da0c 5f72  nder_headers.._r
-00000b80: 656e 6465 725f 726f 7773 2901 7218 0000  ender_rows).r...
-00000b90: 0072 0b00 0000 720b 0000 0072 0c00 0000  .r....r....r....
-00000ba0: da09 5f70 6f70 756c 6174 6578 0000 0073  .._populatex...s
-00000bb0: 0400 0000 0004 0801 7a13 586c 7357 7269  ........z.XlsWri
-00000bc0: 7465 722e 5f70 6f70 756c 6174 6563 0200  ter._populatec..
-00000bd0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-00000be0: 0000 4300 0000 7312 0000 007c 00a0 00a1  ..C...s....|....
-00000bf0: 0001 007c 00a0 017c 01a1 0153 0029 017a  ...|...|...S.).z
-00000c00: 870a 2020 2020 2020 2020 4465 6669 6e69  ..        Defini
-00000c10: 7465 6c79 2072 656e 6465 7220 7468 6520  tely render the 
-00000c20: 776f 726b 626f 6f6b 0a0a 2020 2020 2020  workbook..      
-00000c30: 2020 3a70 6172 616d 206f 626a 2066 5f62    :param obj f_b
-00000c40: 7566 3a20 4120 6669 6c65 2062 7566 6665  uf: A file buffe
-00000c50: 7220 7375 7070 6f72 7469 6e67 2074 6865  r supporting the
-00000c60: 2077 7269 7465 2061 6e64 2073 6565 6b0a   write and seek.
-00000c70: 2020 2020 2020 2020 6d65 7468 6f64 730a          methods.
-00000c80: 2020 2020 2020 2020 2902 7237 0000 0072          ).r7...r
-00000c90: 2300 0000 7221 0000 0072 0b00 0000 720b  #...r!...r....r.
-00000ca0: 0000 0072 0c00 0000 da06 7265 6e64 6572  ...r......render
-00000cb0: 7f00 0000 7304 0000 0000 0708 027a 1058  ....s........z.X
-00000cc0: 6c73 5772 6974 6572 2e72 656e 6465 7263  lsWriter.renderc
-00000cd0: 0100 0000 0000 0000 0000 0000 0b00 0000  ................
-00000ce0: 0600 0000 4300 0000 739c 0000 0074 007c  ....C...s....t.|
-00000cf0: 0064 0164 0283 037d 0174 007c 0064 0364  .d.d...}.t.|.d.d
-00000d00: 0283 037d 0274 017c 0183 0144 005d 765c  ...}.t.|...D.]v\
-00000d10: 027d 037d 047c 0364 0417 007d 0574 017c  .}.}.|.d...}.t.|
-00000d20: 0483 0144 005d 5c5c 027d 067d 077c 006a  ...D.]\\.}.}.|.j
-00000d30: 026a 037c 057c 0664 0517 0064 068d 027d  .j.|.|.d...d...}
-00000d40: 087c 0764 0775 0172 647c 077c 085f 046e  .|.d.u.rd|.|._.n
-00000d50: 0664 087c 085f 0474 057c 0283 017c 066b  .d.|._.t.|...|.k
-00000d60: 0472 387c 027c 0619 007d 0974 067c 0983  .r8|.|...}.t.|..
-00000d70: 017d 0a7c 0a64 0775 0172 387c 0a7c 085f  .}.|.d.u.r8|.|._
-00000d80: 0771 3871 2064 0753 0029 097a 3b0a 2020  .q8q d.S.).z;.  
-00000d90: 2020 2020 2020 5265 6e64 6572 2074 6865        Render the
-00000da0: 2072 6f77 7320 696e 2074 6865 2063 7572   rows in the cur
-00000db0: 7265 6e74 2073 7479 6c65 7368 6565 740a  rent stylesheet.
-00000dc0: 2020 2020 2020 2020 da06 5f64 6174 6173          .._datas
-00000dd0: 720b 0000 0072 2d00 0000 720e 0000 00e9  r....r-...r.....
-00000de0: 0100 0000 a902 7231 0000 0072 3300 0000  ......r1...r3...
-00000df0: 4e72 0800 0000 2908 722b 0000 00da 0965  Nr....).r+.....e
-00000e00: 6e75 6d65 7261 7465 7214 0000 0072 2600  numerater....r&.
-00000e10: 0000 7229 0000 00da 036c 656e da0f 6765  ..r).....len..ge
-00000e20: 745f 6365 6c6c 5f66 6f72 6d61 745a 0d6e  t_cell_formatZ.n
-00000e30: 756d 6265 725f 666f 726d 6174 290b 7218  umber_format).r.
-00000e40: 0000 0072 3900 0000 722d 0000 00da 0569  ...r9...r-.....i
-00000e50: 6e64 6578 7231 0000 005a 0a72 6f77 5f6e  ndexr1...Z.row_n
-00000e60: 756d 6265 725a 0763 6f6c 5f6e 756d 7229  umberZ.col_numr)
-00000e70: 0000 0072 2600 0000 da06 6865 6164 6572  ...r&.....header
-00000e80: da06 666f 726d 6174 720b 0000 0072 0b00  ..formatr....r..
-00000e90: 0000 720c 0000 0072 3600 0000 8a00 0000  ..r....r6.......
-00000ea0: 731c 0000 0000 040c 010c 0110 0108 0110  s...............
-00000eb0: 0114 0108 0108 0206 010c 0108 0108 0108  ................
-00000ec0: 017a 1658 6c73 5772 6974 6572 2e5f 7265  .z.XlsWriter._re
-00000ed0: 6e64 6572 5f72 6f77 7363 0100 0000 0000  nder_rowsc......
-00000ee0: 0000 0000 0000 0700 0000 0500 0000 4300  ..............C.
-00000ef0: 0000 7388 0000 0074 007c 0064 0164 0283  ..s....t.|.d.d..
-00000f00: 037d 0174 017c 0183 0144 005d 265c 027d  .}.t.|...D.]&\.}
-00000f10: 027d 037c 006a 026a 0364 037c 0264 0317  .}.|.j.j.d.|.d..
-00000f20: 0064 048d 027d 047c 0364 0519 007c 045f  .d...}.|.d...|._
-00000f30: 0471 147c 0264 0337 007d 0274 007c 0064  .q.|.d.7.}.t.|.d
-00000f40: 0664 0283 037d 0574 017c 0583 0144 005d  .d...}.t.|...D.]
-00000f50: 2a5c 027d 067d 037c 006a 026a 0364 037c  *\.}.}.|.j.j.d.|
-00000f60: 067c 0217 0064 0317 0064 048d 027d 047c  .|...d...d...}.|
-00000f70: 0364 0519 007c 045f 0471 5864 0753 0029  .d...|._.qXd.S.)
-00000f80: 087a 270a 2020 2020 2020 2020 5772 6974  .z'.        Writ
-00000f90: 6520 7468 6520 6865 6164 6572 7320 726f  e the headers ro
-00000fa0: 770a 2020 2020 2020 2020 722d 0000 0072  w.        r-...r
-00000fb0: 0b00 0000 723a 0000 0072 3b00 0000 da05  ....r:...r;.....
-00000fc0: 6c61 6265 6cda 0d65 7874 7261 5f68 6561  label..extra_hea
-00000fd0: 6465 7273 4e29 0572 2b00 0000 723c 0000  dersN).r+...r<..
-00000fe0: 0072 1400 0000 7226 0000 0072 2900 0000  .r....r&...r)...
-00000ff0: 2907 7218 0000 0072 2d00 0000 723f 0000  ).r....r-...r?..
-00001000: 00da 0363 6f6c 7226 0000 0072 4300 0000  ...colr&...rC...
-00001010: 5a09 6164 645f 696e 6465 7872 0b00 0000  Z.add_indexr....
-00001020: 720b 0000 0072 0c00 0000 7235 0000 009e  r....r....r5....
-00001030: 0000 0073 1200 0000 0004 0c01 1002 1401  ...s............
-00001040: 0c02 0802 0c01 1001 1801 7a19 586c 7357  ..........z.XlsW
-00001050: 7269 7465 722e 5f72 656e 6465 725f 6865  riter._render_he
-00001060: 6164 6572 7363 0200 0000 0000 0000 0000  adersc..........
-00001070: 0000 0200 0000 0200 0000 4300 0000 730c  ..........C...s.
-00001080: 0000 007c 017c 006a 005f 0164 0053 0072  ...|.|.j._.d.S.r
-00001090: 1000 0000 2902 7214 0000 0072 1500 0000  ....).r....r....
-000010a0: 2902 7218 0000 0072 1500 0000 720b 0000  ).r....r....r...
-000010b0: 0072 0b00 0000 720c 0000 00da 0973 6574  .r....r......set
-000010c0: 5f74 6974 6c65 af00 0000 7302 0000 0000  _title....s.....
-000010d0: 017a 1358 6c73 5772 6974 6572 2e73 6574  .z.XlsWriter.set
-000010e0: 5f74 6974 6c65 6302 0000 0000 0000 0000  _titlec.........
-000010f0: 0000 0004 0000 0007 0000 0043 0000 0073  ...........C...s
-00001100: 5a00 0000 6700 7c00 5f00 6401 7c00 6a01  Z...g.|._.d.|.j.
-00001110: 7600 7250 7c00 6a01 6401 1900 4400 5d32  v.rP|.j.d...D.]2
-00001120: 7d02 7c01 4400 5d28 7d03 7c03 a002 6402  }.|.D.](}.|...d.
-00001130: 7c03 6403 1900 a102 7c02 6b02 7222 7c00  |.d.....|.k.r"|.
-00001140: 6a00 a003 7c03 a101 0100 0100 711a 7122  j...|.......q.q"
-00001150: 711a 6e06 7c01 7c00 5f00 6404 5300 2905  q.n.|.|._.d.S.).
-00001160: 7aeb 0a20 2020 2020 2020 2053 6574 2074  z..        Set t
-00001170: 6865 2068 6561 6465 7273 206f 6620 6f75  he headers of ou
-00001180: 7220 7772 6974 6572 0a20 2020 2020 2020  r writer.       
-00001190: 203a 7061 7261 6d20 6c69 7374 2068 6561   :param list hea
-000011a0: 6465 7273 3a20 6c69 7374 206f 6620 6469  ders: list of di
-000011b0: 6374 2077 6974 6820 6174 206c 6561 7374  ct with at least
-000011c0: 2061 206c 6162 656c 206b 6579 0a20 2020   a label key.   
-000011d0: 2020 2020 2028 6c61 6265 6c20 6973 206d       (label is m
-000011e0: 616e 6461 746f 7279 203a 2075 7365 6420  andatory : used 
-000011f0: 666f 7220 7468 6520 6578 706f 7274 290a  for the export).
-00001200: 0a20 2020 2020 2020 2048 6561 6465 7273  .        Headers
-00001210: 2061 7265 2066 696c 7465 7265 6420 616e   are filtered an
-00001220: 6420 6f72 6465 7265 6420 7265 6761 7264  d ordered regard
-00001230: 696e 6720 7468 6520 6f72 6465 7220 6f70  ing the order op
-00001240: 7469 6f6e 0a20 2020 2020 2020 20da 056f  tion.        ..o
-00001250: 7264 6572 da03 6b65 7972 4200 0000 4e29  rder..keyrB...N)
-00001260: 0472 2d00 0000 7217 0000 0072 2f00 0000  .r-...r....r/...
-00001270: 7230 0000 0029 0472 1800 0000 722d 0000  r0...).r....r-..
-00001280: 00da 0765 6c65 6d65 6e74 7240 0000 0072  ...elementr@...r
-00001290: 0b00 0000 720b 0000 0072 0c00 0000 da0b  ....r....r......
-000012a0: 7365 745f 6865 6164 6572 73b2 0000 0073  set_headers....s
-000012b0: 1000 0000 0008 0601 0a01 0e01 0801 1401  ................
-000012c0: 0c01 0a02 7a15 586c 7357 7269 7465 722e  ....z.XlsWriter.
-000012d0: 7365 745f 6865 6164 6572 7329 014e 2901  set_headers).N).
-000012e0: 4e29 014e 2911 da08 5f5f 6e61 6d65 5f5f  N).N)...__name__
-000012f0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-00001300: 7175 616c 6e61 6d65 5f5f da07 5f5f 646f  qualname__..__do
-00001310: 635f 5f72 1500 0000 721a 0000 0072 2300  c__r....r....r#.
-00001320: 0000 7227 0000 00da 0373 7472 722c 0000  ..r'.....strr,..
-00001330: 0072 3400 0000 7237 0000 0072 3800 0000  .r4...r7...r8...
-00001340: 7236 0000 0072 3500 0000 7245 0000 0072  r6...r5...rE...r
-00001350: 4900 0000 720b 0000 0072 0b00 0000 720b  I...r....r....r.
-00001360: 0000 0072 0c00 0000 720f 0000 0029 0000  ...r....r....)..
-00001370: 0073 1a00 0000 0801 0411 0402 0a0a 0a0d  .s..............
-00001380: 080e 1008 080e 0807 0a0b 0814 0811 0803  ................
-00001390: 720f 0000 0063 0200 0000 0000 0000 0000  r....c..........
-000013a0: 0000 0600 0000 0400 0000 4300 0000 7356  ..........C...sV
-000013b0: 0000 007c 00a0 0064 01a1 017d 027c 00a0  ...|...d...}.|..
-000013c0: 0064 02a1 017d 037c 0264 0375 0072 527c  .d...}.|.d.u.rR|
-000013d0: 0364 0375 0172 5274 017c 0364 0483 0272  .d.u.rRt.|.d...r
-000013e0: 527c 036a 0264 0519 007d 0474 037c 046a  R|.j.d...}.t.|.j
-000013f0: 0464 067c 046a 0483 037d 0574 05a0 067c  .d.|.j...}.t...|
-00001400: 05a1 017d 027c 0253 0029 077a 9f0a 2020  ...}.|.S.).z..  
-00001410: 2020 5265 7475 726e 2074 6865 2063 656c    Return the cel
-00001420: 6c20 666f 726d 6174 2066 6f72 2074 6865  l format for the
-00001430: 2067 6976 656e 2063 6f6c 756d 6e0a 0a20   given column.. 
-00001440: 2020 203a 7061 7261 6d20 636f 6c75 6d6e     :param column
-00001450: 5f64 6963 743a 2054 6865 2063 6f6c 756d  _dict: The colum
-00001460: 6e20 6461 7461 7320 636f 6c6c 6563 7465  n datas collecte
-00001470: 6420 6475 7269 6e67 2069 6e73 7065 6374  d during inspect
-00001480: 696f 6e0a 2020 2020 3a70 6172 616d 206b  ion.    :param k
-00001490: 6579 3a20 5468 6520 6578 706f 7274 6174  ey: The exportat
-000014a0: 696f 6e20 6b65 790a 2020 2020 7241 0000  ion key.    rA..
-000014b0: 00da 075f 5f63 6f6c 5f5f 4eda 0763 6f6c  ...__col__N..col
-000014c0: 756d 6e73 7201 0000 00da 0469 6d70 6c29  umnsr......impl)
-000014d0: 0772 2f00 0000 722a 0000 0072 5000 0000  .r/...r*...rP...
-000014e0: 722b 0000 00da 0474 7970 65da 0f46 4f52  r+.....type..FOR
-000014f0: 4d41 545f 5245 4749 5354 5259 da08 6765  MAT_REGISTRY..ge
-00001500: 745f 6974 656d 2906 da0b 636f 6c75 6d6e  t_item)...column
-00001510: 5f64 6963 7472 4700 0000 7241 0000 00da  _dictrG...rA....
-00001520: 0470 726f 70da 0b73 716c 615f 636f 6c75  .prop..sqla_colu
-00001530: 6d6e da0b 636f 6c75 6d6e 5f74 7970 6572  mn..column_typer
-00001540: 0b00 0000 720b 0000 0072 0c00 0000 723e  ....r....r....r>
-00001550: 0000 00c5 0000 0073 1000 0000 0007 0a01  .......s........
-00001560: 0a02 1001 0a01 0a01 1001 0a01 723e 0000  ............r>..
-00001570: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00001580: 0000 0300 0000 4000 0000 7336 0000 0065  ......@...s6...e
-00001590: 005a 0164 005a 0264 015a 0364 025a 0464  .Z.d.Z.d.Z.d.Z.d
-000015a0: 0d64 0564 0684 015a 0564 0764 0884 005a  .d.d...Z.d.d...Z
-000015b0: 0664 0964 0a84 005a 0764 0b64 0c84 005a  .d.d...Z.d.d...Z
-000015c0: 0864 0453 0029 0eda 0f53 716c 6158 6c73  .d.S.)...SqlaXls
-000015d0: 4578 706f 7274 6572 617a 0300 000a 2020  Exporteraz....  
-000015e0: 2020 4d61 696e 2063 6c61 7373 2075 7365    Main class use
-000015f0: 6420 666f 7220 6578 706f 7274 696e 6720  d for exporting 
-00001600: 6461 7461 7320 746f 2074 6865 2078 6c73  datas to the xls
-00001610: 2066 6f72 6d61 740a 0a20 2020 204d 6f64   format..    Mod
-00001620: 656c 7320 6174 7472 6962 7574 6573 206f  els attributes o
-00001630: 7574 7075 7420 6361 6e20 6265 2063 7573  utput can be cus
-00001640: 746f 6d69 7a65 6420 7468 726f 7567 6820  tomized through 
-00001650: 7468 6520 696e 666f 2070 6172 616d 203a  the info param :
-00001660: 0a0a 2020 2020 2020 2020 436f 6c75 6d6e  ..        Column
-00001670: 2849 6e74 6567 6572 2c20 696e 666f 733d  (Integer, infos=
-00001680: 7b27 6578 706f 7274 273a 0a20 2020 2020  {'export':.     
-00001690: 2020 2020 2020 207b 2765 7863 656c 273a         {'excel':
-000016a0: 3c65 7863 656c 5f73 7065 6369 6669 635f  <excel_specific_
-000016b0: 6f70 7469 6f6e 733e 2c0a 2020 2020 2020  options>,.      
-000016c0: 2020 2020 2020 203c 6d61 696e 5f65 7870         <main_exp
-000016d0: 6f72 745f 6f70 7469 6f6e 733e 0a20 2020  ort_options>.   
-000016e0: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-000016f0: 2020 207d 0a0a 2020 2020 6d61 696e 5f65     }..    main_e
-00001700: 7870 6f72 745f 6f70 7469 6f6e 7320 616e  xport_options an
-00001710: 6420 6578 6365 6c5f 7370 6563 6966 6963  d excel_specific
-00001720: 5f6f 7074 696f 6e73 2063 616e 2062 6520  _options can be 
-00001730: 3a0a 0a20 2020 2020 2020 206c 6162 656c  :..        label
-00001740: 0a0a 2020 2020 2020 2020 2020 2020 6c61  ..            la
-00001750: 6265 6c20 6f66 2074 6865 2063 6f6c 756d  bel of the colum
-00001760: 6e20 6865 6164 6572 0a0a 2020 2020 2020  n header..      
-00001770: 2020 666f 726d 6174 0a0a 2020 2020 2020    format..      
-00001780: 2020 2020 2020 6120 6675 6e63 7469 6f6e        a function
-00001790: 2074 6861 7420 7769 6c6c 2062 6520 6669   that will be fi
-000017a0: 7265 6420 6f6e 2065 6163 6820 726f 7720  red on each row 
-000017b0: 746f 2066 6f72 6d61 7420 7468 6520 6f75  to format the ou
-000017c0: 7470 7574 0a0a 2020 2020 2020 2020 7265  tput..        re
-000017d0: 6c61 7465 645f 6b65 790a 0a20 2020 2020  lated_key..     
-000017e0: 2020 2020 2020 2049 6620 7468 6520 6174         If the at
-000017f0: 7472 6962 7574 6520 6973 2061 2072 656c  tribute is a rel
-00001800: 6174 696f 6e73 6869 702c 2074 6865 2076  ationship, the v
-00001810: 616c 7565 206f 6620 7468 6520 6769 7665  alue of the give
-00001820: 6e20 6174 7472 6962 7574 650a 2020 2020  n attribute.    
-00001830: 2020 2020 2020 2020 6f66 2074 6865 2072          of the r
-00001840: 656c 6174 6564 206f 626a 6563 7420 7769  elated object wi
-00001850: 6c6c 2062 6520 7573 6564 2074 6f20 6669  ll be used to fi
-00001860: 6c6c 2074 6865 2063 656c 6c73 0a0a 2020  ll the cells..  
-00001870: 2020 2020 2020 6578 636c 7564 650a 0a20        exclude.. 
-00001880: 2020 2020 2020 2020 2020 2054 6869 7320             This 
-00001890: 6461 7461 2077 696c 6c20 6e6f 7420 6265  data will not be
-000018a0: 2069 6e73 6572 7465 6420 696e 2074 6865   inserted in the
-000018b0: 2065 7870 6f72 7420 6966 2054 7275 650a   export if True.
-000018c0: 0a20 2020 2055 7361 6765 3a0a 0a20 2020  .    Usage:..   
-000018d0: 2020 2020 2061 203d 2053 716c 6158 6c73       a = SqlaXls
-000018e0: 4578 706f 7274 6572 284d 794d 6f64 656c  Exporter(MyModel
-000018f0: 290a 2020 2020 2020 2020 666f 7220 6920  ).        for i 
-00001900: 696e 204d 794d 6f64 656c 2e71 7565 7279  in MyModel.query
-00001910: 2829 2e66 696c 7465 7228 3c6d 7966 696c  ().filter(<myfil
-00001920: 7465 723e 293a 0a20 2020 2020 2020 2020  ter>):.         
-00001930: 2020 2061 2e61 6464 5f72 6f77 2869 290a     a.add_row(i).
-00001940: 2020 2020 2020 2020 612e 7265 6e64 6572          a.render
-00001950: 2829 0a20 2020 2072 1f00 0000 544e 6304  ().    r....TNc.
-00001960: 0000 0000 0000 0000 0000 0005 0000 0005  ................
-00001970: 0000 004b 0000 0073 4200 0000 7c02 7c00  ...K...sB...|.|.
-00001980: 5f00 7c03 6400 7500 7c00 5f01 7402 6a03  _.|.d.u.|._.t.j.
-00001990: 7c00 6601 7c02 7c03 6401 9c02 7c04 a401  |.f.|.|.d...|...
-000019a0: 8e01 0100 7404 6a03 7c00 6601 6402 7c01  ....t.j.|.f.d.|.
-000019b0: 6901 7c04 a401 8e01 0100 6400 5300 2903  i.|.......d.S.).
-000019c0: 4e29 02da 0b67 7565 7373 5f74 7970 6573  N)...guess_types
-000019d0: 7214 0000 00da 056d 6f64 656c 2905 725a  r......model).rZ
-000019e0: 0000 00da 0769 735f 726f 6f74 720f 0000  .....is_rootr...
-000019f0: 0072 1a00 0000 7206 0000 0029 0572 1800  .r....r....).r..
-00001a00: 0000 725b 0000 0072 5a00 0000 7214 0000  ..r[...rZ...r...
-00001a10: 0072 1900 0000 720b 0000 0072 0b00 0000  .r....r....r....
-00001a20: 720c 0000 0072 1a00 0000 0001 0000 7308  r....r........s.
-00001a30: 0000 0000 0106 010a 0118 017a 1853 716c  ...........z.Sql
-00001a40: 6158 6c73 4578 706f 7274 6572 2e5f 5f69  aXlsExporter.__i
-00001a50: 6e69 745f 5f63 0300 0000 0000 0000 0000  nit__c..........
-00001a60: 0000 0500 0000 0500 0000 4300 0000 7342  ..........C...sB
-00001a70: 0000 007c 02a0 0064 01a1 017d 037c 0364  ...|...d...}.|.d
-00001a80: 0275 0072 3e7c 006a 016a 027c 02a0 0064  .u.r>|.j.j.|...d
-00001a90: 0364 04a1 0264 058d 017d 0474 037c 016a  .d...d...}.t.|.j
-00001aa0: 047c 0464 068d 0204 007d 037c 0264 013c  .|.d.....}.|.d.<
-00001ab0: 007c 0353 0029 077a 7f0a 2020 2020 2020  .|.S.).z..      
-00001ac0: 2020 7265 7475 726e 7320 616e 2053 716c    returns an Sql
-00001ad0: 6158 6c73 4578 706f 7274 6572 2066 6f72  aXlsExporter for
-00001ae0: 2074 6865 2067 6976 656e 2072 656c 6174   the given relat
-00001af0: 6564 206f 626a 6563 7420 616e 6420 7374  ed object and st
-00001b00: 6f72 6573 2069 740a 2020 2020 2020 2020  ores it.        
-00001b10: 696e 2074 6865 2063 6f6c 756d 6e20 6f62  in the column ob
-00001b20: 6a65 6374 2061 7320 6120 6361 6368 650a  ject as a cache.
-00001b30: 2020 2020 2020 2020 da11 7371 6c61 5f78          ..sqla_x
-00001b40: 6c73 5f65 7870 6f72 7465 724e 7242 0000  ls_exporterNrB..
-00001b50: 007a 0d64 6566 6175 6c74 2074 6974 6c65  .z.default title
-00001b60: 2901 7215 0000 0029 0172 1400 0000 2905  ).r....).r....).
-00001b70: 722f 0000 0072 1200 0000 5a0c 6372 6561  r/...r....Z.crea
-00001b80: 7465 5f73 6865 6574 7259 0000 00da 095f  te_sheetrY....._
-00001b90: 5f63 6c61 7373 5f5f 2905 7218 0000 00da  _class__).r.....
-00001ba0: 0b72 656c 6174 6564 5f6f 626a 7233 0000  .related_objr3..
-00001bb0: 00da 0672 6573 756c 7472 1400 0000 720b  ...resultr....r.
-00001bc0: 0000 0072 0b00 0000 720c 0000 00da 155f  ...r....r......_
-00001bd0: 6765 745f 7265 6c61 7465 645f 6578 706f  get_related_expo
-00001be0: 7274 6572 0601 0000 7312 0000 0000 050a  rter....s.......
-00001bf0: 0108 0106 010a ff06 0302 0106 ff0e 037a  ...............z
-00001c00: 2553 716c 6158 6c73 4578 706f 7274 6572  %SqlaXlsExporter
-00001c10: 2e5f 6765 745f 7265 6c61 7465 645f 6578  ._get_related_ex
-00001c20: 706f 7274 6572 6303 0000 0000 0000 0000  porterc.........
-00001c30: 0000 0009 0000 0005 0000 0043 0000 0073  ...........C...s
-00001c40: 7e00 0000 7400 a001 7c00 7c01 7c02 a103  ~...t...|.|.|...
-00001c50: 7d03 7c03 6401 6b02 727a 7c02 a002 6402  }.|.d.k.rz|...d.
-00001c60: 6403 a102 7d04 7c02 6404 1900 6a03 727a  d...}.|.d...j.rz
-00001c70: 7c04 6403 7500 727a 7c00 6a04 727a 7c02  |.d.u.rz|.j.rz|.
-00001c80: 6405 1900 7d05 7405 7c01 7c05 6403 8303  d...}.t.|.|.d...
-00001c90: 7d06 7c06 7356 6401 5300 7c00 a006 7c06  }.|.sVd.S.|...|.
-00001ca0: 6406 1900 7c02 a102 7d07 7c06 4400 5d0e  d...|...}.|.D.].
-00001cb0: 7d08 7c07 a007 7c08 a101 0100 716a 7c03  }.|...|.....qj|.
-00001cc0: 5300 2907 7a86 0a20 2020 2020 2020 2052  S.).z..        R
-00001cd0: 6574 7572 6e20 7468 6520 7661 6c75 6520  eturn the value 
-00001ce0: 746f 2069 6e73 6572 7420 696e 2061 2072  to insert in a r
-00001cf0: 656c 6174 696f 6e73 6869 7020 6365 6c6c  elationship cell
-00001d00: 0a20 2020 2020 2020 2048 616e 646c 6520  .        Handle 
-00001d10: 7468 6520 6361 7365 206f 6620 636f 6d70  the case of comp
-00001d20: 6c65 7820 7265 6c61 7465 6420 6461 7461  lex related data
-00001d30: 7320 7765 2077 616e 7420 746f 2068 616e  s we want to han
-00001d40: 646c 650a 2020 2020 2020 2020 7208 0000  dle.        r...
-00001d50: 00da 0b72 656c 6174 6564 5f6b 6579 4e72  ...related_keyNr
-00001d60: 4f00 0000 7247 0000 0072 0100 0000 2908  O...rG...r....).
-00001d70: 7206 0000 00da 1a5f 6765 745f 7265 6c61  r......_get_rela
-00001d80: 7469 6f6e 7368 6970 5f63 656c 6c5f 7661  tionship_cell_va
-00001d90: 6c72 2f00 0000 da07 7573 656c 6973 7472  lr/.....uselistr
-00001da0: 5c00 0000 722b 0000 0072 6100 0000 da07  \...r+...ra.....
-00001db0: 6164 645f 726f 7729 0972 1800 0000 da03  add_row).r......
-00001dc0: 6f62 6a72 3300 0000 da03 7661 6c72 6200  objr3.....valrb.
-00001dd0: 0000 7247 0000 005a 0f72 656c 6174 6564  ..rG...Z.related
-00001de0: 5f6f 626a 6563 7473 5a08 6578 706f 7274  _objectsZ.export
-00001df0: 6572 da07 7265 6c5f 6f62 6a72 0b00 0000  er..rel_objr....
-00001e00: 720b 0000 0072 0c00 0000 7263 0000 0015  r....r....rc....
-00001e10: 0100 0073 1e00 0000 0005 0e01 0801 0c02  ...s............
-00001e20: 1803 0801 0c01 0401 0402 0401 0601 02fe  ................
-00001e30: 0404 0801 0c02 7a2a 5371 6c61 586c 7345  ......z*SqlaXlsE
-00001e40: 7870 6f72 7465 722e 5f67 6574 5f72 656c  xporter._get_rel
-00001e50: 6174 696f 6e73 6869 705f 6365 6c6c 5f76  ationship_cell_v
-00001e60: 616c 6301 0000 0000 0000 0000 0000 0002  alc.............
-00001e70: 0000 0003 0000 0043 0000 0073 2e00 0000  .......C...s....
-00001e80: 7400 a001 7c00 a101 0100 7c00 6a02 4400  t...|.....|.j.D.
-00001e90: 5d18 7d01 6401 7c01 7600 7210 7c01 6401  ].}.d.|.v.r.|.d.
-00001ea0: 1900 a001 a100 0100 7110 6402 5300 2903  ........q.d.S.).
-00001eb0: 7a52 0a20 2020 2020 2020 2045 6e68 616e  zR.        Enhan
-00001ec0: 6365 2074 6865 2064 6566 6175 6c74 2070  ce the default p
-00001ed0: 6f70 756c 6174 6520 7363 7269 7074 2062  opulate script b
-00001ee0: 7920 6861 6e64 6c69 6e67 2072 656c 6174  y handling relat
-00001ef0: 6564 2065 6c65 6d65 6e74 730a 2020 2020  ed elements.    
-00001f00: 2020 2020 725d 0000 004e 2903 720f 0000      r]...N).r...
-00001f10: 0072 3700 0000 722d 0000 0029 0272 1800  .r7...r-...).r..
-00001f20: 0000 7240 0000 0072 0b00 0000 720b 0000  ..r@...r....r...
-00001f30: 0072 0c00 0000 7237 0000 002f 0100 0073  .r....r7.../...s
-00001f40: 0800 0000 0004 0a01 0a01 0801 7a19 5371  ............z.Sq
-00001f50: 6c61 586c 7345 7870 6f72 7465 722e 5f70  laXlsExporter._p
-00001f60: 6f70 756c 6174 6529 0254 4e29 0972 4a00  opulate).TN).rJ.
-00001f70: 0000 724b 0000 0072 4c00 0000 724d 0000  ..rK...rL...rM..
-00001f80: 00da 0a63 6f6e 6669 675f 6b65 7972 1a00  ...config_keyr..
-00001f90: 0000 7261 0000 0072 6300 0000 7237 0000  ..ra...rc...r7..
-00001fa0: 0072 0b00 0000 720b 0000 0072 0b00 0000  .r....r....r....
-00001fb0: 720c 0000 0072 5900 0000 d700 0000 730c  r....rY.......s.
-00001fc0: 0000 0008 0104 2604 020a 0608 0f08 1a72  ......&........r
-00001fd0: 5900 0000 6300 0000 0000 0000 0000 0000  Y...c...........
-00001fe0: 0000 0000 0003 0000 0040 0000 0073 1e00  .........@...s..
-00001ff0: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
-00002000: 5a04 6407 6404 6405 8401 5a05 6406 5300  Z.d.d.d...Z.d.S.
-00002010: 2908 da0b 586c 7345 7870 6f72 7465 727a  )...XlsExporterz
-00002020: bc0a 2020 2020 4120 6d61 696e 2078 6c73  ..    A main xls
-00002030: 2065 7870 6f72 7461 7469 6f6e 2074 6f6f   exportation too
-00002040: 6c20 2877 6974 686f 7574 2073 716c 616c  l (without sqlal
-00002050: 6368 656d 7920 7375 7070 6f72 7429 0a0a  chemy support)..
-00002060: 2020 2020 7772 6974 6572 203d 204d 7958      writer = MyX
-00002070: 6c73 4578 706f 7274 6572 2829 0a20 2020  lsExporter().   
-00002080: 2077 7269 7465 722e 6164 645f 726f 7728   writer.add_row(
-00002090: 7b27 6b65 7927 3a20 7527 4c61 2076 616c  {'key': u'La val
-000020a0: 6575 7220 6465 206c 6120 6365 6c6c 756c  eur de la cellul
-000020b0: 6520 6465 206c 6120 636f 6c6f 6e6e 6520  e de la colonne 
-000020c0: 3127 7d29 0a20 2020 2077 7269 7465 722e  1'}).    writer.
-000020d0: 7265 6e64 6572 2829 0a20 2020 2072 0b00  render().    r..
-000020e0: 0000 5463 0200 0000 0000 0000 0000 0000  ..Tc............
-000020f0: 0300 0000 0400 0000 4b00 0000 732c 0000  ........K...s,..
-00002100: 0074 006a 017c 0066 0164 017c 0169 017c  .t.j.|.f.d.|.i.|
-00002110: 02a4 018e 0101 0074 026a 017c 0066 0169  .......t.j.|.f.i
-00002120: 007c 02a4 018e 0101 0064 0053 0029 024e  .|.......d.S.).N
-00002130: 725a 0000 0029 0372 0f00 0000 721a 0000  rZ...).r....r...
-00002140: 0072 0500 0000 2903 7218 0000 0072 5a00  .r....).r....rZ.
-00002150: 0000 7219 0000 0072 0b00 0000 720b 0000  ..r....r....r...
-00002160: 0072 0c00 0000 721a 0000 0044 0100 0073  .r....r....D...s
-00002170: 0400 0000 0001 1601 7a14 586c 7345 7870  ........z.XlsExp
-00002180: 6f72 7465 722e 5f5f 696e 6974 5f5f 4e29  orter.__init__N)
-00002190: 0154 2906 724a 0000 0072 4b00 0000 724c  .T).rJ...rK...rL
-000021a0: 0000 0072 4d00 0000 722d 0000 0072 1a00  ...rM...r-...r..
-000021b0: 0000 720b 0000 0072 0b00 0000 720b 0000  ..r....r....r...
-000021c0: 0072 0c00 0000 726a 0000 0039 0100 0073  .r....rj...9...s
-000021d0: 0600 0000 0801 0408 0402 726a 0000 0029  ..........rj...)
-000021e0: 014e 2921 724d 0000 00da 0862 7569 6c74  .N)!rM.....built
-000021f0: 696e 73da 0c40 7079 5f62 7569 6c74 696e  ins..@py_builtin
-00002200: 73da 195f 7079 7465 7374 2e61 7373 6572  s.._pytest.asser
-00002210: 7469 6f6e 2e72 6577 7269 7465 da09 6173  tion.rewrite..as
-00002220: 7365 7274 696f 6eda 0772 6577 7269 7465  sertion..rewrite
-00002230: da0a 4070 7974 6573 745f 6172 da09 6974  ..@pytest_ar..it
-00002240: 6572 746f 6f6c 73da 076c 6f67 6769 6e67  ertools..logging
-00002250: 7211 0000 005a 0f6f 7065 6e70 7978 6c2e  r....Z.openpyxl.
-00002260: 7374 796c 6573 7202 0000 0072 0300 0000  stylesr....r....
-00002270: 721b 0000 00da 0673 7472 696e 6772 0400  r......stringr..
-00002280: 0000 da13 7371 6c61 5f69 6e73 7065 6374  ....sqla_inspect
-00002290: 2e65 7870 6f72 7472 0500 0000 7206 0000  .exportr....r...
-000022a0: 005a 1173 716c 615f 696e 7370 6563 742e  .Z.sqla_inspect.
-000022b0: 6261 7365 7207 0000 00da 0967 6574 4c6f  baser......getLo
-000022c0: 6767 6572 724a 0000 00da 036c 6f67 da04  ggerrJ.....log..
-000022d0: 6c69 7374 da1d 636f 6d62 696e 6174 696f  list..combinatio
-000022e0: 6e73 5f77 6974 685f 7265 706c 6163 656d  ns_with_replacem
-000022f0: 656e 745a 0f41 5343 4949 5f55 5050 4552  entZ.ASCII_UPPER
-00002300: 4341 5345 7253 0000 00da 066f 626a 6563  CASErS.....objec
-00002310: 7472 0f00 0000 723e 0000 0072 5900 0000  tr....r>...rY...
-00002320: 726a 0000 0072 0b00 0000 720b 0000 0072  rj...r....r....r
-00002330: 0b00 0000 720c 0000 00da 083c 6d6f 6475  ....r......<modu
-00002340: 6c65 3e06 0000 0073 2400 0000 0404 2201  le>....s$.....".
-00002350: 0801 0801 1005 0801 0c02 1004 0c03 0a04  ................
-00002360: 0e02 0afe 0a06 0603 107f 001d 0a12 1262  ...............b
+00000670: 2020 2020 4eda 0473 6176 6572 0100 0000      N..saver....
+00000680: 290b da02 696f da07 4279 7465 7349 4fda  )...io..BytesIO.
+00000690: 0768 6173 6174 7472 7213 0000 0072 1c00  .hasattrr....r..
+000006a0: 0000 da05 7772 6974 6572 1200 0000 da06  ....writer......
+000006b0: 7772 6974 6572 da05 6578 6365 6c5a 1573  writer..excelZ.s
+000006c0: 6176 655f 7669 7274 7561 6c5f 776f 726b  ave_virtual_work
+000006d0: 626f 6f6b da04 7365 656b a902 7219 0000  book..seek..r...
+000006e0: 00da 0566 5f62 7566 720b 0000 0072 0b00  ...f_bufr....r..
+000006f0: 0000 720c 0000 00da 0973 6176 655f 626f  ..r......save_bo
+00000700: 6f6b 4700 0000 730e 0000 0000 0708 0108  okG...s.........
+00000710: 020c 010e 0316 020a 017a 1358 6c73 5772  .........z.XlsWr
+00000720: 6974 6572 2e73 6176 655f 626f 6f6b 6303  iter.save_bookc.
+00000730: 0000 0000 0000 0000 0000 0003 0000 0004  ................
+00000740: 0000 0043 0000 0073 1600 0000 7400 7401  ...C...s....t.t.
+00000750: 7c02 6401 8d01 6402 8d01 7c01 5f02 6403  |.d...d...|._.d.
+00000760: 5300 2904 7aa8 0a20 2020 2020 2020 2053  S.).z..        S
+00000770: 6574 2074 6865 2067 6976 656e 2063 6f6c  et the given col
+00000780: 6f72 2074 6f20 7468 6520 7072 6f76 6964  or to the provid
+00000790: 6564 2063 656c 6c0a 0a20 2020 2020 2020  ed cell..       
+000007a0: 2020 2020 2063 656c 6c0a 0a20 2020 2020       cell..     
+000007b0: 2020 2020 2020 2020 2020 2041 2078 6c73             A xls
+000007c0: 2063 656c 6c20 6f62 6a65 6374 0a0a 2020   cell object..  
+000007d0: 2020 2020 2020 2020 2020 636f 6c6f 720a            color.
+000007e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000007f0: 2041 206f 7065 6e70 7978 6c20 636f 6c6f   A openpyxl colo
+00000800: 7220 7661 720a 2020 2020 2020 2020 2901  r var.        ).
+00000810: da03 7267 6229 01da 0563 6f6c 6f72 4e29  ..rgb)...colorN)
+00000820: 0372 0300 0000 7202 0000 00da 0466 6f6e  .r....r......fon
+00000830: 7429 0372 1900 0000 da04 6365 6c6c 7228  t).r......cellr(
+00000840: 0000 0072 0b00 0000 720b 0000 0072 0c00  ...r....r....r..
+00000850: 0000 da09 7365 745f 636f 6c6f 725a 0000  ....set_colorZ..
+00000860: 0073 0200 0000 000c 7a13 586c 7357 7269  .s......z.XlsWri
+00000870: 7465 722e 7365 745f 636f 6c6f 7229 02da  ter.set_color)..
+00000880: 0b63 6f6c 756d 6e5f 6e61 6d65 da05 7661  .column_name..va
+00000890: 6c75 6563 0300 0000 0000 0000 0000 0000  luec............
+000008a0: 0300 0000 0400 0000 4300 0000 7324 0000  ........C...s$..
+000008b0: 0074 007c 0064 017c 0116 0083 0272 2074  .t.|.d.|.....r t
+000008c0: 017c 0064 017c 0116 0083 027c 0283 017d  .|.d.|.....|...}
+000008d0: 027c 0253 0029 027a 1f0a 2020 2020 2020  .|.S.).z..      
+000008e0: 2020 466f 726d 6174 2061 2063 656c 6c0a    Format a cell.
+000008f0: 2020 2020 2020 2020 7a09 666f 726d 6174          z.format
+00000900: 5f25 7329 0272 1f00 0000 da07 6765 7461  _%s).r......geta
+00000910: 7474 7229 0372 1900 0000 722c 0000 0072  ttr).r....r,...r
+00000920: 2d00 0000 720b 0000 0072 0b00 0000 720c  -...r....r....r.
+00000930: 0000 00da 0b66 6f72 6d61 745f 6365 6c6c  .....format_cell
+00000940: 6800 0000 7306 0000 0000 040e 0112 017a  h...s..........z
+00000950: 1558 6c73 5772 6974 6572 2e66 6f72 6d61  .XlsWriter.forma
+00000960: 745f 6365 6c6c 6302 0000 0000 0000 0000  t_cellc.........
+00000970: 0000 0007 0000 0005 0000 0043 0000 0073  ...........C...s
+00000980: 4800 0000 6700 7d02 7400 7c00 6401 6700  H...g.}.t.|.d.g.
+00000990: 8303 7d03 7c03 4400 5d2e 7d04 7c04 6402  ..}.|.D.].}.|.d.
+000009a0: 1900 7d05 7c01 a001 7c05 6403 a102 7d06  ..}.|...|.d...}.
+000009b0: 7c00 a002 7c05 7c06 a102 7d06 7c02 a003  |...|.|...}.|...
+000009c0: 7c06 a101 0100 7114 7c02 5300 2904 7a96  |.....q.|.S.).z.
+000009d0: 0a20 2020 2020 2020 2054 6865 2072 656e  .        The ren
+000009e0: 6465 7220 6d65 7468 6f64 2065 7870 6563  der method expec
+000009f0: 7473 2072 6f77 7320 6173 206c 6973 7473  ts rows as lists
+00000a00: 2c20 6865 7265 2077 6520 7377 6974 6368  , here we switch
+00000a10: 206f 7572 2072 6f77 2066 6f72 6d61 740a   our row format.
+00000a20: 2020 2020 2020 2020 6672 6f6d 2064 6963          from dic
+00000a30: 7420 746f 206c 6973 7420 7265 7370 6563  t to list respec
+00000a40: 7469 6e67 2074 6865 206f 7264 6572 206f  ting the order o
+00000a50: 6620 7468 6520 6865 6164 6572 730a 2020  f the headers.  
+00000a60: 2020 2020 2020 da07 6865 6164 6572 73da        ..headers.
+00000a70: 046e 616d 6572 0800 0000 2904 722e 0000  .namer....).r...
+00000a80: 00da 0367 6574 722f 0000 00da 0661 7070  ...getr/.....app
+00000a90: 656e 6429 0772 1900 0000 da03 726f 77da  end).r......row.
+00000aa0: 0372 6573 7230 0000 00da 0663 6f6c 756d  .resr0.....colum
+00000ab0: 6e72 2c00 0000 722d 0000 0072 0b00 0000  nr,...r-...r....
+00000ac0: 720b 0000 0072 0c00 0000 da0a 666f 726d  r....r......form
+00000ad0: 6174 5f72 6f77 7000 0000 7310 0000 0000  at_rowp...s.....
+00000ae0: 0504 010c 0108 0108 010c 010c 010c 017a  ...............z
+00000af0: 1458 6c73 5772 6974 6572 2e66 6f72 6d61  .XlsWriter.forma
+00000b00: 745f 726f 7763 0100 0000 0000 0000 0000  t_rowc..........
+00000b10: 0000 0100 0000 0200 0000 4300 0000 7314  ..........C...s.
+00000b20: 0000 007c 00a0 00a1 0001 007c 00a0 01a1  ...|.......|....
+00000b30: 0001 0064 0153 0029 027a 430a 2020 2020  ...d.S.).zC.    
+00000b40: 2020 2020 506f 7075 6c61 7465 2068 6561      Populate hea
+00000b50: 6465 7273 2061 6e64 2072 6f77 7320 6265  ders and rows be
+00000b60: 666f 7265 2077 7269 7469 6e67 206f 7572  fore writing our
+00000b70: 2062 6f6f 6b0a 2020 2020 2020 2020 4e29   book.        N)
+00000b80: 02da 0f5f 7265 6e64 6572 5f68 6561 6465  ..._render_heade
+00000b90: 7273 da0c 5f72 656e 6465 725f 726f 7773  rs.._render_rows
+00000ba0: 2901 7219 0000 0072 0b00 0000 720b 0000  ).r....r....r...
+00000bb0: 0072 0c00 0000 da09 5f70 6f70 756c 6174  .r......_populat
+00000bc0: 657e 0000 0073 0400 0000 0004 0801 7a13  e~...s........z.
+00000bd0: 586c 7357 7269 7465 722e 5f70 6f70 756c  XlsWriter._popul
+00000be0: 6174 6563 0200 0000 0000 0000 0000 0000  atec............
+00000bf0: 0200 0000 0300 0000 4300 0000 7312 0000  ........C...s...
+00000c00: 007c 00a0 00a1 0001 007c 00a0 017c 01a1  .|.......|...|..
+00000c10: 0153 0029 017a 870a 2020 2020 2020 2020  .S.).z..        
+00000c20: 4465 6669 6e69 7465 6c79 2072 656e 6465  Definitely rende
+00000c30: 7220 7468 6520 776f 726b 626f 6f6b 0a0a  r the workbook..
+00000c40: 2020 2020 2020 2020 3a70 6172 616d 206f          :param o
+00000c50: 626a 2066 5f62 7566 3a20 4120 6669 6c65  bj f_buf: A file
+00000c60: 2062 7566 6665 7220 7375 7070 6f72 7469   buffer supporti
+00000c70: 6e67 2074 6865 2077 7269 7465 2061 6e64  ng the write and
+00000c80: 2073 6565 6b0a 2020 2020 2020 2020 6d65   seek.        me
+00000c90: 7468 6f64 730a 2020 2020 2020 2020 2902  thods.        ).
+00000ca0: 723a 0000 0072 2600 0000 7224 0000 0072  r:...r&...r$...r
+00000cb0: 0b00 0000 720b 0000 0072 0c00 0000 da06  ....r....r......
+00000cc0: 7265 6e64 6572 8500 0000 7304 0000 0000  render....s.....
+00000cd0: 0708 027a 1058 6c73 5772 6974 6572 2e72  ...z.XlsWriter.r
+00000ce0: 656e 6465 7263 0100 0000 0000 0000 0000  enderc..........
+00000cf0: 0000 0b00 0000 0600 0000 4300 0000 739c  ..........C...s.
+00000d00: 0000 0074 007c 0064 0164 0283 037d 0174  ...t.|.d.d...}.t
+00000d10: 007c 0064 0364 0283 037d 0274 017c 0183  .|.d.d...}.t.|..
+00000d20: 0144 005d 765c 027d 037d 047c 0364 0417  .D.]v\.}.}.|.d..
+00000d30: 007d 0574 017c 0483 0144 005d 5c5c 027d  .}.t.|...D.]\\.}
+00000d40: 067d 077c 006a 026a 037c 057c 0664 0517  .}.|.j.j.|.|.d..
+00000d50: 0064 068d 027d 087c 0764 0775 0172 647c  .d...}.|.d.u.rd|
+00000d60: 077c 085f 046e 0664 087c 085f 0474 057c  .|._.n.d.|._.t.|
+00000d70: 0283 017c 066b 0472 387c 027c 0619 007d  ...|.k.r8|.|...}
+00000d80: 0974 067c 0983 017d 0a7c 0a64 0775 0172  .t.|...}.|.d.u.r
+00000d90: 387c 0a7c 085f 0771 3871 2064 0753 0029  8|.|._.q8q d.S.)
+00000da0: 097a 3b0a 2020 2020 2020 2020 5265 6e64  .z;.        Rend
+00000db0: 6572 2074 6865 2072 6f77 7320 696e 2074  er the rows in t
+00000dc0: 6865 2063 7572 7265 6e74 2073 7479 6c65  he current style
+00000dd0: 7368 6565 740a 2020 2020 2020 2020 da06  sheet.        ..
+00000de0: 5f64 6174 6173 720b 0000 0072 3000 0000  _datasr....r0...
+00000df0: 720e 0000 00e9 0100 0000 a902 7234 0000  r...........r4..
+00000e00: 0072 3600 0000 4e72 0800 0000 2908 722e  .r6...Nr....).r.
+00000e10: 0000 00da 0965 6e75 6d65 7261 7465 7215  .....enumerater.
+00000e20: 0000 0072 2a00 0000 722d 0000 00da 036c  ...r*...r-.....l
+00000e30: 656e da0f 6765 745f 6365 6c6c 5f66 6f72  en..get_cell_for
+00000e40: 6d61 745a 0d6e 756d 6265 725f 666f 726d  matZ.number_form
+00000e50: 6174 290b 7219 0000 0072 3c00 0000 7230  at).r....r<...r0
+00000e60: 0000 00da 0569 6e64 6578 7234 0000 00da  .....indexr4....
+00000e70: 0a72 6f77 5f6e 756d 6265 725a 0763 6f6c  .row_numberZ.col
+00000e80: 5f6e 756d 722d 0000 0072 2a00 0000 da06  _numr-...r*.....
+00000e90: 6865 6164 6572 da06 666f 726d 6174 720b  header..formatr.
+00000ea0: 0000 0072 0b00 0000 720c 0000 0072 3900  ...r....r....r9.
+00000eb0: 0000 9000 0000 731c 0000 0000 040c 010c  ......s.........
+00000ec0: 0110 0108 0110 0114 0108 0108 0206 010c  ................
+00000ed0: 0108 0108 0108 017a 1658 6c73 5772 6974  .......z.XlsWrit
+00000ee0: 6572 2e5f 7265 6e64 6572 5f72 6f77 7363  er._render_rowsc
+00000ef0: 0100 0000 0000 0000 0000 0000 0700 0000  ................
+00000f00: 0500 0000 4300 0000 7388 0000 0074 007c  ....C...s....t.|
+00000f10: 0064 0164 0283 037d 0174 017c 0183 0144  .d.d...}.t.|...D
+00000f20: 005d 265c 027d 027d 037c 006a 026a 0364  .]&\.}.}.|.j.j.d
+00000f30: 037c 0264 0317 0064 048d 027d 047c 0364  .|.d...d...}.|.d
+00000f40: 0519 007c 045f 0471 147c 0264 0337 007d  ...|._.q.|.d.7.}
+00000f50: 0274 007c 0064 0664 0283 037d 0574 017c  .t.|.d.d...}.t.|
+00000f60: 0583 0144 005d 2a5c 027d 067d 037c 006a  ...D.]*\.}.}.|.j
+00000f70: 026a 0364 037c 067c 0217 0064 0317 0064  .j.d.|.|...d...d
+00000f80: 048d 027d 047c 0364 0519 007c 045f 0471  ...}.|.d...|._.q
+00000f90: 5864 0753 0029 087a 270a 2020 2020 2020  Xd.S.).z'.      
+00000fa0: 2020 5772 6974 6520 7468 6520 6865 6164    Write the head
+00000fb0: 6572 7320 726f 770a 2020 2020 2020 2020  ers row.        
+00000fc0: 7230 0000 0072 0b00 0000 723d 0000 0072  r0...r....r=...r
+00000fd0: 3e00 0000 da05 6c61 6265 6cda 0d65 7874  >.....label..ext
+00000fe0: 7261 5f68 6561 6465 7273 4e29 0572 2e00  ra_headersN).r..
+00000ff0: 0000 723f 0000 0072 1500 0000 722a 0000  ..r?...r....r*..
+00001000: 0072 2d00 0000 2907 7219 0000 0072 3000  .r-...).r....r0.
+00001010: 0000 7242 0000 00da 0363 6f6c 722a 0000  ..rB.....colr*..
+00001020: 0072 4700 0000 5a09 6164 645f 696e 6465  .rG...Z.add_inde
+00001030: 7872 0b00 0000 720b 0000 0072 0c00 0000  xr....r....r....
+00001040: 7238 0000 00a4 0000 0073 1200 0000 0004  r8.......s......
+00001050: 0c01 1002 1401 0c02 0802 0c01 1001 1801  ................
+00001060: 7a19 586c 7357 7269 7465 722e 5f72 656e  z.XlsWriter._ren
+00001070: 6465 725f 6865 6164 6572 7363 0200 0000  der_headersc....
+00001080: 0000 0000 0000 0000 0200 0000 0200 0000  ................
+00001090: 4300 0000 730c 0000 007c 017c 006a 005f  C...s....|.|.j._
+000010a0: 0164 0053 0072 1100 0000 2902 7215 0000  .d.S.r....).r...
+000010b0: 0072 1600 0000 2902 7219 0000 0072 1600  .r....).r....r..
+000010c0: 0000 720b 0000 0072 0b00 0000 720c 0000  ..r....r....r...
+000010d0: 00da 0973 6574 5f74 6974 6c65 b500 0000  ...set_title....
+000010e0: 7302 0000 0000 017a 1358 6c73 5772 6974  s......z.XlsWrit
+000010f0: 6572 2e73 6574 5f74 6974 6c65 6302 0000  er.set_titlec...
+00001100: 0000 0000 0000 0000 0004 0000 0007 0000  ................
+00001110: 0043 0000 0073 5a00 0000 6700 7c00 5f00  .C...sZ...g.|._.
+00001120: 6401 7c00 6a01 7600 7250 7c00 6a01 6401  d.|.j.v.rP|.j.d.
+00001130: 1900 4400 5d32 7d02 7c01 4400 5d28 7d03  ..D.]2}.|.D.](}.
+00001140: 7c03 a002 6402 7c03 6403 1900 a102 7c02  |...d.|.d.....|.
+00001150: 6b02 7222 7c00 6a00 a003 7c03 a101 0100  k.r"|.j...|.....
+00001160: 0100 711a 7122 711a 6e06 7c01 7c00 5f00  ..q.q"q.n.|.|._.
+00001170: 6404 5300 2905 7aeb 0a20 2020 2020 2020  d.S.).z..       
+00001180: 2053 6574 2074 6865 2068 6561 6465 7273   Set the headers
+00001190: 206f 6620 6f75 7220 7772 6974 6572 0a20   of our writer. 
+000011a0: 2020 2020 2020 203a 7061 7261 6d20 6c69         :param li
+000011b0: 7374 2068 6561 6465 7273 3a20 6c69 7374  st headers: list
+000011c0: 206f 6620 6469 6374 2077 6974 6820 6174   of dict with at
+000011d0: 206c 6561 7374 2061 206c 6162 656c 206b   least a label k
+000011e0: 6579 0a20 2020 2020 2020 2028 6c61 6265  ey.        (labe
+000011f0: 6c20 6973 206d 616e 6461 746f 7279 203a  l is mandatory :
+00001200: 2075 7365 6420 666f 7220 7468 6520 6578   used for the ex
+00001210: 706f 7274 290a 0a20 2020 2020 2020 2048  port)..        H
+00001220: 6561 6465 7273 2061 7265 2066 696c 7465  eaders are filte
+00001230: 7265 6420 616e 6420 6f72 6465 7265 6420  red and ordered 
+00001240: 7265 6761 7264 696e 6720 7468 6520 6f72  regarding the or
+00001250: 6465 7220 6f70 7469 6f6e 0a20 2020 2020  der option.     
+00001260: 2020 20da 056f 7264 6572 da03 6b65 7972     ..order..keyr
+00001270: 4600 0000 4e29 0472 3000 0000 7218 0000  F...N).r0...r...
+00001280: 0072 3200 0000 7233 0000 0029 0472 1900  .r2...r3...).r..
+00001290: 0000 7230 0000 00da 0765 6c65 6d65 6e74  ..r0.....element
+000012a0: 7244 0000 0072 0b00 0000 720b 0000 0072  rD...r....r....r
+000012b0: 0c00 0000 da0b 7365 745f 6865 6164 6572  ......set_header
+000012c0: 73b8 0000 0073 1000 0000 0008 0601 0a01  s....s..........
+000012d0: 0e01 0801 1401 0c01 0a02 7a15 586c 7357  ..........z.XlsW
+000012e0: 7269 7465 722e 7365 745f 6865 6164 6572  riter.set_header
+000012f0: 7329 014e 2901 4e29 014e 2911 da08 5f5f  s).N).N).N)...__
+00001300: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
+00001310: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
+00001320: da07 5f5f 646f 635f 5f72 1600 0000 721b  ..__doc__r....r.
+00001330: 0000 0072 2600 0000 722b 0000 00da 0373  ...r&...r+.....s
+00001340: 7472 722f 0000 0072 3700 0000 723a 0000  trr/...r7...r:..
+00001350: 0072 3b00 0000 7239 0000 0072 3800 0000  .r;...r9...r8...
+00001360: 7249 0000 0072 4d00 0000 720b 0000 0072  rI...rM...r....r
+00001370: 0b00 0000 720b 0000 0072 0c00 0000 720f  ....r....r....r.
+00001380: 0000 0029 0000 0073 1a00 0000 0801 0411  ...)...s........
+00001390: 0402 0a0a 0a13 080e 1008 080e 0807 0a0b  ................
+000013a0: 0814 0811 0803 720f 0000 0063 0200 0000  ......r....c....
+000013b0: 0000 0000 0000 0000 0600 0000 0400 0000  ................
+000013c0: 4300 0000 7356 0000 007c 00a0 0064 01a1  C...sV...|...d..
+000013d0: 017d 027c 00a0 0064 02a1 017d 037c 0264  .}.|...d...}.|.d
+000013e0: 0375 0072 527c 0364 0375 0172 5274 017c  .u.rR|.d.u.rRt.|
+000013f0: 0364 0483 0272 527c 036a 0264 0519 007d  .d...rR|.j.d...}
+00001400: 0474 037c 046a 0464 067c 046a 0483 037d  .t.|.j.d.|.j...}
+00001410: 0574 05a0 067c 05a1 017d 027c 0253 0029  .t...|...}.|.S.)
+00001420: 077a 9f0a 2020 2020 5265 7475 726e 2074  .z..    Return t
+00001430: 6865 2063 656c 6c20 666f 726d 6174 2066  he cell format f
+00001440: 6f72 2074 6865 2067 6976 656e 2063 6f6c  or the given col
+00001450: 756d 6e0a 0a20 2020 203a 7061 7261 6d20  umn..    :param 
+00001460: 636f 6c75 6d6e 5f64 6963 743a 2054 6865  column_dict: The
+00001470: 2063 6f6c 756d 6e20 6461 7461 7320 636f   column datas co
+00001480: 6c6c 6563 7465 6420 6475 7269 6e67 2069  llected during i
+00001490: 6e73 7065 6374 696f 6e0a 2020 2020 3a70  nspection.    :p
+000014a0: 6172 616d 206b 6579 3a20 5468 6520 6578  aram key: The ex
+000014b0: 706f 7274 6174 696f 6e20 6b65 790a 2020  portation key.  
+000014c0: 2020 7245 0000 00da 075f 5f63 6f6c 5f5f    rE.....__col__
+000014d0: 4eda 0763 6f6c 756d 6e73 7201 0000 00da  N..columnsr.....
+000014e0: 0469 6d70 6c29 0772 3200 0000 721f 0000  .impl).r2...r...
+000014f0: 0072 5400 0000 722e 0000 00da 0474 7970  .rT...r......typ
+00001500: 65da 0f46 4f52 4d41 545f 5245 4749 5354  e..FORMAT_REGIST
+00001510: 5259 da08 6765 745f 6974 656d 2906 da0b  RY..get_item)...
+00001520: 636f 6c75 6d6e 5f64 6963 7472 4b00 0000  column_dictrK...
+00001530: 7245 0000 00da 0470 726f 70da 0b73 716c  rE.....prop..sql
+00001540: 615f 636f 6c75 6d6e da0b 636f 6c75 6d6e  a_column..column
+00001550: 5f74 7970 6572 0b00 0000 720b 0000 0072  _typer....r....r
+00001560: 0c00 0000 7241 0000 00cb 0000 0073 1000  ....rA.......s..
+00001570: 0000 0007 0a01 0a02 1001 0a01 0a01 1001  ................
+00001580: 0a01 7241 0000 0063 0000 0000 0000 0000  ..rA...c........
+00001590: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
+000015a0: 7336 0000 0065 005a 0164 005a 0264 015a  s6...e.Z.d.Z.d.Z
+000015b0: 0364 025a 0464 0d64 0564 0684 015a 0564  .d.Z.d.d.d...Z.d
+000015c0: 0764 0884 005a 0664 0964 0a84 005a 0764  .d...Z.d.d...Z.d
+000015d0: 0b64 0c84 005a 0864 0453 0029 0eda 0f53  .d...Z.d.S.)...S
+000015e0: 716c 6158 6c73 4578 706f 7274 6572 617a  qlaXlsExporteraz
+000015f0: 0300 000a 2020 2020 4d61 696e 2063 6c61  ....    Main cla
+00001600: 7373 2075 7365 6420 666f 7220 6578 706f  ss used for expo
+00001610: 7274 696e 6720 6461 7461 7320 746f 2074  rting datas to t
+00001620: 6865 2078 6c73 2066 6f72 6d61 740a 0a20  he xls format.. 
+00001630: 2020 204d 6f64 656c 7320 6174 7472 6962     Models attrib
+00001640: 7574 6573 206f 7574 7075 7420 6361 6e20  utes output can 
+00001650: 6265 2063 7573 746f 6d69 7a65 6420 7468  be customized th
+00001660: 726f 7567 6820 7468 6520 696e 666f 2070  rough the info p
+00001670: 6172 616d 203a 0a0a 2020 2020 2020 2020  aram :..        
+00001680: 436f 6c75 6d6e 2849 6e74 6567 6572 2c20  Column(Integer, 
+00001690: 696e 666f 733d 7b27 6578 706f 7274 273a  infos={'export':
+000016a0: 0a20 2020 2020 2020 2020 2020 207b 2765  .            {'e
+000016b0: 7863 656c 273a 3c65 7863 656c 5f73 7065  xcel':<excel_spe
+000016c0: 6369 6669 635f 6f70 7469 6f6e 733e 2c0a  cific_options>,.
+000016d0: 2020 2020 2020 2020 2020 2020 203c 6d61               <ma
+000016e0: 696e 5f65 7870 6f72 745f 6f70 7469 6f6e  in_export_option
+000016f0: 733e 0a20 2020 2020 2020 2020 2020 207d  s>.            }
+00001700: 0a20 2020 2020 2020 207d 0a0a 2020 2020  .        }..    
+00001710: 6d61 696e 5f65 7870 6f72 745f 6f70 7469  main_export_opti
+00001720: 6f6e 7320 616e 6420 6578 6365 6c5f 7370  ons and excel_sp
+00001730: 6563 6966 6963 5f6f 7074 696f 6e73 2063  ecific_options c
+00001740: 616e 2062 6520 3a0a 0a20 2020 2020 2020  an be :..       
+00001750: 206c 6162 656c 0a0a 2020 2020 2020 2020   label..        
+00001760: 2020 2020 6c61 6265 6c20 6f66 2074 6865      label of the
+00001770: 2063 6f6c 756d 6e20 6865 6164 6572 0a0a   column header..
+00001780: 2020 2020 2020 2020 666f 726d 6174 0a0a          format..
+00001790: 2020 2020 2020 2020 2020 2020 6120 6675              a fu
+000017a0: 6e63 7469 6f6e 2074 6861 7420 7769 6c6c  nction that will
+000017b0: 2062 6520 6669 7265 6420 6f6e 2065 6163   be fired on eac
+000017c0: 6820 726f 7720 746f 2066 6f72 6d61 7420  h row to format 
+000017d0: 7468 6520 6f75 7470 7574 0a0a 2020 2020  the output..    
+000017e0: 2020 2020 7265 6c61 7465 645f 6b65 790a      related_key.
+000017f0: 0a20 2020 2020 2020 2020 2020 2049 6620  .            If 
+00001800: 7468 6520 6174 7472 6962 7574 6520 6973  the attribute is
+00001810: 2061 2072 656c 6174 696f 6e73 6869 702c   a relationship,
+00001820: 2074 6865 2076 616c 7565 206f 6620 7468   the value of th
+00001830: 6520 6769 7665 6e20 6174 7472 6962 7574  e given attribut
+00001840: 650a 2020 2020 2020 2020 2020 2020 6f66  e.            of
+00001850: 2074 6865 2072 656c 6174 6564 206f 626a   the related obj
+00001860: 6563 7420 7769 6c6c 2062 6520 7573 6564  ect will be used
+00001870: 2074 6f20 6669 6c6c 2074 6865 2063 656c   to fill the cel
+00001880: 6c73 0a0a 2020 2020 2020 2020 6578 636c  ls..        excl
+00001890: 7564 650a 0a20 2020 2020 2020 2020 2020  ude..           
+000018a0: 2054 6869 7320 6461 7461 2077 696c 6c20   This data will 
+000018b0: 6e6f 7420 6265 2069 6e73 6572 7465 6420  not be inserted 
+000018c0: 696e 2074 6865 2065 7870 6f72 7420 6966  in the export if
+000018d0: 2054 7275 650a 0a20 2020 2055 7361 6765   True..    Usage
+000018e0: 3a0a 0a20 2020 2020 2020 2061 203d 2053  :..        a = S
+000018f0: 716c 6158 6c73 4578 706f 7274 6572 284d  qlaXlsExporter(M
+00001900: 794d 6f64 656c 290a 2020 2020 2020 2020  yModel).        
+00001910: 666f 7220 6920 696e 204d 794d 6f64 656c  for i in MyModel
+00001920: 2e71 7565 7279 2829 2e66 696c 7465 7228  .query().filter(
+00001930: 3c6d 7966 696c 7465 723e 293a 0a20 2020  <myfilter>):.   
+00001940: 2020 2020 2020 2020 2061 2e61 6464 5f72           a.add_r
+00001950: 6f77 2869 290a 2020 2020 2020 2020 612e  ow(i).        a.
+00001960: 7265 6e64 6572 2829 0a20 2020 2072 2200  render().    r".
+00001970: 0000 544e 6304 0000 0000 0000 0000 0000  ..TNc...........
+00001980: 0005 0000 0005 0000 004b 0000 0073 4200  .........K...sB.
+00001990: 0000 7c02 7c00 5f00 7c03 6400 7500 7c00  ..|.|._.|.d.u.|.
+000019a0: 5f01 7402 6a03 7c00 6601 7c02 7c03 6401  _.t.j.|.f.|.|.d.
+000019b0: 9c02 7c04 a401 8e01 0100 7404 6a03 7c00  ..|.......t.j.|.
+000019c0: 6601 6402 7c01 6901 7c04 a401 8e01 0100  f.d.|.i.|.......
+000019d0: 6400 5300 2903 4e29 02da 0b67 7565 7373  d.S.).N)...guess
+000019e0: 5f74 7970 6573 7215 0000 00da 056d 6f64  _typesr......mod
+000019f0: 656c 2905 725e 0000 00da 0769 735f 726f  el).r^.....is_ro
+00001a00: 6f74 720f 0000 0072 1b00 0000 7206 0000  otr....r....r...
+00001a10: 0029 0572 1900 0000 725f 0000 0072 5e00  .).r....r_...r^.
+00001a20: 0000 7215 0000 0072 1a00 0000 720b 0000  ..r....r....r...
+00001a30: 0072 0b00 0000 720c 0000 0072 1b00 0000  .r....r....r....
+00001a40: 0601 0000 7308 0000 0000 0106 010a 0118  ....s...........
+00001a50: 017a 1853 716c 6158 6c73 4578 706f 7274  .z.SqlaXlsExport
+00001a60: 6572 2e5f 5f69 6e69 745f 5f63 0300 0000  er.__init__c....
+00001a70: 0000 0000 0000 0000 0500 0000 0500 0000  ................
+00001a80: 4300 0000 7342 0000 007c 02a0 0064 01a1  C...sB...|...d..
+00001a90: 017d 037c 0364 0275 0072 3e7c 006a 016a  .}.|.d.u.r>|.j.j
+00001aa0: 027c 02a0 0064 0364 04a1 0264 058d 017d  .|...d.d...d...}
+00001ab0: 0474 037c 016a 047c 0464 068d 0204 007d  .t.|.j.|.d.....}
+00001ac0: 037c 0264 013c 007c 0353 0029 077a 7f0a  .|.d.<.|.S.).z..
+00001ad0: 2020 2020 2020 2020 7265 7475 726e 7320          returns 
+00001ae0: 616e 2053 716c 6158 6c73 4578 706f 7274  an SqlaXlsExport
+00001af0: 6572 2066 6f72 2074 6865 2067 6976 656e  er for the given
+00001b00: 2072 656c 6174 6564 206f 626a 6563 7420   related object 
+00001b10: 616e 6420 7374 6f72 6573 2069 740a 2020  and stores it.  
+00001b20: 2020 2020 2020 696e 2074 6865 2063 6f6c        in the col
+00001b30: 756d 6e20 6f62 6a65 6374 2061 7320 6120  umn object as a 
+00001b40: 6361 6368 650a 2020 2020 2020 2020 da11  cache.        ..
+00001b50: 7371 6c61 5f78 6c73 5f65 7870 6f72 7465  sqla_xls_exporte
+00001b60: 724e 7246 0000 007a 0d64 6566 6175 6c74  rNrF...z.default
+00001b70: 2074 6974 6c65 2901 7216 0000 0029 0172   title).r....).r
+00001b80: 1500 0000 2905 7232 0000 0072 1300 0000  ....).r2...r....
+00001b90: 5a0c 6372 6561 7465 5f73 6865 6574 725d  Z.create_sheetr]
+00001ba0: 0000 00da 095f 5f63 6c61 7373 5f5f 2905  .....__class__).
+00001bb0: 7219 0000 00da 0b72 656c 6174 6564 5f6f  r......related_o
+00001bc0: 626a 7236 0000 00da 0672 6573 756c 7472  bjr6.....resultr
+00001bd0: 1500 0000 720b 0000 0072 0b00 0000 720c  ....r....r....r.
+00001be0: 0000 00da 155f 6765 745f 7265 6c61 7465  ....._get_relate
+00001bf0: 645f 6578 706f 7274 6572 0c01 0000 7312  d_exporter....s.
+00001c00: 0000 0000 050a 0108 0106 010a ff06 0302  ................
+00001c10: 0106 ff0e 037a 2553 716c 6158 6c73 4578  .....z%SqlaXlsEx
+00001c20: 706f 7274 6572 2e5f 6765 745f 7265 6c61  porter._get_rela
+00001c30: 7465 645f 6578 706f 7274 6572 6303 0000  ted_exporterc...
+00001c40: 0000 0000 0000 0000 0009 0000 0005 0000  ................
+00001c50: 0043 0000 0073 7e00 0000 7400 a001 7c00  .C...s~...t...|.
+00001c60: 7c01 7c02 a103 7d03 7c03 6401 6b02 727a  |.|...}.|.d.k.rz
+00001c70: 7c02 a002 6402 6403 a102 7d04 7c02 6404  |...d.d...}.|.d.
+00001c80: 1900 6a03 727a 7c04 6403 7500 727a 7c00  ..j.rz|.d.u.rz|.
+00001c90: 6a04 727a 7c02 6405 1900 7d05 7405 7c01  j.rz|.d...}.t.|.
+00001ca0: 7c05 6403 8303 7d06 7c06 7356 6401 5300  |.d...}.|.sVd.S.
+00001cb0: 7c00 a006 7c06 6406 1900 7c02 a102 7d07  |...|.d...|...}.
+00001cc0: 7c06 4400 5d0e 7d08 7c07 a007 7c08 a101  |.D.].}.|...|...
+00001cd0: 0100 716a 7c03 5300 2907 7a86 0a20 2020  ..qj|.S.).z..   
+00001ce0: 2020 2020 2052 6574 7572 6e20 7468 6520       Return the 
+00001cf0: 7661 6c75 6520 746f 2069 6e73 6572 7420  value to insert 
+00001d00: 696e 2061 2072 656c 6174 696f 6e73 6869  in a relationshi
+00001d10: 7020 6365 6c6c 0a20 2020 2020 2020 2048  p cell.        H
+00001d20: 616e 646c 6520 7468 6520 6361 7365 206f  andle the case o
+00001d30: 6620 636f 6d70 6c65 7820 7265 6c61 7465  f complex relate
+00001d40: 6420 6461 7461 7320 7765 2077 616e 7420  d datas we want 
+00001d50: 746f 2068 616e 646c 650a 2020 2020 2020  to handle.      
+00001d60: 2020 7208 0000 00da 0b72 656c 6174 6564    r......related
+00001d70: 5f6b 6579 4e72 5300 0000 724b 0000 0072  _keyNrS...rK...r
+00001d80: 0100 0000 2908 7206 0000 00da 1a5f 6765  ....).r......_ge
+00001d90: 745f 7265 6c61 7469 6f6e 7368 6970 5f63  t_relationship_c
+00001da0: 656c 6c5f 7661 6c72 3200 0000 da07 7573  ell_valr2.....us
+00001db0: 656c 6973 7472 6000 0000 722e 0000 0072  elistr`...r....r
+00001dc0: 6500 0000 da07 6164 645f 726f 7729 0972  e.....add_row).r
+00001dd0: 1900 0000 da03 6f62 6a72 3600 0000 da03  ......objr6.....
+00001de0: 7661 6c72 6600 0000 724b 0000 00da 0f72  valrf...rK.....r
+00001df0: 656c 6174 6564 5f6f 626a 6563 7473 da08  elated_objects..
+00001e00: 6578 706f 7274 6572 da07 7265 6c5f 6f62  exporter..rel_ob
+00001e10: 6a72 0b00 0000 720b 0000 0072 0c00 0000  jr....r....r....
+00001e20: 7267 0000 001b 0100 0073 1e00 0000 0005  rg.......s......
+00001e30: 0e01 0801 0c02 1803 0801 0c01 0401 0402  ................
+00001e40: 0401 0601 02fe 0404 0801 0c02 7a2a 5371  ............z*Sq
+00001e50: 6c61 586c 7345 7870 6f72 7465 722e 5f67  laXlsExporter._g
+00001e60: 6574 5f72 656c 6174 696f 6e73 6869 705f  et_relationship_
+00001e70: 6365 6c6c 5f76 616c 6301 0000 0000 0000  cell_valc.......
+00001e80: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
+00001e90: 0073 2e00 0000 7400 a001 7c00 a101 0100  .s....t...|.....
+00001ea0: 7c00 6a02 4400 5d18 7d01 6401 7c01 7600  |.j.D.].}.d.|.v.
+00001eb0: 7210 7c01 6401 1900 a001 a100 0100 7110  r.|.d.........q.
+00001ec0: 6402 5300 2903 7a52 0a20 2020 2020 2020  d.S.).zR.       
+00001ed0: 2045 6e68 616e 6365 2074 6865 2064 6566   Enhance the def
+00001ee0: 6175 6c74 2070 6f70 756c 6174 6520 7363  ault populate sc
+00001ef0: 7269 7074 2062 7920 6861 6e64 6c69 6e67  ript by handling
+00001f00: 2072 656c 6174 6564 2065 6c65 6d65 6e74   related element
+00001f10: 730a 2020 2020 2020 2020 7261 0000 004e  s.        ra...N
+00001f20: 2903 720f 0000 0072 3a00 0000 7230 0000  ).r....r:...r0..
+00001f30: 0029 0272 1900 0000 7244 0000 0072 0b00  .).r....rD...r..
+00001f40: 0000 720b 0000 0072 0c00 0000 723a 0000  ..r....r....r:..
+00001f50: 0035 0100 0073 0800 0000 0004 0a01 0a01  .5...s..........
+00001f60: 0801 7a19 5371 6c61 586c 7345 7870 6f72  ..z.SqlaXlsExpor
+00001f70: 7465 722e 5f70 6f70 756c 6174 6529 0254  ter._populate).T
+00001f80: 4e29 0972 4e00 0000 724f 0000 0072 5000  N).rN...rO...rP.
+00001f90: 0000 7251 0000 00da 0a63 6f6e 6669 675f  ..rQ.....config_
+00001fa0: 6b65 7972 1b00 0000 7265 0000 0072 6700  keyr....re...rg.
+00001fb0: 0000 723a 0000 0072 0b00 0000 720b 0000  ..r:...r....r...
+00001fc0: 0072 0b00 0000 720c 0000 0072 5d00 0000  .r....r....r]...
+00001fd0: dd00 0000 730c 0000 0008 0104 2604 020a  ....s.......&...
+00001fe0: 0608 0f08 1a72 5d00 0000 6300 0000 0000  .....r]...c.....
+00001ff0: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
+00002000: 0000 0073 1e00 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
+00002010: 6401 5a03 6402 5a04 6407 6404 6405 8401  d.Z.d.Z.d.d.d...
+00002020: 5a05 6406 5300 2908 da0b 586c 7345 7870  Z.d.S.)...XlsExp
+00002030: 6f72 7465 727a bc0a 2020 2020 4120 6d61  orterz..    A ma
+00002040: 696e 2078 6c73 2065 7870 6f72 7461 7469  in xls exportati
+00002050: 6f6e 2074 6f6f 6c20 2877 6974 686f 7574  on tool (without
+00002060: 2073 716c 616c 6368 656d 7920 7375 7070   sqlalchemy supp
+00002070: 6f72 7429 0a0a 2020 2020 7772 6974 6572  ort)..    writer
+00002080: 203d 204d 7958 6c73 4578 706f 7274 6572   = MyXlsExporter
+00002090: 2829 0a20 2020 2077 7269 7465 722e 6164  ().    writer.ad
+000020a0: 645f 726f 7728 7b27 6b65 7927 3a20 7527  d_row({'key': u'
+000020b0: 4c61 2076 616c 6575 7220 6465 206c 6120  La valeur de la 
+000020c0: 6365 6c6c 756c 6520 6465 206c 6120 636f  cellule de la co
+000020d0: 6c6f 6e6e 6520 3127 7d29 0a20 2020 2077  lonne 1'}).    w
+000020e0: 7269 7465 722e 7265 6e64 6572 2829 0a20  riter.render(). 
+000020f0: 2020 2072 0b00 0000 5463 0200 0000 0000     r....Tc......
+00002100: 0000 0000 0000 0300 0000 0400 0000 4b00  ..............K.
+00002110: 0000 732c 0000 0074 006a 017c 0066 0164  ..s,...t.j.|.f.d
+00002120: 017c 0169 017c 02a4 018e 0101 0074 026a  .|.i.|.......t.j
+00002130: 017c 0066 0169 007c 02a4 018e 0101 0064  .|.f.i.|.......d
+00002140: 0053 0029 024e 725e 0000 0029 0372 0f00  .S.).Nr^...).r..
+00002150: 0000 721b 0000 0072 0500 0000 2903 7219  ..r....r....).r.
+00002160: 0000 0072 5e00 0000 721a 0000 0072 0b00  ...r^...r....r..
+00002170: 0000 720b 0000 0072 0c00 0000 721b 0000  ..r....r....r...
+00002180: 004a 0100 0073 0400 0000 0001 1601 7a14  .J...s........z.
+00002190: 586c 7345 7870 6f72 7465 722e 5f5f 696e  XlsExporter.__in
+000021a0: 6974 5f5f 4e29 0154 2906 724e 0000 0072  it__N).T).rN...r
+000021b0: 4f00 0000 7250 0000 0072 5100 0000 7230  O...rP...rQ...r0
+000021c0: 0000 0072 1b00 0000 720b 0000 0072 0b00  ...r....r....r..
+000021d0: 0000 720b 0000 0072 0c00 0000 7270 0000  ..r....r....rp..
+000021e0: 003f 0100 0073 0600 0000 0801 0408 0402  .?...s..........
+000021f0: 7270 0000 0029 014e 291b 7251 0000 00da  rp...).N).rQ....
+00002200: 0969 7465 7274 6f6f 6c73 da07 6c6f 6767  .itertools..logg
+00002210: 696e 6772 1200 0000 5a0f 6f70 656e 7079  ingr....Z.openpy
+00002220: 786c 2e73 7479 6c65 7372 0200 0000 7203  xl.stylesr....r.
+00002230: 0000 0072 1d00 0000 da06 7374 7269 6e67  ...r......string
+00002240: 7204 0000 00da 1373 716c 615f 696e 7370  r......sqla_insp
+00002250: 6563 742e 6578 706f 7274 7205 0000 0072  ect.exportr....r
+00002260: 0600 0000 da11 7371 6c61 5f69 6e73 7065  ......sqla_inspe
+00002270: 6374 2e62 6173 6572 0700 0000 da09 6765  ct.baser......ge
+00002280: 744c 6f67 6765 7272 4e00 0000 da03 6c6f  tLoggerrN.....lo
+00002290: 67da 046c 6973 74da 1d63 6f6d 6269 6e61  g..list..combina
+000022a0: 7469 6f6e 735f 7769 7468 5f72 6570 6c61  tions_with_repla
+000022b0: 6365 6d65 6e74 5a0f 4153 4349 495f 5550  cementZ.ASCII_UP
+000022c0: 5045 5243 4153 4572 5700 0000 da06 6f62  PERCASErW.....ob
+000022d0: 6a65 6374 720f 0000 0072 4100 0000 725d  jectr....rA...r]
+000022e0: 0000 0072 7000 0000 720b 0000 0072 0b00  ...rp...r....r..
+000022f0: 0000 720b 0000 0072 0c00 0000 da08 3c6d  ..r....r......<m
+00002300: 6f64 756c 653e 0600 0000 7324 0000 0004  odule>....s$....
+00002310: 0408 0108 0108 0110 0508 010c 0210 040c  ................
+00002320: 030a 040e 020a fe0a 0606 0310 7f00 230a  ..............#.
+00002330: 1212 62                                  ..b
```

### Comparing `sqla_inspect-0.7.4/sqla_inspect/__pycache__/excel.cpython-39.pyc` & `sqla_inspect-0.7.5/sqla_inspect/__pycache__/excel.cpython-39-pytest-6.2.5.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Oct 14 14:46:05 2022 UTC, .py size: 9452 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,561 +1,570 @@
-00000000: 610d 0d0a 0000 0000 2d76 4963 ec24 0000  a.......-vIc.$..
+00000000: 610d 0d0a 0000 0000 27a0 7964 7b25 0000  a.......'.yd{%..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0007 0000 0040 0000 0073 d000 0000 6400  .....@...s....d.
-00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
-00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
-00000050: 6d05 5a05 6d06 5a06 0100 6401 6402 6c07  m.Z.m.Z...d.d.l.
-00000060: 5a07 6401 6404 6c08 6d09 5a09 0100 6401  Z.d.d.l.m.Z...d.
-00000070: 6405 6c0a 6d0b 5a0b 6d0c 5a0c 0100 6401  d.l.m.Z.m.Z...d.
-00000080: 6406 6c0d 6d0e 5a0e 0100 6502 a00f 6510  d.l.m.Z...e...e.
-00000090: a101 5a11 6512 6509 8301 6512 6407 6408  ..Z.e.e...e.d.d.
-000000a0: 8400 6501 a013 6509 6409 a102 4400 8301  ..e...e.d...D...
-000000b0: 8301 1700 5a14 650e 8300 5a15 4700 640a  ....Z.e...Z.G.d.
-000000c0: 640b 8400 640b 6516 8303 5a17 6412 640c  d...d.e...Z.d.d.
-000000d0: 640d 8401 5a18 4700 640e 640f 8400 640f  d...Z.G.d.d...d.
-000000e0: 6517 650c 8304 5a19 4700 6410 6411 8400  e.e...Z.G.d.d...
-000000f0: 6411 6517 650b 8304 5a1a 6402 5300 2913  d.e.e...Z.d.S.).
-00000100: 7a1a 0a45 7863 656c 2065 7870 6f72 7461  z..Excel exporta
-00000110: 7469 6f6e 206d 6f64 756c 650a e900 0000  tion module.....
-00000120: 004e 2902 da05 436f 6c6f 72da 0446 6f6e  .N)...Color..Fon
-00000130: 7429 01da 0f61 7363 6969 5f75 7070 6572  t)...ascii_upper
-00000140: 6361 7365 2902 da0c 4261 7365 4578 706f  case)...BaseExpo
-00000150: 7274 6572 da0c 5371 6c61 4578 706f 7274  rter..SqlaExport
-00000160: 6572 2901 da08 5265 6769 7374 7279 6301  er)...Registryc.
-00000170: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00000180: 0000 0063 0000 0073 1800 0000 7c00 5d10  ...c...s....|.].
-00000190: 7d01 6400 a000 7c01 a101 5600 0100 7102  }.d...|...V...q.
-000001a0: 6401 5300 2902 da00 4e29 01da 046a 6f69  d.S.)...N)...joi
-000001b0: 6e29 02da 022e 305a 0564 7570 6c65 a900  n)....0Z.duple..
-000001c0: 720b 0000 00fa 312f 686f 6d65 2f67 6173  r.....1/home/gas
-000001d0: 2f65 6e64 692f 7371 6c61 5f69 6e73 7065  /endi/sqla_inspe
-000001e0: 6374 2f73 716c 615f 696e 7370 6563 742f  ct/sqla_inspect/
-000001f0: 6578 6365 6c2e 7079 da09 3c67 656e 6578  excel.py..<genex
-00000200: 7072 3e20 0000 0073 0400 0000 0402 02ff  pr> ...s........
-00000210: 720d 0000 00e9 0200 0000 6300 0000 0000  r.........c.....
-00000220: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
-00000230: 0000 0073 7a00 0000 6500 5a01 6400 5a02  ...sz...e.Z.d.Z.
-00000240: 6401 5a03 6402 5a04 641b 6404 6405 8401  d.Z.d.Z.d.d.d...
-00000250: 5a05 641c 6406 6407 8401 5a06 6408 6409  Z.d.d.d...Z.d.d.
-00000260: 8400 5a07 6508 6508 640a 9c02 640b 640c  ..Z.e.e.d...d.d.
-00000270: 8404 5a09 640d 640e 8400 5a0a 640f 6410  ..Z.d.d...Z.d.d.
-00000280: 8400 5a0b 641d 6411 6412 8401 5a0c 6413  ..Z.d.d.d...Z.d.
-00000290: 6414 8400 5a0d 6415 6416 8400 5a0e 6417  d...Z.d.d...Z.d.
-000002a0: 6418 8400 5a0f 6419 641a 8400 5a10 6403  d...Z.d.d...Z.d.
-000002b0: 5300 291e da09 586c 7357 7269 7465 7261  S.)...XlsWritera
-000002c0: 9401 0000 0a20 2020 2043 6c61 7373 2070  .....    Class p
-000002d0: 726f 7669 6469 6e67 2063 6f6d 6d6f 6e20  roviding common 
-000002e0: 746f 6f6c 7320 746f 2077 7269 7465 2065  tools to write e
-000002f0: 7863 656c 2066 696c 6573 2066 726f 6d20  xcel files from 
-00000300: 7461 6275 6c61 7220 6461 7461 730a 0a20  tabular datas.. 
-00000310: 2020 2048 6173 2074 6f20 6265 2073 7562     Has to be sub
-00000320: 636c 6173 7365 642c 2074 6865 2073 7562  classed, the sub
-00000330: 636c 6173 7320 7368 6f75 6c64 2070 726f  class should pro
-00000340: 7669 6465 2061 205f 6461 7461 7320 616e  vide a _datas an
-00000350: 6420 6120 6865 6164 6572 730a 2020 2020  d a headers.    
-00000360: 6174 7472 6962 7574 6520 7468 6174 2063  attribute that c
-00000370: 6f6e 7461 696e 7320 7468 6520 6461 7461  ontains the data
-00000380: 7320 746f 2072 656e 6465 7220 616e 6420  s to render and 
-00000390: 7468 6520 6865 6164 6572 730a 0a20 2020  the headers..   
-000003a0: 2020 2020 205f 6461 7461 730a 0a20 2020       _datas..   
-000003b0: 2020 2020 2020 2020 206c 6973 7420 6f66           list of
-000003c0: 2074 7570 6c65 7320 2865 6163 6820 7475   tuples (each tu
-000003d0: 706c 6520 6973 2061 2072 6f77 290a 0a20  ple is a row).. 
-000003e0: 2020 2020 2020 2068 6561 6465 7273 0a0a         headers..
-000003f0: 2020 2020 2020 2020 2020 2020 6c69 7374              list
-00000400: 206f 6620 6469 6374 2063 6f6e 7461 696e   of dict contain
-00000410: 696e 6720 7468 6520 6c61 6265 6c20 6f66  ing the label of
-00000420: 2065 6163 6820 636f 6c75 6d6e 3a0a 2020   each column:.  
-00000430: 2020 2020 2020 2020 2020 2020 2020 7b27                {'
-00000440: 6c61 6265 6c27 3a20 3c61 206c 6162 656c  label': <a label
-00000450: 3e7d 0a0a 2020 2020 da06 4578 706f 7274  >}..    ..Export
-00000460: 4e63 0200 0000 0000 0000 0000 0000 0300  Nc..............
-00000470: 0000 0200 0000 4b00 0000 7342 0000 007c  ......K...sB...|
-00000480: 0164 0075 0072 2a74 006a 01a0 02a1 007c  .d.u.r*t.j.....|
-00000490: 005f 037c 006a 036a 047c 005f 057c 006a  ._.|.j.j.|._.|.j
-000004a0: 067c 006a 055f 066e 0e7c 017c 005f 057c  .|.j._.n.|.|._.|
-000004b0: 016a 077c 005f 037c 027c 005f 0864 0053  .j.|._.|.|._.d.S
-000004c0: 00a9 014e 2909 da08 6f70 656e 7079 786c  ...N)...openpyxl
-000004d0: 5a08 776f 726b 626f 6f6b 5a08 576f 726b  Z.workbookZ.Work
-000004e0: 626f 6f6b da04 626f 6f6b da06 6163 7469  book..book..acti
-000004f0: 7665 da09 776f 726b 7368 6565 74da 0574  ve..worksheet..t
-00000500: 6974 6c65 da06 7061 7265 6e74 da07 6f70  itle..parent..op
-00000510: 7469 6f6e 7329 03da 0473 656c 6672 1500  tions)...selfr..
-00000520: 0000 da02 6b77 720b 0000 0072 0b00 0000  ....kwr....r....
-00000530: 720c 0000 00da 085f 5f69 6e69 745f 5f3d  r......__init__=
-00000540: 0000 0073 0e00 0000 0001 0801 0c01 0a01  ...s............
-00000550: 0c02 0601 0801 7a12 586c 7357 7269 7465  ......z.XlsWrite
-00000560: 722e 5f5f 696e 6974 5f5f 6302 0000 0000  r.__init__c.....
-00000570: 0000 0000 0000 0002 0000 0005 0000 0043  ...............C
-00000580: 0000 0073 3400 0000 7c01 6401 7500 7210  ...s4...|.d.u.r.
-00000590: 7400 a001 a100 7d01 7c01 a002 7403 6a04  t.....}.|...t.j.
-000005a0: 6a05 a006 7c00 6a07 a101 a101 0100 7c01  j...|.j.......|.
-000005b0: a008 6402 a101 0100 7c01 5300 2903 7a9a  ..d.....|.S.).z.
-000005c0: 0a20 2020 2020 2020 2052 6574 7572 6e20  .        Return 
-000005d0: 6120 6669 6c65 2062 7566 6665 7220 636f  a file buffer co
-000005e0: 6e74 6169 6e69 6e67 2074 6865 2072 6573  ntaining the res
-000005f0: 756c 7469 6e67 2078 6c73 0a0a 2020 2020  ulting xls..    
-00000600: 2020 2020 3a70 6172 616d 206f 626a 2066      :param obj f
-00000610: 5f62 7566 3a20 4120 6669 6c65 2062 7566  _buf: A file buf
-00000620: 6665 7220 7375 7070 6f72 7469 6e67 2074  fer supporting t
-00000630: 6865 2077 7269 7465 2061 6e64 2073 6565  he write and see
-00000640: 6b0a 2020 2020 2020 2020 6d65 7468 6f64  k.        method
-00000650: 730a 2020 2020 2020 2020 4e72 0100 0000  s.        Nr....
-00000660: 2909 da02 696f da07 4279 7465 7349 4fda  )...io..BytesIO.
-00000670: 0577 7269 7465 7212 0000 00da 0677 7269  .writer......wri
-00000680: 7465 72da 0565 7863 656c 5a15 7361 7665  ter..excelZ.save
-00000690: 5f76 6972 7475 616c 5f77 6f72 6b62 6f6f  _virtual_workboo
-000006a0: 6b72 1300 0000 da04 7365 656b a902 7219  kr......seek..r.
-000006b0: 0000 00da 0566 5f62 7566 720b 0000 0072  .....f_bufr....r
-000006c0: 0b00 0000 720c 0000 00da 0973 6176 655f  ....r......save_
-000006d0: 626f 6f6b 4700 0000 730a 0000 0000 0708  bookG...s.......
-000006e0: 0108 0116 010a 017a 1358 6c73 5772 6974  .......z.XlsWrit
-000006f0: 6572 2e73 6176 655f 626f 6f6b 6303 0000  er.save_bookc...
-00000700: 0000 0000 0000 0000 0003 0000 0004 0000  ................
-00000710: 0043 0000 0073 1600 0000 7400 7401 7c02  .C...s....t.t.|.
-00000720: 6401 8d01 6402 8d01 7c01 5f02 6403 5300  d...d...|._.d.S.
-00000730: 2904 7aa8 0a20 2020 2020 2020 2053 6574  ).z..        Set
-00000740: 2074 6865 2067 6976 656e 2063 6f6c 6f72   the given color
-00000750: 2074 6f20 7468 6520 7072 6f76 6964 6564   to the provided
-00000760: 2063 656c 6c0a 0a20 2020 2020 2020 2020   cell..         
-00000770: 2020 2063 656c 6c0a 0a20 2020 2020 2020     cell..       
-00000780: 2020 2020 2020 2020 2041 2078 6c73 2063           A xls c
-00000790: 656c 6c20 6f62 6a65 6374 0a0a 2020 2020  ell object..    
-000007a0: 2020 2020 2020 2020 636f 6c6f 720a 0a20          color.. 
-000007b0: 2020 2020 2020 2020 2020 2020 2020 2041                 A
-000007c0: 206f 7065 6e70 7978 6c20 636f 6c6f 7220   openpyxl color 
-000007d0: 7661 720a 2020 2020 2020 2020 2901 da03  var.        )...
-000007e0: 7267 6229 01da 0563 6f6c 6f72 4e29 0372  rgb)...colorN).r
-000007f0: 0300 0000 7202 0000 00da 0466 6f6e 7429  ....r......font)
-00000800: 0372 1900 0000 da04 6365 6c6c 7226 0000  .r......cellr&..
-00000810: 0072 0b00 0000 720b 0000 0072 0c00 0000  .r....r....r....
-00000820: da09 7365 745f 636f 6c6f 7254 0000 0073  ..set_colorT...s
-00000830: 0200 0000 000c 7a13 586c 7357 7269 7465  ......z.XlsWrite
-00000840: 722e 7365 745f 636f 6c6f 7229 02da 0b63  r.set_color)...c
-00000850: 6f6c 756d 6e5f 6e61 6d65 da05 7661 6c75  olumn_name..valu
-00000860: 6563 0300 0000 0000 0000 0000 0000 0300  ec..............
-00000870: 0000 0400 0000 4300 0000 7324 0000 0074  ......C...s$...t
-00000880: 007c 0064 017c 0116 0083 0272 2074 017c  .|.d.|.....r t.|
-00000890: 0064 017c 0116 0083 027c 0283 017d 027c  .d.|.....|...}.|
-000008a0: 0253 0029 027a 1f0a 2020 2020 2020 2020  .S.).z..        
-000008b0: 466f 726d 6174 2061 2063 656c 6c0a 2020  Format a cell.  
-000008c0: 2020 2020 2020 7a09 666f 726d 6174 5f25        z.format_%
-000008d0: 7329 02da 0768 6173 6174 7472 da07 6765  s)...hasattr..ge
-000008e0: 7461 7474 7229 0372 1900 0000 722a 0000  tattr).r....r*..
-000008f0: 0072 2b00 0000 720b 0000 0072 0b00 0000  .r+...r....r....
-00000900: 720c 0000 00da 0b66 6f72 6d61 745f 6365  r......format_ce
-00000910: 6c6c 6200 0000 7306 0000 0000 040e 0112  llb...s.........
-00000920: 017a 1558 6c73 5772 6974 6572 2e66 6f72  .z.XlsWriter.for
-00000930: 6d61 745f 6365 6c6c 6302 0000 0000 0000  mat_cellc.......
-00000940: 0000 0000 0007 0000 0005 0000 0043 0000  .............C..
-00000950: 0073 4600 0000 6700 7d02 7400 7c00 6401  .sF...g.}.t.|.d.
-00000960: 6700 8303 7d03 7c03 4400 5d2c 7d04 7c04  g...}.|.D.],}.|.
-00000970: 6402 1900 7d05 7c01 a001 7c05 6403 a102  d...}.|...|.d...
-00000980: 7d06 7c00 a002 7c06 a101 7d06 7c02 a003  }.|...|...}.|...
-00000990: 7c06 a101 0100 7114 7c02 5300 2904 7a96  |.....q.|.S.).z.
-000009a0: 0a20 2020 2020 2020 2054 6865 2072 656e  .        The ren
-000009b0: 6465 7220 6d65 7468 6f64 2065 7870 6563  der method expec
-000009c0: 7473 2072 6f77 7320 6173 206c 6973 7473  ts rows as lists
-000009d0: 2c20 6865 7265 2077 6520 7377 6974 6368  , here we switch
-000009e0: 206f 7572 2072 6f77 2066 6f72 6d61 740a   our row format.
-000009f0: 2020 2020 2020 2020 6672 6f6d 2064 6963          from dic
-00000a00: 7420 746f 206c 6973 7420 7265 7370 6563  t to list respec
-00000a10: 7469 6e67 2074 6865 206f 7264 6572 206f  ting the order o
-00000a20: 6620 7468 6520 6865 6164 6572 730a 2020  f the headers.  
-00000a30: 2020 2020 2020 da07 6865 6164 6572 73da        ..headers.
-00000a40: 046e 616d 6572 0800 0000 2904 722d 0000  .namer....).r-..
-00000a50: 00da 0367 6574 722e 0000 00da 0661 7070  ...getr......app
-00000a60: 656e 6429 0772 1900 0000 da03 726f 77da  end).r......row.
-00000a70: 0372 6573 722f 0000 00da 0663 6f6c 756d  .resr/.....colum
-00000a80: 6e72 2a00 0000 722b 0000 0072 0b00 0000  nr*...r+...r....
-00000a90: 720b 0000 0072 0c00 0000 da0a 666f 726d  r....r......form
-00000aa0: 6174 5f72 6f77 6a00 0000 7310 0000 0000  at_rowj...s.....
-00000ab0: 0504 010c 0108 0108 010c 010a 010c 017a  ...............z
-00000ac0: 1458 6c73 5772 6974 6572 2e66 6f72 6d61  .XlsWriter.forma
-00000ad0: 745f 726f 7763 0100 0000 0000 0000 0000  t_rowc..........
-00000ae0: 0000 0100 0000 0200 0000 4300 0000 7314  ..........C...s.
-00000af0: 0000 007c 00a0 00a1 0001 007c 00a0 01a1  ...|.......|....
-00000b00: 0001 0064 0153 0029 027a 430a 2020 2020  ...d.S.).zC.    
-00000b10: 2020 2020 506f 7075 6c61 7465 2068 6561      Populate hea
-00000b20: 6465 7273 2061 6e64 2072 6f77 7320 6265  ders and rows be
-00000b30: 666f 7265 2077 7269 7469 6e67 206f 7572  fore writing our
-00000b40: 2062 6f6f 6b0a 2020 2020 2020 2020 4e29   book.        N)
-00000b50: 02da 0f5f 7265 6e64 6572 5f68 6561 6465  ..._render_heade
-00000b60: 7273 da0c 5f72 656e 6465 725f 726f 7773  rs.._render_rows
-00000b70: 2901 7219 0000 0072 0b00 0000 720b 0000  ).r....r....r...
-00000b80: 0072 0c00 0000 da09 5f70 6f70 756c 6174  .r......_populat
-00000b90: 6578 0000 0073 0400 0000 0004 0801 7a13  ex...s........z.
-00000ba0: 586c 7357 7269 7465 722e 5f70 6f70 756c  XlsWriter._popul
-00000bb0: 6174 6563 0200 0000 0000 0000 0000 0000  atec............
-00000bc0: 0200 0000 0300 0000 4300 0000 7312 0000  ........C...s...
-00000bd0: 007c 00a0 00a1 0001 007c 00a0 017c 01a1  .|.......|...|..
-00000be0: 0153 0029 017a 870a 2020 2020 2020 2020  .S.).z..        
-00000bf0: 4465 6669 6e69 7465 6c79 2072 656e 6465  Definitely rende
-00000c00: 7220 7468 6520 776f 726b 626f 6f6b 0a0a  r the workbook..
-00000c10: 2020 2020 2020 2020 3a70 6172 616d 206f          :param o
-00000c20: 626a 2066 5f62 7566 3a20 4120 6669 6c65  bj f_buf: A file
-00000c30: 2062 7566 6665 7220 7375 7070 6f72 7469   buffer supporti
-00000c40: 6e67 2074 6865 2077 7269 7465 2061 6e64  ng the write and
-00000c50: 2073 6565 6b0a 2020 2020 2020 2020 6d65   seek.        me
-00000c60: 7468 6f64 730a 2020 2020 2020 2020 2902  thods.        ).
-00000c70: 7239 0000 0072 2400 0000 7222 0000 0072  r9...r$...r"...r
-00000c80: 0b00 0000 720b 0000 0072 0c00 0000 da06  ....r....r......
-00000c90: 7265 6e64 6572 7f00 0000 7304 0000 0000  render....s.....
-00000ca0: 0708 027a 1058 6c73 5772 6974 6572 2e72  ...z.XlsWriter.r
-00000cb0: 656e 6465 7263 0100 0000 0000 0000 0000  enderc..........
-00000cc0: 0000 0b00 0000 0600 0000 4300 0000 739c  ..........C...s.
-00000cd0: 0000 0074 007c 0064 0164 0283 037d 0174  ...t.|.d.d...}.t
-00000ce0: 007c 0064 0364 0283 037d 0274 017c 0183  .|.d.d...}.t.|..
-00000cf0: 0144 005d 765c 027d 037d 047c 0364 0417  .D.]v\.}.}.|.d..
-00000d00: 007d 0574 017c 0483 0144 005d 5c5c 027d  .}.t.|...D.]\\.}
-00000d10: 067d 077c 006a 026a 037c 057c 0664 0517  .}.|.j.j.|.|.d..
-00000d20: 0064 068d 027d 087c 0764 0775 0172 647c  .d...}.|.d.u.rd|
-00000d30: 077c 085f 046e 0664 087c 085f 0474 057c  .|._.n.d.|._.t.|
-00000d40: 0283 017c 066b 0472 387c 027c 0619 007d  ...|.k.r8|.|...}
-00000d50: 0974 067c 0983 017d 0a7c 0a64 0775 0172  .t.|...}.|.d.u.r
-00000d60: 387c 0a7c 085f 0771 3871 2064 0753 0029  8|.|._.q8q d.S.)
-00000d70: 097a 3b0a 2020 2020 2020 2020 5265 6e64  .z;.        Rend
-00000d80: 6572 2074 6865 2072 6f77 7320 696e 2074  er the rows in t
-00000d90: 6865 2063 7572 7265 6e74 2073 7479 6c65  he current style
-00000da0: 7368 6565 740a 2020 2020 2020 2020 da06  sheet.        ..
-00000db0: 5f64 6174 6173 720b 0000 0072 2f00 0000  _datasr....r/...
-00000dc0: 720e 0000 00e9 0100 0000 a902 7233 0000  r...........r3..
-00000dd0: 0072 3500 0000 4e72 0800 0000 2908 722d  .r5...Nr....).r-
-00000de0: 0000 00da 0965 6e75 6d65 7261 7465 7215  .....enumerater.
-00000df0: 0000 0072 2800 0000 722b 0000 00da 036c  ...r(...r+.....l
-00000e00: 656e da0f 6765 745f 6365 6c6c 5f66 6f72  en..get_cell_for
-00000e10: 6d61 745a 0d6e 756d 6265 725f 666f 726d  matZ.number_form
-00000e20: 6174 290b 7219 0000 0072 3b00 0000 722f  at).r....r;...r/
-00000e30: 0000 00da 0569 6e64 6578 7233 0000 00da  .....indexr3....
-00000e40: 0a72 6f77 5f6e 756d 6265 725a 0763 6f6c  .row_numberZ.col
-00000e50: 5f6e 756d 722b 0000 0072 2800 0000 da06  _numr+...r(.....
-00000e60: 6865 6164 6572 da06 666f 726d 6174 720b  header..formatr.
-00000e70: 0000 0072 0b00 0000 720c 0000 0072 3800  ...r....r....r8.
-00000e80: 0000 8a00 0000 731c 0000 0000 040c 010c  ......s.........
-00000e90: 0110 0108 0110 0114 0108 0108 0206 010c  ................
-00000ea0: 0108 0108 0108 017a 1658 6c73 5772 6974  .......z.XlsWrit
-00000eb0: 6572 2e5f 7265 6e64 6572 5f72 6f77 7363  er._render_rowsc
-00000ec0: 0100 0000 0000 0000 0000 0000 0700 0000  ................
-00000ed0: 0500 0000 4300 0000 7388 0000 0074 007c  ....C...s....t.|
-00000ee0: 0064 0164 0283 037d 0174 017c 0183 0144  .d.d...}.t.|...D
-00000ef0: 005d 265c 027d 027d 037c 006a 026a 0364  .]&\.}.}.|.j.j.d
-00000f00: 037c 0264 0317 0064 048d 027d 047c 0364  .|.d...d...}.|.d
-00000f10: 0519 007c 045f 0471 147c 0264 0337 007d  ...|._.q.|.d.7.}
-00000f20: 0274 007c 0064 0664 0283 037d 0574 017c  .t.|.d.d...}.t.|
-00000f30: 0583 0144 005d 2a5c 027d 067d 037c 006a  ...D.]*\.}.}.|.j
-00000f40: 026a 0364 037c 067c 0217 0064 0317 0064  .j.d.|.|...d...d
-00000f50: 048d 027d 047c 0364 0519 007c 045f 0471  ...}.|.d...|._.q
-00000f60: 5864 0753 0029 087a 270a 2020 2020 2020  Xd.S.).z'.      
-00000f70: 2020 5772 6974 6520 7468 6520 6865 6164    Write the head
-00000f80: 6572 7320 726f 770a 2020 2020 2020 2020  ers row.        
-00000f90: 722f 0000 0072 0b00 0000 723c 0000 0072  r/...r....r<...r
-00000fa0: 3d00 0000 da05 6c61 6265 6cda 0d65 7874  =.....label..ext
-00000fb0: 7261 5f68 6561 6465 7273 4e29 0572 2d00  ra_headersN).r-.
-00000fc0: 0000 723e 0000 0072 1500 0000 7228 0000  ..r>...r....r(..
-00000fd0: 0072 2b00 0000 2907 7219 0000 0072 2f00  .r+...).r....r/.
-00000fe0: 0000 7241 0000 00da 0363 6f6c 7228 0000  ..rA.....colr(..
-00000ff0: 0072 4600 0000 5a09 6164 645f 696e 6465  .rF...Z.add_inde
-00001000: 7872 0b00 0000 720b 0000 0072 0c00 0000  xr....r....r....
-00001010: 7237 0000 009e 0000 0073 1200 0000 0004  r7.......s......
-00001020: 0c01 1002 1401 0c02 0802 0c01 1001 1801  ................
-00001030: 7a19 586c 7357 7269 7465 722e 5f72 656e  z.XlsWriter._ren
-00001040: 6465 725f 6865 6164 6572 7363 0200 0000  der_headersc....
-00001050: 0000 0000 0000 0000 0200 0000 0200 0000  ................
-00001060: 4300 0000 730c 0000 007c 017c 006a 005f  C...s....|.|.j._
-00001070: 0164 0053 0072 1100 0000 2902 7215 0000  .d.S.r....).r...
-00001080: 0072 1600 0000 2902 7219 0000 0072 1600  .r....).r....r..
-00001090: 0000 720b 0000 0072 0b00 0000 720c 0000  ..r....r....r...
-000010a0: 00da 0973 6574 5f74 6974 6c65 af00 0000  ...set_title....
-000010b0: 7302 0000 0000 017a 1358 6c73 5772 6974  s......z.XlsWrit
-000010c0: 6572 2e73 6574 5f74 6974 6c65 6302 0000  er.set_titlec...
-000010d0: 0000 0000 0000 0000 0004 0000 0007 0000  ................
-000010e0: 0043 0000 0073 5a00 0000 6700 7c00 5f00  .C...sZ...g.|._.
-000010f0: 6401 7c00 6a01 7600 7250 7c00 6a01 6401  d.|.j.v.rP|.j.d.
-00001100: 1900 4400 5d32 7d02 7c01 4400 5d28 7d03  ..D.]2}.|.D.](}.
-00001110: 7c03 a002 6402 7c03 6403 1900 a102 7c02  |...d.|.d.....|.
-00001120: 6b02 7222 7c00 6a00 a003 7c03 a101 0100  k.r"|.j...|.....
-00001130: 0100 711a 7122 711a 6e06 7c01 7c00 5f00  ..q.q"q.n.|.|._.
-00001140: 6404 5300 2905 7aeb 0a20 2020 2020 2020  d.S.).z..       
-00001150: 2053 6574 2074 6865 2068 6561 6465 7273   Set the headers
-00001160: 206f 6620 6f75 7220 7772 6974 6572 0a20   of our writer. 
-00001170: 2020 2020 2020 203a 7061 7261 6d20 6c69         :param li
-00001180: 7374 2068 6561 6465 7273 3a20 6c69 7374  st headers: list
-00001190: 206f 6620 6469 6374 2077 6974 6820 6174   of dict with at
-000011a0: 206c 6561 7374 2061 206c 6162 656c 206b   least a label k
-000011b0: 6579 0a20 2020 2020 2020 2028 6c61 6265  ey.        (labe
-000011c0: 6c20 6973 206d 616e 6461 746f 7279 203a  l is mandatory :
-000011d0: 2075 7365 6420 666f 7220 7468 6520 6578   used for the ex
-000011e0: 706f 7274 290a 0a20 2020 2020 2020 2048  port)..        H
-000011f0: 6561 6465 7273 2061 7265 2066 696c 7465  eaders are filte
-00001200: 7265 6420 616e 6420 6f72 6465 7265 6420  red and ordered 
-00001210: 7265 6761 7264 696e 6720 7468 6520 6f72  regarding the or
-00001220: 6465 7220 6f70 7469 6f6e 0a20 2020 2020  der option.     
-00001230: 2020 20da 056f 7264 6572 da03 6b65 7972     ..order..keyr
-00001240: 4500 0000 4e29 0472 2f00 0000 7218 0000  E...N).r/...r...
-00001250: 0072 3100 0000 7232 0000 0029 0472 1900  .r1...r2...).r..
-00001260: 0000 722f 0000 00da 0765 6c65 6d65 6e74  ..r/.....element
-00001270: 7243 0000 0072 0b00 0000 720b 0000 0072  rC...r....r....r
-00001280: 0c00 0000 da0b 7365 745f 6865 6164 6572  ......set_header
-00001290: 73b2 0000 0073 1000 0000 0008 0601 0a01  s....s..........
-000012a0: 0e01 0801 1401 0c01 0a02 7a15 586c 7357  ..........z.XlsW
-000012b0: 7269 7465 722e 7365 745f 6865 6164 6572  riter.set_header
-000012c0: 7329 014e 2901 4e29 014e 2911 da08 5f5f  s).N).N).N)...__
-000012d0: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-000012e0: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-000012f0: da07 5f5f 646f 635f 5f72 1600 0000 721b  ..__doc__r....r.
-00001300: 0000 0072 2400 0000 7229 0000 00da 0373  ...r$...r).....s
-00001310: 7472 722e 0000 0072 3600 0000 7239 0000  trr....r6...r9..
-00001320: 0072 3a00 0000 7238 0000 0072 3700 0000  .r:...r8...r7...
-00001330: 7248 0000 0072 4c00 0000 720b 0000 0072  rH...rL...r....r
-00001340: 0b00 0000 720b 0000 0072 0c00 0000 720f  ....r....r....r.
-00001350: 0000 0029 0000 0073 1a00 0000 0801 0411  ...)...s........
-00001360: 0402 0a0a 0a0d 080e 1008 080e 0807 0a0b  ................
-00001370: 0814 0811 0803 720f 0000 0063 0200 0000  ......r....c....
-00001380: 0000 0000 0000 0000 0600 0000 0400 0000  ................
-00001390: 4300 0000 7356 0000 007c 00a0 0064 01a1  C...sV...|...d..
-000013a0: 017d 027c 00a0 0064 02a1 017d 037c 0264  .}.|...d...}.|.d
-000013b0: 0375 0072 527c 0364 0375 0172 5274 017c  .u.rR|.d.u.rRt.|
-000013c0: 0364 0483 0272 527c 036a 0264 0519 007d  .d...rR|.j.d...}
-000013d0: 0474 037c 046a 0464 067c 046a 0483 037d  .t.|.j.d.|.j...}
-000013e0: 0574 05a0 067c 05a1 017d 027c 0253 0029  .t...|...}.|.S.)
-000013f0: 077a 9f0a 2020 2020 5265 7475 726e 2074  .z..    Return t
-00001400: 6865 2063 656c 6c20 666f 726d 6174 2066  he cell format f
-00001410: 6f72 2074 6865 2067 6976 656e 2063 6f6c  or the given col
-00001420: 756d 6e0a 0a20 2020 203a 7061 7261 6d20  umn..    :param 
-00001430: 636f 6c75 6d6e 5f64 6963 743a 2054 6865  column_dict: The
-00001440: 2063 6f6c 756d 6e20 6461 7461 7320 636f   column datas co
-00001450: 6c6c 6563 7465 6420 6475 7269 6e67 2069  llected during i
-00001460: 6e73 7065 6374 696f 6e0a 2020 2020 3a70  nspection.    :p
-00001470: 6172 616d 206b 6579 3a20 5468 6520 6578  aram key: The ex
-00001480: 706f 7274 6174 696f 6e20 6b65 790a 2020  portation key.  
-00001490: 2020 7244 0000 00da 075f 5f63 6f6c 5f5f    rD.....__col__
-000014a0: 4eda 0763 6f6c 756d 6e73 7201 0000 00da  N..columnsr.....
-000014b0: 0469 6d70 6c29 0772 3100 0000 722c 0000  .impl).r1...r,..
-000014c0: 0072 5300 0000 722d 0000 00da 0474 7970  .rS...r-.....typ
-000014d0: 65da 0f46 4f52 4d41 545f 5245 4749 5354  e..FORMAT_REGIST
-000014e0: 5259 da08 6765 745f 6974 656d 2906 da0b  RY..get_item)...
-000014f0: 636f 6c75 6d6e 5f64 6963 7472 4a00 0000  column_dictrJ...
-00001500: 7244 0000 00da 0470 726f 70da 0b73 716c  rD.....prop..sql
-00001510: 615f 636f 6c75 6d6e da0b 636f 6c75 6d6e  a_column..column
-00001520: 5f74 7970 6572 0b00 0000 720b 0000 0072  _typer....r....r
-00001530: 0c00 0000 7240 0000 00c5 0000 0073 1000  ....r@.......s..
-00001540: 0000 0007 0a01 0a02 1001 0a01 0a01 1001  ................
-00001550: 0a01 7240 0000 0063 0000 0000 0000 0000  ..r@...c........
-00001560: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
-00001570: 7336 0000 0065 005a 0164 005a 0264 015a  s6...e.Z.d.Z.d.Z
-00001580: 0364 025a 0464 0d64 0564 0684 015a 0564  .d.Z.d.d.d...Z.d
-00001590: 0764 0884 005a 0664 0964 0a84 005a 0764  .d...Z.d.d...Z.d
-000015a0: 0b64 0c84 005a 0864 0453 0029 0eda 0f53  .d...Z.d.S.)...S
-000015b0: 716c 6158 6c73 4578 706f 7274 6572 617a  qlaXlsExporteraz
-000015c0: 0300 000a 2020 2020 4d61 696e 2063 6c61  ....    Main cla
-000015d0: 7373 2075 7365 6420 666f 7220 6578 706f  ss used for expo
-000015e0: 7274 696e 6720 6461 7461 7320 746f 2074  rting datas to t
-000015f0: 6865 2078 6c73 2066 6f72 6d61 740a 0a20  he xls format.. 
-00001600: 2020 204d 6f64 656c 7320 6174 7472 6962     Models attrib
-00001610: 7574 6573 206f 7574 7075 7420 6361 6e20  utes output can 
-00001620: 6265 2063 7573 746f 6d69 7a65 6420 7468  be customized th
-00001630: 726f 7567 6820 7468 6520 696e 666f 2070  rough the info p
-00001640: 6172 616d 203a 0a0a 2020 2020 2020 2020  aram :..        
-00001650: 436f 6c75 6d6e 2849 6e74 6567 6572 2c20  Column(Integer, 
-00001660: 696e 666f 733d 7b27 6578 706f 7274 273a  infos={'export':
-00001670: 0a20 2020 2020 2020 2020 2020 207b 2765  .            {'e
-00001680: 7863 656c 273a 3c65 7863 656c 5f73 7065  xcel':<excel_spe
-00001690: 6369 6669 635f 6f70 7469 6f6e 733e 2c0a  cific_options>,.
-000016a0: 2020 2020 2020 2020 2020 2020 203c 6d61               <ma
-000016b0: 696e 5f65 7870 6f72 745f 6f70 7469 6f6e  in_export_option
-000016c0: 733e 0a20 2020 2020 2020 2020 2020 207d  s>.            }
-000016d0: 0a20 2020 2020 2020 207d 0a0a 2020 2020  .        }..    
-000016e0: 6d61 696e 5f65 7870 6f72 745f 6f70 7469  main_export_opti
-000016f0: 6f6e 7320 616e 6420 6578 6365 6c5f 7370  ons and excel_sp
-00001700: 6563 6966 6963 5f6f 7074 696f 6e73 2063  ecific_options c
-00001710: 616e 2062 6520 3a0a 0a20 2020 2020 2020  an be :..       
-00001720: 206c 6162 656c 0a0a 2020 2020 2020 2020   label..        
-00001730: 2020 2020 6c61 6265 6c20 6f66 2074 6865      label of the
-00001740: 2063 6f6c 756d 6e20 6865 6164 6572 0a0a   column header..
-00001750: 2020 2020 2020 2020 666f 726d 6174 0a0a          format..
-00001760: 2020 2020 2020 2020 2020 2020 6120 6675              a fu
-00001770: 6e63 7469 6f6e 2074 6861 7420 7769 6c6c  nction that will
-00001780: 2062 6520 6669 7265 6420 6f6e 2065 6163   be fired on eac
-00001790: 6820 726f 7720 746f 2066 6f72 6d61 7420  h row to format 
-000017a0: 7468 6520 6f75 7470 7574 0a0a 2020 2020  the output..    
-000017b0: 2020 2020 7265 6c61 7465 645f 6b65 790a      related_key.
-000017c0: 0a20 2020 2020 2020 2020 2020 2049 6620  .            If 
-000017d0: 7468 6520 6174 7472 6962 7574 6520 6973  the attribute is
-000017e0: 2061 2072 656c 6174 696f 6e73 6869 702c   a relationship,
-000017f0: 2074 6865 2076 616c 7565 206f 6620 7468   the value of th
-00001800: 6520 6769 7665 6e20 6174 7472 6962 7574  e given attribut
-00001810: 650a 2020 2020 2020 2020 2020 2020 6f66  e.            of
-00001820: 2074 6865 2072 656c 6174 6564 206f 626a   the related obj
-00001830: 6563 7420 7769 6c6c 2062 6520 7573 6564  ect will be used
-00001840: 2074 6f20 6669 6c6c 2074 6865 2063 656c   to fill the cel
-00001850: 6c73 0a0a 2020 2020 2020 2020 6578 636c  ls..        excl
-00001860: 7564 650a 0a20 2020 2020 2020 2020 2020  ude..           
-00001870: 2054 6869 7320 6461 7461 2077 696c 6c20   This data will 
-00001880: 6e6f 7420 6265 2069 6e73 6572 7465 6420  not be inserted 
-00001890: 696e 2074 6865 2065 7870 6f72 7420 6966  in the export if
-000018a0: 2054 7275 650a 0a20 2020 2055 7361 6765   True..    Usage
-000018b0: 3a0a 0a20 2020 2020 2020 2061 203d 2053  :..        a = S
-000018c0: 716c 6158 6c73 4578 706f 7274 6572 284d  qlaXlsExporter(M
-000018d0: 794d 6f64 656c 290a 2020 2020 2020 2020  yModel).        
-000018e0: 666f 7220 6920 696e 204d 794d 6f64 656c  for i in MyModel
-000018f0: 2e71 7565 7279 2829 2e66 696c 7465 7228  .query().filter(
-00001900: 3c6d 7966 696c 7465 723e 293a 0a20 2020  <myfilter>):.   
-00001910: 2020 2020 2020 2020 2061 2e61 6464 5f72           a.add_r
-00001920: 6f77 2869 290a 2020 2020 2020 2020 612e  ow(i).        a.
-00001930: 7265 6e64 6572 2829 0a20 2020 2072 2000  render().    r .
-00001940: 0000 544e 6304 0000 0000 0000 0000 0000  ..TNc...........
-00001950: 0005 0000 0005 0000 004b 0000 0073 4200  .........K...sB.
-00001960: 0000 7c02 7c00 5f00 7c03 6400 7500 7c00  ..|.|._.|.d.u.|.
-00001970: 5f01 7402 6a03 7c00 6601 7c02 7c03 6401  _.t.j.|.f.|.|.d.
-00001980: 9c02 7c04 a401 8e01 0100 7404 6a03 7c00  ..|.......t.j.|.
-00001990: 6601 6402 7c01 6901 7c04 a401 8e01 0100  f.d.|.i.|.......
-000019a0: 6400 5300 2903 4e29 02da 0b67 7565 7373  d.S.).N)...guess
-000019b0: 5f74 7970 6573 7215 0000 00da 056d 6f64  _typesr......mod
-000019c0: 656c 2905 725d 0000 00da 0769 735f 726f  el).r].....is_ro
-000019d0: 6f74 720f 0000 0072 1b00 0000 7206 0000  otr....r....r...
-000019e0: 0029 0572 1900 0000 725e 0000 0072 5d00  .).r....r^...r].
-000019f0: 0000 7215 0000 0072 1a00 0000 720b 0000  ..r....r....r...
-00001a00: 0072 0b00 0000 720c 0000 0072 1b00 0000  .r....r....r....
-00001a10: 0001 0000 7308 0000 0000 0106 010a 0118  ....s...........
-00001a20: 017a 1853 716c 6158 6c73 4578 706f 7274  .z.SqlaXlsExport
-00001a30: 6572 2e5f 5f69 6e69 745f 5f63 0300 0000  er.__init__c....
-00001a40: 0000 0000 0000 0000 0500 0000 0500 0000  ................
-00001a50: 4300 0000 7342 0000 007c 02a0 0064 01a1  C...sB...|...d..
-00001a60: 017d 037c 0364 0275 0072 3e7c 006a 016a  .}.|.d.u.r>|.j.j
-00001a70: 027c 02a0 0064 0364 04a1 0264 058d 017d  .|...d.d...d...}
-00001a80: 0474 037c 016a 047c 0464 068d 0204 007d  .t.|.j.|.d.....}
-00001a90: 037c 0264 013c 007c 0353 0029 077a 7f0a  .|.d.<.|.S.).z..
-00001aa0: 2020 2020 2020 2020 7265 7475 726e 7320          returns 
-00001ab0: 616e 2053 716c 6158 6c73 4578 706f 7274  an SqlaXlsExport
-00001ac0: 6572 2066 6f72 2074 6865 2067 6976 656e  er for the given
-00001ad0: 2072 656c 6174 6564 206f 626a 6563 7420   related object 
-00001ae0: 616e 6420 7374 6f72 6573 2069 740a 2020  and stores it.  
-00001af0: 2020 2020 2020 696e 2074 6865 2063 6f6c        in the col
-00001b00: 756d 6e20 6f62 6a65 6374 2061 7320 6120  umn object as a 
-00001b10: 6361 6368 650a 2020 2020 2020 2020 da11  cache.        ..
-00001b20: 7371 6c61 5f78 6c73 5f65 7870 6f72 7465  sqla_xls_exporte
-00001b30: 724e 7245 0000 007a 0d64 6566 6175 6c74  rNrE...z.default
-00001b40: 2074 6974 6c65 2901 7216 0000 0029 0172   title).r....).r
-00001b50: 1500 0000 2905 7231 0000 0072 1300 0000  ....).r1...r....
-00001b60: 5a0c 6372 6561 7465 5f73 6865 6574 725c  Z.create_sheetr\
-00001b70: 0000 00da 095f 5f63 6c61 7373 5f5f 2905  .....__class__).
-00001b80: 7219 0000 00da 0b72 656c 6174 6564 5f6f  r......related_o
-00001b90: 626a 7235 0000 00da 0672 6573 756c 7472  bjr5.....resultr
-00001ba0: 1500 0000 720b 0000 0072 0b00 0000 720c  ....r....r....r.
-00001bb0: 0000 00da 155f 6765 745f 7265 6c61 7465  ....._get_relate
-00001bc0: 645f 6578 706f 7274 6572 0601 0000 7312  d_exporter....s.
-00001bd0: 0000 0000 050a 0108 0106 010a ff06 0302  ................
-00001be0: 0106 ff0e 037a 2553 716c 6158 6c73 4578  .....z%SqlaXlsEx
-00001bf0: 706f 7274 6572 2e5f 6765 745f 7265 6c61  porter._get_rela
-00001c00: 7465 645f 6578 706f 7274 6572 6303 0000  ted_exporterc...
-00001c10: 0000 0000 0000 0000 0009 0000 0005 0000  ................
-00001c20: 0043 0000 0073 7e00 0000 7400 a001 7c00  .C...s~...t...|.
-00001c30: 7c01 7c02 a103 7d03 7c03 6401 6b02 727a  |.|...}.|.d.k.rz
-00001c40: 7c02 a002 6402 6403 a102 7d04 7c02 6404  |...d.d...}.|.d.
-00001c50: 1900 6a03 727a 7c04 6403 7500 727a 7c00  ..j.rz|.d.u.rz|.
-00001c60: 6a04 727a 7c02 6405 1900 7d05 7405 7c01  j.rz|.d...}.t.|.
-00001c70: 7c05 6403 8303 7d06 7c06 7356 6401 5300  |.d...}.|.sVd.S.
-00001c80: 7c00 a006 7c06 6406 1900 7c02 a102 7d07  |...|.d...|...}.
-00001c90: 7c06 4400 5d0e 7d08 7c07 a007 7c08 a101  |.D.].}.|...|...
-00001ca0: 0100 716a 7c03 5300 2907 7a86 0a20 2020  ..qj|.S.).z..   
-00001cb0: 2020 2020 2052 6574 7572 6e20 7468 6520       Return the 
-00001cc0: 7661 6c75 6520 746f 2069 6e73 6572 7420  value to insert 
-00001cd0: 696e 2061 2072 656c 6174 696f 6e73 6869  in a relationshi
-00001ce0: 7020 6365 6c6c 0a20 2020 2020 2020 2048  p cell.        H
-00001cf0: 616e 646c 6520 7468 6520 6361 7365 206f  andle the case o
-00001d00: 6620 636f 6d70 6c65 7820 7265 6c61 7465  f complex relate
-00001d10: 6420 6461 7461 7320 7765 2077 616e 7420  d datas we want 
-00001d20: 746f 2068 616e 646c 650a 2020 2020 2020  to handle.      
-00001d30: 2020 7208 0000 00da 0b72 656c 6174 6564    r......related
-00001d40: 5f6b 6579 4e72 5200 0000 724a 0000 0072  _keyNrR...rJ...r
-00001d50: 0100 0000 2908 7206 0000 00da 1a5f 6765  ....).r......_ge
-00001d60: 745f 7265 6c61 7469 6f6e 7368 6970 5f63  t_relationship_c
-00001d70: 656c 6c5f 7661 6c72 3100 0000 da07 7573  ell_valr1.....us
-00001d80: 656c 6973 7472 5f00 0000 722d 0000 0072  elistr_...r-...r
-00001d90: 6400 0000 da07 6164 645f 726f 7729 0972  d.....add_row).r
-00001da0: 1900 0000 da03 6f62 6a72 3500 0000 da03  ......objr5.....
-00001db0: 7661 6c72 6500 0000 724a 0000 00da 0f72  valre...rJ.....r
-00001dc0: 656c 6174 6564 5f6f 626a 6563 7473 da08  elated_objects..
-00001dd0: 6578 706f 7274 6572 da07 7265 6c5f 6f62  exporter..rel_ob
-00001de0: 6a72 0b00 0000 720b 0000 0072 0c00 0000  jr....r....r....
-00001df0: 7266 0000 0015 0100 0073 1e00 0000 0005  rf.......s......
-00001e00: 0e01 0801 0c02 1803 0801 0c01 0401 0402  ................
-00001e10: 0401 0601 02fe 0404 0801 0c02 7a2a 5371  ............z*Sq
-00001e20: 6c61 586c 7345 7870 6f72 7465 722e 5f67  laXlsExporter._g
-00001e30: 6574 5f72 656c 6174 696f 6e73 6869 705f  et_relationship_
-00001e40: 6365 6c6c 5f76 616c 6301 0000 0000 0000  cell_valc.......
-00001e50: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
-00001e60: 0073 2e00 0000 7400 a001 7c00 a101 0100  .s....t...|.....
-00001e70: 7c00 6a02 4400 5d18 7d01 6401 7c01 7600  |.j.D.].}.d.|.v.
-00001e80: 7210 7c01 6401 1900 a001 a100 0100 7110  r.|.d.........q.
-00001e90: 6402 5300 2903 7a52 0a20 2020 2020 2020  d.S.).zR.       
-00001ea0: 2045 6e68 616e 6365 2074 6865 2064 6566   Enhance the def
-00001eb0: 6175 6c74 2070 6f70 756c 6174 6520 7363  ault populate sc
-00001ec0: 7269 7074 2062 7920 6861 6e64 6c69 6e67  ript by handling
-00001ed0: 2072 656c 6174 6564 2065 6c65 6d65 6e74   related element
-00001ee0: 730a 2020 2020 2020 2020 7260 0000 004e  s.        r`...N
-00001ef0: 2903 720f 0000 0072 3900 0000 722f 0000  ).r....r9...r/..
-00001f00: 0029 0272 1900 0000 7243 0000 0072 0b00  .).r....rC...r..
-00001f10: 0000 720b 0000 0072 0c00 0000 7239 0000  ..r....r....r9..
-00001f20: 002f 0100 0073 0800 0000 0004 0a01 0a01  ./...s..........
-00001f30: 0801 7a19 5371 6c61 586c 7345 7870 6f72  ..z.SqlaXlsExpor
-00001f40: 7465 722e 5f70 6f70 756c 6174 6529 0254  ter._populate).T
-00001f50: 4e29 0972 4d00 0000 724e 0000 0072 4f00  N).rM...rN...rO.
-00001f60: 0000 7250 0000 00da 0a63 6f6e 6669 675f  ..rP.....config_
-00001f70: 6b65 7972 1b00 0000 7264 0000 0072 6600  keyr....rd...rf.
-00001f80: 0000 7239 0000 0072 0b00 0000 720b 0000  ..r9...r....r...
-00001f90: 0072 0b00 0000 720c 0000 0072 5c00 0000  .r....r....r\...
-00001fa0: d700 0000 730c 0000 0008 0104 2604 020a  ....s.......&...
-00001fb0: 0608 0f08 1a72 5c00 0000 6300 0000 0000  .....r\...c.....
-00001fc0: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
-00001fd0: 0000 0073 1e00 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
-00001fe0: 6401 5a03 6402 5a04 6407 6404 6405 8401  d.Z.d.Z.d.d.d...
-00001ff0: 5a05 6406 5300 2908 da0b 586c 7345 7870  Z.d.S.)...XlsExp
-00002000: 6f72 7465 727a bc0a 2020 2020 4120 6d61  orterz..    A ma
-00002010: 696e 2078 6c73 2065 7870 6f72 7461 7469  in xls exportati
-00002020: 6f6e 2074 6f6f 6c20 2877 6974 686f 7574  on tool (without
-00002030: 2073 716c 616c 6368 656d 7920 7375 7070   sqlalchemy supp
-00002040: 6f72 7429 0a0a 2020 2020 7772 6974 6572  ort)..    writer
-00002050: 203d 204d 7958 6c73 4578 706f 7274 6572   = MyXlsExporter
-00002060: 2829 0a20 2020 2077 7269 7465 722e 6164  ().    writer.ad
-00002070: 645f 726f 7728 7b27 6b65 7927 3a20 7527  d_row({'key': u'
-00002080: 4c61 2076 616c 6575 7220 6465 206c 6120  La valeur de la 
-00002090: 6365 6c6c 756c 6520 6465 206c 6120 636f  cellule de la co
-000020a0: 6c6f 6e6e 6520 3127 7d29 0a20 2020 2077  lonne 1'}).    w
-000020b0: 7269 7465 722e 7265 6e64 6572 2829 0a20  riter.render(). 
-000020c0: 2020 2072 0b00 0000 5463 0200 0000 0000     r....Tc......
-000020d0: 0000 0000 0000 0300 0000 0400 0000 4b00  ..............K.
-000020e0: 0000 732c 0000 0074 006a 017c 0066 0164  ..s,...t.j.|.f.d
-000020f0: 017c 0169 017c 02a4 018e 0101 0074 026a  .|.i.|.......t.j
-00002100: 017c 0066 0169 007c 02a4 018e 0101 0064  .|.f.i.|.......d
-00002110: 0053 0029 024e 725d 0000 0029 0372 0f00  .S.).Nr]...).r..
-00002120: 0000 721b 0000 0072 0500 0000 2903 7219  ..r....r....).r.
-00002130: 0000 0072 5d00 0000 721a 0000 0072 0b00  ...r]...r....r..
-00002140: 0000 720b 0000 0072 0c00 0000 721b 0000  ..r....r....r...
-00002150: 0044 0100 0073 0400 0000 0001 1601 7a14  .D...s........z.
-00002160: 586c 7345 7870 6f72 7465 722e 5f5f 696e  XlsExporter.__in
-00002170: 6974 5f5f 4e29 0154 2906 724d 0000 0072  it__N).T).rM...r
-00002180: 4e00 0000 724f 0000 0072 5000 0000 722f  N...rO...rP...r/
-00002190: 0000 0072 1b00 0000 720b 0000 0072 0b00  ...r....r....r..
-000021a0: 0000 720b 0000 0072 0c00 0000 726f 0000  ..r....r....ro..
-000021b0: 0039 0100 0073 0600 0000 0801 0408 0402  .9...s..........
-000021c0: 726f 0000 0029 014e 291b 7250 0000 00da  ro...).N).rP....
-000021d0: 0969 7465 7274 6f6f 6c73 da07 6c6f 6767  .itertools..logg
-000021e0: 696e 6772 1200 0000 5a0f 6f70 656e 7079  ingr....Z.openpy
-000021f0: 786c 2e73 7479 6c65 7372 0200 0000 7203  xl.stylesr....r.
-00002200: 0000 0072 1c00 0000 da06 7374 7269 6e67  ...r......string
-00002210: 7204 0000 00da 1373 716c 615f 696e 7370  r......sqla_insp
-00002220: 6563 742e 6578 706f 7274 7205 0000 0072  ect.exportr....r
-00002230: 0600 0000 da11 7371 6c61 5f69 6e73 7065  ......sqla_inspe
-00002240: 6374 2e62 6173 6572 0700 0000 da09 6765  ct.baser......ge
-00002250: 744c 6f67 6765 7272 4d00 0000 da03 6c6f  tLoggerrM.....lo
-00002260: 67da 046c 6973 74da 1d63 6f6d 6269 6e61  g..list..combina
-00002270: 7469 6f6e 735f 7769 7468 5f72 6570 6c61  tions_with_repla
-00002280: 6365 6d65 6e74 5a0f 4153 4349 495f 5550  cementZ.ASCII_UP
-00002290: 5045 5243 4153 4572 5600 0000 da06 6f62  PERCASErV.....ob
-000022a0: 6a65 6374 720f 0000 0072 4000 0000 725c  jectr....r@...r\
-000022b0: 0000 0072 6f00 0000 720b 0000 0072 0b00  ...ro...r....r..
-000022c0: 0000 720b 0000 0072 0c00 0000 da08 3c6d  ..r....r......<m
-000022d0: 6f64 756c 653e 0600 0000 7324 0000 0004  odule>....s$....
-000022e0: 0408 0108 0108 0110 0508 010c 0210 040c  ................
-000022f0: 030a 040e 020a fe0a 0606 0310 7f00 1d0a  ................
-00002300: 1212 62                                  ..b
+00000020: 0007 0000 0040 0000 0073 ea00 0000 6400  .....@...s....d.
+00000030: 5a00 6401 6402 6c01 5a02 6401 6402 6c03  Z.d.d.l.Z.d.d.l.
+00000040: 6d04 0200 0100 6d05 5a06 0100 6401 6402  m.....m.Z...d.d.
+00000050: 6c07 5a07 6401 6402 6c08 5a08 6401 6402  l.Z.d.d.l.Z.d.d.
+00000060: 6c09 5a09 6401 6403 6c0a 6d0b 5a0b 6d0c  l.Z.d.d.l.m.Z.m.
+00000070: 5a0c 0100 6401 6402 6c0d 5a0d 6401 6404  Z...d.d.l.Z.d.d.
+00000080: 6c0e 6d0f 5a0f 0100 6401 6405 6c10 6d11  l.m.Z...d.d.l.m.
+00000090: 5a11 6d12 5a12 0100 6401 6406 6c13 6d14  Z.m.Z...d.d.l.m.
+000000a0: 5a14 0100 6508 a015 6516 a101 5a17 6518  Z...e...e...Z.e.
+000000b0: 650f 8301 6518 6407 6408 8400 6507 a019  e...e.d.d...e...
+000000c0: 650f 6409 a102 4400 8301 8301 1700 5a1a  e.d...D.......Z.
+000000d0: 6514 8300 5a1b 4700 640a 640b 8400 640b  e...Z.G.d.d...d.
+000000e0: 651c 8303 5a1d 6412 640c 640d 8401 5a1e  e...Z.d.d.d...Z.
+000000f0: 4700 640e 640f 8400 640f 651d 6512 8304  G.d.d...d.e.e...
+00000100: 5a1f 4700 6410 6411 8400 6411 651d 6511  Z.G.d.d...d.e.e.
+00000110: 8304 5a20 6402 5300 2913 7a1a 0a45 7863  ..Z d.S.).z..Exc
+00000120: 656c 2065 7870 6f72 7461 7469 6f6e 206d  el exportation m
+00000130: 6f64 756c 650a e900 0000 004e 2902 da05  odule......N)...
+00000140: 436f 6c6f 72da 0446 6f6e 7429 01da 0f61  Color..Font)...a
+00000150: 7363 6969 5f75 7070 6572 6361 7365 2902  scii_uppercase).
+00000160: da0c 4261 7365 4578 706f 7274 6572 da0c  ..BaseExporter..
+00000170: 5371 6c61 4578 706f 7274 6572 2901 da08  SqlaExporter)...
+00000180: 5265 6769 7374 7279 6301 0000 0000 0000  Registryc.......
+00000190: 0000 0000 0002 0000 0004 0000 0063 0000  .............c..
+000001a0: 0073 1800 0000 7c00 5d10 7d01 6400 a000  .s....|.].}.d...
+000001b0: 7c01 a101 5600 0100 7102 6401 5300 2902  |...V...q.d.S.).
+000001c0: da00 4e29 01da 046a 6f69 6e29 02da 022e  ..N)...join)....
+000001d0: 305a 0564 7570 6c65 a900 720b 0000 00fa  0Z.duple..r.....
+000001e0: 312f 686f 6d65 2f67 6173 2f65 6e64 692f  1/home/gas/endi/
+000001f0: 7371 6c61 5f69 6e73 7065 6374 2f73 716c  sqla_inspect/sql
+00000200: 615f 696e 7370 6563 742f 6578 6365 6c2e  a_inspect/excel.
+00000210: 7079 da09 3c67 656e 6578 7072 3e20 0000  py..<genexpr> ..
+00000220: 0073 0400 0000 0402 02ff 720d 0000 00e9  .s........r.....
+00000230: 0200 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00000240: 0000 0000 0003 0000 0040 0000 0073 7a00  .........@...sz.
+00000250: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
+00000260: 5a04 641b 6404 6405 8401 5a05 641c 6406  Z.d.d.d...Z.d.d.
+00000270: 6407 8401 5a06 6408 6409 8400 5a07 6508  d...Z.d.d...Z.e.
+00000280: 6508 640a 9c02 640b 640c 8404 5a09 640d  e.d...d.d...Z.d.
+00000290: 640e 8400 5a0a 640f 6410 8400 5a0b 641d  d...Z.d.d...Z.d.
+000002a0: 6411 6412 8401 5a0c 6413 6414 8400 5a0d  d.d...Z.d.d...Z.
+000002b0: 6415 6416 8400 5a0e 6417 6418 8400 5a0f  d.d...Z.d.d...Z.
+000002c0: 6419 641a 8400 5a10 6403 5300 291e da09  d.d...Z.d.S.)...
+000002d0: 586c 7357 7269 7465 7261 9401 0000 0a20  XlsWritera..... 
+000002e0: 2020 2043 6c61 7373 2070 726f 7669 6469     Class providi
+000002f0: 6e67 2063 6f6d 6d6f 6e20 746f 6f6c 7320  ng common tools 
+00000300: 746f 2077 7269 7465 2065 7863 656c 2066  to write excel f
+00000310: 696c 6573 2066 726f 6d20 7461 6275 6c61  iles from tabula
+00000320: 7220 6461 7461 730a 0a20 2020 2048 6173  r datas..    Has
+00000330: 2074 6f20 6265 2073 7562 636c 6173 7365   to be subclasse
+00000340: 642c 2074 6865 2073 7562 636c 6173 7320  d, the subclass 
+00000350: 7368 6f75 6c64 2070 726f 7669 6465 2061  should provide a
+00000360: 205f 6461 7461 7320 616e 6420 6120 6865   _datas and a he
+00000370: 6164 6572 730a 2020 2020 6174 7472 6962  aders.    attrib
+00000380: 7574 6520 7468 6174 2063 6f6e 7461 696e  ute that contain
+00000390: 7320 7468 6520 6461 7461 7320 746f 2072  s the datas to r
+000003a0: 656e 6465 7220 616e 6420 7468 6520 6865  ender and the he
+000003b0: 6164 6572 730a 0a20 2020 2020 2020 205f  aders..        _
+000003c0: 6461 7461 730a 0a20 2020 2020 2020 2020  datas..         
+000003d0: 2020 206c 6973 7420 6f66 2074 7570 6c65     list of tuple
+000003e0: 7320 2865 6163 6820 7475 706c 6520 6973  s (each tuple is
+000003f0: 2061 2072 6f77 290a 0a20 2020 2020 2020   a row)..       
+00000400: 2068 6561 6465 7273 0a0a 2020 2020 2020   headers..      
+00000410: 2020 2020 2020 6c69 7374 206f 6620 6469        list of di
+00000420: 6374 2063 6f6e 7461 696e 696e 6720 7468  ct containing th
+00000430: 6520 6c61 6265 6c20 6f66 2065 6163 6820  e label of each 
+00000440: 636f 6c75 6d6e 3a0a 2020 2020 2020 2020  column:.        
+00000450: 2020 2020 2020 2020 7b27 6c61 6265 6c27          {'label'
+00000460: 3a20 3c61 206c 6162 656c 3e7d 0a0a 2020  : <a label>}..  
+00000470: 2020 5a06 4578 706f 7274 4e63 0200 0000    Z.ExportNc....
+00000480: 0000 0000 0000 0000 0300 0000 0200 0000  ................
+00000490: 4b00 0000 7342 0000 007c 0164 0075 0072  K...sB...|.d.u.r
+000004a0: 2a74 006a 01a0 02a1 007c 005f 037c 006a  *t.j.....|._.|.j
+000004b0: 036a 047c 005f 057c 006a 067c 006a 055f  .j.|._.|.j.|.j._
+000004c0: 066e 0e7c 017c 005f 057c 016a 077c 005f  .n.|.|._.|.j.|._
+000004d0: 037c 027c 005f 0864 0053 00a9 014e 2909  .|.|._.d.S...N).
+000004e0: da08 6f70 656e 7079 786c 5a08 776f 726b  ..openpyxlZ.work
+000004f0: 626f 6f6b 5a08 576f 726b 626f 6f6b da04  bookZ.Workbook..
+00000500: 626f 6f6b da06 6163 7469 7665 da09 776f  book..active..wo
+00000510: 726b 7368 6565 74da 0574 6974 6c65 da06  rksheet..title..
+00000520: 7061 7265 6e74 da07 6f70 7469 6f6e 7329  parent..options)
+00000530: 03da 0473 656c 6672 1400 0000 da02 6b77  ...selfr......kw
+00000540: 720b 0000 0072 0b00 0000 720c 0000 00da  r....r....r.....
+00000550: 085f 5f69 6e69 745f 5f3d 0000 0073 0e00  .__init__=...s..
+00000560: 0000 0001 0801 0c01 0a01 0c02 0601 0801  ................
+00000570: 7a12 586c 7357 7269 7465 722e 5f5f 696e  z.XlsWriter.__in
+00000580: 6974 5f5f 6302 0000 0000 0000 0000 0000  it__c...........
+00000590: 0002 0000 0005 0000 0043 0000 0073 4e00  .........C...sN.
+000005a0: 0000 7c01 6401 7500 7210 7400 a001 a100  ..|.d.u.r.t.....
+000005b0: 7d01 7402 7c00 6a03 6402 8302 722a 7c00  }.t.|.j.d...r*|.
+000005c0: 6a03 a004 7c01 a101 0100 6e16 7c01 a005  j...|.....n.|...
+000005d0: 7406 6a07 6a08 a009 7c00 6a03 a101 a101  t.j.j...|.j.....
+000005e0: 0100 7c01 a00a 6403 a101 0100 7c01 5300  ..|...d.....|.S.
+000005f0: 2904 7a9a 0a20 2020 2020 2020 2052 6574  ).z..        Ret
+00000600: 7572 6e20 6120 6669 6c65 2062 7566 6665  urn a file buffe
+00000610: 7220 636f 6e74 6169 6e69 6e67 2074 6865  r containing the
+00000620: 2072 6573 756c 7469 6e67 2078 6c73 0a0a   resulting xls..
+00000630: 2020 2020 2020 2020 3a70 6172 616d 206f          :param o
+00000640: 626a 2066 5f62 7566 3a20 4120 6669 6c65  bj f_buf: A file
+00000650: 2062 7566 6665 7220 7375 7070 6f72 7469   buffer supporti
+00000660: 6e67 2074 6865 2077 7269 7465 2061 6e64  ng the write and
+00000670: 2073 6565 6b0a 2020 2020 2020 2020 6d65   seek.        me
+00000680: 7468 6f64 730a 2020 2020 2020 2020 4eda  thods.        N.
+00000690: 0473 6176 6572 0100 0000 290b da02 696f  .saver....)...io
+000006a0: da07 4279 7465 7349 4fda 0768 6173 6174  ..BytesIO..hasat
+000006b0: 7472 7212 0000 0072 1b00 0000 da05 7772  trr....r......wr
+000006c0: 6974 6572 1100 0000 da06 7772 6974 6572  iter......writer
+000006d0: da05 6578 6365 6c5a 1573 6176 655f 7669  ..excelZ.save_vi
+000006e0: 7274 7561 6c5f 776f 726b 626f 6f6b da04  rtual_workbook..
+000006f0: 7365 656b a902 7218 0000 00da 0566 5f62  seek..r......f_b
+00000700: 7566 720b 0000 0072 0b00 0000 720c 0000  ufr....r....r...
+00000710: 00da 0973 6176 655f 626f 6f6b 4700 0000  ...save_bookG...
+00000720: 730e 0000 0000 0708 0108 020c 010e 0316  s...............
+00000730: 020a 017a 1358 6c73 5772 6974 6572 2e73  ...z.XlsWriter.s
+00000740: 6176 655f 626f 6f6b 6303 0000 0000 0000  ave_bookc.......
+00000750: 0000 0000 0003 0000 0004 0000 0043 0000  .............C..
+00000760: 0073 1600 0000 7400 7401 7c02 6401 8d01  .s....t.t.|.d...
+00000770: 6402 8d01 7c01 5f02 6403 5300 2904 7aa8  d...|._.d.S.).z.
+00000780: 0a20 2020 2020 2020 2053 6574 2074 6865  .        Set the
+00000790: 2067 6976 656e 2063 6f6c 6f72 2074 6f20   given color to 
+000007a0: 7468 6520 7072 6f76 6964 6564 2063 656c  the provided cel
+000007b0: 6c0a 0a20 2020 2020 2020 2020 2020 2063  l..            c
+000007c0: 656c 6c0a 0a20 2020 2020 2020 2020 2020  ell..           
+000007d0: 2020 2020 2041 2078 6c73 2063 656c 6c20       A xls cell 
+000007e0: 6f62 6a65 6374 0a0a 2020 2020 2020 2020  object..        
+000007f0: 2020 2020 636f 6c6f 720a 0a20 2020 2020      color..     
+00000800: 2020 2020 2020 2020 2020 2041 206f 7065             A ope
+00000810: 6e70 7978 6c20 636f 6c6f 7220 7661 720a  npyxl color var.
+00000820: 2020 2020 2020 2020 2901 da03 7267 6229          )...rgb)
+00000830: 01da 0563 6f6c 6f72 4e29 0372 0300 0000  ...colorN).r....
+00000840: 7202 0000 005a 0466 6f6e 7429 0372 1800  r....Z.font).r..
+00000850: 0000 da04 6365 6c6c 7227 0000 0072 0b00  ....cellr'...r..
+00000860: 0000 720b 0000 0072 0c00 0000 da09 7365  ..r....r......se
+00000870: 745f 636f 6c6f 725a 0000 0073 0200 0000  t_colorZ...s....
+00000880: 000c 7a13 586c 7357 7269 7465 722e 7365  ..z.XlsWriter.se
+00000890: 745f 636f 6c6f 7229 02da 0b63 6f6c 756d  t_color)...colum
+000008a0: 6e5f 6e61 6d65 da05 7661 6c75 6563 0300  n_name..valuec..
+000008b0: 0000 0000 0000 0000 0000 0300 0000 0400  ................
+000008c0: 0000 4300 0000 7324 0000 0074 007c 0064  ..C...s$...t.|.d
+000008d0: 017c 0116 0083 0272 2074 017c 0064 017c  .|.....r t.|.d.|
+000008e0: 0116 0083 027c 0283 017d 027c 0253 0029  .....|...}.|.S.)
+000008f0: 027a 1f0a 2020 2020 2020 2020 466f 726d  .z..        Form
+00000900: 6174 2061 2063 656c 6c0a 2020 2020 2020  at a cell.      
+00000910: 2020 7a09 666f 726d 6174 5f25 7329 0272    z.format_%s).r
+00000920: 1e00 0000 da07 6765 7461 7474 7229 0372  ......getattr).r
+00000930: 1800 0000 722a 0000 0072 2b00 0000 720b  ....r*...r+...r.
+00000940: 0000 0072 0b00 0000 720c 0000 00da 0b66  ...r....r......f
+00000950: 6f72 6d61 745f 6365 6c6c 6800 0000 7306  ormat_cellh...s.
+00000960: 0000 0000 040e 0112 017a 1558 6c73 5772  .........z.XlsWr
+00000970: 6974 6572 2e66 6f72 6d61 745f 6365 6c6c  iter.format_cell
+00000980: 6302 0000 0000 0000 0000 0000 0007 0000  c...............
+00000990: 0005 0000 0043 0000 0073 4800 0000 6700  .....C...sH...g.
+000009a0: 7d02 7400 7c00 6401 6700 8303 7d03 7c03  }.t.|.d.g...}.|.
+000009b0: 4400 5d2e 7d04 7c04 6402 1900 7d05 7c01  D.].}.|.d...}.|.
+000009c0: a001 7c05 6403 a102 7d06 7c00 a002 7c05  ..|.d...}.|...|.
+000009d0: 7c06 a102 7d06 7c02 a003 7c06 a101 0100  |...}.|...|.....
+000009e0: 7114 7c02 5300 2904 7a96 0a20 2020 2020  q.|.S.).z..     
+000009f0: 2020 2054 6865 2072 656e 6465 7220 6d65     The render me
+00000a00: 7468 6f64 2065 7870 6563 7473 2072 6f77  thod expects row
+00000a10: 7320 6173 206c 6973 7473 2c20 6865 7265  s as lists, here
+00000a20: 2077 6520 7377 6974 6368 206f 7572 2072   we switch our r
+00000a30: 6f77 2066 6f72 6d61 740a 2020 2020 2020  ow format.      
+00000a40: 2020 6672 6f6d 2064 6963 7420 746f 206c    from dict to l
+00000a50: 6973 7420 7265 7370 6563 7469 6e67 2074  ist respecting t
+00000a60: 6865 206f 7264 6572 206f 6620 7468 6520  he order of the 
+00000a70: 6865 6164 6572 730a 2020 2020 2020 2020  headers.        
+00000a80: da07 6865 6164 6572 73da 046e 616d 6572  ..headers..namer
+00000a90: 0800 0000 2904 722c 0000 00da 0367 6574  ....).r,.....get
+00000aa0: 722d 0000 00da 0661 7070 656e 6429 0772  r-.....append).r
+00000ab0: 1800 0000 da03 726f 77da 0372 6573 722e  ......row..resr.
+00000ac0: 0000 00da 0663 6f6c 756d 6e72 2a00 0000  .....columnr*...
+00000ad0: 722b 0000 0072 0b00 0000 720b 0000 0072  r+...r....r....r
+00000ae0: 0c00 0000 da0a 666f 726d 6174 5f72 6f77  ......format_row
+00000af0: 7000 0000 7310 0000 0000 0504 010c 0108  p...s...........
+00000b00: 0108 010c 010c 010c 017a 1458 6c73 5772  .........z.XlsWr
+00000b10: 6974 6572 2e66 6f72 6d61 745f 726f 7763  iter.format_rowc
+00000b20: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000b30: 0200 0000 4300 0000 7314 0000 007c 00a0  ....C...s....|..
+00000b40: 00a1 0001 007c 00a0 01a1 0001 0064 0153  .....|.......d.S
+00000b50: 0029 027a 430a 2020 2020 2020 2020 506f  .).zC.        Po
+00000b60: 7075 6c61 7465 2068 6561 6465 7273 2061  pulate headers a
+00000b70: 6e64 2072 6f77 7320 6265 666f 7265 2077  nd rows before w
+00000b80: 7269 7469 6e67 206f 7572 2062 6f6f 6b0a  riting our book.
+00000b90: 2020 2020 2020 2020 4e29 02da 0f5f 7265          N)..._re
+00000ba0: 6e64 6572 5f68 6561 6465 7273 da0c 5f72  nder_headers.._r
+00000bb0: 656e 6465 725f 726f 7773 2901 7218 0000  ender_rows).r...
+00000bc0: 0072 0b00 0000 720b 0000 0072 0c00 0000  .r....r....r....
+00000bd0: da09 5f70 6f70 756c 6174 657e 0000 0073  .._populate~...s
+00000be0: 0400 0000 0004 0801 7a13 586c 7357 7269  ........z.XlsWri
+00000bf0: 7465 722e 5f70 6f70 756c 6174 6563 0200  ter._populatec..
+00000c00: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+00000c10: 0000 4300 0000 7312 0000 007c 00a0 00a1  ..C...s....|....
+00000c20: 0001 007c 00a0 017c 01a1 0153 0029 017a  ...|...|...S.).z
+00000c30: 870a 2020 2020 2020 2020 4465 6669 6e69  ..        Defini
+00000c40: 7465 6c79 2072 656e 6465 7220 7468 6520  tely render the 
+00000c50: 776f 726b 626f 6f6b 0a0a 2020 2020 2020  workbook..      
+00000c60: 2020 3a70 6172 616d 206f 626a 2066 5f62    :param obj f_b
+00000c70: 7566 3a20 4120 6669 6c65 2062 7566 6665  uf: A file buffe
+00000c80: 7220 7375 7070 6f72 7469 6e67 2074 6865  r supporting the
+00000c90: 2077 7269 7465 2061 6e64 2073 6565 6b0a   write and seek.
+00000ca0: 2020 2020 2020 2020 6d65 7468 6f64 730a          methods.
+00000cb0: 2020 2020 2020 2020 2902 7238 0000 0072          ).r8...r
+00000cc0: 2500 0000 7223 0000 0072 0b00 0000 720b  %...r#...r....r.
+00000cd0: 0000 0072 0c00 0000 da06 7265 6e64 6572  ...r......render
+00000ce0: 8500 0000 7304 0000 0000 0708 027a 1058  ....s........z.X
+00000cf0: 6c73 5772 6974 6572 2e72 656e 6465 7263  lsWriter.renderc
+00000d00: 0100 0000 0000 0000 0000 0000 0b00 0000  ................
+00000d10: 0600 0000 4300 0000 739c 0000 0074 007c  ....C...s....t.|
+00000d20: 0064 0164 0283 037d 0174 007c 0064 0364  .d.d...}.t.|.d.d
+00000d30: 0283 037d 0274 017c 0183 0144 005d 765c  ...}.t.|...D.]v\
+00000d40: 027d 037d 047c 0364 0417 007d 0574 017c  .}.}.|.d...}.t.|
+00000d50: 0483 0144 005d 5c5c 027d 067d 077c 006a  ...D.]\\.}.}.|.j
+00000d60: 026a 037c 057c 0664 0517 0064 068d 027d  .j.|.|.d...d...}
+00000d70: 087c 0764 0775 0172 647c 077c 085f 046e  .|.d.u.rd|.|._.n
+00000d80: 0664 087c 085f 0474 057c 0283 017c 066b  .d.|._.t.|...|.k
+00000d90: 0472 387c 027c 0619 007d 0974 067c 0983  .r8|.|...}.t.|..
+00000da0: 017d 0a7c 0a64 0775 0172 387c 0a7c 085f  .}.|.d.u.r8|.|._
+00000db0: 0771 3871 2064 0753 0029 097a 3b0a 2020  .q8q d.S.).z;.  
+00000dc0: 2020 2020 2020 5265 6e64 6572 2074 6865        Render the
+00000dd0: 2072 6f77 7320 696e 2074 6865 2063 7572   rows in the cur
+00000de0: 7265 6e74 2073 7479 6c65 7368 6565 740a  rent stylesheet.
+00000df0: 2020 2020 2020 2020 da06 5f64 6174 6173          .._datas
+00000e00: 720b 0000 0072 2e00 0000 720e 0000 00e9  r....r....r.....
+00000e10: 0100 0000 a902 7232 0000 0072 3400 0000  ......r2...r4...
+00000e20: 4e72 0800 0000 2908 722c 0000 00da 0965  Nr....).r,.....e
+00000e30: 6e75 6d65 7261 7465 7214 0000 0072 2800  numerater....r(.
+00000e40: 0000 722b 0000 00da 036c 656e da0f 6765  ..r+.....len..ge
+00000e50: 745f 6365 6c6c 5f66 6f72 6d61 745a 0d6e  t_cell_formatZ.n
+00000e60: 756d 6265 725f 666f 726d 6174 290b 7218  umber_format).r.
+00000e70: 0000 0072 3a00 0000 722e 0000 00da 0569  ...r:...r......i
+00000e80: 6e64 6578 7232 0000 005a 0a72 6f77 5f6e  ndexr2...Z.row_n
+00000e90: 756d 6265 725a 0763 6f6c 5f6e 756d 722b  umberZ.col_numr+
+00000ea0: 0000 0072 2800 0000 da06 6865 6164 6572  ...r(.....header
+00000eb0: da06 666f 726d 6174 720b 0000 0072 0b00  ..formatr....r..
+00000ec0: 0000 720c 0000 0072 3700 0000 9000 0000  ..r....r7.......
+00000ed0: 731c 0000 0000 040c 010c 0110 0108 0110  s...............
+00000ee0: 0114 0108 0108 0206 010c 0108 0108 0108  ................
+00000ef0: 017a 1658 6c73 5772 6974 6572 2e5f 7265  .z.XlsWriter._re
+00000f00: 6e64 6572 5f72 6f77 7363 0100 0000 0000  nder_rowsc......
+00000f10: 0000 0000 0000 0700 0000 0500 0000 4300  ..............C.
+00000f20: 0000 7388 0000 0074 007c 0064 0164 0283  ..s....t.|.d.d..
+00000f30: 037d 0174 017c 0183 0144 005d 265c 027d  .}.t.|...D.]&\.}
+00000f40: 027d 037c 006a 026a 0364 037c 0264 0317  .}.|.j.j.d.|.d..
+00000f50: 0064 048d 027d 047c 0364 0519 007c 045f  .d...}.|.d...|._
+00000f60: 0471 147c 0264 0337 007d 0274 007c 0064  .q.|.d.7.}.t.|.d
+00000f70: 0664 0283 037d 0574 017c 0583 0144 005d  .d...}.t.|...D.]
+00000f80: 2a5c 027d 067d 037c 006a 026a 0364 037c  *\.}.}.|.j.j.d.|
+00000f90: 067c 0217 0064 0317 0064 048d 027d 047c  .|...d...d...}.|
+00000fa0: 0364 0519 007c 045f 0471 5864 0753 0029  .d...|._.qXd.S.)
+00000fb0: 087a 270a 2020 2020 2020 2020 5772 6974  .z'.        Writ
+00000fc0: 6520 7468 6520 6865 6164 6572 7320 726f  e the headers ro
+00000fd0: 770a 2020 2020 2020 2020 722e 0000 0072  w.        r....r
+00000fe0: 0b00 0000 723b 0000 0072 3c00 0000 da05  ....r;...r<.....
+00000ff0: 6c61 6265 6cda 0d65 7874 7261 5f68 6561  label..extra_hea
+00001000: 6465 7273 4e29 0572 2c00 0000 723d 0000  dersN).r,...r=..
+00001010: 0072 1400 0000 7228 0000 0072 2b00 0000  .r....r(...r+...
+00001020: 2907 7218 0000 0072 2e00 0000 7240 0000  ).r....r....r@..
+00001030: 00da 0363 6f6c 7228 0000 0072 4400 0000  ...colr(...rD...
+00001040: 5a09 6164 645f 696e 6465 7872 0b00 0000  Z.add_indexr....
+00001050: 720b 0000 0072 0c00 0000 7236 0000 00a4  r....r....r6....
+00001060: 0000 0073 1200 0000 0004 0c01 1002 1401  ...s............
+00001070: 0c02 0802 0c01 1001 1801 7a19 586c 7357  ..........z.XlsW
+00001080: 7269 7465 722e 5f72 656e 6465 725f 6865  riter._render_he
+00001090: 6164 6572 7363 0200 0000 0000 0000 0000  adersc..........
+000010a0: 0000 0200 0000 0200 0000 4300 0000 730c  ..........C...s.
+000010b0: 0000 007c 017c 006a 005f 0164 0053 0072  ...|.|.j._.d.S.r
+000010c0: 1000 0000 2902 7214 0000 0072 1500 0000  ....).r....r....
+000010d0: 2902 7218 0000 0072 1500 0000 720b 0000  ).r....r....r...
+000010e0: 0072 0b00 0000 720c 0000 00da 0973 6574  .r....r......set
+000010f0: 5f74 6974 6c65 b500 0000 7302 0000 0000  _title....s.....
+00001100: 017a 1358 6c73 5772 6974 6572 2e73 6574  .z.XlsWriter.set
+00001110: 5f74 6974 6c65 6302 0000 0000 0000 0000  _titlec.........
+00001120: 0000 0004 0000 0007 0000 0043 0000 0073  ...........C...s
+00001130: 5a00 0000 6700 7c00 5f00 6401 7c00 6a01  Z...g.|._.d.|.j.
+00001140: 7600 7250 7c00 6a01 6401 1900 4400 5d32  v.rP|.j.d...D.]2
+00001150: 7d02 7c01 4400 5d28 7d03 7c03 a002 6402  }.|.D.](}.|...d.
+00001160: 7c03 6403 1900 a102 7c02 6b02 7222 7c00  |.d.....|.k.r"|.
+00001170: 6a00 a003 7c03 a101 0100 0100 711a 7122  j...|.......q.q"
+00001180: 711a 6e06 7c01 7c00 5f00 6404 5300 2905  q.n.|.|._.d.S.).
+00001190: 7aeb 0a20 2020 2020 2020 2053 6574 2074  z..        Set t
+000011a0: 6865 2068 6561 6465 7273 206f 6620 6f75  he headers of ou
+000011b0: 7220 7772 6974 6572 0a20 2020 2020 2020  r writer.       
+000011c0: 203a 7061 7261 6d20 6c69 7374 2068 6561   :param list hea
+000011d0: 6465 7273 3a20 6c69 7374 206f 6620 6469  ders: list of di
+000011e0: 6374 2077 6974 6820 6174 206c 6561 7374  ct with at least
+000011f0: 2061 206c 6162 656c 206b 6579 0a20 2020   a label key.   
+00001200: 2020 2020 2028 6c61 6265 6c20 6973 206d       (label is m
+00001210: 616e 6461 746f 7279 203a 2075 7365 6420  andatory : used 
+00001220: 666f 7220 7468 6520 6578 706f 7274 290a  for the export).
+00001230: 0a20 2020 2020 2020 2048 6561 6465 7273  .        Headers
+00001240: 2061 7265 2066 696c 7465 7265 6420 616e   are filtered an
+00001250: 6420 6f72 6465 7265 6420 7265 6761 7264  d ordered regard
+00001260: 696e 6720 7468 6520 6f72 6465 7220 6f70  ing the order op
+00001270: 7469 6f6e 0a20 2020 2020 2020 20da 056f  tion.        ..o
+00001280: 7264 6572 da03 6b65 7972 4300 0000 4e29  rder..keyrC...N)
+00001290: 0472 2e00 0000 7217 0000 0072 3000 0000  .r....r....r0...
+000012a0: 7231 0000 0029 0472 1800 0000 722e 0000  r1...).r....r...
+000012b0: 00da 0765 6c65 6d65 6e74 7241 0000 0072  ...elementrA...r
+000012c0: 0b00 0000 720b 0000 0072 0c00 0000 da0b  ....r....r......
+000012d0: 7365 745f 6865 6164 6572 73b8 0000 0073  set_headers....s
+000012e0: 1000 0000 0008 0601 0a01 0e01 0801 1401  ................
+000012f0: 0c01 0a02 7a15 586c 7357 7269 7465 722e  ....z.XlsWriter.
+00001300: 7365 745f 6865 6164 6572 7329 014e 2901  set_headers).N).
+00001310: 4e29 014e 2911 da08 5f5f 6e61 6d65 5f5f  N).N)...__name__
+00001320: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+00001330: 7175 616c 6e61 6d65 5f5f da07 5f5f 646f  qualname__..__do
+00001340: 635f 5f72 1500 0000 721a 0000 0072 2500  c__r....r....r%.
+00001350: 0000 7229 0000 00da 0373 7472 722d 0000  ..r).....strr-..
+00001360: 0072 3500 0000 7238 0000 0072 3900 0000  .r5...r8...r9...
+00001370: 7237 0000 0072 3600 0000 7246 0000 0072  r7...r6...rF...r
+00001380: 4a00 0000 720b 0000 0072 0b00 0000 720b  J...r....r....r.
+00001390: 0000 0072 0c00 0000 720f 0000 0029 0000  ...r....r....)..
+000013a0: 0073 1a00 0000 0801 0411 0402 0a0a 0a13  .s..............
+000013b0: 080e 1008 080e 0807 0a0b 0814 0811 0803  ................
+000013c0: 720f 0000 0063 0200 0000 0000 0000 0000  r....c..........
+000013d0: 0000 0600 0000 0400 0000 4300 0000 7356  ..........C...sV
+000013e0: 0000 007c 00a0 0064 01a1 017d 027c 00a0  ...|...d...}.|..
+000013f0: 0064 02a1 017d 037c 0264 0375 0072 527c  .d...}.|.d.u.rR|
+00001400: 0364 0375 0172 5274 017c 0364 0483 0272  .d.u.rRt.|.d...r
+00001410: 527c 036a 0264 0519 007d 0474 037c 046a  R|.j.d...}.t.|.j
+00001420: 0464 067c 046a 0483 037d 0574 05a0 067c  .d.|.j...}.t...|
+00001430: 05a1 017d 027c 0253 0029 077a 9f0a 2020  ...}.|.S.).z..  
+00001440: 2020 5265 7475 726e 2074 6865 2063 656c    Return the cel
+00001450: 6c20 666f 726d 6174 2066 6f72 2074 6865  l format for the
+00001460: 2067 6976 656e 2063 6f6c 756d 6e0a 0a20   given column.. 
+00001470: 2020 203a 7061 7261 6d20 636f 6c75 6d6e     :param column
+00001480: 5f64 6963 743a 2054 6865 2063 6f6c 756d  _dict: The colum
+00001490: 6e20 6461 7461 7320 636f 6c6c 6563 7465  n datas collecte
+000014a0: 6420 6475 7269 6e67 2069 6e73 7065 6374  d during inspect
+000014b0: 696f 6e0a 2020 2020 3a70 6172 616d 206b  ion.    :param k
+000014c0: 6579 3a20 5468 6520 6578 706f 7274 6174  ey: The exportat
+000014d0: 696f 6e20 6b65 790a 2020 2020 7242 0000  ion key.    rB..
+000014e0: 00da 075f 5f63 6f6c 5f5f 4eda 0763 6f6c  ...__col__N..col
+000014f0: 756d 6e73 7201 0000 00da 0469 6d70 6c29  umnsr......impl)
+00001500: 0772 3000 0000 721e 0000 0072 5100 0000  .r0...r....rQ...
+00001510: 722c 0000 00da 0474 7970 65da 0f46 4f52  r,.....type..FOR
+00001520: 4d41 545f 5245 4749 5354 5259 da08 6765  MAT_REGISTRY..ge
+00001530: 745f 6974 656d 2906 da0b 636f 6c75 6d6e  t_item)...column
+00001540: 5f64 6963 7472 4800 0000 7242 0000 00da  _dictrH...rB....
+00001550: 0470 726f 70da 0b73 716c 615f 636f 6c75  .prop..sqla_colu
+00001560: 6d6e da0b 636f 6c75 6d6e 5f74 7970 6572  mn..column_typer
+00001570: 0b00 0000 720b 0000 0072 0c00 0000 723f  ....r....r....r?
+00001580: 0000 00cb 0000 0073 1000 0000 0007 0a01  .......s........
+00001590: 0a02 1001 0a01 0a01 1001 0a01 723f 0000  ............r?..
+000015a0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+000015b0: 0000 0300 0000 4000 0000 7336 0000 0065  ......@...s6...e
+000015c0: 005a 0164 005a 0264 015a 0364 025a 0464  .Z.d.Z.d.Z.d.Z.d
+000015d0: 0d64 0564 0684 015a 0564 0764 0884 005a  .d.d...Z.d.d...Z
+000015e0: 0664 0964 0a84 005a 0764 0b64 0c84 005a  .d.d...Z.d.d...Z
+000015f0: 0864 0453 0029 0eda 0f53 716c 6158 6c73  .d.S.)...SqlaXls
+00001600: 4578 706f 7274 6572 617a 0300 000a 2020  Exporteraz....  
+00001610: 2020 4d61 696e 2063 6c61 7373 2075 7365    Main class use
+00001620: 6420 666f 7220 6578 706f 7274 696e 6720  d for exporting 
+00001630: 6461 7461 7320 746f 2074 6865 2078 6c73  datas to the xls
+00001640: 2066 6f72 6d61 740a 0a20 2020 204d 6f64   format..    Mod
+00001650: 656c 7320 6174 7472 6962 7574 6573 206f  els attributes o
+00001660: 7574 7075 7420 6361 6e20 6265 2063 7573  utput can be cus
+00001670: 746f 6d69 7a65 6420 7468 726f 7567 6820  tomized through 
+00001680: 7468 6520 696e 666f 2070 6172 616d 203a  the info param :
+00001690: 0a0a 2020 2020 2020 2020 436f 6c75 6d6e  ..        Column
+000016a0: 2849 6e74 6567 6572 2c20 696e 666f 733d  (Integer, infos=
+000016b0: 7b27 6578 706f 7274 273a 0a20 2020 2020  {'export':.     
+000016c0: 2020 2020 2020 207b 2765 7863 656c 273a         {'excel':
+000016d0: 3c65 7863 656c 5f73 7065 6369 6669 635f  <excel_specific_
+000016e0: 6f70 7469 6f6e 733e 2c0a 2020 2020 2020  options>,.      
+000016f0: 2020 2020 2020 203c 6d61 696e 5f65 7870         <main_exp
+00001700: 6f72 745f 6f70 7469 6f6e 733e 0a20 2020  ort_options>.   
+00001710: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+00001720: 2020 207d 0a0a 2020 2020 6d61 696e 5f65     }..    main_e
+00001730: 7870 6f72 745f 6f70 7469 6f6e 7320 616e  xport_options an
+00001740: 6420 6578 6365 6c5f 7370 6563 6966 6963  d excel_specific
+00001750: 5f6f 7074 696f 6e73 2063 616e 2062 6520  _options can be 
+00001760: 3a0a 0a20 2020 2020 2020 206c 6162 656c  :..        label
+00001770: 0a0a 2020 2020 2020 2020 2020 2020 6c61  ..            la
+00001780: 6265 6c20 6f66 2074 6865 2063 6f6c 756d  bel of the colum
+00001790: 6e20 6865 6164 6572 0a0a 2020 2020 2020  n header..      
+000017a0: 2020 666f 726d 6174 0a0a 2020 2020 2020    format..      
+000017b0: 2020 2020 2020 6120 6675 6e63 7469 6f6e        a function
+000017c0: 2074 6861 7420 7769 6c6c 2062 6520 6669   that will be fi
+000017d0: 7265 6420 6f6e 2065 6163 6820 726f 7720  red on each row 
+000017e0: 746f 2066 6f72 6d61 7420 7468 6520 6f75  to format the ou
+000017f0: 7470 7574 0a0a 2020 2020 2020 2020 7265  tput..        re
+00001800: 6c61 7465 645f 6b65 790a 0a20 2020 2020  lated_key..     
+00001810: 2020 2020 2020 2049 6620 7468 6520 6174         If the at
+00001820: 7472 6962 7574 6520 6973 2061 2072 656c  tribute is a rel
+00001830: 6174 696f 6e73 6869 702c 2074 6865 2076  ationship, the v
+00001840: 616c 7565 206f 6620 7468 6520 6769 7665  alue of the give
+00001850: 6e20 6174 7472 6962 7574 650a 2020 2020  n attribute.    
+00001860: 2020 2020 2020 2020 6f66 2074 6865 2072          of the r
+00001870: 656c 6174 6564 206f 626a 6563 7420 7769  elated object wi
+00001880: 6c6c 2062 6520 7573 6564 2074 6f20 6669  ll be used to fi
+00001890: 6c6c 2074 6865 2063 656c 6c73 0a0a 2020  ll the cells..  
+000018a0: 2020 2020 2020 6578 636c 7564 650a 0a20        exclude.. 
+000018b0: 2020 2020 2020 2020 2020 2054 6869 7320             This 
+000018c0: 6461 7461 2077 696c 6c20 6e6f 7420 6265  data will not be
+000018d0: 2069 6e73 6572 7465 6420 696e 2074 6865   inserted in the
+000018e0: 2065 7870 6f72 7420 6966 2054 7275 650a   export if True.
+000018f0: 0a20 2020 2055 7361 6765 3a0a 0a20 2020  .    Usage:..   
+00001900: 2020 2020 2061 203d 2053 716c 6158 6c73       a = SqlaXls
+00001910: 4578 706f 7274 6572 284d 794d 6f64 656c  Exporter(MyModel
+00001920: 290a 2020 2020 2020 2020 666f 7220 6920  ).        for i 
+00001930: 696e 204d 794d 6f64 656c 2e71 7565 7279  in MyModel.query
+00001940: 2829 2e66 696c 7465 7228 3c6d 7966 696c  ().filter(<myfil
+00001950: 7465 723e 293a 0a20 2020 2020 2020 2020  ter>):.         
+00001960: 2020 2061 2e61 6464 5f72 6f77 2869 290a     a.add_row(i).
+00001970: 2020 2020 2020 2020 612e 7265 6e64 6572          a.render
+00001980: 2829 0a20 2020 2072 2100 0000 544e 6304  ().    r!...TNc.
+00001990: 0000 0000 0000 0000 0000 0005 0000 0005  ................
+000019a0: 0000 004b 0000 0073 4200 0000 7c02 7c00  ...K...sB...|.|.
+000019b0: 5f00 7c03 6400 7500 7c00 5f01 7402 6a03  _.|.d.u.|._.t.j.
+000019c0: 7c00 6601 7c02 7c03 6401 9c02 7c04 a401  |.f.|.|.d...|...
+000019d0: 8e01 0100 7404 6a03 7c00 6601 6402 7c01  ....t.j.|.f.d.|.
+000019e0: 6901 7c04 a401 8e01 0100 6400 5300 2903  i.|.......d.S.).
+000019f0: 4e29 02da 0b67 7565 7373 5f74 7970 6573  N)...guess_types
+00001a00: 7214 0000 00da 056d 6f64 656c 2905 725b  r......model).r[
+00001a10: 0000 00da 0769 735f 726f 6f74 720f 0000  .....is_rootr...
+00001a20: 0072 1a00 0000 7206 0000 0029 0572 1800  .r....r....).r..
+00001a30: 0000 725c 0000 0072 5b00 0000 7214 0000  ..r\...r[...r...
+00001a40: 0072 1900 0000 720b 0000 0072 0b00 0000  .r....r....r....
+00001a50: 720c 0000 0072 1a00 0000 0601 0000 7308  r....r........s.
+00001a60: 0000 0000 0106 010a 0118 017a 1853 716c  ...........z.Sql
+00001a70: 6158 6c73 4578 706f 7274 6572 2e5f 5f69  aXlsExporter.__i
+00001a80: 6e69 745f 5f63 0300 0000 0000 0000 0000  nit__c..........
+00001a90: 0000 0500 0000 0500 0000 4300 0000 7342  ..........C...sB
+00001aa0: 0000 007c 02a0 0064 01a1 017d 037c 0364  ...|...d...}.|.d
+00001ab0: 0275 0072 3e7c 006a 016a 027c 02a0 0064  .u.r>|.j.j.|...d
+00001ac0: 0364 04a1 0264 058d 017d 0474 037c 016a  .d...d...}.t.|.j
+00001ad0: 047c 0464 068d 0204 007d 037c 0264 013c  .|.d.....}.|.d.<
+00001ae0: 007c 0353 0029 077a 7f0a 2020 2020 2020  .|.S.).z..      
+00001af0: 2020 7265 7475 726e 7320 616e 2053 716c    returns an Sql
+00001b00: 6158 6c73 4578 706f 7274 6572 2066 6f72  aXlsExporter for
+00001b10: 2074 6865 2067 6976 656e 2072 656c 6174   the given relat
+00001b20: 6564 206f 626a 6563 7420 616e 6420 7374  ed object and st
+00001b30: 6f72 6573 2069 740a 2020 2020 2020 2020  ores it.        
+00001b40: 696e 2074 6865 2063 6f6c 756d 6e20 6f62  in the column ob
+00001b50: 6a65 6374 2061 7320 6120 6361 6368 650a  ject as a cache.
+00001b60: 2020 2020 2020 2020 da11 7371 6c61 5f78          ..sqla_x
+00001b70: 6c73 5f65 7870 6f72 7465 724e 7243 0000  ls_exporterNrC..
+00001b80: 007a 0d64 6566 6175 6c74 2074 6974 6c65  .z.default title
+00001b90: 2901 7215 0000 0029 0172 1400 0000 2905  ).r....).r....).
+00001ba0: 7230 0000 0072 1200 0000 5a0c 6372 6561  r0...r....Z.crea
+00001bb0: 7465 5f73 6865 6574 725a 0000 00da 095f  te_sheetrZ....._
+00001bc0: 5f63 6c61 7373 5f5f 2905 7218 0000 00da  _class__).r.....
+00001bd0: 0b72 656c 6174 6564 5f6f 626a 7234 0000  .related_objr4..
+00001be0: 00da 0672 6573 756c 7472 1400 0000 720b  ...resultr....r.
+00001bf0: 0000 0072 0b00 0000 720c 0000 00da 155f  ...r....r......_
+00001c00: 6765 745f 7265 6c61 7465 645f 6578 706f  get_related_expo
+00001c10: 7274 6572 0c01 0000 7312 0000 0000 050a  rter....s.......
+00001c20: 0108 0106 010a ff06 0302 0106 ff0e 037a  ...............z
+00001c30: 2553 716c 6158 6c73 4578 706f 7274 6572  %SqlaXlsExporter
+00001c40: 2e5f 6765 745f 7265 6c61 7465 645f 6578  ._get_related_ex
+00001c50: 706f 7274 6572 6303 0000 0000 0000 0000  porterc.........
+00001c60: 0000 0009 0000 0005 0000 0043 0000 0073  ...........C...s
+00001c70: 7e00 0000 7400 a001 7c00 7c01 7c02 a103  ~...t...|.|.|...
+00001c80: 7d03 7c03 6401 6b02 727a 7c02 a002 6402  }.|.d.k.rz|...d.
+00001c90: 6403 a102 7d04 7c02 6404 1900 6a03 727a  d...}.|.d...j.rz
+00001ca0: 7c04 6403 7500 727a 7c00 6a04 727a 7c02  |.d.u.rz|.j.rz|.
+00001cb0: 6405 1900 7d05 7405 7c01 7c05 6403 8303  d...}.t.|.|.d...
+00001cc0: 7d06 7c06 7356 6401 5300 7c00 a006 7c06  }.|.sVd.S.|...|.
+00001cd0: 6406 1900 7c02 a102 7d07 7c06 4400 5d0e  d...|...}.|.D.].
+00001ce0: 7d08 7c07 a007 7c08 a101 0100 716a 7c03  }.|...|.....qj|.
+00001cf0: 5300 2907 7a86 0a20 2020 2020 2020 2052  S.).z..        R
+00001d00: 6574 7572 6e20 7468 6520 7661 6c75 6520  eturn the value 
+00001d10: 746f 2069 6e73 6572 7420 696e 2061 2072  to insert in a r
+00001d20: 656c 6174 696f 6e73 6869 7020 6365 6c6c  elationship cell
+00001d30: 0a20 2020 2020 2020 2048 616e 646c 6520  .        Handle 
+00001d40: 7468 6520 6361 7365 206f 6620 636f 6d70  the case of comp
+00001d50: 6c65 7820 7265 6c61 7465 6420 6461 7461  lex related data
+00001d60: 7320 7765 2077 616e 7420 746f 2068 616e  s we want to han
+00001d70: 646c 650a 2020 2020 2020 2020 7208 0000  dle.        r...
+00001d80: 00da 0b72 656c 6174 6564 5f6b 6579 4e72  ...related_keyNr
+00001d90: 5000 0000 7248 0000 0072 0100 0000 2908  P...rH...r....).
+00001da0: 7206 0000 00da 1a5f 6765 745f 7265 6c61  r......_get_rela
+00001db0: 7469 6f6e 7368 6970 5f63 656c 6c5f 7661  tionship_cell_va
+00001dc0: 6c72 3000 0000 da07 7573 656c 6973 7472  lr0.....uselistr
+00001dd0: 5d00 0000 722c 0000 0072 6200 0000 da07  ]...r,...rb.....
+00001de0: 6164 645f 726f 7729 0972 1800 0000 da03  add_row).r......
+00001df0: 6f62 6a72 3400 0000 da03 7661 6c72 6300  objr4.....valrc.
+00001e00: 0000 7248 0000 005a 0f72 656c 6174 6564  ..rH...Z.related
+00001e10: 5f6f 626a 6563 7473 5a08 6578 706f 7274  _objectsZ.export
+00001e20: 6572 da07 7265 6c5f 6f62 6a72 0b00 0000  er..rel_objr....
+00001e30: 720b 0000 0072 0c00 0000 7264 0000 001b  r....r....rd....
+00001e40: 0100 0073 1e00 0000 0005 0e01 0801 0c02  ...s............
+00001e50: 1803 0801 0c01 0401 0402 0401 0601 02fe  ................
+00001e60: 0404 0801 0c02 7a2a 5371 6c61 586c 7345  ......z*SqlaXlsE
+00001e70: 7870 6f72 7465 722e 5f67 6574 5f72 656c  xporter._get_rel
+00001e80: 6174 696f 6e73 6869 705f 6365 6c6c 5f76  ationship_cell_v
+00001e90: 616c 6301 0000 0000 0000 0000 0000 0002  alc.............
+00001ea0: 0000 0003 0000 0043 0000 0073 2e00 0000  .......C...s....
+00001eb0: 7400 a001 7c00 a101 0100 7c00 6a02 4400  t...|.....|.j.D.
+00001ec0: 5d18 7d01 6401 7c01 7600 7210 7c01 6401  ].}.d.|.v.r.|.d.
+00001ed0: 1900 a001 a100 0100 7110 6402 5300 2903  ........q.d.S.).
+00001ee0: 7a52 0a20 2020 2020 2020 2045 6e68 616e  zR.        Enhan
+00001ef0: 6365 2074 6865 2064 6566 6175 6c74 2070  ce the default p
+00001f00: 6f70 756c 6174 6520 7363 7269 7074 2062  opulate script b
+00001f10: 7920 6861 6e64 6c69 6e67 2072 656c 6174  y handling relat
+00001f20: 6564 2065 6c65 6d65 6e74 730a 2020 2020  ed elements.    
+00001f30: 2020 2020 725e 0000 004e 2903 720f 0000      r^...N).r...
+00001f40: 0072 3800 0000 722e 0000 0029 0272 1800  .r8...r....).r..
+00001f50: 0000 7241 0000 0072 0b00 0000 720b 0000  ..rA...r....r...
+00001f60: 0072 0c00 0000 7238 0000 0035 0100 0073  .r....r8...5...s
+00001f70: 0800 0000 0004 0a01 0a01 0801 7a19 5371  ............z.Sq
+00001f80: 6c61 586c 7345 7870 6f72 7465 722e 5f70  laXlsExporter._p
+00001f90: 6f70 756c 6174 6529 0254 4e29 0972 4b00  opulate).TN).rK.
+00001fa0: 0000 724c 0000 0072 4d00 0000 724e 0000  ..rL...rM...rN..
+00001fb0: 00da 0a63 6f6e 6669 675f 6b65 7972 1a00  ...config_keyr..
+00001fc0: 0000 7262 0000 0072 6400 0000 7238 0000  ..rb...rd...r8..
+00001fd0: 0072 0b00 0000 720b 0000 0072 0b00 0000  .r....r....r....
+00001fe0: 720c 0000 0072 5a00 0000 dd00 0000 730c  r....rZ.......s.
+00001ff0: 0000 0008 0104 2604 020a 0608 0f08 1a72  ......&........r
+00002000: 5a00 0000 6300 0000 0000 0000 0000 0000  Z...c...........
+00002010: 0000 0000 0003 0000 0040 0000 0073 1e00  .........@...s..
+00002020: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
+00002030: 5a04 6407 6404 6405 8401 5a05 6406 5300  Z.d.d.d...Z.d.S.
+00002040: 2908 da0b 586c 7345 7870 6f72 7465 727a  )...XlsExporterz
+00002050: bc0a 2020 2020 4120 6d61 696e 2078 6c73  ..    A main xls
+00002060: 2065 7870 6f72 7461 7469 6f6e 2074 6f6f   exportation too
+00002070: 6c20 2877 6974 686f 7574 2073 716c 616c  l (without sqlal
+00002080: 6368 656d 7920 7375 7070 6f72 7429 0a0a  chemy support)..
+00002090: 2020 2020 7772 6974 6572 203d 204d 7958      writer = MyX
+000020a0: 6c73 4578 706f 7274 6572 2829 0a20 2020  lsExporter().   
+000020b0: 2077 7269 7465 722e 6164 645f 726f 7728   writer.add_row(
+000020c0: 7b27 6b65 7927 3a20 7527 4c61 2076 616c  {'key': u'La val
+000020d0: 6575 7220 6465 206c 6120 6365 6c6c 756c  eur de la cellul
+000020e0: 6520 6465 206c 6120 636f 6c6f 6e6e 6520  e de la colonne 
+000020f0: 3127 7d29 0a20 2020 2077 7269 7465 722e  1'}).    writer.
+00002100: 7265 6e64 6572 2829 0a20 2020 2072 0b00  render().    r..
+00002110: 0000 5463 0200 0000 0000 0000 0000 0000  ..Tc............
+00002120: 0300 0000 0400 0000 4b00 0000 732c 0000  ........K...s,..
+00002130: 0074 006a 017c 0066 0164 017c 0169 017c  .t.j.|.f.d.|.i.|
+00002140: 02a4 018e 0101 0074 026a 017c 0066 0169  .......t.j.|.f.i
+00002150: 007c 02a4 018e 0101 0064 0053 0029 024e  .|.......d.S.).N
+00002160: 725b 0000 0029 0372 0f00 0000 721a 0000  r[...).r....r...
+00002170: 0072 0500 0000 2903 7218 0000 0072 5b00  .r....).r....r[.
+00002180: 0000 7219 0000 0072 0b00 0000 720b 0000  ..r....r....r...
+00002190: 0072 0c00 0000 721a 0000 004a 0100 0073  .r....r....J...s
+000021a0: 0400 0000 0001 1601 7a14 586c 7345 7870  ........z.XlsExp
+000021b0: 6f72 7465 722e 5f5f 696e 6974 5f5f 4e29  orter.__init__N)
+000021c0: 0154 2906 724b 0000 0072 4c00 0000 724d  .T).rK...rL...rM
+000021d0: 0000 0072 4e00 0000 722e 0000 0072 1a00  ...rN...r....r..
+000021e0: 0000 720b 0000 0072 0b00 0000 720b 0000  ..r....r....r...
+000021f0: 0072 0c00 0000 726b 0000 003f 0100 0073  .r....rk...?...s
+00002200: 0600 0000 0801 0408 0402 726b 0000 0029  ..........rk...)
+00002210: 014e 2921 724e 0000 00da 0862 7569 6c74  .N)!rN.....built
+00002220: 696e 73da 0c40 7079 5f62 7569 6c74 696e  ins..@py_builtin
+00002230: 73da 195f 7079 7465 7374 2e61 7373 6572  s.._pytest.asser
+00002240: 7469 6f6e 2e72 6577 7269 7465 da09 6173  tion.rewrite..as
+00002250: 7365 7274 696f 6eda 0772 6577 7269 7465  sertion..rewrite
+00002260: da0a 4070 7974 6573 745f 6172 da09 6974  ..@pytest_ar..it
+00002270: 6572 746f 6f6c 73da 076c 6f67 6769 6e67  ertools..logging
+00002280: 7211 0000 005a 0f6f 7065 6e70 7978 6c2e  r....Z.openpyxl.
+00002290: 7374 796c 6573 7202 0000 0072 0300 0000  stylesr....r....
+000022a0: 721c 0000 00da 0673 7472 696e 6772 0400  r......stringr..
+000022b0: 0000 da13 7371 6c61 5f69 6e73 7065 6374  ....sqla_inspect
+000022c0: 2e65 7870 6f72 7472 0500 0000 7206 0000  .exportr....r...
+000022d0: 005a 1173 716c 615f 696e 7370 6563 742e  .Z.sqla_inspect.
+000022e0: 6261 7365 7207 0000 00da 0967 6574 4c6f  baser......getLo
+000022f0: 6767 6572 724b 0000 00da 036c 6f67 da04  ggerrK.....log..
+00002300: 6c69 7374 da1d 636f 6d62 696e 6174 696f  list..combinatio
+00002310: 6e73 5f77 6974 685f 7265 706c 6163 656d  ns_with_replacem
+00002320: 656e 745a 0f41 5343 4949 5f55 5050 4552  entZ.ASCII_UPPER
+00002330: 4341 5345 7254 0000 00da 066f 626a 6563  CASErT.....objec
+00002340: 7472 0f00 0000 723f 0000 0072 5a00 0000  tr....r?...rZ...
+00002350: 726b 0000 0072 0b00 0000 720b 0000 0072  rk...r....r....r
+00002360: 0b00 0000 720c 0000 00da 083c 6d6f 6475  ....r......<modu
+00002370: 6c65 3e06 0000 0073 2400 0000 0404 2201  le>....s$.....".
+00002380: 0801 0801 1005 0801 0c02 1004 0c03 0a04  ................
+00002390: 0e02 0afe 0a06 0603 107f 0023 0a12 1262  ...........#...b
```

### Comparing `sqla_inspect-0.7.4/sqla_inspect/__pycache__/export.cpython-37-pytest-6.2.1.pyc` & `sqla_inspect-0.7.5/sqla_inspect/__pycache__/export.cpython-37-pytest-6.2.1.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/__pycache__/export.cpython-37.pyc` & `sqla_inspect-0.7.5/sqla_inspect/__pycache__/export.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/__pycache__/export.cpython-38.pyc` & `sqla_inspect-0.7.5/sqla_inspect/__pycache__/export.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/__pycache__/export.cpython-39-pytest-6.2.5.pyc` & `sqla_inspect-0.7.5/sqla_inspect/__pycache__/export.cpython-39-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/__pycache__/export.cpython-39.pyc` & `sqla_inspect-0.7.5/sqla_inspect/__pycache__/export.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/__pycache__/ods.cpython-37-pytest-6.2.1.pyc` & `sqla_inspect-0.7.5/sqla_inspect/__pycache__/ods.cpython-37-pytest-6.2.1.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/__pycache__/ods.cpython-37.pyc` & `sqla_inspect-0.7.5/sqla_inspect/__pycache__/ods.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/__pycache__/ods.cpython-38.pyc` & `sqla_inspect-0.7.5/sqla_inspect/__pycache__/ods.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/__pycache__/ods.cpython-39-pytest-6.2.5.pyc` & `sqla_inspect-0.7.5/sqla_inspect/__pycache__/ods.cpython-39-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/__pycache__/ods.cpython-39.pyc` & `sqla_inspect-0.7.5/sqla_inspect/__pycache__/ods.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/__pycache__/py3o.cpython-37.pyc` & `sqla_inspect-0.7.5/sqla_inspect/__pycache__/py3o.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/__pycache__/py3o.cpython-38.pyc` & `sqla_inspect-0.7.5/sqla_inspect/__pycache__/py3o.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/__pycache__/py3o.cpython-39-pytest-6.2.5.pyc` & `sqla_inspect-0.7.5/sqla_inspect/__pycache__/py3o.cpython-39-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/__pycache__/py3o.cpython-39.pyc` & `sqla_inspect-0.7.5/sqla_inspect/__pycache__/py3o.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/__pycache__/py3o_tmpl.cpython-37.pyc` & `sqla_inspect-0.7.5/sqla_inspect/__pycache__/py3o_tmpl.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/__pycache__/py3o_tmpl.cpython-38.pyc` & `sqla_inspect-0.7.5/sqla_inspect/__pycache__/py3o_tmpl.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/__pycache__/py3o_tmpl.cpython-39-pytest-6.2.5.pyc` & `sqla_inspect-0.7.5/sqla_inspect/__pycache__/py3o_tmpl.cpython-39-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/__pycache__/py3o_tmpl.cpython-39.pyc` & `sqla_inspect-0.7.5/sqla_inspect/__pycache__/py3o_tmpl.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/ascii.py` & `sqla_inspect-0.7.5/sqla_inspect/ascii.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 def force_utf8(value):
     """
     return a utf-8 byte string
 
     :param str value:
     :rtype: bytes
     """
-    return force_encoding(value, 'utf-8')
+    return force_encoding(value, "utf-8")
 
 
 def force_encoding(value, encoding):
     """
     :rtype: bytes
     """
     if not isinstance(value, (str, bytes)):
```

### Comparing `sqla_inspect-0.7.4/sqla_inspect/base.py` & `sqla_inspect-0.7.5/sqla_inspect/base.py`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/csv.py` & `sqla_inspect-0.7.5/sqla_inspect/csv.py`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/excel.py` & `sqla_inspect-0.7.5/sqla_inspect/excel.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,21 @@
         Return a file buffer containing the resulting xls
 
         :param obj f_buf: A file buffer supporting the write and seek
         methods
         """
         if f_buf is None:
             f_buf = io.BytesIO()
-        f_buf.write(openpyxl.writer.excel.save_virtual_workbook(self.book))
+
+        if hasattr(self.book, "save"):
+            self.book.save(f_buf)
+        # older versions of openpyxl
+        else:
+            f_buf.write(openpyxl.writer.excel.save_virtual_workbook(self.book))
+
         f_buf.seek(0)
         return f_buf
 
     def set_color(self, cell, color):
         """
         Set the given color to the provided cell
 
@@ -156,14 +162,15 @@
                         cell.number_format = format
 
     def _render_headers(self):
         """
         Write the headers row
         """
         headers = getattr(self, "headers", ())
+        index = 0
         for index, col in enumerate(headers):
             # We write the headers
             cell = self.worksheet.cell(row=1, column=index + 1)
             cell.value = col["label"]
 
         index += 1
```

### Comparing `sqla_inspect-0.7.4/sqla_inspect/export.py` & `sqla_inspect-0.7.5/sqla_inspect/export.py`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/ods.py` & `sqla_inspect-0.7.5/sqla_inspect/ods.py`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/py3o.py` & `sqla_inspect-0.7.5/sqla_inspect/py3o.py`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/py3o_tmpl.py` & `sqla_inspect-0.7.5/sqla_inspect/py3o_tmpl.py`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/tests/__pycache__/models.cpython-39-pytest-6.2.5.pyc` & `sqla_inspect-0.7.5/sqla_inspect/tests/__pycache__/models.cpython-39-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/tests/__pycache__/test_ascii.cpython-39-pytest-6.2.5.pyc` & `sqla_inspect-0.7.5/sqla_inspect/tests/__pycache__/test_ascii.cpython-39-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/tests/__pycache__/test_base.cpython-39-pytest-6.2.5.pyc` & `sqla_inspect-0.7.5/sqla_inspect/tests/__pycache__/test_base.cpython-39-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/tests/__pycache__/test_csv.cpython-39-pytest-6.2.5.pyc` & `sqla_inspect-0.7.5/sqla_inspect/tests/__pycache__/test_csv.cpython-39-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/tests/__pycache__/test_export.cpython-39-pytest-6.2.5.pyc` & `sqla_inspect-0.7.5/sqla_inspect/tests/__pycache__/test_export.cpython-39-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/tests/models.py` & `sqla_inspect-0.7.5/sqla_inspect/tests/models.py`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/tests/test_ascii.py` & `sqla_inspect-0.7.5/sqla_inspect/tests/test_ascii.py`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/tests/test_base.py` & `sqla_inspect-0.7.5/sqla_inspect/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/tests/test_csv.py` & `sqla_inspect-0.7.5/sqla_inspect/tests/test_csv.py`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect/tests/test_export.py` & `sqla_inspect-0.7.5/sqla_inspect/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.4/sqla_inspect.egg-info/PKG-INFO` & `sqla_inspect-0.7.5/sqla_inspect.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 Metadata-Version: 2.1
 Name: sqla-inspect
-Version: 0.7.4
+Version: 0.7.5
 Summary: Usefull tools for setting/getting datas from SQLAlchemy models
 Home-page: https://github.com/majerteam/sqla_inspect
 Author: Gaston Tjebbes - Majerti
 Author-email: tech@majerti.fr
 License: GPLv3
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Database
 License-File: LICENSE.txt
-
-UNKNOWN
-
```

### Comparing `sqla_inspect-0.7.4/sqla_inspect.egg-info/SOURCES.txt` & `sqla_inspect-0.7.5/sqla_inspect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

