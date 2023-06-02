# Comparing `tmp/midpoint-cli-0.9.0.tar.gz` & `tmp/midpoint-cli-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midpoint-cli-0.9.0.tar", last modified: Fri Dec 17 19:49:00 2021, max compression
+gzip compressed data, was "midpoint-cli-1.0.0.tar", last modified: Fri Jun  2 13:07:03 2023, max compression
```

## Comparing `midpoint-cli-0.9.0.tar` & `midpoint-cli-1.0.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 yk        (1000) yk        (1001)        0 2021-12-17 19:49:00.889679 midpoint-cli-0.9.0/
--rw-r--r--   0 yk        (1000) yk        (1001)     1077 2021-01-30 21:36:56.000000 midpoint-cli-0.9.0/LICENSE
--rw-r--r--   0 yk        (1000) yk        (1001)      605 2021-12-17 19:49:00.889679 midpoint-cli-0.9.0/PKG-INFO
-drwxr-xr-x   0 yk        (1000) yk        (1001)        0 2021-12-17 19:49:00.889679 midpoint-cli-0.9.0/midpoint_cli.egg-info/
--rw-r--r--   0 yk        (1000) yk        (1001)      605 2021-12-17 19:49:00.000000 midpoint-cli-0.9.0/midpoint_cli.egg-info/PKG-INFO
--rw-r--r--   0 yk        (1000) yk        (1001)      788 2021-12-17 19:49:00.000000 midpoint-cli-0.9.0/midpoint_cli.egg-info/SOURCES.txt
--rw-r--r--   0 yk        (1000) yk        (1001)        1 2021-12-17 19:49:00.000000 midpoint-cli-0.9.0/midpoint_cli.egg-info/dependency_links.txt
--rw-r--r--   0 yk        (1000) yk        (1001)       46 2021-12-17 19:49:00.000000 midpoint-cli-0.9.0/midpoint_cli.egg-info/requires.txt
--rw-r--r--   0 yk        (1000) yk        (1001)       13 2021-12-17 19:49:00.000000 midpoint-cli-0.9.0/midpoint_cli.egg-info/top_level.txt
--rw-r--r--   0 yk        (1000) yk        (1001)       63 2021-12-17 19:49:00.893012 midpoint-cli-0.9.0/setup.cfg
--rw-r--r--   0 yk        (1000) yk        (1001)      988 2021-02-27 21:14:01.000000 midpoint-cli-0.9.0/setup.py
-drwxr-xr-x   0 yk        (1000) yk        (1001)        0 2021-12-17 19:49:00.889679 midpoint-cli-0.9.0/src/
--rwxr-xr-x   0 yk        (1000) yk        (1001)     1912 2021-01-30 21:36:56.000000 midpoint-cli-0.9.0/src/midpoint-cli
-drwxr-xr-x   0 yk        (1000) yk        (1001)        0 2021-12-17 19:49:00.889679 midpoint-cli-0.9.0/src/midpoint_cli/
--rw-r--r--   0 yk        (1000) yk        (1001)       22 2021-12-17 19:48:12.000000 midpoint-cli-0.9.0/src/midpoint_cli/__init__.py
--rw-r--r--   0 yk        (1000) yk        (1001)      841 2021-02-27 21:14:01.000000 midpoint-cli-0.9.0/src/midpoint_cli/complete.py
--rw-r--r--   0 yk        (1000) yk        (1001)    12926 2021-12-17 19:34:43.000000 midpoint-cli-0.9.0/src/midpoint_cli/mpclient.py
--rw-r--r--   0 yk        (1000) yk        (1001)      890 2021-01-30 21:36:56.000000 midpoint-cli-0.9.0/src/midpoint_cli/patch.py
--rw-r--r--   0 yk        (1000) yk        (1001)     1583 2021-01-30 21:36:56.000000 midpoint-cli-0.9.0/src/midpoint_cli/prompt.py
--rw-r--r--   0 yk        (1000) yk        (1001)       71 2021-02-27 21:14:01.000000 midpoint-cli-0.9.0/src/midpoint_cli/prompt_base.py
--rw-r--r--   0 yk        (1000) yk        (1001)     1058 2021-02-27 21:14:01.000000 midpoint-cli-0.9.0/src/midpoint_cli/prompt_delete.py
--rw-r--r--   0 yk        (1000) yk        (1001)     1484 2021-02-27 21:14:01.000000 midpoint-cli-0.9.0/src/midpoint_cli/prompt_get.py
--rw-r--r--   0 yk        (1000) yk        (1001)     1647 2021-02-27 21:14:01.000000 midpoint-cli-0.9.0/src/midpoint_cli/prompt_org.py
--rw-r--r--   0 yk        (1000) yk        (1001)     1265 2021-02-27 21:14:01.000000 midpoint-cli-0.9.0/src/midpoint_cli/prompt_put.py
--rw-r--r--   0 yk        (1000) yk        (1001)     2096 2021-02-27 21:14:01.000000 midpoint-cli-0.9.0/src/midpoint_cli/prompt_resource.py
--rw-r--r--   0 yk        (1000) yk        (1001)     1757 2021-02-27 21:14:01.000000 midpoint-cli-0.9.0/src/midpoint_cli/prompt_script.py
--rw-r--r--   0 yk        (1000) yk        (1001)     3419 2021-02-27 21:14:01.000000 midpoint-cli-0.9.0/src/midpoint_cli/prompt_task.py
--rw-r--r--   0 yk        (1000) yk        (1001)     1645 2021-02-27 21:14:01.000000 midpoint-cli-0.9.0/src/midpoint_cli/prompt_user.py
-drwxr-xr-x   0 yk        (1000) yk        (1001)        0 2021-12-17 19:49:00.889679 midpoint-cli-0.9.0/test/
--rw-r--r--   0 yk        (1000) yk        (1001)     1556 2021-01-30 21:36:56.000000 midpoint-cli-0.9.0/test/test_client_api.py
--rw-r--r--   0 yk        (1000) yk        (1001)      698 2021-01-30 21:36:56.000000 midpoint-cli-0.9.0/test/test_client_model.py
--rw-r--r--   0 yk        (1000) yk        (1001)     1276 2021-01-30 21:36:56.000000 midpoint-cli-0.9.0/test/test_client_put.py
--rw-r--r--   0 yk        (1000) yk        (1001)     1751 2021-01-30 21:36:56.000000 midpoint-cli-0.9.0/test/test_parser.py
--rw-r--r--   0 yk        (1000) yk        (1001)      666 2021-01-30 21:36:56.000000 midpoint-cli-0.9.0/test/test_patch.py
--rw-r--r--   0 yk        (1000) yk        (1001)     1736 2021-01-30 21:36:56.000000 midpoint-cli-0.9.0/test/test_script.py
+drwxr-xr-x   0 yk        (1000) yk        (1001)        0 2023-06-02 13:07:03.700721 midpoint-cli-1.0.0/
+-rw-r--r--   0 yk        (1000) yk        (1001)     1077 2023-04-07 21:38:20.000000 midpoint-cli-1.0.0/LICENSE
+-rw-r--r--   0 yk        (1000) yk        (1001)      577 2023-06-02 13:07:03.700721 midpoint-cli-1.0.0/PKG-INFO
+drwxr-xr-x   0 yk        (1000) yk        (1001)        0 2023-06-02 13:07:03.700721 midpoint-cli-1.0.0/midpoint_cli.egg-info/
+-rw-r--r--   0 yk        (1000) yk        (1001)      577 2023-06-02 13:07:03.000000 midpoint-cli-1.0.0/midpoint_cli.egg-info/PKG-INFO
+-rw-r--r--   0 yk        (1000) yk        (1001)      788 2023-06-02 13:07:03.000000 midpoint-cli-1.0.0/midpoint_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 yk        (1000) yk        (1001)        1 2023-06-02 13:07:03.000000 midpoint-cli-1.0.0/midpoint_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 yk        (1000) yk        (1001)       46 2023-06-02 13:07:03.000000 midpoint-cli-1.0.0/midpoint_cli.egg-info/requires.txt
+-rw-r--r--   0 yk        (1000) yk        (1001)       13 2023-06-02 13:07:03.000000 midpoint-cli-1.0.0/midpoint_cli.egg-info/top_level.txt
+-rw-r--r--   0 yk        (1000) yk        (1001)       63 2023-06-02 13:07:03.700721 midpoint-cli-1.0.0/setup.cfg
+-rw-r--r--   0 yk        (1000) yk        (1001)      988 2023-04-07 21:38:20.000000 midpoint-cli-1.0.0/setup.py
+drwxr-xr-x   0 yk        (1000) yk        (1001)        0 2023-06-02 13:07:03.700721 midpoint-cli-1.0.0/src/
+-rwxr-xr-x   0 yk        (1000) yk        (1001)     1912 2023-04-07 21:38:20.000000 midpoint-cli-1.0.0/src/midpoint-cli
+drwxr-xr-x   0 yk        (1000) yk        (1001)        0 2023-06-02 13:07:03.700721 midpoint-cli-1.0.0/src/midpoint_cli/
+-rw-r--r--   0 yk        (1000) yk        (1001)       22 2023-06-02 13:00:03.000000 midpoint-cli-1.0.0/src/midpoint_cli/__init__.py
+-rw-r--r--   0 yk        (1000) yk        (1001)      841 2023-04-07 21:38:20.000000 midpoint-cli-1.0.0/src/midpoint_cli/complete.py
+-rw-r--r--   0 yk        (1000) yk        (1001)    13081 2023-04-07 21:38:20.000000 midpoint-cli-1.0.0/src/midpoint_cli/mpclient.py
+-rw-r--r--   0 yk        (1000) yk        (1001)      890 2023-04-07 21:38:20.000000 midpoint-cli-1.0.0/src/midpoint_cli/patch.py
+-rw-r--r--   0 yk        (1000) yk        (1001)     1583 2023-04-07 21:38:20.000000 midpoint-cli-1.0.0/src/midpoint_cli/prompt.py
+-rw-r--r--   0 yk        (1000) yk        (1001)       71 2023-04-07 21:38:20.000000 midpoint-cli-1.0.0/src/midpoint_cli/prompt_base.py
+-rw-r--r--   0 yk        (1000) yk        (1001)     1058 2023-04-07 21:38:20.000000 midpoint-cli-1.0.0/src/midpoint_cli/prompt_delete.py
+-rw-r--r--   0 yk        (1000) yk        (1001)     1484 2023-04-07 21:38:20.000000 midpoint-cli-1.0.0/src/midpoint_cli/prompt_get.py
+-rw-r--r--   0 yk        (1000) yk        (1001)     1647 2023-04-07 21:38:20.000000 midpoint-cli-1.0.0/src/midpoint_cli/prompt_org.py
+-rw-r--r--   0 yk        (1000) yk        (1001)     1265 2023-04-07 21:38:20.000000 midpoint-cli-1.0.0/src/midpoint_cli/prompt_put.py
+-rw-r--r--   0 yk        (1000) yk        (1001)     2096 2023-04-07 21:38:20.000000 midpoint-cli-1.0.0/src/midpoint_cli/prompt_resource.py
+-rw-r--r--   0 yk        (1000) yk        (1001)     1757 2023-04-07 21:38:20.000000 midpoint-cli-1.0.0/src/midpoint_cli/prompt_script.py
+-rw-r--r--   0 yk        (1000) yk        (1001)     3610 2023-04-07 21:38:20.000000 midpoint-cli-1.0.0/src/midpoint_cli/prompt_task.py
+-rw-r--r--   0 yk        (1000) yk        (1001)     1645 2023-04-07 21:38:20.000000 midpoint-cli-1.0.0/src/midpoint_cli/prompt_user.py
+drwxr-xr-x   0 yk        (1000) yk        (1001)        0 2023-06-02 13:07:03.700721 midpoint-cli-1.0.0/test/
+-rw-r--r--   0 yk        (1000) yk        (1001)     1556 2023-04-07 21:38:20.000000 midpoint-cli-1.0.0/test/test_client_api.py
+-rw-r--r--   0 yk        (1000) yk        (1001)      698 2023-04-07 21:38:20.000000 midpoint-cli-1.0.0/test/test_client_model.py
+-rw-r--r--   0 yk        (1000) yk        (1001)     1276 2023-04-07 21:38:20.000000 midpoint-cli-1.0.0/test/test_client_put.py
+-rw-r--r--   0 yk        (1000) yk        (1001)     1751 2023-04-07 21:38:20.000000 midpoint-cli-1.0.0/test/test_parser.py
+-rw-r--r--   0 yk        (1000) yk        (1001)      666 2023-04-07 21:38:20.000000 midpoint-cli-1.0.0/test/test_patch.py
+-rw-r--r--   0 yk        (1000) yk        (1001)     1736 2023-04-07 21:38:20.000000 midpoint-cli-1.0.0/test/test_script.py
```

### Comparing `midpoint-cli-0.9.0/LICENSE` & `midpoint-cli-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `midpoint-cli-0.9.0/PKG-INFO` & `midpoint-cli-1.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 Metadata-Version: 2.1
 Name: midpoint-cli
-Version: 0.9.0
+Version: 1.0.0
 Summary: A command line client to Midpoint Identity Management system.
 Home-page: https://gitlab.com/alcibiade/midpoint-cli
 Author: Yannick Kirschhoffer
 Author-email: alcibiade@alcibiade.org
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: System :: Systems Administration
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `midpoint-cli-0.9.0/midpoint_cli.egg-info/PKG-INFO` & `midpoint-cli-1.0.0/midpoint_cli.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 Metadata-Version: 2.1
 Name: midpoint-cli
-Version: 0.9.0
+Version: 1.0.0
 Summary: A command line client to Midpoint Identity Management system.
 Home-page: https://gitlab.com/alcibiade/midpoint-cli
 Author: Yannick Kirschhoffer
 Author-email: alcibiade@alcibiade.org
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: System :: Systems Administration
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `midpoint-cli-0.9.0/midpoint_cli.egg-info/SOURCES.txt` & `midpoint-cli-1.0.0/midpoint_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `midpoint-cli-0.9.0/setup.py` & `midpoint-cli-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `midpoint-cli-0.9.0/src/midpoint-cli` & `midpoint-cli-1.0.0/src/midpoint-cli`

 * *Files identical despite different names*

### Comparing `midpoint-cli-0.9.0/src/midpoint_cli/complete.py` & `midpoint-cli-1.0.0/src/midpoint_cli/complete.py`

 * *Files identical despite different names*

### Comparing `midpoint-cli-0.9.0/src/midpoint_cli/mpclient.py` & `midpoint-cli-1.0.0/src/midpoint_cli/mpclient.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,17 +59,21 @@
 class MidpointTask(MidpointObject):
 
     def __init__(self, xml_entity: Element):
         super().__init__()
         self['OID'] = xml_entity.attrib['oid']
         self['Name'] = xml_entity.find('c:name', namespaces).text
 
-        # Execution status is not always present since Midpoint 4.4
         execution_status_entity = xml_entity.find('c:executionStatus', namespaces)
-        self['Execution Status'] = execution_status_entity.text if execution_status_entity else 'n/a'
+
+        # Execution status is renamed executionState since Midpoint 4.4
+        if execution_status_entity is None:
+            execution_status_entity = xml_entity.find('c:executionState', namespaces)
+
+        self['Execution Status'] = execution_status_entity.text if execution_status_entity is not None else 'n/a'
 
         # Midpoint before version 4.2
 
         rs = xml_entity.find('c:resultStatus', namespaces)
 
         # As of Midpoint 4.2, the result has moved
 
@@ -184,15 +188,15 @@
         return response.content.decode()
 
     def get_elements(self, element_class: str) -> Element:
         rest_type = self.resolve_rest_type(element_class)
 
         url = urljoin(self.url, 'ws/rest/' + rest_type)
         response = self.requests_session.get(url=url, auth=(self.username, self.password))
-        if response.status_code != 200:
+        if response.status_code >= 300:
             raise MidpointServerError('Server responded with status code %d on %s' % (response.status_code, url))
 
         tree = ElementTree.fromstring(response.content)
         return tree
 
     def execute_action(self, element_class: str, element_oid: str, action: str) -> bytes:
         rest_type = self.resolve_rest_type(element_class)
@@ -333,15 +337,15 @@
         with AsciiProgressMonitor() as progress:
             while True:
                 time.sleep(2)
                 task_xml = self.api_client.get_element('task', task_oid)
                 task_root = ElementTree.fromstring(task_xml)
                 task = MidpointTask(task_root)
 
-                progress.update(int(task['Progress']))
+                progress.update(int(task['Progress'] or '0'))
 
                 rstatus = task['Result Status']
 
                 if rstatus != 'in_progress':
                     print()
                     if rstatus != 'success':
                         raise TaskExecutionFailure('Failed execution of task ' + task_oid + ' with status ' + rstatus)
```

### Comparing `midpoint-cli-0.9.0/src/midpoint_cli/patch.py` & `midpoint-cli-1.0.0/src/midpoint_cli/patch.py`

 * *Files identical despite different names*

### Comparing `midpoint-cli-0.9.0/src/midpoint_cli/prompt.py` & `midpoint-cli-1.0.0/src/midpoint_cli/prompt.py`

 * *Files identical despite different names*

### Comparing `midpoint-cli-0.9.0/src/midpoint_cli/prompt_delete.py` & `midpoint-cli-1.0.0/src/midpoint_cli/prompt_delete.py`

 * *Files identical despite different names*

### Comparing `midpoint-cli-0.9.0/src/midpoint_cli/prompt_get.py` & `midpoint-cli-1.0.0/src/midpoint_cli/prompt_get.py`

 * *Files identical despite different names*

### Comparing `midpoint-cli-0.9.0/src/midpoint_cli/prompt_org.py` & `midpoint-cli-1.0.0/src/midpoint_cli/prompt_org.py`

 * *Files identical despite different names*

### Comparing `midpoint-cli-0.9.0/src/midpoint_cli/prompt_put.py` & `midpoint-cli-1.0.0/src/midpoint_cli/prompt_put.py`

 * *Files identical despite different names*

### Comparing `midpoint-cli-0.9.0/src/midpoint_cli/prompt_resource.py` & `midpoint-cli-1.0.0/src/midpoint_cli/prompt_resource.py`

 * *Files identical despite different names*

### Comparing `midpoint-cli-0.9.0/src/midpoint_cli/prompt_script.py` & `midpoint-cli-1.0.0/src/midpoint_cli/prompt_script.py`

 * *Files identical despite different names*

### Comparing `midpoint-cli-0.9.0/src/midpoint_cli/prompt_task.py` & `midpoint-cli-1.0.0/src/midpoint_cli/prompt_task.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import shlex
 from argparse import ArgumentParser, RawTextHelpFormatter
 
 import tabulate
 
 # Task command wrapper parser
+from midpoint_cli.mpclient import TaskExecutionFailure
 from midpoint_cli.prompt_base import PromptBase
 
 task_parser = ArgumentParser(
     formatter_class=RawTextHelpFormatter,
     prog='task',
     description='Manage server tasks.',
     epilog='''
@@ -79,15 +80,18 @@
                     else:
                         if ns.command == 'run' and task_obj['Execution Status'] == 'suspended':
                             print('Task currently suspended, activating it...')
                             self.client.task_action(task_obj.get_oid(), 'resume')
                             print('Now running task...')
 
                         print('Task', task_obj.get_name(), '-', ns.command)
-                        self.client.task_action(task_obj.get_oid(), ns.command)
+                        try:
+                            self.client.task_action(task_obj.get_oid(), ns.command)
+                        except TaskExecutionFailure as e:
+                            print(e.message)
 
 
         except SystemExit:
             pass
 
     def help_task(self):
         task_parser.print_help()
```

### Comparing `midpoint-cli-0.9.0/src/midpoint_cli/prompt_user.py` & `midpoint-cli-1.0.0/src/midpoint_cli/prompt_user.py`

 * *Files identical despite different names*

### Comparing `midpoint-cli-0.9.0/test/test_client_api.py` & `midpoint-cli-1.0.0/test/test_client_api.py`

 * *Files identical despite different names*

### Comparing `midpoint-cli-0.9.0/test/test_client_model.py` & `midpoint-cli-1.0.0/test/test_client_model.py`

 * *Files identical despite different names*

### Comparing `midpoint-cli-0.9.0/test/test_client_put.py` & `midpoint-cli-1.0.0/test/test_client_put.py`

 * *Files identical despite different names*

### Comparing `midpoint-cli-0.9.0/test/test_parser.py` & `midpoint-cli-1.0.0/test/test_parser.py`

 * *Files identical despite different names*

### Comparing `midpoint-cli-0.9.0/test/test_patch.py` & `midpoint-cli-1.0.0/test/test_patch.py`

 * *Files identical despite different names*

### Comparing `midpoint-cli-0.9.0/test/test_script.py` & `midpoint-cli-1.0.0/test/test_script.py`

 * *Files identical despite different names*

