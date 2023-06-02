# Comparing `tmp/scenera.node-0.3.17.tar.gz` & `tmp/scenera.node-0.3.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scenera.node-0.3.17.tar", last modified: Thu Jun  1 18:24:06 2023, max compression
+gzip compressed data, was "scenera.node-0.3.18.tar", last modified: Fri Jun  2 18:26:48 2023, max compression
```

## Comparing `scenera.node-0.3.17.tar` & `scenera.node-0.3.18.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:24:06.081582 scenera.node-0.3.17/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-01 18:23:57.000000 scenera.node-0.3.17/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-06-01 18:24:06.081582 scenera.node-0.3.17/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-01 18:23:57.000000 scenera.node-0.3.17/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:24:06.077582 scenera.node-0.3.17/scenera/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:24:06.081582 scenera.node-0.3.17/scenera/node/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-01 18:23:57.000000 scenera.node-0.3.17/scenera/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-01 18:23:57.000000 scenera.node-0.3.17/scenera/node/jwt_decode.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-01 18:23:57.000000 scenera.node-0.3.17/scenera/node/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-06-01 18:23:57.000000 scenera.node-0.3.17/scenera/node/nodesequencer_header_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    30254 2023-06-01 18:23:57.000000 scenera.node-0.3.17/scenera/node/scenemark.py
--rw-r--r--   0 runner    (1001) docker     (123)    38561 2023-06-01 18:23:57.000000 scenera.node-0.3.17/scenera/node/scenemark_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-01 18:23:57.000000 scenera.node-0.3.17/scenera/node/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-06-01 18:23:57.000000 scenera.node-0.3.17/scenera/node/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-01 18:23:57.000000 scenera.node-0.3.17/scenera/node/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:24:06.077582 scenera.node-0.3.17/scenera.node.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-06-01 18:24:06.000000 scenera.node-0.3.17/scenera.node.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-01 18:24:06.000000 scenera.node-0.3.17/scenera.node.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 18:24:06.000000 scenera.node-0.3.17/scenera.node.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-01 18:24:06.000000 scenera.node-0.3.17/scenera.node.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-01 18:24:06.000000 scenera.node-0.3.17/scenera.node.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 18:24:06.081582 scenera.node-0.3.17/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-01 18:23:57.000000 scenera.node-0.3.17/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:26:48.419424 scenera.node-0.3.18/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-02 18:26:40.000000 scenera.node-0.3.18/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-06-02 18:26:48.415424 scenera.node-0.3.18/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-02 18:26:40.000000 scenera.node-0.3.18/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:26:48.415424 scenera.node-0.3.18/scenera/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:26:48.415424 scenera.node-0.3.18/scenera/node/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-02 18:26:40.000000 scenera.node-0.3.18/scenera/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-02 18:26:40.000000 scenera.node-0.3.18/scenera/node/jwt_decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-02 18:26:40.000000 scenera.node-0.3.18/scenera/node/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-06-02 18:26:40.000000 scenera.node-0.3.18/scenera/node/nodesequencer_header_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30254 2023-06-02 18:26:40.000000 scenera.node-0.3.18/scenera/node/scenemark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38051 2023-06-02 18:26:40.000000 scenera.node-0.3.18/scenera/node/scenemark_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-02 18:26:40.000000 scenera.node-0.3.18/scenera/node/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-06-02 18:26:40.000000 scenera.node-0.3.18/scenera/node/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-02 18:26:40.000000 scenera.node-0.3.18/scenera/node/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:26:48.415424 scenera.node-0.3.18/scenera.node.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-06-02 18:26:48.000000 scenera.node-0.3.18/scenera.node.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-02 18:26:48.000000 scenera.node-0.3.18/scenera.node.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 18:26:48.000000 scenera.node-0.3.18/scenera.node.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-02 18:26:48.000000 scenera.node-0.3.18/scenera.node.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 18:26:48.000000 scenera.node-0.3.18/scenera.node.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 18:26:48.419424 scenera.node-0.3.18/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-02 18:26:40.000000 scenera.node-0.3.18/setup.py
```

### Comparing `scenera.node-0.3.17/LICENSE` & `scenera.node-0.3.18/LICENSE`

 * *Files identical despite different names*

### Comparing `scenera.node-0.3.17/PKG-INFO` & `scenera.node-0.3.18/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scenera.node
-Version: 0.3.17
+Version: 0.3.18
 Summary: Scenera Node SDK
 Home-page: https://docs.scenera.live/
 Author: Dirk Meulenbelt
 Author-email: dirkmeulenbelt@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `scenera.node-0.3.17/README.md` & `scenera.node-0.3.18/README.md`

 * *Files identical despite different names*

### Comparing `scenera.node-0.3.17/scenera/node/jwt_decode.py` & `scenera.node-0.3.18/scenera/node/jwt_decode.py`

 * *Files identical despite different names*

### Comparing `scenera.node-0.3.17/scenera/node/logger.py` & `scenera.node-0.3.18/scenera/node/logger.py`

 * *Files identical despite different names*

### Comparing `scenera.node-0.3.17/scenera/node/nodesequencer_header_schema.py` & `scenera.node-0.3.18/scenera/node/nodesequencer_header_schema.py`

 * *Files identical despite different names*

### Comparing `scenera.node-0.3.17/scenera/node/scenemark.py` & `scenera.node-0.3.18/scenera/node/scenemark.py`

 * *Files identical despite different names*

### Comparing `scenera.node-0.3.17/scenera/node/scenemark_schema.py` & `scenera.node-0.3.18/scenera/node/scenemark_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -293,35 +293,15 @@
             "type": "number"
           },
           "AnalysisID": {
             "type": ["string", "null"],
             "description": "Each algorithm and set of weights has a unique ID that is defined by NICE. This value shall be carried in this record."
           },
           "EventType": {
-            "type": "string",
-            "enum": [
-              "ItemPresence",
-              "RegionOfInterest",
-              "Custom",
-              "Loitering",
-              "Intrusion",
-              "Falldown",
-              "Violence",
-              "Fire",
-              "Abandonment",
-              "SpeedGate",
-              "Xray",
-              "Facility",
-              "Scheduled",
-              "LightOff",
-              "IllegalStay",
-              "HatOff",
-              "PosBreak",
-              "Test"
-            ]
+            "type": "string"
           },
           "CustomEventType": {
             "type": ["string", "null"]
           },
           "AnalysisDescription": {
             "type": ["string", "null"]
           },
```

### Comparing `scenera.node-0.3.17/scenera/node/spec.py` & `scenera.node-0.3.18/scenera/node/spec.py`

 * *Files identical despite different names*

### Comparing `scenera.node-0.3.17/scenera/node/utils.py` & `scenera.node-0.3.18/scenera/node/utils.py`

 * *Files identical despite different names*

### Comparing `scenera.node-0.3.17/scenera/node/validators.py` & `scenera.node-0.3.18/scenera/node/validators.py`

 * *Files identical despite different names*

### Comparing `scenera.node-0.3.17/scenera.node.egg-info/PKG-INFO` & `scenera.node-0.3.18/scenera.node.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scenera.node
-Version: 0.3.17
+Version: 0.3.18
 Summary: Scenera Node SDK
 Home-page: https://docs.scenera.live/
 Author: Dirk Meulenbelt
 Author-email: dirkmeulenbelt@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `scenera.node-0.3.17/setup.py` & `scenera.node-0.3.18/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="scenera.node",
-    version="0.3.17",
+    version="0.3.18",
     description="Scenera Node SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://docs.scenera.live/",
     author="Dirk Meulenbelt",
     author_email="dirkmeulenbelt@gmail.com",
     license="MIT",
```

