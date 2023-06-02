# Comparing `tmp/huhangkai-1.1.6.tar.gz` & `tmp/huhangkai-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huhangkai-1.1.6.tar", last modified: Thu May 25 08:35:35 2023, max compression
+gzip compressed data, was "huhangkai-1.1.7.tar", last modified: Fri Jun  2 09:36:54 2023, max compression
```

## Comparing `huhangkai-1.1.6.tar` & `huhangkai-1.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 08:35:35.342184 huhangkai-1.1.6/
--rw-rw-rw-   0        0        0      228 2023-05-25 08:35:35.341192 huhangkai-1.1.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-25 08:35:35.330215 huhangkai-1.1.6/commen/
--rw-rw-rw-   0        0        0      929 2023-01-30 02:59:52.000000 huhangkai-1.1.6/commen/__init__.py
--rw-rw-rw-   0        0        0    32340 2023-05-08 06:03:41.000000 huhangkai-1.1.6/commen/init_project.py
--rw-rw-rw-   0        0        0     4508 2023-05-08 06:03:41.000000 huhangkai-1.1.6/commen/unit_dict.py
--rw-rw-rw-   0        0        0     3821 2023-05-25 08:05:21.000000 huhangkai-1.1.6/commen/unit_encryption.py
--rw-rw-rw-   0        0        0    20401 2023-05-08 07:11:26.000000 huhangkai-1.1.6/commen/unit_fun.py
--rw-rw-rw-   0        0        0     1242 2023-05-08 06:03:41.000000 huhangkai-1.1.6/commen/unit_logger.py
--rw-rw-rw-   0        0        0     6122 2023-05-08 06:03:41.000000 huhangkai-1.1.6/commen/unit_request.py
--rw-rw-rw-   0        0        0     2461 2023-05-16 11:14:52.000000 huhangkai-1.1.6/commen/unit_tasks.py
-drwxrwxrwx   0        0        0        0 2023-05-25 08:35:35.339192 huhangkai-1.1.6/huhangkai.egg-info/
--rw-rw-rw-   0        0        0      228 2023-05-25 08:35:35.000000 huhangkai-1.1.6/huhangkai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      345 2023-05-25 08:35:35.000000 huhangkai-1.1.6/huhangkai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 08:35:35.000000 huhangkai-1.1.6/huhangkai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-25 08:35:35.000000 huhangkai-1.1.6/huhangkai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-25 08:35:35.000000 huhangkai-1.1.6/huhangkai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 08:35:35.342184 huhangkai-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0      558 2023-05-25 08:35:14.000000 huhangkai-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 09:36:54.794816 huhangkai-1.1.7/
+-rw-rw-rw-   0        0        0      228 2023-06-02 09:36:54.794816 huhangkai-1.1.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-02 09:36:54.783844 huhangkai-1.1.7/commen/
+-rw-rw-rw-   0        0        0      929 2023-01-30 02:59:52.000000 huhangkai-1.1.7/commen/__init__.py
+-rw-rw-rw-   0        0        0    31571 2023-06-02 07:34:45.000000 huhangkai-1.1.7/commen/init_project.py
+-rw-rw-rw-   0        0        0     4508 2023-05-25 08:37:49.000000 huhangkai-1.1.7/commen/unit_dict.py
+-rw-rw-rw-   0        0        0     3843 2023-05-25 08:46:34.000000 huhangkai-1.1.7/commen/unit_encryption.py
+-rw-rw-rw-   0        0        0    20401 2023-05-25 08:37:49.000000 huhangkai-1.1.7/commen/unit_fun.py
+-rw-rw-rw-   0        0        0     1242 2023-05-25 08:37:49.000000 huhangkai-1.1.7/commen/unit_logger.py
+-rw-rw-rw-   0        0        0     9067 2023-06-02 07:33:37.000000 huhangkai-1.1.7/commen/unit_request.py
+-rw-rw-rw-   0        0        0     2461 2023-05-25 08:37:49.000000 huhangkai-1.1.7/commen/unit_tasks.py
+drwxrwxrwx   0        0        0        0 2023-06-02 09:36:54.792820 huhangkai-1.1.7/huhangkai.egg-info/
+-rw-rw-rw-   0        0        0      228 2023-06-02 09:36:54.000000 huhangkai-1.1.7/huhangkai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      345 2023-06-02 09:36:54.000000 huhangkai-1.1.7/huhangkai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 09:36:54.000000 huhangkai-1.1.7/huhangkai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-02 09:36:54.000000 huhangkai-1.1.7/huhangkai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-02 09:36:54.000000 huhangkai-1.1.7/huhangkai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 09:36:54.795812 huhangkai-1.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      558 2023-06-02 09:36:44.000000 huhangkai-1.1.7/setup.py
```

### Comparing `huhangkai-1.1.6/commen/__init__.py` & `huhangkai-1.1.7/commen/__init__.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.6/commen/init_project.py` & `huhangkai-1.1.7/commen/init_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,30 +174,22 @@
         if not os.path.exists(os.path.join(self.service_dir, "__init__.py")):
             self.write_file(os.path.join(self.service_dir, "__init__.py"), value=self.get_init_value())
         self.testcase_dir = os.path.join(testcase_path, self.name)
 
     def get_init_value(self):
         """生成项目__init__.py文件"""
         value = 'from commen.init_project import GetApi\n' \
-                'from commen.unit_request import unit_http_requester, get_variable\n\n\n' \
-                'SERVICE_NAME = "%s"\nZEST_ENV = "SIT"\nAPP_KEY = "%s"\n' \
-                '# 环境变量\nvariable = get_variable(APP_KEY, ZEST_ENV)\n' \
-                '# 接口超时时间（毫秒）\n\nTIMEOUT = 30000\n\n\n' \
-                '# 默认headers\ndef init_headers(**kwargs):\n' \
-                '    headers = {"Content-Type": "application/json"}\n' \
-                '    host = variable.get(kwargs.get("_host", "HOST"))\n    if host:\n' \
-                '        headers.update({"referer": host})\n' \
-                '    token = variable.get(kwargs.get("_token", "TOKEN"))\n' \
-                '    if token:\n        headers.update({"authorization": token})\n    return headers\n\n\n' \
-                'def http_requester(*args, **kwargs):\n    host = variable.get(kwargs.get("_host", "HOST"))\n' \
-                '    return unit_http_requester(*args, host=host, timeout=TIMEOUT,' \
-                ' init_headers=init_headers(**kwargs), **kwargs)\n\n\n' \
-                'if __name__ == "__main__":\n' % (self.name, self.app_key)
+                'from commen.unit_request import UnitRequest\n\n\n' \
+                'class Request(UnitRequest):\n    pass\n\n\n' \
+                'unit_request = UnitRequest("SIT", "%s")\n' \
+                '# 环境变量\nvariable = unit_request.variable\n' \
+                'http_requester = unit_request.http_requester\n\n\n' \
+                'if __name__ == "__main__":\n' % (self.app_key)
         if self.app_key:
-            value += "    GetApi(app_key='%s')\n" % (self.app_key,)
+            value += "    GetApi(app_key=APP_KEY)\n"
         else:
             value += "    GetApi("
             value += "api_type=%s, " % self.api_type if self.api_type else ""
             value += "value='%s', " % self.value if self.value else ""
             value += "name='%s', " % self.name if self.name else ""
             value += "yapi_url='%s', " % self.yapi_url if self.yapi_url else ""
             value = value[:-2] + ")"
```

### Comparing `huhangkai-1.1.6/commen/unit_dict.py` & `huhangkai-1.1.7/commen/unit_dict.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.6/commen/unit_encryption.py` & `huhangkai-1.1.7/commen/unit_encryption.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         b = x.read()
         return b
 
 
 # ------------------------加密------------------------
 def rsa_encryption(text: str, public_key: bytes):
     # 字符串指定编码（转为bytes）
-    text = text.encode('utf-8')
+    text = text.replace('\r\n', '\n').encode('utf-8')
     key = RSA.importKey(public_key)
     # 构建公钥对象
     cipher_public = PKCS1_v1_5.new(key)
     # 加密（bytes）
     text_encrypted = cipher_public.encrypt(text)
     # base64编码，并转为字符串
     text_encrypted_base64 = base64.b64encode(text_encrypted).decode()
```

### Comparing `huhangkai-1.1.6/commen/unit_fun.py` & `huhangkai-1.1.7/commen/unit_fun.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.6/commen/unit_logger.py` & `huhangkai-1.1.7/commen/unit_logger.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.6/commen/unit_request.py` & `huhangkai-1.1.7/commen/unit_request.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,129 +11,181 @@
 from urllib.parse import urlencode
 from commen.unit_dict import Dict
 from commen.unit_logger import logger
 from openpyxl.reader.excel import load_workbook
 from commen import admin_host, projects_path, files_path
 
 
-def get_url(url, kwargs):
-    tmp = re.findall(r'\{.+}', url)
-    if not tmp:
-        return url
-    if kwargs.get(tmp[0][1:-1]):
-        url = url.replace(tmp[0], kwargs.get(tmp[0][1:-1]))
-        url = url.split('{')[0]
-        return url
-    else:
-        assert False, "字段：" +tmp[0][1:-1] + "，为必填字段"
-
-
-def unit_http_requester(method, url, params=None, data=None, headers=None, host=None, timeout=10000, init_headers={},
-                        _route="", _files=None, **kwargs):
-    if headers.get("headers"):
-        _headers = init_headers
-        tmp = headers.pop("headers")
-        _headers.update(headers)
-        if isinstance(tmp, dict):
-            _headers.update(tmp)
-    else:
-        headers.pop("headers")
-        _headers = headers
-
-    if url[0] == '/' and host:
-        if _route and _route[0] != '/':
-            _route = '/' + _route
-        url = host + _route + url
-    if method.upper() == "GET":
-        params = params or data
-    logger.info("接口请求参数method: %s, url: %s" % (method, url))
-    logger.info("接口请求参数headers: %s" % str(_headers))
-    logger.info("接口请求参数params: %s" % str(params)) if params else logger.info("接口请求参数data: %s" % str(data))
-    if "//" not in url:
-        assert False, "url没有域名"
-    time_s = time.time()
-    try:
-        if "application/x-www-form-urlencoded" in str(_headers):
-            data = urlencode(data)
-        if "multipart/form-data" in str(_headers) and "file" in data.keys():
-            file = str(data.pop("file"))
-            if not os.path.isfile(file):
+class UnitRequest:
+    def __init__(self, ZEST_ENV=None, APP_KEY=None, TIMEOUT=30000):
+        self.ZEST_ENV = ZEST_ENV
+        self.APP_KEY = APP_KEY
+        self.TIMEOUT = TIMEOUT
+        self.variable = self.get_variable()
+        
+    
+    @staticmethod
+    def get_url(url, kwargs):
+        tmp = re.findall(r'\{.+}', url)
+        if not tmp:
+            return url
+        if kwargs.get(tmp[0][1:-1]):
+            url = url.replace(tmp[0], kwargs.get(tmp[0][1:-1]))
+            url = url.split('{')[0]
+            return url
+        else:
+            assert False, "字段：" + tmp[0][1:-1] + "，为必填字段"
+    
+    @staticmethod
+    def unit_http_requester(method, url, params=None, data=None, headers=None, host=None, timeout=10000,
+                            init_headers={},
+                            _route="", _files=None, **kwargs):
+        if headers.get("headers"):
+            _headers = init_headers
+            tmp = headers.pop("headers")
+            _headers.update(headers)
+            if isinstance(tmp, dict):
+                _headers.update(tmp)
+        else:
+            headers.pop("headers")
+            _headers = headers
+
+        if url[0] == '/' and host:
+            if _route and _route[0] != '/':
+                _route = '/' + _route
+            url = host + _route + url
+        if method.upper() == "GET":
+            params = params or data
+        logger.info("接口请求参数method: %s, url: %s" % (method, url))
+        logger.info("接口请求参数headers: %s" % str(_headers))
+        logger.info("接口请求参数params: %s" % str(params)) if params else logger.info(
+            "接口请求参数data: %s" % str(data))
+        if "//" not in url:
+            assert False, "url没有域名"
+        time_s = time.time()
+        try:
+            if "application/x-www-form-urlencoded" in str(_headers):
+                data = urlencode(data)
+                res = requests.request(method, url, data=data, headers=_headers, timeout=timeout / 1000,
+                                       verify=False)
+            elif "multipart/form-data" in str(_headers) and "file" in data.keys():
+                file = str(data.pop("file"))
+                if not os.path.isfile(file):
+                    try:
+                        out = requests.get(admin_host + '/files/file/', params={"value": file})
+                        if "filename=" in str(out.raw.headers):
+                            file_name = urllib.parse.unquote(re.findall(r'filename=(.+?)\'', str(out.raw.headers))[0])
+                            file = os.path.join(files_path, file_name)
+                            with open(file, 'wb') as f:
+                                f.write(out.content)
+                    except:
+                        pass
+                    if os.path.isfile(file):
+                        pass
+                    elif os.path.isfile(os.path.join(files_path, file)):
+                        file = os.path.join(files_path, file)
+                    elif os.path.isfile(os.path.join(projects_path, file)):
+                        file = os.path.join(projects_path, file)
+                    else:
+                        assert False, "对应的文件不存在"
+                data.update({'md5': hashlib.md5('%d_%d'.encode() % (0, int(time.time()))).hexdigest(),
+                             'filesize': len(open(file, 'rb').read()), })
+                _files = {"file": (os.path.basename(file), open(file, 'rb'))} if file else {}
                 try:
-                    out = requests.get(admin_host + '/files/file/', params={"value": file})
-                    if "filename=" in str(out.raw.headers):
-                        file_name = urllib.parse.unquote(re.findall(r'filename=(.+?)\'', str(out.raw.headers))[0])
-                        file = os.path.join(files_path, file_name)
-                        with open(file, 'wb') as f:
-                            f.write(out.content)
+                    del _headers['Content-Type']
                 except:
                     pass
-                if os.path.isfile(file):
-                    pass
-                elif os.path.isfile(os.path.join(files_path, file)):
-                    file = os.path.join(files_path, file)
-                elif os.path.isfile(os.path.join(projects_path, file)):
-                    file = os.path.join(projects_path, file)
+                if kwargs.get('cookies'):
+                    res = requests.request(method, url, params=params, data=data, files=_files,
+                                           headers=_headers, timeout=timeout / 1000, verify=False,
+                                           cookies=kwargs.get('cookies'))
                 else:
-                    assert False, "对应的文件不存在"
-            data.update({'md5': hashlib.md5('%d_%d'.encode() % (0, int(time.time()))).hexdigest(),
-                         'filesize': len(open(file, 'rb').read()),})
-            _files = {"file": (os.path.basename(file), open(file, 'rb'))} if file else {}
+                    res = requests.request(method, url, params=params, data=data, files=_files,
+                                           headers=_headers, timeout=timeout / 1000, verify=False)
+            else:
+                if kwargs.get('cookies'):
+                    res = requests.request(method, url, params=params, json=data, headers=_headers,
+                                           timeout=timeout / 1000,
+                                           verify=False, cookies=kwargs.get('cookies'))
+                else:
+                    res = requests.request(method, url, params=params, json=data, headers=_headers,
+                                           timeout=timeout / 1000,
+                                           verify=False)
+
+            logger.info("接口响应时间: %.3f毫秒" % (time.time() - time_s))
             try:
-                del _headers['Content-Type']
+                res.rsp = Dict(json.loads(res.text)) if res.text else Dict(
+                    {"code": -1, "msg": "该接口返回的数据为空字符串"})
             except:
-                pass
-            res = requests.request(method, url, params=params, data=data, files=_files,
-                                   headers=_headers, timeout=timeout / 1000, verify=False)
-        else:
-            res = requests.request(method, url, params=params, json=data, headers=_headers, timeout=timeout / 1000, verify=False)
-
-        logger.info("接口响应时间: %.3f毫秒" % (time.time() - time_s))
-        try:
-            res.rsp = Dict(json.loads(res.text)) if res.text else Dict({"code": -1, "msg": "该接口返回的数据为空字符串"})
-        except:
-            if "filename=" in str(res.raw.headers):
-                file_name = urllib.parse.unquote(re.findall(r'filename=(.+?)\'', str(res.raw.headers))[0])
-                if "xlsx" in file_name:
-                    file_path = os.path.join(files_path, file_name)
-                    with open(file_path, 'wb') as f:
-                        f.write(res.content)
-                    wb = load_workbook(file_path)
-                    ws = wb.active
-                    rows = [[cell.value for cell in row] for row in ws]
-                    try:
-                        data = [{c1: c2 for c1, c2 in zip(rows[0], row)} for row in rows[1:]]
-                    except:
-                        data = []
-                    os.remove(file_path)
-                    res.rsp = Dict({"code": 0, "data": data, "filename": file_name, "rows": rows})
+                if "filename=" in str(res.raw.headers):
+                    file_name = urllib.parse.unquote(re.findall(r'filename=(.+?)\'', str(res.raw.headers))[0])
+                    if "xlsx" in file_name:
+                        file_path = os.path.join(files_path, file_name)
+                        with open(file_path, 'wb') as f:
+                            f.write(res.content)
+                        wb = load_workbook(file_path)
+                        ws = wb.active
+                        rows = [[cell.value for cell in row] for row in ws]
+                        try:
+                            data = [{c1: c2 for c1, c2 in zip(rows[0], row)} for row in rows[1:]]
+                        except:
+                            data = []
+                        os.remove(file_path)
+                        res.rsp = Dict({"code": 0, "data": data, "filename": file_name, "rows": rows})
+                    else:
+                        res.rsp = res.text
                 else:
                     res.rsp = res.text
-            else:
-                res.rsp = res.text
-        logger.info("接口返回http_code: %s" % res.status_code)
-        logger.info("接口数据res: %s" % str(res.rsp))
-        return res
-    except ReadTimeout:
-        assert False, "接口响应时间%.3f秒, 超过设置的时间%.3f秒" % (time.time() - time_s, timeout / 1000)
-    except ConnectTimeout:
-        assert False, "接口响应时间%.3f秒, 超过设置的时间%.3f秒" % (time.time() - time_s, timeout / 1000)
-    except MissingSchema:
-        assert False, "url不对，无域名"
-    except Exception as e:
-        print(e)
-        assert False, "调用接口报错"
-
-
-def get_variable(app_key, env):
-    project = requests.post(admin_host + '/variable/variable/',
-                            json={"app_key": app_key, "environment": env}).json()
-    _variable = {}
-    print(admin_host)
-    print(project)
-    for v in project.get('variables', []):
-        if v.get('type') == 0:
-            _variable[v.get('name')] = v.get('value')
-        elif v.get('type') == 1:
-            _variable[v.get('name')] = json.loads(v.get('value'))
-        elif v.get('type') == 2:
-            _variable[v.get('name')] = int(json.loads(v.get('value')))
-    return _variable
+            logger.info("接口返回http_code: %s" % res.status_code)
+            logger.info("接口数据res: %s" % str(res.rsp))
+            return res
+        except ReadTimeout:
+            assert False, "接口响应时间%.3f秒, 超过设置的时间%.3f秒" % (time.time() - time_s, timeout / 1000)
+        except ConnectTimeout:
+            assert False, "接口响应时间%.3f秒, 超过设置的时间%.3f秒" % (time.time() - time_s, timeout / 1000)
+        except MissingSchema:
+            assert False, "url不对，无域名"
+        except Exception as e:
+            print(e)
+            assert False, "调用接口报错"
+
+    def get_variable(self, app_key=None, env=None):
+        app_key = app_key or self.APP_KEY
+        env = env or self.ZEST_ENV
+        project = requests.post(admin_host + '/variable/variable/',
+                                json={"app_key": app_key, "environment": env}).json()
+        _variable = {}
+        for v in project.get('variables', []):
+            if v.get('type') == 0:
+                _variable[v.get('name')] = v.get('value')
+            elif v.get('type') == 1:
+                _variable[v.get('name')] = json.loads(v.get('value'))
+            elif v.get('type') == 2:
+                _variable[v.get('name')] = int(json.loads(v.get('value')))
+        _variable["_token"] = project.get("token")
+        return _variable
+
+    def init_headers(self, **kwargs):
+        headers = {"Content-Type": "application/json"}
+        _host = kwargs.get("_host", "HOST")
+        host = self.variable.get(_host) if "//" not in _host else _host
+        if host:
+            headers.update({"referer": host})
+        _token = kwargs.get("_token", "TOKEN")
+        token = self.variable.get(_token) if len(_token) < 20 else _token
+        if not token and self.variable.get("_token"):
+            token = self.variable.get("_token").get(_token)
+            if not token:
+                token = self.variable.get("_token").get("token")
+        if token:
+            headers.update({"authorization": token})
+        return headers
+    
+    def http_requester(self, *args, **kwargs):
+        _host = kwargs.get("_host", "HOST")
+        host = self.variable.get(_host) if "//" not in _host else _host
+        return self.unit_http_requester(*args, host=host, timeout=self.TIMEOUT, init_headers=self.init_headers(**kwargs), **kwargs)
+
+
+get_url = UnitRequest.get_url
+unit_http_requester = UnitRequest.unit_http_requester
+
```

### Comparing `huhangkai-1.1.6/commen/unit_tasks.py` & `huhangkai-1.1.7/commen/unit_tasks.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.6/setup.py` & `huhangkai-1.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='huhangkai',  # 对外模块的名字
-    version='1.1.6',  # 版本号
+    version='1.1.7',  # 版本号
     description='接口自动化',  # 描述
     author='胡杭凯',  # 作者
     author_email='3173825608@qq.com',
     # package_dir={"": "commen"},
     packages=find_packages(),
     package_data={'by': ['常用命令.bat'],},
     python_requires=">=3.0",
```

