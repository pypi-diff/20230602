# Comparing `tmp/pyhyypapihawkmod-1.0.1.dev1.tar.gz` & `tmp/pyhyypapihawkmod-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhyypapihawkmod-1.0.1.dev1.tar", last modified: Sun May 28 15:51:45 2023, max compression
+gzip compressed data, was "pyhyypapihawkmod-1.0.2.tar", last modified: Fri Jun  2 10:09:37 2023, max compression
```

## Comparing `pyhyypapihawkmod-1.0.1.dev1.tar` & `pyhyypapihawkmod-1.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 15:51:45.633455 pyhyypapihawkmod-1.0.1.dev1/
--rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.0.1.dev1/LICENSE.md
--rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.0.1.dev1/MANIFEST.in
--rw-rw-rw-   0        0        0      522 2023-05-28 15:51:45.632444 pyhyypapihawkmod-1.0.1.dev1/PKG-INFO
--rw-rw-rw-   0        0        0     1224 2023-05-28 15:48:53.000000 pyhyypapihawkmod-1.0.1.dev1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 15:51:45.618640 pyhyypapihawkmod-1.0.1.dev1/pyhyypapihawkmod/
--rw-rw-rw-   0        0        0      429 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.0.1.dev1/pyhyypapihawkmod/__init__.py
--rw-rw-rw-   0        0        0      151 2023-05-24 18:38:52.000000 pyhyypapihawkmod-1.0.1.dev1/pyhyypapihawkmod/__main__.py
--rw-rw-rw-   0        0        0     4950 2023-05-28 15:48:53.000000 pyhyypapihawkmod-1.0.1.dev1/pyhyypapihawkmod/alarm_info.py
--rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.0.1.dev1/pyhyypapihawkmod/android_checkin_pb2.py
--rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.0.1.dev1/pyhyypapihawkmod/checkin_pb2.py
--rw-rw-rw-   0        0        0    26159 2023-05-28 13:40:27.000000 pyhyypapihawkmod-1.0.1.dev1/pyhyypapihawkmod/client.py
--rw-rw-rw-   0        0        0     4005 2023-05-28 09:35:32.000000 pyhyypapihawkmod-1.0.1.dev1/pyhyypapihawkmod/constants.py
--rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.0.1.dev1/pyhyypapihawkmod/exceptions.py
--rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.0.1.dev1/pyhyypapihawkmod/mcs_pb2.py
--rw-rw-rw-   0        0        0    16227 2023-05-27 21:24:48.000000 pyhyypapihawkmod-1.0.1.dev1/pyhyypapihawkmod/push_receiver.py
-drwxrwxrwx   0        0        0        0 2023-05-28 15:51:45.630416 pyhyypapihawkmod-1.0.1.dev1/pyhyypapihawkmod.egg-info/
--rw-rw-rw-   0        0        0      522 2023-05-28 15:51:45.000000 pyhyypapihawkmod-1.0.1.dev1/pyhyypapihawkmod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      551 2023-05-28 15:51:45.000000 pyhyypapihawkmod-1.0.1.dev1/pyhyypapihawkmod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 15:51:45.000000 pyhyypapihawkmod-1.0.1.dev1/pyhyypapihawkmod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-05-28 15:51:45.000000 pyhyypapihawkmod-1.0.1.dev1/pyhyypapihawkmod.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-28 15:51:45.000000 pyhyypapihawkmod-1.0.1.dev1/pyhyypapihawkmod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-28 15:51:45.633455 pyhyypapihawkmod-1.0.1.dev1/setup.cfg
--rw-rw-rw-   0        0        0      926 2023-05-28 15:49:41.000000 pyhyypapihawkmod-1.0.1.dev1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:09:37.855742 pyhyypapihawkmod-1.0.2/
+-rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.0.2/LICENSE.md
+-rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      517 2023-06-02 10:09:37.855228 pyhyypapihawkmod-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1428 2023-06-02 09:22:09.000000 pyhyypapihawkmod-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 10:09:37.843977 pyhyypapihawkmod-1.0.2/pyhyypapihawkmod/
+-rw-rw-rw-   0        0        0      429 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.0.2/pyhyypapihawkmod/__init__.py
+-rw-rw-rw-   0        0        0      151 2023-05-24 18:38:52.000000 pyhyypapihawkmod-1.0.2/pyhyypapihawkmod/__main__.py
+-rw-rw-rw-   0        0        0     5523 2023-06-02 09:20:40.000000 pyhyypapihawkmod-1.0.2/pyhyypapihawkmod/alarm_info.py
+-rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.0.2/pyhyypapihawkmod/android_checkin_pb2.py
+-rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.0.2/pyhyypapihawkmod/checkin_pb2.py
+-rw-rw-rw-   0        0        0    27687 2023-06-02 10:07:05.000000 pyhyypapihawkmod-1.0.2/pyhyypapihawkmod/client.py
+-rw-rw-rw-   0        0        0     4005 2023-05-28 09:35:32.000000 pyhyypapihawkmod-1.0.2/pyhyypapihawkmod/constants.py
+-rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.0.2/pyhyypapihawkmod/exceptions.py
+-rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.0.2/pyhyypapihawkmod/mcs_pb2.py
+-rw-rw-rw-   0        0        0    16227 2023-05-27 21:24:48.000000 pyhyypapihawkmod-1.0.2/pyhyypapihawkmod/push_receiver.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:09:37.852651 pyhyypapihawkmod-1.0.2/pyhyypapihawkmod.egg-info/
+-rw-rw-rw-   0        0        0      517 2023-06-02 10:09:37.000000 pyhyypapihawkmod-1.0.2/pyhyypapihawkmod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      551 2023-06-02 10:09:37.000000 pyhyypapihawkmod-1.0.2/pyhyypapihawkmod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 10:09:37.000000 pyhyypapihawkmod-1.0.2/pyhyypapihawkmod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-06-02 10:09:37.000000 pyhyypapihawkmod-1.0.2/pyhyypapihawkmod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-02 10:09:37.000000 pyhyypapihawkmod-1.0.2/pyhyypapihawkmod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 10:09:37.855742 pyhyypapihawkmod-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      921 2023-06-02 10:07:47.000000 pyhyypapihawkmod-1.0.2/setup.py
```

### Comparing `pyhyypapihawkmod-1.0.1.dev1/LICENSE.md` & `pyhyypapihawkmod-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.0.1.dev1/PKG-INFO` & `pyhyypapihawkmod-1.0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.0.1.dev1
+Version: 1.0.2
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.0.1.dev1/README.md` & `pyhyypapihawkmod-1.0.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 This is a fork from https://github.com/RenierM26. This fork has reversed engineered the protobuf pb2 files and recompiled with version 4.21. THis fixes the issues on newer versions of home assistant.
 
 # pyHyypApi
 API for ADT Secure Home and IDS Hyyp. There could be more variants but it's easy to add package names to the constants.py file.
 
+
 How to use:
 
   1. Install:
 
 ```pip install pyhyypapihawkmod```
 
   2.1. Login (ADT Secure Home):
@@ -40,7 +41,20 @@
 ```
 
 TO Do:
 
 - CLI usage. (GCF client is there, just needs some more automation.)
 - Capture panic api...for obvious reasons.
 - What zone caused arm/arm stay not to work. - Looks like GCM/Firebase push messages. Added GCM client...just run main program and register GCF code in function called register gcf. It works.
+
+
+Changelog 
+
+
+1.0.1
+
+- Added fix where setups with multiple sites would crash
+- Added the ability to find "automations" and also trigger the automations
+
+1.0.0
+
+Bumped main release to 1.0.0
```

### Comparing `pyhyypapihawkmod-1.0.1.dev1/pyhyypapihawkmod/alarm_info.py` & `pyhyypapihawkmod-1.0.2/pyhyypapihawkmod/alarm_info.py`

 * *Files 10% similar despite different names*

```diff
@@ -56,22 +56,37 @@
         stay_ids = {
             stay_profile["id"]: stay_profile
             for stay_profile in self._sync_info["stayProfiles"]
         }
         partition_ids = {
             partition["id"]: partition for partition in self._sync_info["partitions"]
         }
-
+        
+        trigger_ids = {
+            trigger["id"]: trigger for trigger in self._sync_info["triggers"]
+        }
+        
         for site in site_ids:
 
             # Add last site notification.
             _last_notice = self._last_notice(site_id=site)
             site_ids[site]["lastNoticeTime"] = _last_notice["lastNoticeTime"]
             site_ids[site]["lastNoticeName"] = _last_notice["lastNoticeName"]
 
+            # Add triggers (PGM / Automations in APP)
+            for trigger_id in trigger_ids:
+                if trigger_id not in site_ids[site]["triggerIds"]:
+                    continue
+                else:
+                    site_ids[site]["triggers"] = {
+                        key: value
+                        for (key, value) in trigger_ids.items()            
+                    }
+                
+            
             # Add partition info.
             site_ids[site]["partitions"] = {
                 partition_id: partition_ids[partition_id]
                 for partition_id in site_ids[site]["partitionIds"]
             }
 
             for partition in partition_ids:
```

### Comparing `pyhyypapihawkmod-1.0.1.dev1/pyhyypapihawkmod/android_checkin_pb2.py` & `pyhyypapihawkmod-1.0.2/pyhyypapihawkmod/android_checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.0.1.dev1/pyhyypapihawkmod/checkin_pb2.py` & `pyhyypapihawkmod-1.0.2/pyhyypapihawkmod/checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.0.1.dev1/pyhyypapihawkmod/client.py` & `pyhyypapihawkmod-1.0.2/pyhyypapihawkmod/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 API_ENDPOINT_STORE_GCM_REGISTRATION_ID = "/user/storeGcmRegistrationId"
 API_ENDPOINT_ARM_SITE = "/device/armSite"
 API_ENDPOINT_TRIGGER_ALARM = "/device/triggerAlarm"
 API_ENDPOINT_SET_ZONE_BYPASS = "/device/bypass"
 API_ENDPOINT_GET_CAMERA_BY_PARTITION = "/device/getCameraByPartition"
 API_ENDPOINT_UPDATE_SUB_USER = "/user/updateSubUser"
 API_ENDPOINT_SET_NOTIFICATION_SUBSCRIPTIONS = "/user/setNotificationSubscriptionsNew"
+API_ENDPOINT_TRIGGER_AUTOMATION = "/device/trigger"
 
 
 class HyypClient:
     """Initialize api client object."""
 
     def __init__(
         self,
@@ -742,14 +743,63 @@
             ) from err
 
         if _json_result["status"] != "SUCCESS" and _json_result["error"] is not None:
             raise HyypApiError(f"Trigger alarm failed: {_json_result['error']}")
 
         return _json_result
 
+
+    def trigger_automation(
+        self,
+        site_id: int,
+        trigger_id: int | None = None,
+        pin: int | None = None,
+    ) -> Any:
+        """Trigger Alarm via API."""
+
+        _params: dict[Any, Any] = STD_PARAMS.copy()
+        _params["pin"] = pin
+        _params["siteId"] = site_id
+        _params["triggerId"] = trigger_id
+        del _params["imei"]
+        _params["clientImei"] = STD_PARAMS["imei"]
+
+        try:
+            req = self._session.post(
+                "https://" + BASE_URL + API_ENDPOINT_TRIGGER_AUTOMATION,
+                allow_redirects=False,
+                params=_params,
+                timeout=self._timeout,
+            )
+
+            req.raise_for_status()
+
+        except requests.ConnectionError as err:
+            raise InvalidURL("A Invalid URL or Proxy error occured") from err
+
+        except requests.HTTPError as err:
+            raise HTTPError from err
+
+        try:
+            _json_result: dict[Any, Any] = req.json()
+
+        except ValueError as err:
+            raise HyypApiError(
+                "Impossible to decode response: "
+                + str(err)
+                + "\nResponse was: "
+                + str(req.text)
+            ) from err
+
+        if _json_result["status"] != "SUCCESS" and _json_result["error"] is not None:
+            raise HyypApiError(f"Trigger automation failed: {_json_result['error']}")
+
+        return _json_result
+
+
     def set_zone_bypass(
         self,
         zones: int,
         partition_id: int | None = None,
         stay_profile_id: int = 0,
         pin: int | None = None,
     ) -> Any:
```

### Comparing `pyhyypapihawkmod-1.0.1.dev1/pyhyypapihawkmod/constants.py` & `pyhyypapihawkmod-1.0.2/pyhyypapihawkmod/constants.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.0.1.dev1/pyhyypapihawkmod/mcs_pb2.py` & `pyhyypapihawkmod-1.0.2/pyhyypapihawkmod/mcs_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.0.1.dev1/pyhyypapihawkmod/push_receiver.py` & `pyhyypapihawkmod-1.0.2/pyhyypapihawkmod/push_receiver.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.0.1.dev1/pyhyypapihawkmod.egg-info/PKG-INFO` & `pyhyypapihawkmod-1.0.2/pyhyypapihawkmod.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.0.1.dev1
+Version: 1.0.2
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.0.1.dev1/pyhyypapihawkmod.egg-info/SOURCES.txt` & `pyhyypapihawkmod-1.0.2/pyhyypapihawkmod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.0.1.dev1/setup.py` & `pyhyypapihawkmod-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyhyypapihawkmod',
-    version="1.0.1.dev1",
+    version="1.0.2",
     license='Apache Software License 2.0',
     author='hawky358 (Original code by Renier Moorcroft)',
     author_email='hawky358@users.github.com',
     description='IDS Hyyp/ADT Secure Home API',
     long_description="API for accessing IDS Hyyp. This is used by ADT Home Connect and possibly others. Please view readme on github (Based on 0.0.0.8 by Renier Moorcroft with updated protobuf files) ",
     url='https://github.com/hawky358/pyHyypApi',
     packages=setuptools.find_packages(),
```

