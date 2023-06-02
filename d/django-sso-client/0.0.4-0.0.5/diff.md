# Comparing `tmp/django-sso-client-0.0.4.tar.gz` & `tmp/django-sso-client-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-sso-client-0.0.4.tar", last modified: Fri Jun  2 18:09:55 2023, max compression
+gzip compressed data, was "django-sso-client-0.0.5.tar", last modified: Fri Jun  2 19:08:19 2023, max compression
```

## Comparing `django-sso-client-0.0.4.tar` & `django-sso-client-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-02 18:09:55.512978 django-sso-client-0.0.4/
--rw-rw-r--   0 israel    (1000) israel    (1000)       38 2023-06-01 22:36:35.000000 django-sso-client-0.0.4/LICENSE.txt
--rw-rw-r--   0 israel    (1000) israel    (1000)      961 2023-06-02 18:09:55.516978 django-sso-client-0.0.4/PKG-INFO
--rw-rw-r--   0 israel    (1000) israel    (1000)      397 2023-06-01 22:45:46.000000 django-sso-client-0.0.4/README.md
-drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-02 18:09:55.512978 django-sso-client-0.0.4/django_client_sso/
--rw-rw-r--   0 israel    (1000) israel    (1000)       31 2023-06-02 17:02:09.000000 django-sso-client-0.0.4/django_client_sso/__init__.py
--rw-rw-r--   0 israel    (1000) israel    (1000)     1621 2023-06-02 18:08:25.000000 django-sso-client-0.0.4/django_client_sso/client_base.py
--rw-rw-r--   0 israel    (1000) israel    (1000)      319 2023-06-02 17:13:57.000000 django-sso-client-0.0.4/django_client_sso/client_office365.py
--rw-rw-r--   0 israel    (1000) israel    (1000)     1929 2023-06-02 18:09:01.000000 django-sso-client-0.0.4/django_client_sso/decorators.py
-drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-02 18:09:55.512978 django-sso-client-0.0.4/django_sso_client.egg-info/
--rw-rw-r--   0 israel    (1000) israel    (1000)      961 2023-06-02 18:09:55.000000 django-sso-client-0.0.4/django_sso_client.egg-info/PKG-INFO
--rw-rw-r--   0 israel    (1000) israel    (1000)      337 2023-06-02 18:09:55.000000 django-sso-client-0.0.4/django_sso_client.egg-info/SOURCES.txt
--rw-rw-r--   0 israel    (1000) israel    (1000)        1 2023-06-02 18:09:55.000000 django-sso-client-0.0.4/django_sso_client.egg-info/dependency_links.txt
--rw-rw-r--   0 israel    (1000) israel    (1000)       18 2023-06-02 18:09:55.000000 django-sso-client-0.0.4/django_sso_client.egg-info/top_level.txt
--rw-rw-r--   0 israel    (1000) israel    (1000)      106 2023-06-02 18:09:55.516978 django-sso-client-0.0.4/setup.cfg
--rw-rw-r--   0 israel    (1000) israel    (1000)     1079 2023-06-02 18:09:48.000000 django-sso-client-0.0.4/setup.py
+drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-02 19:08:19.380240 django-sso-client-0.0.5/
+-rw-rw-r--   0 israel    (1000) israel    (1000)       38 2023-06-01 22:36:35.000000 django-sso-client-0.0.5/LICENSE.txt
+-rw-rw-r--   0 israel    (1000) israel    (1000)      961 2023-06-02 19:08:19.384240 django-sso-client-0.0.5/PKG-INFO
+-rw-rw-r--   0 israel    (1000) israel    (1000)      397 2023-06-01 22:45:46.000000 django-sso-client-0.0.5/README.md
+drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-02 19:08:19.380240 django-sso-client-0.0.5/django_client_sso/
+-rw-rw-r--   0 israel    (1000) israel    (1000)       31 2023-06-02 17:02:09.000000 django-sso-client-0.0.5/django_client_sso/__init__.py
+-rw-rw-r--   0 israel    (1000) israel    (1000)     1741 2023-06-02 19:03:13.000000 django-sso-client-0.0.5/django_client_sso/client_base.py
+-rw-rw-r--   0 israel    (1000) israel    (1000)      319 2023-06-02 17:13:57.000000 django-sso-client-0.0.5/django_client_sso/client_office365.py
+-rw-rw-r--   0 israel    (1000) israel    (1000)      699 2023-06-02 19:00:45.000000 django-sso-client-0.0.5/django_client_sso/custom_exception_handler.py
+-rw-rw-r--   0 israel    (1000) israel    (1000)     1591 2023-06-02 19:06:53.000000 django-sso-client-0.0.5/django_client_sso/decorators.py
+-rw-rw-r--   0 israel    (1000) israel    (1000)      369 2023-06-02 19:05:40.000000 django-sso-client-0.0.5/django_client_sso/exceptions.py
+drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-02 19:08:19.380240 django-sso-client-0.0.5/django_sso_client.egg-info/
+-rw-rw-r--   0 israel    (1000) israel    (1000)      961 2023-06-02 19:08:19.000000 django-sso-client-0.0.5/django_sso_client.egg-info/PKG-INFO
+-rw-rw-r--   0 israel    (1000) israel    (1000)      415 2023-06-02 19:08:19.000000 django-sso-client-0.0.5/django_sso_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 israel    (1000) israel    (1000)        1 2023-06-02 19:08:19.000000 django-sso-client-0.0.5/django_sso_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 israel    (1000) israel    (1000)       18 2023-06-02 19:08:19.000000 django-sso-client-0.0.5/django_sso_client.egg-info/top_level.txt
+-rw-rw-r--   0 israel    (1000) israel    (1000)      106 2023-06-02 19:08:19.384240 django-sso-client-0.0.5/setup.cfg
+-rw-rw-r--   0 israel    (1000) israel    (1000)     1079 2023-06-02 19:08:09.000000 django-sso-client-0.0.5/setup.py
```

### Comparing `django-sso-client-0.0.4/PKG-INFO` & `django-sso-client-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sso-client
-Version: 0.0.4
+Version: 0.0.5
 Summary: Client for Django Apps - SSO TIT/Hyper by P&D
 Home-page: https://TITBrasil@dev.azure.com/TITBrasil/TITCS%20-%20Live4Safe/_git/Live4Safe_Common
 Author: TIT CS
 Author-email: contato@titcs.com.br
 License: MIT
 Project-URL: Código fonte, https://TITBrasil@dev.azure.com/TITBrasil/Gamefica/_git/DJANGO_CLIENT
 Project-URL: Download, https://TITBrasil@dev.azure.com/TITBrasil/Gamefica/_git/DJANGO_CLIENT
```

### Comparing `django-sso-client-0.0.4/django_client_sso/client_base.py` & `django-sso-client-0.0.5/django_client_sso/client_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import requests
 import jwt
 import tempfile
 import json
 from os import path
 from django.conf import settings
+from django_client_sso.exceptions import Exception401
 
 class ClientBase():
     
     def __init__(self) -> None:
         self.host = settings.SSO_HOST
         self.client = settings.CLIENT_ID
         self.secret = settings.CLIENT_SECRET
@@ -44,8 +45,11 @@
             file.write(content['data'])
             file.close()
             
         
     def decode_token(self,token:str):
         self.get_pub()
         publib_key = open(f'{tempfile.gettempdir()}/sso.pub','r').read()        
-        return jwt.decode(token,key=publib_key,algorithms=['RS256'])    
+        try:
+            return jwt.decode(token,key=publib_key,algorithms=['RS256'])    
+        except:
+            raise Exception401()
```

### Comparing `django-sso-client-0.0.4/django_client_sso/decorators.py` & `django-sso-client-0.0.5/django_client_sso/decorators.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,56 @@
-from rest_framework.response import Response
 from functools import wraps
 from django_client_sso.client_base import ClientBase
-from rest_framework import status
+from django_client_sso.exceptions import Exception403,Exception401
 
 def validator_with_request(permissions):
     def decorator_func(func):
         @wraps(func)
         def wrapper(self, request):
             client = ClientBase()
             token = request.META.get('HTTP_AUTHORIZATION')
+            
+            if not token:
+                raise Exception401()
+            
             token = token.replace('Bearer ', '')
+            token_decode = client.decode_token(token)
             
-            try:
-                token_decode = client.decode_token(token)
-            except Exception as ex:
-                return Response(data={'error':ex.args}, status=status.HTTP_401_UNAUTHORIZED)
-
             required = str(permissions).split()
             scope = token_decode['scope']
 
             for r in required:
                 if r in scope:
                     return func(self,request)
            
-            return Response(data={'error':'User does not have permission to access this resource'}, status=status.HTTP_403_FORBIDDEN)
+            raise Exception403()
     
         return wrapper
 
     return decorator_func
 
 
 def validator_without_request(permissions):
     def decorator_func(func):
         @wraps(func)
         def wrapper(self):
             client = ClientBase()
             token = self.request.META.get('HTTP_AUTHORIZATION')
+            
+            if not token:
+                raise Exception401()
+            
             token = token.replace('Bearer ', '')
+            token_decode = client.decode_token(token)
             
-            try:
-                token_decode = client.decode_token(token)
-            except Exception as ex:
-                return Response(data={'error':ex.args}, status=status.HTTP_401_UNAUTHORIZED)
-
             required = str(permissions).split()
             scope = token_decode['scope']
 
             for r in required:
                 if r in scope:
                     return func(self)
            
-            return Response(data={'error':'User does not have permission to access this resource'}, status=status.HTTP_403_FORBIDDEN)
+            raise Exception403()
     
         return wrapper
 
     return decorator_func
```

### Comparing `django-sso-client-0.0.4/django_sso_client.egg-info/PKG-INFO` & `django-sso-client-0.0.5/django_sso_client.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sso-client
-Version: 0.0.4
+Version: 0.0.5
 Summary: Client for Django Apps - SSO TIT/Hyper by P&D
 Home-page: https://TITBrasil@dev.azure.com/TITBrasil/TITCS%20-%20Live4Safe/_git/Live4Safe_Common
 Author: TIT CS
 Author-email: contato@titcs.com.br
 License: MIT
 Project-URL: Código fonte, https://TITBrasil@dev.azure.com/TITBrasil/Gamefica/_git/DJANGO_CLIENT
 Project-URL: Download, https://TITBrasil@dev.azure.com/TITBrasil/Gamefica/_git/DJANGO_CLIENT
```

### Comparing `django-sso-client-0.0.4/setup.py` & `django-sso-client-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='django-sso-client',
-    version='0.0.4',
+    version='0.0.5',
     author='TIT CS',
     author_email='contato@titcs.com.br',
     packages=['django_client_sso'],
     description='Client for Django Apps - SSO TIT/Hyper by P&D',
     long_description='Client for Django Apps - SSO TIT/Hyper by P&D',
     url='https://TITBrasil@dev.azure.com/TITBrasil/TITCS%20-%20Live4Safe/_git/Live4Safe_Common',
     project_urls={
```

