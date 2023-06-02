# Comparing `tmp/alibabacloud_docmind-api20220729-1.0.0.tar.gz` & `tmp/alibabacloud_docmind-api20220729-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_docmind-api20220729-1.0.0.tar", last modified: Tue Feb  7 12:41:00 2023, max compression
+gzip compressed data, was "dist/alibabacloud_docmind-api20220729-1.0.1.tar", last modified: Fri Jun  2 08:18:14 2023, max compression
```

## Comparing `alibabacloud_docmind-api20220729-1.0.0.tar` & `alibabacloud_docmind-api20220729-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 12:41:00.000000 alibabacloud_docmind-api20220729-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      600 2023-02-07 12:40:59.000000 alibabacloud_docmind-api20220729-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-02-07 12:40:59.000000 alibabacloud_docmind-api20220729-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2376 2023-02-07 12:41:00.000000 alibabacloud_docmind-api20220729-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1046 2023-02-07 12:40:59.000000 alibabacloud_docmind-api20220729-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1131 2023-02-07 12:40:59.000000 alibabacloud_docmind-api20220729-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 12:41:00.000000 alibabacloud_docmind-api20220729-1.0.0/alibabacloud_docmind_api20220729/
--rw-r--r--   0 root         (0) root         (0)       21 2023-02-07 12:40:59.000000 alibabacloud_docmind-api20220729-1.0.0/alibabacloud_docmind_api20220729/__init__.py
--rw-r--r--   0 root         (0) root         (0)    51930 2023-02-07 12:40:59.000000 alibabacloud_docmind-api20220729-1.0.0/alibabacloud_docmind_api20220729/client.py
--rw-r--r--   0 root         (0) root         (0)    27150 2023-02-07 12:40:59.000000 alibabacloud_docmind-api20220729-1.0.0/alibabacloud_docmind_api20220729/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 12:41:00.000000 alibabacloud_docmind-api20220729-1.0.0/alibabacloud_docmind_api20220729.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2376 2023-02-07 12:41:00.000000 alibabacloud_docmind-api20220729-1.0.0/alibabacloud_docmind_api20220729.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      471 2023-02-07 12:41:00.000000 alibabacloud_docmind-api20220729-1.0.0/alibabacloud_docmind_api20220729.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-07 12:41:00.000000 alibabacloud_docmind-api20220729-1.0.0/alibabacloud_docmind_api20220729.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      315 2023-02-07 12:41:00.000000 alibabacloud_docmind-api20220729-1.0.0/alibabacloud_docmind_api20220729.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       33 2023-02-07 12:41:00.000000 alibabacloud_docmind-api20220729-1.0.0/alibabacloud_docmind_api20220729.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-02-07 12:41:00.000000 alibabacloud_docmind-api20220729-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2843 2023-02-07 12:40:59.000000 alibabacloud_docmind-api20220729-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 08:18:14.000000 alibabacloud_docmind-api20220729-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)       68 2023-06-02 08:18:14.000000 alibabacloud_docmind-api20220729-1.0.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-02 08:18:14.000000 alibabacloud_docmind-api20220729-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-02 08:18:14.000000 alibabacloud_docmind-api20220729-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2376 2023-06-02 08:18:14.000000 alibabacloud_docmind-api20220729-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1046 2023-06-02 08:18:14.000000 alibabacloud_docmind-api20220729-1.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-06-02 08:18:14.000000 alibabacloud_docmind-api20220729-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 08:18:14.000000 alibabacloud_docmind-api20220729-1.0.1/alibabacloud_docmind_api20220729/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-02 08:18:14.000000 alibabacloud_docmind-api20220729-1.0.1/alibabacloud_docmind_api20220729/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    51930 2023-06-02 08:18:14.000000 alibabacloud_docmind-api20220729-1.0.1/alibabacloud_docmind_api20220729/client.py
+-rw-r--r--   0 root         (0) root         (0)    27150 2023-06-02 08:18:14.000000 alibabacloud_docmind-api20220729-1.0.1/alibabacloud_docmind_api20220729/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 08:18:14.000000 alibabacloud_docmind-api20220729-1.0.1/alibabacloud_docmind_api20220729.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2376 2023-06-02 08:18:14.000000 alibabacloud_docmind-api20220729-1.0.1/alibabacloud_docmind_api20220729.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      484 2023-06-02 08:18:14.000000 alibabacloud_docmind-api20220729-1.0.1/alibabacloud_docmind_api20220729.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 08:18:14.000000 alibabacloud_docmind-api20220729-1.0.1/alibabacloud_docmind_api20220729.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      315 2023-06-02 08:18:14.000000 alibabacloud_docmind-api20220729-1.0.1/alibabacloud_docmind_api20220729.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-06-02 08:18:14.000000 alibabacloud_docmind-api20220729-1.0.1/alibabacloud_docmind_api20220729.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-02 08:18:14.000000 alibabacloud_docmind-api20220729-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2843 2023-06-02 08:18:14.000000 alibabacloud_docmind-api20220729-1.0.1/setup.py
```

### Comparing `alibabacloud_docmind-api20220729-1.0.0/LICENSE` & `alibabacloud_docmind-api20220729-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_docmind-api20220729-1.0.0/PKG-INFO` & `alibabacloud_docmind-api20220729-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_docmind-api20220729
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud docmind-api (20220729) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_docmind-api20220729-1.0.0/README-CN.md` & `alibabacloud_docmind-api20220729-1.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_docmind-api20220729-1.0.0/README.md` & `alibabacloud_docmind-api20220729-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_docmind-api20220729-1.0.0/alibabacloud_docmind_api20220729/client.py` & `alibabacloud_docmind-api20220729-1.0.1/alibabacloud_docmind_api20220729/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_docmind-api20220729-1.0.0/alibabacloud_docmind_api20220729/models.py` & `alibabacloud_docmind-api20220729-1.0.1/alibabacloud_docmind_api20220729/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_docmind-api20220729-1.0.0/alibabacloud_docmind_api20220729.egg-info/PKG-INFO` & `alibabacloud_docmind-api20220729-1.0.1/alibabacloud_docmind_api20220729.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-docmind-api20220729
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud docmind-api (20220729) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_docmind-api20220729-1.0.0/setup.py` & `alibabacloud_docmind-api20220729-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_docmind-api20220729.
 
-Created on 07/02/2023
+Created on 02/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_docmind_api20220729"
 NAME = "alibabacloud_docmind-api20220729" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud docmind-api (20220729) SDK Library for Python"
@@ -38,15 +38,15 @@
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_tea_util>=0.3.8, <1.0.0",
     "alibabacloud_oss_sdk>=0.1.0, <1.0.0",
     "alibabacloud_openplatform20191219>=2.0.0, <3.0.0",
     "alibabacloud_oss_util>=0.0.5, <1.0.0",
     "alibabacloud_tea_fileform>=0.0.3, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.7, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
```

