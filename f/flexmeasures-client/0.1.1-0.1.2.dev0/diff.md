# Comparing `tmp/flexmeasures-client-0.1.1.tar.gz` & `tmp/flexmeasures-client-0.1.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flexmeasures-client-0.1.1.tar", last modified: Fri May 26 13:38:46 2023, max compression
+gzip compressed data, was "flexmeasures-client-0.1.2.dev0.tar", last modified: Fri Jun  2 13:33:06 2023, max compression
```

## Comparing `flexmeasures-client-0.1.1.tar` & `flexmeasures-client-0.1.2.dev0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:38:46.266334 flexmeasures-client-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:38:46.250332 flexmeasures-client-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:38:46.258333 flexmeasures-client-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13970 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-05-26 13:38:46.266334 flexmeasures-client-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:38:46.262333 flexmeasures-client-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:38:46.262333 flexmeasures-client-0.1.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-26 13:38:46.270334 flexmeasures-client-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:38:46.250332 flexmeasures-client-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:38:46.266334 flexmeasures-client-0.1.1/src/flexmeasures_client/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/src/flexmeasures_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10687 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/src/flexmeasures_client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/src/flexmeasures_client/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/src/flexmeasures_client/response_handling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:38:46.266334 flexmeasures-client-0.1.1/src/flexmeasures_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-05-26 13:38:46.000000 flexmeasures-client-0.1.1/src/flexmeasures_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-26 13:38:46.000000 flexmeasures-client-0.1.1/src/flexmeasures_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:38:46.000000 flexmeasures-client-0.1.1/src/flexmeasures_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:38:45.000000 flexmeasures-client-0.1.1/src/flexmeasures_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-26 13:38:46.000000 flexmeasures-client-0.1.1/src/flexmeasures_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-26 13:38:46.000000 flexmeasures-client-0.1.1/src/flexmeasures_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:38:46.266334 flexmeasures-client-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    12811 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:33:06.751238 flexmeasures-client-0.1.2.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:33:06.743238 flexmeasures-client-0.1.2.dev0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:33:06.743238 flexmeasures-client-0.1.2.dev0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13970 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-06-02 13:33:06.751238 flexmeasures-client-0.1.2.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:33:06.747238 flexmeasures-client-0.1.2.dev0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:33:06.747238 flexmeasures-client-0.1.2.dev0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-02 13:33:06.751238 flexmeasures-client-0.1.2.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:33:06.743238 flexmeasures-client-0.1.2.dev0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:33:06.747238 flexmeasures-client-0.1.2.dev0/src/flexmeasures_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/src/flexmeasures_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11888 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/src/flexmeasures_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/src/flexmeasures_client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/src/flexmeasures_client/response_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:33:06.751238 flexmeasures-client-0.1.2.dev0/src/flexmeasures_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-06-02 13:33:06.000000 flexmeasures-client-0.1.2.dev0/src/flexmeasures_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-02 13:33:06.000000 flexmeasures-client-0.1.2.dev0/src/flexmeasures_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 13:33:06.000000 flexmeasures-client-0.1.2.dev0/src/flexmeasures_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 13:33:06.000000 flexmeasures-client-0.1.2.dev0/src/flexmeasures_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-02 13:33:06.000000 flexmeasures-client-0.1.2.dev0/src/flexmeasures_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-02 13:33:06.000000 flexmeasures-client-0.1.2.dev0/src/flexmeasures_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:33:06.751238 flexmeasures-client-0.1.2.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15102 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-02 13:32:24.000000 flexmeasures-client-0.1.2.dev0/tox.ini
```

### Comparing `flexmeasures-client-0.1.1/.coveragerc` & `flexmeasures-client-0.1.2.dev0/.coveragerc`

 * *Files identical despite different names*

### Comparing `flexmeasures-client-0.1.1/.github/workflows/ci.yml` & `flexmeasures-client-0.1.2.dev0/.github/workflows/ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 
 name: tests
 
 on:
   push:
     # Avoid using all the resources/limits available by checking only
     # relevant branches and tags. Other branches can be checked via PRs.
-    branches: [main]
-    tags: 'v[0-9]+\.[0-9]+\.[0-9]+'  # Match tags that resemble a version
+    branches: [main, hackathon]
+    tags:
+      - 'v[0-9]+\.[0-9]+\.[0-9]+'  # Match tags that resemble a version
+      - 'v[0-9]+\.[0-9]+\.[0-9]+.dev[0-9]+'  # Match tags that resemble a version
   pull_request:  # Run in every PR
   workflow_dispatch:  # Allow manually triggering the workflow
   schedule:
     # Run roughly every 15 days at 00:00 UTC
     # (useful to check if updates on dependencies break the package)
     - cron: '0 0 1,16 * *'
```

### Comparing `flexmeasures-client-0.1.1/.gitignore` & `flexmeasures-client-0.1.2.dev0/.gitignore`

 * *Files identical despite different names*

### Comparing `flexmeasures-client-0.1.1/.pre-commit-config.yaml` & `flexmeasures-client-0.1.2.dev0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `flexmeasures-client-0.1.1/.readthedocs.yml` & `flexmeasures-client-0.1.2.dev0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `flexmeasures-client-0.1.1/CONTRIBUTING.rst` & `flexmeasures-client-0.1.2.dev0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-client-0.1.1/LICENSE.txt` & `flexmeasures-client-0.1.2.dev0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `flexmeasures-client-0.1.1/PKG-INFO` & `flexmeasures-client-0.1.2.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flexmeasures-client
-Version: 0.1.1
+Version: 0.1.2.dev0
 Summary: Async client to connect to the FlexMeasures API
 Home-page: https://github.com/FlexMeasures/flexmeasures-client
 Author: Flexmeasures
 Author-email: info@seita.nl
 License: APACHE
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `flexmeasures-client-0.1.1/README.rst` & `flexmeasures-client-0.1.2.dev0/README.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-client-0.1.1/docs/Makefile` & `flexmeasures-client-0.1.2.dev0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `flexmeasures-client-0.1.1/docs/conf.py` & `flexmeasures-client-0.1.2.dev0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-client-0.1.1/docs/index.rst` & `flexmeasures-client-0.1.2.dev0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-client-0.1.1/setup.cfg` & `flexmeasures-client-0.1.2.dev0/setup.cfg`

 * *Files identical despite different names*

### Comparing `flexmeasures-client-0.1.1/setup.py` & `flexmeasures-client-0.1.2.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-client-0.1.1/src/flexmeasures_client/client.py` & `flexmeasures-client-0.1.2.dev0/src/flexmeasures_client/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -224,14 +224,15 @@
     async def trigger_storage_schedule(
         self,
         sensor_id: int,
         start: str | datetime,
         duration: str | timedelta,
         soc_unit: str,
         soc_at_start: float,
+        soc_max: float | None = None,
         soc_targets: list | None = None,
         consumption_price_sensor: int | None = None,
         production_price_sensor: int | None = None,
         inflexible_device_sensors: list[int] | None = None,
     ) -> str:
         """Post schedule trigger with initial and target states of charge (soc)."""
         if not soc_targets:
@@ -245,14 +246,17 @@
                 "soc-unit": soc_unit,
                 "soc-at-start": soc_at_start,
                 "soc-targets": soc_targets,
             },
             "flex-context": {},
         }
 
+        if soc_max:
+            message["flex-model"]["soc-max"] = soc_max
+
         # Set optional flex context
         if consumption_price_sensor is not None:
             message["flex-context"][
                 "consumption-price-sensor"
             ] = consumption_price_sensor
         if production_price_sensor is not None:
             message["flex-context"]["production-price-sensor"] = production_price_sensor
@@ -295,7 +299,39 @@
         return response
 
     async def get_sensors(self):
         """Get all the sensors available to the current user"""
         response, status = await self.request(uri="sensors", method="GET")
         check_for_status(status, 200)
         return response
+
+    async def trigger_and_get_schedule(
+        self,
+        sensor_id: int,
+        start: str | datetime,
+        duration: str | timedelta,
+        soc_unit: str,
+        soc_at_start: float,
+        soc_max: float | None = None,
+        soc_targets: list | None = None,
+        consumption_price_sensor: int | None = None,
+        production_price_sensor: int | None = None,
+        inflexible_device_sensors: list[int] | None = None,
+    ):
+        schedule_id = await self.trigger_storage_schedule(
+            sensor_id=sensor_id,
+            start=start,
+            duration=duration,
+            soc_unit=soc_unit,
+            soc_max=soc_max,
+            soc_at_start=soc_at_start,
+            soc_targets=soc_targets,
+            consumption_price_sensor=consumption_price_sensor,
+            production_price_sensor=production_price_sensor,
+            inflexible_device_sensors=inflexible_device_sensors,
+        )
+
+        schedule = await self.get_schedule(
+            sensor_id=sensor_id, schedule_id=schedule_id, duration=duration
+        )
+
+        return schedule
```

### Comparing `flexmeasures-client-0.1.1/src/flexmeasures_client/response_handling.py` & `flexmeasures-client-0.1.2.dev0/src/flexmeasures_client/response_handling.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     """
     status = response.status
     payload = await response.json()
     headers = response.headers
     if status < 300:
         pass
     elif status == 401:
-        self.get_access_token()
+        await self.get_access_token()
         self.reauth_once = False
     elif status == 503 and "Retry-After" in headers:
         polling_step += 1
         await asyncio.sleep(self.polling_interval)
     elif status == 400 and (
         "Scheduling job waiting" in payload.get("message", "")
         or "Scheduling job in progress" in payload.get("message", "")
```

### Comparing `flexmeasures-client-0.1.1/src/flexmeasures_client.egg-info/PKG-INFO` & `flexmeasures-client-0.1.2.dev0/src/flexmeasures_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flexmeasures-client
-Version: 0.1.1
+Version: 0.1.2.dev0
 Summary: Async client to connect to the FlexMeasures API
 Home-page: https://github.com/FlexMeasures/flexmeasures-client
 Author: Flexmeasures
 Author-email: info@seita.nl
 License: APACHE
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `flexmeasures-client-0.1.1/src/flexmeasures_client.egg-info/SOURCES.txt` & `flexmeasures-client-0.1.2.dev0/src/flexmeasures_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flexmeasures-client-0.1.1/tests/test_client.py` & `flexmeasures-client-0.1.2.dev0/tests/test_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -411,7 +411,74 @@
 
         with pytest.raises(
             ConnectionError, match="Error occurred while communicating with the API."
         ):
             await flexmeasures_client.get_sensors()
 
     await flexmeasures_client.close()
+
+
+@pytest.mark.asyncio
+async def test_trigger_and_get_schedule() -> None:
+    # todo: relies on https://github.com/pnuckowski/aioresponses/pull/237 to use repeat instead of 3 times the same aioresponse. # noqa: E501
+    with aioresponses() as m:
+        # m.get(
+        #     "http://localhost:5000/api/v3_0/sensors/1/schedules/some-uuid",
+        #     status=400,
+        #     payload={"message": "Scheduling job waiting"},
+        #     repeat=3
+        # )
+        m.post(
+            "http://localhost:5000/api/v3_0/sensors/1/schedules/trigger",
+            status=200,
+            payload={"schedule": "schedule-uuid"},
+        )
+
+        m.get(
+            "http://localhost:5000/api/v3_0/sensors/1/schedules/schedule-uuid",
+            status=400,
+            payload={"message": "Scheduling job waiting"},
+        )
+        m.get(
+            "http://localhost:5000/api/v3_0/sensors/1/schedules/schedule-uuid",
+            status=400,
+            payload={"message": "Scheduling job waiting"},
+        )
+        m.get(
+            "http://localhost:5000/api/v3_0/sensors/1/schedules/schedule-uuid",
+            status=400,
+            payload={"message": "Scheduling job waiting"},
+        )
+        m.get(
+            "http://localhost:5000/api/v3_0/sensors/1/schedules/schedule-uuid",
+            status=200,
+            payload={
+                "values": [2.15, 3, 2],
+                "start": "2015-06-02T10:00:00+00:00",
+                "duration": "PT45M",
+                "unit": "MW",
+            },
+        )
+        flexmeasures_client = FlexMeasuresClient(
+            email="test@test.test",
+            password="test",
+            request_timeout=2,
+            polling_interval=0.2,
+            access_token="skip-auth",
+        )
+
+        schedule = await flexmeasures_client.trigger_and_get_schedule(
+            sensor_id=1,
+            start="2015-06-02T10:00:00+00:00",
+            duration="PT45M",
+            soc_unit="MW",
+            soc_at_start=50,
+            soc_targets=[
+                {
+                    "value": 100,
+                    "datetime": "2023-03-03T11:00+02:00",
+                }
+            ],
+            consumption_price_sensor=3,
+        )
+    assert schedule["values"] == [2.15, 3, 2]
+    await flexmeasures_client.close()
```

### Comparing `flexmeasures-client-0.1.1/tox.ini` & `flexmeasures-client-0.1.2.dev0/tox.ini`

 * *Files identical despite different names*

