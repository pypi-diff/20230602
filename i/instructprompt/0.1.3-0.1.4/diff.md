# Comparing `tmp/instructprompt-0.1.3.tar.gz` & `tmp/instructprompt-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instructprompt-0.1.3.tar", max compression
+gzip compressed data, was "instructprompt-0.1.4.tar", max compression
```

## Comparing `instructprompt-0.1.3.tar` & `instructprompt-0.1.4.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     2260 2023-06-02 02:49:53.992167 instructprompt-0.1.3/README.md
--rw-r--r--   0        0        0      640 2023-06-02 02:57:08.994681 instructprompt-0.1.3/instructprompt/__init__.py
--rw-r--r--   0        0        0      301 2023-06-02 02:57:15.577607 instructprompt-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2752 1970-01-01 00:00:00.000000 instructprompt-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2156 2023-06-02 03:00:39.063265 instructprompt-0.1.4/README.md
+-rw-r--r--   0        0        0      614 2023-06-02 03:01:15.542221 instructprompt-0.1.4/instructprompt/__init__.py
+-rw-r--r--   0        0        0      301 2023-06-02 03:01:19.747151 instructprompt-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2648 1970-01-01 00:00:00.000000 instructprompt-0.1.4/PKG-INFO
```

### Comparing `instructprompt-0.1.3/instructprompt/__init__.py` & `instructprompt-0.1.4/instructprompt/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-__version__ = '0.1.2'
+__version__ = '0.1.4'
 
 import chromadb
 
 chroma_client = chromadb.Client()
 collection = chroma_client.create_collection(name="user_instructprompt_collection")
 
 def add(instruction: str): 
     collection.add(
         documents=[instruction],
         ids=[str(id)]
     )
     print("✅ instruction added")
     return
 
-def list_instructions(): 
+def list(): 
     return collection.get()["documents"]
 
-def query_instructions(query: str): 
+def query(query: str): 
     results = collection.query(
         query_texts=[query],
         n_results=5
     )
     instructions = ""
     for document in results["documents"][0]: 
         instructions += document + "\n"
```

### Comparing `instructprompt-0.1.3/PKG-INFO` & `instructprompt-0.1.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instructprompt
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: krrishdholakia
 Author-email: krrishdholakia@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -27,49 +27,49 @@
 
 Once installed, you can import it into your python project by running the following:
 
 `import InstructPrompt`
 
 ## Using InstructPrompt
 
-InstructPrompt provides 3 main functions: `add()`, `list_instructions()`, and `query_instructions()`.
+InstructPrompt provides 3 main functions: `add()`, `list()`, and `query()`.
 
 ### add()
 
 The `add()` function takes in an instruction as a string and adds it to the collection. It uses ChromaDB to store the instruction and assigns it a unique id. It returns a confirmation message once the instruction is successfully added. 
 
 ```
 import InstructPrompt
 
 instruction = "Please provide the customer's name and order number."
 
 InstructPrompt.add(instruction)
 ```
 
-### list_instructions()
+### list()
 
-The `list_instructions()` function returns a list of all the stored instructions in the collection. 
+The `list()` function returns a list of all the stored instructions in the collection. 
 
 ```
 import InstructPrompt
 
-instructions = InstructPrompt.list_instructions()
+instructions = InstructPrompt.list()
 print(instructions) # Outputs a list of all the stored instructions
 ```
 
-### query_instructions()
+### query()
 
-The `query_instructions()` function takes in a query as a string and returns a list of instructions that match the query. It uses ChromaDB to perform the query and returns up to 5 matching instructions.
+The `query()` function takes in a query as a string and returns a list of instructions that match the query. It uses ChromaDB to perform the query and returns up to 5 matching instructions.
 
 ```
 import InstructPrompt
 
 query = "How do I reset my password?"
 
-instructions = InstructPrompt.query_instructions(query)
+instructions = InstructPrompt.query(query)
 print(instructions) # Outputs a list of instructions that match the query
 ```
 
 ## Version
 
 The current version of InstructPrompt is `0.1.0`.
```

