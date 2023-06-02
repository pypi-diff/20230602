# Comparing `tmp/django-sso-client-0.0.2.tar.gz` & `tmp/django-sso-client-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-sso-client-0.0.2.tar", last modified: Fri Jun  2 17:03:53 2023, max compression
+gzip compressed data, was "django-sso-client-0.0.3.tar", last modified: Fri Jun  2 17:20:31 2023, max compression
```

## Comparing `django-sso-client-0.0.2.tar` & `django-sso-client-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-02 17:03:53.063136 django-sso-client-0.0.2/
--rw-rw-r--   0 israel    (1000) israel    (1000)       38 2023-06-01 22:36:35.000000 django-sso-client-0.0.2/LICENSE.txt
--rw-rw-r--   0 israel    (1000) israel    (1000)      961 2023-06-02 17:03:53.063136 django-sso-client-0.0.2/PKG-INFO
--rw-rw-r--   0 israel    (1000) israel    (1000)      397 2023-06-01 22:45:46.000000 django-sso-client-0.0.2/README.md
-drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-02 17:03:53.059136 django-sso-client-0.0.2/django_client_sso/
--rw-rw-r--   0 israel    (1000) israel    (1000)       31 2023-06-02 17:02:09.000000 django-sso-client-0.0.2/django_client_sso/__init__.py
--rw-rw-r--   0 israel    (1000) israel    (1000)     1630 2023-06-02 16:59:18.000000 django-sso-client-0.0.2/django_client_sso/client_base.py
--rw-rw-r--   0 israel    (1000) israel    (1000)      301 2023-06-02 17:02:26.000000 django-sso-client-0.0.2/django_client_sso/client_office365.py
--rw-rw-r--   0 israel    (1000) israel    (1000)      807 2023-06-02 17:00:06.000000 django-sso-client-0.0.2/django_client_sso/decorators.py
-drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-02 17:03:53.063136 django-sso-client-0.0.2/django_sso_client.egg-info/
--rw-rw-r--   0 israel    (1000) israel    (1000)      961 2023-06-02 17:03:53.000000 django-sso-client-0.0.2/django_sso_client.egg-info/PKG-INFO
--rw-rw-r--   0 israel    (1000) israel    (1000)      337 2023-06-02 17:03:53.000000 django-sso-client-0.0.2/django_sso_client.egg-info/SOURCES.txt
--rw-rw-r--   0 israel    (1000) israel    (1000)        1 2023-06-02 17:03:53.000000 django-sso-client-0.0.2/django_sso_client.egg-info/dependency_links.txt
--rw-rw-r--   0 israel    (1000) israel    (1000)       18 2023-06-02 17:03:53.000000 django-sso-client-0.0.2/django_sso_client.egg-info/top_level.txt
--rw-rw-r--   0 israel    (1000) israel    (1000)      106 2023-06-02 17:03:53.063136 django-sso-client-0.0.2/setup.cfg
--rw-rw-r--   0 israel    (1000) israel    (1000)     1079 2023-06-02 17:03:17.000000 django-sso-client-0.0.2/setup.py
+drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-02 17:20:31.649584 django-sso-client-0.0.3/
+-rw-rw-r--   0 israel    (1000) israel    (1000)       38 2023-06-01 22:36:35.000000 django-sso-client-0.0.3/LICENSE.txt
+-rw-rw-r--   0 israel    (1000) israel    (1000)      961 2023-06-02 17:20:31.649584 django-sso-client-0.0.3/PKG-INFO
+-rw-rw-r--   0 israel    (1000) israel    (1000)      397 2023-06-01 22:45:46.000000 django-sso-client-0.0.3/README.md
+drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-02 17:20:31.649584 django-sso-client-0.0.3/django_client_sso/
+-rw-rw-r--   0 israel    (1000) israel    (1000)       31 2023-06-02 17:02:09.000000 django-sso-client-0.0.3/django_client_sso/__init__.py
+-rw-rw-r--   0 israel    (1000) israel    (1000)     1630 2023-06-02 16:59:18.000000 django-sso-client-0.0.3/django_client_sso/client_base.py
+-rw-rw-r--   0 israel    (1000) israel    (1000)      319 2023-06-02 17:13:57.000000 django-sso-client-0.0.3/django_client_sso/client_office365.py
+-rw-rw-r--   0 israel    (1000) israel    (1000)      839 2023-06-02 17:14:30.000000 django-sso-client-0.0.3/django_client_sso/decorators.py
+drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-02 17:20:31.649584 django-sso-client-0.0.3/django_sso_client.egg-info/
+-rw-rw-r--   0 israel    (1000) israel    (1000)      961 2023-06-02 17:20:31.000000 django-sso-client-0.0.3/django_sso_client.egg-info/PKG-INFO
+-rw-rw-r--   0 israel    (1000) israel    (1000)      337 2023-06-02 17:20:31.000000 django-sso-client-0.0.3/django_sso_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 israel    (1000) israel    (1000)        1 2023-06-02 17:20:31.000000 django-sso-client-0.0.3/django_sso_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 israel    (1000) israel    (1000)       18 2023-06-02 17:20:31.000000 django-sso-client-0.0.3/django_sso_client.egg-info/top_level.txt
+-rw-rw-r--   0 israel    (1000) israel    (1000)      106 2023-06-02 17:20:31.653584 django-sso-client-0.0.3/setup.cfg
+-rw-rw-r--   0 israel    (1000) israel    (1000)     1079 2023-06-02 17:20:05.000000 django-sso-client-0.0.3/setup.py
```

### Comparing `django-sso-client-0.0.2/PKG-INFO` & `django-sso-client-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sso-client
-Version: 0.0.2
+Version: 0.0.3
 Summary: Client for Django Apps - SSO TIT/Hyper by P&D
 Home-page: https://TITBrasil@dev.azure.com/TITBrasil/TITCS%20-%20Live4Safe/_git/Live4Safe_Common
 Author: TIT CS
 Author-email: contato@titcs.com.br
 License: MIT
 Project-URL: Código fonte, https://TITBrasil@dev.azure.com/TITBrasil/Gamefica/_git/DJANGO_CLIENT
 Project-URL: Download, https://TITBrasil@dev.azure.com/TITBrasil/Gamefica/_git/DJANGO_CLIENT
```

### Comparing `django-sso-client-0.0.2/django_client_sso/client_base.py` & `django-sso-client-0.0.3/django_client_sso/client_base.py`

 * *Files identical despite different names*

### Comparing `django-sso-client-0.0.2/django_client_sso/decorators.py` & `django-sso-client-0.0.3/django_client_sso/decorators.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from rest_framework.response import Response
 from functools import wraps
-from client_base import ClientBase
+from django_client_sso.client_base import ClientBase
 from rest_framework import status
 
-def perm_validator(arg1):
+def perm_validator(permissions):
     def decorator_func(func):
         @wraps(func)
         def wrapper(self, request):
             client = ClientBase()
             token = request.META.get('HTTP_AUTHORIZATION')
             token = token.replace('Bearer ', '')
             token_decode = client.decode_token(token)
 
-            required = str(arg1).split()
+            required = str(permissions).split()
             scope = token_decode['scope']
 
             for r in required:
                 if r in scope:
                     return func(self,request)
            
             return Response(data={'error':'UNAUTHORIZED'}, status=status.HTTP_401_UNAUTHORIZED)
```

### Comparing `django-sso-client-0.0.2/django_sso_client.egg-info/PKG-INFO` & `django-sso-client-0.0.3/django_sso_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sso-client
-Version: 0.0.2
+Version: 0.0.3
 Summary: Client for Django Apps - SSO TIT/Hyper by P&D
 Home-page: https://TITBrasil@dev.azure.com/TITBrasil/TITCS%20-%20Live4Safe/_git/Live4Safe_Common
 Author: TIT CS
 Author-email: contato@titcs.com.br
 License: MIT
 Project-URL: Código fonte, https://TITBrasil@dev.azure.com/TITBrasil/Gamefica/_git/DJANGO_CLIENT
 Project-URL: Download, https://TITBrasil@dev.azure.com/TITBrasil/Gamefica/_git/DJANGO_CLIENT
```

### Comparing `django-sso-client-0.0.2/setup.py` & `django-sso-client-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='django-sso-client',
-    version='0.0.2',
+    version='0.0.3',
     author='TIT CS',
     author_email='contato@titcs.com.br',
     packages=['django_client_sso'],
     description='Client for Django Apps - SSO TIT/Hyper by P&D',
     long_description='Client for Django Apps - SSO TIT/Hyper by P&D',
     url='https://TITBrasil@dev.azure.com/TITBrasil/TITCS%20-%20Live4Safe/_git/Live4Safe_Common',
     project_urls={
```

