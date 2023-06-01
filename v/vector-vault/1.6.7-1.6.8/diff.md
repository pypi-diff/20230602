# Comparing `tmp/vector_vault-1.6.7.tar.gz` & `tmp/vector_vault-1.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-1.6.7.tar", last modified: Thu Jun  1 23:45:49 2023, max compression
+gzip compressed data, was "vector_vault-1.6.8.tar", last modified: Thu Jun  1 23:54:15 2023, max compression
```

## Comparing `vector_vault-1.6.7.tar` & `vector_vault-1.6.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-01 23:45:49.737955 vector_vault-1.6.7/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.6.7/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-01 23:45:49.737798 vector_vault-1.6.7/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    19356 2023-05-31 07:01:35.000000 vector_vault-1.6.7/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-01 23:45:49.737993 vector_vault-1.6.7/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-01 23:45:47.000000 vector_vault-1.6.7/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-01 23:45:49.735145 vector_vault-1.6.7/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-01 23:45:49.000000 vector_vault-1.6.7/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-06-01 23:45:49.000000 vector_vault-1.6.7/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-01 23:45:49.000000 vector_vault-1.6.7/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-01 23:45:49.000000 vector_vault-1.6.7/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-01 23:45:49.000000 vector_vault-1.6.7/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-01 23:45:49.737315 vector_vault-1.6.7/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-1.6.7/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)     7621 2023-06-01 06:30:30.000000 vector_vault-1.6.7/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3198 2023-06-01 23:45:17.000000 vector_vault-1.6.7/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1843 2023-05-30 20:06:58.000000 vector_vault-1.6.7/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.6.7/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1582 2023-06-01 23:45:23.000000 vector_vault-1.6.7/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.6.7/vectorvault/signup.py
--rw-r--r--   0 johnrood   (501) staff       (20)    19387 2023-06-01 23:45:10.000000 vector_vault-1.6.7/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3970 2023-05-31 06:48:55.000000 vector_vault-1.6.7/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.6.7/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-01 23:54:15.515844 vector_vault-1.6.8/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.6.8/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-01 23:54:15.515685 vector_vault-1.6.8/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    19356 2023-05-31 07:01:35.000000 vector_vault-1.6.8/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-01 23:54:15.515887 vector_vault-1.6.8/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-01 23:51:53.000000 vector_vault-1.6.8/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-01 23:54:15.512620 vector_vault-1.6.8/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-01 23:54:15.000000 vector_vault-1.6.8/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-06-01 23:54:15.000000 vector_vault-1.6.8/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-01 23:54:15.000000 vector_vault-1.6.8/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-01 23:54:15.000000 vector_vault-1.6.8/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-01 23:54:15.000000 vector_vault-1.6.8/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-01 23:54:15.515380 vector_vault-1.6.8/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-1.6.8/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     7621 2023-06-01 06:30:30.000000 vector_vault-1.6.8/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3198 2023-06-01 23:53:57.000000 vector_vault-1.6.8/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1854 2023-06-01 23:50:20.000000 vector_vault-1.6.8/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.6.8/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1582 2023-06-01 23:54:05.000000 vector_vault-1.6.8/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.6.8/vectorvault/signup.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    19379 2023-06-01 23:53:51.000000 vector_vault-1.6.8/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3970 2023-05-31 06:48:55.000000 vector_vault-1.6.8/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.6.8/vectorvault/wrap.py
```

### Comparing `vector_vault-1.6.7/LICENSE` & `vector_vault-1.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.7/PKG-INFO` & `vector_vault-1.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 1.6.7
+Version: 1.6.8
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.6.7/README.md` & `vector_vault-1.6.8/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.7/setup.py` & `vector_vault-1.6.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="1.6.7",
+    version="1.6.8",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-1.6.7/vector_vault.egg-info/PKG-INFO` & `vector_vault-1.6.8/vector_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 1.6.7
+Version: 1.6.8
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.6.7/vectorvault/__init__.py` & `vector_vault-1.6.8/vectorvault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.7/vectorvault/ai.py` & `vector_vault-1.6.8/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.7/vectorvault/cloudmanager.py` & `vector_vault-1.6.8/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.7/vectorvault/creds.py` & `vector_vault-1.6.8/vectorvault/creds.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,38 +19,38 @@
 
 class CustomCredentials(Credentials):
     def __init__(self, user, api):
         self.user = user
         self.api = api
         self.token = None
         self.expiry = None
-        self.refresh()
+        self.refresh(requests.Request())
 
     def apply(self, headers, token=None):
         headers["Authorization"] = f"Bearer {self.token}"
 
     @property
     def valid(self):
         if self.expiry is None:
             return False
         return datetime.datetime.now() < self.expiry
 
-    def refresh(self):
+    def refresh(self, request):
         if not self.valid:
             data = {
                 "user_id": self.user,
                 "api_key": self.api,
             }
-            response = requests.post('https://credentials.vectorvault.io/access', json=data)
+            response = requests.post('https://vv-creds-etrszydrna-uc.a.run.app/access', json=data)
             response.raise_for_status()  
             response_data = response.json()
             self.token = response_data['access_token']
             self.expiry = datetime.datetime.fromisoformat(response_data['expiry'])
 
-    def before_request(self, auth_request, method, url, request_headers):
-        self.apply(request_headers)
+    def before_request(self, request, method, url, headers):
+        self.apply(headers)
 
     def __getstate__(self):
         return self.__dict__.copy()
 
     def __setstate__(self, state):
-        self.__dict__.update(state)
+        self.__dict__.update(state)
```

### Comparing `vector_vault-1.6.7/vectorvault/download.py` & `vector_vault-1.6.8/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.7/vectorvault/itemize.py` & `vector_vault-1.6.8/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.7/vectorvault/signup.py` & `vector_vault-1.6.8/vectorvault/signup.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.7/vectorvault/vault.py` & `vector_vault-1.6.8/vectorvault/vault.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,27 +28,27 @@
 
 class Vault:
     def __init__(self, user: str = None, api_key: str = None, vault: str = None, dims: int = 1536, verbose: bool = False):
         self.vault = vault.strip() if vault else 'home'
         self.vectors = get_vectors(dims)
         self.api = api_key
         self.dims = dims
+        self.verbose = verbose
         try:
             self.cloud_manager = CloudManager(user, api_key, self.vault)
-            if self.verbose == True:
+            if self.verbose:
                 print(f'Connected vault: {self.vault}')
         except Exception as e:
             print('API KEY NOT FOUND! Using Vault without cloud access. `get_chat()` will still work', e)
             # user can still use the get_chat() function without an api key
             pass
         self.user = user
         self.x = 0
         self.x_checked = False
         self.vecs_loaded = False
-        self.verbose = verbose
         self.items = []
         self.last_time = None
         self.last_chat_time = None
         self.first_run = True
         self.needed_sleep_time = None
         self.saved_already = False
         self.ai = AI()
```

### Comparing `vector_vault-1.6.7/vectorvault/vecreq.py` & `vector_vault-1.6.8/vectorvault/vecreq.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.7/vectorvault/wrap.py` & `vector_vault-1.6.8/vectorvault/wrap.py`

 * *Files identical despite different names*

