# Comparing `tmp/django-sso-client-0.0.5.tar.gz` & `tmp/django-sso-client-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-sso-client-0.0.5.tar", last modified: Fri Jun  2 19:08:19 2023, max compression
+gzip compressed data, was "django-sso-client-0.0.6.tar", last modified: Fri Jun  2 19:35:30 2023, max compression
```

## Comparing `django-sso-client-0.0.5.tar` & `django-sso-client-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-02 19:08:19.380240 django-sso-client-0.0.5/
--rw-rw-r--   0 israel    (1000) israel    (1000)       38 2023-06-01 22:36:35.000000 django-sso-client-0.0.5/LICENSE.txt
--rw-rw-r--   0 israel    (1000) israel    (1000)      961 2023-06-02 19:08:19.384240 django-sso-client-0.0.5/PKG-INFO
--rw-rw-r--   0 israel    (1000) israel    (1000)      397 2023-06-01 22:45:46.000000 django-sso-client-0.0.5/README.md
-drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-02 19:08:19.380240 django-sso-client-0.0.5/django_client_sso/
--rw-rw-r--   0 israel    (1000) israel    (1000)       31 2023-06-02 17:02:09.000000 django-sso-client-0.0.5/django_client_sso/__init__.py
--rw-rw-r--   0 israel    (1000) israel    (1000)     1741 2023-06-02 19:03:13.000000 django-sso-client-0.0.5/django_client_sso/client_base.py
--rw-rw-r--   0 israel    (1000) israel    (1000)      319 2023-06-02 17:13:57.000000 django-sso-client-0.0.5/django_client_sso/client_office365.py
--rw-rw-r--   0 israel    (1000) israel    (1000)      699 2023-06-02 19:00:45.000000 django-sso-client-0.0.5/django_client_sso/custom_exception_handler.py
--rw-rw-r--   0 israel    (1000) israel    (1000)     1591 2023-06-02 19:06:53.000000 django-sso-client-0.0.5/django_client_sso/decorators.py
--rw-rw-r--   0 israel    (1000) israel    (1000)      369 2023-06-02 19:05:40.000000 django-sso-client-0.0.5/django_client_sso/exceptions.py
-drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-02 19:08:19.380240 django-sso-client-0.0.5/django_sso_client.egg-info/
--rw-rw-r--   0 israel    (1000) israel    (1000)      961 2023-06-02 19:08:19.000000 django-sso-client-0.0.5/django_sso_client.egg-info/PKG-INFO
--rw-rw-r--   0 israel    (1000) israel    (1000)      415 2023-06-02 19:08:19.000000 django-sso-client-0.0.5/django_sso_client.egg-info/SOURCES.txt
--rw-rw-r--   0 israel    (1000) israel    (1000)        1 2023-06-02 19:08:19.000000 django-sso-client-0.0.5/django_sso_client.egg-info/dependency_links.txt
--rw-rw-r--   0 israel    (1000) israel    (1000)       18 2023-06-02 19:08:19.000000 django-sso-client-0.0.5/django_sso_client.egg-info/top_level.txt
--rw-rw-r--   0 israel    (1000) israel    (1000)      106 2023-06-02 19:08:19.384240 django-sso-client-0.0.5/setup.cfg
--rw-rw-r--   0 israel    (1000) israel    (1000)     1079 2023-06-02 19:08:09.000000 django-sso-client-0.0.5/setup.py
+drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-02 19:35:30.548005 django-sso-client-0.0.6/
+-rw-rw-r--   0 israel    (1000) israel    (1000)       38 2023-06-01 22:36:35.000000 django-sso-client-0.0.6/LICENSE.txt
+-rw-rw-r--   0 israel    (1000) israel    (1000)      961 2023-06-02 19:35:30.548005 django-sso-client-0.0.6/PKG-INFO
+-rw-rw-r--   0 israel    (1000) israel    (1000)      397 2023-06-01 22:45:46.000000 django-sso-client-0.0.6/README.md
+drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-02 19:35:30.548005 django-sso-client-0.0.6/django_client_sso/
+-rw-rw-r--   0 israel    (1000) israel    (1000)       31 2023-06-02 17:02:09.000000 django-sso-client-0.0.6/django_client_sso/__init__.py
+-rw-rw-r--   0 israel    (1000) israel    (1000)     1741 2023-06-02 19:03:13.000000 django-sso-client-0.0.6/django_client_sso/client_base.py
+-rw-rw-r--   0 israel    (1000) israel    (1000)      319 2023-06-02 17:13:57.000000 django-sso-client-0.0.6/django_client_sso/client_office365.py
+-rw-rw-r--   0 israel    (1000) israel    (1000)     1592 2023-06-02 19:32:28.000000 django-sso-client-0.0.6/django_client_sso/decorators.py
+-rw-rw-r--   0 israel    (1000) israel    (1000)      361 2023-06-02 19:33:03.000000 django-sso-client-0.0.6/django_client_sso/exceptions.py
+-rw-rw-r--   0 israel    (1000) israel    (1000)      700 2023-06-02 19:35:23.000000 django-sso-client-0.0.6/django_client_sso/handlers.py
+drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-02 19:35:30.548005 django-sso-client-0.0.6/django_sso_client.egg-info/
+-rw-rw-r--   0 israel    (1000) israel    (1000)      961 2023-06-02 19:35:30.000000 django-sso-client-0.0.6/django_sso_client.egg-info/PKG-INFO
+-rw-rw-r--   0 israel    (1000) israel    (1000)      399 2023-06-02 19:35:30.000000 django-sso-client-0.0.6/django_sso_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 israel    (1000) israel    (1000)        1 2023-06-02 19:35:30.000000 django-sso-client-0.0.6/django_sso_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 israel    (1000) israel    (1000)       18 2023-06-02 19:35:30.000000 django-sso-client-0.0.6/django_sso_client.egg-info/top_level.txt
+-rw-rw-r--   0 israel    (1000) israel    (1000)      106 2023-06-02 19:35:30.548005 django-sso-client-0.0.6/setup.cfg
+-rw-rw-r--   0 israel    (1000) israel    (1000)     1079 2023-06-02 19:34:43.000000 django-sso-client-0.0.6/setup.py
```

### Comparing `django-sso-client-0.0.5/PKG-INFO` & `django-sso-client-0.0.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sso-client
-Version: 0.0.5
+Version: 0.0.6
 Summary: Client for Django Apps - SSO TIT/Hyper by P&D
 Home-page: https://TITBrasil@dev.azure.com/TITBrasil/TITCS%20-%20Live4Safe/_git/Live4Safe_Common
 Author: TIT CS
 Author-email: contato@titcs.com.br
 License: MIT
 Project-URL: Código fonte, https://TITBrasil@dev.azure.com/TITBrasil/Gamefica/_git/DJANGO_CLIENT
 Project-URL: Download, https://TITBrasil@dev.azure.com/TITBrasil/Gamefica/_git/DJANGO_CLIENT
```

### Comparing `django-sso-client-0.0.5/django_client_sso/client_base.py` & `django-sso-client-0.0.6/django_client_sso/client_base.py`

 * *Files identical despite different names*

### Comparing `django-sso-client-0.0.5/django_client_sso/custom_exception_handler.py` & `django-sso-client-0.0.6/django_client_sso/handlers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from rest_framework.views import exception_handler
 from rest_framework.response import Response
 from rest_framework import status
 from django_client_sso.exceptions import Exception401,Exception403
 
-def custom_exception_handler(exc, context):
+def default_exception_handler(exc, context):
     response = exception_handler(exc, context)
     if response:
         return response
     
     if isinstance(exc, Exception401):
         return Response({'mensagem':str(exc.message)}, status=status.HTTP_401_UNAUTHORIZED)
```

### Comparing `django-sso-client-0.0.5/django_client_sso/decorators.py` & `django-sso-client-0.0.6/django_client_sso/decorators.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -49,8 +49,8 @@
                 if r in scope:
                     return func(self)
            
             raise Exception403()
     
         return wrapper
 
-    return decorator_func
+    return decorator_func
```

### Comparing `django-sso-client-0.0.5/django_sso_client.egg-info/PKG-INFO` & `django-sso-client-0.0.6/django_sso_client.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sso-client
-Version: 0.0.5
+Version: 0.0.6
 Summary: Client for Django Apps - SSO TIT/Hyper by P&D
 Home-page: https://TITBrasil@dev.azure.com/TITBrasil/TITCS%20-%20Live4Safe/_git/Live4Safe_Common
 Author: TIT CS
 Author-email: contato@titcs.com.br
 License: MIT
 Project-URL: Código fonte, https://TITBrasil@dev.azure.com/TITBrasil/Gamefica/_git/DJANGO_CLIENT
 Project-URL: Download, https://TITBrasil@dev.azure.com/TITBrasil/Gamefica/_git/DJANGO_CLIENT
```

### Comparing `django-sso-client-0.0.5/setup.py` & `django-sso-client-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='django-sso-client',
-    version='0.0.5',
+    version='0.0.6',
     author='TIT CS',
     author_email='contato@titcs.com.br',
     packages=['django_client_sso'],
     description='Client for Django Apps - SSO TIT/Hyper by P&D',
     long_description='Client for Django Apps - SSO TIT/Hyper by P&D',
     url='https://TITBrasil@dev.azure.com/TITBrasil/TITCS%20-%20Live4Safe/_git/Live4Safe_Common',
     project_urls={
```

