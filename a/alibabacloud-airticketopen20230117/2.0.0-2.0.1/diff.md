# Comparing `tmp/alibabacloud_airticketopen20230117-2.0.0.tar.gz` & `tmp/alibabacloud_airticketopen20230117-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_airticketopen20230117-2.0.0.tar", last modified: Thu Jun  1 04:11:37 2023, max compression
+gzip compressed data, was "dist/alibabacloud_airticketopen20230117-2.0.1.tar", last modified: Fri Jun  2 02:10:04 2023, max compression
```

## Comparing `alibabacloud_airticketopen20230117-2.0.0.tar` & `alibabacloud_airticketopen20230117-2.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 04:11:37.000000 alibabacloud_airticketopen20230117-2.0.0/
--rw-r--r--   0 root         (0) root         (0)      152 2023-06-01 04:11:37.000000 alibabacloud_airticketopen20230117-2.0.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-06-01 04:11:37.000000 alibabacloud_airticketopen20230117-2.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-01 04:11:37.000000 alibabacloud_airticketopen20230117-2.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2388 2023-06-01 04:11:37.000000 alibabacloud_airticketopen20230117-2.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-01 04:11:37.000000 alibabacloud_airticketopen20230117-2.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1137 2023-06-01 04:11:37.000000 alibabacloud_airticketopen20230117-2.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 04:11:37.000000 alibabacloud_airticketopen20230117-2.0.0/alibabacloud_airticketopen20230117/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-01 04:11:37.000000 alibabacloud_airticketopen20230117-2.0.0/alibabacloud_airticketopen20230117/__init__.py
--rw-r--r--   0 root         (0) root         (0)   104846 2023-06-01 04:11:37.000000 alibabacloud_airticketopen20230117-2.0.0/alibabacloud_airticketopen20230117/client.py
--rw-r--r--   0 root         (0) root         (0)   506226 2023-06-01 04:11:37.000000 alibabacloud_airticketopen20230117-2.0.0/alibabacloud_airticketopen20230117/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 04:11:37.000000 alibabacloud_airticketopen20230117-2.0.0/alibabacloud_airticketopen20230117.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2388 2023-06-01 04:11:37.000000 alibabacloud_airticketopen20230117-2.0.0/alibabacloud_airticketopen20230117.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      500 2023-06-01 04:11:37.000000 alibabacloud_airticketopen20230117-2.0.0/alibabacloud_airticketopen20230117.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 04:11:37.000000 alibabacloud_airticketopen20230117-2.0.0/alibabacloud_airticketopen20230117.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-06-01 04:11:37.000000 alibabacloud_airticketopen20230117-2.0.0/alibabacloud_airticketopen20230117.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       35 2023-06-01 04:11:37.000000 alibabacloud_airticketopen20230117-2.0.0/alibabacloud_airticketopen20230117.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-01 04:11:37.000000 alibabacloud_airticketopen20230117-2.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2660 2023-06-01 04:11:37.000000 alibabacloud_airticketopen20230117-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 02:10:04.000000 alibabacloud_airticketopen20230117-2.0.1/
+-rw-r--r--   0 root         (0) root         (0)      228 2023-06-02 02:10:03.000000 alibabacloud_airticketopen20230117-2.0.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-02 02:10:03.000000 alibabacloud_airticketopen20230117-2.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-02 02:10:03.000000 alibabacloud_airticketopen20230117-2.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2388 2023-06-02 02:10:04.000000 alibabacloud_airticketopen20230117-2.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-06-02 02:10:03.000000 alibabacloud_airticketopen20230117-2.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1137 2023-06-02 02:10:03.000000 alibabacloud_airticketopen20230117-2.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 02:10:04.000000 alibabacloud_airticketopen20230117-2.0.1/alibabacloud_airticketopen20230117/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-02 02:10:03.000000 alibabacloud_airticketopen20230117-2.0.1/alibabacloud_airticketopen20230117/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   104846 2023-06-02 02:10:03.000000 alibabacloud_airticketopen20230117-2.0.1/alibabacloud_airticketopen20230117/client.py
+-rw-r--r--   0 root         (0) root         (0)   506516 2023-06-02 02:10:03.000000 alibabacloud_airticketopen20230117-2.0.1/alibabacloud_airticketopen20230117/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 02:10:04.000000 alibabacloud_airticketopen20230117-2.0.1/alibabacloud_airticketopen20230117.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2388 2023-06-02 02:10:03.000000 alibabacloud_airticketopen20230117-2.0.1/alibabacloud_airticketopen20230117.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      500 2023-06-02 02:10:03.000000 alibabacloud_airticketopen20230117-2.0.1/alibabacloud_airticketopen20230117.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 02:10:03.000000 alibabacloud_airticketopen20230117-2.0.1/alibabacloud_airticketopen20230117.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-06-02 02:10:03.000000 alibabacloud_airticketopen20230117-2.0.1/alibabacloud_airticketopen20230117.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-06-02 02:10:03.000000 alibabacloud_airticketopen20230117-2.0.1/alibabacloud_airticketopen20230117.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-02 02:10:04.000000 alibabacloud_airticketopen20230117-2.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2660 2023-06-02 02:10:03.000000 alibabacloud_airticketopen20230117-2.0.1/setup.py
```

### Comparing `alibabacloud_airticketopen20230117-2.0.0/LICENSE` & `alibabacloud_airticketopen20230117-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_airticketopen20230117-2.0.0/PKG-INFO` & `alibabacloud_airticketopen20230117-2.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_airticketopen20230117
-Version: 2.0.0
+Version: 2.0.1
 Summary: Alibaba Cloud airticketOpen (20230117) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_airticketopen20230117-2.0.0/README-CN.md` & `alibabacloud_airticketopen20230117-2.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_airticketopen20230117-2.0.0/README.md` & `alibabacloud_airticketopen20230117-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_airticketopen20230117-2.0.0/alibabacloud_airticketopen20230117/client.py` & `alibabacloud_airticketopen20230117-2.0.1/alibabacloud_airticketopen20230117/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_airticketopen20230117-2.0.0/alibabacloud_airticketopen20230117/models.py` & `alibabacloud_airticketopen20230117-2.0.1/alibabacloud_airticketopen20230117/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2963,26 +2963,28 @@
         arrival_airport: str = None,
         arrival_city: str = None,
         arrive_terminal: str = None,
         arrive_time: int = None,
         code_share: bool = None,
         departure_airport: str = None,
         departure_city: str = None,
+        departure_date: str = None,
         departure_terminal: str = None,
         departure_time: int = None,
         marketing_flight_no: str = None,
         operating_flight_no: str = None,
     ):
         self.arrival_airport = arrival_airport
         self.arrival_city = arrival_city
         self.arrive_terminal = arrive_terminal
         self.arrive_time = arrive_time
         self.code_share = code_share
         self.departure_airport = departure_airport
         self.departure_city = departure_city
+        self.departure_date = departure_date
         self.departure_terminal = departure_terminal
         self.departure_time = departure_time
         self.marketing_flight_no = marketing_flight_no
         self.operating_flight_no = operating_flight_no
 
     def validate(self):
         pass
@@ -3003,14 +3005,16 @@
             result['arrive_time'] = self.arrive_time
         if self.code_share is not None:
             result['code_share'] = self.code_share
         if self.departure_airport is not None:
             result['departure_airport'] = self.departure_airport
         if self.departure_city is not None:
             result['departure_city'] = self.departure_city
+        if self.departure_date is not None:
+            result['departure_date'] = self.departure_date
         if self.departure_terminal is not None:
             result['departure_terminal'] = self.departure_terminal
         if self.departure_time is not None:
             result['departure_time'] = self.departure_time
         if self.marketing_flight_no is not None:
             result['marketing_flight_no'] = self.marketing_flight_no
         if self.operating_flight_no is not None:
@@ -3029,14 +3033,16 @@
             self.arrive_time = m.get('arrive_time')
         if m.get('code_share') is not None:
             self.code_share = m.get('code_share')
         if m.get('departure_airport') is not None:
             self.departure_airport = m.get('departure_airport')
         if m.get('departure_city') is not None:
             self.departure_city = m.get('departure_city')
+        if m.get('departure_date') is not None:
+            self.departure_date = m.get('departure_date')
         if m.get('departure_terminal') is not None:
             self.departure_terminal = m.get('departure_terminal')
         if m.get('departure_time') is not None:
             self.departure_time = m.get('departure_time')
         if m.get('marketing_flight_no') is not None:
             self.marketing_flight_no = m.get('marketing_flight_no')
         if m.get('operating_flight_no') is not None:
```

### Comparing `alibabacloud_airticketopen20230117-2.0.0/alibabacloud_airticketopen20230117.egg-info/PKG-INFO` & `alibabacloud_airticketopen20230117-2.0.1/alibabacloud_airticketopen20230117.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-airticketopen20230117
-Version: 2.0.0
+Version: 2.0.1
 Summary: Alibaba Cloud airticketOpen (20230117) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_airticketopen20230117-2.0.0/setup.py` & `alibabacloud_airticketopen20230117-2.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_airticketopen20230117.
 
-Created on 01/06/2023
+Created on 02/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_airticketopen20230117"
 NAME = "alibabacloud_airticketopen20230117" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud airticketOpen (20230117) SDK Library for Python"
```

