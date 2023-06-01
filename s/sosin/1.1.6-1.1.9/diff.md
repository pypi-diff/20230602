# Comparing `tmp/sosin-1.1.6.tar.gz` & `tmp/sosin-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sosin-1.1.6.tar", last modified: Sun May 21 13:59:45 2023, max compression
+gzip compressed data, was "sosin-1.1.9.tar", last modified: Thu Jun  1 22:28:10 2023, max compression
```

## Comparing `sosin-1.1.6.tar` & `sosin-1.1.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 13:59:45.245981 sosin-1.1.6/
--rw-rw-rw-   0        0        0     1083 2023-04-17 11:46:46.000000 sosin-1.1.6/LICENSE
--rw-rw-rw-   0        0        0     1268 2023-05-21 13:59:45.244981 sosin-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      863 2023-04-17 11:46:46.000000 sosin-1.1.6/README.md
--rw-rw-rw-   0        0        0       42 2023-05-21 13:59:45.245981 sosin-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0      984 2023-05-21 13:58:42.000000 sosin-1.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-21 13:59:45.191923 sosin-1.1.6/sosin/
--rw-rw-rw-   0        0        0      302 2023-05-21 13:58:51.000000 sosin-1.1.6/sosin/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-21 13:59:45.229620 sosin-1.1.6/sosin/databases/
--rw-rw-rw-   0        0        0     4934 2023-04-24 10:38:48.000000 sosin-1.1.6/sosin/databases/fs.py
--rw-rw-rw-   0        0        0    13108 2023-05-21 13:58:00.000000 sosin-1.1.6/sosin/databases/rdb.py
-drwxrwxrwx   0        0        0        0 2023-05-21 13:59:45.232622 sosin-1.1.6/sosin/rpa/
--rw-rw-rw-   0        0        0    11055 2023-05-15 08:13:19.000000 sosin-1.1.6/sosin/rpa/email_mgr.py
--rw-rw-rw-   0        0        0     3698 2023-05-10 06:56:55.000000 sosin-1.1.6/sosin/rpa/sms_mgr.py
-drwxrwxrwx   0        0        0        0 2023-05-21 13:59:45.238621 sosin-1.1.6/sosin/utils/
--rw-rw-rw-   0        0        0     1797 2023-05-14 01:57:45.000000 sosin-1.1.6/sosin/utils/currency.py
--rw-rw-rw-   0        0        0      304 2023-04-17 11:46:46.000000 sosin-1.1.6/sosin/utils/log.py
--rw-rw-rw-   0        0        0      527 2023-04-17 11:46:46.000000 sosin-1.1.6/sosin/utils/progress.py
--rw-rw-rw-   0        0        0      385 2023-04-17 11:46:46.000000 sosin-1.1.6/sosin/utils/secret.py
--rw-rw-rw-   0        0        0      885 2023-05-10 06:56:55.000000 sosin-1.1.6/sosin/utils/zip.py
-drwxrwxrwx   0        0        0        0 2023-05-21 13:59:45.243974 sosin-1.1.6/sosin/web/
--rw-rw-rw-   0        0        0     1055 2023-04-18 14:49:45.000000 sosin-1.1.6/sosin/web/content.py
--rw-rw-rw-   0        0        0     5506 2023-05-14 01:57:26.000000 sosin-1.1.6/sosin/web/session.py
--rw-rw-rw-   0        0        0     1051 2023-05-14 01:57:45.000000 sosin-1.1.6/sosin/web/translate.py
--rw-rw-rw-   0        0        0     4394 2023-05-14 01:57:45.000000 sosin-1.1.6/sosin/web/virtual.py
-drwxrwxrwx   0        0        0        0 2023-05-21 13:59:45.214621 sosin-1.1.6/sosin.egg-info/
--rw-rw-rw-   0        0        0     1268 2023-05-21 13:59:44.000000 sosin-1.1.6/sosin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      471 2023-05-21 13:59:45.000000 sosin-1.1.6/sosin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 13:59:44.000000 sosin-1.1.6/sosin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-05-21 13:59:44.000000 sosin-1.1.6/sosin.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-21 13:59:44.000000 sosin-1.1.6/sosin.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 22:28:10.661978 sosin-1.1.9/
+-rw-rw-rw-   0        0        0     1083 2023-04-17 11:46:46.000000 sosin-1.1.9/LICENSE
+-rw-rw-rw-   0        0        0     1268 2023-06-01 22:28:10.660977 sosin-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      863 2023-04-17 11:46:46.000000 sosin-1.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-01 22:28:10.661978 sosin-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      984 2023-06-01 22:27:08.000000 sosin-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 22:28:10.615369 sosin-1.1.9/sosin/
+-rw-rw-rw-   0        0        0      302 2023-06-01 22:27:31.000000 sosin-1.1.9/sosin/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 22:28:10.644970 sosin-1.1.9/sosin/databases/
+-rw-rw-rw-   0        0        0     4934 2023-04-24 10:38:48.000000 sosin-1.1.9/sosin/databases/fs.py
+-rw-rw-rw-   0        0        0    13108 2023-05-22 10:51:13.000000 sosin-1.1.9/sosin/databases/rdb.py
+drwxrwxrwx   0        0        0        0 2023-06-01 22:28:10.647977 sosin-1.1.9/sosin/rpa/
+-rw-rw-rw-   0        0        0    11993 2023-05-22 12:23:47.000000 sosin-1.1.9/sosin/rpa/email_mgr.py
+-rw-rw-rw-   0        0        0     3698 2023-05-10 06:56:55.000000 sosin-1.1.9/sosin/rpa/sms_mgr.py
+drwxrwxrwx   0        0        0        0 2023-06-01 22:28:10.652976 sosin-1.1.9/sosin/utils/
+-rw-rw-rw-   0        0        0     1797 2023-05-14 01:57:45.000000 sosin-1.1.9/sosin/utils/currency.py
+-rw-rw-rw-   0        0        0      304 2023-04-17 11:46:46.000000 sosin-1.1.9/sosin/utils/log.py
+-rw-rw-rw-   0        0        0      527 2023-04-17 11:46:46.000000 sosin-1.1.9/sosin/utils/progress.py
+-rw-rw-rw-   0        0        0      385 2023-04-17 11:46:46.000000 sosin-1.1.9/sosin/utils/secret.py
+-rw-rw-rw-   0        0        0      885 2023-05-10 06:56:55.000000 sosin-1.1.9/sosin/utils/zip.py
+drwxrwxrwx   0        0        0        0 2023-06-01 22:28:10.658978 sosin-1.1.9/sosin/web/
+-rw-rw-rw-   0        0        0     1055 2023-04-18 14:49:45.000000 sosin-1.1.9/sosin/web/content.py
+-rw-rw-rw-   0        0        0     6086 2023-05-24 13:44:32.000000 sosin-1.1.9/sosin/web/session.py
+-rw-rw-rw-   0        0        0     1051 2023-05-14 01:57:45.000000 sosin-1.1.9/sosin/web/translate.py
+-rw-rw-rw-   0        0        0     4423 2023-06-01 22:11:36.000000 sosin-1.1.9/sosin/web/virtual.py
+drwxrwxrwx   0        0        0        0 2023-06-01 22:28:10.642828 sosin-1.1.9/sosin.egg-info/
+-rw-rw-rw-   0        0        0     1268 2023-06-01 22:28:10.000000 sosin-1.1.9/sosin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      471 2023-06-01 22:28:10.000000 sosin-1.1.9/sosin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 22:28:10.000000 sosin-1.1.9/sosin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-01 22:28:10.000000 sosin-1.1.9/sosin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-01 22:28:10.000000 sosin-1.1.9/sosin.egg-info/top_level.txt
```

### Comparing `sosin-1.1.6/LICENSE` & `sosin-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sosin-1.1.6/PKG-INFO` & `sosin-1.1.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sosin
-Version: 1.1.6
+Version: 1.1.9
 Summary: Python utils for general works
 Home-page: https://github.com/devsosin/sosin
 Author: Jason Choi
 Author-email: svstar94@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sosin-1.1.6/README.md` & `sosin-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `sosin-1.1.6/setup.py` & `sosin-1.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name                                = "sosin",
-    version                             = "1.1.6",
+    version                             = "1.1.9",
     license                             = 'MIT',
     author                              = "Jason Choi",
     author_email                        = "svstar94@gmail.com",
     description                         = "Python utils for general works",
     long_description                    = open('README.md').read(),
     url                                 = "https://github.com/devsosin/sosin",
     install_requires                    = ['requests', 'requests-toolbelt'],
```

### Comparing `sosin-1.1.6/sosin/databases/fs.py` & `sosin-1.1.9/sosin/databases/fs.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.6/sosin/databases/rdb.py` & `sosin-1.1.9/sosin/databases/rdb.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -145,20 +145,20 @@
         
         example) 
         column_qry = "*"
         column_qry = "id, name, email"
         table = "Students"
         """
         sql_qr = "SELECT {0} FROM {1}".format(column_qry, table)
+        if order_by:
+            sql_qr += ' ORDER BY {}'.format(order_by)
         if limit:
             sql_qr += ' LIMIT {}'.format(limit)
         if offset:
             sql_qr += ' OFFSET {}'.format(offset)
-        if order_by:
-            sql_qr += ' ORDER BY {}'.format(order_by)
         if where_condition:
             for i, (col, eq, val) in enumerate(where_condition):
                 is_equal = '=' if eq else '!='
                 is_multiple = ' AND' if i > 1 else ' WHERE'
                 sql_qr += f'{is_multiple} {col}{is_equal}{val}'
```

### Comparing `sosin-1.1.6/sosin/rpa/email_mgr.py` & `sosin-1.1.9/sosin/rpa/email_mgr.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 
 import time
 from datetime import datetime
 
 import traceback
 from typing import Union
 
+from dataclasses import dataclass
+
 def _is_ascii(s):
     '''
     ASCII 체크
     '''
     return all(ord(c) < 128 for c in s)
 
 def _get_subject(subject):
@@ -37,15 +39,20 @@
     '''
     메일 내용 반환
     '''
     if msg.is_multipart():
         return _get_body(msg.get_payload(0))
     else:
         return msg.get_payload(None, True)
-    
+
+@dataclass
+class EmailAccount:
+    email_id: str
+    email_pw: str
+
 class EmailManager:
     """
     Email Manager
     """
 
     def __init__(self, email_id, email_pw, mail_server:str='naver', mode='send') -> None:
         """
@@ -254,14 +261,15 @@
             return True
 
         except Exception:
             traceback.print_exc()
         
         return False
 
+# deprecated
 def _get_emails(email_id, email_pw, **kwargs):
     """
     kwargs
     mail_server = ['gmail', 'naver']
     header_subjects:list=[], header_since:str=None, header_from:str=None, 
     label:str=None, save_path:str=None, 
 
@@ -269,27 +277,48 @@
     encode_type='utf-8',
     """
     emgr = EmailManager(email_id, email_pw, mail_server=kwargs.pop('mail_server', 'naver'), mode='get')
     emails = emgr.get_email(**kwargs)
     del emgr
     return emails
 
+# deprecated
 def _send_email(email_id, email_pw, **kwargs):
     """
     kwargs
     mail_server = ['gmail', 'naver']
     from_user:str, to_users:list, 
     subject:str, contents:list[Union[tuple, str]],
     attachments:list=[], cc_targets=[]
     """
     emgr = EmailManager(email_id, email_pw, mail_server=kwargs.pop('mail_server', 'naver'))
     result = emgr.send_email(**kwargs)
     del emgr
     return result
 
+class GmailManager(EmailManager):
+    def __init__(self, email_id, email_pw, mode='send') -> None:
+        super().__init__(email_id, email_pw, 'gmail', mode)
+
+class NaverManager(EmailManager):
+    def __init__(self, email_id, email_pw, mode='send') -> None:
+        super().__init__(email_id, email_pw, 'naver', mode)
+
+def send_with_gmail(email_id, email_pw, **kwargs):
+    return GmailManager(email_id, email_pw).send_email(**kwargs)
+
+def send_with_naver(email_id, email_pw, **kwargs):
+    return NaverManager(email_id, email_pw).send_email(**kwargs)
+
+def get_with_gmail(email_id, email_pw, **kwargs):
+    return GmailManager(email_id, email_pw).get_email(**kwargs)
+
+def get_with_naver(email_id, email_pw, **kwargs):
+    return NaverManager(email_id, email_pw).get_email(**kwargs)
+
 if __name__ == '__main__':
     config = {
         'EMAIL_ID': 'your-email-id',
         'EMAIL_PW': 'your-email-pw',
     }
     emgr = EmailManager(config.get('EMAIL_ID'), config.get('EMAIL_PW'), mail_server='gmail')
     emgr.send_email(config['EMAIL_ID'], ['target-user-email'], 'this is test email !',
```

### Comparing `sosin-1.1.6/sosin/rpa/sms_mgr.py` & `sosin-1.1.9/sosin/rpa/sms_mgr.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.6/sosin/utils/currency.py` & `sosin-1.1.9/sosin/utils/currency.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.6/sosin/utils/progress.py` & `sosin-1.1.9/sosin/utils/progress.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.6/sosin/utils/zip.py` & `sosin-1.1.9/sosin/utils/zip.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.6/sosin/web/content.py` & `sosin-1.1.9/sosin/web/content.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.6/sosin/web/session.py` & `sosin-1.1.9/sosin/web/session.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,14 +52,22 @@
                  data:Union[str, dict, list]={}, files:dict[str]={}, **kwargs):
         r = self._request(url, headers=headers, cookies=cookies, data=data, files=files, method='put', **kwargs)
 
         if self._mode:
             self.history.append(r)
         return r
 
+    def patch(self, url:str, headers:dict={}, cookies:dict={}, 
+                 data:Union[str, dict, list]={}, files:dict[str]={}, **kwargs):
+        r = self._request(url, headers=headers, cookies=cookies, data=data, files=files, method='patch', **kwargs)
+
+        if self._mode:
+            self.history.append(r)
+        return r
+
     def _request(self, url:str, headers:dict={}, cookies:dict={}, 
                  data:Union[str, dict]={}, files:dict[str]={}, 
                  method:str='post', no_parsing:bool=False, **kwargs) -> requests.Response:
         """
         request
 
         method = get, post, put
@@ -85,15 +93,18 @@
                               data=data if type(data) in [str, MultipartEncoder] or no_parsing else json.dumps(data), **kwargs)
         elif method.lower() == 'get':
             r = requests.get(url, headers={**self._headers, **type_header, **headers}, 
                              cookies={**self._cookies, **cookies}, **kwargs)
         elif method.lower() == 'put':
             r = requests.put(url, headers={**self._headers, **type_header, **headers}, 
                              cookies={**self._cookies, **cookies}, data=json.dumps(data), **kwargs)
-        
+        elif method.lower() == 'patch':
+            r = requests.patch(url, headers={**self._headers, **type_header, **headers},
+                             cookies={**self._cookies, **cookies}, data=json.dumps(data), **kwargs)
+            
         self._set_cookies(r)
         return r
     
     # ------------------------------------------------------------------------
     # Cookie Management
     def add_cookies(self, cookies:dict) -> None:
         self._cookies.update(cookies)
```

### Comparing `sosin-1.1.6/sosin/web/translate.py` & `sosin-1.1.9/sosin/web/translate.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.6/sosin/web/virtual.py` & `sosin-1.1.9/sosin/web/virtual.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,20 +65,20 @@
         if user_agent:
             self.options.add_argument("user-agent=Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/105.0.0.0 Safari/537.36")
         if lang_kr:
             self.options.add_argument("--lang=ko_KR")
         if secret_mode:
             self.options.add_argument("--incognito")
 
-    def get_driver(self):
+    def get_driver(self, version=None):
         """
         셀레니움 웹드라이버 실행
         """
         if self.engine == 'chrome':
-            driver = webdriver.Chrome(service=Service(ChromeDriverManager().install()), options=self.options)
+            driver = webdriver.Chrome(service=Service(ChromeDriverManager(version=version).install()), options=self.options)
             driver.maximize_window()
             driver.implicitly_wait(5)
             return driver
 
 
 # ---------------------------------------------------------------------------------------------
 # Selenium Utils
```

### Comparing `sosin-1.1.6/sosin.egg-info/PKG-INFO` & `sosin-1.1.9/sosin.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sosin
-Version: 1.1.6
+Version: 1.1.9
 Summary: Python utils for general works
 Home-page: https://github.com/devsosin/sosin
 Author: Jason Choi
 Author-email: svstar94@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

