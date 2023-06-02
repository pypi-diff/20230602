# Comparing `tmp/influxdb3-python-0.1.3.tar.gz` & `tmp/influxdb3-python-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "influxdb3-python-0.1.3.tar", last modified: Thu Jun  1 17:55:27 2023, max compression
+gzip compressed data, was "influxdb3-python-0.1.4.tar", last modified: Fri Jun  2 16:50:59 2023, max compression
```

## Comparing `influxdb3-python-0.1.3.tar` & `influxdb3-python-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:55:27.468312 influxdb3-python-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-01 17:55:17.000000 influxdb3-python-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-06-01 17:55:27.468312 influxdb3-python-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-06-01 17:55:17.000000 influxdb3-python-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:55:27.468312 influxdb3-python-0.1.3/influxdb3_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-06-01 17:55:27.000000 influxdb3-python-0.1.3/influxdb3_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-01 17:55:27.000000 influxdb3-python-0.1.3/influxdb3_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 17:55:27.000000 influxdb3-python-0.1.3/influxdb3_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-01 17:55:27.000000 influxdb3-python-0.1.3/influxdb3_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-01 17:55:27.000000 influxdb3-python-0.1.3/influxdb3_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:55:27.468312 influxdb3-python-0.1.3/influxdb_client_3/
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-06-01 17:55:17.000000 influxdb3-python-0.1.3/influxdb_client_3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 17:55:27.468312 influxdb3-python-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-01 17:55:17.000000 influxdb3-python-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:55:27.468312 influxdb3-python-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-01 17:55:17.000000 influxdb3-python-0.1.3/tests/test_influxdb_client_3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:50:59.654442 influxdb3-python-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-02 16:50:50.000000 influxdb3-python-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-06-02 16:50:59.650442 influxdb3-python-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-06-02 16:50:50.000000 influxdb3-python-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:50:59.650442 influxdb3-python-0.1.4/influxdb3_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-06-02 16:50:59.000000 influxdb3-python-0.1.4/influxdb3_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-02 16:50:59.000000 influxdb3-python-0.1.4/influxdb3_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 16:50:59.000000 influxdb3-python-0.1.4/influxdb3_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-02 16:50:59.000000 influxdb3-python-0.1.4/influxdb3_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 16:50:59.000000 influxdb3-python-0.1.4/influxdb3_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:50:59.650442 influxdb3-python-0.1.4/influxdb_client_3/
+-rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-06-02 16:50:50.000000 influxdb3-python-0.1.4/influxdb_client_3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-06-02 16:50:50.000000 influxdb3-python-0.1.4/influxdb_client_3/read_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 16:50:59.654442 influxdb3-python-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-02 16:50:50.000000 influxdb3-python-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:50:59.650442 influxdb3-python-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-02 16:50:50.000000 influxdb3-python-0.1.4/tests/test_influxdb_client_3.py
```

### Comparing `influxdb3-python-0.1.3/LICENSE` & `influxdb3-python-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.1.3/PKG-INFO` & `influxdb3-python-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: influxdb3-python
-Version: 0.1.3
+Version: 0.1.4
 Summary: Community Python client for InfluxDB 3.0
 Home-page: https://github.com/InfluxCommunity/influxdb3-python
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: influxdb3-python Version: 0.1.3 Summary: Community
+Metadata-Version: 2.1 Name: influxdb3-python Version: 0.1.4 Summary: Community
 Python client for InfluxDB 3.0 Home-page: https://github.com/InfluxCommunity/
 influxdb3-python Author: InfluxData Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `influxdb3-python-0.1.3/README.md` & `influxdb3-python-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.1.3/influxdb3_python.egg-info/PKG-INFO` & `influxdb3-python-0.1.4/influxdb3_python.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: influxdb3-python
-Version: 0.1.3
+Version: 0.1.4
 Summary: Community Python client for InfluxDB 3.0
 Home-page: https://github.com/InfluxCommunity/influxdb3-python
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: influxdb3-python Version: 0.1.3 Summary: Community
+Metadata-Version: 2.1 Name: influxdb3-python Version: 0.1.4 Summary: Community
 Python client for InfluxDB 3.0 Home-page: https://github.com/InfluxCommunity/
 influxdb3-python Author: InfluxData Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `influxdb3-python-0.1.3/influxdb_client_3/__init__.py` & `influxdb3-python-0.1.4/influxdb_client_3/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # influxdb_client_3/__init__.py
 
-from pyarrow import csv
+import pyarrow as pa
 from pyarrow.flight import FlightClient, Ticket, FlightCallOptions
 from influxdb_client import InfluxDBClient as _InfluxDBClient
 from influxdb_client import WriteOptions as WriteOptions
 from influxdb_client.client.write_api import WriteApi as _WriteApi
 from influxdb_client.client.write_api import SYNCHRONOUS, ASYNCHRONOUS, PointSettings
 from influxdb_client.domain.write_precision import WritePrecision
 from influxdb_client.client.exceptions import InfluxDBError
 from influxdb_client import Point
 import json
 
+from influxdb_client_3.read_file import upload_file
+
 
 def write_client_options(**kwargs):
     return kwargs
 
 
 def flight_client_options(**kwargs):
     return kwargs  # You can replace this with a specific data structure if needed
@@ -71,36 +73,64 @@
         """
         try:
             self._write_api.write(
                 bucket=self._database, record=record, **kwargs)
         except Exception as e:
             print(e)
 
-    def write_csv(
+    def write_file(
             self,
-            csv_file,
+            file,
             measurement_name=None,
             tag_columns=[],
             timestamp_column='time',
             **kwargs):
         """
-        Write data from a CSV file to InfluxDB.
+        Write data from a  file to InfluxDB.
 
-        :param csv_file: The CSV file to write.
-        :type csv_file: str
+        :param file: The file to write.
         :param kwargs: Additional arguments to pass to the write API.
         """
         try:
-            atable = csv.read_csv(csv_file, **kwargs)
+            rf = upload_file(file)
+            Table = rf.load_file()
 
-            df = atable.to_pandas()
-            self._write_api.write(bucket=self._database, record=df,
-                                  data_frame_measurement_name=measurement_name,
-                                  data_frame_tag_columns=tag_columns,
-                                  data_frame_timestamp_column=timestamp_column)
+            if isinstance(Table, pa.Table):
+                df = Table.to_pandas()
+            else:
+                df = Table
+            print(df)
+
+            measurement_column = None
+
+            if measurement_name is None:
+                if 'measurement' in df.columns:
+                        measurement_column = 'measurement'
+                elif 'iox::measurement' in df.columns:
+                        measurement_column = 'iox::measurement'
+
+                if measurement_column is not None:
+                    unique_measurements = df[measurement_column].unique()
+                    for measurement in unique_measurements:
+                        df_measurement = df[df[measurement_column] == measurement]
+                        df_measurement = df_measurement.drop(columns=[measurement_column])
+                        print(df_measurement)
+                        self._write_api.write(bucket=self._database, record=df_measurement,
+                                            data_frame_measurement_name=measurement,
+                                            data_frame_tag_columns=tag_columns,
+                                            data_frame_timestamp_column=timestamp_column)
+                else:
+                    print("'measurement' column not found in the dataframe.")
+            else:
+                if 'measurement' in df.columns:
+                    df = df.drop(columns=['measurement'])
+                self._write_api.write(bucket=self._database, record=df,
+                                    data_frame_measurement_name=measurement_name,
+                                    data_frame_tag_columns=tag_columns,
+                                    data_frame_timestamp_column=timestamp_column)
         except Exception as e:
             print(e)
 
     def query(self, query, language="sql"):
         # create a flight client pointing to the InfluxDB
         # create a ticket
         ticket_data = {
```

### Comparing `influxdb3-python-0.1.3/setup.py` & `influxdb3-python-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.1.3/tests/test_influxdb_client_3.py` & `influxdb3-python-0.1.4/tests/test_influxdb_client_3.py`

 * *Files identical despite different names*

