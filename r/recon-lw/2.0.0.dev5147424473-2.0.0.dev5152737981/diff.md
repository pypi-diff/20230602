# Comparing `tmp/recon_lw-2.0.0.dev5147424473.tar.gz` & `tmp/recon_lw-2.0.0.dev5152737981.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev5147424473.tar", last modified: Thu Jun  1 17:34:05 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev5152737981.tar", last modified: Fri Jun  2 06:56:35 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev5147424473.tar` & `recon_lw-2.0.0.dev5152737981.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 17:34:05.000000 recon_lw-2.0.0.dev5147424473/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-01 17:33:20.000000 recon_lw-2.0.0.dev5147424473/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-01 17:34:05.000000 recon_lw-2.0.0.dev5147424473/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-01 17:33:20.000000 recon_lw-2.0.0.dev5147424473/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-01 17:33:42.000000 recon_lw-2.0.0.dev5147424473/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 17:34:05.000000 recon_lw-2.0.0.dev5147424473/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-01 17:33:20.000000 recon_lw-2.0.0.dev5147424473/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     1096 2023-06-01 17:33:20.000000 recon_lw-2.0.0.dev5147424473/recon_lw/LastStateMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-06-01 17:33:20.000000 recon_lw-2.0.0.dev5147424473/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-06-01 17:33:20.000000 recon_lw-2.0.0.dev5147424473/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-01 17:33:20.000000 recon_lw-2.0.0.dev5147424473/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-06-01 17:33:20.000000 recon_lw-2.0.0.dev5147424473/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    32667 2023-06-01 17:33:20.000000 recon_lw-2.0.0.dev5147424473/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    22337 2023-06-01 17:33:20.000000 recon_lw-2.0.0.dev5147424473/recon_lw/recon_ob_cross_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 17:34:05.000000 recon_lw-2.0.0.dev5147424473/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-01 17:34:05.000000 recon_lw-2.0.0.dev5147424473/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      454 2023-06-01 17:34:05.000000 recon_lw-2.0.0.dev5147424473/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 17:34:05.000000 recon_lw-2.0.0.dev5147424473/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-06-01 17:34:05.000000 recon_lw-2.0.0.dev5147424473/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-01 17:34:05.000000 recon_lw-2.0.0.dev5147424473/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-01 17:33:20.000000 recon_lw-2.0.0.dev5147424473/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-01 17:34:05.000000 recon_lw-2.0.0.dev5147424473/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-01 17:33:20.000000 recon_lw-2.0.0.dev5147424473/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 17:34:05.000000 recon_lw-2.0.0.dev5147424473/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-06-01 17:33:20.000000 recon_lw-2.0.0.dev5147424473/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 06:56:35.000000 recon_lw-2.0.0.dev5152737981/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-02 06:55:51.000000 recon_lw-2.0.0.dev5152737981/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-02 06:56:35.000000 recon_lw-2.0.0.dev5152737981/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-02 06:55:51.000000 recon_lw-2.0.0.dev5152737981/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-02 06:56:16.000000 recon_lw-2.0.0.dev5152737981/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 06:56:35.000000 recon_lw-2.0.0.dev5152737981/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-02 06:55:51.000000 recon_lw-2.0.0.dev5152737981/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1096 2023-06-02 06:55:51.000000 recon_lw-2.0.0.dev5152737981/recon_lw/LastStateMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-06-02 06:55:51.000000 recon_lw-2.0.0.dev5152737981/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-06-02 06:55:51.000000 recon_lw-2.0.0.dev5152737981/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-02 06:55:51.000000 recon_lw-2.0.0.dev5152737981/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-06-02 06:55:51.000000 recon_lw-2.0.0.dev5152737981/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32667 2023-06-02 06:55:51.000000 recon_lw-2.0.0.dev5152737981/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22335 2023-06-02 06:55:51.000000 recon_lw-2.0.0.dev5152737981/recon_lw/recon_ob_cross_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 06:56:35.000000 recon_lw-2.0.0.dev5152737981/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-02 06:56:35.000000 recon_lw-2.0.0.dev5152737981/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      454 2023-06-02 06:56:35.000000 recon_lw-2.0.0.dev5152737981/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-02 06:56:35.000000 recon_lw-2.0.0.dev5152737981/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-06-02 06:56:35.000000 recon_lw-2.0.0.dev5152737981/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-02 06:56:35.000000 recon_lw-2.0.0.dev5152737981/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-02 06:55:51.000000 recon_lw-2.0.0.dev5152737981/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-02 06:56:35.000000 recon_lw-2.0.0.dev5152737981/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-02 06:55:51.000000 recon_lw-2.0.0.dev5152737981/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 06:56:35.000000 recon_lw-2.0.0.dev5152737981/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-06-02 06:55:51.000000 recon_lw-2.0.0.dev5152737981/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev5147424473/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev5152737981/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5147424473/recon_lw/LastStateMatcher.py` & `recon_lw-2.0.0.dev5152737981/recon_lw/LastStateMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5147424473/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev5152737981/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5147424473/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev5152737981/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5147424473/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev5152737981/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5147424473/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev5152737981/recon_lw/recon_ob.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5147424473/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev5152737981/recon_lw/recon_ob_cross_stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     problems = []
     for side in ["ask", "bid"]:
         full_levels = list(full_book[side].keys())
         if side == "ask":
             full_levels.sort()
         else:
             full_levels.sort(reverse=True)
-        aggr_levels = [level for level in aggr_book[side + "_aggr"] if level["real_num_orders"] != "0"]
+        aggr_levels = [level for level in aggr_book[side + "_aggr"] if level["real_num_orders"] != 0]
         for i in range(aggr_book["aggr_max_levels"]):
             if i < len(full_levels) and i < len(aggr_levels):
                 price_condition = full_levels[i] == aggr_levels[i]["price"]
                 num_orders_condition = len(full_book[side][full_levels[i]]) == \
                                        (aggr_levels[i]["real_num_orders"])
                 size_condition = sum(full_book[side][full_levels[i]].values()) == \
                                  (aggr_levels[i]["real_qty"])
```

### Comparing `recon_lw-2.0.0.dev5147424473/setup.py` & `recon_lw-2.0.0.dev5152737981/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5147424473/test/test_recon_ob.py` & `recon_lw-2.0.0.dev5152737981/test/test_recon_ob.py`

 * *Files identical despite different names*

