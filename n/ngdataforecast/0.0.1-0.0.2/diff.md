# Comparing `tmp/ngdataforecast-0.0.1.tar.gz` & `tmp/ngdataforecast-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngdataforecast-0.0.1.tar", max compression
+gzip compressed data, was "ngdataforecast-0.0.2.tar", max compression
```

## Comparing `ngdataforecast-0.0.1.tar` & `ngdataforecast-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     6255 2023-06-01 14:46:48.684432 ngdataforecast-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-06-01 14:46:48.705432 ngdataforecast-0.0.1/ngdataforecast/__init__.py
--rw-r--r--   0        0        0     6180 2023-06-01 14:46:48.684432 ngdataforecast-0.0.1/ngdataforecast/forecast_model.py
--rw-r--r--   0        0        0        0 2023-06-01 14:46:48.706432 ngdataforecast-0.0.1/ngdataforecast/local_level/__init__.py
--rw-r--r--   0        0        0     3391 2023-06-01 14:46:48.684432 ngdataforecast-0.0.1/ngdataforecast/local_level/model.py
--rw-r--r--   0        0        0      367 2023-06-01 14:46:48.684432 ngdataforecast-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     6834 1970-01-01 00:00:00.000000 ngdataforecast-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     6255 2023-06-02 18:41:47.234492 ngdataforecast-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-02 18:41:47.258491 ngdataforecast-0.0.2/ngdataforecast/__init__.py
+-rw-r--r--   0        0        0     6180 2023-06-02 18:41:47.234492 ngdataforecast-0.0.2/ngdataforecast/forecast_model.py
+-rw-r--r--   0        0        0        0 2023-06-02 18:41:47.258491 ngdataforecast-0.0.2/ngdataforecast/local_level/__init__.py
+-rw-r--r--   0        0        0     3544 2023-06-02 18:41:47.235492 ngdataforecast-0.0.2/ngdataforecast/local_level/model.py
+-rw-r--r--   0        0        0      367 2023-06-02 18:41:47.235492 ngdataforecast-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6834 1970-01-01 00:00:00.000000 ngdataforecast-0.0.2/PKG-INFO
```

### Comparing `ngdataforecast-0.0.1/README.md` & `ngdataforecast-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ngdataforecast-0.0.1/ngdataforecast/forecast_model.py` & `ngdataforecast-0.0.2/ngdataforecast/forecast_model.py`

 * *Files identical despite different names*

### Comparing `ngdataforecast-0.0.1/ngdataforecast/local_level/model.py` & `ngdataforecast-0.0.2/ngdataforecast/local_level/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,18 +14,20 @@
 
     def __init__(self, input_dict):
         super().__init__(input_dict)
 
     def _create_point_forecast(self, df, forecast_timestamps):
         """Create the point forecast DataFrame."""
         point_forecast = pd.DataFrame(index=forecast_timestamps, columns=["value"])
-        point_forecast["value"] = [
-            df[df.index.hour == hour]["value"].iloc[-7]
-            for hour in forecast_timestamps.hour
-        ]
+        for current_timestamp in forecast_timestamps:
+            one_week_prior = current_timestamp - pd.DateOffset(weeks=1)
+            if one_week_prior in df.index:
+                point_forecast.loc[current_timestamp, "value"] = df.loc[
+                    one_week_prior, "value"
+                ]
         return point_forecast
 
     def _calculate_variance(self, df, forecast_timestamps):
         """Calculate the variance DataFrame."""
         # Initialize an empty DataFrame for variance
         variance = pd.DataFrame(index=forecast_timestamps, columns=["variance"])
```

### Comparing `ngdataforecast-0.0.1/PKG-INFO` & `ngdataforecast-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngdataforecast
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library for facilitating the development forecast models in NG.CASH
 Author: NG.CASH
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

