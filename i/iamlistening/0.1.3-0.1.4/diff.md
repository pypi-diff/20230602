# Comparing `tmp/iamlistening-0.1.3.tar.gz` & `tmp/iamlistening-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamlistening-0.1.3.tar", max compression
+gzip compressed data, was "iamlistening-0.1.4.tar", max compression
```

## Comparing `iamlistening-0.1.3.tar` & `iamlistening-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-06-02 16:57:43.343311 iamlistening-0.1.3/LICENSE
--rw-r--r--   0        0        0     1507 2023-06-02 16:57:43.343311 iamlistening-0.1.3/README.md
--rw-r--r--   0        0        0       99 2023-06-02 16:57:44.079436 iamlistening-0.1.3/iamlistening/__init__.py
--rw-r--r--   0        0        0      630 2023-06-02 16:57:43.343311 iamlistening-0.1.3/iamlistening/config.py
--rw-r--r--   0        0        0      229 2023-06-02 16:57:43.343311 iamlistening-0.1.3/iamlistening/default_settings.toml
--rw-r--r--   0        0        0     7319 2023-06-02 16:57:43.343311 iamlistening-0.1.3/iamlistening/main.py
--rw-r--r--   0        0        0     1692 2023-06-02 16:57:44.079436 iamlistening-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2410 1970-01-01 00:00:00.000000 iamlistening-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-02 20:19:16.824405 iamlistening-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1504 2023-06-02 20:19:16.824405 iamlistening-0.1.4/README.md
+-rw-r--r--   0        0        0       99 2023-06-02 20:19:17.564414 iamlistening-0.1.4/iamlistening/__init__.py
+-rw-r--r--   0        0        0      630 2023-06-02 20:19:16.824405 iamlistening-0.1.4/iamlistening/config.py
+-rw-r--r--   0        0        0      229 2023-06-02 20:19:16.824405 iamlistening-0.1.4/iamlistening/default_settings.toml
+-rw-r--r--   0        0        0     4292 2023-06-02 20:19:16.824405 iamlistening-0.1.4/iamlistening/main.py
+-rw-r--r--   0        0        0     1692 2023-06-02 20:19:17.564414 iamlistening-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2407 1970-01-01 00:00:00.000000 iamlistening-0.1.4/PKG-INFO
```

### Comparing `iamlistening-0.1.3/LICENSE` & `iamlistening-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `iamlistening-0.1.3/README.md` & `iamlistening-0.1.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ## Install
 
 `pip install iamlistening`
 
 ## How to use it
 
 ```
- from iamlisterning import Listerner
- 
- bot = listerner.start()
+  from iamlistening import Listerner as bot
+  bot.start()
+  
 ```
 
 ### Example
 
 [example](https://github.com/mraniki/iamlistening/blob/main/examples/example.py)
 
 ### Real use case
```

### Comparing `iamlistening-0.1.3/iamlistening/config.py` & `iamlistening-0.1.4/iamlistening/config.py`

 * *Files identical despite different names*

### Comparing `iamlistening-0.1.3/pyproject.toml` & `iamlistening-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iamlistening"
-version = "0.1.3"
+version = "0.1.4"
 description = "A python package to interact with messaging platform."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["discord", "telegram", "bot","messaging","matrix"]
 packages = [
     {include = "iamlistening"}
```

### Comparing `iamlistening-0.1.3/PKG-INFO` & `iamlistening-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamlistening
-Version: 0.1.3
+Version: 0.1.4
 Summary: A python package to interact with messaging platform.
 License: MIT
 Keywords: discord,telegram,bot,messaging,matrix
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -35,17 +35,17 @@
 ## Install
 
 `pip install iamlistening`
 
 ## How to use it
 
 ```
- from iamlisterning import Listerner
- 
- bot = listerner.start()
+  from iamlistening import Listerner as bot
+  bot.start()
+  
 ```
 
 ### Example
 
 [example](https://github.com/mraniki/iamlistening/blob/main/examples/example.py)
 
 ### Real use case
```

