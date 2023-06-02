# Comparing `tmp/apigratis-sdk-python-1.0.3.tar.gz` & `tmp/apigratis-sdk-python-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apigratis-sdk-python-1.0.3.tar", last modified: Fri Jun  2 17:02:00 2023, max compression
+gzip compressed data, was "apigratis-sdk-python-1.0.4.tar", last modified: Fri Jun  2 17:04:15 2023, max compression
```

## Comparing `apigratis-sdk-python-1.0.3.tar` & `apigratis-sdk-python-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 17:02:00.840472 apigratis-sdk-python-1.0.3/
--rw-rw-rw-   0        0        0     6399 2023-06-02 17:02:00.839474 apigratis-sdk-python-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     4492 2023-06-02 17:01:33.000000 apigratis-sdk-python-1.0.3/README
-drwxrwxrwx   0        0        0        0 2023-06-02 17:02:00.812546 apigratis-sdk-python-1.0.3/apigratis-sdk-python/
--rw-rw-rw-   0        0        0     1663 2023-06-02 17:01:33.000000 apigratis-sdk-python-1.0.3/apigratis-sdk-python/Service.py
--rw-rw-rw-   0        0        0        0 2023-05-29 19:43:41.000000 apigratis-sdk-python-1.0.3/apigratis-sdk-python/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:02:00.837479 apigratis-sdk-python-1.0.3/apigratis_sdk_python.egg-info/
--rw-rw-rw-   0        0        0     6399 2023-06-02 17:02:00.000000 apigratis-sdk-python-1.0.3/apigratis_sdk_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2023-06-02 17:02:00.000000 apigratis-sdk-python-1.0.3/apigratis_sdk_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 17:02:00.000000 apigratis-sdk-python-1.0.3/apigratis_sdk_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-02 17:02:00.000000 apigratis-sdk-python-1.0.3/apigratis_sdk_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-02 17:02:00.000000 apigratis-sdk-python-1.0.3/apigratis_sdk_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1069 2023-06-02 17:01:33.000000 apigratis-sdk-python-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-02 17:02:00.840472 apigratis-sdk-python-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      861 2023-06-02 17:01:33.000000 apigratis-sdk-python-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 17:04:15.662237 apigratis-sdk-python-1.0.4/
+-rw-rw-rw-   0        0        0     6399 2023-06-02 17:04:15.661239 apigratis-sdk-python-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4492 2023-06-02 17:01:33.000000 apigratis-sdk-python-1.0.4/README
+drwxrwxrwx   0        0        0        0 2023-06-02 17:04:15.639299 apigratis-sdk-python-1.0.4/apigratis-sdk-python/
+-rw-rw-rw-   0        0        0     1663 2023-06-02 17:01:33.000000 apigratis-sdk-python-1.0.4/apigratis-sdk-python/Service.py
+-rw-rw-rw-   0        0        0        0 2023-05-29 19:43:41.000000 apigratis-sdk-python-1.0.4/apigratis-sdk-python/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 17:04:15.660244 apigratis-sdk-python-1.0.4/apigratis_sdk_python.egg-info/
+-rw-rw-rw-   0        0        0     6399 2023-06-02 17:04:15.000000 apigratis-sdk-python-1.0.4/apigratis_sdk_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2023-06-02 17:04:15.000000 apigratis-sdk-python-1.0.4/apigratis_sdk_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 17:04:15.000000 apigratis-sdk-python-1.0.4/apigratis_sdk_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-02 17:04:15.000000 apigratis-sdk-python-1.0.4/apigratis_sdk_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-02 17:04:15.000000 apigratis-sdk-python-1.0.4/apigratis_sdk_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1069 2023-06-02 17:03:50.000000 apigratis-sdk-python-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-02 17:04:15.662237 apigratis-sdk-python-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      861 2023-06-02 17:02:59.000000 apigratis-sdk-python-1.0.4/setup.py
```

### Comparing `apigratis-sdk-python-1.0.3/PKG-INFO` & `apigratis-sdk-python-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apigratis-sdk-python
-Version: 1.0.3
+Version: 1.0.4
 Summary: Transforme seus projetos em soluções inteligentes com nossa API. Com recursos como API do WhatsApp, geolocalização, rastreamento de encomendas, verificação de CPF/CNPJ e mais, você pode criar soluções eficientes e funcionais
 Home-page: https://github.com/APIBrasil/apigratis-sdk-python
 Author: APIBRASIL
 Author-email: contato@apibrasil.com.br
 License: MIT License
 Description: # SDK Python - APIGratis by API BRASIL
```

### Comparing `apigratis-sdk-python-1.0.3/README` & `apigratis-sdk-python-1.0.4/README`

 * *Files identical despite different names*

### Comparing `apigratis-sdk-python-1.0.3/apigratis-sdk-python/Service.py` & `apigratis-sdk-python-1.0.4/apigratis-sdk-python/Service.py`

 * *Files identical despite different names*

### Comparing `apigratis-sdk-python-1.0.3/apigratis_sdk_python.egg-info/PKG-INFO` & `apigratis-sdk-python-1.0.4/apigratis_sdk_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apigratis-sdk-python
-Version: 1.0.3
+Version: 1.0.4
 Summary: Transforme seus projetos em soluções inteligentes com nossa API. Com recursos como API do WhatsApp, geolocalização, rastreamento de encomendas, verificação de CPF/CNPJ e mais, você pode criar soluções eficientes e funcionais
 Home-page: https://github.com/APIBrasil/apigratis-sdk-python
 Author: APIBRASIL
 Author-email: contato@apibrasil.com.br
 License: MIT License
 Description: # SDK Python - APIGratis by API BRASIL
```

### Comparing `apigratis-sdk-python-1.0.3/pyproject.toml` & `apigratis-sdk-python-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "apigratis-sdk-python"
 description = "A ideia desse SDK é otimizar o tempo de código dos usuários auxiliando na integração com a plataforma."
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="APIBRASIL", email="contato@apibrasil.com.br" },
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
 keywords = ["python", "package", "build", "tutorial"]
 requires-python = ">=3.7"
```

### Comparing `apigratis-sdk-python-1.0.3/setup.py` & `apigratis-sdk-python-1.0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     readme = fh.read()
 
 setup(name='apigratis-sdk-python',
-    version='1.0.3',
+    version='1.0.4',
     url='https://github.com/APIBrasil/apigratis-sdk-python',
     license='MIT License',
     author='APIBRASIL',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='contato@apibrasil.com.br',
     keywords='whatsapp api, apibrasil, cnpj, sms, cep, consulta, api, brasil, gratis, free, whatsapp, apiwhatsapp, apigratis, apifree',
```

