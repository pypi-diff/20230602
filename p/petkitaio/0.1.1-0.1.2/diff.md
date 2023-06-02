# Comparing `tmp/petkitaio-0.1.1.tar.gz` & `tmp/petkitaio-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petkitaio-0.1.1.tar", last modified: Wed Feb 22 20:40:46 2023, max compression
+gzip compressed data, was "petkitaio-0.1.2.tar", last modified: Fri Jun  2 03:02:44 2023, max compression
```

## Comparing `petkitaio-0.1.1.tar` & `petkitaio-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-02-22 20:40:46.337437 petkitaio-0.1.1/
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1067 2023-02-16 00:09:30.000000 petkitaio-0.1.1/LICENSE
--rw-r--r--   0 robertdrinovac   (501) staff       (20)     5034 2023-02-22 20:40:46.337625 petkitaio-0.1.1/PKG-INFO
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     3580 2023-02-16 00:09:30.000000 petkitaio-0.1.1/README.md
-drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-02-22 20:40:46.334673 petkitaio-0.1.1/petkitaio/
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1433 2023-02-16 00:09:30.000000 petkitaio-0.1.1/petkitaio/__init__.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     6051 2023-02-16 00:09:30.000000 petkitaio-0.1.1/petkitaio/constants.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)      647 2023-02-16 00:09:30.000000 petkitaio-0.1.1/petkitaio/exceptions.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1148 2023-02-16 00:09:30.000000 petkitaio-0.1.1/petkitaio/model.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)    33694 2023-02-16 00:09:30.000000 petkitaio-0.1.1/petkitaio/petkit_client.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)      680 2023-02-16 00:09:30.000000 petkitaio-0.1.1/petkitaio/str_enum.py
-drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-02-22 20:40:46.337135 petkitaio-0.1.1/petkitaio.egg-info/
--rw-r--r--   0 robertdrinovac   (501) staff       (20)     5034 2023-02-22 20:40:46.000000 petkitaio-0.1.1/petkitaio.egg-info/PKG-INFO
--rw-r--r--   0 robertdrinovac   (501) staff       (20)      337 2023-02-22 20:40:46.000000 petkitaio-0.1.1/petkitaio.egg-info/SOURCES.txt
--rw-r--r--   0 robertdrinovac   (501) staff       (20)        1 2023-02-22 20:40:46.000000 petkitaio-0.1.1/petkitaio.egg-info/dependency_links.txt
--rw-r--r--   0 robertdrinovac   (501) staff       (20)       28 2023-02-22 20:40:46.000000 petkitaio-0.1.1/petkitaio.egg-info/requires.txt
--rw-r--r--   0 robertdrinovac   (501) staff       (20)       10 2023-02-22 20:40:46.000000 petkitaio-0.1.1/petkitaio.egg-info/top_level.txt
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)       38 2023-02-22 20:40:46.338191 petkitaio-0.1.1/setup.cfg
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1022 2023-02-22 20:39:43.000000 petkitaio-0.1.1/setup.py
+drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-06-02 03:02:44.187123 petkitaio-0.1.2/
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1067 2023-06-02 02:50:52.000000 petkitaio-0.1.2/LICENSE
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)     5340 2023-06-02 03:02:44.187333 petkitaio-0.1.2/PKG-INFO
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)     3853 2023-06-02 02:50:52.000000 petkitaio-0.1.2/README.md
+drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-06-02 03:02:44.184608 petkitaio-0.1.2/petkitaio/
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1550 2023-06-02 02:50:52.000000 petkitaio-0.1.2/petkitaio/__init__.py
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)     8893 2023-06-02 02:50:52.000000 petkitaio-0.1.2/petkitaio/constants.py
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)      835 2023-06-02 02:50:52.000000 petkitaio-0.1.2/petkitaio/exceptions.py
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1148 2023-06-02 02:50:52.000000 petkitaio-0.1.2/petkitaio/model.py
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)    37648 2023-06-02 02:50:52.000000 petkitaio-0.1.2/petkitaio/petkit_client.py
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)      680 2023-06-02 02:50:52.000000 petkitaio-0.1.2/petkitaio/str_enum.py
+drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-06-02 03:02:44.186790 petkitaio-0.1.2/petkitaio.egg-info/
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)     5340 2023-06-02 03:02:44.000000 petkitaio-0.1.2/petkitaio.egg-info/PKG-INFO
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)      337 2023-06-02 03:02:44.000000 petkitaio-0.1.2/petkitaio.egg-info/SOURCES.txt
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)        1 2023-06-02 03:02:44.000000 petkitaio-0.1.2/petkitaio.egg-info/dependency_links.txt
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)       28 2023-06-02 03:02:44.000000 petkitaio-0.1.2/petkitaio.egg-info/requires.txt
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)       10 2023-06-02 03:02:44.000000 petkitaio-0.1.2/petkitaio.egg-info/top_level.txt
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)       38 2023-06-02 03:02:44.188002 petkitaio-0.1.2/setup.cfg
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1050 2023-06-02 02:50:52.000000 petkitaio-0.1.2/setup.py
```

### Comparing `petkitaio-0.1.1/LICENSE` & `petkitaio-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `petkitaio-0.1.1/PKG-INFO` & `petkitaio-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: petkitaio
-Version: 0.1.1
+Version: 0.1.2
 Summary: Asynchronous Python library for PetKit's API
 Home-page: https://github.com/RobertD502/petkitaio
 Author: Robert Drinovac
 Author-email: unlisted@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/RobertD502/petkitaio/issues
 Project-URL: Source, https://github.com/RobertD502/petkitaio/
 Description: # PetKitAIO
         
         Asynchronous Python library for PetKit's API.
         
-        This is PetKit's undocumented API. With that said, future changes made by PetKit may break this library. All API calls are made to PetKit's USA servers.
+        This is PetKit's undocumented API. With that said, future changes made by PetKit may break this library. The API endpoint used is determined based on the region your account is locked to. Although support has been added for the PetKit Asia API endpoint, I have not personally tested it.
         
         ## **Currently Supported Devices**:
         - [D3 Feeder (Fresh Element Infinity)](https://www.amazon.com/PETKIT-Automatic-Stainless-Programmable-Dispenser/dp/B09JFK8BCQ)
         - [D4 Feeder (Fresh Element Solo)](https://www.amazon.com/PETKIT-Automatic-Dispenser-Compatible-Freeze-Dried/dp/B09158J9PF/)
         - [Mini Feeder](https://www.amazon.com/PETKIT-Automatic-Stainless-Indicator-Dispenser-2-8L/dp/B08GS1CPHH/)
         - [W5 Water Fountain (Eversweet 3 Pro)](https://www.amazon.com/PETKIT-Wireless-Fountain-Stainless-Dispenser/dp/B09QRH6L3M/)
         - [T3 Litter Box (Pura X)](https://www.amazon.com/PETKIT-Self-Cleaning-Scooping-Automatic-Multiple/dp/B08T9CCP1M)
+        - [T4 Litter Box (Pura MAX) with/without Pura Air](https://www.amazon.com/PETKIT-Self-Cleaning-Capacity-Multiple-Automatic/dp/B09KC7Q4YF)
         
         ## Important
         
         PetKit accounts can only be logged in on one device at a time. Using this library will result in getting signed out of the mobile app. You can avoid this by creating a secondary account and sharing devices from the main account (except water fountains). However, some device functionality is lost when using a secondary account as well as not being able to share pets between accounts.
         
         
         This package depends on [aiohttp](https://docs.aiohttp.org/en/stable/) and [tzlocal](https://pypi.org/project/tzlocal/). `Python 3.7` or greater is required.
@@ -78,15 +79,15 @@
         # See constants.py FeederSetting class for available settings
         # Additional import needed:
         from petkitaio.constants import FeederSetting
         
         
         # Enabling child lock on a D4 feeder. Note: Mini Feeders use a different setting.
         # Reusing retrieved devices from above.
-        await client.update_feeder_settings(feeder=devices.feeders[feederid], setting=FeederSetting.CHILDLOCK, value=1)
+        await client.update_feeder_settings(feeder=devices.feeders[feederid], setting=FeederSetting.CHILD_LOCK, value=1)
         ```
         
         ### Reset Feeder Desiccant
         ```python
         # Reusing retrieved devices from above.
         await client.reset_feeder_desiccant(feeder=devices.feeders[feederid])
         ```
@@ -98,14 +99,14 @@
         # Additional import needed:
         from petkitaio.constants import W5Command
         
         # Set Water Fountain to Smart Mode. Reusing retrieved devices from above.
         await client.control_water_fountain(water_fountain=devices.water_fountains[water_fountain_id], command=W5Command.SMART)
         ```
         
-Keywords: petkit,eversweet 3 pro,feeder mini,d4,petkit feeder,petkit water fountain,freshelement solo
+Keywords: petkit,eversweet 3 pro,feeder mini,d4,petkit feeder,petkit water fountain,freshelement solo,pura x,pura max,pura air
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `petkitaio-0.1.1/README.md` & `petkitaio-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # PetKitAIO
 
 Asynchronous Python library for PetKit's API.
 
-This is PetKit's undocumented API. With that said, future changes made by PetKit may break this library. All API calls are made to PetKit's USA servers.
+This is PetKit's undocumented API. With that said, future changes made by PetKit may break this library. The API endpoint used is determined based on the region your account is locked to. Although support has been added for the PetKit Asia API endpoint, I have not personally tested it.
 
 ## **Currently Supported Devices**:
 - [D3 Feeder (Fresh Element Infinity)](https://www.amazon.com/PETKIT-Automatic-Stainless-Programmable-Dispenser/dp/B09JFK8BCQ)
 - [D4 Feeder (Fresh Element Solo)](https://www.amazon.com/PETKIT-Automatic-Dispenser-Compatible-Freeze-Dried/dp/B09158J9PF/)
 - [Mini Feeder](https://www.amazon.com/PETKIT-Automatic-Stainless-Indicator-Dispenser-2-8L/dp/B08GS1CPHH/)
 - [W5 Water Fountain (Eversweet 3 Pro)](https://www.amazon.com/PETKIT-Wireless-Fountain-Stainless-Dispenser/dp/B09QRH6L3M/)
 - [T3 Litter Box (Pura X)](https://www.amazon.com/PETKIT-Self-Cleaning-Scooping-Automatic-Multiple/dp/B08T9CCP1M)
+- [T4 Litter Box (Pura MAX) with/without Pura Air](https://www.amazon.com/PETKIT-Self-Cleaning-Capacity-Multiple-Automatic/dp/B09KC7Q4YF)
 
 ## Important
 
 PetKit accounts can only be logged in on one device at a time. Using this library will result in getting signed out of the mobile app. You can avoid this by creating a secondary account and sharing devices from the main account (except water fountains). However, some device functionality is lost when using a secondary account as well as not being able to share pets between accounts.
 
 
 This package depends on [aiohttp](https://docs.aiohttp.org/en/stable/) and [tzlocal](https://pypi.org/project/tzlocal/). `Python 3.7` or greater is required.
@@ -68,15 +69,15 @@
 # See constants.py FeederSetting class for available settings
 # Additional import needed:
 from petkitaio.constants import FeederSetting
 
 
 # Enabling child lock on a D4 feeder. Note: Mini Feeders use a different setting.
 # Reusing retrieved devices from above.
-await client.update_feeder_settings(feeder=devices.feeders[feederid], setting=FeederSetting.CHILDLOCK, value=1)
+await client.update_feeder_settings(feeder=devices.feeders[feederid], setting=FeederSetting.CHILD_LOCK, value=1)
 ```
 
 ### Reset Feeder Desiccant
 ```python
 # Reusing retrieved devices from above.
 await client.reset_feeder_desiccant(feeder=devices.feeders[feederid])
 ```
```

### Comparing `petkitaio-0.1.1/petkitaio/__init__.py` & `petkitaio-0.1.2/petkitaio/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 from .constants import (
+    ASIA_REGIONS,
+    AUTH_ERROR_CODES,
     BLE_HEADER,
     BLUETOOTH_ERRORS,
     CLIENT_DICT,
-    ERROR_CODES,
     FEEDER_LIST,
     FeederSetting,
     LB_CMD_TO_KEY,
     LB_CMD_TO_TYPE,
     LB_CMD_TO_VALUE,
     LitterBoxCommand,
     LitterBoxCommandKey,
     LitterBoxCommandType,
     LitterBoxSetting,
     LITTER_LIST,
     PetSetting,
     Header,
     Endpoint,
     Region,
+    SERVER_ERROR_CODES,
     TIMEOUT,
     WATER_FOUNTAIN_LIST,
     W5Command,
     W5_COMMAND_TO_CODE,
     W5_DND_COMMANDS,
     W5_LIGHT_BRIGHTNESS,
     W5_LIGHT_POWER,
     W5_MODE,
     W5_SETTINGS_COMMANDS,
 )
 from .petkit_client import (PetKitClient, LOGGER,)
-from .exceptions import (AuthError, BluetoothError, PetKitError,)
+from .exceptions import (AuthError, BluetoothError, PetKitError, ServerError)
 from .model import (Feeder, LitterBox, Pet, PetKitData, W5Fountain, )
 from .str_enum import StrEnum
 
-__all__ = ['AuthError', 'BLE_HEADER', 'BluetoothError', 'BLUETOOTH_ERRORS', 'CLIENT_DICT', 'Feeder', 'Endpoint',
-           'ERROR_CODES', 'FEEDER_LIST', 'FeederSetting', 'Header', 'LB_CMD_TO_KEY', 'LB_CMD_TO_TYPE', 'LB_CMD_TO_VALUE',
+__all__ = ['ASIA_REGIONS', 'AuthError', 'AUTH_ERROR_CODES', 'BLE_HEADER', 'BluetoothError', 'BLUETOOTH_ERRORS', 'CLIENT_DICT', 'Feeder', 'Endpoint',
+           'FEEDER_LIST', 'FeederSetting', 'Header', 'LB_CMD_TO_KEY', 'LB_CMD_TO_TYPE', 'LB_CMD_TO_VALUE',
            'LitterBox', 'LitterBoxCommand', 'LitterBoxCommandKey', 'LitterBoxCommandType', 'LitterBoxSetting', 'LITTER_LIST',
-           'LOGGER', 'Pet', 'PetKitClient', 'PetKitData', 'PetKitError', 'PetSetting', 'Region', 'TIMEOUT', 'StrEnum',
+           'LOGGER', 'Pet', 'PetKitClient', 'PetKitData', 'PetKitError', 'PetSetting', 'Region', 'ServerError', 'SERVER_ERROR_CODES', 'StrEnum', 'TIMEOUT',
            'WATER_FOUNTAIN_LIST', 'W5Command', 'W5_COMMAND_TO_CODE', 'W5_DND_COMMANDS', 'W5Fountain', 'W5_LIGHT_BRIGHTNESS',
            'W5_LIGHT_POWER', 'W5_MODE', 'W5_SETTINGS_COMMANDS',  ]
```

### Comparing `petkitaio-0.1.1/petkitaio/exceptions.py` & `petkitaio-0.1.2/petkitaio/exceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,8 +19,15 @@
         Exception.__init__(self, *args)
 
 class BluetoothError(Exception):
     """Bluetooth issue from PetKit api."""
 
     def __init__(self, *args: Any) -> None:
         """Initialize the exception."""
-        Exception.__init__(self, *args)
+        Exception.__init__(self, *args)
+
+class ServerError(Exception):
+    """PetKit server error."""
+
+    def __init__(self, *args: Any) -> None:
+        """Initialize the exception."""
+        Exception.__init__(self, *args)
```

### Comparing `petkitaio-0.1.1/petkitaio/model.py` & `petkitaio-0.1.2/petkitaio/model.py`

 * *Files identical despite different names*

### Comparing `petkitaio-0.1.1/petkitaio/petkit_client.py` & `petkitaio-0.1.2/petkitaio/petkit_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,40 +11,42 @@
 import urllib.parse as urlencode
 
 from aiohttp import ClientResponse, ClientSession
 import hashlib
 from tzlocal import get_localzone_name
 
 from petkitaio.constants import (
+    ASIA_REGIONS,
+    AUTH_ERROR_CODES,
     BLE_HEADER,
     BLUETOOTH_ERRORS,
     CLIENT_DICT,
     Endpoint,
-    ERROR_CODES,
     FEEDER_LIST,
     FeederSetting,
     Header,
     LB_CMD_TO_KEY,
     LB_CMD_TO_TYPE,
     LB_CMD_TO_VALUE,
     LitterBoxCommand,
     LitterBoxSetting,
     LITTER_LIST,
     PetSetting,
     Region,
+    SERVER_ERROR_CODES,
     TIMEOUT,
     WATER_FOUNTAIN_LIST,
     W5Command,
     W5_COMMAND_TO_CODE,
     W5_DND_COMMANDS,
     W5_LIGHT_BRIGHTNESS,
     W5_LIGHT_POWER,
     W5_SETTINGS_COMMANDS,
 )
-from petkitaio.exceptions import (AuthError, BluetoothError, PetKitError)
+from petkitaio.exceptions import (AuthError, BluetoothError, PetKitError, ServerError)
 from petkitaio.model import (Feeder, LitterBox, Pet, PetKitData, W5Fountain)
 
 LOGGER = logging.getLogger(__name__)
 
 
 class PetKitClient:
     """PetKit client."""
@@ -57,51 +59,86 @@
         username: PetKit username/email
         password: PetKit account password
         session: aiohttp.ClientSession or None to create a new session
         """
 
         self.username: str = username
         self.password: str = password
-        self.base_url: Region = Region.US
+        self.base_login: Region = Region.US
+        self.base_url: str | None = None
+        self.server_list: list | None = None
         self._session: ClientSession = session if session else ClientSession()
         self.tz: str = get_localzone_name()
         self.timeout: int = timeout
         self.token: str | None = None
         self.token_expiration: datetime | None = None
         self.user_id: str | None = None
         self.has_relay: bool = False
         self.ble_sequence: int = 0
         self.manually_paused: dict[int, bool] = {}
         self.manual_pause_end: dict[int, datetime | None] = {}
 
+    async def get_api_server_list(self) -> None:
+        """Fetches a list of all api urls categorized by region."""
+
+        url = 'https://passport.petkt.com/6/account/regionservers'
+
+        headers = {
+            'Accept': Header.ACCEPT,
+            'Accept-Language': Header.ACCEPT_LANG,
+            'Accept-Encoding': Header.ENCODING,
+            'X-Api-Version': Header.API_VERSION,
+            'Content-Type': Header.CONTENT_TYPE,
+            'User-Agent': Header.AGENT,
+            'X-Client': Header.CLIENT,
+        }
+        data = {}
+        response = await self._post(url, headers, data)
+        self.server_list = response['result']['list']
+
     async def login(self) -> None:
-        login_url = f'{self.base_url}{Endpoint.LOGIN}'
+
+        await self.get_api_server_list()
+        login_url = f'{self.base_login}{Endpoint.LOGIN}'
 
         headers = {
             'Accept': Header.ACCEPT,
-            'Accept-Language': Header.ACCEPTLANG,
+            'Accept-Language': Header.ACCEPT_LANG,
             'Accept-Encoding': Header.ENCODING,
-            'X-Api-Version': Header.APIVERSION,
-            'Content-Type': Header.CONTENTTYPE,
+            'X-Api-Version': Header.API_VERSION,
+            'Content-Type': Header.CONTENT_TYPE,
             'User-Agent': Header.AGENT,
             'X-Client': Header.CLIENT,
         }
 
         data = {
             'client': str(CLIENT_DICT),
             'encrypt': '1',
-            'oldVersion': Header.APIVERSION,
+            'oldVersion': Header.API_VERSION,
             'password': hashlib.md5(self.password.encode()).hexdigest(),
             'username': self.username
         }
 
         response = await self._post(login_url, headers, data)
         self.user_id = response['result']['session']['userId']
         self.token = response['result']['session']['id']
         self.token_expiration = datetime.now() + timedelta(seconds=response['result']['session']['expiresIn'])
+        account_region = response['result']['user']['account']['region']
+        # Determine base URL based on region account is from
+        for region in self.server_list:
+            if region['id'] == account_region:
+                # Need to remove trailing forward slash
+                self.base_url = region['gateway'][:-1]
+                break
+            else:
+                # Fallback base url if region server can't be found based on account region
+                if account_region in ASIA_REGIONS:
+                    self.base_url = Region.ASIA
+                else:
+                    self.base_url = Region.US
 
     async def check_token(self) -> None:
         """Check to see if there is a valid token or if token is about to expire.
         If there is no token, a new token is obtained. In addition,
         if the current token is about to expire within 60 minutes
         or has already expired, a new token is obtained.
         """
@@ -117,29 +154,29 @@
     async def create_header(self) -> dict[str, str]:
         """Create header for interaction with devices."""
 
         header = {
             'X-Session': self.token,
             'F-Session': self.token,
             'Accept': Header.ACCEPT,
-            'Accept-Language': Header.ACCEPTLANG,
+            'Accept-Language': Header.ACCEPT_LANG,
             'Accept-Encoding': Header.ENCODING,
-            'X-Api-Version': Header.APIVERSION,
-            'Content-Type': Header.CONTENTTYPE,
+            'X-Api-Version': Header.API_VERSION,
+            'Content-Type': Header.CONTENT_TYPE,
             'User-Agent': Header.AGENT,
             'X-Client': Header.CLIENT,
             'X-TimezoneId': self.tz,
         }
         return header
 
     async def get_device_roster(self) -> dict[str, Any]:
         """Fetch device roster endpoint to get all available devices."""
 
         await self.check_token()
-        url = f'{self.base_url}{Endpoint.DEVICEROSTER}'
+        url = f'{self.base_url}{Endpoint.DEVICE_ROSTER}'
         header = await self.create_header()
         data = {
             'day': str(datetime.now().date()).replace('-', ''),
         }
         device_roster = await self._post(url, header, data)
         return device_roster
 
@@ -172,15 +209,15 @@
                         'id': device['data']['id']
                     }
 
                     if self.has_relay:
                         ble_available: bool = False
                         main_online: bool = False
                         fountain_tcode = str(device['data']['typeCode'])
-                        ble_url = f'{self.base_url}{Endpoint.BLEDEVICES}'
+                        ble_url = f'{self.base_url}{Endpoint.BLE_DEVICES}'
                         relay_devices = await self._post(ble_url, header, data={})
                         if relay_devices['result']:
                             ble_available = True
                             for relay_device in relay_devices['result']:
                                 if relay_device['pim'] == 1:
                                     main_online = True
                                     break
@@ -188,27 +225,27 @@
                                     main_online = False
 
                             if ble_available and main_online:
                                 device_details = await self._post(wf_url, header, data)
                                 mac = device_details['result']['mac']
                                 type_code = int(f'1{fountain_tcode}')
                                 relay_tc = type_code
-                                conn_url = f'{self.base_url}{Endpoint.BLECONNECT}'
+                                conn_url = f'{self.base_url}{Endpoint.BLE_CONNECT}'
                                 ble_data = {
                                     'bleId': device_details['result']['id'],
                                     'mac': mac,
                                     'type': type_code
                                 }
                                 conn_resp = await self._post(conn_url, header, ble_data)
                                 # Check to see if BLE connection was successful
                                 if conn_resp['result']['state'] != 1:
                                     LOGGER.warning(f'BLE connection to {device_details["result"]["name"]} failed. Will try again during next refresh.')
                                     fountain_data = device_details
                                 else:
-                                    poll_url = f'{self.base_url}{Endpoint.BLEPOLL}'
+                                    poll_url = f'{self.base_url}{Endpoint.BLE_POLL}'
                                     poll_resp = await self._post(poll_url, header, ble_data)
                                     if poll_resp['result'] != 0:
                                         LOGGER.warning(
                                             f'BLE polling to {device_details["result"]["name"]} failed. Will try again during next refresh.')
                                         fountain_data = device_details
                                     else:
                                         # Wait a bit for BLE connection to be established before looking up most recent data
@@ -238,23 +275,23 @@
                         data=fountain_data['result'],
                         type=device_type,
                         ble_relay=relay_tc
                     )
                 # Feeders
                 if device['type'] in FEEDER_LIST:
                     sound_list: dict[int, str] = {}
-                    feeder_url = f'{self.base_url}/{device["type"].lower()}{Endpoint.DEVICEDETAIL}'
+                    feeder_url = f'{self.base_url}/{device["type"].lower()}{Endpoint.DEVICE_DETAIL}'
                     data = {
                         'id': device['data']['id']
                     }
                     feeder_data = await self._post(feeder_url, header, data)
 
                     if device['type'] == 'D3':
                         sound_list[-1] = 'Default'
-                        sound_url = f'{self.base_url}/{device["type"].lower()}{Endpoint.SOUNDLIST}'
+                        sound_url = f'{self.base_url}/{device["type"].lower()}{Endpoint.SOUND_LIST}'
                         sound_data = {
                             'deviceId': device['data']['id']
                         }
                         sound_response = await self._post(sound_url, header, sound_data)
                         result = sound_response['result']
                         for sound in result:
                             sound_list[sound['id']] = sound['name']
@@ -265,24 +302,28 @@
                         type=device['type'].lower(),
                         sound_list=sound_list
                     )
 
                 # Litter Boxes
                 if device['type'] in LITTER_LIST:
                     ### Fetch device_detail page
-                    dd_url = f'{self.base_url}/{device["type"].lower()}{Endpoint.DEVICEDETAIL}'
+                    dd_url = f'{self.base_url}/{device["type"].lower()}{Endpoint.DEVICE_DETAIL}'
                     dd_data = {
                         'id': device['data']['id']
                     }
                     device_detail = await self._post(dd_url, header, dd_data)
 
                     ### Fetch DeviceRecord page
-                    dr_url = f'{self.base_url}/{device["type"].lower()}{Endpoint.DEVICERECORD}'
+                    dr_url = f'{self.base_url}/{device["type"].lower()}{Endpoint.DEVICE_RECORD}'
+                    if device['type'] == 'T4':
+                        date_key = 'date'
+                    else:
+                        date_key = 'day'
                     dr_data = {
-                        'day': str(datetime.now().date()).replace('-', ''),
+                        date_key: str(datetime.now().date()).replace('-', ''),
                         'deviceId': device['data']['id']
                     }
                     device_record = await self._post(dr_url, header, dr_data)
 
                     ### Fetch statistic page
                     stat_url = f'{self.base_url}/{device["type"].lower()}{Endpoint.STATISTIC}'
                     stat_data = {
@@ -317,15 +358,15 @@
                         device_record=device_record['result'],
                         statistics=device_stats['result'],
                         type=device['type'].lower(),
                         manually_paused=manually_paused,
                         manual_pause_end=manual_pause_end,
                     )
         ### Get user details page
-        details_url = f'{self.base_url}{Endpoint.USERDETAILS}'
+        details_url = f'{self.base_url}{Endpoint.USER_DETAILS}'
         details_data = {
             'userId': self.user_id
         }
         user_details = await self._post(details_url, header, details_data)
         user_pets = user_details['result']['user']['dogs']
         if user_pets:
             for pet in user_pets:
@@ -354,42 +395,44 @@
             raise PetKitError(f'PetKit API error: {error}')
         try:
             response: dict[str, Any] = await resp.json()
         except Exception as error:
             raise PetKitError(f'Could not return json {error}') from error
         if 'error' in response:
             code = response['error']['code']
-            if code in ERROR_CODES:
-                raise AuthError(f'PetKit Error {code}: {ERROR_CODES[code]}')
+            if code in AUTH_ERROR_CODES:
+                raise AuthError(f'PetKit Error {code}: {AUTH_ERROR_CODES[code]}')
+            elif code in SERVER_ERROR_CODES:
+                raise ServerError(f'PetKit Error {code}: {SERVER_ERROR_CODES[code]}')
             elif code in BLUETOOTH_ERRORS:
                 raise BluetoothError(f'{BLUETOOTH_ERRORS[code]}')
             else:
                 raise PetKitError(f'PetKit Error {code}: {response["error"]["msg"]}')
         return response
 
 
 # <--------------------------------------- Methods for controlling devices --------------------------------------->
 
 
     async def initial_ble_commands(self, device: dict[str, Any], relay_type: int) -> None:
         """We have to make two calls to get updated date from the water fountain."""
-        command_url = f'{self.base_url}{Endpoint.CONTROLWF}'
+        command_url = f'{self.base_url}{Endpoint.CONTROL_WF}'
         header = await self.create_header()
-        data1 = await self.create_ble_data(W5Command.FIRSTBLECMND)
+        data1 = await self.create_ble_data(W5Command.FIRST_BLE_CMND)
         first_command = {
             'bleId': device['result']['id'],
             'cmd': '215',
             'data': data1,
             'mac': device['result']['mac'],
             'type': relay_type
         }
         await self._post(command_url, header, first_command)
         self.ble_sequence += 1
 
-        data2 = await self.create_ble_data(W5Command.SECONDBLECMND)
+        data2 = await self.create_ble_data(W5Command.SECOND_BLE_CMND)
         second_command = {
             'bleId': device['result']['id'],
             'cmd': '216',
             'data': data2,
             'mac': device['result']['mac'],
             'type': relay_type
         }
@@ -397,57 +440,57 @@
         self.ble_sequence += 1
 
 
     async def create_ble_data(self, command: W5Command, device: W5Fountain | None = None) -> str:
         """Create URL encoded data from specific byte array."""
 
         byte_list: list = []
-        if command == W5Command.FIRSTBLECMND:
+        if command == W5Command.FIRST_BLE_CMND:
             byte_list = [-6, -4, -3, -41, 1, self.ble_sequence, 0, 0, -5]
-        if command == W5Command.SECONDBLECMND:
+        if command == W5Command.SECOND_BLE_CMND:
             byte_list = [-6, -4, -3, -40, 1, self.ble_sequence, 0, 0, -5]
-        if command == W5Command.NORMALTOPAUSE:
+        if command == W5Command.NORMAL_TO_PAUSE:
             byte_list = [-6, -4, -3, -36, 1, self.ble_sequence, 2, 0, 0, 1, -5]
-        if command == W5Command.SMARTTOPAUSE:
+        if command == W5Command.SMART_TO_PAUSE:
             byte_list = [-6, -4, -3, -36, 1, self.ble_sequence, 2, 0, 0, 2, -5]
         if command == W5Command.NORMAL:
             byte_list = [-6, -4, -3, -36, 1, self.ble_sequence, 2, 0, 1, 1, -5]
         if command == W5Command.SMART:
             byte_list = [-6, -4, -3, -36, 1, self.ble_sequence, 2, 0, 1, 2, -5]
 
-        if command == W5Command.LIGHTOFF:
+        if command == W5Command.LIGHT_OFF:
             # byte_list example = [-6, -4, -3, -35, 1, self.ble_sequence, 13, 0, 3, 3, 0, light_brightness, 0, 0, 0, 0, 0, 5, 40, 1, 104, -5]
             data_list = await self.w5_command_data_creator(device=device, command=command, setting=[0])
             byte_list = await self.create_ble_byte_list(command=-35, data_list=data_list)
 
-        if command == W5Command.LIGHTON:
+        if command == W5Command.LIGHT_ON:
             data_list = await self.w5_command_data_creator(device=device, command=command, setting=[1])
             byte_list = await self.create_ble_byte_list(command=-35, data_list=data_list)
 
-        if command == W5Command.LIGHTLOW:
+        if command == W5Command.LIGHT_LOW:
             data_list = await self.w5_command_data_creator(device=device, command=command, setting=[1])
             byte_list = await self.create_ble_byte_list(command=-35, data_list=data_list)
 
-        if command == W5Command.LIGHTMEDIUM:
+        if command == W5Command.LIGHT_MEDIUM:
             data_list = await self.w5_command_data_creator(device=device, command=command, setting=[2])
             byte_list = await self.create_ble_byte_list(command=-35, data_list=data_list)
 
-        if command == W5Command.LIGHTHIGH:
+        if command == W5Command.LIGHT_HIGH:
             data_list = await self.w5_command_data_creator(device=device, command=command, setting=[3])
             byte_list = await self.create_ble_byte_list(command=-35, data_list=data_list)
 
-        if command == W5Command.DONOTDISTURB:
+        if command == W5Command.DO_NOT_DISTURB:
             data_list = await self.w5_command_data_creator(device=device, command=command, setting=[1])
             byte_list = await self.create_ble_byte_list(command=-35, data_list=data_list)
 
-        if command == W5Command.DONOTDISTURBOFF:
+        if command == W5Command.DO_NOT_DISTURB_OFF:
             data_list = await self.w5_command_data_creator(device=device, command=command, setting=[0])
             byte_list = await self.create_ble_byte_list(command=-35, data_list=data_list)
 
-        if command == W5Command.RESETFILTER:
+        if command == W5Command.RESET_FILTER:
             byte_list = [-6, -4, -3, -34, 1, self.ble_sequence, 0, 0, -5]
 
         byte_array = bytearray([x % 256 for x in byte_list])
         b64_encoded = base64.b64encode(byte_array)
         url_encoded = urlencode.quote(b64_encoded, 'utf-8')
         return url_encoded
 
@@ -529,15 +572,15 @@
             byte_list.append(((input >> (16 - (i2 * 8))) & 255))
             i = i2
         return byte_list
 
     async def get_litter_box_record(self, id: int, type: str, header: dict[str, Any]) -> dict[str, Any]:
         """Fetch the litter box getDeviceRecord endpoint."""
 
-        url = f'{self.base_url}/{type}{Endpoint.DEVICERECORD}'
+        url = f'{self.base_url}/{type}{Endpoint.DEVICE_RECORD}'
         data = {
             'day': str(datetime.now().date()).replace('-', ''),
             'deviceId': id
         }
         response = await self._post(url, header, data)
         return response
 
@@ -548,17 +591,17 @@
         else:
             # Pause command sent depends on initial mode
             if command == W5Command.PAUSE:
                 if water_fountain.data['powerStatus'] == 0:
                     raise PetKitError(f'{water_fountain.data["name"]} is already paused.')
                 else:
                     if water_fountain.data['mode'] == 1:
-                        ble_data = await self.create_ble_data(W5Command.NORMALTOPAUSE, water_fountain)
+                        ble_data = await self.create_ble_data(W5Command.NORMAL_TO_PAUSE, water_fountain)
                     else:
-                        ble_data = await self.create_ble_data(W5Command.SMARTTOPAUSE, water_fountain)
+                        ble_data = await self.create_ble_data(W5Command.SMART_TO_PAUSE, water_fountain)
 
             # make sure light is on if brightness is being set
             elif command in W5_LIGHT_BRIGHTNESS:
                 if water_fountain.data['settings']['lampRingSwitch'] != 1:
                     raise PetKitError(f'{water_fountain.data["name"]} indicator light is Off. You can only change light brightness when the indicator light is On.')
                 else:
                     ble_data = await self.create_ble_data(command, water_fountain)
@@ -569,17 +612,17 @@
                 ble_data = await self.create_ble_data(command, water_fountain)
             header = await self.create_header()
             conn_data = {
                 'bleId': water_fountain.data['id'],
                 'mac': water_fountain.data['mac'],
                 'type': water_fountain.ble_relay
             }
-            connect_url = f'{self.base_url}{Endpoint.BLECONNECT}'
-            poll_url = f'{self.base_url}{Endpoint.BLEPOLL}'
-            command_url = f'{self.base_url}{Endpoint.CONTROLWF}'
+            connect_url = f'{self.base_url}{Endpoint.BLE_CONNECT}'
+            poll_url = f'{self.base_url}{Endpoint.BLE_POLL}'
+            command_url = f'{self.base_url}{Endpoint.CONTROL_WF}'
             cmnd_code = W5_COMMAND_TO_CODE[command]
 
             command_data = {
                 'bleId': water_fountain.data['id'],
                 'cmd': cmnd_code,
                 'data': ble_data,
                 'mac': water_fountain.data['mac'],
@@ -594,32 +637,52 @@
             send_command = await self._post(command_url, header, command_data)
             # Reset ble_sequence
             self.ble_sequence = 0
 
     async def call_pet(self, feeder: Feeder) -> None:
         """Call pet on D3 (Infinity) feeder."""
 
-        url = f'{self.base_url}/{feeder.type}{Endpoint.CALLPET}'
+        url = f'{self.base_url}/{feeder.type}{Endpoint.CALL_PET}'
         header = await self.create_header()
         data = {
             'deviceId': feeder.id
         }
         await self._post(url, header, data)
 
     async def control_litter_box(self, litter_box: LitterBox, command: LitterBoxCommand) -> None:
         """Control PetKit litter boxes."""
 
-        url = f'{self.base_url}/{litter_box.type}{Endpoint.CONTROLDEVICE}'
+        url = f'{self.base_url}/{litter_box.type}{Endpoint.CONTROL_DEVICE}'
         value: int = 0
+
+        if litter_box.type == 't4':
+            if command == LitterBoxCommand.START_CLEAN:
+                # If the litter box is currently paused then send a resume cleaning command.
+                # Otherwise, you can't start a manual clean while it is in an unsupported mode.
+                if 'workState' in litter_box.device_detail['state']:
+                    state =  litter_box.device_detail['state']['workState']
+                    # This workState is equivalent to a paused manual cleaning
+                    if (state['workMode'] == 0) and (state['workProcess'] == 20):
+                        command = LitterBoxCommand.RESUME_CLEAN
+                        self.manually_paused[litter_box.id] = False
+                        self.manual_pause_end[litter_box.id] = None
+                    else:
+                        raise PetKitError('Unable to call start cleaning command while litter box is in operation.')
+            if command == LitterBoxCommand.PAUSE_CLEAN:
+                self.manually_paused[litter_box.id] = True
+                ## The manual pause will end after a 10-minute wait + 1 minute to complete cleaning
+                self.manual_pause_end[litter_box.id] = datetime.now() + timedelta(seconds=660)
+
         if command == LitterBoxCommand.POWER:
             #If litter box is currently turned on then you want the command to turn it off
             if litter_box.device_detail['state']['power'] == 1:
                 value = 0
             else:
                 value = 1
+        # For all non-power commands, get the value associated with the command
         else:
             value = LB_CMD_TO_VALUE[command]
 
         key = LB_CMD_TO_KEY[command]
         header = await self.create_header()
 
         command_dict = {
@@ -628,33 +691,35 @@
         data = {
             'id': litter_box.id,
             'kv': json.dumps(command_dict),
             'type': LB_CMD_TO_TYPE[command]
         }
         await self._post(url, header, data)
 
-        ### If the current session was ended while the device was paused, the new session wouldn't know the manual pause is active.
-        ### Only way of resuming cleaning is to send the STARTCLEAN command followed by a RESUMECLEAN command.
+        ### For Pura X, if the current session was ended while the device was paused, the new session wouldn't know the manual pause is active.
+        ### Only way of resuming cleaning is to send the START_CLEAN command followed by a RESUME_CLEAN command.
         ### In addition, the resume command doesn't work by itself - start followed by resume is always needed if currently paused.
         ### Check if the device is currently paused - if so, the resume command needs to be sent after start clean.
-        if command == LitterBoxCommand.STARTCLEAN:
-            await asyncio.sleep(1)
-            record = await self.get_litter_box_record(litter_box.id, litter_box.type, header)
-            if record['result']:
-                last_item = record['result'][-1]
-                if last_item['enumEventType'] == 'clean_over':
-                    if (last_item['content']['startReason'] in [0, 1, 2, 3]) and (last_item['content']['result'] == 3):
-                        await self.control_litter_box(litter_box, LitterBoxCommand.RESUMECLEAN)
-                        self.manually_paused[litter_box.id] = False
-                        self.manual_pause_end[litter_box.id] = None
-
-        if command == LitterBoxCommand.PAUSECLEAN:
-            self.manually_paused[litter_box.id] = True
-            ## The manual pause will end after a 10-minute wait + 1 minute to complete cleaning
-            self.manual_pause_end[litter_box.id] = datetime.now() + timedelta(seconds=660)
+        ### Unlike the Pura Max, we need to send the START clean command before getting the litter box record due to the Pura X not returning its current workState.
+        if litter_box.type == 't3':
+            if command == LitterBoxCommand.START_CLEAN:
+                await asyncio.sleep(1)
+                record = await self.get_litter_box_record(litter_box.id, litter_box.type, header)
+                if record['result']:
+                    last_item = record['result'][-1]
+                    if last_item['enumEventType'] == 'clean_over':
+                        if (last_item['content']['startReason'] in [0, 1, 2, 3]) and (last_item['content']['result'] == 3):
+                            await self.control_litter_box(litter_box, LitterBoxCommand.RESUME_CLEAN)
+                            self.manually_paused[litter_box.id] = False
+                            self.manual_pause_end[litter_box.id] = None
+
+            if command == LitterBoxCommand.PAUSE_CLEAN:
+                self.manually_paused[litter_box.id] = True
+                ## The manual pause will end after a 10-minute wait + 1 minute to complete cleaning
+                self.manual_pause_end[litter_box.id] = datetime.now() + timedelta(seconds=660)
 
     async def check_manual_pause_expiration(self, id: int):
         """Check to see if manual pause has expired and litter box resumed the cleanin on its own."""
 
         current_dt = datetime.now()
         current_end = self.manual_pause_end[id]
         if (current_end - current_dt).total_seconds() <= 0:
@@ -664,88 +729,100 @@
     async def manual_feeding(self, feeder: Feeder, amount: int) -> None:
         """Dispense food manually.
         Mini Feeder allowed amount (in grams) is 5, 10, 15, 20, 25, 30, 35, 40, 45, 50.
         D4 (Element Solo) allowed amount is 10, 20, 30, 40, 50.
         """
 
         if feeder.type == 'feedermini':
-            url = f'{self.base_url}{Endpoint.MINIMANUALFEED}'
+            url = f'{self.base_url}{Endpoint.MINI_MANUAL_FEED}'
         else:
-            url = f'{self.base_url}/{feeder.type}{Endpoint.MANUALFEED}'
+            url = f'{self.base_url}/{feeder.type}{Endpoint.MANUAL_FEED}'
         header = await self.create_header()
         data = {
             'amount': amount,
             'day': str(datetime.now().date()).replace('-', ''),
             'deviceId': feeder.id,
             'time': '-1'
         }
         await self._post(url, header, data)
 
     async def update_feeder_settings(self, feeder: Feeder, setting: FeederSetting, value: int) -> None:
         """Change the setting on a feeder."""
 
         if feeder.type == 'feedermini':
-            url = f'{self.base_url}{Endpoint.MINISETTING}'
+            url = f'{self.base_url}{Endpoint.MINI_SETTING}'
         # D3 and D4 Feeders
         else:
-            url = f'{self.base_url}/{feeder.type}{Endpoint.UPDATESETTING}'
+            url = f'{self.base_url}/{feeder.type}{Endpoint.UPDATE_SETTING}'
         header = await self.create_header()
         setting_dict = {
             setting: value
         }
         data = {
             'id': feeder.id,
             'kv': json.dumps(setting_dict)
         }
         await self._post(url, header, data)
 
     async def update_litter_box_settings(self, litter_box: LitterBox, setting: LitterBoxSetting | None = None, value: int | None = None) -> None:
         """Change the setting on a litter box."""
 
-        url = f'{self.base_url}/{litter_box.type}{Endpoint.UPDATESETTING}'
+        url = f'{self.base_url}/{litter_box.type}{Endpoint.UPDATE_SETTING}'
         header = await self.create_header()
         setting_dict = {
             setting: value
         }
         data = {
             'id': litter_box.id,
             'kv': json.dumps(setting_dict)
         }
         await self._post(url, header, data)
 
     async def update_pet_settings(self, pet: Pet, setting: PetSetting, value: int | float) -> None:
         """Change the setting for a pet."""
 
-        url = f'{self.base_url}{Endpoint.PETPROPS}'
+        url = f'{self.base_url}{Endpoint.PET_PROPS}'
         header = await self.create_header()
         setting_dict = {
             setting: value
         }
         data = {
             'petId': int(pet.id),
             'kv': json.dumps(setting_dict)
         }
         await self._post(url, header, data)
 
     async def cancel_manual_feed(self, feeder: Feeder) -> None:
         """Cancel a manual feed that is currently in progress. Not available for mini feeders"""
 
-        url = f'{self.base_url}/{feeder.type}{Endpoint.CANCELFEED}'
+        url = f'{self.base_url}/{feeder.type}{Endpoint.CANCEL_FEED}'
         header = await self.create_header()
         data = {
             'day': str(datetime.now().date()).replace('-', ''),
             'deviceId': feeder.id
         }
         await self._post(url, header, data)
 
     async def reset_feeder_desiccant(self, feeder: Feeder) -> None:
         """Reset the desiccant of a single feeder."""
 
         if feeder.type == 'feedermini':
-            url = f'{self.base_url}{Endpoint.MINIDESICCANTRESET}'
+            url = f'{self.base_url}{Endpoint.MINI_DESICCANT_RESET}'
         else:
-            url = f'{self.base_url}/{feeder.type}{Endpoint.FEEDERDESICCANTRESET}'
+            url = f'{self.base_url}/{feeder.type}{Endpoint.FEEDER_DESICCANT_RESET}'
         header = await self.create_header()
         data = {
             'deviceId': feeder.id
         }
         await self._post(url, header, data)
+
+    async def reset_pura_max_deodorizer(self, litter_box: LitterBox) -> None:
+        """Reset the N50 odor eliminator for Pura Max."""
+
+        if litter_box.type != 't4':
+            raise PetKitError('Invalid litter box type. Only Pura Max litter boxes have N50 odor eliminators.')
+        url = f'{self.base_url}/{litter_box.type}{Endpoint.MAX_ODOR_RESET}'
+        header = await self.create_header()
+        data = {
+            'deviceId': litter_box.id
+        }
+        await self._post(url, header, data)
```

### Comparing `petkitaio-0.1.1/petkitaio/str_enum.py` & `petkitaio-0.1.2/petkitaio/str_enum.py`

 * *Files identical despite different names*

### Comparing `petkitaio-0.1.1/petkitaio.egg-info/PKG-INFO` & `petkitaio-0.1.2/petkitaio.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: petkitaio
-Version: 0.1.1
+Version: 0.1.2
 Summary: Asynchronous Python library for PetKit's API
 Home-page: https://github.com/RobertD502/petkitaio
 Author: Robert Drinovac
 Author-email: unlisted@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/RobertD502/petkitaio/issues
 Project-URL: Source, https://github.com/RobertD502/petkitaio/
 Description: # PetKitAIO
         
         Asynchronous Python library for PetKit's API.
         
-        This is PetKit's undocumented API. With that said, future changes made by PetKit may break this library. All API calls are made to PetKit's USA servers.
+        This is PetKit's undocumented API. With that said, future changes made by PetKit may break this library. The API endpoint used is determined based on the region your account is locked to. Although support has been added for the PetKit Asia API endpoint, I have not personally tested it.
         
         ## **Currently Supported Devices**:
         - [D3 Feeder (Fresh Element Infinity)](https://www.amazon.com/PETKIT-Automatic-Stainless-Programmable-Dispenser/dp/B09JFK8BCQ)
         - [D4 Feeder (Fresh Element Solo)](https://www.amazon.com/PETKIT-Automatic-Dispenser-Compatible-Freeze-Dried/dp/B09158J9PF/)
         - [Mini Feeder](https://www.amazon.com/PETKIT-Automatic-Stainless-Indicator-Dispenser-2-8L/dp/B08GS1CPHH/)
         - [W5 Water Fountain (Eversweet 3 Pro)](https://www.amazon.com/PETKIT-Wireless-Fountain-Stainless-Dispenser/dp/B09QRH6L3M/)
         - [T3 Litter Box (Pura X)](https://www.amazon.com/PETKIT-Self-Cleaning-Scooping-Automatic-Multiple/dp/B08T9CCP1M)
+        - [T4 Litter Box (Pura MAX) with/without Pura Air](https://www.amazon.com/PETKIT-Self-Cleaning-Capacity-Multiple-Automatic/dp/B09KC7Q4YF)
         
         ## Important
         
         PetKit accounts can only be logged in on one device at a time. Using this library will result in getting signed out of the mobile app. You can avoid this by creating a secondary account and sharing devices from the main account (except water fountains). However, some device functionality is lost when using a secondary account as well as not being able to share pets between accounts.
         
         
         This package depends on [aiohttp](https://docs.aiohttp.org/en/stable/) and [tzlocal](https://pypi.org/project/tzlocal/). `Python 3.7` or greater is required.
@@ -78,15 +79,15 @@
         # See constants.py FeederSetting class for available settings
         # Additional import needed:
         from petkitaio.constants import FeederSetting
         
         
         # Enabling child lock on a D4 feeder. Note: Mini Feeders use a different setting.
         # Reusing retrieved devices from above.
-        await client.update_feeder_settings(feeder=devices.feeders[feederid], setting=FeederSetting.CHILDLOCK, value=1)
+        await client.update_feeder_settings(feeder=devices.feeders[feederid], setting=FeederSetting.CHILD_LOCK, value=1)
         ```
         
         ### Reset Feeder Desiccant
         ```python
         # Reusing retrieved devices from above.
         await client.reset_feeder_desiccant(feeder=devices.feeders[feederid])
         ```
@@ -98,14 +99,14 @@
         # Additional import needed:
         from petkitaio.constants import W5Command
         
         # Set Water Fountain to Smart Mode. Reusing retrieved devices from above.
         await client.control_water_fountain(water_fountain=devices.water_fountains[water_fountain_id], command=W5Command.SMART)
         ```
         
-Keywords: petkit,eversweet 3 pro,feeder mini,d4,petkit feeder,petkit water fountain,freshelement solo
+Keywords: petkit,eversweet 3 pro,feeder mini,d4,petkit feeder,petkit water fountain,freshelement solo,pura x,pura max,pura air
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `petkitaio-0.1.1/setup.py` & `petkitaio-0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="petkitaio",
-    version="0.1.1",
+    version="0.1.2",
     author="Robert Drinovac",
     author_email="unlisted@gmail.com",
     description="Asynchronous Python library for PetKit's API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/RobertD502/petkitaio',
-    keywords='petkit, eversweet 3 pro, feeder mini, d4, petkit feeder, petkit water fountain, freshelement solo',
+    keywords='petkit, eversweet 3 pro, feeder mini, d4, petkit feeder, petkit water fountain, freshelement solo, pura x, pura max, pura air',
     packages=setuptools.find_packages(),
     python_requires= ">=3.7",
     install_requires=[
         "aiohttp>=3.8.1",
         "tzlocal>=4.2",
     ],
-    classifiers=(
+    classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent"
-    ),
+    ],
     project_urls={  # Optional
     'Bug Reports': 'https://github.com/RobertD502/petkitaio/issues',
     'Source': 'https://github.com/RobertD502/petkitaio/',
     },
 )
```

