# Comparing `tmp/pointstorm-1.1.3.tar.gz` & `tmp/pointstorm-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pointstorm-1.1.3.tar", last modified: Sat May 20 01:20:48 2023, max compression
+gzip compressed data, was "pointstorm-1.1.4.tar", last modified: Fri Jun  2 19:49:59 2023, max compression
```

## Comparing `pointstorm-1.1.3.tar` & `pointstorm-1.1.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-05-20 01:20:48.003048 pointstorm-1.1.3/
--rw-r--r--   0 tesfa      (501) staff       (20)    11357 2023-04-16 03:52:15.000000 pointstorm-1.1.3/LICENSE
--rw-r--r--   0 tesfa      (501) staff       (20)    13576 2023-05-20 01:20:48.002847 pointstorm-1.1.3/PKG-INFO
--rw-r--r--   0 tesfa      (501) staff       (20)      737 2023-05-20 01:17:30.000000 pointstorm-1.1.3/README.md
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-05-20 01:20:48.000657 pointstorm-1.1.3/pointstorm/
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 03:52:45.000000 pointstorm-1.1.3/pointstorm/__init__.py
--rw-r--r--   0 tesfa      (501) staff       (20)      363 2023-04-16 22:54:08.000000 pointstorm-1.1.3/pointstorm/config.py
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-05-20 01:20:48.001502 pointstorm-1.1.3/pointstorm/destinations/
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:51:39.000000 pointstorm-1.1.3/pointstorm/destinations/__init__.py
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-05-20 01:20:48.002058 pointstorm-1.1.3/pointstorm/embedding/
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:21:31.000000 pointstorm-1.1.3/pointstorm/embedding/__init__.py
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 22:40:54.000000 pointstorm-1.1.3/pointstorm/embedding/abstract.py
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 22:40:36.000000 pointstorm-1.1.3/pointstorm/embedding/image.py
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 22:40:29.000000 pointstorm-1.1.3/pointstorm/embedding/text.py
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 22:40:42.000000 pointstorm-1.1.3/pointstorm/embedding/time.py
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-05-20 01:20:48.002187 pointstorm-1.1.3/pointstorm/ingestion/
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-05-20 00:59:06.000000 pointstorm-1.1.3/pointstorm/ingestion/__init__.py
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-05-20 01:20:48.002412 pointstorm-1.1.3/pointstorm/ingestion/cdc/
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:50:52.000000 pointstorm-1.1.3/pointstorm/ingestion/cdc/__init__.py
--rw-r--r--   0 tesfa      (501) staff       (20)       78 2023-04-30 00:19:04.000000 pointstorm-1.1.3/pointstorm/ingestion/cdc/debezium.py
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-05-20 01:20:48.002637 pointstorm-1.1.3/pointstorm/ingestion/event/
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:02:57.000000 pointstorm-1.1.3/pointstorm/ingestion/event/__init__.py
--rw-r--r--   0 tesfa      (501) staff       (20)     3695 2023-05-20 01:14:17.000000 pointstorm-1.1.3/pointstorm/ingestion/event/kafka.py
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 04:50:18.000000 pointstorm-1.1.3/pointstorm/monitoring.py
--rw-r--r--   0 tesfa      (501) staff       (20)       62 2023-04-30 00:21:05.000000 pointstorm-1.1.3/pointstorm/reference_db.py
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-05-20 01:20:48.001366 pointstorm-1.1.3/pointstorm.egg-info/
--rw-r--r--   0 tesfa      (501) staff       (20)    13576 2023-05-20 01:20:47.000000 pointstorm-1.1.3/pointstorm.egg-info/PKG-INFO
--rw-r--r--   0 tesfa      (501) staff       (20)      678 2023-05-20 01:20:47.000000 pointstorm-1.1.3/pointstorm.egg-info/SOURCES.txt
--rw-r--r--   0 tesfa      (501) staff       (20)        1 2023-05-20 01:20:47.000000 pointstorm-1.1.3/pointstorm.egg-info/dependency_links.txt
--rw-r--r--   0 tesfa      (501) staff       (20)       94 2023-05-20 01:20:47.000000 pointstorm-1.1.3/pointstorm.egg-info/requires.txt
--rw-r--r--   0 tesfa      (501) staff       (20)       11 2023-05-20 01:20:47.000000 pointstorm-1.1.3/pointstorm.egg-info/top_level.txt
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:22:49.000000 pointstorm-1.1.3/pyproject.toml
--rw-r--r--   0 tesfa      (501) staff       (20)       38 2023-05-20 01:20:48.003099 pointstorm-1.1.3/setup.cfg
--rw-r--r--   0 tesfa      (501) staff       (20)     1010 2023-05-20 01:20:43.000000 pointstorm-1.1.3/setup.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 19:49:59.724818 pointstorm-1.1.4/
+-rw-r--r--   0 tesfa      (501) staff       (20)    11357 2023-04-16 03:52:15.000000 pointstorm-1.1.4/LICENSE
+-rw-r--r--   0 tesfa      (501) staff       (20)    13576 2023-06-02 19:49:59.724614 pointstorm-1.1.4/PKG-INFO
+-rw-r--r--   0 tesfa      (501) staff       (20)      737 2023-05-20 01:17:30.000000 pointstorm-1.1.4/README.md
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 19:49:59.721956 pointstorm-1.1.4/pointstorm/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 03:52:45.000000 pointstorm-1.1.4/pointstorm/__init__.py
+-rw-r--r--   0 tesfa      (501) staff       (20)      363 2023-04-16 22:54:08.000000 pointstorm-1.1.4/pointstorm/config.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 19:49:59.723030 pointstorm-1.1.4/pointstorm/destinations/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:51:39.000000 pointstorm-1.1.4/pointstorm/destinations/__init__.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 19:49:59.723641 pointstorm-1.1.4/pointstorm/embedding/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:21:31.000000 pointstorm-1.1.4/pointstorm/embedding/__init__.py
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 22:40:54.000000 pointstorm-1.1.4/pointstorm/embedding/abstract.py
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 22:40:36.000000 pointstorm-1.1.4/pointstorm/embedding/image.py
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 22:40:29.000000 pointstorm-1.1.4/pointstorm/embedding/text.py
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 22:40:42.000000 pointstorm-1.1.4/pointstorm/embedding/time.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 19:49:59.723740 pointstorm-1.1.4/pointstorm/ingestion/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-05-20 00:59:06.000000 pointstorm-1.1.4/pointstorm/ingestion/__init__.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 19:49:59.723945 pointstorm-1.1.4/pointstorm/ingestion/cdc/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:50:52.000000 pointstorm-1.1.4/pointstorm/ingestion/cdc/__init__.py
+-rw-r--r--   0 tesfa      (501) staff       (20)       78 2023-04-30 00:19:04.000000 pointstorm-1.1.4/pointstorm/ingestion/cdc/debezium.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 19:49:59.724357 pointstorm-1.1.4/pointstorm/ingestion/event/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:02:57.000000 pointstorm-1.1.4/pointstorm/ingestion/event/__init__.py
+-rw-r--r--   0 tesfa      (501) staff       (20)     3732 2023-06-02 19:44:33.000000 pointstorm-1.1.4/pointstorm/ingestion/event/kafka.py
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 04:50:18.000000 pointstorm-1.1.4/pointstorm/monitoring.py
+-rw-r--r--   0 tesfa      (501) staff       (20)       62 2023-04-30 00:21:05.000000 pointstorm-1.1.4/pointstorm/reference_db.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 19:49:59.722881 pointstorm-1.1.4/pointstorm.egg-info/
+-rw-r--r--   0 tesfa      (501) staff       (20)    13576 2023-06-02 19:49:59.000000 pointstorm-1.1.4/pointstorm.egg-info/PKG-INFO
+-rw-r--r--   0 tesfa      (501) staff       (20)      678 2023-06-02 19:49:59.000000 pointstorm-1.1.4/pointstorm.egg-info/SOURCES.txt
+-rw-r--r--   0 tesfa      (501) staff       (20)        1 2023-06-02 19:49:59.000000 pointstorm-1.1.4/pointstorm.egg-info/dependency_links.txt
+-rw-r--r--   0 tesfa      (501) staff       (20)       94 2023-06-02 19:49:59.000000 pointstorm-1.1.4/pointstorm.egg-info/requires.txt
+-rw-r--r--   0 tesfa      (501) staff       (20)       11 2023-06-02 19:49:59.000000 pointstorm-1.1.4/pointstorm.egg-info/top_level.txt
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:22:49.000000 pointstorm-1.1.4/pyproject.toml
+-rw-r--r--   0 tesfa      (501) staff       (20)       38 2023-06-02 19:49:59.724869 pointstorm-1.1.4/setup.cfg
+-rw-r--r--   0 tesfa      (501) staff       (20)     1010 2023-05-20 01:20:43.000000 pointstorm-1.1.4/setup.py
```

### Comparing `pointstorm-1.1.3/LICENSE` & `pointstorm-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pointstorm-1.1.3/PKG-INFO` & `pointstorm-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pointstorm
-Version: 1.1.3
+Version: 1.1.4
 Summary: Embedding vectors for data on the move
 Home-page: https://github.com/xsfa/pointstorm
 Author: xsfa
 Author-email: tesfaaog@gmail.com
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `pointstorm-1.1.3/README.md` & `pointstorm-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pointstorm-1.1.3/pointstorm/ingestion/event/kafka.py` & `pointstorm-1.1.4/pointstorm/ingestion/event/kafka.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 # Generic imports
 import json
 import logging
 import warnings
+import os
 warnings.filterwarnings(action = 'ignore')
 
 # Ingestion Imports
-from bytewax import Dataflow, cluster_main, spawn_cluster
-from bytewax.inputs import KafkaInputConfig
-from kafka import KafkaConsumer, TopicPartition
+from bytewax.testing import run_main
+from bytewax.dataflow import Dataflow
+from bytewax.connectors.kafka import KafkaInput
+from bytewax.connectors.stdio import StdOutput
+# from kafka import KafkaConsumer, TopicPartition
 
 # ML imports
 from transformers import AutoTokenizer, AutoModel
 import torch
 
 # Local imports
 from pointstorm.config import abstract_logger as kafka_logger
@@ -26,16 +29,16 @@
         self.kafka_group_id = kafka_group_id
         self.text_field = text_field
         self.model_name = huggingface_model_name
         self.tokenizer = AutoTokenizer.from_pretrained(self.model_name)
         self.model = AutoModel.from_pretrained(self.model_name)
         # self.previous_messages = self.get_previous_messages()
 
-    def set_topic(self, kafka_topic):
-        self.kafka_topic = kafka_topic
+    #     def set_topic(self, kafka_topic):
+    #         self.kafka_topic = kafka_topic
 
     # def get_previous_messages(self):
     #     previous_messages = []
 
     #     consumer = KafkaConsumer(
     #         self.kafka_topic,
     #         bootstrap_servers=self.kafka_bootstrap_server,
@@ -75,29 +78,25 @@
         inputs = self.tokenizer(message, return_tensors="pt", padding=True, truncation=True)
 
         with torch.no_grad():
             outputs = self.model(**inputs)
 
         embeddings = outputs.last_hidden_state.mean(dim=1).numpy()
         kafka_logger.info(f"Generated embeddings for message: {message}, {embeddings}")
-
+    
     def run(self):
+        input_config = KafkaInput(
+            brokers=[self.kafka_bootstrap_server],
+            topics=[self.kafka_topic],
+            add_config={
+                'group.id': self.kafka_group_id,
+                'auto.offset.reset': 'earliest',
+                'enable.auto.commit': True
+            }
+        )
+
         kafka_logger.info("Started KafkaTextEmbeddings for topic: " + self.kafka_topic)
         flow = Dataflow()
-
+        flow.input(self.kafka_topic, input_config)
         flow.map(self.vectorize)
-        flow.capture()
-
-        input_config = KafkaInputConfig(
-            self.kafka_bootstrap_server,
-            self.kafka_group_id,
-            self.kafka_topic,
-            messages_per_epoch=1
-        )
-
-        def print_output(worker_index, worker_count):
-            def destination_helper(feed):
-                offset = feed[0]
-                data = feed[1]
-                # . . .
-            return destination_helper
-        spawn_cluster(flow, input_config, print_output)
+        flow.output("stdout", StdOutput())
+        run_main(flow)
```

### Comparing `pointstorm-1.1.3/pointstorm.egg-info/PKG-INFO` & `pointstorm-1.1.4/pointstorm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pointstorm
-Version: 1.1.3
+Version: 1.1.4
 Summary: Embedding vectors for data on the move
 Home-page: https://github.com/xsfa/pointstorm
 Author: xsfa
 Author-email: tesfaaog@gmail.com
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `pointstorm-1.1.3/pointstorm.egg-info/SOURCES.txt` & `pointstorm-1.1.4/pointstorm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pointstorm-1.1.3/setup.py` & `pointstorm-1.1.4/setup.py`

 * *Files identical despite different names*

