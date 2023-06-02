# Comparing `tmp/cs-binance-c2c-sapi-0.0.7.tar.gz` & `tmp/cs-binance-c2c-sapi-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs-binance-c2c-sapi-0.0.7.tar", last modified: Mon May 29 17:55:17 2023, max compression
+gzip compressed data, was "cs-binance-c2c-sapi-0.0.8.tar", last modified: Fri Jun  2 16:10:49 2023, max compression
```

## Comparing `cs-binance-c2c-sapi-0.0.7.tar` & `cs-binance-c2c-sapi-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:55:17.296864 cs-binance-c2c-sapi-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-29 17:55:17.296864 cs-binance-c2c-sapi-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-29 17:55:06.000000 cs-binance-c2c-sapi-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:55:17.296864 cs-binance-c2c-sapi-0.0.7/binance_c2c/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-29 17:55:06.000000 cs-binance-c2c-sapi-0.0.7/binance_c2c/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-05-29 17:55:06.000000 cs-binance-c2c-sapi-0.0.7/binance_c2c/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:55:17.296864 cs-binance-c2c-sapi-0.0.7/cs_binance_c2c_sapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-29 17:55:17.000000 cs-binance-c2c-sapi-0.0.7/cs_binance_c2c_sapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-29 17:55:17.000000 cs-binance-c2c-sapi-0.0.7/cs_binance_c2c_sapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 17:55:17.000000 cs-binance-c2c-sapi-0.0.7/cs_binance_c2c_sapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-29 17:55:17.000000 cs-binance-c2c-sapi-0.0.7/cs_binance_c2c_sapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-29 17:55:17.000000 cs-binance-c2c-sapi-0.0.7/cs_binance_c2c_sapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 17:55:17.296864 cs-binance-c2c-sapi-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-29 17:55:06.000000 cs-binance-c2c-sapi-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:10:49.618006 cs-binance-c2c-sapi-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-02 16:10:49.618006 cs-binance-c2c-sapi-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-02 16:10:36.000000 cs-binance-c2c-sapi-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:10:49.618006 cs-binance-c2c-sapi-0.0.8/binance_c2c/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-02 16:10:36.000000 cs-binance-c2c-sapi-0.0.8/binance_c2c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8309 2023-06-02 16:10:36.000000 cs-binance-c2c-sapi-0.0.8/binance_c2c/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:10:49.618006 cs-binance-c2c-sapi-0.0.8/cs_binance_c2c_sapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-02 16:10:49.000000 cs-binance-c2c-sapi-0.0.8/cs_binance_c2c_sapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-02 16:10:49.000000 cs-binance-c2c-sapi-0.0.8/cs_binance_c2c_sapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 16:10:49.000000 cs-binance-c2c-sapi-0.0.8/cs_binance_c2c_sapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-02 16:10:49.000000 cs-binance-c2c-sapi-0.0.8/cs_binance_c2c_sapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-02 16:10:49.000000 cs-binance-c2c-sapi-0.0.8/cs_binance_c2c_sapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 16:10:49.618006 cs-binance-c2c-sapi-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-02 16:10:36.000000 cs-binance-c2c-sapi-0.0.8/setup.py
```

### Comparing `cs-binance-c2c-sapi-0.0.7/PKG-INFO` & `cs-binance-c2c-sapi-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs-binance-c2c-sapi
-Version: 0.0.7
+Version: 0.0.8
 Summary: Binance C2C SAPI Wrapper
 Author: Richard
 Author-email: <rich_swainson@hotmail.co.uk>
 Keywords: binance,api,wrapper,c2c,sapi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cs-binance-c2c-sapi-0.0.7/README.md` & `cs-binance-c2c-sapi-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `cs-binance-c2c-sapi-0.0.7/binance_c2c/api.py` & `cs-binance-c2c-sapi-0.0.8/binance_c2c/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -193,17 +193,35 @@
             page (int, optional): Page number. Defaults to 1.
             rows (int, optional): Number of rows per page. Defaults to 20.
             filter_type (str, optional): Filter type. Defaults to 'all'.
 
         Returns:
             dict: List of matching advertisements.
         """
+
         return self.make_request('POST', '/sapi/v1/c2c/ads/search',
                                  body_params={'page': page, 'rows': rows, 'asset': asset, 'fiat': fiat,
                                               'tradeType': trade_type, 'filterType': filter_type})['data']
+    
+    def get_ads(self, asset, fiat, trade_type):
+        """
+        Get the first 2 pages of adverts in p2p market.
+
+        Args:
+            asset (str): Asset.
+            fiat (str): Fiat currency.
+            trade_type (str): Trade type ('BUY' or 'SELL').
+
+        Returns:
+            dict: List of matching advertisements.
+        """
+        ads = []
+        for i in range(1, 3):
+            ads += self.search_ads(asset, fiat, trade_type, i, 20, 'all')
+        return ads        
 
     def get_order_details(self, order_number):
         """
         Get details of a specific order.
 
         Args:
             order_number (str): Order number.
```

### Comparing `cs-binance-c2c-sapi-0.0.7/cs_binance_c2c_sapi.egg-info/PKG-INFO` & `cs-binance-c2c-sapi-0.0.8/cs_binance_c2c_sapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs-binance-c2c-sapi
-Version: 0.0.7
+Version: 0.0.8
 Summary: Binance C2C SAPI Wrapper
 Author: Richard
 Author-email: <rich_swainson@hotmail.co.uk>
 Keywords: binance,api,wrapper,c2c,sapi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cs-binance-c2c-sapi-0.0.7/setup.py` & `cs-binance-c2c-sapi-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 DESCRIPTION = 'Binance C2C SAPI Wrapper'
 LONG_DESCRIPTION = 'A Python wrapper for the Binance C2C (Customer-to-Customer) SAPI.'
 
 # Setting up
 setup(
     name="cs-binance-c2c-sapi",
     version=VERSION,
```

