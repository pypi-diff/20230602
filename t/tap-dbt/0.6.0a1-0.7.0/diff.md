# Comparing `tmp/tap_dbt-0.6.0a1.tar.gz` & `tmp/tap_dbt-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_dbt-0.6.0a1.tar", max compression
+gzip compressed data, was "tap_dbt-0.7.0.tar", max compression
```

## Comparing `tap_dbt-0.6.0a1.tar` & `tap_dbt-0.7.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2023-05-19 22:32:03.917137 tap_dbt-0.6.0a1/LICENSE
--rw-r--r--   0        0        0     4899 2023-05-19 22:32:03.917137 tap_dbt-0.6.0a1/README.md
--rw-r--r--   0        0        0     1651 2023-05-19 22:32:20.177365 tap_dbt-0.6.0a1/pyproject.toml
--rw-r--r--   0        0        0       40 2023-05-19 22:32:03.917137 tap_dbt-0.6.0a1/tap_dbt/__init__.py
--rw-r--r--   0        0        0     2360 2023-05-19 22:32:03.917137 tap_dbt-0.6.0a1/tap_dbt/client.py
--rw-r--r--   0        0        0     1780 2023-05-19 22:32:03.917137 tap_dbt-0.6.0a1/tap_dbt/schemas/accounts.json
--rw-r--r--   0        0        0     2264 2023-05-19 22:32:03.917137 tap_dbt-0.6.0a1/tap_dbt/schemas/jobs.json
--rw-r--r--   0        0        0     1821 2023-05-19 22:32:03.917137 tap_dbt-0.6.0a1/tap_dbt/schemas/projects.json
--rw-r--r--   0        0        0     3368 2023-05-19 22:32:03.917137 tap_dbt-0.6.0a1/tap_dbt/schemas/runs.json
--rw-r--r--   0        0        0     3538 2023-05-19 22:32:03.917137 tap_dbt-0.6.0a1/tap_dbt/streams.py
--rw-r--r--   0        0        0     2033 2023-05-19 22:32:03.917137 tap_dbt-0.6.0a1/tap_dbt/tap.py
--rw-r--r--   0        0        0     5795 1970-01-01 00:00:00.000000 tap_dbt-0.6.0a1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-02 17:06:15.377086 tap_dbt-0.7.0/LICENSE
+-rw-r--r--   0        0        0     7180 2023-06-02 17:06:15.377086 tap_dbt-0.7.0/README.md
+-rw-r--r--   0        0        0     1654 2023-06-02 17:06:35.809497 tap_dbt-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0       40 2023-06-02 17:06:15.377086 tap_dbt-0.7.0/tap_dbt/__init__.py
+-rw-r--r--   0        0        0     2333 2023-06-02 17:06:15.377086 tap_dbt-0.7.0/tap_dbt/client.py
+-rw-r--r--   0        0        0     1780 2023-06-02 17:06:15.377086 tap_dbt-0.7.0/tap_dbt/schemas/accounts.json
+-rw-r--r--   0        0        0     2264 2023-06-02 17:06:15.377086 tap_dbt-0.7.0/tap_dbt/schemas/jobs.json
+-rw-r--r--   0        0        0     1821 2023-06-02 17:06:15.377086 tap_dbt-0.7.0/tap_dbt/schemas/projects.json
+-rw-r--r--   0        0        0     3368 2023-06-02 17:06:15.377086 tap_dbt-0.7.0/tap_dbt/schemas/runs.json
+-rw-r--r--   0        0        0     6900 2023-06-02 17:06:15.377086 tap_dbt-0.7.0/tap_dbt/streams.py
+-rw-r--r--   0        0        0     2230 2023-06-02 17:06:15.377086 tap_dbt-0.7.0/tap_dbt/tap.py
+-rw-r--r--   0        0        0     8074 1970-01-01 00:00:00.000000 tap_dbt-0.7.0/PKG-INFO
```

### Comparing `tap_dbt-0.6.0a1/LICENSE` & `tap_dbt-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_dbt-0.6.0a1/pyproject.toml` & `tap_dbt-0.7.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 [build-system]
-requires = ["poetry-core==1.6.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
+requires = [
+  "poetry-core==1.6",
+  "poetry-dynamic-versioning",
+]
 
 [tool.poetry]
 name = "tap-dbt"
-version = "0.6.0a1"
+version = "0.7.0"
 description = "Singer tap for dbt, built with the Singer SDK."
 license = "Apache-2.0"
 authors = ["Edgar Ramírez Mondragón <edgarrm358@sample.com>"]
 maintainers = ["Edgar Ramírez Mondragón <edgarrm358@sample.com>"]
 readme = "README.md"
 repository = "https://github.com/edgarrmondragon/tap-dbt"
 keywords = ["singer.io", "elt", "dbt", "singer-sdk"]
```

### Comparing `tap_dbt-0.6.0a1/tap_dbt/client.py` & `tap_dbt-0.7.0/tap_dbt/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,14 @@
     return yaml.safe_load(response.text)
 
 
 class DBTStream(RESTStream):
     """dbt stream class."""
 
     primary_keys = ["id"]
-    replication_key = None
     records_jsonpath = "$.data[*]"
 
     @property
     def url_base(self) -> str:
         """Base URL for this stream."""
         return self.config.get("base_url", "https://cloud.getdbt.com/api/v2")
```

### Comparing `tap_dbt-0.6.0a1/tap_dbt/schemas/accounts.json` & `tap_dbt-0.7.0/tap_dbt/schemas/accounts.json`

 * *Files identical despite different names*

### Comparing `tap_dbt-0.6.0a1/tap_dbt/schemas/jobs.json` & `tap_dbt-0.7.0/tap_dbt/schemas/jobs.json`

 * *Files identical despite different names*

### Comparing `tap_dbt-0.6.0a1/tap_dbt/schemas/projects.json` & `tap_dbt-0.7.0/tap_dbt/schemas/projects.json`

 * *Files identical despite different names*

### Comparing `tap_dbt-0.6.0a1/tap_dbt/schemas/runs.json` & `tap_dbt-0.7.0/tap_dbt/schemas/runs.json`

 * *Files identical despite different names*

### Comparing `tap_dbt-0.6.0a1/tap_dbt/tap.py` & `tap_dbt-0.7.0/tap_dbt/tap.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,22 +8,35 @@
     ArrayType,
     IntegerType,
     PropertiesList,
     Property,
     StringType,
 )
 
-from tap_dbt.streams import AccountsStream, JobsStream, ProjectsStream, RunsStream
+from tap_dbt.streams import (
+    AccountsStream,
+    ConnectionsStream,
+    EnvironmentsStream,
+    JobsStream,
+    ProjectsStream,
+    RepositoriesStream,
+    RunsStream,
+    UsersStream,
+)
 
 TAP_NAME = "tap-dbt"
 STREAM_TYPES = [
     AccountsStream,
+    ConnectionsStream,
+    EnvironmentsStream,
     JobsStream,
     ProjectsStream,
+    RepositoriesStream,
     RunsStream,
+    UsersStream,
 ]
 
 
 class TapDBT(Tap):
     """Singer tap for the dbt Cloud API."""
 
     name = TAP_NAME
```

### Comparing `tap_dbt-0.6.0a1/PKG-INFO` & `tap_dbt-0.7.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,12 @@
-Metadata-Version: 2.1
-Name: tap-dbt
-Version: 0.6.0a1
-Summary: Singer tap for dbt, built with the Singer SDK.
-Home-page: https://github.com/edgarrmondragon/tap-dbt
-License: Apache-2.0
-Keywords: singer.io,elt,dbt,singer-sdk
-Author: Edgar Ramírez Mondragón
-Author-email: edgarrm358@sample.com
-Maintainer: Edgar Ramírez Mondragón
-Maintainer-email: edgarrm358@sample.com
-Requires-Python: >=3.7.1,<3.12
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pyyaml (>=6.0,<7.0)
-Requires-Dist: singer-sdk (==0.27.0)
-Project-URL: Repository, https://github.com/edgarrmondragon/tap-dbt
-Description-Content-Type: text/markdown
-
 # tap-dbt
 
 [![PyPI](https://img.shields.io/pypi/v/tap-dbt.svg?color=blue)](https://pypi.org/project/tap-dbt/)
 [![Python versions](https://img.shields.io/pypi/pyversions/tap-dbt.svg)](https://pypi.org/project/tap-dbt/)
 [![Singer](https://img.shields.io/badge/Singer-Tap-purple.svg)](https://hub.meltano.com/taps/dbt)
-[![TestPyPI](https://github.com/edgarrmondragon/tap-dbt/actions/workflows/test-pypi.yml/badge.svg)](https://github.com/edgarrmondragon/tap-dbt/actions/workflows/test-pypi.yml)
 [![Test Tap](https://github.com/edgarrmondragon/tap-dbt/actions/workflows/test-tap.yml/badge.svg)](https://github.com/edgarrmondragon/tap-dbt/actions/workflows/test-tap.yml)
 
 `tap-dbt` is a Singer tap for the [dbt Cloud API v2][dbtcloud].
 
 Built with the [Singer SDK][sdk].
 
 - [Installation](#Installation)
@@ -48,19 +24,59 @@
 
 ```shell
 pip install tap-dbt
 ```
 
 ## Features
 
+### Streams
+
+Full stream metadata is available in the dbt Labs repository: [openapi_schema]
+
+#### Selected by default
+The following will be extracted by default if no catalog is used:
+
 - [x] Stream: accounts
-- [x] Stream: projects
 - [x] Stream: jobs
+- [x] Stream: projects
 - [x] Stream: runs
-- [ ] Incremental streams
+
+
+#### Configurable
+Can be enabled by setting `selected` in the catalog:
+
+- [x] Stream: connections
+- [x] Stream: environments
+- [x] Stream: repositories
+- [x] Stream: users
+
+
+### Incremental Run Stream
+
+Ordering the query from the Runs endpoint by `-finished_at`, i.e. descending Run Finished Datetime, yields:
+
+|id|finished_at|updated_at|created_at|
+|---|---|---|---|
+|314516|None|2023-05-27 21:05:16.109548+00:00|2023-05-27 21:05:05.664170+00:00|
+|314514|None|2023-05-27 21:00:16.847296+00:00|2023-05-27 21:00:05.458908+00:00|
+|314513|None|2023-05-27 21:00:16.355680+00:00|2023-05-27 21:00:05.427258+00:00|
+|314517|None|2023-05-27 21:05:17.094309+00:00|2023-05-27 21:05:05.696222+00:00|
+|314515|2023-05-27 21:01:28.568431+00:00|2023-05-27 21:01:29.269048+00:00|2023-05-27 21:00:05.488543+00:00|
+|314512|2023-05-27 20:48:59.342035+00:00|2023-05-27 20:48:59.844412+00:00|2023-05-27 20:45:04.509746+00:00|
+|314511|2023-05-27 20:48:46.571106+00:00|2023-05-27 20:48:47.079130+00:00|2023-05-27 20:40:04.257950+00:00|
+|314505|2023-05-27 20:41:35.591976+00:00|2023-05-27 20:41:36.305364+00:00|2023-05-27 20:15:02.808079+00:00|
+|314510|2023-05-27 20:39:27.162437+00:00|2023-05-27 20:39:28.628257+00:00|2023-05-27 20:35:03.939439+00:00|
+|314509|2023-05-27 20:37:39.965974+00:00|2023-05-27 20:37:40.496212+00:00|2023-05-27 20:30:03.802620+00:00|
+
+The incremental sync has been set up so that it works on `replication_key = "finished_at"`, when an INCREMENTAL sync is run:
+
+- If the bookmark is set, the stream is queried in reverse `finished_at` order.
+- If the `finished_at` value is not set, the run is assumed to still be running so the record is included, plus the sort order implies that there should be records with populated `finished_at` appearing later in the stream - *Repeated sync operation will yield the same records if the dbt Job Run is still underway, however this adheres to the 'at least once' delivery promise - https://sdk.meltano.com/en/latest/implementation/at_least_once.html*
+- Once the sync operation reaches records with populated `finished_at`, the values are compared with the bookmark and once the `finished_at` value becomes less than the bookmark the stream finishes syncing.
+
 
 ## Configuration
 
 Visit the [API docs][apidocs] for instructions on how to get your API key.
 
 You can pass configuration using environment variables with the `TAP_DBT_` prefix followed by the uppercased field name
 
@@ -166,8 +182,8 @@
 meltano elt tap-dbt target-snowflake --job_id dbt_snowflake
 ```
 
 [dbtcloud]: https://cloud.getdbt.com
 [sdk]: https://gitlab.com/meltano/singer-sdk
 [apidocs]: https://docs.getdbt.com/dbt-cloud/api#section/Authentication
 [meltano]: https://www.meltano.com
-
+[openapi_schema]: https://github.com/dbt-labs/dbt-cloud-openapi-spec/blob/master/openapi-v3.yaml
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

