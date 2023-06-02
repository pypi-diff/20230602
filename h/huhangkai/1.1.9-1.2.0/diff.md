# Comparing `tmp/huhangkai-1.1.9.tar.gz` & `tmp/huhangkai-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huhangkai-1.1.9.tar", last modified: Fri Jun  2 10:03:21 2023, max compression
+gzip compressed data, was "huhangkai-1.2.0.tar", last modified: Fri Jun  2 10:32:55 2023, max compression
```

## Comparing `huhangkai-1.1.9.tar` & `huhangkai-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 10:03:21.049224 huhangkai-1.1.9/
--rw-rw-rw-   0        0        0      228 2023-06-02 10:03:21.049224 huhangkai-1.1.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-02 10:03:21.037411 huhangkai-1.1.9/commen/
--rw-rw-rw-   0        0        0      929 2023-01-30 02:59:52.000000 huhangkai-1.1.9/commen/__init__.py
--rw-rw-rw-   0        0        0    31571 2023-06-02 07:34:45.000000 huhangkai-1.1.9/commen/init_project.py
--rw-rw-rw-   0        0        0     4508 2023-05-25 08:37:49.000000 huhangkai-1.1.9/commen/unit_dict.py
--rw-rw-rw-   0        0        0     3843 2023-05-25 08:46:34.000000 huhangkai-1.1.9/commen/unit_encryption.py
--rw-rw-rw-   0        0        0    20401 2023-05-25 08:37:49.000000 huhangkai-1.1.9/commen/unit_fun.py
--rw-rw-rw-   0        0        0     1242 2023-05-25 08:37:49.000000 huhangkai-1.1.9/commen/unit_logger.py
--rw-rw-rw-   0        0        0     9218 2023-06-02 10:02:56.000000 huhangkai-1.1.9/commen/unit_request.py
--rw-rw-rw-   0        0        0     2461 2023-05-25 08:37:49.000000 huhangkai-1.1.9/commen/unit_tasks.py
-drwxrwxrwx   0        0        0        0 2023-06-02 10:03:21.047235 huhangkai-1.1.9/huhangkai.egg-info/
--rw-rw-rw-   0        0        0      228 2023-06-02 10:03:20.000000 huhangkai-1.1.9/huhangkai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      345 2023-06-02 10:03:20.000000 huhangkai-1.1.9/huhangkai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 10:03:20.000000 huhangkai-1.1.9/huhangkai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-06-02 10:03:20.000000 huhangkai-1.1.9/huhangkai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-02 10:03:20.000000 huhangkai-1.1.9/huhangkai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 10:03:21.050220 huhangkai-1.1.9/setup.cfg
--rw-rw-rw-   0        0        0      558 2023-06-02 10:03:15.000000 huhangkai-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:32:55.447068 huhangkai-1.2.0/
+-rw-rw-rw-   0        0        0      228 2023-06-02 10:32:55.446068 huhangkai-1.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-02 10:32:55.435098 huhangkai-1.2.0/commen/
+-rw-rw-rw-   0        0        0      929 2023-01-30 02:59:52.000000 huhangkai-1.2.0/commen/__init__.py
+-rw-rw-rw-   0        0        0    31571 2023-06-02 07:34:45.000000 huhangkai-1.2.0/commen/init_project.py
+-rw-rw-rw-   0        0        0     4508 2023-05-25 08:37:49.000000 huhangkai-1.2.0/commen/unit_dict.py
+-rw-rw-rw-   0        0        0     3843 2023-05-25 08:46:34.000000 huhangkai-1.2.0/commen/unit_encryption.py
+-rw-rw-rw-   0        0        0    20438 2023-06-02 10:32:12.000000 huhangkai-1.2.0/commen/unit_fun.py
+-rw-rw-rw-   0        0        0     1242 2023-05-25 08:37:49.000000 huhangkai-1.2.0/commen/unit_logger.py
+-rw-rw-rw-   0        0        0     9218 2023-06-02 10:02:56.000000 huhangkai-1.2.0/commen/unit_request.py
+-rw-rw-rw-   0        0        0     2461 2023-05-25 08:37:49.000000 huhangkai-1.2.0/commen/unit_tasks.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:32:55.445071 huhangkai-1.2.0/huhangkai.egg-info/
+-rw-rw-rw-   0        0        0      228 2023-06-02 10:32:55.000000 huhangkai-1.2.0/huhangkai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      345 2023-06-02 10:32:55.000000 huhangkai-1.2.0/huhangkai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 10:32:55.000000 huhangkai-1.2.0/huhangkai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-02 10:32:55.000000 huhangkai-1.2.0/huhangkai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-02 10:32:55.000000 huhangkai-1.2.0/huhangkai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 10:32:55.447068 huhangkai-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      558 2023-06-02 10:32:46.000000 huhangkai-1.2.0/setup.py
```

### Comparing `huhangkai-1.1.9/commen/__init__.py` & `huhangkai-1.2.0/commen/__init__.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.9/commen/init_project.py` & `huhangkai-1.2.0/commen/init_project.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.9/commen/unit_dict.py` & `huhangkai-1.2.0/commen/unit_dict.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.9/commen/unit_encryption.py` & `huhangkai-1.2.0/commen/unit_encryption.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.9/commen/unit_fun.py` & `huhangkai-1.2.0/commen/unit_fun.py`

 * *Files 0% similar despite different names*

```diff
@@ -447,29 +447,29 @@
                         return [i.get(name) for i in value]
                     elif isinstance(value, dict):
                         for key2, value2 in value.items():
                             if isinstance(value2, list):
                                 return [i.get(name) for i in value2 if i.get(name)]
             return []
 
-    def excelWriter(self, filename, data):
+    def excelWriter(self, filename, data, sheet_name="sheet", set_column=[]):
         from pandas import DataFrame, ExcelWriter
         filename = filename[:4] + filename[4:].replace(":", "").replace(' ', '_')
         with ExcelWriter(filename) as writer:
             # 写入到第一个sheet
             if data and isinstance(data[0], list):
                 h = data[0]
                 data1 = []
                 for i in data[1:]:
                     data1.append({x[0]: str(x[1]) for x in zip(h, i)})
                 data = data1
             elif data and isinstance(data[0], dict):
                 data = [{k: str(v) for k, v in i.items()} for i in data]
             DataFrame(data).to_excel(writer,
-                              sheet_name="sheet1",
+                              sheet_name=sheet_name,
                               index=False,
                               engine="openpyxl"
                               )
 
 
 if __name__ == '__main__':
     print(FunBase().random_carnum())
```

### Comparing `huhangkai-1.1.9/commen/unit_logger.py` & `huhangkai-1.2.0/commen/unit_logger.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.9/commen/unit_request.py` & `huhangkai-1.2.0/commen/unit_request.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.9/commen/unit_tasks.py` & `huhangkai-1.2.0/commen/unit_tasks.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.9/setup.py` & `huhangkai-1.2.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='huhangkai',  # 对外模块的名字
-    version='1.1.9',  # 版本号
+    version='1.2.0',  # 版本号
     description='接口自动化',  # 描述
     author='胡杭凯',  # 作者
     author_email='3173825608@qq.com',
     # package_dir={"": "commen"},
     packages=find_packages(),
     package_data={'by': ['常用命令.bat'],},
     python_requires=">=3.0",
```

