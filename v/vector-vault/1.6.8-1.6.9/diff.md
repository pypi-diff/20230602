# Comparing `tmp/vector_vault-1.6.8.tar.gz` & `tmp/vector_vault-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-1.6.8.tar", last modified: Thu Jun  1 23:54:15 2023, max compression
+gzip compressed data, was "vector_vault-1.6.9.tar", last modified: Fri Jun  2 00:01:45 2023, max compression
```

## Comparing `vector_vault-1.6.8.tar` & `vector_vault-1.6.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-01 23:54:15.515844 vector_vault-1.6.8/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.6.8/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-01 23:54:15.515685 vector_vault-1.6.8/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    19356 2023-05-31 07:01:35.000000 vector_vault-1.6.8/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-01 23:54:15.515887 vector_vault-1.6.8/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-01 23:51:53.000000 vector_vault-1.6.8/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-01 23:54:15.512620 vector_vault-1.6.8/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-01 23:54:15.000000 vector_vault-1.6.8/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-06-01 23:54:15.000000 vector_vault-1.6.8/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-01 23:54:15.000000 vector_vault-1.6.8/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-01 23:54:15.000000 vector_vault-1.6.8/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-01 23:54:15.000000 vector_vault-1.6.8/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-01 23:54:15.515380 vector_vault-1.6.8/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-1.6.8/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)     7621 2023-06-01 06:30:30.000000 vector_vault-1.6.8/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3198 2023-06-01 23:53:57.000000 vector_vault-1.6.8/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1854 2023-06-01 23:50:20.000000 vector_vault-1.6.8/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.6.8/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1582 2023-06-01 23:54:05.000000 vector_vault-1.6.8/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.6.8/vectorvault/signup.py
--rw-r--r--   0 johnrood   (501) staff       (20)    19379 2023-06-01 23:53:51.000000 vector_vault-1.6.8/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3970 2023-05-31 06:48:55.000000 vector_vault-1.6.8/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.6.8/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-02 00:01:45.356590 vector_vault-1.6.9/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.6.9/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-02 00:01:45.356422 vector_vault-1.6.9/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    19356 2023-05-31 07:01:35.000000 vector_vault-1.6.9/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-02 00:01:45.356630 vector_vault-1.6.9/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-01 23:59:45.000000 vector_vault-1.6.9/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-02 00:01:45.353402 vector_vault-1.6.9/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-02 00:01:45.000000 vector_vault-1.6.9/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-06-02 00:01:45.000000 vector_vault-1.6.9/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-02 00:01:45.000000 vector_vault-1.6.9/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-02 00:01:45.000000 vector_vault-1.6.9/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-02 00:01:45.000000 vector_vault-1.6.9/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-02 00:01:45.356014 vector_vault-1.6.9/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-1.6.9/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     7621 2023-06-01 06:30:30.000000 vector_vault-1.6.9/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3198 2023-06-01 23:53:57.000000 vector_vault-1.6.9/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1854 2023-06-01 23:50:20.000000 vector_vault-1.6.9/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.6.9/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1582 2023-06-01 23:54:05.000000 vector_vault-1.6.9/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.6.9/vectorvault/signup.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    19675 2023-06-02 00:01:38.000000 vector_vault-1.6.9/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3970 2023-05-31 06:48:55.000000 vector_vault-1.6.9/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.6.9/vectorvault/wrap.py
```

### Comparing `vector_vault-1.6.8/LICENSE` & `vector_vault-1.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.8/PKG-INFO` & `vector_vault-1.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 1.6.8
+Version: 1.6.9
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.6.8/README.md` & `vector_vault-1.6.9/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.8/setup.py` & `vector_vault-1.6.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="1.6.8",
+    version="1.6.9",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-1.6.8/vector_vault.egg-info/PKG-INFO` & `vector_vault-1.6.9/vector_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 1.6.8
+Version: 1.6.9
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.6.8/vectorvault/__init__.py` & `vector_vault-1.6.9/vectorvault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.8/vectorvault/ai.py` & `vector_vault-1.6.9/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.8/vectorvault/cloudmanager.py` & `vector_vault-1.6.9/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.8/vectorvault/creds.py` & `vector_vault-1.6.9/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.8/vectorvault/download.py` & `vector_vault-1.6.9/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.8/vectorvault/itemize.py` & `vector_vault-1.6.9/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.8/vectorvault/signup.py` & `vector_vault-1.6.9/vectorvault/signup.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.8/vectorvault/vault.py` & `vector_vault-1.6.9/vectorvault/vault.py`

 * *Files 2% similar despite different names*

```diff
@@ -243,14 +243,16 @@
         start_time = time.time()
         if not self.last_time:
             self.last_time = start_time - 1
         
         if not self.needed_sleep_time:
             self.needed_sleep_time = 0
         
+        deduction = self.needed_sleep_time - (time.time() - self.last_chat_time)
+        self.needed_sleep_time = deduction if deduction > 0 else 0
         time.sleep(self.needed_sleep_time)
         
         texts = []
         text_len = 0
         for item in self.items:
             text = item['text']
             text_len += self.ai.get_tokens(text)
@@ -348,14 +350,16 @@
         
         if not self.needed_sleep_time:
             self.needed_sleep_time = 0
         
         if not history:
             history = ''
         
+        deduction = self.needed_sleep_time - (time.time() - self.last_chat_time)
+        self.needed_sleep_time = deduction if deduction > 0 else 0
         time.sleep(self.needed_sleep_time)
 
         if self.ai.get_tokens(text) > 4000:
             if summary:
                 inputs = self.split_text(text, 14500)
             else:
                 inputs = self.split_text(text)
```

### Comparing `vector_vault-1.6.8/vectorvault/vecreq.py` & `vector_vault-1.6.9/vectorvault/vecreq.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.8/vectorvault/wrap.py` & `vector_vault-1.6.9/vectorvault/wrap.py`

 * *Files identical despite different names*

