# Comparing `tmp/pyCocos-0.2.0.tar.gz` & `tmp/pyCocos-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyCocos-0.2.0.tar", last modified: Tue May 30 21:40:28 2023, max compression
+gzip compressed data, was "pyCocos-0.2.1.tar", last modified: Fri Jun  2 03:04:55 2023, max compression
```

## Comparing `pyCocos-0.2.0.tar` & `pyCocos-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:40:28.534076 pyCocos-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-30 21:40:17.000000 pyCocos-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-05-30 21:40:28.534076 pyCocos-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-05-30 21:40:17.000000 pyCocos-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 21:40:28.534076 pyCocos-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-30 21:40:17.000000 pyCocos-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:40:28.530076 pyCocos-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:40:28.534076 pyCocos-0.2.0/src/pyCocos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-05-30 21:40:28.000000 pyCocos-0.2.0/src/pyCocos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-30 21:40:28.000000 pyCocos-0.2.0/src/pyCocos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 21:40:28.000000 pyCocos-0.2.0/src/pyCocos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-30 21:40:28.000000 pyCocos-0.2.0/src/pyCocos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-30 21:40:28.000000 pyCocos-0.2.0/src/pyCocos.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:40:28.534076 pyCocos-0.2.0/src/pycocos/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-30 21:40:17.000000 pyCocos-0.2.0/src/pycocos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:40:28.534076 pyCocos-0.2.0/src/pycocos/components/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-30 21:40:17.000000 pyCocos-0.2.0/src/pycocos/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15074 2023-05-30 21:40:17.000000 pyCocos-0.2.0/src/pycocos/components/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-30 21:40:17.000000 pyCocos-0.2.0/src/pycocos/components/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-30 21:40:17.000000 pyCocos-0.2.0/src/pycocos/components/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-30 21:40:17.000000 pyCocos-0.2.0/src/pycocos/components/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    46478 2023-05-30 21:40:17.000000 pyCocos-0.2.0/src/pycocos/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:04:55.918514 pyCocos-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-02 03:04:44.000000 pyCocos-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-06-02 03:04:55.918514 pyCocos-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-06-02 03:04:44.000000 pyCocos-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 03:04:55.918514 pyCocos-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-02 03:04:44.000000 pyCocos-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:04:55.914514 pyCocos-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:04:55.914514 pyCocos-0.2.1/src/pyCocos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-06-02 03:04:55.000000 pyCocos-0.2.1/src/pyCocos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-02 03:04:55.000000 pyCocos-0.2.1/src/pyCocos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 03:04:55.000000 pyCocos-0.2.1/src/pyCocos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-02 03:04:55.000000 pyCocos-0.2.1/src/pyCocos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 03:04:55.000000 pyCocos-0.2.1/src/pyCocos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:04:55.914514 pyCocos-0.2.1/src/pycocos/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-02 03:04:44.000000 pyCocos-0.2.1/src/pycocos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:04:55.918514 pyCocos-0.2.1/src/pycocos/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-02 03:04:44.000000 pyCocos-0.2.1/src/pycocos/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15371 2023-06-02 03:04:44.000000 pyCocos-0.2.1/src/pycocos/components/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-02 03:04:44.000000 pyCocos-0.2.1/src/pycocos/components/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-02 03:04:44.000000 pyCocos-0.2.1/src/pycocos/components/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-02 03:04:44.000000 pyCocos-0.2.1/src/pycocos/components/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46762 2023-06-02 03:04:44.000000 pyCocos-0.2.1/src/pycocos/main.py
```

### Comparing `pyCocos-0.2.0/LICENSE` & `pyCocos-0.2.1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 NAcho Herrera
+Copyright (c) 2023 Nacho Herrera
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pyCocos-0.2.0/PKG-INFO` & `pyCocos-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyCocos
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python connector for Cocos Capital's Rest APIs.
 Home-page: https://github.com/nacho-herrera/pyCocos
 Author: Nacho Herrera
 Author-email: github@nachoherrera.com.ar
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -28,38 +28,38 @@
 *pyCocos* is not owned by Cocos Capital, and the authors are not responsible for the use of this library.
 
 ## Installation
 
 To install *pyCocos*, you can use the following command:
 
 ```shell
-git+https://github.com/nacho-herrera/pyCocos.git
+pip install pycocos
 ```
 
 ## API Credentials
 
-To use this library, you need to have the correct authentication credentials and a valid reCAPTCHA token.
+To use this library, you need to have the correct authentication credentials.
 
 ## Dependencies
 
 The library has the following dependency:
 
 ```
-requests==2.28.2
-simplejson==3.19.1
+requests>=2.31.0
+simplejson>=3.19.1
 ```
 ## Features
 
 This section describes the functionality and components of the library.
 
 #### Available Methods
 
 #### Initialization
 
-Before using the library, you need to initialize it with a valid email, password, and reCAPTCHA token. You can find the token using the browser dev-yTools.
+Before using the library, you need to initialize it with a valid email and password. You can find the token using the browser dev-yTools.
 
 #### REST
 
 The library provides functions to make requests to the REST API and retrieve the corresponding responses.
 
 ###### Functions
 
@@ -116,15 +116,15 @@
 ## Usage
 
 Once the library has been installed, you can import and initialize it. The initialization sets the email, password, and reCAPTCHA token. It then attempts to authenticate with the provided credentials. If the authentication fails, an `ApiException` is thrown.
 
 ```python
 from pycocos import Cocos
 
-app = Cocos(email="sample@email.com", password="S4mp13.p4ssW0rd", recaptcha_token="AsDfrEcAPtcHA-ToKeNaSDf")
+app = Cocos(email="sample@email.com", password="S4mp13.p4ssW0rd")
 ```
 
 #### REST
 
 ```python
 # Get the available portfolio with the current market valuation
 app.my_portfolio()
```

### Comparing `pyCocos-0.2.0/README.md` & `pyCocos-0.2.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -9,38 +9,38 @@
 *pyCocos* is not owned by Cocos Capital, and the authors are not responsible for the use of this library.
 
 ## Installation
 
 To install *pyCocos*, you can use the following command:
 
 ```shell
-git+https://github.com/nacho-herrera/pyCocos.git
+pip install pycocos
 ```
 
 ## API Credentials
 
-To use this library, you need to have the correct authentication credentials and a valid reCAPTCHA token.
+To use this library, you need to have the correct authentication credentials.
 
 ## Dependencies
 
 The library has the following dependency:
 
 ```
-requests==2.28.2
-simplejson==3.19.1
+requests>=2.31.0
+simplejson>=3.19.1
 ```
 ## Features
 
 This section describes the functionality and components of the library.
 
 #### Available Methods
 
 #### Initialization
 
-Before using the library, you need to initialize it with a valid email, password, and reCAPTCHA token. You can find the token using the browser dev-yTools.
+Before using the library, you need to initialize it with a valid email and password. You can find the token using the browser dev-yTools.
 
 #### REST
 
 The library provides functions to make requests to the REST API and retrieve the corresponding responses.
 
 ###### Functions
 
@@ -97,15 +97,15 @@
 ## Usage
 
 Once the library has been installed, you can import and initialize it. The initialization sets the email, password, and reCAPTCHA token. It then attempts to authenticate with the provided credentials. If the authentication fails, an `ApiException` is thrown.
 
 ```python
 from pycocos import Cocos
 
-app = Cocos(email="sample@email.com", password="S4mp13.p4ssW0rd", recaptcha_token="AsDfrEcAPtcHA-ToKeNaSDf")
+app = Cocos(email="sample@email.com", password="S4mp13.p4ssW0rd")
 ```
 
 #### REST
 
 ```python
 # Get the available portfolio with the current market valuation
 app.my_portfolio()
```

### Comparing `pyCocos-0.2.0/setup.py` & `pyCocos-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyCocos",
-    version="0.2.0",
+    version="0.2.1",
     author="Nacho Herrera",
     author_email="github@nachoherrera.com.ar",
     description="Python connector for Cocos Capital's Rest APIs.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nacho-herrera/pyCocos",
     packages=setuptools.find_packages(where='src'),
     package_dir={'': 'src'},
     install_requires=[
-        'requests>=2.28.2',
+        'requests>=2.31.0',
         'simplejson>=3.19.1',
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Development Status :: 4 - Beta",
```

### Comparing `pyCocos-0.2.0/src/pyCocos.egg-info/PKG-INFO` & `pyCocos-0.2.1/src/pyCocos.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyCocos
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python connector for Cocos Capital's Rest APIs.
 Home-page: https://github.com/nacho-herrera/pyCocos
 Author: Nacho Herrera
 Author-email: github@nachoherrera.com.ar
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -28,38 +28,38 @@
 *pyCocos* is not owned by Cocos Capital, and the authors are not responsible for the use of this library.
 
 ## Installation
 
 To install *pyCocos*, you can use the following command:
 
 ```shell
-git+https://github.com/nacho-herrera/pyCocos.git
+pip install pycocos
 ```
 
 ## API Credentials
 
-To use this library, you need to have the correct authentication credentials and a valid reCAPTCHA token.
+To use this library, you need to have the correct authentication credentials.
 
 ## Dependencies
 
 The library has the following dependency:
 
 ```
-requests==2.28.2
-simplejson==3.19.1
+requests>=2.31.0
+simplejson>=3.19.1
 ```
 ## Features
 
 This section describes the functionality and components of the library.
 
 #### Available Methods
 
 #### Initialization
 
-Before using the library, you need to initialize it with a valid email, password, and reCAPTCHA token. You can find the token using the browser dev-yTools.
+Before using the library, you need to initialize it with a valid email and password. You can find the token using the browser dev-yTools.
 
 #### REST
 
 The library provides functions to make requests to the REST API and retrieve the corresponding responses.
 
 ###### Functions
 
@@ -116,15 +116,15 @@
 ## Usage
 
 Once the library has been installed, you can import and initialize it. The initialization sets the email, password, and reCAPTCHA token. It then attempts to authenticate with the provided credentials. If the authentication fails, an `ApiException` is thrown.
 
 ```python
 from pycocos import Cocos
 
-app = Cocos(email="sample@email.com", password="S4mp13.p4ssW0rd", recaptcha_token="AsDfrEcAPtcHA-ToKeNaSDf")
+app = Cocos(email="sample@email.com", password="S4mp13.p4ssW0rd")
 ```
 
 #### REST
 
 ```python
 # Get the available portfolio with the current market valuation
 app.my_portfolio()
```

### Comparing `pyCocos-0.2.0/src/pycocos/components/client.py` & `pyCocos-0.2.1/src/pycocos/components/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,48 +28,48 @@
         Returns:
             dict: Dict with token and user data
         """
         return self.api_request(
             urls.endpoints["token"], method="post", params=params, data=data
         )
 
-    def logout(self) -> Dict[str, Any]:
+    def logout(self) -> None:
         """Makes a request to the api to logout current session
 
         Returns:
             dict: empty dict
         """
         return self.api_request(urls.endpoints["logout"], method="post")
 
-    def get_market_status(self) -> Dict[str, Any]:
+    def get_market_status(self) -> Dict[str, bool]:
         """Makes a request to the api to know if market is open
 
 
         Returns:
-            dict: Market status (0-CI, 1-24hs, 2-48hs, 3-DolarMEP Bot) as boolean
+            dict: Market status (0-CI, 1-24hs, 2-48hs, 3-DolarMEP Bot, 4-??, 5-??) as boolean
         """
         return self.api_request(urls.endpoints["open_market"])
 
-    def get_university(self) -> Dict[str, Any]:
+    def get_university(self) -> List[Dict[str, str]]:
         """Makes a request to the api to get Cocos University articles
 
         Returns:
             list: List of Cocos University articles
         """
         return self.api_request(urls.endpoints["university"])
 
-    def get_carrousel(self) -> Dict[str, Any]:
+    def get_carrousel(self) -> List[Dict[str, str]]:
         """Makes a request to the api to get home page's promoted instruments
 
         Returns:
             list: List of home page's promoted instruments
         """
         return self.api_request(urls.endpoints["carrousel"])
 
-    def get_news(self) -> Dict[str, Any]:
+    def get_news(self) -> List[Dict[str, Any]]:
         """Makes a request to the api to get home page's news
 
         Returns:
             list: List of home page's news
         """
         return self.api_request(urls.endpoints["news"])
 
@@ -77,15 +77,15 @@
         """Makes a request to the api to get my account data
 
         Returns:
             dict: Dict with account information
         """
         return self.api_request(urls.endpoints["my_data"])
 
-    def get_investor_test(self) -> Dict[str, Any]:
+    def get_investor_test(self) -> List[Dict[str, Any]]:
         """Makes a request to get the investor test questions
 
         Returns:
             list: List of questions
         """
         return self.api_request(urls.endpoints["investor_test"])
 
@@ -106,15 +106,15 @@
         """Makes a request to get daily performance of our account
 
         Returns:
             dict: Dictionary with the daily performance by ticker
         """
         return self.api_request(urls.endpoints["daily_performance"])
 
-    def get_historic_performance(self) -> Dict[str, Any]:
+    def get_historic_performance(self) -> List[Dict[str, Any]]:
         """Makes a request to get historic performance of our account
 
         Returns:
             list: List of historic performance by ticker
         """
         return self.api_request(urls.endpoints["historic_performance"])
 
@@ -190,15 +190,15 @@
             json (dict): Dictionary with withdraw information
 
         Returns:
             dict: API Response
         """
         return self.api_request(urls.endpoints["withdraw"], method="post", data=data)
 
-    def get_orders(self) -> Dict[str, Any]:
+    def get_orders(self) -> List[Dict[str, Any]]:
         """Makes a request to get the status of all orders
 
         Returns:
             list: List of orders statuses
         """
         return self.api_request(urls.endpoints["orders"])
 
@@ -281,23 +281,23 @@
         """Makes a request to get bot's dolar mep quotes
 
         Returns:
             dict: Dictionary with quotes and additional info
         """
         return self.api_request(urls.endpoints["open_dolar_mep"])
 
-    def get_home_list(self) -> List[Dict[str, Any]]:
+    def get_home_list(self) -> Dict[str, Any]:
         """Makes a request to get Home page quote list
 
         Returns:
             list: List of homepage quotes
         """
         return self.api_request(urls.endpoints["home_list"])
 
-    def get_my_list(self) -> List[Dict[str, Any]]:
+    def get_my_list(self) -> Dict[str, Any]:
         """Makes a request to get favorite quote list
 
         Returns:
             list: List of favorite quotes
         """
         return self.api_request(urls.endpoints["my_list"])
 
@@ -389,15 +389,15 @@
             segment (Segments (Enum)): Segment of the instrument
 
         Returns:
             list: List of long tickers for the same short ticker
         """
         return self.api_request(urls.endpoints["tickers"].format(ticker, segment))
 
-    def search_tickers(self, ticker: str) -> Dict[str, Any]:
+    def search_tickers(self, ticker: str) -> List[Dict[str, Any]]:
         """Makes a request to search tickers
 
         Args:
             ticker (str): Query of the search
 
         Returns:
             list: List of possible tickers
@@ -408,15 +408,15 @@
         """Makes a request to get BYMA price rules
 
         Returns:
             list: List of rules for specific instruments price ranges
         """
         return self.api_request(urls.endpoints["rules"])
 
-    def get_instrument_types(self) -> Dict[str, Any]:
+    def get_instrument_types(self) -> List[Dict[str, Any]]:
         """Makes a request to get types of instruments lists
 
         Returns:
             list: List of Types and Subtypes of available instruments
         """
         return self.api_request(urls.endpoints["types"])
 
@@ -429,41 +429,50 @@
         path: str,
         retry: bool = True,
         method: str = "get",
         params: str = "",
         json_data: Dict[str, Any] = {},
         data: str = "",
     ):
+        response = None
+
+        if method not in ["get", "post", "delete"]:
+            raise ApiException(f"Method {method} not suported")
         if method == "get":
             response = self.session.get(self._api_url(path))
 
         if method == "post":
             response = self.session.post(
                 self._api_url(path),
                 params=params,
                 data=data,
                 json=json_data,
             )
 
         if method == "delete":
-            response = self.session.delete(self._api_url(path), json=json_data)
+            response = self.session.delete(
+                self._api_url(path), json=json_data
+            )
+
+        if not response:
+            raise ApiException("Bad HTTP API Response")
 
         json_response = simplejson.loads(response.text)
 
         if response.status_code == 401:
             if retry:
                 self.api_request(path, retry=False)
             else:
                 raise ApiException("Authentication Fails.")
 
         if response.status_code == 500:
             raise ApiException(f"Error 500 {json_response}")
 
         if response.status_code == 200:
-            self._log_message(path, json_response)
+            self._log_message(path, str(json_response))
         return json_response
 
     def update_session_headers(self, header_update: Dict[str, Any]) -> None:
         self.session.headers.update(header_update)
 
     def _api_url(self, path: str) -> str:
         return urls.api_url + path
```

### Comparing `pyCocos-0.2.0/src/pycocos/components/enums.py` & `pyCocos-0.2.1/src/pycocos/components/enums.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 
 from enum import Enum
 
 
 class Currency(Enum):
     """Enumerates the supported currencies in the application."""
 
-    DOLAR_CABLE = "CABLE"
-    DOLAR_MEP = "MEP"
+    ALL = "INDISTINTO"
+    CABLE = "EXT"
+    NONE = ""
     PESOS = "ARS"
-
+    USD = "USD"
 
 class OrderType(Enum):
     """Enumerates the types of orders supported in the application."""
 
     LIMIT = "LIMIT"
     MARKET = "MARKET"
 
@@ -27,19 +28,19 @@
 
     BUY = "BUY"
     SELL = "SELL"
 
 
 class Segment(Enum):
     """Enumerates the market segments in the application.
-    
-    For FCI instruments use Segments.FCI; 
-    for stock options use Segments.OPTIONS; 
-    for Repo instruments use Segments.REPO. 
-    Otherwise use Segments.DEFAULT for everything else
+
+    For FCI instruments use Segment.FCI;
+    for stock options use Segment.OPTIONS;
+    for Repo instruments use Segment.REPO.
+    Otherwise use Segment.DEFAULT for everything else
     """
 
     DEFAULT = "C"
     FCI = "FCI"
     OPTIONS = "O"
     REPO = "U"
 
@@ -57,31 +58,35 @@
 
 
 class InstrumentSubType(Enum):
     """Enumerates the instruments sub-categories in the application."""
 
     ARS = "NACIONALES_ARS"
     CER = "CER"
+    CRYPTO = "CRYPTO"
     ETF = "ETF"
     FIXED = "TASA_FIJA"
     GENERAL = "GENERAL"
     LIDERES = "LIDERES"
     NEW = "NUEVOS"
+    NONE = ""
+    OTROS = "OTROS"
+    PF = "PF"
     PROV = "PROVINCIALES"
     TOP = "TOP"
     USD = "NACIONALES_USD"
-    NONE = None
+
 
 class Settlement(Enum):
     """Enumerates the settlement options for trades in the application."""
 
     T0 = "CI"
     T1 = "24hs"
     T2 = "48hs"
-
+    NONE = ""
 
 class PerformanceTimeframe(Enum):
     """Enumerates the different types of performance reports available in the application."""
 
     DAILY = "daily"
     HISTORICAL = "historical"
     RANGE = "range"
```

### Comparing `pyCocos-0.2.0/src/pycocos/components/urls.py` & `pyCocos-0.2.1/src/pycocos/components/urls.py`

 * *Files identical despite different names*

### Comparing `pyCocos-0.2.0/src/pycocos/main.py` & `pyCocos-0.2.1/src/pycocos/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,20 +19,20 @@
     RestClient,
     Segment,
     Settlement,
 )
 
 
 class Cocos:
-    headers = {
+    headers: dict[str, str] = {
         "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:91.0) Gecko/20100101 Firefox/91.0",
         "Content-Type": "application/json",
     }
 
-    def __init__(self, email: str, password: str, recaptcha_token: str) -> None:
+    def __init__(self, email: str, password: str, recaptcha_token: str = "undefined") -> None:
         ## Parameters validation
         required_fields = [
             ("email", email, str),
             ("password", password, str),
             ("recaptcha_token", recaptcha_token, str),
         ]
         self._check_fields(required_fields)
@@ -70,20 +70,20 @@
         It then updates the session headers with the obtained token for subsequent API requests.
 
         Raises:
             Exception: If there is an error during the authentication process.
             Exception: If the access token is not found in the API response.
         """
         params = "grant_type=password"
-        payload = json.dumps({"email": self.email, "password": self.password})
+        payload: str = json.dumps({"email": self.email, "password": self.password})
 
         self.client.update_session_headers(self.headers)
 
-        response = self.client.get_token(params=params, data=payload)
-        
+        response: Dict[str, Any] = self.client.get_token(params=params, data=payload)
+
         if "error" in response.keys():
             raise Exception(f'Error: {response["error_description"]}')
 
         if "access_token" not in response.keys():
             raise Exception("Error: Access token not found in the API response")
 
         self.access_token = response["access_token"]
@@ -93,15 +93,15 @@
         """Updates the session headers and performs additional steps after login.
 
         After successful login and obtaining the access token, this method is responsible for updating the session headers
         with the necessary authentication information. It replicates the workflow of the web app.
 
         """
 
-        headers_update = {
+        headers_update: dict[str, str] = {
             "authorization": f"Bearer {self.access_token}",
             "recaptcha-token": self.recaptcha_token,
             "x-account-id": self.account_number,
         }
 
         self.client.update_session_headers(headers_update)
 
@@ -170,24 +170,24 @@
 
         Note:
             The returned dictionary may include details such as the list of holdings, their quantities, market values, and other relevant data.
 
         Raises:
             Exception: If there is an error while retrieving the portfolio information.
         """
-        response = self.client.get_portfolio()
+        response: Dict[str, Any] = self.client.get_portfolio()
         return response
 
-    def funds_available(self) -> Dict[str, float]:
+    def funds_available(self) -> Dict[str, Dict[str, float]]:
         """Retrieves the available funds for trading in T+0, T+1, and T+2 settlement dates.
 
         This method calls the API to fetch the available funds that can be used for trading on different settlement dates.
 
         Returns:
-            Dict[str, float]: A dictionary containing the available funds for each settlement date.
+            Dict[str, Dict[str, float]: A dictionary containing the available funds for each settlement date.
 
         Note:
             The returned dictionary contains key-value pairs, where the keys represent the settlement dates (e.g., T+0, T+1, T+2),
             and the values represent the corresponding available funds as floating-point numbers.
 
         Raises:
             Exception: If there is an error while retrieving the available funds.
@@ -236,14 +236,15 @@
 
         Raises:
             Exception: If there is an error while retrieving the account funds activity.
         """
 
         # Parameters validation
         required_fields = [("date_from", date_from, str), ("date_to", date_to, str)]
+
         self._check_fields(required_fields)
 
         return self.client.get_account_movements(date_from, date_to)
 
     def portfolio_performance(
         self, timeframe: PerformanceTimeframe, date_from: str = "", date_to: str = ""
     ) -> Dict[str, Any]:
@@ -291,15 +292,15 @@
 
         This method sends a request to add a new bank account to the user's profile. The account is associated with the
         provided CBU/CVU and CUIT, and is specified in the specified currency.
 
         Args:
             cbu (str): The CBU/CVU of the new bank account.
             cuit (str): The CUIT (tax identification number) of the account owner.
-            currency (Currencies): The currency of the new bank account.
+            currency (Currency): The currency of the new bank account.
 
         Returns:
             Dict[str, Any]: A dictionary containing the response from the API.
 
         Raises:
             Exception: If there is an error while submitting the new bank account.
 
@@ -310,28 +311,30 @@
             ("cbu_cvu", cbu, str),
             ("cuit", cuit, str),
             ("currency", currency, Currency),
         ]
         self._check_fields(required_fields)
 
         # Create payload object
-        payload = json.dumps({"cbu_cvu": cbu, "cuit": cuit, "currency": currency.value})
-        response = self.client.submit_new_bank_account(data=payload)
+        payload: str = json.dumps(
+            {"cbu_cvu": cbu, "cuit": cuit, "currency": currency.value}
+        )
+        response: Dict[str, Any] = self.client.submit_new_bank_account(data=payload)
         return response
 
     def withdraw_funds(
         self, currency: Currency, amount: str, cbu_cvu: str
     ) -> Dict[str, Any]:
         """Submits a request to withdraw funds through the API.
 
         This method sends a request to withdraw funds from the user's account. The specified amount of funds in the given
         currency will be transferred to the provided bank account (CBU/CVU).
 
         Args:
-            currency (Currencies): The currency of the funds to withdraw.
+            currency (Currency): The currency of the funds to withdraw.
             amount (str): The amount of funds to withdraw.
             cbu_cvu (str): The bank account (CBU/CVU) to transfer the funds to.
 
         Raises:
             ApiException: If the specified bank account is not available. Please add it to your account.
 
         Returns:
@@ -402,23 +405,23 @@
         self._check_fields(required_fields)
 
         # Check if account has enough money to purchase
         if not self._validate_buy_power(long_ticker, quantity, price):
             raise ApiException(f"Not enough money to purchase")
 
         # Create payload object
-        payload = {
+        payload: Dict[str, str] = {
             "type": order_type.value,
             "side": self.order_sides.BUY.value,
             "quantity": quantity,
             "long_ticker": long_ticker,
             "price": price,
         }
 
-        response = self.client.submit_order(json=payload)
+        response: Dict[str, Any] = self.client.submit_order(json=payload)
         if "success" in response.keys():
             self._add_order(response["Orden"])
         return response
 
     def submit_sell_order(
         self,
         long_ticker: str,
@@ -450,23 +453,23 @@
         self._check_fields(required_fields)
 
         # Check if account has enough stocks to sell
         if not self._validate_sell_power(long_ticker, quantity):
             raise ApiException(f"Not enough stocks to sell")
 
         ## Create Payload object
-        payload = {
+        payload: Dict[str, str] = {
             "type": order_type.value,
             "side": self.order_sides.SELL.value,
             "quantity": quantity,
             "long_ticker": long_ticker,
             "price": price,
         }
 
-        response = self.client.submit_order(json=payload)
+        response: Dict[str, Any] = self.client.submit_order(json=payload)
         return response
 
     def place_repo_order(
         self, currency: Currency, amount: float, term: int, rate: float
     ) -> Dict[str, Any]:
         """Submits a repo order through the API.
 
@@ -491,24 +494,24 @@
             ("amount", amount, float),
             ("term", term, int),
             ("rate", rate, float),
         ]
         self._check_fields(required_fields)
 
         # Create payload object
-        payload = json.dumps(
+        payload: str = json.dumps(
             {
                 "currency": currency.value,
                 "amount": amount,
                 "term": term,
                 "rate": rate,
             }
         )
 
-        response = self.client.submit_repo_order(data=payload)
+        response: Dict[str, Any] = self.client.submit_repo_order(data=payload)
         return response
 
     def cancel_order(self, order_number: str) -> Dict[str, Any]:
         """Cancels an existing order through the API.
 
         This method sends a request to cancel a previously submitted order identified by its order number. The order will be
         cancelled, and the API response will provide information about the cancellation status.
@@ -522,25 +525,27 @@
         """
 
         # Parameters validation
         required_fields = [("order_number", order_number, str)]
         self._check_fields(required_fields)
 
         # Retrieve order information
-        order = self.order_status(order_number)
+        order: Dict[str, Any] = self.order_status(order_number)  # type: ignore
 
         # Create payload object
-        payload = json.dumps(
+        payload: str = json.dumps(
             {"instrument": order["instrument"], "ticker": order["ticker"]}
         )
 
-        response = self.client.cancel_order(order_number, data=payload)
+        response: Dict[str, Any] = self.client.cancel_order(order_number, data=payload)
         return response
 
-    def order_status(self, order_number: str = "") -> Dict[str, Any]:
+    def order_status(
+        self, order_number: str = ""
+    ) -> Dict[str, Any] | List[Dict[str, Any]]:
         """Calls the API to retrieve order status information.
 
         This method retrieves the status information of one or more orders from the API. If an `order_number` is provided,
         it returns the status of the specific order. If no `order_number` is provided, it returns the status of all orders.
 
         Args:
             order_number (str, optional): The order number of the specific order to retrieve the status for.
@@ -592,23 +597,26 @@
     ) -> List[Dict[str, Any]]:
         """Calls the API to retrieve a snapshot of price data for a given ticker.
 
         This method retrieves the snapshot price data for a specified ticker in a specific segment.
 
         Args:
             ticker (str): The ticker symbol to retrieve the price data for.
-            segment (Segments): The segment of the ticker.
+            segment (Segment): The segment of the ticker.
 
         Returns:
             List[Dict[str, Any]]: A list of dictionaries containing the snapshot price data for all possible settlement dates of the ticker.
 
         """
 
         # Parameters validation
-        required_fields = [("ticker", ticker, str), ("segment", segment, Segment)]
+        required_fields = [
+            ("ticker", ticker, str),
+            ("segment", segment, Segment),
+        ]
         self._check_fields(required_fields)
 
         return self.client.get_tickers(ticker, segment.value)
 
     def get_instrument_list_snapshot(
         self,
         instrument_type: InstrumentType,
@@ -619,19 +627,19 @@
     ) -> List[Dict[str, Any]]:
         """Calls the API to retrieve a list of instruments based on specified criteria.
 
         This method retrieves a list of instruments based on the provided instrument type, instrument subtype,
         settlement, currency, and segment.
 
         Args:
-            instrument_type (InstrumentTypes): The category type of the instruments.
-            instrument_subtype (InstrumentSubTypes): The category subtype of the instruments.
+            instrument_type (InstrumentType): The category type of the instruments.
+            instrument_subtype (InstrumentSubType): The category subtype of the instruments.
             settlement (Settlements): The settlement type for the instruments.
-            currency (Currencies): The currency for the instruments.
-            segment (Segments): The segment for the instruments.
+            currency (Currency): The currency for the instruments.
+            segment (Segment): The segment for the instruments.
 
         Returns:
             List[Dict[str, Any]]: A list of dictionaries containing the instrument information for the selected instruments.
 
         Raises:
             ValueError: If the combination of instrument type and subtype is invalid. Refer to the instrument_types_and_subtypes method.
 
@@ -674,19 +682,19 @@
     ) -> Dict[str, Any]:
         """Calls the API to retrieve a paginated list of instruments based on specified criteria.
 
         This method retrieves a paginated list of instruments based on the provided instrument type, instrument subtype,
         settlement, currency, segment, page number, and items per page.
 
         Args:
-            instrument_type (InstrumentTypes): The category type of the instruments.
-            instrument_subtype (InstrumentSubTypes): The category subtype of the instruments.
-            settlement (Settlements): The settlement type for the instruments.
-            currency (Currencies): The currency for the instruments.
-            segment (Segments): The segment for the instruments.
+            instrument_type (InstrumentType): The category type of the instruments.
+            instrument_subtype (InstrumentSubType): The category subtype of the instruments.
+            settlement (Settlement): The settlement type for the instruments.
+            currency (Currency): The currency for the instruments.
+            segment (Segment): The segment for the instruments.
             page (int): The page number to retrieve.
             size (int): The number of items per page.
 
         Returns:
             Dict[str, Any]: A dictionary containing the paginated list of selected instruments.
 
         Raises:
@@ -719,15 +727,15 @@
             settlement.value,
             currency.value,
             segment.value,
             page,
             size,
         )
 
-    def get_recommended_tickers(self) -> List[Dict[str, Any]]:
+    def get_recommended_tickers(self) -> Dict[str, Any]:
         """Calls the API to retrieve the list of recommended tickers from the home page.
 
         This method retrieves the list of recommended tickers provided on the home page of the application.
 
         Returns:
             List[Dict[str, Any]]: A list of dictionaries containing the recommended tickers.
 
@@ -735,15 +743,15 @@
             The structure and content of the returned list may vary depending on the API response. Each dictionary in the list
             represents a recommended ticker and may contain different fields such as ticker symbol, company name, price, etc.
 
         """
 
         return self.client.get_home_list()
 
-    def get_favorites_tickers(self) -> List[Dict[str, Any]]:
+    def get_favorites_tickers(self) -> Dict[str, Any]:
         """Calls the API to retrieve the list of favorite instruments from the home page.
 
         This method retrieves the list of favorite instruments that have been saved by the user on the home page of the application.
 
         Returns:
             List[Dict[str, Any]]: A list of dictionaries containing the favorite instruments.
 
@@ -751,25 +759,25 @@
             The structure and content of the returned list may vary depending on the API response. Each dictionary in the list
             represents a favorite instrument and may contain different fields such as ticker symbol, company name, price, etc.
 
         """
 
         return self.client.get_my_list()
 
-    def search_ticker(self, query: str) -> Dict[str, Any]:
+    def search_ticker(self, query: str) -> List[Dict[str, Any]]:
         """Calls the API to search for a ticker by name.
 
         This method allows searching for a ticker by providing a query string representing the name or part of the name of the ticker.
         The API will return the search results matching the query.
 
         Args:
             query (str): The query string representing the ticker name to search.
 
         Returns:
-            Dict[str, Any]: The API response with the search results.
+            List[Dict[str, Any]]: The API response with the search results.
 
         Raises:
             ValueError: If the query string is less than 2 characters long.
 
         Note:
             The structure and content of the returned dictionary may vary depending on the API response.
 
@@ -814,15 +822,15 @@
         Note:
             The structure and content of the returned dictionary may vary depending on the API response.
 
         """
 
         return self.client.get_instrument_rules()
 
-    def instrument_types_and_subtypes(self) -> Dict[str, Any]:
+    def instrument_types_and_subtypes(self) -> List[Dict[str, Any]]:
         """Calls the API to retrieve the types and subtypes of available instruments.
 
         This method retrieves information about the different types and subtypes of instruments
         available for trading. It provides a comprehensive list of instrument categories and their
         corresponding subcategories.
 
         Returns:
@@ -901,15 +909,15 @@
 
         return self.client.get_open_dolar_mep()
 
     ##########
     ## MISC ##
     ##########
 
-    def get_ads_carrousel(self) -> Dict[str, Any]:
+    def get_ads_carrousel(self) -> List[Dict[str, Any]]:
         """Calls API to retrieve the carousel ads.
 
         The carousel ads are a collection of advertisements displayed in a carousel format.
         This method calls the API to fetch the carousel ads.
 
         Returns:
             Dict[str, Any]: API Response with the carousel ads.
@@ -917,15 +925,15 @@
         Note:
             The structure and content of the returned dictionary may vary depending on the API response.
 
         """
 
         return self.client.get_carrousel()
 
-    def get_news(self) -> Dict[str, Any]:
+    def get_news(self) -> List[Dict[str, Any]]:
         """Calls API to retrieve news articles.
 
         This method calls the API to fetch the latest news articles. The returned news articles
         can contain information about various topics such as finance, economy, market updates, etc.
 
         Returns:
             Dict[str, Any]: API Response with the news articles.
@@ -933,15 +941,15 @@
         Note:
             The structure and content of the returned dictionary may vary depending on the API response.
 
         """
 
         return self.client.get_news()
 
-    def get_cocos_university_articles(self) -> Dict[str, Any]:
+    def get_cocos_university_articles(self) -> List[Dict[str, Any]]:
         """Calls API to retrieve articles from Cocos University.
 
         This method calls the API to fetch articles from Cocos University, which provides educational content
         related to finance, investing, trading, and other relevant topics. The articles aim to educate and
         inform users about various aspects of the financial industry.
 
         Returns:
@@ -969,16 +977,16 @@
         Helper function to create a long ticker based on the ticker, settlement, segment, and currency.
         It does not validate the segment against valid ticker and segment combinations.
         If you're unsure, it's recommended to use the `search_instrument` method to validate.
 
         Args:
             ticker (str): Ticker symbol of the instrument.
             settlement (Settlements): Settlement date of the instrument.
-            currency (Currencies): Currency of the instrument.
-            segment (Segments, optional): Segment of the instrument. Defaults to Segments.DEFAULT.
+            currency (Currency): Currency of the instrument.
+            segment (Segment, optional): Segment of the instrument. Defaults to Segment.DEFAULT.
 
         Returns:
             str: The long ticker representing the ticker and settlement date.
 
         Notes:
             - The `segment` argument is not validated against valid ticker and segment combinations.
             It's important to ensure the appropriate segment is provided.
@@ -987,25 +995,25 @@
                 - <TICKER> represents the ticker symbol in uppercase.
                 - <SETTLEMENT> is a code representing the settlement date (e.g., "0001" for T0).
                 - <SEGMENT> is the segment of the instrument.
                 - CT indicates the BYMA market venue.
                 - <CURRENCY> represents the currency code.
 
         Examples:
-            long_ticker("AAPL", Settlements.T1, Currencies.PESOS) returns "AAPL-0002-C-CT-ARS"
-            long_ticker("GOOGD", Settlements.T0, Currencies.DOLAR_MEP) returns "GOOGD-0001-C-CT-USD"
-            long_ticker("GFGC500.JU", Settlements.T2, Currencies.PESOS, Segments.OPTIONS) returns "GFGC500.JU-0001-O-CT-ARS"
+            long_ticker("AAPL", Settlements.T1, Currency.PESOS) returns "AAPL-0002-C-CT-ARS"
+            long_ticker("GOOGD", Settlements.T0, Currency.DOLAR_MEP) returns "GOOGD-0001-C-CT-USD"
+            long_ticker("GFGC500.JU", Settlements.T2, Currency.PESOS, Segment.OPTIONS) returns "GFGC500.JU-0001-O-CT-ARS"
 
         """
 
         if segment is Segment.FCI:
             return ticker.upper()
 
-        _settlement = self._get_byma_settlement(settlement)
-        _currency = self._get_byma_currency(currency)
+        _settlement: str = self._get_byma_settlement(settlement)
+        _currency: str = self._get_byma_currency(currency)
 
         return f"{ticker.upper()}-{_settlement}-{segment.value}-CT-{_currency}"
 
     def _validate_buy_power(self, long_ticker: str, quantity: str, price: str) -> bool:
         """
         Validates if there are sufficient funds available to place a buy order.
 
@@ -1017,19 +1025,24 @@
         Returns:
             bool: True if there are sufficient funds, False otherwise.
         """
         _, settlement, segment, _, currency = long_ticker.split("-")
 
         settlement = self._get_cocos_settlement(settlement)
         segment = self._get_cocos_segment(segment)
+        if not settlement:
+            return False
+        if not segment:
+            return False
+
         instrument_code = self._find_instrument_code(long_ticker)
         price_factor = self._get_price_factor(instrument_code, long_ticker, segment)
 
         available_funds = self.funds_available()
-        available_at_settlement_currency = available_funds[settlement.value][
+        available_at_settlement_currency: float = available_funds[settlement.value][
             currency.lower()
         ]
         order_total = float(quantity) * float(price) / price_factor
 
         print(f"{order_total}, {available_at_settlement_currency}")
 
         return available_at_settlement_currency >= order_total
@@ -1040,39 +1053,43 @@
 
         Args:
             long_ticker (str): The long ticker of the instrument.
             quantity (str): The quantity of instruments to sell.
 
         Returns:
             bool: True if there are sufficient stocks, False otherwise.
-        """        
+        """
         settlement = long_ticker.split("-")[1]
         settlement = self._get_cocos_settlement(settlement)
         available_stocks = self.stocks_available(long_ticker)
-        available_at_settlement = available_stocks.get(settlement.value, 0)
+        if not settlement:
+            return False
 
+        available_at_settlement = available_stocks.get(settlement.value, 0)
         return available_at_settlement >= float(quantity)
 
     def _find_instrument_code(self, long_ticker: str) -> str:
         """
         Finds the instrument code for the given long ticker.
 
         Args:
             long_ticker (str): The long ticker of the instrument.
 
         Returns:
-            str: The instrument code, or None if not found.
+            str: The instrument code, or "" if not found.
         """
-        ticker_search = self.search_ticker(long_ticker.split("-")[0])
+        ticker_search: List[Dict[str, Any]] = self.search_ticker(
+            long_ticker.split("-")[0]
+        )
         for ticker in ticker_search:
             for subtype in ticker["instrument_subtypes"]:
                 for data in subtype["market_data"]:
                     if data.get("long_ticker") == long_ticker:
                         return data["instrument_code"]
-        return None
+        return ""
 
     def _get_price_factor(
         self, instrument_code: str, long_ticker: str, segment: Segment
     ) -> float:
         """
         Retrieves the price factor for the given instrument code and long ticker.
 
@@ -1080,15 +1097,17 @@
             instrument_code (str): The instrument code.
             long_ticker (str): The long ticker of the instrument.
             segment (Segment): The segment of the instrument.
 
         Returns:
             float: The price factor if found, or 1 if not found.
         """
-        instrument_snapshot = self.get_instrument_snapshot(instrument_code, segment)
+        instrument_snapshot: List[Dict[str, Any]] = self.get_instrument_snapshot(
+            instrument_code, segment
+        )
         for instrument in instrument_snapshot:
             if instrument.get("long_ticker") == long_ticker:
                 return instrument["price_factor"]
         return 1
 
     ##############
     ## INTERNAL ##
@@ -1100,87 +1119,77 @@
 
         Args:
             settlement (Settlement): The settlement type.
 
         Returns:
             str: The corresponding BYMA settlement code.
         """
-        byma_settlement_map = {
+        byma_settlement_map: dict[Settlement, str] = {
             Settlement.T0: "0001",
             Settlement.T1: "0002",
             Settlement.T2: "0003",
         }
         return byma_settlement_map.get(settlement, "")
 
-    def _get_byma_currency(self, currency: Currency) -> str:
-        """
-        Retrieves the BYMA currency code for the given currency type.
-
-        Args:
-            currency (Currency): The currency type.
-
-        Returns:
-            str: The corresponding BYMA currency code.
-        """
-        byma_currency_map = {
-            Currency.PESOS: "ARS",
-            Currency.DOLAR_MEP: "USD",
-            Currency.DOLAR_CABLE: "",
-        }
-        return byma_currency_map.get(currency, "")
-
     def _get_cocos_settlement(self, settlement: str) -> Optional[Settlement]:
         """
         Retrieves the Settlement type for the given BYMA settlement code in Cocos.
 
         Args:
             settlement (str): The BYMA settlement code.
 
         Returns:
             Settlement or None: The corresponding Settlement type, or None if not found.
         """
-        cocos_settlement_map = {
+        cocos_settlement_map: dict[str, Settlement] = {
             "0001": Settlement.T0,
             "0002": Settlement.T1,
             "0003": Settlement.T2,
         }
         return cocos_settlement_map.get(settlement)
 
     def _get_cocos_segment(self, segment: str) -> Segment:
-        cocos_segment_map = {
-            "C": Segment.DEFAULT,
-            "O": Segment.OPTIONS,
-            "U": Segment.REPO,
-        }
-        return cocos_segment_map.get(segment)
+        return self.segments(segment)
+
+    def _get_byma_currency(self, currency: Currency) -> str:
+        """
+        Retrieves the BYMA currency code for the given currency type.
+
+        Args:
+            currency (Currency): The currency type.
 
-    def _get_cocos_currency(self, currency: str) -> Optional[Currency]:
+        Returns:
+            str: The corresponding BYMA currency code.
+        """
+        return currency.value
+
+    def _get_cocos_currency(self, currency: str) -> Currency:
         """
         Retrieves the Currency type for the given BYMA currency code in Cocos.
 
         Args:
             currency (str): The BYMA currency code.
 
         Returns:
             Currency or None: The corresponding Currency type, or None if not found.
         """
-        cocos_currency_map = {"ARS": Currency.PESOS, "USD": Currency.DOLAR_MEP}
-        return cocos_currency_map.get(currency)
+
+        return self.currencies(currency)
 
     def _check_cbu_cvu_exists(self, cbu_cvu_to_check: str) -> bool:
         """
         Private helper function that checks if a given CBU/CVU exists in the user's bank accounts.
 
         Args:
             cbu_cvu_to_check (str): The CBU/CVU to check for existence.
 
         Returns:
             bool: True if the CBU/CVU exists in the user's bank accounts, False otherwise.
         """
-        accounts_list = self.my_bank_accounts()
+        accounts_list: List[Dict[str, Any]] = self.my_bank_accounts()
         return any(item["cbu_cvu"] == cbu_cvu_to_check for item in accounts_list)
 
     def _add_order(self, order_number: str) -> None:
         """
         Private helper function to add an order number to the list of orders.
 
         Args:
@@ -1199,15 +1208,15 @@
             new_account_number (str): The new account number to set.
 
         Returns:
             None
         """
         self.account_number = new_account_number
 
-    def _check_fields(self, fields) -> None:
+    def _check_fields(self, fields: List[Tuple[str, Any, Any]]) -> None:
         """
         Private helper function to check the types of fields.
 
         Args:
             fields (list): A list of tuples containing the field name, field value, and field type.
 
         Raises:
@@ -1216,15 +1225,15 @@
         Returns:
             None
         """
         for field_name, field_value, field_type in fields:
             if not isinstance(field_value, field_type):
                 raise ValueError(f"{field_name} is not of type {field_type.__name__}")
 
-    def _validate_list_parameters(self, type, subtype) -> bool:
+    def _validate_list_parameters(self, type: str, subtype: str) -> bool:
         """
         Private helper function to validate instrument type and subtype combinations.
 
         Args:
             type (str): Instrument type.
             subtype (str): Instrument subtype.
```

