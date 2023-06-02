# Comparing `tmp/redoubt_agent-0.1.9.tar.gz` & `tmp/redoubt_agent-0.1.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redoubt_agent-0.1.9.tar", last modified: Fri Jun  2 13:00:37 2023, max compression
+gzip compressed data, was "redoubt_agent-0.1.95.tar", last modified: Fri Jun  2 13:16:59 2023, max compression
```

## Comparing `redoubt_agent-0.1.9.tar` & `redoubt_agent-0.1.95.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mnechepurenko   (501) staff       (20)        0 2023-06-02 13:00:37.290494 redoubt_agent-0.1.9/
--rw-rw-r--   0 mnechepurenko   (501) staff       (20)    11357 2023-05-31 14:59:32.000000 redoubt_agent-0.1.9/LICENSE
--rw-r--r--   0 mnechepurenko   (501) staff       (20)     2629 2023-06-02 13:00:37.290797 redoubt_agent-0.1.9/PKG-INFO
--rw-rw-r--   0 mnechepurenko   (501) staff       (20)     1649 2023-06-02 13:00:29.000000 redoubt_agent-0.1.9/README.md
--rw-r--r--   0 mnechepurenko   (501) staff       (20)      104 2023-06-02 11:38:53.000000 redoubt_agent-0.1.9/pyproject.toml
-drwxr-xr-x   0 mnechepurenko   (501) staff       (20)        0 2023-06-02 13:00:37.270742 redoubt_agent-0.1.9/redoubt_agent/
--rw-r--r--   0 mnechepurenko   (501) staff       (20)       67 2023-06-02 12:57:25.000000 redoubt_agent-0.1.9/redoubt_agent/__init__.py
--rw-r--r--   0 mnechepurenko   (501) staff       (20)     2900 2023-06-02 12:57:25.000000 redoubt_agent-0.1.9/redoubt_agent/redoubt_sdk.py
-drwxr-xr-x   0 mnechepurenko   (501) staff       (20)        0 2023-06-02 13:00:37.289920 redoubt_agent-0.1.9/redoubt_agent.egg-info/
--rw-r--r--   0 mnechepurenko   (501) staff       (20)     2629 2023-06-02 13:00:37.000000 redoubt_agent-0.1.9/redoubt_agent.egg-info/PKG-INFO
--rw-r--r--   0 mnechepurenko   (501) staff       (20)      326 2023-06-02 13:00:37.000000 redoubt_agent-0.1.9/redoubt_agent.egg-info/SOURCES.txt
--rw-r--r--   0 mnechepurenko   (501) staff       (20)        1 2023-06-02 13:00:37.000000 redoubt_agent-0.1.9/redoubt_agent.egg-info/dependency_links.txt
--rw-r--r--   0 mnechepurenko   (501) staff       (20)        1 2023-06-02 12:57:34.000000 redoubt_agent-0.1.9/redoubt_agent.egg-info/not-zip-safe
--rw-r--r--   0 mnechepurenko   (501) staff       (20)       25 2023-06-02 13:00:37.000000 redoubt_agent-0.1.9/redoubt_agent.egg-info/requires.txt
--rw-r--r--   0 mnechepurenko   (501) staff       (20)       14 2023-06-02 13:00:37.000000 redoubt_agent-0.1.9/redoubt_agent.egg-info/top_level.txt
--rw-rw-r--   0 mnechepurenko   (501) staff       (20)     1104 2023-06-02 13:00:37.292000 redoubt_agent-0.1.9/setup.cfg
--rw-rw-r--   0 mnechepurenko   (501) staff       (20)       68 2023-06-02 11:01:57.000000 redoubt_agent-0.1.9/setup.py
+drwxr-xr-x   0 mnechepurenko   (501) staff       (20)        0 2023-06-02 13:16:59.085777 redoubt_agent-0.1.95/
+-rw-rw-r--   0 mnechepurenko   (501) staff       (20)    11357 2023-05-31 14:59:32.000000 redoubt_agent-0.1.95/LICENSE
+-rw-r--r--   0 mnechepurenko   (501) staff       (20)     2630 2023-06-02 13:16:59.085874 redoubt_agent-0.1.95/PKG-INFO
+-rw-rw-r--   0 mnechepurenko   (501) staff       (20)     1649 2023-06-02 13:16:55.000000 redoubt_agent-0.1.95/README.md
+-rw-r--r--   0 mnechepurenko   (501) staff       (20)      104 2023-06-02 11:38:53.000000 redoubt_agent-0.1.95/pyproject.toml
+drwxr-xr-x   0 mnechepurenko   (501) staff       (20)        0 2023-06-02 13:16:59.084340 redoubt_agent-0.1.95/redoubt_agent/
+-rw-r--r--   0 mnechepurenko   (501) staff       (20)       67 2023-06-02 12:57:25.000000 redoubt_agent-0.1.95/redoubt_agent/__init__.py
+-rw-r--r--   0 mnechepurenko   (501) staff       (20)     2900 2023-06-02 13:16:23.000000 redoubt_agent-0.1.95/redoubt_agent/redoubt_sdk.py
+drwxr-xr-x   0 mnechepurenko   (501) staff       (20)        0 2023-06-02 13:16:59.085609 redoubt_agent-0.1.95/redoubt_agent.egg-info/
+-rw-r--r--   0 mnechepurenko   (501) staff       (20)     2630 2023-06-02 13:16:59.000000 redoubt_agent-0.1.95/redoubt_agent.egg-info/PKG-INFO
+-rw-r--r--   0 mnechepurenko   (501) staff       (20)      326 2023-06-02 13:16:59.000000 redoubt_agent-0.1.95/redoubt_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 mnechepurenko   (501) staff       (20)        1 2023-06-02 13:16:59.000000 redoubt_agent-0.1.95/redoubt_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 mnechepurenko   (501) staff       (20)        1 2023-06-02 12:57:34.000000 redoubt_agent-0.1.95/redoubt_agent.egg-info/not-zip-safe
+-rw-r--r--   0 mnechepurenko   (501) staff       (20)       25 2023-06-02 13:16:59.000000 redoubt_agent-0.1.95/redoubt_agent.egg-info/requires.txt
+-rw-r--r--   0 mnechepurenko   (501) staff       (20)       14 2023-06-02 13:16:59.000000 redoubt_agent-0.1.95/redoubt_agent.egg-info/top_level.txt
+-rw-rw-r--   0 mnechepurenko   (501) staff       (20)     1105 2023-06-02 13:16:59.086288 redoubt_agent-0.1.95/setup.cfg
+-rw-rw-r--   0 mnechepurenko   (501) staff       (20)       68 2023-06-02 11:01:57.000000 redoubt_agent-0.1.95/setup.py
```

### Comparing `redoubt_agent-0.1.9/LICENSE` & `redoubt_agent-0.1.95/LICENSE`

 * *Files identical despite different names*

### Comparing `redoubt_agent-0.1.9/PKG-INFO` & `redoubt_agent-0.1.95/redoubt_agent.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: redoubt_agent
-Version: 0.1.9
+Name: redoubt-agent
+Version: 0.1.95
 Summary: re:doubt Bot Python SDK
 Home-page: https://www.redoubt.online/
 Author: maksymds
 Author-email: redoubt@devnull.ae
 License: Apache 2.0
 Project-URL: Github, https://github.com/re-doubt/redoubt-bot-python-sdk
 Project-URL: Documentation, https://docs.redoubt.online/
```

### Comparing `redoubt_agent-0.1.9/README.md` & `redoubt_agent-0.1.95/README.md`

 * *Files identical despite different names*

### Comparing `redoubt_agent-0.1.9/redoubt_agent/redoubt_sdk.py` & `redoubt_agent-0.1.95/redoubt_agent/redoubt_sdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from gql.transport.websockets import WebsocketsTransport
 from loguru import logger
 
 DEFAULT_ENDPOINT = 'ws://44.210.191.88:9080/v1/graphql'  # TODO update to wss
 
 
 class RedoubtEventsStream:
-    def __init__(self, endpoint=DEFAULT_ENDPOINT, api_key=None):
+    def __init__(self, api_key=None, endpoint=DEFAULT_ENDPOINT):
         if api_key is None:
             api_key = os.environ.get('REDOUBT_API_KEY', None)
         assert api_key is not None, "API key not found"
         self.transport = WebsocketsTransport(
             url=endpoint, ping_interval=1, pong_timeout=1, headers={
                 'X-API-Key': api_key
             }
```

### Comparing `redoubt_agent-0.1.9/redoubt_agent.egg-info/PKG-INFO` & `redoubt_agent-0.1.95/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: redoubt-agent
-Version: 0.1.9
+Name: redoubt_agent
+Version: 0.1.95
 Summary: re:doubt Bot Python SDK
 Home-page: https://www.redoubt.online/
 Author: maksymds
 Author-email: redoubt@devnull.ae
 License: Apache 2.0
 Project-URL: Github, https://github.com/re-doubt/redoubt-bot-python-sdk
 Project-URL: Documentation, https://docs.redoubt.online/
```

### Comparing `redoubt_agent-0.1.9/setup.cfg` & `redoubt_agent-0.1.95/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = redoubt_agent
-version = 0.1.9
+version = 0.1.95
 description = re:doubt Bot Python SDK
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://www.redoubt.online/
 keywords = TON, redoubt, sdk
 license = Apache 2.0
 classifiers =
```

