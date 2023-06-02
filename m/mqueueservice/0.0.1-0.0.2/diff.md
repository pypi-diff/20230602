# Comparing `tmp/mqueueservice-0.0.1.tar.gz` & `tmp/mqueueservice-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mqueueservice-0.0.1.tar", last modified: Thu Jun  1 07:25:12 2023, max compression
+gzip compressed data, was "mqueueservice-0.0.2.tar", last modified: Fri Jun  2 17:14:18 2023, max compression
```

## Comparing `mqueueservice-0.0.1.tar` & `mqueueservice-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 soniyas   (1000) soniyas   (1000)        0 2023-06-01 07:25:12.463970 mqueueservice-0.0.1/
--rw-rw-r--   0 soniyas   (1000) soniyas   (1000)     1776 2023-06-01 07:25:12.463970 mqueueservice-0.0.1/PKG-INFO
--rw-rw-r--   0 soniyas   (1000) soniyas   (1000)      881 2023-05-31 11:53:08.000000 mqueueservice-0.0.1/README.md
-drwxrwxr-x   0 soniyas   (1000) soniyas   (1000)        0 2023-06-01 07:25:12.463970 mqueueservice-0.0.1/mqueueservice.egg-info/
--rw-rw-r--   0 soniyas   (1000) soniyas   (1000)     1776 2023-06-01 07:25:12.000000 mqueueservice-0.0.1/mqueueservice.egg-info/PKG-INFO
--rw-rw-r--   0 soniyas   (1000) soniyas   (1000)      292 2023-06-01 07:25:12.000000 mqueueservice-0.0.1/mqueueservice.egg-info/SOURCES.txt
--rw-rw-r--   0 soniyas   (1000) soniyas   (1000)        1 2023-06-01 07:25:12.000000 mqueueservice-0.0.1/mqueueservice.egg-info/dependency_links.txt
--rw-rw-r--   0 soniyas   (1000) soniyas   (1000)        1 2023-05-31 14:18:30.000000 mqueueservice-0.0.1/mqueueservice.egg-info/not-zip-safe
--rw-rw-r--   0 soniyas   (1000) soniyas   (1000)        9 2023-06-01 07:25:12.000000 mqueueservice-0.0.1/mqueueservice.egg-info/requires.txt
--rw-rw-r--   0 soniyas   (1000) soniyas   (1000)       13 2023-06-01 07:25:12.000000 mqueueservice-0.0.1/mqueueservice.egg-info/top_level.txt
-drwxrwxr-x   0 soniyas   (1000) soniyas   (1000)        0 2023-06-01 07:25:12.463970 mqueueservice-0.0.1/queueService/
--rw-rw-r--   0 soniyas   (1000) soniyas   (1000)      183 2023-05-31 14:10:04.000000 mqueueservice-0.0.1/queueService/__init__.py
--rw-rw-r--   0 soniyas   (1000) soniyas   (1000)     1319 2023-05-31 14:10:31.000000 mqueueservice-0.0.1/queueService/queueService.py
--rw-rw-r--   0 soniyas   (1000) soniyas   (1000)       38 2023-06-01 07:25:12.463970 mqueueservice-0.0.1/setup.cfg
--rw-rw-r--   0 soniyas   (1000) soniyas   (1000)     1026 2023-05-31 14:17:05.000000 mqueueservice-0.0.1/setup.py
+drwxrwxr-x   0 soniyas   (1000) soniyas   (1000)        0 2023-06-02 17:14:18.051989 mqueueservice-0.0.2/
+-rw-rw-r--   0 soniyas   (1000) soniyas   (1000)     1601 2023-06-02 17:14:18.051989 mqueueservice-0.0.2/PKG-INFO
+-rw-rw-r--   0 soniyas   (1000) soniyas   (1000)      770 2023-06-02 13:00:38.000000 mqueueservice-0.0.2/README.md
+drwxrwxr-x   0 soniyas   (1000) soniyas   (1000)        0 2023-06-02 17:14:18.051989 mqueueservice-0.0.2/mqueueservice.egg-info/
+-rw-rw-r--   0 soniyas   (1000) soniyas   (1000)     1601 2023-06-02 17:14:17.000000 mqueueservice-0.0.2/mqueueservice.egg-info/PKG-INFO
+-rw-rw-r--   0 soniyas   (1000) soniyas   (1000)      292 2023-06-02 17:14:17.000000 mqueueservice-0.0.2/mqueueservice.egg-info/SOURCES.txt
+-rw-rw-r--   0 soniyas   (1000) soniyas   (1000)        1 2023-06-02 17:14:17.000000 mqueueservice-0.0.2/mqueueservice.egg-info/dependency_links.txt
+-rw-rw-r--   0 soniyas   (1000) soniyas   (1000)        1 2023-05-31 14:18:30.000000 mqueueservice-0.0.2/mqueueservice.egg-info/not-zip-safe
+-rw-rw-r--   0 soniyas   (1000) soniyas   (1000)        9 2023-06-02 17:14:17.000000 mqueueservice-0.0.2/mqueueservice.egg-info/requires.txt
+-rw-rw-r--   0 soniyas   (1000) soniyas   (1000)       13 2023-06-02 17:14:17.000000 mqueueservice-0.0.2/mqueueservice.egg-info/top_level.txt
+drwxrwxr-x   0 soniyas   (1000) soniyas   (1000)        0 2023-06-02 17:14:18.051989 mqueueservice-0.0.2/queueService/
+-rw-rw-r--   0 soniyas   (1000) soniyas   (1000)      183 2023-06-02 17:13:45.000000 mqueueservice-0.0.2/queueService/__init__.py
+-rw-rw-r--   0 soniyas   (1000) soniyas   (1000)     2281 2023-06-02 12:21:23.000000 mqueueservice-0.0.2/queueService/queueService.py
+-rw-rw-r--   0 soniyas   (1000) soniyas   (1000)       38 2023-06-02 17:14:18.051989 mqueueservice-0.0.2/setup.cfg
+-rw-rw-r--   0 soniyas   (1000) soniyas   (1000)     1026 2023-05-31 14:17:05.000000 mqueueservice-0.0.2/setup.py
```

### Comparing `mqueueservice-0.0.1/PKG-INFO` & `mqueueservice-0.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqueueservice
-Version: 0.0.1
+Version: 0.0.2
 Summary: A free queue service using ActiveMQ
 Home-page: https://github.com/Soniyasharma6868/activeMqServices
 Author: Soniya Sharma
 Author-email: sharmasoniya6868@email.com
 License: MIT
 Project-URL: Source, https://github.com/Soniyasharma6868/activeMqServices
 Description: # activeMqServices
@@ -14,43 +14,35 @@
         ## requirements
         
         For running this, you need to have `python3` installed on your system.
         
         
         ## Installation
         ```
-        Download the tar file from the below link:
-        https://github.com/Soniyasharma6868/queueServicePkg.git
         
-        pip install queue-service-1.0.0.tar.gz
+        pip install mqueueservice==0.0.1
         
         ```
         
         ## Example
         
-        1. Queue Service Configuration
         ```
-        from pyqservice.queue_service import QueueService
+        from queueService.queueService import QueueService
         
-        * Create an instance of the QueueService class
-        service = QueueService(host='localhost', port=61613, username='admin', password='admin', destination='/queue/test')
-        ```
-        
-        2. Connect to ActiveMQ
-        service.connect()
+        #Create an instance of the QueueService class
+        service = QueueService(host='localhost', port=61613, username='your_username', password='your_password', destination='/queue/test')
         
-        3. Send a message
-        service.send_message('Hello, World!')
+        service.connect() #Connect to ActiveMQ
         
-        4. Receive messages
-        service.receive_message()  # This will start listening for incoming messages
+        service.send_message('Hello, World Mr Shrijeet!') # Send a message
         
-        5. Disconnect from ActiveMQ
-        service.disconnect()
+        msg=service.receive_message()  # This will start listening for incoming messages# Receive messages
         
+        service.disconnect() # Disconnect from ActiveMQ
+        ```
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `mqueueservice-0.0.1/README.md` & `mqueueservice-0.0.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -5,35 +5,28 @@
 ## requirements
 
 For running this, you need to have `python3` installed on your system.
 
 
 ## Installation
 ```
-Download the tar file from the below link:
-https://github.com/Soniyasharma6868/queueServicePkg.git
 
-pip install queue-service-1.0.0.tar.gz
+pip install mqueueservice==0.0.1
 
 ```
 
 ## Example
 
-1. Queue Service Configuration
 ```
-from pyqservice.queue_service import QueueService
+from queueService.queueService import QueueService
 
-* Create an instance of the QueueService class
-service = QueueService(host='localhost', port=61613, username='admin', password='admin', destination='/queue/test')
-```
+#Create an instance of the QueueService class
+service = QueueService(host='localhost', port=61613, username='your_username', password='your_password', destination='/queue/test')
 
-2. Connect to ActiveMQ
-service.connect()
+service.connect() #Connect to ActiveMQ
 
-3. Send a message
-service.send_message('Hello, World!')
+service.send_message('Hello, World Mr Shrijeet!') # Send a message
 
-4. Receive messages
-service.receive_message()  # This will start listening for incoming messages
+msg=service.receive_message()  # This will start listening for incoming messages# Receive messages
 
-5. Disconnect from ActiveMQ
-service.disconnect()
+service.disconnect() # Disconnect from ActiveMQ
+```
```

### Comparing `mqueueservice-0.0.1/mqueueservice.egg-info/PKG-INFO` & `mqueueservice-0.0.2/mqueueservice.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqueueservice
-Version: 0.0.1
+Version: 0.0.2
 Summary: A free queue service using ActiveMQ
 Home-page: https://github.com/Soniyasharma6868/activeMqServices
 Author: Soniya Sharma
 Author-email: sharmasoniya6868@email.com
 License: MIT
 Project-URL: Source, https://github.com/Soniyasharma6868/activeMqServices
 Description: # activeMqServices
@@ -14,43 +14,35 @@
         ## requirements
         
         For running this, you need to have `python3` installed on your system.
         
         
         ## Installation
         ```
-        Download the tar file from the below link:
-        https://github.com/Soniyasharma6868/queueServicePkg.git
         
-        pip install queue-service-1.0.0.tar.gz
+        pip install mqueueservice==0.0.1
         
         ```
         
         ## Example
         
-        1. Queue Service Configuration
         ```
-        from pyqservice.queue_service import QueueService
+        from queueService.queueService import QueueService
         
-        * Create an instance of the QueueService class
-        service = QueueService(host='localhost', port=61613, username='admin', password='admin', destination='/queue/test')
-        ```
-        
-        2. Connect to ActiveMQ
-        service.connect()
+        #Create an instance of the QueueService class
+        service = QueueService(host='localhost', port=61613, username='your_username', password='your_password', destination='/queue/test')
         
-        3. Send a message
-        service.send_message('Hello, World!')
+        service.connect() #Connect to ActiveMQ
         
-        4. Receive messages
-        service.receive_message()  # This will start listening for incoming messages
+        service.send_message('Hello, World Mr Shrijeet!') # Send a message
         
-        5. Disconnect from ActiveMQ
-        service.disconnect()
+        msg=service.receive_message()  # This will start listening for incoming messages# Receive messages
         
+        service.disconnect() # Disconnect from ActiveMQ
+        ```
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `mqueueservice-0.0.1/setup.py` & `mqueueservice-0.0.2/setup.py`

 * *Files identical despite different names*

