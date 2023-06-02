# Comparing `tmp/liveports-0.1.tar.gz` & `tmp/liveports-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liveports-0.1.tar", last modified: Fri Jun  2 18:29:19 2023, max compression
+gzip compressed data, was "liveports-0.1.1.tar", last modified: Fri Jun  2 19:03:20 2023, max compression
```

## Comparing `liveports-0.1.tar` & `liveports-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-02 18:29:19.765352 liveports-0.1/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      210 2023-06-02 18:29:19.765352 liveports-0.1/PKG-INFO
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-02 18:29:19.765352 liveports-0.1/liveports/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-06-02 16:32:43.000000 liveports-0.1/liveports/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3327 2023-06-02 16:38:40.000000 liveports-0.1/liveports/blaster_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5944 2023-06-02 16:55:44.000000 liveports-0.1/liveports/client.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-02 18:29:19.765352 liveports-0.1/liveports.egg-info/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      210 2023-06-02 18:29:19.000000 liveports-0.1/liveports.egg-info/PKG-INFO
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      245 2023-06-02 18:29:19.000000 liveports-0.1/liveports.egg-info/SOURCES.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        1 2023-06-02 18:29:19.000000 liveports-0.1/liveports.egg-info/dependency_links.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       53 2023-06-02 18:29:19.000000 liveports-0.1/liveports.egg-info/entry_points.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       10 2023-06-02 18:29:19.000000 liveports-0.1/liveports.egg-info/top_level.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2023-06-02 18:29:19.765352 liveports-0.1/setup.cfg
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      419 2023-06-02 16:37:17.000000 liveports-0.1/setup.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-02 19:03:20.430358 liveports-0.1.1/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      212 2023-06-02 19:03:20.430358 liveports-0.1.1/PKG-INFO
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-02 19:03:20.426358 liveports-0.1.1/liveports/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-06-02 16:32:43.000000 liveports-0.1.1/liveports/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3327 2023-06-02 16:38:40.000000 liveports-0.1.1/liveports/blaster_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5942 2023-06-02 19:02:37.000000 liveports-0.1.1/liveports/client.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-02 19:03:20.426358 liveports-0.1.1/liveports.egg-info/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      212 2023-06-02 19:03:20.000000 liveports-0.1.1/liveports.egg-info/PKG-INFO
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      245 2023-06-02 19:03:20.000000 liveports-0.1.1/liveports.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        1 2023-06-02 19:03:20.000000 liveports-0.1.1/liveports.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       53 2023-06-02 19:03:20.000000 liveports-0.1.1/liveports.egg-info/entry_points.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       10 2023-06-02 19:03:20.000000 liveports-0.1.1/liveports.egg-info/top_level.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2023-06-02 19:03:20.430358 liveports-0.1.1/setup.cfg
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      421 2023-06-02 19:03:15.000000 liveports-0.1.1/setup.py
```

### Comparing `liveports-0.1/liveports/blaster_utils.py` & `liveports-0.1.1/liveports/blaster_utils.py`

 * *Files identical despite different names*

### Comparing `liveports-0.1/liveports/client.py` & `liveports-0.1.1/liveports/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,15 +160,15 @@
 
 		cache = json.loads(os.path.isfile(SERVER_CACHED_RESP_FILE) and open(SERVER_CACHED_RESP_FILE).read().strip() or "{}")
 		cache_file = open(SERVER_CACHED_RESP_FILE, "w")
 		try:
 			fcntl.flock(cache_file.fileno(), fcntl.LOCK_EX)
 
 			prev_resp = cache.get(SOURCE) or {}
-			server_hostname = prev_resp.get("server_hostname") or "a.ports.live"
+			server_hostname = prev_resp.get("server_hostname") or "ports.live"
 			resp = requests.post(
 				"https://" + server_hostname + "/api/register",
 				json={
 					"source": SOURCE,
 					"api_key": CommandLineArgs.get("api_key", prev_resp.get("api_key"))
 				}
 			).json()
```

