# Comparing `tmp/vector_vault-1.6.5.tar.gz` & `tmp/vector_vault-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-1.6.5.tar", last modified: Thu Jun  1 21:44:38 2023, max compression
+gzip compressed data, was "vector_vault-1.6.6.tar", last modified: Thu Jun  1 22:25:26 2023, max compression
```

## Comparing `vector_vault-1.6.5.tar` & `vector_vault-1.6.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-01 21:44:38.622686 vector_vault-1.6.5/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.6.5/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-01 21:44:38.622516 vector_vault-1.6.5/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    19356 2023-05-31 07:01:35.000000 vector_vault-1.6.5/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-01 21:44:38.622721 vector_vault-1.6.5/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-01 21:44:19.000000 vector_vault-1.6.5/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-01 21:44:38.619806 vector_vault-1.6.5/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-01 21:44:38.000000 vector_vault-1.6.5/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-06-01 21:44:38.000000 vector_vault-1.6.5/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-01 21:44:38.000000 vector_vault-1.6.5/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-01 21:44:38.000000 vector_vault-1.6.5/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-01 21:44:38.000000 vector_vault-1.6.5/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-01 21:44:38.622189 vector_vault-1.6.5/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-1.6.5/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)     7621 2023-06-01 06:30:30.000000 vector_vault-1.6.5/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3249 2023-06-01 21:39:08.000000 vector_vault-1.6.5/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1843 2023-05-30 20:06:58.000000 vector_vault-1.6.5/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.6.5/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1582 2023-06-01 21:39:11.000000 vector_vault-1.6.5/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.6.5/vectorvault/signup.py
--rw-r--r--   0 johnrood   (501) staff       (20)    19247 2023-06-01 21:39:02.000000 vector_vault-1.6.5/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3970 2023-05-31 06:48:55.000000 vector_vault-1.6.5/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.6.5/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-01 22:25:26.904293 vector_vault-1.6.6/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.6.6/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-01 22:25:26.904116 vector_vault-1.6.6/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    19356 2023-05-31 07:01:35.000000 vector_vault-1.6.6/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-01 22:25:26.904334 vector_vault-1.6.6/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-01 22:25:21.000000 vector_vault-1.6.6/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-01 22:25:26.902182 vector_vault-1.6.6/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-01 22:25:26.000000 vector_vault-1.6.6/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-06-01 22:25:26.000000 vector_vault-1.6.6/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-01 22:25:26.000000 vector_vault-1.6.6/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-01 22:25:26.000000 vector_vault-1.6.6/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-01 22:25:26.000000 vector_vault-1.6.6/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-01 22:25:26.903886 vector_vault-1.6.6/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-1.6.6/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     7621 2023-06-01 06:30:30.000000 vector_vault-1.6.6/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3198 2023-06-01 22:20:47.000000 vector_vault-1.6.6/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1843 2023-05-30 20:06:58.000000 vector_vault-1.6.6/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.6.6/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1582 2023-06-01 21:39:11.000000 vector_vault-1.6.6/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.6.6/vectorvault/signup.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    19363 2023-06-01 22:24:57.000000 vector_vault-1.6.6/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3970 2023-05-31 06:48:55.000000 vector_vault-1.6.6/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.6.6/vectorvault/wrap.py
```

### Comparing `vector_vault-1.6.5/LICENSE` & `vector_vault-1.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.5/PKG-INFO` & `vector_vault-1.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 1.6.5
+Version: 1.6.6
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.6.5/README.md` & `vector_vault-1.6.6/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.5/setup.py` & `vector_vault-1.6.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="1.6.5",
+    version="1.6.6",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-1.6.5/vector_vault.egg-info/PKG-INFO` & `vector_vault-1.6.6/vector_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 1.6.5
+Version: 1.6.6
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.6.5/vectorvault/__init__.py` & `vector_vault-1.6.6/vectorvault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.5/vectorvault/ai.py` & `vector_vault-1.6.6/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.5/vectorvault/cloudmanager.py` & `vector_vault-1.6.6/vectorvault/cloudmanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,14 @@
         self.vault = vault
         # Creates the credentials
         credentials = CustomCredentials(user, self.api)
         # Instantiates the client 
         self.storage_client = storage.Client(project=call_proj(), credentials=credentials)
         self.cloud = self.storage_client.bucket(self.get_bkt(self.user))
         self.cloud_name = cloud_name
-        print(f'Connected to Vault: {self.vault}')
 
     def vault_exists(self, vault_name):
         return storage.Blob(bucket=self.cloud, name=vault_name).exists(self.storage_client)
 
     def upload_to_cloud(self, vault_name, content):
         blob = self.cloud.blob(vault_name)
         blob.upload_from_string(content)
```

### Comparing `vector_vault-1.6.5/vectorvault/creds.py` & `vector_vault-1.6.6/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.5/vectorvault/download.py` & `vector_vault-1.6.6/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.5/vectorvault/itemize.py` & `vector_vault-1.6.6/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.5/vectorvault/signup.py` & `vector_vault-1.6.6/vectorvault/signup.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.5/vectorvault/vault.py` & `vector_vault-1.6.6/vectorvault/vault.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,16 @@
     def __init__(self, user: str = None, api_key: str = None, vault: str = None, dims: int = 1536, verbose: bool = False):
         self.vault = vault.strip() if vault else 'home'
         self.vectors = get_vectors(dims)
         self.api = api_key
         self.dims = dims
         try:
             self.cloud_manager = CloudManager(user, api_key, self.vault)
+            if self.verbose == True:
+                print(f'Connected vault: {self.vault}')
         except Exception as e:
             print('API KEY NOT FOUND! Using Vault without cloud access. `get_chat()` will still work')
             # user can still use the get_chat() function without an api key
             pass
         self.user = user
         self.x = 0
         self.x_checked = False
@@ -424,15 +426,15 @@
             self.last_chat_time = start_time
 
         if self.verbose == True:
             print("get chat time --- %s seconds ---" % (time.time() - start_time))
 
         if return_context == False:
             return response
-        else:
+        elif return_context == True:
             return {'response': response, 'context': context}
         
 
     def print_stream(self, function):
         full_text= ''
         newlinetime=1
         for word in function:
```

### Comparing `vector_vault-1.6.5/vectorvault/vecreq.py` & `vector_vault-1.6.6/vectorvault/vecreq.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.5/vectorvault/wrap.py` & `vector_vault-1.6.6/vectorvault/wrap.py`

 * *Files identical despite different names*

