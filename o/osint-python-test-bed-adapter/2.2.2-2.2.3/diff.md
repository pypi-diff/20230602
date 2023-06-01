# Comparing `tmp/osint-python-test-bed-adapter-2.2.2.tar.gz` & `tmp/osint-python-test-bed-adapter-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osint-python-test-bed-adapter-2.2.2.tar", last modified: Fri Apr  7 15:10:42 2023, max compression
+gzip compressed data, was "osint-python-test-bed-adapter-2.2.3.tar", last modified: Thu Jun  1 22:39:50 2023, max compression
```

## Comparing `osint-python-test-bed-adapter-2.2.2.tar` & `osint-python-test-bed-adapter-2.2.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-07 15:10:42.667866 osint-python-test-bed-adapter-2.2.2/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1064 2022-04-23 22:07:41.000000 osint-python-test-bed-adapter-2.2.2/LICENSE
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1743 2023-04-07 15:10:42.667866 osint-python-test-bed-adapter-2.2.2/PKG-INFO
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1316 2023-04-06 23:36:33.000000 osint-python-test-bed-adapter-2.2.2/README.md
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-07 15:10:42.667866 osint-python-test-bed-adapter-2.2.2/osint_python_test_bed_adapter.egg-info/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1743 2023-04-07 15:10:42.000000 osint-python-test-bed-adapter-2.2.2/osint_python_test_bed_adapter.egg-info/PKG-INFO
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      782 2023-04-07 15:10:42.000000 osint-python-test-bed-adapter-2.2.2/osint_python_test_bed_adapter.egg-info/SOURCES.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        1 2023-04-07 15:10:42.000000 osint-python-test-bed-adapter-2.2.2/osint_python_test_bed_adapter.egg-info/dependency_links.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       39 2023-04-07 15:10:42.000000 osint-python-test-bed-adapter-2.2.2/osint_python_test_bed_adapter.egg-info/requires.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       17 2023-04-07 15:10:42.000000 osint-python-test-bed-adapter-2.2.2/osint_python_test_bed_adapter.egg-info/top_level.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       38 2023-04-07 15:10:42.667866 osint-python-test-bed-adapter-2.2.2/setup.cfg
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      758 2023-04-07 15:09:30.000000 osint-python-test-bed-adapter-2.2.2/setup.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-07 15:10:42.667866 osint-python-test-bed-adapter-2.2.2/test_bed_adapter/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1361 2022-09-07 21:58:21.000000 osint-python-test-bed-adapter-2.2.2/test_bed_adapter/__init__.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-07 15:10:42.667866 osint-python-test-bed-adapter-2.2.2/test_bed_adapter/kafka/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       68 2022-09-07 21:58:21.000000 osint-python-test-bed-adapter-2.2.2/test_bed_adapter/kafka/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1722 2023-04-07 15:09:30.000000 osint-python-test-bed-adapter-2.2.2/test_bed_adapter/kafka/consumer_manager.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1660 2023-03-16 17:49:08.000000 osint-python-test-bed-adapter-2.2.2/test_bed_adapter/kafka/heartbeat_manager.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2897 2023-03-16 17:49:08.000000 osint-python-test-bed-adapter-2.2.2/test_bed_adapter/kafka/log_manager.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2122 2023-04-06 23:32:08.000000 osint-python-test-bed-adapter-2.2.2/test_bed_adapter/kafka/producer_manager.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-07 15:10:42.667866 osint-python-test-bed-adapter-2.2.2/test_bed_adapter/options/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       31 2022-04-23 22:07:41.000000 osint-python-test-bed-adapter-2.2.2/test_bed_adapter/options/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3327 2023-03-16 16:43:04.000000 osint-python-test-bed-adapter-2.2.2/test_bed_adapter/options/test_bed_options.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-07 15:10:42.667866 osint-python-test-bed-adapter-2.2.2/test_bed_adapter/services/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-03-14 11:55:32.000000 osint-python-test-bed-adapter-2.2.2/test_bed_adapter/services/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2065 2023-03-14 12:17:24.000000 osint-python-test-bed-adapter-2.2.2/test_bed_adapter/services/http_server.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-07 15:10:42.667866 osint-python-test-bed-adapter-2.2.2/test_bed_adapter/utils/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       22 2022-09-07 21:58:21.000000 osint-python-test-bed-adapter-2.2.2/test_bed_adapter/utils/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      598 2022-09-07 21:58:21.000000 osint-python-test-bed-adapter-2.2.2/test_bed_adapter/utils/helpers.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1005 2023-03-16 17:51:41.000000 osint-python-test-bed-adapter-2.2.2/test_bed_adapter/utils/key.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-01 22:39:50.616154 osint-python-test-bed-adapter-2.2.3/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1064 2022-04-23 22:07:41.000000 osint-python-test-bed-adapter-2.2.3/LICENSE
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1743 2023-06-01 22:39:50.616154 osint-python-test-bed-adapter-2.2.3/PKG-INFO
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1316 2023-04-06 23:36:33.000000 osint-python-test-bed-adapter-2.2.3/README.md
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-01 22:39:50.616154 osint-python-test-bed-adapter-2.2.3/osint_python_test_bed_adapter.egg-info/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1743 2023-06-01 22:39:50.000000 osint-python-test-bed-adapter-2.2.3/osint_python_test_bed_adapter.egg-info/PKG-INFO
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      782 2023-06-01 22:39:50.000000 osint-python-test-bed-adapter-2.2.3/osint_python_test_bed_adapter.egg-info/SOURCES.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        1 2023-06-01 22:39:50.000000 osint-python-test-bed-adapter-2.2.3/osint_python_test_bed_adapter.egg-info/dependency_links.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       39 2023-06-01 22:39:50.000000 osint-python-test-bed-adapter-2.2.3/osint_python_test_bed_adapter.egg-info/requires.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       17 2023-06-01 22:39:50.000000 osint-python-test-bed-adapter-2.2.3/osint_python_test_bed_adapter.egg-info/top_level.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       38 2023-06-01 22:39:50.616154 osint-python-test-bed-adapter-2.2.3/setup.cfg
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      758 2023-06-01 22:37:37.000000 osint-python-test-bed-adapter-2.2.3/setup.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-01 22:39:50.616154 osint-python-test-bed-adapter-2.2.3/test_bed_adapter/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1361 2022-09-07 21:58:21.000000 osint-python-test-bed-adapter-2.2.3/test_bed_adapter/__init__.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-01 22:39:50.616154 osint-python-test-bed-adapter-2.2.3/test_bed_adapter/kafka/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       68 2022-09-07 21:58:21.000000 osint-python-test-bed-adapter-2.2.3/test_bed_adapter/kafka/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2413 2023-06-01 22:37:01.000000 osint-python-test-bed-adapter-2.2.3/test_bed_adapter/kafka/consumer_manager.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1660 2023-03-16 17:49:08.000000 osint-python-test-bed-adapter-2.2.3/test_bed_adapter/kafka/heartbeat_manager.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2897 2023-03-16 17:49:08.000000 osint-python-test-bed-adapter-2.2.3/test_bed_adapter/kafka/log_manager.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2122 2023-04-06 23:32:08.000000 osint-python-test-bed-adapter-2.2.3/test_bed_adapter/kafka/producer_manager.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-01 22:39:50.616154 osint-python-test-bed-adapter-2.2.3/test_bed_adapter/options/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       31 2022-04-23 22:07:41.000000 osint-python-test-bed-adapter-2.2.3/test_bed_adapter/options/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3486 2023-06-01 22:28:40.000000 osint-python-test-bed-adapter-2.2.3/test_bed_adapter/options/test_bed_options.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-01 22:39:50.616154 osint-python-test-bed-adapter-2.2.3/test_bed_adapter/services/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-03-14 11:55:32.000000 osint-python-test-bed-adapter-2.2.3/test_bed_adapter/services/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2065 2023-03-14 12:17:24.000000 osint-python-test-bed-adapter-2.2.3/test_bed_adapter/services/http_server.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-01 22:39:50.616154 osint-python-test-bed-adapter-2.2.3/test_bed_adapter/utils/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       22 2022-09-07 21:58:21.000000 osint-python-test-bed-adapter-2.2.3/test_bed_adapter/utils/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      598 2022-09-07 21:58:21.000000 osint-python-test-bed-adapter-2.2.3/test_bed_adapter/utils/helpers.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1005 2023-03-16 17:51:41.000000 osint-python-test-bed-adapter-2.2.3/test_bed_adapter/utils/key.py
```

### Comparing `osint-python-test-bed-adapter-2.2.2/LICENSE` & `osint-python-test-bed-adapter-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.2.2/PKG-INFO` & `osint-python-test-bed-adapter-2.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osint-python-test-bed-adapter
-Version: 2.2.2
+Version: 2.2.3
 Summary: Python adapter for Kafka
 Home-page: https://github.com/OSINT-VDU-TNO/python-adapter
 Author: TimovdK
 Author-email: timo_kuil@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `osint-python-test-bed-adapter-2.2.2/README.md` & `osint-python-test-bed-adapter-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.2.2/osint_python_test_bed_adapter.egg-info/PKG-INFO` & `osint-python-test-bed-adapter-2.2.3/osint_python_test_bed_adapter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osint-python-test-bed-adapter
-Version: 2.2.2
+Version: 2.2.3
 Summary: Python adapter for Kafka
 Home-page: https://github.com/OSINT-VDU-TNO/python-adapter
 Author: TimovdK
 Author-email: timo_kuil@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `osint-python-test-bed-adapter-2.2.2/osint_python_test_bed_adapter.egg-info/SOURCES.txt` & `osint-python-test-bed-adapter-2.2.3/osint_python_test_bed_adapter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.2.2/setup.py` & `osint-python-test-bed-adapter-2.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="osint-python-test-bed-adapter",
-    version="2.2.2",
+    version="2.2.3",
     author="TimovdK",
     author_email="timo_kuil@hotmail.com",
     description="Python adapter for Kafka",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/OSINT-VDU-TNO/python-adapter",
     include_package_data=True,
```

### Comparing `osint-python-test-bed-adapter-2.2.2/test_bed_adapter/__init__.py` & `osint-python-test-bed-adapter-2.2.3/test_bed_adapter/__init__.py`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.2.2/test_bed_adapter/kafka/consumer_manager.py` & `osint-python-test-bed-adapter-2.2.3/test_bed_adapter/kafka/consumer_manager.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from confluent_kafka import DeserializingConsumer
+from confluent_kafka import DeserializingConsumer, TopicPartition
 from confluent_kafka.schema_registry import SchemaRegistryClient
 from confluent_kafka.schema_registry.avro import AvroDeserializer
+import time
 
 from ..options.test_bed_options import TestBedOptions
 
 
 class ConsumerManager():
     def __init__(self, options: TestBedOptions, kafka_topic, handle_message, run):
         self.options = options
@@ -20,23 +21,39 @@
 
         consumer_conf = {'bootstrap.servers': self.options.kafka_host,
                          'key.deserializer': self.avro_deserializer,
                          'value.deserializer': self.avro_deserializer,
                          'group.id': self.options.consumer_group,
                          'message.max.bytes': self.options.message_max_bytes,
                          'auto.offset.reset': self.options.offset_type}
-
         self.consumer = DeserializingConsumer(consumer_conf)
-        self.consumer.subscribe([kafka_topic])
+        if self.options.offset_type == 'earliest':
+            self.consumer.assign([TopicPartition(topic=self.kafka_topic, partition=0, offset=0)])
+        else:
+            self.consumer.subscribe([kafka_topic])
 
     def listen(self):
+        _start_time = time.time()
+        _latest_message = None
+
+        # Ignore messages for a period of time
+        while True and self.options.ignore_timeout:
+            msg = self.consumer.poll(1)
+            if msg:
+                _latest_message = msg
+            elapsed_time = time.time() - _start_time
+            if elapsed_time > self.options.ignore_timeout:
+                break
+        if _latest_message and self.options.use_latest:
+            self.handle_message(_latest_message.value(), _latest_message.topic())
+
+        # Continue to listen for messages
         while self.run():
-            # SIGINT can't be handled when polling, limit timeout to 1 second.
-            msg = self.consumer.poll(1.0)
+            msg = self.consumer.poll(1)
             if msg is None:
                 continue
-
             self.handle_message(msg.value(), msg.topic())
+
         self.consumer.close()
 
     def stop(self):
         self.consumer.close()
```

### Comparing `osint-python-test-bed-adapter-2.2.2/test_bed_adapter/kafka/heartbeat_manager.py` & `osint-python-test-bed-adapter-2.2.3/test_bed_adapter/kafka/heartbeat_manager.py`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.2.2/test_bed_adapter/kafka/log_manager.py` & `osint-python-test-bed-adapter-2.2.3/test_bed_adapter/kafka/log_manager.py`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.2.2/test_bed_adapter/kafka/producer_manager.py` & `osint-python-test-bed-adapter-2.2.3/test_bed_adapter/kafka/producer_manager.py`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.2.2/test_bed_adapter/options/test_bed_options.py` & `osint-python-test-bed-adapter-2.2.3/test_bed_adapter/options/test_bed_options.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,15 +46,19 @@
         # self.exclude_internal_topics = False
 
         # Reset the offset messages on start.
         # Not implemented
         # self.reset_offset_on_start = False
 
         # Offset type possibles: earliest, latest, error
-        self.offset_type = "earliest"
+        self.offset_type = "latest"
+        # Ignore messages that for timeout
+        self.ignore_timeout = None
+        # If true, use the send the latest message
+        self.use_latest = False
 
         # How often should the adapter try to reconnect to the kafka server if the first time fails
         # Not implemented
         # self.reconnection_retries = 5
 
         # Interval between two heartbeat messages in secs
         self.heartbeat_interval = 10
```

### Comparing `osint-python-test-bed-adapter-2.2.2/test_bed_adapter/services/http_server.py` & `osint-python-test-bed-adapter-2.2.3/test_bed_adapter/services/http_server.py`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.2.2/test_bed_adapter/utils/helpers.py` & `osint-python-test-bed-adapter-2.2.3/test_bed_adapter/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.2.2/test_bed_adapter/utils/key.py` & `osint-python-test-bed-adapter-2.2.3/test_bed_adapter/utils/key.py`

 * *Files identical despite different names*

