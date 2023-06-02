# Comparing `tmp/pop-llm-0.0.6.tar.gz` & `tmp/pop-llm-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pop-llm-0.0.6.tar", last modified: Fri Jun  2 10:54:40 2023, max compression
+gzip compressed data, was "pop-llm-0.0.7.tar", last modified: Fri Jun  2 11:47:34 2023, max compression
```

## Comparing `pop-llm-0.0.6.tar` & `pop-llm-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 wyb       (1000) wyb       (1000)        0 2023-06-02 10:54:40.669091 pop-llm-0.0.6/
--rw-r--r--   0 wyb       (1000) wyb       (1000)      214 2023-06-02 09:19:20.000000 pop-llm-0.0.6/.gitignore
--rw-r--r--   0 wyb       (1000) wyb       (1000)     1065 2023-06-02 07:40:05.000000 pop-llm-0.0.6/LICENSE
--rw-r--r--   0 wyb       (1000) wyb       (1000)     3051 2023-06-02 10:54:40.669091 pop-llm-0.0.6/PKG-INFO
--rw-r--r--   0 wyb       (1000) wyb       (1000)     2571 2023-06-02 09:19:20.000000 pop-llm-0.0.6/README.md
--rw-r--r--   0 wyb       (1000) wyb       (1000)    13272 2023-06-02 09:32:43.000000 pop-llm-0.0.6/demo.ipynb
--rw-r--r--   0 wyb       (1000) wyb       (1000)      620 2023-06-02 10:54:23.000000 pop-llm-0.0.6/pyproject.toml
--rw-r--r--   0 wyb       (1000) wyb       (1000)       15 2023-06-01 07:43:51.000000 pop-llm-0.0.6/requirement.txt
--rw-r--r--   0 wyb       (1000) wyb       (1000)       38 2023-06-02 10:54:40.669091 pop-llm-0.0.6/setup.cfg
-drwxr-xr-x   0 wyb       (1000) wyb       (1000)        0 2023-06-02 10:54:40.665758 pop-llm-0.0.6/src/
-drwxr-xr-x   0 wyb       (1000) wyb       (1000)        0 2023-06-02 10:54:40.669091 pop-llm-0.0.6/src/pop_llm/
--rw-r--r--   0 wyb       (1000) wyb       (1000)       29 2023-06-02 07:40:05.000000 pop-llm-0.0.6/src/pop_llm/__init__.py
--rw-r--r--   0 wyb       (1000) wyb       (1000)    12718 2023-06-02 09:19:20.000000 pop-llm-0.0.6/src/pop_llm/chat_agent.py
--rw-r--r--   0 wyb       (1000) wyb       (1000)     3960 2023-06-02 10:46:38.000000 pop-llm-0.0.6/src/pop_llm/pop.py
--rw-r--r--   0 wyb       (1000) wyb       (1000)     1689 2023-06-02 07:40:05.000000 pop-llm-0.0.6/src/pop_llm/prompts.py
-drwxr-xr-x   0 wyb       (1000) wyb       (1000)        0 2023-06-02 10:54:40.669091 pop-llm-0.0.6/src/pop_llm.egg-info/
--rw-r--r--   0 wyb       (1000) wyb       (1000)     3051 2023-06-02 10:54:40.000000 pop-llm-0.0.6/src/pop_llm.egg-info/PKG-INFO
--rw-r--r--   0 wyb       (1000) wyb       (1000)      336 2023-06-02 10:54:40.000000 pop-llm-0.0.6/src/pop_llm.egg-info/SOURCES.txt
--rw-r--r--   0 wyb       (1000) wyb       (1000)        1 2023-06-02 10:54:40.000000 pop-llm-0.0.6/src/pop_llm.egg-info/dependency_links.txt
--rw-r--r--   0 wyb       (1000) wyb       (1000)       16 2023-06-02 10:54:40.000000 pop-llm-0.0.6/src/pop_llm.egg-info/requires.txt
--rw-r--r--   0 wyb       (1000) wyb       (1000)        8 2023-06-02 10:54:40.000000 pop-llm-0.0.6/src/pop_llm.egg-info/top_level.txt
+drwxr-xr-x   0 wyb       (1000) wyb       (1000)        0 2023-06-02 11:47:34.301441 pop-llm-0.0.7/
+-rw-r--r--   0 wyb       (1000) wyb       (1000)      214 2023-06-02 09:19:20.000000 pop-llm-0.0.7/.gitignore
+-rw-r--r--   0 wyb       (1000) wyb       (1000)     1065 2023-06-02 07:40:05.000000 pop-llm-0.0.7/LICENSE
+-rw-r--r--   0 wyb       (1000) wyb       (1000)     3051 2023-06-02 11:47:34.301441 pop-llm-0.0.7/PKG-INFO
+-rw-r--r--   0 wyb       (1000) wyb       (1000)     2571 2023-06-02 09:19:20.000000 pop-llm-0.0.7/README.md
+-rw-r--r--   0 wyb       (1000) wyb       (1000)    13238 2023-06-02 10:54:49.000000 pop-llm-0.0.7/demo.ipynb
+-rw-r--r--   0 wyb       (1000) wyb       (1000)      620 2023-06-02 11:47:10.000000 pop-llm-0.0.7/pyproject.toml
+-rw-r--r--   0 wyb       (1000) wyb       (1000)       15 2023-06-01 07:43:51.000000 pop-llm-0.0.7/requirement.txt
+-rw-r--r--   0 wyb       (1000) wyb       (1000)       38 2023-06-02 11:47:34.301441 pop-llm-0.0.7/setup.cfg
+drwxr-xr-x   0 wyb       (1000) wyb       (1000)        0 2023-06-02 11:47:34.298107 pop-llm-0.0.7/src/
+drwxr-xr-x   0 wyb       (1000) wyb       (1000)        0 2023-06-02 11:47:34.301441 pop-llm-0.0.7/src/pop_llm/
+-rw-r--r--   0 wyb       (1000) wyb       (1000)       29 2023-06-02 07:40:05.000000 pop-llm-0.0.7/src/pop_llm/__init__.py
+-rw-r--r--   0 wyb       (1000) wyb       (1000)    12718 2023-06-02 11:26:25.000000 pop-llm-0.0.7/src/pop_llm/chat_agent.py
+-rw-r--r--   0 wyb       (1000) wyb       (1000)     3946 2023-06-02 11:46:07.000000 pop-llm-0.0.7/src/pop_llm/pop.py
+-rw-r--r--   0 wyb       (1000) wyb       (1000)     1689 2023-06-02 11:25:51.000000 pop-llm-0.0.7/src/pop_llm/prompts.py
+drwxr-xr-x   0 wyb       (1000) wyb       (1000)        0 2023-06-02 11:47:34.301441 pop-llm-0.0.7/src/pop_llm.egg-info/
+-rw-r--r--   0 wyb       (1000) wyb       (1000)     3051 2023-06-02 11:47:34.000000 pop-llm-0.0.7/src/pop_llm.egg-info/PKG-INFO
+-rw-r--r--   0 wyb       (1000) wyb       (1000)      336 2023-06-02 11:47:34.000000 pop-llm-0.0.7/src/pop_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 wyb       (1000) wyb       (1000)        1 2023-06-02 11:47:34.000000 pop-llm-0.0.7/src/pop_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 wyb       (1000) wyb       (1000)       16 2023-06-02 11:47:34.000000 pop-llm-0.0.7/src/pop_llm.egg-info/requires.txt
+-rw-r--r--   0 wyb       (1000) wyb       (1000)        8 2023-06-02 11:47:34.000000 pop-llm-0.0.7/src/pop_llm.egg-info/top_level.txt
```

### Comparing `pop-llm-0.0.6/LICENSE` & `pop-llm-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pop-llm-0.0.6/PKG-INFO` & `pop-llm-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pop-llm
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python library for Prompt Oriented Programming with Large Language Models
 Author-email: Yibo Wei <david_wyb2001@outlook.com>
 Project-URL: Homepage, https://github.com/Microwave_WYB/POP
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `pop-llm-0.0.6/README.md` & `pop-llm-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pop-llm-0.0.6/demo.ipynb` & `pop-llm-0.0.7/demo.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9991071428571429%*

 * *Differences: {"'cells'": "{13: {'source': []}}"}*

```diff
@@ -301,17 +301,15 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
-            "source": [
-                "tldr_with_tools.history"
-            ]
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "pop",
             "language": "python",
             "name": "python3"
```

### Comparing `pop-llm-0.0.6/src/pop_llm/chat_agent.py` & `pop-llm-0.0.7/src/pop_llm/chat_agent.py`

 * *Files identical despite different names*

### Comparing `pop-llm-0.0.6/src/pop_llm/pop.py` & `pop-llm-0.0.7/src/pop_llm/pop.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import json
 from typing import Any, List, Callable
 from .chat_agent import OpenAIAgent
 from .prompts import POP_PROMPT_PREFIX
 
 INDENT = "    "
 
 from typing import List
@@ -33,70 +34,72 @@
             name (str, optional): The name of the function. Defaults to "function".
             input_assert (Callable[[Any], bool], optional): The assertion function for the input. Defaults to None.
             temperature (float, optional): The temperature of the chatbot. Defaults to 0.0.
             tools (List[Callable], optional): The tools of the chatbot. Defaults to None.
         """
         self.input_keys = input_keys
         self.name = name
+        self.description = description
         self.output_keys = output_keys
         self.system_prompt = POP_PROMPT_PREFIX
         self.system_prompt += f"Your name is: {self.name}.\n"
         self.system_prompt += f"Your task is described as follows:\n"
         self.system_prompt += f"{INDENT}{description}\n"
         self.system_prompt += f"Your input keys are: \n"
         self.system_prompt += (
-            "[" + ", ".join([f'"{key}"' for key in self.input_keys]) + "].\n"
+            json.dumps(self.input_keys) + "\n"
         )
         self.system_prompt += f"Your output keys are: \n"
         self.system_prompt += (
-            "[" + ", ".join([f'"{key}"' for key in self.output_keys]) + "].\n"
+            json.dumps(self.output_keys) + "\n"
         )
         super().__init__(
             system_prompt=self.system_prompt,
             output_keys=output_keys,
             temperature=temperature,
             history=[],
             tools=tools,
         )
-        self.assert_callback = input_assert
-    
-    def __doc__(self):
-        doc = f"POP function {self.name}.\n"
-        doc += self.description
-        doc += "\n\nArgs:\n"
+        self.input_assert = input_assert
+
+        doc = f"Description: {self.description}\n"
+        doc += "\nArgs:\n"
         for key in self.input_keys:
-            doc += f"{INDENT}{key} (Any): function input.\n"
+            doc += f"{INDENT}{key}: function input.\n"
         doc += "\nReturns:\n"
         for key in self.output_keys:
-            doc += f"{INDENT}{key} (Any): function output.\n"
+            doc += f"{INDENT}{key}: function output.\n"
+        self.__doc__ = doc
 
     def __call__(self, *args: Any, **kwds: Any) -> dict:
         """
         Run the function by sending input to the chatbot.
 
         Returns:
             dict: The output of the function.
         """
         logging.info(f"Calling function {self.name} with args {args} and kwds {kwds}")
-        if self.assert_callback is not None:
-            assert self.assert_callback(
-                *args, **kwds
-            ), "Input does not satisfy assertion."
+        if self.input_assert is not None:
+            assert self.input_assert(*args, **kwds), "Input does not satisfy assertion."
         input_dict = dict(zip(self.input_keys, args))
         input_dict.update(kwds)
         input_dict_str = str(input_dict).replace("'", '"')
         output_dict = self.run(input_dict_str)
         # raise error if output_dict does not contain all output_keys
         for key in self.output_keys:
             if key not in output_dict:
                 # raise KeyError(
                 #     f"Output key {key} is not found in the output dictionary."
                 # )
-                logging.warning(f"Output key '{key}' is not found in the output dictionary.")
-                self.run(f"Make sure you have all the required output keys: {self.output_keys}.")
+                logging.warning(
+                    f"Output key '{key}' is not found in the output dictionary."
+                )
+                self.run(
+                    f"Make sure you have all the required output keys: {self.output_keys}."
+                )
         return output_dict
 
 
 if __name__ == "__main__":
     add = PopFunction(
         input_keys=["a", "b"],
         output_keys=["sum"],
```

### Comparing `pop-llm-0.0.6/src/pop_llm/prompts.py` & `pop-llm-0.0.7/src/pop_llm/prompts.py`

 * *Files identical despite different names*

### Comparing `pop-llm-0.0.6/src/pop_llm.egg-info/PKG-INFO` & `pop-llm-0.0.7/src/pop_llm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pop-llm
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python library for Prompt Oriented Programming with Large Language Models
 Author-email: Yibo Wei <david_wyb2001@outlook.com>
 Project-URL: Homepage, https://github.com/Microwave_WYB/POP
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

