# Comparing `tmp/zeuscloud_iamspy-0.7.0.tar.gz` & `tmp/zeuscloud_iamspy-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeuscloud_iamspy-0.7.0.tar", max compression
+gzip compressed data, was "zeuscloud_iamspy-0.8.0.tar", max compression
```

## Comparing `zeuscloud_iamspy-0.7.0.tar` & `zeuscloud_iamspy-0.8.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11347 2023-03-24 18:14:28.794551 zeuscloud_iamspy-0.7.0/LICENSE.md
--rw-r--r--   0        0        0      564 2023-03-24 23:12:32.582059 zeuscloud_iamspy-0.7.0/pyproject.toml
--rw-r--r--   0        0        0       41 2023-03-24 22:40:26.551965 zeuscloud_iamspy-0.7.0/zeuscloud_iamspy/__init__.py
--rw-r--r--   0        0        0     2656 2023-03-24 18:23:16.154477 zeuscloud_iamspy-0.7.0/zeuscloud_iamspy/cli.py
--rw-r--r--   0        0        0    11163 2023-03-24 18:23:27.934874 zeuscloud_iamspy-0.7.0/zeuscloud_iamspy/conditions.py
--rw-r--r--   0        0        0     2995 2023-03-24 18:17:05.350265 zeuscloud_iamspy-0.7.0/zeuscloud_iamspy/datatypes.py
--rw-r--r--   0        0        0     6646 2023-03-24 18:17:05.350344 zeuscloud_iamspy-0.7.0/zeuscloud_iamspy/iam.py
--rw-r--r--   0        0        0      499 2023-03-24 18:17:05.350412 zeuscloud_iamspy-0.7.0/zeuscloud_iamspy/log_config.py
--rw-r--r--   0        0        0     7935 2023-03-24 23:05:32.997831 zeuscloud_iamspy-0.7.0/zeuscloud_iamspy/model.py
--rw-r--r--   0        0        0    16913 2023-03-24 18:23:32.769909 zeuscloud_iamspy-0.7.0/zeuscloud_iamspy/parse.py
--rw-r--r--   0        0        0     1057 2023-03-24 18:17:05.350666 zeuscloud_iamspy-0.7.0/zeuscloud_iamspy/utils.py
--rw-r--r--   0        0        0      542 1970-01-01 00:00:00.000000 zeuscloud_iamspy-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11347 2023-03-24 18:14:28.794551 zeuscloud_iamspy-0.8.0/LICENSE.md
+-rw-r--r--   0        0        0      564 2023-06-02 06:50:40.982834 zeuscloud_iamspy-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0       41 2023-03-24 22:40:26.551965 zeuscloud_iamspy-0.8.0/zeuscloud_iamspy/__init__.py
+-rw-r--r--   0        0        0     2656 2023-03-24 18:23:16.154477 zeuscloud_iamspy-0.8.0/zeuscloud_iamspy/cli.py
+-rw-r--r--   0        0        0    11163 2023-03-24 18:23:27.934874 zeuscloud_iamspy-0.8.0/zeuscloud_iamspy/conditions.py
+-rw-r--r--   0        0        0     2995 2023-03-24 18:17:05.350265 zeuscloud_iamspy-0.8.0/zeuscloud_iamspy/datatypes.py
+-rw-r--r--   0        0        0     6646 2023-03-24 18:17:05.350344 zeuscloud_iamspy-0.8.0/zeuscloud_iamspy/iam.py
+-rw-r--r--   0        0        0      499 2023-03-24 18:17:05.350412 zeuscloud_iamspy-0.8.0/zeuscloud_iamspy/log_config.py
+-rw-r--r--   0        0        0     7935 2023-03-24 23:05:32.997831 zeuscloud_iamspy-0.8.0/zeuscloud_iamspy/model.py
+-rw-r--r--   0        0        0    17072 2023-06-02 01:31:20.502932 zeuscloud_iamspy-0.8.0/zeuscloud_iamspy/parse.py
+-rw-r--r--   0        0        0     1057 2023-03-24 18:17:05.350666 zeuscloud_iamspy-0.8.0/zeuscloud_iamspy/utils.py
+-rw-r--r--   0        0        0      542 1970-01-01 00:00:00.000000 zeuscloud_iamspy-0.8.0/PKG-INFO
```

### Comparing `zeuscloud_iamspy-0.7.0/LICENSE.md` & `zeuscloud_iamspy-0.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `zeuscloud_iamspy-0.7.0/pyproject.toml` & `zeuscloud_iamspy-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zeuscloud-iamspy"
-version = "0.7.0"
+version = "0.8.0"
 description = "ZeusCloud fork of IAMSpy"
 authors = ["Varun Jain <varun@zeuscloud.io>"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 z3-solver = "*"
 pydantic = "*"
```

### Comparing `zeuscloud_iamspy-0.7.0/zeuscloud_iamspy/cli.py` & `zeuscloud_iamspy-0.8.0/zeuscloud_iamspy/cli.py`

 * *Files identical despite different names*

### Comparing `zeuscloud_iamspy-0.7.0/zeuscloud_iamspy/conditions.py` & `zeuscloud_iamspy-0.8.0/zeuscloud_iamspy/conditions.py`

 * *Files identical despite different names*

### Comparing `zeuscloud_iamspy-0.7.0/zeuscloud_iamspy/datatypes.py` & `zeuscloud_iamspy-0.8.0/zeuscloud_iamspy/datatypes.py`

 * *Files identical despite different names*

### Comparing `zeuscloud_iamspy-0.7.0/zeuscloud_iamspy/iam.py` & `zeuscloud_iamspy-0.8.0/zeuscloud_iamspy/iam.py`

 * *Files identical despite different names*

### Comparing `zeuscloud_iamspy-0.7.0/zeuscloud_iamspy/model.py` & `zeuscloud_iamspy-0.8.0/zeuscloud_iamspy/model.py`

 * *Files identical despite different names*

### Comparing `zeuscloud_iamspy-0.7.0/zeuscloud_iamspy/parse.py` & `zeuscloud_iamspy-0.8.0/zeuscloud_iamspy/parse.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,18 @@
 
 # equivalient to chars in  string.ascii_letters + string.digits + string.punctuation
 ANY = z3.Range("!", "~")
 logger = logging.getLogger("iamspy.parse")
 
 used_conditions = set()
 
+def remove_suffix(input_string, suffix):
+    if suffix and input_string.endswith(suffix):
+        return input_string[:-len(suffix)]
+    return input_string
 
 def json_encoder(obj: Any, nested=True) -> Any:
     """
     For printing results
     """
     if nested:
         obj = pydantic_encoder(obj)
@@ -63,15 +67,15 @@
         logger.debug(f"Condition test: {test}, variables: {variables}")
         if ":" in test:
             logger.warning(
                 f"Multi key/value operator detected: {test}, this is currently not supported, skipping condition"
             )
             continue
         if if_exists := test.endswith("IfExists"):
-            test = test.removesuffix("IfExists")
+            test = remove_suffix(test, "IfExists")
         for key, value in variables.items():
             logger.debug(f"Variable key: {key}, value: {value}")
             used_conditions.add(key)
             if not isinstance(value, list):
                 value = [value]
             items.append(condition_functions[test](f"condition_{key}", value, if_exists=if_exists))
```

### Comparing `zeuscloud_iamspy-0.7.0/zeuscloud_iamspy/utils.py` & `zeuscloud_iamspy-0.8.0/zeuscloud_iamspy/utils.py`

 * *Files identical despite different names*

### Comparing `zeuscloud_iamspy-0.7.0/PKG-INFO` & `zeuscloud_iamspy-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeuscloud-iamspy
-Version: 0.7.0
+Version: 0.8.0
 Summary: ZeusCloud fork of IAMSpy
 Author: Varun Jain
 Author-email: varun@zeuscloud.io
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

