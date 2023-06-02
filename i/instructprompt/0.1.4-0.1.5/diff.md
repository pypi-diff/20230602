# Comparing `tmp/instructprompt-0.1.4.tar.gz` & `tmp/instructprompt-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instructprompt-0.1.4.tar", max compression
+gzip compressed data, was "instructprompt-0.1.5.tar", max compression
```

## Comparing `instructprompt-0.1.4.tar` & `instructprompt-0.1.5.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0     2156 2023-06-02 03:00:39.063265 instructprompt-0.1.4/README.md
--rw-r--r--   0        0        0      614 2023-06-02 03:01:15.542221 instructprompt-0.1.4/instructprompt/__init__.py
--rw-r--r--   0        0        0      301 2023-06-02 03:01:19.747151 instructprompt-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2648 1970-01-01 00:00:00.000000 instructprompt-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-02 03:10:21.039071 instructprompt-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2156 2023-06-02 03:13:29.844863 instructprompt-0.1.5/README.md
+-rw-r--r--   0        0        0      662 2023-06-02 03:51:23.392049 instructprompt-0.1.5/instructprompt/__init__.py
+-rw-r--r--   0        0        0      301 2023-06-02 03:51:25.310821 instructprompt-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2648 1970-01-01 00:00:00.000000 instructprompt-0.1.5/PKG-INFO
```

### Comparing `instructprompt-0.1.4/README.md` & `instructprompt-0.1.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,57 +4,57 @@
 
 Our goal with InstructPrompt is to make it easier to tame large language models and make improving your LLM in production simpler to do. This package allows users to store instructions, which can be retrieved to dynamically create prompts giving gpt instructions on how to respond to a specific user's query. 
 
 ## Getting Started 
 
 To get started with InstructPrompt, you will need to first install the library by running the following command:
 
-`pip install InstructPrompt`
+`pip install instructprompt`
 
 Once installed, you can import it into your python project by running the following:
 
-`import InstructPrompt`
+`import instructprompt`
 
 ## Using InstructPrompt
 
 InstructPrompt provides 3 main functions: `add()`, `list()`, and `query()`.
 
 ### add()
 
 The `add()` function takes in an instruction as a string and adds it to the collection. It uses ChromaDB to store the instruction and assigns it a unique id. It returns a confirmation message once the instruction is successfully added. 
 
 ```
-import InstructPrompt
+import instructprompt
 
 instruction = "Please provide the customer's name and order number."
 
-InstructPrompt.add(instruction)
+instructprompt.add(instruction)
 ```
 
 ### list()
 
 The `list()` function returns a list of all the stored instructions in the collection. 
 
 ```
-import InstructPrompt
+import instructprompt
 
-instructions = InstructPrompt.list()
+instructions = instructprompt.list()
 print(instructions) # Outputs a list of all the stored instructions
 ```
 
 ### query()
 
 The `query()` function takes in a query as a string and returns a list of instructions that match the query. It uses ChromaDB to perform the query and returns up to 5 matching instructions.
 
 ```
-import InstructPrompt
+import instructprompt
 
 query = "How do I reset my password?"
 
-instructions = InstructPrompt.query(query)
+instructions = instructprompt.query(query)
 print(instructions) # Outputs a list of instructions that match the query
 ```
 
 ## Version
 
 The current version of InstructPrompt is `0.1.0`.
```

### Comparing `instructprompt-0.1.4/instructprompt/__init__.py` & `instructprompt-0.1.5/instructprompt/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-__version__ = '0.1.4'
+__version__ = '0.1.5'
 
 import chromadb
+import random
+
 
 chroma_client = chromadb.Client()
 collection = chroma_client.create_collection(name="user_instructprompt_collection")
 
 def add(instruction: str): 
+    id = random.randint(1, 9999)
     collection.add(
         documents=[instruction],
         ids=[str(id)]
     )
     print("✅ instruction added")
     return
```

### Comparing `instructprompt-0.1.4/PKG-INFO` & `instructprompt-0.1.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instructprompt
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: krrishdholakia
 Author-email: krrishdholakia@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -19,57 +19,57 @@
 
 Our goal with InstructPrompt is to make it easier to tame large language models and make improving your LLM in production simpler to do. This package allows users to store instructions, which can be retrieved to dynamically create prompts giving gpt instructions on how to respond to a specific user's query. 
 
 ## Getting Started 
 
 To get started with InstructPrompt, you will need to first install the library by running the following command:
 
-`pip install InstructPrompt`
+`pip install instructprompt`
 
 Once installed, you can import it into your python project by running the following:
 
-`import InstructPrompt`
+`import instructprompt`
 
 ## Using InstructPrompt
 
 InstructPrompt provides 3 main functions: `add()`, `list()`, and `query()`.
 
 ### add()
 
 The `add()` function takes in an instruction as a string and adds it to the collection. It uses ChromaDB to store the instruction and assigns it a unique id. It returns a confirmation message once the instruction is successfully added. 
 
 ```
-import InstructPrompt
+import instructprompt
 
 instruction = "Please provide the customer's name and order number."
 
-InstructPrompt.add(instruction)
+instructprompt.add(instruction)
 ```
 
 ### list()
 
 The `list()` function returns a list of all the stored instructions in the collection. 
 
 ```
-import InstructPrompt
+import instructprompt
 
-instructions = InstructPrompt.list()
+instructions = instructprompt.list()
 print(instructions) # Outputs a list of all the stored instructions
 ```
 
 ### query()
 
 The `query()` function takes in a query as a string and returns a list of instructions that match the query. It uses ChromaDB to perform the query and returns up to 5 matching instructions.
 
 ```
-import InstructPrompt
+import instructprompt
 
 query = "How do I reset my password?"
 
-instructions = InstructPrompt.query(query)
+instructions = instructprompt.query(query)
 print(instructions) # Outputs a list of instructions that match the query
 ```
 
 ## Version
 
 The current version of InstructPrompt is `0.1.0`.
```

