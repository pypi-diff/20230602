# Comparing `tmp/idoctorai-0.1.5.tar.gz` & `tmp/idoctorai-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idoctorai-0.1.5.tar", max compression
+gzip compressed data, was "idoctorai-0.1.6.tar", max compression
```

## Comparing `idoctorai-0.1.5.tar` & `idoctorai-0.1.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1077 2023-05-31 07:10:59.339636 idoctorai-0.1.5/LICENSE
--rw-r--r--   0        0        0    16565 2023-05-31 09:14:44.387529 idoctorai-0.1.5/pandasai/__init__.py
--rw-r--r--   0        0        0     1200 2023-05-31 07:10:59.362575 idoctorai-0.1.5/pandasai/constants.py
--rw-r--r--   0        0        0     1001 2023-05-31 07:10:59.362575 idoctorai-0.1.5/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.362575 idoctorai-0.1.5/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     5529 2023-05-31 07:10:59.363572 idoctorai-0.1.5/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0      593 2023-05-31 07:10:59.363572 idoctorai-0.1.5/pandasai/helpers/from_excel.py
--rw-r--r--   0        0        0     1537 2023-05-31 07:10:59.363572 idoctorai-0.1.5/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0     2723 2023-05-31 07:10:59.364569 idoctorai-0.1.5/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.364569 idoctorai-0.1.5/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     4456 2023-05-31 07:10:59.365592 idoctorai-0.1.5/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0    11245 2023-05-31 07:10:59.365592 idoctorai-0.1.5/pandasai/llm/base.py
--rw-r--r--   0        0        0      566 2023-05-31 07:10:59.366593 idoctorai-0.1.5/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1913 2023-05-31 07:10:59.366593 idoctorai-0.1.5/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0     1535 2023-05-31 07:10:59.367662 idoctorai-0.1.5/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     2973 2023-05-31 07:10:59.367662 idoctorai-0.1.5/pandasai/llm/openai.py
--rw-r--r--   0        0        0     1269 2023-05-31 07:10:59.368559 idoctorai-0.1.5/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.368559 idoctorai-0.1.5/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0      764 2023-05-31 07:10:59.368559 idoctorai-0.1.5/pandasai/prompts/base.py
--rw-r--r--   0        0        0     1845 2023-05-31 07:10:59.369581 idoctorai-0.1.5/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0     1381 2023-05-31 07:10:59.369581 idoctorai-0.1.5/pandasai/prompts/correct_multiples_prompt.py
--rw-r--r--   0        0        0     1646 2023-05-31 07:10:59.370561 idoctorai-0.1.5/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      528 2023-05-31 07:10:59.370561 idoctorai-0.1.5/pandasai/prompts/generate_response.py
--rw-r--r--   0        0        0     1455 2023-05-31 07:10:59.371552 idoctorai-0.1.5/pandasai/prompts/multiple_dataframes.py
--rw-r--r--   0        0        0     1080 2023-06-01 01:15:02.064966 idoctorai-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       33 2023-05-31 09:11:00.839811 idoctorai-0.1.5/README.md
--rw-r--r--   0        0        0      803 1970-01-01 00:00:00.000000 idoctorai-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-31 07:10:59.339636 idoctorai-0.1.6/LICENSE
+-rw-r--r--   0        0        0    16565 2023-06-02 04:05:23.763126 idoctorai-0.1.6/pandasai/__init__.py
+-rw-r--r--   0        0        0     1200 2023-06-02 03:38:48.762886 idoctorai-0.1.6/pandasai/constants.py
+-rw-r--r--   0        0        0     1001 2023-06-02 03:38:48.762886 idoctorai-0.1.6/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.362575 idoctorai-0.1.6/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     5529 2023-05-31 07:10:59.363572 idoctorai-0.1.6/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0      593 2023-05-31 07:10:59.363572 idoctorai-0.1.6/pandasai/helpers/from_excel.py
+-rw-r--r--   0        0        0     1537 2023-05-31 07:10:59.363572 idoctorai-0.1.6/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     2723 2023-05-31 07:10:59.364569 idoctorai-0.1.6/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.364569 idoctorai-0.1.6/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     4456 2023-05-31 07:10:59.365592 idoctorai-0.1.6/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    11245 2023-06-02 03:38:48.763883 idoctorai-0.1.6/pandasai/llm/base.py
+-rw-r--r--   0        0        0      566 2023-05-31 07:10:59.366593 idoctorai-0.1.6/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1913 2023-05-31 07:10:59.366593 idoctorai-0.1.6/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0     1535 2023-05-31 07:10:59.367662 idoctorai-0.1.6/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     2973 2023-05-31 07:10:59.367662 idoctorai-0.1.6/pandasai/llm/openai.py
+-rw-r--r--   0        0        0     1269 2023-05-31 07:10:59.368559 idoctorai-0.1.6/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.368559 idoctorai-0.1.6/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0      764 2023-05-31 07:10:59.368559 idoctorai-0.1.6/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1845 2023-05-31 07:10:59.369581 idoctorai-0.1.6/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     1381 2023-05-31 07:10:59.369581 idoctorai-0.1.6/pandasai/prompts/correct_multiples_prompt.py
+-rw-r--r--   0        0        0     1646 2023-05-31 07:10:59.370561 idoctorai-0.1.6/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      528 2023-05-31 07:10:59.370561 idoctorai-0.1.6/pandasai/prompts/generate_response.py
+-rw-r--r--   0        0        0     1511 2023-06-02 04:03:56.645964 idoctorai-0.1.6/pandasai/prompts/multiple_dataframes.py
+-rw-r--r--   0        0        0     1093 2023-06-02 03:41:13.186309 idoctorai-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       33 2023-06-02 03:40:47.303734 idoctorai-0.1.6/README.md
+-rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 idoctorai-0.1.6/PKG-INFO
```

### Comparing `idoctorai-0.1.5/LICENSE` & `idoctorai-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.5/pandasai/__init__.py` & `idoctorai-0.1.6/pandasai/__init__.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.5/pandasai/constants.py` & `idoctorai-0.1.6/pandasai/constants.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.5/pandasai/exceptions.py` & `idoctorai-0.1.6/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.5/pandasai/helpers/anonymizer.py` & `idoctorai-0.1.6/pandasai/helpers/anonymizer.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.5/pandasai/helpers/from_excel.py` & `idoctorai-0.1.6/pandasai/helpers/from_excel.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.5/pandasai/helpers/notebook.py` & `idoctorai-0.1.6/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.5/pandasai/helpers/save_chart.py` & `idoctorai-0.1.6/pandasai/helpers/save_chart.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.5/pandasai/llm/azure_openai.py` & `idoctorai-0.1.6/pandasai/llm/azure_openai.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.5/pandasai/llm/base.py` & `idoctorai-0.1.6/pandasai/llm/base.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.5/pandasai/llm/fake.py` & `idoctorai-0.1.6/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.5/pandasai/llm/google_palm.py` & `idoctorai-0.1.6/pandasai/llm/google_palm.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.5/pandasai/llm/open_assistant.py` & `idoctorai-0.1.6/pandasai/llm/open_assistant.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.5/pandasai/llm/openai.py` & `idoctorai-0.1.6/pandasai/llm/openai.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.5/pandasai/llm/starcoder.py` & `idoctorai-0.1.6/pandasai/llm/starcoder.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.5/pandasai/prompts/base.py` & `idoctorai-0.1.6/pandasai/prompts/base.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.5/pandasai/prompts/correct_error_prompt.py` & `idoctorai-0.1.6/pandasai/prompts/correct_error_prompt.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.5/pandasai/prompts/correct_multiples_prompt.py` & `idoctorai-0.1.6/pandasai/prompts/correct_multiples_prompt.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.5/pandasai/prompts/generate_python_code.py` & `idoctorai-0.1.6/pandasai/prompts/generate_python_code.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.5/pandasai/prompts/generate_response.py` & `idoctorai-0.1.6/pandasai/prompts/generate_response.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.5/pandasai/prompts/multiple_dataframes.py` & `idoctorai-0.1.6/pandasai/prompts/multiple_dataframes.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,18 +21,20 @@
 Using the provided dataframes and no other dataframes, return the python code and make sure to prefix the requested python code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG} exactly to get the answer to the following question:
 """
 
     def __init__(self, dataframes: list[pd.DataFrame]): # pylint: disable=super-init-not-called
         for i, dataframe in enumerate(dataframes, start=1):
             row, col = dataframe.shape
 
+            data_text = dataframe.head().to_string()
+
             self.text += f"""
 Dataframe df{i}, with {row} rows and {col} columns.
 This is the result of `print(df{i}.head())`:
-{dataframe}"""
+{data_text}"""
 
         self.text += self.instruction
         self.text = self.text.format(
             today_date=date.today(),
             START_CODE_TAG=START_CODE_TAG,
             END_CODE_TAG=END_CODE_TAG,
         )
```

### Comparing `idoctorai-0.1.5/pyproject.toml` & `idoctorai-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "idoctorai"
-version = "0.1.5"
-description = "this is idoctor-ai"
-authors = ["HF"]
+version = "0.1.6"
+description = "this is idoctorai"
+authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 python-dotenv = "^1.0.0"
```

### Comparing `idoctorai-0.1.5/PKG-INFO` & `idoctorai-0.1.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: idoctorai
-Version: 0.1.5
-Summary: this is idoctor-ai
+Version: 0.1.6
+Summary: this is idoctorai
 License: MIT
-Author: HF
+Author: Gabriele Venturi
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: google
@@ -16,10 +16,10 @@
 Requires-Dist: ipython (>=8.13.1,<9.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: openai (>=0.27.5,<0.28.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
-## idoctor-nocode-ai
+## idoctorai
 
-no  info 
+this is idoctorai
```

