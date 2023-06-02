# Comparing `tmp/huhangkai-1.1.7.tar.gz` & `tmp/huhangkai-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huhangkai-1.1.7.tar", last modified: Fri Jun  2 09:36:54 2023, max compression
+gzip compressed data, was "huhangkai-1.1.8.tar", last modified: Fri Jun  2 09:56:22 2023, max compression
```

## Comparing `huhangkai-1.1.7.tar` & `huhangkai-1.1.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 09:36:54.794816 huhangkai-1.1.7/
--rw-rw-rw-   0        0        0      228 2023-06-02 09:36:54.794816 huhangkai-1.1.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-02 09:36:54.783844 huhangkai-1.1.7/commen/
--rw-rw-rw-   0        0        0      929 2023-01-30 02:59:52.000000 huhangkai-1.1.7/commen/__init__.py
--rw-rw-rw-   0        0        0    31571 2023-06-02 07:34:45.000000 huhangkai-1.1.7/commen/init_project.py
--rw-rw-rw-   0        0        0     4508 2023-05-25 08:37:49.000000 huhangkai-1.1.7/commen/unit_dict.py
--rw-rw-rw-   0        0        0     3843 2023-05-25 08:46:34.000000 huhangkai-1.1.7/commen/unit_encryption.py
--rw-rw-rw-   0        0        0    20401 2023-05-25 08:37:49.000000 huhangkai-1.1.7/commen/unit_fun.py
--rw-rw-rw-   0        0        0     1242 2023-05-25 08:37:49.000000 huhangkai-1.1.7/commen/unit_logger.py
--rw-rw-rw-   0        0        0     9067 2023-06-02 07:33:37.000000 huhangkai-1.1.7/commen/unit_request.py
--rw-rw-rw-   0        0        0     2461 2023-05-25 08:37:49.000000 huhangkai-1.1.7/commen/unit_tasks.py
-drwxrwxrwx   0        0        0        0 2023-06-02 09:36:54.792820 huhangkai-1.1.7/huhangkai.egg-info/
--rw-rw-rw-   0        0        0      228 2023-06-02 09:36:54.000000 huhangkai-1.1.7/huhangkai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      345 2023-06-02 09:36:54.000000 huhangkai-1.1.7/huhangkai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 09:36:54.000000 huhangkai-1.1.7/huhangkai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-06-02 09:36:54.000000 huhangkai-1.1.7/huhangkai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-02 09:36:54.000000 huhangkai-1.1.7/huhangkai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 09:36:54.795812 huhangkai-1.1.7/setup.cfg
--rw-rw-rw-   0        0        0      558 2023-06-02 09:36:44.000000 huhangkai-1.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 09:56:22.053095 huhangkai-1.1.8/
+-rw-rw-rw-   0        0        0      228 2023-06-02 09:56:22.053095 huhangkai-1.1.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-02 09:56:22.041128 huhangkai-1.1.8/commen/
+-rw-rw-rw-   0        0        0      929 2023-01-30 02:59:52.000000 huhangkai-1.1.8/commen/__init__.py
+-rw-rw-rw-   0        0        0    31571 2023-06-02 07:34:45.000000 huhangkai-1.1.8/commen/init_project.py
+-rw-rw-rw-   0        0        0     4508 2023-05-25 08:37:49.000000 huhangkai-1.1.8/commen/unit_dict.py
+-rw-rw-rw-   0        0        0     3843 2023-05-25 08:46:34.000000 huhangkai-1.1.8/commen/unit_encryption.py
+-rw-rw-rw-   0        0        0    20401 2023-05-25 08:37:49.000000 huhangkai-1.1.8/commen/unit_fun.py
+-rw-rw-rw-   0        0        0     1242 2023-05-25 08:37:49.000000 huhangkai-1.1.8/commen/unit_logger.py
+-rw-rw-rw-   0        0        0     9108 2023-06-02 09:56:08.000000 huhangkai-1.1.8/commen/unit_request.py
+-rw-rw-rw-   0        0        0     2461 2023-05-25 08:37:49.000000 huhangkai-1.1.8/commen/unit_tasks.py
+drwxrwxrwx   0        0        0        0 2023-06-02 09:56:22.051099 huhangkai-1.1.8/huhangkai.egg-info/
+-rw-rw-rw-   0        0        0      228 2023-06-02 09:56:21.000000 huhangkai-1.1.8/huhangkai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      345 2023-06-02 09:56:21.000000 huhangkai-1.1.8/huhangkai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 09:56:21.000000 huhangkai-1.1.8/huhangkai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-02 09:56:21.000000 huhangkai-1.1.8/huhangkai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-02 09:56:21.000000 huhangkai-1.1.8/huhangkai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 09:56:22.054092 huhangkai-1.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      558 2023-06-02 09:56:08.000000 huhangkai-1.1.8/setup.py
```

### Comparing `huhangkai-1.1.7/commen/__init__.py` & `huhangkai-1.1.8/commen/__init__.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.7/commen/init_project.py` & `huhangkai-1.1.8/commen/init_project.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.7/commen/unit_dict.py` & `huhangkai-1.1.8/commen/unit_dict.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.7/commen/unit_encryption.py` & `huhangkai-1.1.8/commen/unit_encryption.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.7/commen/unit_fun.py` & `huhangkai-1.1.8/commen/unit_fun.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.7/commen/unit_logger.py` & `huhangkai-1.1.8/commen/unit_logger.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.7/commen/unit_request.py` & `huhangkai-1.1.8/commen/unit_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,8 +184,8 @@
         _host = kwargs.get("_host", "HOST")
         host = self.variable.get(_host) if "//" not in _host else _host
         return self.unit_http_requester(*args, host=host, timeout=self.TIMEOUT, init_headers=self.init_headers(**kwargs), **kwargs)
 
 
 get_url = UnitRequest.get_url
 unit_http_requester = UnitRequest.unit_http_requester
-
+get_variable = UnitRequest().get_variable
```

### Comparing `huhangkai-1.1.7/commen/unit_tasks.py` & `huhangkai-1.1.8/commen/unit_tasks.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.7/setup.py` & `huhangkai-1.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='huhangkai',  # 对外模块的名字
-    version='1.1.7',  # 版本号
+    version='1.1.8',  # 版本号
     description='接口自动化',  # 描述
     author='胡杭凯',  # 作者
     author_email='3173825608@qq.com',
     # package_dir={"": "commen"},
     packages=find_packages(),
     package_data={'by': ['常用命令.bat'],},
     python_requires=">=3.0",
```

