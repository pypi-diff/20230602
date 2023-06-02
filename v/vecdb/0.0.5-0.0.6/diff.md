# Comparing `tmp/vecdb-0.0.5.tar.gz` & `tmp/vecdb-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vecdb-0.0.5.tar", last modified: Mon May 15 23:58:46 2023, max compression
+gzip compressed data, was "vecdb-0.0.6.tar", last modified: Fri Jun  2 20:12:27 2023, max compression
```

## Comparing `vecdb-0.0.5.tar` & `vecdb-0.0.6.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:46.238985 vecdb-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-05-15 23:58:26.000000 vecdb-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-15 23:58:46.238985 vecdb-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-05-15 23:58:26.000000 vecdb-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-15 23:58:26.000000 vecdb-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 23:58:46.238985 vecdb-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-15 23:58:26.000000 vecdb-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:46.234985 vecdb-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:26.000000 vecdb-0.0.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-05-15 23:58:26.000000 vecdb-0.0.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:46.234985 vecdb-0.0.5/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:26.000000 vecdb-0.0.5/tests/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:46.234985 vecdb-0.0.5/tests/core/test_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:26.000000 vecdb-0.0.5/tests/core/test_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-15 23:58:26.000000 vecdb-0.0.5/tests/core/test_api/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-15 23:58:26.000000 vecdb-0.0.5/tests/core/test_api/test_endpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:46.234985 vecdb-0.0.5/tests/core/test_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:26.000000 vecdb-0.0.5/tests/core/test_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-05-15 23:58:26.000000 vecdb-0.0.5/tests/core/test_dataset/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-15 23:58:26.000000 vecdb-0.0.5/tests/core/test_dataset/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-15 23:58:26.000000 vecdb-0.0.5/tests/test_connection_retry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:46.234985 vecdb-0.0.5/vecdb/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-15 23:58:26.000000 vecdb-0.0.5/vecdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:46.234985 vecdb-0.0.5/vecdb/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:26.000000 vecdb-0.0.5/vecdb/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16922 2023-05-15 23:58:26.000000 vecdb-0.0.5/vecdb/api/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-15 23:58:26.000000 vecdb-0.0.5/vecdb/api/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-05-15 23:58:26.000000 vecdb-0.0.5/vecdb/api/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:46.234985 vecdb-0.0.5/vecdb/collections/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:26.000000 vecdb-0.0.5/vecdb/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11210 2023-05-15 23:58:26.000000 vecdb-0.0.5/vecdb/collections/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-05-15 23:58:26.000000 vecdb-0.0.5/vecdb/collections/field.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-15 23:58:26.000000 vecdb-0.0.5/vecdb/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-15 23:58:26.000000 vecdb-0.0.5/vecdb/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-15 23:58:26.000000 vecdb-0.0.5/vecdb/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:46.238985 vecdb-0.0.5/vecdb/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:26.000000 vecdb-0.0.5/vecdb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14246 2023-05-15 23:58:26.000000 vecdb-0.0.5/vecdb/utils/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-05-15 23:58:26.000000 vecdb-0.0.5/vecdb/utils/example_documents.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-15 23:58:26.000000 vecdb-0.0.5/vecdb/utils/json_encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:46.234985 vecdb-0.0.5/vecdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-15 23:58:46.000000 vecdb-0.0.5/vecdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-15 23:58:46.000000 vecdb-0.0.5/vecdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 23:58:46.000000 vecdb-0.0.5/vecdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-15 23:58:46.000000 vecdb-0.0.5/vecdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-15 23:58:46.000000 vecdb-0.0.5/vecdb.egg-info/top_level.txt
+drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-02 20:12:27.324248 vecdb-0.0.6/
+-rw-r--r--   0 jackykoh   (502) staff       (20)    11346 2023-06-02 17:34:02.000000 vecdb-0.0.6/LICENSE
+-rw-r--r--   0 jackykoh   (502) staff       (20)      208 2023-06-02 20:12:27.324099 vecdb-0.0.6/PKG-INFO
+-rw-r--r--   0 jackykoh   (502) staff       (20)     2720 2023-06-02 17:34:02.000000 vecdb-0.0.6/README.md
+-rw-r--r--   0 jackykoh   (502) staff       (20)      128 2023-06-02 17:34:02.000000 vecdb-0.0.6/pyproject.toml
+-rw-r--r--   0 jackykoh   (502) staff       (20)       38 2023-06-02 20:12:27.324286 vecdb-0.0.6/setup.cfg
+-rw-r--r--   0 jackykoh   (502) staff       (20)      634 2023-06-02 17:56:53.000000 vecdb-0.0.6/setup.py
+drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-02 20:12:27.319348 vecdb-0.0.6/tests/
+-rw-r--r--   0 jackykoh   (502) staff       (20)        0 2023-06-02 17:34:02.000000 vecdb-0.0.6/tests/__init__.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     3717 2023-06-02 17:34:02.000000 vecdb-0.0.6/tests/conftest.py
+drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-02 20:12:27.319497 vecdb-0.0.6/tests/core/
+-rw-r--r--   0 jackykoh   (502) staff       (20)        0 2023-06-02 17:34:02.000000 vecdb-0.0.6/tests/core/__init__.py
+drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-02 20:12:27.319981 vecdb-0.0.6/tests/core/test_api/
+-rw-r--r--   0 jackykoh   (502) staff       (20)        0 2023-06-02 17:34:02.000000 vecdb-0.0.6/tests/core/test_api/__init__.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1563 2023-06-02 18:16:19.000000 vecdb-0.0.6/tests/core/test_api/test_client.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)      320 2023-06-02 17:34:02.000000 vecdb-0.0.6/tests/core/test_api/test_endpoints.py
+drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-02 20:12:27.320477 vecdb-0.0.6/tests/core/test_dataset/
+-rw-r--r--   0 jackykoh   (502) staff       (20)        0 2023-06-02 17:34:02.000000 vecdb-0.0.6/tests/core/test_dataset/__init__.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     5691 2023-06-02 17:34:02.000000 vecdb-0.0.6/tests/core/test_dataset/test_dataset.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)      708 2023-06-02 17:34:02.000000 vecdb-0.0.6/tests/core/test_dataset/test_field.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)      411 2023-06-02 17:34:02.000000 vecdb-0.0.6/tests/test_connection_retry.py
+drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-02 20:12:27.321289 vecdb-0.0.6/vecdb/
+-rw-r--r--   0 jackykoh   (502) staff       (20)      458 2023-06-02 18:03:17.000000 vecdb-0.0.6/vecdb/__init__.py
+drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-02 20:12:27.322725 vecdb-0.0.6/vecdb/api/
+-rw-r--r--   0 jackykoh   (502) staff       (20)        0 2023-06-02 17:34:02.000000 vecdb-0.0.6/vecdb/api/__init__.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)    14469 2023-06-02 17:35:55.000000 vecdb-0.0.6/vecdb/api/api.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)      208 2023-06-02 18:14:18.000000 vecdb-0.0.6/vecdb/api/helpers.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     3209 2023-06-02 18:48:17.000000 vecdb-0.0.6/vecdb/api/local.py
+drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-02 20:12:27.323258 vecdb-0.0.6/vecdb/collections/
+-rw-r--r--   0 jackykoh   (502) staff       (20)        0 2023-06-02 17:34:02.000000 vecdb-0.0.6/vecdb/collections/__init__.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)    11210 2023-06-02 17:34:02.000000 vecdb-0.0.6/vecdb/collections/dataset.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     7580 2023-06-02 17:34:02.000000 vecdb-0.0.6/vecdb/collections/field.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)      165 2023-06-02 18:10:07.000000 vecdb-0.0.6/vecdb/constants.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)       86 2023-06-02 17:34:02.000000 vecdb-0.0.6/vecdb/errors.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)      922 2023-06-02 18:05:53.000000 vecdb-0.0.6/vecdb/types.py
+drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-02 20:12:27.323899 vecdb-0.0.6/vecdb/utils/
+-rw-r--r--   0 jackykoh   (502) staff       (20)        0 2023-06-02 17:34:02.000000 vecdb-0.0.6/vecdb/utils/__init__.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)    14246 2023-06-02 17:34:02.000000 vecdb-0.0.6/vecdb/utils/document.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     3623 2023-06-02 17:38:21.000000 vecdb-0.0.6/vecdb/utils/example_documents.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     3235 2023-06-02 17:34:02.000000 vecdb-0.0.6/vecdb/utils/json_encoder.py
+drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-02 20:12:27.322004 vecdb-0.0.6/vecdb.egg-info/
+-rw-r--r--   0 jackykoh   (502) staff       (20)      208 2023-06-02 20:12:27.000000 vecdb-0.0.6/vecdb.egg-info/PKG-INFO
+-rw-r--r--   0 jackykoh   (502) staff       (20)      836 2023-06-02 20:12:27.000000 vecdb-0.0.6/vecdb.egg-info/SOURCES.txt
+-rw-r--r--   0 jackykoh   (502) staff       (20)        1 2023-06-02 20:12:27.000000 vecdb-0.0.6/vecdb.egg-info/dependency_links.txt
+-rw-r--r--   0 jackykoh   (502) staff       (20)      128 2023-06-02 20:12:27.000000 vecdb-0.0.6/vecdb.egg-info/requires.txt
+-rw-r--r--   0 jackykoh   (502) staff       (20)       12 2023-06-02 20:12:27.000000 vecdb-0.0.6/vecdb.egg-info/top_level.txt
```

### Comparing `vecdb-0.0.5/LICENSE` & `vecdb-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vecdb-0.0.5/README.md` & `vecdb-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `vecdb-0.0.5/setup.py` & `vecdb-0.0.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 test_requirements = ["pytest", "pytest-xdist", "pytest-cov"]
 
 chunk_requirements = ["fuzzysearch==0.7.3"]
 
 setup(
     name="vecdb",
     version=__version__,
-    url="https://relevanceai.com.au/",
+    url="https://relevanceai.com/",
     author="Relevance AI",
-    author_email="dev@tryrelevance.com",
+    author_email="jacky@relevanceai.com",
     packages=find_packages(),
     setup_requires=["wheel"],
     install_requires=requirements,
     package_data={"": ["*.ini"]},
     extras_require=dict(tests=test_requirements, chunk=chunk_requirements),
 )
```

### Comparing `vecdb-0.0.5/tests/conftest.py` & `vecdb-0.0.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `vecdb-0.0.5/tests/core/test_api/test_client.py` & `vecdb-0.0.6/tests/core/test_api/test_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 from vecdb.api.local import Client
 from vecdb.utils.example_documents import mock_documents
 
 
 class TestClient:
     def test_init(self):
-        vecdb.init(os.getenv("DEVELOPMENT_TOKEN"))
-        client = Client()
+        # vecdb.init(os.getenv("DEVELOPMENT_TOKEN"))
+        client = Client(os.getenv("DEVELOPMENT_TOKEN"))
         assert True
 
     def test_init_dataset(self, test_client: Client, test_dataset_id: str):
         test_client.create_dataset(test_dataset_id)
         test_client.delete_dataset(test_dataset_id)
         assert True
```

### Comparing `vecdb-0.0.5/tests/core/test_dataset/test_dataset.py` & `vecdb-0.0.6/tests/core/test_dataset/test_dataset.py`

 * *Files identical despite different names*

### Comparing `vecdb-0.0.5/tests/core/test_dataset/test_field.py` & `vecdb-0.0.6/tests/core/test_dataset/test_field.py`

 * *Files identical despite different names*

### Comparing `vecdb-0.0.5/vecdb/api/api.py` & `vecdb-0.0.6/vecdb/api/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -112,19 +112,24 @@
 
         return function_wrapper
 
     return _retry
 
 
 class API:
-    def __init__(self, credentials: Credentials, job_id: str = None, name: str = None) -> None:
+    def __init__(
+        self, credentials: Credentials, job_id: str = None, name: str = None
+    ) -> None:
         self._credentials = credentials
-        self._base_url = f"https://api-{self.credentials.region}.stack.tryrelevance.com/latest"
+        self._base_url = (
+            f"https://api-{self.credentials.region}.stack.tryrelevance.com/latest"
+        )
         self._headers = dict(
-            Authorization=f"{self.credentials.project}:{self.credentials.api_key}", vecdb_version=__version__
+            Authorization=f"{self.credentials.project}:{self.credentials.api_key}",
+            vecdb_version=__version__,
         )
         if job_id is not None:
             self.headers.update(vecdb_job_id=job_id)
         if name is not None:
             self.headers.update(vecdb_name=name)
 
         self.session = requests.Session()
@@ -138,16 +143,24 @@
         return self._base_url
 
     @property
     def headers(self) -> Dict[str, str]:
         return self._headers
 
     @retry()
-    def _request(self, method: Literal["GET", "POST"], suffix: str, *args, **kwargs) -> Response:
-        request = requests.Request(method=method, url=self.base_url + suffix, headers=self.headers, *args, **kwargs)
+    def _request(
+        self, method: Literal["GET", "POST"], suffix: str, *args, **kwargs
+    ) -> Response:
+        request = requests.Request(
+            method=method,
+            url=self.base_url + suffix,
+            headers=self.headers,
+            *args,
+            **kwargs,
+        )
         prepared_request = request.prepare()
 
         if LOG_REQUESTS:
             log_request(prepared_request)
 
         response = self.session.send(prepared_request)
 
@@ -163,18 +176,23 @@
         return self._request(method="POST", suffix=suffix, *args, **kwargs)
 
     def _list_datasets(self):
         response = self.get(suffix="/datasets/list")
         return get_response(response)
 
     def _create_dataset(
-        self, dataset_id: str, schema: Optional[Schema] = None, upsert: bool = True, expire: bool = False
+        self,
+        dataset_id: str,
+        schema: Optional[Schema] = None,
+        upsert: bool = True,
+        expire: bool = False,
     ) -> Any:
         response = self.post(
-            suffix=f"/datasets/create", json=dict(id=dataset_id, schema=schema, upsert=upsert, expire=expire)
+            suffix=f"/datasets/create",
+            json=dict(id=dataset_id, schema=schema, upsert=upsert, expire=expire),
         )
         return get_response(response)
 
     def _delete_dataset(self, dataset_id: str) -> Any:
         response = self.post(suffix=f"/datasets/{dataset_id}/delete")
         return get_response(response)
 
@@ -197,15 +215,17 @@
         response = self.post(
             suffix=f"/datasets/{dataset_id}/documents/bulk_insert",
             json=dict(
                 documents=documents,
                 insert_date=insert_date,
                 overwrite=overwrite,
                 update_schema=update_schema,
-                field_transformers=[] if field_transformers is None else field_transformers,
+                field_transformers=[]
+                if field_transformers is None
+                else field_transformers,
                 ingest_in_background=ingest_in_background,
                 wait_for_update=wait_for_update,
                 encoders=encoders if encoders else [],
             ),
         )
         return get_response(response)
 
@@ -253,94 +273,72 @@
             json["include_vector"] = include_vector
         if after_id:
             json["after_id"] = after_id
         if query:
             json["query"] = query
         if vector_search_query:
             json["vector_search_query"] = vector_search_query
-        response = self.post(suffix=f"/datasets/{dataset_id}/documents/get_where", json=json)
+        response = self.post(
+            suffix=f"/datasets/{dataset_id}/documents/get_where", json=json
+        )
         return get_response(response)
 
     def _delete_where(self, dataset_id: str, filters: Optional[List[Filter]] = None):
         response = self.post(
             suffix=f"/datasets/{dataset_id}/documents/delete_where",
             json=dict(filters=[] if filters is None else filters),
         )
         return get_response(response)
 
     def _update_dataset_metadata(self, dataset_id: str, metadata: Dict[str, Any]):
         """
         Edit and add metadata about a dataset. Notably description, data source, etc
         """
         response = self.post(
-            suffix=f"/datasets/{dataset_id}/metadata", json=dict(dataset_id=dataset_id, metadata=metadata)
+            suffix=f"/datasets/{dataset_id}/metadata",
+            json=dict(dataset_id=dataset_id, metadata=metadata),
         )
         return get_response(response)
 
     def _get_metadata(self, dataset_id: str) -> Dict[str, Any]:
         response = self.get(suffix=f"/datasets/{dataset_id}/metadata")
         return get_response(response)
 
-    def _insert_centroids(
-        self, dataset_id: str, cluster_centers: List[document.Document], vector_fields: List[str], alias: str
-    ):
-        response = self.post(
-            suffix=f"/datasets/{dataset_id}/cluster/centroids/insert",
-            json=dict(dataset_id=dataset_id, cluster_centers=cluster_centers, vector_fields=vector_fields, alias=alias),
-        )
-        return get_response(response)
-
-    def _get_centroids(
-        self,
-        dataset_id: str,
-        vector_fields: List[str],
-        alias: str,
-        page_size: int = 5,
-        page: int = 1,
-        cluster_ids: Optional[List] = None,
-        include_vector: bool = False,
-    ):
-        response = self.post(
-            suffix=f"/datasets/{dataset_id}/cluster/centroids/documents",
-            json=dict(
-                cluster_ids=[] if cluster_ids is None else cluster_ids,
-                vector_fields=vector_fields,
-                alias=alias,
-                page_size=min(9999, page_size),
-                page=page,
-                include_vector=include_vector,
-            ),
-        )
-        return get_response(response)
-
     def _get_health(self, dataset_id: str):
         response = self.get(suffix=f"/datasets/{dataset_id}/monitor/health")
         return get_response(response)
 
     def _get_workflow_status(self, job_id: str):
         response = self.post(suffix=f"/workflows/{job_id}/get")
         return get_response(response)
 
     def _update_workflow_metadata(self, job_id: str, metadata: Dict[str, Any]):
-        response = self.post(suffix=f"/workflows/{job_id}/metadata", json=dict(metadata=metadata))
+        response = self.post(
+            suffix=f"/workflows/{job_id}/metadata", json=dict(metadata=metadata)
+        )
         return get_response(response)
 
     def _get_file_upload_urls(self, dataset_id: str, files: List[str]):
-        response = self.post(suffix=f"/datasets/{dataset_id}/get_file_upload_urls", json=dict(files=files))
+        response = self.post(
+            suffix=f"/datasets/{dataset_id}/get_file_upload_urls",
+            json=dict(files=files),
+        )
         return get_response(response)
 
     def _get_temp_file_upload_url(self):
         """Use this for temporary file uploads.
         returns: {'download_url': ..., 'upload_url': ...}
         """
         response = self.post(suffix=f"/services/get_temporary_file_upload_url")
         return get_response(response)
 
     def _upload_temporary_media(self, presigned_url: str, media_content: bytes):
-        return requests.put(presigned_url, headers={"x-amz-tagging": "Expire=true"}, data=media_content)
+        return requests.put(
+            presigned_url, headers={"x-amz-tagging": "Expire=true"}, data=media_content
+        )
 
     def _upload_media(self, presigned_url: str, media_content: bytes):
         # dont use get response since response cannot be json decoded
         return requests.put(presigned_url, data=media_content)
 
     def _facets(
         self,
@@ -348,32 +346,44 @@
         fields: List[str],
         data_interval: str = "monthly",
         page_size: int = 1000,
         asc: bool = False,
     ):
         response = self.post(
             suffix=f"/datasets/{dataset_id}/facets",
-            json=dict(fields=fields, data_interval=data_interval, page_size=min(9999, page_size), asc=asc),
+            json=dict(
+                fields=fields,
+                data_interval=data_interval,
+                page_size=min(9999, page_size),
+                asc=asc,
+            ),
         )
         return get_response(response)
 
-    def _upsert_dataset_settings(self, dataset_id: str, settings: Optional[Dict[str, Any]] = None):
+    def _upsert_dataset_settings(
+        self, dataset_id: str, settings: Optional[Dict[str, Any]] = None
+    ):
         response = self.post(
-            suffix=f"/datasets/{dataset_id}/settings", json=dict(settings={} if settings is None else settings)
+            suffix=f"/datasets/{dataset_id}/settings",
+            json=dict(settings={} if settings is None else settings),
         )
         return get_response(response)
 
     def _get_dataset_settings(self, dataset_id: str):
         response = self.get(suffix=f"/datasets/{dataset_id}/settings")
         return get_response(response)
 
-    def _create_deployable(self, dataset_id: Optional[str] = None, config: Optional[Dict[str, Any]] = None):
+    def _create_deployable(
+        self, dataset_id: Optional[str] = None, config: Optional[Dict[str, Any]] = None
+    ):
         response = self.post(
             suffix="/deployables/create",
-            json=dict(dataset_id=dataset_id, configuration={} if config is None else config),
+            json=dict(
+                dataset_id=dataset_id, configuration={} if config is None else config
+            ),
         )
         return get_response(response)
 
     def _aggregate(
         self,
         dataset_id: str,
         page_size: str = 20,
@@ -393,77 +403,43 @@
                 asc=asc,
                 dataset_ids=[] if dataset_ids is None else dataset_ids,
                 dataset_id=dataset_id,
             ),
         )
         return get_response(response)
 
-    def _list_closest_to_center(
-        self,
-        dataset_id: str,
-        vector_fields: List[str],
-        alias: str,
-        approx: int = 0,
-        sum_fields: bool = True,
-        page: int = 1,
-        similarity_metric: str = "cosine",
-        min_score: float = 0,
-        include_vector: bool = False,
-        include_count: bool = True,
-        include_relevance: bool = False,
-        page_size: int = 20,
-        cluster_properties_filter: Dict[str, Any] = None,
-        cluster_ids: List[str] = None,
-        filters: List[Filter] = None,
-        select_fields: List[str] = None,
-    ):
-        response = self.post(
-            suffix=f"/datasets/{dataset_id}/cluster/centroids/list_closest_to_center",
-            json=dict(
-                vector_fields=vector_fields,
-                alias=alias,
-                approx=approx,
-                sum_fields=sum_fields,
-                page=page,
-                similarity_metric=similarity_metric,
-                min_score=min_score,
-                include_vector=include_vector,
-                include_count=include_count,
-                include_relevance=include_relevance,
-                page_size=min(9999, page_size),
-                cluster_properties_filter=cluster_properties_filter if cluster_properties_filter is not None else {},
-                filters=filters if filters is not None else [],
-                cluster_ids=cluster_ids if cluster_ids is not None else [],
-                select_fields=select_fields if select_fields is not None else [],
-            ),
-        )
-        return get_response(response)
-
     def _list_project_keys(self):
         response = self.get(suffix="/projects/keys/list")
         return get_response(response)
 
     def _get_project_key(self, key: str, token: str):
-        response = self.post(suffix="/projects/keys/get", json=dict(key=key, token=token))
+        response = self.post(
+            suffix="/projects/keys/get", json=dict(key=key, token=token)
+        )
         return get_response(response)
 
     def _set_project_key(self, key: str, value: str):
-        response = self.post(suffix="/projects/keys/set", json=dict(key=key, value=value))
+        response = self.post(
+            suffix="/projects/keys/set", json=dict(key=key, value=value)
+        )
         return get_response(response)
 
     def _delete_project_key(self, key: str):
         response = self.post(suffix="/projects/keys/delete", json=dict(key=key))
         return get_response(response)
 
-    def _update_version_aliases(self, development_version: str, production_version: str):
-        response = self.post(
-            suffix="/workflows/types/version_aliases/update",
-            json={"aliases": {"development_version": development_version, "production_version": production_version}},
-        )
-        return get_response(response)
-
-    def _search(self, dataset_id: str, query: str, page_size: int, filters: Optional[List[Filter]]):
+    def _search(
+        self,
+        dataset_id: str,
+        query: str,
+        page_size: int,
+        filters: Optional[List[Filter]],
+    ):
         response = self.post(
             suffix=f"/datasets/{dataset_id}/search",
-            json={"query": query, "pageSize": page_size, "filters": [] if filters is None else filters},
+            json={
+                "query": query,
+                "pageSize": page_size,
+                "filters": [] if filters is None else filters,
+            },
         )
         return get_response(response)
```

### Comparing `vecdb-0.0.5/vecdb/api/local.py` & `vecdb-0.0.6/vecdb/api/local.py`

 * *Files 8% similar despite different names*

```diff
@@ -81,18 +81,18 @@
 
     def set_project_key(self, key: str, value: str):
         return self.api._set_project_key(key=key, value=value)
 
     def delete_project_key(self, key: str):
         return self.api._delete_project_key(key=key)
 
-    def openai_completion(
-        self,
-        prompt: str,
-        model: str = "text-davinci-003",
-        workflows_admin_token: str = None,
-        max_tokens: int = 20,
-        temperature: float = 0.0,
-    ):
-        if workflows_admin_token is None:
-            workflows_admin_token = os.getenv("WORKFLOWS_ADMIN_TOKEN")
-        return self.api._openai_completion(workflows_admin_token, model, prompt, max_tokens, temperature)
+    # def openai_completion(
+    #     self,
+    #     prompt: str,
+    #     model: str = "text-davinci-003",
+    #     workflows_admin_token: str = None,
+    #     max_tokens: int = 20,
+    #     temperature: float = 0.0,
+    # ):
+    #     if workflows_admin_token is None:
+    #         workflows_admin_token = os.getenv("WORKFLOWS_ADMIN_TOKEN")
+    #     return self.api._openai_completion(workflows_admin_token, model, prompt, max_tokens, temperature)
```

### Comparing `vecdb-0.0.5/vecdb/collections/dataset.py` & `vecdb-0.0.6/vecdb/collections/dataset.py`

 * *Files identical despite different names*

### Comparing `vecdb-0.0.5/vecdb/collections/field.py` & `vecdb-0.0.6/vecdb/collections/field.py`

 * *Files identical despite different names*

### Comparing `vecdb-0.0.5/vecdb/types.py` & `vecdb-0.0.6/vecdb/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,19 +10,18 @@
 Schema = NewType("Schema", Dict[str, str])
 
 
 class Credentials(NamedTuple):
     project: str
     api_key: str
     region: str
-    firebase_uid: str
 
     @property
     def token(self):
-        return f"{self.project}:{self.api_key}:{self.region}:{self.firebase_uid}"
+        return f"{self.project}:{self.api_key}:{self.region}"
 
 
 GroupBy = NewType("GroupBy", List[Dict[str, Any]])
 Metric = NewType("Metric", List[Dict[str, Any]])
 
 EncoderModel = Literal[
     "image_text",
```

### Comparing `vecdb-0.0.5/vecdb/utils/document.py` & `vecdb-0.0.6/vecdb/utils/document.py`

 * *Files identical despite different names*

### Comparing `vecdb-0.0.5/vecdb/utils/example_documents.py` & `vecdb-0.0.6/vecdb/utils/example_documents.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,17 +47,19 @@
 
 
 def create_id():
     return str(uuid.uuid4())
 
 
 def generate_random_string(string_length: int = 5) -> str:
-
     """Generate a random string of letters and numbers"""
-    return "".join(random.choice(string.ascii_uppercase + string.digits) for _ in range(string_length))
+    return "".join(
+        random.choice(string.ascii_uppercase + string.digits)
+        for _ in range(string_length)
+    )
 
 
 def generate_random_vector(vector_length: int = 5) -> types.Vector:
     """Generate a random list of floats"""
     return [random.random() for _ in range(vector_length)]
 
 
@@ -81,25 +83,32 @@
             "sample_3_description": generate_random_string(),
             "sample_1_vector_": generate_random_vector(vector_length),
             "sample_2_vector_": generate_random_vector(vector_length),
             "sample_3_vector_": generate_random_vector(vector_length),
             "sample_1_value": generate_random_integer(),
             "sample_2_value": generate_random_integer(),
             "sample_3_value": generate_random_integer(),
-            "_chunk_": [{"label": generate_random_label(), "label_chunkvector_": generate_random_vector()}],
+            "_chunk_": [
+                {
+                    "label": generate_random_label(),
+                    "label_chunkvector_": generate_random_vector(),
+                }
+            ],
         }
     )
 
 
 def mock_documents(n: int = 100, vector_length: int = 5) -> document.DocumentList:
     return document.DocumentList([vector_document(vector_length) for _ in range(n)])
 
 
 def static_documents(n: int = 100) -> document.DocumentList:
-    return document.DocumentList([{"text_field": str(i), "numeric_field": i} for i in range(n)])
+    return document.DocumentList(
+        [{"text_field": str(i), "numeric_field": i} for i in range(n)]
+    )
 
 
 def tag_document(n_tags: int = 5):
     return document.Document(
         {
             "text": "This is some random text",
             "_surveytag_": {
```

### Comparing `vecdb-0.0.5/vecdb/utils/json_encoder.py` & `vecdb-0.0.6/vecdb/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `vecdb-0.0.5/vecdb.egg-info/SOURCES.txt` & `vecdb-0.0.6/vecdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

