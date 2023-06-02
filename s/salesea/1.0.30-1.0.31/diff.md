# Comparing `tmp/salesea-1.0.30.tar.gz` & `tmp/salesea-1.0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salesea-1.0.30.tar", last modified: Mon May 29 08:31:28 2023, max compression
+gzip compressed data, was "salesea-1.0.31.tar", last modified: Fri Jun  2 01:38:29 2023, max compression
```

## Comparing `salesea-1.0.30.tar` & `salesea-1.0.31.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 08:31:28.057137 salesea-1.0.30/
--rw-rw-rw-   0        0        0     2588 2023-05-29 08:31:28.057137 salesea-1.0.30/PKG-INFO
--rw-rw-rw-   0        0        0     1613 2023-05-29 03:44:29.000000 salesea-1.0.30/README.md
--rw-rw-rw-   0        0        0      111 2023-05-29 08:31:28.057137 salesea-1.0.30/setup.cfg
--rw-rw-rw-   0        0        0     2312 2023-05-29 08:31:18.000000 salesea-1.0.30/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-29 08:31:28.037019 salesea-1.0.30/src/
-drwxrwxrwx   0        0        0        0 2023-05-29 08:31:28.050137 salesea-1.0.30/src/salesea/
--rw-rw-rw-   0        0        0     6571 2023-05-29 06:18:27.000000 salesea-1.0.30/src/salesea/__command__.py
--rw-rw-rw-   0        0        0       25 2023-05-18 07:08:55.000000 salesea-1.0.30/src/salesea/__init__.py
--rw-rw-rw-   0        0        0     5833 2023-05-29 06:15:02.000000 salesea-1.0.30/src/salesea/__main__.py
--rw-rw-rw-   0        0        0     7628 2023-05-29 05:35:49.000000 salesea-1.0.30/src/salesea/app.py
--rw-rw-rw-   0        0        0     3580 2023-05-29 06:01:45.000000 salesea-1.0.30/src/salesea/config.py
--rw-rw-rw-   0        0        0     1214 2023-05-22 05:27:18.000000 salesea-1.0.30/src/salesea/log.py
--rw-rw-rw-   0        0        0    23808 2023-05-29 08:31:12.000000 salesea-1.0.30/src/salesea/nginx.py
--rw-rw-rw-   0        0        0      970 2023-05-24 10:13:19.000000 salesea-1.0.30/src/salesea/solution.py
--rw-rw-rw-   0        0        0      134 2023-05-18 07:39:33.000000 salesea-1.0.30/src/salesea/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-29 08:31:28.055137 salesea-1.0.30/src/salesea.egg-info/
--rw-rw-rw-   0        0        0     2588 2023-05-29 08:31:27.000000 salesea-1.0.30/src/salesea.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      441 2023-05-29 08:31:28.000000 salesea-1.0.30/src/salesea.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 08:31:27.000000 salesea-1.0.30/src/salesea.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-29 08:31:27.000000 salesea-1.0.30/src/salesea.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-05-29 08:31:27.000000 salesea-1.0.30/src/salesea.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-29 08:31:27.000000 salesea-1.0.30/src/salesea.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 01:38:29.968793 salesea-1.0.31/
+-rw-rw-rw-   0        0        0     2588 2023-06-02 01:38:29.969793 salesea-1.0.31/PKG-INFO
+-rw-rw-rw-   0        0        0     1613 2023-05-29 03:44:29.000000 salesea-1.0.31/README.md
+-rw-rw-rw-   0        0        0      111 2023-06-02 01:38:29.969793 salesea-1.0.31/setup.cfg
+-rw-rw-rw-   0        0        0     2312 2023-06-02 01:38:24.000000 salesea-1.0.31/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 01:38:29.947793 salesea-1.0.31/src/
+drwxrwxrwx   0        0        0        0 2023-06-02 01:38:29.961793 salesea-1.0.31/src/salesea/
+-rw-rw-rw-   0        0        0     6571 2023-05-29 06:18:27.000000 salesea-1.0.31/src/salesea/__command__.py
+-rw-rw-rw-   0        0        0       25 2023-05-18 07:08:55.000000 salesea-1.0.31/src/salesea/__init__.py
+-rw-rw-rw-   0        0        0     5833 2023-05-29 06:15:02.000000 salesea-1.0.31/src/salesea/__main__.py
+-rw-rw-rw-   0        0        0     8109 2023-06-02 01:35:39.000000 salesea-1.0.31/src/salesea/app.py
+-rw-rw-rw-   0        0        0     3580 2023-05-29 06:01:45.000000 salesea-1.0.31/src/salesea/config.py
+-rw-rw-rw-   0        0        0     1214 2023-05-22 05:27:18.000000 salesea-1.0.31/src/salesea/log.py
+-rw-rw-rw-   0        0        0    23808 2023-05-29 08:31:12.000000 salesea-1.0.31/src/salesea/nginx.py
+-rw-rw-rw-   0        0        0      970 2023-05-24 10:13:19.000000 salesea-1.0.31/src/salesea/solution.py
+-rw-rw-rw-   0        0        0      134 2023-05-18 07:39:33.000000 salesea-1.0.31/src/salesea/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-02 01:38:29.967793 salesea-1.0.31/src/salesea.egg-info/
+-rw-rw-rw-   0        0        0     2588 2023-06-02 01:38:29.000000 salesea-1.0.31/src/salesea.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      441 2023-06-02 01:38:29.000000 salesea-1.0.31/src/salesea.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 01:38:29.000000 salesea-1.0.31/src/salesea.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-02 01:38:29.000000 salesea-1.0.31/src/salesea.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-06-02 01:38:29.000000 salesea-1.0.31/src/salesea.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-02 01:38:29.000000 salesea-1.0.31/src/salesea.egg-info/top_level.txt
```

### Comparing `salesea-1.0.30/PKG-INFO` & `salesea-1.0.31/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salesea
-Version: 1.0.30
+Version: 1.0.31
 Summary: This is an Nginx log collection tool.
 Author: howard
 Author-email: 18071131140telephone@gmail.com
 Keywords: nginx,logs,collection
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.0
```

### Comparing `salesea-1.0.30/README.md` & `salesea-1.0.31/README.md`

 * *Files identical despite different names*

### Comparing `salesea-1.0.30/setup.py` & `salesea-1.0.31/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #     print(requires.splitlines())
 # ------------------------------------------------------------------------------- #
 
 setup(
     name='salesea',
     author='howard',
     author_email='18071131140telephone@gmail.com',
-    version='1.0.30',
+    version='1.0.31',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     description='This is an Nginx log collection tool.',
     long_description=readme,
     long_description_content_type='text/markdown',
     keywords=[
         'nginx',
```

### Comparing `salesea-1.0.30/src/salesea/__command__.py` & `salesea-1.0.31/src/salesea/__command__.py`

 * *Files identical despite different names*

### Comparing `salesea-1.0.30/src/salesea/__main__.py` & `salesea-1.0.31/src/salesea/__main__.py`

 * *Files identical despite different names*

### Comparing `salesea-1.0.30/src/salesea/app.py` & `salesea-1.0.31/src/salesea/app.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,26 @@
 from pathlib import Path
 
 from .nginx import Nginx, NginxException
 from .log import logger
 from .solution import print_solution
 
 
+# 输入迭代器和一个数字n，返回n个元素的列表，直到迭代器耗尽，不使用islice， 使用yield
+def take(iterable, n):
+    result = []
+    for i in iterable:
+        result.append(i)
+        if len(result) == n:
+            yield result
+            result = []
+    if result:
+        yield result
+
+
 def launch():
     # 将PID写入文件
     # pid = os.getpid()
     # with open("salesea.pid", "w") as f:sys
     #     f.write(str(pid))
     #############################################################################
     #####Global Variable#########################################################
@@ -105,38 +117,40 @@
         def task():
             count = 0
             with requests.session() as sess:
                 for server in servers:
                     # logger.debug(f"开始扫描日志文件：{[str(server.logfile) for p in servers]}")
                     nginx_log_iter = parse_nginx_log(server.logfile, log_pattern)
 
-                    for data in nginx_log_iter:
-                        try:
-                            # 使用并发请求
+                    for datas in take(nginx_log_iter, 100):
+                        send_data = []
+                        for data in datas:
                             d = re.match(r"[a-zA-Z]+\s(?P<path>/.*?)(?P<query>\?.*?)?\s",
                                          data['request']).groupdict()
-                            data = {
+                            send_data.append({
                                 'visitApiKey': SERVER_MAP.get(server.default_name),
                                 'domain': server.default_name or server.names[0],
                                 'path': d.get('path'),
                                 'query': d.get('query'),
                                 'referrer': data['http_referer'],
                                 'user_agent': data['http_user_agent'],
                                 'ip': data['remote_addr'],
-                            }
-                            result: requests.Response = sess.post('https://salesea.cn/api/visit', data=json.dumps(data),
+                            })
+                        try:
+                            result: requests.Response = sess.post('https://salesea.cn/api/visit/batch',
+                                                                  data=json.dumps(send_data),
                                                                   headers={
                                                                       'Content-Type': 'application/json'
                                                                   })
-                            count += 1
+                            count += len(send_data)
                             obj = result.json()
                             if obj['code'] == 'error':
                                 logger.error(f"响应错误: {obj} - {data}")
                             else:
-                                logger.debug(f"响应结果: {obj}")
+                                logger.info(f"响应结果: {obj}")
                         except Exception as e:
                             logger.error(f"请求错误: {e} - {data}")
 
             logger.__getattribute__('info' if count else 'debug')(f"解析到[{count}]条日志")
 
         task()
```

### Comparing `salesea-1.0.30/src/salesea/config.py` & `salesea-1.0.31/src/salesea/config.py`

 * *Files identical despite different names*

### Comparing `salesea-1.0.30/src/salesea/log.py` & `salesea-1.0.31/src/salesea/log.py`

 * *Files identical despite different names*

### Comparing `salesea-1.0.30/src/salesea/nginx.py` & `salesea-1.0.31/src/salesea/nginx.py`

 * *Files identical despite different names*

### Comparing `salesea-1.0.30/src/salesea/solution.py` & `salesea-1.0.31/src/salesea/solution.py`

 * *Files identical despite different names*

### Comparing `salesea-1.0.30/src/salesea.egg-info/PKG-INFO` & `salesea-1.0.31/src/salesea.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salesea
-Version: 1.0.30
+Version: 1.0.31
 Summary: This is an Nginx log collection tool.
 Author: howard
 Author-email: 18071131140telephone@gmail.com
 Keywords: nginx,logs,collection
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.0
```

