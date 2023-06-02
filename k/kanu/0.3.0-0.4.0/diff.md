# Comparing `tmp/kanu-0.3.0.tar.gz` & `tmp/kanu-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kanu-0.3.0.tar", last modified: Tue May 30 07:11:15 2023, max compression
+gzip compressed data, was "kanu-0.4.0.tar", last modified: Fri Jun  2 03:37:51 2023, max compression
```

## Comparing `kanu-0.3.0.tar` & `kanu-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-05-30 07:11:15.489367 kanu-0.3.0/
--rw-r--r--   0 sbslee     (501) staff       (20)     1080 2023-05-30 07:11:03.000000 kanu-0.3.0/LICENSE
--rw-r--r--   0 sbslee     (501) staff       (20)      737 2023-05-30 07:11:15.489215 kanu-0.3.0/PKG-INFO
--rw-r--r--   0 sbslee     (501) staff       (20)      421 2023-05-30 07:11:03.000000 kanu-0.3.0/README.md
-drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-05-30 07:11:15.488401 kanu-0.3.0/kanu/
--rw-r--r--   0 sbslee     (501) staff       (20)        0 2023-05-30 07:11:03.000000 kanu-0.3.0/kanu/__init__.py
--rw-r--r--   0 sbslee     (501) staff       (20)     5278 2023-05-30 07:11:03.000000 kanu-0.3.0/kanu/__main__.py
--rw-r--r--   0 sbslee     (501) staff       (20)     1847 2023-05-30 07:11:03.000000 kanu-0.3.0/kanu/chatgpt.py
--rw-r--r--   0 sbslee     (501) staff       (20)     6858 2023-05-30 07:11:03.000000 kanu-0.3.0/kanu/docgpt.py
--rw-r--r--   0 sbslee     (501) staff       (20)      828 2023-05-30 07:11:03.000000 kanu-0.3.0/kanu/utils.py
--rw-r--r--   0 sbslee     (501) staff       (20)       21 2023-05-30 07:11:03.000000 kanu-0.3.0/kanu/version.py
-drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-05-30 07:11:15.489021 kanu-0.3.0/kanu.egg-info/
--rw-r--r--   0 sbslee     (501) staff       (20)      737 2023-05-30 07:11:15.000000 kanu-0.3.0/kanu.egg-info/PKG-INFO
--rw-r--r--   0 sbslee     (501) staff       (20)      264 2023-05-30 07:11:15.000000 kanu-0.3.0/kanu.egg-info/SOURCES.txt
--rw-r--r--   0 sbslee     (501) staff       (20)        1 2023-05-30 07:11:15.000000 kanu-0.3.0/kanu.egg-info/dependency_links.txt
--rw-r--r--   0 sbslee     (501) staff       (20)       44 2023-05-30 07:11:15.000000 kanu-0.3.0/kanu.egg-info/entry_points.txt
--rw-r--r--   0 sbslee     (501) staff       (20)        5 2023-05-30 07:11:15.000000 kanu-0.3.0/kanu.egg-info/top_level.txt
--rw-r--r--   0 sbslee     (501) staff       (20)       38 2023-05-30 07:11:15.489413 kanu-0.3.0/setup.cfg
--rw-r--r--   0 sbslee     (501) staff       (20)      627 2023-05-30 07:11:03.000000 kanu-0.3.0/setup.py
+drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-06-02 03:37:51.877966 kanu-0.4.0/
+-rw-r--r--   0 sbslee     (501) staff       (20)     1080 2023-06-02 03:37:35.000000 kanu-0.4.0/LICENSE
+-rw-r--r--   0 sbslee     (501) staff       (20)      853 2023-06-02 03:37:51.877811 kanu-0.4.0/PKG-INFO
+-rw-r--r--   0 sbslee     (501) staff       (20)      537 2023-06-02 03:37:35.000000 kanu-0.4.0/README.md
+drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-06-02 03:37:51.876967 kanu-0.4.0/kanu/
+-rw-r--r--   0 sbslee     (501) staff       (20)        0 2023-06-02 03:37:35.000000 kanu-0.4.0/kanu/__init__.py
+-rw-r--r--   0 sbslee     (501) staff       (20)     7176 2023-06-02 03:37:35.000000 kanu-0.4.0/kanu/__main__.py
+-rw-r--r--   0 sbslee     (501) staff       (20)     1959 2023-06-02 03:37:35.000000 kanu-0.4.0/kanu/chatgpt.py
+-rw-r--r--   0 sbslee     (501) staff       (20)     7877 2023-06-02 03:37:35.000000 kanu-0.4.0/kanu/docgpt.py
+-rw-r--r--   0 sbslee     (501) staff       (20)      844 2023-06-02 03:37:35.000000 kanu-0.4.0/kanu/utils.py
+-rw-r--r--   0 sbslee     (501) staff       (20)       21 2023-06-02 03:37:35.000000 kanu-0.4.0/kanu/version.py
+drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-06-02 03:37:51.877624 kanu-0.4.0/kanu.egg-info/
+-rw-r--r--   0 sbslee     (501) staff       (20)      853 2023-06-02 03:37:51.000000 kanu-0.4.0/kanu.egg-info/PKG-INFO
+-rw-r--r--   0 sbslee     (501) staff       (20)      264 2023-06-02 03:37:51.000000 kanu-0.4.0/kanu.egg-info/SOURCES.txt
+-rw-r--r--   0 sbslee     (501) staff       (20)        1 2023-06-02 03:37:51.000000 kanu-0.4.0/kanu.egg-info/dependency_links.txt
+-rw-r--r--   0 sbslee     (501) staff       (20)       44 2023-06-02 03:37:51.000000 kanu-0.4.0/kanu.egg-info/entry_points.txt
+-rw-r--r--   0 sbslee     (501) staff       (20)        5 2023-06-02 03:37:51.000000 kanu-0.4.0/kanu.egg-info/top_level.txt
+-rw-r--r--   0 sbslee     (501) staff       (20)       38 2023-06-02 03:37:51.878024 kanu-0.4.0/setup.cfg
+-rw-r--r--   0 sbslee     (501) staff       (20)      627 2023-06-02 03:37:35.000000 kanu-0.4.0/setup.py
```

### Comparing `kanu-0.3.0/LICENSE` & `kanu-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kanu-0.3.0/kanu/chatgpt.py` & `kanu-0.4.0/kanu/chatgpt.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import tkinter as tk
 
 import openai
 
 class ChatGPT:
-    def __init__(self, kanu, openai_key, model):
+    def __init__(self, kanu, openai_key, model, temperature, prompt):
         self.kanu = kanu
         self.model = model
+        self.temperature = temperature
+        self.prompt = prompt
         openai.api_key = openai_key
 
     def run(self):
         self.kanu.container.pack_forget()
         self.kanu.container = tk.Frame(self.kanu.root)
         self.kanu.container.pack()
         l = tk.Label(self.kanu.container, text="ChatGPT")
@@ -24,19 +26,20 @@
         b = tk.Button(self.kanu.container, text="Clear", command=lambda: self.clear_session())
         b.grid(row=3, column=1)
         b = tk.Button(self.kanu.container, text="Go back", command=lambda: self.kanu.config_chatgpt())
         b.grid(row=3, column=2)
 
     def send_message(self, entry):
         if not self.messages:
-            self.messages.append({"role": "system", "content": "You are a helpful assistant."})
+            self.messages.append({"role": "system", "content": self.prompt})
         self.messages += [{"role": "user", "content": entry.get()}]
         bot_response = openai.ChatCompletion.create(
             model=self.model,
             messages=self.messages,
+            temperature=self.temperature,
         )
         response = bot_response["choices"][0]["message"]["content"]
         self.messages += [{"role": "assistant", "content": response}]
         self.session.insert(tk.END, "You: " + entry.get() + "\n")
         self.session.insert(tk.END, f"Bot: " + response + "\n")
         entry.delete(0, tk.END)
```

### Comparing `kanu-0.3.0/kanu/docgpt.py` & `kanu-0.4.0/kanu/docgpt.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from tkinter import filedialog
 
 from langchain.embeddings.openai import OpenAIEmbeddings
 from langchain.text_splitter import RecursiveCharacterTextSplitter
 from langchain.vectorstores import Chroma
 from langchain.chat_models import ChatOpenAI
 from langchain.chains import RetrievalQA
+from langchain.prompts import PromptTemplate
 
 from langchain.document_loaders import (
     TextLoader,
     PDFMinerLoader,
     UnstructuredWordDocumentLoader
 )
 
@@ -18,66 +19,83 @@
 
 DOCUMENT_LOADERS = {
     ".txt": TextLoader,
     ".pdf": PDFMinerLoader,
     ".doc": UnstructuredWordDocumentLoader,
     ".docx": UnstructuredWordDocumentLoader,
 }
-
 class DocGPT:
-    def __init__(self, kanu, openai_key, model):
+    def __init__(self, kanu, openai_key, model, prompt):
         self.kanu = kanu
         self.model = model
+        self.prompt = prompt
         os.environ["OPENAI_API_KEY"] = openai_key
 
     def run(self):
         self.kanu.container.pack_forget()
         self.kanu.container = tk.Frame(self.kanu.root)
         self.kanu.container.pack()
         l = tk.Label(self.kanu.container, text="DocGPT")
         l.grid(row=0, column=0, columnspan=3)
         b = tk.Button(self.kanu.container, text="Go back", command=lambda: self.kanu.config_docgpt())
         b.grid(row=1, column=0)
         b = tk.Button(self.kanu.container, text="Reload", command=lambda: self.run())
         b.grid(row=1, column=2)
-        l = tk.Message(self.kanu.container, width=300, text="Option 1. Create a new database")
-        l.grid(row=2, column=0, columnspan=3)
+        m = tk.Message(self.kanu.container, width=300, text="Option 1. Create a new database")
+        m.grid(row=2, column=0, columnspan=3)
         l = tk.Label(self.kanu.container, text="Document ⓘ:")
         Tooltip(l, "Directory containing documents for the database.")
         l.grid(row=3, column=0) 
         self.document_label = tk.Label(self.kanu.container, text="Not selected", fg="red")
         self.document_label.grid(row=3, column=1)
         b = tk.Button(self.kanu.container, text="Browse", command=self.specify_document_directory)
         b.grid(row=3, column=2)
         l = tk.Label(self.kanu.container, text="Database ⓘ:")
         Tooltip(l, "Directory where the database will be stored.")
         l.grid(row=4, column=0)       
         self.new_database_label = tk.Label(self.kanu.container, text="Not selected", fg="red")
         self.new_database_label.grid(row=4, column=1)
         b = tk.Button(self.kanu.container, text="Browse", command=self.specify_new_database_directory)
         b.grid(row=4, column=2)
+        l = tk.Label(self.kanu.container, text="Chunk size ⓘ:")
+        Tooltip(l, "The maximum number of characters in each chunk.")
+        l.grid(row=5, column=0)
+        self.chunk_size = tk.IntVar(self.kanu.container, value=1000)
+        e = tk.Entry(self.kanu.container, textvariable=self.chunk_size)
+        e.grid(row=5, column=1, columnspan=2)
+        l = tk.Label(self.kanu.container, text="Chunk overlap ⓘ:")
+        Tooltip(l, "The number of overlapping characters between adjacent chunks.")
+        l.grid(row=6, column=0)
+        self.chunk_overlap = tk.IntVar(self.kanu.container, value=50)
+        e = tk.Entry(self.kanu.container, textvariable=self.chunk_overlap)
+        e.grid(row=6, column=1, columnspan=2)
         self.option1_button = tk.Button(self.kanu.container, text="Go with Option 1", command=self.go_with_option1)
-        self.option1_button.grid(row=5, column=0, columnspan=3)
+        self.option1_button.grid(row=7, column=0, columnspan=3)
         self.option1_button["state"] = tk.DISABLED
-        l = tk.Message(self.kanu.container, width=300, text="Option 2. Use an existing database")
-        l.grid(row=6, column=0, columnspan=3)
+        m = tk.Message(self.kanu.container, width=300, text="Option 2. Use an existing database")
+        m.grid(row=8, column=0, columnspan=3)
         l = tk.Label(self.kanu.container, text="Database ⓘ:")
         Tooltip(l, "Directory where the database is stored.")
-        l.grid(row=7, column=0)
+        l.grid(row=9, column=0)
         self.old_database_label = tk.Label(self.kanu.container, text="Not selected", fg="red")
-        self.old_database_label.grid(row=7, column=1)
+        self.old_database_label.grid(row=9, column=1)
         b = tk.Button(self.kanu.container, text="Browse", command=self.specify_old_database_directory)
-        b.grid(row=7, column=2)
+        b.grid(row=9, column=2)
         self.option2_button = tk.Button(self.kanu.container, text="Go with Option 2", command=self.go_with_option2)
-        self.option2_button.grid(row=8, column=0, columnspan=3)
+        self.option2_button.grid(row=10, column=0, columnspan=3)
         self.option2_button["state"] = tk.DISABLED
 
     def query(self):
         self.db = Chroma(persist_directory=self.database_directory, embedding_function=OpenAIEmbeddings())
-        self.qa = RetrievalQA.from_chain_type(llm=ChatOpenAI(model_name=self.model), chain_type="stuff", retriever=self.db.as_retriever())
+        self.qa = RetrievalQA.from_chain_type(
+            llm=ChatOpenAI(model_name=self.model),
+            chain_type="stuff",
+            retriever=self.db.as_retriever(),
+            chain_type_kwargs={"prompt": PromptTemplate(template=self.prompt, input_variables=["context", "question"])}
+        )
         self.kanu.container.pack_forget()
         self.kanu.container = tk.Frame(self.kanu.root)
         self.kanu.container.pack()
         l = tk.Label(self.kanu.container, text="DocGPT")
         l.grid(row=0, column=0, columnspan=3)    
         self.session = tk.Text(self.kanu.container, width=70, height=20)
         self.session.grid(row=1, column=0, columnspan=3)
@@ -103,15 +121,15 @@
                 file_path = os.path.join(root, file)
                 file_ext = os.path.splitext(file_path)[1]
                 if file_ext not in DOCUMENT_LOADERS:
                     continue
                 loader = DOCUMENT_LOADERS[file_ext](file_path)
                 document = loader.load()[0]
                 documents.append(document)
-        text_splitter = RecursiveCharacterTextSplitter(chunk_size=1000, chunk_overlap=50)
+        text_splitter = RecursiveCharacterTextSplitter(chunk_size=self.chunk_size.get(), chunk_overlap=self.chunk_overlap.get())
         texts = text_splitter.split_documents(documents)
         db = Chroma.from_documents(texts, OpenAIEmbeddings(), persist_directory=self.database_directory)
         db.add_documents(texts)    
         db.persist()
         db = None
         self.query()
```

### Comparing `kanu-0.3.0/kanu/utils.py` & `kanu-0.4.0/kanu/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,14 @@
     def show_tooltip(self, event):
         x, y, _, _ = self.widget.bbox("insert")
         x += self.widget.winfo_rootx() + 25
         y += self.widget.winfo_rooty() + 25
         self.tooltip = tk.Toplevel(self.widget)
         self.tooltip.wm_overrideredirect(True)
         self.tooltip.wm_geometry(f"+{x}+{y}")
-        l = tk.Label(self.tooltip, text=self.text, background="#ffffe0", relief="solid", borderwidth=1)
+        l = tk.Label(self.tooltip, text=self.text, background="#ffffe0", relief="solid", borderwidth=1, wraplength=400)
         l.pack()
 
     def hide_tooltip(self, event):
         if self.tooltip:
             self.tooltip.destroy()
             self.tooltip = None
```

### Comparing `kanu-0.3.0/setup.py` & `kanu-0.4.0/setup.py`

 * *Files identical despite different names*

