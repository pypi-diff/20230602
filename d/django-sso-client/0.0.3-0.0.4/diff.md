# Comparing `tmp/django-sso-client-0.0.3.tar.gz` & `tmp/django-sso-client-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-sso-client-0.0.3.tar", last modified: Fri Jun  2 17:20:31 2023, max compression
+gzip compressed data, was "django-sso-client-0.0.4.tar", last modified: Fri Jun  2 18:09:55 2023, max compression
```

## Comparing `django-sso-client-0.0.3.tar` & `django-sso-client-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-02 17:20:31.649584 django-sso-client-0.0.3/
--rw-rw-r--   0 israel    (1000) israel    (1000)       38 2023-06-01 22:36:35.000000 django-sso-client-0.0.3/LICENSE.txt
--rw-rw-r--   0 israel    (1000) israel    (1000)      961 2023-06-02 17:20:31.649584 django-sso-client-0.0.3/PKG-INFO
--rw-rw-r--   0 israel    (1000) israel    (1000)      397 2023-06-01 22:45:46.000000 django-sso-client-0.0.3/README.md
-drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-02 17:20:31.649584 django-sso-client-0.0.3/django_client_sso/
--rw-rw-r--   0 israel    (1000) israel    (1000)       31 2023-06-02 17:02:09.000000 django-sso-client-0.0.3/django_client_sso/__init__.py
--rw-rw-r--   0 israel    (1000) israel    (1000)     1630 2023-06-02 16:59:18.000000 django-sso-client-0.0.3/django_client_sso/client_base.py
--rw-rw-r--   0 israel    (1000) israel    (1000)      319 2023-06-02 17:13:57.000000 django-sso-client-0.0.3/django_client_sso/client_office365.py
--rw-rw-r--   0 israel    (1000) israel    (1000)      839 2023-06-02 17:14:30.000000 django-sso-client-0.0.3/django_client_sso/decorators.py
-drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-02 17:20:31.649584 django-sso-client-0.0.3/django_sso_client.egg-info/
--rw-rw-r--   0 israel    (1000) israel    (1000)      961 2023-06-02 17:20:31.000000 django-sso-client-0.0.3/django_sso_client.egg-info/PKG-INFO
--rw-rw-r--   0 israel    (1000) israel    (1000)      337 2023-06-02 17:20:31.000000 django-sso-client-0.0.3/django_sso_client.egg-info/SOURCES.txt
--rw-rw-r--   0 israel    (1000) israel    (1000)        1 2023-06-02 17:20:31.000000 django-sso-client-0.0.3/django_sso_client.egg-info/dependency_links.txt
--rw-rw-r--   0 israel    (1000) israel    (1000)       18 2023-06-02 17:20:31.000000 django-sso-client-0.0.3/django_sso_client.egg-info/top_level.txt
--rw-rw-r--   0 israel    (1000) israel    (1000)      106 2023-06-02 17:20:31.653584 django-sso-client-0.0.3/setup.cfg
--rw-rw-r--   0 israel    (1000) israel    (1000)     1079 2023-06-02 17:20:05.000000 django-sso-client-0.0.3/setup.py
+drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-02 18:09:55.512978 django-sso-client-0.0.4/
+-rw-rw-r--   0 israel    (1000) israel    (1000)       38 2023-06-01 22:36:35.000000 django-sso-client-0.0.4/LICENSE.txt
+-rw-rw-r--   0 israel    (1000) israel    (1000)      961 2023-06-02 18:09:55.516978 django-sso-client-0.0.4/PKG-INFO
+-rw-rw-r--   0 israel    (1000) israel    (1000)      397 2023-06-01 22:45:46.000000 django-sso-client-0.0.4/README.md
+drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-02 18:09:55.512978 django-sso-client-0.0.4/django_client_sso/
+-rw-rw-r--   0 israel    (1000) israel    (1000)       31 2023-06-02 17:02:09.000000 django-sso-client-0.0.4/django_client_sso/__init__.py
+-rw-rw-r--   0 israel    (1000) israel    (1000)     1621 2023-06-02 18:08:25.000000 django-sso-client-0.0.4/django_client_sso/client_base.py
+-rw-rw-r--   0 israel    (1000) israel    (1000)      319 2023-06-02 17:13:57.000000 django-sso-client-0.0.4/django_client_sso/client_office365.py
+-rw-rw-r--   0 israel    (1000) israel    (1000)     1929 2023-06-02 18:09:01.000000 django-sso-client-0.0.4/django_client_sso/decorators.py
+drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-02 18:09:55.512978 django-sso-client-0.0.4/django_sso_client.egg-info/
+-rw-rw-r--   0 israel    (1000) israel    (1000)      961 2023-06-02 18:09:55.000000 django-sso-client-0.0.4/django_sso_client.egg-info/PKG-INFO
+-rw-rw-r--   0 israel    (1000) israel    (1000)      337 2023-06-02 18:09:55.000000 django-sso-client-0.0.4/django_sso_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 israel    (1000) israel    (1000)        1 2023-06-02 18:09:55.000000 django-sso-client-0.0.4/django_sso_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 israel    (1000) israel    (1000)       18 2023-06-02 18:09:55.000000 django-sso-client-0.0.4/django_sso_client.egg-info/top_level.txt
+-rw-rw-r--   0 israel    (1000) israel    (1000)      106 2023-06-02 18:09:55.516978 django-sso-client-0.0.4/setup.cfg
+-rw-rw-r--   0 israel    (1000) israel    (1000)     1079 2023-06-02 18:09:48.000000 django-sso-client-0.0.4/setup.py
```

### Comparing `django-sso-client-0.0.3/PKG-INFO` & `django-sso-client-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sso-client
-Version: 0.0.3
+Version: 0.0.4
 Summary: Client for Django Apps - SSO TIT/Hyper by P&D
 Home-page: https://TITBrasil@dev.azure.com/TITBrasil/TITCS%20-%20Live4Safe/_git/Live4Safe_Common
 Author: TIT CS
 Author-email: contato@titcs.com.br
 License: MIT
 Project-URL: Código fonte, https://TITBrasil@dev.azure.com/TITBrasil/Gamefica/_git/DJANGO_CLIENT
 Project-URL: Download, https://TITBrasil@dev.azure.com/TITBrasil/Gamefica/_git/DJANGO_CLIENT
```

### Comparing `django-sso-client-0.0.3/django_client_sso/client_base.py` & `django-sso-client-0.0.4/django_client_sso/client_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,9 +44,8 @@
             file.write(content['data'])
             file.close()
             
         
     def decode_token(self,token:str):
         self.get_pub()
         publib_key = open(f'{tempfile.gettempdir()}/sso.pub','r').read()        
-        return jwt.decode(token,key=publib_key,algorithms=['RS256'])
-            
+        return jwt.decode(token,key=publib_key,algorithms=['RS256'])
```

### Comparing `django-sso-client-0.0.3/django_client_sso/decorators.py` & `django-sso-client-0.0.4/django_client_sso/decorators.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,57 @@
 from rest_framework.response import Response
 from functools import wraps
 from django_client_sso.client_base import ClientBase
 from rest_framework import status
 
-def perm_validator(permissions):
+def validator_with_request(permissions):
     def decorator_func(func):
         @wraps(func)
         def wrapper(self, request):
             client = ClientBase()
             token = request.META.get('HTTP_AUTHORIZATION')
             token = token.replace('Bearer ', '')
-            token_decode = client.decode_token(token)
+            
+            try:
+                token_decode = client.decode_token(token)
+            except Exception as ex:
+                return Response(data={'error':ex.args}, status=status.HTTP_401_UNAUTHORIZED)
 
             required = str(permissions).split()
             scope = token_decode['scope']
 
             for r in required:
                 if r in scope:
                     return func(self,request)
            
-            return Response(data={'error':'UNAUTHORIZED'}, status=status.HTTP_401_UNAUTHORIZED)
+            return Response(data={'error':'User does not have permission to access this resource'}, status=status.HTTP_403_FORBIDDEN)
+    
+        return wrapper
+
+    return decorator_func
+
+
+def validator_without_request(permissions):
+    def decorator_func(func):
+        @wraps(func)
+        def wrapper(self):
+            client = ClientBase()
+            token = self.request.META.get('HTTP_AUTHORIZATION')
+            token = token.replace('Bearer ', '')
+            
+            try:
+                token_decode = client.decode_token(token)
+            except Exception as ex:
+                return Response(data={'error':ex.args}, status=status.HTTP_401_UNAUTHORIZED)
+
+            required = str(permissions).split()
+            scope = token_decode['scope']
+
+            for r in required:
+                if r in scope:
+                    return func(self)
+           
+            return Response(data={'error':'User does not have permission to access this resource'}, status=status.HTTP_403_FORBIDDEN)
     
         return wrapper
 
     return decorator_func
```

### Comparing `django-sso-client-0.0.3/django_sso_client.egg-info/PKG-INFO` & `django-sso-client-0.0.4/django_sso_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sso-client
-Version: 0.0.3
+Version: 0.0.4
 Summary: Client for Django Apps - SSO TIT/Hyper by P&D
 Home-page: https://TITBrasil@dev.azure.com/TITBrasil/TITCS%20-%20Live4Safe/_git/Live4Safe_Common
 Author: TIT CS
 Author-email: contato@titcs.com.br
 License: MIT
 Project-URL: Código fonte, https://TITBrasil@dev.azure.com/TITBrasil/Gamefica/_git/DJANGO_CLIENT
 Project-URL: Download, https://TITBrasil@dev.azure.com/TITBrasil/Gamefica/_git/DJANGO_CLIENT
```

### Comparing `django-sso-client-0.0.3/setup.py` & `django-sso-client-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='django-sso-client',
-    version='0.0.3',
+    version='0.0.4',
     author='TIT CS',
     author_email='contato@titcs.com.br',
     packages=['django_client_sso'],
     description='Client for Django Apps - SSO TIT/Hyper by P&D',
     long_description='Client for Django Apps - SSO TIT/Hyper by P&D',
     url='https://TITBrasil@dev.azure.com/TITBrasil/TITCS%20-%20Live4Safe/_git/Live4Safe_Common',
     project_urls={
```

