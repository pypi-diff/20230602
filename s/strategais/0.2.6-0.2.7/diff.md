# Comparing `tmp/strategais-0.2.6.tar.gz` & `tmp/strategais-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strategais-0.2.6.tar", last modified: Fri Jun  2 13:52:46 2023, max compression
+gzip compressed data, was "strategais-0.2.7.tar", last modified: Fri Jun  2 15:04:17 2023, max compression
```

## Comparing `strategais-0.2.6.tar` & `strategais-0.2.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-02 13:52:46.840149 strategais-0.2.6/
--rw-r--r--   0 collin     (501) staff       (20)     1066 2023-05-26 03:15:25.000000 strategais-0.2.6/LICENSE
--rw-r--r--   0 collin     (501) staff       (20)     1305 2023-06-02 13:52:46.839982 strategais-0.2.6/PKG-INFO
--rw-r--r--   0 collin     (501) staff       (20)     1096 2023-06-02 03:54:08.000000 strategais-0.2.6/README.md
--rw-r--r--   0 collin     (501) staff       (20)       38 2023-06-02 13:52:46.840204 strategais-0.2.6/setup.cfg
--rw-r--r--   0 collin     (501) staff       (20)     1459 2023-06-02 12:21:36.000000 strategais-0.2.6/setup.py
-drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-02 13:52:46.836483 strategais-0.2.6/strategais/
--rw-r--r--   0 collin     (501) staff       (20)       78 2023-06-01 03:43:48.000000 strategais-0.2.6/strategais/__init__.py
--rw-r--r--   0 collin     (501) staff       (20)     4679 2023-06-02 12:49:21.000000 strategais-0.2.6/strategais/__main__.py
--rw-r--r--   0 collin     (501) staff       (20)      368 2023-05-31 04:51:38.000000 strategais-0.2.6/strategais/llm_tools.py
--rw-r--r--   0 collin     (501) staff       (20)     2280 2023-05-31 04:07:36.000000 strategais-0.2.6/strategais/save_tools.py
-drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-02 13:52:46.838104 strategais-0.2.6/strategais/templates/
--rw-r--r--   0 collin     (501) staff       (20)    18358 2023-06-01 03:39:47.000000 strategais-0.2.6/strategais/templates/index.html
-drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-02 13:52:46.837457 strategais-0.2.6/strategais.egg-info/
--rw-r--r--   0 collin     (501) staff       (20)     1305 2023-06-02 13:52:46.000000 strategais-0.2.6/strategais.egg-info/PKG-INFO
--rw-r--r--   0 collin     (501) staff       (20)      322 2023-06-02 13:52:46.000000 strategais-0.2.6/strategais.egg-info/SOURCES.txt
--rw-r--r--   0 collin     (501) staff       (20)        1 2023-06-02 13:52:46.000000 strategais-0.2.6/strategais.egg-info/dependency_links.txt
--rw-r--r--   0 collin     (501) staff       (20)      463 2023-06-02 13:52:46.000000 strategais-0.2.6/strategais.egg-info/requires.txt
--rw-r--r--   0 collin     (501) staff       (20)       11 2023-06-02 13:52:46.000000 strategais-0.2.6/strategais.egg-info/top_level.txt
+drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-02 15:04:17.015421 strategais-0.2.7/
+-rw-r--r--   0 collin     (501) staff       (20)     1066 2023-05-26 03:15:25.000000 strategais-0.2.7/LICENSE
+-rw-r--r--   0 collin     (501) staff       (20)     1305 2023-06-02 15:04:17.015274 strategais-0.2.7/PKG-INFO
+-rw-r--r--   0 collin     (501) staff       (20)     1096 2023-06-02 14:50:13.000000 strategais-0.2.7/README.md
+-rw-r--r--   0 collin     (501) staff       (20)       38 2023-06-02 15:04:17.015464 strategais-0.2.7/setup.cfg
+-rw-r--r--   0 collin     (501) staff       (20)     1459 2023-06-02 15:03:49.000000 strategais-0.2.7/setup.py
+drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-02 15:04:17.013474 strategais-0.2.7/strategais/
+-rw-r--r--   0 collin     (501) staff       (20)       78 2023-06-02 14:50:13.000000 strategais-0.2.7/strategais/__init__.py
+-rw-r--r--   0 collin     (501) staff       (20)     4749 2023-06-02 15:03:41.000000 strategais-0.2.7/strategais/__main__.py
+-rw-r--r--   0 collin     (501) staff       (20)      368 2023-05-31 04:51:38.000000 strategais-0.2.7/strategais/llm_tools.py
+-rw-r--r--   0 collin     (501) staff       (20)     2280 2023-05-31 04:07:36.000000 strategais-0.2.7/strategais/save_tools.py
+drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-02 15:04:17.014738 strategais-0.2.7/strategais/templates/
+-rw-r--r--   0 collin     (501) staff       (20)    18358 2023-06-02 14:50:13.000000 strategais-0.2.7/strategais/templates/index.html
+drwxr-xr-x   0 collin     (501) staff       (20)        0 2023-06-02 15:04:17.014586 strategais-0.2.7/strategais.egg-info/
+-rw-r--r--   0 collin     (501) staff       (20)     1305 2023-06-02 15:04:17.000000 strategais-0.2.7/strategais.egg-info/PKG-INFO
+-rw-r--r--   0 collin     (501) staff       (20)      322 2023-06-02 15:04:17.000000 strategais-0.2.7/strategais.egg-info/SOURCES.txt
+-rw-r--r--   0 collin     (501) staff       (20)        1 2023-06-02 15:04:17.000000 strategais-0.2.7/strategais.egg-info/dependency_links.txt
+-rw-r--r--   0 collin     (501) staff       (20)      463 2023-06-02 15:04:17.000000 strategais-0.2.7/strategais.egg-info/requires.txt
+-rw-r--r--   0 collin     (501) staff       (20)       11 2023-06-02 15:04:17.000000 strategais-0.2.7/strategais.egg-info/top_level.txt
```

### Comparing `strategais-0.2.6/LICENSE` & `strategais-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `strategais-0.2.6/PKG-INFO` & `strategais-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strategais
-Version: 0.2.6
+Version: 0.2.7
 Summary: A Python library for deploying large language models (LLMs) in local environments.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Strategais
 
 ## 🚀 Quick Install
```

### Comparing `strategais-0.2.6/README.md` & `strategais-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `strategais-0.2.6/setup.py` & `strategais-0.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='strategais',
-    version='0.2.6', 
+    version='0.2.7', 
     description='A Python library for deploying large language models (LLMs) in local environments.',
     long_description=long_description,
     long_description_content_type="text/markdown", 
     packages=find_packages(),
     package_data={'strategais': ['templates/*.html', 'static/*.js', 'static/*.css' , 'models/*.sav']},
     install_requires=[
         'fastapi',
```

### Comparing `strategais-0.2.6/strategais/__main__.py` & `strategais-0.2.7/strategais/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,19 +59,19 @@
 if args.llm:
     spec = importlib.util.spec_from_file_location("llm", args.llm)
     llm_module = importlib.util.module_from_spec(spec)
     spec.loader.exec_module(llm_module)
     chatbot = llm_module.main_chat()
 else:
     def main_chat(question):
-        models_dir = pkg_resources.resource_filename('strategais', 'models')
-        model_file = 'model.sav'
-        tokenizer_file = 'tokenizer.sav'
-        model = load_model(f'{models_dir}/{model_file}')
-        tokenizer = load_tokenizer(f'{models_dir}/{tokenizer_file}')
+        # models_dir = pkg_resources.resource_filename('strategais', 'models')
+        # model_file = 'model.sav'
+        # tokenizer_file = 'tokenizer.sav'
+        model = load_model('https://github.com/professai/strategais/raw/main/model.sav')
+        tokenizer = load_tokenizer('https://github.com/professai/strategais/raw/main/tokenizer.sav')
 
         input_text = question
 
         input_ids = tokenizer(input_text, return_tensors="pt").input_ids.to('cpu')
 
         outputs = model.generate(input_ids, max_length=10000)
         return tokenizer.decode(outputs[0], skip_special_tokens=True)
```

### Comparing `strategais-0.2.6/strategais/save_tools.py` & `strategais-0.2.7/strategais/save_tools.py`

 * *Files identical despite different names*

### Comparing `strategais-0.2.6/strategais/templates/index.html` & `strategais-0.2.7/strategais/templates/index.html`

 * *Files identical despite different names*

### Comparing `strategais-0.2.6/strategais.egg-info/PKG-INFO` & `strategais-0.2.7/strategais.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strategais
-Version: 0.2.6
+Version: 0.2.7
 Summary: A Python library for deploying large language models (LLMs) in local environments.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Strategais
 
 ## 🚀 Quick Install
```

