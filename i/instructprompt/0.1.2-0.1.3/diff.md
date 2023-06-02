# Comparing `tmp/instructprompt-0.1.2.tar.gz` & `tmp/instructprompt-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instructprompt-0.1.2.tar", max compression
+gzip compressed data, was "instructprompt-0.1.3.tar", max compression
```

## Comparing `instructprompt-0.1.2.tar` & `instructprompt-0.1.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     2260 2023-06-02 02:49:53.992167 instructprompt-0.1.2/README.md
--rw-r--r--   0        0        0      641 2023-06-02 02:55:41.502578 instructprompt-0.1.2/instructprompt/__init__.py
--rw-r--r--   0        0        0      301 2023-06-02 02:55:43.259621 instructprompt-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2752 1970-01-01 00:00:00.000000 instructprompt-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2260 2023-06-02 02:49:53.992167 instructprompt-0.1.3/README.md
+-rw-r--r--   0        0        0      640 2023-06-02 02:57:08.994681 instructprompt-0.1.3/instructprompt/__init__.py
+-rw-r--r--   0        0        0      301 2023-06-02 02:57:15.577607 instructprompt-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2752 1970-01-01 00:00:00.000000 instructprompt-0.1.3/PKG-INFO
```

### Comparing `instructprompt-0.1.2/README.md` & `instructprompt-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `instructprompt-0.1.2/instructprompt/__init__.py` & `instructprompt-0.1.3/instructprompt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ == "0.1.2"
+__version__ = '0.1.2'
 
 import chromadb
 
 chroma_client = chromadb.Client()
 collection = chroma_client.create_collection(name="user_instructprompt_collection")
 
 def add(instruction: str):
```

### Comparing `instructprompt-0.1.2/PKG-INFO` & `instructprompt-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instructprompt
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: krrishdholakia
 Author-email: krrishdholakia@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

