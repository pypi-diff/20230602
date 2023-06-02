# Comparing `tmp/chater-1.0.2.tar.gz` & `tmp/chater-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chater-1.0.2.tar", last modified: Fri Jun  2 16:28:37 2023, max compression
+gzip compressed data, was "chater-1.0.3.tar", last modified: Fri Jun  2 16:38:55 2023, max compression
```

## Comparing `chater-1.0.2.tar` & `chater-1.0.3.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:28:37.395574 chater-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-02 16:28:27.000000 chater-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-02 16:28:37.395574 chater-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-02 16:28:27.000000 chater-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:28:37.391574 chater-1.0.2/chater/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-02 16:28:27.000000 chater-1.0.2/chater/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:28:37.395574 chater-1.0.2/chater/api/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-02 16:28:27.000000 chater-1.0.2/chater/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:28:37.395574 chater-1.0.2/chater/api/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-02 16:28:27.000000 chater-1.0.2/chater/api/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-02 16:28:27.000000 chater-1.0.2/chater/api/abstract/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-02 16:28:27.000000 chater-1.0.2/chater/api/abstract/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-06-02 16:28:27.000000 chater-1.0.2/chater/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-02 16:28:27.000000 chater-1.0.2/chater/api/billing.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-02 16:28:27.000000 chater-1.0.2/chater/api/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-02 16:28:27.000000 chater-1.0.2/chater/api/stream_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-02 16:28:27.000000 chater-1.0.2/chater/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:28:37.391574 chater-1.0.2/chater.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-02 16:28:37.000000 chater-1.0.2/chater.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-02 16:28:37.000000 chater-1.0.2/chater.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 16:28:37.000000 chater-1.0.2/chater.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 16:28:37.000000 chater-1.0.2/chater.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-02 16:28:37.000000 chater-1.0.2/chater.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 16:28:37.395574 chater-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-02 16:28:27.000000 chater-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:38:55.888944 chater-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-02 16:38:46.000000 chater-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-02 16:38:55.888944 chater-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-02 16:38:46.000000 chater-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 16:38:55.888944 chater-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-02 16:38:46.000000 chater-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:38:55.888944 chater-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:38:55.888944 chater-1.0.3/src/chater/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-02 16:38:46.000000 chater-1.0.3/src/chater/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:38:55.888944 chater-1.0.3/src/chater/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-02 16:38:46.000000 chater-1.0.3/src/chater/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:38:55.888944 chater-1.0.3/src/chater/api/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-02 16:38:46.000000 chater-1.0.3/src/chater/api/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-02 16:38:46.000000 chater-1.0.3/src/chater/api/abstract/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-02 16:38:46.000000 chater-1.0.3/src/chater/api/abstract/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-06-02 16:38:46.000000 chater-1.0.3/src/chater/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-02 16:38:46.000000 chater-1.0.3/src/chater/api/billing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-02 16:38:46.000000 chater-1.0.3/src/chater/api/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-02 16:38:46.000000 chater-1.0.3/src/chater/api/stream_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-02 16:38:46.000000 chater-1.0.3/src/chater/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:38:55.888944 chater-1.0.3/src/chater.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-02 16:38:55.000000 chater-1.0.3/src/chater.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-02 16:38:55.000000 chater-1.0.3/src/chater.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 16:38:55.000000 chater-1.0.3/src/chater.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 16:38:55.000000 chater-1.0.3/src/chater.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-02 16:38:55.000000 chater-1.0.3/src/chater.egg-info/top_level.txt
```

### Comparing `chater-1.0.2/LICENSE` & `chater-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chater-1.0.2/PKG-INFO` & `chater-1.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 Metadata-Version: 2.1
 Name: chater
-Version: 1.0.2
+Version: 1.0.3
 Summary: Using ChatGPT in Python
 Author: Sricor
 Author-email: josricor@outlook.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Chatbot
+# chater
 
 Using ChatGPT in Python.
 
 Use the same format for the messages as you would for the [official OpenAI API](https://platform.openai.com/docs/api-reference/chat).
 
 ## Installation
 
 Download or clone this GitHub repo  
 install requirements with:
 
 ```bash
 pip install chater
 ```
 
-## A Simple Example
+## Simple Example
 ### 1. Accessing GPT through an API KEY (This will consume API quota).
 ```python
 import chatbot
 
 chatbot.api_key = ''
 chatbot.StreamCompletion.create('Hello world!')
 
 ```
+
+
 ### 2. Accessing GPT through an Access Token (Free 3.5).
 ```python
 import chatbot
 
 auth = chatbot.Auth('email', 'password')
 chatbot.api_key = auth.get_access_token()
 chatbot.StreamCompletion.create('Hello world!')
```

### Comparing `chater-1.0.2/README.md` & `chater-1.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,33 @@
-# Chatbot
+# chater
 
 Using ChatGPT in Python.
 
 Use the same format for the messages as you would for the [official OpenAI API](https://platform.openai.com/docs/api-reference/chat).
 
 ## Installation
 
 Download or clone this GitHub repo  
 install requirements with:
 
 ```bash
 pip install chater
 ```
 
-## A Simple Example
+## Simple Example
 ### 1. Accessing GPT through an API KEY (This will consume API quota).
 ```python
 import chatbot
 
 chatbot.api_key = ''
 chatbot.StreamCompletion.create('Hello world!')
 
 ```
+
+
 ### 2. Accessing GPT through an Access Token (Free 3.5).
 ```python
 import chatbot
 
 auth = chatbot.Auth('email', 'password')
 chatbot.api_key = auth.get_access_token()
 chatbot.StreamCompletion.create('Hello world!')
```

### Comparing `chater-1.0.2/chater/api/abstract/client.py` & `chater-1.0.3/src/chater/api/abstract/client.py`

 * *Files identical despite different names*

### Comparing `chater-1.0.2/chater/api/abstract/typings.py` & `chater-1.0.3/src/chater/api/abstract/typings.py`

 * *Files identical despite different names*

### Comparing `chater-1.0.2/chater/api/auth.py` & `chater-1.0.3/src/chater/api/auth.py`

 * *Files identical despite different names*

### Comparing `chater-1.0.2/chater/api/billing.py` & `chater-1.0.3/src/chater/api/billing.py`

 * *Files identical despite different names*

### Comparing `chater-1.0.2/chater/api/stream_completion.py` & `chater-1.0.3/src/chater/api/stream_completion.py`

 * *Files identical despite different names*

### Comparing `chater-1.0.2/chater.egg-info/PKG-INFO` & `chater-1.0.3/src/chater.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 Metadata-Version: 2.1
 Name: chater
-Version: 1.0.2
+Version: 1.0.3
 Summary: Using ChatGPT in Python
 Author: Sricor
 Author-email: josricor@outlook.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Chatbot
+# chater
 
 Using ChatGPT in Python.
 
 Use the same format for the messages as you would for the [official OpenAI API](https://platform.openai.com/docs/api-reference/chat).
 
 ## Installation
 
 Download or clone this GitHub repo  
 install requirements with:
 
 ```bash
 pip install chater
 ```
 
-## A Simple Example
+## Simple Example
 ### 1. Accessing GPT through an API KEY (This will consume API quota).
 ```python
 import chatbot
 
 chatbot.api_key = ''
 chatbot.StreamCompletion.create('Hello world!')
 
 ```
+
+
 ### 2. Accessing GPT through an Access Token (Free 3.5).
 ```python
 import chatbot
 
 auth = chatbot.Auth('email', 'password')
 chatbot.api_key = auth.get_access_token()
 chatbot.StreamCompletion.create('Hello world!')
```

