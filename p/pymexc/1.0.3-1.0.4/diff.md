# Comparing `tmp/pymexc-1.0.3.tar.gz` & `tmp/pymexc-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pymexc-1.0.3.tar", last modified: Fri Jun  2 19:58:41 2023, max compression
+gzip compressed data, was "dist\pymexc-1.0.4.tar", last modified: Fri Jun  2 20:27:56 2023, max compression
```

## Comparing `pymexc-1.0.3.tar` & `pymexc-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 19:58:41.467867 pymexc-1.0.3/
--rw-rw-rw-   0        0        0     1088 2022-10-20 18:54:22.000000 pymexc-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     3321 2023-06-02 19:58:41.467867 pymexc-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2221 2023-05-30 13:04:58.000000 pymexc-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 19:58:41.442859 pymexc-1.0.3/pymexc/
--rw-rw-rw-   0        0        0     1431 2023-05-30 13:22:30.000000 pymexc-1.0.3/pymexc/__init__.py
--rw-rw-rw-   0        0        0     5824 2023-06-02 19:49:27.000000 pymexc-1.0.3/pymexc/base.py
--rw-rw-rw-   0        0        0    18102 2023-06-02 19:53:45.000000 pymexc-1.0.3/pymexc/base_websocket.py
--rw-rw-rw-   0        0        0    67666 2023-06-02 19:56:06.000000 pymexc-1.0.3/pymexc/futures.py
--rw-rw-rw-   0        0        0    68220 2023-06-02 19:56:58.000000 pymexc-1.0.3/pymexc/spot.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:58:41.466872 pymexc-1.0.3/pymexc.egg-info/
--rw-rw-rw-   0        0        0     3321 2023-06-02 19:58:41.000000 pymexc-1.0.3/pymexc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-06-02 19:58:41.000000 pymexc-1.0.3/pymexc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 19:58:41.000000 pymexc-1.0.3/pymexc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-02 19:58:41.000000 pymexc-1.0.3/pymexc.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       26 2023-06-02 19:58:41.000000 pymexc-1.0.3/pymexc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-02 19:58:41.000000 pymexc-1.0.3/pymexc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 19:58:41.473868 pymexc-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1697 2023-05-30 18:54:32.000000 pymexc-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:27:56.528108 pymexc-1.0.4/
+-rw-rw-rw-   0        0        0     1088 2022-10-20 18:54:22.000000 pymexc-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     3321 2023-06-02 20:27:56.528108 pymexc-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2221 2023-05-30 13:04:58.000000 pymexc-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 20:27:56.508103 pymexc-1.0.4/pymexc/
+-rw-rw-rw-   0        0        0     1431 2023-05-30 13:22:30.000000 pymexc-1.0.4/pymexc/__init__.py
+-rw-rw-rw-   0        0        0     5890 2023-06-02 20:17:49.000000 pymexc-1.0.4/pymexc/base.py
+-rw-rw-rw-   0        0        0    18102 2023-06-02 19:53:45.000000 pymexc-1.0.4/pymexc/base_websocket.py
+-rw-rw-rw-   0        0        0    67666 2023-06-02 19:56:06.000000 pymexc-1.0.4/pymexc/futures.py
+-rw-rw-rw-   0        0        0    68220 2023-06-02 19:56:58.000000 pymexc-1.0.4/pymexc/spot.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:27:56.527108 pymexc-1.0.4/pymexc.egg-info/
+-rw-rw-rw-   0        0        0     3321 2023-06-02 20:27:56.000000 pymexc-1.0.4/pymexc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-06-02 20:27:56.000000 pymexc-1.0.4/pymexc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 20:27:56.000000 pymexc-1.0.4/pymexc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-02 20:27:56.000000 pymexc-1.0.4/pymexc.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       26 2023-06-02 20:27:56.000000 pymexc-1.0.4/pymexc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-02 20:27:56.000000 pymexc-1.0.4/pymexc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 20:27:56.529108 pymexc-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1697 2023-06-02 19:59:59.000000 pymexc-1.0.4/setup.py
```

### Comparing `pymexc-1.0.3/LICENSE` & `pymexc-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pymexc-1.0.3/PKG-INFO` & `pymexc-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pymexc
-Version: 1.0.3
+Version: 1.0.4
 Summary: Unofficial python library for interacting with the MEXC crypto exchange
 Home-page: https://github.com/makarworld/pymexc.git
-Download-URL: https://github.com/makarworld/pymexc/archive/refs/tags/v1.0.3.zip
+Download-URL: https://github.com/makarworld/pymexc/archive/refs/tags/v1.0.4.zip
 Author: abuztrade
 Author-email: abuztrade.work@gmail.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Communications :: Email
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymexc-1.0.3/README.md` & `pymexc-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pymexc-1.0.3/pymexc/__init__.py` & `pymexc-1.0.4/pymexc/__init__.py`

 * *Files identical despite different names*

### Comparing `pymexc-1.0.3/pymexc/base.py` & `pymexc-1.0.4/pymexc/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     
     @abstractclassmethod
     def call(self, method: Union[Literal["GET"], Literal["POST"], Literal["PUT"], Literal["DELETE"]], router: str, *args, **kwargs) -> dict:
         ...
 
 class _SpotHTTP(MexcSDK):
     def __init__(self, api_key: str = None, api_secret: str = None, proxies: dict = None):
-        super().__init__(api_key, api_secret, "https://api.mexc.com")
+        super().__init__(api_key, api_secret, "https://api.mexc.com", proxies = proxies)
 
         self.session.headers.update({
             "X-MEXC-APIKEY": self.api_key
         })
 
     def sign(self, **kwargs) -> str:
         """
@@ -82,15 +82,20 @@
 
         response = self.session.request(method, f"{self.base_url}{router}", *args, **kwargs)
 
         return response.json()
     
 class _FuturesHTTP(MexcSDK):
     def __init__(self, api_key: str = None, api_secret: str = None, proxies: dict = None):
-        super().__init__(api_key, api_secret, "https://contract.mexc.com")
+        super().__init__(api_key, api_secret, "https://contract.mexc.com", proxies = proxies)
+
+        self.session.headers.update({
+            "Content-Type": "application/json",
+            "ApiKey": self.api_key
+        })
 
     def sign(self, timestamp: str, **kwargs) -> str:
         """
         Generates a signature for an API request using HMAC SHA256 encryption.
 
         :param timestamp: A string representing the timestamp of the request.
         :type timestamp: str
@@ -133,16 +138,14 @@
                 kwargs[variant] = {k: v for k, v in kwargs[variant].items() if v is not None}
             
                 if self.api_key and self.api_secret:
                     # add signature
                     timestamp = str(int(time.time() * 1000))
 
                     kwargs['headers'] = {
-                        "Content-Type": "application/json",
-                        "ApiKey": self.api_key,
                         "Request-Time": timestamp,
                         "Signature": self.sign(timestamp, **kwargs[variant])
                     }
 
         response = self.session.request(method, f"{self.base_url}{router}", *args, **kwargs)
 
         return response.json()
```

### Comparing `pymexc-1.0.3/pymexc/base_websocket.py` & `pymexc-1.0.4/pymexc/base_websocket.py`

 * *Files identical despite different names*

### Comparing `pymexc-1.0.3/pymexc/futures.py` & `pymexc-1.0.4/pymexc/futures.py`

 * *Files identical despite different names*

### Comparing `pymexc-1.0.3/pymexc/spot.py` & `pymexc-1.0.4/pymexc/spot.py`

 * *Files identical despite different names*

### Comparing `pymexc-1.0.3/pymexc.egg-info/PKG-INFO` & `pymexc-1.0.4/pymexc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pymexc
-Version: 1.0.3
+Version: 1.0.4
 Summary: Unofficial python library for interacting with the MEXC crypto exchange
 Home-page: https://github.com/makarworld/pymexc.git
-Download-URL: https://github.com/makarworld/pymexc/archive/refs/tags/v1.0.3.zip
+Download-URL: https://github.com/makarworld/pymexc/archive/refs/tags/v1.0.4.zip
 Author: abuztrade
 Author-email: abuztrade.work@gmail.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Communications :: Email
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymexc-1.0.3/setup.py` & `pymexc-1.0.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 :author: abuztrade
 :license: MIT License, see LICENSE file.
 :copyright: (c) 2022 by abuztrade.
 """
 
 
-version = '1.0.3'
+version = '1.0.4'
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="pymexc",
     version=version,
```

