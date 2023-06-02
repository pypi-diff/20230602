# Comparing `tmp/jax-tools-1.0.30.tar.gz` & `tmp/jax-tools-1.0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax-tools-1.0.30.tar", last modified: Fri Jun  2 07:32:48 2023, max compression
+gzip compressed data, was "jax-tools-1.0.32.tar", last modified: Fri Jun  2 08:48:37 2023, max compression
```

## Comparing `jax-tools-1.0.30.tar` & `jax-tools-1.0.32.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-02 07:32:48.649627 jax-tools-1.0.30/
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      965 2023-06-02 07:32:48.648973 jax-tools-1.0.30/PKG-INFO
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      582 2023-06-01 06:56:40.000000 jax-tools-1.0.30/README.md
-drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-02 07:32:48.640334 jax-tools-1.0.30/jax_tools/
--rw-r--r--   0 cyber.anonym   (501) staff       (20)        0 2023-05-31 12:57:36.000000 jax-tools-1.0.30/jax_tools/__init__.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     6222 2023-06-01 10:53:38.000000 jax-tools-1.0.30/jax_tools/colorful_font.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     4387 2023-06-02 06:44:22.000000 jax-tools-1.0.30/jax_tools/encrypt.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     1733 2023-06-02 06:47:01.000000 jax-tools-1.0.30/jax_tools/jax_encrypt.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     1919 2023-06-01 08:32:18.000000 jax-tools-1.0.30/jax_tools/logger.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     3385 2023-06-02 07:27:14.000000 jax-tools-1.0.30/jax_tools/network_test.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      651 2023-06-02 07:00:58.000000 jax-tools-1.0.30/jax_tools/proxies.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     2765 2023-06-02 07:32:47.000000 jax-tools-1.0.30/jax_tools/ssh.py
-drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-02 07:32:48.648254 jax-tools-1.0.30/jax_tools/utils/
--rw-r--r--   0 cyber.anonym   (501) staff       (20)        0 2023-05-31 13:11:26.000000 jax-tools-1.0.30/jax_tools/utils/__init__.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      254 2023-06-01 08:29:19.000000 jax-tools-1.0.30/jax_tools/utils/settings.py
-drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-02 07:32:48.646166 jax-tools-1.0.30/jax_tools.egg-info/
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      965 2023-06-02 07:32:48.000000 jax-tools-1.0.30/jax_tools.egg-info/PKG-INFO
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      453 2023-06-02 07:32:48.000000 jax-tools-1.0.30/jax_tools.egg-info/SOURCES.txt
--rw-r--r--   0 cyber.anonym   (501) staff       (20)        1 2023-06-02 07:32:48.000000 jax-tools-1.0.30/jax_tools.egg-info/dependency_links.txt
--rw-r--r--   0 cyber.anonym   (501) staff       (20)       92 2023-06-02 07:32:48.000000 jax-tools-1.0.30/jax_tools.egg-info/entry_points.txt
--rw-r--r--   0 cyber.anonym   (501) staff       (20)       66 2023-06-02 07:32:48.000000 jax-tools-1.0.30/jax_tools.egg-info/requires.txt
--rw-r--r--   0 cyber.anonym   (501) staff       (20)       10 2023-06-02 07:32:48.000000 jax-tools-1.0.30/jax_tools.egg-info/top_level.txt
--rw-r--r--   0 cyber.anonym   (501) staff       (20)       38 2023-06-02 07:32:48.649783 jax-tools-1.0.30/setup.cfg
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     1712 2023-06-02 07:32:47.000000 jax-tools-1.0.30/setup.py
+drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-02 08:48:37.616229 jax-tools-1.0.32/
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      963 2023-06-02 08:48:37.615968 jax-tools-1.0.32/PKG-INFO
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      580 2023-06-02 08:47:19.000000 jax-tools-1.0.32/README.md
+drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-02 08:48:37.611276 jax-tools-1.0.32/jax_tools/
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)        0 2023-05-31 12:57:36.000000 jax-tools-1.0.32/jax_tools/__init__.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)     6222 2023-06-01 10:53:38.000000 jax-tools-1.0.32/jax_tools/colorful_font.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)     4387 2023-06-02 06:44:22.000000 jax-tools-1.0.32/jax_tools/encrypt.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)     1733 2023-06-02 06:47:01.000000 jax-tools-1.0.32/jax_tools/jax_encrypt.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)     1919 2023-06-01 08:32:18.000000 jax-tools-1.0.32/jax_tools/logger.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)     3385 2023-06-02 07:27:14.000000 jax-tools-1.0.32/jax_tools/network_test.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      651 2023-06-02 07:00:58.000000 jax-tools-1.0.32/jax_tools/proxies.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)     2780 2023-06-02 08:47:19.000000 jax-tools-1.0.32/jax_tools/ssh.py
+drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-02 08:48:37.615294 jax-tools-1.0.32/jax_tools/utils/
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)        0 2023-05-31 13:11:26.000000 jax-tools-1.0.32/jax_tools/utils/__init__.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      254 2023-06-01 08:29:19.000000 jax-tools-1.0.32/jax_tools/utils/settings.py
+drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-02 08:48:37.614236 jax-tools-1.0.32/jax_tools.egg-info/
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      963 2023-06-02 08:48:37.000000 jax-tools-1.0.32/jax_tools.egg-info/PKG-INFO
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      453 2023-06-02 08:48:37.000000 jax-tools-1.0.32/jax_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)        1 2023-06-02 08:48:37.000000 jax-tools-1.0.32/jax_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)       92 2023-06-02 08:48:37.000000 jax-tools-1.0.32/jax_tools.egg-info/entry_points.txt
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)       66 2023-06-02 08:48:37.000000 jax-tools-1.0.32/jax_tools.egg-info/requires.txt
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)       10 2023-06-02 08:48:37.000000 jax-tools-1.0.32/jax_tools.egg-info/top_level.txt
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)       38 2023-06-02 08:48:37.616323 jax-tools-1.0.32/setup.cfg
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)     1712 2023-06-02 08:48:36.000000 jax-tools-1.0.32/setup.py
```

### Comparing `jax-tools-1.0.30/PKG-INFO` & `jax-tools-1.0.32/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-tools
-Version: 1.0.30
+Version: 1.0.32
 Summary: Jax common tools library
 Home-page: https://jax-arsenals.com
 Download-URL: https://jax-arsenals.com
 Author: Jax
 Author-email: alvin.wan.cn@hotmail.com
 License: MIT Licence
 Keywords: jax
@@ -46,12 +46,12 @@
 logger.warning('warning')
 logger.error('error')
 logger.critical('critical')
 ```
 ### Use ssh
 
 ```python
-from jax_tools.ssh import SSHConnect
-ssh_client = SSHConnect(host='dest_ip', port=22, username='username', password='password')
+from jax_tools.ssh import SSHClient
+ssh_client = SSHClient(host='dest_ip', port=22, username='username', password='password')
 print(ssh_client.run_cmd('ls'))
 ```
```

### Comparing `jax-tools-1.0.30/README.md` & `jax-tools-1.0.32/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -29,12 +29,12 @@
 logger.warning('warning')
 logger.error('error')
 logger.critical('critical')
 ```
 ### Use ssh
 
 ```python
-from jax_tools.ssh import SSHConnect
-ssh_client = SSHConnect(host='dest_ip', port=22, username='username', password='password')
+from jax_tools.ssh import SSHClient
+ssh_client = SSHClient(host='dest_ip', port=22, username='username', password='password')
 print(ssh_client.run_cmd('ls'))
 ```
```

### Comparing `jax-tools-1.0.30/jax_tools/colorful_font.py` & `jax-tools-1.0.32/jax_tools/colorful_font.py`

 * *Files identical despite different names*

### Comparing `jax-tools-1.0.30/jax_tools/encrypt.py` & `jax-tools-1.0.32/jax_tools/encrypt.py`

 * *Files identical despite different names*

### Comparing `jax-tools-1.0.30/jax_tools/jax_encrypt.py` & `jax-tools-1.0.32/jax_tools/jax_encrypt.py`

 * *Files identical despite different names*

### Comparing `jax-tools-1.0.30/jax_tools/logger.py` & `jax-tools-1.0.32/jax_tools/logger.py`

 * *Files identical despite different names*

### Comparing `jax-tools-1.0.30/jax_tools/network_test.py` & `jax-tools-1.0.32/jax_tools/network_test.py`

 * *Files identical despite different names*

### Comparing `jax-tools-1.0.30/jax_tools/proxies.py` & `jax-tools-1.0.32/jax_tools/proxies.py`

 * *Files identical despite different names*

### Comparing `jax-tools-1.0.30/jax_tools/ssh.py` & `jax-tools-1.0.32/jax_tools/ssh.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 # -*- coding: utf-8 -*-
 """
 ssh operations
 """
 import paramiko
 from jax_tools.logger import logger
-import logging
-logging.getLogger("paramiko").setLevel(logging.WARNING)
 
 
-class SSHConnect(object):
+class SSHClient(object):
     """
     SSH Connector
     """
 
     def __init__(self, host, port, username, password) -> None:
         """
         SSH Connector
@@ -95,7 +93,10 @@
 
         """
         self.ssh_client.close()
 
     def __del__(self):
         if self.ssh_client:
             self.close()
+
+if __name__ == '__main__':
+    print(SSHClient('vm37',22,'root','').run_cmd('whoami'))
```

### Comparing `jax-tools-1.0.30/jax_tools.egg-info/PKG-INFO` & `jax-tools-1.0.32/jax_tools.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-tools
-Version: 1.0.30
+Version: 1.0.32
 Summary: Jax common tools library
 Home-page: https://jax-arsenals.com
 Download-URL: https://jax-arsenals.com
 Author: Jax
 Author-email: alvin.wan.cn@hotmail.com
 License: MIT Licence
 Keywords: jax
@@ -46,12 +46,12 @@
 logger.warning('warning')
 logger.error('error')
 logger.critical('critical')
 ```
 ### Use ssh
 
 ```python
-from jax_tools.ssh import SSHConnect
-ssh_client = SSHConnect(host='dest_ip', port=22, username='username', password='password')
+from jax_tools.ssh import SSHClient
+ssh_client = SSHClient(host='dest_ip', port=22, username='username', password='password')
 print(ssh_client.run_cmd('ls'))
 ```
```

### Comparing `jax-tools-1.0.30/setup.py` & `jax-tools-1.0.32/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     """
     with open(file_path, 'r') as f:
         return f.read()
 
 
 setuptools.setup(
     name="jax-tools",
-    version="1.0.30",
+    version="1.0.32",
     author=u"Jax",
     author_email='alvin.wan.cn@hotmail.com',
     description=u"Jax common tools library",
     platforms=['CentOS', 'Redhat', 'MacOS', 'Windows'],
     long_description=read_file('README.md'),
     long_description_content_type="text/markdown",
     url="https://jax-arsenals.com",
```

