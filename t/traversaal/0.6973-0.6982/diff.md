# Comparing `tmp/traversaal-0.6973-py3-none-any.whl.zip` & `tmp/traversaal-0.6982-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4284 bytes, number of entries: 8
--rw-r--r--  2.0 unx     2307 b- defN 23-May-16 05:45 traversaal/SemanticSearch.py
+Zip file size: 4898 bytes, number of entries: 8
+-rw-r--r--  2.0 unx     4959 b- defN 23-May-30 17:28 traversaal/SemanticSearch.py
 -rw-r--r--  2.0 unx       73 b- defN 23-May-16 06:01 traversaal/__init__.py
 -rw-r--r--  2.0 unx       18 b- defN 23-May-16 06:01 traversaal/test.py
--rw-r--r--  2.0 unx     1059 b- defN 23-May-16 06:02 traversaal-0.6973.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     2478 b- defN 23-May-16 06:02 traversaal-0.6973.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-16 06:02 traversaal-0.6973.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-May-16 06:02 traversaal-0.6973.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      645 b- defN 23-May-16 06:02 traversaal-0.6973.dist-info/RECORD
-8 files, 6683 bytes uncompressed, 3152 bytes compressed:  52.8%
+-rw-r--r--  2.0 unx     1059 b- defN 23-Jun-02 06:26 traversaal-0.6982.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     2510 b- defN 23-Jun-02 06:26 traversaal-0.6982.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-02 06:26 traversaal-0.6982.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-02 06:26 traversaal-0.6982.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      645 b- defN 23-Jun-02 06:26 traversaal-0.6982.dist-info/RECORD
+8 files, 9367 bytes uncompressed, 3766 bytes compressed:  59.8%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: traversaal/__init__.py
 Comment: 
 
 Filename: traversaal/test.py
 Comment: 
 
-Filename: traversaal-0.6973.dist-info/LICENSE.txt
+Filename: traversaal-0.6982.dist-info/LICENSE.txt
 Comment: 
 
-Filename: traversaal-0.6973.dist-info/METADATA
+Filename: traversaal-0.6982.dist-info/METADATA
 Comment: 
 
-Filename: traversaal-0.6973.dist-info/WHEEL
+Filename: traversaal-0.6982.dist-info/WHEEL
 Comment: 
 
-Filename: traversaal-0.6973.dist-info/top_level.txt
+Filename: traversaal-0.6982.dist-info/top_level.txt
 Comment: 
 
-Filename: traversaal-0.6973.dist-info/RECORD
+Filename: traversaal-0.6982.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## traversaal/SemanticSearch.py

```diff
@@ -1,46 +1,81 @@
 # traversaal/semantic_search.py
 
 import warnings
 import torch
 from transformers import AutoTokenizer, AutoModel
+import time
+from sentence_transformers import SentenceTransformer
+from openai.embeddings_utils import get_embedding, cosine_similarity
 
 
 class SemanticSearch:
-    def __init__(self, model_name):
+    def __init__(self):
         warnings.filterwarnings("ignore")  # Hide warnings
-        self.tokenizer = AutoTokenizer.from_pretrained(model_name)
-        self.model = AutoModel.from_pretrained(model_name)
+        self.model = SentenceTransformer("sentence-transformers/all-mpnet-base-v2")
+        if not torch.cuda.is_available():
+            print("Warning: No GPU found. Please add GPU to your notebook")
+        else:
+            print(
+                """
+
+  _______ .______    __    __      _______   ______    __    __  .__   __.  _______   __  
+ /  _____||   _  \  |  |  |  |    |   ____| /  __  \  |  |  |  | |  \ |  | |       \ |  | 
+|  |  __  |  |_)  | |  |  |  |    |  |__   |  |  |  | |  |  |  | |   \|  | |  .--.  ||  | 
+|  | |_ | |   ___/  |  |  |  |    |   __|  |  |  |  | |  |  |  | |  . `  | |  |  |  ||  | 
+|  |__| | |  |      |  `--'  |    |  |     |  `--'  | |  `--'  | |  |\   | |  '--'  ||__| 
+ \______| | _|       \______/     |__|      \______/   \______/  |__| \__| |_______/ (__) 
+                                                                                          
+
+            
+            """
+            )
+            self.model = self.model.to("cuda")
 
     def encode(self, text):
         with warnings.catch_warnings():
-            warnings.filterwarnings("ignore")  # Hide warnings
-            inputs = self.tokenizer(
-                text, padding=True, truncation=True, return_tensors="pt"
-            )
-            with torch.no_grad():
-                outputs = self.model(**inputs)
-        embeddings = outputs.last_hidden_state[:, 0, :]
-        return embeddings.numpy()
+            embeddings = self.model.encode(text)
+
+        return embeddings
 
     def encode_data(self, df):
         encoded_data = df.copy()
+        print(
+            """
+
+.___________.__    __   __       _______.   .___  ___.      ___   ____    ____    .___________.    ___       __  ___  _______ 
+|           |  |  |  | |  |     /       |   |   \/   |     /   \  \   \  /   /    |           |   /   \     |  |/  / |   ____|
+`---|  |----|  |__|  | |  |    |   (----`   |  \  /  |    /  ^  \  \   \/   /     `---|  |----`  /  ^  \    |  '  /  |  |__   
+    |  |    |   __   | |  |     \   \       |  |\/|  |   /  /_\  \  \_    _/          |  |      /  /_\  \   |    <   |   __|  
+    |  |    |  |  |  | |  | .----)   |      |  |  |  |  /  _____  \   |  |            |  |     /  _____  \  |  .  \  |  |____ 
+    |__|    |__|  |__| |__| |_______/       |__|  |__| /__/     \__\  |__|            |__|    /__/     \__\ |__|\__\ |_______|
+                                                                                                                              
+     _______.  ______   .___  ___.  _______    .___________.__  .___  ___.  _______                                           
+    /       | /  __  \  |   \/   | |   ____|   |           |  | |   \/   | |   ____|                                          
+   |   (----`|  |  |  | |  \  /  | |  |__      `---|  |----|  | |  \  /  | |  |__                                             
+    \   \    |  |  |  | |  |\/|  | |   __|         |  |    |  | |  |\/|  | |   __|                                            
+.----)   |   |  `--'  | |  |  |  | |  |____        |  |    |  | |  |  |  | |  |____ __ __ __                                  
+|_______/     \______/  |__|  |__| |_______|       |__|    |__| |__|  |__| |_______(__(__(__)                                 
+                                                                                                                              
+
+        """
+        )
+        startTime = time.time()
         encoded_data["embedding"] = encoded_data["hotel_review"].apply(
             self.encode
         ) + encoded_data["hotel_description"].apply(self.encode)
+        executionTime = time.time() - startTime
+        print("Execution time in seconds: " + str(executionTime))
         return encoded_data
 
     def search(self, encoded_data, query):
+        # query_embedding = embedder.encode(query,show_progress_bar=True)
         query_embedding = self.encode(query)
         encoded_data["score"] = encoded_data["embedding"].apply(
-            lambda x: float(
-                torch.cosine_similarity(
-                    torch.Tensor(x), torch.Tensor(query_embedding)
-                ).numpy()
-            )
+            lambda x: cosine_similarity(x, query_embedding.reshape(768, -1))
         )
         encoded_data = encoded_data.sort_values(by="score", ascending=False)
 
         # Get relevant reviews
         # encoded_data["relevant_reviews"] = encoded_data.apply(
         #     lambda row: self.get_relevant_reviews(
         #         row["id"], row["hotel_name"], encoded_data, query
```

## Comparing `traversaal-0.6973.dist-info/LICENSE.txt` & `traversaal-0.6982.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `traversaal-0.6973.dist-info/METADATA` & `traversaal-0.6982.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traversaal
-Version: 0.6973
+Version: 0.6982
 Summary: A semantic search package for hotel data
 Home-page: https://github.com/hamzafarooq
 Author: Traversaal
 Author-email: hello@traversaal.com
 License: Apache License 2.0
 Keywords: Transformer Networks BERT XLNet sentence embedding PyTorch NLP deep learning
 Classifier: Development Status :: 5 - Production/Stable
@@ -24,35 +24,36 @@
 Requires-Dist: scipy
 Requires-Dist: nltk
 Requires-Dist: sentencepiece
 Requires-Dist: huggingface-hub (>=0.4.0)
 
 ## Traversaal
 
-Traversaal is a Python package that provides a simple semantic search functionality for hotel data. It leverages large language models such as BERT to encode hotel descriptions and reviews, allowing users to perform semantic search queries and retrieve relevant results based on the provided search query.
+Traversaal is a Python package that provides a simple semantic search functionality for hotel data. It leverages large language models such as mpnet to encode hotel descriptions and reviews, allowing users to perform semantic search queries and retrieve relevant results based on the provided search query.
 
 ## Features
 
 - Efficient semantic search for hotel data based on descriptions and reviews.
 - Utilizes state-of-the-art language models to encode and compare text embeddings.
 - Returns relevant search results with corresponding scores for ranking.
 - Supports GPU acceleration for faster encoding and search performance.
+- Utilizes distributed computing to increase speed in embedding creation
 
 ## Installation
 
 You can install Traversaal using pip:
 
 ```bash
 pip install traversaal
 
 import pandas as pd
 import traversaal
 
-model_name = 'bert-base-uncased'
-search = traversaal.SemanticSearch(model_name)
+
+search = traversaal.SemanticSearch()
 
 df = pd.read_csv('hotels.csv')
 encoded_data = search.encode_data(df)
 query = 'great location and service'
 
 relevant_results = search.search(encoded_data, query)
```

## Comparing `traversaal-0.6973.dist-info/RECORD` & `traversaal-0.6982.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-traversaal/SemanticSearch.py,sha256=tMlX5iV68KLgzrHT6ogJxrQDoaEgw-R8lQbT6OP8jVg,2307
+traversaal/SemanticSearch.py,sha256=1XON885ZAKvHclYeicVBewDSqBTGvduswHh0C-RjeGc,4959
 traversaal/__init__.py,sha256=gkHr2gZfrUJkesV2ZqxviiBUs5eFDAL9YjU8IZC4itM,73
 traversaal/test.py,sha256=2Q0ISpOirF3iJzLrdDxwmrX3oGLQgS4z2rQlekiYP9Q,18
-traversaal-0.6973.dist-info/LICENSE.txt,sha256=4ieZa9sI6QYkg-hmMvbEHhrYEXCqB6-GX4UNLHK0Qms,1059
-traversaal-0.6973.dist-info/METADATA,sha256=lUWRNie6gz3dp25GqtCOumDwxdDrmJamthHzazMqLA0,2478
-traversaal-0.6973.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-traversaal-0.6973.dist-info/top_level.txt,sha256=gA5p8wVpz8HudjDJ0q0F97At5EG7mwaHfDToON1pGYs,11
-traversaal-0.6973.dist-info/RECORD,,
+traversaal-0.6982.dist-info/LICENSE.txt,sha256=4ieZa9sI6QYkg-hmMvbEHhrYEXCqB6-GX4UNLHK0Qms,1059
+traversaal-0.6982.dist-info/METADATA,sha256=y9GxiPqFwhXbMahIzHMkFss716ehnGPqbaKj_mSTJcQ,2510
+traversaal-0.6982.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+traversaal-0.6982.dist-info/top_level.txt,sha256=gA5p8wVpz8HudjDJ0q0F97At5EG7mwaHfDToON1pGYs,11
+traversaal-0.6982.dist-info/RECORD,,
```

