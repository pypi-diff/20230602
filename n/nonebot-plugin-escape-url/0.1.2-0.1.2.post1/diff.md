# Comparing `tmp/nonebot_plugin_escape_url-0.1.2.tar.gz` & `tmp/nonebot_plugin_escape_url-0.1.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_escape_url-0.1.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_escape_url-0.1.2.post1.tar", max compression
```

## Comparing `nonebot_plugin_escape_url-0.1.2.tar` & `nonebot_plugin_escape_url-0.1.2.post1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       49 2023-05-31 15:01:24.094557 nonebot_plugin_escape_url-0.1.2/nonebot_plugin_escape_url/__init__.py
--rw-r--r--   0        0        0      240 2023-06-02 00:25:18.879236 nonebot_plugin_escape_url-0.1.2/nonebot_plugin_escape_url/config.py
--rw-r--r--   0        0        0     1055 2023-06-02 02:59:27.534005 nonebot_plugin_escape_url-0.1.2/nonebot_plugin_escape_url/core.py
--rw-r--r--   0        0        0     1148 2023-06-02 00:25:54.493031 nonebot_plugin_escape_url-0.1.2/nonebot_plugin_escape_url/onebot_v11.py
--rw-r--r--   0        0        0      915 2023-06-02 00:25:54.503107 nonebot_plugin_escape_url-0.1.2/nonebot_plugin_escape_url/qqguild.py
--rw-r--r--   0        0        0      549 2023-06-02 02:59:43.524176 nonebot_plugin_escape_url-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      223 2023-05-31 15:17:18.124586 nonebot_plugin_escape_url-0.1.2/README.md
--rw-r--r--   0        0        0      657 1970-01-01 00:00:00.000000 nonebot_plugin_escape_url-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      249 2023-06-02 03:07:29.081683 nonebot_plugin_escape_url-0.1.2.post1/nonebot_plugin_escape_url/__init__.py
+-rw-r--r--   0        0        0      240 2023-06-02 00:25:18.879236 nonebot_plugin_escape_url-0.1.2.post1/nonebot_plugin_escape_url/config.py
+-rw-r--r--   0        0        0     1055 2023-06-02 02:59:27.534005 nonebot_plugin_escape_url-0.1.2.post1/nonebot_plugin_escape_url/core.py
+-rw-r--r--   0        0        0     1148 2023-06-02 00:25:54.493031 nonebot_plugin_escape_url-0.1.2.post1/nonebot_plugin_escape_url/onebot_v11.py
+-rw-r--r--   0        0        0      915 2023-06-02 00:25:54.503107 nonebot_plugin_escape_url-0.1.2.post1/nonebot_plugin_escape_url/qqguild.py
+-rw-r--r--   0        0        0      555 2023-06-02 03:07:51.613869 nonebot_plugin_escape_url-0.1.2.post1/pyproject.toml
+-rw-r--r--   0        0        0      223 2023-05-31 15:17:18.124586 nonebot_plugin_escape_url-0.1.2.post1/README.md
+-rw-r--r--   0        0        0      663 1970-01-01 00:00:00.000000 nonebot_plugin_escape_url-0.1.2.post1/PKG-INFO
```

### Comparing `nonebot_plugin_escape_url-0.1.2/nonebot_plugin_escape_url/core.py` & `nonebot_plugin_escape_url-0.1.2.post1/nonebot_plugin_escape_url/core.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_escape_url-0.1.2/nonebot_plugin_escape_url/onebot_v11.py` & `nonebot_plugin_escape_url-0.1.2.post1/nonebot_plugin_escape_url/onebot_v11.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_escape_url-0.1.2/nonebot_plugin_escape_url/qqguild.py` & `nonebot_plugin_escape_url-0.1.2.post1/nonebot_plugin_escape_url/qqguild.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_escape_url-0.1.2/pyproject.toml` & `nonebot_plugin_escape_url-0.1.2.post1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-escape-url"
-version = "0.1.2"
+version = "0.1.2.post1"
 description = ""
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 readme = "README.md"
 packages = [{ include = "nonebot_plugin_escape_url" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `nonebot_plugin_escape_url-0.1.2/PKG-INFO` & `nonebot_plugin_escape_url-0.1.2.post1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-escape-url
-Version: 0.1.2
+Version: 0.1.2.post1
 Summary: 
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

