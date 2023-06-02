# Comparing `tmp/corby-0.1.3.tar.gz` & `tmp/corby-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corby-0.1.3.tar", last modified: Fri Jun  2 09:05:10 2023, max compression
+gzip compressed data, was "corby-0.1.4.tar", last modified: Fri Jun  2 13:09:18 2023, max compression
```

## Comparing `corby-0.1.3.tar` & `corby-0.1.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:05:10.429923 corby-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-06-02 09:04:56.000000 corby-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-02 09:05:10.429923 corby-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-02 09:04:56.000000 corby-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:05:10.425923 corby-0.1.3/corby/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-02 09:04:56.000000 corby-0.1.3/corby/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-02 09:04:56.000000 corby-0.1.3/corby/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:05:10.425923 corby-0.1.3/corby/generator/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-02 09:04:56.000000 corby-0.1.3/corby/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-06-02 09:04:56.000000 corby-0.1.3/corby/generator/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:05:10.429923 corby-0.1.3/corby/generator/chatbot/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-02 09:04:56.000000 corby-0.1.3/corby/generator/chatbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-02 09:04:56.000000 corby-0.1.3/corby/generator/chatbot/base_chatbot.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-02 09:04:56.000000 corby-0.1.3/corby/generator/chatbot/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-02 09:04:56.000000 corby-0.1.3/corby/generator/chatbot/index.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-02 09:04:56.000000 corby-0.1.3/corby/generator/chatbot/telegram.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-02 09:04:56.000000 corby-0.1.3/corby/generator/chatbot/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:05:10.429923 corby-0.1.3/corby/generator/notebook/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-02 09:04:56.000000 corby-0.1.3/corby/generator/notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-02 09:04:56.000000 corby-0.1.3/corby/generator/notebook/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-02 09:04:56.000000 corby-0.1.3/corby/index.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:05:10.425923 corby-0.1.3/corby.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-02 09:05:10.000000 corby-0.1.3/corby.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-02 09:05:10.000000 corby-0.1.3/corby.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 09:05:10.000000 corby-0.1.3/corby.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-02 09:05:10.000000 corby-0.1.3/corby.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-02 09:05:10.000000 corby-0.1.3/corby.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-02 09:05:10.000000 corby-0.1.3/corby.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 09:05:10.429923 corby-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-02 09:04:56.000000 corby-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:09:18.530074 corby-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-06-02 13:09:04.000000 corby-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-02 13:09:18.530074 corby-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-02 13:09:04.000000 corby-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:09:18.530074 corby-0.1.4/corby/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-02 13:09:04.000000 corby-0.1.4/corby/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-02 13:09:04.000000 corby-0.1.4/corby/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:09:18.530074 corby-0.1.4/corby/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-02 13:09:04.000000 corby-0.1.4/corby/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-06-02 13:09:04.000000 corby-0.1.4/corby/generator/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:09:18.530074 corby-0.1.4/corby/generator/chatbot/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-02 13:09:04.000000 corby-0.1.4/corby/generator/chatbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-02 13:09:04.000000 corby-0.1.4/corby/generator/chatbot/base_chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-02 13:09:04.000000 corby-0.1.4/corby/generator/chatbot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-02 13:09:04.000000 corby-0.1.4/corby/generator/chatbot/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-02 13:09:04.000000 corby-0.1.4/corby/generator/chatbot/telegram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-02 13:09:04.000000 corby-0.1.4/corby/generator/chatbot/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:09:18.530074 corby-0.1.4/corby/generator/notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-02 13:09:04.000000 corby-0.1.4/corby/generator/notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-02 13:09:04.000000 corby-0.1.4/corby/generator/notebook/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-02 13:09:04.000000 corby-0.1.4/corby/index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:09:18.530074 corby-0.1.4/corby.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-02 13:09:18.000000 corby-0.1.4/corby.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-02 13:09:18.000000 corby-0.1.4/corby.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 13:09:18.000000 corby-0.1.4/corby.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-02 13:09:18.000000 corby-0.1.4/corby.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-02 13:09:18.000000 corby-0.1.4/corby.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-02 13:09:18.000000 corby-0.1.4/corby.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 13:09:18.530074 corby-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-02 13:09:04.000000 corby-0.1.4/setup.py
```

### Comparing `corby-0.1.3/LICENSE` & `corby-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `corby-0.1.3/PKG-INFO` & `corby-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corby
-Version: 0.1.3
+Version: 0.1.4
 Summary: ⚡ Create your LLMs applications from zero to deploy in minutes ⚡
 Author: Jose Hervás Díaz
 Author-email: jhervasdiaz@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `corby-0.1.3/README.md` & `corby-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `corby-0.1.3/corby/generator/base.py` & `corby-0.1.4/corby/generator/base.py`

 * *Files identical despite different names*

### Comparing `corby-0.1.3/corby/generator/chatbot/base_chatbot.py` & `corby-0.1.4/corby/generator/chatbot/base_chatbot.py`

 * *Files identical despite different names*

### Comparing `corby-0.1.3/corby/generator/chatbot/index.py` & `corby-0.1.4/corby/generator/chatbot/index.py`

 * *Files identical despite different names*

### Comparing `corby-0.1.3/corby/generator/chatbot/telegram.py` & `corby-0.1.4/corby/generator/chatbot/telegram.py`

 * *Files identical despite different names*

### Comparing `corby-0.1.3/corby/generator/notebook/index.py` & `corby-0.1.4/corby/generator/notebook/index.py`

 * *Files identical despite different names*

### Comparing `corby-0.1.3/corby/index.py` & `corby-0.1.4/corby/index.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """Main CLI entrypoint for Corby"""
 
 import argparse
 from string import Template
 from .generator.chatbot.index import create_chatbot
 from .generator.notebook.index import create_notebook
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 
 # We'll include more features in the future
 available_actions = ['new']
 
 available_entities = ['chatbot', 'notebook']
 
 parser = argparse.ArgumentParser(
```

### Comparing `corby-0.1.3/corby.egg-info/PKG-INFO` & `corby-0.1.4/corby.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corby
-Version: 0.1.3
+Version: 0.1.4
 Summary: ⚡ Create your LLMs applications from zero to deploy in minutes ⚡
 Author: Jose Hervás Díaz
 Author-email: jhervasdiaz@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `corby-0.1.3/corby.egg-info/SOURCES.txt` & `corby-0.1.4/corby.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `corby-0.1.3/setup.py` & `corby-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 '''Pypi setup file for corby'''
 
 from setuptools import setup, find_packages
 
 setup(
     name="corby",
-    version="0.1.3",
+    version="0.1.4",
     description="⚡ Create your LLMs applications from zero to deploy in minutes ⚡",
     # pylint: disable=consider-using-with
     long_description=open("README.md", encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     author="Jose Hervás Díaz",
     author_email='jhervasdiaz@gmail.com',
     license='MIT',
```

