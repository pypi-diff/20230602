# Comparing `tmp/apigratis-sdk-python-1.0.4.tar.gz` & `tmp/apigratis-sdk-python-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apigratis-sdk-python-1.0.4.tar", last modified: Fri Jun  2 17:04:15 2023, max compression
+gzip compressed data, was "apigratis-sdk-python-1.0.5.tar", last modified: Fri Jun  2 17:07:28 2023, max compression
```

## Comparing `apigratis-sdk-python-1.0.4.tar` & `apigratis-sdk-python-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 17:04:15.662237 apigratis-sdk-python-1.0.4/
--rw-rw-rw-   0        0        0     6399 2023-06-02 17:04:15.661239 apigratis-sdk-python-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     4492 2023-06-02 17:01:33.000000 apigratis-sdk-python-1.0.4/README
-drwxrwxrwx   0        0        0        0 2023-06-02 17:04:15.639299 apigratis-sdk-python-1.0.4/apigratis-sdk-python/
--rw-rw-rw-   0        0        0     1663 2023-06-02 17:01:33.000000 apigratis-sdk-python-1.0.4/apigratis-sdk-python/Service.py
--rw-rw-rw-   0        0        0        0 2023-05-29 19:43:41.000000 apigratis-sdk-python-1.0.4/apigratis-sdk-python/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:04:15.660244 apigratis-sdk-python-1.0.4/apigratis_sdk_python.egg-info/
--rw-rw-rw-   0        0        0     6399 2023-06-02 17:04:15.000000 apigratis-sdk-python-1.0.4/apigratis_sdk_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2023-06-02 17:04:15.000000 apigratis-sdk-python-1.0.4/apigratis_sdk_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 17:04:15.000000 apigratis-sdk-python-1.0.4/apigratis_sdk_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-02 17:04:15.000000 apigratis-sdk-python-1.0.4/apigratis_sdk_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-02 17:04:15.000000 apigratis-sdk-python-1.0.4/apigratis_sdk_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1069 2023-06-02 17:03:50.000000 apigratis-sdk-python-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-02 17:04:15.662237 apigratis-sdk-python-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      861 2023-06-02 17:02:59.000000 apigratis-sdk-python-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 17:07:28.183146 apigratis-sdk-python-1.0.5/
+-rw-rw-rw-   0        0        0     6381 2023-06-02 17:07:28.182150 apigratis-sdk-python-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4558 2023-06-02 17:07:18.000000 apigratis-sdk-python-1.0.5/README
+drwxrwxrwx   0        0        0        0 2023-06-02 17:07:28.164197 apigratis-sdk-python-1.0.5/apigratis-sdk-python/
+-rw-rw-rw-   0        0        0     1663 2023-06-02 17:01:33.000000 apigratis-sdk-python-1.0.5/apigratis-sdk-python/Service.py
+-rw-rw-rw-   0        0        0        0 2023-05-29 19:43:41.000000 apigratis-sdk-python-1.0.5/apigratis-sdk-python/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 17:07:28.181151 apigratis-sdk-python-1.0.5/apigratis_sdk_python.egg-info/
+-rw-rw-rw-   0        0        0     6381 2023-06-02 17:07:27.000000 apigratis-sdk-python-1.0.5/apigratis_sdk_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2023-06-02 17:07:28.000000 apigratis-sdk-python-1.0.5/apigratis_sdk_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 17:07:27.000000 apigratis-sdk-python-1.0.5/apigratis_sdk_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-02 17:07:27.000000 apigratis-sdk-python-1.0.5/apigratis_sdk_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-02 17:07:27.000000 apigratis-sdk-python-1.0.5/apigratis_sdk_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1069 2023-06-02 17:07:14.000000 apigratis-sdk-python-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-02 17:07:28.183146 apigratis-sdk-python-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      861 2023-06-02 17:07:22.000000 apigratis-sdk-python-1.0.5/setup.py
```

### Comparing `apigratis-sdk-python-1.0.4/PKG-INFO` & `apigratis-sdk-python-1.0.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apigratis-sdk-python
-Version: 1.0.4
+Version: 1.0.5
 Summary: Transforme seus projetos em soluções inteligentes com nossa API. Com recursos como API do WhatsApp, geolocalização, rastreamento de encomendas, verificação de CPF/CNPJ e mais, você pode criar soluções eficientes e funcionais
 Home-page: https://github.com/APIBrasil/apigratis-sdk-python
 Author: APIBRASIL
 Author-email: contato@apibrasil.com.br
 License: MIT License
 Description: # SDK Python - APIGratis by API BRASIL
         
@@ -12,35 +12,35 @@
         
         _Transforme seus projetos em solucoes inteligentes com nossa API. Com recursos como API do WhatsApp, geolocalizacao, rastreamento de encomendas, verificacao de CPF/CNPJ e mais, voce pode criar solucoes eficientes e funcionais._
         
         ## Como instalar
         
         ```pip install apigratis-sdk-python```
         ## Canais de suporte (Comunidade)
-        [![WhatsApp Group](https://img.shields.io/badge/WhatsApp-Group-25D366?logo=whatsapp)](https://chat.whatsapp.com/KsxrUGIPWvUBYAjI1ogaGs)
+        [![WhatsApp Group](https://img.shields.io/badge/WhatsApp-Group-25D366?logo=whatsapp)](https://chat.whatsapp.com/KsPendingrUGIPWvUBYAjI1ogaGs)
         [![Telegram Group](https://img.shields.io/badge/Telegram-Group-32AFED?logo=telegram)](https://t.me/apigratisoficial)
         
         ## Obtenha suas credenciais
         https://apigratis.com.br
         
         ## Mais informacoes
         
         https://pypi.org/project/apigratis-sdk-python
         
         ## Servicos de API disponiveis
         
         | Up  | Services available            | Description       | Free    | Beta        | Stable   |
         ------|-------------------------------|-------------------|---------| ------------------------- | ------------------------- |
-        | âœ“ | WhatsAppService                | API do WhatsApp Gratuita.               |   âœ“   | âœ“                   | x                   |
-        | âœ“ | Receita Data CNPJ              | API Dados CNPJ Receita.                 |   âœ“   | âœ“                   | x                   |
-        | âœ“ | Receita Data CPF               | API Dados de CPF Serasa.                |   âœ“   | âœ“                   | x                   |
-        | âœ“ | CorreiosService                | API Busca encomendas Correios Brazil.   |   âœ“   | âœ“                   | x                   |
-        | âœ“ | CEPLocation                    | API CEP Geolocation + IBGE Brazil.      |   âœ“   | âœ“                   | x                   |
-        | âœ“ | VehiclesService                | API Placa Dados.                        |   âœ“   | âœ“                   | x                   |
-        | âœ“ | FipeService                    | API Placa FIPE.                         |   âœ“   | âœ“                   | x                   |
+        | Yes | WhatsAppService                | API do WhatsApp Gratuita.               |   Yes   | Yes                   | Pending                   |
+        | Yes | Receita Data CNPJ              | API Dados CNPJ Receita.                 |   Yes   | Yes                   | Pending                   |
+        | Yes | Receita Data CPF               | API Dados de CPF Serasa.                |   Yes   | Yes                   | Pending                   |
+        | Yes | CorreiosService                | API Busca encomendas Correios Brazil.   |   Yes   | Yes                   | Pending                   |
+        | Yes | CEPLocation                    | API CEP Geolocation + IBGE Brazil.      |   Yes   | Yes                   | Pending                   |
+        | Yes | VehiclesService                | API Placa Dados.                        |   Yes   | Yes                   | Pending                   |
+        | Yes | FipeService                    | API Placa FIPE.                         |   Yes   | Yes                   | Pending                   |
         
         ## Como utilizar
         
         _Voce pode utilizar todos os endpoints da API do WhatsApp, basta mudar o action e o body_
         
         ## Documentacoes
         https://apibrasil.com.br/documentacoes
@@ -49,30 +49,30 @@
         
         ```python
         from apigratis.Service import Service
         import json
         
         def whatsapp():
         
-            sendText = Service().whatsapp(json.dumps({
-                "action": "sendText",
+            sendTePendingt = Service().whatsapp(json.dumps({
+                "action": "sendTePendingt",
                 "credentials": {
                     "SecretKey": "SEU_SECRET_KEY",
                     "PublicToken": "SEU_PUBLIC_TOKEN",
                     "DeviceToken": "SEU_DEVICE_TOKEN",
                     "BearerToken": "SEU_BEARER_TOKEN",
                 },
                 "body": {
                     "message": "Hello World for Python",
                     "phone": "5531994359434",
                     "time_typing": 1
                 }
             }))
         
-            print(sendText)
+            print(sendTePendingt)
         
         if __name__ == "__main__":
             whatsapp()
         ```
         
         ## Vehicles Data Service
```

### Comparing `apigratis-sdk-python-1.0.4/README` & `apigratis-sdk-python-1.0.5/README`

 * *Files 12% similar despite different names*

```diff
@@ -4,35 +4,35 @@
 
 _Transforme seus projetos em solucoes inteligentes com nossa API. Com recursos como API do WhatsApp, geolocalizacao, rastreamento de encomendas, verificacao de CPF/CNPJ e mais, voce pode criar solucoes eficientes e funcionais._
 
 ## Como instalar
 
 ```pip install apigratis-sdk-python```
 ## Canais de suporte (Comunidade)
-[![WhatsApp Group](https://img.shields.io/badge/WhatsApp-Group-25D366?logo=whatsapp)](https://chat.whatsapp.com/KsxrUGIPWvUBYAjI1ogaGs)
+[![WhatsApp Group](https://img.shields.io/badge/WhatsApp-Group-25D366?logo=whatsapp)](https://chat.whatsapp.com/KsPendingrUGIPWvUBYAjI1ogaGs)
 [![Telegram Group](https://img.shields.io/badge/Telegram-Group-32AFED?logo=telegram)](https://t.me/apigratisoficial)
 
 ## Obtenha suas credenciais
 https://apigratis.com.br
 
 ## Mais informacoes
 
 https://pypi.org/project/apigratis-sdk-python
 
 ## Servicos de API disponiveis
 
 | Up  | Services available            | Description       | Free    | Beta        | Stable   |
 ------|-------------------------------|-------------------|---------| ------------------------- | ------------------------- |
-| ✓ | WhatsAppService                | API do WhatsApp Gratuita.               |   ✓   | ✓                   | x                   |
-| ✓ | Receita Data CNPJ              | API Dados CNPJ Receita.                 |   ✓   | ✓                   | x                   |
-| ✓ | Receita Data CPF               | API Dados de CPF Serasa.                |   ✓   | ✓                   | x                   |
-| ✓ | CorreiosService                | API Busca encomendas Correios Brazil.   |   ✓   | ✓                   | x                   |
-| ✓ | CEPLocation                    | API CEP Geolocation + IBGE Brazil.      |   ✓   | ✓                   | x                   |
-| ✓ | VehiclesService                | API Placa Dados.                        |   ✓   | ✓                   | x                   |
-| ✓ | FipeService                    | API Placa FIPE.                         |   ✓   | ✓                   | x                   |
+| Yes | WhatsAppService                | API do WhatsApp Gratuita.               |   Yes   | Yes                   | Pending                   |
+| Yes | Receita Data CNPJ              | API Dados CNPJ Receita.                 |   Yes   | Yes                   | Pending                   |
+| Yes | Receita Data CPF               | API Dados de CPF Serasa.                |   Yes   | Yes                   | Pending                   |
+| Yes | CorreiosService                | API Busca encomendas Correios Brazil.   |   Yes   | Yes                   | Pending                   |
+| Yes | CEPLocation                    | API CEP Geolocation + IBGE Brazil.      |   Yes   | Yes                   | Pending                   |
+| Yes | VehiclesService                | API Placa Dados.                        |   Yes   | Yes                   | Pending                   |
+| Yes | FipeService                    | API Placa FIPE.                         |   Yes   | Yes                   | Pending                   |
 
 ## Como utilizar
 
 _Voce pode utilizar todos os endpoints da API do WhatsApp, basta mudar o action e o body_
 
 ## Documentacoes
 https://apibrasil.com.br/documentacoes
@@ -41,30 +41,30 @@
 
 ```python
 from apigratis.Service import Service
 import json
 
 def whatsapp():
 
-    sendText = Service().whatsapp(json.dumps({
-        "action": "sendText",
+    sendTePendingt = Service().whatsapp(json.dumps({
+        "action": "sendTePendingt",
         "credentials": {
             "SecretKey": "SEU_SECRET_KEY",
             "PublicToken": "SEU_PUBLIC_TOKEN",
             "DeviceToken": "SEU_DEVICE_TOKEN",
             "BearerToken": "SEU_BEARER_TOKEN",
         },
         "body": {
             "message": "Hello World for Python",
             "phone": "5531994359434",
             "time_typing": 1
         }
     }))
 
-    print(sendText)
+    print(sendTePendingt)
 
 if __name__ == "__main__":
     whatsapp()
 ```
 
 ## Vehicles Data Service
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `apigratis-sdk-python-1.0.4/apigratis-sdk-python/Service.py` & `apigratis-sdk-python-1.0.5/apigratis-sdk-python/Service.py`

 * *Files identical despite different names*

### Comparing `apigratis-sdk-python-1.0.4/apigratis_sdk_python.egg-info/PKG-INFO` & `apigratis-sdk-python-1.0.5/apigratis_sdk_python.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apigratis-sdk-python
-Version: 1.0.4
+Version: 1.0.5
 Summary: Transforme seus projetos em soluções inteligentes com nossa API. Com recursos como API do WhatsApp, geolocalização, rastreamento de encomendas, verificação de CPF/CNPJ e mais, você pode criar soluções eficientes e funcionais
 Home-page: https://github.com/APIBrasil/apigratis-sdk-python
 Author: APIBRASIL
 Author-email: contato@apibrasil.com.br
 License: MIT License
 Description: # SDK Python - APIGratis by API BRASIL
         
@@ -12,35 +12,35 @@
         
         _Transforme seus projetos em solucoes inteligentes com nossa API. Com recursos como API do WhatsApp, geolocalizacao, rastreamento de encomendas, verificacao de CPF/CNPJ e mais, voce pode criar solucoes eficientes e funcionais._
         
         ## Como instalar
         
         ```pip install apigratis-sdk-python```
         ## Canais de suporte (Comunidade)
-        [![WhatsApp Group](https://img.shields.io/badge/WhatsApp-Group-25D366?logo=whatsapp)](https://chat.whatsapp.com/KsxrUGIPWvUBYAjI1ogaGs)
+        [![WhatsApp Group](https://img.shields.io/badge/WhatsApp-Group-25D366?logo=whatsapp)](https://chat.whatsapp.com/KsPendingrUGIPWvUBYAjI1ogaGs)
         [![Telegram Group](https://img.shields.io/badge/Telegram-Group-32AFED?logo=telegram)](https://t.me/apigratisoficial)
         
         ## Obtenha suas credenciais
         https://apigratis.com.br
         
         ## Mais informacoes
         
         https://pypi.org/project/apigratis-sdk-python
         
         ## Servicos de API disponiveis
         
         | Up  | Services available            | Description       | Free    | Beta        | Stable   |
         ------|-------------------------------|-------------------|---------| ------------------------- | ------------------------- |
-        | âœ“ | WhatsAppService                | API do WhatsApp Gratuita.               |   âœ“   | âœ“                   | x                   |
-        | âœ“ | Receita Data CNPJ              | API Dados CNPJ Receita.                 |   âœ“   | âœ“                   | x                   |
-        | âœ“ | Receita Data CPF               | API Dados de CPF Serasa.                |   âœ“   | âœ“                   | x                   |
-        | âœ“ | CorreiosService                | API Busca encomendas Correios Brazil.   |   âœ“   | âœ“                   | x                   |
-        | âœ“ | CEPLocation                    | API CEP Geolocation + IBGE Brazil.      |   âœ“   | âœ“                   | x                   |
-        | âœ“ | VehiclesService                | API Placa Dados.                        |   âœ“   | âœ“                   | x                   |
-        | âœ“ | FipeService                    | API Placa FIPE.                         |   âœ“   | âœ“                   | x                   |
+        | Yes | WhatsAppService                | API do WhatsApp Gratuita.               |   Yes   | Yes                   | Pending                   |
+        | Yes | Receita Data CNPJ              | API Dados CNPJ Receita.                 |   Yes   | Yes                   | Pending                   |
+        | Yes | Receita Data CPF               | API Dados de CPF Serasa.                |   Yes   | Yes                   | Pending                   |
+        | Yes | CorreiosService                | API Busca encomendas Correios Brazil.   |   Yes   | Yes                   | Pending                   |
+        | Yes | CEPLocation                    | API CEP Geolocation + IBGE Brazil.      |   Yes   | Yes                   | Pending                   |
+        | Yes | VehiclesService                | API Placa Dados.                        |   Yes   | Yes                   | Pending                   |
+        | Yes | FipeService                    | API Placa FIPE.                         |   Yes   | Yes                   | Pending                   |
         
         ## Como utilizar
         
         _Voce pode utilizar todos os endpoints da API do WhatsApp, basta mudar o action e o body_
         
         ## Documentacoes
         https://apibrasil.com.br/documentacoes
@@ -49,30 +49,30 @@
         
         ```python
         from apigratis.Service import Service
         import json
         
         def whatsapp():
         
-            sendText = Service().whatsapp(json.dumps({
-                "action": "sendText",
+            sendTePendingt = Service().whatsapp(json.dumps({
+                "action": "sendTePendingt",
                 "credentials": {
                     "SecretKey": "SEU_SECRET_KEY",
                     "PublicToken": "SEU_PUBLIC_TOKEN",
                     "DeviceToken": "SEU_DEVICE_TOKEN",
                     "BearerToken": "SEU_BEARER_TOKEN",
                 },
                 "body": {
                     "message": "Hello World for Python",
                     "phone": "5531994359434",
                     "time_typing": 1
                 }
             }))
         
-            print(sendText)
+            print(sendTePendingt)
         
         if __name__ == "__main__":
             whatsapp()
         ```
         
         ## Vehicles Data Service
```

### Comparing `apigratis-sdk-python-1.0.4/pyproject.toml` & `apigratis-sdk-python-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "apigratis-sdk-python"
 description = "A ideia desse SDK é otimizar o tempo de código dos usuários auxiliando na integração com a plataforma."
-version = "1.0.4"
+version = "1.0.5"
 authors = [
   { name="APIBRASIL", email="contato@apibrasil.com.br" },
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
 keywords = ["python", "package", "build", "tutorial"]
 requires-python = ">=3.7"
```

### Comparing `apigratis-sdk-python-1.0.4/setup.py` & `apigratis-sdk-python-1.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     readme = fh.read()
 
 setup(name='apigratis-sdk-python',
-    version='1.0.4',
+    version='1.0.5',
     url='https://github.com/APIBrasil/apigratis-sdk-python',
     license='MIT License',
     author='APIBRASIL',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='contato@apibrasil.com.br',
     keywords='whatsapp api, apibrasil, cnpj, sms, cep, consulta, api, brasil, gratis, free, whatsapp, apiwhatsapp, apigratis, apifree',
```

