# Comparing `tmp/pop-llm-0.0.5.tar.gz` & `tmp/pop-llm-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pop-llm-0.0.5.tar", last modified: Fri Jun  2 09:49:57 2023, max compression
+gzip compressed data, was "pop-llm-0.0.6.tar", last modified: Fri Jun  2 10:54:40 2023, max compression
```

## Comparing `pop-llm-0.0.5.tar` & `pop-llm-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 wyb       (1000) wyb       (1000)        0 2023-06-02 09:49:57.735896 pop-llm-0.0.5/
--rw-r--r--   0 wyb       (1000) wyb       (1000)      214 2023-06-02 09:19:20.000000 pop-llm-0.0.5/.gitignore
--rw-r--r--   0 wyb       (1000) wyb       (1000)     1065 2023-06-02 07:40:05.000000 pop-llm-0.0.5/LICENSE
--rw-r--r--   0 wyb       (1000) wyb       (1000)     3051 2023-06-02 09:49:57.735896 pop-llm-0.0.5/PKG-INFO
--rw-r--r--   0 wyb       (1000) wyb       (1000)     2571 2023-06-02 09:19:20.000000 pop-llm-0.0.5/README.md
--rw-r--r--   0 wyb       (1000) wyb       (1000)    13272 2023-06-02 09:32:43.000000 pop-llm-0.0.5/demo.ipynb
--rw-r--r--   0 wyb       (1000) wyb       (1000)      620 2023-06-02 09:49:25.000000 pop-llm-0.0.5/pyproject.toml
--rw-r--r--   0 wyb       (1000) wyb       (1000)       15 2023-06-01 07:43:51.000000 pop-llm-0.0.5/requirement.txt
--rw-r--r--   0 wyb       (1000) wyb       (1000)       38 2023-06-02 09:49:57.735896 pop-llm-0.0.5/setup.cfg
-drwxr-xr-x   0 wyb       (1000) wyb       (1000)        0 2023-06-02 09:49:57.732563 pop-llm-0.0.5/src/
-drwxr-xr-x   0 wyb       (1000) wyb       (1000)        0 2023-06-02 09:49:57.735896 pop-llm-0.0.5/src/pop_llm/
--rw-r--r--   0 wyb       (1000) wyb       (1000)       29 2023-06-02 07:40:05.000000 pop-llm-0.0.5/src/pop_llm/__init__.py
--rw-r--r--   0 wyb       (1000) wyb       (1000)    12718 2023-06-02 09:19:20.000000 pop-llm-0.0.5/src/pop_llm/chat_agent.py
--rw-r--r--   0 wyb       (1000) wyb       (1000)     3962 2023-06-02 09:19:20.000000 pop-llm-0.0.5/src/pop_llm/pop.py
--rw-r--r--   0 wyb       (1000) wyb       (1000)     1689 2023-06-02 07:40:05.000000 pop-llm-0.0.5/src/pop_llm/prompts.py
-drwxr-xr-x   0 wyb       (1000) wyb       (1000)        0 2023-06-02 09:49:57.735896 pop-llm-0.0.5/src/pop_llm.egg-info/
--rw-r--r--   0 wyb       (1000) wyb       (1000)     3051 2023-06-02 09:49:57.000000 pop-llm-0.0.5/src/pop_llm.egg-info/PKG-INFO
--rw-r--r--   0 wyb       (1000) wyb       (1000)      336 2023-06-02 09:49:57.000000 pop-llm-0.0.5/src/pop_llm.egg-info/SOURCES.txt
--rw-r--r--   0 wyb       (1000) wyb       (1000)        1 2023-06-02 09:49:57.000000 pop-llm-0.0.5/src/pop_llm.egg-info/dependency_links.txt
--rw-r--r--   0 wyb       (1000) wyb       (1000)       16 2023-06-02 09:49:57.000000 pop-llm-0.0.5/src/pop_llm.egg-info/requires.txt
--rw-r--r--   0 wyb       (1000) wyb       (1000)        8 2023-06-02 09:49:57.000000 pop-llm-0.0.5/src/pop_llm.egg-info/top_level.txt
+drwxr-xr-x   0 wyb       (1000) wyb       (1000)        0 2023-06-02 10:54:40.669091 pop-llm-0.0.6/
+-rw-r--r--   0 wyb       (1000) wyb       (1000)      214 2023-06-02 09:19:20.000000 pop-llm-0.0.6/.gitignore
+-rw-r--r--   0 wyb       (1000) wyb       (1000)     1065 2023-06-02 07:40:05.000000 pop-llm-0.0.6/LICENSE
+-rw-r--r--   0 wyb       (1000) wyb       (1000)     3051 2023-06-02 10:54:40.669091 pop-llm-0.0.6/PKG-INFO
+-rw-r--r--   0 wyb       (1000) wyb       (1000)     2571 2023-06-02 09:19:20.000000 pop-llm-0.0.6/README.md
+-rw-r--r--   0 wyb       (1000) wyb       (1000)    13272 2023-06-02 09:32:43.000000 pop-llm-0.0.6/demo.ipynb
+-rw-r--r--   0 wyb       (1000) wyb       (1000)      620 2023-06-02 10:54:23.000000 pop-llm-0.0.6/pyproject.toml
+-rw-r--r--   0 wyb       (1000) wyb       (1000)       15 2023-06-01 07:43:51.000000 pop-llm-0.0.6/requirement.txt
+-rw-r--r--   0 wyb       (1000) wyb       (1000)       38 2023-06-02 10:54:40.669091 pop-llm-0.0.6/setup.cfg
+drwxr-xr-x   0 wyb       (1000) wyb       (1000)        0 2023-06-02 10:54:40.665758 pop-llm-0.0.6/src/
+drwxr-xr-x   0 wyb       (1000) wyb       (1000)        0 2023-06-02 10:54:40.669091 pop-llm-0.0.6/src/pop_llm/
+-rw-r--r--   0 wyb       (1000) wyb       (1000)       29 2023-06-02 07:40:05.000000 pop-llm-0.0.6/src/pop_llm/__init__.py
+-rw-r--r--   0 wyb       (1000) wyb       (1000)    12718 2023-06-02 09:19:20.000000 pop-llm-0.0.6/src/pop_llm/chat_agent.py
+-rw-r--r--   0 wyb       (1000) wyb       (1000)     3960 2023-06-02 10:46:38.000000 pop-llm-0.0.6/src/pop_llm/pop.py
+-rw-r--r--   0 wyb       (1000) wyb       (1000)     1689 2023-06-02 07:40:05.000000 pop-llm-0.0.6/src/pop_llm/prompts.py
+drwxr-xr-x   0 wyb       (1000) wyb       (1000)        0 2023-06-02 10:54:40.669091 pop-llm-0.0.6/src/pop_llm.egg-info/
+-rw-r--r--   0 wyb       (1000) wyb       (1000)     3051 2023-06-02 10:54:40.000000 pop-llm-0.0.6/src/pop_llm.egg-info/PKG-INFO
+-rw-r--r--   0 wyb       (1000) wyb       (1000)      336 2023-06-02 10:54:40.000000 pop-llm-0.0.6/src/pop_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 wyb       (1000) wyb       (1000)        1 2023-06-02 10:54:40.000000 pop-llm-0.0.6/src/pop_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 wyb       (1000) wyb       (1000)       16 2023-06-02 10:54:40.000000 pop-llm-0.0.6/src/pop_llm.egg-info/requires.txt
+-rw-r--r--   0 wyb       (1000) wyb       (1000)        8 2023-06-02 10:54:40.000000 pop-llm-0.0.6/src/pop_llm.egg-info/top_level.txt
```

### Comparing `pop-llm-0.0.5/LICENSE` & `pop-llm-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pop-llm-0.0.5/PKG-INFO` & `pop-llm-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pop-llm
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python library for Prompt Oriented Programming with Large Language Models
 Author-email: Yibo Wei <david_wyb2001@outlook.com>
 Project-URL: Homepage, https://github.com/Microwave_WYB/POP
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `pop-llm-0.0.5/README.md` & `pop-llm-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pop-llm-0.0.5/demo.ipynb` & `pop-llm-0.0.6/demo.ipynb`

 * *Files identical despite different names*

### Comparing `pop-llm-0.0.5/pyproject.toml` & `pop-llm-0.0.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pop-llm"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Yibo Wei", email="david_wyb2001@outlook.com" },
 ]
 description = "A Python library for Prompt Oriented Programming with Large Language Models"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `pop-llm-0.0.5/src/pop_llm/chat_agent.py` & `pop-llm-0.0.6/src/pop_llm/chat_agent.py`

 * *Files identical despite different names*

### Comparing `pop-llm-0.0.5/src/pop_llm/pop.py` & `pop-llm-0.0.6/src/pop_llm/pop.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         self,
         input_keys: List[str],
         output_keys: List[str],
         description: str,
         name: str = "function",
         input_assert: Callable[[Any], bool] = None,
         temperature: float = 0.0,
-        tools: List[Callable] = None,
+        tools: List[Callable] = [],
     ) -> None:
         """
         Initialize a POP function.
 
         Args:
             input_keys (List[str]): The input keys of the function.
             output_keys (List[str]): The output keys of the function.
```

### Comparing `pop-llm-0.0.5/src/pop_llm/prompts.py` & `pop-llm-0.0.6/src/pop_llm/prompts.py`

 * *Files identical despite different names*

### Comparing `pop-llm-0.0.5/src/pop_llm.egg-info/PKG-INFO` & `pop-llm-0.0.6/src/pop_llm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pop-llm
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python library for Prompt Oriented Programming with Large Language Models
 Author-email: Yibo Wei <david_wyb2001@outlook.com>
 Project-URL: Homepage, https://github.com/Microwave_WYB/POP
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

