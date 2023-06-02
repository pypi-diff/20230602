# Comparing `tmp/saagieapi-2.4.1.tar.gz` & `tmp/saagieapi-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saagieapi-2.4.1.tar", max compression
+gzip compressed data, was "saagieapi-2.5.0.tar", max compression
```

## Comparing `saagieapi-2.4.1.tar` & `saagieapi-2.5.0.tar`

### file list

```diff
@@ -1,37 +1,44 @@
--rw-r--r--   0        0        0    11357 2023-04-18 13:00:45.947220 saagieapi-2.4.1/LICENSE
--rw-r--r--   0        0        0     4555 2023-04-18 13:00:45.947220 saagieapi-2.4.1/README.md
--rw-r--r--   0        0        0     1562 2023-04-18 13:01:22.735811 saagieapi-2.4.1/pyproject.toml
--rw-r--r--   0        0        0      502 2023-04-18 13:00:45.951220 saagieapi-2.4.1/saagieapi/__init__.py
--rw-r--r--   0        0        0       43 2023-04-18 13:00:45.951220 saagieapi-2.4.1/saagieapi/apps/__init__.py
--rw-r--r--   0        0        0    33369 2023-04-18 13:00:45.951220 saagieapi-2.4.1/saagieapi/apps/apps.py
--rw-r--r--   0        0        0     7591 2023-04-18 13:00:45.951220 saagieapi-2.4.1/saagieapi/apps/gql_queries.py
--rw-r--r--   0        0        0       83 2023-04-18 13:00:45.951220 saagieapi-2.4.1/saagieapi/docker_credentials/__init__.py
--rw-r--r--   0        0        0     8465 2023-04-18 13:00:45.951220 saagieapi-2.4.1/saagieapi/docker_credentials/docker_credentials.py
--rw-r--r--   0        0        0     1657 2023-04-18 13:00:45.951220 saagieapi-2.4.1/saagieapi/docker_credentials/gql_queries.py
--rw-r--r--   0        0        0       53 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/env_vars/__init__.py
--rw-r--r--   0        0        0    27280 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/env_vars/env_vars.py
--rw-r--r--   0        0        0     2671 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/env_vars/gql_queries.py
--rw-r--r--   0        0        0     2414 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/gql_queries.py
--rw-r--r--   0        0        0       43 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/jobs/__init__.py
--rw-r--r--   0        0        0     9510 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/jobs/gql_queries.py
--rw-r--r--   0        0        0    36314 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/jobs/jobs.py
--rw-r--r--   0        0        0      141 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/pipelines/__init__.py
--rw-r--r--   0        0        0     7785 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/pipelines/gql_queries.py
--rw-r--r--   0        0        0     2384 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/pipelines/graph_pipeline.py
--rw-r--r--   0        0        0    29262 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/pipelines/pipelines.py
--rw-r--r--   0        0        0       55 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/projects/__init__.py
--rw-r--r--   0        0        0     2962 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/projects/gql_queries.py
--rw-r--r--   0        0        0    24404 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/projects/projects.py
--rw-r--r--   0        0        0       67 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/repositories/__init__.py
--rw-r--r--   0        0        0     8443 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/repositories/gql_queries.py
--rw-r--r--   0        0        0    10534 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/repositories/repositories.py
--rw-r--r--   0        0        0    14653 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/saagie_api.py
--rw-r--r--   0        0        0       55 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/storages/__init__.py
--rw-r--r--   0        0        0     1384 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/storages/gql_queries.py
--rw-r--r--   0        0        0     6561 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/storages/storages.py
--rw-r--r--   0        0        0        0 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/utils/__init__.py
--rw-r--r--   0        0        0     1725 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/utils/bearer_auth.py
--rw-r--r--   0        0        0     3969 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/utils/folder_functions.py
--rw-r--r--   0        0        0     3113 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/utils/gql_client.py
--rw-r--r--   0        0        0       54 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/utils/rich_console.py
--rw-r--r--   0        0        0     5504 1970-01-01 00:00:00.000000 saagieapi-2.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-02 14:47:33.139649 saagieapi-2.5.0/LICENSE
+-rw-r--r--   0        0        0     4555 2023-06-02 14:47:33.139649 saagieapi-2.5.0/README.md
+-rw-r--r--   0        0        0     1562 2023-06-02 14:48:02.680101 saagieapi-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0      502 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/__init__.py
+-rw-r--r--   0        0        0       43 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/apps/__init__.py
+-rw-r--r--   0        0        0    33369 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/apps/apps.py
+-rw-r--r--   0        0        0     7591 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/apps/gql_queries.py
+-rw-r--r--   0        0        0       83 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/docker_credentials/__init__.py
+-rw-r--r--   0        0        0     8465 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/docker_credentials/docker_credentials.py
+-rw-r--r--   0        0        0     1657 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/docker_credentials/gql_queries.py
+-rw-r--r--   0        0        0       53 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/env_vars/__init__.py
+-rw-r--r--   0        0        0    27280 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/env_vars/env_vars.py
+-rw-r--r--   0        0        0     2671 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/env_vars/gql_queries.py
+-rw-r--r--   0        0        0     2414 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/gql_queries.py
+-rw-r--r--   0        0        0       49 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/groups/__init__.py
+-rw-r--r--   0        0        0    14568 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/groups/groups.py
+-rw-r--r--   0        0        0       43 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/jobs/__init__.py
+-rw-r--r--   0        0        0     9510 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/jobs/gql_queries.py
+-rw-r--r--   0        0        0    36314 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/jobs/jobs.py
+-rw-r--r--   0        0        0      141 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/pipelines/__init__.py
+-rw-r--r--   0        0        0     7785 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/pipelines/gql_queries.py
+-rw-r--r--   0        0        0     2384 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/pipelines/graph_pipeline.py
+-rw-r--r--   0        0        0    29262 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/pipelines/pipelines.py
+-rw-r--r--   0        0        0       55 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/profiles/__init__.py
+-rw-r--r--   0        0        0     4954 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/profiles/profiles.py
+-rw-r--r--   0        0        0       55 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/projects/__init__.py
+-rw-r--r--   0        0        0     2962 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/projects/gql_queries.py
+-rw-r--r--   0        0        0    24404 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/projects/projects.py
+-rw-r--r--   0        0        0       67 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/repositories/__init__.py
+-rw-r--r--   0        0        0     8443 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/repositories/gql_queries.py
+-rw-r--r--   0        0        0    10534 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/repositories/repositories.py
+-rw-r--r--   0        0        0    15082 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/saagie_api.py
+-rw-r--r--   0        0        0       55 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/storages/__init__.py
+-rw-r--r--   0        0        0     1384 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/storages/gql_queries.py
+-rw-r--r--   0        0        0     6561 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/storages/storages.py
+-rw-r--r--   0        0        0       46 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/users/__init__.py
+-rw-r--r--   0        0        0    10891 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/users/users.py
+-rw-r--r--   0        0        0        0 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/utils/__init__.py
+-rw-r--r--   0        0        0     1725 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/utils/bearer_auth.py
+-rw-r--r--   0        0        0     3969 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/utils/folder_functions.py
+-rw-r--r--   0        0        0     3113 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/utils/gql_client.py
+-rw-r--r--   0        0        0     2336 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/utils/request_client.py
+-rw-r--r--   0        0        0       54 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/utils/rich_console.py
+-rw-r--r--   0        0        0     5504 1970-01-01 00:00:00.000000 saagieapi-2.5.0/PKG-INFO
```

### Comparing `saagieapi-2.4.1/LICENSE` & `saagieapi-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `saagieapi-2.4.1/README.md` & `saagieapi-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `saagieapi-2.4.1/pyproject.toml` & `saagieapi-2.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "saagieapi"
-version = "2.4.1"
+version = "2.5.0"
 description = "Python API to interact with Saagie"
 authors = ["Saagie"]
 license = "GLWTPL"
 readme = "README.md"
 repository = "https://github.com/saagie/api-saagie"
 
 [tool.poetry.dependencies]
```

### Comparing `saagieapi-2.4.1/saagieapi/apps/apps.py` & `saagieapi-2.5.0/saagieapi/apps/apps.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.4.1/saagieapi/apps/gql_queries.py` & `saagieapi-2.5.0/saagieapi/apps/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.4.1/saagieapi/docker_credentials/docker_credentials.py` & `saagieapi-2.5.0/saagieapi/docker_credentials/docker_credentials.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.4.1/saagieapi/docker_credentials/gql_queries.py` & `saagieapi-2.5.0/saagieapi/docker_credentials/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.4.1/saagieapi/env_vars/env_vars.py` & `saagieapi-2.5.0/saagieapi/env_vars/env_vars.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.4.1/saagieapi/env_vars/gql_queries.py` & `saagieapi-2.5.0/saagieapi/env_vars/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.4.1/saagieapi/gql_queries.py` & `saagieapi-2.5.0/saagieapi/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.4.1/saagieapi/jobs/gql_queries.py` & `saagieapi-2.5.0/saagieapi/jobs/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.4.1/saagieapi/jobs/jobs.py` & `saagieapi-2.5.0/saagieapi/jobs/jobs.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.4.1/saagieapi/pipelines/gql_queries.py` & `saagieapi-2.5.0/saagieapi/pipelines/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.4.1/saagieapi/pipelines/graph_pipeline.py` & `saagieapi-2.5.0/saagieapi/pipelines/graph_pipeline.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.4.1/saagieapi/pipelines/pipelines.py` & `saagieapi-2.5.0/saagieapi/pipelines/pipelines.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.4.1/saagieapi/projects/gql_queries.py` & `saagieapi-2.5.0/saagieapi/projects/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.4.1/saagieapi/projects/projects.py` & `saagieapi-2.5.0/saagieapi/projects/projects.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.4.1/saagieapi/repositories/gql_queries.py` & `saagieapi-2.5.0/saagieapi/repositories/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.4.1/saagieapi/repositories/repositories.py` & `saagieapi-2.5.0/saagieapi/repositories/repositories.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.4.1/saagieapi/saagie_api.py` & `saagieapi-2.5.0/saagieapi/saagie_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,21 +6,25 @@
 from croniter import croniter
 from gql import gql
 
 from .apps import Apps
 from .docker_credentials import DockerCredentials
 from .env_vars import EnvVars
 from .gql_queries import GQL_GET_CLUSTER_INFO, GQL_GET_PLATFORM_INFO, GQL_GET_REPOSITORIES_INFO, GQL_GET_RUNTIMES
+from .groups import Groups
 from .jobs import Jobs
 from .pipelines import Pipelines
+from .profiles import Profiles
 from .projects import Projects
 from .repositories import Repositories
 from .storages import Storages
+from .users import Users
 from .utils.bearer_auth import BearerAuth
 from .utils.gql_client import GqlClient
+from .utils.request_client import RequestClient
 
 
 class SaagieApi:
     # pylint: disable=too-many-instance-attributes
     """Define several methods to interact with Saagie API in Python"""
 
     def __init__(
@@ -51,15 +55,18 @@
         pprint_global : bool
             Change the default pprint of all the requests made with this client
         """
         if not url_saagie.endswith("/"):
             url_saagie += "/"
 
         self.url_saagie = url_saagie
-        self.auth = BearerAuth(realm=realm, url=self.url_saagie, platform=id_platform, login=user, password=password)
+        self.realm = realm
+        self.auth = BearerAuth(
+            realm=self.realm, url=self.url_saagie, platform=id_platform, login=user, password=password
+        )
         logging.info("✅ Successfully connected to your platform %s", self.url_saagie)
         url_api = f"{self.url_saagie}projects/api/platform/{str(id_platform)}/graphql"
         self.client = GqlClient(auth=self.auth, api_endpoint=url_api, retries=retries)
 
         url_gateway = f"{self.url_saagie}gateway/api/graphql"
         self.client_gateway = GqlClient(auth=self.auth, api_endpoint=url_gateway, retries=retries)
 
@@ -67,17 +74,22 @@
         self.jobs = Jobs(self)
         self.pipelines = Pipelines(self)
         self.env_vars = EnvVars(self)
         self.apps = Apps(self)
         self.docker_credentials = DockerCredentials(self)
         self.repositories = Repositories(self)
         self.storages = Storages(self)
+        self.users = Users(self)
+        self.groups = Groups(self)
+        self.profiles = Profiles(self)
         self.pprint_global = pprint_global
         self.client.pprint_global = pprint_global
         self.client_gateway.pprint_global = pprint_global
+        self.verify_ssl = True
+        self.request_client = RequestClient(auth=self.auth, realm=self.realm, verify_ssl=self.verify_ssl)
 
     @classmethod
     def easy_connect(cls, url_saagie_platform: str, user: str, password: str):
         """
         Alternative constructor which uses the complete URL (eg:
         https://saagie-workspace.prod.saagie.io/projects/platform/6/) and will
         parse it in order to retrieve the platform URL, platform id and the
```

### Comparing `saagieapi-2.4.1/saagieapi/storages/gql_queries.py` & `saagieapi-2.5.0/saagieapi/storages/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.4.1/saagieapi/storages/storages.py` & `saagieapi-2.5.0/saagieapi/storages/storages.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.4.1/saagieapi/utils/bearer_auth.py` & `saagieapi-2.5.0/saagieapi/utils/bearer_auth.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.4.1/saagieapi/utils/folder_functions.py` & `saagieapi-2.5.0/saagieapi/utils/folder_functions.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.4.1/saagieapi/utils/gql_client.py` & `saagieapi-2.5.0/saagieapi/utils/gql_client.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.4.1/PKG-INFO` & `saagieapi-2.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saagieapi
-Version: 2.4.1
+Version: 2.5.0
 Summary: Python API to interact with Saagie
 Home-page: https://github.com/saagie/api-saagie
 License: GLWTPL
 Author: Saagie
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

