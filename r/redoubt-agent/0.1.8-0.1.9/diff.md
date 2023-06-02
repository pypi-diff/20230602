# Comparing `tmp/redoubt_agent-0.1.8.tar.gz` & `tmp/redoubt_agent-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redoubt_agent-0.1.8.tar", last modified: Fri Jun  2 12:58:59 2023, max compression
+gzip compressed data, was "redoubt_agent-0.1.9.tar", last modified: Fri Jun  2 13:00:37 2023, max compression
```

## Comparing `redoubt_agent-0.1.8.tar` & `redoubt_agent-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mnechepurenko   (501) staff       (20)        0 2023-06-02 12:58:59.689144 redoubt_agent-0.1.8/
--rw-rw-r--   0 mnechepurenko   (501) staff       (20)    11357 2023-05-31 14:59:32.000000 redoubt_agent-0.1.8/LICENSE
--rw-r--r--   0 mnechepurenko   (501) staff       (20)     2584 2023-06-02 12:58:59.689259 redoubt_agent-0.1.8/PKG-INFO
--rw-rw-r--   0 mnechepurenko   (501) staff       (20)     1604 2023-06-02 12:58:57.000000 redoubt_agent-0.1.8/README.md
--rw-r--r--   0 mnechepurenko   (501) staff       (20)      104 2023-06-02 11:38:53.000000 redoubt_agent-0.1.8/pyproject.toml
-drwxr-xr-x   0 mnechepurenko   (501) staff       (20)        0 2023-06-02 12:58:59.686627 redoubt_agent-0.1.8/redoubt_agent/
--rw-r--r--   0 mnechepurenko   (501) staff       (20)       67 2023-06-02 12:57:25.000000 redoubt_agent-0.1.8/redoubt_agent/__init__.py
--rw-r--r--   0 mnechepurenko   (501) staff       (20)     2900 2023-06-02 12:57:25.000000 redoubt_agent-0.1.8/redoubt_agent/redoubt_sdk.py
-drwxr-xr-x   0 mnechepurenko   (501) staff       (20)        0 2023-06-02 12:58:59.688939 redoubt_agent-0.1.8/redoubt_agent.egg-info/
--rw-r--r--   0 mnechepurenko   (501) staff       (20)     2584 2023-06-02 12:58:59.000000 redoubt_agent-0.1.8/redoubt_agent.egg-info/PKG-INFO
--rw-r--r--   0 mnechepurenko   (501) staff       (20)      326 2023-06-02 12:58:59.000000 redoubt_agent-0.1.8/redoubt_agent.egg-info/SOURCES.txt
--rw-r--r--   0 mnechepurenko   (501) staff       (20)        1 2023-06-02 12:58:59.000000 redoubt_agent-0.1.8/redoubt_agent.egg-info/dependency_links.txt
--rw-r--r--   0 mnechepurenko   (501) staff       (20)        1 2023-06-02 12:57:34.000000 redoubt_agent-0.1.8/redoubt_agent.egg-info/not-zip-safe
--rw-r--r--   0 mnechepurenko   (501) staff       (20)       25 2023-06-02 12:58:59.000000 redoubt_agent-0.1.8/redoubt_agent.egg-info/requires.txt
--rw-r--r--   0 mnechepurenko   (501) staff       (20)       14 2023-06-02 12:58:59.000000 redoubt_agent-0.1.8/redoubt_agent.egg-info/top_level.txt
--rw-rw-r--   0 mnechepurenko   (501) staff       (20)     1104 2023-06-02 12:58:59.689966 redoubt_agent-0.1.8/setup.cfg
--rw-rw-r--   0 mnechepurenko   (501) staff       (20)       68 2023-06-02 11:01:57.000000 redoubt_agent-0.1.8/setup.py
+drwxr-xr-x   0 mnechepurenko   (501) staff       (20)        0 2023-06-02 13:00:37.290494 redoubt_agent-0.1.9/
+-rw-rw-r--   0 mnechepurenko   (501) staff       (20)    11357 2023-05-31 14:59:32.000000 redoubt_agent-0.1.9/LICENSE
+-rw-r--r--   0 mnechepurenko   (501) staff       (20)     2629 2023-06-02 13:00:37.290797 redoubt_agent-0.1.9/PKG-INFO
+-rw-rw-r--   0 mnechepurenko   (501) staff       (20)     1649 2023-06-02 13:00:29.000000 redoubt_agent-0.1.9/README.md
+-rw-r--r--   0 mnechepurenko   (501) staff       (20)      104 2023-06-02 11:38:53.000000 redoubt_agent-0.1.9/pyproject.toml
+drwxr-xr-x   0 mnechepurenko   (501) staff       (20)        0 2023-06-02 13:00:37.270742 redoubt_agent-0.1.9/redoubt_agent/
+-rw-r--r--   0 mnechepurenko   (501) staff       (20)       67 2023-06-02 12:57:25.000000 redoubt_agent-0.1.9/redoubt_agent/__init__.py
+-rw-r--r--   0 mnechepurenko   (501) staff       (20)     2900 2023-06-02 12:57:25.000000 redoubt_agent-0.1.9/redoubt_agent/redoubt_sdk.py
+drwxr-xr-x   0 mnechepurenko   (501) staff       (20)        0 2023-06-02 13:00:37.289920 redoubt_agent-0.1.9/redoubt_agent.egg-info/
+-rw-r--r--   0 mnechepurenko   (501) staff       (20)     2629 2023-06-02 13:00:37.000000 redoubt_agent-0.1.9/redoubt_agent.egg-info/PKG-INFO
+-rw-r--r--   0 mnechepurenko   (501) staff       (20)      326 2023-06-02 13:00:37.000000 redoubt_agent-0.1.9/redoubt_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 mnechepurenko   (501) staff       (20)        1 2023-06-02 13:00:37.000000 redoubt_agent-0.1.9/redoubt_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 mnechepurenko   (501) staff       (20)        1 2023-06-02 12:57:34.000000 redoubt_agent-0.1.9/redoubt_agent.egg-info/not-zip-safe
+-rw-r--r--   0 mnechepurenko   (501) staff       (20)       25 2023-06-02 13:00:37.000000 redoubt_agent-0.1.9/redoubt_agent.egg-info/requires.txt
+-rw-r--r--   0 mnechepurenko   (501) staff       (20)       14 2023-06-02 13:00:37.000000 redoubt_agent-0.1.9/redoubt_agent.egg-info/top_level.txt
+-rw-rw-r--   0 mnechepurenko   (501) staff       (20)     1104 2023-06-02 13:00:37.292000 redoubt_agent-0.1.9/setup.cfg
+-rw-rw-r--   0 mnechepurenko   (501) staff       (20)       68 2023-06-02 11:01:57.000000 redoubt_agent-0.1.9/setup.py
```

### Comparing `redoubt_agent-0.1.8/LICENSE` & `redoubt_agent-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `redoubt_agent-0.1.8/PKG-INFO` & `redoubt_agent-0.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redoubt_agent
-Version: 0.1.8
+Version: 0.1.9
 Summary: re:doubt Bot Python SDK
 Home-page: https://www.redoubt.online/
 Author: maksymds
 Author-email: redoubt@devnull.ae
 License: Apache 2.0
 Project-URL: Github, https://github.com/re-doubt/redoubt-bot-python-sdk
 Project-URL: Documentation, https://docs.redoubt.online/
@@ -44,20 +44,21 @@
 To use SDK one need to request API key from [@RedoubtAPIBot](https://t.me/RedoubtAPIBot) and pass it either directly 
 to `RedoubtEventsStream` instance or using `REDOUBT_API_KEY` environment variable.
 
 ## Examples
 
 ### New pools bot
 
-* [New pools detector](https://pypi.org/project/redoubt-agent/examples/new_pools.py)
+* [New pools detector](https://github.com/re-doubt/redoubt-bot-python-sdk/blob/main/examples/new_pools.py)
+
 It is monitoring for new pools and just prints info.
 
 ### Jetton transfers bot
 
-* [Jetton transfers bot](https://pypi.org/project/redoubt-agent/examples/jetton_transfer.py)
+* [Jetton transfers bot](https://github.com/re-doubt/redoubt-bot-python-sdk/blob/main/examples/jetton_transfer.py)
 
 More complicated example. It listens for all Jetton transfers and after receiving info 
 about the transfer it requests additional info over GraphQL API. In this case it
 uses additional GraphQL request to get Jetton metadata (symbol and decimals).
 
 As a result you will get such a message:
 ```
```

### Comparing `redoubt_agent-0.1.8/README.md` & `redoubt_agent-0.1.9/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -18,20 +18,21 @@
 To use SDK one need to request API key from [@RedoubtAPIBot](https://t.me/RedoubtAPIBot) and pass it either directly 
 to `RedoubtEventsStream` instance or using `REDOUBT_API_KEY` environment variable.
 
 ## Examples
 
 ### New pools bot
 
-* [New pools detector](https://pypi.org/project/redoubt-agent/examples/new_pools.py)
+* [New pools detector](https://github.com/re-doubt/redoubt-bot-python-sdk/blob/main/examples/new_pools.py)
+
 It is monitoring for new pools and just prints info.
 
 ### Jetton transfers bot
 
-* [Jetton transfers bot](https://pypi.org/project/redoubt-agent/examples/jetton_transfer.py)
+* [Jetton transfers bot](https://github.com/re-doubt/redoubt-bot-python-sdk/blob/main/examples/jetton_transfer.py)
 
 More complicated example. It listens for all Jetton transfers and after receiving info 
 about the transfer it requests additional info over GraphQL API. In this case it
 uses additional GraphQL request to get Jetton metadata (symbol and decimals).
 
 As a result you will get such a message:
 ```
```

### Comparing `redoubt_agent-0.1.8/redoubt_agent/redoubt_sdk.py` & `redoubt_agent-0.1.9/redoubt_agent/redoubt_sdk.py`

 * *Files identical despite different names*

### Comparing `redoubt_agent-0.1.8/redoubt_agent.egg-info/PKG-INFO` & `redoubt_agent-0.1.9/redoubt_agent.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redoubt-agent
-Version: 0.1.8
+Version: 0.1.9
 Summary: re:doubt Bot Python SDK
 Home-page: https://www.redoubt.online/
 Author: maksymds
 Author-email: redoubt@devnull.ae
 License: Apache 2.0
 Project-URL: Github, https://github.com/re-doubt/redoubt-bot-python-sdk
 Project-URL: Documentation, https://docs.redoubt.online/
@@ -44,20 +44,21 @@
 To use SDK one need to request API key from [@RedoubtAPIBot](https://t.me/RedoubtAPIBot) and pass it either directly 
 to `RedoubtEventsStream` instance or using `REDOUBT_API_KEY` environment variable.
 
 ## Examples
 
 ### New pools bot
 
-* [New pools detector](https://pypi.org/project/redoubt-agent/examples/new_pools.py)
+* [New pools detector](https://github.com/re-doubt/redoubt-bot-python-sdk/blob/main/examples/new_pools.py)
+
 It is monitoring for new pools and just prints info.
 
 ### Jetton transfers bot
 
-* [Jetton transfers bot](https://pypi.org/project/redoubt-agent/examples/jetton_transfer.py)
+* [Jetton transfers bot](https://github.com/re-doubt/redoubt-bot-python-sdk/blob/main/examples/jetton_transfer.py)
 
 More complicated example. It listens for all Jetton transfers and after receiving info 
 about the transfer it requests additional info over GraphQL API. In this case it
 uses additional GraphQL request to get Jetton metadata (symbol and decimals).
 
 As a result you will get such a message:
 ```
```

### Comparing `redoubt_agent-0.1.8/setup.cfg` & `redoubt_agent-0.1.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = redoubt_agent
-version = 0.1.8
+version = 0.1.9
 description = re:doubt Bot Python SDK
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://www.redoubt.online/
 keywords = TON, redoubt, sdk
 license = Apache 2.0
 classifiers =
```

