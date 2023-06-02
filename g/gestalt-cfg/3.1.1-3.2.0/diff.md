# Comparing `tmp/gestalt-cfg-3.1.1.tar.gz` & `tmp/gestalt-cfg-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gestalt-cfg-3.1.1.tar", last modified: Fri Jan 27 15:35:35 2023, max compression
+gzip compressed data, was "gestalt-cfg-3.2.0.tar", last modified: Fri Jun  2 00:26:43 2023, max compression
```

## Comparing `gestalt-cfg-3.1.1.tar` & `gestalt-cfg-3.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 15:35:35.411431 gestalt-cfg-3.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-01-27 15:35:05.000000 gestalt-cfg-3.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-01-27 15:35:35.415431 gestalt-cfg-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-01-27 15:35:05.000000 gestalt-cfg-3.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 15:35:35.411431 gestalt-cfg-3.1.1/gestalt/
--rw-r--r--   0 runner    (1001) docker     (123)    24817 2023-01-27 15:35:05.000000 gestalt-cfg-3.1.1/gestalt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-01-27 15:35:05.000000 gestalt-cfg-3.1.1/gestalt/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-01-27 15:35:05.000000 gestalt-cfg-3.1.1/gestalt/vault.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 15:35:35.411431 gestalt-cfg-3.1.1/gestalt_cfg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-01-27 15:35:35.000000 gestalt-cfg-3.1.1/gestalt_cfg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-01-27 15:35:35.000000 gestalt-cfg-3.1.1/gestalt_cfg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 15:35:35.000000 gestalt-cfg-3.1.1/gestalt_cfg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-01-27 15:35:35.000000 gestalt-cfg-3.1.1/gestalt_cfg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-27 15:35:35.000000 gestalt-cfg-3.1.1/gestalt_cfg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-01-27 15:35:35.415431 gestalt-cfg-3.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-01-27 15:35:05.000000 gestalt-cfg-3.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 15:35:35.411431 gestalt-cfg-3.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 15:35:05.000000 gestalt-cfg-3.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-01-27 15:35:05.000000 gestalt-cfg-3.1.1/tests/test_gestalt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:26:43.458014 gestalt-cfg-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-02 00:26:19.000000 gestalt-cfg-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-06-02 00:26:43.458014 gestalt-cfg-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-06-02 00:26:19.000000 gestalt-cfg-3.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:26:43.458014 gestalt-cfg-3.2.0/gestalt/
+-rw-r--r--   0 runner    (1001) docker     (123)    24817 2023-06-02 00:26:19.000000 gestalt-cfg-3.2.0/gestalt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-02 00:26:19.000000 gestalt-cfg-3.2.0/gestalt/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-06-02 00:26:19.000000 gestalt-cfg-3.2.0/gestalt/vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:26:43.458014 gestalt-cfg-3.2.0/gestalt_cfg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-06-02 00:26:43.000000 gestalt-cfg-3.2.0/gestalt_cfg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-02 00:26:43.000000 gestalt-cfg-3.2.0/gestalt_cfg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 00:26:43.000000 gestalt-cfg-3.2.0/gestalt_cfg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-02 00:26:43.000000 gestalt-cfg-3.2.0/gestalt_cfg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-02 00:26:43.000000 gestalt-cfg-3.2.0/gestalt_cfg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-02 00:26:43.462014 gestalt-cfg-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-02 00:26:19.000000 gestalt-cfg-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:26:43.458014 gestalt-cfg-3.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 00:26:19.000000 gestalt-cfg-3.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20668 2023-06-02 00:26:19.000000 gestalt-cfg-3.2.0/tests/test_gestalt.py
```

### Comparing `gestalt-cfg-3.1.1/LICENSE` & `gestalt-cfg-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gestalt-cfg-3.1.1/PKG-INFO` & `gestalt-cfg-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gestalt-cfg
-Version: 3.1.1
+Version: 3.2.0
 Summary: A sensible configuration library for Python
 Home-page: https://github.com/clear-street/gestalt
 Author: Clear Street
 Author-email: engineering@clearstreet.io
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `gestalt-cfg-3.1.1/README.md` & `gestalt-cfg-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `gestalt-cfg-3.1.1/gestalt/__init__.py` & `gestalt-cfg-3.2.0/gestalt/__init__.py`

 * *Files identical despite different names*

### Comparing `gestalt-cfg-3.1.1/gestalt/provider.py` & `gestalt-cfg-3.2.0/gestalt/provider.py`

 * *Files identical despite different names*

### Comparing `gestalt-cfg-3.1.1/gestalt/vault.py` & `gestalt-cfg-3.2.0/gestalt/vault.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
             response = self.vault_client.read(path)
             if response is None:
                 raise RuntimeError("Gestalt Error: No secrets found")
             if response['lease_id']:
                 dynamic_token = ("dynamic", response['lease_id'],
                                  response['lease_duration'])
                 self.dynamic_token_queue.put_nowait(dynamic_token)
-            requested_data = response["data"]["data"]
+            requested_data = response["data"].get("data", response["data"])
         except hvac.exceptions.InvalidPath:
             raise RuntimeError(
                 "Gestalt Error: The secret path or mount is set incorrectly")
         except requests.exceptions.ConnectionError:
             raise RuntimeError(
                 "Gestalt Error: Gestalt couldn't connect to Vault")
         except Exception as err:
```

### Comparing `gestalt-cfg-3.1.1/gestalt_cfg.egg-info/PKG-INFO` & `gestalt-cfg-3.2.0/gestalt_cfg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gestalt-cfg
-Version: 3.1.1
+Version: 3.2.0
 Summary: A sensible configuration library for Python
 Home-page: https://github.com/clear-street/gestalt
 Author: Clear Street
 Author-email: engineering@clearstreet.io
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `gestalt-cfg-3.1.1/setup.py` & `gestalt-cfg-3.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 with open("requirements.txt") as reqs_file:
     reqs = filter(lambda x: not x.startswith("-"), reqs_file.readlines())
     reqs_list = list(map(lambda x: x.rstrip(), reqs))
 
 setup(name='gestalt-cfg',
-      version='3.1.1',
+      version='3.2.0',
       description='A sensible configuration library for Python',
       long_description=readme(),
       long_description_content_type="text/markdown",
       url='https://github.com/clear-street/gestalt',
       author='Clear Street',
       author_email='engineering@clearstreet.io',
       license='MIT',
```

### Comparing `gestalt-cfg-3.1.1/tests/test_gestalt.py` & `gestalt-cfg-3.2.0/tests/test_gestalt.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,51 @@
 from gestalt.vault import Vault
 from gestalt import merge_into
 import asyncio
 import pytest
 import os
 import gestalt
 import hvac
+import requests
+
+
+class MockSession(requests.Session):
+    def request(self, *_, **__):
+        resp = {
+            'request_id': '230f5e67-e55d-bdae-bd24-c7bc13c1a3e9',
+            'lease_id': '',
+            'renewable': False,
+            'lease_duration': 0,
+            'data': {
+                'last_vault_rotation': '2023-05-31T14:24:41.724285249Z',
+                'password': 'foo',
+                'rotation_period': 60,
+                'ttl': 0,
+                'username': 'foo'
+            },
+            'wrap_info': None,
+            'warnings': None,
+            'auth': None
+        }
+        return MockResponse(resp, 200)
+
+
+class MockResponse:
+    def __init__(self, json_data, status_code):
+        self.json_data = json_data
+        self.status_code = status_code
+        self.ok = True
+
+    def json(self):
+        return self.json_data
+
+
+@pytest.fixture
+def mock_db_role_request(mocker):
+    mocker.patch("requests.Session", MockSession)
 
 
 # Testing member function
 def test_merge_into():
     combine1 = {}
     combine2 = {}
     combine3 = {"local": 1234, "pg": {"host": "dict1_pg", "pass": "dict1_pg"}}
@@ -571,14 +608,23 @@
     g.build_config()
     secret_db = g.get_string("remoteAPI.database.test_secret")
     secret_slack = g.get_string("remoteAPI.slack.token")
     assert secret_db == "test_secret_password"
     assert secret_slack == "random-token"
 
 
+def test_read_no_nest_db_role(env_setup, mock_db_role_request):
+    g = gestalt.Gestalt()
+    g.add_config_file("./tests/testvault/testsfdynamic.json")
+    g.configure_provider("vault", Vault(role=None, jwt=None))
+    g.build_config()
+    secret_username = g.get_string("snowflake.username")
+    assert secret_username == "foo"
+
+
 def test_set_vault_key(env_setup, nested_setup):
     g = gestalt.Gestalt()
     g.configure_provider("vault", Vault(role=None, jwt=None))
     g.set_string(key="test",
                  value="ref+vault://secret/data/testnested#.slack.token")
     g.build_config()
     secret = g.get_string("test")
```

