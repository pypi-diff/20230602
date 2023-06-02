# Comparing `tmp/microservicebus-py-0.9.1.tar.gz` & `tmp/microservicebus-py-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microservicebus-py-0.9.1.tar", last modified: Fri Apr 28 14:19:27 2023, max compression
+gzip compressed data, was "microservicebus-py-0.9.2.tar", last modified: Fri Jun  2 10:03:27 2023, max compression
```

## Comparing `microservicebus-py-0.9.1.tar` & `microservicebus-py-0.9.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2023-04-28 14:19:27.627327 microservicebus-py-0.9.1/
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4745 2023-04-28 14:19:27.623328 microservicebus-py-0.9.1/PKG-INFO
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3680 2022-12-12 08:25:32.000000 microservicebus-py-0.9.1/README.md
-drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2023-04-28 14:19:27.155788 microservicebus-py-0.9.1/microservicebus_py.egg-info/
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4745 2023-04-28 14:19:26.000000 microservicebus-py-0.9.1/microservicebus_py.egg-info/PKG-INFO
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)      455 2023-04-28 14:19:26.000000 microservicebus-py-0.9.1/microservicebus_py.egg-info/SOURCES.txt
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)        1 2023-04-28 14:19:26.000000 microservicebus-py-0.9.1/microservicebus_py.egg-info/dependency_links.txt
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)       55 2023-04-28 14:19:26.000000 microservicebus-py-0.9.1/microservicebus_py.egg-info/entry_points.txt
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)        4 2023-04-28 14:19:26.000000 microservicebus-py-0.9.1/microservicebus_py.egg-info/top_level.txt
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)       38 2023-04-28 14:19:27.629352 microservicebus-py-0.9.1/setup.cfg
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     1711 2023-04-28 14:15:01.000000 microservicebus-py-0.9.1/setup.py
-drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2023-04-28 14:19:27.591430 microservicebus-py-0.9.1/src/
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)      807 2022-12-19 11:22:24.000000 microservicebus-py-0.9.1/src/axians.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     5687 2023-03-06 08:28:59.000000 microservicebus-py-0.9.1/src/base_service.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     1324 2023-01-05 09:33:48.000000 microservicebus-py-0.9.1/src/logger_service.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)    29588 2023-04-26 22:27:47.000000 microservicebus-py-0.9.1/src/msb_handler.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     6536 2023-03-06 08:30:37.000000 microservicebus-py-0.9.1/src/orchestrator_service.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)      340 2022-03-14 19:13:32.000000 microservicebus-py-0.9.1/src/queue_message.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4414 2022-12-02 13:59:45.000000 microservicebus-py-0.9.1/src/rauc_handler.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)      807 2023-01-24 11:06:53.000000 microservicebus-py-0.9.1/src/start.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3311 2023-01-09 21:54:56.000000 microservicebus-py-0.9.1/src/terminal_service.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)      672 2022-03-23 09:36:17.000000 microservicebus-py-0.9.1/src/test.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)      472 2022-04-27 07:36:56.000000 microservicebus-py-0.9.1/src/utils.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3136 2022-12-12 08:35:01.000000 microservicebus-py-0.9.1/src/vpn_helper.py
+drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2023-06-02 10:03:27.388543 microservicebus-py-0.9.2/
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4745 2023-06-02 10:03:27.383549 microservicebus-py-0.9.2/PKG-INFO
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3680 2022-12-12 08:25:32.000000 microservicebus-py-0.9.2/README.md
+drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2023-06-02 10:03:26.963785 microservicebus-py-0.9.2/microservicebus_py.egg-info/
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4745 2023-06-02 10:03:26.000000 microservicebus-py-0.9.2/microservicebus_py.egg-info/PKG-INFO
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)      455 2023-06-02 10:03:26.000000 microservicebus-py-0.9.2/microservicebus_py.egg-info/SOURCES.txt
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)        1 2023-06-02 10:03:26.000000 microservicebus-py-0.9.2/microservicebus_py.egg-info/dependency_links.txt
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)       55 2023-06-02 10:03:26.000000 microservicebus-py-0.9.2/microservicebus_py.egg-info/entry_points.txt
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)        4 2023-06-02 10:03:26.000000 microservicebus-py-0.9.2/microservicebus_py.egg-info/top_level.txt
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)       38 2023-06-02 10:03:27.389544 microservicebus-py-0.9.2/setup.cfg
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     1707 2023-06-02 09:59:05.000000 microservicebus-py-0.9.2/setup.py
+drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2023-06-02 10:03:27.351061 microservicebus-py-0.9.2/src/
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)      807 2022-12-19 11:22:24.000000 microservicebus-py-0.9.2/src/axians.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     5689 2023-05-31 17:27:32.000000 microservicebus-py-0.9.2/src/base_service.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     1324 2023-01-05 09:33:48.000000 microservicebus-py-0.9.2/src/logger_service.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)    29617 2023-06-02 09:27:26.000000 microservicebus-py-0.9.2/src/msb_handler.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     6536 2023-03-06 08:30:37.000000 microservicebus-py-0.9.2/src/orchestrator_service.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)      340 2022-03-14 19:13:32.000000 microservicebus-py-0.9.2/src/queue_message.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4414 2022-12-02 13:59:45.000000 microservicebus-py-0.9.2/src/rauc_handler.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)      846 2023-06-02 09:05:37.000000 microservicebus-py-0.9.2/src/start.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3311 2023-01-09 21:54:56.000000 microservicebus-py-0.9.2/src/terminal_service.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)      672 2022-03-23 09:36:17.000000 microservicebus-py-0.9.2/src/test.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3971 2023-06-02 09:05:37.000000 microservicebus-py-0.9.2/src/utils.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3136 2022-12-12 08:35:01.000000 microservicebus-py-0.9.2/src/vpn_helper.py
```

### Comparing `microservicebus-py-0.9.1/PKG-INFO` & `microservicebus-py-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microservicebus-py
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python agent for microServiceBus.com. Please visit https://microservicebus.com for more information.
 Home-page: https://github.com/axians/microservicebus-py
 Author: AXIANS IoT Operations
 Author-email: microservicebus@axians.com
 License: MIT
 Description: # microservicebus-py
```

### Comparing `microservicebus-py-0.9.1/README.md` & `microservicebus-py-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.1/microservicebus_py.egg-info/PKG-INFO` & `microservicebus-py-0.9.2/microservicebus_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microservicebus-py
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python agent for microServiceBus.com. Please visit https://microservicebus.com for more information.
 Home-page: https://github.com/axians/microservicebus-py
 Author: AXIANS IoT Operations
 Author-email: microservicebus@axians.com
 License: MIT
 Description: # microservicebus-py
```

### Comparing `microservicebus-py-0.9.1/setup.py` & `microservicebus-py-0.9.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,16 +19,14 @@
 thelibFolder = os.path.dirname(os.path.realpath(__file__))
 requirementPath = thelibFolder + '/requirements.txt'
 install_req = []  # Here we'll get: ["gunicorn", "docutils>=0.3", "lxml==0.5a7"]
 if os.path.isfile(requirementPath):
     with open(requirementPath) as f:
         install_req = f.read().splitlines()
 
-
-
 # This call to setup() does all the work
 setup(
     name=settings["name"],
     version                         = settings["version"],
     description                     = settings["description"],
     long_description_content_type   = settings["long_description_content_type"],
     url                             = settings["url"],
```

### Comparing `microservicebus-py-0.9.1/src/axians.py` & `microservicebus-py-0.9.2/src/axians.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.1/src/base_service.py` & `microservicebus-py-0.9.2/src/base_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,14 +52,15 @@
             settings = {
                 "hubUri": self.base_uri
             }
             self.save_settings(settings)
         
         return settings
 
+
     async def msb_signed_in(self, args):
         pass
     # endregion
 
     # region Communication functions
     async def SubmitAction(self, destination, action, message):
         msg = QueueMessage(self.id, destination, action, message)
```

### Comparing `microservicebus-py-0.9.1/src/logger_service.py` & `microservicebus-py-0.9.2/src/logger_service.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.1/src/msb_handler.py` & `microservicebus-py-0.9.2/src/msb_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,19 +27,20 @@
 class microServiceBusHandler(BaseService):
     # region Constructor
     def __init__(self, id, queue):
         self.ready = False
         self._connected = False
         self._reconnect = False
         self._missedheartbeat = 0
-        self.base_uri = "https://microservicebus.com"
+
+        self.base_uri = os.getenv('MSB_HOST') if os.getenv('MSB_HOST') != None else "https://microservicebus.com"
+                
         home = str(Path.home())
         self.msb_dir = f"{os.environ['HOME']}/msb-py"
-        self.printf(f"os.environ =  {os.environ}")
-
+        
         self.service_path = f"{self.msb_dir}/services"
         self.msb_settings_path = f"{self.msb_dir}/settings.json"
         try:
             from rauc_handler import RaucHandler
             self.rauc_handler = RaucHandler()
         except Exception as e:
             self.printf("")
@@ -49,15 +50,14 @@
     # endregion
     # region Base functions
 
     async def Start(self):
         try:
             
             self.settings = self.get_settings()
-            
             if "hubUri" in self.settings:
                 self.base_uri = self.settings["hubUri"]
             else:
                 self.printf("hubUri not set")
                 self.settings["hubUri"] = self.base_uri
 
             await self.Debug(f"instance: {self.base_uri}")
@@ -348,15 +348,16 @@
 
         asyncio.run(self.Debug(f"Node {node_name} signed in successfully"))
         
         if "hubUri" not in self.settings:
             sign_in_response["hubUri"] = self.settings["hubUri"]
         
         sign_in_response["hubUri"] = self.base_uri
-        self.save_settings(sign_in_response)
+        self.save_settings(sign_in_response)        
+        
         asyncio.run(self.SubmitAction("*", "msb_signed_in", {}))
         
         if os.path.isdir(self.service_path) == False:
             os.mkdir(self.service_path)
 
         state = self.settings["state"]
         asyncio.run(self.Debug(f"Node state {state}"))
@@ -569,15 +570,15 @@
         rootfs0_status = platform_status["rootfs0"]["state"]
         current_platform = platform_status["rootfs0"] if rootfs0_status == "booted" else platform_status["rootfs1"]
         platform = current_platform["bundle.compatible"]
         current_version = current_platform["bundle.version"]
         boot_status = current_platform["boot-status"]
         installed = current_platform["installed.timestamp"]
 
-        uri = "https://microservicebus.com/api/nodeimages/" + \
+        uri = f"{self.base_uri}/api/nodeimages/" + \
             self.get_settings()["organizationId"] + "/" + platform
         self.printf("Notified on new firmware")
         self.printf("Current firmware platform: " + platform)
         self.printf("Current firmware version: " + current_version)
         self.printf("Current boot status: " + boot_status)
         self.printf("Current firmware installed: " + installed)
```

### Comparing `microservicebus-py-0.9.1/src/orchestrator_service.py` & `microservicebus-py-0.9.2/src/orchestrator_service.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.1/src/rauc_handler.py` & `microservicebus-py-0.9.2/src/rauc_handler.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.1/src/start.py` & `microservicebus-py-0.9.2/src/start.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 #!/usr/bin/python3
 import asyncio
 import logging
 import os
 import sys
+import utils
+
 sys.path.insert(1, os.path.dirname(__file__))
+
+#utils.check_version()
+
 from orchestrator_service import Orchestrator
 
 logging.basicConfig(
     level=logging.WARNING,
     format="%(asctime)s,%(msecs)d %(levelname)s: %(message)s",
     datefmt="%H:%M:%S",
 )
```

### Comparing `microservicebus-py-0.9.1/src/terminal_service.py` & `microservicebus-py-0.9.2/src/terminal_service.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.1/src/test.py` & `microservicebus-py-0.9.2/src/test.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.1/src/vpn_helper.py` & `microservicebus-py-0.9.2/src/vpn_helper.py`

 * *Files identical despite different names*

