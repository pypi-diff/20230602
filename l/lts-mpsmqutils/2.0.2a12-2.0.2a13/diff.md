# Comparing `tmp/lts-mpsmqutils-2.0.2a12.tar.gz` & `tmp/lts-mpsmqutils-2.0.2a13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lts-mpsmqutils-2.0.2a12.tar", last modified: Sat May 20 01:40:17 2023, max compression
+gzip compressed data, was "dist/lts-mpsmqutils-2.0.2a13.tar", last modified: Fri Jun  2 16:46:06 2023, max compression
```

## Comparing `lts-mpsmqutils-2.0.2a12.tar` & `lts-mpsmqutils-2.0.2a13.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 appuser   (1000) appuser   (1000)        0 2023-05-20 01:40:17.185020 lts-mpsmqutils-2.0.2a12/
--rw-r--r--   0 appuser   (1000) appuser   (1000)     5501 2023-05-20 01:40:17.182383 lts-mpsmqutils-2.0.2a12/PKG-INFO
--rw-r--r--   0 appuser   (1000) appuser   (1000)     5103 2022-04-07 20:19:50.000000 lts-mpsmqutils-2.0.2a12/README.md
-drwxr-xr-x   0 appuser   (1000) appuser   (1000)        0 2023-05-20 01:40:17.098631 lts-mpsmqutils-2.0.2a12/lts_mpsmqutils.egg-info/
--rw-r--r--   0 appuser   (1000) appuser   (1000)     5501 2023-05-20 01:40:16.000000 lts-mpsmqutils-2.0.2a12/lts_mpsmqutils.egg-info/PKG-INFO
--rw-r--r--   0 appuser   (1000) appuser   (1000)      343 2023-05-20 01:40:16.000000 lts-mpsmqutils-2.0.2a12/lts_mpsmqutils.egg-info/SOURCES.txt
--rw-r--r--   0 appuser   (1000) appuser   (1000)        1 2023-05-20 01:40:16.000000 lts-mpsmqutils-2.0.2a12/lts_mpsmqutils.egg-info/dependency_links.txt
--rw-r--r--   0 appuser   (1000) appuser   (1000)       62 2023-05-20 01:40:16.000000 lts-mpsmqutils-2.0.2a12/lts_mpsmqutils.egg-info/requires.txt
--rw-r--r--   0 appuser   (1000) appuser   (1000)       11 2023-05-20 01:40:16.000000 lts-mpsmqutils-2.0.2a12/lts_mpsmqutils.egg-info/top_level.txt
-drwxr-xr-x   0 appuser   (1000) appuser   (1000)        0 2023-05-20 01:40:17.139251 lts-mpsmqutils-2.0.2a12/mpsmqutils/
--rw-r--r--   0 appuser   (1000) appuser   (1000)        0 2022-04-07 20:19:50.000000 lts-mpsmqutils-2.0.2a12/mpsmqutils/__init__.py
--rw-r--r--   0 appuser   (1000) appuser   (1000)    29537 2023-05-20 01:23:03.000000 lts-mpsmqutils-2.0.2a12/mpsmqutils/messagehandler.py
--rw-r--r--   0 appuser   (1000) appuser   (1000)     7247 2023-05-12 14:23:30.000000 lts-mpsmqutils-2.0.2a12/mpsmqutils/mqutils.py
-drwxr-xr-x   0 appuser   (1000) appuser   (1000)        0 2023-05-20 01:40:17.177213 lts-mpsmqutils-2.0.2a12/mpsmqutils/tests/
--rw-r--r--   0 appuser   (1000) appuser   (1000)        0 2022-04-07 20:19:50.000000 lts-mpsmqutils-2.0.2a12/mpsmqutils/tests/__init__.py
--rw-r--r--   0 appuser   (1000) appuser   (1000)     4783 2022-04-07 20:19:50.000000 lts-mpsmqutils-2.0.2a12/mpsmqutils/tests/test_mqutils.py
--rw-r--r--   0 appuser   (1000) appuser   (1000)       38 2023-05-20 01:40:17.186135 lts-mpsmqutils-2.0.2a12/setup.cfg
--rw-r--r--   0 appuser   (1000) appuser   (1000)      899 2023-05-20 01:23:05.000000 lts-mpsmqutils-2.0.2a12/setup.py
+drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-02 16:46:06.780110 lts-mpsmqutils-2.0.2a13/
+-rw-r--r--   0 dougsimon   (502) staff       (20)     6652 2023-06-02 16:46:06.779665 lts-mpsmqutils-2.0.2a13/PKG-INFO
+-rw-r--r--   0 dougsimon   (502) staff       (20)     5103 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a13/README.md
+drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-02 16:46:06.776831 lts-mpsmqutils-2.0.2a13/lts_mpsmqutils.egg-info/
+-rw-r--r--   0 dougsimon   (502) staff       (20)     6652 2023-06-02 16:46:06.000000 lts-mpsmqutils-2.0.2a13/lts_mpsmqutils.egg-info/PKG-INFO
+-rw-r--r--   0 dougsimon   (502) staff       (20)      343 2023-06-02 16:46:06.000000 lts-mpsmqutils-2.0.2a13/lts_mpsmqutils.egg-info/SOURCES.txt
+-rw-r--r--   0 dougsimon   (502) staff       (20)        1 2023-06-02 16:46:06.000000 lts-mpsmqutils-2.0.2a13/lts_mpsmqutils.egg-info/dependency_links.txt
+-rw-r--r--   0 dougsimon   (502) staff       (20)       62 2023-06-02 16:46:06.000000 lts-mpsmqutils-2.0.2a13/lts_mpsmqutils.egg-info/requires.txt
+-rw-r--r--   0 dougsimon   (502) staff       (20)       11 2023-06-02 16:46:06.000000 lts-mpsmqutils-2.0.2a13/lts_mpsmqutils.egg-info/top_level.txt
+drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-02 16:46:06.778009 lts-mpsmqutils-2.0.2a13/mpsmqutils/
+-rw-r--r--   0 dougsimon   (502) staff       (20)        0 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a13/mpsmqutils/__init__.py
+-rw-r--r--   0 dougsimon   (502) staff       (20)    27140 2023-06-02 15:32:14.000000 lts-mpsmqutils-2.0.2a13/mpsmqutils/messagehandler.py
+-rw-r--r--   0 dougsimon   (502) staff       (20)     7160 2023-06-02 15:06:59.000000 lts-mpsmqutils-2.0.2a13/mpsmqutils/mqutils.py
+drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-02 16:46:06.779060 lts-mpsmqutils-2.0.2a13/mpsmqutils/tests/
+-rw-r--r--   0 dougsimon   (502) staff       (20)        0 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a13/mpsmqutils/tests/__init__.py
+-rw-r--r--   0 dougsimon   (502) staff       (20)     4783 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a13/mpsmqutils/tests/test_mqutils.py
+-rw-r--r--   0 dougsimon   (502) staff       (20)       38 2023-06-02 16:46:06.780264 lts-mpsmqutils-2.0.2a13/setup.cfg
+-rw-r--r--   0 dougsimon   (502) staff       (20)      899 2023-06-02 16:46:00.000000 lts-mpsmqutils-2.0.2a13/setup.py
```

### Comparing `lts-mpsmqutils-2.0.2a12/PKG-INFO` & `lts-mpsmqutils-2.0.2a13/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: lts-mpsmqutils
-Version: 2.0.2a12
-Summary: A set of utilities for communicating with a message queue
-Home-page: https://github.huit.harvard.edu/LTS/mps-mqutils
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 # mps-mqutils
 
 ## Introduction
 A set of utilities for Media Preservation Services that provides standard methods to communicate with the message queue.
 
 ## Prerequisites
 Read the README in the worker prototype project [mps-worker-prototype](https://github.huit.harvard.edu/LTS/mps-worker-prototype/blob/main/README.md) for information on how to build and integrate a worker microservice. Read the [WORKER PROGRAMMING](https://github.huit.harvard.edu/LTS/mps-worker-prototype/blob/main/README.md#worker-programming) section for the standard worker API request and responses that are required.
@@ -143,8 +132,8 @@
 ## More information
 Read the documenation for more information on building and publishing the distribution.
 
 * [Generating distribution archives](https://packaging.python.org/tutorials/packaging-projects/#generating-distribution-archives)
 
 * [Uploading the distribution archives](https://packaging.python.org/tutorials/packaging-projects/#uploading-the-distribution-archives)
 
-* https://tom-christie.github.io/articles/pypi/
+* https://tom-christie.github.io/articles/pypi/
```

### Comparing `lts-mpsmqutils-2.0.2a12/mpsmqutils/messagehandler.py` & `lts-mpsmqutils-2.0.2a13/mpsmqutils/messagehandler.py`

 * *Files 6% similar despite different names*

```diff
@@ -107,18 +107,18 @@
       Call worker API internally to perform the task
       This API call is calling the worker task in the same container and must use the internal container port
     """
     try:
 
         if not worker_url:
             error_msg = 'Missing configuration WORKER_API_URL'
-            print(error_msg)
+            print(error_msg, flush=True)
             raise Exception(error_msg)
         url = worker_url + '/' + worker_url_endpoint
-        print('mqlistener call_worker_api url {}'.format(url))
+        print('mqlistener call_worker_api url {}'.format(url), flush=True)
         json_params = { 'task_name': task_name }
         if add_params:
             json_params = {**json_params, **add_params}
         if job_ticket_id:
             json_params['job_ticket_id'] = job_ticket_id
         if parent_job_ticket_id:
             json_params['parent_job_ticket_id'] = parent_job_ticket_id
@@ -130,30 +130,30 @@
         print(response)
     except Exception as e:
         print(e)
         if job_ticket_id:
             job_tracker.append_error(job_ticket_id, 'mqlistener call_worker_api API call failed', traceback.format_exc(), True)
         raise Exception(e)
 
-    print(f'mqlistener call_worker_api COMPLETE{job_ticket_id_str}{parent_job_ticket_id_str} task_name {task_name} response.json() {response.json()}')
+    print(f'mqlistener call_worker_api COMPLETE{job_ticket_id_str}{parent_job_ticket_id_str} task_name {task_name} response.json() {response.json()}', flush=True)
 
     response_json = response.json()
     print(response_json)
 
     success = False if not response_json.get('success') else True
     print("success:")
     print(success)
     result['success'] = success
     result['error'] = response_json.get('error', None)
     result['message'] = response_json.get('message', None)
 
     return result
 
 def call_generic_worker_api(message_data, worker_endpoint):
-    print("************************ MQUTILS MQLISTENER - CALL GENERIC WORKER API *******************************")
+    print("************************ MQUTILS MQLISTENER - CALL GENERIC WORKER API *******************************", flush=True)
     '''Call the worker API and process the response in a standard format'''
 
     result = {
       'success': False,
       'error': None,
       'message': None,
       'next_queue': None
@@ -163,33 +163,33 @@
     """
       Call worker API internally to perform the task
       This API call is calling the worker task in the same container and must use the internal container port
     """
     try:
         if not worker_url:
             error_msg = 'Missing configuration WORKER_API_URL'
-            print(error_msg)
+            print(error_msg, flush=True)
             raise Exception(error_msg)
         url = worker_url
-        print('mqlistener call_generic_worker_api url {}'.format(url))
+        print('mqlistener call_generic_worker_api url {}'.format(url), flush=True)
         # The worker uses a self-signed certificate and it does not need to be verified since the listener makes a request to the worker inside the same container internally
         response = http_client.post(url, json = message_data, verify=False)
         response.raise_for_status()
-        print('response.raise_for_status')
-        print(response)
+        print('response.raise_for_status', flush=True)
+        print(response, flush=True)
     except Exception as e:
         print(e)
         raise Exception(e)
 
     response_json = response.json()
-    print(response_json)
+    print(response_json, flush=True)
 
     success = False if not response_json.get('success') else True
-    print("success:")
-    print(success)
+    print("success:", flush=True)
+    print(success, flush=True)
     result['success'] = success
     result['error'] = response_json.get('error', None)
     result['message'] = response_json.get('message', None)
     result['next_queue'] = response_json.get('next_queue', None)
 
     return result
 
@@ -234,15 +234,15 @@
         print('job_tracker_doc {}'.format(job_tracker_doc))
         status = job_tracker_doc['job_management']['job_status']
         if status in completed_statuses:
             print(f'Status {status} counts as completed, assuming job is complete')
             #Assume if the tracker is completed or not there, that this job is no longer running
             return
 
-        print(f"Dispatching based on category: {category}")
+        print(f"Dispatching based on category: {category}", flush=True)
         if (category == "ingest"):
             task_success = self.__ingest_message_handler(self.message)
         elif (category == "task_management"):
             task_success = self.__task_management_message_handler(self.message)
         elif (category == "service"):
             task_success = self.__service_message_handler(self.message)
         elif (category == "cache_management"):
@@ -250,15 +250,15 @@
 
         #Sometimes the ack/nack might be sent in the handler
         if (task_success != None):
             if not task_success:
                 # TODO: ack is sent automatically after task completes
                 # TODO: unsure how nack works in the case of celery
                 job_tracker.set_job_status('failed', job_ticket_id, "failed")
-                logger.warning('Task unsuccessful')
+                print('Task unsuccessful')
                 # self.conn.nack(message_id, self._sub_id)
 
         #TODO- Handle
         print('processed message for job id {}'.format(job_ticket_id))
 
     def __ingest_message_handler(self, message_data):
         print("************************ MQUTILS MQLISTENER - INGEST_MESSAGE_HANDLER *******************************")
@@ -360,15 +360,15 @@
                 try:
                     print('******** UPDATE TRACKER FILE ********')
                     updated_tracker_doc = job_tracker.replace_tracker_doc(tracker_doc)
                     print('updated_tracker_doc {}'.format(updated_tracker_doc))
                 except Exception as e:
                     #TODO what to do here - what does this mean if the tracker retrieval fails?
                     print("TRACKER RETRIEVAL FAILED")
-                    print(e)
+                    print(e, flush=True)
                     raise e
                 celeryapp.execute.send_task("tasks.tasks.do_task", args=[nextmessage], kwargs={}, queue=queue)
         print('task_success')
         print(task_success)
         return task_success
 
     def __task_management_message_handler(self, message_data):
@@ -449,15 +449,15 @@
     def __cache_management_message_handler(self, message_data, message_id):
         print('cache management message')
         try:
             worker_response = call_worker_api('update_cache')
         except Exception as e:
             import traceback;
             print('Failure in cache management handler')
-            print(traceback.format_exc())
+            print(traceback.format_exc(), flush=True)
             # print('Nack message_id {}'.format(message_id))
             # self.conn.nack(message_id, self._sub_id)
             # TODO: HOW DO WE NACK IN CELERY?
             return False
         return True
 
 # Generalized listener based on MQListener for use with components that do not use jobtracker
@@ -472,17 +472,16 @@
         task_success = False
 
         task_success = self.__generic_message_handler(self.message, self.worker_endpoint)
 
         # #Sometimes the ack/nack might be sent in the handler
         if (task_success != None):
             if not task_success:
-                logger.warning('Task unsuccessful')
+                print('Task unsuccessful')
                 # TODO: HOW TO NACK A TASK?
-        # print('processed message message_id {}'.format(message_id))
 
     def __generic_message_handler(self, message_data, worker_endpoint):
         print("************************ MQUTILS MQLISTENER - GENERIC_MESSAGE_HANDLER *******************************")
         task_success = False
 
         # Call task
         try:
@@ -522,15 +521,15 @@
 #         print("Handling message from notification queue")
 #         message = json.loads(frame.body)
 
 #         if not 'to' in message:
 #             message['to'] = [NOTIFY_DEFAULT_EMAIL]
 
 #         if message['method'] == "email":
-#             print("Method is email")
+#             print("Method is email", flush=True)
 #             if isinstance(message['to'], str):
 #                 message['to'] = recipient_separators.split(message['to'])
 #             msg = dedent(f"""\
 #             From: {message['from']}
 #             Subject: {message['subject']}
 
 #             """) + message["message"]
@@ -543,15 +542,15 @@
 #                         to_addrs=message['to'],
 #                         msg = msg
 #                     )
 #                 except Exception as e:
 #                     print(f"Sendmail failed with exception {e}")
 #                     import traceback
 #                     print(traceback.format_exc())
-#                 print(f"Result of sendmail: {result}")
+#                 print(f"Result of sendmail: {result}", flush=True)
 #         else:
 #             raise RuntimeError('Unknown method for notification')
 
 
 #     def handle_dlq(self, frame):
 #         print('Handling DLQ notification')
 #         message = json.loads(frame.body)
@@ -576,15 +575,15 @@
 #                     msg = msg
 #                 )
 #             except Exception as e:
 #                 print(f"Sendmail failed with exception {e}")
 #                 import traceback
 #                 print(traceback.format_exc())
 #                 raise(e)
-#             print(f"Result of sendmail: {result}")
+#             print(f"Result of sendmail: {result}", flush=True)
 
 #     def on_message(self, frame):
 #         headers, body = frame.headers, frame.body
 #         message_id = headers.get('message-id')
 #         sub_id = int(headers.get('subscription'))
 #         print(f'handling message {message_id} from sub {sub_id}')
 #         try:
@@ -599,59 +598,7 @@
 #         except Exception as e:
 #             self.conn.nack(message_id, sub_id)
 #             raise(e)
 #         self.conn.ack(message_id, sub_id)
 
 #     def on_error(self, frame):
 #         print('received an error "%s"' % frame.body)
-
-
-# def initialize_mqlistener():
-#     if _failback_host and _failback_port:
-#         print('failback host and port in use')
-#         conn = stomp.Connection([(_host, _port),(_failback_host, _failback_port)], heartbeats=(40000, 40000), keepalive=True)
-#     else:
-#         print('failback host and port not in use')
-#         conn = stomp.Connection([(_host, _port)], heartbeats=(40000, 40000), keepalive=True)
-#     conn.set_listener('', MqListener(conn))
-#     connect_and_subscribe(conn)
-#     # http_clients://github.com/jasonrbriggs/stomp.py/issues/206
-#     while True:
-#         time.sleep(2)
-#         if not conn.is_connected():
-#             print('Disconnected in loop, reconnecting')
-#             connect_and_subscribe(conn)
-
-# def initialize_generic_listener(worker_endpoint='do_task'):
-#     if _failback_host and _failback_port:
-#         print('failback host and port in use')
-#         conn = stomp.Connection([(_host, _port),(_failback_host, _failback_port)], heartbeats=(40000, 40000), keepalive=True)
-#     else:
-#         print('failback host and port not in use')
-#         conn = stomp.Connection([(_host, _port)], heartbeats=(40000, 40000), keepalive=True)
-#     conn.set_listener('', GenericListener(conn, worker_endpoint))
-#     conn_list.append(conn)
-#     connect_and_subscribe(conn)
-#     # http_clients://github.com/jasonrbriggs/stomp.py/issues/206
-#     while True:
-#         time.sleep(2)
-#         if not conn.is_connected():
-#             print('Disconnected in loop, reconnecting')
-#             connect_and_subscribe(conn)
-
-# def initialize_notify_listener():
-#     if _failback_host and _failback_port:
-#         print('failback host and port in use')
-#         conn = stomp.Connection([(_host, _port),(_failback_host, _failback_port)], heartbeats=(40000, 40000), keepalive=True)
-#     else:
-#         print('failback host and port not in use')
-#         conn = stomp.Connection([(_host, _port)], heartbeats=(40000, 40000), keepalive=True)
-#     conn.set_listener('', NotificationListener(conn))
-#     connect_and_subscribe(conn, NOTIFY_QUEUE, sub_id=NOTIFY_SUB)
-#     connect_and_subscribe(conn, DLQ_QUEUE, sub_id=DLQ_SUB)
-#     # http_clients://github.com/jasonrbriggs/stomp.py/issues/206
-#     while True:
-#         time.sleep(2)
-#         if not conn.is_connected():
-#             print('Disconnected in loop, reconnecting')
-#             connect_and_subscribe(conn, NOTIFY_QUEUE, sub_id=NOTIFY_SUB)
-#             connect_and_subscribe(conn, DLQ_QUEUE, sub_id=DLQ_SUB)
```

### Comparing `lts-mpsmqutils-2.0.2a12/mpsmqutils/mqutils.py` & `lts-mpsmqutils-2.0.2a13/mpsmqutils/mqutils.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,144 +24,145 @@
 _hosts = [(_host, _port,)]
 
 if _failback_host and _failback_port:
     _hosts.append((_failback_host, _failback_port,))
 
 _max_reconnects = 1000
 
+# TODO: Research how to setup logging in the module the logs were not writing to the worker output
 # Logging
-import logging
-logging.basicConfig(level=os.environ.get('APP_LOG_LEVEL', 'INFO'))
-logger = logging.getLogger(__name__)
+#import logging
+#logging.basicConfig(level=os.environ.get('APP_LOG_LEVEL', 'INFO'))
+#logger = logging.getLogger(__name__)
 
 def create_initial_queue_message(job_ticket_id, parent_job_ticket_id = None):
     '''Creates a queue json message to be picked up by the worker'''
-    logger.debug("************************ MQUTILS - CREATE_INITIAL_QUEUE_MESSAGE *******************************")
+    print("************************ MQUTILS - CREATE_INITIAL_QUEUE_MESSAGE *******************************")
     try:
         message = __create_ingest_message(job_ticket_id, 0, "success", parent_job_ticket_id)
-        logger.debug("MESSAGE TO QUEUE create_initial_queue_message")
-        logger.debug(message)
+        print("MESSAGE TO QUEUE create_initial_queue_message")
+        print(message)
     except Exception as e:
-        logger.error(e)
+        print(e)
         raise(e)
     return message
 
 def create_next_queue_message(ticket_id, parent_job_ticket_id = None):
     '''Creates a message for the next task in the job'''
-    logger.debug("************************ MQUTILS - CREATE_NEXT_QUEUE_MESSAGE *******************************")
+    print("************************ MQUTILS - CREATE_NEXT_QUEUE_MESSAGE *******************************")
     message = None
     try:
         message = __create_ingest_message(ticket_id, 1, "success", parent_job_ticket_id)
-        logger.debug("MESSAGE TO QUEUE create_next_queue_message")
-        logger.debug(message)
+        print("MESSAGE TO QUEUE create_next_queue_message")
+        print(message)
     except Exception as e:
-        logger.error(e)
+        print(e)
         raise(e)
     return message
 
 def create_requeue_message(ticket_id, parent_job_ticket_id = None):
     '''Creates a queue json message for the current task to be requeued'''
-    logger.debug("************************ MQUTILS - CREATE_REQUEUE_MESSAGE *******************************")
+    print("************************ MQUTILS - CREATE_REQUEUE_MESSAGE *******************************")
     try:
         jt = get_jt()
         job_tracker_file = jt.get_tracker_document(ticket_id)
         job_management = job_tracker_file.get("job_management")
         if (job_management is None):
             raise Exception ('Tracker File is malformed, missing job_management')
         prev_step_status = job_management["previous_step_status"]
         message = __create_ingest_message(ticket_id, 0, prev_step_status, parent_job_ticket_id)
-        logger.debug("MESSAGE TO QUEUE create_requeue_message")
-        logger.debug(message)
+        print("MESSAGE TO QUEUE create_requeue_message")
+        print(message)
     except Exception as e:
-        logger.error(e)
+        print(e)
         raise(e)
     return message
 
 def create_revert_message(ticket_id, parent_job_ticket_id = None):
-    logger.debug("************************ MQUTILS - CREATE_REVERT_MESSAGE *******************************")
+    print("************************ MQUTILS - CREATE_REVERT_MESSAGE *******************************")
     '''Creates a queue json message to revert the previous task
          Returns None if there is no previous message'''
     message = None
     try:
         message = __create_ingest_message(ticket_id, -1, "failed", parent_job_ticket_id)
-        logger.debug("MESSAGE TO QUEUE create_revert_message")
-        logger.debug(message)
+        print("MESSAGE TO QUEUE create_revert_message")
+        print(message)
     except Exception as e:
-        logger.error(e)
+        print(e)
         raise(e)
     return message
 
 def create_task_manager_queue_message(job_ticket_id, parent_job_ticket_id = None):
-    logger.debug("************************ MQUTILS - CREATE_TASK_MANANGER_QUEUE_MESSAGE *******************************")
+    print("************************ MQUTILS - CREATE_TASK_MANANGER_QUEUE_MESSAGE *******************************")
     json_message = {
         "job_ticket_id": job_ticket_id,
         "task_name": "task_manager_worker_inprocess",
         "previous_step_status" : "success",
         "category": "task_management"
     }
     if parent_job_ticket_id:
         json_message["parent_job_ticket_id"] = parent_job_ticket_id
     message = json.dumps(json_message)
-    logger.debug(message)
+    print(message)
     return message
 
 NOTIFY_QUEUE = os.getenv('MQ_NOTIFY_QUEUE', '/queue/iiif_notify')
 def create_notification(sender, recipients, subject, message, method="email", **opts):
-    logger.debug("************************ MQUTILS - CREATE_NOTIFICATION *******************************")
+    print("************************ MQUTILS - CREATE_NOTIFICATION *******************************")
     jt=get_jt()
     message = json.dumps({
         "from": sender,
         "to": recipients,
         "subject": subject,
         "message": message,
         "options": opts,
         "timestamp": jt.get_timestamp_utc_now(),
         "method": method
     })
-    logger.debug(message)
+    print(message)
 
     with managed_mq_connect() as conn:
         conn.send(NOTIFY_QUEUE, message, headers = {"persistent": "true"})
 
 CACHE_MANAGER_QUEUE = os.getenv('MQ_CACHE_MANAGER_QUEUE', '/queue/mps-asset-db-cache')
 def create_cache_refresh_message(**opts):
-    logger.debug("************************ MQUTILS - CREATE_CACHE_REFRESH_MESSAGE *******************************")
+    print("************************ MQUTILS - CREATE_CACHE_REFRESH_MESSAGE *******************************")
     jt = get_jt()
     message = json.dumps({
         "category": "cache_management",
         "timestamp": jt.get_timestamp_utc_now(),
         "options": opts
     })
-    logger.debug(message)
+    print(message)
     with managed_mq_connect() as conn:
         conn.send(CACHE_MANAGER_QUEUE, message, headers = {"persistent": "true"})
 
 def create_multi_asset_ingest_queue_message(job_ticket_id):
-    logger.debug("************************ MQUTILS - CREATE_MULTI_ASSET_INGEST_QUEUE_MESSAGE *******************************")
+    print("************************ MQUTILS - CREATE_MULTI_ASSET_INGEST_QUEUE_MESSAGE *******************************")
     json_message = {
         "job_ticket_id": job_ticket_id,
         "task_name": "multi_asset_ingest",
         "previous_step_status" : "success",
         "category": "task_management"
     }
-    logger.debug(json_message)
+    print(json_message)
     message = json.dumps(json_message)
     return message
 
 def __create_ingest_message(ticket_id, step_number_increment, prev_step_status, parent_job_ticket_id = None):
-    logger.debug("************************ MQUTILS - CREATE_INGEST_MESSAGE *******************************")
+    print("************************ MQUTILS - CREATE_INGEST_MESSAGE *******************************")
     '''Helper method for the create messages above'''
     jt = get_jt()
     job_tracker_file = jt.get_tracker_document(ticket_id)
 
     timestamp = jt.get_timestamp_utc_now()
 
     job_management = job_tracker_file.get("job_management")
     if (job_management is None):
-        logger.error("Malformed Tracker File")
+        print("Malformed Tracker File")
         raise Exception ('Tracker File is malformed, missing job_management.')
 
     current_step = int(job_management["current_step"])
     step_number = current_step + step_number_increment
     steps_list = job_management["steps"]
     # Get step by looking up the step by step number
     event = jt.filter_element_by_property(steps_list, "step_number", step_number)
@@ -178,10 +179,10 @@
         "current_step": step_number,
         "previous_step_status": prev_step_status,
         "category": "ingest"
     }
     if parent_job_ticket_id:
         msg_json["parent_job_ticket_id"] = parent_job_ticket_id
 
-    logger.debug(msg_json)
+    print(msg_json)
     message = json.dumps(msg_json)
     return message
```

### Comparing `lts-mpsmqutils-2.0.2a12/mpsmqutils/tests/test_mqutils.py` & `lts-mpsmqutils-2.0.2a13/mpsmqutils/tests/test_mqutils.py`

 * *Files identical despite different names*

### Comparing `lts-mpsmqutils-2.0.2a12/setup.py` & `lts-mpsmqutils-2.0.2a13/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lts-mpsmqutils",
-    version="2.0.2a12",
+    version="2.0.2a13",
     description="A set of utilities for communicating with a message queue",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.huit.harvard.edu/LTS/mps-mqutils",
     packages=setuptools.find_packages(),
     install_requires=[
         'lts-mpsjobtracker-mongo',
```

