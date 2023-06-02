# Comparing `tmp/chatdocs-0.0.2.tar.gz` & `tmp/chatdocs-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatdocs-0.0.2.tar", last modified: Fri Jun  2 20:40:00 2023, max compression
+gzip compressed data, was "chatdocs-0.0.3.tar", last modified: Fri Jun  2 21:12:53 2023, max compression
```

## Comparing `chatdocs-0.0.2.tar` & `chatdocs-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-02 20:40:00.657853 chatdocs-0.0.2/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      951 2023-06-02 20:40:00.657853 chatdocs-0.0.2/PKG-INFO
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2067 2023-06-02 19:31:02.000000 chatdocs-0.0.2/README.md
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-02 20:40:00.647853 chatdocs-0.0.2/chatdocs/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        0 2023-06-01 18:46:12.000000 chatdocs-0.0.2/chatdocs/__init__.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       29 2023-06-01 19:38:54.000000 chatdocs-0.0.2/chatdocs/__main__.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     6201 2023-06-02 17:41:03.000000 chatdocs-0.0.2/chatdocs/add.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     3061 2023-06-02 19:30:06.000000 chatdocs-0.0.2/chatdocs/chat.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      178 2023-06-02 17:43:46.000000 chatdocs-0.0.2/chatdocs/config.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      290 2023-06-02 20:37:18.000000 chatdocs-0.0.2/chatdocs/download.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2454 2023-06-02 11:45:11.000000 chatdocs-0.0.2/chatdocs/main.py
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-02 20:40:00.647853 chatdocs-0.0.2/chatdocs.egg-info/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      951 2023-06-02 20:40:00.000000 chatdocs-0.0.2/chatdocs.egg-info/PKG-INFO
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      375 2023-06-02 20:40:00.000000 chatdocs-0.0.2/chatdocs.egg-info/SOURCES.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-06-02 20:40:00.000000 chatdocs-0.0.2/chatdocs.egg-info/dependency_links.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       48 2023-06-02 20:40:00.000000 chatdocs-0.0.2/chatdocs.egg-info/entry_points.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-06-02 20:40:00.000000 chatdocs-0.0.2/chatdocs.egg-info/not-zip-safe
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      313 2023-06-02 20:40:00.000000 chatdocs-0.0.2/chatdocs.egg-info/requires.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        9 2023-06-02 20:40:00.000000 chatdocs-0.0.2/chatdocs.egg-info/top_level.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       38 2023-06-02 20:40:00.657853 chatdocs-0.0.2/setup.cfg
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1985 2023-06-02 20:39:50.000000 chatdocs-0.0.2/setup.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-02 21:12:53.507828 chatdocs-0.0.3/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     3994 2023-06-02 21:12:53.507828 chatdocs-0.0.3/PKG-INFO
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2279 2023-06-02 20:59:47.000000 chatdocs-0.0.3/README.md
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-02 21:12:53.507828 chatdocs-0.0.3/chatdocs/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        0 2023-06-01 18:46:12.000000 chatdocs-0.0.3/chatdocs/__init__.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       29 2023-06-01 19:38:54.000000 chatdocs-0.0.3/chatdocs/__main__.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     6201 2023-06-02 17:41:03.000000 chatdocs-0.0.3/chatdocs/add.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     3061 2023-06-02 19:30:06.000000 chatdocs-0.0.3/chatdocs/chat.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      178 2023-06-02 17:43:46.000000 chatdocs-0.0.3/chatdocs/config.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      290 2023-06-02 20:37:18.000000 chatdocs-0.0.3/chatdocs/download.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2454 2023-06-02 11:45:11.000000 chatdocs-0.0.3/chatdocs/main.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-02 21:12:53.507828 chatdocs-0.0.3/chatdocs.egg-info/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     3994 2023-06-02 21:12:53.000000 chatdocs-0.0.3/chatdocs.egg-info/PKG-INFO
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      375 2023-06-02 21:12:53.000000 chatdocs-0.0.3/chatdocs.egg-info/SOURCES.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-06-02 21:12:53.000000 chatdocs-0.0.3/chatdocs.egg-info/dependency_links.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       48 2023-06-02 21:12:53.000000 chatdocs-0.0.3/chatdocs.egg-info/entry_points.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-06-02 21:12:53.000000 chatdocs-0.0.3/chatdocs.egg-info/not-zip-safe
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      313 2023-06-02 21:12:53.000000 chatdocs-0.0.3/chatdocs.egg-info/requires.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        9 2023-06-02 21:12:53.000000 chatdocs-0.0.3/chatdocs.egg-info/top_level.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       38 2023-06-02 21:12:53.507828 chatdocs-0.0.3/setup.cfg
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1979 2023-06-02 21:12:20.000000 chatdocs-0.0.3/setup.py
```

### Comparing `chatdocs-0.0.2/README.md` & `chatdocs-0.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-# [ChatDocs](https://github.com/marella/chatdocs) [![PyPI](https://img.shields.io/pypi/v/chatdocs)](https://pypi.org/project/chatdocs/)
+# [ChatDocs](https://github.com/marella/chatdocs) [![PyPI](https://img.shields.io/pypi/v/chatdocs)](https://pypi.org/project/chatdocs/) [![tests](https://github.com/marella/chatdocs/actions/workflows/tests.yml/badge.svg)](https://github.com/marella/chatdocs/actions/workflows/tests.yml)
 
 Chat with your documents offline using AI. No data leaves your system. Internet connection is only required to install the tool and download the AI models.
 
-![Demo](docs/demo.png)
+![Demo](https://github.com/marella/chatdocs/raw/main/docs/demo.png)
 
-It is based on (PrivateGPT)[https://github.com/imartinez/privateGPT] but uses [C Transformers](https://github.com/marella/ctransformers) which supports more GGML models. It also supports [🤗 Transformers](https://github.com/huggingface/transformers).
+It is based on [PrivateGPT](https://github.com/imartinez/privateGPT) but uses [C Transformers](https://github.com/marella/ctransformers) which supports more GGML models. It also supports [🤗 Transformers](https://github.com/huggingface/transformers).
 
 ## Installation
 
 Install the tool using:
 
 ```sh
 pip install chatdocs
@@ -43,39 +43,39 @@
 ```sh
 chatdocs add --help
 chatdocs chat --help
 ```
 
 ### LLM
 
-By default it uses the [Wizard-Vicuna-7B-Uncensored-GGML](https://huggingface.co/TheBloke/Wizard-Vicuna-7B-Uncensored-GGML) model which can be changed using `--model` option:
+By default it uses the [Wizard-Vicuna-7B-Uncensored-GGML](https://huggingface.co/TheBloke/Wizard-Vicuna-7B-Uncensored-GGML) model which can be changed using the `--model` option:
 
 ```sh
 chatdocs chat --model TheBloke/MPT-7B-GGML --download
 ```
 
-> **Note:** `--download` option is only required when you use a model for the first time.
+> **Note:** The `--download` option is only required when you use a model for the first time.
 
 It can also be used with an existing local model file:
 
 ```sh
 chatdocs chat --model /path/to/mpt-7b-ggml.bin --model-type mpt
 ```
 
 ### LLM Provider
 
-By default it uses C Transformers as the LLM provider which can be changed to 🤗 Transformers using `--hf` option:
+By default it uses C Transformers as the LLM provider which can be changed to 🤗 Transformers using the `--hf` option:
 
 ```sh
 chatdocs chat --hf --model TheBloke/Wizard-Vicuna-7B-Uncensored-HF --download
 ```
 
 ### DB
 
-By default it stores the processed documents in `db` directory which can be changed using `--db` option:
+By default it stores the processed documents in `db` directory which can be changed using the `--db` option:
 
 ```sh
 chatdocs add documents --db /path/to/some/directory
 chatdocs chat --db /path/to/some/directory
 ```
 
 ## UI
```

### Comparing `chatdocs-0.0.2/chatdocs/add.py` & `chatdocs-0.0.3/chatdocs/add.py`

 * *Files identical despite different names*

### Comparing `chatdocs-0.0.2/chatdocs/chat.py` & `chatdocs-0.0.3/chatdocs/chat.py`

 * *Files identical despite different names*

### Comparing `chatdocs-0.0.2/chatdocs/main.py` & `chatdocs-0.0.3/chatdocs/main.py`

 * *Files identical despite different names*

### Comparing `chatdocs-0.0.2/setup.py` & `chatdocs-0.0.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 with open("README.md") as f:
     long_description = f.read()
 
 name = "chatdocs"
 
 setup(
     name=name,
-    version="0.0.2",
-    # description="Chat with your documents offline using AI.",
-    # long_description=long_description,
-    # long_description_content_type="text/markdown",
+    version="0.0.3",
+    description="Chat with your documents offline using AI.",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     author="Ravindra Marella",
     author_email="mv.ravindra007@gmail.com",
     url="https://github.com/marella/{}".format(name),
     license="MIT",
     packages=[name],
     entry_points={
         "console_scripts": [
```

