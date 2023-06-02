# Comparing `tmp/ringcentral-0.7.9.tar.gz` & `tmp/ringcentral-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ringcentral-0.7.9.tar", last modified: Tue Mar 13 22:10:09 2018, max compression
+gzip compressed data, was "ringcentral-0.8.0.tar", last modified: Fri Jun  2 20:50:23 2023, max compression
```

## Comparing `ringcentral-0.7.9.tar` & `ringcentral-0.8.0.tar`

### file list

```diff
@@ -1,45 +1,51 @@
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-03-13 22:10:09.000000 ringcentral-0.7.9/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-03-13 22:10:09.000000 ringcentral-0.7.9/ringcentral/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-03-13 22:10:09.000000 ringcentral-0.7.9/ringcentral/core/
--rw-r--r--   0 travis    (2000) travis    (2000)      826 2018-03-13 22:09:26.000000 ringcentral-0.7.9/ringcentral/core/__init__.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-03-13 22:10:09.000000 ringcentral-0.7.9/ringcentral/http/
--rw-r--r--   0 travis    (2000) travis    (2000)      194 2018-03-13 22:09:26.000000 ringcentral-0.7.9/ringcentral/http/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)      695 2018-03-13 22:09:26.000000 ringcentral-0.7.9/ringcentral/http/api_exception.py
--rw-r--r--   0 travis    (2000) travis    (2000)      941 2018-03-13 22:09:26.000000 ringcentral-0.7.9/ringcentral/http/api_exception_test.py
--rw-r--r--   0 travis    (2000) travis    (2000)     3118 2018-03-13 22:09:26.000000 ringcentral-0.7.9/ringcentral/http/api_response.py
--rw-r--r--   0 travis    (2000) travis    (2000)     4690 2018-03-13 22:09:26.000000 ringcentral-0.7.9/ringcentral/http/api_response_test.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2403 2018-03-13 22:09:26.000000 ringcentral-0.7.9/ringcentral/http/client.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1279 2018-03-13 22:09:26.000000 ringcentral-0.7.9/ringcentral/http/client_test.py
--rw-r--r--   0 travis    (2000) travis    (2000)      794 2018-03-13 22:09:26.000000 ringcentral-0.7.9/ringcentral/http/json_object.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1118 2018-03-13 22:09:26.000000 ringcentral-0.7.9/ringcentral/http/multipart_builder.py
--rw-r--r--   0 travis    (2000) travis    (2000)      741 2018-03-13 22:09:26.000000 ringcentral-0.7.9/ringcentral/http/multipart_builder_test.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-03-13 22:10:09.000000 ringcentral-0.7.9/ringcentral/platform/
--rw-r--r--   0 travis    (2000) travis    (2000)       95 2018-03-13 22:09:26.000000 ringcentral-0.7.9/ringcentral/platform/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)     3491 2018-03-13 22:09:26.000000 ringcentral-0.7.9/ringcentral/platform/auth.py
--rw-r--r--   0 travis    (2000) travis    (2000)      298 2018-03-13 22:09:26.000000 ringcentral-0.7.9/ringcentral/platform/events.py
--rw-r--r--   0 travis    (2000) travis    (2000)     7037 2018-03-13 22:09:26.000000 ringcentral-0.7.9/ringcentral/platform/platform.py
--rw-r--r--   0 travis    (2000) travis    (2000)     4614 2018-03-13 22:09:26.000000 ringcentral-0.7.9/ringcentral/platform/platform_test.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-03-13 22:10:09.000000 ringcentral-0.7.9/ringcentral/subscription/
--rw-r--r--   0 travis    (2000) travis    (2000)      107 2018-03-13 22:09:26.000000 ringcentral-0.7.9/ringcentral/subscription/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)      380 2018-03-13 22:09:26.000000 ringcentral-0.7.9/ringcentral/subscription/events.py
--rw-r--r--   0 travis    (2000) travis    (2000)     6740 2018-03-13 22:09:26.000000 ringcentral-0.7.9/ringcentral/subscription/subscription.py
--rw-r--r--   0 travis    (2000) travis    (2000)     4894 2018-03-13 22:09:26.000000 ringcentral-0.7.9/ringcentral/subscription/subscription_test.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-03-13 22:10:09.000000 ringcentral-0.7.9/ringcentral/test/
--rw-r--r--   0 travis    (2000) travis    (2000)       93 2018-03-13 22:09:26.000000 ringcentral-0.7.9/ringcentral/test/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)      205 2018-03-13 22:09:26.000000 ringcentral-0.7.9/ringcentral/test/spy.py
--rw-r--r--   0 travis    (2000) travis    (2000)     4391 2018-03-13 22:09:26.000000 ringcentral-0.7.9/ringcentral/test/testcase.py
--rw-r--r--   0 travis    (2000) travis    (2000)       61 2018-03-13 22:09:26.000000 ringcentral-0.7.9/ringcentral/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)      628 2018-03-13 22:09:26.000000 ringcentral-0.7.9/ringcentral/sdk.py
--rw-r--r--   0 travis    (2000) travis    (2000)      381 2018-03-13 22:09:26.000000 ringcentral-0.7.9/ringcentral/sdk_test.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-03-13 22:10:09.000000 ringcentral-0.7.9/ringcentral.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)      471 2018-03-13 22:10:09.000000 ringcentral-0.7.9/ringcentral.egg-info/PKG-INFO
--rw-r--r--   0 travis    (2000) travis    (2000)     1077 2018-03-13 22:10:09.000000 ringcentral-0.7.9/ringcentral.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        1 2018-03-13 22:10:09.000000 ringcentral-0.7.9/ringcentral.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (2000) travis    (2000)       67 2018-03-13 22:10:09.000000 ringcentral-0.7.9/ringcentral.egg-info/requires.txt
--rw-r--r--   0 travis    (2000) travis    (2000)       12 2018-03-13 22:10:09.000000 ringcentral-0.7.9/ringcentral.egg-info/top_level.txt
--rw-r--r--   0 travis    (2000) travis    (2000)       42 2018-03-13 22:09:26.000000 ringcentral-0.7.9/MANIFEST.in
--rw-r--r--   0 travis    (2000) travis    (2000)     1405 2018-03-13 22:09:26.000000 ringcentral-0.7.9/README.md
--rw-r--r--   0 travis    (2000) travis    (2000)       66 2018-03-13 22:09:26.000000 ringcentral-0.7.9/requirements.txt
--rw-r--r--   0 travis    (2000) travis    (2000)       79 2018-03-13 22:10:09.000000 ringcentral-0.7.9/setup.cfg
--rw-r--r--   0 travis    (2000) travis    (2000)      640 2018-03-13 22:09:26.000000 ringcentral-0.7.9/setup.py
--rw-r--r--   0 travis    (2000) travis    (2000)      471 2018-03-13 22:10:09.000000 ringcentral-0.7.9/PKG-INFO
+drwxr-xr-x   0 tyler.liu   (502) staff       (20)        0 2023-06-02 20:50:23.022863 ringcentral-0.8.0/
+-rw-r--r--   0 tyler.liu   (502) staff       (20)     1088 2023-05-18 20:46:38.000000 ringcentral-0.8.0/LICENSE.md
+-rw-r--r--   0 tyler.liu   (502) staff       (20)       42 2023-05-18 20:46:38.000000 ringcentral-0.8.0/MANIFEST.in
+-rw-r--r--   0 tyler.liu   (502) staff       (20)      328 2023-06-02 20:50:23.022984 ringcentral-0.8.0/PKG-INFO
+-rw-r--r--   0 tyler.liu   (502) staff       (20)     4593 2023-06-02 17:50:12.000000 ringcentral-0.8.0/README.md
+-rw-r--r--   0 tyler.liu   (502) staff       (20)       78 2023-06-02 17:50:12.000000 ringcentral-0.8.0/requirements.txt
+drwxr-xr-x   0 tyler.liu   (502) staff       (20)        0 2023-06-02 20:50:23.005001 ringcentral-0.8.0/ringcentral/
+-rw-r--r--   0 tyler.liu   (502) staff       (20)       20 2023-05-18 22:08:54.000000 ringcentral-0.8.0/ringcentral/__init__.py
+drwxr-xr-x   0 tyler.liu   (502) staff       (20)        0 2023-06-02 20:50:23.007639 ringcentral-0.8.0/ringcentral/core/
+-rw-r--r--   0 tyler.liu   (502) staff       (20)      826 2023-05-18 20:46:38.000000 ringcentral-0.8.0/ringcentral/core/__init__.py
+drwxr-xr-x   0 tyler.liu   (502) staff       (20)        0 2023-06-02 20:50:23.009861 ringcentral-0.8.0/ringcentral/deprecated_pubnub_subscription/
+-rw-r--r--   0 tyler.liu   (502) staff       (20)       66 2023-06-02 17:50:12.000000 ringcentral-0.8.0/ringcentral/deprecated_pubnub_subscription/__init__.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)      352 2023-06-02 17:50:12.000000 ringcentral-0.8.0/ringcentral/deprecated_pubnub_subscription/events.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)     7076 2023-06-02 17:50:12.000000 ringcentral-0.8.0/ringcentral/deprecated_pubnub_subscription/subscription.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)     5017 2023-06-02 17:50:12.000000 ringcentral-0.8.0/ringcentral/deprecated_pubnub_subscription/subscription_test.py
+drwxr-xr-x   0 tyler.liu   (502) staff       (20)        0 2023-06-02 20:50:23.015456 ringcentral-0.8.0/ringcentral/http/
+-rw-r--r--   0 tyler.liu   (502) staff       (20)      153 2023-05-18 22:08:54.000000 ringcentral-0.8.0/ringcentral/http/__init__.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)      654 2023-05-18 22:08:54.000000 ringcentral-0.8.0/ringcentral/http/api_exception.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)      900 2023-05-18 22:08:54.000000 ringcentral-0.8.0/ringcentral/http/api_exception_test.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)     3118 2023-05-18 20:46:38.000000 ringcentral-0.8.0/ringcentral/http/api_response.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)     4649 2023-05-18 22:08:54.000000 ringcentral-0.8.0/ringcentral/http/api_response_test.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)     2865 2023-05-18 20:46:38.000000 ringcentral-0.8.0/ringcentral/http/client.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)     1405 2023-05-18 22:08:54.000000 ringcentral-0.8.0/ringcentral/http/client_test.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)      794 2023-05-18 20:46:38.000000 ringcentral-0.8.0/ringcentral/http/json_object.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)     1754 2023-05-18 20:46:38.000000 ringcentral-0.8.0/ringcentral/http/multipart_builder.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)     1337 2023-05-18 22:08:54.000000 ringcentral-0.8.0/ringcentral/http/multipart_builder_test.py
+drwxr-xr-x   0 tyler.liu   (502) staff       (20)        0 2023-06-02 20:50:23.018013 ringcentral-0.8.0/ringcentral/platform/
+-rw-r--r--   0 tyler.liu   (502) staff       (20)       54 2023-05-18 22:08:54.000000 ringcentral-0.8.0/ringcentral/platform/__init__.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)     3450 2023-05-18 22:08:54.000000 ringcentral-0.8.0/ringcentral/platform/auth.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)      257 2023-05-18 22:08:54.000000 ringcentral-0.8.0/ringcentral/platform/events.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)     8362 2023-06-02 17:50:12.000000 ringcentral-0.8.0/ringcentral/platform/platform.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)     5070 2023-05-18 22:08:54.000000 ringcentral-0.8.0/ringcentral/platform/platform_test.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)      861 2023-06-02 17:50:12.000000 ringcentral-0.8.0/ringcentral/sdk.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)      342 2023-05-18 22:07:52.000000 ringcentral-0.8.0/ringcentral/sdk_test.py
+drwxr-xr-x   0 tyler.liu   (502) staff       (20)        0 2023-06-02 20:50:23.020105 ringcentral-0.8.0/ringcentral/test/
+-rw-r--r--   0 tyler.liu   (502) staff       (20)       52 2023-05-18 22:08:54.000000 ringcentral-0.8.0/ringcentral/test/__init__.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)      164 2023-05-18 22:08:54.000000 ringcentral-0.8.0/ringcentral/test/spy.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)     4378 2023-05-18 22:22:44.000000 ringcentral-0.8.0/ringcentral/test/testcase.py
+drwxr-xr-x   0 tyler.liu   (502) staff       (20)        0 2023-06-02 20:50:23.022387 ringcentral-0.8.0/ringcentral/websocket/
+-rw-r--r--   0 tyler.liu   (502) staff       (20)      143 2023-06-02 17:50:12.000000 ringcentral-0.8.0/ringcentral/websocket/__init__.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)      828 2023-06-02 17:50:12.000000 ringcentral-0.8.0/ringcentral/websocket/events.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)     5406 2023-06-02 17:50:12.000000 ringcentral-0.8.0/ringcentral/websocket/web_socket_client.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)     4557 2023-06-02 17:50:12.000000 ringcentral-0.8.0/ringcentral/websocket/web_socket_subscription.py
+drwxr-xr-x   0 tyler.liu   (502) staff       (20)        0 2023-06-02 20:50:23.007255 ringcentral-0.8.0/ringcentral.egg-info/
+-rw-r--r--   0 tyler.liu   (502) staff       (20)      328 2023-06-02 20:50:22.000000 ringcentral-0.8.0/ringcentral.egg-info/PKG-INFO
+-rw-r--r--   0 tyler.liu   (502) staff       (20)     1318 2023-06-02 20:50:22.000000 ringcentral-0.8.0/ringcentral.egg-info/SOURCES.txt
+-rw-r--r--   0 tyler.liu   (502) staff       (20)        1 2023-06-02 20:50:22.000000 ringcentral-0.8.0/ringcentral.egg-info/dependency_links.txt
+-rw-r--r--   0 tyler.liu   (502) staff       (20)       79 2023-06-02 20:50:22.000000 ringcentral-0.8.0/ringcentral.egg-info/requires.txt
+-rw-r--r--   0 tyler.liu   (502) staff       (20)       12 2023-06-02 20:50:22.000000 ringcentral-0.8.0/ringcentral.egg-info/top_level.txt
+-rw-r--r--   0 tyler.liu   (502) staff       (20)       79 2023-06-02 20:50:23.023434 ringcentral-0.8.0/setup.cfg
+-rw-r--r--   0 tyler.liu   (502) staff       (20)      557 2023-06-02 17:50:12.000000 ringcentral-0.8.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ringcentral-0.7.9/ringcentral/core/__init__.py` & `ringcentral-0.8.0/ringcentral/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ringcentral-0.7.9/ringcentral/http/api_exception.py` & `ringcentral-0.8.0/ringcentral/http/api_exception.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-#!/usr/bin/env python
-# encoding: utf-8
-
 
 class ApiException(Exception):
     def __init__(self, api_response, previous=None):
         self.__apiResponse = api_response
 
         message = previous.message if previous and hasattr(previous, 'message') else 'Unknown error'
         status = 0  # previous.status if previous else 0
```

### Comparing `ringcentral-0.7.9/ringcentral/http/api_exception_test.py` & `ringcentral-0.8.0/ringcentral/http/api_exception_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-#!/usr/bin/env python
-# encoding: utf-8
-
 import unittest
 
 from ..test import TestCase
 from .api_response import ApiResponse
 from .api_response_test import create_response
 from .api_exception import ApiException
```

### Comparing `ringcentral-0.7.9/ringcentral/http/api_response.py` & `ringcentral-0.8.0/ringcentral/http/api_response.py`

 * *Files identical despite different names*

### Comparing `ringcentral-0.7.9/ringcentral/http/api_response_test.py` & `ringcentral-0.8.0/ringcentral/http/api_response_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-#!/usr/bin/env python
-# encoding: utf-8
-
 import unittest
 
 from ..test import TestCase
 from ..core import is_third
 from .api_response import ApiResponse
 from requests import Response
```

### Comparing `ringcentral-0.7.9/ringcentral/http/client.py` & `ringcentral-0.8.0/ringcentral/http/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,15 +13,18 @@
     def __init__(self):
         pass
 
     def send(self, request):
         response = None
 
         try:
-            response = self.load_response(request.prepare())
+            prepared = request
+            if isinstance(prepared, requests.models.Request): # not a prepared request
+                prepared = request.prepare()
+            response = self.load_response(prepared)
 
             if response.ok():
                 return response
             else:
                 response.response().raise_for_status()
 
         except Exception as e:
@@ -53,39 +56,44 @@
         :param query_params:
         :param body:
         :param headers:
         :return:requests.Request
         """
 
         if query_params:
-            query = urlencode(query_params)
+            if type(query_params) is dict:
+                query = ""
+                for key, value in  iter(query_params.items()):
+                    if type(value) is list:
+                        for k in value:
+                            query += ("%s=%s&" % (key, k))
+                    else:
+                        query += ("%s=%s&" % (key, value))
+                query = query[:-1]
+            else:
+                query = urlencode(query_params)
             if query:
                 url = url + ('&' if url.find('?') > 0 else '?') + query
 
         content_type = None
-        accept = None
-
+        
         if headers is None:
             headers = {}
 
         it = iterator(headers)
 
         for key, value in it:
             if key.lower().find('content-type') >= 0:
                 content_type = value
             if key.lower().find('accept') >= 0:
-                accept = value
+                headers['Accept'] = value
 
         if content_type is None:
             content_type = 'application/json'
             headers['Content-Type'] = content_type
 
-        if accept is None:
-            accept = 'application/json'
-            headers['Accept'] = accept
-
         if content_type.lower().find('application/json') >= 0:
             body = json.dumps(body) if body else None
         elif content_type.lower().find('application/x-www-form-urlencoded') >= 0:
             body = urlencode(body) if body else None
 
         return requests.Request(method, url, headers=headers, data=body)
```

### Comparing `ringcentral-0.7.9/ringcentral/http/client_test.py` & `ringcentral-0.8.0/ringcentral/http/client_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-#!/usr/bin/env python
-# encoding: utf-8
-
 import unittest
 
 from ..test import TestCase
 from .client import Client
 
 body = {'foo': 'bar', 'baz': 'qux'}
 
 
 class TestClient(TestCase):
     def test_create_request_with_query_string(self):
         req = Client().create_request(url='http://whatever', query_params={'foo': 'bar', 'baz': 'qux'})
         self.assertEqual('http://whatever?foo=bar&baz=qux', req.url)
 
+        req = Client().create_request(url='http://whatever', query_params={'a2z':['abc','xyz']})
+        self.assertEqual('http://whatever?a2z=abc&a2z=xyz', req.url)
+
     def test_create_request_encode_body_url(self):
         r = Client().create_request(body=body, headers={'Content-Type': 'application/x-www-form-urlencoded'})
         self.assertEqual('foo=bar&baz=qux', r.data)
 
     def test_create_request_encode_body_json(self):
         r = Client().create_request(body=body, headers={'Content-Type': 'application/json'})
         self.assertEqual('{"foo": "bar", "baz": "qux"}', r.data)
```

### Comparing `ringcentral-0.7.9/ringcentral/http/json_object.py` & `ringcentral-0.8.0/ringcentral/http/json_object.py`

 * *Files identical despite different names*

### Comparing `ringcentral-0.7.9/ringcentral/platform/auth.py` & `ringcentral-0.8.0/ringcentral/platform/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-#!/usr/bin/env python
-# encoding: utf-8
-
 from time import time
 
 RELEASE_TIMEOUT = 10
 
 
 class Auth:
     def __init__(self):
```

### Comparing `ringcentral-0.7.9/ringcentral/platform/platform.py` & `ringcentral-0.8.0/ringcentral/platform/platform.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,36 @@
-#!/usr/bin/env python
-# encoding: utf-8
-
 import sys
+try:
+    from urllib.parse import urlparse
+except ImportError:
+    from urlparse import urlparse
 from observable import Observable
 from functools import reduce
 from .auth import Auth
 from .events import Events
 from ..core import base64encode
+import warnings
 
 ACCOUNT_ID = '~'
 ACCOUNT_PREFIX = '/account/'
 URL_PREFIX = '/restapi'
 TOKEN_ENDPOINT = '/restapi/oauth/token'
 REVOKE_ENDPOINT = '/restapi/oauth/revoke'
+AUTHORIZE_ENDPOINT = '/restapi/oauth/authorize'
 API_VERSION = 'v1.0'
 ACCESS_TOKEN_TTL = 3600  # 60 minutes
 REFRESH_TOKEN_TTL = 604800  # 1 week
 KNOWN_PREFIXES = [
     URL_PREFIX,
     '/rcvideo',
+    '/video',
+    '/webinar',
+    '/analytics',
+    '/ai',
+    '/team-messaging',
     '/scim'
 ]
 
 
 class Platform(Observable):
     def __init__(self, client, key='', secret='', server='', name='', version='', redirect_uri='',
                  known_prefixes=None):
@@ -45,15 +53,15 @@
                           'RCPYTHONSDK/VERSION'
 
     def auth(self):
         return self._auth
 
     def create_url(self, url, add_server=False, add_method=None, add_token=False):
         built_url = ''
-        has_http = url.find('http://') >= 0 or url.find('https://') >= 0
+        has_http = url.startswith('http://') or url.startswith('https://')
 
         if add_server and not has_http:
             built_url += self._server
 
         if not reduce(lambda res, prefix: res if res else url.find(prefix) == 0, self._known_prefixes, False) and not has_http:
             built_url += URL_PREFIX + '/' + API_VERSION
 
@@ -72,35 +80,55 @@
 
     def logged_in(self):
         try:
             return self._auth.access_token_valid() or self.refresh()
         except:
             return False
 
-    def login(self, username='', extension='', password='', code='', redirect_uri=''):
+    def login_url(self, redirect_uri, state='', challenge='', challenge_method='S256'):
+        built_url = self.create_url( AUTHORIZE_ENDPOINT, add_server=True )
+        built_url += '?response_type=code&client_id=' + self._key + '&redirect_uri=' + urllib.parse.quote(redirect_uri)
+        if state:
+            built_url += '&state=' + urllib.parse.quote(state)
+        if challenge:
+            built_url += '&code_challenge=' + urllib.parse.quote(challenge) + '&code_challenge_method=' + challenge_method
+        return built_url
+        
+    def login(self, username='', extension='', password='', code='', redirect_uri='', jwt='', verifier=''):
         try:
-            if not code and not username and not password:
-                raise Exception('Either code or username with password has to be provided')
-
-            if not code:
+            if not code and not username and not password and not jwt:
+                raise Exception('Either code, or username with password, or jwt has to be provided')
+            if username and password:
+                warnings.warn("username-password login will soon be deprecated. Please use jwt or OAuth instead.")
+            if not code and not jwt:
                 body = {
                     'grant_type': 'password',
                     'username': username,
-                    'extension': extension,
                     'password': password,
                     'access_token_ttl': ACCESS_TOKEN_TTL,
                     'refresh_token_ttl': REFRESH_TOKEN_TTL
                 }
+                if extension:
+                    body['extension'] = extension
+            elif jwt:
+                body = {
+                    'grant_type': 'urn:ietf:params:oauth:grant-type:jwt-bearer',
+                    'assertion': jwt
+                }
             else:
                 body = {
                     'grant_type': 'authorization_code',
                     'redirect_uri': redirect_uri if redirect_uri else self._redirect_uri,
                     'code': code
                 }
-            response = self._request_token(TOKEN_ENDPOINT, body=body)
+                if verifier:
+                    body['code_verifier'] = verifier
+
+            built_url = self.create_url( TOKEN_ENDPOINT, add_server=True )
+            response = self._request_token( built_url, body=body)
             self._auth.set_data(response.json_dict())
             self.trigger(Events.loginSuccess, response)
             return response
         except Exception as e:
             self.trigger(Events.loginError, e)
             raise e
 
@@ -135,15 +163,15 @@
 
     def inflate_request(self, request, skip_auth_check=False):
         if not skip_auth_check:
             self._ensure_authentication()
             request.headers['Authorization'] = self._auth_header()
 
         request.headers['User-Agent'] = self._userAgent
-        request.headers['RC-User-Agent'] = self._userAgent
+        request.headers['X-User-Agent'] = self._userAgent
         request.url = self.create_url(request.url, add_server=True)
 
         return request
 
     def send_request(self, request, skip_auth_check=False):
         return self._client.send(self.inflate_request(request, skip_auth_check=skip_auth_check))
```

### Comparing `ringcentral-0.7.9/ringcentral/platform/platform_test.py` & `ringcentral-0.8.0/ringcentral/platform/platform_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-#!/usr/bin/env python
-# encoding: utf-8
-
 import sys
 import unittest
 import requests_mock
 
 from ..test import TestCase
 
 
@@ -22,18 +19,28 @@
         sdk = self.get_sdk(mock)
         self.logout_mock(mock)
         sdk.platform().logout()
         self.authentication_mock(mock)
         sdk.platform().login(code='foo')
         text = str(mock.request_history[-1].text)
         if sys.version_info[0] == 3:
-            self.assertEqual(text, 'grant_type=authorization_code&redirect_uri=mock%3A%2F%2Fwhatever-redirect&code=foo')
+            self.assertEqual(text, 'grant_type=authorization_code&redirect_uri=https%3A%2F%2Fwhatever-redirect&code=foo')
         else:
-            self.assertEqual(text, 'code=foo&grant_type=authorization_code&redirect_uri=mock%3A%2F%2Fwhatever-redirect')
+            self.assertEqual(text, 'code=foo&grant_type=authorization_code&redirect_uri=https%3A%2F%2Fwhatever-redirect')
 
+    def test_login_fail(self, mock):
+        sdk = self.get_sdk(mock)
+        self.logout_mock(mock)
+        sdk.platform().logout()
+        self.authentication_mock(mock)
+        try:
+            sdk.platform().login()
+        except Exception as e:
+            self.assertTrue( e )
+            
     def test_login_code_redirect(self, mock):
         sdk = self.get_sdk(mock)
         self.logout_mock(mock)
         sdk.platform().logout()
         self.authentication_mock(mock)
         sdk.platform().login(code='foo', redirect_uri='bar')
         text = str(mock.request_history[-1].text)
@@ -109,26 +116,31 @@
         self.assertEqual('', sdk.platform().auth().data()['access_token'])
         self.assertEqual('', sdk.platform().auth().data()['refresh_token'])
         self.assertFalse(sdk.platform().logged_in())
 
     def test_api_url(self, mock):
         sdk = self.get_sdk(mock)
 
-        exp1 = 'mock://whatever/restapi/v1.0/account/~/extension/~?_method=POST&access_token=ACCESS_TOKEN'
+        exp1 = 'https://whatever/restapi/v1.0/account/~/extension/~?_method=POST&access_token=ACCESS_TOKEN'
         act1 = sdk.platform().create_url('/account/~/extension/~', add_server=True, add_method='POST', add_token=True)
         self.assertEqual(exp1, act1)
 
         exp2 = 'https://foo/account/~/extension/~?_method=POST&access_token=ACCESS_TOKEN'
         url2 = 'https://foo/account/~/extension/~'
         act2 = sdk.platform().create_url(url2, add_server=True, add_method='POST', add_token=True)
         self.assertEqual(exp2, act2)
 
     def test_api_url_custom_prefixes(self, mock):
         sdk = self.get_sdk(mock)
-        exp = 'mock://whatever/scim/v2/foo'
+        exp = 'https://whatever/scim/v2/foo'
         url = '/scim/v2/foo'
         act = sdk.platform().create_url(url, add_server=True)
         self.assertEqual(exp, act)
 
+        exp = 'https://whatever/analytics/phone/foo'
+        url = '/analytics/phone/foo'
+        act = sdk.platform().create_url(url, add_server=True)
+        self.assertEqual(exp, act)
+        
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ringcentral-0.7.9/ringcentral/subscription/subscription.py` & `ringcentral-0.8.0/ringcentral/deprecated_pubnub_subscription/subscription.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,219 +1,220 @@
-#!/usr/bin/env python
-# encoding: utf-8
-import json
-import base64
-from threading import Timer
-from observable import Observable
-from .events import Events
-from ..core import tostr, clean_decrypted
-
-RENEW_HANDICAP = 60
-
-
-class Subscription(Observable):
-    def __init__(self, platform):
-        Observable.__init__(self)
-        self._platform = platform
-        self._event_filters = []
-        self._timeout = None
-        self._subscription = {
-            'eventFilters': [],
-            'expirationTime': '',  # 2014-03-12T19:54:35.613Z
-            'expiresIn': 0,
-            'deliveryMode': {
-                'transportType': 'PubNub',
-                'encryption': False,
-                'address': '',
-                'subscriberKey': '',
-                'secretKey': ''
-            },
-            'id': '',
-            'creationTime': '',  # 2014-03-12T19:54:35.613Z
-            'status': '',  # Active
-            'uri': ''
-        }
-        self._pubnub = None
-
-    def pubnub(self):
-        return self._pubnub
-
-    def register(self, events=None):
-        if self.alive():
-            return self.renew(events=events)
-        else:
-            return self.subscribe(events=events)
-
-    def add_events(self, events):
-        self._event_filters += events
-        pass
-
-    def set_events(self, events):
-        self._event_filters = events
-
-    def subscribe(self, events=None):
-
-        if events:
-            self.set_events(events)
-
-        if not self._event_filters or len(self._event_filters) == 0:
-            raise Exception('Events are undefined')
-
-        try:
-            response = self._platform.post('/restapi/v1.0/subscription', body={
-                'eventFilters': self._get_full_events_filter(),
-                'deliveryMode': {
-                    'transportType': 'PubNub'
-                }
-            })
-
-            self.set_subscription(response.json_dict())
-            self._subscribe_at_pubnub()
-            self.trigger(Events.subscribeSuccess, response)
-
-            return response
-
-        except Exception as e:
-            self.reset()
-            self.trigger(Events.subscribeError, e)
-            raise
-
-    def renew(self, events=None):
-
-        if events:
-            self.set_events(events)
-
-        if not self.alive():
-            raise Exception('Subscription is not alive')
-
-        if not self._event_filters or len(self._event_filters) == 0:
-            raise Exception('Events are undefined')
-
-        self._clear_timeout()
-
-        try:
-            response = self._platform.put('/restapi/v1.0/subscription/' + self._subscription['id'], body={
-                'eventFilters': self._get_full_events_filter()
-            })
-
-            self.set_subscription(response.json_dict())
-            self.trigger(Events.renewSuccess, response)
-
-            return response
-
-        except Exception as e:
-            self.reset()
-            self.trigger(Events.renewError, e)
-            raise
-
-    def remove(self):
-        if not self.alive():
-            raise Exception('Subscription is not alive')
-
-        try:
-            response = self._platform.delete('/restapi/v1.0/subscription/' + self._subscription['id'])
-
-            self.reset()
-            self.trigger(Events.removeSuccess, response)
-
-            return response
-
-        except Exception as e:
-            self.reset()
-            self.trigger(Events.removeError, e)
-            raise
-
-    def alive(self):
-        s = self._subscription
-        return s and \
-               ('deliveryMode' in s and s['deliveryMode']) and \
-               ('subscriberKey' in s['deliveryMode'] and s['deliveryMode']['subscriberKey']) and \
-               ('address' in s['deliveryMode'] and s['deliveryMode']['address'])
-
-    def subscription(self):
-        return self._subscription
-
-    def set_subscription(self, data):
-        self._clear_timeout()
-        self._subscription = data
-        self._set_timeout()
-
-    def reset(self):
-        self._clear_timeout()
-        self._unsubscribe_at_pubnub()
-        self._subscription = None
-
-    def destroy(self):
-        self.reset()
-        self.off()
-
-    def _subscribe_at_pubnub(self):
-        if not self.alive():
-            raise Exception('Subscription is not alive')
-
-        from pubnub.pubnub import PubNub
-        from pubnub.pnconfiguration import PNConfiguration
-        from pubnub.callbacks import SubscribeCallback
-        from pubnub.enums import PNStatusCategory
-
-        pnconf = PNConfiguration()
-        pnconf.subscribe_key = self._subscription['deliveryMode']['subscriberKey']
-        self._pubnub = PubNub(pnconf)
-
-        subscription = self
-
-        class SubscribeCallbackImpl(SubscribeCallback):
-            def presence(self, pubnub, presence):
-                pass  # handle incoming presence data
-
-            def status(self, pubnub, status):
-                if status.category == PNStatusCategory.PNUnexpectedDisconnectCategory:
-                    subscription.trigger(Events.connectionError, 'Connectivity loss')
-                    pass
-
-            def message(self, pubnub, pnmessage):  # instance of PNMessageResult
-                subscription._notify(pnmessage.message)
-
-        self._pubnub.add_listener(SubscribeCallbackImpl())
-        self._pubnub.subscribe().channels(self._subscription['deliveryMode']['address']).execute()
-
-    def _notify(self, message):
-        message = self._decrypt(message)
-        self.trigger(Events.notification, message)
-
-    def _decrypt(self, message):
-        if not self.alive():
-            raise Exception('Subscription is not alive')
-
-        from Crypto.Cipher import AES
-
-        delivery_mode = self._subscription['deliveryMode']
-        is_encrypted = ('encryption' in delivery_mode) and ('encryptionKey' in delivery_mode)
-
-        if is_encrypted:
-            key = base64.b64decode(self._subscription['deliveryMode']['encryptionKey'])
-            data = base64.b64decode(message)
-            cipher = AES.new(key, AES.MODE_ECB)
-            decrypted = clean_decrypted(tostr(cipher.decrypt(data)))
-            message = json.loads(decrypted)
-
-        return message
-
-    def _unsubscribe_at_pubnub(self):
-        if self._pubnub and self.alive():
-            self._pubnub.unsubscribe().channels(self._subscription['deliveryMode']['address']).execute()
-
-    def _get_full_events_filter(self):
-        return [self._platform.create_url(e) for e in self._event_filters]
-
-    def _set_timeout(self):
-        time_to_expiration = self._subscription['expiresIn'] - RENEW_HANDICAP
-        self._timeout = Timer(time_to_expiration, self.renew)
-        self._timeout.start()
-
-    def _clear_timeout(self):
-        if self._timeout:
-            self._timeout.cancel()
-
-
-if __name__ == '__main__':
-    pass
+#!/usr/bin/env python
+# encoding: utf-8
+import json
+import base64
+from threading import Timer
+from observable import Observable
+from .events import Events
+from ..core import tostr, clean_decrypted
+
+RENEW_HANDICAP = 60
+stripped = lambda s: ''.join([c for c in s if ord(c) > 31 or ord(c) == 9])
+
+class Subscription(Observable):
+    def __init__(self, platform):
+        Observable.__init__(self)
+        self._platform = platform
+        self._event_filters = []
+        self._timeout = None
+        self._subscription = {
+            'eventFilters': [],
+            'expirationTime': '',  # 2014-03-12T19:54:35.613Z
+            'expiresIn': 0,
+            'deliveryMode': {
+                'transportType': 'PubNub',
+                'encryption': False,
+                'address': '',
+                'subscriberKey': '',
+                'secretKey': ''
+            },
+            'id': '',
+            'creationTime': '',  # 2014-03-12T19:54:35.613Z
+            'status': '',  # Active
+            'uri': ''
+        }
+        self._pubnub = None
+
+    def pubnub(self):
+        return self._pubnub
+
+    def register(self, events=None):
+        if self.alive():
+            return self.renew(events=events)
+        else:
+            return self.subscribe(events=events)
+
+    def add_events(self, events):
+        self._event_filters += events
+        pass
+
+    def set_events(self, events):
+        self._event_filters = events
+
+    def subscribe(self, events=None):
+
+        if events:
+            self.set_events(events)
+
+        if not self._event_filters or len(self._event_filters) == 0:
+            raise Exception('Events are undefined')
+
+        try:
+            response = self._platform.post('/restapi/v1.0/subscription', body={
+                'eventFilters': self._get_full_events_filter(),
+                'deliveryMode': {
+                    'transportType': 'PubNub'
+                }
+            })
+
+            self.set_subscription(response.json_dict())
+            self._subscribe_at_pubnub()
+            self.trigger(Events.subscribeSuccess, response)
+
+            return response
+
+        except Exception as e:
+            self.reset()
+            self.trigger(Events.subscribeError, e)
+            raise
+
+    def renew(self, events=None):
+
+        if events:
+            self.set_events(events)
+
+        if not self.alive():
+            raise Exception('Subscription is not alive')
+
+        if not self._event_filters or len(self._event_filters) == 0:
+            raise Exception('Events are undefined')
+
+        self._clear_timeout()
+
+        try:
+            response = self._platform.put('/restapi/v1.0/subscription/' + self._subscription['id'], body={
+                'eventFilters': self._get_full_events_filter()
+            })
+
+            self.set_subscription(response.json_dict())
+            self.trigger(Events.renewSuccess, response)
+
+            return response
+
+        except Exception as e:
+            self.reset()
+            self.trigger(Events.renewError, e)
+            raise
+
+    def remove(self):
+        if not self.alive():
+            raise Exception('Subscription is not alive')
+
+        try:
+            response = self._platform.delete('/restapi/v1.0/subscription/' + self._subscription['id'])
+
+            self.reset()
+            self.trigger(Events.removeSuccess, response)
+
+            return response
+
+        except Exception as e:
+            self.reset()
+            self.trigger(Events.removeError, e)
+            raise
+
+    def alive(self):
+        s = self._subscription
+        return s and \
+               ('deliveryMode' in s and s['deliveryMode']) and \
+               ('subscriberKey' in s['deliveryMode'] and s['deliveryMode']['subscriberKey']) and \
+               ('address' in s['deliveryMode'] and s['deliveryMode']['address'])
+
+    def subscription(self):
+        return self._subscription
+
+    def set_subscription(self, data):
+        self._clear_timeout()
+        self._subscription = data
+        self._set_timeout()
+
+    def reset(self):
+        self._clear_timeout()
+        self._unsubscribe_at_pubnub()
+        self._subscription = None
+
+    def destroy(self):
+        self.reset()
+        self.off()
+
+    def _subscribe_at_pubnub(self):
+        if not self.alive():
+            raise Exception('Subscription is not alive')
+
+        from pubnub.pubnub import PubNub
+        from pubnub.pnconfiguration import PNConfiguration
+        from pubnub.callbacks import SubscribeCallback
+        from pubnub.enums import PNStatusCategory
+
+        pnconf = PNConfiguration()
+        pnconf.subscribe_key = self._subscription['deliveryMode']['subscriberKey']
+        self._pubnub = PubNub(pnconf)
+
+        subscription = self
+
+        class SubscribeCallbackImpl(SubscribeCallback):
+            def presence(self, pubnub, presence):
+                pass  # handle incoming presence data
+
+            def status(self, pubnub, status):
+                if status.category == PNStatusCategory.PNUnexpectedDisconnectCategory:
+                    subscription.trigger(Events.connectionError, 'Connectivity loss')
+                    pass
+
+            def message(self, pubnub, pnmessage):  # instance of PNMessageResult
+                subscription._notify(pnmessage.message)
+
+        self._pubnub.add_listener(SubscribeCallbackImpl())
+        self._pubnub.subscribe().channels(self._subscription['deliveryMode']['address']).execute()
+
+    def _notify(self, message):
+        message = self._decrypt(message)
+        self.trigger(Events.notification, message)
+
+    def _decrypt(self, message):
+        if not self.alive():
+            raise Exception('Subscription is not alive')
+
+        from Crypto.Cipher import AES
+
+        delivery_mode = self._subscription['deliveryMode']
+        is_encrypted = ('encryption' in delivery_mode) and ('encryptionKey' in delivery_mode)
+
+        if is_encrypted:
+            key = base64.b64decode(self._subscription['deliveryMode']['encryptionKey'])
+            data = base64.b64decode(message)
+            cipher = AES.new(key, AES.MODE_ECB)
+            decrypted = clean_decrypted(tostr(cipher.decrypt(data)))
+            message = stripped(decrypted)
+            message = json.loads(decrypted)
+
+        return message
+
+    def _unsubscribe_at_pubnub(self):
+        if self._pubnub and self.alive():
+            self._pubnub.unsubscribe().channels(self._subscription['deliveryMode']['address']).execute()
+
+    def _get_full_events_filter(self):
+        return [self._platform.create_url(e) for e in self._event_filters]
+
+    def _set_timeout(self):
+        time_to_expiration = self._subscription['expiresIn'] - RENEW_HANDICAP
+        self._timeout = Timer(time_to_expiration, self.renew)
+        self._timeout.start()
+
+    def _clear_timeout(self):
+        if self._timeout:
+            self._timeout.cancel()
+
+
+if __name__ == '__main__':
+    pass
```

### Comparing `ringcentral-0.7.9/ringcentral/test/testcase.py` & `ringcentral-0.8.0/ringcentral/test/testcase.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-#!/usr/bin/env python
-# encoding: utf-8
-
 import unittest
 import requests_mock
 import json
 import re
 from time import time
 from datetime import date
 from .. import SDK
@@ -14,15 +11,15 @@
 
 class TestCase(unittest.TestCase):
     def __init__(self, method_name=None):
         unittest.TestCase.__init__(self, method_name)
 
     def get_sdk(self, mock):
 
-        sdk = SDK('whatever', 'whatever', 'mock://whatever', redirect_uri='mock://whatever-redirect')
+        sdk = SDK('whatever', 'whatever', 'https://whatever', redirect_uri='https://whatever-redirect')
 
         self.authentication_mock(mock)
         sdk.platform().login('18881112233', None, 'password')
 
         matcher = re.compile('pubsub\.pubnub\.com')
 
         mock.register_uri(
@@ -40,16 +37,16 @@
         )
 
         return sdk
 
     def add(self, mock, method, url, body, status=200):
         mock.register_uri(
             method=method,
-            url='mock://whatever' + url,
-            text=json.dumps(body),
+            url='https://whatever' + url,
+            text= '' if body is None else json.dumps(body),
             headers={'Content-Type': 'application/json'},
             status_code=status
         )
 
     def authentication_mock(self, mock):
         return self.add(mock, 'POST', '/restapi/oauth/token', {
             'access_token': 'ACCESS_TOKEN',
```

### Comparing `ringcentral-0.7.9/ringcentral.egg-info/SOURCES.txt` & `ringcentral-0.8.0/ringcentral.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,26 @@
+LICENSE.md
 MANIFEST.in
 README.md
 requirements.txt
 setup.cfg
 setup.py
 ringcentral/__init__.py
 ringcentral/sdk.py
 ringcentral/sdk_test.py
 ringcentral.egg-info/PKG-INFO
 ringcentral.egg-info/SOURCES.txt
 ringcentral.egg-info/dependency_links.txt
 ringcentral.egg-info/requires.txt
 ringcentral.egg-info/top_level.txt
 ringcentral/core/__init__.py
+ringcentral/deprecated_pubnub_subscription/__init__.py
+ringcentral/deprecated_pubnub_subscription/events.py
+ringcentral/deprecated_pubnub_subscription/subscription.py
+ringcentral/deprecated_pubnub_subscription/subscription_test.py
 ringcentral/http/__init__.py
 ringcentral/http/api_exception.py
 ringcentral/http/api_exception_test.py
 ringcentral/http/api_response.py
 ringcentral/http/api_response_test.py
 ringcentral/http/client.py
 ringcentral/http/client_test.py
@@ -23,14 +28,14 @@
 ringcentral/http/multipart_builder.py
 ringcentral/http/multipart_builder_test.py
 ringcentral/platform/__init__.py
 ringcentral/platform/auth.py
 ringcentral/platform/events.py
 ringcentral/platform/platform.py
 ringcentral/platform/platform_test.py
-ringcentral/subscription/__init__.py
-ringcentral/subscription/events.py
-ringcentral/subscription/subscription.py
-ringcentral/subscription/subscription_test.py
 ringcentral/test/__init__.py
 ringcentral/test/spy.py
-ringcentral/test/testcase.py
+ringcentral/test/testcase.py
+ringcentral/websocket/__init__.py
+ringcentral/websocket/events.py
+ringcentral/websocket/web_socket_client.py
+ringcentral/websocket/web_socket_subscription.py
```

### Comparing `ringcentral-0.7.9/setup.py` & `ringcentral-0.8.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.7.9'
+VERSION = '0.8.0'
 
 setup(
     name='ringcentral',
     packages=find_packages(exclude=[]),
     version=VERSION,
-    description='RingCentral Connect Platform Python SDK',
-    author='Kirill Konshin @ RingCentral, Inc.',
-    author_email='devsupport@ringcentral.com',
+    description='RingCentral Python SDK',
+    author='Kirill Konshin',
     url='https://github.com/ringcentral/ringcentral-python',
     download_url='https://github.com/ringcentral/ringcentral-python/tarball/%s' % VERSION,
     keywords=['sdk', 'ringcentral', 'connect', 'platform', 'api', 'python'],
     install_requires=[i.strip() for i in open('requirements.txt').readlines()],
     classifiers=[]
-)
+)
```

