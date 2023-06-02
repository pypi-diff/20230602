# Comparing `tmp/rongdavbaaddins-0.0.0.1.tar.gz` & `tmp/rongdavbaaddins-0.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rongdavbaaddins-0.0.0.1.tar", last modified: Thu Jun  1 01:46:02 2023, max compression
+gzip compressed data, was "rongdavbaaddins-0.0.0.2.tar", last modified: Fri Jun  2 08:20:42 2023, max compression
```

## Comparing `rongdavbaaddins-0.0.0.1.tar` & `rongdavbaaddins-0.0.0.2.tar`

### file list

```diff
@@ -1,12 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 01:46:02.599491 rongdavbaaddins-0.0.0.1/
--rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 rongdavbaaddins-0.0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 rongdavbaaddins-0.0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      397 2023-06-01 01:46:02.600489 rongdavbaaddins-0.0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 rongdavbaaddins-0.0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 01:46:02.598492 rongdavbaaddins-0.0.0.1/rongdavbaaddins.egg-info/
--rw-rw-rw-   0        0        0      397 2023-06-01 01:46:02.000000 rongdavbaaddins-0.0.0.1/rongdavbaaddins.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      208 2023-06-01 01:46:02.000000 rongdavbaaddins-0.0.0.1/rongdavbaaddins.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 01:46:02.000000 rongdavbaaddins-0.0.0.1/rongdavbaaddins.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 01:46:02.000000 rongdavbaaddins-0.0.0.1/rongdavbaaddins.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      136 2023-06-01 01:46:02.600489 rongdavbaaddins-0.0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      979 2023-06-01 01:45:49.000000 rongdavbaaddins-0.0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 08:20:42.389924 rongdavbaaddins-0.0.0.2/
+-rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 rongdavbaaddins-0.0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 rongdavbaaddins-0.0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      397 2023-06-02 08:20:42.389924 rongdavbaaddins-0.0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 rongdavbaaddins-0.0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 08:20:42.329888 rongdavbaaddins-0.0.0.2/rongdavbaaddins/
+-rw-rw-rw-   0        0        0    15227 2023-06-02 06:14:22.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/Excel.officeUI
+-rw-rw-rw-   0        0        0    54784 2023-05-31 09:26:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/Vbalog.pyd
+-rw-rw-rw-   0        0        0     1041 2023-05-29 08:29:49.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/Vbalogpy.py
+-rw-rw-rw-   0        0        0        0 2023-06-01 01:46:56.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/__init__.py
+-rw-rw-rw-   0        0        0     2596 2023-06-01 06:14:19.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/getNumber.py
+-rw-rw-rw-   0        0        0      368 2023-05-31 09:29:33.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/getNumberpy.py
+-rw-rw-rw-   0        0        0     2076 2023-06-01 02:55:54.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/minusFunction.py
+drwxrwxrwx   0        0        0        0 2023-06-02 08:20:42.355890 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/
+-rw-rw-rw-   0        0        0    90081 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/__init__.py
+-rw-rw-rw-   0        0        0    30117 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/_common.py
+-rw-rw-rw-   0        0        0    15475 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/_compat.py
+-rw-rw-rw-   0        0        0    19220 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/_psaix.py
+-rw-rw-rw-   0        0        0    32696 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/_psbsd.py
+-rw-rw-rw-   0        0        0    89178 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/_pslinux.py
+-rw-rw-rw-   0        0        0    16818 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/_psosx.py
+-rw-rw-rw-   0        0        0     8477 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/_psposix.py
+-rw-rw-rw-   0        0        0    26213 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/_pssunos.py
+-rw-rw-rw-   0        0        0    78336 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/_psutil_windows.pyd
+-rw-rw-rw-   0        0        0    38545 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/_pswindows.py
+drwxrwxrwx   0        0        0        0 2023-06-02 08:20:42.387888 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/
+-rw-rw-rw-   0        0        0    61064 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/__init__.py
+-rw-rw-rw-   0        0        0      308 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/__main__.py
+-rw-rw-rw-   0        0        0    11554 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/runner.py
+-rw-rw-rw-   0        0        0     4630 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/test_aix.py
+-rw-rw-rw-   0        0        0    21638 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/test_bsd.py
+-rw-rw-rw-   0        0        0    21458 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/test_connections.py
+-rw-rw-rw-   0        0        0    28501 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/test_contracts.py
+-rw-rw-rw-   0        0        0    97598 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/test_linux.py
+-rw-rw-rw-   0        0        0    15520 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/test_memleaks.py
+-rw-rw-rw-   0        0        0    35604 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/test_misc.py
+-rw-rw-rw-   0        0        0     6791 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/test_osx.py
+-rw-rw-rw-   0        0        0    17487 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/test_posix.py
+-rw-rw-rw-   0        0        0    64702 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/test_process.py
+-rw-rw-rw-   0        0        0     1379 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/test_sunos.py
+-rw-rw-rw-   0        0        0    36812 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/test_system.py
+-rw-rw-rw-   0        0        0    15064 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/test_testutils.py
+-rw-rw-rw-   0        0        0    12576 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/test_unicode.py
+-rw-rw-rw-   0        0        0    36065 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/test_windows.py
+-rw-rw-rw-   0        0        0    10397 2023-06-02 06:35:19.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/rongdaVbaAddins.py
+-rw-rw-rw-   0        0        0    69632 2023-05-31 09:26:36.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/vbaLogin.pyd
+-rw-rw-rw-   0        0        0      156 2023-05-29 09:14:34.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/vbaloginpy.py
+-rw-rw-rw-   0        0        0    26574 2023-06-01 06:58:31.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/荣大工具箱.xlam
+drwxrwxrwx   0        0        0        0 2023-06-02 08:20:42.335885 rongdavbaaddins-0.0.0.2/rongdavbaaddins.egg-info/
+-rw-rw-rw-   0        0        0      397 2023-06-02 08:20:42.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1716 2023-06-02 08:20:42.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 08:20:42.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-02 08:20:42.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      136 2023-06-02 08:20:42.391887 rongdavbaaddins-0.0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2023-06-02 08:20:11.000000 rongdavbaaddins-0.0.0.2/setup.py
```

### Comparing `rongdavbaaddins-0.0.0.1/LICENSE.txt` & `rongdavbaaddins-0.0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.1/setup.py` & `rongdavbaaddins-0.0.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 0
 PATCH = 0
-VERSION = f"{MAJOR}.{MINOR}.{PATCH}.1"
+VERSION = f"{MAJOR}.{MINOR}.{PATCH}.2"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "rongdavbaaddins",
     version=VERSION,
@@ -26,11 +26,11 @@
     packages=find_packages(),
     # license = '',
     classifiers=[
         'Programming Language :: Python',
 
     ],
     # 包含的类型
-    package_data={'': ['*.csv', '*.txt', '.toml', "*.pyd", '*.exe', '*.db', '*.xlsm']},  # 这个很重要
+    package_data={'': ['*.csv', '*.txt', '.toml', "*.pyd", '*.exe', '*.db', '*.xlsm', '*.xlam', '*.officeUI']},  # 这个很重要
     include_package_data=True  # 也选上
 
 )
```

