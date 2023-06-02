# Comparing `tmp/nonebot_plugin_escape_url-0.1.1.tar.gz` & `tmp/nonebot_plugin_escape_url-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_escape_url-0.1.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_escape_url-0.1.2.tar", max compression
```

## Comparing `nonebot_plugin_escape_url-0.1.1.tar` & `nonebot_plugin_escape_url-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       49 2023-05-31 15:01:24.094557 nonebot_plugin_escape_url-0.1.1/nonebot_plugin_escape_url/__init__.py
--rw-r--r--   0        0        0      240 2023-06-02 00:25:18.879236 nonebot_plugin_escape_url-0.1.1/nonebot_plugin_escape_url/config.py
--rw-r--r--   0        0        0     1031 2023-06-02 00:36:31.049274 nonebot_plugin_escape_url-0.1.1/nonebot_plugin_escape_url/core.py
--rw-r--r--   0        0        0     1148 2023-06-02 00:25:54.493031 nonebot_plugin_escape_url-0.1.1/nonebot_plugin_escape_url/onebot_v11.py
--rw-r--r--   0        0        0      915 2023-06-02 00:25:54.503107 nonebot_plugin_escape_url-0.1.1/nonebot_plugin_escape_url/qqguild.py
--rw-r--r--   0        0        0      549 2023-06-02 02:42:05.013519 nonebot_plugin_escape_url-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      223 2023-05-31 15:17:18.124586 nonebot_plugin_escape_url-0.1.1/README.md
--rw-r--r--   0        0        0      657 1970-01-01 00:00:00.000000 nonebot_plugin_escape_url-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       49 2023-05-31 15:01:24.094557 nonebot_plugin_escape_url-0.1.2/nonebot_plugin_escape_url/__init__.py
+-rw-r--r--   0        0        0      240 2023-06-02 00:25:18.879236 nonebot_plugin_escape_url-0.1.2/nonebot_plugin_escape_url/config.py
+-rw-r--r--   0        0        0     1055 2023-06-02 02:59:27.534005 nonebot_plugin_escape_url-0.1.2/nonebot_plugin_escape_url/core.py
+-rw-r--r--   0        0        0     1148 2023-06-02 00:25:54.493031 nonebot_plugin_escape_url-0.1.2/nonebot_plugin_escape_url/onebot_v11.py
+-rw-r--r--   0        0        0      915 2023-06-02 00:25:54.503107 nonebot_plugin_escape_url-0.1.2/nonebot_plugin_escape_url/qqguild.py
+-rw-r--r--   0        0        0      549 2023-06-02 02:59:43.524176 nonebot_plugin_escape_url-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      223 2023-05-31 15:17:18.124586 nonebot_plugin_escape_url-0.1.2/README.md
+-rw-r--r--   0        0        0      657 1970-01-01 00:00:00.000000 nonebot_plugin_escape_url-0.1.2/PKG-INFO
```

### Comparing `nonebot_plugin_escape_url-0.1.1/nonebot_plugin_escape_url/core.py` & `nonebot_plugin_escape_url-0.1.2/nonebot_plugin_escape_url/core.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 from io import StringIO
 
 # reg_url = re.compile(
 #     r"(https?://(?:www\.)?[-a-zA-Z\d@:%._+~#=]{1,256}\.[a-zA-Z\d()]{1,6}\b[-a-zA-Z\d()@:%_+.~#?&/=]*)")
-reg_url = re.compile(r"([-a-zA-Z\d]+\.)+[-a-zA-Z\d]+")
+reg_url = re.compile(r"((?=.*[a-z])[-A-Za-z\d]+\.)+((?=.*[a-z])[-A-Za-z\d]+)")
 
 
 def escape_url(url: str, replace_dot_by: str = '🤔') -> str:
     seg = url.split('.')
     return replace_dot_by.join(seg)
```

### Comparing `nonebot_plugin_escape_url-0.1.1/nonebot_plugin_escape_url/onebot_v11.py` & `nonebot_plugin_escape_url-0.1.2/nonebot_plugin_escape_url/onebot_v11.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_escape_url-0.1.1/nonebot_plugin_escape_url/qqguild.py` & `nonebot_plugin_escape_url-0.1.2/nonebot_plugin_escape_url/qqguild.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_escape_url-0.1.1/pyproject.toml` & `nonebot_plugin_escape_url-0.1.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-escape-url"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 readme = "README.md"
 packages = [{ include = "nonebot_plugin_escape_url" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `nonebot_plugin_escape_url-0.1.1/PKG-INFO` & `nonebot_plugin_escape_url-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-escape-url
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

