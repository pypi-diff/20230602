# Comparing `tmp/fmo-cli-1.0.2.tar.gz` & `tmp/fmo-cli-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fmo-cli-1.0.2.tar", last modified: Sat May 13 02:12:05 2023, max compression
+gzip compressed data, was "fmo-cli-1.1.0.tar", last modified: Fri Jun  2 20:45:25 2023, max compression
```

## Comparing `fmo-cli-1.0.2.tar` & `fmo-cli-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 02:12:05.426279 fmo-cli-1.0.2/
--rw-r--r--   0 root         (0) root         (0)     1871 2023-05-13 02:12:05.426279 fmo-cli-1.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1588 2023-05-13 02:11:37.000000 fmo-cli-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 02:12:05.426279 fmo-cli-1.0.2/fmo/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-13 02:11:37.000000 fmo-cli-1.0.2/fmo/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1693 2023-05-13 02:11:37.000000 fmo-cli-1.0.2/fmo/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1730 2023-05-13 02:11:37.000000 fmo-cli-1.0.2/fmo/fmo.py
--rw-rw-rw-   0 root         (0) root         (0)     1106 2023-05-13 02:11:37.000000 fmo-cli-1.0.2/fmo/nmea.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 02:12:05.426279 fmo-cli-1.0.2/fmo_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1871 2023-05-13 02:12:05.000000 fmo-cli-1.0.2/fmo_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      256 2023-05-13 02:12:05.000000 fmo-cli-1.0.2/fmo_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-13 02:12:05.000000 fmo-cli-1.0.2/fmo_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       36 2023-05-13 02:12:05.000000 fmo-cli-1.0.2/fmo_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-13 02:12:05.000000 fmo-cli-1.0.2/fmo_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-05-13 02:12:05.000000 fmo-cli-1.0.2/fmo_cli.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-13 02:12:05.426279 fmo-cli-1.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      880 2023-05-13 02:11:37.000000 fmo-cli-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 20:45:25.074311 fmo-cli-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)     1871 2023-06-02 20:45:25.074311 fmo-cli-1.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1588 2023-05-13 02:11:37.000000 fmo-cli-1.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 20:45:25.074311 fmo-cli-1.1.0/fmo/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-13 02:11:37.000000 fmo-cli-1.1.0/fmo/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2397 2023-06-02 20:44:58.000000 fmo-cli-1.1.0/fmo/api.py
+-rw-rw-rw-   0 root         (0) root         (0)      538 2023-06-02 20:44:58.000000 fmo-cli-1.1.0/fmo/lease.py
+-rw-rw-rw-   0 root         (0) root         (0)     1106 2023-06-02 20:44:58.000000 fmo-cli-1.1.0/fmo/nmea.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 20:45:25.074311 fmo-cli-1.1.0/fmo_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1871 2023-06-02 20:45:25.000000 fmo-cli-1.1.0/fmo_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      258 2023-06-02 20:45:25.000000 fmo-cli-1.1.0/fmo_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 20:45:25.000000 fmo-cli-1.1.0/fmo_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2023-06-02 20:45:25.000000 fmo-cli-1.1.0/fmo_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-02 20:45:25.000000 fmo-cli-1.1.0/fmo_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-06-02 20:45:25.000000 fmo-cli-1.1.0/fmo_cli.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-02 20:45:25.074311 fmo-cli-1.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      880 2023-05-13 02:11:37.000000 fmo-cli-1.1.0/setup.py
```

### Comparing `fmo-cli-1.0.2/PKG-INFO` & `fmo-cli-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmo-cli
-Version: 1.0.2
+Version: 1.1.0
 Summary: Command Line Interface to access and upload FindMyOyster data
 Author: Gudjon Magnusson
 Author-email: gmagnusson@fraunhofer.org
 Keywords: FindMyOyster,CLI
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
```

### Comparing `fmo-cli-1.0.2/README.md` & `fmo-cli-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `fmo-cli-1.0.2/fmo/fmo.py` & `fmo-cli-1.1.0/fmo/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import requests
 import pandas
 import datetime
+import geojson
 
 FMO_API_URL = "https://api.findmyoyster.com/v1"
 
 
 def any_to_unix_time(any):
     if isinstance(any, datetime.datetime):
         return int(datetime.datetime.timestamp(any))
 
     if isinstance(any, str):
         return int(datetime.datetime.fromisoformat(any).timestamp())
-    
+
     if isinstance(any, int):
         return any
 
     raise Exception("Failed to convert timestamp")
 
 
 def login_to_get_token(url, farm, user, password) -> str:
@@ -44,22 +45,41 @@
                 {"lat": c[1], "lng": c[2], "timestamp": any_to_unix_time(c[0])}
                 for c in self._coords
             ]
         }
 
     def dataframe(self):
         return pandas.DataFrame(self._coords, columns=["Time", "Latitude", "Longitude"])
+    
+    def geojson(self):
+        line_coordinates = [(lng, lat) for _, lat, lng in self._coords]
+        line = geojson.LineString(line_coordinates)
+        feature = geojson.Feature(geometry=line)
+        feature_collection = geojson.FeatureCollection([feature])
+        return feature_collection
 
 
 class FMO:
     def __init__(self, token, url="api.findmyoyster.com/v1"):
         self._url = url
         self._token = token
 
     def upload_path(self, path: GPSPath):
         response = requests.post(
             f"{self._url}/paths",
             json=path.fmo_path_json(),
             headers={"Authorization": f"Bearer {self._token}"},
         )
         if not response.ok:
+            print(response.text)
             raise Exception(response.reason)
+
+    def list_water_leases(self):
+        response = requests.get(
+            f"{self._url}/leases",
+            headers={"Authorization": f"Bearer {self._token}"},
+        )
+        if not response.ok:
+            print(response.text)
+            raise Exception(response.reason)
+
+        return response.json()["data"]
```

### Comparing `fmo-cli-1.0.2/fmo/nmea.py` & `fmo-cli-1.1.0/fmo/nmea.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 from datetime import datetime
 import pandas
 # Convert DMS coordinates to decimal degrees
-from fmo.fmo import GPSPath
+from fmo.api import GPSPath
 
 
 def nmea_latitude(dms, direction):
     decimal = float(dms[:2]) + float(dms[2:])/60
     if direction == 'S':
         decimal = -decimal
     return decimal
```

### Comparing `fmo-cli-1.0.2/fmo_cli.egg-info/PKG-INFO` & `fmo-cli-1.1.0/fmo_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmo-cli
-Version: 1.0.2
+Version: 1.1.0
 Summary: Command Line Interface to access and upload FindMyOyster data
 Author: Gudjon Magnusson
 Author-email: gmagnusson@fraunhofer.org
 Keywords: FindMyOyster,CLI
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
```

### Comparing `fmo-cli-1.0.2/setup.py` & `fmo-cli-1.1.0/setup.py`

 * *Files identical despite different names*

