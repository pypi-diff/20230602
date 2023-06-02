# Comparing `tmp/wombo-0.1.4.tar.gz` & `tmp/wombo-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wombo-0.1.4.tar", max compression
+gzip compressed data, was "wombo-0.1.5.tar", max compression
```

## Comparing `wombo-0.1.4.tar` & `wombo-0.1.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1066 2023-06-02 14:02:35.382424 wombo-0.1.4/LICENSE
--rw-r--r--   0        0        0       35 2023-06-02 15:32:46.562424 wombo-0.1.4/README.md
--rw-r--r--   0        0        0      340 2023-06-02 16:01:10.574424 wombo-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       70 2023-06-02 14:20:19.386424 wombo-0.1.4/wombo/__init__.py
--rw-r--r--   0        0        0     4013 2023-06-02 15:51:51.722424 wombo-0.1.4/wombo/async_dream.py
--rw-r--r--   0        0        0     3421 2023-06-02 15:37:20.226424 wombo-0.1.4/wombo/dream.py
--rw-r--r--   0        0        0       93 2023-06-02 14:55:39.890424 wombo-0.1.4/wombo/models/__init__.py
--rw-r--r--   0        0        0      524 2023-06-02 15:01:24.554424 wombo-0.1.4/wombo/models/check_task.py
--rw-r--r--   0        0        0      513 2023-06-02 14:46:35.578424 wombo-0.1.4/wombo/models/create_task.py
--rw-r--r--   0        0        0     3274 2023-06-02 14:21:55.846424 wombo-0.1.4/wombo/urls.py
--rw-r--r--   0        0        0      558 1970-01-01 00:00:00.000000 wombo-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-02 14:02:35.382424 wombo-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1335 2023-06-02 16:53:17.418424 wombo-0.1.5/README.md
+-rw-r--r--   0        0        0      340 2023-06-02 16:54:17.362424 wombo-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       70 2023-06-02 14:20:19.386424 wombo-0.1.5/wombo/__init__.py
+-rw-r--r--   0        0        0     4013 2023-06-02 15:51:51.722424 wombo-0.1.5/wombo/async_dream.py
+-rw-r--r--   0        0        0     3421 2023-06-02 15:37:20.226424 wombo-0.1.5/wombo/dream.py
+-rw-r--r--   0        0        0       93 2023-06-02 14:55:39.890424 wombo-0.1.5/wombo/models/__init__.py
+-rw-r--r--   0        0        0      524 2023-06-02 15:01:24.554424 wombo-0.1.5/wombo/models/check_task.py
+-rw-r--r--   0        0        0      513 2023-06-02 14:46:35.578424 wombo-0.1.5/wombo/models/create_task.py
+-rw-r--r--   0        0        0     3274 2023-06-02 14:21:55.846424 wombo-0.1.5/wombo/urls.py
+-rw-r--r--   0        0        0     1858 1970-01-01 00:00:00.000000 wombo-0.1.5/PKG-INFO
```

### Comparing `wombo-0.1.4/LICENSE` & `wombo-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wombo-0.1.4/wombo/async_dream.py` & `wombo-0.1.5/wombo/async_dream.py`

 * *Files identical despite different names*

### Comparing `wombo-0.1.4/wombo/dream.py` & `wombo-0.1.5/wombo/dream.py`

 * *Files identical despite different names*

### Comparing `wombo-0.1.4/wombo/models/check_task.py` & `wombo-0.1.5/wombo/models/check_task.py`

 * *Files identical despite different names*

### Comparing `wombo-0.1.4/wombo/models/create_task.py` & `wombo-0.1.5/wombo/models/create_task.py`

 * *Files identical despite different names*

### Comparing `wombo-0.1.4/wombo/urls.py` & `wombo-0.1.5/wombo/urls.py`

 * *Files identical despite different names*

