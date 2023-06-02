# Comparing `tmp/huhangkai-1.1.8.tar.gz` & `tmp/huhangkai-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huhangkai-1.1.8.tar", last modified: Fri Jun  2 09:56:22 2023, max compression
+gzip compressed data, was "huhangkai-1.1.9.tar", last modified: Fri Jun  2 10:03:21 2023, max compression
```

## Comparing `huhangkai-1.1.8.tar` & `huhangkai-1.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 09:56:22.053095 huhangkai-1.1.8/
--rw-rw-rw-   0        0        0      228 2023-06-02 09:56:22.053095 huhangkai-1.1.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-02 09:56:22.041128 huhangkai-1.1.8/commen/
--rw-rw-rw-   0        0        0      929 2023-01-30 02:59:52.000000 huhangkai-1.1.8/commen/__init__.py
--rw-rw-rw-   0        0        0    31571 2023-06-02 07:34:45.000000 huhangkai-1.1.8/commen/init_project.py
--rw-rw-rw-   0        0        0     4508 2023-05-25 08:37:49.000000 huhangkai-1.1.8/commen/unit_dict.py
--rw-rw-rw-   0        0        0     3843 2023-05-25 08:46:34.000000 huhangkai-1.1.8/commen/unit_encryption.py
--rw-rw-rw-   0        0        0    20401 2023-05-25 08:37:49.000000 huhangkai-1.1.8/commen/unit_fun.py
--rw-rw-rw-   0        0        0     1242 2023-05-25 08:37:49.000000 huhangkai-1.1.8/commen/unit_logger.py
--rw-rw-rw-   0        0        0     9108 2023-06-02 09:56:08.000000 huhangkai-1.1.8/commen/unit_request.py
--rw-rw-rw-   0        0        0     2461 2023-05-25 08:37:49.000000 huhangkai-1.1.8/commen/unit_tasks.py
-drwxrwxrwx   0        0        0        0 2023-06-02 09:56:22.051099 huhangkai-1.1.8/huhangkai.egg-info/
--rw-rw-rw-   0        0        0      228 2023-06-02 09:56:21.000000 huhangkai-1.1.8/huhangkai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      345 2023-06-02 09:56:21.000000 huhangkai-1.1.8/huhangkai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 09:56:21.000000 huhangkai-1.1.8/huhangkai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-06-02 09:56:21.000000 huhangkai-1.1.8/huhangkai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-02 09:56:21.000000 huhangkai-1.1.8/huhangkai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 09:56:22.054092 huhangkai-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0      558 2023-06-02 09:56:08.000000 huhangkai-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:03:21.049224 huhangkai-1.1.9/
+-rw-rw-rw-   0        0        0      228 2023-06-02 10:03:21.049224 huhangkai-1.1.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-02 10:03:21.037411 huhangkai-1.1.9/commen/
+-rw-rw-rw-   0        0        0      929 2023-01-30 02:59:52.000000 huhangkai-1.1.9/commen/__init__.py
+-rw-rw-rw-   0        0        0    31571 2023-06-02 07:34:45.000000 huhangkai-1.1.9/commen/init_project.py
+-rw-rw-rw-   0        0        0     4508 2023-05-25 08:37:49.000000 huhangkai-1.1.9/commen/unit_dict.py
+-rw-rw-rw-   0        0        0     3843 2023-05-25 08:46:34.000000 huhangkai-1.1.9/commen/unit_encryption.py
+-rw-rw-rw-   0        0        0    20401 2023-05-25 08:37:49.000000 huhangkai-1.1.9/commen/unit_fun.py
+-rw-rw-rw-   0        0        0     1242 2023-05-25 08:37:49.000000 huhangkai-1.1.9/commen/unit_logger.py
+-rw-rw-rw-   0        0        0     9218 2023-06-02 10:02:56.000000 huhangkai-1.1.9/commen/unit_request.py
+-rw-rw-rw-   0        0        0     2461 2023-05-25 08:37:49.000000 huhangkai-1.1.9/commen/unit_tasks.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:03:21.047235 huhangkai-1.1.9/huhangkai.egg-info/
+-rw-rw-rw-   0        0        0      228 2023-06-02 10:03:20.000000 huhangkai-1.1.9/huhangkai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      345 2023-06-02 10:03:20.000000 huhangkai-1.1.9/huhangkai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 10:03:20.000000 huhangkai-1.1.9/huhangkai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-02 10:03:20.000000 huhangkai-1.1.9/huhangkai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-02 10:03:20.000000 huhangkai-1.1.9/huhangkai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 10:03:21.050220 huhangkai-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      558 2023-06-02 10:03:15.000000 huhangkai-1.1.9/setup.py
```

### Comparing `huhangkai-1.1.8/commen/__init__.py` & `huhangkai-1.1.9/commen/__init__.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.8/commen/init_project.py` & `huhangkai-1.1.9/commen/init_project.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.8/commen/unit_dict.py` & `huhangkai-1.1.9/commen/unit_dict.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.8/commen/unit_encryption.py` & `huhangkai-1.1.9/commen/unit_encryption.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.8/commen/unit_fun.py` & `huhangkai-1.1.9/commen/unit_fun.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.8/commen/unit_logger.py` & `huhangkai-1.1.9/commen/unit_logger.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.8/commen/unit_request.py` & `huhangkai-1.1.9/commen/unit_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,28 +145,31 @@
         except MissingSchema:
             assert False, "url不对，无域名"
         except Exception as e:
             print(e)
             assert False, "调用接口报错"
 
     def get_variable(self, app_key=None, env=None):
-        app_key = app_key or self.APP_KEY
-        env = env or self.ZEST_ENV
-        project = requests.post(admin_host + '/variable/variable/',
-                                json={"app_key": app_key, "environment": env}).json()
-        _variable = {}
-        for v in project.get('variables', []):
-            if v.get('type') == 0:
-                _variable[v.get('name')] = v.get('value')
-            elif v.get('type') == 1:
-                _variable[v.get('name')] = json.loads(v.get('value'))
-            elif v.get('type') == 2:
-                _variable[v.get('name')] = int(json.loads(v.get('value')))
-        _variable["_token"] = project.get("token")
-        return _variable
+        try:
+            app_key = app_key or self.APP_KEY
+            env = env or self.ZEST_ENV
+            project = requests.post(admin_host + '/variable/variable/',
+                                    json={"app_key": app_key, "environment": env}).json()
+            _variable = {}
+            for v in project.get('variables', []):
+                if v.get('type') == 0:
+                    _variable[v.get('name')] = v.get('value')
+                elif v.get('type') == 1:
+                    _variable[v.get('name')] = json.loads(v.get('value'))
+                elif v.get('type') == 2:
+                    _variable[v.get('name')] = int(json.loads(v.get('value')))
+            _variable["_token"] = project.get("token")
+            return _variable
+        except:
+            return {}
 
     def init_headers(self, **kwargs):
         headers = {"Content-Type": "application/json"}
         _host = kwargs.get("_host", "HOST")
         host = self.variable.get(_host) if "//" not in _host else _host
         if host:
             headers.update({"referer": host})
```

### Comparing `huhangkai-1.1.8/commen/unit_tasks.py` & `huhangkai-1.1.9/commen/unit_tasks.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.8/setup.py` & `huhangkai-1.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='huhangkai',  # 对外模块的名字
-    version='1.1.8',  # 版本号
+    version='1.1.9',  # 版本号
     description='接口自动化',  # 描述
     author='胡杭凯',  # 作者
     author_email='3173825608@qq.com',
     # package_dir={"": "commen"},
     packages=find_packages(),
     package_data={'by': ['常用命令.bat'],},
     python_requires=">=3.0",
```

