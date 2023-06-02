# Comparing `tmp/coregio-0.1.0.tar.gz` & `tmp/coregio-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coregio-0.1.0.tar", last modified: Fri Jun  2 08:07:59 2023, max compression
+gzip compressed data, was "coregio-0.2.0.tar", last modified: Fri Jun  2 12:56:04 2023, max compression
```

## Comparing `coregio-0.1.0.tar` & `coregio-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 araszka   (1000) araszka   (1000)        0 2023-06-02 08:07:59.326168 coregio-0.1.0/
--rw-r--r--   0 araszka   (1000) araszka   (1000)      344 2023-06-02 08:07:59.326168 coregio-0.1.0/PKG-INFO
--rw-r--r--   0 araszka   (1000) araszka   (1000)       48 2023-06-02 07:57:11.000000 coregio-0.1.0/README.md
-drwxr-xr-x   0 araszka   (1000) araszka   (1000)        0 2023-06-02 08:07:59.325168 coregio-0.1.0/coregio.egg-info/
--rw-r--r--   0 araszka   (1000) araszka   (1000)      344 2023-06-02 08:07:59.000000 coregio-0.1.0/coregio.egg-info/PKG-INFO
--rw-r--r--   0 araszka   (1000) araszka   (1000)      335 2023-06-02 08:07:59.000000 coregio-0.1.0/coregio.egg-info/SOURCES.txt
--rw-r--r--   0 araszka   (1000) araszka   (1000)        1 2023-06-02 08:07:59.000000 coregio-0.1.0/coregio.egg-info/dependency_links.txt
--rw-r--r--   0 araszka   (1000) araszka   (1000)      180 2023-06-02 08:07:59.000000 coregio-0.1.0/coregio.egg-info/requires.txt
--rw-r--r--   0 araszka   (1000) araszka   (1000)        7 2023-06-02 08:07:59.000000 coregio-0.1.0/coregio.egg-info/top_level.txt
--rw-r--r--   0 araszka   (1000) araszka   (1000)      640 2023-06-02 08:07:54.000000 coregio-0.1.0/pyproject.toml
-drwxr-xr-x   0 araszka   (1000) araszka   (1000)        0 2023-06-02 08:07:59.326168 coregio-0.1.0/regapi/
--rw-r--r--   0 araszka   (1000) araszka   (1000)        0 2023-06-01 09:13:39.000000 coregio-0.1.0/regapi/__init__.py
--rw-r--r--   0 araszka   (1000) araszka   (1000)    14641 2023-06-02 07:58:50.000000 coregio-0.1.0/regapi/registry_api.py
--rw-r--r--   0 araszka   (1000) araszka   (1000)     5661 2023-06-01 15:20:47.000000 coregio-0.1.0/regapi/registry_auth.py
--rw-r--r--   0 araszka   (1000) araszka   (1000)     2175 2023-06-01 09:21:31.000000 coregio-0.1.0/regapi/utils.py
--rw-r--r--   0 araszka   (1000) araszka   (1000)       38 2023-06-02 08:07:59.326168 coregio-0.1.0/setup.cfg
-drwxr-xr-x   0 araszka   (1000) araszka   (1000)        0 2023-06-02 08:07:59.326168 coregio-0.1.0/tests/
--rw-r--r--   0 araszka   (1000) araszka   (1000)     8307 2023-06-02 07:58:51.000000 coregio-0.1.0/tests/test_registry_api.py
--rw-r--r--   0 araszka   (1000) araszka   (1000)      302 2023-06-02 07:58:50.000000 coregio-0.1.0/tests/test_registry_auth.py
--rw-r--r--   0 araszka   (1000) araszka   (1000)      457 2023-06-02 07:58:50.000000 coregio-0.1.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:56:04.118136 coregio-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-02 12:56:04.118136 coregio-0.2.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:56:04.114136 coregio-0.2.0/coregio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 12:55:54.000000 coregio-0.2.0/coregio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11821 2023-06-02 12:55:54.000000 coregio-0.2.0/coregio/registry_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-06-02 12:55:54.000000 coregio-0.2.0/coregio/registry_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-02 12:55:54.000000 coregio-0.2.0/coregio/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:56:04.114136 coregio-0.2.0/coregio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-02 12:56:04.000000 coregio-0.2.0/coregio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-02 12:56:04.000000 coregio-0.2.0/coregio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 12:56:04.000000 coregio-0.2.0/coregio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-02 12:56:04.000000 coregio-0.2.0/coregio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 12:56:04.000000 coregio-0.2.0/coregio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-02 12:55:54.000000 coregio-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 12:56:04.118136 coregio-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:56:04.118136 coregio-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-06-02 12:55:54.000000 coregio-0.2.0/tests/test_registry_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-02 12:55:54.000000 coregio-0.2.0/tests/test_registry_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-02 12:55:54.000000 coregio-0.2.0/tests/test_utils.py
```

### Comparing `coregio-0.1.0/pyproject.toml` & `coregio-0.2.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.pdm]
 
 [project]
 name = "coregio"
-version = "0.1.0"
+version = "0.2.0"
 description = "Python container registry API library."
 authors = [{ name = "Ales Raszka", email = "araszka@redhat.com" }]
 dependencies = []
 requires-python = ">=3.10"
 readme = "README.md"
 license = { text = "MIT" }
 [project.optional-dependencies]
```

### Comparing `coregio-0.1.0/regapi/registry_auth.py` & `coregio-0.2.0/coregio/registry_auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """Registry authentication module."""
 
-import os
 import re
 from urllib.parse import urlparse
 
 import requests
 from requests.auth import AuthBase
 from requests.cookies import extract_cookies_to_jar
 from requests.utils import parse_dict_header
 
 # This module comes from atomic-reactor
 # https://github.com/containerbuildsystem/atomic-reactor/blob/1.6.41/atomic_reactor/auth.py
 
 
-class HTTPBearerAuth(AuthBase):  # pragma: no cover
+class HTTPBearerAuth(AuthBase):
     """
     Performs Bearer authentication for the given Request object.
 
     username and password are optional. If provided, they will be used
     when fetching the Bearer token from realm. Otherwise, Bearer token
     is retrieved with anonymous access.
 
@@ -53,15 +52,15 @@
     def __call__(self, response):
         repo = self._get_repo_from_url(response.url)
 
         if repo in self.token_cache:
             self._set_header(response, repo)
             return response
 
-        def handle_401_with_repo(resp, **kwargs):
+        def handle_401_with_repo(resp, **kwargs):  # pragma: no cover
             return self.handle_401(resp, repo, **kwargs)
 
         response.register_hook("response", handle_401_with_repo)
         return response
 
     def handle_401(self, response, repo, **kwargs):
         """Fetch Bearer token and retry."""
@@ -102,19 +101,20 @@
             bearer_info["scope"] = f"repository:{repo}:{','.join(self.access)}"
         realm = bearer_info.pop("realm")
 
         realm_auth = None
         if self.auth_b64:
             realm_auth = HTTPBasicAuthWithB64(self.auth_b64)
 
-        registry_proxy = os.environ.get("EXTERNAL_REGISTRY_PROXY")
-        if registry_proxy:
-            proxies = {"https": registry_proxy}
-        else:
-            proxies = None
+        # registry_proxy = os.environ.get("EXTERNAL_REGISTRY_PROXY")
+        # if registry_proxy:
+        #     proxies = {"https": registry_proxy}
+        # else:
+        #     proxies = None
+        proxies = None
         realm_response = requests.get(
             realm,
             params=bearer_info,
             verify=self.verify,
             auth=realm_auth,
             proxies=proxies,
             timeout=60,
```

### Comparing `coregio-0.1.0/regapi/utils.py` & `coregio-0.2.0/coregio/utils.py`

 * *Files identical despite different names*

### Comparing `coregio-0.1.0/tests/test_registry_api.py` & `coregio-0.2.0/tests/test_registry_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 from typing import Any, Dict, Set
 from unittest.mock import MagicMock, patch
 
 import pytest
 import requests
 
-from regio.registry_api import (
-    ContainerRegistry,
-    get_manifest,
-    get_manifest_headers,
-    get_tags,
-)
+from coregio.registry_api import ContainerRegistry
 
 
 @pytest.mark.parametrize(
     ["registry", "cfg", "auth", "token"],
     [
         ("quay.io", None, None, None),
         ("quay.io", "qwe", None, None),
         ("quay.io", "{}", None, None),
         ("quay.io", "{}", {"auth": "Zm9vOmJhcg=="}, "Zm9vOmJhcg=="),
     ],
 )
 @patch(
-    "regio.registry_api.ContainerRegistry._select_registry_auth_token_from_docker_config"
+    "coregio.registry_api.ContainerRegistry._select_registry_auth_token_from_docker_config"
 )
 def test__get__get_auth_token(
     mock_select_token: MagicMock,
     registry: str,
     cfg: Any,
     auth: Any,
     token: Any,
@@ -64,15 +59,15 @@
     registry_api = ContainerRegistry(registry, "")
 
     token = registry_api._select_registry_auth_token_from_docker_config(docker_config)
 
     assert token == expected_token
 
 
-@patch("regio.registry_api.ContainerRegistry._get_auth_token")
+@patch("coregio.registry_api.ContainerRegistry._get_auth_token")
 def test__get_session(mock_auth_token: MagicMock) -> None:
     mock_auth_token.return_value = "Zm9vOmJhcg=="
     registry = ContainerRegistry("test-quay.io", "foo")
 
     mock_auth = MagicMock()
 
     def auth_method(token: Any) -> Any:
@@ -87,15 +82,15 @@
     ["status_codes"],
     [
         ((200,),),
         ((401, 200),),
         ((401, 401, 401),),
     ],
 )
-@patch("regio.registry_api.ContainerRegistry._get_session")
+@patch("coregio.registry_api.ContainerRegistry._get_session")
 def test__get(mock_session: MagicMock, status_codes: Set[int]) -> None:
     sessions = []
     for code in status_codes:
         expected_response = requests.Response()
         expected_response.status_code = code
 
         session = MagicMock()
@@ -104,44 +99,44 @@
     mock_session.side_effect = sessions
 
     registry = ContainerRegistry("test-quay.io", "foo")
     resp = registry._get("foo", {}, {}, True)
     assert resp.status_code == sessions[-1].get.return_value.status_code
 
 
-@patch("regio.utils.handle_response")
-@patch("regio.registry_api.ContainerRegistry._get")
+@patch("coregio.utils.handle_response")
+@patch("coregio.registry_api.ContainerRegistry._get")
 def test_get_request(
     mock_get: MagicMock,
     mock_handle: MagicMock,
     monkeypatch: Any,
 ) -> None:
     mock_handle.return_value = None
     resp = ContainerRegistry("foo", "bar").get_request("/v1/api")
     assert resp == mock_get.return_value
     mock_get.assert_called_once_with("https://foo/v1/api", params=None, headers=None)
 
 
-@patch("regio.registry_api.requests.Session.get")
-@patch("regio.registry_api.ContainerRegistry._get_session")
+@patch("coregio.registry_api.requests.Session.get")
+@patch("coregio.registry_api.ContainerRegistry._get_session")
 def test_get_request_error(
     mock_session: MagicMock, mock_get: MagicMock, monkeypatch: Any
 ) -> None:
     mock_session.return_value = requests.Session()
     monkeypatch.setenv("ENVIRONMENT", "unit-tests")
 
     response = requests.Response()
     response.status_code = 400
     mock_get.return_value = response
 
     with pytest.raises(requests.HTTPError):
         ContainerRegistry("foo", "bar").get_request("/v1/api")
 
 
-@patch("regio.registry_api.ContainerRegistry.get_request")
+@patch("coregio.registry_api.ContainerRegistry.get_request")
 def test_paginated_response(mock_get: MagicMock) -> None:
     get = MagicMock()
     get.json.return_value = {"foo": ["bar1", "bar2"]}
     get.links = {"next": {"url": "test.url"}}
     mock_get.return_value = get
 
     registry = ContainerRegistry("foo", "bar")
@@ -152,101 +147,104 @@
     get.links = {}
     mock_get.return_value = get
     mock_get.reset_mock()
     result = registry.get_paginated_response("v2/foo", "foo")
     assert result == ["bar1", "bar2"]
 
 
-@patch("regio.utils.handle_response")
-@patch("regio.registry_api.ContainerRegistry.get_request")
+@patch("coregio.utils.handle_response")
+@patch("coregio.registry_api.ContainerRegistry.get_request")
 def test_get_manifest(
     mock_get: MagicMock,
     mock_handle: MagicMock,
 ) -> None:
     get = MagicMock()
     get.json.return_value = {"foo": "bar"}
     mock_get.return_value = get
     mock_handle.return_value = None
-    result = get_manifest("registry", "docker_cfg", "repo", "ref")
+    registry = ContainerRegistry("registry", "docker_cfg")
+    result = registry.get_manifest("repo", "ref")
 
     assert result == {"foo": "bar"}
     mock_get.assert_called_once_with(
         "v2/repo/manifests/ref",
         headers={
             "Accept": "application/vnd.docker.distribution.manifest.v2+json, application/vnd.oci.image.manifest.v1+json"
         },
     )
 
     mock_get.reset_mock()
     response = requests.Response()
     response.status_code = 200
     response.headers = {"Docker-Content-Digest": "demo_manifest_1"}  # type: ignore
     mock_get.return_value = response
-    result = get_manifest("registry", "docker_cfg", "repo", "ref", is_headers=True)
+    result = registry.get_manifest("repo", "ref", is_headers=True)
     assert result == {"Docker-Content-Digest": "demo_manifest_1"}
 
     mock_get.assert_called_once_with(
         "v2/repo/manifests/ref",
         headers={
             "Accept": "application/vnd.docker.distribution.manifest.v2+json, application/vnd.oci.image.manifest.v1+json"
         },
     )
 
     mock_resp = MagicMock()
     mock_resp.status_code = 400
     mock_get.side_effect = requests.HTTPError(response=mock_resp)
     with pytest.raises(requests.HTTPError):
-        get_manifest("registry", "docker_cfg", "repo", "ref")
+        registry.get_manifest("repo", "ref")
 
 
-@patch("regio.utils.handle_response")
-@patch("regio.registry_api.ContainerRegistry.get_request")
+@patch("coregio.utils.handle_response")
+@patch("coregio.registry_api.ContainerRegistry.get_request")
 def test_get_manifest_headers(
     mock_get: MagicMock,
     mock_handle: MagicMock,
 ) -> None:
     get = MagicMock()
     get.headers = {"foo": "bar"}
     mock_get.return_value = get
     mock_handle.return_value = None
     registry_api = ContainerRegistry(url="registry")
-    result = get_manifest_headers(registry_api, "repo", "ref")
+    result = registry_api.get_manifest_headers("repo", "ref")
 
     assert result == {"foo": "bar"}
     mock_get.assert_called_once_with(
         "v2/repo/manifests/ref",
         headers={
             "Accept": "application/vnd.docker.distribution.manifest.v2+json, application/vnd.oci.image.manifest.v1+json"
         },
     )
 
     mock_get.reset_mock()
     response = requests.Response()
     response.status_code = 200
     response.headers = {"Docker-Content-Digest": "demo_manifest_1"}  # type: ignore
     mock_get.return_value = response
-    result = get_manifest_headers(registry_api, "repo", "ref")
+    result = registry_api.get_manifest_headers("repo", "ref")
     assert result == {"Docker-Content-Digest": "demo_manifest_1"}
 
     mock_get.assert_called_once_with(
         "v2/repo/manifests/ref",
         headers={
             "Accept": "application/vnd.docker.distribution.manifest.v2+json, application/vnd.oci.image.manifest.v1+json"
         },
     )
 
     mock_resp = MagicMock()
     mock_resp.status_code = 400
     mock_get.side_effect = requests.HTTPError(response=mock_resp)
     with pytest.raises(requests.HTTPError):
-        get_manifest_headers(registry_api, "repo", "ref")
+        registry_api.get_manifest_headers("repo", "ref")
 
 
-@patch("regio.registry_api.ContainerRegistry.get_paginated_response")
+@patch("coregio.registry_api.ContainerRegistry.get_paginated_response")
 def test_get_tags(mock_get: MagicMock) -> None:
     mock_get.return_value = ["foo", "bar"]
-    result = get_tags("registry", "docker_cfg", "repo")
+
+    registry = ContainerRegistry("registry", "docker_cfg")
+    result = registry.get_tags("repo")
 
     assert result == ["foo", "bar"]
     mock_get.assert_called_once_with(
         "v2/repo/tags/list", list_name="tags", page_size=100, limit=2000
     )
```

