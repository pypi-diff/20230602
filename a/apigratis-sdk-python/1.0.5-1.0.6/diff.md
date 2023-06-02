# Comparing `tmp/apigratis-sdk-python-1.0.5.tar.gz` & `tmp/apigratis-sdk-python-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apigratis-sdk-python-1.0.5.tar", last modified: Fri Jun  2 17:07:28 2023, max compression
+gzip compressed data, was "apigratis-sdk-python-1.0.6.tar", last modified: Fri Jun  2 17:46:23 2023, max compression
```

## Comparing `apigratis-sdk-python-1.0.5.tar` & `apigratis-sdk-python-1.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 17:07:28.183146 apigratis-sdk-python-1.0.5/
--rw-rw-rw-   0        0        0     6381 2023-06-02 17:07:28.182150 apigratis-sdk-python-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     4558 2023-06-02 17:07:18.000000 apigratis-sdk-python-1.0.5/README
-drwxrwxrwx   0        0        0        0 2023-06-02 17:07:28.164197 apigratis-sdk-python-1.0.5/apigratis-sdk-python/
--rw-rw-rw-   0        0        0     1663 2023-06-02 17:01:33.000000 apigratis-sdk-python-1.0.5/apigratis-sdk-python/Service.py
--rw-rw-rw-   0        0        0        0 2023-05-29 19:43:41.000000 apigratis-sdk-python-1.0.5/apigratis-sdk-python/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:07:28.181151 apigratis-sdk-python-1.0.5/apigratis_sdk_python.egg-info/
--rw-rw-rw-   0        0        0     6381 2023-06-02 17:07:27.000000 apigratis-sdk-python-1.0.5/apigratis_sdk_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2023-06-02 17:07:28.000000 apigratis-sdk-python-1.0.5/apigratis_sdk_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 17:07:27.000000 apigratis-sdk-python-1.0.5/apigratis_sdk_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-02 17:07:27.000000 apigratis-sdk-python-1.0.5/apigratis_sdk_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-02 17:07:27.000000 apigratis-sdk-python-1.0.5/apigratis_sdk_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1069 2023-06-02 17:07:14.000000 apigratis-sdk-python-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-02 17:07:28.183146 apigratis-sdk-python-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      861 2023-06-02 17:07:22.000000 apigratis-sdk-python-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 17:46:23.789873 apigratis-sdk-python-1.0.6/
+-rw-rw-rw-   0        0        0     6391 2023-06-02 17:46:23.789873 apigratis-sdk-python-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4568 2023-06-02 17:45:54.000000 apigratis-sdk-python-1.0.6/README
+drwxrwxrwx   0        0        0        0 2023-06-02 17:46:23.772878 apigratis-sdk-python-1.0.6/apigratis-sdk-python/
+-rw-rw-rw-   0        0        0     1663 2023-06-02 17:01:33.000000 apigratis-sdk-python-1.0.6/apigratis-sdk-python/Service.py
+-rw-rw-rw-   0        0        0        0 2023-05-29 19:43:41.000000 apigratis-sdk-python-1.0.6/apigratis-sdk-python/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 17:46:23.787369 apigratis-sdk-python-1.0.6/apigratis_sdk_python.egg-info/
+-rw-rw-rw-   0        0        0     6391 2023-06-02 17:46:23.000000 apigratis-sdk-python-1.0.6/apigratis_sdk_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2023-06-02 17:46:23.000000 apigratis-sdk-python-1.0.6/apigratis_sdk_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 17:46:23.000000 apigratis-sdk-python-1.0.6/apigratis_sdk_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-02 17:46:23.000000 apigratis-sdk-python-1.0.6/apigratis_sdk_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-02 17:46:23.000000 apigratis-sdk-python-1.0.6/apigratis_sdk_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1069 2023-06-02 17:46:10.000000 apigratis-sdk-python-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-02 17:46:23.790876 apigratis-sdk-python-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      861 2023-06-02 17:46:08.000000 apigratis-sdk-python-1.0.6/setup.py
```

### Comparing `apigratis-sdk-python-1.0.5/PKG-INFO` & `apigratis-sdk-python-1.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apigratis-sdk-python
-Version: 1.0.5
+Version: 1.0.6
 Summary: Transforme seus projetos em soluções inteligentes com nossa API. Com recursos como API do WhatsApp, geolocalização, rastreamento de encomendas, verificação de CPF/CNPJ e mais, você pode criar soluções eficientes e funcionais
 Home-page: https://github.com/APIBrasil/apigratis-sdk-python
 Author: APIBRASIL
 Author-email: contato@apibrasil.com.br
 License: MIT License
 Description: # SDK Python - APIGratis by API BRASIL
         
@@ -124,23 +124,23 @@
         
             print(vehicle)
         
         if __name__ == "__main__":
             fipe()
         ```
         
-        ## CNPJ
+        ## Dados CNPJ Service
         
         ```python
         from apigratis.Service import Service
         import json
         
-        def fipe():
+        def cnpj():
         
-            vehicle = Service().vehicles(json.dumps({
+            vehicle = Service().cnpj(json.dumps({
                 "action": "/",
                 "credentials": {
                     "SecretKey": "SEU_SECRET_KEY",
                     "PublicToken": "SEU_PUBLIC_TOKEN",
                     "DeviceToken": "SEU_DEVICE_TOKEN",
                     "BearerToken": "SEU_BEARER_TOKEN",
                 },
@@ -148,12 +148,12 @@
                     "placa": "OQH3065",
                 }
             }))
         
             print(vehicle)
         
         if __name__ == "__main__":
-            fipe()
+            cnpj()
         ```
 Keywords: whatsapp api,apibrasil,cnpj,sms,cep,consulta,api,brasil,gratis,free,whatsapp,apiwhatsapp,apigratis,apifree
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `apigratis-sdk-python-1.0.5/README` & `apigratis-sdk-python-1.0.6/README`

 * *Files 2% similar despite different names*

```diff
@@ -116,23 +116,23 @@
 
     print(vehicle)
 
 if __name__ == "__main__":
     fipe()
 ```
 
-## CNPJ
+## Dados CNPJ Service
 
 ```python
 from apigratis.Service import Service
 import json
 
-def fipe():
+def cnpj():
 
-    vehicle = Service().vehicles(json.dumps({
+    vehicle = Service().cnpj(json.dumps({
         "action": "/",
         "credentials": {
             "SecretKey": "SEU_SECRET_KEY",
             "PublicToken": "SEU_PUBLIC_TOKEN",
             "DeviceToken": "SEU_DEVICE_TOKEN",
             "BearerToken": "SEU_BEARER_TOKEN",
         },
@@ -140,9 +140,9 @@
             "placa": "OQH3065",
         }
     }))
 
     print(vehicle)
 
 if __name__ == "__main__":
-    fipe()
+    cnpj()
 ```
```

### Comparing `apigratis-sdk-python-1.0.5/apigratis-sdk-python/Service.py` & `apigratis-sdk-python-1.0.6/apigratis-sdk-python/Service.py`

 * *Files identical despite different names*

### Comparing `apigratis-sdk-python-1.0.5/apigratis_sdk_python.egg-info/PKG-INFO` & `apigratis-sdk-python-1.0.6/apigratis_sdk_python.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apigratis-sdk-python
-Version: 1.0.5
+Version: 1.0.6
 Summary: Transforme seus projetos em soluções inteligentes com nossa API. Com recursos como API do WhatsApp, geolocalização, rastreamento de encomendas, verificação de CPF/CNPJ e mais, você pode criar soluções eficientes e funcionais
 Home-page: https://github.com/APIBrasil/apigratis-sdk-python
 Author: APIBRASIL
 Author-email: contato@apibrasil.com.br
 License: MIT License
 Description: # SDK Python - APIGratis by API BRASIL
         
@@ -124,23 +124,23 @@
         
             print(vehicle)
         
         if __name__ == "__main__":
             fipe()
         ```
         
-        ## CNPJ
+        ## Dados CNPJ Service
         
         ```python
         from apigratis.Service import Service
         import json
         
-        def fipe():
+        def cnpj():
         
-            vehicle = Service().vehicles(json.dumps({
+            vehicle = Service().cnpj(json.dumps({
                 "action": "/",
                 "credentials": {
                     "SecretKey": "SEU_SECRET_KEY",
                     "PublicToken": "SEU_PUBLIC_TOKEN",
                     "DeviceToken": "SEU_DEVICE_TOKEN",
                     "BearerToken": "SEU_BEARER_TOKEN",
                 },
@@ -148,12 +148,12 @@
                     "placa": "OQH3065",
                 }
             }))
         
             print(vehicle)
         
         if __name__ == "__main__":
-            fipe()
+            cnpj()
         ```
 Keywords: whatsapp api,apibrasil,cnpj,sms,cep,consulta,api,brasil,gratis,free,whatsapp,apiwhatsapp,apigratis,apifree
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `apigratis-sdk-python-1.0.5/pyproject.toml` & `apigratis-sdk-python-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "apigratis-sdk-python"
 description = "A ideia desse SDK é otimizar o tempo de código dos usuários auxiliando na integração com a plataforma."
-version = "1.0.5"
+version = "1.0.6"
 authors = [
   { name="APIBRASIL", email="contato@apibrasil.com.br" },
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
 keywords = ["python", "package", "build", "tutorial"]
 requires-python = ">=3.7"
```

### Comparing `apigratis-sdk-python-1.0.5/setup.py` & `apigratis-sdk-python-1.0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     readme = fh.read()
 
 setup(name='apigratis-sdk-python',
-    version='1.0.5',
+    version='1.0.6',
     url='https://github.com/APIBrasil/apigratis-sdk-python',
     license='MIT License',
     author='APIBRASIL',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='contato@apibrasil.com.br',
     keywords='whatsapp api, apibrasil, cnpj, sms, cep, consulta, api, brasil, gratis, free, whatsapp, apiwhatsapp, apigratis, apifree',
```

