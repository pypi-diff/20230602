# Comparing `tmp/vector_vault-1.6.9.69.tar.gz` & `tmp/vector_vault-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-1.6.9.69.tar", last modified: Fri Jun  2 00:05:23 2023, max compression
+gzip compressed data, was "vector_vault-1.7.0.tar", last modified: Fri Jun  2 08:27:06 2023, max compression
```

## Comparing `vector_vault-1.6.9.69.tar` & `vector_vault-1.7.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-02 00:05:23.633906 vector_vault-1.6.9.69/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.6.9.69/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    20084 2023-06-02 00:05:23.633727 vector_vault-1.6.9.69/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    19356 2023-05-31 07:01:35.000000 vector_vault-1.6.9.69/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-02 00:05:23.633944 vector_vault-1.6.9.69/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1078 2023-06-02 00:05:12.000000 vector_vault-1.6.9.69/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-02 00:05:23.630813 vector_vault-1.6.9.69/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    20084 2023-06-02 00:05:23.000000 vector_vault-1.6.9.69/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-06-02 00:05:23.000000 vector_vault-1.6.9.69/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-02 00:05:23.000000 vector_vault-1.6.9.69/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-02 00:05:23.000000 vector_vault-1.6.9.69/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-02 00:05:23.000000 vector_vault-1.6.9.69/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-02 00:05:23.633373 vector_vault-1.6.9.69/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-1.6.9.69/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)     7621 2023-06-01 06:30:30.000000 vector_vault-1.6.9.69/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3198 2023-06-01 23:53:57.000000 vector_vault-1.6.9.69/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1854 2023-06-01 23:50:20.000000 vector_vault-1.6.9.69/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.6.9.69/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1582 2023-06-01 23:54:05.000000 vector_vault-1.6.9.69/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.6.9.69/vectorvault/signup.py
--rw-r--r--   0 johnrood   (501) staff       (20)    19670 2023-06-02 00:05:01.000000 vector_vault-1.6.9.69/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3970 2023-05-31 06:48:55.000000 vector_vault-1.6.9.69/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.6.9.69/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-02 08:27:06.842913 vector_vault-1.7.0/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.7.0/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-02 08:27:06.842729 vector_vault-1.7.0/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    19356 2023-05-31 07:01:35.000000 vector_vault-1.7.0/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-02 08:27:06.842955 vector_vault-1.7.0/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-02 08:27:00.000000 vector_vault-1.7.0/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-02 08:27:06.839743 vector_vault-1.7.0/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-02 08:27:06.000000 vector_vault-1.7.0/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-06-02 08:27:06.000000 vector_vault-1.7.0/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-02 08:27:06.000000 vector_vault-1.7.0/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-02 08:27:06.000000 vector_vault-1.7.0/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-02 08:27:06.000000 vector_vault-1.7.0/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-02 08:27:06.842321 vector_vault-1.7.0/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-1.7.0/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     7621 2023-06-01 06:30:30.000000 vector_vault-1.7.0/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3123 2023-06-02 08:26:16.000000 vector_vault-1.7.0/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1858 2023-06-02 08:00:20.000000 vector_vault-1.7.0/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.7.0/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1639 2023-06-02 08:26:22.000000 vector_vault-1.7.0/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.7.0/vectorvault/signup.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    27022 2023-06-02 08:26:36.000000 vector_vault-1.7.0/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3970 2023-05-31 06:48:55.000000 vector_vault-1.7.0/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.7.0/vectorvault/wrap.py
```

### Comparing `vector_vault-1.6.9.69/LICENSE` & `vector_vault-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.9.69/PKG-INFO` & `vector_vault-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 1.6.9.69
+Version: 1.7.0
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.6.9.69/README.md` & `vector_vault-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.9.69/setup.py` & `vector_vault-1.7.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="1.6.9.69",
+    version="1.7.0",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-1.6.9.69/vector_vault.egg-info/PKG-INFO` & `vector_vault-1.7.0/vector_vault.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 1.6.9.69
+Version: 1.7.0
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.6.9.69/vectorvault/__init__.py` & `vector_vault-1.7.0/vectorvault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.9.69/vectorvault/ai.py` & `vector_vault-1.7.0/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.9.69/vectorvault/cloudmanager.py` & `vector_vault-1.7.0/vectorvault/cloudmanager.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,23 +24,23 @@
 
 class CloudManager:
     def __init__(self, user: str, api_key: str, vault: str):
         self.user = user
         self.api = api_key
         self.vault = vault
         # Creates the credentials
-        credentials = CustomCredentials(user, self.api)
+        self.credentials = CustomCredentials(user, self.api)
         # Instantiates the client 
-        self.storage_client = storage.Client(project=call_proj(), credentials=credentials)
+        self.storage_client = storage.Client(project=call_proj(), credentials=self.credentials)
         self.cloud = self.storage_client.bucket(self.get_bkt(self.user))
         self.cloud_name = cloud_name
 
     def vault_exists(self, vault_name):
         return storage.Blob(bucket=self.cloud, name=vault_name).exists(self.storage_client)
-
+    
     def upload_to_cloud(self, vault_name, content):
         blob = self.cloud.blob(vault_name)
         blob.upload_from_string(content)
 
     def download_text_from_cloud(self, vault_name):
         blob = self.cloud.blob(vault_name)
         return blob.download_as_text()
@@ -53,17 +53,16 @@
     def download_to_temp_file(self, vault_name):
         with tempfile.NamedTemporaryFile(delete=False) as temp_file:
             blob = self.cloud.blob(vault_name)
             blob.download_to_filename(temp_file.name) 
             return temp_file.name
 
     def upload(self, item, text, meta):
-        with ThreadPoolExecutor() as executor:
-            executor.submit(self.upload_to_cloud, self.cloud_name(self.vault, item, self.user, self.api, item=True), text)
-            executor.submit(self.upload_to_cloud, self.cloud_name(self.vault, item, self.user, self.api, meta=True), json.dumps(meta))
+        self.upload_to_cloud(self.cloud_name(self.vault, item, self.user, self.api, item=True), text)
+        self.upload_to_cloud(self.cloud_name(self.vault, item, self.user, self.api, meta=True), json.dumps(meta))
     
     def delete_blob(self, blob):
         blob.delete()
      
     def get_bkt(self, input_string):
         return input_string.replace("@", "_at_").replace(".", "_dot_") + '_vvclient'
```

### Comparing `vector_vault-1.6.9.69/vectorvault/creds.py` & `vector_vault-1.7.0/vectorvault/creds.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def apply(self, headers, token=None):
         headers["Authorization"] = f"Bearer {self.token}"
 
     @property
     def valid(self):
         if self.expiry is None:
             return False
-        return datetime.datetime.now() < self.expiry
+        return datetime.datetime.utcnow() < self.expiry
 
     def refresh(self, request):
         if not self.valid:
             data = {
                 "user_id": self.user,
                 "api_key": self.api,
             }
@@ -49,8 +49,8 @@
     def before_request(self, request, method, url, headers):
         self.apply(headers)
 
     def __getstate__(self):
         return self.__dict__.copy()
 
     def __setstate__(self, state):
-        self.__dict__.update(state)
+        self.__dict__.update(state)
```

### Comparing `vector_vault-1.6.9.69/vectorvault/download.py` & `vector_vault-1.7.0/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.9.69/vectorvault/itemize.py` & `vector_vault-1.7.0/vectorvault/itemize.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import datetime 
 from .vecreq import call_name_vecs, call_buildpath
 from annoy import AnnoyIndex
 import threading
+from copy import deepcopy
 
 def itemize(vault, x, meta=None, text=None, name=None):
-    meta = {} if meta is None else meta
-
-    if 'name' not in meta and name is None:
-        name = f'{vault}-{x}'
-    elif name is not None:
-        name = __name__
+    meta = deepcopy(meta) if meta else {}
+    if 'name' not in meta and name is not None:
+        meta['name'] = name
+    elif name is None:
+        meta['name'] = f'{vault}-{x}'
     metaize(meta, name, x)
     return package(text, meta)
     
 def metaize(meta, name, x):
-    meta['name'] = name
+    meta['name'] = meta.get('name', name)
     meta['item_id'] = x  
     if 'created_at' not in meta:
         meta['created_at'] = datetime.datetime.utcnow().isoformat()
     if 'updated_at' not in meta:
         meta['updated_at'] = datetime.datetime.utcnow().isoformat()
 
 def package(text, meta):
```

### Comparing `vector_vault-1.6.9.69/vectorvault/signup.py` & `vector_vault-1.7.0/vectorvault/signup.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.9.69/vectorvault/vault.py` & `vector_vault-1.7.0/vectorvault/vault.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import numpy as np
 import tempfile
 import os
 import time
 import re
 import openai
-from concurrent.futures import ThreadPoolExecutor
+from concurrent.futures import ThreadPoolExecutor, as_completed
 from .cloudmanager import CloudManager
 from .ai import AI
 from .itemize import itemize, name_vecs, get_item, get_vectors
 from .vecreq import call_items_by_vector, call_get_total_vectors, call_get_vaults, call_get_similar, call_get_chat
 
 
 class Vault:
@@ -59,39 +59,44 @@
 
     def get_total_vectors(self):
         return call_get_total_vectors(self.user, self.vault, self.api)
     
     def save(self, trees=16):
         if self.saved_already == True:
             self.clear_cache()
-            print("The last save was aborted before the build finished. The cache was cleared and Save is empty now.")
+            print("The last save was aborted before build finished. Clearing cache to start again...")
         self.saved_already = True
         start_time = time.time()
         self.vectors.build(trees)
 
         total_saved_items = 0
-        for item in self.items:
-            item_text, item_id, item_meta = get_item(item)
-            self.cloud_manager.upload(item_id, item_text, item_meta)
-            total_saved_items += 1
+
+        with ThreadPoolExecutor() as executor:
+            for item in self.items:
+                item_text, item_id, item_meta = get_item(item)
+                executor.submit(self.cloud_manager.upload, item_id, item_text, item_meta)
+                total_saved_items += 1
 
         with tempfile.NamedTemporaryFile(delete=False) as temp_file:
             self.vectors.save(temp_file.name)
             byte = os.path.getsize(temp_file.name)
             self.cloud_manager.upload_temp_file(temp_file.name, name_vecs(self.vault, self.user, self.api, byte))
 
-        self.clear_cache()
+        self.items.clear()
+        self.x_checked = False
+        self.vecs_loaded = False
+        self.saved_already = False
 
         if self.verbose:
-            print("save vectors time --- %s seconds ---" % (time.time() - start_time))
+            print(f"upload time --- {(time.time() - start_time)} seconds --- {total_saved_items} items saved")
         
     def clear_cache(self):
-        self.items.clear()
-        self.x_checked = False
-        self.vecs_loaded = False
+        self.reload_vectors()
+        self.x_checked = True
+        self.vecs_loaded = True
         self.saved_already = False
 
     def delete(self):
         if self.verbose == True:
             print('Deleting started. Note: this can take a while for large datasets')
         # Clear the local vector data
         self.vectors = get_vectors(self.dims)
@@ -114,15 +119,24 @@
             self.vectors = new_index
         else:
             pass
         
         self.x_checked = True
         if self.verbose == True:
             print("initialize index --- %s seconds ---" % (time.time() - start_time))
-        
+    
+    def reload_vectors(self):
+            num_existing_items = self.vectors.get_n_items()
+            new_index = get_vectors(self.dims)
+            for i in range(num_existing_items):
+                vector = self.vectors.get_item_vector(i)
+                new_index.add_item(i, vector)
+            self.x = i + 1
+            self.vectors = new_index
+
     def load_vectors(self):
         start_time = time.time()
         temp_file_path = self.cloud_manager.download_to_temp_file(name_vecs(self.vault, self.user, self.api))
         self.vectors.load(temp_file_path)
         os.remove(temp_file_path)
         self.vecs_loaded = True
         if self.verbose:
@@ -166,40 +180,40 @@
     def get_similar_local(self, text, n: int = 4):
         vector = self.process_batch([text], never_stop=False, loop_timeout=180)[0]
         return call_items_by_vector(self.user, self.vault, self.api, vector, n)
     
     def get_similar(self, text, n: int = 4):
         return call_get_similar(self.user, self.vault, self.api, text, n)
 
-    def add_item(self, text: str, meta: dict = None, name: str = None):
+    def add_item(self, text: str, meta: dict = None, name: str = ''):
         """
             If your text length lenght is greater than 15000 characters, you should use Vault.split_text(your_text) to 
             get a list of text segments that are the right size
         """
         if self.x_checked == False:
             self.check_index()
         else: 
             pass
-
-        self.items.append(itemize(self.vault, self.x, meta, text, name))
+        
+        new_item = itemize(self.vault, self.x, meta, text, name)
+        self.items.append(new_item)
         self.x += 1
 
-    def add(self, text: str, meta: dict = None, name: str = None):
+    def add(self, text: str, meta: dict = None, name: str = ''):
         """
             If your text length lenght is greater than 4000 tokens, Vault.split_text(your_text)  
             will automatically be added
         """
 
         if self.ai.get_tokens(text) > 4000:
             if self.verbose == True:
                 print('Text length too long. Using the built-in "split_text()" function to get a list of text segments') 
             texts = self.split_text(text) # returns list of text segments
         else:
             texts = [text]
-
         for text in texts:
             self.add_item(text, meta, name)
 
     def add_item_with_vector(self, text: str, vector: list, meta: dict = None, name: str = None):
         """
             If your text length lenght is greater than 15000 characters, you should use Vault.split_text(your_text) to 
             get a list of text segments that are the right size
@@ -275,15 +289,15 @@
                 print(f'Projected Tokens per min:{projected_tokens_per_min} | Rate Limit Ratio: {rate_ratio} | Text Length: {text_len}')
             # 1 min divided by the cap per min and the total we are sending now and factor in the last trip time
             self.needed_sleep_time = 60 / (350000 / text_len) - trip_time 
             if self.needed_sleep_time < 0:
                 self.needed_sleep_time = 0
 
             if self.verbose == True:
-                print(f"Time calc'd to sleep: {self.needed_sleep_time}")
+                print(f"Sleep time needed to stay under Rate Limit: {self.needed_sleep_time}")
             if req_min > 3500:
                 time.sleep(1)
 
         # Process the batches in parallel using ThreadPoolExecutor
         with ThreadPoolExecutor() as executor:
             process_batch_with_params = lambda batch_text_chunks: self.process_batch(batch_text_chunks, never_stop, loop_timeout)
             batch_embeddings_list = list(executor.map(process_batch_with_params, batches_text_chunks))
@@ -299,15 +313,15 @@
         self.first_run = False
         if self.verbose == True:
             print("get vectors time --- %s seconds ---" % (time.time() - start_time))
 
     def get_chat_cloud(self, text: str, history: str = None, summary: bool = False, get_context = False, n_context = 4, return_context = False, expansion = False, history_search = False, model='gpt-3.5-turbo', include_context_meta=False):
         return call_get_chat(self.user, self.vault, self.api, text, history, summary, get_context, n_context, return_context, expansion, history_search, model, include_context_meta)
     
-    def get_chat(self, text: str, history: str = None, summary: bool = False, get_context = False, n_context = 4, return_context = False, expansion = False, history_search = False, model='gpt-3.5-turbo', include_context_meta=False, stream=False):
+    def get_chat(self, text: str, history: str = None, summary: bool = False, get_context = False, n_context = 4, return_context = False, expansion = False, history_search = False, model='gpt-3.5-turbo', include_context_meta=False):
         '''
             Chat get response from OpenAI's ChatGPT. 
             Rate limiting, auto retries, and chat histroy slicing built-in so you can chat with ease. 
             Enter your text, add optional chat history, and optionally choose a summary response (default: summmary = False)
 
             Example Signle Usage: 
             `response = vault.get_chat(text)`
@@ -407,25 +421,159 @@
                             context = self.get_similar(user_input, n=n_context)
                             input_ = str(context)
                         else:
                             context = self.get_similar(user_input, n=n_context)
                             input_ = ''
                             for text in context:
                                 input_ += text['data']
-                        if stream == False:
-                            response = self.ai.llm_w_context(segment, input_, history, model=model)
-                        elif stream == True:
-                            for word in self.ai.llm_w_context(segment, input_, history, model=model, stream=True):
-                                yield word
+                        response = self.ai.llm_w_context(segment, input_, history, model=model)
                     else:
-                        if stream == False:
-                            response = self.ai.llm(segment, history, model=model)
-                        elif stream == True:
-                            for word in self.ai.llm(segment, history, model=model, stream=True):
-                                yield word
+                        response = self.ai.llm(segment, history, model=model)
+                    break
+                except Exception as e:
+                    print(f"API Error: {e}. Sleeping 5 seconds")
+                    time.sleep(5)
+                    
+            self.last_chat_time = start_time
+
+        if self.verbose == True:
+            print("get chat time --- %s seconds ---" % (time.time() - start_time))
+
+        if return_context == False:
+            return response
+        elif return_context == True:
+            return {'response': response, 'context': context}
+        
+    def get_chat_stream(self, text: str, history: str = None, summary: bool = False, get_context = False, n_context = 4, return_context = False, expansion = False, history_search = False, model='gpt-3.5-turbo', include_context_meta=False, metatag=False, metatag_prefixes=False, metatag_suffixes=False):
+        '''
+            Chat get response from OpenAI's ChatGPT. 
+            Rate limiting, auto retries, and chat histroy slicing built-in so you can chat with ease. 
+            Enter your text, add optional chat history, and optionally choose a summary response (default: summmary = False)
+
+            Example Signle Usage: 
+            `response = vault.get_chat(text)`
+
+            Example Chat: 
+            `response = vault.get_chat(text, chat_history)`
+            
+            Example Summary: 
+            `summary = vault.get_chat(text, summary=True)`
+
+            Example Context-Based Response:
+            `response = vault.get_chat(text, get_context = True)`
+
+            Example Context-Based Response w/ Chat History:
+            `response = vault.get_chat(text, chat_history, get_context = True)`
+
+            Example Context-Response with Context Samples Returned:
+            `vault_response = vault.get_chat(text, get_context = True, return_context = True)`
+            
+            Response is a string, unless return_context == True, then response will be a dictionary 
+
+            Example to print dictionary results:
+            # print response:
+            `print(vault_response['response'])` 
+
+            # print context:
+            for item in vault_response['context']['results']:
+                print("\n\n", f"item {item['metadata']['item_index']}")
+                print(item['data'])
+
+            Default `expansion = False` can be set to True to create additional context from user input for vector retrieval. Allowing for greater search accuracy if
+            user input is too short or lacks the specificity needed for a quality retrieval search. ('expansion' is not context-aware). Default is good.
+
+            history_search is False by default skip adding the history of the conversation to the question to retrieval search 
+        '''
+
+        start_time = time.time()
+        if not self.last_chat_time:
+            self.last_chat_time = start_time - 20
+        
+        if not self.needed_sleep_time:
+            self.needed_sleep_time = 0
+        
+        if not history:
+            history = ''
+        
+        deduction = self.needed_sleep_time - (time.time() - self.last_chat_time)
+        self.needed_sleep_time = deduction if deduction > 0 else 0
+        time.sleep(self.needed_sleep_time)
+
+        if self.ai.get_tokens(text) > 4000:
+            if summary:
+                inputs = self.split_text(text, 14500)
+            else:
+                inputs = self.split_text(text)
+        else:
+            inputs = [text]
+        response = ''
+        for segment in inputs:
+            start_time = time.time()
+            seg_len = self.ai.get_tokens(segment)
+            # max 90,000 tokens per minute | max requests per minute = 3500
+            trip_time = float(start_time - self.last_chat_time)
+            req_min = 60 / trip_time # 1 min (60) / time between requests (trip_time)
+            projected_tokens_per_min = req_min * seg_len
+            rate_ratio = projected_tokens_per_min / 90000
+            if self.verbose == True:
+                print(f'Projected Tokens per min:{projected_tokens_per_min} | Rate Limit Ratio: {rate_ratio} | Text Length: {seg_len}')
+            # 1 min divided by the cap per min and the total we are sending now and factor in the last trip time
+            if seg_len == 0:
+                raise('No input. Add text input to continue')
+            self.needed_sleep_time = 60 / (90000 / seg_len) - trip_time 
+            if self.needed_sleep_time < 0:
+                self.needed_sleep_time = 0
+            if self.verbose == True:
+                print(f"Time calc'd to sleep: {self.needed_sleep_time}")
+
+            if expansion:
+                iq = f"be direct and short. Question: {segment} \n The intent of this question is to: "
+                intent_expansion = self.ai.llm(iq)
+                kq = f"be general, direct, and short. Don't give an answer, only topics this question falls under to this question: {segment}"
+                knowledge_expansion = self.ai.llm(kq)
+                segment = f'question_intent: {intent_expansion} | {knowledge_expansion}\n\
+                Question: {segment}'
+
+            while True:
+                try:
+                    if summary and not get_context:
+                        response += self.ai.summarize(segment, model=model)
+                    elif get_context and not summary:
+                        user_input = segment + history if history_search else segment
+                        if self.ai.get_tokens(user_input) > 4000:
+                            user_input = user_input[-16000:]
+                        if self.ai.get_tokens(user_input) > 4000:
+                            user_input = user_input[-15000:]
+                        if include_context_meta:
+                            context = self.get_similar(user_input, n=n_context)
+                            input_ = str(context)
+                        else:
+                            context = self.get_similar(user_input, n=n_context)
+                            input_ = ''
+                        for text in context:
+                            input_ += text['data']
+                        for word in self.ai.llm_w_context(segment, input_, history, model=model, stream=True):
+                            yield word
+                        for item in context:
+                            if type(metatag) is not list:
+                                for tag in item['metadata']:
+                                    yield str(item['metadata'][f'{tag}'])
+                            else:
+                                if metatag_prefixes:
+                                    if metatag_suffixes:
+                                        for i in range(len(metatag)):
+                                            yield str(metatag_prefixes[i]) + str(item['metadata'][f'{metatag[i]}']) + str(metatag_suffixes[i])
+                                    else:
+                                        for i in range(len(metatag)):
+                                            yield str(metatag_prefixes[i]) + str(item['metadata'][f'{metatag[i]}'])
+                            
+                            yield item['data']
+                    else:
+                        for word in self.ai.llm(segment, history, model=model, stream=True):
+                            yield word
                     break
                 except Exception as e:
                     print(f"API Error: {e}. Sleeping 5 seconds")
                     time.sleep(5)
                     
             self.last_chat_time = start_time
 
@@ -439,21 +587,20 @@
         
 
     def print_stream(self, function):
         full_text= ''
         newlinetime=1
         for word in function:
             full_text += word
-            self.print_stream(word) 
+            print(word, end='', flush=True) 
             if len(full_text) / 80 > newlinetime:
                 newlinetime += 1
                 print('\n', end='', flush=True)
     
             
     def cloud_stream(self, function):
         for word in function:
             try:
                 word = word.replace('\n', '<br/>')
                 yield f"data: {word} \n\n"
             except:
                 yield f"data: {word} \n\n"
-
```

### Comparing `vector_vault-1.6.9.69/vectorvault/vecreq.py` & `vector_vault-1.7.0/vectorvault/vecreq.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.9.69/vectorvault/wrap.py` & `vector_vault-1.7.0/vectorvault/wrap.py`

 * *Files identical despite different names*

