# Comparing `tmp/nsedt-0.0.2.tar.gz` & `tmp/nsedt-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsedt-0.0.2.tar", last modified: Mon May 29 14:52:13 2023, max compression
+gzip compressed data, was "nsedt-0.0.3.tar", last modified: Fri Jun  2 13:56:06 2023, max compression
```

## Comparing `nsedt-0.0.2.tar` & `nsedt-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:52:13.856552 nsedt-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-29 14:51:56.000000 nsedt-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-29 14:52:13.856552 nsedt-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-29 14:51:56.000000 nsedt-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:52:13.856552 nsedt-0.0.2/nsedt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:51:56.000000 nsedt-0.0.2/nsedt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-05-29 14:51:56.000000 nsedt-0.0.2/nsedt/equity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:52:13.856552 nsedt-0.0.2/nsedt/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:51:56.000000 nsedt-0.0.2/nsedt/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-29 14:51:56.000000 nsedt-0.0.2/nsedt/resources/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:52:13.856552 nsedt-0.0.2/nsedt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-29 14:51:56.000000 nsedt-0.0.2/nsedt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-29 14:51:56.000000 nsedt-0.0.2/nsedt/utils/data_format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:52:13.856552 nsedt-0.0.2/nsedt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-29 14:52:13.000000 nsedt-0.0.2/nsedt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-29 14:52:13.000000 nsedt-0.0.2/nsedt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 14:52:13.000000 nsedt-0.0.2/nsedt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-29 14:52:13.000000 nsedt-0.0.2/nsedt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-29 14:52:13.000000 nsedt-0.0.2/nsedt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-29 14:52:13.856552 nsedt-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-29 14:51:56.000000 nsedt-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:56:06.620614 nsedt-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-02 13:55:54.000000 nsedt-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-02 13:56:06.620614 nsedt-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-02 13:55:54.000000 nsedt-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:56:06.620614 nsedt-0.0.3/nsedt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 13:55:54.000000 nsedt-0.0.3/nsedt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-06-02 13:55:54.000000 nsedt-0.0.3/nsedt/equity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:56:06.620614 nsedt-0.0.3/nsedt/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 13:55:54.000000 nsedt-0.0.3/nsedt/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-02 13:55:54.000000 nsedt-0.0.3/nsedt/resources/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:56:06.620614 nsedt-0.0.3/nsedt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-02 13:55:54.000000 nsedt-0.0.3/nsedt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-02 13:55:54.000000 nsedt-0.0.3/nsedt/utils/data_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:56:06.620614 nsedt-0.0.3/nsedt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-02 13:56:06.000000 nsedt-0.0.3/nsedt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-02 13:56:06.000000 nsedt-0.0.3/nsedt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 13:56:06.000000 nsedt-0.0.3/nsedt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-02 13:56:06.000000 nsedt-0.0.3/nsedt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-02 13:56:06.000000 nsedt-0.0.3/nsedt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-02 13:56:06.620614 nsedt-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-02 13:55:54.000000 nsedt-0.0.3/setup.py
```

### Comparing `nsedt-0.0.2/LICENSE` & `nsedt-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nsedt-0.0.2/PKG-INFO` & `nsedt-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsedt
-Version: 0.0.2
+Version: 0.0.3
 Summary: Library to collect NSE data in pandas dataframe
 Home-page: https://github.com/pratik141/nsedt
 Author: Pratik Anand
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nsedt-0.0.2/README.md` & `nsedt-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nsedt-0.0.2/nsedt/equity.py` & `nsedt-0.0.3/nsedt/equity.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 logging.basicConfig(
     level=logging.INFO,
     format=cns.log_format,
     datefmt="%m/%d/%Y %I:%M:%S %p",
 )
 
 
-def get_price(start_date, end_date, symbol=None, input_type="stock"):
+def get_price(start_date, end_date, symbol=None, input_type="stock", series="EQ"):
     """
     Create threads for different requests, parses data, combines them and returns dataframe
     Args:
         start_date (datetime.datetime): start date
         end_date (datetime.datetime): end date
         input_type (str): Either 'stock' or 'index'
         symbol (str, optional): stock symbol. Defaults to None. TODO: implement for index`
@@ -47,15 +47,15 @@
 
         if input_type == "stock":
             params = {
                 "symbol": symbol,
                 "from": st,
                 "to": et,
                 "dataType": "priceVolumeDeliverable",
-                "series": "EQ",
+                "series": series,
             }
             url = base_url + price_api + urllib.parse.urlencode(params)
             url_list.append(url)
 
         # move the window start to the next day after the current window end
         current_window_start = current_window_end + datetime.timedelta(days=1)
```

### Comparing `nsedt-0.0.2/nsedt/resources/constants.py` & `nsedt-0.0.3/nsedt/resources/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-window_size = 180
-max_workers = 5
+window_size = 50
+max_workers = 10
 log_format = """{
     "time": "%(asctime)s",
     "lineno": "%(lineno)d",
     "name": "[%(name)s]",
     "levelname": "%(levelname)s",
     "process": "%(process)s",
     "filename": "%(filename)s",
```

### Comparing `nsedt-0.0.2/nsedt/utils/__init__.py` & `nsedt-0.0.3/nsedt/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nsedt-0.0.2/nsedt/utils/data_format.py` & `nsedt-0.0.3/nsedt/utils/data_format.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
         "CH_TOT_TRADED_QTY",
         "CH_TOT_TRADED_VAL",
         "CH_52WEEK_HIGH_PRICE",
         "CH_52WEEK_LOW_PRICE",
         "VWAP",
         "COP_DELIV_QTY",
         "COP_DELIV_PERC",
+        "CH_SERIES",
     ]
     try:
         result = result[columns_required]
     except:
         return result
     result = result.set_axis(
         [
@@ -32,14 +33,15 @@
             "Total Traded Quantity",
             "Total Traded Value",
             "52 Week High Price",
             "52 Week Low Price",
             "VWAP",
             "Deliverable Volume",
             "Deliverable Percent",
+            "Series",
         ],
         axis=1,
     )
 
     result["Date"] = pd.to_datetime(result["Date"])
     result = result.sort_values("Date", ascending=True)
     result.reset_index(drop=True, inplace=True)
```

### Comparing `nsedt-0.0.2/nsedt.egg-info/PKG-INFO` & `nsedt-0.0.3/nsedt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsedt
-Version: 0.0.2
+Version: 0.0.3
 Summary: Library to collect NSE data in pandas dataframe
 Home-page: https://github.com/pratik141/nsedt
 Author: Pratik Anand
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nsedt-0.0.2/setup.py` & `nsedt-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 from setuptools import setup, find_packages
 
 setup(
     name="nsedt",
-    version="0.0.2",
+    version="0.0.3",
     author="Pratik Anand",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     description="Library to collect NSE data in pandas dataframe",
     packages=find_packages(),
     url="https://github.com/pratik141/nsedt",
     install_requires=[
```

