# Comparing `tmp/pop-llm-0.0.3.tar.gz` & `tmp/pop-llm-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pop-llm-0.0.3.tar", last modified: Fri Jun  2 01:49:12 2023, max compression
+gzip compressed data, was "pop-llm-0.0.4.tar", last modified: Fri Jun  2 05:25:21 2023, max compression
```

## Comparing `pop-llm-0.0.3.tar` & `pop-llm-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 wyb       (1000) wyb       (1000)        0 2023-06-02 01:49:12.026116 pop-llm-0.0.3/
--rw-r--r--   0 wyb       (1000) wyb       (1000)      193 2023-06-02 01:27:27.000000 pop-llm-0.0.3/.gitignore
--rw-r--r--   0 wyb       (1000) wyb       (1000)     1843 2023-06-02 01:49:12.026116 pop-llm-0.0.3/PKG-INFO
--rw-r--r--   0 wyb       (1000) wyb       (1000)     1385 2023-06-02 01:00:39.000000 pop-llm-0.0.3/README.md
--rw-r--r--   0 wyb       (1000) wyb       (1000)     8840 2023-06-02 00:24:13.000000 pop-llm-0.0.3/demo.ipynb
--rw-r--r--   0 wyb       (1000) wyb       (1000)      620 2023-06-02 01:48:27.000000 pop-llm-0.0.3/pyproject.toml
--rw-r--r--   0 wyb       (1000) wyb       (1000)       15 2023-06-02 00:09:11.000000 pop-llm-0.0.3/requirement.txt
--rw-r--r--   0 wyb       (1000) wyb       (1000)       38 2023-06-02 01:49:12.026116 pop-llm-0.0.3/setup.cfg
-drwxr-xr-x   0 wyb       (1000) wyb       (1000)        0 2023-06-02 01:49:12.022783 pop-llm-0.0.3/src/
-drwxr-xr-x   0 wyb       (1000) wyb       (1000)        0 2023-06-02 01:49:12.026116 pop-llm-0.0.3/src/pop_llm/
--rw-r--r--   0 wyb       (1000) wyb       (1000)       29 2023-06-02 00:52:36.000000 pop-llm-0.0.3/src/pop_llm/__init__.py
--rw-r--r--   0 wyb       (1000) wyb       (1000)    12658 2023-06-02 01:43:07.000000 pop-llm-0.0.3/src/pop_llm/chat_agent.py
--rw-r--r--   0 wyb       (1000) wyb       (1000)     2659 2023-06-02 01:36:45.000000 pop-llm-0.0.3/src/pop_llm/pop.py
--rw-r--r--   0 wyb       (1000) wyb       (1000)     1689 2023-06-02 00:36:24.000000 pop-llm-0.0.3/src/pop_llm/prompts.py
-drwxr-xr-x   0 wyb       (1000) wyb       (1000)        0 2023-06-02 01:49:12.026116 pop-llm-0.0.3/src/pop_llm.egg-info/
--rw-r--r--   0 wyb       (1000) wyb       (1000)     1843 2023-06-02 01:49:11.000000 pop-llm-0.0.3/src/pop_llm.egg-info/PKG-INFO
--rw-r--r--   0 wyb       (1000) wyb       (1000)      328 2023-06-02 01:49:12.000000 pop-llm-0.0.3/src/pop_llm.egg-info/SOURCES.txt
--rw-r--r--   0 wyb       (1000) wyb       (1000)        1 2023-06-02 01:49:11.000000 pop-llm-0.0.3/src/pop_llm.egg-info/dependency_links.txt
--rw-r--r--   0 wyb       (1000) wyb       (1000)       16 2023-06-02 01:49:11.000000 pop-llm-0.0.3/src/pop_llm.egg-info/requires.txt
--rw-r--r--   0 wyb       (1000) wyb       (1000)        8 2023-06-02 01:49:11.000000 pop-llm-0.0.3/src/pop_llm.egg-info/top_level.txt
+drwxr-xr-x   0 wyb       (1000) wyb       (1000)        0 2023-06-02 05:25:21.946389 pop-llm-0.0.4/
+-rw-r--r--   0 wyb       (1000) wyb       (1000)      205 2023-06-02 03:16:11.000000 pop-llm-0.0.4/.gitignore
+-rw-r--r--   0 wyb       (1000) wyb       (1000)     1065 2023-06-02 03:16:11.000000 pop-llm-0.0.4/LICENSE
+-rw-r--r--   0 wyb       (1000) wyb       (1000)     1865 2023-06-02 05:25:21.946389 pop-llm-0.0.4/PKG-INFO
+-rw-r--r--   0 wyb       (1000) wyb       (1000)     1385 2023-06-02 03:16:11.000000 pop-llm-0.0.4/README.md
+-rw-r--r--   0 wyb       (1000) wyb       (1000)     8844 2023-06-02 03:16:11.000000 pop-llm-0.0.4/demo.ipynb
+-rw-r--r--   0 wyb       (1000) wyb       (1000)      620 2023-06-02 05:23:39.000000 pop-llm-0.0.4/pyproject.toml
+-rw-r--r--   0 wyb       (1000) wyb       (1000)       15 2023-06-02 00:09:11.000000 pop-llm-0.0.4/requirement.txt
+-rw-r--r--   0 wyb       (1000) wyb       (1000)       38 2023-06-02 05:25:21.946389 pop-llm-0.0.4/setup.cfg
+drwxr-xr-x   0 wyb       (1000) wyb       (1000)        0 2023-06-02 05:25:21.943055 pop-llm-0.0.4/src/
+drwxr-xr-x   0 wyb       (1000) wyb       (1000)        0 2023-06-02 05:25:21.943055 pop-llm-0.0.4/src/pop_llm/
+-rw-r--r--   0 wyb       (1000) wyb       (1000)       29 2023-06-02 03:16:11.000000 pop-llm-0.0.4/src/pop_llm/__init__.py
+-rw-r--r--   0 wyb       (1000) wyb       (1000)    12589 2023-06-02 05:21:45.000000 pop-llm-0.0.4/src/pop_llm/chat_agent.py
+-rw-r--r--   0 wyb       (1000) wyb       (1000)     2682 2023-06-02 05:21:45.000000 pop-llm-0.0.4/src/pop_llm/pop.py
+-rw-r--r--   0 wyb       (1000) wyb       (1000)     1689 2023-06-02 03:16:11.000000 pop-llm-0.0.4/src/pop_llm/prompts.py
+drwxr-xr-x   0 wyb       (1000) wyb       (1000)        0 2023-06-02 05:25:21.946389 pop-llm-0.0.4/src/pop_llm.egg-info/
+-rw-r--r--   0 wyb       (1000) wyb       (1000)     1865 2023-06-02 05:25:21.000000 pop-llm-0.0.4/src/pop_llm.egg-info/PKG-INFO
+-rw-r--r--   0 wyb       (1000) wyb       (1000)      336 2023-06-02 05:25:21.000000 pop-llm-0.0.4/src/pop_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 wyb       (1000) wyb       (1000)        1 2023-06-02 05:25:21.000000 pop-llm-0.0.4/src/pop_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 wyb       (1000) wyb       (1000)       16 2023-06-02 05:25:21.000000 pop-llm-0.0.4/src/pop_llm.egg-info/requires.txt
+-rw-r--r--   0 wyb       (1000) wyb       (1000)        8 2023-06-02 05:25:21.000000 pop-llm-0.0.4/src/pop_llm.egg-info/top_level.txt
```

### Comparing `pop-llm-0.0.3/PKG-INFO` & `pop-llm-0.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: pop-llm
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python library for Prompt Oriented Programming with Large Language Models
 Author-email: Yibo Wei <david_wyb2001@outlook.com>
 Project-URL: Homepage, https://github.com/Microwave_WYB/POP
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # POP: Prompt Oriented Programming
 
 ## Setup
 
 Install from PyPI:
```

### Comparing `pop-llm-0.0.3/README.md` & `pop-llm-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pop-llm-0.0.3/demo.ipynb` & `pop-llm-0.0.4/demo.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, 'from pop_llm import PopFunction\\n')], delete: [0]}}}"}*

```diff
@@ -2,15 +2,15 @@
     "cells": [
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from pop import PopFunction\n",
+                "from pop_llm import PopFunction\n",
                 "import openai\n",
                 "\n",
                 "openai.api_key_path = \"openai_api_key.txt\""
             ]
         },
         {
             "attachments": {},
```

### Comparing `pop-llm-0.0.3/pyproject.toml` & `pop-llm-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pop-llm"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Yibo Wei", email="david_wyb2001@outlook.com" },
 ]
 description = "A Python library for Prompt Oriented Programming with Large Language Models"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `pop-llm-0.0.3/src/pop_llm/chat_agent.py` & `pop-llm-0.0.4/src/pop_llm/chat_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
         logging.info("Chatbot history summarized. Summary: %s", summary)
 
     def pop_oldest_history(self) -> None:
         """
         Pop the oldest message from the chatbot's history
         """
         # Keep the first system message
-        if len(self.history) > 1:
+        if len(self.history) > 2:
             self.history.pop(1)
         else:
             logging.error("Cannot pop oldest history. History is empty.")
             raise ValueError("Cannot pop oldest history. History is empty.")
 
     def reset_history(self) -> None:
         """
@@ -182,16 +182,14 @@
             # self.summarize_history()
             # TODO: summarize history
             try:
                 self.pop_oldest_history()
             except ValueError:
                 raise ValueError("Token usage exceeded maximum tokens.")
         response = self.send_history()
-        # Add response to history
-        self.add_message(response)
         # Parse output if output keys are specified
         parsed_content = self.parse_output(response.content)
 
         # Call the tool if the output contains a tool name
         args = None
         if (
             parsed_content.get("tool", None) is not None
```

### Comparing `pop-llm-0.0.3/src/pop_llm/pop.py` & `pop-llm-0.0.4/src/pop_llm/pop.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         self.system_prompt += (
             "[" + ", ".join([f'"{key}"' for key in self.output_keys]) + "].\n"
         )
         super().__init__(
             system_prompt=self.system_prompt,
             output_keys=output_keys,
             temperature=temperature,
+            history=[]
         )
         self.assert_callback = input_assert
 
     def __call__(self, *args: Any, **kwds: Any) -> dict:
         """
         Run the function by sending input to the chatbot.
```

### Comparing `pop-llm-0.0.3/src/pop_llm/prompts.py` & `pop-llm-0.0.4/src/pop_llm/prompts.py`

 * *Files identical despite different names*

### Comparing `pop-llm-0.0.3/src/pop_llm.egg-info/PKG-INFO` & `pop-llm-0.0.4/src/pop_llm.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: pop-llm
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python library for Prompt Oriented Programming with Large Language Models
 Author-email: Yibo Wei <david_wyb2001@outlook.com>
 Project-URL: Homepage, https://github.com/Microwave_WYB/POP
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # POP: Prompt Oriented Programming
 
 ## Setup
 
 Install from PyPI:
```

