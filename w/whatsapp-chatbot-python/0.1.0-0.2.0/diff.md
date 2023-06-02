# Comparing `tmp/whatsapp-chatbot-python-0.1.0.tar.gz` & `tmp/whatsapp-chatbot-python-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatsapp-chatbot-python-0.1.0.tar", last modified: Sat May 27 08:31:42 2023, max compression
+gzip compressed data, was "whatsapp-chatbot-python-0.2.0.tar", last modified: Fri Jun  2 06:13:43 2023, max compression
```

## Comparing `whatsapp-chatbot-python-0.1.0.tar` & `whatsapp-chatbot-python-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 08:31:42.675092 whatsapp-chatbot-python-0.1.0/
--rw-rw-rw-   0        0        0    18829 2023-05-27 08:06:12.000000 whatsapp-chatbot-python-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     8572 2023-05-27 08:31:42.675092 whatsapp-chatbot-python-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     7547 2023-05-27 08:19:22.000000 whatsapp-chatbot-python-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-27 08:31:42.676095 whatsapp-chatbot-python-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1405 2023-05-26 04:40:24.000000 whatsapp-chatbot-python-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-27 08:31:42.665066 whatsapp-chatbot-python-0.1.0/tests/
--rw-rw-rw-   0        0        0     1208 2023-05-27 07:42:49.000000 whatsapp-chatbot-python-0.1.0/tests/test_manager.py
-drwxrwxrwx   0        0        0        0 2023-05-27 08:31:42.667071 whatsapp-chatbot-python-0.1.0/whatsapp_chatbot_python/
--rw-rw-rw-   0        0        0      156 2023-05-27 08:01:20.000000 whatsapp-chatbot-python-0.1.0/whatsapp_chatbot_python/__init__.py
--rw-rw-rw-   0        0        0      966 2023-05-27 07:59:28.000000 whatsapp-chatbot-python-0.1.0/whatsapp_chatbot_python/bot.py
--rw-rw-rw-   0        0        0     3569 2023-05-27 07:58:05.000000 whatsapp-chatbot-python-0.1.0/whatsapp_chatbot_python/filters.py
-drwxrwxrwx   0        0        0        0 2023-05-27 08:31:42.674089 whatsapp-chatbot-python-0.1.0/whatsapp_chatbot_python/manager/
--rw-rw-rw-   0        0        0        0 2023-05-27 07:57:13.000000 whatsapp-chatbot-python-0.1.0/whatsapp_chatbot_python/manager/__init__.py
--rw-rw-rw-   0        0        0     3277 2023-05-27 07:59:28.000000 whatsapp-chatbot-python-0.1.0/whatsapp_chatbot_python/manager/handler.py
--rw-rw-rw-   0        0        0     1821 2023-05-27 07:59:28.000000 whatsapp-chatbot-python-0.1.0/whatsapp_chatbot_python/manager/observer.py
--rw-rw-rw-   0        0        0     1144 2023-05-27 07:59:28.000000 whatsapp-chatbot-python-0.1.0/whatsapp_chatbot_python/manager/router.py
-drwxrwxrwx   0        0        0        0 2023-05-27 08:31:42.671081 whatsapp-chatbot-python-0.1.0/whatsapp_chatbot_python.egg-info/
--rw-rw-rw-   0        0        0     8572 2023-05-27 08:31:42.000000 whatsapp-chatbot-python-0.1.0/whatsapp_chatbot_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      557 2023-05-27 08:31:42.000000 whatsapp-chatbot-python-0.1.0/whatsapp_chatbot_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 08:31:42.000000 whatsapp-chatbot-python-0.1.0/whatsapp_chatbot_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-05-27 08:31:42.000000 whatsapp-chatbot-python-0.1.0/whatsapp_chatbot_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-05-27 08:31:42.000000 whatsapp-chatbot-python-0.1.0/whatsapp_chatbot_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 06:13:43.795410 whatsapp-chatbot-python-0.2.0/
+-rw-rw-rw-   0        0        0    18829 2023-05-30 11:55:05.000000 whatsapp-chatbot-python-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     8648 2023-06-02 06:13:43.794407 whatsapp-chatbot-python-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7623 2023-06-01 09:39:39.000000 whatsapp-chatbot-python-0.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-02 06:13:43.795410 whatsapp-chatbot-python-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1405 2023-06-02 06:13:11.000000 whatsapp-chatbot-python-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 06:13:43.784381 whatsapp-chatbot-python-0.2.0/tests/
+-rw-rw-rw-   0        0        0     1224 2023-06-01 09:34:28.000000 whatsapp-chatbot-python-0.2.0/tests/test_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-02 06:13:43.786386 whatsapp-chatbot-python-0.2.0/whatsapp_chatbot_python/
+-rw-rw-rw-   0        0        0      184 2023-06-01 09:19:08.000000 whatsapp-chatbot-python-0.2.0/whatsapp_chatbot_python/__init__.py
+-rw-rw-rw-   0        0        0     1020 2023-06-01 09:17:35.000000 whatsapp-chatbot-python-0.2.0/whatsapp_chatbot_python/bot.py
+-rw-rw-rw-   0        0        0     3569 2023-05-30 11:55:05.000000 whatsapp-chatbot-python-0.2.0/whatsapp_chatbot_python/filters.py
+drwxrwxrwx   0        0        0        0 2023-06-02 06:13:43.793404 whatsapp-chatbot-python-0.2.0/whatsapp_chatbot_python/manager/
+-rw-rw-rw-   0        0        0        0 2023-05-30 11:55:05.000000 whatsapp-chatbot-python-0.2.0/whatsapp_chatbot_python/manager/__init__.py
+-rw-rw-rw-   0        0        0     3277 2023-05-30 11:55:05.000000 whatsapp-chatbot-python-0.2.0/whatsapp_chatbot_python/manager/handler.py
+-rw-rw-rw-   0        0        0     1821 2023-05-30 11:55:05.000000 whatsapp-chatbot-python-0.2.0/whatsapp_chatbot_python/manager/observer.py
+-rw-rw-rw-   0        0        0     1144 2023-05-30 11:55:05.000000 whatsapp-chatbot-python-0.2.0/whatsapp_chatbot_python/manager/router.py
+drwxrwxrwx   0        0        0        0 2023-06-02 06:13:43.790397 whatsapp-chatbot-python-0.2.0/whatsapp_chatbot_python.egg-info/
+-rw-rw-rw-   0        0        0     8648 2023-06-02 06:13:43.000000 whatsapp-chatbot-python-0.2.0/whatsapp_chatbot_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      557 2023-06-02 06:13:43.000000 whatsapp-chatbot-python-0.2.0/whatsapp_chatbot_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 06:13:43.000000 whatsapp-chatbot-python-0.2.0/whatsapp_chatbot_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-06-02 06:13:43.000000 whatsapp-chatbot-python-0.2.0/whatsapp_chatbot_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-06-02 06:13:43.000000 whatsapp-chatbot-python-0.2.0/whatsapp_chatbot_python.egg-info/top_level.txt
```

### Comparing `whatsapp-chatbot-python-0.1.0/LICENSE` & `whatsapp-chatbot-python-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.1.0/PKG-INFO` & `whatsapp-chatbot-python-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsapp-chatbot-python
-Version: 0.1.0
+Version: 0.2.0
 Summary: This library helps you easily create a Python chatbot with WhatsApp API.
 Home-page: https://github.com/green-api/whatsapp-chatbot-python
 Author: GREEN API
 Author-email: support@green-api.com
 License: Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -20,15 +20,18 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # whatsapp-chatbot-python
 
 ![](https://img.shields.io/badge/license-CC%20BY--ND%204.0-green)
+![](https://img.shields.io/pypi/status/whatsapp-chatbot-python)
 ![](https://img.shields.io/pypi/pyversions/whatsapp-chatbot-python)
+![](https://img.shields.io/github/actions/workflow/status/green-api/whatsapp-chatbot-python/python-package.yml)
+![](https://img.shields.io/pypi/dm/whatsapp-chatbot-python)
 
 - [Документация на русском языке](docs/README.md).
 
 whatsapp-chatbot-python is a library for integration with WhatsApp messenger using the API
 service [green-api.com](https://green-api.com/en/). You should get a registration token and an account ID in
 your [personal cabinet](https://console.green-api.com/) to use the library. There is a free developer account tariff.
 
@@ -49,32 +52,25 @@
 ```shell
 python -m pip install whatsapp-chatbot-python
 ```
 
 ## Import
 
 ```
-from whatsapp_chatbot_python import Bot, Notification
+from whatsapp_chatbot_python import GreenAPIBot, Notification
 ```
 
 ## Examples
 
 ### How to initialize an object
 
 ```
-bot = Bot("1101000001", "d75b3a66374942c5b3c019c698abc2067e151558acbd412345")
-```
-
-Note that keys can be taken from environment variables:
-
-```
-from os import environ
-
-ID_INSTANCE = environ["ID_INSTANCE"]
-API_TOKEN_INSTANCE = environ["API_TOKEN_INSTANCE"]
+bot = GreenAPIBot(
+    "1101000001", "d75b3a66374942c5b3c019c698abc2067e151558acbd412345"
+)
 ```
 
 ### How to start receiving and answering messages
 
 To start receiving messages, you must create a handler function with one parameter (`notification`). The `notification`
 parameter is the class where the notification object (`event`) and the functions to answer the message are stored. To
 send a text message in response to a notification, you need to call the `notification.answer` function and pass there
```

### Comparing `whatsapp-chatbot-python-0.1.0/README.md` & `whatsapp-chatbot-python-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # whatsapp-chatbot-python
 
 ![](https://img.shields.io/badge/license-CC%20BY--ND%204.0-green)
+![](https://img.shields.io/pypi/status/whatsapp-chatbot-python)
 ![](https://img.shields.io/pypi/pyversions/whatsapp-chatbot-python)
+![](https://img.shields.io/github/actions/workflow/status/green-api/whatsapp-chatbot-python/python-package.yml)
+![](https://img.shields.io/pypi/dm/whatsapp-chatbot-python)
 
 - [Документация на русском языке](docs/README.md).
 
 whatsapp-chatbot-python is a library for integration with WhatsApp messenger using the API
 service [green-api.com](https://green-api.com/en/). You should get a registration token and an account ID in
 your [personal cabinet](https://console.green-api.com/) to use the library. There is a free developer account tariff.
 
@@ -26,32 +29,25 @@
 ```shell
 python -m pip install whatsapp-chatbot-python
 ```
 
 ## Import
 
 ```
-from whatsapp_chatbot_python import Bot, Notification
+from whatsapp_chatbot_python import GreenAPIBot, Notification
 ```
 
 ## Examples
 
 ### How to initialize an object
 
 ```
-bot = Bot("1101000001", "d75b3a66374942c5b3c019c698abc2067e151558acbd412345")
-```
-
-Note that keys can be taken from environment variables:
-
-```
-from os import environ
-
-ID_INSTANCE = environ["ID_INSTANCE"]
-API_TOKEN_INSTANCE = environ["API_TOKEN_INSTANCE"]
+bot = GreenAPIBot(
+    "1101000001", "d75b3a66374942c5b3c019c698abc2067e151558acbd412345"
+)
 ```
 
 ### How to start receiving and answering messages
 
 To start receiving messages, you must create a handler function with one parameter (`notification`). The `notification`
 parameter is the class where the notification object (`event`) and the functions to answer the message are stored. To
 send a text message in response to a notification, you need to call the `notification.answer` function and pass there
```

### Comparing `whatsapp-chatbot-python-0.1.0/setup.py` & `whatsapp-chatbot-python-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="UTF-8") as file:
     long_description = file.read()
 
 setup(
     name="whatsapp-chatbot-python",
-    version="0.1.0",
+    version="0.2.0",
     description=(
         "This library helps you easily create"
         " a Python chatbot with WhatsApp API."
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="GREEN API",
```

### Comparing `whatsapp-chatbot-python-0.1.0/tests/test_manager.py` & `whatsapp-chatbot-python-0.2.0/tests/test_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 
-from whatsapp_chatbot_python import Bot, Notification
+from whatsapp_chatbot_python import GreenAPIBot, Notification
 
 event_example = {
     "typeWebhook": "incomingMessageReceived",
     "messageData": {
         "typeMessage": "textMessage",
         "textMessageData": {
             "textMessage": "Hello"
@@ -41,12 +41,12 @@
 
         bot.router.message.add_handler(handler)
 
         self.assertEqual(len(bot.router.message.handlers), 2)
 
     @property
     def bot(self):
-        return Bot("", "")
+        return GreenAPIBot("", "")
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `whatsapp-chatbot-python-0.1.0/whatsapp_chatbot_python/bot.py` & `whatsapp-chatbot-python-0.2.0/whatsapp_chatbot_python/bot.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,16 +23,20 @@
                 self.router.route_event(response["body"])
 
                 self.api.receiving.deleteNotification(response["receiptId"])
             except KeyboardInterrupt:
                 break
 
 
+class GreenAPIBot(Bot):
+    pass
+
+
 class GreenAPI(GreenApi):
     pass
 
 
 class GreenAPIError(Exception):
     pass
 
 
-__all__ = ["Bot", "GreenAPI", "GreenAPIError"]
+__all__ = ["Bot", "GreenAPIBot", "GreenAPI", "GreenAPIError"]
```

### Comparing `whatsapp-chatbot-python-0.1.0/whatsapp_chatbot_python/filters.py` & `whatsapp-chatbot-python-0.2.0/whatsapp_chatbot_python/filters.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.1.0/whatsapp_chatbot_python/manager/handler.py` & `whatsapp-chatbot-python-0.2.0/whatsapp_chatbot_python/manager/handler.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.1.0/whatsapp_chatbot_python/manager/observer.py` & `whatsapp-chatbot-python-0.2.0/whatsapp_chatbot_python/manager/observer.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.1.0/whatsapp_chatbot_python/manager/router.py` & `whatsapp-chatbot-python-0.2.0/whatsapp_chatbot_python/manager/router.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.1.0/whatsapp_chatbot_python.egg-info/PKG-INFO` & `whatsapp-chatbot-python-0.2.0/whatsapp_chatbot_python.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsapp-chatbot-python
-Version: 0.1.0
+Version: 0.2.0
 Summary: This library helps you easily create a Python chatbot with WhatsApp API.
 Home-page: https://github.com/green-api/whatsapp-chatbot-python
 Author: GREEN API
 Author-email: support@green-api.com
 License: Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -20,15 +20,18 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # whatsapp-chatbot-python
 
 ![](https://img.shields.io/badge/license-CC%20BY--ND%204.0-green)
+![](https://img.shields.io/pypi/status/whatsapp-chatbot-python)
 ![](https://img.shields.io/pypi/pyversions/whatsapp-chatbot-python)
+![](https://img.shields.io/github/actions/workflow/status/green-api/whatsapp-chatbot-python/python-package.yml)
+![](https://img.shields.io/pypi/dm/whatsapp-chatbot-python)
 
 - [Документация на русском языке](docs/README.md).
 
 whatsapp-chatbot-python is a library for integration with WhatsApp messenger using the API
 service [green-api.com](https://green-api.com/en/). You should get a registration token and an account ID in
 your [personal cabinet](https://console.green-api.com/) to use the library. There is a free developer account tariff.
 
@@ -49,32 +52,25 @@
 ```shell
 python -m pip install whatsapp-chatbot-python
 ```
 
 ## Import
 
 ```
-from whatsapp_chatbot_python import Bot, Notification
+from whatsapp_chatbot_python import GreenAPIBot, Notification
 ```
 
 ## Examples
 
 ### How to initialize an object
 
 ```
-bot = Bot("1101000001", "d75b3a66374942c5b3c019c698abc2067e151558acbd412345")
-```
-
-Note that keys can be taken from environment variables:
-
-```
-from os import environ
-
-ID_INSTANCE = environ["ID_INSTANCE"]
-API_TOKEN_INSTANCE = environ["API_TOKEN_INSTANCE"]
+bot = GreenAPIBot(
+    "1101000001", "d75b3a66374942c5b3c019c698abc2067e151558acbd412345"
+)
 ```
 
 ### How to start receiving and answering messages
 
 To start receiving messages, you must create a handler function with one parameter (`notification`). The `notification`
 parameter is the class where the notification object (`event`) and the functions to answer the message are stored. To
 send a text message in response to a notification, you need to call the `notification.answer` function and pass there
```

### Comparing `whatsapp-chatbot-python-0.1.0/whatsapp_chatbot_python.egg-info/SOURCES.txt` & `whatsapp-chatbot-python-0.2.0/whatsapp_chatbot_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

