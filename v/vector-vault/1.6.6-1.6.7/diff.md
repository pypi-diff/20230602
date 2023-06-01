# Comparing `tmp/vector_vault-1.6.6.tar.gz` & `tmp/vector_vault-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-1.6.6.tar", last modified: Thu Jun  1 22:25:26 2023, max compression
+gzip compressed data, was "vector_vault-1.6.7.tar", last modified: Thu Jun  1 23:45:49 2023, max compression
```

## Comparing `vector_vault-1.6.6.tar` & `vector_vault-1.6.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-01 22:25:26.904293 vector_vault-1.6.6/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.6.6/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-01 22:25:26.904116 vector_vault-1.6.6/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    19356 2023-05-31 07:01:35.000000 vector_vault-1.6.6/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-01 22:25:26.904334 vector_vault-1.6.6/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-01 22:25:21.000000 vector_vault-1.6.6/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-01 22:25:26.902182 vector_vault-1.6.6/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-01 22:25:26.000000 vector_vault-1.6.6/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-06-01 22:25:26.000000 vector_vault-1.6.6/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-01 22:25:26.000000 vector_vault-1.6.6/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-01 22:25:26.000000 vector_vault-1.6.6/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-01 22:25:26.000000 vector_vault-1.6.6/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-01 22:25:26.903886 vector_vault-1.6.6/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-1.6.6/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)     7621 2023-06-01 06:30:30.000000 vector_vault-1.6.6/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3198 2023-06-01 22:20:47.000000 vector_vault-1.6.6/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1843 2023-05-30 20:06:58.000000 vector_vault-1.6.6/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.6.6/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1582 2023-06-01 21:39:11.000000 vector_vault-1.6.6/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.6.6/vectorvault/signup.py
--rw-r--r--   0 johnrood   (501) staff       (20)    19363 2023-06-01 22:24:57.000000 vector_vault-1.6.6/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3970 2023-05-31 06:48:55.000000 vector_vault-1.6.6/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.6.6/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-01 23:45:49.737955 vector_vault-1.6.7/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.6.7/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-01 23:45:49.737798 vector_vault-1.6.7/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    19356 2023-05-31 07:01:35.000000 vector_vault-1.6.7/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-01 23:45:49.737993 vector_vault-1.6.7/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-01 23:45:47.000000 vector_vault-1.6.7/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-01 23:45:49.735145 vector_vault-1.6.7/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-01 23:45:49.000000 vector_vault-1.6.7/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-06-01 23:45:49.000000 vector_vault-1.6.7/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-01 23:45:49.000000 vector_vault-1.6.7/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-01 23:45:49.000000 vector_vault-1.6.7/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-01 23:45:49.000000 vector_vault-1.6.7/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-01 23:45:49.737315 vector_vault-1.6.7/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-1.6.7/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     7621 2023-06-01 06:30:30.000000 vector_vault-1.6.7/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3198 2023-06-01 23:45:17.000000 vector_vault-1.6.7/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1843 2023-05-30 20:06:58.000000 vector_vault-1.6.7/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.6.7/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1582 2023-06-01 23:45:23.000000 vector_vault-1.6.7/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.6.7/vectorvault/signup.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    19387 2023-06-01 23:45:10.000000 vector_vault-1.6.7/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3970 2023-05-31 06:48:55.000000 vector_vault-1.6.7/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.6.7/vectorvault/wrap.py
```

### Comparing `vector_vault-1.6.6/LICENSE` & `vector_vault-1.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.6/PKG-INFO` & `vector_vault-1.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 1.6.6
+Version: 1.6.7
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.6.6/README.md` & `vector_vault-1.6.7/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.6/setup.py` & `vector_vault-1.6.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="1.6.6",
+    version="1.6.7",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-1.6.6/vector_vault.egg-info/PKG-INFO` & `vector_vault-1.6.7/vector_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 1.6.6
+Version: 1.6.7
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.6.6/vectorvault/__init__.py` & `vector_vault-1.6.7/vectorvault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.6/vectorvault/ai.py` & `vector_vault-1.6.7/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.6/vectorvault/cloudmanager.py` & `vector_vault-1.6.7/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.6/vectorvault/creds.py` & `vector_vault-1.6.7/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.6/vectorvault/download.py` & `vector_vault-1.6.7/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.6/vectorvault/itemize.py` & `vector_vault-1.6.7/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.6/vectorvault/signup.py` & `vector_vault-1.6.7/vectorvault/signup.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.6/vectorvault/vault.py` & `vector_vault-1.6.7/vectorvault/vault.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         self.api = api_key
         self.dims = dims
         try:
             self.cloud_manager = CloudManager(user, api_key, self.vault)
             if self.verbose == True:
                 print(f'Connected vault: {self.vault}')
         except Exception as e:
-            print('API KEY NOT FOUND! Using Vault without cloud access. `get_chat()` will still work')
+            print('API KEY NOT FOUND! Using Vault without cloud access. `get_chat()` will still work', e)
             # user can still use the get_chat() function without an api key
             pass
         self.user = user
         self.x = 0
         self.x_checked = False
         self.vecs_loaded = False
         self.verbose = verbose
@@ -397,24 +397,24 @@
                         user_input = segment + history if history_search else segment
                         if self.ai.get_tokens(user_input) > 4000:
                             user_input = user_input[-16000:]
                         if self.ai.get_tokens(user_input) > 4000:
                             user_input = user_input[-15000:]
                         if include_context_meta:
                             context = self.get_similar(user_input, n=n_context)
-                            input = str(context)
+                            input_ = str(context)
                         else:
                             context = self.get_similar(user_input, n=n_context)
-                            input = ''
+                            input_ = ''
                             for text in context:
-                                input += text['data']
+                                input_ += text['data']
                         if stream == False:
-                            response = self.ai.llm_w_context(segment, input, history, model=model)
+                            response = self.ai.llm_w_context(segment, input_, history, model=model)
                         elif stream == True:
-                            for word in self.ai.llm_w_context(segment, input, history, model=model, stream=True):
+                            for word in self.ai.llm_w_context(segment, input_, history, model=model, stream=True):
                                 yield word
                     else:
                         if stream == False:
                             response = self.ai.llm(segment, history, model=model)
                         elif stream == True:
                             for word in self.ai.llm(segment, history, model=model, stream=True):
                                 yield word
@@ -447,9 +447,9 @@
             
     def cloud_stream(self, function):
         for word in function:
             try:
                 word = word.replace('\n', '<br/>')
                 yield f"data: {word} \n\n"
             except:
-                yield word
+                yield f"data: {word} \n\n"
```

### Comparing `vector_vault-1.6.6/vectorvault/vecreq.py` & `vector_vault-1.6.7/vectorvault/vecreq.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.6/vectorvault/wrap.py` & `vector_vault-1.6.7/vectorvault/wrap.py`

 * *Files identical despite different names*

