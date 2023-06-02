# Comparing `tmp/cmem_plugin_kafka-1.2.0rc3.tar.gz` & `tmp/cmem_plugin_kafka-1.2.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmem_plugin_kafka-1.2.0rc3.tar", max compression
+gzip compressed data, was "cmem_plugin_kafka-1.2.0rc4.tar", max compression
```

## Comparing `cmem_plugin_kafka-1.2.0rc3.tar` & `cmem_plugin_kafka-1.2.0rc4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11334 2023-05-17 07:44:13.374173 cmem_plugin_kafka-1.2.0rc3/LICENSE
--rw-r--r--   0        0        0     3733 2023-05-17 07:44:13.374173 cmem_plugin_kafka-1.2.0rc3/README-public.md
--rw-r--r--   0        0        0        0 2023-05-17 07:44:13.374173 cmem_plugin_kafka-1.2.0rc3/cmem_plugin_kafka/__init__.py
--rw-r--r--   0        0        0     3836 2023-05-17 07:44:13.374173 cmem_plugin_kafka-1.2.0rc3/cmem_plugin_kafka/constants.py
--rw-r--r--   0        0        0    14685 2023-05-17 07:44:13.374173 cmem_plugin_kafka-1.2.0rc3/cmem_plugin_kafka/kafka_handlers.py
--rw-r--r--   0        0        0    13450 2023-05-17 07:44:13.374173 cmem_plugin_kafka-1.2.0rc3/cmem_plugin_kafka/utils.py
--rw-r--r--   0        0        0        0 2023-05-17 07:44:13.374173 cmem_plugin_kafka-1.2.0rc3/cmem_plugin_kafka/workflow/__init__.py
--rw-r--r--   0        0        0    10768 2023-05-17 07:44:13.374173 cmem_plugin_kafka-1.2.0rc3/cmem_plugin_kafka/workflow/consumer.py
--rw-r--r--   0        0        0     9203 2023-05-17 07:44:13.374173 cmem_plugin_kafka-1.2.0rc3/cmem_plugin_kafka/workflow/producer.py
--rw-r--r--   0        0        0     2268 2023-05-17 07:44:44.446513 cmem_plugin_kafka-1.2.0rc3/pyproject.toml
--rw-r--r--   0        0        0     4918 1970-01-01 00:00:00.000000 cmem_plugin_kafka-1.2.0rc3/PKG-INFO
+-rw-r--r--   0        0        0    11334 2023-06-02 06:59:45.948679 cmem_plugin_kafka-1.2.0rc4/LICENSE
+-rw-r--r--   0        0        0     3733 2023-06-02 06:59:45.948679 cmem_plugin_kafka-1.2.0rc4/README-public.md
+-rw-r--r--   0        0        0        0 2023-06-02 06:59:45.948679 cmem_plugin_kafka-1.2.0rc4/cmem_plugin_kafka/__init__.py
+-rw-r--r--   0        0        0     4432 2023-06-02 06:59:45.948679 cmem_plugin_kafka-1.2.0rc4/cmem_plugin_kafka/constants.py
+-rw-r--r--   0        0        0    14682 2023-06-02 06:59:45.948679 cmem_plugin_kafka-1.2.0rc4/cmem_plugin_kafka/kafka_handlers.py
+-rw-r--r--   0        0        0    11743 2023-06-02 06:59:45.948679 cmem_plugin_kafka-1.2.0rc4/cmem_plugin_kafka/utils.py
+-rw-r--r--   0        0        0        0 2023-06-02 06:59:45.948679 cmem_plugin_kafka-1.2.0rc4/cmem_plugin_kafka/workflow/__init__.py
+-rw-r--r--   0        0        0    11640 2023-06-02 06:59:45.948679 cmem_plugin_kafka-1.2.0rc4/cmem_plugin_kafka/workflow/consumer.py
+-rw-r--r--   0        0        0     9739 2023-06-02 06:59:45.948679 cmem_plugin_kafka-1.2.0rc4/cmem_plugin_kafka/workflow/producer.py
+-rw-r--r--   0        0        0     2268 2023-06-02 07:00:13.677158 cmem_plugin_kafka-1.2.0rc4/pyproject.toml
+-rw-r--r--   0        0        0     4918 1970-01-01 00:00:00.000000 cmem_plugin_kafka-1.2.0rc4/PKG-INFO
```

### Comparing `cmem_plugin_kafka-1.2.0rc3/LICENSE` & `cmem_plugin_kafka-1.2.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `cmem_plugin_kafka-1.2.0rc3/README-public.md` & `cmem_plugin_kafka-1.2.0rc4/README-public.md`

 * *Files identical despite different names*

### Comparing `cmem_plugin_kafka-1.2.0rc3/cmem_plugin_kafka/constants.py` & `cmem_plugin_kafka-1.2.0rc4/cmem_plugin_kafka/constants.py`

 * *Files 18% similar despite different names*

```diff
@@ -79,20 +79,39 @@
 
 COMPRESSION_TYPE_DESCRIPTION = """
 The compression type for all data generated by the producer.
 
 The default is none (i.e. no compression).
 """
 
+MESSAGE_MAX_SIZE_DESCRIPTION = """
+The maximum size of a request message in bytes. This is also effectively a cap on
+the maximum record size.
+
+Note that the server has its own cap on record size which may be different from this.
+"""
+
 LOCAL_CONSUMER_QUEUE_MAX_SIZE_DESCRIPTION = """
 Maximum total message size in kilobytes that the consumer can buffer for
 a specific partition. The consumer will stop fetching from the partition
 if it hits this limit. This helps prevent consumers from running out of memory.
 """
 
+MESSAGE_LIMIT_DESCRIPTION = """
+The maximum number of messages to fetch and process in each run.
+If 0 or less, all messages will be fetched.
+"""
+
+ENABLE_AUTO_COMMIT_DESCRIPTION = """
+Automatically and periodically commit offsets in the background.
+
+Note: setting this to false does not prevent the consumer from fetching
+previously committed start offsets.
+"""
+
 XML_SAMPLE = """
 ```xml
     <?xml version="1.0" encoding="utf-8"?>
     <KafkaMessages>
         <Message>
         <PurchaseOrder OrderDate="1996-04-06">
             <ShipTo country="string">
```

### Comparing `cmem_plugin_kafka-1.2.0rc3/cmem_plugin_kafka/kafka_handlers.py` & `cmem_plugin_kafka-1.2.0rc4/cmem_plugin_kafka/kafka_handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,17 +65,19 @@
         This method splits the input data into individual messages, then sends each
         message as a separate Kafka record.
 
         :param data: The input data to produce messages from.
         :type data: any
         """
         messages = self._split_data(data)
+        count = 0
         for message in messages:
             self._kafka_producer.process(message)
-            if self._kafka_producer.get_success_messages_count() % 10 == 0:
+            count += 1
+            if count % 10 == 0:
                 self._kafka_producer.poll(0)
                 self.update_report()
         self._kafka_producer.flush()
 
     def _split_data(self, data):
         """
         Split the input data into individual messages.
```

### Comparing `cmem_plugin_kafka-1.2.0rc3/cmem_plugin_kafka/utils.py` & `cmem_plugin_kafka-1.2.0rc4/cmem_plugin_kafka/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 """Kafka utils modules"""
-import gzip
 import json
 import re
 from typing import Dict, Any, Iterator, Optional
 from urllib.parse import urlparse
 
-import lz4.frame as lz4frame
-import zstandard
 from cmem.cmempy.config import get_cmem_base_uri
 from cmem.cmempy.workspace.projects.resources.resource import get_resource_response
 from cmem.cmempy.workspace.search import list_items
 from cmem.cmempy.workspace.tasks import get_task
 from cmem_plugin_base.dataintegration.context import (
     ExecutionContext,
     ExecutionReport,
@@ -22,15 +19,14 @@
 from cmem_plugin_base.dataintegration.utils import (
     setup_cmempy_user_access,
     split_task_id,
 )
 from confluent_kafka import Producer, Consumer, KafkaException, KafkaError
 from confluent_kafka.admin import AdminClient, TopicMetadata, ClusterMetadata
 from defusedxml import ElementTree
-from snappy import snappy
 
 from cmem_plugin_kafka.constants import KAFKA_TIMEOUT
 
 
 # pylint: disable-msg=too-few-public-methods
 class KafkaMessage:
     """
@@ -62,53 +58,32 @@
         self._producer = Producer(config)
         self._topic = topic
         self._no_of_success_messages: int = 0
         self.compression_type = config.get("compression.type", 'none')
 
     def process(self, message: KafkaMessage):
         """Produce message to topic."""
-        self._no_of_success_messages += 1
+        # self._no_of_success_messages += 1
         headers = message.headers if message.headers else {}
-        if self.compression_type != 'none' :
-            headers['compression.type'] = self.compression_type
         self._producer.produce(
             self._topic,
-            value=self.compress(message.value),
+            value=message.value.encode('utf-8'),
             key=message.key,
-            headers=headers
+            headers=headers,
+            on_delivery=self.on_delivery
         )
 
-    def compress(self, value: str):
+    def on_delivery(self, err, msg):
         """
-        Compresses the given value based on the configured compression type.
-
-        Args:
-            value (bytes): The value to compress.
-
-        Returns:
-            bytes: The compressed value.
-
-        Raises:
-            ValueError: If an unsupported compression type is provided.
+        Callback method executed after a message is delivered to the Kafka broker.
         """
-        _ = value.encode('utf-8')
-        if self.compression_type == 'none':
-            return _
-        if self.compression_type == 'gzip':
-            return gzip.compress(_)
-        if self.compression_type == 'snappy':
-            return snappy.compress(_)
-        if self.compression_type == 'zstd':
-            compressor = zstandard.ZstdCompressor(level=3)
-            compressed_data = compressor.compress(_)
-            return compressed_data
-        if self.compression_type == 'lz4':
-            compressed_data = lz4frame.compress(_)
-            return compressed_data
-        raise ValueError(f'Unsupported compression type: {self.compression_type}')
+        _ = msg
+        if err:
+            raise KafkaException(err)
+        self._no_of_success_messages += 1
 
     def poll(self, timeout):
         """Polls the producer for events and calls the corresponding callbacks"""
         self._producer.poll(timeout)
 
     def flush(self, timeout=KAFKA_TIMEOUT):
         """Wait for all messages in the Producer queue to be delivered."""
@@ -133,14 +108,15 @@
         """Create consumer instance"""
         self._consumer = Consumer(config)
         self._context = context
         self._topic = topic
         self._log = log
         self._no_of_success_messages = 0
         self._first_message: Optional[KafkaMessage] = None
+        self.fetch_limit = -1
 
     def get_success_messages_count(self) -> int:
         """Return count of the successful messages"""
         return self._no_of_success_messages
 
     def subscribe(self):
         """Subscribes to a topic to consume messages"""
@@ -169,46 +145,32 @@
                 value=msg.value().decode("utf-8"),
             )
         return self._first_message
 
     def poll(self) -> Iterator[KafkaMessage]:
         """Polls the consumer for events and calls the corresponding callbacks"""
         while True:
+            if 0 <= self.fetch_limit == self._no_of_success_messages:
+                self._log.info("Message fetch fetch_limit reached")
+                break
+
             msg = self._consumer.poll(timeout=KAFKA_TIMEOUT)
             if msg is None:
                 self._log.info("Messages are empty")
                 break
             if msg.error():
                 self._log.error(f"Consumer poll Error:{msg.error()}")
                 raise KafkaException(msg.error())
 
             self._no_of_success_messages += 1
-            headers = dict(msg.headers()) if msg.headers() else {}
-            if headers and 'compression.type' in headers:
-                compression_type = headers['compression.type']
-                if compression_type == b'gzip':
-                    decompressed_message = gzip.decompress(msg.value())
-                elif compression_type == b'snappy':
-                    decompressed_message = snappy.decompress(msg.value())
-                elif compression_type == b'zstd':
-                    decompressor = zstandard.ZstdDecompressor()
-                    decompressed_message = decompressor.decompress(msg.value())
-                elif compression_type == b'lz4':
-                    decompressed_message = lz4frame.decompress(msg.value())
-                else:
-                    raise ValueError(
-                        f'Unsupported compression codec: {compression_type}'
-                    )
-            else:
-                decompressed_message = msg.value()
 
             kafka_message = KafkaMessage(
                 key=msg.key().decode("utf-8") if msg.key() else "",
                 headers=msg.headers(),
-                value=decompressed_message.decode("utf-8"),
+                value=msg.value().decode("utf-8"),
             )
 
             if not self._first_message:
                 self._first_message = kafka_message
             if not self._no_of_success_messages % 10:
                 self._context.report.update(
                     ExecutionReport(
```

### Comparing `cmem_plugin_kafka-1.2.0rc3/cmem_plugin_kafka/workflow/consumer.py` & `cmem_plugin_kafka-1.2.0rc4/cmem_plugin_kafka/workflow/consumer.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from cmem.cmempy.workspace.tasks import get_task
 from cmem_plugin_base.dataintegration.context import ExecutionContext, ExecutionReport
 from cmem_plugin_base.dataintegration.description import PluginParameter, Plugin
 from cmem_plugin_base.dataintegration.entity import Entities
 from cmem_plugin_base.dataintegration.parameter.choice import ChoiceParameterType
 from cmem_plugin_base.dataintegration.plugins import WorkflowPlugin
-from cmem_plugin_base.dataintegration.types import IntParameterType
+from cmem_plugin_base.dataintegration.types import IntParameterType, BoolParameterType
 from cmem_plugin_base.dataintegration.utils import write_to_dataset, \
     setup_cmempy_user_access
 from confluent_kafka import KafkaError
 
 from cmem_plugin_kafka.constants import (
     SECURITY_PROTOCOLS,
     SASL_MECHANISMS,
@@ -19,15 +19,15 @@
     BOOTSTRAP_SERVERS_DESCRIPTION,
     SECURITY_PROTOCOL_DESCRIPTION,
     SASL_ACCOUNT_DESCRIPTION,
     SASL_PASSWORD_DESCRIPTION,
     CLIENT_ID_DESCRIPTION,
     LOCAL_CONSUMER_QUEUE_MAX_SIZE_DESCRIPTION,
     XML_SAMPLE,
-    JSON_SAMPLE,
+    JSON_SAMPLE, MESSAGE_LIMIT_DESCRIPTION, ENABLE_AUTO_COMMIT_DESCRIPTION,
 )
 from cmem_plugin_kafka.utils import (
     KafkaConsumer,
     validate_kafka_config,
     get_kafka_statistics,
     get_default_client_id,
     DatasetParameterType,
@@ -160,14 +160,31 @@
             name="local_consumer_queue_size",
             label="Local Consumer Queue Size",
             advanced=True,
             param_type=IntParameterType(),
             default_value=5000,
             description=LOCAL_CONSUMER_QUEUE_MAX_SIZE_DESCRIPTION,
         ),
+        PluginParameter(
+            name="message_limit",
+            label="Message Limit",
+            advanced=True,
+            param_type=IntParameterType(),
+            default_value=100000,
+            description=MESSAGE_LIMIT_DESCRIPTION,
+        ),
+
+        PluginParameter(
+            name="enable_auto_commit",
+            label="Enable Auto Commit",
+            advanced=True,
+            param_type=BoolParameterType(),
+            default_value=True,
+            description=ENABLE_AUTO_COMMIT_DESCRIPTION,
+        ),
     ],
 )
 class KafkaConsumerPlugin(WorkflowPlugin):
     """Kafka Consumer Plugin"""
 
     # pylint: disable=too-many-instance-attributes
     def __init__(
@@ -179,28 +196,32 @@
         sasl_username: str,
         sasl_password: str,
         kafka_topic: str,
         auto_offset_reset: str,
         group_id: str = "",
         client_id: str = "",
         local_consumer_queue_size: int = 5000,
+        message_limit: int = 100000,
+        enable_auto_commit: bool = True
     ) -> None:
         if not isinstance(bootstrap_servers, str):
             raise ValueError("Specified server id is invalid")
         self.message_dataset = message_dataset
         self.bootstrap_servers = bootstrap_servers
         self.security_protocol = security_protocol
         self.sasl_mechanisms = sasl_mechanisms
         self.sasl_username = sasl_username
         self.sasl_password = sasl_password
         self.kafka_topic = kafka_topic
         self.group_id = group_id
         self.auto_offset_reset = auto_offset_reset
         self.client_id = client_id
         self.local_consumer_queue_size = local_consumer_queue_size
+        self.message_limit = int(message_limit)
+        self.enable_auto_commit = bool(enable_auto_commit)
         self._kafka_stats: dict = {}
 
     def metrics_callback(self, json: str):
         """sends producer metrics to server"""
         self._kafka_stats = get_kafka_statistics(json_data=json)
         for key, value in self._kafka_stats.items():
             self.log.info(f"kafka-stats: {key:10} - {value:10}")
@@ -215,15 +236,15 @@
         """construct and return kafka connection configuration"""
         default_client_id = get_default_client_id(
             project_id=project_id, task_id=task_id
         )
         config = {
             "bootstrap.servers": self.bootstrap_servers,
             "security.protocol": self.security_protocol,
-            "enable.auto.commit": True,
+            "enable.auto.commit": self.enable_auto_commit,
             "auto.offset.reset": self.auto_offset_reset,
             "group.id": self.group_id if self.group_id else default_client_id,
             "client.id": self.client_id if self.client_id else default_client_id,
             "statistics.interval.ms": "1000",
             "queued.max.messages.kbytes": self.local_consumer_queue_size,
             # "stats_cb": self.metrics_callback,
             "error_cb": self.error_callback,
@@ -252,14 +273,15 @@
             config=self.get_config(
                 project_id=context.task.project_id(), task_id=context.task.task_id()
             ),
             topic=self.kafka_topic,
             log=self.log,
             context=context,
         )
+        kafka_consumer.fetch_limit = self.message_limit
         kafka_consumer.subscribe()
         if not self.message_dataset:
             return KafkaEntitiesDataHandler(
                 context=context, plugin_logger=self.log, kafka_consumer=kafka_consumer
             ).consume_messages()
         setup_cmempy_user_access(context=context.user)
         task_meta_data = get_task(
```

### Comparing `cmem_plugin_kafka-1.2.0rc3/cmem_plugin_kafka/workflow/producer.py` & `cmem_plugin_kafka-1.2.0rc4/cmem_plugin_kafka/workflow/producer.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,27 +5,28 @@
     ExecutionContext,
     ExecutionReport,
 )
 from cmem_plugin_base.dataintegration.description import PluginParameter, Plugin
 from cmem_plugin_base.dataintegration.entity import Entities
 from cmem_plugin_base.dataintegration.parameter.choice import ChoiceParameterType
 from cmem_plugin_base.dataintegration.plugins import WorkflowPlugin
+from cmem_plugin_base.dataintegration.types import IntParameterType
 from confluent_kafka import KafkaError
 
 from cmem_plugin_kafka.constants import (
     SECURITY_PROTOCOLS,
     SASL_MECHANISMS,
     BOOTSTRAP_SERVERS_DESCRIPTION,
     SECURITY_PROTOCOL_DESCRIPTION,
     SASL_ACCOUNT_DESCRIPTION,
     SASL_PASSWORD_DESCRIPTION,
     CLIENT_ID_DESCRIPTION,
     XML_SAMPLE,
     JSON_SAMPLE, COMPRESSION_TYPES, COMPRESSION_TYPE_DESCRIPTION,
-)
+    MESSAGE_MAX_SIZE_DESCRIPTION, )
 from cmem_plugin_kafka.kafka_handlers import (
     KafkaJSONDataHandler,
     KafkaXMLDataHandler,
     KafkaEntitiesDataHandler,
     KafkaDataHandler,
 )
 from cmem_plugin_kafka.utils import (
@@ -128,14 +129,22 @@
             name="client_id",
             label="Client Id",
             advanced=True,
             default_value="",
             description=CLIENT_ID_DESCRIPTION,
         ),
         PluginParameter(
+            name="message_max_bytes",
+            label="Maximum Message Size",
+            advanced=True,
+            param_type=IntParameterType(),
+            default_value="1048576",
+            description=MESSAGE_MAX_SIZE_DESCRIPTION,
+        ),
+        PluginParameter(
             name="compression_type",
             label="Compression Type",
             advanced=True,
             param_type=ChoiceParameterType(COMPRESSION_TYPES),
             default_value="none",
             description=COMPRESSION_TYPE_DESCRIPTION,
         ),
@@ -151,26 +160,28 @@
         bootstrap_servers: str,
         security_protocol: str,
         sasl_mechanisms: str,
         sasl_username: str,
         sasl_password: str,
         kafka_topic: str,
         client_id: str = "",
+        message_max_bytes: str = "1048576",
         compression_type: str = "none"
     ) -> None:
         if not isinstance(bootstrap_servers, str):
             raise ValueError("Specified server id is invalid")
         self.message_dataset = message_dataset
         self.bootstrap_servers = bootstrap_servers
         self.security_protocol = security_protocol
         self.sasl_mechanisms = sasl_mechanisms
         self.sasl_username = sasl_username
         self.sasl_password = sasl_password
         self.kafka_topic = kafka_topic
         self.client_id = client_id
+        self.message_max_bytes = message_max_bytes
         self.compression_type = compression_type
         self._kafka_stats: dict = {}
 
     def metrics_callback(self, json: str):
         """sends producer metrics to server"""
         self._kafka_stats = get_kafka_statistics(json_data=json)
         for key, value in self._kafka_stats.items():
@@ -187,14 +198,15 @@
         config = {
             "bootstrap.servers": self.bootstrap_servers,
             "security.protocol": self.security_protocol,
             "client.id": self.client_id
             if self.client_id
             else get_default_client_id(project_id=project_id, task_id=task_id),
             "statistics.interval.ms": "1000",
+            "message.max.bytes": int(self.message_max_bytes),
             "compression.type": self.compression_type,
             "stats_cb": self.metrics_callback,
             "error_cb": self.error_callback,
         }
         if self.security_protocol.startswith("SASL"):
             config.update(
                 {
```

### Comparing `cmem_plugin_kafka-1.2.0rc3/pyproject.toml` & `cmem_plugin_kafka-1.2.0rc4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmem-plugin-kafka"
-version = "1.2.0rc3"
+version = "1.2.0rc4"
 license = "Apache-2.0"
 description = "Send and receive messages from Apache Kafka."
 authors = ["eccenca GmbH <cmempy-developer@eccenca.com>"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Plugins",
     "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `cmem_plugin_kafka-1.2.0rc3/PKG-INFO` & `cmem_plugin_kafka-1.2.0rc4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmem-plugin-kafka
-Version: 1.2.0rc3
+Version: 1.2.0rc4
 Summary: Send and receive messages from Apache Kafka.
 Home-page: https://github.com/eccenca/cmem-plugin-kafka
 License: Apache-2.0
 Keywords: eccenca Corporate Memory,plugin,kafka,kafka-producer,kafka-consumer
 Author: eccenca GmbH
 Author-email: cmempy-developer@eccenca.com
 Requires-Python: >=3.9,<4.0
```
