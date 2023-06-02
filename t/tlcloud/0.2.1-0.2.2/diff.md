# Comparing `tmp/tlcloud-0.2.1.tar.gz` & `tmp/tlcloud-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tlcloud-0.2.1.tar", last modified: Mon May 29 03:31:49 2023, max compression
+gzip compressed data, was "tlcloud-0.2.2.tar", last modified: Fri Jun  2 05:36:29 2023, max compression
```

## Comparing `tlcloud-0.2.1.tar` & `tlcloud-0.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 craiet     (501) staff       (20)        0 2023-05-29 03:31:49.685217 tlcloud-0.2.1/
--rw-r--r--   0 craiet     (501) staff       (20)      322 2023-05-29 03:31:49.685058 tlcloud-0.2.1/PKG-INFO
--rw-r--r--   0 craiet     (501) staff       (20)       23 2023-05-29 03:21:17.000000 tlcloud-0.2.1/README.md
--rw-r--r--   0 craiet     (501) staff       (20)       38 2023-05-29 03:31:49.685257 tlcloud-0.2.1/setup.cfg
--rw-r--r--   0 craiet     (501) staff       (20)      505 2023-05-29 03:30:22.000000 tlcloud-0.2.1/setup.py
-drwxr-xr-x   0 craiet     (501) staff       (20)        0 2023-05-29 03:31:49.684423 tlcloud-0.2.1/tlcloud/
--rw-r--r--   0 craiet     (501) staff       (20)        0 2023-05-29 03:27:53.000000 tlcloud-0.2.1/tlcloud/__init__.py
--rw-r--r--   0 craiet     (501) staff       (20)    12708 2023-05-29 03:18:34.000000 tlcloud-0.2.1/tlcloud/geo.py
-drwxr-xr-x   0 craiet     (501) staff       (20)        0 2023-05-29 03:31:49.684886 tlcloud-0.2.1/tlcloud.egg-info/
--rw-r--r--   0 craiet     (501) staff       (20)      322 2023-05-29 03:31:49.000000 tlcloud-0.2.1/tlcloud.egg-info/PKG-INFO
--rw-r--r--   0 craiet     (501) staff       (20)      177 2023-05-29 03:31:49.000000 tlcloud-0.2.1/tlcloud.egg-info/SOURCES.txt
--rw-r--r--   0 craiet     (501) staff       (20)        1 2023-05-29 03:31:49.000000 tlcloud-0.2.1/tlcloud.egg-info/dependency_links.txt
--rw-r--r--   0 craiet     (501) staff       (20)        8 2023-05-29 03:31:49.000000 tlcloud-0.2.1/tlcloud.egg-info/top_level.txt
+drwxr-xr-x   0 craiet     (501) staff       (20)        0 2023-06-02 05:36:29.402334 tlcloud-0.2.2/
+-rw-r--r--   0 craiet     (501) staff       (20)      323 2023-06-02 05:36:29.402217 tlcloud-0.2.2/PKG-INFO
+-rw-r--r--   0 craiet     (501) staff       (20)       25 2023-06-02 05:29:43.000000 tlcloud-0.2.2/README.md
+-rw-r--r--   0 craiet     (501) staff       (20)       38 2023-06-02 05:36:29.402385 tlcloud-0.2.2/setup.cfg
+-rw-r--r--   0 craiet     (501) staff       (20)      505 2023-06-02 05:26:19.000000 tlcloud-0.2.2/setup.py
+drwxr-xr-x   0 craiet     (501) staff       (20)        0 2023-06-02 05:36:29.401482 tlcloud-0.2.2/tlcloud/
+-rw-r--r--   0 craiet     (501) staff       (20)        0 2023-05-29 03:27:53.000000 tlcloud-0.2.2/tlcloud/__init__.py
+-rw-r--r--   0 craiet     (501) staff       (20)    13371 2023-06-02 05:25:48.000000 tlcloud-0.2.2/tlcloud/geo.py
+drwxr-xr-x   0 craiet     (501) staff       (20)        0 2023-06-02 05:36:29.402048 tlcloud-0.2.2/tlcloud.egg-info/
+-rw-r--r--   0 craiet     (501) staff       (20)      323 2023-06-02 05:36:29.000000 tlcloud-0.2.2/tlcloud.egg-info/PKG-INFO
+-rw-r--r--   0 craiet     (501) staff       (20)      177 2023-06-02 05:36:29.000000 tlcloud-0.2.2/tlcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 craiet     (501) staff       (20)        1 2023-06-02 05:36:29.000000 tlcloud-0.2.2/tlcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 craiet     (501) staff       (20)        8 2023-06-02 05:36:29.000000 tlcloud-0.2.2/tlcloud.egg-info/top_level.txt
```

### Comparing `tlcloud-0.2.1/tlcloud/geo.py` & `tlcloud-0.2.2/tlcloud/geo.py`

 * *Files 6% similar despite different names*

```diff
@@ -373,14 +373,34 @@
     :return:     返回两点间距(单位m)
     '''
     x1, y1 = wgs84toutm(lng1, lat1)
     x2, y2 = wgs84toutm(lng2, lat2)
     return pts_dist_xy(x1, y1, x2, y2)
 
 
+def gps_distance(lon1, lat1, lon2, lat2):
+    """
+    Calculate the great circle distance between two points
+    on the earth (specified in decimal degrees)
+    unit - meter
+    """
+    lon1, lat1 = gcj02towgs84(lon1, lat1)
+    lon2, lat2 = gcj02towgs84(lon2, lat2)
+
+    # 将十进制度数转化为弧度
+    lon1, lat1, lon2, lat2 = map(math.radians, [lon1, lat1, lon2, lat2])
+
+    # haversine公式
+    dlon = lon2 - lon1
+    dlat = lat2 - lat1
+    tmp_a = math.sin(dlat / 2) ** 2 + math.cos(lat1) * math.cos(lat2) * math.sin(dlon / 2) ** 2
+    c = 2 * math.asin(math.sqrt(tmp_a))
+    r = 6371  # 地球平均半径，单位为公里
+    return c * r * 1000
+
 if __name__ == "__main__":
     # import pandas as pd
     # data=pd.read_excel(r"D:\项目数据\2021年项目数据\20210421_徐汇井盖\2021-11月徐汇井盖\2021-11-徐汇问题井盖_v3.xlsx",sheet_name="问题井盖")
     # data[["loc_area","loc_location"]]=data.apply(lambda row:gcjtoaddress(row["longitude_gcj"],row["latitude_gcj"]),axis=1,result_type="expand")
     # data.to_excel(r"D:\项目数据\2021年项目数据\20210421_徐汇井盖\2021-11月徐汇井盖\2021-11-徐汇问题井盖_v4.xlsx",index=None)
     # print(gcjtoaddress(113.9158541507666,21.997084380976084))
     print(gcj02towgs84(121.111362566, 31.164911318))
```

