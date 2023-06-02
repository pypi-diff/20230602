# Comparing `tmp/sleepyask-7.0.0.tar.gz` & `tmp/sleepyask-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleepyask-7.0.0.tar", last modified: Sun May 21 10:08:26 2023, max compression
+gzip compressed data, was "sleepyask-7.1.0.tar", last modified: Fri Jun  2 04:00:29 2023, max compression
```

## Comparing `sleepyask-7.0.0.tar` & `sleepyask-7.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:08:26.071340 sleepyask-7.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-21 10:08:14.000000 sleepyask-7.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-05-21 10:08:26.071340 sleepyask-7.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-05-21 10:08:14.000000 sleepyask-7.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-21 10:08:14.000000 sleepyask-7.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 10:08:26.071340 sleepyask-7.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:08:26.067340 sleepyask-7.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:08:26.071340 sleepyask-7.0.0/src/sleepyask/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:08:14.000000 sleepyask-7.0.0/src/sleepyask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-05-21 10:08:14.000000 sleepyask-7.0.0/src/sleepyask/chat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:08:26.071340 sleepyask-7.0.0/src/sleepyask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-05-21 10:08:26.000000 sleepyask-7.0.0/src/sleepyask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-21 10:08:26.000000 sleepyask-7.0.0/src/sleepyask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 10:08:26.000000 sleepyask-7.0.0/src/sleepyask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-21 10:08:26.000000 sleepyask-7.0.0/src/sleepyask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-21 10:08:26.000000 sleepyask-7.0.0/src/sleepyask.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:00:29.552163 sleepyask-7.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-02 04:00:16.000000 sleepyask-7.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-06-02 04:00:29.552163 sleepyask-7.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-02 04:00:16.000000 sleepyask-7.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-02 04:00:16.000000 sleepyask-7.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 04:00:29.552163 sleepyask-7.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:00:29.548163 sleepyask-7.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:00:29.552163 sleepyask-7.1.0/src/sleepyask/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 04:00:16.000000 sleepyask-7.1.0/src/sleepyask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-02 04:00:16.000000 sleepyask-7.1.0/src/sleepyask/chat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:00:29.552163 sleepyask-7.1.0/src/sleepyask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-06-02 04:00:29.000000 sleepyask-7.1.0/src/sleepyask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-02 04:00:29.000000 sleepyask-7.1.0/src/sleepyask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 04:00:29.000000 sleepyask-7.1.0/src/sleepyask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-02 04:00:29.000000 sleepyask-7.1.0/src/sleepyask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-02 04:00:29.000000 sleepyask-7.1.0/src/sleepyask.egg-info/top_level.txt
```

### Comparing `sleepyask-7.0.0/LICENSE` & `sleepyask-7.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sleepyask-7.0.0/PKG-INFO` & `sleepyask-7.1.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleepyask
-Version: 7.0.0
+Version: 7.1.0
 Summary: A small tool for automating collecting data from ChatGPT
 Author-email: hwelsters <redacted@redacted.redacted>
 Project-URL: Homepage, https://github.com/hwelsters/sleepyask
 Project-URL: Bug Tracker, https://github.com/hwelsters/sleepyask/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -65,58 +65,42 @@
 - `count` - This specifies the number of workers to create for asking questions. You can have multiple workers asking questions in parallel.  
 	
 ### Sample code
 It is recommended that you do not store your user credentials directly in your code. Instead, use something like `python-dotenv` to store your credentials in another file.
 ```python
 import os
 from dotenv import load_dotenv
-from sleepyask.openai import chat
+
+from sleepyask.chat import Sleepyask
 
 load_dotenv()  # take environment variables from .env.
 
-# Your ChatGPT authentication configs
-config = {
-	"organization": os.getenv('OPENAI_ORGANIZATION_1'),
-	"api_key": os.getenv('OPENAI_API_KEY_1'),
-	"count": 1
-}
-
-# List of authentication configs
-configs = [config]
-
-# List of questions you would like to ask ChatGPT
-question_list = ['What is 1 + 1?', 'What is 1 + 2?', 'What is 1 + 3?']
-
-# The filename in which you would like your responses to be stored.
-# sleepyask will create this file for you. If you create it yourself, there might be some problems.
-output_file_path = 'draw.json'  
-
-# Run sleepy_ask
-chat.ask(config=config,
-           questions=question_list,
-           output_file_path=output_file_path,
-           verbose=True)
-```
+TIMEOUT = 10000
+RETRY_TIME = 5
+RATE_LIMIT = 5
+API_KEY = os.getenv('OPENAI_API_KEY')
+
+# Index should be unique as it will be used to avoid repeat questions
+QUESTION_LIST = [
+	{'index': 1, 'text': 'What is 1 + 1?'},
+	{'index': 2, 'text': 'What is 1 + 2?'},
+	{'index': 3, 'text': 'What is 1 + 3?'}
+]
+OUT_PATH = 'output.jsonl'
+
+
+CONFIGS = { "model": "gpt-3.5-turbo", "n": 10, "temperature": 0.7}
+sleepyask = Sleepyask(configs=CONFIGS, 
+                      rate_limit=RATE_LIMIT,
+                      api_key=API_KEY, 
+                      timeout=TIMEOUT, 
+                      verbose=True,
+                      retry_time=RETRY_TIME)
 
-<p align="center">
-  <img src="https://user-images.githubusercontent.com/84760072/227817860-f4aef84b-9992-4ddd-a99d-019566cce0c5.png" width="900" />
-</p>
-
-### Parameters
-`sleepyask.openai.ask` has the following parameters:
-#### Required
-- `configs` :: **(required)** - should be a list of dicts containing `organization` (your OpenAI organization ID), `api key` (your OpenAI api key) and the `count` (the number of instances to spin up for asking questions)
-- `questions` :: **(required)** - should be a list of strings containing questions you would like to ask ChatGPT.
-- `output_file_path` :: **(required)** - should be a valid file path where you would like your responses to be stored. sleepyask will create this file for you. If you create this file yourself, there might be some problems.
-
-#### Optional
-- `verbose` :: **(optional)** - a boolean which specifies whether or not sleepyask should print its progress to the console. It is `False` by default
-- `model` :: **(optional)** - to specify which ChatGPT model to use. It is `"gpt-3.5-turbo"` by default
-- `system_text` :: **(optional)** - to specify system text. It is `
-- `temperature` :: **(optional)** - to specify how deterministic ChatGPT's responses are. Ranges from `0-2` where higher numbers represent increased randomness. It is `1` by default.
-- `max_tokens` :: **(optional)** - to specify the maximum number of tokens in ChatGPT's response. This is `2048` by default
+sleepyask.start(question_list=QUESTION, out_path=OUT_PATH)
+```
 
 ## 💬 Get involved
 - 🐛 **Found a bug or interested in adding a feature?** - Create an [issue][issue]  
 - 🤗 **Want to help?** - Create a pull-request!  
 
 [issue]: https://github.com/hwelsters/sleepyask/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sleepyask Version: 7.0.0 Summary: A small tool for
+Metadata-Version: 2.1 Name: sleepyask Version: 7.1.0 Summary: A small tool for
 automating collecting data from ChatGPT Author-email: hwelsters
 redacted.redacted> Project-URL: Homepage, https://github.com/hwelsters/
 sleepyask Project-URL: Bug Tracker, https://github.com/hwelsters/sleepyask/
 issues Requires-Python: >=3.7 Description-Content-Type: text/markdown License-
 File: LICENSE
  [https://user-images.githubusercontent.com/84760072/227817729-098182f3-6916-
                           48d8-b17a-4e4126ddd245.png]
@@ -25,40 +25,19 @@
 Key. To get it: ```bash > Go to https://platform.openai.com/account/api-keys >
 Login (if it is required) > Click on your profile picture on the top-right >
 View API Keys > Create new secret key. ``` - `count` - This specifies the
 number of workers to create for asking questions. You can have multiple workers
 asking questions in parallel. ### Sample code It is recommended that you do not
 store your user credentials directly in your code. Instead, use something like
 `python-dotenv` to store your credentials in another file. ```python import os
-from dotenv import load_dotenv from sleepyask.openai import chat load_dotenv()
-# take environment variables from .env. # Your ChatGPT authentication configs
-config = { "organization": os.getenv('OPENAI_ORGANIZATION_1'), "api_key":
-os.getenv('OPENAI_API_KEY_1'), "count": 1 } # List of authentication configs
-configs = [config] # List of questions you would like to ask ChatGPT
-question_list = ['What is 1 + 1?', 'What is 1 + 2?', 'What is 1 + 3?'] # The
-filename in which you would like your responses to be stored. # sleepyask will
-create this file for you. If you create it yourself, there might be some
-problems. output_file_path = 'draw.json' # Run sleepy_ask chat.ask
-(config=config, questions=question_list, output_file_path=output_file_path,
-verbose=True) ```
- [https://user-images.githubusercontent.com/84760072/227817860-f4aef84b-9992-
-                          4ddd-a99d-019566cce0c5.png]
-### Parameters `sleepyask.openai.ask` has the following parameters: ####
-Required - `configs` :: **(required)** - should be a list of dicts containing
-`organization` (your OpenAI organization ID), `api key` (your OpenAI api key)
-and the `count` (the number of instances to spin up for asking questions) -
-`questions` :: **(required)** - should be a list of strings containing
-questions you would like to ask ChatGPT. - `output_file_path` :: **(required)**
-- should be a valid file path where you would like your responses to be stored.
-sleepyask will create this file for you. If you create this file yourself,
-there might be some problems. #### Optional - `verbose` :: **(optional)** - a
-boolean which specifies whether or not sleepyask should print its progress to
-the console. It is `False` by default - `model` :: **(optional)** - to specify
-which ChatGPT model to use. It is `"gpt-3.5-turbo"` by default - `system_text`
-:: **(optional)** - to specify system text. It is ` - `temperature` :: **
-(optional)** - to specify how deterministic ChatGPT's responses are. Ranges
-from `0-2` where higher numbers represent increased randomness. It is `1` by
-default. - `max_tokens` :: **(optional)** - to specify the maximum number of
-tokens in ChatGPT's response. This is `2048` by default ## ð¬ Get involved -
-ð **Found a bug or interested in adding a feature?** - Create an [issue]
-[issue] - ð¤ **Want to help?** - Create a pull-request! [issue]: https://
-github.com/hwelsters/sleepyask/issues
+from dotenv import load_dotenv from sleepyask.chat import Sleepyask load_dotenv
+() # take environment variables from .env. TIMEOUT = 10000 RETRY_TIME = 5
+RATE_LIMIT = 5 API_KEY = os.getenv('OPENAI_API_KEY') # Index should be unique
+as it will be used to avoid repeat questions QUESTION_LIST = [ {'index': 1,
+'text': 'What is 1 + 1?'}, {'index': 2, 'text': 'What is 1 + 2?'}, {'index': 3,
+'text': 'What is 1 + 3?'} ] OUT_PATH = 'output.jsonl' CONFIGS = { "model":
+"gpt-3.5-turbo", "n": 10, "temperature": 0.7} sleepyask = Sleepyask
+(configs=CONFIGS, rate_limit=RATE_LIMIT, api_key=API_KEY, timeout=TIMEOUT,
+verbose=True, retry_time=RETRY_TIME) sleepyask.start(question_list=QUESTION,
+out_path=OUT_PATH) ``` ## ð¬ Get involved - ð **Found a bug or interested
+in adding a feature?** - Create an [issue][issue] - ð¤ **Want to help?** -
+Create a pull-request! [issue]: https://github.com/hwelsters/sleepyask/issues
```

### Comparing `sleepyask-7.0.0/README.md` & `sleepyask-7.1.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -54,58 +54,42 @@
 - `count` - This specifies the number of workers to create for asking questions. You can have multiple workers asking questions in parallel.  
 	
 ### Sample code
 It is recommended that you do not store your user credentials directly in your code. Instead, use something like `python-dotenv` to store your credentials in another file.
 ```python
 import os
 from dotenv import load_dotenv
-from sleepyask.openai import chat
+
+from sleepyask.chat import Sleepyask
 
 load_dotenv()  # take environment variables from .env.
 
-# Your ChatGPT authentication configs
-config = {
-	"organization": os.getenv('OPENAI_ORGANIZATION_1'),
-	"api_key": os.getenv('OPENAI_API_KEY_1'),
-	"count": 1
-}
-
-# List of authentication configs
-configs = [config]
-
-# List of questions you would like to ask ChatGPT
-question_list = ['What is 1 + 1?', 'What is 1 + 2?', 'What is 1 + 3?']
-
-# The filename in which you would like your responses to be stored.
-# sleepyask will create this file for you. If you create it yourself, there might be some problems.
-output_file_path = 'draw.json'  
-
-# Run sleepy_ask
-chat.ask(config=config,
-           questions=question_list,
-           output_file_path=output_file_path,
-           verbose=True)
-```
+TIMEOUT = 10000
+RETRY_TIME = 5
+RATE_LIMIT = 5
+API_KEY = os.getenv('OPENAI_API_KEY')
+
+# Index should be unique as it will be used to avoid repeat questions
+QUESTION_LIST = [
+	{'index': 1, 'text': 'What is 1 + 1?'},
+	{'index': 2, 'text': 'What is 1 + 2?'},
+	{'index': 3, 'text': 'What is 1 + 3?'}
+]
+OUT_PATH = 'output.jsonl'
+
+
+CONFIGS = { "model": "gpt-3.5-turbo", "n": 10, "temperature": 0.7}
+sleepyask = Sleepyask(configs=CONFIGS, 
+                      rate_limit=RATE_LIMIT,
+                      api_key=API_KEY, 
+                      timeout=TIMEOUT, 
+                      verbose=True,
+                      retry_time=RETRY_TIME)
 
-<p align="center">
-  <img src="https://user-images.githubusercontent.com/84760072/227817860-f4aef84b-9992-4ddd-a99d-019566cce0c5.png" width="900" />
-</p>
-
-### Parameters
-`sleepyask.openai.ask` has the following parameters:
-#### Required
-- `configs` :: **(required)** - should be a list of dicts containing `organization` (your OpenAI organization ID), `api key` (your OpenAI api key) and the `count` (the number of instances to spin up for asking questions)
-- `questions` :: **(required)** - should be a list of strings containing questions you would like to ask ChatGPT.
-- `output_file_path` :: **(required)** - should be a valid file path where you would like your responses to be stored. sleepyask will create this file for you. If you create this file yourself, there might be some problems.
-
-#### Optional
-- `verbose` :: **(optional)** - a boolean which specifies whether or not sleepyask should print its progress to the console. It is `False` by default
-- `model` :: **(optional)** - to specify which ChatGPT model to use. It is `"gpt-3.5-turbo"` by default
-- `system_text` :: **(optional)** - to specify system text. It is `
-- `temperature` :: **(optional)** - to specify how deterministic ChatGPT's responses are. Ranges from `0-2` where higher numbers represent increased randomness. It is `1` by default.
-- `max_tokens` :: **(optional)** - to specify the maximum number of tokens in ChatGPT's response. This is `2048` by default
+sleepyask.start(question_list=QUESTION, out_path=OUT_PATH)
+```
 
 ## 💬 Get involved
 - 🐛 **Found a bug or interested in adding a feature?** - Create an [issue][issue]  
 - 🤗 **Want to help?** - Create a pull-request!  
 
 [issue]: https://github.com/hwelsters/sleepyask/issues
```

#### html2text {}

```diff
@@ -19,40 +19,19 @@
 Key. To get it: ```bash > Go to https://platform.openai.com/account/api-keys >
 Login (if it is required) > Click on your profile picture on the top-right >
 View API Keys > Create new secret key. ``` - `count` - This specifies the
 number of workers to create for asking questions. You can have multiple workers
 asking questions in parallel. ### Sample code It is recommended that you do not
 store your user credentials directly in your code. Instead, use something like
 `python-dotenv` to store your credentials in another file. ```python import os
-from dotenv import load_dotenv from sleepyask.openai import chat load_dotenv()
-# take environment variables from .env. # Your ChatGPT authentication configs
-config = { "organization": os.getenv('OPENAI_ORGANIZATION_1'), "api_key":
-os.getenv('OPENAI_API_KEY_1'), "count": 1 } # List of authentication configs
-configs = [config] # List of questions you would like to ask ChatGPT
-question_list = ['What is 1 + 1?', 'What is 1 + 2?', 'What is 1 + 3?'] # The
-filename in which you would like your responses to be stored. # sleepyask will
-create this file for you. If you create it yourself, there might be some
-problems. output_file_path = 'draw.json' # Run sleepy_ask chat.ask
-(config=config, questions=question_list, output_file_path=output_file_path,
-verbose=True) ```
- [https://user-images.githubusercontent.com/84760072/227817860-f4aef84b-9992-
-                          4ddd-a99d-019566cce0c5.png]
-### Parameters `sleepyask.openai.ask` has the following parameters: ####
-Required - `configs` :: **(required)** - should be a list of dicts containing
-`organization` (your OpenAI organization ID), `api key` (your OpenAI api key)
-and the `count` (the number of instances to spin up for asking questions) -
-`questions` :: **(required)** - should be a list of strings containing
-questions you would like to ask ChatGPT. - `output_file_path` :: **(required)**
-- should be a valid file path where you would like your responses to be stored.
-sleepyask will create this file for you. If you create this file yourself,
-there might be some problems. #### Optional - `verbose` :: **(optional)** - a
-boolean which specifies whether or not sleepyask should print its progress to
-the console. It is `False` by default - `model` :: **(optional)** - to specify
-which ChatGPT model to use. It is `"gpt-3.5-turbo"` by default - `system_text`
-:: **(optional)** - to specify system text. It is ` - `temperature` :: **
-(optional)** - to specify how deterministic ChatGPT's responses are. Ranges
-from `0-2` where higher numbers represent increased randomness. It is `1` by
-default. - `max_tokens` :: **(optional)** - to specify the maximum number of
-tokens in ChatGPT's response. This is `2048` by default ## ð¬ Get involved -
-ð **Found a bug or interested in adding a feature?** - Create an [issue]
-[issue] - ð¤ **Want to help?** - Create a pull-request! [issue]: https://
-github.com/hwelsters/sleepyask/issues
+from dotenv import load_dotenv from sleepyask.chat import Sleepyask load_dotenv
+() # take environment variables from .env. TIMEOUT = 10000 RETRY_TIME = 5
+RATE_LIMIT = 5 API_KEY = os.getenv('OPENAI_API_KEY') # Index should be unique
+as it will be used to avoid repeat questions QUESTION_LIST = [ {'index': 1,
+'text': 'What is 1 + 1?'}, {'index': 2, 'text': 'What is 1 + 2?'}, {'index': 3,
+'text': 'What is 1 + 3?'} ] OUT_PATH = 'output.jsonl' CONFIGS = { "model":
+"gpt-3.5-turbo", "n": 10, "temperature": 0.7} sleepyask = Sleepyask
+(configs=CONFIGS, rate_limit=RATE_LIMIT, api_key=API_KEY, timeout=TIMEOUT,
+verbose=True, retry_time=RETRY_TIME) sleepyask.start(question_list=QUESTION,
+out_path=OUT_PATH) ``` ## ð¬ Get involved - ð **Found a bug or interested
+in adding a feature?** - Create an [issue][issue] - ð¤ **Want to help?** -
+Create a pull-request! [issue]: https://github.com/hwelsters/sleepyask/issues
```

### Comparing `sleepyask-7.0.0/pyproject.toml` & `sleepyask-7.1.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sleepyask"
-version = "7.0.0"
+version = "7.1.0"
 authors = [
   { name="hwelsters", email="redacted@redacted.redacted" },
 ]
 description = "A small tool for automating collecting data from ChatGPT"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = []
 dependencies = [
   'openai-async>=0.0.3'
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/hwelsters/sleepyask"
-"Bug Tracker" = "https://github.com/hwelsters/sleepyask/issues"
+"Bug Tracker" = "https://github.com/hwelsters/sleepyask/issues"
```

### Comparing `sleepyask-7.0.0/src/sleepyask/chat.py` & `sleepyask-7.1.0/src/sleepyask/chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     """
 
     def __init__(self, 
                  configs : dict ={}, 
                  rate_limit: int = 5, 
                  api_key: str = "", 
                  timeout: int = 100, 
-                 out_path : str = "", 
                  verbose: bool = False, 
                  retry_time: int = 60,
                  system_text: str = ""
     ):
         """
         `configs` a dict containing parameters which will be part of the payload such as model, temperature, etc
         `rate_limit` the maximum number of questions you would like to ask a minute.
@@ -30,15 +29,14 @@
         `timeout` the amount of time to wait before timing out
         `out_path` the path in which the responses will be outputted
         """
         self.configs = configs
         self.rate_limit = rate_limit
         self.api_key = api_key
         self.timeout = timeout
-        self.out_path = out_path
         self.verbose = verbose
         self.retry_time = retry_time
         self.system_text = system_text
 
     def get_asked_ids(self):
         asked_ids = set()
 
@@ -54,31 +52,31 @@
                     if "question_id" in row: 
                         asked_ids.add(str(row["question_id"]))
                         self.succeed += 1
                 except: pass
             outfile.close()
         return asked_ids
 
-    def start(self, question_list):
+    def start(self, question_list, out_path):
         """
         `question_list` list of questions to ask ChatGPT
         """
+        self.out_path = out_path
+        
         asyncio.run(self.__start(question_list))
 
     async def __start(self, question_list):
         self.succeed = 0
         self.file_lock = asyncio.Lock()
         self.question_queue = queue.Queue()
 
         asked_ids = self.get_asked_ids()
 
-        # print("HERE")
         for question in question_list: 
             if str(question["id"]) in asked_ids: continue
-            print(question)
             self.question_queue.put(question)
 
         while self.succeed < len(question_list):
             tasks = []
             for _ in range(self.rate_limit):
                 try: tasks.append(self.async_ask(self.question_queue.get(False)))
                 except: pass
@@ -111,8 +109,8 @@
             if response.status_code != 200: 
                 if self.verbose: print(f"[sleepyask] INFO | ID {question_index} | {response.status_code}")
                 raise ValueError("Should be 200")
 
             await self.log({"question_id": question_index,  **json.loads(response.text), "question": question_text, **self.configs})
         except: 
             if self.verbose: print(f"[sleepyask] INFO | ID {question_index} | ERROR")
-            self.question_queue.put(question_text)
+            self.question_queue.put(question)
```

### Comparing `sleepyask-7.0.0/src/sleepyask.egg-info/PKG-INFO` & `sleepyask-7.1.0/src/sleepyask.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleepyask
-Version: 7.0.0
+Version: 7.1.0
 Summary: A small tool for automating collecting data from ChatGPT
 Author-email: hwelsters <redacted@redacted.redacted>
 Project-URL: Homepage, https://github.com/hwelsters/sleepyask
 Project-URL: Bug Tracker, https://github.com/hwelsters/sleepyask/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -65,58 +65,42 @@
 - `count` - This specifies the number of workers to create for asking questions. You can have multiple workers asking questions in parallel.  
 	
 ### Sample code
 It is recommended that you do not store your user credentials directly in your code. Instead, use something like `python-dotenv` to store your credentials in another file.
 ```python
 import os
 from dotenv import load_dotenv
-from sleepyask.openai import chat
+
+from sleepyask.chat import Sleepyask
 
 load_dotenv()  # take environment variables from .env.
 
-# Your ChatGPT authentication configs
-config = {
-	"organization": os.getenv('OPENAI_ORGANIZATION_1'),
-	"api_key": os.getenv('OPENAI_API_KEY_1'),
-	"count": 1
-}
-
-# List of authentication configs
-configs = [config]
-
-# List of questions you would like to ask ChatGPT
-question_list = ['What is 1 + 1?', 'What is 1 + 2?', 'What is 1 + 3?']
-
-# The filename in which you would like your responses to be stored.
-# sleepyask will create this file for you. If you create it yourself, there might be some problems.
-output_file_path = 'draw.json'  
-
-# Run sleepy_ask
-chat.ask(config=config,
-           questions=question_list,
-           output_file_path=output_file_path,
-           verbose=True)
-```
+TIMEOUT = 10000
+RETRY_TIME = 5
+RATE_LIMIT = 5
+API_KEY = os.getenv('OPENAI_API_KEY')
+
+# Index should be unique as it will be used to avoid repeat questions
+QUESTION_LIST = [
+	{'index': 1, 'text': 'What is 1 + 1?'},
+	{'index': 2, 'text': 'What is 1 + 2?'},
+	{'index': 3, 'text': 'What is 1 + 3?'}
+]
+OUT_PATH = 'output.jsonl'
+
+
+CONFIGS = { "model": "gpt-3.5-turbo", "n": 10, "temperature": 0.7}
+sleepyask = Sleepyask(configs=CONFIGS, 
+                      rate_limit=RATE_LIMIT,
+                      api_key=API_KEY, 
+                      timeout=TIMEOUT, 
+                      verbose=True,
+                      retry_time=RETRY_TIME)
 
-<p align="center">
-  <img src="https://user-images.githubusercontent.com/84760072/227817860-f4aef84b-9992-4ddd-a99d-019566cce0c5.png" width="900" />
-</p>
-
-### Parameters
-`sleepyask.openai.ask` has the following parameters:
-#### Required
-- `configs` :: **(required)** - should be a list of dicts containing `organization` (your OpenAI organization ID), `api key` (your OpenAI api key) and the `count` (the number of instances to spin up for asking questions)
-- `questions` :: **(required)** - should be a list of strings containing questions you would like to ask ChatGPT.
-- `output_file_path` :: **(required)** - should be a valid file path where you would like your responses to be stored. sleepyask will create this file for you. If you create this file yourself, there might be some problems.
-
-#### Optional
-- `verbose` :: **(optional)** - a boolean which specifies whether or not sleepyask should print its progress to the console. It is `False` by default
-- `model` :: **(optional)** - to specify which ChatGPT model to use. It is `"gpt-3.5-turbo"` by default
-- `system_text` :: **(optional)** - to specify system text. It is `
-- `temperature` :: **(optional)** - to specify how deterministic ChatGPT's responses are. Ranges from `0-2` where higher numbers represent increased randomness. It is `1` by default.
-- `max_tokens` :: **(optional)** - to specify the maximum number of tokens in ChatGPT's response. This is `2048` by default
+sleepyask.start(question_list=QUESTION, out_path=OUT_PATH)
+```
 
 ## 💬 Get involved
 - 🐛 **Found a bug or interested in adding a feature?** - Create an [issue][issue]  
 - 🤗 **Want to help?** - Create a pull-request!  
 
 [issue]: https://github.com/hwelsters/sleepyask/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sleepyask Version: 7.0.0 Summary: A small tool for
+Metadata-Version: 2.1 Name: sleepyask Version: 7.1.0 Summary: A small tool for
 automating collecting data from ChatGPT Author-email: hwelsters
 redacted.redacted> Project-URL: Homepage, https://github.com/hwelsters/
 sleepyask Project-URL: Bug Tracker, https://github.com/hwelsters/sleepyask/
 issues Requires-Python: >=3.7 Description-Content-Type: text/markdown License-
 File: LICENSE
  [https://user-images.githubusercontent.com/84760072/227817729-098182f3-6916-
                           48d8-b17a-4e4126ddd245.png]
@@ -25,40 +25,19 @@
 Key. To get it: ```bash > Go to https://platform.openai.com/account/api-keys >
 Login (if it is required) > Click on your profile picture on the top-right >
 View API Keys > Create new secret key. ``` - `count` - This specifies the
 number of workers to create for asking questions. You can have multiple workers
 asking questions in parallel. ### Sample code It is recommended that you do not
 store your user credentials directly in your code. Instead, use something like
 `python-dotenv` to store your credentials in another file. ```python import os
-from dotenv import load_dotenv from sleepyask.openai import chat load_dotenv()
-# take environment variables from .env. # Your ChatGPT authentication configs
-config = { "organization": os.getenv('OPENAI_ORGANIZATION_1'), "api_key":
-os.getenv('OPENAI_API_KEY_1'), "count": 1 } # List of authentication configs
-configs = [config] # List of questions you would like to ask ChatGPT
-question_list = ['What is 1 + 1?', 'What is 1 + 2?', 'What is 1 + 3?'] # The
-filename in which you would like your responses to be stored. # sleepyask will
-create this file for you. If you create it yourself, there might be some
-problems. output_file_path = 'draw.json' # Run sleepy_ask chat.ask
-(config=config, questions=question_list, output_file_path=output_file_path,
-verbose=True) ```
- [https://user-images.githubusercontent.com/84760072/227817860-f4aef84b-9992-
-                          4ddd-a99d-019566cce0c5.png]
-### Parameters `sleepyask.openai.ask` has the following parameters: ####
-Required - `configs` :: **(required)** - should be a list of dicts containing
-`organization` (your OpenAI organization ID), `api key` (your OpenAI api key)
-and the `count` (the number of instances to spin up for asking questions) -
-`questions` :: **(required)** - should be a list of strings containing
-questions you would like to ask ChatGPT. - `output_file_path` :: **(required)**
-- should be a valid file path where you would like your responses to be stored.
-sleepyask will create this file for you. If you create this file yourself,
-there might be some problems. #### Optional - `verbose` :: **(optional)** - a
-boolean which specifies whether or not sleepyask should print its progress to
-the console. It is `False` by default - `model` :: **(optional)** - to specify
-which ChatGPT model to use. It is `"gpt-3.5-turbo"` by default - `system_text`
-:: **(optional)** - to specify system text. It is ` - `temperature` :: **
-(optional)** - to specify how deterministic ChatGPT's responses are. Ranges
-from `0-2` where higher numbers represent increased randomness. It is `1` by
-default. - `max_tokens` :: **(optional)** - to specify the maximum number of
-tokens in ChatGPT's response. This is `2048` by default ## ð¬ Get involved -
-ð **Found a bug or interested in adding a feature?** - Create an [issue]
-[issue] - ð¤ **Want to help?** - Create a pull-request! [issue]: https://
-github.com/hwelsters/sleepyask/issues
+from dotenv import load_dotenv from sleepyask.chat import Sleepyask load_dotenv
+() # take environment variables from .env. TIMEOUT = 10000 RETRY_TIME = 5
+RATE_LIMIT = 5 API_KEY = os.getenv('OPENAI_API_KEY') # Index should be unique
+as it will be used to avoid repeat questions QUESTION_LIST = [ {'index': 1,
+'text': 'What is 1 + 1?'}, {'index': 2, 'text': 'What is 1 + 2?'}, {'index': 3,
+'text': 'What is 1 + 3?'} ] OUT_PATH = 'output.jsonl' CONFIGS = { "model":
+"gpt-3.5-turbo", "n": 10, "temperature": 0.7} sleepyask = Sleepyask
+(configs=CONFIGS, rate_limit=RATE_LIMIT, api_key=API_KEY, timeout=TIMEOUT,
+verbose=True, retry_time=RETRY_TIME) sleepyask.start(question_list=QUESTION,
+out_path=OUT_PATH) ``` ## ð¬ Get involved - ð **Found a bug or interested
+in adding a feature?** - Create an [issue][issue] - ð¤ **Want to help?** -
+Create a pull-request! [issue]: https://github.com/hwelsters/sleepyask/issues
```

