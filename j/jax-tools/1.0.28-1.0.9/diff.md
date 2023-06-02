# Comparing `tmp/jax-tools-1.0.28.tar.gz` & `tmp/jax-tools-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax-tools-1.0.28.tar", last modified: Fri Jun  2 07:27:15 2023, max compression
+gzip compressed data, was "jax-tools-1.0.9.tar", last modified: Thu Jun  1 04:58:33 2023, max compression
```

## Comparing `jax-tools-1.0.28.tar` & `jax-tools-1.0.9.tar`

### file list

```diff
@@ -1,24 +1,21 @@
-drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-02 07:27:15.135315 jax-tools-1.0.28/
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      965 2023-06-02 07:27:15.134923 jax-tools-1.0.28/PKG-INFO
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      582 2023-06-01 06:56:40.000000 jax-tools-1.0.28/README.md
-drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-02 07:27:15.122415 jax-tools-1.0.28/jax_tools/
--rw-r--r--   0 cyber.anonym   (501) staff       (20)        0 2023-05-31 12:57:36.000000 jax-tools-1.0.28/jax_tools/__init__.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     6222 2023-06-01 10:53:38.000000 jax-tools-1.0.28/jax_tools/colorful_font.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     4387 2023-06-02 06:44:22.000000 jax-tools-1.0.28/jax_tools/encrypt.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     1733 2023-06-02 06:47:01.000000 jax-tools-1.0.28/jax_tools/jax_encrypt.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     1919 2023-06-01 08:32:18.000000 jax-tools-1.0.28/jax_tools/logger.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     3385 2023-06-02 07:27:14.000000 jax-tools-1.0.28/jax_tools/network_test.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      651 2023-06-02 07:00:58.000000 jax-tools-1.0.28/jax_tools/proxies.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     2694 2023-06-01 11:45:26.000000 jax-tools-1.0.28/jax_tools/ssh.py
-drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-02 07:27:15.131012 jax-tools-1.0.28/jax_tools/utils/
--rw-r--r--   0 cyber.anonym   (501) staff       (20)        0 2023-05-31 13:11:26.000000 jax-tools-1.0.28/jax_tools/utils/__init__.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      254 2023-06-01 08:29:19.000000 jax-tools-1.0.28/jax_tools/utils/settings.py
-drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-02 07:27:15.129616 jax-tools-1.0.28/jax_tools.egg-info/
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      965 2023-06-02 07:27:14.000000 jax-tools-1.0.28/jax_tools.egg-info/PKG-INFO
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      453 2023-06-02 07:27:14.000000 jax-tools-1.0.28/jax_tools.egg-info/SOURCES.txt
--rw-r--r--   0 cyber.anonym   (501) staff       (20)        1 2023-06-02 07:27:14.000000 jax-tools-1.0.28/jax_tools.egg-info/dependency_links.txt
--rw-r--r--   0 cyber.anonym   (501) staff       (20)       92 2023-06-02 07:27:14.000000 jax-tools-1.0.28/jax_tools.egg-info/entry_points.txt
--rw-r--r--   0 cyber.anonym   (501) staff       (20)       66 2023-06-02 07:27:14.000000 jax-tools-1.0.28/jax_tools.egg-info/requires.txt
--rw-r--r--   0 cyber.anonym   (501) staff       (20)       10 2023-06-02 07:27:14.000000 jax-tools-1.0.28/jax_tools.egg-info/top_level.txt
--rw-r--r--   0 cyber.anonym   (501) staff       (20)       38 2023-06-02 07:27:15.135409 jax-tools-1.0.28/setup.cfg
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     1712 2023-06-02 07:27:14.000000 jax-tools-1.0.28/setup.py
+drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-01 04:58:33.625723 jax-tools-1.0.9/
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      392 2023-06-01 04:58:33.625277 jax-tools-1.0.9/PKG-INFO
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)       28 2023-06-01 03:10:01.000000 jax-tools-1.0.9/README.md
+drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-01 04:58:33.617631 jax-tools-1.0.9/jax_tools/
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      378 2023-06-01 03:54:45.000000 jax-tools-1.0.9/jax_tools/CHANGELOG.md
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)        0 2023-05-31 12:57:36.000000 jax-tools-1.0.9/jax_tools/__init__.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)     1919 2023-06-01 03:00:26.000000 jax-tools-1.0.9/jax_tools/logger.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)     2901 2023-06-01 02:46:34.000000 jax-tools-1.0.9/jax_tools/network_test.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)     2819 2023-06-01 04:58:18.000000 jax-tools-1.0.9/jax_tools/ssh_ops.py
+drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-01 04:58:33.624649 jax-tools-1.0.9/jax_tools/utils/
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)        0 2023-05-31 13:11:26.000000 jax-tools-1.0.9/jax_tools/utils/__init__.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      119 2023-06-01 04:28:51.000000 jax-tools-1.0.9/jax_tools/utils/settings.py
+drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-01 04:58:33.622707 jax-tools-1.0.9/jax_tools.egg-info/
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      392 2023-06-01 04:58:33.000000 jax-tools-1.0.9/jax_tools.egg-info/PKG-INFO
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      386 2023-06-01 04:58:33.000000 jax-tools-1.0.9/jax_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)        1 2023-06-01 04:58:33.000000 jax-tools-1.0.9/jax_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)       51 2023-06-01 04:58:33.000000 jax-tools-1.0.9/jax_tools.egg-info/entry_points.txt
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)       45 2023-06-01 04:58:33.000000 jax-tools-1.0.9/jax_tools.egg-info/requires.txt
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)       10 2023-06-01 04:58:33.000000 jax-tools-1.0.9/jax_tools.egg-info/top_level.txt
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)       38 2023-06-01 04:58:33.625922 jax-tools-1.0.9/setup.cfg
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)     1611 2023-06-01 04:58:18.000000 jax-tools-1.0.9/setup.py
```

### Comparing `jax-tools-1.0.28/jax_tools/logger.py` & `jax-tools-1.0.9/jax_tools/logger.py`

 * *Files identical despite different names*

### Comparing `jax-tools-1.0.28/jax_tools/network_test.py` & `jax-tools-1.0.9/jax_tools/network_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,28 +23,25 @@
         else:
             return False
     except Exception as e:
         print(e)
         return False
 
 
-def check_connectivity(ip, port, need_print_msg=False):
+def check_connectivity(ip, port):
     """
     检查目标IP和端口是否可以连接
     Args:
-        ip (str): Destination IP address or hostname
-        port (int): Destination port
-        need_print_msg (bool): Whether to print the result
+        ip: 目标IP
+        port:  目标端口
 
     Returns:
         True if the port is open
         False if the port is closed or the connection is refused
     """
-    print_msg = PrintMSG
-    print_msg.need_print = need_print_msg
     s = None
     network_unreachable = 'Network is unreachable'
     result_dict = {
         35: 'The port is closed',
         61: 'Connection refused, firewall restrictions may be set on the target port',
         111: 'Connection refused',
         113: 'No route to host',
@@ -63,63 +60,50 @@
         # 创建一个socket对象
         s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         s.settimeout(5)  # 设置超时时间（单位：秒）
         if isinstance(port, str):
             try:
                 port = int(port)
                 if port < 0 or port > 65535:
-                    print_msg("The port must be between 0 and 65535")
+                    print("The port must be between 0 and 65535")
                     sys.exit(1)
             except ValueError:
-                print_msg("The port must be a number")
+                print("The port must be a number")
                 sys.exit(1)
         # 尝试连接到目标IP和端口
         result = s.connect_ex((ip, port))
         if result == 0:
-            print_msg("Connection success")
+            print("Connection success")
             result = True
         elif result in result_dict.keys():
             if check_icmp_connectivity(ip):
-                print_msg("Connection error: " + result_dict[result])
+                print("Connection error: ", result_dict[result])
             else:
-                print_msg("Connection error: " + result_dict[result] + "and ping not work")
+                print("Connection error: ", result_dict[result], "and ping not work")
             result = False
         else:
-            print_msg("Connection error：" + str(result))
+            print("Connection error：", result)
             result = False
     except socket.error as e:
-        print_msg("Connection error：" + e)
+        print("Connection error：", e)
         result = False
     finally:
         if s:
             s.close()
     return result
 
 
-class PrintMSG(object):
-    """
-    Print message
-    """
-    need_print = True
-
-    def __init__(self, msg):
-        """
-        Init
-        Args:
-            msg (str): Message to print
-        """
-        if self.need_print:
-            print(msg)
-
-
 def main():
     """
     Main function
     Returns:
 
     """
     if len(sys.argv) == 3:
         target_ip = sys.argv[1]
         target_port = int(sys.argv[2])
-        check_connectivity(target_ip, target_port, True)
+        check_connectivity(target_ip, target_port)
     else:
-        print("Usage: nd <TargetIP> <TargetPort>")
+        print("Usage: ns <TargetIP> <TargetPort>")
+
+
+
```

### Comparing `jax-tools-1.0.28/jax_tools/ssh.py` & `jax-tools-1.0.9/jax_tools/ssh_ops.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 ssh operations
 """
 import paramiko
-from jax_tools.logger import logger
+import traceback
+import logging
 
 
 class SSHConnect(object):
     """
     SSH Connector
     """
 
@@ -21,42 +22,46 @@
             password (str): password
         """
         self.host = host
         self.username = username
         self.password = password
         self.port = port
         self.ssh_client = self.__get_ssh_client()
+        if self.ssh_client is None:
+            print('SSH connection failed')
 
     def __get_ssh_client(self):
         """
         Get ssh client
         Args:
 
         Returns:
-            ssh client or None
+            ssh client
 
         """
+        paramiko_logger = paramiko.util.logging.getLogger()
+        paramiko_logger.setLevel(logging.WARN)
         client = paramiko.SSHClient()
         client.set_missing_host_key_policy(paramiko.AutoAddPolicy())
         response = True
         try:
             client.connect(
                 self.host,
                 self.port,
                 username=str(self.username),
                 password=str(self.password),
                 timeout=10)
         except paramiko.ssh_exception.AuthenticationException:
-            logger.error('authentication failed')
+            paramiko_logger.error('身份验证失败')
             response = None
         except paramiko.ssh_exception.NoValidConnectionsError:
-            logger.error('can not connect to host')
+            paramiko_logger.error('无法连接到目标主机')
             response = None
         except Exception as e:
-            logger.error(e)
+            paramiko_logger.error(e)
             response = None
         if response:
             return client
         else:
             return response
 
     def run_cmd(self, cmd, read_line=False, time_out=300):
@@ -67,33 +72,33 @@
             read_line (bool): True if read line by line, False if read all
             time_out (int): timeout in seconds
 
         Returns:
             String if read_line is False
 
         """
-        result = None
         if self.ssh_client is None:
-            logger.warning('SSH connection failed')
-            return result
+            return 'SSH connection failed'
         try:
             std_in, std_out, std_err = self.ssh_client.exec_command(cmd, timeout=time_out)
             if read_line:
                 result = std_out.readlines()
             else:
                 result = std_out.read().decode('utf-8').rstrip()
         except Exception as e:
-            logger.error('Connection exception, User login info may be wrong, or connection has been closed, '
-                         ' msg: %s' % e)
+            logging.error(traceback.format_exc())
+            logging.error(e)
+            result = 'user login info may be wrong'
         return result
 
     def close(self) -> None:
         """
         Close ssh connection
         Returns:
 
         """
         self.ssh_client.close()
 
     def __del__(self):
         if self.ssh_client:
             self.close()
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `jax-tools-1.0.28/setup.py` & `jax-tools-1.0.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,20 +16,20 @@
     """
     with open(file_path, 'r') as f:
         return f.read()
 
 
 setuptools.setup(
     name="jax-tools",
-    version="1.0.28",
+    version="1.0.9",
     author=u"Jax",
     author_email='alvin.wan.cn@hotmail.com',
     description=u"Jax common tools library",
     platforms=['CentOS', 'Redhat', 'MacOS', 'Windows'],
-    long_description=read_file('README.md'),
+    long_description='Jax Tools',
     long_description_content_type="text/markdown",
     url="https://jax-arsenals.com",
     license="MIT Licence",
     python_requires=">=3.0.0",
     # 定义要构建到包中的文件列表，这些文件会放到/usr/local下
     data_files=[],
     packages=['jax_tools', 'jax_tools.utils', ],
@@ -46,17 +46,15 @@
     download_url="https://jax-arsenals.com",
     # 定义可以为哪些模块提供依赖
     provides=[],
     install_requires=[
         "ping3 >= 4.0.4",
         "paramiko >= 3.2.0",
         "colorlog >= 6.7.0",
-        "pycryptodome >= 3.18.0",
     ],
     # 定义entry points, 前面的sta指的是命令，第二个sta表示模块名，也是目录名，第三个sta表示脚本名，最好那个main，表示sta.py中的main函数
     entry_points={
         'console_scripts': [
-            'nd=jax_tools.network_test:main',
-            'jax-encrypt=jax_tools.jax_encrypt:main',
+            'ns=jax_tools.network_test:main'
         ]
     }
 )
```

