# Comparing `tmp/langchainplus_sdk-0.0.1rc4.tar.gz` & `tmp/langchainplus_sdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchainplus_sdk-0.0.1rc4.tar", max compression
+gzip compressed data, was "langchainplus_sdk-0.0.2.tar", max compression
```

## Comparing `langchainplus_sdk-0.0.1rc4.tar` & `langchainplus_sdk-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      757 2023-06-01 21:57:11.090090 langchainplus_sdk-0.0.1rc4/README.md
--rw-r--r--   0        0        0      119 2023-06-01 21:57:11.090090 langchainplus_sdk-0.0.1rc4/langchainplus_sdk/__init__.py
--rw-r--r--   0        0        0    17480 2023-06-01 21:57:11.090090 langchainplus_sdk-0.0.1rc4/langchainplus_sdk/client.py
--rw-r--r--   0        0        0     6994 2023-06-01 21:57:11.090090 langchainplus_sdk-0.0.1rc4/langchainplus_sdk/run_trees.py
--rw-r--r--   0        0        0     6893 2023-06-01 21:57:11.090090 langchainplus_sdk-0.0.1rc4/langchainplus_sdk/schemas.py
--rw-r--r--   0        0        0     2801 2023-06-01 21:57:11.090090 langchainplus_sdk-0.0.1rc4/langchainplus_sdk/utils.py
--rw-r--r--   0        0        0      796 2023-06-01 21:57:11.090090 langchainplus_sdk-0.0.1rc4/pyproject.toml
--rw-r--r--   0        0        0     1393 1970-01-01 00:00:00.000000 langchainplus_sdk-0.0.1rc4/PKG-INFO
+-rw-r--r--   0        0        0     6974 2023-06-02 03:35:04.040844 langchainplus_sdk-0.0.2/README.md
+-rw-r--r--   0        0        0      119 2023-06-02 03:35:04.040844 langchainplus_sdk-0.0.2/langchainplus_sdk/__init__.py
+-rw-r--r--   0        0        0    17480 2023-06-02 03:35:04.040844 langchainplus_sdk-0.0.2/langchainplus_sdk/client.py
+-rw-r--r--   0        0        0     6994 2023-06-02 03:35:04.040844 langchainplus_sdk-0.0.2/langchainplus_sdk/run_trees.py
+-rw-r--r--   0        0        0     6893 2023-06-02 03:35:04.040844 langchainplus_sdk-0.0.2/langchainplus_sdk/schemas.py
+-rw-r--r--   0        0        0     2801 2023-06-02 03:35:04.040844 langchainplus_sdk-0.0.2/langchainplus_sdk/utils.py
+-rw-r--r--   0        0        0      792 2023-06-02 03:35:04.040844 langchainplus_sdk-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     7607 1970-01-01 00:00:00.000000 langchainplus_sdk-0.0.2/PKG-INFO
```

### Comparing `langchainplus_sdk-0.0.1rc4/langchainplus_sdk/client.py` & `langchainplus_sdk-0.0.2/langchainplus_sdk/client.py`

 * *Files identical despite different names*

### Comparing `langchainplus_sdk-0.0.1rc4/langchainplus_sdk/run_trees.py` & `langchainplus_sdk-0.0.2/langchainplus_sdk/run_trees.py`

 * *Files identical despite different names*

### Comparing `langchainplus_sdk-0.0.1rc4/langchainplus_sdk/schemas.py` & `langchainplus_sdk-0.0.2/langchainplus_sdk/schemas.py`

 * *Files identical despite different names*

### Comparing `langchainplus_sdk-0.0.1rc4/langchainplus_sdk/utils.py` & `langchainplus_sdk-0.0.2/langchainplus_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `langchainplus_sdk-0.0.1rc4/pyproject.toml` & `langchainplus_sdk-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchainplus-sdk"
-version = "0.0.1-rc4"
+version = "0.0.2"
 description = "Client library to connect to the LangChainPlus LLM Tracing and Evaluation Platform."
 authors = ["LangChain"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "langchainplus_sdk"}]
 
 [tool.poetry.dependencies]
```

