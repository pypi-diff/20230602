# Comparing `tmp/pop_llm-0.0.2.tar.gz` & `tmp/pop-llm-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "pop-llm-0.0.3.tar", last modified: Fri Jun  2 01:49:12 2023, max compression
```

## Comparing `pop_llm-0.0.2.tar` & `pop-llm-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,20 @@
--rw-r--r--   0        0        0     8840 2020-02-02 00:00:00.000000 pop_llm-0.0.2/demo.ipynb
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 pop_llm-0.0.2/requirement.txt
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pop_llm-0.0.2/src/pop_llm/__init__.py
--rw-r--r--   0        0        0    12657 2020-02-02 00:00:00.000000 pop_llm-0.0.2/src/pop_llm/chat_agent.py
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 pop_llm-0.0.2/src/pop_llm/pop.py
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 pop_llm-0.0.2/src/pop_llm/prompts.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 pop_llm-0.0.2/.gitignore
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 pop_llm-0.0.2/README.md
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 pop_llm-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 pop_llm-0.0.2/PKG-INFO
+drwxr-xr-x   0 wyb       (1000) wyb       (1000)        0 2023-06-02 01:49:12.026116 pop-llm-0.0.3/
+-rw-r--r--   0 wyb       (1000) wyb       (1000)      193 2023-06-02 01:27:27.000000 pop-llm-0.0.3/.gitignore
+-rw-r--r--   0 wyb       (1000) wyb       (1000)     1843 2023-06-02 01:49:12.026116 pop-llm-0.0.3/PKG-INFO
+-rw-r--r--   0 wyb       (1000) wyb       (1000)     1385 2023-06-02 01:00:39.000000 pop-llm-0.0.3/README.md
+-rw-r--r--   0 wyb       (1000) wyb       (1000)     8840 2023-06-02 00:24:13.000000 pop-llm-0.0.3/demo.ipynb
+-rw-r--r--   0 wyb       (1000) wyb       (1000)      620 2023-06-02 01:48:27.000000 pop-llm-0.0.3/pyproject.toml
+-rw-r--r--   0 wyb       (1000) wyb       (1000)       15 2023-06-02 00:09:11.000000 pop-llm-0.0.3/requirement.txt
+-rw-r--r--   0 wyb       (1000) wyb       (1000)       38 2023-06-02 01:49:12.026116 pop-llm-0.0.3/setup.cfg
+drwxr-xr-x   0 wyb       (1000) wyb       (1000)        0 2023-06-02 01:49:12.022783 pop-llm-0.0.3/src/
+drwxr-xr-x   0 wyb       (1000) wyb       (1000)        0 2023-06-02 01:49:12.026116 pop-llm-0.0.3/src/pop_llm/
+-rw-r--r--   0 wyb       (1000) wyb       (1000)       29 2023-06-02 00:52:36.000000 pop-llm-0.0.3/src/pop_llm/__init__.py
+-rw-r--r--   0 wyb       (1000) wyb       (1000)    12658 2023-06-02 01:43:07.000000 pop-llm-0.0.3/src/pop_llm/chat_agent.py
+-rw-r--r--   0 wyb       (1000) wyb       (1000)     2659 2023-06-02 01:36:45.000000 pop-llm-0.0.3/src/pop_llm/pop.py
+-rw-r--r--   0 wyb       (1000) wyb       (1000)     1689 2023-06-02 00:36:24.000000 pop-llm-0.0.3/src/pop_llm/prompts.py
+drwxr-xr-x   0 wyb       (1000) wyb       (1000)        0 2023-06-02 01:49:12.026116 pop-llm-0.0.3/src/pop_llm.egg-info/
+-rw-r--r--   0 wyb       (1000) wyb       (1000)     1843 2023-06-02 01:49:11.000000 pop-llm-0.0.3/src/pop_llm.egg-info/PKG-INFO
+-rw-r--r--   0 wyb       (1000) wyb       (1000)      328 2023-06-02 01:49:12.000000 pop-llm-0.0.3/src/pop_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 wyb       (1000) wyb       (1000)        1 2023-06-02 01:49:11.000000 pop-llm-0.0.3/src/pop_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 wyb       (1000) wyb       (1000)       16 2023-06-02 01:49:11.000000 pop-llm-0.0.3/src/pop_llm.egg-info/requires.txt
+-rw-r--r--   0 wyb       (1000) wyb       (1000)        8 2023-06-02 01:49:11.000000 pop-llm-0.0.3/src/pop_llm.egg-info/top_level.txt
```

### Comparing `pop_llm-0.0.2/demo.ipynb` & `pop-llm-0.0.3/demo.ipynb`

 * *Files identical despite different names*

### Comparing `pop_llm-0.0.2/src/pop_llm/chat_agent.py` & `pop-llm-0.0.3/src/pop_llm/chat_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import tiktoken
 import logging
 import json
 import os
 from typing import List
 from datetime import datetime
 from typing import Union, Callable
-from prompts import TOOL_PROMPT_PREFIX, TOOL_PROMPT_SUFFIX, INDENT
+from .prompts import TOOL_PROMPT_PREFIX, TOOL_PROMPT_SUFFIX, INDENT
 
 
 class OpenAIMessage(dict):
     """
     Class representing a message. A message includes role and content.
     """
```

### Comparing `pop_llm-0.0.2/src/pop_llm/pop.py` & `pop-llm-0.0.3/src/pop_llm/pop.py`

 * *Files identical despite different names*

### Comparing `pop_llm-0.0.2/src/pop_llm/prompts.py` & `pop-llm-0.0.3/src/pop_llm/prompts.py`

 * *Files identical despite different names*

### Comparing `pop_llm-0.0.2/README.md` & `pop-llm-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pop_llm-0.0.2/PKG-INFO` & `pop-llm-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pop-llm
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python library for Prompt Oriented Programming with Large Language Models
-Project-URL: Homepage, https://github.com/Microwave_WYB/POP
 Author-email: Yibo Wei <david_wyb2001@outlook.com>
+Project-URL: Homepage, https://github.com/Microwave_WYB/POP
+Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # POP: Prompt Oriented Programming
 
 ## Setup
 
@@ -59,8 +59,8 @@
     description="Add two numbers.", # The description of the task
     name = "add", # A name for the function, default to "function"
     input_assert=lambda a, b: type(a) == int and type(b) == int, # A function to assert the input
     temperature=0 # Set to 0 for deterministic, 1 for the most randomness
 )
 ```
 
-For more examples, please refer to the [Demo Notebook](./demo.ipynb)
+For more examples, please refer to the [Demo Notebook](./demo.ipynb)
```

