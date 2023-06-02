# Comparing `tmp/pymexc-1.0.2.tar.gz` & `tmp/pymexc-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pymexc-1.0.2.tar", last modified: Tue May 30 18:45:17 2023, max compression
+gzip compressed data, was "dist\pymexc-1.0.3.tar", last modified: Fri Jun  2 19:58:41 2023, max compression
```

## Comparing `pymexc-1.0.2.tar` & `pymexc-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 18:45:17.558055 pymexc-1.0.2/
--rw-rw-rw-   0        0        0     1088 2022-10-20 18:54:22.000000 pymexc-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     3321 2023-05-30 18:45:17.559055 pymexc-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2221 2023-05-30 13:04:58.000000 pymexc-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 18:45:17.543052 pymexc-1.0.2/pymexc/
--rw-rw-rw-   0        0        0     1431 2023-05-30 13:22:30.000000 pymexc-1.0.2/pymexc/__init__.py
--rw-rw-rw-   0        0        0     5684 2023-05-30 13:09:13.000000 pymexc-1.0.2/pymexc/base.py
--rw-rw-rw-   0        0        0    17551 2023-05-30 18:42:16.000000 pymexc-1.0.2/pymexc/base_websocket.py
--rw-rw-rw-   0        0        0    67093 2023-05-30 18:41:16.000000 pymexc-1.0.2/pymexc/futures.py
--rw-rw-rw-   0        0        0    67652 2023-05-30 18:31:58.000000 pymexc-1.0.2/pymexc/spot.py
-drwxrwxrwx   0        0        0        0 2023-05-30 18:45:17.557055 pymexc-1.0.2/pymexc.egg-info/
--rw-rw-rw-   0        0        0     3321 2023-05-30 18:45:17.000000 pymexc-1.0.2/pymexc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-05-30 18:45:17.000000 pymexc-1.0.2/pymexc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 18:45:17.000000 pymexc-1.0.2/pymexc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-30 18:45:17.000000 pymexc-1.0.2/pymexc.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       26 2023-05-30 18:45:17.000000 pymexc-1.0.2/pymexc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-30 18:45:17.000000 pymexc-1.0.2/pymexc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 18:45:17.560055 pymexc-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1697 2023-05-30 18:44:25.000000 pymexc-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:58:41.467867 pymexc-1.0.3/
+-rw-rw-rw-   0        0        0     1088 2022-10-20 18:54:22.000000 pymexc-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     3321 2023-06-02 19:58:41.467867 pymexc-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2221 2023-05-30 13:04:58.000000 pymexc-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 19:58:41.442859 pymexc-1.0.3/pymexc/
+-rw-rw-rw-   0        0        0     1431 2023-05-30 13:22:30.000000 pymexc-1.0.3/pymexc/__init__.py
+-rw-rw-rw-   0        0        0     5824 2023-06-02 19:49:27.000000 pymexc-1.0.3/pymexc/base.py
+-rw-rw-rw-   0        0        0    18102 2023-06-02 19:53:45.000000 pymexc-1.0.3/pymexc/base_websocket.py
+-rw-rw-rw-   0        0        0    67666 2023-06-02 19:56:06.000000 pymexc-1.0.3/pymexc/futures.py
+-rw-rw-rw-   0        0        0    68220 2023-06-02 19:56:58.000000 pymexc-1.0.3/pymexc/spot.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:58:41.466872 pymexc-1.0.3/pymexc.egg-info/
+-rw-rw-rw-   0        0        0     3321 2023-06-02 19:58:41.000000 pymexc-1.0.3/pymexc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-06-02 19:58:41.000000 pymexc-1.0.3/pymexc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 19:58:41.000000 pymexc-1.0.3/pymexc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-02 19:58:41.000000 pymexc-1.0.3/pymexc.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       26 2023-06-02 19:58:41.000000 pymexc-1.0.3/pymexc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-02 19:58:41.000000 pymexc-1.0.3/pymexc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 19:58:41.473868 pymexc-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1697 2023-05-30 18:54:32.000000 pymexc-1.0.3/setup.py
```

### Comparing `pymexc-1.0.2/LICENSE` & `pymexc-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pymexc-1.0.2/PKG-INFO` & `pymexc-1.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pymexc
-Version: 1.0.2
+Version: 1.0.3
 Summary: Unofficial python library for interacting with the MEXC crypto exchange
 Home-page: https://github.com/makarworld/pymexc.git
-Download-URL: https://github.com/makarworld/pymexc/archive/refs/tags/v1.0.2.zip
+Download-URL: https://github.com/makarworld/pymexc/archive/refs/tags/v1.0.3.zip
 Author: abuztrade
 Author-email: abuztrade.work@gmail.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Communications :: Email
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymexc-1.0.2/README.md` & `pymexc-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pymexc-1.0.2/pymexc/__init__.py` & `pymexc-1.0.3/pymexc/__init__.py`

 * *Files identical despite different names*

### Comparing `pymexc-1.0.2/pymexc/base.py` & `pymexc-1.0.3/pymexc/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,38 +11,41 @@
     """
     Initializes a new instance of the class with the given `api_key` and `api_secret` parameters.
 
     :param api_key: A string representing the API key.
     :param api_secret: A string representing the API secret.
     :param base_url: A string representing the base URL of the API.
     """
-    def __init__(self, api_key: str, api_secret: str, base_url: str):
+    def __init__(self, api_key: str, api_secret: str, base_url: str, proxies: dict = None):
         self.api_key = api_key
         self.api_secret = api_secret
 
         self.recvWindow = 5000
 
         self.base_url = base_url
 
         self.session = requests.Session()
         self.session.headers.update({
-            "Content-Type": "application/json"
+            "Content-Type": "application/json",
         })
 
+        if proxies:
+            self.session.proxies.update(proxies)
+
 
     @abstractclassmethod
     def sign(self, **kwargs) -> str:
         ...
     
     @abstractclassmethod
     def call(self, method: Union[Literal["GET"], Literal["POST"], Literal["PUT"], Literal["DELETE"]], router: str, *args, **kwargs) -> dict:
         ...
 
 class _SpotHTTP(MexcSDK):
-    def __init__(self, api_key: str = None, api_secret: str = None):
+    def __init__(self, api_key: str = None, api_secret: str = None, proxies: dict = None):
         super().__init__(api_key, api_secret, "https://api.mexc.com")
 
         self.session.headers.update({
             "X-MEXC-APIKEY": self.api_key
         })
 
     def sign(self, **kwargs) -> str:
@@ -78,15 +81,15 @@
                 kwargs['params']['signature']  = self.sign(**kwargs['params'])
 
         response = self.session.request(method, f"{self.base_url}{router}", *args, **kwargs)
 
         return response.json()
     
 class _FuturesHTTP(MexcSDK):
-    def __init__(self, api_key: str = None, api_secret: str = None):
+    def __init__(self, api_key: str = None, api_secret: str = None, proxies: dict = None):
         super().__init__(api_key, api_secret, "https://contract.mexc.com")
 
     def sign(self, timestamp: str, **kwargs) -> str:
         """
         Generates a signature for an API request using HMAC SHA256 encryption.
 
         :param timestamp: A string representing the timestamp of the request.
```

### Comparing `pymexc-1.0.2/pymexc/base_websocket.py` & `pymexc-1.0.3/pymexc/base_websocket.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,28 @@
 
 SPOT = "wss://wbs.mexc.com/ws"
 FUTURES = "wss://contract.mexc.com/ws"
 
 class _WebSocketManager:
     def __init__(self, callback_function, ws_name, api_key=None, api_secret=None,
                  ping_interval=20, ping_timeout=10, retries=10,
-                 restart_on_error=True, trace_logging=False):
+                 restart_on_error=True, trace_logging=False, 
+                 http_proxy_host = None,
+                 http_proxy_port = None,
+                 http_no_proxy = None,
+                 http_proxy_auth = None,
+                 http_proxy_timeout = None):
+        
+        self.proxy_settings = dict(
+            http_proxy_host = http_proxy_host,
+            http_proxy_port = http_proxy_port,
+            http_no_proxy = http_no_proxy,
+            http_proxy_auth = http_proxy_auth,
+            http_proxy_timeout = http_proxy_timeout
+        )
 
         # Set API keys.
         self.api_key = api_key
         self.api_secret = api_secret
 
         self.callback = callback_function
         self.ws_name = ws_name
@@ -122,15 +135,16 @@
                 on_open=self._on_open(),
                 on_error=lambda ws, err: self._on_error(err)
             )
 
             # Setup the thread running WebSocketApp.
             self.wst = threading.Thread(target=lambda: self.ws.run_forever(
                 ping_interval=self.ping_interval,
-                ping_timeout=self.ping_timeout
+                ping_timeout=self.ping_timeout,
+                **self.proxy_settings
             ))
 
             # Configure as daemon; start.
             self.wst.daemon = True
             self.wst.start()
 
             # setup ping loop
```

### Comparing `pymexc-1.0.2/pymexc/futures.py` & `pymexc-1.0.3/pymexc/futures.py`

 * *Files 2% similar despite different names*

```diff
@@ -1382,30 +1382,40 @@
                                     stopPlanOrderId = stop_plan_order_id,
                                     stopLossPrice = stop_loss_price,
                                     takeProfitPrice = take_profit_price
                             ))
 
 class WebSocket(_FuturesWebSocket):
     def __init__(self, 
-                 api_key:          Optional[str]  = None, 
-                 api_secret:       Optional[str]  = None,
-                 ping_interval:    Optional[int]  = 20, 
-                 ping_timeout:     Optional[int]  = 10, 
-                 retries:          Optional[int]  = 10,
-                 restart_on_error: Optional[bool] = True, 
-                 trace_logging:    Optional[bool] = False):
+                 api_key:            Optional[str]   = None, 
+                 api_secret:         Optional[str]   = None,
+                 ping_interval:      Optional[int]   = 20, 
+                 ping_timeout:       Optional[int]   = 10, 
+                 retries:            Optional[int]   = 10,
+                 restart_on_error:   Optional[bool]  = True, 
+                 trace_logging:      Optional[bool]  = False,
+                 http_proxy_host:    Optional[str]   = None,
+                 http_proxy_port:    Optional[int]   = None,
+                 http_no_proxy:      Optional[list]  = None,
+                 http_proxy_auth:    Optional[tuple] = None,
+                 http_proxy_timeout: Optional[int]   = None):
 
         kwargs = dict(
             api_key = api_key,
             api_secret = api_secret,
             ping_interval = ping_interval,
             ping_timeout = ping_timeout,
             retries = retries,
             restart_on_error = restart_on_error,
-            trace_logging = trace_logging
+            trace_logging = trace_logging,
+            http_proxy_host = http_proxy_host,
+            http_proxy_port = http_proxy_port,
+            http_no_proxy = http_no_proxy,
+            http_proxy_auth = http_proxy_auth,
+            http_proxy_timeout = http_proxy_timeout
         )
         
         super().__init__(**kwargs)
         
 
     def tickers_stream(self, callback: Callable[..., None]):
         """
```

### Comparing `pymexc-1.0.2/pymexc/spot.py` & `pymexc-1.0.3/pymexc/spot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1575,22 +1575,27 @@
         :return: response dictionary
         :rtype: dict
         """
         return self.call("GET", "api/v3/rebate/referCode", params=dict(please_sign_me = None))
 
 class WebSocket(_SpotWebSocket):
     def __init__(self, 
-                 api_key:          Optional[str]  = None, 
-                 api_secret:       Optional[str]  = None,
-                 listenKey:        Optional[str]  = None,
-                 ping_interval:    Optional[int]  = 20, 
-                 ping_timeout:     Optional[int]  = 10, 
-                 retries:          Optional[int]  = 10,
-                 restart_on_error: Optional[bool] = True, 
-                 trace_logging:    Optional[bool] = False):
+                 api_key:            Optional[str]  = None, 
+                 api_secret:         Optional[str]  = None,
+                 listenKey:          Optional[str]  = None,
+                 ping_interval:      Optional[int]  = 20, 
+                 ping_timeout:       Optional[int]  = 10, 
+                 retries:            Optional[int]  = 10,
+                 restart_on_error:   Optional[bool] = True, 
+                 trace_logging:      Optional[bool] = False,
+                 http_proxy_host:    Optional[str]   = None,
+                 http_proxy_port:    Optional[int]   = None,
+                 http_no_proxy:      Optional[list]  = None,
+                 http_proxy_auth:    Optional[tuple] = None,
+                 http_proxy_timeout: Optional[int]   = None):
         """
         Initializes the class instance with the provided arguments.
 
         :param api_key: API key for authentication. (Optional)
         :type api_key: str
 
         :param api_secret: API secret for authentication. (Optional)
@@ -1618,15 +1623,20 @@
         kwargs = dict(
             api_key = api_key,
             api_secret = api_secret,
             ping_interval = ping_interval,
             ping_timeout = ping_timeout,
             retries = retries,
             restart_on_error = restart_on_error,
-            trace_logging = trace_logging
+            trace_logging = trace_logging,
+            http_proxy_host = http_proxy_host,
+            http_proxy_port = http_proxy_port,
+            http_no_proxy = http_no_proxy,
+            http_proxy_auth = http_proxy_auth,
+            http_proxy_timeout = http_proxy_timeout
         )
 
         self.listenKey = listenKey
 
         # for keep alive connection to private spot websocket
         # need to send listen key at connection and send keep-alive request every 60 mins
         if api_key and api_secret:
```

### Comparing `pymexc-1.0.2/pymexc.egg-info/PKG-INFO` & `pymexc-1.0.3/pymexc.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pymexc
-Version: 1.0.2
+Version: 1.0.3
 Summary: Unofficial python library for interacting with the MEXC crypto exchange
 Home-page: https://github.com/makarworld/pymexc.git
-Download-URL: https://github.com/makarworld/pymexc/archive/refs/tags/v1.0.2.zip
+Download-URL: https://github.com/makarworld/pymexc/archive/refs/tags/v1.0.3.zip
 Author: abuztrade
 Author-email: abuztrade.work@gmail.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Communications :: Email
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymexc-1.0.2/setup.py` & `pymexc-1.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 :author: abuztrade
 :license: MIT License, see LICENSE file.
 :copyright: (c) 2022 by abuztrade.
 """
 
 
-version = '1.0.2'
+version = '1.0.3'
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="pymexc",
     version=version,
```

