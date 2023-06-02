# Comparing `tmp/instructprompt-0.1.1.tar.gz` & `tmp/instructprompt-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instructprompt-0.1.1.tar", max compression
+gzip compressed data, was "instructprompt-0.1.2.tar", max compression
```

## Comparing `instructprompt-0.1.1.tar` & `instructprompt-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     2260 2023-06-02 02:49:53.992167 instructprompt-0.1.1/README.md
--rw-r--r--   0        0        0      641 2023-06-02 02:50:32.737847 instructprompt-0.1.1/instructprompt/__init__.py
--rw-r--r--   0        0        0      302 2023-06-02 02:50:30.106927 instructprompt-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2602 1970-01-01 00:00:00.000000 instructprompt-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2260 2023-06-02 02:49:53.992167 instructprompt-0.1.2/README.md
+-rw-r--r--   0        0        0      641 2023-06-02 02:55:41.502578 instructprompt-0.1.2/instructprompt/__init__.py
+-rw-r--r--   0        0        0      301 2023-06-02 02:55:43.259621 instructprompt-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2752 1970-01-01 00:00:00.000000 instructprompt-0.1.2/PKG-INFO
```

### Comparing `instructprompt-0.1.1/README.md` & `instructprompt-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `instructprompt-0.1.1/instructprompt/__init__.py` & `instructprompt-0.1.2/instructprompt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ == "0.1.1"
+__version__ == "0.1.2"
 
 import chromadb
 
 chroma_client = chromadb.Client()
 collection = chroma_client.create_collection(name="user_instructprompt_collection")
 
 def add(instruction: str):
```

### Comparing `instructprompt-0.1.1/PKG-INFO` & `instructprompt-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: instructprompt
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: krrishdholakia
 Author-email: krrishdholakia@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: chromadb (>=0.3.25,<0.4.0)
 Description-Content-Type: text/markdown
 
 # InstructPrompt 📝🔍
 
 ⚡ A Python package for storing, retrieving, and dynamically creating prompts for GPT models ⚡
```

