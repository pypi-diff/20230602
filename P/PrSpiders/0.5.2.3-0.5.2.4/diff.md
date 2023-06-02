# Comparing `tmp/PrSpiders-0.5.2.3.tar.gz` & `tmp/PrSpiders-0.5.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PrSpiders-0.5.2.3.tar", last modified: Fri May 26 09:31:22 2023, max compression
+gzip compressed data, was "PrSpiders-0.5.2.4.tar", last modified: Fri Jun  2 02:53:07 2023, max compression
```

## Comparing `PrSpiders-0.5.2.3.tar` & `PrSpiders-0.5.2.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 09:31:22.051569 PrSpiders-0.5.2.3/
--rw-rw-rw-   0        0        0     1091 2023-02-21 09:22:44.000000 PrSpiders-0.5.2.3/LICENSE.txt
--rw-rw-rw-   0        0        0     5497 2023-05-26 09:31:22.047565 PrSpiders-0.5.2.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-26 09:31:21.763574 PrSpiders-0.5.2.3/PrSpider/
--rw-rw-rw-   0        0        0    11294 2023-05-26 09:30:37.000000 PrSpiders-0.5.2.3/PrSpider/PrSpiders.py
--rw-rw-rw-   0        0        0       98 2023-05-23 06:27:42.000000 PrSpiders-0.5.2.3/PrSpider/__init__.py
--rw-rw-rw-   0        0        0     2725 2023-05-26 09:30:30.000000 PrSpiders-0.5.2.3/PrSpider/log.py
--rw-rw-rw-   0        0        0    11257 2023-05-24 01:36:58.000000 PrSpiders-0.5.2.3/PrSpider/pxpath.py
--rw-rw-rw-   0        0        0     3260 2023-05-25 07:23:26.000000 PrSpiders-0.5.2.3/PrSpider/pyconn.py
--rw-rw-rw-   0        0        0     4560 2023-05-23 06:28:17.000000 PrSpiders-0.5.2.3/PrSpider/requestXpath.py
--rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.5.2.3/PrSpider/useragent.py
-drwxrwxrwx   0        0        0        0 2023-05-26 09:31:21.957568 PrSpiders-0.5.2.3/PrSpiders.egg-info/
--rw-rw-rw-   0        0        0     5497 2023-05-26 09:31:21.000000 PrSpiders-0.5.2.3/PrSpiders.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      598 2023-05-26 09:31:21.000000 PrSpiders-0.5.2.3/PrSpiders.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 09:31:21.000000 PrSpiders-0.5.2.3/PrSpiders.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-05-26 09:31:21.000000 PrSpiders-0.5.2.3/PrSpiders.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       55 2023-05-26 09:31:21.000000 PrSpiders-0.5.2.3/PrSpiders.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-05-26 09:31:21.000000 PrSpiders-0.5.2.3/PrSpiders.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5136 2023-05-25 03:36:57.000000 PrSpiders-0.5.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 09:31:21.971568 PrSpiders-0.5.2.3/pkg/
--rw-rw-rw-   0        0        0       23 2023-05-24 01:39:05.000000 PrSpiders-0.5.2.3/pkg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 09:31:22.011568 PrSpiders-0.5.2.3/pkg/prspider/
--rw-rw-rw-   0        0        0     1212 2023-04-20 09:13:43.000000 PrSpiders-0.5.2.3/pkg/prspider/PrSpider_CMD.py
--rw-rw-rw-   0        0        0      257 2023-04-17 12:23:25.000000 PrSpiders-0.5.2.3/pkg/prspider/PrSpider_run.py
--rw-rw-rw-   0        0        0       73 2023-03-31 05:29:27.000000 PrSpiders-0.5.2.3/pkg/prspider/__init__.py
--rw-rw-rw-   0        0        0      833 2023-04-23 03:22:54.000000 PrSpiders-0.5.2.3/pkg/prspider/start.py
-drwxrwxrwx   0        0        0        0 2023-05-26 09:31:22.041564 PrSpiders-0.5.2.3/requestXpath/
--rw-rw-rw-   0        0        0      933 2023-03-23 08:11:59.000000 PrSpiders-0.5.2.3/requestXpath/__init__.py
--rw-rw-rw-   0        0        0     8642 2023-04-18 08:44:05.000000 PrSpiders-0.5.2.3/requestXpath/pxpath.py
--rw-rw-rw-   0        0        0     4210 2023-03-23 08:11:59.000000 PrSpiders-0.5.2.3/requestXpath/requestXpath.py
--rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.5.2.3/requestXpath/useragent.py
--rw-rw-rw-   0        0        0       42 2023-05-26 09:31:22.053566 PrSpiders-0.5.2.3/setup.cfg
--rw-rw-rw-   0        0        0      897 2023-05-26 09:30:52.000000 PrSpiders-0.5.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 02:53:07.105864 PrSpiders-0.5.2.4/
+-rw-rw-rw-   0        0        0     1091 2023-02-21 09:22:44.000000 PrSpiders-0.5.2.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     5497 2023-06-02 02:53:07.043852 PrSpiders-0.5.2.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-02 02:53:03.791852 PrSpiders-0.5.2.4/PrSpider/
+-rw-rw-rw-   0        0        0    11246 2023-06-02 02:52:44.000000 PrSpiders-0.5.2.4/PrSpider/PrSpiders.py
+-rw-rw-rw-   0        0        0       98 2023-05-23 06:27:42.000000 PrSpiders-0.5.2.4/PrSpider/__init__.py
+-rw-rw-rw-   0        0        0     2799 2023-05-29 06:44:50.000000 PrSpiders-0.5.2.4/PrSpider/log.py
+-rw-rw-rw-   0        0        0    11257 2023-05-24 01:36:58.000000 PrSpiders-0.5.2.4/PrSpider/pxpath.py
+-rw-rw-rw-   0        0        0     3260 2023-05-25 07:23:26.000000 PrSpiders-0.5.2.4/PrSpider/pyconn.py
+-rw-rw-rw-   0        0        0     4554 2023-06-02 01:23:50.000000 PrSpiders-0.5.2.4/PrSpider/requestXpath.py
+-rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.5.2.4/PrSpider/useragent.py
+drwxrwxrwx   0        0        0        0 2023-06-02 02:53:04.689852 PrSpiders-0.5.2.4/PrSpiders.egg-info/
+-rw-rw-rw-   0        0        0     5497 2023-06-02 02:53:01.000000 PrSpiders-0.5.2.4/PrSpiders.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      598 2023-06-02 02:53:02.000000 PrSpiders-0.5.2.4/PrSpiders.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 02:53:02.000000 PrSpiders-0.5.2.4/PrSpiders.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-06-02 02:53:02.000000 PrSpiders-0.5.2.4/PrSpiders.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       55 2023-06-02 02:53:02.000000 PrSpiders-0.5.2.4/PrSpiders.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-06-02 02:53:02.000000 PrSpiders-0.5.2.4/PrSpiders.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5136 2023-05-25 03:36:57.000000 PrSpiders-0.5.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 02:53:04.886855 PrSpiders-0.5.2.4/pkg/
+-rw-rw-rw-   0        0        0       23 2023-05-24 01:39:05.000000 PrSpiders-0.5.2.4/pkg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 02:53:05.601858 PrSpiders-0.5.2.4/pkg/prspider/
+-rw-rw-rw-   0        0        0     1212 2023-04-20 09:13:43.000000 PrSpiders-0.5.2.4/pkg/prspider/PrSpider_CMD.py
+-rw-rw-rw-   0        0        0      257 2023-04-17 12:23:25.000000 PrSpiders-0.5.2.4/pkg/prspider/PrSpider_run.py
+-rw-rw-rw-   0        0        0       73 2023-03-31 05:29:27.000000 PrSpiders-0.5.2.4/pkg/prspider/__init__.py
+-rw-rw-rw-   0        0        0      833 2023-04-23 03:22:54.000000 PrSpiders-0.5.2.4/pkg/prspider/start.py
+drwxrwxrwx   0        0        0        0 2023-06-02 02:53:06.952852 PrSpiders-0.5.2.4/requestXpath/
+-rw-rw-rw-   0        0        0      933 2023-03-23 08:11:59.000000 PrSpiders-0.5.2.4/requestXpath/__init__.py
+-rw-rw-rw-   0        0        0     8642 2023-04-18 08:44:05.000000 PrSpiders-0.5.2.4/requestXpath/pxpath.py
+-rw-rw-rw-   0        0        0     4217 2023-06-01 06:51:18.000000 PrSpiders-0.5.2.4/requestXpath/requestXpath.py
+-rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.5.2.4/requestXpath/useragent.py
+-rw-rw-rw-   0        0        0       42 2023-06-02 02:53:07.105864 PrSpiders-0.5.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      897 2023-06-02 02:52:53.000000 PrSpiders-0.5.2.4/setup.py
```

### Comparing `PrSpiders-0.5.2.3/LICENSE.txt` & `PrSpiders-0.5.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.3/PKG-INFO` & `PrSpiders-0.5.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrSpiders
-Version: 0.5.2.3
+Version: 0.5.2.4
 Summary: Inherit the requests module, add xpath functionality to expand the API, and handle request failures and retries
 Home-page: https://github.com/peng0928/prequests
 Author: penr
 Author-email: 1944542244@qq.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `PrSpiders-0.5.2.3/PrSpider/PrSpiders.py` & `PrSpiders-0.5.2.4/PrSpider/PrSpiders.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,15 +181,15 @@
                     f'<yellow>ThreadPoolExecutor workers not enough {len(cls.futures)}</yellow>, {cls.workers}.')
 
             for future in as_completed(futures):
                 futures.remove(future)
                 worker_exception = future.exception()
                 cls.futures.remove(future) if future in cls.futures else cls.futures
                 if worker_exception:
-                    loguercor.error(f"<red>[PrSpider Exception] %s<red>" % worker_exception)
+                    loguercor.error(f"<red>[PrSpider Exception] %s</red>" % worker_exception)
 
     @classmethod
     def fetch(
             self,
             url,
             callback,
             headers=None,
@@ -198,15 +198,15 @@
             meta=None,
             encoding="utf-8",
             retry_interval=1,
             timeout=30,
             **kwargs,
     ):
         settions.request_num += 1
-        response = prequest(loguer).get(
+        response = prequest().get(
             url,
             headers=headers,
             retry_time=retry_time,
             method=method,
             meta=meta,
             encoding=encoding,
             retry_interval=retry_interval,
@@ -277,8 +277,7 @@
             self.retry_num,
             self.process_timestamp(self.start_time),
             self.process_timestamp(end_time),
             spend_time,
             average_time,
         )
         loguer.opt(colors=True).info(m)
-        self.executor.shutdown(wait=True)
```

### Comparing `PrSpiders-0.5.2.3/PrSpider/log.py` & `PrSpiders-0.5.2.4/PrSpider/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,27 +15,28 @@
             "success": 'SUCCESS',
         }
         self.level_stdout = {
             "critical": ['Start', 'Print', 'CRITICAL'],
             "error": ['Start', 'Print', 'ERROR', 'CRITICAL', ],
             "success": ['Start', 'Print', 'Crawl', 'CRITICAL', ],
             "warn": ['Start', 'Print', 'SUCCESS', 'WARNING', 'ERROR', 'CRITICAL'],
-            "info": ['Start', 'Print', 'SUCCESS', 'Crawl', 'INFO', 'WARNING', 'ERROR', 'CRITICAL'],
-            "debug": ['Start', 'Print', 'SUCCESS', 'Crawl', 'DEBUG', 'INFO', 'WARNING', 'ERROR', 'CRITICAL'],
+            "info": ['Close', 'Start', 'Print', 'SUCCESS', 'Crawl', 'INFO', 'WARNING', 'ERROR', 'CRITICAL'],
+            "debug": ['Close', 'Start', 'Print', 'SUCCESS', 'Crawl', 'DEBUG', 'INFO', 'WARNING', 'ERROR', 'CRITICAL'],
         }
         self.log_stdout, self.log_level, self.log_file = log_stdout, log_level, log_file
         loguer.level("DEBUG", color="<green>")
         loguer.level("INFO", color="<cyan>")
         loguer.level("SUCCESS", color="<light-green>")
         loguer.level("WARNING", color="<yellow>")
         loguer.level("ERROR", color="<red>")
         loguer.level("CRITICAL", color="<red>")
         loguer.level("Print", no=30, color="<green>")
         loguer.level("Crawl", no=40, color="<green>")
         loguer.level("Start", no=50, color="<yellow>")
+        loguer.level("Close", no=50, color="<yellow>")
 
     def loggering(self):
         levels = self.level_dict.get(self.log_level.lower())
         slevel = self.level_stdout.get(self.log_level.lower())
         format = "<b><green>{time:YYYY-MM-DD HH:mm:ss.SSS}</green></b><b><level> | {level: ^8} | </level></b><b><i>{message}</i></b>"
         stdout_handler = {
             "sink": sys.stdout,
```

### Comparing `PrSpiders-0.5.2.3/PrSpider/pxpath.py` & `PrSpiders-0.5.2.4/PrSpider/pxpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.3/PrSpider/pyconn.py` & `PrSpiders-0.5.2.4/PrSpider/pyconn.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.3/PrSpider/requestXpath.py` & `PrSpiders-0.5.2.4/PrSpider/requestXpath.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import requests
 import time
 import json
 from requests.models import Response
 from .useragent import get_ua
 from .pxpath import Xpath
-
+from .log import loguercor
 """
 -------------------------------------------------
    File Name:     prequest
    Description :   Network Requests Class
    Author :        penr
    date:          2023/02/16
 -------------------------------------------------
@@ -16,17 +16,16 @@
                    2023/02/16:
 -------------------------------------------------
 """
 __author__ = "penr"
 
 
 class prequest(Xpath):
-    def __init__(self, log):
+    def __init__(self):
         self.response = Response()
-        self.log = log
         self.retry_num = 0
         self.start_time = time.time()
 
     @property
     def user_agent(self):
         """
         :return: an User-Agent at random
@@ -84,31 +83,31 @@
                     *args,
                     **kwargs,
                 )
                 self.response.encoding = encoding
                 if self.response.ok:
                     return self
                 else:
-                    raise Exception(f"Requests False %s" % self.code)
+                    raise Exception(f"Crawl False %s" % self.code)
 
             except Exception as e:
                 retry_time -= 1
                 self.retry_num += 1
                 if retry_time < 0 or settion.retry is False:
-                    self.log.error("\033[31m[Retry Fasle] %s %s %s\033[0m" % (self.method, url, e))
+                    loguercor.error("<yellow>[Crawl Fasle] %s %s %s</yellow>" % (self.method, url, e))
                     self.response.status_code = (
                         410
                         if not self.response.status_code
                         else self.response.status_code
                     )
                     self.meta_["retry_num"] = self.retry_num
                     return self
                 else:
-                    self.log.info(
-                        "\033[31m[Retry] %s %s %s %ss\033[0m"
+                    loguercor.info(
+                        "<red>[Retry] %s %s %s %ss</red>"
                         % (url, self.method, e, retry_interval)
                     )
 
                 time.sleep(retry_interval)
 
     @property
     def text(self):
```

### Comparing `PrSpiders-0.5.2.3/PrSpider/useragent.py` & `PrSpiders-0.5.2.4/PrSpider/useragent.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.3/PrSpiders.egg-info/PKG-INFO` & `PrSpiders-0.5.2.4/PrSpiders.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrSpiders
-Version: 0.5.2.3
+Version: 0.5.2.4
 Summary: Inherit the requests module, add xpath functionality to expand the API, and handle request failures and retries
 Home-page: https://github.com/peng0928/prequests
 Author: penr
 Author-email: 1944542244@qq.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `PrSpiders-0.5.2.3/PrSpiders.egg-info/SOURCES.txt` & `PrSpiders-0.5.2.4/PrSpiders.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.3/README.md` & `PrSpiders-0.5.2.4/README.md`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.3/pkg/prspider/PrSpider_CMD.py` & `PrSpiders-0.5.2.4/pkg/prspider/PrSpider_CMD.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.3/pkg/prspider/start.py` & `PrSpiders-0.5.2.4/pkg/prspider/start.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.3/requestXpath/__init__.py` & `PrSpiders-0.5.2.4/requestXpath/__init__.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.3/requestXpath/pxpath.py` & `PrSpiders-0.5.2.4/requestXpath/pxpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.3/requestXpath/requestXpath.py` & `PrSpiders-0.5.2.4/requestXpath/requestXpath.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,39 @@
-from requests.exceptions import SSLError
-import requests
-import logging
 import time
 import json
+import sys
+import datetime
+import requests
+from requests.exceptions import SSLError
 from requests.models import Response
 from .useragent import get_ua
 from .pxpath import Xpath
-import datetime
-
 """
 -------------------------------------------------
    File Name:     prequest
    Description :   Network Requests Class
    Author :        penr
    date:          2023/02/16
 -------------------------------------------------
    Change Activity:
                    2023/02/16:
 -------------------------------------------------
 """
 __author__ = 'penr'
 __version__ = 0.1
-logging.basicConfig(format='%(message)s', level=logging.INFO)
 
+from loguru import logger
+
+format = "<b><green>{time:YYYY-MM-DD HH:mm:ss.SSS}</green></b><b><level> | {level: ^8} | </level></b><b><i>{message}</i></b>"
+stdout_handler = {
+    "sink": sys.stdout,
+    "colorize": True,
+    "format": format
+}
+logger.configure(handlers=[stdout_handler])
 
 class prequest(Xpath):
     def __init__(self):
         self.response = Response()
         self.amount = 0
         self.samount = 0
         self.famount = 0
@@ -53,43 +60,43 @@
         :param url: target url
         :param header: headers default:
         :param retry_time: retry time default: 3
         :param retry_interval: retry interval default: 1
         :param timeout: network timeout default: 3
         :return:
         """
-        self.current_time = datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
         header = self.header
+        method = method.upper()
         self.method = method
         self.retry_time = retry_time
         self.retry_interval = retry_interval
         if headers and isinstance(headers, dict):
             header.update(headers)
         while True:
             try:
                 self.amount += 1
                 self.response = requests.request(
                     url=url, headers=header, timeout=timeout, method=method, *args, **kwargs)
                 self.response.encoding = encoding
                 if self.response.status_code == 200:
                     self.samount += 1
-                    logging.info(
-                        f'{self.current_time} [Spider] True [Method] {method} [Num] {self.amount} [Status] {self.response.status_code} [Url]: {self.response.url}')
+                    logger.info(
+                        f'{method} {self.response.status_code} {self.response.url}')
                     return self
                 else:
-                    logging.error(
-                        f'{self.current_time} [Spider] False [Method] {self.method} [Num] {self.amount} [Status] {self.response.status_code} [Url]: {self.response.url}')
+                    logger.error(
+                        f'{method} {self.response.status_code} {self.response.url}')
                     raise Exception(f'Respider {self.retry_interval}s')
             except SSLError as e:
                 self.famount += 1
                 logging.error(e)
                 return self
             except Exception as e:
                 self.famount += 1
-                logging.error(e)
+                logger.error(e)
                 retry_time -= 1
                 if retry_time <= 0:
                     return None
                 time.sleep(retry_interval)
 
     @property
     def text(self):
@@ -132,8 +139,8 @@
         spend_time = self.end_time - self.start_time
         msg = """
 Requests: %s
 Success Requests: %s
 False Requests: %s
 Requests Time: %s
         """ % (self.amount, self.samount, self.famount, spend_time)
-        logging.info(msg)
+        logger.info(msg)
```

### Comparing `PrSpiders-0.5.2.3/requestXpath/useragent.py` & `PrSpiders-0.5.2.4/requestXpath/useragent.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.3/setup.py` & `PrSpiders-0.5.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!python
 # -*- coding:utf-8 -*-
 from __future__ import print_function
 from setuptools import setup, find_packages
 
-__version__ = "0.5.2.3"
+__version__ = "0.5.2.4"
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="PrSpiders",
     version=__version__,
```

