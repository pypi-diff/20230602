# Comparing `tmp/manubot-ai-editor-0.4.4.tar.gz` & `tmp/manubot-ai-editor-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manubot-ai-editor-0.4.4.tar", last modified: Thu Jun  1 19:58:35 2023, max compression
+gzip compressed data, was "manubot-ai-editor-0.4.5.tar", last modified: Fri Jun  2 14:13:38 2023, max compression
```

## Comparing `manubot-ai-editor-0.4.4.tar` & `manubot-ai-editor-0.4.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-06-01 19:58:35.896522 manubot-ai-editor-0.4.4/
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     2544 2023-06-01 19:58:35.896522 manubot-ai-editor-0.4.4/PKG-INFO
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     2062 2023-06-01 16:26:59.000000 manubot-ai-editor-0.4.4/README.md
-drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-06-01 19:58:35.896522 manubot-ai-editor-0.4.4/libs/
-drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-06-01 19:58:35.896522 manubot-ai-editor-0.4.4/libs/manubot_ai_editor/
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)        0 2023-01-26 21:56:19.000000 manubot-ai-editor-0.4.4/libs/manubot_ai_editor/__init__.py
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)    16883 2023-06-01 19:57:14.000000 manubot-ai-editor-0.4.4/libs/manubot_ai_editor/editor.py
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     2965 2023-06-01 19:38:16.000000 manubot-ai-editor-0.4.4/libs/manubot_ai_editor/env_vars.py
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)    20582 2023-06-01 16:43:05.000000 manubot-ai-editor-0.4.4/libs/manubot_ai_editor/models.py
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)      632 2023-01-26 21:56:19.000000 manubot-ai-editor-0.4.4/libs/manubot_ai_editor/utils.py
-drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-06-01 19:58:35.896522 manubot-ai-editor-0.4.4/libs/manubot_ai_editor.egg-info/
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     2544 2023-06-01 19:58:35.000000 manubot-ai-editor-0.4.4/libs/manubot_ai_editor.egg-info/PKG-INFO
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)      498 2023-06-01 19:58:35.000000 manubot-ai-editor-0.4.4/libs/manubot_ai_editor.egg-info/SOURCES.txt
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)        1 2023-06-01 19:58:35.000000 manubot-ai-editor-0.4.4/libs/manubot_ai_editor.egg-info/dependency_links.txt
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)       20 2023-06-01 19:58:35.000000 manubot-ai-editor-0.4.4/libs/manubot_ai_editor.egg-info/requires.txt
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)       19 2023-06-01 19:58:35.000000 manubot-ai-editor-0.4.4/libs/manubot_ai_editor.egg-info/top_level.txt
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)       38 2023-06-01 19:58:35.896522 manubot-ai-editor-0.4.4/setup.cfg
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)      938 2023-06-01 19:58:06.000000 manubot-ai-editor-0.4.4/setup.py
-drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-06-01 19:58:35.896522 manubot-ai-editor-0.4.4/tests/
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)    61034 2023-06-01 15:22:56.000000 manubot-ai-editor-0.4.4/tests/test_completion_model.py
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)    41575 2023-06-01 19:57:26.000000 manubot-ai-editor-0.4.4/tests/test_editor.py
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     7738 2023-06-01 16:46:08.000000 manubot-ai-editor-0.4.4/tests/test_model_get_prompt.py
+drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-06-02 14:13:38.236326 manubot-ai-editor-0.4.5/
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     2544 2023-06-02 14:13:38.236326 manubot-ai-editor-0.4.5/PKG-INFO
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     2062 2023-06-01 16:26:59.000000 manubot-ai-editor-0.4.5/README.md
+drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-06-02 14:13:38.236326 manubot-ai-editor-0.4.5/libs/
+drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-06-02 14:13:38.236326 manubot-ai-editor-0.4.5/libs/manubot_ai_editor/
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)        0 2023-01-26 21:56:19.000000 manubot-ai-editor-0.4.5/libs/manubot_ai_editor/__init__.py
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)    16883 2023-06-01 19:57:14.000000 manubot-ai-editor-0.4.5/libs/manubot_ai_editor/editor.py
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     3399 2023-06-02 13:56:51.000000 manubot-ai-editor-0.4.5/libs/manubot_ai_editor/env_vars.py
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)    20582 2023-06-01 16:43:05.000000 manubot-ai-editor-0.4.5/libs/manubot_ai_editor/models.py
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)      632 2023-01-26 21:56:19.000000 manubot-ai-editor-0.4.5/libs/manubot_ai_editor/utils.py
+drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-06-02 14:13:38.236326 manubot-ai-editor-0.4.5/libs/manubot_ai_editor.egg-info/
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     2544 2023-06-02 14:13:38.000000 manubot-ai-editor-0.4.5/libs/manubot_ai_editor.egg-info/PKG-INFO
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)      498 2023-06-02 14:13:38.000000 manubot-ai-editor-0.4.5/libs/manubot_ai_editor.egg-info/SOURCES.txt
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)        1 2023-06-02 14:13:38.000000 manubot-ai-editor-0.4.5/libs/manubot_ai_editor.egg-info/dependency_links.txt
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)       20 2023-06-02 14:13:38.000000 manubot-ai-editor-0.4.5/libs/manubot_ai_editor.egg-info/requires.txt
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)       19 2023-06-02 14:13:38.000000 manubot-ai-editor-0.4.5/libs/manubot_ai_editor.egg-info/top_level.txt
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)       38 2023-06-02 14:13:38.236326 manubot-ai-editor-0.4.5/setup.cfg
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)      938 2023-06-02 14:13:22.000000 manubot-ai-editor-0.4.5/setup.py
+drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-06-02 14:13:38.236326 manubot-ai-editor-0.4.5/tests/
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)    61034 2023-06-01 15:22:56.000000 manubot-ai-editor-0.4.5/tests/test_completion_model.py
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)    41575 2023-06-01 19:57:26.000000 manubot-ai-editor-0.4.5/tests/test_editor.py
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     7738 2023-06-01 16:46:08.000000 manubot-ai-editor-0.4.5/tests/test_model_get_prompt.py
```

### Comparing `manubot-ai-editor-0.4.4/PKG-INFO` & `manubot-ai-editor-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manubot-ai-editor
-Version: 0.4.4
+Version: 0.4.5
 Summary: A Manubot plugin to revise a manuscript using GPT-3
 Home-page: https://github.com/greenelab/manubot-ai-editor
 Author: Milton Pividori
 Author-email: miltondp@gmail.com
 License: BSD-2-Clause Plus Patent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `manubot-ai-editor-0.4.4/README.md` & `manubot-ai-editor-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `manubot-ai-editor-0.4.4/libs/manubot_ai_editor/editor.py` & `manubot-ai-editor-0.4.5/libs/manubot_ai_editor/editor.py`

 * *Files identical despite different names*

### Comparing `manubot-ai-editor-0.4.4/libs/manubot_ai_editor/env_vars.py` & `manubot-ai-editor-0.4.5/libs/manubot_ai_editor/env_vars.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 """
 This file contains environment variables names used by manubot-ai-editor
-package. Several of them allow to specify different parameters when calling the
-OpenAI model, such as LAGUANGE_MODEL or MAX_TOKENS_PER_REQUEST. For this, see
-more details in https://beta.openai.com/docs/api-reference/completions/create
+package. They allow to specify different parameters when calling the
+OpenAI model, such as the language model or the maximum tokens per request
+(see more details in https://beta.openai.com/docs/api-reference/completions/create).
+
+If you are using our GitHub Actions workflow provided by manubot/rootstock, you need
+to modify the "Revise manuscript" step in the workflow file (.github/workflows/ai-revision.yaml)
+by adding the environment variable name specificed in the _value_ of the variables. For instance,
+if you want to provide a custom prompt, then you need to add a line like this to the workflow:
+
+    AI_EDITOR_CUSTOM_PROMPT="proofread the following paragraph"
 """
 
 # OpenAI API key to use
 OPENAI_API_KEY = "OPENAI_API_KEY"
 
 # Language model to use. For example, "text-davinci-003", "gpt-3.5-turbo", "gpt-3.5-turbo-0301", etc
 LANGUAGE_MODEL = "AI_EDITOR_LANGUAGE_MODEL"
```

### Comparing `manubot-ai-editor-0.4.4/libs/manubot_ai_editor/models.py` & `manubot-ai-editor-0.4.5/libs/manubot_ai_editor/models.py`

 * *Files identical despite different names*

### Comparing `manubot-ai-editor-0.4.4/libs/manubot_ai_editor/utils.py` & `manubot-ai-editor-0.4.5/libs/manubot_ai_editor/utils.py`

 * *Files identical despite different names*

### Comparing `manubot-ai-editor-0.4.4/libs/manubot_ai_editor.egg-info/PKG-INFO` & `manubot-ai-editor-0.4.5/libs/manubot_ai_editor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manubot-ai-editor
-Version: 0.4.4
+Version: 0.4.5
 Summary: A Manubot plugin to revise a manuscript using GPT-3
 Home-page: https://github.com/greenelab/manubot-ai-editor
 Author: Milton Pividori
 Author-email: miltondp@gmail.com
 License: BSD-2-Clause Plus Patent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `manubot-ai-editor-0.4.4/setup.py` & `manubot-ai-editor-0.4.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # twine upload dist/*
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="manubot-ai-editor",
-    version="0.4.4",
+    version="0.4.5",
     author="Milton Pividori",
     author_email="miltondp@gmail.com",
     description="A Manubot plugin to revise a manuscript using GPT-3",
     license="BSD-2-Clause Plus Patent",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/greenelab/manubot-ai-editor",
```

### Comparing `manubot-ai-editor-0.4.4/tests/test_completion_model.py` & `manubot-ai-editor-0.4.5/tests/test_completion_model.py`

 * *Files identical despite different names*

### Comparing `manubot-ai-editor-0.4.4/tests/test_editor.py` & `manubot-ai-editor-0.4.5/tests/test_editor.py`

 * *Files identical despite different names*

### Comparing `manubot-ai-editor-0.4.4/tests/test_model_get_prompt.py` & `manubot-ai-editor-0.4.5/tests/test_model_get_prompt.py`

 * *Files identical despite different names*

