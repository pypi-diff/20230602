# Comparing `tmp/sellix-python-sdk-1.0.7.tar.gz` & `tmp/sellix-python-sdk-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sellix-python-sdk-1.0.7.tar", last modified: Thu May 25 18:03:18 2023, max compression
+gzip compressed data, was "sellix-python-sdk-1.0.8.tar", last modified: Fri Jun  2 13:56:11 2023, max compression
```

## Comparing `sellix-python-sdk-1.0.7.tar` & `sellix-python-sdk-1.0.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:03:18.062286 sellix-python-sdk-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-25 18:03:05.000000 sellix-python-sdk-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-25 18:03:18.062286 sellix-python-sdk-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-25 18:03:05.000000 sellix-python-sdk-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:03:18.058286 sellix-python-sdk-1.0.7/sellix/
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-05-25 18:03:05.000000 sellix-python-sdk-1.0.7/sellix/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:03:18.058286 sellix-python-sdk-1.0.7/sellix/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 18:03:05.000000 sellix-python-sdk-1.0.7/sellix/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-25 18:03:05.000000 sellix-python-sdk-1.0.7/sellix/resources/blacklist.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-25 18:03:05.000000 sellix-python-sdk-1.0.7/sellix/resources/categories.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-25 18:03:05.000000 sellix-python-sdk-1.0.7/sellix/resources/coupons.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-25 18:03:05.000000 sellix-python-sdk-1.0.7/sellix/resources/customers.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-25 18:03:05.000000 sellix-python-sdk-1.0.7/sellix/resources/feedback.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-25 18:03:05.000000 sellix-python-sdk-1.0.7/sellix/resources/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-25 18:03:05.000000 sellix-python-sdk-1.0.7/sellix/resources/orders.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-25 18:03:05.000000 sellix-python-sdk-1.0.7/sellix/resources/payments.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-25 18:03:05.000000 sellix-python-sdk-1.0.7/sellix/resources/products.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-25 18:03:05.000000 sellix-python-sdk-1.0.7/sellix/resources/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-25 18:03:05.000000 sellix-python-sdk-1.0.7/sellix/resources/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-25 18:03:05.000000 sellix-python-sdk-1.0.7/sellix/resources/whitelists.py
--rw-r--r--   0 runner    (1001) docker     (123)    12077 2023-05-25 18:03:05.000000 sellix-python-sdk-1.0.7/sellix/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:03:18.058286 sellix-python-sdk-1.0.7/sellix_python_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-25 18:03:18.000000 sellix-python-sdk-1.0.7/sellix_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-25 18:03:18.000000 sellix-python-sdk-1.0.7/sellix_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 18:03:18.000000 sellix-python-sdk-1.0.7/sellix_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 18:03:18.000000 sellix-python-sdk-1.0.7/sellix_python_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-25 18:03:18.000000 sellix-python-sdk-1.0.7/sellix_python_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 18:03:18.062286 sellix-python-sdk-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-25 18:03:05.000000 sellix-python-sdk-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:56:11.337054 sellix-python-sdk-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-02 13:55:59.000000 sellix-python-sdk-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-02 13:56:11.333054 sellix-python-sdk-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-02 13:55:59.000000 sellix-python-sdk-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:56:11.325055 sellix-python-sdk-1.0.8/sellix/
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-02 13:55:59.000000 sellix-python-sdk-1.0.8/sellix/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:56:11.333054 sellix-python-sdk-1.0.8/sellix/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 13:55:59.000000 sellix-python-sdk-1.0.8/sellix/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-02 13:55:59.000000 sellix-python-sdk-1.0.8/sellix/resources/blacklist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-02 13:55:59.000000 sellix-python-sdk-1.0.8/sellix/resources/categories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-02 13:55:59.000000 sellix-python-sdk-1.0.8/sellix/resources/coupons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-02 13:55:59.000000 sellix-python-sdk-1.0.8/sellix/resources/customers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-02 13:55:59.000000 sellix-python-sdk-1.0.8/sellix/resources/feedback.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-02 13:55:59.000000 sellix-python-sdk-1.0.8/sellix/resources/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-02 13:55:59.000000 sellix-python-sdk-1.0.8/sellix/resources/orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-02 13:55:59.000000 sellix-python-sdk-1.0.8/sellix/resources/payments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-02 13:55:59.000000 sellix-python-sdk-1.0.8/sellix/resources/products.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-02 13:55:59.000000 sellix-python-sdk-1.0.8/sellix/resources/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-02 13:55:59.000000 sellix-python-sdk-1.0.8/sellix/resources/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-02 13:55:59.000000 sellix-python-sdk-1.0.8/sellix/resources/whitelists.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12077 2023-06-02 13:55:59.000000 sellix-python-sdk-1.0.8/sellix/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:56:11.333054 sellix-python-sdk-1.0.8/sellix_python_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-02 13:56:11.000000 sellix-python-sdk-1.0.8/sellix_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-02 13:56:11.000000 sellix-python-sdk-1.0.8/sellix_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 13:56:11.000000 sellix-python-sdk-1.0.8/sellix_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-02 13:56:11.000000 sellix-python-sdk-1.0.8/sellix_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-02 13:56:11.000000 sellix-python-sdk-1.0.8/sellix_python_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 13:56:11.337054 sellix-python-sdk-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-02 13:55:59.000000 sellix-python-sdk-1.0.8/setup.py
```

### Comparing `sellix-python-sdk-1.0.7/LICENSE` & `sellix-python-sdk-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sellix-python-sdk-1.0.7/PKG-INFO` & `sellix-python-sdk-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sellix-python-sdk
-Version: 1.0.7
+Version: 1.0.8
 Home-page: https://github.com/Sellix/python-sdk
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Sellix Python SDK 
 
 ![tag](https://img.shields.io/github/v/tag/sellix/python-sdk?sort=date&color=blueviolet)
```

### Comparing `sellix-python-sdk-1.0.7/README.md` & `sellix-python-sdk-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `sellix-python-sdk-1.0.7/sellix/__init__.py` & `sellix-python-sdk-1.0.8/sellix/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     from .resources.blacklist import get_blacklists, create_blacklist, get_blacklist, update_blacklist, delete_blacklist
     from .resources.categories import get_categories, create_category, get_category, update_category, delete_category
     from .resources.groups import get_groups, create_group, get_group, update_group, delete_group
     from .resources.coupons import get_coupons, create_coupon, get_coupon, update_coupon, delete_coupon
     from .resources.feedback import get_feedback, reply_feedback
     from .resources.orders import get_orders, get_order, update_order, issue_order_replacement
     from .resources.payments import create_payment, delete_payment
-    from .resources.products import get_products, create_product, get_product, update_product, delete_product
+    from .resources.products import get_products, create_product, get_product, update_product, delete_product, licensing_check, licensing_update_hardware_id
     from .resources.queries import get_queries, get_query, reply_query, close_query, reopen_query
     from .resources.whitelists import get_whitelists, create_whitelist, get_whitelist, update_whitelist, delete_whitelist
     from .resources.customers import get_customers, create_customer, get_customer, update_customer
     from .resources.subscriptions import get_subscriptions, create_subscription, get_subscription, delete_subscription
     from .test import sellix_test_sdk
 
     class SellixException(Exception):
```

### Comparing `sellix-python-sdk-1.0.7/sellix/resources/blacklist.py` & `sellix-python-sdk-1.0.8/sellix/resources/blacklist.py`

 * *Files identical despite different names*

### Comparing `sellix-python-sdk-1.0.7/sellix/resources/categories.py` & `sellix-python-sdk-1.0.8/sellix/resources/categories.py`

 * *Files identical despite different names*

### Comparing `sellix-python-sdk-1.0.7/sellix/resources/coupons.py` & `sellix-python-sdk-1.0.8/sellix/resources/coupons.py`

 * *Files identical despite different names*

### Comparing `sellix-python-sdk-1.0.7/sellix/resources/customers.py` & `sellix-python-sdk-1.0.8/sellix/resources/customers.py`

 * *Files identical despite different names*

### Comparing `sellix-python-sdk-1.0.7/sellix/resources/groups.py` & `sellix-python-sdk-1.0.8/sellix/resources/groups.py`

 * *Files identical despite different names*

### Comparing `sellix-python-sdk-1.0.7/sellix/resources/orders.py` & `sellix-python-sdk-1.0.8/sellix/resources/orders.py`

 * *Files identical despite different names*

### Comparing `sellix-python-sdk-1.0.7/sellix/resources/products.py` & `sellix-python-sdk-1.0.8/sellix/resources/products.py`

 * *Files identical despite different names*

### Comparing `sellix-python-sdk-1.0.7/sellix/resources/queries.py` & `sellix-python-sdk-1.0.8/sellix/resources/queries.py`

 * *Files identical despite different names*

### Comparing `sellix-python-sdk-1.0.7/sellix/resources/subscriptions.py` & `sellix-python-sdk-1.0.8/sellix/resources/subscriptions.py`

 * *Files identical despite different names*

### Comparing `sellix-python-sdk-1.0.7/sellix/resources/whitelists.py` & `sellix-python-sdk-1.0.8/sellix/resources/whitelists.py`

 * *Files identical despite different names*

### Comparing `sellix-python-sdk-1.0.7/sellix/test.py` & `sellix-python-sdk-1.0.8/sellix/test.py`

 * *Files identical despite different names*

### Comparing `sellix-python-sdk-1.0.7/sellix_python_sdk.egg-info/PKG-INFO` & `sellix-python-sdk-1.0.8/sellix_python_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sellix-python-sdk
-Version: 1.0.7
+Version: 1.0.8
 Home-page: https://github.com/Sellix/python-sdk
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Sellix Python SDK 
 
 ![tag](https://img.shields.io/github/v/tag/sellix/python-sdk?sort=date&color=blueviolet)
```

### Comparing `sellix-python-sdk-1.0.7/sellix_python_sdk.egg-info/SOURCES.txt` & `sellix-python-sdk-1.0.8/sellix_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

