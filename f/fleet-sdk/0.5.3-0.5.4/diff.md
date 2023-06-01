# Comparing `tmp/fleet_sdk-0.5.3.tar.gz` & `tmp/fleet_sdk-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fleet_sdk-0.5.3.tar", max compression
+gzip compressed data, was "fleet_sdk-0.5.4.tar", max compression
```

## Comparing `fleet_sdk-0.5.3.tar` & `fleet_sdk-0.5.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1074 2023-05-28 23:24:11.000000 fleet_sdk-0.5.3/LICENSE
--rw-r--r--   0        0        0       39 2023-05-29 20:36:49.448172 fleet_sdk-0.5.3/README.md
--rw-r--r--   0        0        0      536 2023-05-31 20:40:35.140960 fleet_sdk-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-05-30 17:33:57.142994 fleet_sdk-0.5.3/src/fleet_sdk/.DS_Store
--rw-r--r--   0        0        0     5724 2023-05-31 20:40:01.146348 fleet_sdk-0.5.3/src/fleet_sdk/Tracker.py
--rw-r--r--   0        0        0       56 2023-05-29 21:37:45.269045 fleet_sdk-0.5.3/src/fleet_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 23:36:32.000000 fleet_sdk-0.5.3/src/fleet_sdk/adapters/__init__.py
--rw-r--r--   0        0        0     1243 2023-05-30 17:34:06.613851 fleet_sdk-0.5.3/src/fleet_sdk/adapters/base_adapter.py
--rw-r--r--   0        0        0     2138 2023-05-30 17:34:19.971392 fleet_sdk-0.5.3/src/fleet_sdk/adapters/fastapi_adapter.py
--rw-r--r--   0        0        0     1871 2023-05-30 17:34:57.215879 fleet_sdk-0.5.3/src/fleet_sdk/adapters/flask_adapter.py
--rw-r--r--   0        0        0     1987 2023-05-30 17:35:08.954831 fleet_sdk-0.5.3/src/fleet_sdk/adapters/quart_adapter.py
--rw-r--r--   0        0        0      672 1970-01-01 00:00:00.000000 fleet_sdk-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-28 23:24:11.000000 fleet_sdk-0.5.4/LICENSE
+-rw-r--r--   0        0        0       39 2023-05-29 20:36:49.448172 fleet_sdk-0.5.4/README.md
+-rw-r--r--   0        0        0      536 2023-06-01 19:46:30.814760 fleet_sdk-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-05-30 17:33:57.142994 fleet_sdk-0.5.4/src/fleet_sdk/.DS_Store
+-rw-r--r--   0        0        0     5724 2023-05-31 20:40:01.146348 fleet_sdk-0.5.4/src/fleet_sdk/Tracker.py
+-rw-r--r--   0        0        0       56 2023-05-29 21:37:45.269045 fleet_sdk-0.5.4/src/fleet_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-28 23:36:32.000000 fleet_sdk-0.5.4/src/fleet_sdk/adapters/__init__.py
+-rw-r--r--   0        0        0     1243 2023-05-30 17:34:06.613851 fleet_sdk-0.5.4/src/fleet_sdk/adapters/base_adapter.py
+-rw-r--r--   0        0        0     2138 2023-05-30 17:34:19.971392 fleet_sdk-0.5.4/src/fleet_sdk/adapters/fastapi_adapter.py
+-rw-r--r--   0        0        0     1955 2023-06-01 19:34:06.261840 fleet_sdk-0.5.4/src/fleet_sdk/adapters/flask_adapter.py
+-rw-r--r--   0        0        0     2103 2023-06-01 19:33:04.775976 fleet_sdk-0.5.4/src/fleet_sdk/adapters/quart_adapter.py
+-rw-r--r--   0        0        0      672 1970-01-01 00:00:00.000000 fleet_sdk-0.5.4/PKG-INFO
```

### Comparing `fleet_sdk-0.5.3/LICENSE` & `fleet_sdk-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fleet_sdk-0.5.3/pyproject.toml` & `fleet_sdk-0.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fleet-sdk"
-version = "0.5.3"
+version = "0.5.4"
 description = "Fleet SDK for building and managing chatGPT plugins"
 authors = ["fleet_team <fleet.ai.team@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.6"
 fastapi = "^0.95.0"
```

### Comparing `fleet_sdk-0.5.3/src/fleet_sdk/.DS_Store` & `fleet_sdk-0.5.4/src/fleet_sdk/.DS_Store`

 * *Files identical despite different names*

### Comparing `fleet_sdk-0.5.3/src/fleet_sdk/Tracker.py` & `fleet_sdk-0.5.4/src/fleet_sdk/Tracker.py`

 * *Files identical despite different names*

### Comparing `fleet_sdk-0.5.3/src/fleet_sdk/adapters/base_adapter.py` & `fleet_sdk-0.5.4/src/fleet_sdk/adapters/base_adapter.py`

 * *Files identical despite different names*

### Comparing `fleet_sdk-0.5.3/src/fleet_sdk/adapters/fastapi_adapter.py` & `fleet_sdk-0.5.4/src/fleet_sdk/adapters/fastapi_adapter.py`

 * *Files identical despite different names*

### Comparing `fleet_sdk-0.5.3/src/fleet_sdk/adapters/flask_adapter.py` & `fleet_sdk-0.5.4/src/fleet_sdk/adapters/quart_adapter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,31 @@
-from flask import request
+from quart import request, Response
 from .base_adapter import BaseAdapter
+import time
+import json
 
-class FlaskAdapter(BaseAdapter):
-  def extract_data(self, event_name, request, response, latency):
+
+class QuartAdapter(BaseAdapter):
+
+  async def extract_data(self, event_name, request, response, latency):
     # Extract the data from the request and response
-    request_data = self.extract_request_data(request)
-    response_data = self.extract_response_data(response)
+    request_data = await self.extract_request_data(request)
+    response_data = await self.extract_response_data(response)
 
     # Combine request data and response data into one dictionary
     data = request_data
     data.update(response_data)
     data['latency'] = latency
     data[
       'function_name'] = event_name  # Add the event_name to the data dictionary
 
     return data
 
-  def extract_request_data(self, request):
+  async def extract_request_data(self, request):
+    print(f"Request: {request}")
     # Extract the data from the request
     data = {}
 
     # Add the headers
     data['headers'] = dict(request.headers)
 
     # Add required fields
@@ -31,30 +36,31 @@
     # Add endpoint info
     data['endpoint'] = request.path
     data['ip_address'] = request.remote_addr
     data['query_params'] = request.args.to_dict()
     data['method'] = request.method
 
     # Add request data
-    data['request_body'] = request.get_json()
+    data['request_body'] = await request.get_json()
 
     return data
 
-  def extract_response_data(self, response):
+  async def extract_response_data(self, response):
     # Print debug information about the response
     print(f"Response type: {type(response)}")
     print(f"Response content: {response}")
-
+  
     if isinstance(response, Response):
       # If the response is a 'Response' object, extract its JSON data
       data = {}
       try:
-        data['response_data'] = response.get_json()
+        raw_data = await response.get_data()  # Get the raw response data
+        data['response_data'] = json.loads(raw_data.decode('utf-8'))  # Parse the data as JSON
       except Exception:
         data['response_data'] = None
       data['response_code'] = response.status_code
       data['response_size'] = len(json.dumps(data['response_data']))
-
+  
       return data
     else:
       # If the response is not a 'Response' object, defer to the base adapter
-      return super().extract_response_data(response)
+      return await super().extract_response_data(response)
```

### Comparing `fleet_sdk-0.5.3/PKG-INFO` & `fleet_sdk-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fleet-sdk
-Version: 0.5.3
+Version: 0.5.4
 Summary: Fleet SDK for building and managing chatGPT plugins
 Author: fleet_team
 Author-email: fleet.ai.team@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

