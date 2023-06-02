# Comparing `tmp/strategais-0.2.5.tar.gz` & `tmp/strategais-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strategais-0.2.5.tar", last modified: Thu Jun  1 21:53:24 2023, max compression
+gzip compressed data, was "strategais-0.2.6.tar", last modified: Fri Jun  2 13:52:46 2023, max compression
```

## Comparing `strategais-0.2.5.tar` & `strategais-0.2.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 21:53:24.259669 strategais-0.2.5/
--rw-r--r--   0 collin     (501) staff       (20)     1066 2023-05-26 03:15:25.000000 strategais-0.2.5/LICENSE
--rw-r--r--   0 collin     (501) staff       (20)     1305 2023-06-01 21:53:24.259458 strategais-0.2.5/PKG-INFO
--rw-r--r--   0 collin     (501) staff       (20)     1096 2023-06-01 21:27:39.000000 strategais-0.2.5/README.md
--rw-r--r--   0 collin     (501) staff       (20)       38 2023-06-01 21:53:24.259721 strategais-0.2.5/setup.cfg
--rw-r--r--   0 collin     (501) staff       (20)     1411 2023-06-01 21:52:44.000000 strategais-0.2.5/setup.py
-drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 21:53:24.257855 strategais-0.2.5/strategais/
--rw-r--r--   0 collin     (501) staff       (20)       78 2023-06-01 03:43:48.000000 strategais-0.2.5/strategais/__init__.py
--rw-r--r--   0 collin     (501) staff       (20)     4355 2023-06-01 21:52:25.000000 strategais-0.2.5/strategais/__main__.py
--rw-r--r--   0 collin     (501) staff       (20)      368 2023-05-31 04:51:38.000000 strategais-0.2.5/strategais/llm_tools.py
--rw-r--r--   0 collin     (501) staff       (20)     2280 2023-05-31 04:07:36.000000 strategais-0.2.5/strategais/save_tools.py
-drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 21:53:24.258866 strategais-0.2.5/strategais/templates/
--rw-r--r--   0 collin     (501) staff       (20)    18358 2023-06-01 03:39:47.000000 strategais-0.2.5/strategais/templates/index.html
-drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-01 21:53:24.258744 strategais-0.2.5/strategais.egg-info/
--rw-r--r--   0 collin     (501) staff       (20)     1305 2023-06-01 21:53:24.000000 strategais-0.2.5/strategais.egg-info/PKG-INFO
--rw-r--r--   0 collin     (501) staff       (20)      322 2023-06-01 21:53:24.000000 strategais-0.2.5/strategais.egg-info/SOURCES.txt
--rw-r--r--   0 collin     (501) staff       (20)        1 2023-06-01 21:53:24.000000 strategais-0.2.5/strategais.egg-info/dependency_links.txt
--rw-r--r--   0 collin     (501) staff       (20)      463 2023-06-01 21:53:24.000000 strategais-0.2.5/strategais.egg-info/requires.txt
--rw-r--r--   0 collin     (501) staff       (20)       11 2023-06-01 21:53:24.000000 strategais-0.2.5/strategais.egg-info/top_level.txt
+drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-02 13:52:46.840149 strategais-0.2.6/
+-rw-r--r--   0 collin     (501) staff       (20)     1066 2023-05-26 03:15:25.000000 strategais-0.2.6/LICENSE
+-rw-r--r--   0 collin     (501) staff       (20)     1305 2023-06-02 13:52:46.839982 strategais-0.2.6/PKG-INFO
+-rw-r--r--   0 collin     (501) staff       (20)     1096 2023-06-02 03:54:08.000000 strategais-0.2.6/README.md
+-rw-r--r--   0 collin     (501) staff       (20)       38 2023-06-02 13:52:46.840204 strategais-0.2.6/setup.cfg
+-rw-r--r--   0 collin     (501) staff       (20)     1459 2023-06-02 12:21:36.000000 strategais-0.2.6/setup.py
+drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-02 13:52:46.836483 strategais-0.2.6/strategais/
+-rw-r--r--   0 collin     (501) staff       (20)       78 2023-06-01 03:43:48.000000 strategais-0.2.6/strategais/__init__.py
+-rw-r--r--   0 collin     (501) staff       (20)     4679 2023-06-02 12:49:21.000000 strategais-0.2.6/strategais/__main__.py
+-rw-r--r--   0 collin     (501) staff       (20)      368 2023-05-31 04:51:38.000000 strategais-0.2.6/strategais/llm_tools.py
+-rw-r--r--   0 collin     (501) staff       (20)     2280 2023-05-31 04:07:36.000000 strategais-0.2.6/strategais/save_tools.py
+drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-02 13:52:46.838104 strategais-0.2.6/strategais/templates/
+-rw-r--r--   0 collin     (501) staff       (20)    18358 2023-06-01 03:39:47.000000 strategais-0.2.6/strategais/templates/index.html
+drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-02 13:52:46.837457 strategais-0.2.6/strategais.egg-info/
+-rw-r--r--   0 collin     (501) staff       (20)     1305 2023-06-02 13:52:46.000000 strategais-0.2.6/strategais.egg-info/PKG-INFO
+-rw-r--r--   0 collin     (501) staff       (20)      322 2023-06-02 13:52:46.000000 strategais-0.2.6/strategais.egg-info/SOURCES.txt
+-rw-r--r--   0 collin     (501) staff       (20)        1 2023-06-02 13:52:46.000000 strategais-0.2.6/strategais.egg-info/dependency_links.txt
+-rw-r--r--   0 collin     (501) staff       (20)      463 2023-06-02 13:52:46.000000 strategais-0.2.6/strategais.egg-info/requires.txt
+-rw-r--r--   0 collin     (501) staff       (20)       11 2023-06-02 13:52:46.000000 strategais-0.2.6/strategais.egg-info/top_level.txt
```

### Comparing `strategais-0.2.5/LICENSE` & `strategais-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `strategais-0.2.5/PKG-INFO` & `strategais-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: strategais
-Version: 0.2.5
+Version: 0.2.6
 Summary: A Python library for deploying large language models (LLMs) in local environments.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Strategais
 
 ## 🚀 Quick Install
 
 ```pip install strategais```
 
 Then run 
 
-```python -m strategais -t Hello -p 8181 --env prod.env```
+```python -m strategais -t Hello -p 8181 --env main.env```
 
 ## Additional Flags
 
 | Short Flag | Long Flag | Default Value | Description |
 |------------|-----------|---------------|-------------|
 | -t | --title | 'Strategais Server' | The title of the server. |
 | -d | --description | 'Strategais Server' | The description of the server. |
```

### Comparing `strategais-0.2.5/README.md` & `strategais-0.2.6/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 ## 🚀 Quick Install
 
 ```pip install strategais```
 
 Then run 
 
-```python -m strategais -t Hello -p 8181 --env prod.env```
+```python -m strategais -t Hello -p 8181 --env main.env```
 
 ## Additional Flags
 
 | Short Flag | Long Flag | Default Value | Description |
 |------------|-----------|---------------|-------------|
 | -t | --title | 'Strategais Server' | The title of the server. |
 | -d | --description | 'Strategais Server' | The description of the server. |
```

### Comparing `strategais-0.2.5/setup.py` & `strategais-0.2.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='strategais',
-    version='0.2.5', 
+    version='0.2.6', 
     description='A Python library for deploying large language models (LLMs) in local environments.',
     long_description=long_description,
     long_description_content_type="text/markdown", 
     packages=find_packages(),
-    package_data={'strategais': ['templates/*.html']},
+    package_data={'strategais': ['templates/*.html', 'static/*.js', 'static/*.css' , 'models/*.sav']},
     install_requires=[
         'fastapi',
         'fastapi_utils',
         'uvicorn',
         'starlette',
         'websockets',
         'flask',
```

### Comparing `strategais-0.2.5/strategais/__main__.py` & `strategais-0.2.6/strategais/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import io
 import importlib.util
 from .save_tools import *
 from .llm_tools import *
 import json
 import asyncio
 import uvicorn
+import pkg_resources
 
 from fastapi import FastAPI, Request, WebSocket  # ,Response, Body, Form,
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.responses import HTMLResponse, RedirectResponse
 from fastapi.staticfiles import StaticFiles
 from fastapi.templating import Jinja2Templates
 from fastapi.openapi.docs import (
@@ -58,17 +59,26 @@
 if args.llm:
     spec = importlib.util.spec_from_file_location("llm", args.llm)
     llm_module = importlib.util.module_from_spec(spec)
     spec.loader.exec_module(llm_module)
     chatbot = llm_module.main_chat()
 else:
     def main_chat(question):
-        from transformers.tools import HfAgent
-        agent = HfAgent("https://api-inference.huggingface.co/models/OpenAssistant/oasst-sft-4-pythia-12b-epoch-3.5")
-        return agent.run(question)
+        models_dir = pkg_resources.resource_filename('strategais', 'models')
+        model_file = 'model.sav'
+        tokenizer_file = 'tokenizer.sav'
+        model = load_model(f'{models_dir}/{model_file}')
+        tokenizer = load_tokenizer(f'{models_dir}/{tokenizer_file}')
+
+        input_text = question
+
+        input_ids = tokenizer(input_text, return_tensors="pt").input_ids.to('cpu')
+
+        outputs = model.generate(input_ids, max_length=10000)
+        return tokenizer.decode(outputs[0], skip_special_tokens=True)
     
     chatbot = main_chat
 
 server = FastAPI(
     title=args.title,
     description=args.description)
 
@@ -109,16 +119,14 @@
     while True:
         question = await websocket.receive_text()
         await websocket.send_text(chatbot(question))
 
 import urllib3
 urllib3.disable_warnings()
 
-import pkg_resources
-
 template_path = pkg_resources.resource_filename('strategais', 'templates')
 templates = Jinja2Templates(directory=template_path)
 
 @server.get("/chat", response_class=HTMLResponse,
             tags=['Chat'],
             summary="Chat Home Page",
             description="Chat Home Page")
```

### Comparing `strategais-0.2.5/strategais/save_tools.py` & `strategais-0.2.6/strategais/save_tools.py`

 * *Files identical despite different names*

### Comparing `strategais-0.2.5/strategais/templates/index.html` & `strategais-0.2.6/strategais/templates/index.html`

 * *Files identical despite different names*

### Comparing `strategais-0.2.5/strategais.egg-info/PKG-INFO` & `strategais-0.2.6/strategais.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: strategais
-Version: 0.2.5
+Version: 0.2.6
 Summary: A Python library for deploying large language models (LLMs) in local environments.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Strategais
 
 ## 🚀 Quick Install
 
 ```pip install strategais```
 
 Then run 
 
-```python -m strategais -t Hello -p 8181 --env prod.env```
+```python -m strategais -t Hello -p 8181 --env main.env```
 
 ## Additional Flags
 
 | Short Flag | Long Flag | Default Value | Description |
 |------------|-----------|---------------|-------------|
 | -t | --title | 'Strategais Server' | The title of the server. |
 | -d | --description | 'Strategais Server' | The description of the server. |
```

