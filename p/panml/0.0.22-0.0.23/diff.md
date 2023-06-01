# Comparing `tmp/panml-0.0.22.tar.gz` & `tmp/panml-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panml-0.0.22.tar", last modified: Thu Jun  1 11:13:04 2023, max compression
+gzip compressed data, was "panml-0.0.23.tar", last modified: Thu Jun  1 22:37:31 2023, max compression
```

## Comparing `panml-0.0.22.tar` & `panml-0.0.23.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-01 11:13:04.050526 panml-0.0.22/
--rw-r--r--   0 williamzheng   (501) staff       (20)     1063 2023-05-11 06:11:04.000000 panml-0.0.22/LICENSE
--rw-r--r--   0 williamzheng   (501) staff       (20)    14824 2023-06-01 11:13:04.050887 panml-0.0.22/PKG-INFO
--rw-r--r--   0 williamzheng   (501) staff       (20)    13645 2023-06-01 11:12:21.000000 panml-0.0.22/README.md
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-01 11:13:04.042740 panml-0.0.22/panml/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-19 12:08:24.000000 panml-0.0.22/panml/__init__.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     3617 2023-06-01 11:12:21.000000 panml-0.0.22/panml/constants.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-01 11:13:04.045507 panml-0.0.22/panml/core/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.22/panml/core/__init__.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-01 11:13:04.046242 panml-0.0.22/panml/core/clustering/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.22/panml/core/clustering/__init__.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     9033 2023-05-24 12:19:14.000000 panml-0.0.22/panml/core/clustering/faiss.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-01 11:13:04.047847 panml-0.0.22/panml/core/llm/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.22/panml/core/llm/__init__.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    20328 2023-05-29 09:35:44.000000 panml-0.0.22/panml/core/llm/huggingface.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    13708 2023-05-28 12:46:27.000000 panml-0.0.22/panml/core/llm/openai.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     3085 2023-05-28 12:46:27.000000 panml-0.0.22/panml/models.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     2608 2023-05-28 12:46:27.000000 panml-0.0.22/panml/search.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-01 11:13:04.045175 panml-0.0.22/panml.egg-info/
--rw-r--r--   0 williamzheng   (501) staff       (20)    14824 2023-06-01 11:13:03.000000 panml-0.0.22/panml.egg-info/PKG-INFO
--rw-r--r--   0 williamzheng   (501) staff       (20)      468 2023-06-01 11:13:03.000000 panml-0.0.22/panml.egg-info/SOURCES.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)        1 2023-06-01 11:13:03.000000 panml-0.0.22/panml.egg-info/dependency_links.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)      215 2023-06-01 11:13:03.000000 panml-0.0.22/panml.egg-info/requires.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)        6 2023-06-01 11:13:03.000000 panml-0.0.22/panml.egg-info/top_level.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)       79 2023-06-01 11:13:04.051993 panml-0.0.22/setup.cfg
--rw-r--r--   0 williamzheng   (501) staff       (20)     2384 2023-06-01 11:12:21.000000 panml-0.0.22/setup.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-01 11:13:04.049493 panml-0.0.22/test/
--rw-r--r--   0 williamzheng   (501) staff       (20)     4383 2023-05-25 13:23:02.000000 panml-0.0.22/test/test_ModelPack.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    11162 2023-05-22 09:48:53.000000 panml-0.0.22/test/test_VectorEngine.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-01 22:37:31.378286 panml-0.0.23/
+-rw-r--r--   0 williamzheng   (501) staff       (20)     1063 2023-05-11 06:11:04.000000 panml-0.0.23/LICENSE
+-rw-r--r--   0 williamzheng   (501) staff       (20)    14824 2023-06-01 22:37:31.378644 panml-0.0.23/PKG-INFO
+-rw-r--r--   0 williamzheng   (501) staff       (20)    13645 2023-06-01 11:12:21.000000 panml-0.0.23/README.md
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-01 22:37:31.370960 panml-0.0.23/panml/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-19 12:08:24.000000 panml-0.0.23/panml/__init__.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     3617 2023-06-01 11:12:21.000000 panml-0.0.23/panml/constants.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-01 22:37:31.372947 panml-0.0.23/panml/core/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.23/panml/core/__init__.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-01 22:37:31.373594 panml-0.0.23/panml/core/clustering/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.23/panml/core/clustering/__init__.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     9033 2023-05-24 12:19:14.000000 panml-0.0.23/panml/core/clustering/faiss.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-01 22:37:31.375263 panml-0.0.23/panml/core/llm/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.23/panml/core/llm/__init__.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    20353 2023-06-01 22:37:04.000000 panml-0.0.23/panml/core/llm/huggingface.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    13741 2023-06-01 22:37:04.000000 panml-0.0.23/panml/core/llm/openai.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     3085 2023-05-28 12:46:27.000000 panml-0.0.23/panml/models.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     2608 2023-05-28 12:46:27.000000 panml-0.0.23/panml/search.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-01 22:37:31.372627 panml-0.0.23/panml.egg-info/
+-rw-r--r--   0 williamzheng   (501) staff       (20)    14824 2023-06-01 22:37:31.000000 panml-0.0.23/panml.egg-info/PKG-INFO
+-rw-r--r--   0 williamzheng   (501) staff       (20)      468 2023-06-01 22:37:31.000000 panml-0.0.23/panml.egg-info/SOURCES.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)        1 2023-06-01 22:37:31.000000 panml-0.0.23/panml.egg-info/dependency_links.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)      215 2023-06-01 22:37:31.000000 panml-0.0.23/panml.egg-info/requires.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)        6 2023-06-01 22:37:31.000000 panml-0.0.23/panml.egg-info/top_level.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)       79 2023-06-01 22:37:31.379730 panml-0.0.23/setup.cfg
+-rw-r--r--   0 williamzheng   (501) staff       (20)     2384 2023-06-01 22:37:04.000000 panml-0.0.23/setup.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-01 22:37:31.377142 panml-0.0.23/test/
+-rw-r--r--   0 williamzheng   (501) staff       (20)     4383 2023-05-25 13:23:02.000000 panml-0.0.23/test/test_ModelPack.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    11162 2023-05-22 09:48:53.000000 panml-0.0.23/test/test_VectorEngine.py
```

### Comparing `panml-0.0.22/LICENSE` & `panml-0.0.23/LICENSE`

 * *Files identical despite different names*

### Comparing `panml-0.0.22/PKG-INFO` & `panml-0.0.23/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panml
-Version: 0.0.22
+Version: 0.0.23
 Summary: PanML is a high level generative AI/ML development library designed for ease of use and fast experimentation.
 Home-page: https://github.com/Pan-ML/panml
 Author: PanML team
 Author-email: teampanml@gmail.com
 License: MIT
 Keywords: generative AI,generative model,machine learning,large language model,LLM,prompt engineering,fine tuning,prompt tuning,retrieval augmentation,AI safety,AI alignment
 Platform: UNKNOWN
```

### Comparing `panml-0.0.22/README.md` & `panml-0.0.23/README.md`

 * *Files identical despite different names*

### Comparing `panml-0.0.22/panml/constants.py` & `panml-0.0.23/panml/constants.py`

 * *Files identical despite different names*

### Comparing `panml-0.0.22/panml/core/clustering/faiss.py` & `panml-0.0.23/panml/core/clustering/faiss.py`

 * *Files identical despite different names*

### Comparing `panml-0.0.22/panml/core/llm/huggingface.py` & `panml-0.0.23/panml/core/llm/huggingface.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,20 +181,21 @@
         if isinstance(text, str): # wrap input text into list if available
             if len(text) == 0:
                 raise ValueError('Input text cannot be empty')
             input_context = [text]
         if isinstance(text, list):
             if len(text) == 0:
                 raise ValueError('Input text list cannot be empty')
+            input_context = text
         if prompt_modifier is None:
             prompt_modifier = self._init_prompt()
         else:
             if not isinstance(prompt_modifier, list):
                 raise TypeError('Input prompt modifier needs to be of type: list')
-        
+
         # Run prediction on text samples
         prediction = []
         for context in input_context:
             # Create loop for text prediction
             history = []
             for count, mod in enumerate(prompt_modifier):
                 # Set prepend or append to empty str if there is no input for these
```

### Comparing `panml-0.0.22/panml/core/llm/openai.py` & `panml-0.0.23/panml/core/llm/openai.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,14 +123,15 @@
         if isinstance(text, str): # wrap input text into list if available
             if len(text) == 0:
                 raise ValueError('Input text cannot be empty')
             input_context = [text]
         if isinstance(text, list):
             if len(text) == 0:
                 raise ValueError('Input text list cannot be empty')
+            input_context = text
         if prompt_modifier is None:
             prompt_modifier = self._init_prompt()
         else:
             if not isinstance(prompt_modifier, list):
                 raise TypeError('Input prompt modifier needs to be of type: list')
         if not isinstance(chat_role, str):
             raise TypeError('Input chat role needs to be of type: string')
```

### Comparing `panml-0.0.22/panml/models.py` & `panml-0.0.23/panml/models.py`

 * *Files identical despite different names*

### Comparing `panml-0.0.22/panml/search.py` & `panml-0.0.23/panml/search.py`

 * *Files identical despite different names*

### Comparing `panml-0.0.22/panml.egg-info/PKG-INFO` & `panml-0.0.23/panml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panml
-Version: 0.0.22
+Version: 0.0.23
 Summary: PanML is a high level generative AI/ML development library designed for ease of use and fast experimentation.
 Home-page: https://github.com/Pan-ML/panml
 Author: PanML team
 Author-email: teampanml@gmail.com
 License: MIT
 Keywords: generative AI,generative model,machine learning,large language model,LLM,prompt engineering,fine tuning,prompt tuning,retrieval augmentation,AI safety,AI alignment
 Platform: UNKNOWN
```

### Comparing `panml-0.0.22/setup.py` & `panml-0.0.23/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding="utf-8")
 
 setup(
   name = 'panml', # package name     
   packages = find_packages(exclude=['test']), # package name
-  version = '0.0.22', # version
+  version = '0.0.23', # version
   license = 'MIT', # license
   description = 'PanML is a high level generative AI/ML development library designed for ease of use and fast experimentation.', # short description about the package
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'PanML team', # team name
   author_email = 'teampanml@gmail.com', # contact email
   url = 'https://github.com/Pan-ML/panml', # url link
```

### Comparing `panml-0.0.22/test/test_ModelPack.py` & `panml-0.0.23/test/test_ModelPack.py`

 * *Files identical despite different names*

### Comparing `panml-0.0.22/test/test_VectorEngine.py` & `panml-0.0.23/test/test_VectorEngine.py`

 * *Files identical despite different names*

