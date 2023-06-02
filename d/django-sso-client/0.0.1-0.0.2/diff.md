# Comparing `tmp/django-sso-client-0.0.1.tar.gz` & `tmp/django-sso-client-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-sso-client-0.0.1.tar", last modified: Thu Jun  1 22:40:29 2023, max compression
+gzip compressed data, was "django-sso-client-0.0.2.tar", last modified: Fri Jun  2 17:03:53 2023, max compression
```

## Comparing `django-sso-client-0.0.1.tar` & `django-sso-client-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-01 22:40:29.391190 django-sso-client-0.0.1/
--rw-rw-r--   0 israel    (1000) israel    (1000)       38 2023-06-01 22:36:35.000000 django-sso-client-0.0.1/LICENSE.txt
--rw-rw-r--   0 israel    (1000) israel    (1000)      954 2023-06-01 22:40:29.391190 django-sso-client-0.0.1/PKG-INFO
--rw-rw-r--   0 israel    (1000) israel    (1000)      377 2023-06-01 22:36:35.000000 django-sso-client-0.0.1/README.md
-drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-01 22:40:29.387190 django-sso-client-0.0.1/client_sso/
--rw-rw-r--   0 israel    (1000) israel    (1000)       24 2023-06-01 22:36:35.000000 django-sso-client-0.0.1/client_sso/__init__.py
--rw-rw-r--   0 israel    (1000) israel    (1000)     1391 2023-06-01 22:36:35.000000 django-sso-client-0.0.1/client_sso/client_base.py
--rw-rw-r--   0 israel    (1000) israel    (1000)      317 2023-06-01 22:36:35.000000 django-sso-client-0.0.1/client_sso/client_office365.py
--rw-rw-r--   0 israel    (1000) israel    (1000)      775 2023-06-01 22:36:35.000000 django-sso-client-0.0.1/client_sso/decorators.py
-drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-01 22:40:29.391190 django-sso-client-0.0.1/django_sso_client.egg-info/
--rw-rw-r--   0 israel    (1000) israel    (1000)      954 2023-06-01 22:40:29.000000 django-sso-client-0.0.1/django_sso_client.egg-info/PKG-INFO
--rw-rw-r--   0 israel    (1000) israel    (1000)      309 2023-06-01 22:40:29.000000 django-sso-client-0.0.1/django_sso_client.egg-info/SOURCES.txt
--rw-rw-r--   0 israel    (1000) israel    (1000)        1 2023-06-01 22:40:29.000000 django-sso-client-0.0.1/django_sso_client.egg-info/dependency_links.txt
--rw-rw-r--   0 israel    (1000) israel    (1000)       11 2023-06-01 22:40:29.000000 django-sso-client-0.0.1/django_sso_client.egg-info/top_level.txt
--rw-rw-r--   0 israel    (1000) israel    (1000)      106 2023-06-01 22:40:29.391190 django-sso-client-0.0.1/setup.cfg
--rw-rw-r--   0 israel    (1000) israel    (1000)     1065 2023-06-01 22:36:35.000000 django-sso-client-0.0.1/setup.py
+drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-02 17:03:53.063136 django-sso-client-0.0.2/
+-rw-rw-r--   0 israel    (1000) israel    (1000)       38 2023-06-01 22:36:35.000000 django-sso-client-0.0.2/LICENSE.txt
+-rw-rw-r--   0 israel    (1000) israel    (1000)      961 2023-06-02 17:03:53.063136 django-sso-client-0.0.2/PKG-INFO
+-rw-rw-r--   0 israel    (1000) israel    (1000)      397 2023-06-01 22:45:46.000000 django-sso-client-0.0.2/README.md
+drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-02 17:03:53.059136 django-sso-client-0.0.2/django_client_sso/
+-rw-rw-r--   0 israel    (1000) israel    (1000)       31 2023-06-02 17:02:09.000000 django-sso-client-0.0.2/django_client_sso/__init__.py
+-rw-rw-r--   0 israel    (1000) israel    (1000)     1630 2023-06-02 16:59:18.000000 django-sso-client-0.0.2/django_client_sso/client_base.py
+-rw-rw-r--   0 israel    (1000) israel    (1000)      301 2023-06-02 17:02:26.000000 django-sso-client-0.0.2/django_client_sso/client_office365.py
+-rw-rw-r--   0 israel    (1000) israel    (1000)      807 2023-06-02 17:00:06.000000 django-sso-client-0.0.2/django_client_sso/decorators.py
+drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-02 17:03:53.063136 django-sso-client-0.0.2/django_sso_client.egg-info/
+-rw-rw-r--   0 israel    (1000) israel    (1000)      961 2023-06-02 17:03:53.000000 django-sso-client-0.0.2/django_sso_client.egg-info/PKG-INFO
+-rw-rw-r--   0 israel    (1000) israel    (1000)      337 2023-06-02 17:03:53.000000 django-sso-client-0.0.2/django_sso_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 israel    (1000) israel    (1000)        1 2023-06-02 17:03:53.000000 django-sso-client-0.0.2/django_sso_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 israel    (1000) israel    (1000)       18 2023-06-02 17:03:53.000000 django-sso-client-0.0.2/django_sso_client.egg-info/top_level.txt
+-rw-rw-r--   0 israel    (1000) israel    (1000)      106 2023-06-02 17:03:53.063136 django-sso-client-0.0.2/setup.cfg
+-rw-rw-r--   0 israel    (1000) israel    (1000)     1079 2023-06-02 17:03:17.000000 django-sso-client-0.0.2/setup.py
```

### Comparing `django-sso-client-0.0.1/PKG-INFO` & `django-sso-client-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: django-sso-client
-Version: 0.0.1
+Version: 0.0.2
 Summary: Client for Django Apps - SSO TIT/Hyper by P&D
 Home-page: https://TITBrasil@dev.azure.com/TITBrasil/TITCS%20-%20Live4Safe/_git/Live4Safe_Common
 Author: TIT CS
 Author-email: contato@titcs.com.br
 License: MIT
 Project-URL: Código fonte, https://TITBrasil@dev.azure.com/TITBrasil/Gamefica/_git/DJANGO_CLIENT
 Project-URL: Download, https://TITBrasil@dev.azure.com/TITBrasil/Gamefica/_git/DJANGO_CLIENT
-Keywords: django_sso
+Keywords: django_client_sso
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Portuguese (Brazilian)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Internationalization
```

### Comparing `django-sso-client-0.0.1/client_sso/client_base.py` & `django-sso-client-0.0.2/django_client_sso/client_base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,52 @@
 import requests
 import jwt
-from os import getenv, path
+import tempfile
+import json
+from os import path
+from django.conf import settings
 
 class ClientBase():
     
     def __init__(self) -> None:
-        self.host = getenv('SSO_HOST','http://localhost:8000')
-        self.client = getenv('CLIENT_ID','app')
-        self.secret = getenv('CLIENT_SECRET','app')
+        self.host = settings.SSO_HOST
+        self.client = settings.CLIENT_ID
+        self.secret = settings.CLIENT_SECRET
 
     def get_app_token(self):
         data = {
             'client_id':self.client,
-            'client_secret':self.secret
+            'client_secret':self.secret,
+            'grant_type':'client_credentials'
         }
         response = requests.post(f'{self.host}/o/token/',data=data)
         
         if response.status_code != 200:
             raise Exception(f'Erro ao tentar conectar no servidor sso. cod:{response.status_code}')
         
-        return response.content['access_token']
-    
-    def save_public_key(self, app_token:str):
+        content = response.content.decode('utf-8')
+        content = json.loads(content)
+        
+        return content['access_token']
+   
+    def get_pub(self):
+        if path.exists(f'{tempfile.gettempdir()}/sso.pub'):
+            return        
+        
+        app_token = self.get_app_token()
         headers = {
             'Authorization':f'Bearer {app_token}'
-        }
-        response = requests.get(f'{self.host}/o/token/',headers=headers)
+        }        
+        response = requests.get(f'{self.host}/pub/',headers=headers)
+        content = response.content.decode('utf-8')
+        content = json.loads(content)
         
-        if response.status_code != 200:
-            raise Exception(f'Erro ao tentar conectar no servidor sso. cod:{response.status_code}')
-
-        with open('sso.pub','w') as file:
-            file.write(response.content['data'])
+        with open(f'{tempfile.gettempdir()}/sso.pub','w') as file:
+            file.write(content['data'])
             file.close()
-
+            
+        
     def decode_token(self,token:str):
-        if not path.exists('ssp.pub'):
-            self.save_public_key(token)
-
-        public_key = open('sso.pub', 'r').read()
-        return jwt.decode(token,key=public_key,algorithms=['RS256'])
+        self.get_pub()
+        publib_key = open(f'{tempfile.gettempdir()}/sso.pub','r').read()        
+        return jwt.decode(token,key=publib_key,algorithms=['RS256'])
+
```

### Comparing `django-sso-client-0.0.1/django_sso_client.egg-info/PKG-INFO` & `django-sso-client-0.0.2/django_sso_client.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: django-sso-client
-Version: 0.0.1
+Version: 0.0.2
 Summary: Client for Django Apps - SSO TIT/Hyper by P&D
 Home-page: https://TITBrasil@dev.azure.com/TITBrasil/TITCS%20-%20Live4Safe/_git/Live4Safe_Common
 Author: TIT CS
 Author-email: contato@titcs.com.br
 License: MIT
 Project-URL: Código fonte, https://TITBrasil@dev.azure.com/TITBrasil/Gamefica/_git/DJANGO_CLIENT
 Project-URL: Download, https://TITBrasil@dev.azure.com/TITBrasil/Gamefica/_git/DJANGO_CLIENT
-Keywords: django_sso
+Keywords: django_client_sso
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Portuguese (Brazilian)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Internationalization
```

### Comparing `django-sso-client-0.0.1/setup.py` & `django-sso-client-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup
 
 setup(
     name='django-sso-client',
-    version='0.0.1',
+    version='0.0.2',
     author='TIT CS',
     author_email='contato@titcs.com.br',
-    packages=['client_sso'],
+    packages=['django_client_sso'],
     description='Client for Django Apps - SSO TIT/Hyper by P&D',
     long_description='Client for Django Apps - SSO TIT/Hyper by P&D',
     url='https://TITBrasil@dev.azure.com/TITBrasil/TITCS%20-%20Live4Safe/_git/Live4Safe_Common',
     project_urls={
         'Código fonte': 'https://TITBrasil@dev.azure.com/TITBrasil/Gamefica/_git/DJANGO_CLIENT',
         'Download': 'https://TITBrasil@dev.azure.com/TITBrasil/Gamefica/_git/DJANGO_CLIENT'
     },
     license='MIT',
-    keywords='django_sso',
+    keywords='django_client_sso',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: Portuguese (Brazilian)',
         'Operating System :: OS Independent',
         'Topic :: Software Development :: Internationalization',
```

