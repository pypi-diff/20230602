# Comparing `tmp/wallbox-0.4.8.tar.gz` & `tmp/wallbox-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wallbox-0.4.8.tar", last modified: Sun Apr 10 19:40:22 2022, max compression
+gzip compressed data, was "wallbox-0.4.9.tar", last modified: Thu Jun  2 20:09:57 2022, max compression
```

## Comparing `wallbox-0.4.8.tar` & `wallbox-0.4.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 liviu      (502) staff       (20)        0 2022-04-10 19:40:22.922707 wallbox-0.4.8/
--rw-r--r--   0 liviu      (502) staff       (20)    11357 2020-08-04 22:03:23.000000 wallbox-0.4.8/LICENSE
--rw-r--r--   0 liviu      (502) staff       (20)     2714 2022-04-10 19:40:22.922079 wallbox-0.4.8/PKG-INFO
--rw-r--r--   0 liviu      (502) staff       (20)     2327 2022-04-01 16:20:31.000000 wallbox-0.4.8/README.md
--rw-r--r--   0 liviu      (502) staff       (20)       38 2022-04-10 19:40:22.922873 wallbox-0.4.8/setup.cfg
--rw-r--r--   0 liviu      (502) staff       (20)      691 2022-04-10 19:33:41.000000 wallbox-0.4.8/setup.py
-drwxr-xr-x   0 liviu      (502) staff       (20)        0 2022-04-10 19:40:22.880789 wallbox-0.4.8/wallbox/
--rw-r--r--   0 liviu      (502) staff       (20)      106 2022-04-01 16:20:31.000000 wallbox-0.4.8/wallbox/__init__.py
--rw-r--r--   0 liviu      (502) staff       (20)      355 2022-04-01 16:20:31.000000 wallbox-0.4.8/wallbox/statuses.py
--rw-r--r--   0 liviu      (502) staff       (20)     4684 2021-08-08 11:56:02.000000 wallbox-0.4.8/wallbox/wallbox.py
-drwxr-xr-x   0 liviu      (502) staff       (20)        0 2022-04-10 19:40:22.920756 wallbox-0.4.8/wallbox.egg-info/
--rw-r--r--   0 liviu      (502) staff       (20)     2714 2022-04-10 19:40:21.000000 wallbox-0.4.8/wallbox.egg-info/PKG-INFO
--rw-r--r--   0 liviu      (502) staff       (20)      239 2022-04-10 19:40:21.000000 wallbox-0.4.8/wallbox.egg-info/SOURCES.txt
--rw-r--r--   0 liviu      (502) staff       (20)        1 2022-04-10 19:40:21.000000 wallbox-0.4.8/wallbox.egg-info/dependency_links.txt
--rw-r--r--   0 liviu      (502) staff       (20)       49 2022-04-10 19:40:21.000000 wallbox-0.4.8/wallbox.egg-info/requires.txt
--rw-r--r--   0 liviu      (502) staff       (20)        8 2022-04-10 19:40:21.000000 wallbox-0.4.8/wallbox.egg-info/top_level.txt
+drwxrwxr-x   0 liviu     (1000) liviu     (1000)        0 2022-06-02 20:09:57.292498 wallbox-0.4.9/
+-rw-rw-r--   0 liviu     (1000) liviu     (1000)    11357 2022-06-02 19:45:49.000000 wallbox-0.4.9/LICENSE
+-rw-rw-r--   0 liviu     (1000) liviu     (1000)     2714 2022-06-02 20:09:57.292498 wallbox-0.4.9/PKG-INFO
+-rw-rw-r--   0 liviu     (1000) liviu     (1000)     2327 2022-06-02 19:45:49.000000 wallbox-0.4.9/README.md
+-rw-rw-r--   0 liviu     (1000) liviu     (1000)       38 2022-06-02 20:09:57.292498 wallbox-0.4.9/setup.cfg
+-rw-rw-r--   0 liviu     (1000) liviu     (1000)      691 2022-06-02 19:57:54.000000 wallbox-0.4.9/setup.py
+drwxrwxr-x   0 liviu     (1000) liviu     (1000)        0 2022-06-02 20:09:57.292498 wallbox-0.4.9/wallbox/
+-rw-rw-r--   0 liviu     (1000) liviu     (1000)      106 2022-06-02 19:45:49.000000 wallbox-0.4.9/wallbox/__init__.py
+-rw-rw-r--   0 liviu     (1000) liviu     (1000)      355 2022-06-02 19:45:49.000000 wallbox-0.4.9/wallbox/statuses.py
+-rw-rw-r--   0 liviu     (1000) liviu     (1000)     5086 2022-06-02 19:46:33.000000 wallbox-0.4.9/wallbox/wallbox.py
+drwxrwxr-x   0 liviu     (1000) liviu     (1000)        0 2022-06-02 20:09:57.292498 wallbox-0.4.9/wallbox.egg-info/
+-rw-rw-r--   0 liviu     (1000) liviu     (1000)     2714 2022-06-02 20:09:57.000000 wallbox-0.4.9/wallbox.egg-info/PKG-INFO
+-rw-rw-r--   0 liviu     (1000) liviu     (1000)      239 2022-06-02 20:09:57.000000 wallbox-0.4.9/wallbox.egg-info/SOURCES.txt
+-rw-rw-r--   0 liviu     (1000) liviu     (1000)        1 2022-06-02 20:09:57.000000 wallbox-0.4.9/wallbox.egg-info/dependency_links.txt
+-rw-rw-r--   0 liviu     (1000) liviu     (1000)       49 2022-06-02 20:09:57.000000 wallbox-0.4.9/wallbox.egg-info/requires.txt
+-rw-rw-r--   0 liviu     (1000) liviu     (1000)        8 2022-06-02 20:09:57.000000 wallbox-0.4.9/wallbox.egg-info/top_level.txt
```

### Comparing `wallbox-0.4.8/LICENSE` & `wallbox-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wallbox-0.4.8/PKG-INFO` & `wallbox-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wallbox
-Version: 0.4.8
+Version: 0.4.9
 Summary: Module for interacting with Wallbox EV charger api
 Home-page: https://github.com/cliviu74/wallbox
 Author: Liviu Chiribuca
 Author-email: cliviu74@yahoo.com
 License: Apache 2
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wallbox-0.4.8/README.md` & `wallbox-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `wallbox-0.4.8/setup.py` & `wallbox-0.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 def read(name):
     return open(os.path.join(os.path.dirname(__file__), name)).read()
 
 
 setup(
     name="wallbox",
-    version="0.4.8",
+    version="0.4.9",
     description="Module for interacting with Wallbox EV charger api",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     keywords="",
     author="Liviu Chiribuca",
     author_email="cliviu74@yahoo.com",
     url="https://github.com/cliviu74/wallbox",
```

### Comparing `wallbox-0.4.8/wallbox/wallbox.py` & `wallbox-0.4.9/wallbox/wallbox.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,54 @@
 """
 
 Wallbox class
 
 """
 
+from datetime import datetime
+from time import timezone
 from requests.auth import HTTPBasicAuth
 import requests
 import json
 
 
 class Wallbox:
     def __init__(self, username, password, requestGetTimeout = None):
         self.username = username
         self.password = password
         self._requestGetTimeout = requestGetTimeout
         self.baseUrl = "https://api.wall-box.com/"
+        self.authUrl = "https://user-api.wall-box.com/"
         self.jwtToken = ""
+        self.jwtTokenTtl = 0
         self.headers = {
             "Accept": "application/json",
             "Content-Type": "application/json;charset=UTF-8",
         }
 
     @property
     def requestGetTimeout(self):
         return self._requestGetTimeout
 
     def authenticate(self):
+        if self.jwtToken != "" and self.jwtTokenTtl > datetime.timestamp(datetime.now()):
+            return
+
         try:
             response = requests.get(
-                f"{self.baseUrl}auth/token/user",
+                f"{self.authUrl}users/signin",
                 auth=HTTPBasicAuth(self.username, self.password),
+                headers={'Partner': 'wallbox'},
                 timeout=self._requestGetTimeout
             )
             response.raise_for_status()
         except requests.exceptions.HTTPError as err:
             raise (err)
-        self.jwtToken = json.loads(response.text)["jwt"]
+        self.jwtToken = json.loads(response.text)["data"]["attributes"]["token"]
+        self.jwtTokenTtl = json.loads(response.text)["data"]["attributes"]["ttl"]
         self.headers["Authorization"] = f"Bearer {self.jwtToken}"
 
     def getChargersList(self):
         chargerIds = []
         try:
             response = requests.get(
                 f"{self.baseUrl}v3/chargers/groups", headers=self.headers,
```

### Comparing `wallbox-0.4.8/wallbox.egg-info/PKG-INFO` & `wallbox-0.4.9/wallbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wallbox
-Version: 0.4.8
+Version: 0.4.9
 Summary: Module for interacting with Wallbox EV charger api
 Home-page: https://github.com/cliviu74/wallbox
 Author: Liviu Chiribuca
 Author-email: cliviu74@yahoo.com
 License: Apache 2
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

