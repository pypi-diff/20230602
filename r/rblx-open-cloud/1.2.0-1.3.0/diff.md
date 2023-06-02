# Comparing `tmp/rblx-open-cloud-1.2.0.tar.gz` & `tmp/rblx-open-cloud-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rblx-open-cloud-1.2.0.tar", last modified: Fri Mar 31 22:29:02 2023, max compression
+gzip compressed data, was "rblx-open-cloud-1.3.0.tar", last modified: Fri Jun  2 07:05:48 2023, max compression
```

## Comparing `rblx-open-cloud-1.2.0.tar` & `rblx-open-cloud-1.3.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 22:29:02.482995 rblx-open-cloud-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-31 22:28:47.000000 rblx-open-cloud-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-03-31 22:29:02.482995 rblx-open-cloud-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-03-31 22:28:47.000000 rblx-open-cloud-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 22:29:02.482995 rblx-open-cloud-1.2.0/rblx_open_cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-03-31 22:29:02.000000 rblx-open-cloud-1.2.0/rblx_open_cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-03-31 22:29:02.000000 rblx-open-cloud-1.2.0/rblx_open_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 22:29:02.000000 rblx-open-cloud-1.2.0/rblx_open_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-31 22:29:02.000000 rblx-open-cloud-1.2.0/rblx_open_cloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-31 22:29:02.000000 rblx-open-cloud-1.2.0/rblx_open_cloud.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 22:29:02.482995 rblx-open-cloud-1.2.0/rblxopencloud/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-03-31 22:28:47.000000 rblx-open-cloud-1.2.0/rblxopencloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-03-31 22:28:47.000000 rblx-open-cloud-1.2.0/rblxopencloud/creator.py
--rw-r--r--   0 runner    (1001) docker     (123)    27780 2023-03-31 22:28:47.000000 rblx-open-cloud-1.2.0/rblxopencloud/datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-03-31 22:28:47.000000 rblx-open-cloud-1.2.0/rblxopencloud/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-03-31 22:28:47.000000 rblx-open-cloud-1.2.0/rblxopencloud/experience.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-03-31 22:28:47.000000 rblx-open-cloud-1.2.0/rblxopencloud/group.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-31 22:28:47.000000 rblx-open-cloud-1.2.0/rblxopencloud/user.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 22:29:02.482995 rblx-open-cloud-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-03-31 22:28:47.000000 rblx-open-cloud-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:05:48.802884 rblx-open-cloud-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-02 07:05:35.000000 rblx-open-cloud-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-06-02 07:05:48.802884 rblx-open-cloud-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-06-02 07:05:35.000000 rblx-open-cloud-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:05:48.802884 rblx-open-cloud-1.3.0/rblx_open_cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-06-02 07:05:48.000000 rblx-open-cloud-1.3.0/rblx_open_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-02 07:05:48.000000 rblx-open-cloud-1.3.0/rblx_open_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 07:05:48.000000 rblx-open-cloud-1.3.0/rblx_open_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-02 07:05:48.000000 rblx-open-cloud-1.3.0/rblx_open_cloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-02 07:05:48.000000 rblx-open-cloud-1.3.0/rblx_open_cloud.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:05:48.802884 rblx-open-cloud-1.3.0/rblxopencloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-02 07:05:35.000000 rblx-open-cloud-1.3.0/rblxopencloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8153 2023-06-02 07:05:35.000000 rblx-open-cloud-1.3.0/rblxopencloud/creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29069 2023-06-02 07:05:35.000000 rblx-open-cloud-1.3.0/rblxopencloud/datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-02 07:05:35.000000 rblx-open-cloud-1.3.0/rblxopencloud/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-06-02 07:05:35.000000 rblx-open-cloud-1.3.0/rblxopencloud/experience.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-02 07:05:35.000000 rblx-open-cloud-1.3.0/rblxopencloud/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11769 2023-06-02 07:05:35.000000 rblx-open-cloud-1.3.0/rblxopencloud/oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-02 07:05:35.000000 rblx-open-cloud-1.3.0/rblxopencloud/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 07:05:48.806884 rblx-open-cloud-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-02 07:05:35.000000 rblx-open-cloud-1.3.0/setup.py
```

### Comparing `rblx-open-cloud-1.2.0/LICENSE` & `rblx-open-cloud-1.3.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 TreeBen77
+Copyright (c) 2022-2023 TreeBen77
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `rblx-open-cloud-1.2.0/PKG-INFO` & `rblx-open-cloud-1.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: rblx-open-cloud
-Version: 1.2.0
+Version: 1.3.0
 Summary: API wrapper for Roblox Open Cloud
 Home-page: https://github.com/TreeBen77/rblx-open-cloud
 Author: TreeBen77
 License: MIT
 Keywords: roblox,open-cloud,data-store,place-publishing,mesageing-service
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # rblx-open-cloud
  
-Python API wrapper for [Roblox Open Cloud](https://create.roblox.com/docs/open-cloud/index).
+Python API wrapper for [Roblox Open Cloud](https://create.roblox.com/docs/open-cloud/index), it currently has 100% API coverage and I plan to add all new Open Cloud additions to the library.
 
 **Documentation: https://rblx-open-cloud.readthedocs.io**
 
+**Devforum Post: https://devforum.roblox.com/t/1991959**
+
 **Discord Server: https://discord.gg/gEBdHNAR46**
 
 ## Quickstart
 
 ### Getting Started
 
 1. Install the library with pip in your terminal.
@@ -28,15 +30,14 @@
     ```
 
 2. Create an API key from the [Creator Dashboard](https://create.roblox.com/credentials). You can read [Managing API Keys](https://create.roblox.com/docs/open-cloud/managing-api-keys) for help.
 
 You've got the basics down, below are examples for some of the APIs.
 
 ### Accessing Data Stores
-**NOTE: Roblox doesn't support access to ordered data stores via open cloud yet.**
 ```py
 import rblxopencloud
 
 # create an Experience object with your experience ID and your api key
 # TODO: replace '13058' with your experience ID
 experience = rblxopencloud.Experience(13058, api_key="api-key-from-step-2")
```

### Comparing `rblx-open-cloud-1.2.0/README.md` & `rblx-open-cloud-1.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # rblx-open-cloud
  
-Python API wrapper for [Roblox Open Cloud](https://create.roblox.com/docs/open-cloud/index).
+Python API wrapper for [Roblox Open Cloud](https://create.roblox.com/docs/open-cloud/index), it currently has 100% API coverage and I plan to add all new Open Cloud additions to the library.
 
 **Documentation: https://rblx-open-cloud.readthedocs.io**
 
+**Devforum Post: https://devforum.roblox.com/t/1991959**
+
 **Discord Server: https://discord.gg/gEBdHNAR46**
 
 ## Quickstart
 
 ### Getting Started
 
 1. Install the library with pip in your terminal.
@@ -16,15 +18,14 @@
     ```
 
 2. Create an API key from the [Creator Dashboard](https://create.roblox.com/credentials). You can read [Managing API Keys](https://create.roblox.com/docs/open-cloud/managing-api-keys) for help.
 
 You've got the basics down, below are examples for some of the APIs.
 
 ### Accessing Data Stores
-**NOTE: Roblox doesn't support access to ordered data stores via open cloud yet.**
 ```py
 import rblxopencloud
 
 # create an Experience object with your experience ID and your api key
 # TODO: replace '13058' with your experience ID
 experience = rblxopencloud.Experience(13058, api_key="api-key-from-step-2")
 
@@ -89,8 +90,8 @@
         # this will try to check if the asset has been processed yet
         operation = asset.fetch_operation()
         if operation:
             # if it has been print it then stop the loop.
             print(operation)
             break
 ```
-Examples for more APIs are avalible in the [examples](https://github.com/TreeBen77/rblx-open-cloud/tree/main/examples) directory.
+Examples for more APIs are avalible in the [examples](https://github.com/TreeBen77/rblx-open-cloud/tree/main/examples) directory.
```

### Comparing `rblx-open-cloud-1.2.0/rblx_open_cloud.egg-info/PKG-INFO` & `rblx-open-cloud-1.3.0/rblx_open_cloud.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: rblx-open-cloud
-Version: 1.2.0
+Version: 1.3.0
 Summary: API wrapper for Roblox Open Cloud
 Home-page: https://github.com/TreeBen77/rblx-open-cloud
 Author: TreeBen77
 License: MIT
 Keywords: roblox,open-cloud,data-store,place-publishing,mesageing-service
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # rblx-open-cloud
  
-Python API wrapper for [Roblox Open Cloud](https://create.roblox.com/docs/open-cloud/index).
+Python API wrapper for [Roblox Open Cloud](https://create.roblox.com/docs/open-cloud/index), it currently has 100% API coverage and I plan to add all new Open Cloud additions to the library.
 
 **Documentation: https://rblx-open-cloud.readthedocs.io**
 
+**Devforum Post: https://devforum.roblox.com/t/1991959**
+
 **Discord Server: https://discord.gg/gEBdHNAR46**
 
 ## Quickstart
 
 ### Getting Started
 
 1. Install the library with pip in your terminal.
@@ -28,15 +30,14 @@
     ```
 
 2. Create an API key from the [Creator Dashboard](https://create.roblox.com/credentials). You can read [Managing API Keys](https://create.roblox.com/docs/open-cloud/managing-api-keys) for help.
 
 You've got the basics down, below are examples for some of the APIs.
 
 ### Accessing Data Stores
-**NOTE: Roblox doesn't support access to ordered data stores via open cloud yet.**
 ```py
 import rblxopencloud
 
 # create an Experience object with your experience ID and your api key
 # TODO: replace '13058' with your experience ID
 experience = rblxopencloud.Experience(13058, api_key="api-key-from-step-2")
```

### Comparing `rblx-open-cloud-1.2.0/rblxopencloud/creator.py` & `rblx-open-cloud-1.3.0/rblxopencloud/creator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .exceptions import *
+from .exceptions import InvalidAsset, InvalidKey, ModeratedText, rblx_opencloudException, RateLimited, ServiceUnavailable
 import requests, json, io
 from typing import Union, Optional, TYPE_CHECKING
 import urllib3
 from enum import Enum
 from datetime import datetime
 
 if TYPE_CHECKING:
@@ -48,15 +48,15 @@
         self.__creator = creator
     
     def __repr__(self) -> str:
         return f"rblxopencloud.PendingAsset()"
     
     def fetch_operation(self) -> Union[None, Asset]:
         response = requests.get(f"https://apis.roblox.com/assets/v1/{self.__path}",
-            headers={"x-api-key": self.__api_key})
+            headers={"x-api-key" if not self.__api_key.startswith("Bearer ") else "authorization": self.__api_key})
         
         if response.ok:
             info = response.json()
             if not info.get("done"): return None
             return Asset(info["response"], self.__creator)
         else:
             if response.status_code == 401 or response.status_code == 403: raise InvalidKey("Your key may have expired, or may not have permission to access this resource.")
@@ -97,24 +97,26 @@
                 },
                 "displayName": name,
                 "description": description
             }),
             "fileContent": (file.name, file.read(), mimetypes.get(file.name.split(".")[-1]))
         })
         response = requests.post(f"https://apis.roblox.com/assets/v1/assets",
-            headers={"x-api-key": self.__api_key, "content-type": contentType}, data=body)
+            headers={"x-api-key" if not self.__api_key.startswith("Bearer ") else "authorization": self.__api_key, "content-type": contentType}, data=body)
         
-        if response.status_code == 400: raise InvalidAsset(f"The file is not a supported type, or is corrupted")
+        if response.status_code == 400 and response.json()["message"] == "\"InvalidImage\"": raise InvalidAsset(f"The file is not a supported type, or is corrupted")
+        elif response.status_code == 400 and response.json()["message"] == "AssetName is moderated.": raise ModeratedText(f"The asset's name was moderated.")
+        elif response.status_code == 400 and response.json()["message"] == "AssetDescription is moderated.": raise ModeratedText(f"The asset's description was moderated.")
         elif response.status_code == 401 or response.status_code == 403: raise InvalidKey("Your key may have expired, or may not have permission to access this resource.")
         elif response.status_code == 429: raise RateLimited("You're being rate limited.")
         elif response.status_code >= 500: raise ServiceUnavailable("The service is unavailable or has encountered an error.")
         elif not response.ok: raise rblx_opencloudException(f"Unexpected HTTP {response.status_code}")
 
         response_op = requests.get(f"https://apis.roblox.com/assets/v1/{response.json()['path']}",
-            headers={"x-api-key": self.__api_key})
+            headers={"x-api-key" if not self.__api_key.startswith("Bearer ") else "authorization": self.__api_key})
         
         if not response_op.ok:
             return PendingAsset(response_op.json()['path'], self.__api_key, self)
         else:
             info = response_op.json()
             if not info.get("done"):
                 return PendingAsset(response_op.json()['path'], self.__api_key, self)
@@ -125,24 +127,26 @@
         body, contentType = urllib3.encode_multipart_formdata({
             "request": json.dumps({
                 "assetId": asset_id
             }),
             "fileContent": (file.name, file.read(), mimetypes.get(file.name.split(".")[-1]))
         })
         response = requests.patch(f"https://apis.roblox.com/assets/v1/assets/{asset_id}",
-            headers={"x-api-key": self.__api_key, "content-type": contentType}, data=body)
-        
-        if response.status_code == 400: raise InvalidAsset(f"The file is not a decal or is corrupted")
+            headers={"x-api-key" if not self.__api_key.startswith("Bearer ") else "authorization": self.__api_key, "content-type": contentType}, data=body)
+
+        if response.status_code == 400 and response.json()["message"] == "\"InvalidImage\"": raise InvalidAsset(f"The file is not a supported type, or is corrupted")
+        elif response.status_code == 400 and response.json()["message"] == "AssetName is moderated.": raise ModeratedText(f"The asset's name was moderated.")
+        elif response.status_code == 400 and response.json()["message"] == "AssetDescription is moderated.": raise ModeratedText(f"The asset's description was moderated.")
         elif response.status_code == 401 or response.status_code == 403: raise InvalidKey("Your key may have expired, or may not have permission to access this resource.")
         elif response.status_code == 429: raise RateLimited("You're being rate limited.")
         elif response.status_code >= 500: raise ServiceUnavailable("The service is unavailable or has encountered an error.")
         elif not response.ok: raise rblx_opencloudException(f"Unexpected HTTP {response.status_code}")
 
         response_op = requests.get(f"https://apis.roblox.com/assets/v1/{response.json()['path']}",
-            headers={"x-api-key": self.__api_key})
+            headers={"x-api-key" if not self.__api_key.startswith("Bearer ") else "authorization": self.__api_key})
         
         if not response_op.ok:
             return PendingAsset(response_op.json()['path'], self.__api_key, self)
         else:
             info = response_op.json()
             if not info.get("done"):
                 return PendingAsset(response_op.json()['path'], self.__api_key, self)
```

### Comparing `rblx-open-cloud-1.2.0/rblxopencloud/datastore.py` & `rblx-open-cloud-1.3.0/rblxopencloud/datastore.py`

 * *Files 12% similar despite different names*

```diff
@@ -103,19 +103,21 @@
                 headers={"x-api-key": self.__api_key}, params={
                 "datastoreName": self.name,
                 "scope": self.scope,
                 "AllScopes": not self.scope,
                 "prefix": prefix,
                 "cursor": nextcursor if nextcursor else None
             })
-            if response.status_code == 401 or response.status_code == 403: raise InvalidKey("Your key may have expired, or may not have permission to access this resource.")
-            elif response.status_code == 404: raise NotFound("The datastore you're trying to access does not exist.")
-            elif response.status_code == 429: raise RateLimited("You're being rate limited.")
-            elif response.status_code >= 500: raise ServiceUnavailable("The service is unavailable or has encountered an error.")
-            elif not response.ok: raise rblx_opencloudException(f"Unexpected HTTP {response.status_code}")
+            if response.status_code == 400: raise rblx_opencloudException(response.json()["message"])
+            elif response.status_code == 401: raise InvalidKey(response.text)
+            elif response.status_code == 403: raise InvalidKey(response.json()["message"])
+            elif response.status_code == 404: raise NotFound(response.json()["message"])
+            elif response.status_code == 429: raise RateLimited(response.json()["message"])
+            elif response.status_code >= 500: raise ServiceUnavailable(f"Internal Server Error: '{response.text}'")
+            elif not response.ok: raise rblx_opencloudException(f"Unexpected HTTP {response.status_code}: '{response.text}'")
             
             data = response.json()
             for key in data["keys"]:
                 yields += 1
                 yield ListedEntry(key["key"], key["scope"])
                 if limit != None and yields >= limit: break
             nextcursor = data.get("nextPageCursor")
@@ -139,19 +141,21 @@
             try: metadata = json.loads(response.headers["roblox-entry-attributes"])
             except(KeyError): metadata = {}
             try: userids = json.loads(response.headers["roblox-entry-userids"])
             except(KeyError): userids = []
             
             return json.loads(response.text), EntryInfo(response.headers["roblox-entry-version"], response.headers["roblox-entry-created-time"],
     response.headers["roblox-entry-version-created-time"], userids, metadata)
-        elif response.status_code == 401: raise InvalidKey("Your key may have expired, or may not have permission to access this resource.")
-        elif response.status_code == 404: raise NotFound(f"The key {key} does not exist.")
-        elif response.status_code == 429: raise RateLimited("You're being rate limited.")
-        elif response.status_code >= 500: raise ServiceUnavailable("The service is unavailable or has encountered an error.")
-        else: raise rblx_opencloudException(f"Unexpected HTTP {response.status_code}")
+        elif response.status_code == 400: raise rblx_opencloudException(response.json()["message"])
+        elif response.status_code == 401: raise InvalidKey(response.text)
+        elif response.status_code == 403: raise InvalidKey(response.json()["message"])
+        elif response.status_code == 404: raise NotFound(response.json()["message"])
+        elif response.status_code == 429: raise RateLimited(response.json()["message"])
+        elif response.status_code >= 500: raise ServiceUnavailable(f"Internal Server Error: '{response.text}'")
+        else: raise rblx_opencloudException(f"Unexpected HTTP {response.status_code}: '{response.text}'")
 
     def set(self, key: str, value: Union[str, dict, list, int, float], users:Optional[list[int]]=None, metadata:dict={}, exclusive_create:bool=False, previous_version:Optional[str]=None) -> EntryVersion:
         """Sets the value of a key. If `DataStore.scope` is `None` then `key` must be formatted like `scope/key`."""
         if previous_version and exclusive_create: raise ValueError("previous_version and exclusive_create can not both be set")
         try:
             scope = self.scope
             if not scope: scope, key = key.split("/", maxsplit=1)
@@ -169,17 +173,20 @@
                 "exclusiveCreate": exclusive_create,
                 "matchVersion": previous_version
             })
         
         if response.status_code == 200:
             data = json.loads(response.text)
             return EntryVersion(data["version"], data["deleted"], data["contentLength"], data["createdTime"], data["objectCreatedTime"], self, key, self.scope if self.scope else scope)
-        elif response.status_code == 401: raise InvalidKey("Your key may have expired, or may not have permission to access this resource.")
-        elif response.status_code == 429: raise RateLimited("You're being rate limited.")
-        elif response.status_code >= 500: raise ServiceUnavailable("The service is unavailable or has encountered an error.")
+        elif response.status_code == 400: raise rblx_opencloudException(response.json()["message"])
+        elif response.status_code == 401: raise InvalidKey(response.text)
+        elif response.status_code == 403: raise InvalidKey(response.json()["message"])
+        elif response.status_code == 404: raise NotFound(response.json()["message"])
+        elif response.status_code == 429: raise RateLimited(response.json()["message"])
+        elif response.status_code >= 500: raise ServiceUnavailable(f"Internal Server Error: '{response.text}'")
         elif response.status_code == 412:
             try: metadata = json.loads(response.headers["roblox-entry-attributes"])
             except(KeyError): metadata = {}
             try: userids = json.loads(response.headers["roblox-entry-userids"])
             except(KeyError): userids = []
 
             if exclusive_create:
@@ -187,15 +194,15 @@
             elif previous_version:
                 error = f"The current version is not '{previous_version}'"
             else:
                 error = "A Precondition Failed"
 
             raise PreconditionFailed(json.loads(response.text), EntryInfo(response.headers["roblox-entry-version"], response.headers["roblox-entry-created-time"],
     response.headers["roblox-entry-version-created-time"], userids, metadata), error)
-        else: raise rblx_opencloudException(f"Unexpected HTTP {response.status_code}")
+        else: raise rblx_opencloudException(f"Unexpected HTTP {response.status_code}: '{response.text}'")
 
     def increment(self, key: str, increment: Union[int, float], users:Optional[list[int]]=None, metadata:dict={}) -> tuple[Union[str, dict, list, int, float], EntryInfo]:
         """Increments the value of a key. If `DataStore.scope` is `None` then `key` must be formatted like `scope/key`."""
         try:
             scope = self.scope
             if not scope: scope, key = key.split("/", maxsplit=1)
         except(ValueError):
@@ -214,18 +221,21 @@
             try: metadata = json.loads(response.headers["roblox-entry-attributes"])
             except(KeyError): metadata = {}
             try: userids = json.loads(response.headers["roblox-entry-userids"])
             except(KeyError): userids = []
             
             return json.loads(response.text), EntryInfo(response.headers["roblox-entry-version"], response.headers["roblox-entry-created-time"],
     response.headers["roblox-entry-version-created-time"], userids, metadata)
-        elif response.status_code == 401: raise InvalidKey("Your key may have expired, or may not have permission to access this resource.")
-        elif response.status_code == 429: raise RateLimited("You're being rate limited.")
-        elif response.status_code >= 500: raise ServiceUnavailable("The service is unavailable or has encountered an error.")
-        else: raise rblx_opencloudException(f"Unexpected HTTP {response.status_code}")
+        elif response.status_code == 400: raise rblx_opencloudException(response.json()["message"])
+        elif response.status_code == 401: raise InvalidKey(response.text)
+        elif response.status_code == 403: raise InvalidKey(response.json()["message"])
+        elif response.status_code == 404: raise NotFound(response.json()["message"])
+        elif response.status_code == 429: raise RateLimited(response.json()["message"])
+        elif response.status_code >= 500: raise ServiceUnavailable(f"Internal Server Error: '{response.text}'")
+        else: raise rblx_opencloudException(f"Unexpected HTTP {response.status_code}: '{response.text}'")
     
     def remove(self, key: str) -> None:
         """Removes a key. If `DataStore.scope` is `None` then `key` must be formatted like `scope/key`."""
         try:
             scope = self.scope
             if not scope: scope, key = key.split("/", maxsplit=1)
         except(ValueError):
@@ -234,19 +244,21 @@
             headers={"x-api-key": self.__api_key}, params={
                 "datastoreName": self.name,
                 "scope": scope,
                 "entryKey": key
             })
 
         if response.status_code == 204: return None
-        elif response.status_code == 401: raise InvalidKey("Your key may have expired, or may not have permission to access this resource.")
-        elif response.status_code == 404: raise NotFound(f"The key {key} does not exist.")
-        elif response.status_code == 429: raise RateLimited("You're being rate limited.")
-        elif response.status_code >= 500: raise ServiceUnavailable("The service is unavailable or has encountered an error.")
-        else: raise rblx_opencloudException(f"Unexpected HTTP {response.status_code}")
+        elif response.status_code == 400: raise rblx_opencloudException(response.json()["message"])
+        elif response.status_code == 401: raise InvalidKey(response.text)
+        elif response.status_code == 403: raise InvalidKey(response.json()["message"])
+        elif response.status_code == 404: raise NotFound(response.json()["message"])
+        elif response.status_code == 429: raise RateLimited(response.json()["message"])
+        elif response.status_code >= 500: raise ServiceUnavailable(f"Internal Server Error: '{response.text}'")
+        else: raise rblx_opencloudException(f"Unexpected HTTP {response.status_code}: '{response.text}'")
     
     def list_versions(self, key: str, after: Optional[datetime.datetime]=None, before: Optional[datetime.datetime]=None, limit: Optional[int]=None, descending: bool=True) -> Iterable[EntryVersion]:
         """Returns an Iterable of previous versions of a key. If `DataStore.scope` is `None` then `key` must be formatted like `scope/key`. The example below would list all versions, along with their value.
                 
         ```py
             for version in datastore.list_versions("key-name"):
                 print(version, version.get_value())
@@ -272,19 +284,21 @@
                     "entryKey": key,
                     "sortOrder": "Descending" if descending else "Ascending",
                     "cursor": nextcursor if nextcursor else None,
                     "startTime": after.isoformat() if after else None,
                     "endTime": before.isoformat() if before else None
                 })
             
-            if response.status_code == 401: raise InvalidKey("Your key may have expired, or may not have permission to access this resource.")
-            elif response.status_code == 404: raise NotFound("The datastore you're trying to access does not exist.")
-            elif response.status_code == 429: raise RateLimited("You're being rate limited.")
-            elif response.status_code >= 500: raise ServiceUnavailable("The service is unavailable or has encountered an error.")
-            elif not response.ok: raise rblx_opencloudException(f"Unexpected HTTP {response.status_code}")
+            if response.status_code == 400: raise rblx_opencloudException(response.json()["message"])
+            elif response.status_code == 401: raise InvalidKey(response.text)
+            elif response.status_code == 403: raise InvalidKey(response.json()["message"])
+            elif response.status_code == 404: raise NotFound(response.json()["message"])
+            elif response.status_code == 429: raise RateLimited(response.json()["message"])
+            elif response.status_code >= 500: raise ServiceUnavailable(f"Internal Server Error: '{response.text}'")
+            elif not response.ok: raise rblx_opencloudException(f"Unexpected HTTP {response.status_code}: '{response.text}'")
 
             data = response.json()
             for version in data["versions"]:
                 yields += 1
                 yield EntryVersion(version["version"], version["deleted"], version["contentLength"], version["createdTime"], version["objectCreatedTime"], self, key, self.scope if self.scope else scope)
                 if limit == None or yields >= limit: break
             nextcursor = data.get("nextPageCursor")
@@ -309,19 +323,25 @@
             try: metadata = json.loads(response.headers["roblox-entry-attributes"])
             except(KeyError): metadata = {}
             try: userids = json.loads(response.headers["roblox-entry-userids"])
             except(KeyError): userids = []
             
             return json.loads(response.text), EntryInfo(response.headers["roblox-entry-version"], response.headers["roblox-entry-created-time"],
                 response.headers["roblox-entry-version-created-time"], userids, metadata)
-        elif response.status_code == 401: raise InvalidKey("Your key may have expired, or may not have permission to access this resource.")
-        elif response.status_code == 404: raise NotFound(f"The key {key} does not exist.")
-        elif response.status_code == 429: raise RateLimited("You're being rate limited.")
-        elif response.status_code >= 500: raise ServiceUnavailable("The service is unavailable or has encountered an error.")
-        else: raise rblx_opencloudException(f"Unexpected HTTP {response.status_code}")
+        elif response.status_code == 400:
+            if response.json()["message"] == "Invalid version id.":
+                raise NotFound(response.json()["message"])
+            else:
+                raise rblx_opencloudException(response.json()["message"])
+        elif response.status_code == 401: raise InvalidKey(response.text)
+        elif response.status_code == 403: raise InvalidKey(response.json()["message"])
+        elif response.status_code == 404: raise NotFound(response.json()["message"])
+        elif response.status_code == 429: raise RateLimited(response.json()["message"])
+        elif response.status_code >= 500: raise ServiceUnavailable(f"Internal Server Error: '{response.text}'")
+        else: raise rblx_opencloudException(f"Unexpected HTTP {response.status_code}: '{response.text}'")
 
 class SortedEntry():
     def __init__(self, key: str, value: int, scope: str="global") -> None:
         self.key: str = key
         self.scope: str = scope
         self.value: int = value
     
@@ -363,19 +383,22 @@
             response = requests.get(f"https://apis.roblox.com/ordered-data-stores/v1/universes/{self.experince.id}/orderedDataStores/{urllib.parse.quote(self.name)}/scopes/{urllib.parse.quote(self.scope)}/entries",
                 headers={"x-api-key": self.__api_key}, params={
                 "max_page_size": limit if limit and limit < 100 else 100,
                 "order_by": "desc" if descending else None,
                 "page_token": nextcursor if nextcursor else None,
                 "filter": filter
             })
-            if response.status_code == 401 or response.status_code == 403: raise InvalidKey("Your key may have expired, or may not have permission to access this resource.")
-            elif response.status_code == 404: raise NotFound("The datastore you're trying to access does not exist.")
-            elif response.status_code == 429: raise RateLimited("You're being rate limited.")
-            elif response.status_code >= 500: raise ServiceUnavailable("The service is unavailable or has encountered an error.")
-            elif not response.ok: raise rblx_opencloudException(f"Unexpected HTTP {response.status_code}")
+
+            if response.status_code == 400: raise rblx_opencloudException(response.json()["message"])
+            elif response.status_code == 401: raise InvalidKey(response.text)
+            elif response.status_code == 403: raise InvalidKey(response.json()["message"])
+            elif response.status_code == 404: raise NotFound(response.json()["message"])
+            elif response.status_code == 429: raise RateLimited(response.json()["message"])
+            elif response.status_code >= 500: raise ServiceUnavailable(f"Internal Server Error: '{response.text}'")
+            elif not response.ok: raise rblx_opencloudException(f"Unexpected HTTP {response.status_code}: '{response.text}'")
             
             data = response.json()
             for key in data["entries"]:
                 yields += 1
                 yield SortedEntry(key["id"], key["value"], self.scope)
                 if limit != None and yields >= limit: break
             nextcursor = data.get("nextPageToken")
@@ -387,19 +410,21 @@
             else: scope = self.scope
         except(ValueError): raise ValueError("a scope and key seperated by a forward slash is required for OrderedDataStore without a scope.")
 
         response = requests.get(f"https://apis.roblox.com/ordered-data-stores/v1/universes/{self.experince.id}/orderedDataStores/{urllib.parse.quote(self.name)}/scopes/{urllib.parse.quote(scope)}/entries/{urllib.parse.quote(key)}",
             headers={"x-api-key": self.__api_key})
         
         if response.status_code == 200: return int(response.json()["value"])
-        elif response.status_code == 401: raise InvalidKey("Your key may have expired, or may not have permission to access this resource.")
-        elif response.status_code == 404: raise NotFound(f"The key {key} does not exist.")
-        elif response.status_code == 429: raise RateLimited("You're being rate limited.")
-        elif response.status_code >= 500: raise ServiceUnavailable("The service is unavailable or has encountered an error.")
-        else: raise rblx_opencloudException(f"Unexpected HTTP {response.status_code}")
+        elif response.status_code == 400: raise rblx_opencloudException(response.json()["message"])
+        elif response.status_code == 401: raise InvalidKey(response.text)
+        elif response.status_code == 403: raise InvalidKey(response.json()["message"])
+        elif response.status_code == 404: raise NotFound(response.json()["message"])
+        elif response.status_code == 429: raise RateLimited(response.json()["message"])
+        elif response.status_code >= 500: raise ServiceUnavailable(f"Internal Server Error: '{response.text}'")
+        else: raise rblx_opencloudException(f"Unexpected HTTP {response.status_code}: '{response.text}'")
         
     def set(self, key: str, value: int, exclusive_create: bool=False, exclusive_update: bool=False) -> int:
         try:
             if not self.scope: scope, key = key.split("/", maxsplit=1)
             else: scope = self.scope
         except(ValueError): raise ValueError("a scope and key seperated by a forward slash is required for OrderedDataStore without a scope.")
         if exclusive_create and exclusive_update: raise ValueError("exclusive_create and exclusive_updated can not both be True")
@@ -411,58 +436,56 @@
                 })
         else:
             response = requests.post(f"https://apis.roblox.com/ordered-data-stores/v1/universes/{self.experince.id}/orderedDatastores/{urllib.parse.quote(self.name)}/scopes/{urllib.parse.quote(scope)}/entries",
                 headers={"x-api-key": self.__api_key}, params={"id": key}, json={
                     "value": value
                 })
         
-        if exclusive_create and response.status_code == 400 and response.json()["code"] == "INVALID_ARGUMENT":
-            raise PreconditionFailed(None, None, f"An entry already exists with the provided key and scope")
-        elif response.status_code == 200: return int(response.json()["value"])
-        elif response.status_code == 401: raise InvalidKey("Your key may have expired, or may not have permission to access this resource.")
-        elif response.status_code in [404, 409]:
-            if exclusive_create:
-                error = "An entry already exists with the provided key and scope"
-            elif exclusive_update:
-                error = "There is no pre-existing entry with the provided key"
+        if response.status_code == 200: return int(response.json()["value"])
+        elif response.status_code == 400:
+            if response.json()["message"] == "Entry already exists.":
+                raise PreconditionFailed(None, None, response.json()["message"])
             else:
-                error = "A Precondition Failed"
+                raise rblx_opencloudException(response.json()["message"])
+        elif response.status_code == 401: raise InvalidKey(response.text)
+        elif response.status_code == 403: raise InvalidKey(response.json()["message"])
+        elif response.status_code == 404 and exclusive_update and response.json()["code"] == "NOT_FOUND": raise PreconditionFailed(response.json()["message"])
+        elif response.status_code == 429: raise RateLimited(response.json()["message"])
+        elif response.status_code >= 500: raise ServiceUnavailable(f"Internal Server Error: '{response.text}'")
+        else: raise rblx_opencloudException(f"Unexpected HTTP {response.status_code}: '{response.text}'")
 
-            raise PreconditionFailed(None, None, error)
-        if response.status_code == 429: raise RateLimited("You're being rate limited.")
-        elif response.status_code >= 500: raise ServiceUnavailable("The service is unavailable or has encountered an error.")
-        else: raise rblx_opencloudException(f"Unexpected HTTP {response.status_code}")
-    
     def increment(self, key: str, increment: int) -> None:
         try:
             if not self.scope: scope, key = key.split("/", maxsplit=1)
             else: scope = self.scope
         except(ValueError): raise ValueError("a scope and key seperated by a forward slash is required for OrderedDataStore without a scope.")
 
         response = requests.post(f"https://apis.roblox.com/ordered-data-stores/v1/universes/{self.experince.id}/orderedDatastores/{urllib.parse.quote(self.name)}/scopes/{urllib.parse.quote(scope)}/entries/{urllib.parse.quote(key)}:increment",
             headers={"x-api-key": self.__api_key}, json={
                 "amount": increment
             })
         
         if response.status_code == 200: return int(response.json()["value"])
         elif response.status_code == 401: raise InvalidKey("Your key may have expired, or may not have permission to access this resource.")
         elif response.status_code == 404: raise NotFound(f"The key {key} does not exist.")
-        elif response.status_code == 409 and response.json()["code"] == 10: raise ValueError("New value can't be less than 0.")
+        elif response.status_code == 409 and response.json()["message"] == "Entry value outside of bounds.": raise ValueError("New value can't be less than 0.")
         elif response.status_code == 429: raise RateLimited("You're being rate limited.")
         elif response.status_code >= 500: raise ServiceUnavailable("The service is unavailable or has encountered an error.")
         else: raise rblx_opencloudException(f"Unexpected HTTP {response.status_code}")
 
     def remove(self, key: str) -> None:
         try:
             if not self.scope: scope, key = key.split("/", maxsplit=1)
             else: scope = self.scope
         except(ValueError): raise ValueError("a scope and key seperated by a forward slash is required for OrderedDataStore without a scope.")
 
         response = requests.delete(f"https://apis.roblox.com/ordered-data-stores/v1/universes/{self.experince.id}/orderedDatastores/{urllib.parse.quote(self.name)}/scopes/{urllib.parse.quote(scope)}/entries/{urllib.parse.quote(key)}",
             headers={"x-api-key": self.__api_key})
         
-        if response.status_code == 200: return None
-        elif response.status_code == 401: raise InvalidKey("Your key may have expired, or may not have permission to access this resource.")
-        elif response.status_code == 404: raise NotFound(f"The key {key} does not exist.")
-        elif response.status_code == 429: raise RateLimited("You're being rate limited.")
-        elif response.status_code >= 500: raise ServiceUnavailable("The service is unavailable or has encountered an error.")
-        else: raise rblx_opencloudException(f"Unexpected HTTP {response.status_code}")
+        if response.status_code in [200, 204]: return None
+        elif response.status_code == 400: raise rblx_opencloudException(response.json()["message"])
+        elif response.status_code == 401: raise InvalidKey(response.text)
+        elif response.status_code == 403: raise InvalidKey(response.json()["message"])
+        elif response.status_code == 404: raise NotFound(response.json()["message"])
+        elif response.status_code == 429: raise RateLimited(response.json()["message"])
+        elif response.status_code >= 500: raise ServiceUnavailable(f"Internal Server Error: '{response.text}'")
+        else: raise rblx_opencloudException(f"Unexpected HTTP {response.status_code}: '{response.text}'")
```

### Comparing `rblx-open-cloud-1.2.0/rblxopencloud/exceptions.py` & `rblx-open-cloud-1.3.0/rblxopencloud/exceptions.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,21 +6,30 @@
 __all__ = (
     "rblx_opencloudException",
     "NotFound",
     "InvalidKey",
     "RateLimited",
     "ServiceUnavailable",
     "PreconditionFailed",
+    "InsufficientScope",
     "InvalidAsset",
+    "InvalidCode"
+    "ModeratedText"
 )
 
 class rblx_opencloudException(Exception): pass
 class NotFound(rblx_opencloudException): pass
 class InvalidKey(rblx_opencloudException): pass
 class RateLimited(rblx_opencloudException): pass
 class ServiceUnavailable(rblx_opencloudException): pass
 class PreconditionFailed(rblx_opencloudException):
     def __init__(self, value, info, *args: object) -> None:
         self.value: Optional[Union[str, dict, list, int, float]] = value
         self.info: Optional[EntryInfo] = info
         super().__init__(*args)
+class InsufficientScope(InvalidKey):
+    def __init__(self, scope, *args: object) -> None:
+        self.required_scope: str = scope
+        super().__init__(*args)
+class InvalidCode(InvalidKey): pass
 class InvalidAsset(rblx_opencloudException): pass
+class ModeratedText(rblx_opencloudException): pass
```

### Comparing `rblx-open-cloud-1.2.0/rblxopencloud/experience.py` & `rblx-open-cloud-1.3.0/rblxopencloud/experience.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from .exceptions import rblx_opencloudException, InvalidKey, NotFound, RateLimited, ServiceUnavailable
 import requests, io
-
-from typing import Optional, Iterable
+from typing import Optional, Iterable, Literal
 from .datastore import DataStore, OrderedDataStore
 
 __all__ = (
     "Experience",
 )
 
 class Experience():
     def __init__(self, id: int, api_key: str):
         self.id: int = id
+        self.owner = None
         self.__api_key: str = api_key
     
     def __repr__(self) -> str:
         return f"rblxopencloud.Experience({self.id})"
     
     def get_data_store(self, name: str, scope: Optional[str]="global") -> DataStore:
         """Creates a `rblx-open-cloud.DataStore` without `DataStore.created` with the provided name and scope. If `scope` is `None` then keys require to be formatted like `scope/key` and `DataStore.list_keys` will return keys from all scopes."""
@@ -57,17 +57,19 @@
                 if limit == None or yields >= limit: break
             nextcursor = data.get("nextPageCursor")
             if not nextcursor: break
     
     def publish_message(self, topic:str, data:str):
         """
         Publishes a message to live game servers that can be recieved with [MessagingService](https://create.roblox.com/docs/reference/engine/classes/MessagingService).
+
+        The `universe-messaging-service:publish` scope is required if authentication is from OAuth2.
         """
         response = requests.post(f"https://apis.roblox.com/messaging-service/v1/universes/{self.id}/topics/{topic}",
-            headers={"x-api-key": self.__api_key}, json={"message": data})
+        json={"message": data}, headers={"x-api-key" if not self.__api_key.startswith("Bearer ") else "authorization": self.__api_key})
         if response.status_code == 200: return
         elif response.status_code == 401: raise InvalidKey("Your key may have expired, or may not have permission to access this resource.")
         elif response.status_code == 404: raise NotFound(f"The place does not exist.")
         elif response.status_code == 429: raise RateLimited("You're being rate limited.")
         elif response.status_code >= 500: raise ServiceUnavailable("The service is unavailable or has encountered an error.")
         else: raise rblx_opencloudException(f"Unexpected HTTP {response.status_code}")
```

### Comparing `rblx-open-cloud-1.2.0/setup.py` & `rblx-open-cloud-1.3.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,10 +19,12 @@
     author="TreeBen77",
     packages=[
         'rblxopencloud'
     ],
     url='https://github.com/TreeBen77/rblx-open-cloud',
     keywords='roblox, open-cloud, data-store, place-publishing, mesageing-service',
     install_requires=[
-        'requests'
+        'requests',
+        'cryptography',
+        'jwt'
     ]
 )
```

