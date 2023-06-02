# Comparing `tmp/pypixelai-0.2.0.tar.gz` & `tmp/pypixelai-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypixelai-0.2.0.tar", max compression
+gzip compressed data, was "pypixelai-0.2.1.tar", max compression
```

## Comparing `pypixelai-0.2.0.tar` & `pypixelai-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1060 2023-06-01 17:01:54.973143 pypixelai-0.2.0/LICENSE
--rw-r--r--   0        0        0     3411 2023-06-02 10:33:23.984832 pypixelai-0.2.0/README.md
--rw-r--r--   0        0        0     8056 2023-06-02 09:17:25.760870 pypixelai-0.2.0/pypixelai/__init__.py
--rw-r--r--   0        0        0      704 2023-06-02 09:17:25.761230 pypixelai-0.2.0/pypixelai/constants.py
--rw-r--r--   0        0        0     2108 2023-06-02 09:17:25.761719 pypixelai-0.2.0/pypixelai/exceptions.py
--rw-r--r--   0        0        0      111 2023-06-02 09:17:25.762384 pypixelai-0.2.0/pypixelai/models/__init__.py
--rw-r--r--   0        0        0     1994 2023-06-02 09:40:51.216881 pypixelai-0.2.0/pypixelai/models/base.py
--rw-r--r--   0        0        0     1130 2023-06-02 09:17:25.763028 pypixelai-0.2.0/pypixelai/models/cohere.py
--rw-r--r--   0        0        0     4403 2023-06-02 09:17:25.763326 pypixelai-0.2.0/pypixelai/models/openai.py
--rw-r--r--   0        0        0      959 2023-06-02 09:17:25.763563 pypixelai-0.2.0/pypixelai/models/starcoder.py
--rw-r--r--   0        0        0      199 2023-06-02 09:17:25.763957 pypixelai-0.2.0/pypixelai/prompts/__init__.py
--rw-r--r--   0        0        0      535 2023-06-02 09:17:25.764188 pypixelai-0.2.0/pypixelai/prompts/edit_image.py
--rw-r--r--   0        0        0      819 2023-06-02 09:17:25.764387 pypixelai-0.2.0/pypixelai/prompts/fix_errors.py
--rw-r--r--   0        0        0      991 2023-06-02 09:17:25.764555 pypixelai-0.2.0/pypixelai/prompts/generate_code.py
--rw-r--r--   0        0        0      541 2023-06-02 09:17:25.764724 pypixelai-0.2.0/pypixelai/prompts/generate_image.py
--rw-r--r--   0        0        0      603 2023-06-02 09:17:25.764890 pypixelai-0.2.0/pypixelai/prompts/prompt.py
--rw-r--r--   0        0        0     1237 2023-06-02 10:40:00.091004 pypixelai-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4547 1970-01-01 00:00:00.000000 pypixelai-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-06-01 17:01:54.973143 pypixelai-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3259 2023-06-02 11:03:36.225014 pypixelai-0.2.1/README.md
+-rw-r--r--   0        0        0     8056 2023-06-02 09:17:25.760870 pypixelai-0.2.1/pypixelai/__init__.py
+-rw-r--r--   0        0        0      704 2023-06-02 09:17:25.761230 pypixelai-0.2.1/pypixelai/constants.py
+-rw-r--r--   0        0        0     2108 2023-06-02 09:17:25.761719 pypixelai-0.2.1/pypixelai/exceptions.py
+-rw-r--r--   0        0        0      111 2023-06-02 09:17:25.762384 pypixelai-0.2.1/pypixelai/models/__init__.py
+-rw-r--r--   0        0        0     1988 2023-06-02 11:06:39.821504 pypixelai-0.2.1/pypixelai/models/base.py
+-rw-r--r--   0        0        0     1130 2023-06-02 09:17:25.763028 pypixelai-0.2.1/pypixelai/models/cohere.py
+-rw-r--r--   0        0        0     4403 2023-06-02 09:17:25.763326 pypixelai-0.2.1/pypixelai/models/openai.py
+-rw-r--r--   0        0        0      959 2023-06-02 09:17:25.763563 pypixelai-0.2.1/pypixelai/models/starcoder.py
+-rw-r--r--   0        0        0      199 2023-06-02 09:17:25.763957 pypixelai-0.2.1/pypixelai/prompts/__init__.py
+-rw-r--r--   0        0        0      535 2023-06-02 09:17:25.764188 pypixelai-0.2.1/pypixelai/prompts/edit_image.py
+-rw-r--r--   0        0        0      819 2023-06-02 09:17:25.764387 pypixelai-0.2.1/pypixelai/prompts/fix_errors.py
+-rw-r--r--   0        0        0      991 2023-06-02 09:17:25.764555 pypixelai-0.2.1/pypixelai/prompts/generate_code.py
+-rw-r--r--   0        0        0      541 2023-06-02 09:17:25.764724 pypixelai-0.2.1/pypixelai/prompts/generate_image.py
+-rw-r--r--   0        0        0      603 2023-06-02 09:17:25.764890 pypixelai-0.2.1/pypixelai/prompts/prompt.py
+-rw-r--r--   0        0        0     1237 2023-06-02 11:07:40.377656 pypixelai-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4395 1970-01-01 00:00:00.000000 pypixelai-0.2.1/PKG-INFO
```

### Comparing `pypixelai-0.2.0/LICENSE` & `pypixelai-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pypixelai-0.2.0/README.md` & `pypixelai-0.2.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 # pypixel
 [![Code Quality](https://github.com/navneetdesai/pypixel/actions/workflows/code-quality.yml/badge.svg)](https://github.com/navneetdesai/pypixel/actions/workflows/code-quality.yml)
-[![Code coverage](https://img.shields.io/badge/codecoverage-73%25-green.svg)](#)
-![Tests](https://img.shields.io/badge/Tests-40-blue)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 
 
 Pypixel is an NLP-powered code generation tool for image processing.
 With Pypixel, you can generate Python code snippets for a wide range
 of image processing tasks, such as applying filters, performing transformations,
 extracting features, and more. Harness the power of natural language prompts
@@ -15,15 +13,14 @@
 
 
 
 ## Table of Contents
 
 - [Features](#features)
 - [Installation](#installation)
-- [Usage](#usage)
 - [Examples](#examples)
 - [Contributing](#contributing)
 - [License](#license)
 
 ## Features
 
 - **Natural language code generation**: Generate Python code snippets for image processing tasks using natural language prompts.
```

### Comparing `pypixelai-0.2.0/pypixelai/__init__.py` & `pypixelai-0.2.1/pypixelai/__init__.py`

 * *Files identical despite different names*

### Comparing `pypixelai-0.2.0/pypixelai/constants.py` & `pypixelai-0.2.1/pypixelai/constants.py`

 * *Files identical despite different names*

### Comparing `pypixelai-0.2.0/pypixelai/exceptions.py` & `pypixelai-0.2.1/pypixelai/exceptions.py`

 * *Files identical despite different names*

### Comparing `pypixelai-0.2.0/pypixelai/models/base.py` & `pypixelai-0.2.1/pypixelai/models/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     @staticmethod
     def read_secrets(secrets_file: str) -> dict:
         """
         Read the secrets file and return the secrets
         :param secrets_file:
         :return:
         """
-        if env_vars := dotenv_values("../../.env"):
+        if env_vars := dotenv_values(".env"):
             return env_vars
         try:
             current_dir = os.path.dirname(os.path.abspath(__file__))
             secrets_file = os.path.join(current_dir, secrets_file)
             with open(secrets_file) as f:
                 return json.load(f)
         except FileNotFoundError as e:
```

### Comparing `pypixelai-0.2.0/pypixelai/models/cohere.py` & `pypixelai-0.2.1/pypixelai/models/cohere.py`

 * *Files identical despite different names*

### Comparing `pypixelai-0.2.0/pypixelai/models/openai.py` & `pypixelai-0.2.1/pypixelai/models/openai.py`

 * *Files identical despite different names*

### Comparing `pypixelai-0.2.0/pypixelai/models/starcoder.py` & `pypixelai-0.2.1/pypixelai/models/starcoder.py`

 * *Files identical despite different names*

### Comparing `pypixelai-0.2.0/pypixelai/prompts/edit_image.py` & `pypixelai-0.2.1/pypixelai/prompts/edit_image.py`

 * *Files identical despite different names*

### Comparing `pypixelai-0.2.0/pypixelai/prompts/fix_errors.py` & `pypixelai-0.2.1/pypixelai/prompts/fix_errors.py`

 * *Files identical despite different names*

### Comparing `pypixelai-0.2.0/pypixelai/prompts/generate_code.py` & `pypixelai-0.2.1/pypixelai/prompts/generate_code.py`

 * *Files identical despite different names*

### Comparing `pypixelai-0.2.0/pypixelai/prompts/generate_image.py` & `pypixelai-0.2.1/pypixelai/prompts/generate_image.py`

 * *Files identical despite different names*

### Comparing `pypixelai-0.2.0/pypixelai/prompts/prompt.py` & `pypixelai-0.2.1/pypixelai/prompts/prompt.py`

 * *Files identical despite different names*

### Comparing `pypixelai-0.2.0/pyproject.toml` & `pypixelai-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pypixelai"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Navneet Desai", email="navneetdesai44@gmail.com" },
 ]
 description = "Image processing made easy."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -14,15 +14,15 @@
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/navneetdesai/pypixel"
 
 [tool.poetry]
 name = "pypixelai"
-version = "0.2.0"
+version = "0.2.1"
 description = "Image processing made easy"
 authors = ["Navneet Desai <navneetdesai44@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pre-commit = "^3.3.2"
```

### Comparing `pypixelai-0.2.0/PKG-INFO` & `pypixelai-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypixelai
-Version: 0.2.0
+Version: 0.2.1
 Summary: Image processing made easy
 Author: Navneet Desai
 Author-email: navneetdesai44@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -26,16 +26,14 @@
 Requires-Dist: pytest-mock (>=3.10.0,<4.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # pypixel
 [![Code Quality](https://github.com/navneetdesai/pypixel/actions/workflows/code-quality.yml/badge.svg)](https://github.com/navneetdesai/pypixel/actions/workflows/code-quality.yml)
-[![Code coverage](https://img.shields.io/badge/codecoverage-73%25-green.svg)](#)
-![Tests](https://img.shields.io/badge/Tests-40-blue)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 
 
 Pypixel is an NLP-powered code generation tool for image processing.
 With Pypixel, you can generate Python code snippets for a wide range
 of image processing tasks, such as applying filters, performing transformations,
 extracting features, and more. Harness the power of natural language prompts
@@ -45,15 +43,14 @@
 
 
 
 ## Table of Contents
 
 - [Features](#features)
 - [Installation](#installation)
-- [Usage](#usage)
 - [Examples](#examples)
 - [Contributing](#contributing)
 - [License](#license)
 
 ## Features
 
 - **Natural language code generation**: Generate Python code snippets for image processing tasks using natural language prompts.
```

