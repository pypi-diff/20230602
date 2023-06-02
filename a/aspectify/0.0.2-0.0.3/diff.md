# Comparing `tmp/aspectify-0.0.2.tar.gz` & `tmp/aspectify-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aspectify-0.0.2.tar", last modified: Fri Jun  2 06:38:25 2023, max compression
+gzip compressed data, was "aspectify-0.0.3.tar", last modified: Fri Jun  2 07:29:44 2023, max compression
```

## Comparing `aspectify-0.0.2.tar` & `aspectify-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-x---   0 ruescog   (1008) ruescog   (1011)        0 2023-06-02 06:38:25.096353 aspectify-0.0.2/
--rw-r-----   0 ruescog   (1008) ruescog   (1011)     7048 2023-05-29 07:08:03.000000 aspectify-0.0.2/LICENSE
--rw-rw-r--   0 ruescog   (1008) ruescog   (1011)      111 2023-04-27 10:12:58.000000 aspectify-0.0.2/MANIFEST.in
--rw-r-----   0 ruescog   (1008) ruescog   (1011)     6787 2023-06-02 06:38:25.096353 aspectify-0.0.2/PKG-INFO
--rw-r-----   0 ruescog   (1008) ruescog   (1011)     4758 2023-06-01 07:25:52.000000 aspectify-0.0.2/README.md
-drwxr-x---   0 ruescog   (1008) ruescog   (1011)        0 2023-06-02 06:38:25.092353 aspectify-0.0.2/aspectify/
--rw-r--r--   0 ruescog   (1008) ruescog   (1011)       22 2023-06-02 06:37:48.000000 aspectify-0.0.2/aspectify/__init__.py
--rw-r-----   0 ruescog   (1008) ruescog   (1011)     1537 2023-06-02 06:37:48.000000 aspectify-0.0.2/aspectify/_modidx.py
--rw-r--r--   0 ruescog   (1008) ruescog   (1011)     6490 2023-06-02 06:37:48.000000 aspectify-0.0.2/aspectify/aop.py
--rw-r-----   0 ruescog   (1008) ruescog   (1011)      142 2023-05-29 07:42:30.000000 aspectify-0.0.2/aspectify/core.py
-drwxr-x---   0 ruescog   (1008) ruescog   (1011)        0 2023-06-02 06:38:25.096353 aspectify-0.0.2/aspectify.egg-info/
--rw-r-----   0 ruescog   (1008) ruescog   (1011)     6787 2023-06-02 06:38:25.000000 aspectify-0.0.2/aspectify.egg-info/PKG-INFO
--rw-r-----   0 ruescog   (1008) ruescog   (1011)      361 2023-06-02 06:38:25.000000 aspectify-0.0.2/aspectify.egg-info/SOURCES.txt
--rw-r-----   0 ruescog   (1008) ruescog   (1011)        1 2023-06-02 06:38:25.000000 aspectify-0.0.2/aspectify.egg-info/dependency_links.txt
--rw-r-----   0 ruescog   (1008) ruescog   (1011)       61 2023-06-02 06:38:25.000000 aspectify-0.0.2/aspectify.egg-info/entry_points.txt
--rw-r-----   0 ruescog   (1008) ruescog   (1011)        1 2023-05-29 07:48:24.000000 aspectify-0.0.2/aspectify.egg-info/not-zip-safe
--rw-r-----   0 ruescog   (1008) ruescog   (1011)        7 2023-06-02 06:38:25.000000 aspectify-0.0.2/aspectify.egg-info/requires.txt
--rw-r-----   0 ruescog   (1008) ruescog   (1011)       10 2023-06-02 06:38:25.000000 aspectify-0.0.2/aspectify.egg-info/top_level.txt
--rw-r-----   0 ruescog   (1008) ruescog   (1011)      802 2023-06-02 06:32:55.000000 aspectify-0.0.2/settings.ini
--rw-r-----   0 ruescog   (1008) ruescog   (1011)       38 2023-06-02 06:38:25.096353 aspectify-0.0.2/setup.cfg
--rw-rw-r--   0 ruescog   (1008) ruescog   (1011)     2596 2023-04-27 10:12:58.000000 aspectify-0.0.2/setup.py
+drwxr-x---   0 ruescog   (1008) ruescog   (1011)        0 2023-06-02 07:29:44.120417 aspectify-0.0.3/
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)     7048 2023-05-29 07:08:03.000000 aspectify-0.0.3/LICENSE
+-rw-rw-r--   0 ruescog   (1008) ruescog   (1011)      111 2023-04-27 10:12:58.000000 aspectify-0.0.3/MANIFEST.in
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)     6872 2023-06-02 07:29:44.120417 aspectify-0.0.3/PKG-INFO
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)     4835 2023-06-02 07:27:18.000000 aspectify-0.0.3/README.md
+drwxr-x---   0 ruescog   (1008) ruescog   (1011)        0 2023-06-02 07:29:44.120417 aspectify-0.0.3/aspectify/
+-rw-r--r--   0 ruescog   (1008) ruescog   (1011)       22 2023-06-02 07:29:39.000000 aspectify-0.0.3/aspectify/__init__.py
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)     1537 2023-06-02 07:29:39.000000 aspectify-0.0.3/aspectify/_modidx.py
+-rw-r--r--   0 ruescog   (1008) ruescog   (1011)     6488 2023-06-02 07:29:39.000000 aspectify-0.0.3/aspectify/aop.py
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)      142 2023-05-29 07:42:30.000000 aspectify-0.0.3/aspectify/core.py
+drwxr-x---   0 ruescog   (1008) ruescog   (1011)        0 2023-06-02 07:29:44.120417 aspectify-0.0.3/aspectify.egg-info/
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)     6872 2023-06-02 07:29:44.000000 aspectify-0.0.3/aspectify.egg-info/PKG-INFO
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)      361 2023-06-02 07:29:44.000000 aspectify-0.0.3/aspectify.egg-info/SOURCES.txt
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)        1 2023-06-02 07:29:44.000000 aspectify-0.0.3/aspectify.egg-info/dependency_links.txt
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)       61 2023-06-02 07:29:44.000000 aspectify-0.0.3/aspectify.egg-info/entry_points.txt
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)        1 2023-05-29 07:48:24.000000 aspectify-0.0.3/aspectify.egg-info/not-zip-safe
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)        7 2023-06-02 07:29:44.000000 aspectify-0.0.3/aspectify.egg-info/requires.txt
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)       10 2023-06-02 07:29:44.000000 aspectify-0.0.3/aspectify.egg-info/top_level.txt
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)      802 2023-06-02 07:29:21.000000 aspectify-0.0.3/settings.ini
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)       38 2023-06-02 07:29:44.120417 aspectify-0.0.3/setup.cfg
+-rw-rw-r--   0 ruescog   (1008) ruescog   (1011)     2596 2023-04-27 10:12:58.000000 aspectify-0.0.3/setup.py
```

### Comparing `aspectify-0.0.2/LICENSE` & `aspectify-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aspectify-0.0.2/PKG-INFO` & `aspectify-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aspectify
-Version: 0.0.2
+Version: 0.0.3
 Summary: Apply Aspect Oriented Programming to your Python code
 Home-page: https://github.com/ruescog/aspectify
 Author: ruescog
 Author-email: ruescog@unirioja.es
 License: Apache Software License 2.0
 Description: aspectify
         ================
@@ -135,15 +135,15 @@
         
         First of all, we need to define a method to gather all the classes
         loaded in the `aspects.py` file, in order to modify their behaviour
         dynamically. This method will be always be the same:
         
         ``` python
         def get_classes():
-            return [element for element in list(globals().items()) if is_detectable(*element)]
+            return [element for element in list(globals().items())]
         ```
         
         At this point, we can define our first
         [`Aspect`](https://ruescog.github.io/aspectify/aop.html#aspect). We will
         call it “add-message”, and it will show a message `before` the addition
         is done.
         
@@ -155,15 +155,16 @@
         Finally, we will create a `PointCut` that will define which methods will
         show this message. We will use the regular expression `.*add`.
         
         ``` python
         add_message_aspect.create_pointcut(get_classes(), ".*add")
         ```
         
-            AttributeError: 'ZMQExitAutocall' object has no attribute '__name__'
+            Captured method: __main__.Calculator.add
+            [WARNING]: If executed in a notebook, the cell is shown being executed, but this message proves that the execution is finished.
         
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `aspectify-0.0.2/README.md` & `aspectify-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 
 First of all, we need to define a method to gather all the classes
 loaded in the `aspects.py` file, in order to modify their behaviour
 dynamically. This method will be always be the same:
 
 ``` python
 def get_classes():
-    return [element for element in list(globals().items()) if is_detectable(*element)]
+    return [element for element in list(globals().items())]
 ```
 
 At this point, we can define our first
 [`Aspect`](https://ruescog.github.io/aspectify/aop.html#aspect). We will
 call it “add-message”, and it will show a message `before` the addition
 is done.
 
@@ -147,8 +147,9 @@
 Finally, we will create a `PointCut` that will define which methods will
 show this message. We will use the regular expression `.*add`.
 
 ``` python
 add_message_aspect.create_pointcut(get_classes(), ".*add")
 ```
 
-    AttributeError: 'ZMQExitAutocall' object has no attribute '__name__'
+    Captured method: __main__.Calculator.add
+    [WARNING]: If executed in a notebook, the cell is shown being executed, but this message proves that the execution is finished.
```

### Comparing `aspectify-0.0.2/aspectify/_modidx.py` & `aspectify-0.0.3/aspectify/_modidx.py`

 * *Files identical despite different names*

### Comparing `aspectify-0.0.2/aspectify/aop.py` & `aspectify-0.0.3/aspectify/aop.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             try:
                 if moment == "before": todo(*todo_args, **kwargs) # returned value is lost
                 result = todo(*todo_args, **kwargs) if moment == "around" else method(*args, **kwargs)
                 if moment in ["after_returning", "after"]: todo(*todo_args, **kwargs)
                 return result
 
             except Exception as e:
-                if moment in ["after_throwing", "after"]: todo([e, *todo_args], **kwargs)
+                if moment in ["after_throwing", "after"]: todo(e, *todo_args, **kwargs)
                 raise e
 
         return inner
     return dec
 
 # %% ../nbs/00_aop.ipynb 6
 class Aspect():
```

### Comparing `aspectify-0.0.2/aspectify.egg-info/PKG-INFO` & `aspectify-0.0.3/aspectify.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aspectify
-Version: 0.0.2
+Version: 0.0.3
 Summary: Apply Aspect Oriented Programming to your Python code
 Home-page: https://github.com/ruescog/aspectify
 Author: ruescog
 Author-email: ruescog@unirioja.es
 License: Apache Software License 2.0
 Description: aspectify
         ================
@@ -135,15 +135,15 @@
         
         First of all, we need to define a method to gather all the classes
         loaded in the `aspects.py` file, in order to modify their behaviour
         dynamically. This method will be always be the same:
         
         ``` python
         def get_classes():
-            return [element for element in list(globals().items()) if is_detectable(*element)]
+            return [element for element in list(globals().items())]
         ```
         
         At this point, we can define our first
         [`Aspect`](https://ruescog.github.io/aspectify/aop.html#aspect). We will
         call it “add-message”, and it will show a message `before` the addition
         is done.
         
@@ -155,15 +155,16 @@
         Finally, we will create a `PointCut` that will define which methods will
         show this message. We will use the regular expression `.*add`.
         
         ``` python
         add_message_aspect.create_pointcut(get_classes(), ".*add")
         ```
         
-            AttributeError: 'ZMQExitAutocall' object has no attribute '__name__'
+            Captured method: __main__.Calculator.add
+            [WARNING]: If executed in a notebook, the cell is shown being executed, but this message proves that the execution is finished.
         
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `aspectify-0.0.2/settings.ini` & `aspectify-0.0.3/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = aspectify
 lib_name = aspectify
-version = 0.0.2
+version = 0.0.3
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = aspectify
 nbs_path = nbs
 recursive = True
```

### Comparing `aspectify-0.0.2/setup.py` & `aspectify-0.0.3/setup.py`

 * *Files identical despite different names*

